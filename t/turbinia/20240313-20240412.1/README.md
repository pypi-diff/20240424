# Comparing `tmp/turbinia-20240313.tar.gz` & `tmp/turbinia-20240412.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "turbinia-20240313.tar", max compression
+gzip compressed data, was "turbinia-20240412.1.tar", max compression
```

## Comparing `turbinia-20240313.tar` & `turbinia-20240412.1.tar`

### file list

```diff
@@ -1,325 +1,263 @@
--rw-r--r--   0        0        0      427 2024-03-13 18:51:24.085477 turbinia-20240313/AUTHORS
--rw-r--r--   0        0        0    11358 2024-03-13 18:51:24.085477 turbinia-20240313/LICENSE
--rw-r--r--   0        0        0     6466 2024-03-13 18:51:24.085477 turbinia-20240313/README.md
--rw-r--r--   0        0        0     1846 2024-03-13 18:51:24.097477 turbinia-20240313/pyproject.toml
--rw-r--r--   0        0        0     1613 2024-03-13 18:51:24.453475 turbinia-20240313/turbinia/__init__.py
--rw-r--r--   0        0        0      626 2024-03-13 18:51:24.453475 turbinia-20240313/turbinia/api/__init__.py
--rw-r--r--   0        0        0     3060 2024-03-13 18:51:24.453475 turbinia-20240313/turbinia/api/api_server.py
--rw-r--r--   0        0        0    18162 2024-03-13 18:51:24.453475 turbinia-20240313/turbinia/api/api_server_test.py
--rw-r--r--   0        0        0      823 2024-03-13 18:51:24.453475 turbinia-20240313/turbinia/api/cli/.turbinia_api_config.json
--rw-r--r--   0        0        0    11358 2024-03-13 18:51:24.453475 turbinia-20240313/turbinia/api/cli/LICENSE
--rw-r--r--   0        0        0     8306 2024-03-13 18:51:24.453475 turbinia-20240313/turbinia/api/cli/README.rst
--rw-r--r--   0        0        0    52542 2024-03-13 18:51:24.453475 turbinia-20240313/turbinia/api/cli/poetry.lock
--rw-r--r--   0        0        0      697 2024-03-13 18:51:24.453475 turbinia-20240313/turbinia/api/cli/pyproject.toml
--rw-r--r--   0        0        0    17381 2024-03-13 18:51:24.457475 turbinia-20240313/turbinia/api/cli/requirements.txt
--rw-r--r--   0        0        0      645 2024-03-13 18:51:24.457475 turbinia-20240313/turbinia/api/cli/turbinia_client/__init__.py
--rw-r--r--   0        0        0      645 2024-03-13 18:51:24.457475 turbinia-20240313/turbinia/api/cli/turbinia_client/core/__init__.py
--rw-r--r--   0        0        0    17824 2024-03-13 18:51:24.457475 turbinia-20240313/turbinia/api/cli/turbinia_client/core/commands.py
--rw-r--r--   0        0        0     2276 2024-03-13 18:51:24.457475 turbinia-20240313/turbinia/api/cli/turbinia_client/core/groups.py
--rw-r--r--   0        0        0      645 2024-03-13 18:51:24.457475 turbinia-20240313/turbinia/api/cli/turbinia_client/factory/__init__.py
--rw-r--r--   0        0        0     5695 2024-03-13 18:51:24.457475 turbinia-20240313/turbinia/api/cli/turbinia_client/factory/factory.py
--rw-r--r--   0        0        0      645 2024-03-13 18:51:24.457475 turbinia-20240313/turbinia/api/cli/turbinia_client/helpers/__init__.py
--rw-r--r--   0        0        0     2628 2024-03-13 18:51:24.457475 turbinia-20240313/turbinia/api/cli/turbinia_client/helpers/auth_helper.py
--rw-r--r--   0        0        0     5031 2024-03-13 18:51:24.457475 turbinia-20240313/turbinia/api/cli/turbinia_client/helpers/click_helper.py
--rw-r--r--   0        0        0    22850 2024-03-13 18:51:24.457475 turbinia-20240313/turbinia/api/cli/turbinia_client/helpers/formatter.py
--rw-r--r--   0        0        0     8285 2024-03-13 18:51:24.457475 turbinia-20240313/turbinia/api/cli/turbinia_client/helpers/formatter_test.py
--rw-r--r--   0        0        0     8967 2024-03-13 18:51:24.457475 turbinia-20240313/turbinia/api/cli/turbinia_client/turbiniacli.py
--rw-r--r--   0        0        0     2768 2024-03-13 18:51:24.457475 turbinia-20240313/turbinia/api/cli/turbinia_client/turbiniacli_test.py
--rw-r--r--   0        0        0     4489 2024-03-13 18:51:24.457475 turbinia-20240313/turbinia/api/cli/turbinia_client/turbiniacli_tool.py
--rw-r--r--   0        0        0     1354 2024-03-13 18:51:24.457475 turbinia-20240313/turbinia/api/client/.github/workflows/python.yml
--rw-r--r--   0        0        0      807 2024-03-13 18:51:24.457475 turbinia-20240313/turbinia/api/client/.gitignore
--rw-r--r--   0        0        0      711 2024-03-13 18:51:24.457475 turbinia-20240313/turbinia/api/client/.gitlab-ci.yml
--rw-r--r--   0        0        0     1039 2024-03-13 18:51:24.457475 turbinia-20240313/turbinia/api/client/.openapi-generator-ignore
--rw-r--r--   0        0        0      431 2024-03-13 18:51:24.457475 turbinia-20240313/turbinia/api/client/.travis.yml
--rw-r--r--   0        0        0    11358 2024-03-13 18:51:24.457475 turbinia-20240313/turbinia/api/client/LICENSE
--rw-r--r--   0        0        0     5834 2024-03-13 18:51:24.457475 turbinia-20240313/turbinia/api/client/README.md
--rw-r--r--   0        0        0     1465 2024-03-13 18:51:24.457475 turbinia-20240313/turbinia/api/client/docs/BaseRequestOptions.md
--rw-r--r--   0        0        0     1325 2024-03-13 18:51:24.457475 turbinia-20240313/turbinia/api/client/docs/BodyUploadEvidenceApiEvidenceUploadPost.md
--rw-r--r--   0        0        0     1328 2024-03-13 18:51:24.457475 turbinia-20240313/turbinia/api/client/docs/CompleteTurbiniaStats.md
--rw-r--r--   0        0        0     1004 2024-03-13 18:51:24.457475 turbinia-20240313/turbinia/api/client/docs/HTTPValidationError.md
--rw-r--r--   0        0        0      841 2024-03-13 18:51:24.457475 turbinia-20240313/turbinia/api/client/docs/LocationInner.md
--rw-r--r--   0        0        0      967 2024-03-13 18:51:24.457475 turbinia-20240313/turbinia/api/client/docs/Request.md
--rw-r--r--   0        0        0     4251 2024-03-13 18:51:24.457475 turbinia-20240313/turbinia/api/client/docs/TurbiniaConfigurationApi.md
--rw-r--r--   0        0        0    15608 2024-03-13 18:51:24.457475 turbinia-20240313/turbinia/api/client/docs/TurbiniaEvidenceApi.md
--rw-r--r--   0        0        0     2116 2024-03-13 18:51:24.457475 turbinia-20240313/turbinia/api/client/docs/TurbiniaJobsApi.md
--rw-r--r--   0        0        0     2241 2024-03-13 18:51:24.457475 turbinia-20240313/turbinia/api/client/docs/TurbiniaLogsApi.md
--rw-r--r--   0        0        0     4720 2024-03-13 18:51:24.457475 turbinia-20240313/turbinia/api/client/docs/TurbiniaRequestResultsApi.md
--rw-r--r--   0        0        0     7397 2024-03-13 18:51:24.457475 turbinia-20240313/turbinia/api/client/docs/TurbiniaRequestsApi.md
--rw-r--r--   0        0        0     8008 2024-03-13 18:51:24.457475 turbinia-20240313/turbinia/api/client/docs/TurbiniaTasksApi.md
--rw-r--r--   0        0        0      976 2024-03-13 18:51:24.457475 turbinia-20240313/turbinia/api/client/docs/ValidationError.md
--rw-r--r--   0        0        0      985 2024-03-13 18:51:24.457475 turbinia-20240313/turbinia/api/client/docs/ValidationErrorLocInner.md
--rw-r--r--   0        0        0     6236 2024-03-13 18:51:24.457475 turbinia-20240313/turbinia/api/client/docs/apis/tags/TurbiniaConfigurationApi.md
--rw-r--r--   0        0        0    31803 2024-03-13 18:51:24.457475 turbinia-20240313/turbinia/api/client/docs/apis/tags/TurbiniaEvidenceApi.md
--rw-r--r--   0        0        0     3118 2024-03-13 18:51:24.457475 turbinia-20240313/turbinia/api/client/docs/apis/tags/TurbiniaJobsApi.md
--rw-r--r--   0        0        0     4908 2024-03-13 18:51:24.457475 turbinia-20240313/turbinia/api/client/docs/apis/tags/TurbiniaLogsApi.md
--rw-r--r--   0        0        0     9632 2024-03-13 18:51:24.457475 turbinia-20240313/turbinia/api/client/docs/apis/tags/TurbiniaRequestResultsApi.md
--rw-r--r--   0        0        0    14336 2024-03-13 18:51:24.457475 turbinia-20240313/turbinia/api/client/docs/apis/tags/TurbiniaRequestsApi.md
--rw-r--r--   0        0        0    16149 2024-03-13 18:51:24.457475 turbinia-20240313/turbinia/api/client/docs/apis/tags/TurbiniaTasksApi.md
--rw-r--r--   0        0        0     2788 2024-03-13 18:51:24.457475 turbinia-20240313/turbinia/api/client/docs/models/BaseRequestOptions.md
--rw-r--r--   0        0        0     3997 2024-03-13 18:51:24.457475 turbinia-20240313/turbinia/api/client/docs/models/CompleteTurbiniaStats.md
--rw-r--r--   0        0        0     1447 2024-03-13 18:51:24.457475 turbinia-20240313/turbinia/api/client/docs/models/HTTPValidationError.md
--rw-r--r--   0        0        0     1483 2024-03-13 18:51:24.457475 turbinia-20240313/turbinia/api/client/docs/models/Request.md
--rw-r--r--   0        0        0     2665 2024-03-13 18:51:24.457475 turbinia-20240313/turbinia/api/client/docs/models/ValidationError.md
--rw-r--r--   0        0        0     1830 2024-03-13 18:51:24.457475 turbinia-20240313/turbinia/api/client/git_push.sh
--rw-r--r--   0        0        0    20827 2024-03-13 18:51:24.457475 turbinia-20240313/turbinia/api/client/poetry.lock
--rw-r--r--   0        0        0      838 2024-03-13 18:51:24.457475 turbinia-20240313/turbinia/api/client/pyproject.toml
--rw-r--r--   0        0        0      113 2024-03-13 18:51:24.457475 turbinia-20240313/turbinia/api/client/requirements.txt
--rw-r--r--   0        0        0       56 2024-03-13 18:51:24.457475 turbinia-20240313/turbinia/api/client/test-requirements.txt
--rw-r--r--   0        0        0      152 2024-03-13 18:51:24.457475 turbinia-20240313/turbinia/api/client/tox.ini
--rw-r--r--   0        0        0     1888 2024-03-13 18:51:24.457475 turbinia-20240313/turbinia/api/client/turbinia_api_lib/__init__.py
--rw-r--r--   0        0        0      574 2024-03-13 18:51:24.457475 turbinia-20240313/turbinia/api/client/turbinia_api_lib/api/__init__.py
--rw-r--r--   0        0        0    11962 2024-03-13 18:51:24.457475 turbinia-20240313/turbinia/api/client/turbinia_api_lib/api/turbinia_configuration_api.py
--rw-r--r--   0        0        0    41146 2024-03-13 18:51:24.457475 turbinia-20240313/turbinia/api/client/turbinia_api_lib/api/turbinia_evidence_api.py
--rw-r--r--   0        0        0     6449 2024-03-13 18:51:24.457475 turbinia-20240313/turbinia/api/client/turbinia_api_lib/api/turbinia_jobs_api.py
--rw-r--r--   0        0        0     6741 2024-03-13 18:51:24.457475 turbinia-20240313/turbinia/api/client/turbinia_api_lib/api/turbinia_logs_api.py
--rw-r--r--   0        0        0    12850 2024-03-13 18:51:24.457475 turbinia-20240313/turbinia/api/client/turbinia_api_lib/api/turbinia_request_results_api.py
--rw-r--r--   0        0        0    19936 2024-03-13 18:51:24.457475 turbinia-20240313/turbinia/api/client/turbinia_api_lib/api/turbinia_requests_api.py
--rw-r--r--   0        0        0    21265 2024-03-13 18:51:24.457475 turbinia-20240313/turbinia/api/client/turbinia_api_lib/api/turbinia_tasks_api.py
--rw-r--r--   0        0        0    29543 2024-03-13 18:51:24.457475 turbinia-20240313/turbinia/api/client/turbinia_api_lib/api_client.py
--rw-r--r--   0        0        0      852 2024-03-13 18:51:24.457475 turbinia-20240313/turbinia/api/client/turbinia_api_lib/api_response.py
--rw-r--r--   0        0        0      214 2024-03-13 18:51:24.457475 turbinia-20240313/turbinia/api/client/turbinia_api_lib/apis/__init__.py
--rw-r--r--   0        0        0     3713 2024-03-13 18:51:24.457475 turbinia-20240313/turbinia/api/client/turbinia_api_lib/apis/path_to_api.py
--rw-r--r--   0        0        0      243 2024-03-13 18:51:24.457475 turbinia-20240313/turbinia/api/client/turbinia_api_lib/apis/paths/__init__.py
--rw-r--r--   0        0        0      107 2024-03-13 18:51:24.457475 turbinia-20240313/turbinia/api/client/turbinia_api_lib/apis/paths/api_config_.py
--rw-r--r--   0        0        0      136 2024-03-13 18:51:24.457475 turbinia-20240313/turbinia/api/client/turbinia_api_lib/apis/paths/api_config_request_options.py
--rw-r--r--   0        0        0      132 2024-03-13 18:51:24.457475 turbinia-20240313/turbinia/api/client/turbinia_api_lib/apis/paths/api_evidence_evidence_id.py
--rw-r--r--   0        0        0      121 2024-03-13 18:51:24.457475 turbinia-20240313/turbinia/api/client/turbinia_api_lib/apis/paths/api_evidence_query.py
--rw-r--r--   0        0        0      125 2024-03-13 18:51:24.457475 turbinia-20240313/turbinia/api/client/turbinia_api_lib/apis/paths/api_evidence_summary.py
--rw-r--r--   0        0        0      121 2024-03-13 18:51:24.461475 turbinia-20240313/turbinia/api/client/turbinia_api_lib/apis/paths/api_evidence_types.py
--rw-r--r--   0        0        0      147 2024-03-13 18:51:24.461475 turbinia-20240313/turbinia/api/client/turbinia_api_lib/apis/paths/api_evidence_types_evidence_type.py
--rw-r--r--   0        0        0      126 2024-03-13 18:51:24.461475 turbinia-20240313/turbinia/api/client/turbinia_api_lib/apis/paths/api_evidence_upload.py
--rw-r--r--   0        0        0      103 2024-03-13 18:51:24.461475 turbinia-20240313/turbinia/api/client/turbinia_api_lib/apis/paths/api_jobs_.py
--rw-r--r--   0        0        0      113 2024-03-13 18:51:24.461475 turbinia-20240313/turbinia/api/client/turbinia_api_lib/apis/paths/api_logs_query.py
--rw-r--r--   0        0        0      112 2024-03-13 18:51:24.461475 turbinia-20240313/turbinia/api/client/turbinia_api_lib/apis/paths/api_request_.py
--rw-r--r--   0        0        0      128 2024-03-13 18:51:24.461475 turbinia-20240313/turbinia/api/client/turbinia_api_lib/apis/paths/api_request_request_id.py
--rw-r--r--   0        0        0      123 2024-03-13 18:51:24.461475 turbinia-20240313/turbinia/api/client/turbinia_api_lib/apis/paths/api_request_summary.py
--rw-r--r--   0        0        0      141 2024-03-13 18:51:24.461475 turbinia-20240313/turbinia/api/client/turbinia_api_lib/apis/paths/api_result_request_request_id.py
--rw-r--r--   0        0        0      129 2024-03-13 18:51:24.461475 turbinia-20240313/turbinia/api/client/turbinia_api_lib/apis/paths/api_result_task_task_id.py
--rw-r--r--   0        0        0      123 2024-03-13 18:51:24.461475 turbinia-20240313/turbinia/api/client/turbinia_api_lib/apis/paths/api_task_statistics.py
--rw-r--r--   0        0        0      116 2024-03-13 18:51:24.461475 turbinia-20240313/turbinia/api/client/turbinia_api_lib/apis/paths/api_task_task_id.py
--rw-r--r--   0        0        0      117 2024-03-13 18:51:24.461475 turbinia-20240313/turbinia/api/client/turbinia_api_lib/apis/paths/api_task_workers.py
--rw-r--r--   0        0        0     1566 2024-03-13 18:51:24.461475 turbinia-20240313/turbinia/api/client/turbinia_api_lib/apis/tag_to_api.py
--rw-r--r--   0        0        0      599 2024-03-13 18:51:24.461475 turbinia-20240313/turbinia/api/client/turbinia_api_lib/apis/tags/__init__.py
--rw-r--r--   0        0        0      649 2024-03-13 18:51:24.461475 turbinia-20240313/turbinia/api/client/turbinia_api_lib/apis/tags/turbinia_configuration_api.py
--rw-r--r--   0        0        0     1067 2024-03-13 18:51:24.461475 turbinia-20240313/turbinia/api/client/turbinia_api_lib/apis/tags/turbinia_evidence_api.py
--rw-r--r--   0        0        0      527 2024-03-13 18:51:24.461475 turbinia-20240313/turbinia/api/client/turbinia_api_lib/apis/tags/turbinia_jobs_api.py
--rw-r--r--   0        0        0      530 2024-03-13 18:51:24.461475 turbinia-20240313/turbinia/api/client/turbinia_api_lib/apis/tags/turbinia_logs_api.py
--rw-r--r--   0        0        0      669 2024-03-13 18:51:24.461475 turbinia-20240313/turbinia/api/client/turbinia_api_lib/apis/tags/turbinia_request_results_api.py
--rw-r--r--   0        0        0      748 2024-03-13 18:51:24.461475 turbinia-20240313/turbinia/api/client/turbinia_api_lib/apis/tags/turbinia_requests_api.py
--rw-r--r--   0        0        0      740 2024-03-13 18:51:24.461475 turbinia-20240313/turbinia/api/client/turbinia_api_lib/apis/tags/turbinia_tasks_api.py
--rw-r--r--   0        0        0    14640 2024-03-13 18:51:24.461475 turbinia-20240313/turbinia/api/client/turbinia_api_lib/configuration.py
--rw-r--r--   0        0        0     5435 2024-03-13 18:51:24.461475 turbinia-20240313/turbinia/api/client/turbinia_api_lib/exceptions.py
--rw-r--r--   0        0        0      350 2024-03-13 18:51:24.461475 turbinia-20240313/turbinia/api/client/turbinia_api_lib/model/__init__.py
--rw-r--r--   0        0        0    10687 2024-03-13 18:51:24.461475 turbinia-20240313/turbinia/api/client/turbinia_api_lib/model/base_request_options.py
--rw-r--r--   0        0        0    10687 2024-03-13 18:51:24.461475 turbinia-20240313/turbinia/api/client/turbinia_api_lib/model/base_request_options.pyi
--rw-r--r--   0        0        0     6329 2024-03-13 18:51:24.461475 turbinia-20240313/turbinia/api/client/turbinia_api_lib/model/complete_turbinia_stats.py
--rw-r--r--   0        0        0     6329 2024-03-13 18:51:24.461475 turbinia-20240313/turbinia/api/client/turbinia_api_lib/model/complete_turbinia_stats.pyi
--rw-r--r--   0        0        0     3426 2024-03-13 18:51:24.461475 turbinia-20240313/turbinia/api/client/turbinia_api_lib/model/http_validation_error.py
--rw-r--r--   0        0        0     3426 2024-03-13 18:51:24.461475 turbinia-20240313/turbinia/api/client/turbinia_api_lib/model/http_validation_error.pyi
--rw-r--r--   0        0        0     3879 2024-03-13 18:51:24.461475 turbinia-20240313/turbinia/api/client/turbinia_api_lib/model/request.py
--rw-r--r--   0        0        0     3879 2024-03-13 18:51:24.461475 turbinia-20240313/turbinia/api/client/turbinia_api_lib/model/request.pyi
--rw-r--r--   0        0        0     6615 2024-03-13 18:51:24.461475 turbinia-20240313/turbinia/api/client/turbinia_api_lib/model/validation_error.py
--rw-r--r--   0        0        0     6615 2024-03-13 18:51:24.461475 turbinia-20240313/turbinia/api/client/turbinia_api_lib/model/validation_error.pyi
--rw-r--r--   0        0        0    11208 2024-03-13 18:51:24.461475 turbinia-20240313/turbinia/api/client/turbinia_api_lib/model/validation_error_loc_inner.py
--rw-r--r--   0        0        0    82314 2024-03-13 18:51:24.461475 turbinia-20240313/turbinia/api/client/turbinia_api_lib/model_utils.py
--rw-r--r--   0        0        0      800 2024-03-13 18:51:24.461475 turbinia-20240313/turbinia/api/client/turbinia_api_lib/models/__init__.py
--rw-r--r--   0        0        0     3164 2024-03-13 18:51:24.461475 turbinia-20240313/turbinia/api/client/turbinia_api_lib/models/base_request_options.py
--rw-r--r--   0        0        0     2897 2024-03-13 18:51:24.461475 turbinia-20240313/turbinia/api/client/turbinia_api_lib/models/body_upload_evidence_api_evidence_upload_post.py
--rw-r--r--   0        0        0     2771 2024-03-13 18:51:24.461475 turbinia-20240313/turbinia/api/client/turbinia_api_lib/models/complete_turbinia_stats.py
--rw-r--r--   0        0        0     2438 2024-03-13 18:51:24.461475 turbinia-20240313/turbinia/api/client/turbinia_api_lib/models/http_validation_error.py
--rw-r--r--   0        0        0     4694 2024-03-13 18:51:24.461475 turbinia-20240313/turbinia/api/client/turbinia_api_lib/models/location_inner.py
--rw-r--r--   0        0        0     2603 2024-03-13 18:51:24.461475 turbinia-20240313/turbinia/api/client/turbinia_api_lib/models/request.py
--rw-r--r--   0        0        0     2527 2024-03-13 18:51:24.461475 turbinia-20240313/turbinia/api/client/turbinia_api_lib/models/validation_error.py
--rw-r--r--   0        0        0     4709 2024-03-13 18:51:24.461475 turbinia-20240313/turbinia/api/client/turbinia_api_lib/models/validation_error_loc_inner.py
--rw-r--r--   0        0        0        0 2024-03-13 18:51:24.461475 turbinia-20240313/turbinia/api/client/turbinia_api_lib/py.typed
--rw-r--r--   0        0        0    13888 2024-03-13 18:51:24.461475 turbinia-20240313/turbinia/api/client/turbinia_api_lib/rest.py
--rw-r--r--   0        0        0    97694 2024-03-13 18:51:24.461475 turbinia-20240313/turbinia/api/client/turbinia_api_lib/schemas.py
--rw-r--r--   0        0        0      634 2024-03-13 18:51:24.461475 turbinia-20240313/turbinia/api/models/__init__.py
--rw-r--r--   0        0        0     7505 2024-03-13 18:51:24.461475 turbinia-20240313/turbinia/api/models/request_status.py
--rw-r--r--   0        0        0    10220 2024-03-13 18:51:24.461475 turbinia-20240313/turbinia/api/models/tasks_statistics.py
--rw-r--r--   0        0        0     5611 2024-03-13 18:51:24.461475 turbinia-20240313/turbinia/api/models/workers_status.py
--rw-r--r--   0        0        0    20391 2024-03-13 18:51:24.461475 turbinia-20240313/turbinia/api/openapi.yaml
--rw-r--r--   0        0        0      634 2024-03-13 18:51:24.461475 turbinia-20240313/turbinia/api/routes/__init__.py
--rw-r--r--   0        0        0     1870 2024-03-13 18:51:24.461475 turbinia-20240313/turbinia/api/routes/config.py
--rw-r--r--   0        0        0     9554 2024-03-13 18:51:24.461475 turbinia-20240313/turbinia/api/routes/evidence.py
--rw-r--r--   0        0        0     1755 2024-03-13 18:51:24.461475 turbinia-20240313/turbinia/api/routes/jobs.py
--rw-r--r--   0        0        0     1050 2024-03-13 18:51:24.461475 turbinia-20240313/turbinia/api/routes/logs.py
--rw-r--r--   0        0        0     8104 2024-03-13 18:51:24.461475 turbinia-20240313/turbinia/api/routes/request.py
--rw-r--r--   0        0        0     2876 2024-03-13 18:51:24.461475 turbinia-20240313/turbinia/api/routes/result.py
--rw-r--r--   0        0        0     1317 2024-03-13 18:51:24.461475 turbinia-20240313/turbinia/api/routes/router.py
--rw-r--r--   0        0        0     3603 2024-03-13 18:51:24.461475 turbinia-20240313/turbinia/api/routes/task.py
--rw-r--r--   0        0        0     1921 2024-03-13 18:51:24.461475 turbinia-20240313/turbinia/api/routes/ui.py
--rw-r--r--   0        0        0      635 2024-03-13 18:51:24.461475 turbinia-20240313/turbinia/api/schemas/__init__.py
--rw-r--r--   0        0        0      953 2024-03-13 18:51:24.461475 turbinia-20240313/turbinia/api/schemas/request.py
--rw-r--r--   0        0        0     1249 2024-03-13 18:51:24.461475 turbinia-20240313/turbinia/api/schemas/request_options.py
--rw-r--r--   0        0        0     4807 2024-03-13 18:51:24.461475 turbinia-20240313/turbinia/api/utils.py
--rw-r--r--   0        0        0    36095 2024-03-13 18:51:24.461475 turbinia-20240313/turbinia/client.py
--rw-r--r--   0        0        0     3127 2024-03-13 18:51:24.461475 turbinia-20240313/turbinia/client_stats_test.py
--rw-r--r--   0        0        0    16015 2024-03-13 18:51:24.461475 turbinia-20240313/turbinia/client_test.py
--rw-r--r--   0        0        0     7684 2024-03-13 18:51:24.465475 turbinia-20240313/turbinia/config/__init__.py
--rw-r--r--   0        0        0     3837 2024-03-13 18:51:24.465475 turbinia-20240313/turbinia/config/logger.py
--rw-r--r--   0        0        0      981 2024-03-13 18:51:24.465475 turbinia-20240313/turbinia/config/recipes/all.yaml
--rw-r--r--   0        0        0     1316 2024-03-13 18:51:24.465475 turbinia-20240313/turbinia/config/recipes/triage-linux-extended.yaml
--rw-r--r--   0        0        0      607 2024-03-13 18:51:24.465475 turbinia-20240313/turbinia/config/recipes/triage-linux.yaml
--rw-r--r--   0        0        0     1442 2024-03-13 18:51:24.465475 turbinia-20240313/turbinia/config/recipes/triage-macos.yml
--rw-r--r--   0        0        0     1378 2024-03-13 18:51:24.465475 turbinia-20240313/turbinia/config/recipes/triage-windows.yaml
--rw-r--r--   0        0        0      114 2024-03-13 18:51:24.465475 turbinia-20240313/turbinia/config/recipes/triage.yaml
--rw-r--r--   0        0        0      475 2024-03-13 18:51:24.465475 turbinia-20240313/turbinia/config/rules/pgsql_from_program.yar
--rw-r--r--   0        0        0      521 2024-03-13 18:51:24.465475 turbinia-20240313/turbinia/config/rules/redis_replicaof.yar
--rw-r--r--   0        0        0      671 2024-03-13 18:51:24.465475 turbinia-20240313/turbinia/config/rules/suspicious_cron.yar
--rw-r--r--   0        0        0      349 2024-03-13 18:51:24.465475 turbinia-20240313/turbinia/config/rules/suspicious_gitlab.yar
--rw-r--r--   0        0        0      290 2024-03-13 18:51:24.465475 turbinia-20240313/turbinia/config/rules/suspicious_hadoop.yar
--rw-r--r--   0        0        0     6889 2024-03-13 18:51:24.465475 turbinia-20240313/turbinia/config/turbinia_config_test.py
--rw-r--r--   0        0        0    14080 2024-03-13 18:51:24.465475 turbinia-20240313/turbinia/config/turbinia_config_tmpl.py
--rwxr-xr-x   0        0        0     2512 2024-03-13 18:51:24.465475 turbinia-20240313/turbinia/e2e/e2e-local.sh
--rw-r--r--   0        0        0      122 2024-03-13 18:51:24.465475 turbinia-20240313/turbinia/e2e/e2e-recipe.yaml
--rw-r--r--   0        0        0     5012 2024-03-13 18:51:24.465475 turbinia-20240313/turbinia/e2e/run-e2e-gke.sh
--rw-r--r--   0        0        0    50692 2024-03-13 18:51:24.465475 turbinia-20240313/turbinia/evidence.py
--rw-r--r--   0        0        0     4482 2024-03-13 18:51:24.465475 turbinia-20240313/turbinia/evidence_test.py
--rw-r--r--   0        0        0     1506 2024-03-13 18:51:24.465475 turbinia-20240313/turbinia/job_utils.py
--rw-r--r--   0        0        0     1728 2024-03-13 18:51:24.465475 turbinia-20240313/turbinia/jobs/__init__.py
--rw-r--r--   0        0        0     1730 2024-03-13 18:51:24.465475 turbinia-20240313/turbinia/jobs/binary_extractor.py
--rw-r--r--   0        0        0     1929 2024-03-13 18:51:24.465475 turbinia-20240313/turbinia/jobs/bulk_extractor.py
--rw-r--r--   0        0        0     1500 2024-03-13 18:51:24.465475 turbinia-20240313/turbinia/jobs/containerd.py
--rw-r--r--   0        0        0     1554 2024-03-13 18:51:24.465475 turbinia-20240313/turbinia/jobs/dfdewey.py
--rw-r--r--   0        0        0     1586 2024-03-13 18:51:24.465475 turbinia-20240313/turbinia/jobs/docker.py
--rw-r--r--   0        0        0     1776 2024-03-13 18:51:24.465475 turbinia-20240313/turbinia/jobs/file_system_timeline.py
--rw-r--r--   0        0        0     1665 2024-03-13 18:51:24.465475 turbinia-20240313/turbinia/jobs/finalize_request.py
--rw-r--r--   0        0        0     1277 2024-03-13 18:51:24.465475 turbinia-20240313/turbinia/jobs/fsstat.py
--rw-r--r--   0        0        0     1454 2024-03-13 18:51:24.465475 turbinia-20240313/turbinia/jobs/grep.py
--rw-r--r--   0        0        0     1438 2024-03-13 18:51:24.465475 turbinia-20240313/turbinia/jobs/hindsight.py
--rw-r--r--   0        0        0     2700 2024-03-13 18:51:24.465475 turbinia-20240313/turbinia/jobs/http_access_logs.py
--rw-r--r--   0        0        0     2306 2024-03-13 18:51:24.465475 turbinia-20240313/turbinia/jobs/imports_test.py
--rw-r--r--   0        0        0     3642 2024-03-13 18:51:24.465475 turbinia-20240313/turbinia/jobs/interface.py
--rw-r--r--   0        0        0     1914 2024-03-13 18:51:24.465475 turbinia-20240313/turbinia/jobs/interface_test.py
--rw-r--r--   0        0        0     1801 2024-03-13 18:51:24.465475 turbinia-20240313/turbinia/jobs/jenkins.py
--rw-r--r--   0        0        0     2615 2024-03-13 18:51:24.465475 turbinia-20240313/turbinia/jobs/jupyter.py
--rw-r--r--   0        0        0     1827 2024-03-13 18:51:24.465475 turbinia-20240313/turbinia/jobs/linux_acct.py
--rw-r--r--   0        0        0     4535 2024-03-13 18:51:24.465475 turbinia-20240313/turbinia/jobs/llm_artifacts_analyzer.py
--rw-r--r--   0        0        0     8630 2024-03-13 18:51:24.465475 turbinia-20240313/turbinia/jobs/manager.py
--rw-r--r--   0        0        0     5185 2024-03-13 18:51:24.465475 turbinia-20240313/turbinia/jobs/manager_test.py
--rw-r--r--   0        0        0     1735 2024-03-13 18:51:24.465475 turbinia-20240313/turbinia/jobs/partitions.py
--rw-r--r--   0        0        0     1304 2024-03-13 18:51:24.465475 turbinia-20240313/turbinia/jobs/photorec.py
--rw-r--r--   0        0        0     2210 2024-03-13 18:51:24.465475 turbinia-20240313/turbinia/jobs/plaso.py
--rw-r--r--   0        0        0     1668 2024-03-13 18:51:24.465475 turbinia-20240313/turbinia/jobs/postgres_acct.py
--rw-r--r--   0        0        0     1379 2024-03-13 18:51:24.465475 turbinia-20240313/turbinia/jobs/psort.py
--rw-r--r--   0        0        0     2571 2024-03-13 18:51:24.465475 turbinia-20240313/turbinia/jobs/redis.py
--rw-r--r--   0        0        0     1832 2024-03-13 18:51:24.465475 turbinia-20240313/turbinia/jobs/ssh_analyzer.py
--rw-r--r--   0        0        0     2562 2024-03-13 18:51:24.465475 turbinia-20240313/turbinia/jobs/sshd.py
--rw-r--r--   0        0        0     1672 2024-03-13 18:51:24.465475 turbinia-20240313/turbinia/jobs/strings.py
--rw-r--r--   0        0        0     2563 2024-03-13 18:51:24.465475 turbinia-20240313/turbinia/jobs/tomcat.py
--rw-r--r--   0        0        0     1554 2024-03-13 18:51:24.465475 turbinia-20240313/turbinia/jobs/volatility.py
--rw-r--r--   0        0        0     1844 2024-03-13 18:51:24.465475 turbinia-20240313/turbinia/jobs/windows_acct.py
--rw-r--r--   0        0        0     1855 2024-03-13 18:51:24.465475 turbinia-20240313/turbinia/jobs/wordpress_creds.py
--rw-r--r--   0        0        0     1465 2024-03-13 18:51:24.465475 turbinia-20240313/turbinia/jobs/worker_stat.py
--rw-r--r--   0        0        0     1587 2024-03-13 18:51:24.465475 turbinia-20240313/turbinia/jobs/yara.py
--rw-r--r--   0        0        0        0 2024-03-13 18:51:24.465475 turbinia-20240313/turbinia/lib/__init__.py
--rw-r--r--   0        0        0     9648 2024-03-13 18:51:24.465475 turbinia-20240313/turbinia/lib/docker_manager.py
--rw-r--r--   0        0        0     8382 2024-03-13 18:51:24.465475 turbinia-20240313/turbinia/lib/dockermanager_test.py
--rw-r--r--   0        0        0     2865 2024-03-13 18:51:24.465475 turbinia-20240313/turbinia/lib/file_helpers.py
--rw-r--r--   0        0        0     2470 2024-03-13 18:51:24.465475 turbinia-20240313/turbinia/lib/google_cloud.py
--rw-r--r--   0        0        0     1290 2024-03-13 18:51:24.465475 turbinia-20240313/turbinia/lib/google_cloud_test.py
--rw-r--r--   0        0        0        0 2024-03-13 18:51:24.465475 turbinia-20240313/turbinia/lib/llm_libs/__init__.py
--rw-r--r--   0        0        0      782 2024-03-13 18:51:24.465475 turbinia-20240313/turbinia/lib/llm_libs/llm_client.py
--rw-r--r--   0        0        0      678 2024-03-13 18:51:24.465475 turbinia-20240313/turbinia/lib/llm_libs/llm_lib_base.py
--rw-r--r--   0        0        0     4392 2024-03-13 18:51:24.465475 turbinia-20240313/turbinia/lib/llm_libs/vertex_ai_lib.py
--rw-r--r--   0        0        0     1462 2024-03-13 18:51:24.465475 turbinia-20240313/turbinia/lib/llm_libs/vertex_ai_lib_test.py
--rw-r--r--   0        0        0     7265 2024-03-13 18:51:24.465475 turbinia-20240313/turbinia/lib/recipe_helpers.py
--rw-r--r--   0        0        0     7341 2024-03-13 18:51:24.465475 turbinia-20240313/turbinia/lib/recipe_helpers_test.py
--rw-r--r--   0        0        0     2300 2024-03-13 18:51:24.465475 turbinia-20240313/turbinia/lib/text_formatter.py
--rw-r--r--   0        0        0     1551 2024-03-13 18:51:24.465475 turbinia-20240313/turbinia/lib/text_formatter_test.py
--rw-r--r--   0        0        0     8373 2024-03-13 18:51:24.465475 turbinia-20240313/turbinia/lib/utils.py
--rw-r--r--   0        0        0     4854 2024-03-13 18:51:24.465475 turbinia-20240313/turbinia/message.py
--rw-r--r--   0        0        0     2675 2024-03-13 18:51:24.465475 turbinia-20240313/turbinia/notify.py
--rw-r--r--   0        0        0     4011 2024-03-13 18:51:24.465475 turbinia-20240313/turbinia/notify_test.py
--rw-r--r--   0        0        0    18093 2024-03-13 18:51:24.465475 turbinia-20240313/turbinia/output_manager.py
--rw-r--r--   0        0        0     9307 2024-03-13 18:51:24.465475 turbinia-20240313/turbinia/output_manager_test.py
--rw-r--r--   0        0        0        0 2024-03-13 18:51:24.465475 turbinia-20240313/turbinia/processors/__init__.py
--rw-r--r--   0        0        0     4292 2024-03-13 18:51:24.465475 turbinia-20240313/turbinia/processors/archive.py
--rw-r--r--   0        0        0     3001 2024-03-13 18:51:24.465475 turbinia-20240313/turbinia/processors/archive_test.py
--rw-r--r--   0        0        0     3100 2024-03-13 18:51:24.469475 turbinia-20240313/turbinia/processors/containerd.py
--rw-r--r--   0        0        0     3045 2024-03-13 18:51:24.469475 turbinia-20240313/turbinia/processors/docker.py
--rw-r--r--   0        0        0     5319 2024-03-13 18:51:24.469475 turbinia-20240313/turbinia/processors/google_cloud.py
--rw-r--r--   0        0        0    21986 2024-03-13 18:51:24.469475 turbinia-20240313/turbinia/processors/mount_local.py
--rw-r--r--   0        0        0    21404 2024-03-13 18:51:24.469475 turbinia-20240313/turbinia/processors/mount_local_test.py
--rw-r--r--   0        0        0     2907 2024-03-13 18:51:24.469475 turbinia-20240313/turbinia/processors/partitions.py
--rw-r--r--   0        0        0     4175 2024-03-13 18:51:24.469475 turbinia-20240313/turbinia/processors/partitions_test.py
--rw-r--r--   0        0        0     5019 2024-03-13 18:51:24.469475 turbinia-20240313/turbinia/processors/resource_manager.py
--rw-r--r--   0        0        0     4828 2024-03-13 18:51:24.469475 turbinia-20240313/turbinia/processors/resource_manager_test.py
--rw-r--r--   0        0        0     2103 2024-03-13 18:51:24.469475 turbinia-20240313/turbinia/server.py
--rw-r--r--   0        0        0     1973 2024-03-13 18:51:24.469475 turbinia-20240313/turbinia/server_test.py
--rw-r--r--   0        0        0    19142 2024-03-13 18:51:24.469475 turbinia-20240313/turbinia/state_manager.py
--rw-r--r--   0        0        0     8222 2024-03-13 18:51:24.469475 turbinia-20240313/turbinia/state_manager_test.py
--rw-r--r--   0        0        0    26661 2024-03-13 18:51:24.469475 turbinia-20240313/turbinia/task_manager.py
--rw-r--r--   0        0        0    13214 2024-03-13 18:51:24.469475 turbinia-20240313/turbinia/task_manager_test.py
--rw-r--r--   0        0        0     7138 2024-03-13 18:51:24.469475 turbinia-20240313/turbinia/task_utils.py
--rw-r--r--   0        0        0     2579 2024-03-13 18:51:24.469475 turbinia-20240313/turbinia/task_utils_test.py
--rw-r--r--   0        0        0     3474 2024-03-13 18:51:24.469475 turbinia-20240313/turbinia/tcelery.py
--rw-r--r--   0        0        0    40378 2024-03-13 18:51:24.469475 turbinia-20240313/turbinia/turbiniactl.py
--rw-r--r--   0        0        0    22722 2024-03-13 18:51:24.469475 turbinia-20240313/turbinia/turbiniactl_test.py
--rw-r--r--   0        0        0     9081 2024-03-13 18:51:24.469475 turbinia-20240313/turbinia/worker.py
--rw-r--r--   0        0        0     7357 2024-03-13 18:51:24.469475 turbinia-20240313/turbinia/worker_test.py
--rw-r--r--   0        0        0    43291 2024-03-13 18:51:24.469475 turbinia-20240313/turbinia/workers/__init__.py
--rw-r--r--   0        0        0      771 2024-03-13 18:51:24.469475 turbinia-20240313/turbinia/workers/abort.py
--rw-r--r--   0        0        0        0 2024-03-13 18:51:24.469475 turbinia-20240313/turbinia/workers/analysis/__init__.py
--rw-r--r--   0        0        0     3001 2024-03-13 18:51:24.469475 turbinia-20240313/turbinia/workers/analysis/analyzer_output.py
--rw-r--r--   0        0        0    28184 2024-03-13 18:51:24.469475 turbinia-20240313/turbinia/workers/analysis/auth.py
--rw-r--r--   0        0        0    21227 2024-03-13 18:51:24.469475 turbinia-20240313/turbinia/workers/analysis/auth_test.py
--rw-r--r--   0        0        0     7038 2024-03-13 18:51:24.469475 turbinia-20240313/turbinia/workers/analysis/jenkins.py
--rw-r--r--   0        0        0     6527 2024-03-13 18:51:24.469475 turbinia-20240313/turbinia/workers/analysis/jenkins_test.py
--rw-r--r--   0        0        0     4446 2024-03-13 18:51:24.469475 turbinia-20240313/turbinia/workers/analysis/jupyter.py
--rw-r--r--   0        0        0     2343 2024-03-13 18:51:24.469475 turbinia-20240313/turbinia/workers/analysis/jupyter_test.py
--rw-r--r--   0        0        0     5175 2024-03-13 18:51:24.469475 turbinia-20240313/turbinia/workers/analysis/linux_acct.py
--rw-r--r--   0        0        0     3301 2024-03-13 18:51:24.469475 turbinia-20240313/turbinia/workers/analysis/linux_acct_test.py
--rw-r--r--   0        0        0     9174 2024-03-13 18:51:24.469475 turbinia-20240313/turbinia/workers/analysis/llm_analyzer.py
--rw-r--r--   0        0        0     3352 2024-03-13 18:51:24.469475 turbinia-20240313/turbinia/workers/analysis/llm_analyzer_test.py
--rw-r--r--   0        0        0     9655 2024-03-13 18:51:24.469475 turbinia-20240313/turbinia/workers/analysis/postgresql_acct.py
--rw-r--r--   0        0        0     4113 2024-03-13 18:51:24.469475 turbinia-20240313/turbinia/workers/analysis/postgresql_acct_test.py
--rw-r--r--   0        0        0     3270 2024-03-13 18:51:24.469475 turbinia-20240313/turbinia/workers/analysis/redis.py
--rw-r--r--   0        0        0     1912 2024-03-13 18:51:24.469475 turbinia-20240313/turbinia/workers/analysis/redis_test.py
--rw-r--r--   0        0        0    18021 2024-03-13 18:51:24.469475 turbinia-20240313/turbinia/workers/analysis/ssh_analyzer.py
--rw-r--r--   0        0        0     5147 2024-03-13 18:51:24.469475 turbinia-20240313/turbinia/workers/analysis/ssh_analyzer_test.py
--rw-r--r--   0        0        0     3770 2024-03-13 18:51:24.469475 turbinia-20240313/turbinia/workers/analysis/sshd.py
--rw-r--r--   0        0        0     1984 2024-03-13 18:51:24.469475 turbinia-20240313/turbinia/workers/analysis/sshd_test.py
--rw-r--r--   0        0        0     3968 2024-03-13 18:51:24.469475 turbinia-20240313/turbinia/workers/analysis/tomcat.py
--rw-r--r--   0        0        0     3928 2024-03-13 18:51:24.469475 turbinia-20240313/turbinia/workers/analysis/tomcat_test.py
--rw-r--r--   0        0        0     9398 2024-03-13 18:51:24.469475 turbinia-20240313/turbinia/workers/analysis/windows_acct.py
--rw-r--r--   0        0        0     2992 2024-03-13 18:51:24.469475 turbinia-20240313/turbinia/workers/analysis/windows_acct_test.py
--rw-r--r--   0        0        0     4522 2024-03-13 18:51:24.469475 turbinia-20240313/turbinia/workers/analysis/wordpress_access.py
--rw-r--r--   0        0        0     2003 2024-03-13 18:51:24.469475 turbinia-20240313/turbinia/workers/analysis/wordpress_access_test.py
--rw-r--r--   0        0        0     7245 2024-03-13 18:51:24.469475 turbinia-20240313/turbinia/workers/analysis/wordpress_creds.py
--rw-r--r--   0        0        0     2750 2024-03-13 18:51:24.469475 turbinia-20240313/turbinia/workers/analysis/wordpress_creds_test.py
--rw-r--r--   0        0        0     5325 2024-03-13 18:51:24.469475 turbinia-20240313/turbinia/workers/analysis/yara.py
--rw-r--r--   0        0        0     2670 2024-03-13 18:51:24.469475 turbinia-20240313/turbinia/workers/analysis/yara_test.py
--rw-r--r--   0        0        0     6455 2024-03-13 18:51:24.469475 turbinia-20240313/turbinia/workers/artifact.py
--rw-r--r--   0        0        0     5824 2024-03-13 18:51:24.469475 turbinia-20240313/turbinia/workers/binary_extractor.py
--rw-r--r--   0        0        0     3572 2024-03-13 18:51:24.469475 turbinia-20240313/turbinia/workers/binary_extractor_test.py
--rw-r--r--   0        0        0     8311 2024-03-13 18:51:24.469475 turbinia-20240313/turbinia/workers/bulk_extractor.py
--rw-r--r--   0        0        0     3299 2024-03-13 18:51:24.469475 turbinia-20240313/turbinia/workers/bulk_extractor_test.py
--rw-r--r--   0        0        0    10652 2024-03-13 18:51:24.469475 turbinia-20240313/turbinia/workers/containerd.py
--rw-r--r--   0        0        0     2373 2024-03-13 18:51:24.469475 turbinia-20240313/turbinia/workers/containerd_test.py
--rw-r--r--   0        0        0     3208 2024-03-13 18:51:24.469475 turbinia-20240313/turbinia/workers/dfdewey.py
--rw-r--r--   0        0        0     2490 2024-03-13 18:51:24.469475 turbinia-20240313/turbinia/workers/dfdewey_test.py
--rw-r--r--   0        0        0     4334 2024-03-13 18:51:24.469475 turbinia-20240313/turbinia/workers/docker.py
--rw-r--r--   0        0        0     2355 2024-03-13 18:51:24.469475 turbinia-20240313/turbinia/workers/docker_test.py
--rw-r--r--   0        0        0     5146 2024-03-13 18:51:24.469475 turbinia-20240313/turbinia/workers/file_system_timeline.py
--rw-r--r--   0        0        0     3159 2024-03-13 18:51:24.469475 turbinia-20240313/turbinia/workers/file_system_timeline_test.py
--rw-r--r--   0        0        0     2045 2024-03-13 18:51:24.469475 turbinia-20240313/turbinia/workers/finalize_request.py
--rw-r--r--   0        0        0     2148 2024-03-13 18:51:24.473475 turbinia-20240313/turbinia/workers/fsstat.py
--rw-r--r--   0        0        0     2648 2024-03-13 18:51:24.473475 turbinia-20240313/turbinia/workers/fsstat_test.py
--rw-r--r--   0        0        0     2493 2024-03-13 18:51:24.473475 turbinia-20240313/turbinia/workers/grep.py
--rw-r--r--   0        0        0     1969 2024-03-13 18:51:24.473475 turbinia-20240313/turbinia/workers/hindsight.py
--rw-r--r--   0        0        0    10479 2024-03-13 18:51:24.473475 turbinia-20240313/turbinia/workers/partitions.py
--rw-r--r--   0        0        0    10303 2024-03-13 18:51:24.473475 turbinia-20240313/turbinia/workers/partitions_test.py
--rw-r--r--   0        0        0     2873 2024-03-13 18:51:24.473475 turbinia-20240313/turbinia/workers/photorec.py
--rw-r--r--   0        0        0     1694 2024-03-13 18:51:24.473475 turbinia-20240313/turbinia/workers/photorec_test.py
--rw-r--r--   0        0        0     6031 2024-03-13 18:51:24.473475 turbinia-20240313/turbinia/workers/plaso.py
--rw-r--r--   0        0        0     2518 2024-03-13 18:51:24.473475 turbinia-20240313/turbinia/workers/plaso_test.py
--rw-r--r--   0        0        0     2882 2024-03-13 18:51:24.473475 turbinia-20240313/turbinia/workers/psort.py
--rw-r--r--   0        0        0     3034 2024-03-13 18:51:24.473475 turbinia-20240313/turbinia/workers/strings.py
--rw-r--r--   0        0        0     3652 2024-03-13 18:51:24.473475 turbinia-20240313/turbinia/workers/volatility.py
--rw-r--r--   0        0        0     2971 2024-03-13 18:51:24.473475 turbinia-20240313/turbinia/workers/volatility_test.py
--rw-r--r--   0        0        0     1718 2024-03-13 18:51:24.473475 turbinia-20240313/turbinia/workers/worker_stat.py
--rw-r--r--   0        0        0    18072 2024-03-13 18:51:24.473475 turbinia-20240313/turbinia/workers/workers_test.py
--rw-r--r--   0        0        0     1063 2024-03-13 18:51:24.473475 turbinia-20240313/turbinia/yapf_test.py
--rw-r--r--   0        0        0     8271 1970-01-01 00:00:00.000000 turbinia-20240313/PKG-INFO
+-rw-r--r--   0        0        0      427 2024-04-24 20:07:16.282061 turbinia-20240412.1/AUTHORS
+-rw-r--r--   0        0        0    11358 2024-04-24 20:07:16.282061 turbinia-20240412.1/LICENSE
+-rw-r--r--   0        0        0     6641 2024-04-24 20:07:16.282061 turbinia-20240412.1/README.md
+-rw-r--r--   0        0        0     1960 2024-04-24 20:07:16.294061 turbinia-20240412.1/pyproject.toml
+-rw-r--r--   0        0        0     1611 2024-04-24 20:07:16.670056 turbinia-20240412.1/turbinia/__init__.py
+-rw-r--r--   0        0        0      626 2024-04-24 20:07:16.670056 turbinia-20240412.1/turbinia/api/__init__.py
+-rw-r--r--   0        0        0     3019 2024-04-24 20:07:16.670056 turbinia-20240412.1/turbinia/api/api_server.py
+-rw-r--r--   0        0        0    18203 2024-04-24 20:07:16.674056 turbinia-20240412.1/turbinia/api/api_server_test.py
+-rw-r--r--   0        0        0      823 2024-04-24 20:07:16.674056 turbinia-20240412.1/turbinia/api/cli/.turbinia_api_config.json
+-rw-r--r--   0        0        0    11358 2024-04-24 20:07:16.674056 turbinia-20240412.1/turbinia/api/cli/LICENSE
+-rw-r--r--   0        0        0     8306 2024-04-24 20:07:16.674056 turbinia-20240412.1/turbinia/api/cli/README.rst
+-rw-r--r--   0        0        0    45781 2024-04-24 20:07:16.674056 turbinia-20240412.1/turbinia/api/cli/poetry.lock
+-rw-r--r--   0        0        0      697 2024-04-24 20:07:16.674056 turbinia-20240412.1/turbinia/api/cli/pyproject.toml
+-rw-r--r--   0        0        0    17381 2024-04-24 20:07:16.674056 turbinia-20240412.1/turbinia/api/cli/requirements.txt
+-rw-r--r--   0        0        0      645 2024-04-24 20:07:16.674056 turbinia-20240412.1/turbinia/api/cli/turbinia_client/__init__.py
+-rw-r--r--   0        0        0      645 2024-04-24 20:07:16.674056 turbinia-20240412.1/turbinia/api/cli/turbinia_client/core/__init__.py
+-rw-r--r--   0        0        0    19782 2024-04-24 20:07:16.674056 turbinia-20240412.1/turbinia/api/cli/turbinia_client/core/commands.py
+-rw-r--r--   0        0        0     2274 2024-04-24 20:07:16.674056 turbinia-20240412.1/turbinia/api/cli/turbinia_client/core/groups.py
+-rw-r--r--   0        0        0      645 2024-04-24 20:07:16.674056 turbinia-20240412.1/turbinia/api/cli/turbinia_client/factory/__init__.py
+-rw-r--r--   0        0        0     5693 2024-04-24 20:07:16.674056 turbinia-20240412.1/turbinia/api/cli/turbinia_client/factory/factory.py
+-rw-r--r--   0        0        0      645 2024-04-24 20:07:16.674056 turbinia-20240412.1/turbinia/api/cli/turbinia_client/helpers/__init__.py
+-rw-r--r--   0        0        0     2626 2024-04-24 20:07:16.674056 turbinia-20240412.1/turbinia/api/cli/turbinia_client/helpers/auth_helper.py
+-rw-r--r--   0        0        0     5033 2024-04-24 20:07:16.674056 turbinia-20240412.1/turbinia/api/cli/turbinia_client/helpers/click_helper.py
+-rw-r--r--   0        0        0    22848 2024-04-24 20:07:16.674056 turbinia-20240412.1/turbinia/api/cli/turbinia_client/helpers/formatter.py
+-rw-r--r--   0        0        0     8285 2024-04-24 20:07:16.674056 turbinia-20240412.1/turbinia/api/cli/turbinia_client/helpers/formatter_test.py
+-rw-r--r--   0        0        0     8988 2024-04-24 20:07:16.674056 turbinia-20240412.1/turbinia/api/cli/turbinia_client/turbiniacli.py
+-rw-r--r--   0        0        0     2768 2024-04-24 20:07:16.674056 turbinia-20240412.1/turbinia/api/cli/turbinia_client/turbiniacli_test.py
+-rw-r--r--   0        0        0     4487 2024-04-24 20:07:16.674056 turbinia-20240412.1/turbinia/api/cli/turbinia_client/turbiniacli_tool.py
+-rw-r--r--   0        0        0     1354 2024-04-24 20:07:16.674056 turbinia-20240412.1/turbinia/api/client/.github/workflows/python.yml
+-rw-r--r--   0        0        0      807 2024-04-24 20:07:16.674056 turbinia-20240412.1/turbinia/api/client/.gitignore
+-rw-r--r--   0        0        0      711 2024-04-24 20:07:16.674056 turbinia-20240412.1/turbinia/api/client/.gitlab-ci.yml
+-rw-r--r--   0        0        0     1133 2024-04-24 20:07:16.674056 turbinia-20240412.1/turbinia/api/client/.openapi-generator-ignore
+-rw-r--r--   0        0        0      431 2024-04-24 20:07:16.674056 turbinia-20240412.1/turbinia/api/client/.travis.yml
+-rw-r--r--   0        0        0    11358 2024-04-24 20:07:16.674056 turbinia-20240412.1/turbinia/api/client/LICENSE
+-rw-r--r--   0        0        0     6158 2024-04-24 20:07:16.674056 turbinia-20240412.1/turbinia/api/client/README.md
+-rw-r--r--   0        0        0     1465 2024-04-24 20:07:16.674056 turbinia-20240412.1/turbinia/api/client/docs/BaseRequestOptions.md
+-rw-r--r--   0        0        0     1328 2024-04-24 20:07:16.674056 turbinia-20240412.1/turbinia/api/client/docs/CompleteTurbiniaStats.md
+-rw-r--r--   0        0        0     1004 2024-04-24 20:07:16.674056 turbinia-20240412.1/turbinia/api/client/docs/HTTPValidationError.md
+-rw-r--r--   0        0        0      841 2024-04-24 20:07:16.674056 turbinia-20240412.1/turbinia/api/client/docs/LocationInner.md
+-rw-r--r--   0        0        0      967 2024-04-24 20:07:16.674056 turbinia-20240412.1/turbinia/api/client/docs/Request.md
+-rw-r--r--   0        0        0     6243 2024-04-24 20:07:16.674056 turbinia-20240412.1/turbinia/api/client/docs/TurbiniaConfigurationApi.md
+-rw-r--r--   0        0        0    15608 2024-04-24 20:07:16.674056 turbinia-20240412.1/turbinia/api/client/docs/TurbiniaEvidenceApi.md
+-rw-r--r--   0        0        0     2116 2024-04-24 20:07:16.674056 turbinia-20240412.1/turbinia/api/client/docs/TurbiniaJobsApi.md
+-rw-r--r--   0        0        0     2241 2024-04-24 20:07:16.674056 turbinia-20240412.1/turbinia/api/client/docs/TurbiniaLogsApi.md
+-rw-r--r--   0        0        0     6932 2024-04-24 20:07:16.674056 turbinia-20240412.1/turbinia/api/client/docs/TurbiniaRequestResultsApi.md
+-rw-r--r--   0        0        0     7397 2024-04-24 20:07:16.674056 turbinia-20240412.1/turbinia/api/client/docs/TurbiniaRequestsApi.md
+-rw-r--r--   0        0        0     8008 2024-04-24 20:07:16.674056 turbinia-20240412.1/turbinia/api/client/docs/TurbiniaTasksApi.md
+-rw-r--r--   0        0        0      976 2024-04-24 20:07:16.674056 turbinia-20240412.1/turbinia/api/client/docs/ValidationError.md
+-rw-r--r--   0        0        0     1830 2024-04-24 20:07:16.674056 turbinia-20240412.1/turbinia/api/client/git_push.sh
+-rw-r--r--   0        0        0    20835 2024-04-24 20:07:16.674056 turbinia-20240412.1/turbinia/api/client/poetry.lock
+-rw-r--r--   0        0        0      838 2024-04-24 20:07:16.674056 turbinia-20240412.1/turbinia/api/client/pyproject.toml
+-rw-r--r--   0        0        0      152 2024-04-24 20:07:16.674056 turbinia-20240412.1/turbinia/api/client/tox.ini
+-rw-r--r--   0        0        0     1888 2024-04-24 20:07:16.674056 turbinia-20240412.1/turbinia/api/client/turbinia_api_lib/__init__.py
+-rw-r--r--   0        0        0      574 2024-04-24 20:07:16.674056 turbinia-20240412.1/turbinia/api/client/turbinia_api_lib/api/__init__.py
+-rw-r--r--   0        0        0    17390 2024-04-24 20:07:16.674056 turbinia-20240412.1/turbinia/api/client/turbinia_api_lib/api/turbinia_configuration_api.py
+-rw-r--r--   0        0        0    41146 2024-04-24 20:07:16.674056 turbinia-20240412.1/turbinia/api/client/turbinia_api_lib/api/turbinia_evidence_api.py
+-rw-r--r--   0        0        0     6449 2024-04-24 20:07:16.674056 turbinia-20240412.1/turbinia/api/client/turbinia_api_lib/api/turbinia_jobs_api.py
+-rw-r--r--   0        0        0     6741 2024-04-24 20:07:16.674056 turbinia-20240412.1/turbinia/api/client/turbinia_api_lib/api/turbinia_logs_api.py
+-rw-r--r--   0        0        0    18611 2024-04-24 20:07:16.674056 turbinia-20240412.1/turbinia/api/client/turbinia_api_lib/api/turbinia_request_results_api.py
+-rw-r--r--   0        0        0    19936 2024-04-24 20:07:16.674056 turbinia-20240412.1/turbinia/api/client/turbinia_api_lib/api/turbinia_requests_api.py
+-rw-r--r--   0        0        0    21265 2024-04-24 20:07:16.674056 turbinia-20240412.1/turbinia/api/client/turbinia_api_lib/api/turbinia_tasks_api.py
+-rw-r--r--   0        0        0    29543 2024-04-24 20:07:16.674056 turbinia-20240412.1/turbinia/api/client/turbinia_api_lib/api_client.py
+-rw-r--r--   0        0        0      852 2024-04-24 20:07:16.674056 turbinia-20240412.1/turbinia/api/client/turbinia_api_lib/api_response.py
+-rw-r--r--   0        0        0    14640 2024-04-24 20:07:16.674056 turbinia-20240412.1/turbinia/api/client/turbinia_api_lib/configuration.py
+-rw-r--r--   0        0        0     5435 2024-04-24 20:07:16.674056 turbinia-20240412.1/turbinia/api/client/turbinia_api_lib/exceptions.py
+-rw-r--r--   0        0        0      800 2024-04-24 20:07:16.674056 turbinia-20240412.1/turbinia/api/client/turbinia_api_lib/models/__init__.py
+-rw-r--r--   0        0        0     3164 2024-04-24 20:07:16.674056 turbinia-20240412.1/turbinia/api/client/turbinia_api_lib/models/base_request_options.py
+-rw-r--r--   0        0        0     2771 2024-04-24 20:07:16.674056 turbinia-20240412.1/turbinia/api/client/turbinia_api_lib/models/complete_turbinia_stats.py
+-rw-r--r--   0        0        0     2438 2024-04-24 20:07:16.674056 turbinia-20240412.1/turbinia/api/client/turbinia_api_lib/models/http_validation_error.py
+-rw-r--r--   0        0        0     4694 2024-04-24 20:07:16.674056 turbinia-20240412.1/turbinia/api/client/turbinia_api_lib/models/location_inner.py
+-rw-r--r--   0        0        0     2603 2024-04-24 20:07:16.678056 turbinia-20240412.1/turbinia/api/client/turbinia_api_lib/models/request.py
+-rw-r--r--   0        0        0     2527 2024-04-24 20:07:16.678056 turbinia-20240412.1/turbinia/api/client/turbinia_api_lib/models/validation_error.py
+-rw-r--r--   0        0        0        0 2024-04-24 20:07:16.678056 turbinia-20240412.1/turbinia/api/client/turbinia_api_lib/py.typed
+-rw-r--r--   0        0        0    13888 2024-04-24 20:07:16.678056 turbinia-20240412.1/turbinia/api/client/turbinia_api_lib/rest.py
+-rw-r--r--   0        0        0      634 2024-04-24 20:07:16.678056 turbinia-20240412.1/turbinia/api/models/__init__.py
+-rw-r--r--   0        0        0     7505 2024-04-24 20:07:16.678056 turbinia-20240412.1/turbinia/api/models/request_status.py
+-rw-r--r--   0        0        0    10220 2024-04-24 20:07:16.678056 turbinia-20240412.1/turbinia/api/models/tasks_statistics.py
+-rw-r--r--   0        0        0     5611 2024-04-24 20:07:16.678056 turbinia-20240412.1/turbinia/api/models/workers_status.py
+-rw-r--r--   0        0        0    21448 2024-04-24 20:07:16.678056 turbinia-20240412.1/turbinia/api/openapi.yaml
+-rw-r--r--   0        0        0      634 2024-04-24 20:07:16.678056 turbinia-20240412.1/turbinia/api/routes/__init__.py
+-rw-r--r--   0        0        0     2101 2024-04-24 20:07:16.678056 turbinia-20240412.1/turbinia/api/routes/config.py
+-rw-r--r--   0        0        0     9535 2024-04-24 20:07:16.678056 turbinia-20240412.1/turbinia/api/routes/evidence.py
+-rw-r--r--   0        0        0     1753 2024-04-24 20:07:16.678056 turbinia-20240412.1/turbinia/api/routes/jobs.py
+-rw-r--r--   0        0        0     1048 2024-04-24 20:07:16.678056 turbinia-20240412.1/turbinia/api/routes/logs.py
+-rw-r--r--   0        0        0     8102 2024-04-24 20:07:16.678056 turbinia-20240412.1/turbinia/api/routes/request.py
+-rw-r--r--   0        0        0     3557 2024-04-24 20:07:16.678056 turbinia-20240412.1/turbinia/api/routes/result.py
+-rw-r--r--   0        0        0     1369 2024-04-24 20:07:16.678056 turbinia-20240412.1/turbinia/api/routes/router.py
+-rw-r--r--   0        0        0     3603 2024-04-24 20:07:16.678056 turbinia-20240412.1/turbinia/api/routes/task.py
+-rw-r--r--   0        0        0     1921 2024-04-24 20:07:16.678056 turbinia-20240412.1/turbinia/api/routes/ui.py
+-rw-r--r--   0        0        0      635 2024-04-24 20:07:16.678056 turbinia-20240412.1/turbinia/api/schemas/__init__.py
+-rw-r--r--   0        0        0      953 2024-04-24 20:07:16.678056 turbinia-20240412.1/turbinia/api/schemas/request.py
+-rw-r--r--   0        0        0     1249 2024-04-24 20:07:16.678056 turbinia-20240412.1/turbinia/api/schemas/request_options.py
+-rw-r--r--   0        0        0     6282 2024-04-24 20:07:16.678056 turbinia-20240412.1/turbinia/api/utils.py
+-rw-r--r--   0        0        0    36093 2024-04-24 20:07:16.678056 turbinia-20240412.1/turbinia/client.py
+-rw-r--r--   0        0        0     3127 2024-04-24 20:07:16.678056 turbinia-20240412.1/turbinia/client_stats_test.py
+-rw-r--r--   0        0        0    16015 2024-04-24 20:07:16.678056 turbinia-20240412.1/turbinia/client_test.py
+-rw-r--r--   0        0        0     7682 2024-04-24 20:07:16.678056 turbinia-20240412.1/turbinia/config/__init__.py
+-rw-r--r--   0        0        0     3869 2024-04-24 20:07:16.678056 turbinia-20240412.1/turbinia/config/logger.py
+-rw-r--r--   0        0        0      981 2024-04-24 20:07:16.678056 turbinia-20240412.1/turbinia/config/recipes/all.yaml
+-rw-r--r--   0        0        0     1316 2024-04-24 20:07:16.678056 turbinia-20240412.1/turbinia/config/recipes/triage-linux-extended.yaml
+-rw-r--r--   0        0        0      607 2024-04-24 20:07:16.678056 turbinia-20240412.1/turbinia/config/recipes/triage-linux.yaml
+-rw-r--r--   0        0        0     1442 2024-04-24 20:07:16.678056 turbinia-20240412.1/turbinia/config/recipes/triage-macos.yml
+-rw-r--r--   0        0        0     1378 2024-04-24 20:07:16.678056 turbinia-20240412.1/turbinia/config/recipes/triage-windows.yaml
+-rw-r--r--   0        0        0      114 2024-04-24 20:07:16.678056 turbinia-20240412.1/turbinia/config/recipes/triage.yaml
+-rw-r--r--   0        0        0      475 2024-04-24 20:07:16.678056 turbinia-20240412.1/turbinia/config/rules/pgsql_from_program.yar
+-rw-r--r--   0        0        0      521 2024-04-24 20:07:16.678056 turbinia-20240412.1/turbinia/config/rules/redis_replicaof.yar
+-rw-r--r--   0        0        0      671 2024-04-24 20:07:16.678056 turbinia-20240412.1/turbinia/config/rules/suspicious_cron.yar
+-rw-r--r--   0        0        0      349 2024-04-24 20:07:16.678056 turbinia-20240412.1/turbinia/config/rules/suspicious_gitlab.yar
+-rw-r--r--   0        0        0      290 2024-04-24 20:07:16.678056 turbinia-20240412.1/turbinia/config/rules/suspicious_hadoop.yar
+-rw-r--r--   0        0        0     6889 2024-04-24 20:07:16.678056 turbinia-20240412.1/turbinia/config/turbinia_config_test.py
+-rw-r--r--   0        0        0    14077 2024-04-24 20:07:16.678056 turbinia-20240412.1/turbinia/config/turbinia_config_tmpl.py
+-rwxr-xr-x   0        0        0     3766 2024-04-24 20:07:16.678056 turbinia-20240412.1/turbinia/e2e/e2e-local.sh
+-rw-r--r--   0        0        0      122 2024-04-24 20:07:16.678056 turbinia-20240412.1/turbinia/e2e/e2e-recipe.yaml
+-rw-r--r--   0        0        0     5012 2024-04-24 20:07:16.678056 turbinia-20240412.1/turbinia/e2e/run-e2e-gke.sh
+-rw-r--r--   0        0        0    50691 2024-04-24 20:07:16.678056 turbinia-20240412.1/turbinia/evidence.py
+-rw-r--r--   0        0        0     4482 2024-04-24 20:07:16.678056 turbinia-20240412.1/turbinia/evidence_test.py
+-rw-r--r--   0        0        0     1504 2024-04-24 20:07:16.678056 turbinia-20240412.1/turbinia/job_utils.py
+-rw-r--r--   0        0        0     1728 2024-04-24 20:07:16.678056 turbinia-20240412.1/turbinia/jobs/__init__.py
+-rw-r--r--   0        0        0     1730 2024-04-24 20:07:16.678056 turbinia-20240412.1/turbinia/jobs/binary_extractor.py
+-rw-r--r--   0        0        0     1929 2024-04-24 20:07:16.678056 turbinia-20240412.1/turbinia/jobs/bulk_extractor.py
+-rw-r--r--   0        0        0     1500 2024-04-24 20:07:16.678056 turbinia-20240412.1/turbinia/jobs/containerd.py
+-rw-r--r--   0        0        0     1554 2024-04-24 20:07:16.678056 turbinia-20240412.1/turbinia/jobs/dfdewey.py
+-rw-r--r--   0        0        0     1586 2024-04-24 20:07:16.678056 turbinia-20240412.1/turbinia/jobs/docker.py
+-rw-r--r--   0        0        0     1776 2024-04-24 20:07:16.678056 turbinia-20240412.1/turbinia/jobs/file_system_timeline.py
+-rw-r--r--   0        0        0     1665 2024-04-24 20:07:16.678056 turbinia-20240412.1/turbinia/jobs/finalize_request.py
+-rw-r--r--   0        0        0     1277 2024-04-24 20:07:16.678056 turbinia-20240412.1/turbinia/jobs/fsstat.py
+-rw-r--r--   0        0        0     1454 2024-04-24 20:07:16.678056 turbinia-20240412.1/turbinia/jobs/grep.py
+-rw-r--r--   0        0        0     1438 2024-04-24 20:07:16.678056 turbinia-20240412.1/turbinia/jobs/hindsight.py
+-rw-r--r--   0        0        0     2700 2024-04-24 20:07:16.678056 turbinia-20240412.1/turbinia/jobs/http_access_logs.py
+-rw-r--r--   0        0        0     2306 2024-04-24 20:07:16.678056 turbinia-20240412.1/turbinia/jobs/imports_test.py
+-rw-r--r--   0        0        0     3640 2024-04-24 20:07:16.678056 turbinia-20240412.1/turbinia/jobs/interface.py
+-rw-r--r--   0        0        0     1914 2024-04-24 20:07:16.678056 turbinia-20240412.1/turbinia/jobs/interface_test.py
+-rw-r--r--   0        0        0     1801 2024-04-24 20:07:16.678056 turbinia-20240412.1/turbinia/jobs/jenkins.py
+-rw-r--r--   0        0        0     2615 2024-04-24 20:07:16.678056 turbinia-20240412.1/turbinia/jobs/jupyter.py
+-rw-r--r--   0        0        0     1827 2024-04-24 20:07:16.678056 turbinia-20240412.1/turbinia/jobs/linux_acct.py
+-rw-r--r--   0        0        0     4534 2024-04-24 20:07:16.678056 turbinia-20240412.1/turbinia/jobs/llm_artifacts_analyzer.py
+-rw-r--r--   0        0        0     8630 2024-04-24 20:07:16.678056 turbinia-20240412.1/turbinia/jobs/manager.py
+-rw-r--r--   0        0        0     5185 2024-04-24 20:07:16.678056 turbinia-20240412.1/turbinia/jobs/manager_test.py
+-rw-r--r--   0        0        0     1735 2024-04-24 20:07:16.678056 turbinia-20240412.1/turbinia/jobs/partitions.py
+-rw-r--r--   0        0        0     1304 2024-04-24 20:07:16.678056 turbinia-20240412.1/turbinia/jobs/photorec.py
+-rw-r--r--   0        0        0     2210 2024-04-24 20:07:16.678056 turbinia-20240412.1/turbinia/jobs/plaso.py
+-rw-r--r--   0        0        0     1668 2024-04-24 20:07:16.678056 turbinia-20240412.1/turbinia/jobs/postgres_acct.py
+-rw-r--r--   0        0        0     1379 2024-04-24 20:07:16.678056 turbinia-20240412.1/turbinia/jobs/psort.py
+-rw-r--r--   0        0        0     2571 2024-04-24 20:07:16.678056 turbinia-20240412.1/turbinia/jobs/redis.py
+-rw-r--r--   0        0        0     1832 2024-04-24 20:07:16.678056 turbinia-20240412.1/turbinia/jobs/ssh_analyzer.py
+-rw-r--r--   0        0        0     2562 2024-04-24 20:07:16.678056 turbinia-20240412.1/turbinia/jobs/sshd.py
+-rw-r--r--   0        0        0     1672 2024-04-24 20:07:16.682056 turbinia-20240412.1/turbinia/jobs/strings.py
+-rw-r--r--   0        0        0     2563 2024-04-24 20:07:16.682056 turbinia-20240412.1/turbinia/jobs/tomcat.py
+-rw-r--r--   0        0        0     1554 2024-04-24 20:07:16.682056 turbinia-20240412.1/turbinia/jobs/volatility.py
+-rw-r--r--   0        0        0     1844 2024-04-24 20:07:16.682056 turbinia-20240412.1/turbinia/jobs/windows_acct.py
+-rw-r--r--   0        0        0     1855 2024-04-24 20:07:16.682056 turbinia-20240412.1/turbinia/jobs/wordpress_creds.py
+-rw-r--r--   0        0        0     1465 2024-04-24 20:07:16.682056 turbinia-20240412.1/turbinia/jobs/worker_stat.py
+-rw-r--r--   0        0        0     1587 2024-04-24 20:07:16.682056 turbinia-20240412.1/turbinia/jobs/yara.py
+-rw-r--r--   0        0        0        0 2024-04-24 20:07:16.682056 turbinia-20240412.1/turbinia/lib/__init__.py
+-rw-r--r--   0        0        0     9646 2024-04-24 20:07:16.682056 turbinia-20240412.1/turbinia/lib/docker_manager.py
+-rw-r--r--   0        0        0     8382 2024-04-24 20:07:16.682056 turbinia-20240412.1/turbinia/lib/dockermanager_test.py
+-rw-r--r--   0        0        0     2863 2024-04-24 20:07:16.682056 turbinia-20240412.1/turbinia/lib/file_helpers.py
+-rw-r--r--   0        0        0     2470 2024-04-24 20:07:16.682056 turbinia-20240412.1/turbinia/lib/google_cloud.py
+-rw-r--r--   0        0        0     1290 2024-04-24 20:07:16.682056 turbinia-20240412.1/turbinia/lib/google_cloud_test.py
+-rw-r--r--   0        0        0        0 2024-04-24 20:07:16.682056 turbinia-20240412.1/turbinia/lib/llm_libs/__init__.py
+-rw-r--r--   0        0        0      782 2024-04-24 20:07:16.682056 turbinia-20240412.1/turbinia/lib/llm_libs/llm_client.py
+-rw-r--r--   0        0        0      678 2024-04-24 20:07:16.682056 turbinia-20240412.1/turbinia/lib/llm_libs/llm_lib_base.py
+-rw-r--r--   0        0        0     4392 2024-04-24 20:07:16.682056 turbinia-20240412.1/turbinia/lib/llm_libs/vertex_ai_lib.py
+-rw-r--r--   0        0        0     1462 2024-04-24 20:07:16.682056 turbinia-20240412.1/turbinia/lib/llm_libs/vertex_ai_lib_test.py
+-rw-r--r--   0        0        0     7263 2024-04-24 20:07:16.682056 turbinia-20240412.1/turbinia/lib/recipe_helpers.py
+-rw-r--r--   0        0        0     7341 2024-04-24 20:07:16.682056 turbinia-20240412.1/turbinia/lib/recipe_helpers_test.py
+-rw-r--r--   0        0        0     2300 2024-04-24 20:07:16.682056 turbinia-20240412.1/turbinia/lib/text_formatter.py
+-rw-r--r--   0        0        0     1551 2024-04-24 20:07:16.682056 turbinia-20240412.1/turbinia/lib/text_formatter_test.py
+-rw-r--r--   0        0        0     8371 2024-04-24 20:07:16.682056 turbinia-20240412.1/turbinia/lib/utils.py
+-rw-r--r--   0        0        0     4852 2024-04-24 20:07:16.682056 turbinia-20240412.1/turbinia/message.py
+-rw-r--r--   0        0        0     2673 2024-04-24 20:07:16.682056 turbinia-20240412.1/turbinia/notify.py
+-rw-r--r--   0        0        0     4039 2024-04-24 20:07:16.682056 turbinia-20240412.1/turbinia/notify_test.py
+-rw-r--r--   0        0        0    18091 2024-04-24 20:07:16.682056 turbinia-20240412.1/turbinia/output_manager.py
+-rw-r--r--   0        0        0     9307 2024-04-24 20:07:16.682056 turbinia-20240412.1/turbinia/output_manager_test.py
+-rw-r--r--   0        0        0        0 2024-04-24 20:07:16.682056 turbinia-20240412.1/turbinia/processors/__init__.py
+-rw-r--r--   0        0        0     4290 2024-04-24 20:07:16.682056 turbinia-20240412.1/turbinia/processors/archive.py
+-rw-r--r--   0        0        0     3001 2024-04-24 20:07:16.682056 turbinia-20240412.1/turbinia/processors/archive_test.py
+-rw-r--r--   0        0        0     3098 2024-04-24 20:07:16.682056 turbinia-20240412.1/turbinia/processors/containerd.py
+-rw-r--r--   0        0        0     3043 2024-04-24 20:07:16.682056 turbinia-20240412.1/turbinia/processors/docker.py
+-rw-r--r--   0        0        0     5317 2024-04-24 20:07:16.682056 turbinia-20240412.1/turbinia/processors/google_cloud.py
+-rw-r--r--   0        0        0    21984 2024-04-24 20:07:16.682056 turbinia-20240412.1/turbinia/processors/mount_local.py
+-rw-r--r--   0        0        0    21404 2024-04-24 20:07:16.682056 turbinia-20240412.1/turbinia/processors/mount_local_test.py
+-rw-r--r--   0        0        0     2936 2024-04-24 20:07:16.682056 turbinia-20240412.1/turbinia/processors/partitions.py
+-rw-r--r--   0        0        0     4175 2024-04-24 20:07:16.682056 turbinia-20240412.1/turbinia/processors/partitions_test.py
+-rw-r--r--   0        0        0     5017 2024-04-24 20:07:16.682056 turbinia-20240412.1/turbinia/processors/resource_manager.py
+-rw-r--r--   0        0        0     4828 2024-04-24 20:07:16.682056 turbinia-20240412.1/turbinia/processors/resource_manager_test.py
+-rw-r--r--   0        0        0     2116 2024-04-24 20:07:16.682056 turbinia-20240412.1/turbinia/server.py
+-rw-r--r--   0        0        0     1973 2024-04-24 20:07:16.682056 turbinia-20240412.1/turbinia/server_test.py
+-rw-r--r--   0        0        0    19140 2024-04-24 20:07:16.682056 turbinia-20240412.1/turbinia/state_manager.py
+-rw-r--r--   0        0        0     8222 2024-04-24 20:07:16.682056 turbinia-20240412.1/turbinia/state_manager_test.py
+-rw-r--r--   0        0        0    26606 2024-04-24 20:07:16.682056 turbinia-20240412.1/turbinia/task_manager.py
+-rw-r--r--   0        0        0    13214 2024-04-24 20:07:16.682056 turbinia-20240412.1/turbinia/task_manager_test.py
+-rw-r--r--   0        0        0     7136 2024-04-24 20:07:16.682056 turbinia-20240412.1/turbinia/task_utils.py
+-rw-r--r--   0        0        0     2579 2024-04-24 20:07:16.682056 turbinia-20240412.1/turbinia/task_utils_test.py
+-rw-r--r--   0        0        0     3443 2024-04-24 20:07:16.682056 turbinia-20240412.1/turbinia/tcelery.py
+-rw-r--r--   0        0        0     7520 2024-04-24 20:07:16.682056 turbinia-20240412.1/turbinia/turbiniactl.py
+-rw-r--r--   0        0        0     3270 2024-04-24 20:07:16.682056 turbinia-20240412.1/turbinia/turbiniactl_test.py
+-rw-r--r--   0        0        0     9081 2024-04-24 20:07:16.682056 turbinia-20240412.1/turbinia/worker.py
+-rw-r--r--   0        0        0     7357 2024-04-24 20:07:16.682056 turbinia-20240412.1/turbinia/worker_test.py
+-rw-r--r--   0        0        0    43289 2024-04-24 20:07:16.682056 turbinia-20240412.1/turbinia/workers/__init__.py
+-rw-r--r--   0        0        0      771 2024-04-24 20:07:16.682056 turbinia-20240412.1/turbinia/workers/abort.py
+-rw-r--r--   0        0        0        0 2024-04-24 20:07:16.682056 turbinia-20240412.1/turbinia/workers/analysis/__init__.py
+-rw-r--r--   0        0        0     2999 2024-04-24 20:07:16.682056 turbinia-20240412.1/turbinia/workers/analysis/analyzer_output.py
+-rw-r--r--   0        0        0    28182 2024-04-24 20:07:16.682056 turbinia-20240412.1/turbinia/workers/analysis/auth.py
+-rw-r--r--   0        0        0    21225 2024-04-24 20:07:16.682056 turbinia-20240412.1/turbinia/workers/analysis/auth_test.py
+-rw-r--r--   0        0        0     7038 2024-04-24 20:07:16.682056 turbinia-20240412.1/turbinia/workers/analysis/jenkins.py
+-rw-r--r--   0        0        0     6527 2024-04-24 20:07:16.682056 turbinia-20240412.1/turbinia/workers/analysis/jenkins_test.py
+-rw-r--r--   0        0        0     4446 2024-04-24 20:07:16.682056 turbinia-20240412.1/turbinia/workers/analysis/jupyter.py
+-rw-r--r--   0        0        0     2343 2024-04-24 20:07:16.682056 turbinia-20240412.1/turbinia/workers/analysis/jupyter_test.py
+-rw-r--r--   0        0        0     5175 2024-04-24 20:07:16.682056 turbinia-20240412.1/turbinia/workers/analysis/linux_acct.py
+-rw-r--r--   0        0        0     3301 2024-04-24 20:07:16.682056 turbinia-20240412.1/turbinia/workers/analysis/linux_acct_test.py
+-rw-r--r--   0        0        0     9174 2024-04-24 20:07:16.682056 turbinia-20240412.1/turbinia/workers/analysis/llm_analyzer.py
+-rw-r--r--   0        0        0     3352 2024-04-24 20:07:16.682056 turbinia-20240412.1/turbinia/workers/analysis/llm_analyzer_test.py
+-rw-r--r--   0        0        0     9655 2024-04-24 20:07:16.686056 turbinia-20240412.1/turbinia/workers/analysis/postgresql_acct.py
+-rw-r--r--   0        0        0     4113 2024-04-24 20:07:16.686056 turbinia-20240412.1/turbinia/workers/analysis/postgresql_acct_test.py
+-rw-r--r--   0        0        0     3270 2024-04-24 20:07:16.686056 turbinia-20240412.1/turbinia/workers/analysis/redis.py
+-rw-r--r--   0        0        0     1912 2024-04-24 20:07:16.686056 turbinia-20240412.1/turbinia/workers/analysis/redis_test.py
+-rw-r--r--   0        0        0    18019 2024-04-24 20:07:16.686056 turbinia-20240412.1/turbinia/workers/analysis/ssh_analyzer.py
+-rw-r--r--   0        0        0     5147 2024-04-24 20:07:16.686056 turbinia-20240412.1/turbinia/workers/analysis/ssh_analyzer_test.py
+-rw-r--r--   0        0        0     3770 2024-04-24 20:07:16.686056 turbinia-20240412.1/turbinia/workers/analysis/sshd.py
+-rw-r--r--   0        0        0     1984 2024-04-24 20:07:16.686056 turbinia-20240412.1/turbinia/workers/analysis/sshd_test.py
+-rw-r--r--   0        0        0     3968 2024-04-24 20:07:16.686056 turbinia-20240412.1/turbinia/workers/analysis/tomcat.py
+-rw-r--r--   0        0        0     3928 2024-04-24 20:07:16.686056 turbinia-20240412.1/turbinia/workers/analysis/tomcat_test.py
+-rw-r--r--   0        0        0     9398 2024-04-24 20:07:16.686056 turbinia-20240412.1/turbinia/workers/analysis/windows_acct.py
+-rw-r--r--   0        0        0     2992 2024-04-24 20:07:16.686056 turbinia-20240412.1/turbinia/workers/analysis/windows_acct_test.py
+-rw-r--r--   0        0        0     4522 2024-04-24 20:07:16.686056 turbinia-20240412.1/turbinia/workers/analysis/wordpress_access.py
+-rw-r--r--   0        0        0     2003 2024-04-24 20:07:16.686056 turbinia-20240412.1/turbinia/workers/analysis/wordpress_access_test.py
+-rw-r--r--   0        0        0     7245 2024-04-24 20:07:16.686056 turbinia-20240412.1/turbinia/workers/analysis/wordpress_creds.py
+-rw-r--r--   0        0        0     2750 2024-04-24 20:07:16.686056 turbinia-20240412.1/turbinia/workers/analysis/wordpress_creds_test.py
+-rw-r--r--   0        0        0     5325 2024-04-24 20:07:16.686056 turbinia-20240412.1/turbinia/workers/analysis/yara.py
+-rw-r--r--   0        0        0     2670 2024-04-24 20:07:16.686056 turbinia-20240412.1/turbinia/workers/analysis/yara_test.py
+-rw-r--r--   0        0        0     6455 2024-04-24 20:07:16.686056 turbinia-20240412.1/turbinia/workers/artifact.py
+-rw-r--r--   0        0        0     5824 2024-04-24 20:07:16.686056 turbinia-20240412.1/turbinia/workers/binary_extractor.py
+-rw-r--r--   0        0        0     3572 2024-04-24 20:07:16.686056 turbinia-20240412.1/turbinia/workers/binary_extractor_test.py
+-rw-r--r--   0        0        0     8309 2024-04-24 20:07:16.686056 turbinia-20240412.1/turbinia/workers/bulk_extractor.py
+-rw-r--r--   0        0        0     3299 2024-04-24 20:07:16.686056 turbinia-20240412.1/turbinia/workers/bulk_extractor_test.py
+-rw-r--r--   0        0        0    10650 2024-04-24 20:07:16.686056 turbinia-20240412.1/turbinia/workers/containerd.py
+-rw-r--r--   0        0        0     2373 2024-04-24 20:07:16.686056 turbinia-20240412.1/turbinia/workers/containerd_test.py
+-rw-r--r--   0        0        0     3208 2024-04-24 20:07:16.686056 turbinia-20240412.1/turbinia/workers/dfdewey.py
+-rw-r--r--   0        0        0     2490 2024-04-24 20:07:16.686056 turbinia-20240412.1/turbinia/workers/dfdewey_test.py
+-rw-r--r--   0        0        0     4332 2024-04-24 20:07:16.686056 turbinia-20240412.1/turbinia/workers/docker.py
+-rw-r--r--   0        0        0     2355 2024-04-24 20:07:16.686056 turbinia-20240412.1/turbinia/workers/docker_test.py
+-rw-r--r--   0        0        0     5146 2024-04-24 20:07:16.686056 turbinia-20240412.1/turbinia/workers/file_system_timeline.py
+-rw-r--r--   0        0        0     3159 2024-04-24 20:07:16.686056 turbinia-20240412.1/turbinia/workers/file_system_timeline_test.py
+-rw-r--r--   0        0        0     2045 2024-04-24 20:07:16.686056 turbinia-20240412.1/turbinia/workers/finalize_request.py
+-rw-r--r--   0        0        0     2148 2024-04-24 20:07:16.686056 turbinia-20240412.1/turbinia/workers/fsstat.py
+-rw-r--r--   0        0        0     2648 2024-04-24 20:07:16.686056 turbinia-20240412.1/turbinia/workers/fsstat_test.py
+-rw-r--r--   0        0        0     2493 2024-04-24 20:07:16.686056 turbinia-20240412.1/turbinia/workers/grep.py
+-rw-r--r--   0        0        0     1969 2024-04-24 20:07:16.686056 turbinia-20240412.1/turbinia/workers/hindsight.py
+-rw-r--r--   0        0        0    10477 2024-04-24 20:07:16.686056 turbinia-20240412.1/turbinia/workers/partitions.py
+-rw-r--r--   0        0        0    10303 2024-04-24 20:07:16.686056 turbinia-20240412.1/turbinia/workers/partitions_test.py
+-rw-r--r--   0        0        0     2873 2024-04-24 20:07:16.686056 turbinia-20240412.1/turbinia/workers/photorec.py
+-rw-r--r--   0        0        0     1694 2024-04-24 20:07:16.686056 turbinia-20240412.1/turbinia/workers/photorec_test.py
+-rw-r--r--   0        0        0     6031 2024-04-24 20:07:16.686056 turbinia-20240412.1/turbinia/workers/plaso.py
+-rw-r--r--   0        0        0     2518 2024-04-24 20:07:16.686056 turbinia-20240412.1/turbinia/workers/plaso_test.py
+-rw-r--r--   0        0        0     2882 2024-04-24 20:07:16.686056 turbinia-20240412.1/turbinia/workers/psort.py
+-rw-r--r--   0        0        0     3034 2024-04-24 20:07:16.686056 turbinia-20240412.1/turbinia/workers/strings.py
+-rw-r--r--   0        0        0     3652 2024-04-24 20:07:16.686056 turbinia-20240412.1/turbinia/workers/volatility.py
+-rw-r--r--   0        0        0     2971 2024-04-24 20:07:16.686056 turbinia-20240412.1/turbinia/workers/volatility_test.py
+-rw-r--r--   0        0        0     1718 2024-04-24 20:07:16.686056 turbinia-20240412.1/turbinia/workers/worker_stat.py
+-rw-r--r--   0        0        0    18072 2024-04-24 20:07:16.686056 turbinia-20240412.1/turbinia/workers/workers_test.py
+-rw-r--r--   0        0        0     1063 2024-04-24 20:07:16.686056 turbinia-20240412.1/turbinia/yapf_test.py
+-rw-r--r--   0        0        0     8497 1970-01-01 00:00:00.000000 turbinia-20240412.1/PKG-INFO
```

### Comparing `turbinia-20240313/LICENSE` & `turbinia-20240412.1/LICENSE`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/README.md` & `turbinia-20240412.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # Turbinia
+![Unit tests](https://github.com/google/turbinia/actions/workflows/actions.yml/badge.svg) ![e2e tests](https://github.com/google/turbinia/actions/workflows/e2e.yml/badge.svg)
 
 ## Summary
 
 Turbinia is an open-source framework for deploying, managing, and running
 distributed forensic workloads. It is intended to automate running of common
 forensic processing tools (i.e. Plaso, TSK, strings, etc) to help with
 processing evidence in the Cloud, scaling the processing of large amounts of
```

### Comparing `turbinia-20240313/pyproject.toml` & `turbinia-20240412.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "turbinia"
-version = "20240313"
+version = "20240412.1"
 description = "Automation and Scaling of Digital Forensics Tools"
 authors = ["Turbinia Developers <turbinia-dev@googlegroups.com>"]
 maintainers = ["Turbinia Developers <turbinia-dev@googlegroups.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/google/turbinia"
 documentation = "https://turbinia.readthedocs.io/en/latest/"
@@ -12,22 +12,23 @@
 [tool.poetry.scripts]
 turbiniactl = "turbinia.turbiniactl:main"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 backoff = { version = ">=2.2.1" }
 celery = { version = "^5.2.2" }
-dfDewey = { version = "^20220603", optional = true }
-dfimagetools = { version = "^20230806", optional = true }
+dfDewey = { version = "^20231016", optional = true }
+dfimagetools = { version = "^20240301", optional = true }
 docker = { version = "^6.1.3" }
 fastapi = {extras = ["all"], version = ">=0.75.0,<0.99.0"}
 filelock = { version = "*" }
 google-api-core = { version = "<3.0.0", optional = true }
 google-generativeai = { version = ">=0.3.2" }
-libcloudforensics = { version = "20240214" }
+libcloudforensics = "^20240325"
+opensearch-py = {version = "2.4.2"}
 pandas = { version = "^2.1.0" }
 plaso = { version = "20240308", optional = true }
 prometheus_client = { version = "^0.17.1" }
 protobuf = { version = ">=3.19.0", optional = true }
 pydantic = { version = "^1.10.5,<2"}
 pyglove = { version = ">=0.4.4" }
 pyhindsight = { version = "^20230327.0", optional = true }
@@ -43,21 +44,27 @@
 
 [tool.poetry.group.test.dependencies]
 coverage = "*"
 fakeredis = "^1.8.1"
 google-auth-oauthlib = "^1.1.0"
 mock = "*"
 pytest = "*"
+tabulate = "*"
 turbinia-api-lib = "^1.0.2"
 yapf = "*"
 
 [tool.poetry.extras]
 worker = [
   "dfimagetools",
   "dfDewey",
   "plaso",
   "pyhindsight",
 ]
 
+[tool.yapfignore]
+ignore_patterns = [
+  "turbinia/api/client/**/*.py",
+]
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `turbinia-20240313/turbinia/__init__.py` & `turbinia-20240412.1/turbinia/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # limitations under the License.
 """Main Turbinia application."""
 
 import logging
 
 from importlib import metadata as importlib_metadata
 
-log = logging.getLogger('turbinia')
+log = logging.getLogger(__name__)
 
 try:
   dist = importlib_metadata.distribution(__name__)
   __version__ = dist.version
 except importlib_metadata.PackageNotFoundError:
   __version__ = 'unknown'
```

### Comparing `turbinia-20240313/turbinia/api/__init__.py` & `turbinia-20240412.1/turbinia/api/__init__.py`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/api/api_server.py` & `turbinia-20240412.1/turbinia/api/api_server.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,18 +24,16 @@
 from fastapi.middleware.cors import CORSMiddleware
 from fastapi.routing import APIRoute
 
 from turbinia import config
 from turbinia.api.routes.router import api_router
 from turbinia.api.routes.ui import ui_router
 
-from turbinia.config import logger
-
-logger.setup()
 log = logging.getLogger('turbinia')
+log.setLevel(logging.INFO)
 
 
 def get_application() -> FastAPI:
   """Returns a FastAPI application object."""
   description: str = (
       'Turbinia is an open-source framework for deploying,'
       ' managing, and running distributed forensic workloads')
@@ -60,16 +58,16 @@
 
 app = get_application()
 
 app.add_middleware(
     CORSMiddleware,
     allow_origins=config.API_ALLOWED_ORIGINS,
     allow_credentials=False,
-    allow_methods=["*"],
-    allow_headers=["*"],
+    allow_methods=['GET', 'POST'],
+    allow_headers=['*'],
 )
 
 app.include_router(api_router)
 app.include_router(ui_router)
 
 set_operation_ids(app)
 
@@ -93,16 +91,15 @@
   def start(self, app_name: str):
     """Runs the Turbinia API server
 
     Args:
       app_name (str): module:app string used by Uvicorn
           to start the HTTP server.
     """
-    _config: config = config.LoadConfig()
     uvicorn.run(
-        app_name, host=_config.API_SERVER_ADDRESS, port=_config.API_SERVER_PORT,
-        log_level="info", reload=False, workers=4)
+        app_name, host=config.API_SERVER_ADDRESS, port=config.API_SERVER_PORT,
+        log_config=None, log_level='info', reload=False, workers=4)
 
 
 if __name__ == '__main__':
   api_server = TurbiniaAPIServer(app=app)
   api_server.start('api_server:app')
```

### Comparing `turbinia-20240313/turbinia/api/api_server_test.py` & `turbinia-20240412.1/turbinia/api/api_server_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -409,28 +409,28 @@
   @mock.patch('turbinia.api.routes.evidence.os.makedirs')
   def testEvidenceUpload(
       self, mock_makedirs, mock_datetime, mock_get_attribute):
     """Tests uploading evidence."""
     mocked_now = datetime.datetime.now()
     mock_datetime.now.return_value = mocked_now
     mocked_now_str = mocked_now.strftime(turbinia_config.DATETIME_FORMAT)
-
+    self.maxDiff = None
     filedir = os.path.dirname(os.path.realpath(__file__))
     evidence_1_name = 'wordpress_access_logs.txt'
     evidence_2_name = 'mbr.raw'
     evidence_1_path = os.path.join(
         filedir, '..', '..', 'test_data', evidence_1_name)
     evidence_2_path = os.path.join(
         filedir, '..', '..', 'test_data', evidence_2_name)
     ticket_id = '981234098'
 
     expected_evidence_1_name = (
-        f'{os.path.splitext(evidence_1_name)[0]}_{mocked_now_str}')
+        f'{os.path.splitext(evidence_1_name)[0]}_{mocked_now_str}') + '.txt'
     expected_evidence_2_name = (
-        f'{os.path.splitext(evidence_2_name)[0]}_{mocked_now_str}')
+        f'{os.path.splitext(evidence_2_name)[0]}_{mocked_now_str}') + '.raw'
     expected_evidence_1_path = os.path.join(
         turbinia_config.API_EVIDENCE_UPLOAD_DIR, ticket_id,
         expected_evidence_1_name)
     expected_evidence_2_path = os.path.join(
         turbinia_config.API_EVIDENCE_UPLOAD_DIR, ticket_id,
         expected_evidence_2_name)
     expected_response = [{
```

### Comparing `turbinia-20240313/turbinia/api/cli/.turbinia_api_config.json` & `turbinia-20240412.1/turbinia/api/cli/.turbinia_api_config.json`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/api/cli/LICENSE` & `turbinia-20240412.1/turbinia/api/cli/LICENSE`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/api/cli/README.rst` & `turbinia-20240412.1/turbinia/api/cli/README.rst`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/api/cli/poetry.lock` & `turbinia-20240412.1/turbinia/api/cli/poetry.lock`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file is automatically @generated by Poetry 1.7.0 and should not be changed by hand.
+# This file is automatically @generated by Poetry 1.8.2 and should not be changed by hand.
 
 [[package]]
 name = "aenum"
 version = "3.1.15"
 description = "Advanced Enumerations (compatible with Python's stdlib Enum), NamedTuples, and NamedConstants"
 optional = false
 python-versions = "*"
@@ -10,32 +10,32 @@
     {file = "aenum-3.1.15-py2-none-any.whl", hash = "sha256:27b1710b9d084de6e2e695dab78fe9f269de924b51ae2850170ee7e1ca6288a5"},
     {file = "aenum-3.1.15-py3-none-any.whl", hash = "sha256:e0dfaeea4c2bd362144b87377e2c61d91958c5ed0b4daf89cb6f45ae23af6288"},
     {file = "aenum-3.1.15.tar.gz", hash = "sha256:8cbd76cd18c4f870ff39b24284d3ea028fbe8731a58df3aa581e434c575b9559"},
 ]
 
 [[package]]
 name = "cachetools"
-version = "5.3.2"
+version = "5.3.3"
 description = "Extensible memoizing collections and decorators"
 optional = false
 python-versions = ">=3.7"
 files = [
-    {file = "cachetools-5.3.2-py3-none-any.whl", hash = "sha256:861f35a13a451f94e301ce2bec7cac63e881232ccce7ed67fab9b5df4d3beaa1"},
-    {file = "cachetools-5.3.2.tar.gz", hash = "sha256:086ee420196f7b2ab9ca2db2520aca326318b68fe5ba8bc4d49cca91add450f2"},
+    {file = "cachetools-5.3.3-py3-none-any.whl", hash = "sha256:0abad1021d3f8325b2fc1d2e9c8b9c9d57b04c3932657a72465447332c24d945"},
+    {file = "cachetools-5.3.3.tar.gz", hash = "sha256:ba29e2dfa0b8b556606f097407ed1aa62080ee108ab0dc5ec9d6a723a007d105"},
 ]
 
 [[package]]
 name = "certifi"
-version = "2023.7.22"
+version = "2024.2.2"
 description = "Python package for providing Mozilla's CA Bundle."
 optional = false
 python-versions = ">=3.6"
 files = [
-    {file = "certifi-2023.7.22-py3-none-any.whl", hash = "sha256:92d6037539857d8206b8f6ae472e8b77db8058fec5937a1ef3f54304089edbb9"},
-    {file = "certifi-2023.7.22.tar.gz", hash = "sha256:539cc1d13202e33ca466e88b2807e29f4c13049d6d87031a3c110744495cb082"},
+    {file = "certifi-2024.2.2-py3-none-any.whl", hash = "sha256:dc383c07b76109f368f6106eee2b593b04a011ea4d55f652c6ca24a754d1cdd1"},
+    {file = "certifi-2024.2.2.tar.gz", hash = "sha256:0569859f95fc761b18b45ef421b1290a0f65f147e92a1e5eb3e635f9a5e4e66f"},
 ]
 
 [[package]]
 name = "charset-normalizer"
 version = "3.3.2"
 description = "The Real First Universal Charset Detector. Open, modern and actively maintained alternative to Chardet."
 optional = false
@@ -156,21 +156,21 @@
 files = [
     {file = "colorama-0.4.6-py2.py3-none-any.whl", hash = "sha256:4f1d9991f5acc0ca119f9d443620b77f9d6b33703e51011c16baf57afb285fc6"},
     {file = "colorama-0.4.6.tar.gz", hash = "sha256:08695f5cb7ed6e0531a20572697297273c47b8cae5a63ffc6d6ed5c201be6e44"},
 ]
 
 [[package]]
 name = "google-auth"
-version = "2.23.4"
+version = "2.29.0"
 description = "Google Authentication Library"
 optional = false
 python-versions = ">=3.7"
 files = [
-    {file = "google-auth-2.23.4.tar.gz", hash = "sha256:79905d6b1652187def79d491d6e23d0cbb3a21d3c7ba0dbaa9c8a01906b13ff3"},
-    {file = "google_auth-2.23.4-py2.py3-none-any.whl", hash = "sha256:d4bbc92fe4b8bfd2f3e8d88e5ba7085935da208ee38a134fc280e7ce682a05f2"},
+    {file = "google-auth-2.29.0.tar.gz", hash = "sha256:672dff332d073227550ffc7457868ac4218d6c500b155fe6cc17d2b13602c360"},
+    {file = "google_auth-2.29.0-py2.py3-none-any.whl", hash = "sha256:d452ad095688cd52bae0ad6fafe027f6a6d6f560e810fec20914e17a09526415"},
 ]
 
 [package.dependencies]
 cachetools = ">=2.0.0,<6.0"
 pyasn1-modules = ">=0.2.1"
 rsa = ">=3.1.4,<5"
 
@@ -179,114 +179,84 @@
 enterprise-cert = ["cryptography (==36.0.2)", "pyopenssl (==22.0.0)"]
 pyopenssl = ["cryptography (>=38.0.3)", "pyopenssl (>=20.0.0)"]
 reauth = ["pyu2f (>=0.1.5)"]
 requests = ["requests (>=2.20.0,<3.0.0.dev0)"]
 
 [[package]]
 name = "google-auth-oauthlib"
-version = "1.1.0"
+version = "1.2.0"
 description = "Google Authentication Library"
 optional = false
 python-versions = ">=3.6"
 files = [
-    {file = "google-auth-oauthlib-1.1.0.tar.gz", hash = "sha256:83ea8c3b0881e453790baff4448e8a6112ac8778d1de9da0b68010b843937afb"},
-    {file = "google_auth_oauthlib-1.1.0-py2.py3-none-any.whl", hash = "sha256:089c6e587d36f4803ac7e0720c045c6a8b1fd1790088b8424975b90d0ee61c12"},
+    {file = "google-auth-oauthlib-1.2.0.tar.gz", hash = "sha256:292d2d3783349f2b0734a0a0207b1e1e322ac193c2c09d8f7c613fb7cc501ea8"},
+    {file = "google_auth_oauthlib-1.2.0-py2.py3-none-any.whl", hash = "sha256:297c1ce4cb13a99b5834c74a1fe03252e1e499716718b190f56bcb9c4abc4faf"},
 ]
 
 [package.dependencies]
 google-auth = ">=2.15.0"
 requests-oauthlib = ">=0.7.0"
 
 [package.extras]
 tool = ["click (>=6.0.0)"]
 
 [[package]]
 name = "idna"
-version = "3.4"
+version = "3.7"
 description = "Internationalized Domain Names in Applications (IDNA)"
 optional = false
 python-versions = ">=3.5"
 files = [
-    {file = "idna-3.4-py3-none-any.whl", hash = "sha256:90b77e79eaa3eba6de819a0c442c0b4ceefc341a7a2ab77d7562bf49f425c5c2"},
-    {file = "idna-3.4.tar.gz", hash = "sha256:814f528e8dead7d329833b91c5faa87d60bf71824cd12a7530b5526063d02cb4"},
+    {file = "idna-3.7-py3-none-any.whl", hash = "sha256:82fee1fc78add43492d3a1898bfa6d8a904cc97d8427f683ed8e798d07761aa0"},
+    {file = "idna-3.7.tar.gz", hash = "sha256:028ff3aadf0609c1fd278d8ea3089299412a7a8b9bd005dd08b9f8285bcb5cfc"},
 ]
 
 [[package]]
 name = "numpy"
-version = "1.25.2"
+version = "1.26.4"
 description = "Fundamental package for array computing in Python"
 optional = false
 python-versions = ">=3.9"
 files = [
-    {file = "numpy-1.25.2-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:db3ccc4e37a6873045580d413fe79b68e47a681af8db2e046f1dacfa11f86eb3"},
-    {file = "numpy-1.25.2-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:90319e4f002795ccfc9050110bbbaa16c944b1c37c0baeea43c5fb881693ae1f"},
-    {file = "numpy-1.25.2-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:dfe4a913e29b418d096e696ddd422d8a5d13ffba4ea91f9f60440a3b759b0187"},
-    {file = "numpy-1.25.2-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:f08f2e037bba04e707eebf4bc934f1972a315c883a9e0ebfa8a7756eabf9e357"},
-    {file = "numpy-1.25.2-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:bec1e7213c7cb00d67093247f8c4db156fd03075f49876957dca4711306d39c9"},
-    {file = "numpy-1.25.2-cp310-cp310-win32.whl", hash = "sha256:7dc869c0c75988e1c693d0e2d5b26034644399dd929bc049db55395b1379e044"},
-    {file = "numpy-1.25.2-cp310-cp310-win_amd64.whl", hash = "sha256:834b386f2b8210dca38c71a6e0f4fd6922f7d3fcff935dbe3a570945acb1b545"},
-    {file = "numpy-1.25.2-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:c5462d19336db4560041517dbb7759c21d181a67cb01b36ca109b2ae37d32418"},
-    {file = "numpy-1.25.2-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:c5652ea24d33585ea39eb6a6a15dac87a1206a692719ff45d53c5282e66d4a8f"},
-    {file = "numpy-1.25.2-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:0d60fbae8e0019865fc4784745814cff1c421df5afee233db6d88ab4f14655a2"},
-    {file = "numpy-1.25.2-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:60e7f0f7f6d0eee8364b9a6304c2845b9c491ac706048c7e8cf47b83123b8dbf"},
-    {file = "numpy-1.25.2-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:bb33d5a1cf360304754913a350edda36d5b8c5331a8237268c48f91253c3a364"},
-    {file = "numpy-1.25.2-cp311-cp311-win32.whl", hash = "sha256:5883c06bb92f2e6c8181df7b39971a5fb436288db58b5a1c3967702d4278691d"},
-    {file = "numpy-1.25.2-cp311-cp311-win_amd64.whl", hash = "sha256:5c97325a0ba6f9d041feb9390924614b60b99209a71a69c876f71052521d42a4"},
-    {file = "numpy-1.25.2-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:b79e513d7aac42ae918db3ad1341a015488530d0bb2a6abcbdd10a3a829ccfd3"},
-    {file = "numpy-1.25.2-cp39-cp39-macosx_11_0_arm64.whl", hash = "sha256:eb942bfb6f84df5ce05dbf4b46673ffed0d3da59f13635ea9b926af3deb76926"},
-    {file = "numpy-1.25.2-cp39-cp39-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:3e0746410e73384e70d286f93abf2520035250aad8c5714240b0492a7302fdca"},
-    {file = "numpy-1.25.2-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:d7806500e4f5bdd04095e849265e55de20d8cc4b661b038957354327f6d9b295"},
-    {file = "numpy-1.25.2-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:8b77775f4b7df768967a7c8b3567e309f617dd5e99aeb886fa14dc1a0791141f"},
-    {file = "numpy-1.25.2-cp39-cp39-win32.whl", hash = "sha256:2792d23d62ec51e50ce4d4b7d73de8f67a2fd3ea710dcbc8563a51a03fb07b01"},
-    {file = "numpy-1.25.2-cp39-cp39-win_amd64.whl", hash = "sha256:76b4115d42a7dfc5d485d358728cdd8719be33cc5ec6ec08632a5d6fca2ed380"},
-    {file = "numpy-1.25.2-pp39-pypy39_pp73-macosx_10_9_x86_64.whl", hash = "sha256:1a1329e26f46230bf77b02cc19e900db9b52f398d6722ca853349a782d4cff55"},
-    {file = "numpy-1.25.2-pp39-pypy39_pp73-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:4c3abc71e8b6edba80a01a52e66d83c5d14433cbcd26a40c329ec7ed09f37901"},
-    {file = "numpy-1.25.2-pp39-pypy39_pp73-win_amd64.whl", hash = "sha256:1b9735c27cea5d995496f46a8b1cd7b408b3f34b6d50459d9ac8fe3a20cc17bf"},
-    {file = "numpy-1.25.2.tar.gz", hash = "sha256:fd608e19c8d7c55021dffd43bfe5492fab8cc105cc8986f813f8c3c048b38760"},
-]
-
-[[package]]
-name = "numpy"
-version = "1.26.1"
-description = "Fundamental package for array computing in Python"
-optional = false
-python-versions = "<3.13,>=3.9"
-files = [
-    {file = "numpy-1.26.1-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:82e871307a6331b5f09efda3c22e03c095d957f04bf6bc1804f30048d0e5e7af"},
-    {file = "numpy-1.26.1-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:cdd9ec98f0063d93baeb01aad472a1a0840dee302842a2746a7a8e92968f9575"},
-    {file = "numpy-1.26.1-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:d78f269e0c4fd365fc2992c00353e4530d274ba68f15e968d8bc3c69ce5f5244"},
-    {file = "numpy-1.26.1-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:8ab9163ca8aeb7fd32fe93866490654d2f7dda4e61bc6297bf72ce07fdc02f67"},
-    {file = "numpy-1.26.1-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:78ca54b2f9daffa5f323f34cdf21e1d9779a54073f0018a3094ab907938331a2"},
-    {file = "numpy-1.26.1-cp310-cp310-win32.whl", hash = "sha256:d1cfc92db6af1fd37a7bb58e55c8383b4aa1ba23d012bdbba26b4bcca45ac297"},
-    {file = "numpy-1.26.1-cp310-cp310-win_amd64.whl", hash = "sha256:d2984cb6caaf05294b8466966627e80bf6c7afd273279077679cb010acb0e5ab"},
-    {file = "numpy-1.26.1-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:cd7837b2b734ca72959a1caf3309457a318c934abef7a43a14bb984e574bbb9a"},
-    {file = "numpy-1.26.1-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:1c59c046c31a43310ad0199d6299e59f57a289e22f0f36951ced1c9eac3665b9"},
-    {file = "numpy-1.26.1-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:d58e8c51a7cf43090d124d5073bc29ab2755822181fcad978b12e144e5e5a4b3"},
-    {file = "numpy-1.26.1-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:6081aed64714a18c72b168a9276095ef9155dd7888b9e74b5987808f0dd0a974"},
-    {file = "numpy-1.26.1-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:97e5d6a9f0702c2863aaabf19f0d1b6c2628fbe476438ce0b5ce06e83085064c"},
-    {file = "numpy-1.26.1-cp311-cp311-win32.whl", hash = "sha256:b9d45d1dbb9de84894cc50efece5b09939752a2d75aab3a8b0cef6f3a35ecd6b"},
-    {file = "numpy-1.26.1-cp311-cp311-win_amd64.whl", hash = "sha256:3649d566e2fc067597125428db15d60eb42a4e0897fc48d28cb75dc2e0454e53"},
-    {file = "numpy-1.26.1-cp312-cp312-macosx_10_9_x86_64.whl", hash = "sha256:1d1bd82d539607951cac963388534da3b7ea0e18b149a53cf883d8f699178c0f"},
-    {file = "numpy-1.26.1-cp312-cp312-macosx_11_0_arm64.whl", hash = "sha256:afd5ced4e5a96dac6725daeb5242a35494243f2239244fad10a90ce58b071d24"},
-    {file = "numpy-1.26.1-cp312-cp312-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:a03fb25610ef560a6201ff06df4f8105292ba56e7cdd196ea350d123fc32e24e"},
-    {file = "numpy-1.26.1-cp312-cp312-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:dcfaf015b79d1f9f9c9fd0731a907407dc3e45769262d657d754c3a028586124"},
-    {file = "numpy-1.26.1-cp312-cp312-musllinux_1_1_x86_64.whl", hash = "sha256:e509cbc488c735b43b5ffea175235cec24bbc57b227ef1acc691725beb230d1c"},
-    {file = "numpy-1.26.1-cp312-cp312-win32.whl", hash = "sha256:af22f3d8e228d84d1c0c44c1fbdeb80f97a15a0abe4f080960393a00db733b66"},
-    {file = "numpy-1.26.1-cp312-cp312-win_amd64.whl", hash = "sha256:9f42284ebf91bdf32fafac29d29d4c07e5e9d1af862ea73686581773ef9e73a7"},
-    {file = "numpy-1.26.1-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:bb894accfd16b867d8643fc2ba6c8617c78ba2828051e9a69511644ce86ce83e"},
-    {file = "numpy-1.26.1-cp39-cp39-macosx_11_0_arm64.whl", hash = "sha256:e44ccb93f30c75dfc0c3aa3ce38f33486a75ec9abadabd4e59f114994a9c4617"},
-    {file = "numpy-1.26.1-cp39-cp39-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:9696aa2e35cc41e398a6d42d147cf326f8f9d81befcb399bc1ed7ffea339b64e"},
-    {file = "numpy-1.26.1-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:a5b411040beead47a228bde3b2241100454a6abde9df139ed087bd73fc0a4908"},
-    {file = "numpy-1.26.1-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:1e11668d6f756ca5ef534b5be8653d16c5352cbb210a5c2a79ff288e937010d5"},
-    {file = "numpy-1.26.1-cp39-cp39-win32.whl", hash = "sha256:d1d2c6b7dd618c41e202c59c1413ef9b2c8e8a15f5039e344af64195459e3104"},
-    {file = "numpy-1.26.1-cp39-cp39-win_amd64.whl", hash = "sha256:59227c981d43425ca5e5c01094d59eb14e8772ce6975d4b2fc1e106a833d5ae2"},
-    {file = "numpy-1.26.1-pp39-pypy39_pp73-macosx_10_9_x86_64.whl", hash = "sha256:06934e1a22c54636a059215d6da99e23286424f316fddd979f5071093b648668"},
-    {file = "numpy-1.26.1-pp39-pypy39_pp73-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:76ff661a867d9272cd2a99eed002470f46dbe0943a5ffd140f49be84f68ffc42"},
-    {file = "numpy-1.26.1-pp39-pypy39_pp73-win_amd64.whl", hash = "sha256:6965888d65d2848e8768824ca8288db0a81263c1efccec881cb35a0d805fcd2f"},
-    {file = "numpy-1.26.1.tar.gz", hash = "sha256:c8c6c72d4a9f831f328efb1312642a1cafafaa88981d9ab76368d50d07d93cbe"},
+    {file = "numpy-1.26.4-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:9ff0f4f29c51e2803569d7a51c2304de5554655a60c5d776e35b4a41413830d0"},
+    {file = "numpy-1.26.4-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:2e4ee3380d6de9c9ec04745830fd9e2eccb3e6cf790d39d7b98ffd19b0dd754a"},
+    {file = "numpy-1.26.4-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:d209d8969599b27ad20994c8e41936ee0964e6da07478d6c35016bc386b66ad4"},
+    {file = "numpy-1.26.4-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:ffa75af20b44f8dba823498024771d5ac50620e6915abac414251bd971b4529f"},
+    {file = "numpy-1.26.4-cp310-cp310-musllinux_1_1_aarch64.whl", hash = "sha256:62b8e4b1e28009ef2846b4c7852046736bab361f7aeadeb6a5b89ebec3c7055a"},
+    {file = "numpy-1.26.4-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:a4abb4f9001ad2858e7ac189089c42178fcce737e4169dc61321660f1a96c7d2"},
+    {file = "numpy-1.26.4-cp310-cp310-win32.whl", hash = "sha256:bfe25acf8b437eb2a8b2d49d443800a5f18508cd811fea3181723922a8a82b07"},
+    {file = "numpy-1.26.4-cp310-cp310-win_amd64.whl", hash = "sha256:b97fe8060236edf3662adfc2c633f56a08ae30560c56310562cb4f95500022d5"},
+    {file = "numpy-1.26.4-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:4c66707fabe114439db9068ee468c26bbdf909cac0fb58686a42a24de1760c71"},
+    {file = "numpy-1.26.4-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:edd8b5fe47dab091176d21bb6de568acdd906d1887a4584a15a9a96a1dca06ef"},
+    {file = "numpy-1.26.4-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:7ab55401287bfec946ced39700c053796e7cc0e3acbef09993a9ad2adba6ca6e"},
+    {file = "numpy-1.26.4-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:666dbfb6ec68962c033a450943ded891bed2d54e6755e35e5835d63f4f6931d5"},
+    {file = "numpy-1.26.4-cp311-cp311-musllinux_1_1_aarch64.whl", hash = "sha256:96ff0b2ad353d8f990b63294c8986f1ec3cb19d749234014f4e7eb0112ceba5a"},
+    {file = "numpy-1.26.4-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:60dedbb91afcbfdc9bc0b1f3f402804070deed7392c23eb7a7f07fa857868e8a"},
+    {file = "numpy-1.26.4-cp311-cp311-win32.whl", hash = "sha256:1af303d6b2210eb850fcf03064d364652b7120803a0b872f5211f5234b399f20"},
+    {file = "numpy-1.26.4-cp311-cp311-win_amd64.whl", hash = "sha256:cd25bcecc4974d09257ffcd1f098ee778f7834c3ad767fe5db785be9a4aa9cb2"},
+    {file = "numpy-1.26.4-cp312-cp312-macosx_10_9_x86_64.whl", hash = "sha256:b3ce300f3644fb06443ee2222c2201dd3a89ea6040541412b8fa189341847218"},
+    {file = "numpy-1.26.4-cp312-cp312-macosx_11_0_arm64.whl", hash = "sha256:03a8c78d01d9781b28a6989f6fa1bb2c4f2d51201cf99d3dd875df6fbd96b23b"},
+    {file = "numpy-1.26.4-cp312-cp312-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:9fad7dcb1aac3c7f0584a5a8133e3a43eeb2fe127f47e3632d43d677c66c102b"},
+    {file = "numpy-1.26.4-cp312-cp312-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:675d61ffbfa78604709862923189bad94014bef562cc35cf61d3a07bba02a7ed"},
+    {file = "numpy-1.26.4-cp312-cp312-musllinux_1_1_aarch64.whl", hash = "sha256:ab47dbe5cc8210f55aa58e4805fe224dac469cde56b9f731a4c098b91917159a"},
+    {file = "numpy-1.26.4-cp312-cp312-musllinux_1_1_x86_64.whl", hash = "sha256:1dda2e7b4ec9dd512f84935c5f126c8bd8b9f2fc001e9f54af255e8c5f16b0e0"},
+    {file = "numpy-1.26.4-cp312-cp312-win32.whl", hash = "sha256:50193e430acfc1346175fcbdaa28ffec49947a06918b7b92130744e81e640110"},
+    {file = "numpy-1.26.4-cp312-cp312-win_amd64.whl", hash = "sha256:08beddf13648eb95f8d867350f6a018a4be2e5ad54c8d8caed89ebca558b2818"},
+    {file = "numpy-1.26.4-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:7349ab0fa0c429c82442a27a9673fc802ffdb7c7775fad780226cb234965e53c"},
+    {file = "numpy-1.26.4-cp39-cp39-macosx_11_0_arm64.whl", hash = "sha256:52b8b60467cd7dd1e9ed082188b4e6bb35aa5cdd01777621a1658910745b90be"},
+    {file = "numpy-1.26.4-cp39-cp39-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:d5241e0a80d808d70546c697135da2c613f30e28251ff8307eb72ba696945764"},
+    {file = "numpy-1.26.4-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:f870204a840a60da0b12273ef34f7051e98c3b5961b61b0c2c1be6dfd64fbcd3"},
+    {file = "numpy-1.26.4-cp39-cp39-musllinux_1_1_aarch64.whl", hash = "sha256:679b0076f67ecc0138fd2ede3a8fd196dddc2ad3254069bcb9faf9a79b1cebcd"},
+    {file = "numpy-1.26.4-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:47711010ad8555514b434df65f7d7b076bb8261df1ca9bb78f53d3b2db02e95c"},
+    {file = "numpy-1.26.4-cp39-cp39-win32.whl", hash = "sha256:a354325ee03388678242a4d7ebcd08b5c727033fcff3b2f536aea978e15ee9e6"},
+    {file = "numpy-1.26.4-cp39-cp39-win_amd64.whl", hash = "sha256:3373d5d70a5fe74a2c1bb6d2cfd9609ecf686d47a2d7b1d37a8f3b6bf6003aea"},
+    {file = "numpy-1.26.4-pp39-pypy39_pp73-macosx_10_9_x86_64.whl", hash = "sha256:afedb719a9dcfc7eaf2287b839d8198e06dcd4cb5d276a3df279231138e83d30"},
+    {file = "numpy-1.26.4-pp39-pypy39_pp73-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:95a7476c59002f2f6c590b9b7b998306fba6a5aa646b1e22ddfeaf8f78c3a29c"},
+    {file = "numpy-1.26.4-pp39-pypy39_pp73-win_amd64.whl", hash = "sha256:7e50d0a0cc3189f9cb0aeb3a6a6af18c16f59f004b866cd2be1c14b36134a4a0"},
+    {file = "numpy-1.26.4.tar.gz", hash = "sha256:2a02aba9ed12e4ac4eb3ea9421c420301a0c6460d9830d74a9df87efa4912010"},
 ]
 
 [[package]]
 name = "oauthlib"
 version = "3.2.2"
 description = "A generic, spec-compliant, thorough implementation of the OAuth request-signing logic"
 optional = false
@@ -299,146 +269,94 @@
 [package.extras]
 rsa = ["cryptography (>=3.0.0)"]
 signals = ["blinker (>=1.4.0)"]
 signedtoken = ["cryptography (>=3.0.0)", "pyjwt (>=2.0.0,<3)"]
 
 [[package]]
 name = "pandas"
-version = "2.1.0"
+version = "2.2.1"
 description = "Powerful data structures for data analysis, time series, and statistics"
 optional = false
 python-versions = ">=3.9"
 files = [
-    {file = "pandas-2.1.0-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:40dd20439ff94f1b2ed55b393ecee9cb6f3b08104c2c40b0cb7186a2f0046242"},
-    {file = "pandas-2.1.0-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:d4f38e4fedeba580285eaac7ede4f686c6701a9e618d8a857b138a126d067f2f"},
-    {file = "pandas-2.1.0-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:6e6a0fe052cf27ceb29be9429428b4918f3740e37ff185658f40d8702f0b3e09"},
-    {file = "pandas-2.1.0-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:9d81e1813191070440d4c7a413cb673052b3b4a984ffd86b8dd468c45742d3cc"},
-    {file = "pandas-2.1.0-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:eb20252720b1cc1b7d0b2879ffc7e0542dd568f24d7c4b2347cb035206936421"},
-    {file = "pandas-2.1.0-cp310-cp310-win_amd64.whl", hash = "sha256:38f74ef7ebc0ffb43b3d633e23d74882bce7e27bfa09607f3c5d3e03ffd9a4a5"},
-    {file = "pandas-2.1.0-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:cda72cc8c4761c8f1d97b169661f23a86b16fdb240bdc341173aee17e4d6cedd"},
-    {file = "pandas-2.1.0-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:d97daeac0db8c993420b10da4f5f5b39b01fc9ca689a17844e07c0a35ac96b4b"},
-    {file = "pandas-2.1.0-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:d8c58b1113892e0c8078f006a167cc210a92bdae23322bb4614f2f0b7a4b510f"},
-    {file = "pandas-2.1.0-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:629124923bcf798965b054a540f9ccdfd60f71361255c81fa1ecd94a904b9dd3"},
-    {file = "pandas-2.1.0-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:70cf866af3ab346a10debba8ea78077cf3a8cd14bd5e4bed3d41555a3280041c"},
-    {file = "pandas-2.1.0-cp311-cp311-win_amd64.whl", hash = "sha256:d53c8c1001f6a192ff1de1efe03b31a423d0eee2e9e855e69d004308e046e694"},
-    {file = "pandas-2.1.0-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:86f100b3876b8c6d1a2c66207288ead435dc71041ee4aea789e55ef0e06408cb"},
-    {file = "pandas-2.1.0-cp39-cp39-macosx_11_0_arm64.whl", hash = "sha256:28f330845ad21c11db51e02d8d69acc9035edfd1116926ff7245c7215db57957"},
-    {file = "pandas-2.1.0-cp39-cp39-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:b9a6ccf0963db88f9b12df6720e55f337447aea217f426a22d71f4213a3099a6"},
-    {file = "pandas-2.1.0-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:d99e678180bc59b0c9443314297bddce4ad35727a1a2656dbe585fd78710b3b9"},
-    {file = "pandas-2.1.0-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:b31da36d376d50a1a492efb18097b9101bdbd8b3fbb3f49006e02d4495d4c644"},
-    {file = "pandas-2.1.0-cp39-cp39-win_amd64.whl", hash = "sha256:0164b85937707ec7f70b34a6c3a578dbf0f50787f910f21ca3b26a7fd3363437"},
-    {file = "pandas-2.1.0.tar.gz", hash = "sha256:62c24c7fc59e42b775ce0679cfa7b14a5f9bfb7643cfbe708c960699e05fb918"},
-]
-
-[package.dependencies]
-numpy = {version = ">=1.23.2", markers = "python_version >= \"3.11\""}
-python-dateutil = ">=2.8.2"
-pytz = ">=2020.1"
-tzdata = ">=2022.1"
-
-[package.extras]
-all = ["PyQt5 (>=5.15.6)", "SQLAlchemy (>=1.4.36)", "beautifulsoup4 (>=4.11.1)", "bottleneck (>=1.3.4)", "dataframe-api-compat (>=0.1.7)", "fastparquet (>=0.8.1)", "fsspec (>=2022.05.0)", "gcsfs (>=2022.05.0)", "html5lib (>=1.1)", "hypothesis (>=6.46.1)", "jinja2 (>=3.1.2)", "lxml (>=4.8.0)", "matplotlib (>=3.6.1)", "numba (>=0.55.2)", "numexpr (>=2.8.0)", "odfpy (>=1.4.1)", "openpyxl (>=3.0.10)", "pandas-gbq (>=0.17.5)", "psycopg2 (>=2.9.3)", "pyarrow (>=7.0.0)", "pymysql (>=1.0.2)", "pyreadstat (>=1.1.5)", "pytest (>=7.3.2)", "pytest-asyncio (>=0.17.0)", "pytest-xdist (>=2.2.0)", "pyxlsb (>=1.0.9)", "qtpy (>=2.2.0)", "s3fs (>=2022.05.0)", "scipy (>=1.8.1)", "tables (>=3.7.0)", "tabulate (>=0.8.10)", "xarray (>=2022.03.0)", "xlrd (>=2.0.1)", "xlsxwriter (>=3.0.3)", "zstandard (>=0.17.0)"]
-aws = ["s3fs (>=2022.05.0)"]
-clipboard = ["PyQt5 (>=5.15.6)", "qtpy (>=2.2.0)"]
-compression = ["zstandard (>=0.17.0)"]
-computation = ["scipy (>=1.8.1)", "xarray (>=2022.03.0)"]
-consortium-standard = ["dataframe-api-compat (>=0.1.7)"]
-excel = ["odfpy (>=1.4.1)", "openpyxl (>=3.0.10)", "pyxlsb (>=1.0.9)", "xlrd (>=2.0.1)", "xlsxwriter (>=3.0.3)"]
-feather = ["pyarrow (>=7.0.0)"]
-fss = ["fsspec (>=2022.05.0)"]
-gcp = ["gcsfs (>=2022.05.0)", "pandas-gbq (>=0.17.5)"]
-hdf5 = ["tables (>=3.7.0)"]
-html = ["beautifulsoup4 (>=4.11.1)", "html5lib (>=1.1)", "lxml (>=4.8.0)"]
-mysql = ["SQLAlchemy (>=1.4.36)", "pymysql (>=1.0.2)"]
-output-formatting = ["jinja2 (>=3.1.2)", "tabulate (>=0.8.10)"]
-parquet = ["pyarrow (>=7.0.0)"]
-performance = ["bottleneck (>=1.3.4)", "numba (>=0.55.2)", "numexpr (>=2.8.0)"]
-plot = ["matplotlib (>=3.6.1)"]
-postgresql = ["SQLAlchemy (>=1.4.36)", "psycopg2 (>=2.9.3)"]
-spss = ["pyreadstat (>=1.1.5)"]
-sql-other = ["SQLAlchemy (>=1.4.36)"]
-test = ["hypothesis (>=6.46.1)", "pytest (>=7.3.2)", "pytest-asyncio (>=0.17.0)", "pytest-xdist (>=2.2.0)"]
-xml = ["lxml (>=4.8.0)"]
-
-[[package]]
-name = "pandas"
-version = "2.1.2"
-description = "Powerful data structures for data analysis, time series, and statistics"
-optional = false
-python-versions = ">=3.9"
-files = [
-    {file = "pandas-2.1.2-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:24057459f19db9ebb02984c6fdd164a970b31a95f38e4a49cf7615b36a1b532c"},
-    {file = "pandas-2.1.2-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:a6cf8fcc8a63d333970b950a7331a30544cf59b1a97baf0a7409e09eafc1ac38"},
-    {file = "pandas-2.1.2-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:6ae6ffbd9d614c20d028c7117ee911fc4e266b4dca2065d5c5909e401f8ff683"},
-    {file = "pandas-2.1.2-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:eff794eeb7883c5aefb1ed572e7ff533ae779f6c6277849eab9e77986e352688"},
-    {file = "pandas-2.1.2-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:02954e285e8e2f4006b6f22be6f0df1f1c3c97adbb7ed211c6b483426f20d5c8"},
-    {file = "pandas-2.1.2-cp310-cp310-win_amd64.whl", hash = "sha256:5b40c9f494e1f27588c369b9e4a6ca19cd924b3a0e1ef9ef1a8e30a07a438f43"},
-    {file = "pandas-2.1.2-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:08d287b68fd28906a94564f15118a7ca8c242e50ae7f8bd91130c362b2108a81"},
-    {file = "pandas-2.1.2-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:bbd98dcdcd32f408947afdb3f7434fade6edd408c3077bbce7bd840d654d92c6"},
-    {file = "pandas-2.1.2-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:e90c95abb3285d06f6e4feedafc134306a8eced93cb78e08cf50e224d5ce22e2"},
-    {file = "pandas-2.1.2-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:52867d69a54e71666cd184b04e839cff7dfc8ed0cd6b936995117fdae8790b69"},
-    {file = "pandas-2.1.2-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:8d0382645ede2fde352da2a885aac28ec37d38587864c0689b4b2361d17b1d4c"},
-    {file = "pandas-2.1.2-cp311-cp311-win_amd64.whl", hash = "sha256:65177d1c519b55e5b7f094c660ed357bb7d86e799686bb71653b8a4803d8ff0d"},
-    {file = "pandas-2.1.2-cp312-cp312-macosx_10_9_x86_64.whl", hash = "sha256:5aa6b86802e8cf7716bf4b4b5a3c99b12d34e9c6a9d06dad254447a620437931"},
-    {file = "pandas-2.1.2-cp312-cp312-macosx_11_0_arm64.whl", hash = "sha256:d594e2ce51b8e0b4074e6644758865dc2bb13fd654450c1eae51201260a539f1"},
-    {file = "pandas-2.1.2-cp312-cp312-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:3223f997b6d2ebf9c010260cf3d889848a93f5d22bb4d14cd32638b3d8bba7ad"},
-    {file = "pandas-2.1.2-cp312-cp312-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:fc4944dc004ca6cc701dfa19afb8bdb26ad36b9bed5bcec617d2a11e9cae6902"},
-    {file = "pandas-2.1.2-cp312-cp312-musllinux_1_1_x86_64.whl", hash = "sha256:3f76280ce8ec216dde336e55b2b82e883401cf466da0fe3be317c03fb8ee7c7d"},
-    {file = "pandas-2.1.2-cp312-cp312-win_amd64.whl", hash = "sha256:7ad20d24acf3a0042512b7e8d8fdc2e827126ed519d6bd1ed8e6c14ec8a2c813"},
-    {file = "pandas-2.1.2-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:021f09c15e1381e202d95d4a21ece8e7f2bf1388b6d7e9cae09dfe27bd2043d1"},
-    {file = "pandas-2.1.2-cp39-cp39-macosx_11_0_arm64.whl", hash = "sha256:e7f12b2de0060b0b858cfec0016e7d980ae5bae455a1746bfcc70929100ee633"},
-    {file = "pandas-2.1.2-cp39-cp39-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:83c166b9bb27c1715bed94495d9598a7f02950b4749dba9349c1dd2cbf10729d"},
-    {file = "pandas-2.1.2-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:25c9976c17311388fcd953cb3d0697999b2205333f4e11e669d90ff8d830d429"},
-    {file = "pandas-2.1.2-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:851b5afbb0d62f6129ae891b533aa508cc357d5892c240c91933d945fff15731"},
-    {file = "pandas-2.1.2-cp39-cp39-win_amd64.whl", hash = "sha256:e78507adcc730533619de07bfdd1c62b2918a68cd4419ea386e28abf7f6a1e5c"},
-    {file = "pandas-2.1.2.tar.gz", hash = "sha256:52897edc2774d2779fbeb6880d2cfb305daa0b1a29c16b91f531a18918a6e0f3"},
+    {file = "pandas-2.2.1-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:8df8612be9cd1c7797c93e1c5df861b2ddda0b48b08f2c3eaa0702cf88fb5f88"},
+    {file = "pandas-2.2.1-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:0f573ab277252ed9aaf38240f3b54cfc90fff8e5cab70411ee1d03f5d51f3944"},
+    {file = "pandas-2.2.1-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:f02a3a6c83df4026e55b63c1f06476c9aa3ed6af3d89b4f04ea656ccdaaaa359"},
+    {file = "pandas-2.2.1-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:c38ce92cb22a4bea4e3929429aa1067a454dcc9c335799af93ba9be21b6beb51"},
+    {file = "pandas-2.2.1-cp310-cp310-musllinux_1_1_aarch64.whl", hash = "sha256:c2ce852e1cf2509a69e98358e8458775f89599566ac3775e70419b98615f4b06"},
+    {file = "pandas-2.2.1-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:53680dc9b2519cbf609c62db3ed7c0b499077c7fefda564e330286e619ff0dd9"},
+    {file = "pandas-2.2.1-cp310-cp310-win_amd64.whl", hash = "sha256:94e714a1cca63e4f5939cdce5f29ba8d415d85166be3441165edd427dc9f6bc0"},
+    {file = "pandas-2.2.1-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:f821213d48f4ab353d20ebc24e4faf94ba40d76680642fb7ce2ea31a3ad94f9b"},
+    {file = "pandas-2.2.1-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:c70e00c2d894cb230e5c15e4b1e1e6b2b478e09cf27cc593a11ef955b9ecc81a"},
+    {file = "pandas-2.2.1-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:e97fbb5387c69209f134893abc788a6486dbf2f9e511070ca05eed4b930b1b02"},
+    {file = "pandas-2.2.1-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:101d0eb9c5361aa0146f500773395a03839a5e6ecde4d4b6ced88b7e5a1a6403"},
+    {file = "pandas-2.2.1-cp311-cp311-musllinux_1_1_aarch64.whl", hash = "sha256:7d2ed41c319c9fb4fd454fe25372028dfa417aacb9790f68171b2e3f06eae8cd"},
+    {file = "pandas-2.2.1-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:af5d3c00557d657c8773ef9ee702c61dd13b9d7426794c9dfeb1dc4a0bf0ebc7"},
+    {file = "pandas-2.2.1-cp311-cp311-win_amd64.whl", hash = "sha256:06cf591dbaefb6da9de8472535b185cba556d0ce2e6ed28e21d919704fef1a9e"},
+    {file = "pandas-2.2.1-cp312-cp312-macosx_10_9_x86_64.whl", hash = "sha256:88ecb5c01bb9ca927ebc4098136038519aa5d66b44671861ffab754cae75102c"},
+    {file = "pandas-2.2.1-cp312-cp312-macosx_11_0_arm64.whl", hash = "sha256:04f6ec3baec203c13e3f8b139fb0f9f86cd8c0b94603ae3ae8ce9a422e9f5bee"},
+    {file = "pandas-2.2.1-cp312-cp312-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:a935a90a76c44fe170d01e90a3594beef9e9a6220021acfb26053d01426f7dc2"},
+    {file = "pandas-2.2.1-cp312-cp312-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:c391f594aae2fd9f679d419e9a4d5ba4bce5bb13f6a989195656e7dc4b95c8f0"},
+    {file = "pandas-2.2.1-cp312-cp312-musllinux_1_1_aarch64.whl", hash = "sha256:9d1265545f579edf3f8f0cb6f89f234f5e44ba725a34d86535b1a1d38decbccc"},
+    {file = "pandas-2.2.1-cp312-cp312-musllinux_1_1_x86_64.whl", hash = "sha256:11940e9e3056576ac3244baef2fedade891977bcc1cb7e5cc8f8cc7d603edc89"},
+    {file = "pandas-2.2.1-cp312-cp312-win_amd64.whl", hash = "sha256:4acf681325ee1c7f950d058b05a820441075b0dd9a2adf5c4835b9bc056bf4fb"},
+    {file = "pandas-2.2.1-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:9bd8a40f47080825af4317d0340c656744f2bfdb6819f818e6ba3cd24c0e1397"},
+    {file = "pandas-2.2.1-cp39-cp39-macosx_11_0_arm64.whl", hash = "sha256:df0c37ebd19e11d089ceba66eba59a168242fc6b7155cba4ffffa6eccdfb8f16"},
+    {file = "pandas-2.2.1-cp39-cp39-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:739cc70eaf17d57608639e74d63387b0d8594ce02f69e7a0b046f117974b3019"},
+    {file = "pandas-2.2.1-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:f9d3558d263073ed95e46f4650becff0c5e1ffe0fc3a015de3c79283dfbdb3df"},
+    {file = "pandas-2.2.1-cp39-cp39-musllinux_1_1_aarch64.whl", hash = "sha256:4aa1d8707812a658debf03824016bf5ea0d516afdea29b7dc14cf687bc4d4ec6"},
+    {file = "pandas-2.2.1-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:76f27a809cda87e07f192f001d11adc2b930e93a2b0c4a236fde5429527423be"},
+    {file = "pandas-2.2.1-cp39-cp39-win_amd64.whl", hash = "sha256:1ba21b1d5c0e43416218db63037dbe1a01fc101dc6e6024bcad08123e48004ab"},
+    {file = "pandas-2.2.1.tar.gz", hash = "sha256:0ab90f87093c13f3e8fa45b48ba9f39181046e8f3317d3aadb2fffbb1b978572"},
 ]
 
 [package.dependencies]
 numpy = [
     {version = ">=1.22.4,<2", markers = "python_version < \"3.11\""},
     {version = ">=1.23.2,<2", markers = "python_version == \"3.11\""},
+    {version = ">=1.26.0,<2", markers = "python_version >= \"3.12\""},
 ]
 python-dateutil = ">=2.8.2"
 pytz = ">=2020.1"
-tzdata = ">=2022.1"
+tzdata = ">=2022.7"
 
 [package.extras]
-all = ["PyQt5 (>=5.15.6)", "SQLAlchemy (>=1.4.36)", "beautifulsoup4 (>=4.11.1)", "bottleneck (>=1.3.4)", "dataframe-api-compat (>=0.1.7)", "fastparquet (>=0.8.1)", "fsspec (>=2022.05.0)", "gcsfs (>=2022.05.0)", "html5lib (>=1.1)", "hypothesis (>=6.46.1)", "jinja2 (>=3.1.2)", "lxml (>=4.8.0)", "matplotlib (>=3.6.1)", "numba (>=0.55.2)", "numexpr (>=2.8.0)", "odfpy (>=1.4.1)", "openpyxl (>=3.0.10)", "pandas-gbq (>=0.17.5)", "psycopg2 (>=2.9.3)", "pyarrow (>=7.0.0)", "pymysql (>=1.0.2)", "pyreadstat (>=1.1.5)", "pytest (>=7.3.2)", "pytest-asyncio (>=0.17.0)", "pytest-xdist (>=2.2.0)", "pyxlsb (>=1.0.9)", "qtpy (>=2.2.0)", "s3fs (>=2022.05.0)", "scipy (>=1.8.1)", "tables (>=3.7.0)", "tabulate (>=0.8.10)", "xarray (>=2022.03.0)", "xlrd (>=2.0.1)", "xlsxwriter (>=3.0.3)", "zstandard (>=0.17.0)"]
-aws = ["s3fs (>=2022.05.0)"]
-clipboard = ["PyQt5 (>=5.15.6)", "qtpy (>=2.2.0)"]
-compression = ["zstandard (>=0.17.0)"]
-computation = ["scipy (>=1.8.1)", "xarray (>=2022.03.0)"]
+all = ["PyQt5 (>=5.15.9)", "SQLAlchemy (>=2.0.0)", "adbc-driver-postgresql (>=0.8.0)", "adbc-driver-sqlite (>=0.8.0)", "beautifulsoup4 (>=4.11.2)", "bottleneck (>=1.3.6)", "dataframe-api-compat (>=0.1.7)", "fastparquet (>=2022.12.0)", "fsspec (>=2022.11.0)", "gcsfs (>=2022.11.0)", "html5lib (>=1.1)", "hypothesis (>=6.46.1)", "jinja2 (>=3.1.2)", "lxml (>=4.9.2)", "matplotlib (>=3.6.3)", "numba (>=0.56.4)", "numexpr (>=2.8.4)", "odfpy (>=1.4.1)", "openpyxl (>=3.1.0)", "pandas-gbq (>=0.19.0)", "psycopg2 (>=2.9.6)", "pyarrow (>=10.0.1)", "pymysql (>=1.0.2)", "pyreadstat (>=1.2.0)", "pytest (>=7.3.2)", "pytest-xdist (>=2.2.0)", "python-calamine (>=0.1.7)", "pyxlsb (>=1.0.10)", "qtpy (>=2.3.0)", "s3fs (>=2022.11.0)", "scipy (>=1.10.0)", "tables (>=3.8.0)", "tabulate (>=0.9.0)", "xarray (>=2022.12.0)", "xlrd (>=2.0.1)", "xlsxwriter (>=3.0.5)", "zstandard (>=0.19.0)"]
+aws = ["s3fs (>=2022.11.0)"]
+clipboard = ["PyQt5 (>=5.15.9)", "qtpy (>=2.3.0)"]
+compression = ["zstandard (>=0.19.0)"]
+computation = ["scipy (>=1.10.0)", "xarray (>=2022.12.0)"]
 consortium-standard = ["dataframe-api-compat (>=0.1.7)"]
-excel = ["odfpy (>=1.4.1)", "openpyxl (>=3.0.10)", "pyxlsb (>=1.0.9)", "xlrd (>=2.0.1)", "xlsxwriter (>=3.0.3)"]
-feather = ["pyarrow (>=7.0.0)"]
-fss = ["fsspec (>=2022.05.0)"]
-gcp = ["gcsfs (>=2022.05.0)", "pandas-gbq (>=0.17.5)"]
-hdf5 = ["tables (>=3.7.0)"]
-html = ["beautifulsoup4 (>=4.11.1)", "html5lib (>=1.1)", "lxml (>=4.8.0)"]
-mysql = ["SQLAlchemy (>=1.4.36)", "pymysql (>=1.0.2)"]
-output-formatting = ["jinja2 (>=3.1.2)", "tabulate (>=0.8.10)"]
-parquet = ["pyarrow (>=7.0.0)"]
-performance = ["bottleneck (>=1.3.4)", "numba (>=0.55.2)", "numexpr (>=2.8.0)"]
-plot = ["matplotlib (>=3.6.1)"]
-postgresql = ["SQLAlchemy (>=1.4.36)", "psycopg2 (>=2.9.3)"]
-spss = ["pyreadstat (>=1.1.5)"]
-sql-other = ["SQLAlchemy (>=1.4.36)"]
-test = ["hypothesis (>=6.46.1)", "pytest (>=7.3.2)", "pytest-asyncio (>=0.17.0)", "pytest-xdist (>=2.2.0)"]
-xml = ["lxml (>=4.8.0)"]
+excel = ["odfpy (>=1.4.1)", "openpyxl (>=3.1.0)", "python-calamine (>=0.1.7)", "pyxlsb (>=1.0.10)", "xlrd (>=2.0.1)", "xlsxwriter (>=3.0.5)"]
+feather = ["pyarrow (>=10.0.1)"]
+fss = ["fsspec (>=2022.11.0)"]
+gcp = ["gcsfs (>=2022.11.0)", "pandas-gbq (>=0.19.0)"]
+hdf5 = ["tables (>=3.8.0)"]
+html = ["beautifulsoup4 (>=4.11.2)", "html5lib (>=1.1)", "lxml (>=4.9.2)"]
+mysql = ["SQLAlchemy (>=2.0.0)", "pymysql (>=1.0.2)"]
+output-formatting = ["jinja2 (>=3.1.2)", "tabulate (>=0.9.0)"]
+parquet = ["pyarrow (>=10.0.1)"]
+performance = ["bottleneck (>=1.3.6)", "numba (>=0.56.4)", "numexpr (>=2.8.4)"]
+plot = ["matplotlib (>=3.6.3)"]
+postgresql = ["SQLAlchemy (>=2.0.0)", "adbc-driver-postgresql (>=0.8.0)", "psycopg2 (>=2.9.6)"]
+pyarrow = ["pyarrow (>=10.0.1)"]
+spss = ["pyreadstat (>=1.2.0)"]
+sql-other = ["SQLAlchemy (>=2.0.0)", "adbc-driver-postgresql (>=0.8.0)", "adbc-driver-sqlite (>=0.8.0)"]
+test = ["hypothesis (>=6.46.1)", "pytest (>=7.3.2)", "pytest-xdist (>=2.2.0)"]
+xml = ["lxml (>=4.9.2)"]
 
 [[package]]
 name = "pyasn1"
-version = "0.5.0"
+version = "0.5.1"
 description = "Pure-Python implementation of ASN.1 types and DER/BER/CER codecs (X.208)"
 optional = false
 python-versions = "!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*,!=3.5.*,>=2.7"
 files = [
-    {file = "pyasn1-0.5.0-py2.py3-none-any.whl", hash = "sha256:87a2121042a1ac9358cabcaf1d07680ff97ee6404333bacca15f76aa8ad01a57"},
-    {file = "pyasn1-0.5.0.tar.gz", hash = "sha256:97b7290ca68e62a832558ec3976f15cbf911bf5d7c7039d8b861c2a0ece69fde"},
+    {file = "pyasn1-0.5.1-py2.py3-none-any.whl", hash = "sha256:4439847c58d40b1d0a573d07e3856e95333f1976294494c325775aeca506eb58"},
+    {file = "pyasn1-0.5.1.tar.gz", hash = "sha256:6d391a96e59b23130a5cfa74d6fd7f388dbbe26cc8f1edf39fdddf08d9d6676c"},
 ]
 
 [[package]]
 name = "pyasn1-modules"
 version = "0.3.0"
 description = "A collection of ASN.1-based protocols modules"
 optional = false
@@ -449,87 +367,87 @@
 ]
 
 [package.dependencies]
 pyasn1 = ">=0.4.6,<0.6.0"
 
 [[package]]
 name = "pydantic"
-version = "1.10.13"
+version = "1.10.14"
 description = "Data validation and settings management using python type hints"
 optional = false
 python-versions = ">=3.7"
 files = [
-    {file = "pydantic-1.10.13-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:efff03cc7a4f29d9009d1c96ceb1e7a70a65cfe86e89d34e4a5f2ab1e5693737"},
-    {file = "pydantic-1.10.13-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:3ecea2b9d80e5333303eeb77e180b90e95eea8f765d08c3d278cd56b00345d01"},
-    {file = "pydantic-1.10.13-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:1740068fd8e2ef6eb27a20e5651df000978edce6da6803c2bef0bc74540f9548"},
-    {file = "pydantic-1.10.13-cp310-cp310-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:84bafe2e60b5e78bc64a2941b4c071a4b7404c5c907f5f5a99b0139781e69ed8"},
-    {file = "pydantic-1.10.13-cp310-cp310-musllinux_1_1_i686.whl", hash = "sha256:bc0898c12f8e9c97f6cd44c0ed70d55749eaf783716896960b4ecce2edfd2d69"},
-    {file = "pydantic-1.10.13-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:654db58ae399fe6434e55325a2c3e959836bd17a6f6a0b6ca8107ea0571d2e17"},
-    {file = "pydantic-1.10.13-cp310-cp310-win_amd64.whl", hash = "sha256:75ac15385a3534d887a99c713aa3da88a30fbd6204a5cd0dc4dab3d770b9bd2f"},
-    {file = "pydantic-1.10.13-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:c553f6a156deb868ba38a23cf0df886c63492e9257f60a79c0fd8e7173537653"},
-    {file = "pydantic-1.10.13-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:5e08865bc6464df8c7d61439ef4439829e3ab62ab1669cddea8dd00cd74b9ffe"},
-    {file = "pydantic-1.10.13-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:e31647d85a2013d926ce60b84f9dd5300d44535a9941fe825dc349ae1f760df9"},
-    {file = "pydantic-1.10.13-cp311-cp311-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:210ce042e8f6f7c01168b2d84d4c9eb2b009fe7bf572c2266e235edf14bacd80"},
-    {file = "pydantic-1.10.13-cp311-cp311-musllinux_1_1_i686.whl", hash = "sha256:8ae5dd6b721459bfa30805f4c25880e0dd78fc5b5879f9f7a692196ddcb5a580"},
-    {file = "pydantic-1.10.13-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:f8e81fc5fb17dae698f52bdd1c4f18b6ca674d7068242b2aff075f588301bbb0"},
-    {file = "pydantic-1.10.13-cp311-cp311-win_amd64.whl", hash = "sha256:61d9dce220447fb74f45e73d7ff3b530e25db30192ad8d425166d43c5deb6df0"},
-    {file = "pydantic-1.10.13-cp37-cp37m-macosx_10_9_x86_64.whl", hash = "sha256:4b03e42ec20286f052490423682016fd80fda830d8e4119f8ab13ec7464c0132"},
-    {file = "pydantic-1.10.13-cp37-cp37m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:f59ef915cac80275245824e9d771ee939133be38215555e9dc90c6cb148aaeb5"},
-    {file = "pydantic-1.10.13-cp37-cp37m-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:5a1f9f747851338933942db7af7b6ee8268568ef2ed86c4185c6ef4402e80ba8"},
-    {file = "pydantic-1.10.13-cp37-cp37m-musllinux_1_1_i686.whl", hash = "sha256:97cce3ae7341f7620a0ba5ef6cf043975cd9d2b81f3aa5f4ea37928269bc1b87"},
-    {file = "pydantic-1.10.13-cp37-cp37m-musllinux_1_1_x86_64.whl", hash = "sha256:854223752ba81e3abf663d685f105c64150873cc6f5d0c01d3e3220bcff7d36f"},
-    {file = "pydantic-1.10.13-cp37-cp37m-win_amd64.whl", hash = "sha256:b97c1fac8c49be29486df85968682b0afa77e1b809aff74b83081cc115e52f33"},
-    {file = "pydantic-1.10.13-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:c958d053453a1c4b1c2062b05cd42d9d5c8eb67537b8d5a7e3c3032943ecd261"},
-    {file = "pydantic-1.10.13-cp38-cp38-macosx_11_0_arm64.whl", hash = "sha256:4c5370a7edaac06daee3af1c8b1192e305bc102abcbf2a92374b5bc793818599"},
-    {file = "pydantic-1.10.13-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:7d6f6e7305244bddb4414ba7094ce910560c907bdfa3501e9db1a7fd7eaea127"},
-    {file = "pydantic-1.10.13-cp38-cp38-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:d3a3c792a58e1622667a2837512099eac62490cdfd63bd407993aaf200a4cf1f"},
-    {file = "pydantic-1.10.13-cp38-cp38-musllinux_1_1_i686.whl", hash = "sha256:c636925f38b8db208e09d344c7aa4f29a86bb9947495dd6b6d376ad10334fb78"},
-    {file = "pydantic-1.10.13-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:678bcf5591b63cc917100dc50ab6caebe597ac67e8c9ccb75e698f66038ea953"},
-    {file = "pydantic-1.10.13-cp38-cp38-win_amd64.whl", hash = "sha256:6cf25c1a65c27923a17b3da28a0bdb99f62ee04230c931d83e888012851f4e7f"},
-    {file = "pydantic-1.10.13-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:8ef467901d7a41fa0ca6db9ae3ec0021e3f657ce2c208e98cd511f3161c762c6"},
-    {file = "pydantic-1.10.13-cp39-cp39-macosx_11_0_arm64.whl", hash = "sha256:968ac42970f57b8344ee08837b62f6ee6f53c33f603547a55571c954a4225691"},
-    {file = "pydantic-1.10.13-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:9849f031cf8a2f0a928fe885e5a04b08006d6d41876b8bbd2fc68a18f9f2e3fd"},
-    {file = "pydantic-1.10.13-cp39-cp39-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:56e3ff861c3b9c6857579de282ce8baabf443f42ffba355bf070770ed63e11e1"},
-    {file = "pydantic-1.10.13-cp39-cp39-musllinux_1_1_i686.whl", hash = "sha256:9f00790179497767aae6bcdc36355792c79e7bbb20b145ff449700eb076c5f96"},
-    {file = "pydantic-1.10.13-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:75b297827b59bc229cac1a23a2f7a4ac0031068e5be0ce385be1462e7e17a35d"},
-    {file = "pydantic-1.10.13-cp39-cp39-win_amd64.whl", hash = "sha256:e70ca129d2053fb8b728ee7d1af8e553a928d7e301a311094b8a0501adc8763d"},
-    {file = "pydantic-1.10.13-py3-none-any.whl", hash = "sha256:b87326822e71bd5f313e7d3bfdc77ac3247035ac10b0c0618bd99dcf95b1e687"},
-    {file = "pydantic-1.10.13.tar.gz", hash = "sha256:32c8b48dcd3b2ac4e78b0ba4af3a2c2eb6048cb75202f0ea7b34feb740efc340"},
+    {file = "pydantic-1.10.14-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:7f4fcec873f90537c382840f330b90f4715eebc2bc9925f04cb92de593eae054"},
+    {file = "pydantic-1.10.14-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:8e3a76f571970fcd3c43ad982daf936ae39b3e90b8a2e96c04113a369869dc87"},
+    {file = "pydantic-1.10.14-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:82d886bd3c3fbeaa963692ef6b643159ccb4b4cefaf7ff1617720cbead04fd1d"},
+    {file = "pydantic-1.10.14-cp310-cp310-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:798a3d05ee3b71967844a1164fd5bdb8c22c6d674f26274e78b9f29d81770c4e"},
+    {file = "pydantic-1.10.14-cp310-cp310-musllinux_1_1_i686.whl", hash = "sha256:23d47a4b57a38e8652bcab15a658fdb13c785b9ce217cc3a729504ab4e1d6bc9"},
+    {file = "pydantic-1.10.14-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:f9f674b5c3bebc2eba401de64f29948ae1e646ba2735f884d1594c5f675d6f2a"},
+    {file = "pydantic-1.10.14-cp310-cp310-win_amd64.whl", hash = "sha256:24a7679fab2e0eeedb5a8924fc4a694b3bcaac7d305aeeac72dd7d4e05ecbebf"},
+    {file = "pydantic-1.10.14-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:9d578ac4bf7fdf10ce14caba6f734c178379bd35c486c6deb6f49006e1ba78a7"},
+    {file = "pydantic-1.10.14-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:fa7790e94c60f809c95602a26d906eba01a0abee9cc24150e4ce2189352deb1b"},
+    {file = "pydantic-1.10.14-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:aad4e10efa5474ed1a611b6d7f0d130f4aafadceb73c11d9e72823e8f508e663"},
+    {file = "pydantic-1.10.14-cp311-cp311-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:1245f4f61f467cb3dfeced2b119afef3db386aec3d24a22a1de08c65038b255f"},
+    {file = "pydantic-1.10.14-cp311-cp311-musllinux_1_1_i686.whl", hash = "sha256:21efacc678a11114c765eb52ec0db62edffa89e9a562a94cbf8fa10b5db5c046"},
+    {file = "pydantic-1.10.14-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:412ab4a3f6dbd2bf18aefa9f79c7cca23744846b31f1d6555c2ee2b05a2e14ca"},
+    {file = "pydantic-1.10.14-cp311-cp311-win_amd64.whl", hash = "sha256:e897c9f35281f7889873a3e6d6b69aa1447ceb024e8495a5f0d02ecd17742a7f"},
+    {file = "pydantic-1.10.14-cp37-cp37m-macosx_10_9_x86_64.whl", hash = "sha256:d604be0f0b44d473e54fdcb12302495fe0467c56509a2f80483476f3ba92b33c"},
+    {file = "pydantic-1.10.14-cp37-cp37m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:a42c7d17706911199798d4c464b352e640cab4351efe69c2267823d619a937e5"},
+    {file = "pydantic-1.10.14-cp37-cp37m-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:596f12a1085e38dbda5cbb874d0973303e34227b400b6414782bf205cc14940c"},
+    {file = "pydantic-1.10.14-cp37-cp37m-musllinux_1_1_i686.whl", hash = "sha256:bfb113860e9288d0886e3b9e49d9cf4a9d48b441f52ded7d96db7819028514cc"},
+    {file = "pydantic-1.10.14-cp37-cp37m-musllinux_1_1_x86_64.whl", hash = "sha256:bc3ed06ab13660b565eed80887fcfbc0070f0aa0691fbb351657041d3e874efe"},
+    {file = "pydantic-1.10.14-cp37-cp37m-win_amd64.whl", hash = "sha256:ad8c2bc677ae5f6dbd3cf92f2c7dc613507eafe8f71719727cbc0a7dec9a8c01"},
+    {file = "pydantic-1.10.14-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:c37c28449752bb1f47975d22ef2882d70513c546f8f37201e0fec3a97b816eee"},
+    {file = "pydantic-1.10.14-cp38-cp38-macosx_11_0_arm64.whl", hash = "sha256:49a46a0994dd551ec051986806122767cf144b9702e31d47f6d493c336462597"},
+    {file = "pydantic-1.10.14-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:53e3819bd20a42470d6dd0fe7fc1c121c92247bca104ce608e609b59bc7a77ee"},
+    {file = "pydantic-1.10.14-cp38-cp38-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:0fbb503bbbbab0c588ed3cd21975a1d0d4163b87e360fec17a792f7d8c4ff29f"},
+    {file = "pydantic-1.10.14-cp38-cp38-musllinux_1_1_i686.whl", hash = "sha256:336709883c15c050b9c55a63d6c7ff09be883dbc17805d2b063395dd9d9d0022"},
+    {file = "pydantic-1.10.14-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:4ae57b4d8e3312d486e2498d42aed3ece7b51848336964e43abbf9671584e67f"},
+    {file = "pydantic-1.10.14-cp38-cp38-win_amd64.whl", hash = "sha256:dba49d52500c35cfec0b28aa8b3ea5c37c9df183ffc7210b10ff2a415c125c4a"},
+    {file = "pydantic-1.10.14-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:c66609e138c31cba607d8e2a7b6a5dc38979a06c900815495b2d90ce6ded35b4"},
+    {file = "pydantic-1.10.14-cp39-cp39-macosx_11_0_arm64.whl", hash = "sha256:d986e115e0b39604b9eee3507987368ff8148222da213cd38c359f6f57b3b347"},
+    {file = "pydantic-1.10.14-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:646b2b12df4295b4c3148850c85bff29ef6d0d9621a8d091e98094871a62e5c7"},
+    {file = "pydantic-1.10.14-cp39-cp39-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:282613a5969c47c83a8710cc8bfd1e70c9223feb76566f74683af889faadc0ea"},
+    {file = "pydantic-1.10.14-cp39-cp39-musllinux_1_1_i686.whl", hash = "sha256:466669501d08ad8eb3c4fecd991c5e793c4e0bbd62299d05111d4f827cded64f"},
+    {file = "pydantic-1.10.14-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:13e86a19dca96373dcf3190fcb8797d40a6f12f154a244a8d1e8e03b8f280593"},
+    {file = "pydantic-1.10.14-cp39-cp39-win_amd64.whl", hash = "sha256:08b6ec0917c30861e3fe71a93be1648a2aa4f62f866142ba21670b24444d7fd8"},
+    {file = "pydantic-1.10.14-py3-none-any.whl", hash = "sha256:8ee853cd12ac2ddbf0ecbac1c289f95882b2d4482258048079d13be700aa114c"},
+    {file = "pydantic-1.10.14.tar.gz", hash = "sha256:46f17b832fe27de7850896f3afee50ea682220dd218f7e9c88d436788419dca6"},
 ]
 
 [package.dependencies]
 typing-extensions = ">=4.2.0"
 
 [package.extras]
 dotenv = ["python-dotenv (>=0.10.4)"]
 email = ["email-validator (>=1.0.3)"]
 
 [[package]]
 name = "python-dateutil"
-version = "2.8.2"
+version = "2.9.0.post0"
 description = "Extensions to the standard Python datetime module"
 optional = false
 python-versions = "!=3.0.*,!=3.1.*,!=3.2.*,>=2.7"
 files = [
-    {file = "python-dateutil-2.8.2.tar.gz", hash = "sha256:0123cacc1627ae19ddf3c27a5de5bd67ee4586fbdd6440d9748f8abb483d3e86"},
-    {file = "python_dateutil-2.8.2-py2.py3-none-any.whl", hash = "sha256:961d03dc3453ebbc59dbdea9e4e11c5651520a876d0f4db161e8674aae935da9"},
+    {file = "python-dateutil-2.9.0.post0.tar.gz", hash = "sha256:37dd54208da7e1cd875388217d5e00ebd4179249f90fb72437e91a35459a0ad3"},
+    {file = "python_dateutil-2.9.0.post0-py2.py3-none-any.whl", hash = "sha256:a8b2bc7bffae282281c8140a97d3aa9c14da0b136dfe83f850eea9a5f7470427"},
 ]
 
 [package.dependencies]
 six = ">=1.5"
 
 [[package]]
 name = "pytz"
-version = "2023.3.post1"
+version = "2024.1"
 description = "World timezone definitions, modern and historical"
 optional = false
 python-versions = "*"
 files = [
-    {file = "pytz-2023.3.post1-py2.py3-none-any.whl", hash = "sha256:ce42d816b81b68506614c11e8937d3aa9e41007ceb50bfdcb0749b921bf646c7"},
-    {file = "pytz-2023.3.post1.tar.gz", hash = "sha256:7b4fddbeb94a1eba4b557da24f19fdf9db575192544270a9101d8509f9f43d7b"},
+    {file = "pytz-2024.1-py2.py3-none-any.whl", hash = "sha256:328171f4e3623139da4983451950b28e95ac706e13f3f2630a879749e7a8b319"},
+    {file = "pytz-2024.1.tar.gz", hash = "sha256:2a29735ea9c18baf14b448846bde5a48030ed267578472d8955cd0e7443a9812"},
 ]
 
 [[package]]
 name = "requests"
 version = "2.31.0"
 description = "Python HTTP for Humans."
 optional = false
@@ -547,21 +465,21 @@
 
 [package.extras]
 socks = ["PySocks (>=1.5.6,!=1.5.7)"]
 use-chardet-on-py3 = ["chardet (>=3.0.2,<6)"]
 
 [[package]]
 name = "requests-oauthlib"
-version = "1.3.1"
+version = "2.0.0"
 description = "OAuthlib authentication support for Requests."
 optional = false
-python-versions = ">=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*"
+python-versions = ">=3.4"
 files = [
-    {file = "requests-oauthlib-1.3.1.tar.gz", hash = "sha256:75beac4a47881eeb94d5ea5d6ad31ef88856affe2332b9aafb52c6452ccf0d7a"},
-    {file = "requests_oauthlib-1.3.1-py2.py3-none-any.whl", hash = "sha256:2577c501a2fb8d05a304c09d090d6e47c306fef15809d102b327cf8364bddab5"},
+    {file = "requests-oauthlib-2.0.0.tar.gz", hash = "sha256:b3dffaebd884d8cd778494369603a9e7b58d29111bf6b41bdc2dcd87203af4e9"},
+    {file = "requests_oauthlib-2.0.0-py2.py3-none-any.whl", hash = "sha256:7dd8a5c40426b779b0868c404bdef9768deccf22749cde15852df527e6269b36"},
 ]
 
 [package.dependencies]
 oauthlib = ">=3.0.0"
 requests = ">=2.0.0"
 
 [package.extras]
@@ -590,49 +508,52 @@
 files = [
     {file = "six-1.16.0-py2.py3-none-any.whl", hash = "sha256:8abb2f1d86890a2dfb989f9a77cfcfd3e47c2a354b01111771326f8aa26e0254"},
     {file = "six-1.16.0.tar.gz", hash = "sha256:1e61c37477a1626458e36f7b1d82aa5c9b094fa4802892072e49de9c60c4c926"},
 ]
 
 [[package]]
 name = "turbinia-api-lib"
-version = "1.0.2"
+version = "1.0.3"
 description = "Turbinia API Server"
 optional = false
-python-versions = ">=3.7,<4.0"
+python-versions = ">=3.9,<4.0"
 files = [
-    {file = "turbinia_api_lib-1.0.2-py3-none-any.whl", hash = "sha256:04b3f471fb01046d81031cc0f95e5368f855647251eb7823dad00d0c07f8f80b"},
-    {file = "turbinia_api_lib-1.0.2.tar.gz", hash = "sha256:b1885c43987591294c0beacd03732fb07decb5608f0c69a3158ead178f3c6b9e"},
+    {file = "turbinia_api_lib-1.0.3-py3-none-any.whl", hash = "sha256:93aceb3c2eb99d718cb793b1a01445cc4643d43076de037ae85191e047d3163c"},
+    {file = "turbinia_api_lib-1.0.3.tar.gz", hash = "sha256:b8ee44ee85b0b4b92976a0ee57c2d6d54c6b5f8c85abf94235b790f314150372"},
 ]
 
 [package.dependencies]
 aenum = ">=3.1.11"
 pydantic = ">=1.10.5,<2.0.0"
 python-dateutil = ">=2.8.2"
-urllib3 = ">=1.25.3,<2"
+urllib3 = [
+    {version = ">=1.25.4,<1.27", markers = "python_version < \"3.10\""},
+    {version = ">=1.25.4,<2.1", markers = "python_version >= \"3.10\""},
+]
 
 [[package]]
 name = "typing-extensions"
-version = "4.8.0"
+version = "4.10.0"
 description = "Backported and Experimental Type Hints for Python 3.8+"
 optional = false
 python-versions = ">=3.8"
 files = [
-    {file = "typing_extensions-4.8.0-py3-none-any.whl", hash = "sha256:8f92fc8806f9a6b641eaa5318da32b44d401efaac0f6678c9bc448ba3605faa0"},
-    {file = "typing_extensions-4.8.0.tar.gz", hash = "sha256:df8e4339e9cb77357558cbdbceca33c303714cf861d1eef15e1070055ae8b7ef"},
+    {file = "typing_extensions-4.10.0-py3-none-any.whl", hash = "sha256:69b1a937c3a517342112fb4c6df7e72fc39a38e7891a5730ed4985b5214b5475"},
+    {file = "typing_extensions-4.10.0.tar.gz", hash = "sha256:b0abd7c89e8fb96f98db18d86106ff1d90ab692004eb746cf6eda2682f91b3cb"},
 ]
 
 [[package]]
 name = "tzdata"
-version = "2023.3"
+version = "2024.1"
 description = "Provider of IANA time zone data"
 optional = false
 python-versions = ">=2"
 files = [
-    {file = "tzdata-2023.3-py2.py3-none-any.whl", hash = "sha256:7e65763eef3120314099b6939b5546db7adce1e7d6f2e179e3df563c70511eda"},
-    {file = "tzdata-2023.3.tar.gz", hash = "sha256:11ef1e08e54acb0d4f95bdb1be05da659673de4acbd21bf9c69e94cc5e907a3a"},
+    {file = "tzdata-2024.1-py2.py3-none-any.whl", hash = "sha256:9068bc196136463f5245e51efda838afa15aaeca9903f49050dfa2679db4d252"},
+    {file = "tzdata-2024.1.tar.gz", hash = "sha256:2674120f8d891909751c38abcdfd386ac0a5a1127954fbc332af6b5ceae07efd"},
 ]
 
 [[package]]
 name = "urllib3"
 version = "1.26.18"
 description = "HTTP library with thread-safe connection pooling, file post, and more."
 optional = false
@@ -643,11 +564,28 @@
 ]
 
 [package.extras]
 brotli = ["brotli (==1.0.9)", "brotli (>=1.0.9)", "brotlicffi (>=0.8.0)", "brotlipy (>=0.6.0)"]
 secure = ["certifi", "cryptography (>=1.3.4)", "idna (>=2.0.0)", "ipaddress", "pyOpenSSL (>=0.14)", "urllib3-secure-extra"]
 socks = ["PySocks (>=1.5.6,!=1.5.7,<2.0)"]
 
+[[package]]
+name = "urllib3"
+version = "2.0.7"
+description = "HTTP library with thread-safe connection pooling, file post, and more."
+optional = false
+python-versions = ">=3.7"
+files = [
+    {file = "urllib3-2.0.7-py3-none-any.whl", hash = "sha256:fdb6d215c776278489906c2f8916e6e7d4f5a9b602ccbcfdf7f016fc8da0596e"},
+    {file = "urllib3-2.0.7.tar.gz", hash = "sha256:c97dfde1f7bd43a71c8d2a58e369e9b2bf692d1334ea9f9cae55add7d0dd0f84"},
+]
+
+[package.extras]
+brotli = ["brotli (>=1.0.9)", "brotlicffi (>=0.8.0)"]
+secure = ["certifi", "cryptography (>=1.9)", "idna (>=2.0.0)", "pyopenssl (>=17.1.0)", "urllib3-secure-extra"]
+socks = ["pysocks (>=1.5.6,!=1.5.7,<2.0)"]
+zstd = ["zstandard (>=0.18.0)"]
+
 [metadata]
 lock-version = "2.0"
 python-versions = "^3.9"
-content-hash = "fd61f76bd449559541e8f462cf98e29fcdf4b12676512227b3e8f702783d7af6"
+content-hash = "a4a664abc86733d9bcd43fc4a7cc58f6f8ccaab52953d79fc020c95ccdbbd401"
```

### Comparing `turbinia-20240313/turbinia/api/cli/pyproject.toml` & `turbinia-20240412.1/turbinia/api/cli/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "turbinia-client"
-version = "1.0.5"
+version = "1.0.6"
 description = "Turbinia command-line tool"
 authors = ["Turbinia Developers <turbinia-dev@googlegroups.com>"]
 maintainers = ["Turbinia Developers <turbinia-dev@googlegroups.com>"]
 license = "Apache-2.0"
 readme = "README.rst"
 repository = "https://github.com/google/turbinia"
 documentation = "https://turbinia.readthedocs.io/en/latest/"
```

### Comparing `turbinia-20240313/turbinia/api/cli/requirements.txt` & `turbinia-20240412.1/turbinia/api/cli/requirements.txt`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/api/cli/turbinia_client/__init__.py` & `turbinia-20240412.1/turbinia/api/cli/turbinia_client/__init__.py`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/api/cli/turbinia_client/core/__init__.py` & `turbinia-20240412.1/turbinia/api/cli/turbinia_client/core/__init__.py`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/api/cli/turbinia_client/core/commands.py` & `turbinia-20240412.1/turbinia/api/cli/turbinia_client/core/commands.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 from turbinia_api_lib.api import turbinia_configuration_api
 from turbinia_api_lib.api import turbinia_jobs_api
 from turbinia_api_lib.api import turbinia_request_results_api
 from turbinia_api_lib.api import turbinia_evidence_api
 from turbinia_client.core import groups
 from turbinia_client.helpers import formatter
 
-log = logging.getLogger('turbinia')
+log = logging.getLogger(__name__)
 
 
 @groups.config_group.command('list')
 @click.pass_context
 def get_config(ctx: click.Context) -> None:
   """Gets Turbinia server configuration."""
   client: api_client.ApiClient = ctx.obj.api_client
@@ -45,61 +45,102 @@
   try:
     api_response = api_instance.read_config_with_http_info()
     decoded_response = formatter.decode_api_response(api_response)
     formatter.echo_json(decoded_response)
   except exceptions.ApiException as exception:
     log.error(
         f'Received status code {exception.status} '
-        f'when calling get_config: {exception.body}')
+        f'when calling read_config_with_http_info: {exception.body}')
+
+
+@groups.config_group.command('version')
+@click.pass_context
+def get_api_server_version(ctx: click.Context) -> None:
+  """Gets Turbinia API server version."""
+  client: api_client.ApiClient = ctx.obj.api_client
+  api_instance = turbinia_configuration_api.TurbiniaConfigurationApi(client)
+  try:
+    api_response = api_instance.get_version()
+    decoded_response = formatter.decode_api_response(api_response)
+    formatter.echo_json(decoded_response)
+  except exceptions.ApiException as exception:
+    log.error(
+        f'Received status code {exception.status} '
+        f'when calling get_version: {exception.body}')
 
 
 @groups.result_group.command('request')
 @click.pass_context
 @click.argument('request_id')
 def get_request_result(ctx: click.Context, request_id: str) -> None:
   """Gets Turbinia request results / output files."""
   client: api_client.ApiClient = ctx.obj.api_client
   api_instance = turbinia_request_results_api.TurbiniaRequestResultsApi(client)
   filename = f'{request_id}.tgz'
+  click.echo(f'Downloading output for request {request_id} to: {filename}')
   try:
     api_response = api_instance.get_request_output_with_http_info(
-        request_id, _preload_content=False, _request_timeout=(30, 300))
-    click.echo(f'Saving output for request {request_id} to: {filename}')
+        request_id, _preload_content=False, _request_timeout=(30, 900))
     # Read the response and save into a local file.
     with open(filename, 'wb') as file:
       file.write(api_response.raw_data)
   except exceptions.ApiException as exception:
     log.error(
         f'Received status code {exception.status} '
-        f'when calling get_request_output: {exception.body}')
+        f'when calling get_request_output_with_http_info: {exception.body}')
   except OSError as exception:
     log.error(f'Unable to save file: {exception}')
   except (ValueError, tarfile.ReadError, tarfile.CompressionError) as exception:
     log.error(f'Error reading saved results file {filename}: {exception}')
 
 
 @groups.result_group.command('task')
 @click.pass_context
 @click.argument('task_id')
 def get_task_result(ctx: click.Context, task_id: str) -> None:
   """Gets Turbinia task results / output files."""
   client: api_client.ApiClient = ctx.obj.api_client
   api_instance = turbinia_request_results_api.TurbiniaRequestResultsApi(client)
   filename = f'{task_id}.tgz'
+  click.echo(f'Downloading output for task {task_id} to: {filename}')
   try:
     api_response = api_instance.get_task_output_with_http_info(
-        task_id, _preload_content=False, _request_timeout=(30, 300))
-    click.echo(f'Saving output for task {task_id} to: {filename}')
+        task_id, _preload_content=False, _request_timeout=(30, 900))
+    # Read the response and save into a local file.
+    with open(filename, 'wb') as file:
+      file.write(api_response.raw_data)
+  except exceptions.ApiException as exception:
+    log.error(
+        f'Received status code {exception.status} '
+        f'when calling get_task_output_with_http_info: {exception.body}')
+  except OSError as exception:
+    log.error(f'Unable to save file: {exception}')
+  except (ValueError, tarfile.ReadError, tarfile.CompressionError) as exception:
+    log.error(f'Error reading saved results file {filename}: {exception}')
+
+
+@groups.result_group.command('plasofile')
+@click.pass_context
+@click.argument('task_id')
+def get_plaso_file(ctx: click.Context, task_id: str) -> None:
+  """Gets Turbinia task results / output files."""
+  client: api_client.ApiClient = ctx.obj.api_client
+  api_instance = turbinia_request_results_api.TurbiniaRequestResultsApi(client)
+  filename = f'{task_id}.plaso'
+  click.echo(f'Downloading output for task {task_id} to: {filename}')
+  try:
+    api_response = api_instance.get_plaso_file_with_http_info(
+        task_id, _preload_content=False, _request_timeout=(30, 900))
     # Read the response and save into a local file.
     with open(filename, 'wb') as file:
       file.write(api_response.raw_data)
   except exceptions.ApiException as exception:
     log.error(
         f'Received status code {exception.status} '
-        f'when calling get_task_output: {exception.body}')
+        f'when calling get_plaso_file_with_http_info: {exception.body}')
   except OSError as exception:
     log.error(f'Unable to save file: {exception}')
   except (ValueError, tarfile.ReadError, tarfile.CompressionError) as exception:
     log.error(f'Error reading saved results file {filename}: {exception}')
 
 
 @groups.jobs_group.command('list')
@@ -111,15 +152,15 @@
   try:
     api_response = api_instance.read_jobs_with_http_info()
     decoded_response = formatter.decode_api_response(api_response)
     formatter.echo_json(decoded_response)
   except exceptions.ApiException as exception:
     log.error(
         f'Received status code {exception.status} '
-        f'when calling read_jobs: {exception.body}')
+        f'when calling read_jobs_with_http_info: {exception.body}')
 
 
 @groups.status_group.command('request')
 @click.pass_context
 @click.argument('request_id')
 @click.option(
     '--priority_filter', '-p', help='This sets what report sections are '
@@ -156,15 +197,15 @@
       report = formatter.RequestMarkdownReport(
           decoded_response).generate_markdown(
               priority_filter=priority_filter, show_all=show_all)
       click.echo(report)
   except exceptions.ApiException as exception:
     log.error(
         f'Received status code {exception.status} '
-        f'when calling get_request_status: {exception.body}')
+        f'when calling get_request_status_with_http_info: {exception.body}')
 
 
 @groups.status_group.command('workers')
 @click.pass_context
 @click.option(
     '--days', '-d', help='Specifies status timeframe.', required=False)
 @click.option(
@@ -189,15 +230,15 @@
     else:
       report = formatter.WorkersMarkdownReport(decoded_response,
                                                days).generate_markdown()
       click.echo(report)
   except exceptions.ApiException as exception:
     log.error(
         f'Received status code {exception.status} '
-        f'when calling get_workers_status: {exception.body}')
+        f'when calling get_workers_status_with_http_info: {exception.body}')
 
 
 @groups.status_group.command('statistics')
 @click.pass_context
 @click.option(
     '--days', '-d', help='Specifies statistics timeframe.', required=False)
 @click.option(
@@ -234,15 +275,15 @@
         report = stat_formatter.generate_csv()
       else:
         report = stat_formatter.generate_markdown()
       click.echo(report)
   except exceptions.ApiException as exception:
     log.error(
         f'Received status code {exception.status} '
-        f'when calling get_task_statistics: {exception.body}')
+        f'when calling get_task_statistics_with_http_info: {exception.body}')
 
 
 @groups.status_group.command('summary')
 @click.pass_context
 @click.option(
     '--json_dump', '-j', help='Generates JSON output.', is_flag=True,
     required=False)
@@ -259,15 +300,15 @@
     else:
       report = formatter.SummaryMarkdownReport(
           decoded_response).generate_markdown()
       click.echo(report)
   except exceptions.ApiException as exception:
     log.error(
         f'Received status code {exception.status} '
-        f'when calling get_requests_summary: {exception.body}')
+        f'when calling get_requests_summary_with_http_info: {exception.body}')
 
 
 @groups.status_group.command('task')
 @click.pass_context
 @click.argument('task_id')
 @click.option(
     '--show_all', '-a', help='Shows all field regardless of priority.',
@@ -288,15 +329,15 @@
     else:
       report = formatter.TaskMarkdownReport(decoded_response).generate_markdown(
           show_all=show_all, priority_filter=100)
       click.echo(report)
   except exceptions.ApiException as exception:
     log.error(
         f'Received status code {exception.status} '
-        f'when calling get_task_status: {exception.body}')
+        f'when calling get_task_status_with_http_info: {exception.body}')
 
 
 @groups.evidence_group.command('summary')
 @click.pass_context
 @click.option(
     '--group', '-g', help='Attribute by which output will be grouped.',
     default=None, required=False)
@@ -321,15 +362,15 @@
     else:
       report = formatter.EvidenceSummaryMarkdownReport(
           decoded_response).generate_summary_markdown(output)
       click.echo(report)
   except exceptions.ApiException as exception:
     log.error(
         f'Received status code {exception.status} '
-        f'when calling get_evidence_summary: {exception.body}')
+        f'when calling get_evidence_summary_with_http_info: {exception.body}')
 
 
 @groups.evidence_group.command('query')
 @click.pass_context
 @click.argument('attribute_name')
 @click.argument('attribute_value')
 @click.option(
@@ -354,15 +395,15 @@
     else:
       report = formatter.EvidenceSummaryMarkdownReport(
           decoded_response).generate_summary_markdown(output)
       click.echo(report)
   except exceptions.ApiException as exception:
     log.error(
         f'Received status code {exception.status} '
-        f'when calling get_task_status: {exception.body}')
+        f'when calling query_evidence_with_http_info: {exception.body}')
 
 
 @groups.evidence_group.command('get')
 @click.pass_context
 @click.argument('evidence_id')
 @click.option(
     '--show_all', '-a', help='Shows all evidence attributes.', is_flag=True,
@@ -385,15 +426,15 @@
     else:
       report = formatter.EvidenceMarkdownReport(
           decoded_response).generate_markdown(1, show_all=show_all)
       click.echo(report)
   except exceptions.ApiException as exception:
     log.error(
         f'Received status code {exception.status} '
-        f'when calling get_evidence: {exception.body}')
+        f'when calling get_evidence_by_id_with_http_info: {exception.body}')
 
 
 @groups.evidence_group.command('upload')
 @click.pass_context
 @click.argument('ticket_id')
 @click.option(
     '--path', '-p', help='Path of file or directory to be uploaded.',
@@ -439,15 +480,15 @@
     try:
       api_response = api_instance.upload_evidence_with_http_info(
           [file_path], ticket_id, calculate_hash)
       report[abs_path] = formatter.decode_api_response(api_response)
     except exceptions.ApiException as exception:
       error_message = (
           f'Received status code {exception.status} '
-          f'when calling upload_evidence: {exception}')
+          f'when calling upload_evidence_with_http_info: {exception}')
       log.error(error_message)
       report[abs_path] = error_message
   if json_dump:
     formatter.echo_json(report)
   else:
     report = '\n'.join(
         formatter.EvidenceMarkdownReport({}).dict_to_markdown(
```

### Comparing `turbinia-20240313/turbinia/api/cli/turbinia_client/core/groups.py` & `turbinia-20240412.1/turbinia/api/cli/turbinia_client/core/groups.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import click
 import logging
 import sys
 
 from turbinia_api_lib import exceptions
 from turbinia_client.factory import factory
 
-log = logging.getLogger('turbinia')
+log = logging.getLogger(__name__)
 
 
 @click.group('config')
 def config_group():
   """Get Turbinia configuration."""
```

### Comparing `turbinia-20240313/turbinia/api/cli/turbinia_client/factory/__init__.py` & `turbinia-20240412.1/turbinia/api/cli/turbinia_client/factory/__init__.py`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/api/cli/turbinia_client/factory/factory.py` & `turbinia-20240412.1/turbinia/api/cli/turbinia_client/factory/factory.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 import logging
 import click
 
 from turbinia_client.helpers import click_helper
 
 T = TypeVar('T', bound='FactoryInterface')
 
-log = logging.getLogger('turbinia')
+log = logging.getLogger(__name__)
 
 
 class FactoryInterface(ABC):
   """Factory Interface."""
 
   @classmethod
   def get_evidence_attributes(
```

### Comparing `turbinia-20240313/turbinia/api/cli/turbinia_client/helpers/__init__.py` & `turbinia-20240412.1/turbinia/api/cli/turbinia_client/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/api/cli/turbinia_client/helpers/auth_helper.py` & `turbinia-20240412.1/turbinia/api/cli/turbinia_client/helpers/auth_helper.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 import sys
 
 from google_auth_oauthlib import flow
 from google.oauth2.credentials import Credentials
 from google.auth.transport.requests import Request
 from google.auth import exceptions as google_exceptions
 
-log = logging.getLogger('turbinia')
+log = logging.getLogger(__name__)
 
 
 def get_oauth2_token_id(credentials_path, client_secrets_path):
   """Authenticates the user using Google OAuth and get ID Token."""
   scopes = ['openid', 'https://www.googleapis.com/auth/userinfo.email']
   credentials = None
```

### Comparing `turbinia-20240313/turbinia/api/cli/turbinia_client/helpers/click_helper.py` & `turbinia-20240412.1/turbinia/api/cli/turbinia_client/helpers/click_helper.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 from typing import Tuple, Sequence
 from turbinia_api_lib.api import turbinia_configuration_api
 from turbinia_api_lib.api import turbinia_requests_api
 
 from turbinia_api_lib import exceptions
 from turbinia_api_lib import api_client
 
-log = logging.getLogger('turbinia')
+log = logging.getLogger(__name__)
 
 
 def generate_option_parameters(
     option_name: str) -> Tuple[Tuple[Sequence[str], str], dict]:
   """Builds click.Option or click.Command arguments based on a given parameter 
       name.
   """
@@ -111,16 +111,16 @@
     # from the request so that we only have recipe_data.
     request['request_options'].pop('recipe_name')
     # recipe_data should be a UTF-8 encoded string.
     request['request_options']['recipe_data'] = recipe_data.decode('utf-8')
 
   # Send the request to the API server.
   try:
-    log.info(f'Sending request: {request}')
+    click.echo(f'Sending request: {request}')
     api_response = api_instance.create_request(request)
-    log.info(f'Received response: {api_response}')
+    click.echo(f'Received response: {api_response}')
   except exceptions.ApiException as exception:
     log.error(
         f'Received status code {exception.status} '
         f'when calling create_request: {exception.body}')
   except (TypeError, exceptions.ApiTypeError) as exception:
     log.error(f'The request object is invalid. {exception}')
```

### Comparing `turbinia-20240313/turbinia/api/cli/turbinia_client/helpers/formatter.py` & `turbinia-20240412.1/turbinia/api/cli/turbinia_client/helpers/formatter.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 import json
 import pandas
 
 MEDIUM_PRIORITY = 50
 HIGH_PRIORITY = 20
 CRITICAL_PRIORITY = 10
 
-log = logging.getLogger('turbinia')
+log = logging.getLogger(__name__)
 
 IMPORTANT_ATTRIBUTES = {
     'id', '_name', 'type', 'size', 'request_id', 'tasks', 'source_path',
     'local_path', 'creation_time', 'last_update'
 }
```

### Comparing `turbinia-20240313/turbinia/api/cli/turbinia_client/helpers/formatter_test.py` & `turbinia-20240412.1/turbinia/api/cli/turbinia_client/helpers/formatter_test.py`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/api/cli/turbinia_client/turbiniacli.py` & `turbinia-20240412.1/turbinia/api/cli/turbinia_client/turbiniacli.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 from turbinia_api_lib.api import turbinia_configuration_api
 from turbinia_api_lib.api import turbinia_evidence_api
 
 from turbinia_client.helpers import auth_helper
 from turbinia_client.helpers import formatter
 
-log = logging.getLogger('turbinia')
+log = logging.getLogger(__name__)
 
 
 class TurbiniaCli:
   """Turbinia API client tool.
 
   Attributes:
     _api_client (turbinia_api_lib.ApiClient): An instance of the ApiClient
@@ -152,14 +152,15 @@
   def request_options(self, request_options):
     self._request_options = request_options
 
   def default_api_client(
       self,
       config: turbinia_api_lib.Configuration) -> turbinia_api_lib.ApiClient:
     """Default value for API client instance."""
+    config.retries = 3
     return turbinia_api_lib.ApiClient(configuration=config)
 
   def default_config(self, host: str) -> turbinia_api_lib.Configuration:
     """Default value for API client configuration."""
     return turbinia_api_lib.Configuration(host=host)
 
   def get_evidence_arguments(self, evidence_name=None) -> dict[str, str]:
```

### Comparing `turbinia-20240313/turbinia/api/cli/turbinia_client/turbiniacli_test.py` & `turbinia-20240412.1/turbinia/api/cli/turbinia_client/turbiniacli_test.py`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/api/cli/turbinia_client/turbiniacli_tool.py` & `turbinia-20240412.1/turbinia/api/cli/turbinia_client/turbiniacli_tool.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 from turbinia_client.turbiniacli import TurbiniaCli
 from turbinia_client.core import groups
 from turbinia_client.core.commands import version
 
 _LOGGER_FORMAT = '%(asctime)s %(levelname)s %(name)s - %(message)s'
 logging.basicConfig(format=_LOGGER_FORMAT, level=logging.INFO)
-log = logging.getLogger('turbinia')
+log = logging.getLogger(__name__)
 
 
 @click.group(context_settings={
     'help_option_names': ['-h', '--help'],
 })
 @click.option(
     '--config_instance', '-c', help='A Turbinia instance configuration name.',
```

### Comparing `turbinia-20240313/turbinia/api/client/.github/workflows/python.yml` & `turbinia-20240412.1/turbinia/api/client/.github/workflows/python.yml`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/api/client/.gitignore` & `turbinia-20240412.1/turbinia/api/client/.gitignore`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/api/client/.gitlab-ci.yml` & `turbinia-20240412.1/turbinia/api/client/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/api/client/.openapi-generator-ignore` & `turbinia-20240412.1/turbinia/api/client/.openapi-generator-ignore`

 * *Files 26% similar despite different names*

```diff
@@ -16,8 +16,16 @@
 #foo/**/qux
 # This matches foo/bar/qux, foo/baz/qux, and foo/bar/baz/qux
 
 # You can also negate patterns with an exclamation (!).
 # For example, you can ignore all files in a docs folder with the file extension .md:
 #docs/*.md
 # Then explicitly reverse the ignore rule for a single file:
-#!docs/README.md
+#!docs/README.md
+
+pyproject.toml
+setup.py
+setup.cfg
+*requirements.txt
+test/*
+.openapi-generator-ignore
+LICENSE
```

### Comparing `turbinia-20240313/turbinia/api/client/LICENSE` & `turbinia-20240412.1/turbinia/api/client/LICENSE`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/api/client/README.md` & `turbinia-20240412.1/turbinia/api/client/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # turbinia-api-lib
 Turbinia is an open-source framework for deploying, managing, and running distributed forensic workloads
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 - API version: 1.0.0
 - Package version: 1.0.0
+- Generator version: 7.4.0
 - Build package: org.openapitools.codegen.languages.PythonPydanticV1ClientCodegen
 
 ## Requirements.
 
 Python 3.7+
 
 ## Installation & Usage
@@ -87,23 +88,25 @@
 ## Documentation for API Endpoints
 
 All URIs are relative to *http://localhost*
 
 Class | Method | HTTP request | Description
 ------------ | ------------- | ------------- | -------------
 *TurbiniaConfigurationApi* | [**get_request_options**](docs/TurbiniaConfigurationApi.md#get_request_options) | **GET** /api/config/request_options | Get Request Options
+*TurbiniaConfigurationApi* | [**get_version**](docs/TurbiniaConfigurationApi.md#get_version) | **GET** /api/config/version | Get Version
 *TurbiniaConfigurationApi* | [**read_config**](docs/TurbiniaConfigurationApi.md#read_config) | **GET** /api/config/ | Read Config
 *TurbiniaEvidenceApi* | [**get_evidence_attributes**](docs/TurbiniaEvidenceApi.md#get_evidence_attributes) | **GET** /api/evidence/types/{evidence_type} | Get Evidence Attributes
 *TurbiniaEvidenceApi* | [**get_evidence_by_id**](docs/TurbiniaEvidenceApi.md#get_evidence_by_id) | **GET** /api/evidence/{evidence_id} | Get Evidence By Id
 *TurbiniaEvidenceApi* | [**get_evidence_summary**](docs/TurbiniaEvidenceApi.md#get_evidence_summary) | **GET** /api/evidence/summary | Get Evidence Summary
 *TurbiniaEvidenceApi* | [**get_evidence_types**](docs/TurbiniaEvidenceApi.md#get_evidence_types) | **GET** /api/evidence/types | Get Evidence Types
 *TurbiniaEvidenceApi* | [**query_evidence**](docs/TurbiniaEvidenceApi.md#query_evidence) | **GET** /api/evidence/query | Query Evidence
 *TurbiniaEvidenceApi* | [**upload_evidence**](docs/TurbiniaEvidenceApi.md#upload_evidence) | **POST** /api/evidence/upload | Upload Evidence
 *TurbiniaJobsApi* | [**read_jobs**](docs/TurbiniaJobsApi.md#read_jobs) | **GET** /api/jobs/ | Read Jobs
 *TurbiniaLogsApi* | [**get_logs**](docs/TurbiniaLogsApi.md#get_logs) | **GET** /api/logs/{query} | Get Logs
+*TurbiniaRequestResultsApi* | [**get_plaso_file**](docs/TurbiniaRequestResultsApi.md#get_plaso_file) | **GET** /api/result/plasofile/{task_id} | Get Plaso File
 *TurbiniaRequestResultsApi* | [**get_request_output**](docs/TurbiniaRequestResultsApi.md#get_request_output) | **GET** /api/result/request/{request_id} | Get Request Output
 *TurbiniaRequestResultsApi* | [**get_task_output**](docs/TurbiniaRequestResultsApi.md#get_task_output) | **GET** /api/result/task/{task_id} | Get Task Output
 *TurbiniaRequestsApi* | [**create_request**](docs/TurbiniaRequestsApi.md#create_request) | **POST** /api/request/ | Create Request
 *TurbiniaRequestsApi* | [**get_request_status**](docs/TurbiniaRequestsApi.md#get_request_status) | **GET** /api/request/{request_id} | Get Request Status
 *TurbiniaRequestsApi* | [**get_requests_summary**](docs/TurbiniaRequestsApi.md#get_requests_summary) | **GET** /api/request/summary | Get Requests Summary
 *TurbiniaTasksApi* | [**get_task_statistics**](docs/TurbiniaTasksApi.md#get_task_statistics) | **GET** /api/task/statistics | Get Task Statistics
 *TurbiniaTasksApi* | [**get_task_status**](docs/TurbiniaTasksApi.md#get_task_status) | **GET** /api/task/{task_id} | Get Task Status
```

### Comparing `turbinia-20240313/turbinia/api/client/docs/BaseRequestOptions.md` & `turbinia-20240412.1/turbinia/api/client/docs/BaseRequestOptions.md`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/api/client/docs/CompleteTurbiniaStats.md` & `turbinia-20240412.1/turbinia/api/client/docs/CompleteTurbiniaStats.md`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/api/client/docs/HTTPValidationError.md` & `turbinia-20240412.1/turbinia/api/client/docs/HTTPValidationError.md`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/api/client/docs/LocationInner.md` & `turbinia-20240412.1/turbinia/api/client/docs/LocationInner.md`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/api/client/docs/Request.md` & `turbinia-20240412.1/turbinia/api/client/docs/Request.md`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/api/client/docs/TurbiniaConfigurationApi.md` & `turbinia-20240412.1/turbinia/api/client/docs/TurbiniaConfigurationApi.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # turbinia_api_lib.TurbiniaConfigurationApi
 
 All URIs are relative to *http://localhost*
 
 Method | HTTP request | Description
 ------------- | ------------- | -------------
 [**get_request_options**](TurbiniaConfigurationApi.md#get_request_options) | **GET** /api/config/request_options | Get Request Options
+[**get_version**](TurbiniaConfigurationApi.md#get_version) | **GET** /api/config/version | Get Version
 [**read_config**](TurbiniaConfigurationApi.md#read_config) | **GET** /api/config/ | Read Config
 
 
 # **get_request_options**
 > object get_request_options()
 
 Get Request Options
@@ -53,14 +54,83 @@
 ```
 
 
 
 ### Parameters
 This endpoint does not need any parameter.
 
+### Return type
+
+**object**
+
+### Authorization
+
+[oAuth2](../README.md#oAuth2)
+
+### HTTP request headers
+
+ - **Content-Type**: Not defined
+ - **Accept**: application/json
+
+### HTTP response details
+| Status code | Description | Response headers |
+|-------------|-------------|------------------|
+**200** | Successful Response |  -  |
+
+[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)
+
+# **get_version**
+> object get_version()
+
+Get Version
+
+Returns the Turbinia version.
+
+### Example
+
+* OAuth Authentication (oAuth2):
+```python
+import time
+import os
+import turbinia_api_lib
+from turbinia_api_lib.rest import ApiException
+from pprint import pprint
+
+# Defining the host is optional and defaults to http://localhost
+# See configuration.py for a list of all supported configuration parameters.
+configuration = turbinia_api_lib.Configuration(
+    host = "http://localhost"
+)
+
+# The client must configure the authentication and authorization parameters
+# in accordance with the API server security policy.
+# Examples for each auth method are provided below, use the example that
+# satisfies your auth use case.
+
+configuration.access_token = os.environ["ACCESS_TOKEN"]
+
+# Enter a context with an instance of the API client
+with turbinia_api_lib.ApiClient(configuration) as api_client:
+    # Create an instance of the API class
+    api_instance = turbinia_api_lib.TurbiniaConfigurationApi(api_client)
+
+    try:
+        # Get Version
+        api_response = api_instance.get_version()
+        print("The response of TurbiniaConfigurationApi->get_version:\n")
+        pprint(api_response)
+    except Exception as e:
+        print("Exception when calling TurbiniaConfigurationApi->get_version: %s\n" % e)
+```
+
+
+
+### Parameters
+This endpoint does not need any parameter.
+
 ### Return type
 
 **object**
 
 ### Authorization
 
 [oAuth2](../README.md#oAuth2)
```

### Comparing `turbinia-20240313/turbinia/api/client/docs/TurbiniaEvidenceApi.md` & `turbinia-20240412.1/turbinia/api/client/docs/TurbiniaEvidenceApi.md`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/api/client/docs/TurbiniaJobsApi.md` & `turbinia-20240412.1/turbinia/api/client/docs/TurbiniaJobsApi.md`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/api/client/docs/TurbiniaLogsApi.md` & `turbinia-20240412.1/turbinia/api/client/docs/TurbiniaLogsApi.md`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/api/client/docs/TurbiniaRequestResultsApi.md` & `turbinia-20240412.1/turbinia/api/client/docs/TurbiniaRequestResultsApi.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,17 +1,90 @@
 # turbinia_api_lib.TurbiniaRequestResultsApi
 
 All URIs are relative to *http://localhost*
 
 Method | HTTP request | Description
 ------------- | ------------- | -------------
+[**get_plaso_file**](TurbiniaRequestResultsApi.md#get_plaso_file) | **GET** /api/result/plasofile/{task_id} | Get Plaso File
 [**get_request_output**](TurbiniaRequestResultsApi.md#get_request_output) | **GET** /api/result/request/{request_id} | Get Request Output
 [**get_task_output**](TurbiniaRequestResultsApi.md#get_task_output) | **GET** /api/result/task/{task_id} | Get Task Output
 
 
+# **get_plaso_file**
+> bytearray get_plaso_file(task_id)
+
+Get Plaso File
+
+### Example
+
+* OAuth Authentication (oAuth2):
+```python
+import time
+import os
+import turbinia_api_lib
+from turbinia_api_lib.rest import ApiException
+from pprint import pprint
+
+# Defining the host is optional and defaults to http://localhost
+# See configuration.py for a list of all supported configuration parameters.
+configuration = turbinia_api_lib.Configuration(
+    host = "http://localhost"
+)
+
+# The client must configure the authentication and authorization parameters
+# in accordance with the API server security policy.
+# Examples for each auth method are provided below, use the example that
+# satisfies your auth use case.
+
+configuration.access_token = os.environ["ACCESS_TOKEN"]
+
+# Enter a context with an instance of the API client
+with turbinia_api_lib.ApiClient(configuration) as api_client:
+    # Create an instance of the API class
+    api_instance = turbinia_api_lib.TurbiniaRequestResultsApi(api_client)
+    task_id = 'task_id_example' # str | 
+
+    try:
+        # Get Plaso File
+        api_response = api_instance.get_plaso_file(task_id)
+        print("The response of TurbiniaRequestResultsApi->get_plaso_file:\n")
+        pprint(api_response)
+    except Exception as e:
+        print("Exception when calling TurbiniaRequestResultsApi->get_plaso_file: %s\n" % e)
+```
+
+
+
+### Parameters
+
+Name | Type | Description  | Notes
+------------- | ------------- | ------------- | -------------
+ **task_id** | **str**|  | 
+
+### Return type
+
+**bytearray**
+
+### Authorization
+
+[oAuth2](../README.md#oAuth2)
+
+### HTTP request headers
+
+ - **Content-Type**: Not defined
+ - **Accept**: application/octet-stream, application/json
+
+### HTTP response details
+| Status code | Description | Response headers |
+|-------------|-------------|------------------|
+**200** | Successful Response |  -  |
+**422** | Validation Error |  -  |
+
+[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)
+
 # **get_request_output**
 > bytearray get_request_output(request_id)
 
 Get Request Output
 
 Retrieve request output.
```

### Comparing `turbinia-20240313/turbinia/api/client/docs/TurbiniaRequestsApi.md` & `turbinia-20240412.1/turbinia/api/client/docs/TurbiniaRequestsApi.md`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/api/client/docs/TurbiniaTasksApi.md` & `turbinia-20240412.1/turbinia/api/client/docs/TurbiniaTasksApi.md`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/api/client/docs/ValidationError.md` & `turbinia-20240412.1/turbinia/api/client/docs/ValidationError.md`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/api/client/git_push.sh` & `turbinia-20240412.1/turbinia/api/client/git_push.sh`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/api/client/poetry.lock` & `turbinia-20240412.1/turbinia/api/client/poetry.lock`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file is automatically @generated by Poetry 1.7.1 and should not be changed by hand.
+# This file is automatically @generated by Poetry 1.8.2 and should not be changed by hand.
 
 [[package]]
 name = "aenum"
 version = "3.1.15"
 description = "Advanced Enumerations (compatible with Python's stdlib Enum), NamedTuples, and NamedConstants"
 optional = false
 python-versions = "*"
@@ -68,26 +68,26 @@
 ]
 
 [package.extras]
 test = ["pytest (>=6)"]
 
 [[package]]
 name = "filelock"
-version = "3.13.1"
+version = "3.13.3"
 description = "A platform independent file lock."
 optional = false
 python-versions = ">=3.8"
 files = [
-    {file = "filelock-3.13.1-py3-none-any.whl", hash = "sha256:57dbda9b35157b05fb3e58ee91448612eb674172fab98ee235ccb0b5bee19a1c"},
-    {file = "filelock-3.13.1.tar.gz", hash = "sha256:521f5f56c50f8426f5e03ad3b281b490a87ef15bc6c526f168290f0c7148d44e"},
+    {file = "filelock-3.13.3-py3-none-any.whl", hash = "sha256:5ffa845303983e7a0b7ae17636509bc97997d58afeafa72fb141a17b152284cb"},
+    {file = "filelock-3.13.3.tar.gz", hash = "sha256:a79895a25bbefdf55d1a2a0a80968f7dbb28edcd6d4234a0afb3f37ecde4b546"},
 ]
 
 [package.extras]
-docs = ["furo (>=2023.9.10)", "sphinx (>=7.2.6)", "sphinx-autodoc-typehints (>=1.24)"]
-testing = ["covdefaults (>=2.3)", "coverage (>=7.3.2)", "diff-cover (>=8)", "pytest (>=7.4.3)", "pytest-cov (>=4.1)", "pytest-mock (>=3.12)", "pytest-timeout (>=2.2)"]
+docs = ["furo (>=2023.9.10)", "sphinx (>=7.2.6)", "sphinx-autodoc-typehints (>=1.25.2)"]
+testing = ["covdefaults (>=2.3)", "coverage (>=7.3.2)", "diff-cover (>=8.0.1)", "pytest (>=7.4.3)", "pytest-cov (>=4.1)", "pytest-mock (>=3.12)", "pytest-timeout (>=2.2)"]
 typing = ["typing-extensions (>=4.8)"]
 
 [[package]]
 name = "flake8"
 version = "7.0.0"
 description = "the modular source code checker: pep8 pyflakes and co"
 optional = false
@@ -122,21 +122,21 @@
 files = [
     {file = "mccabe-0.7.0-py2.py3-none-any.whl", hash = "sha256:6c2d30ab6be0e4a46919781807b4f0d834ebdd6c6e3dca0bda5a15f863427b6e"},
     {file = "mccabe-0.7.0.tar.gz", hash = "sha256:348e0240c33b60bbdf4e523192ef919f28cb2c3d7d5c7794f74009290f236325"},
 ]
 
 [[package]]
 name = "packaging"
-version = "23.2"
+version = "24.0"
 description = "Core utilities for Python packages"
 optional = false
 python-versions = ">=3.7"
 files = [
-    {file = "packaging-23.2-py3-none-any.whl", hash = "sha256:8c491190033a9af7e1d931d0b5dacc2ef47509b34dd0de67ed209b5203fc88c7"},
-    {file = "packaging-23.2.tar.gz", hash = "sha256:048fb0e9405036518eaaf48a55953c750c11e1a1b68e0dd1a9d62ed0c092cfc5"},
+    {file = "packaging-24.0-py3-none-any.whl", hash = "sha256:2ddfb553fdf02fb784c234c7ba6ccc288296ceabec964ad2eae3777778130bc5"},
+    {file = "packaging-24.0.tar.gz", hash = "sha256:eb82c5e3e56209074766e6885bb04b8c38a0c015d0a30036ebe7ece34c9989e9"},
 ]
 
 [[package]]
 name = "platformdirs"
 version = "4.2.0"
 description = "A small Python package for determining appropriate platform-specific dirs, e.g. a \"user data dir\"."
 optional = false
@@ -256,43 +256,43 @@
 
 [package.extras]
 docs = ["furo (>=2023.8.19)", "sphinx (<7.2)", "sphinx-autodoc-typehints (>=1.24)"]
 testing = ["covdefaults (>=2.3)", "pytest (>=7.4)", "pytest-cov (>=4.1)", "pytest-mock (>=3.11.1)", "setuptools (>=68.1.2)", "wheel (>=0.41.2)"]
 
 [[package]]
 name = "pytest"
-version = "8.0.2"
+version = "8.1.1"
 description = "pytest: simple powerful testing with Python"
 optional = false
 python-versions = ">=3.8"
 files = [
-    {file = "pytest-8.0.2-py3-none-any.whl", hash = "sha256:edfaaef32ce5172d5466b5127b42e0d6d35ebbe4453f0e3505d96afd93f6b096"},
-    {file = "pytest-8.0.2.tar.gz", hash = "sha256:d4051d623a2e0b7e51960ba963193b09ce6daeb9759a451844a21e4ddedfc1bd"},
+    {file = "pytest-8.1.1-py3-none-any.whl", hash = "sha256:2a8386cfc11fa9d2c50ee7b2a57e7d898ef90470a7a34c4b949ff59662bb78b7"},
+    {file = "pytest-8.1.1.tar.gz", hash = "sha256:ac978141a75948948817d360297b7aae0fcb9d6ff6bc9ec6d514b85d5a65c044"},
 ]
 
 [package.dependencies]
 colorama = {version = "*", markers = "sys_platform == \"win32\""}
 exceptiongroup = {version = ">=1.0.0rc8", markers = "python_version < \"3.11\""}
 iniconfig = "*"
 packaging = "*"
-pluggy = ">=1.3.0,<2.0"
-tomli = {version = ">=1.0.0", markers = "python_version < \"3.11\""}
+pluggy = ">=1.4,<2.0"
+tomli = {version = ">=1", markers = "python_version < \"3.11\""}
 
 [package.extras]
-testing = ["argcomplete", "attrs (>=19.2.0)", "hypothesis (>=3.56)", "mock", "nose", "pygments (>=2.7.2)", "requests", "setuptools", "xmlschema"]
+testing = ["argcomplete", "attrs (>=19.2)", "hypothesis (>=3.56)", "mock", "pygments (>=2.7.2)", "requests", "setuptools", "xmlschema"]
 
 [[package]]
 name = "python-dateutil"
-version = "2.8.2"
+version = "2.9.0.post0"
 description = "Extensions to the standard Python datetime module"
 optional = false
 python-versions = "!=3.0.*,!=3.1.*,!=3.2.*,>=2.7"
 files = [
-    {file = "python-dateutil-2.8.2.tar.gz", hash = "sha256:0123cacc1627ae19ddf3c27a5de5bd67ee4586fbdd6440d9748f8abb483d3e86"},
-    {file = "python_dateutil-2.8.2-py2.py3-none-any.whl", hash = "sha256:961d03dc3453ebbc59dbdea9e4e11c5651520a876d0f4db161e8674aae935da9"},
+    {file = "python-dateutil-2.9.0.post0.tar.gz", hash = "sha256:37dd54208da7e1cd875388217d5e00ebd4179249f90fb72437e91a35459a0ad3"},
+    {file = "python_dateutil-2.9.0.post0-py2.py3-none-any.whl", hash = "sha256:a8b2bc7bffae282281c8140a97d3aa9c14da0b136dfe83f850eea9a5f7470427"},
 ]
 
 [package.dependencies]
 six = ">=1.5"
 
 [[package]]
 name = "six"
@@ -314,21 +314,21 @@
 files = [
     {file = "tomli-2.0.1-py3-none-any.whl", hash = "sha256:939de3e7a6161af0c887ef91b7d41a53e7c5a1ca976325f429cb46ea9bc30ecc"},
     {file = "tomli-2.0.1.tar.gz", hash = "sha256:de526c12914f0c550d15924c62d72abc48d6fe7364aa87328337a31007fe8a4f"},
 ]
 
 [[package]]
 name = "tox"
-version = "4.13.0"
+version = "4.14.2"
 description = "tox is a generic virtualenv management and test command line tool"
 optional = false
 python-versions = ">=3.8"
 files = [
-    {file = "tox-4.13.0-py3-none-any.whl", hash = "sha256:1143c7e2489c68026a55d3d4ae84c02c449f073b28e62f80e3e440a3b72a4afa"},
-    {file = "tox-4.13.0.tar.gz", hash = "sha256:dd789a554c16c4b532924ba393c92fc8991323c4b3d466712bfecc8c9b9f24f7"},
+    {file = "tox-4.14.2-py3-none-any.whl", hash = "sha256:2900c4eb7b716af4a928a7fdc2ed248ad6575294ed7cfae2ea41203937422847"},
+    {file = "tox-4.14.2.tar.gz", hash = "sha256:0defb44f6dafd911b61788325741cc6b2e12ea71f987ac025ad4d649f1f1a104"},
 ]
 
 [package.dependencies]
 cachetools = ">=5.3.2"
 chardet = ">=5.2"
 colorama = ">=0.4.6"
 filelock = ">=3.13.1"
```

### Comparing `turbinia-20240313/turbinia/api/client/pyproject.toml` & `turbinia-20240412.1/turbinia/api/client/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "turbinia-api-lib"
-version = "1.0.3"
+version = "1.0.4"
 description = "Turbinia API Server"
 authors = ["OpenAPI Generator Community <team@openapitools.org>"]
 license = "Apache License 2.0"
 readme = "README.md"
 repository = "https://github.com/google/turbinia"
 keywords = ["OpenAPI", "OpenAPI-Generator", "Turbinia API Server"]
 include = ["turbinia_api_lib/py.typed"]
```

### Comparing `turbinia-20240313/turbinia/api/client/turbinia_api_lib/__init__.py` & `turbinia-20240412.1/turbinia/api/client/turbinia_api_lib/__init__.py`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/api/client/turbinia_api_lib/api/__init__.py` & `turbinia-20240412.1/turbinia/api/client/turbinia_api_lib/api/__init__.py`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/api/client/turbinia_api_lib/api/turbinia_configuration_api.py` & `turbinia-20240412.1/turbinia/api/client/turbinia_api_lib/api/turbinia_configuration_api.py`

 * *Files 15% similar despite different names*

```diff
@@ -170,14 +170,146 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
+    def get_version(self, **kwargs) -> object:  # noqa: E501
+        """Get Version  # noqa: E501
+
+        Returns the Turbinia version.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.get_version(async_req=True)
+        >>> result = thread.get()
+
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _request_timeout: timeout setting for this request.
+               If one number provided, it will be total request
+               timeout. It can also be a pair (tuple) of
+               (connection, read) timeouts.
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: object
+        """
+        kwargs['_return_http_data_only'] = True
+        if '_preload_content' in kwargs:
+            message = "Error! Please call the get_version_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data"  # noqa: E501
+            raise ValueError(message)
+        return self.get_version_with_http_info(**kwargs)  # noqa: E501
+
+    @validate_arguments
+    def get_version_with_http_info(self, **kwargs) -> ApiResponse:  # noqa: E501
+        """Get Version  # noqa: E501
+
+        Returns the Turbinia version.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.get_version_with_http_info(async_req=True)
+        >>> result = thread.get()
+
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _preload_content: if False, the ApiResponse.data will
+                                 be set to none and raw_data will store the
+                                 HTTP response body without reading/decoding.
+                                 Default is True.
+        :type _preload_content: bool, optional
+        :param _return_http_data_only: response data instead of ApiResponse
+                                       object with status code, headers, etc
+        :type _return_http_data_only: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the authentication
+                              in the spec for a single request.
+        :type _request_auth: dict, optional
+        :type _content_type: string, optional: force content-type for the request
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: tuple(object, status_code(int), headers(HTTPHeaderDict))
+        """
+
+        _params = locals()
+
+        _all_params = [
+        ]
+        _all_params.extend(
+            [
+                'async_req',
+                '_return_http_data_only',
+                '_preload_content',
+                '_request_timeout',
+                '_request_auth',
+                '_content_type',
+                '_headers'
+            ]
+        )
+
+        # validate the arguments
+        for _key, _val in _params['kwargs'].items():
+            if _key not in _all_params:
+                raise ApiTypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method get_version" % _key
+                )
+            _params[_key] = _val
+        del _params['kwargs']
+
+        _collection_formats = {}
+
+        # process the path parameters
+        _path_params = {}
+
+        # process the query parameters
+        _query_params = []
+        # process the header parameters
+        _header_params = dict(_params.get('_headers', {}))
+        # process the form parameters
+        _form_params = []
+        _files = {}
+        # process the body parameter
+        _body_params = None
+        # set the HTTP header `Accept`
+        _header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # authentication setting
+        _auth_settings = ['oAuth2']  # noqa: E501
+
+        _response_types_map = {
+            '200': "object",
+        }
+
+        return self.api_client.call_api(
+            '/api/config/version', 'GET',
+            _path_params,
+            _query_params,
+            _header_params,
+            body=_body_params,
+            post_params=_form_params,
+            files=_files,
+            response_types_map=_response_types_map,
+            auth_settings=_auth_settings,
+            async_req=_params.get('async_req'),
+            _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=_params.get('_preload_content', True),
+            _request_timeout=_params.get('_request_timeout'),
+            collection_formats=_collection_formats,
+            _request_auth=_params.get('_request_auth'))
+
+    @validate_arguments
     def read_config(self, **kwargs) -> object:  # noqa: E501
         """Read Config  # noqa: E501
 
         Retrieve turbinia config.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
```

### Comparing `turbinia-20240313/turbinia/api/client/turbinia_api_lib/api/turbinia_evidence_api.py` & `turbinia-20240412.1/turbinia/api/client/turbinia_api_lib/api/turbinia_evidence_api.py`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/api/client/turbinia_api_lib/api/turbinia_jobs_api.py` & `turbinia-20240412.1/turbinia/api/client/turbinia_api_lib/api/turbinia_jobs_api.py`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/api/client/turbinia_api_lib/api/turbinia_logs_api.py` & `turbinia-20240412.1/turbinia/api/client/turbinia_api_lib/api/turbinia_logs_api.py`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/api/client/turbinia_api_lib/api/turbinia_request_results_api.py` & `turbinia-20240412.1/turbinia/api/client/turbinia_api_lib/api/turbinia_request_results_api.py`

 * *Files 18% similar despite different names*

```diff
@@ -40,14 +40,153 @@
 
     def __init__(self, api_client=None) -> None:
         if api_client is None:
             api_client = ApiClient.get_default()
         self.api_client = api_client
 
     @validate_arguments
+    def get_plaso_file(self, task_id : StrictStr, **kwargs) -> bytearray:  # noqa: E501
+        """Get Plaso File  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.get_plaso_file(task_id, async_req=True)
+        >>> result = thread.get()
+
+        :param task_id: (required)
+        :type task_id: str
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _request_timeout: timeout setting for this request.
+               If one number provided, it will be total request
+               timeout. It can also be a pair (tuple) of
+               (connection, read) timeouts.
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: bytearray
+        """
+        kwargs['_return_http_data_only'] = True
+        if '_preload_content' in kwargs:
+            message = "Error! Please call the get_plaso_file_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data"  # noqa: E501
+            raise ValueError(message)
+        return self.get_plaso_file_with_http_info(task_id, **kwargs)  # noqa: E501
+
+    @validate_arguments
+    def get_plaso_file_with_http_info(self, task_id : StrictStr, **kwargs) -> ApiResponse:  # noqa: E501
+        """Get Plaso File  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.get_plaso_file_with_http_info(task_id, async_req=True)
+        >>> result = thread.get()
+
+        :param task_id: (required)
+        :type task_id: str
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _preload_content: if False, the ApiResponse.data will
+                                 be set to none and raw_data will store the
+                                 HTTP response body without reading/decoding.
+                                 Default is True.
+        :type _preload_content: bool, optional
+        :param _return_http_data_only: response data instead of ApiResponse
+                                       object with status code, headers, etc
+        :type _return_http_data_only: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the authentication
+                              in the spec for a single request.
+        :type _request_auth: dict, optional
+        :type _content_type: string, optional: force content-type for the request
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: tuple(bytearray, status_code(int), headers(HTTPHeaderDict))
+        """
+
+        _params = locals()
+
+        _all_params = [
+            'task_id'
+        ]
+        _all_params.extend(
+            [
+                'async_req',
+                '_return_http_data_only',
+                '_preload_content',
+                '_request_timeout',
+                '_request_auth',
+                '_content_type',
+                '_headers'
+            ]
+        )
+
+        # validate the arguments
+        for _key, _val in _params['kwargs'].items():
+            if _key not in _all_params:
+                raise ApiTypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method get_plaso_file" % _key
+                )
+            _params[_key] = _val
+        del _params['kwargs']
+
+        _collection_formats = {}
+
+        # process the path parameters
+        _path_params = {}
+        if _params['task_id'] is not None:
+            _path_params['task_id'] = _params['task_id']
+
+
+        # process the query parameters
+        _query_params = []
+        # process the header parameters
+        _header_params = dict(_params.get('_headers', {}))
+        # process the form parameters
+        _form_params = []
+        _files = {}
+        # process the body parameter
+        _body_params = None
+        # set the HTTP header `Accept`
+        _header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/octet-stream', 'application/json'])  # noqa: E501
+
+        # authentication setting
+        _auth_settings = ['oAuth2']  # noqa: E501
+
+        _response_types_map = {
+            '200': "bytearray",
+            '422': "HTTPValidationError",
+        }
+
+        return self.api_client.call_api(
+            '/api/result/plasofile/{task_id}', 'GET',
+            _path_params,
+            _query_params,
+            _header_params,
+            body=_body_params,
+            post_params=_form_params,
+            files=_files,
+            response_types_map=_response_types_map,
+            auth_settings=_auth_settings,
+            async_req=_params.get('async_req'),
+            _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=_params.get('_preload_content', True),
+            _request_timeout=_params.get('_request_timeout'),
+            collection_formats=_collection_formats,
+            _request_auth=_params.get('_request_auth'))
+
+    @validate_arguments
     def get_request_output(self, request_id : StrictStr, **kwargs) -> bytearray:  # noqa: E501
         """Get Request Output  # noqa: E501
 
         Retrieve request output.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
```

### Comparing `turbinia-20240313/turbinia/api/client/turbinia_api_lib/api/turbinia_requests_api.py` & `turbinia-20240412.1/turbinia/api/client/turbinia_api_lib/api/turbinia_requests_api.py`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/api/client/turbinia_api_lib/api/turbinia_tasks_api.py` & `turbinia-20240412.1/turbinia/api/client/turbinia_api_lib/api/turbinia_tasks_api.py`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/api/client/turbinia_api_lib/api_client.py` & `turbinia-20240412.1/turbinia/api/client/turbinia_api_lib/api_client.py`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/api/client/turbinia_api_lib/api_response.py` & `turbinia-20240412.1/turbinia/api/client/turbinia_api_lib/api_response.py`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/api/client/turbinia_api_lib/configuration.py` & `turbinia-20240412.1/turbinia/api/client/turbinia_api_lib/configuration.py`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/api/client/turbinia_api_lib/exceptions.py` & `turbinia-20240412.1/turbinia/api/client/turbinia_api_lib/exceptions.py`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/api/client/turbinia_api_lib/models/__init__.py` & `turbinia-20240412.1/turbinia/api/client/turbinia_api_lib/models/__init__.py`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/api/client/turbinia_api_lib/models/base_request_options.py` & `turbinia-20240412.1/turbinia/api/client/turbinia_api_lib/models/base_request_options.py`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/api/client/turbinia_api_lib/models/body_upload_evidence_api_evidence_upload_post.py` & `turbinia-20240412.1/turbinia/api/client/turbinia_api_lib/models/request.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 # coding: utf-8
 
 """
     Turbinia API Server
 
-    Turbinia API server
+    Turbinia is an open-source framework for deploying, managing, and running distributed forensic workloads
 
     The version of the OpenAPI document: 1.0.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
-from typing import Any, Optional
-from pydantic import BaseModel, Field
+from typing import Any, Dict, Optional
+from pydantic import BaseModel, Field, StrictStr
+from turbinia_api_lib.models.base_request_options import BaseRequestOptions
 
-class BodyUploadEvidenceApiEvidenceUploadPost(BaseModel):
+class Request(BaseModel):
     """
-    BodyUploadEvidenceApiEvidenceUploadPost
+    Base request object.   # noqa: E501
     """
-    calculate_hash: Optional[Any] = None
-    files: Optional[Any] = Field(...)
-    ticket_id: Optional[Any] = Field(...)
-    __properties = ["calculate_hash", "files", "ticket_id"]
+    description: Optional[StrictStr] = 'Turbinia request object'
+    evidence: Dict[str, Any] = Field(...)
+    request_options: BaseRequestOptions = Field(...)
+    __properties = ["description", "evidence", "request_options"]
 
     class Config:
         """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
@@ -40,51 +41,39 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> BodyUploadEvidenceApiEvidenceUploadPost:
-        """Create an instance of BodyUploadEvidenceApiEvidenceUploadPost from a JSON string"""
+    def from_json(cls, json_str: str) -> Request:
+        """Create an instance of Request from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
-        # set to None if calculate_hash (nullable) is None
-        # and __fields_set__ contains the field
-        if self.calculate_hash is None and "calculate_hash" in self.__fields_set__:
-            _dict['calculate_hash'] = None
-
-        # set to None if files (nullable) is None
-        # and __fields_set__ contains the field
-        if self.files is None and "files" in self.__fields_set__:
-            _dict['files'] = None
-
-        # set to None if ticket_id (nullable) is None
-        # and __fields_set__ contains the field
-        if self.ticket_id is None and "ticket_id" in self.__fields_set__:
-            _dict['ticket_id'] = None
-
+        # override the default output from pydantic by calling `to_dict()` of request_options
+        if self.request_options:
+            _dict['request_options'] = self.request_options.to_dict()
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> BodyUploadEvidenceApiEvidenceUploadPost:
-        """Create an instance of BodyUploadEvidenceApiEvidenceUploadPost from a dict"""
+    def from_dict(cls, obj: dict) -> Request:
+        """Create an instance of Request from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
-            return BodyUploadEvidenceApiEvidenceUploadPost.parse_obj(obj)
+            return Request.parse_obj(obj)
 
-        _obj = BodyUploadEvidenceApiEvidenceUploadPost.parse_obj({
-            "calculate_hash": obj.get("calculate_hash"),
-            "files": obj.get("files"),
-            "ticket_id": obj.get("ticket_id")
+        _obj = Request.parse_obj({
+            "description": obj.get("description") if obj.get("description") is not None else 'Turbinia request object',
+            "evidence": obj.get("evidence"),
+            "request_options": BaseRequestOptions.from_dict(obj.get("request_options")) if obj.get("request_options") is not None else None
         })
         return _obj
```

### Comparing `turbinia-20240313/turbinia/api/client/turbinia_api_lib/models/complete_turbinia_stats.py` & `turbinia-20240412.1/turbinia/api/client/turbinia_api_lib/models/complete_turbinia_stats.py`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/api/client/turbinia_api_lib/models/http_validation_error.py` & `turbinia-20240412.1/turbinia/api/client/turbinia_api_lib/models/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/api/client/turbinia_api_lib/models/location_inner.py` & `turbinia-20240412.1/turbinia/api/client/turbinia_api_lib/models/location_inner.py`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/api/client/turbinia_api_lib/models/validation_error.py` & `turbinia-20240412.1/turbinia/api/client/turbinia_api_lib/models/validation_error.py`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/api/client/turbinia_api_lib/rest.py` & `turbinia-20240412.1/turbinia/api/client/turbinia_api_lib/rest.py`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/api/models/__init__.py` & `turbinia-20240412.1/turbinia/api/models/__init__.py`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/api/models/request_status.py` & `turbinia-20240412.1/turbinia/api/models/request_status.py`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/api/models/tasks_statistics.py` & `turbinia-20240412.1/turbinia/api/models/tasks_statistics.py`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/api/models/workers_status.py` & `turbinia-20240412.1/turbinia/api/models/workers_status.py`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/api/openapi.yaml` & `turbinia-20240412.1/turbinia/api/openapi.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -186,14 +186,27 @@
           content:
             application/json:
               schema: {}
           description: Successful Response
       summary: Get Request Options
       tags:
       - Turbinia Configuration
+  /api/config/version:
+      get:
+        description: Returns the Turbinia version.
+        operationId: get_version
+        responses:
+          '200':
+            content:
+              application/json:
+                schema: {}
+            description: Successful Response
+        summary: Get Version
+        tags:
+        - Turbinia Configuration
   /api/evidence/query:
     get:
       description: "Queries evidence in Redis that have the specified attribute value.\n\
         \nArgs:\n  attribute_name (str): Name of attribute to be queried.\n  attribute_value\
         \ (str): Value the attribute must have.\n  output Optional(str): Sets how\
         \ the evidence found will be output.\n\nReturns:\n  summary (dict): Summary\
         \ of all evidences and their content.\n\nRaises:\n  HTTPException: If no matching\
@@ -530,14 +543,41 @@
             application/json:
               schema:
                 $ref: '#/components/schemas/HTTPValidationError'
           description: Validation Error
       summary: Get Request Status
       tags:
       - Turbinia Requests
+  /api/result/plasofile/{task_id}:
+    get:
+      operationId: get_plaso_file
+      parameters:
+      - in: path
+        name: task_id
+        required: true
+        schema:
+          title: Task Id
+          type: string
+      responses:
+        '200':
+          content:
+            application/octet-stream:
+              schema:
+                format: binary
+                type: string
+          description: Successful Response
+        '422':
+          content:
+            application/json:
+              schema:
+                $ref: '#/components/schemas/HTTPValidationError'
+          description: Validation Error
+      summary: Get Plaso File
+      tags:
+      - Turbinia Request Results
   /api/result/request/{request_id}:
     get:
       description: Retrieve request output.
       operationId: get_request_output
       parameters:
       - in: path
         name: request_id
```

### Comparing `turbinia-20240313/turbinia/api/routes/__init__.py` & `turbinia-20240412.1/turbinia/api/routes/__init__.py`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/api/routes/config.py` & `turbinia-20240412.1/turbinia/api/routes/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,18 +17,19 @@
 import json
 import logging
 
 from fastapi import HTTPException, APIRouter
 from fastapi.responses import JSONResponse
 from fastapi.requests import Request
 
+from turbinia import __version__
 from turbinia import config as turbinia_config
 from turbinia.api.schemas import request_options
 
-log = logging.getLogger('turbinia')
+log = logging.getLogger(__name__)
 
 router = APIRouter(prefix='/config', tags=['Turbinia Configuration'])
 
 
 @router.get('/')
 async def read_config(request: Request):
   """Retrieve turbinia config."""
@@ -46,7 +47,14 @@
 async def get_request_options(request: Request):
   """Returns a list BaseRequestOptions attributes."""
   attributes = request_options.BaseRequestOptions.__annotations__
   attributes_dict = {}
   for attribute_name, attribute_type in attributes.items():
     attributes_dict[attribute_name] = {'type': str(attribute_type)}
   return JSONResponse(content=attributes_dict, status_code=200)
+
+
+@router.get('/version')
+async def get_version(request: Request):
+  """Returns the Turbinia version."""
+  response = {'version': __version__}
+  return JSONResponse(content=response, status_code=200)
```

### Comparing `turbinia-20240313/turbinia/api/routes/evidence.py` & `turbinia-20240412.1/turbinia/api/routes/evidence.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 from turbinia.api.schemas import request_options
 from turbinia import evidence
 from turbinia import config as turbinia_config
 from turbinia import state_manager
 from turbinia import TurbiniaException
 
-log = logging.getLogger('turbinia')
+log = logging.getLogger(__name__)
 router = APIRouter(prefix='/evidence', tags=['Turbinia Evidence'])
 redis_manager = state_manager.RedisStateManager()
 
 EVIDENCE_SUMMARY_ATTRIBUTES = (
     '_name', 'cloud_only', 'context_dependent', 'copyable', 'creation_time',
     'description', 'has_child_evidence', 'last_update', 'local_path',
     'mount_path', 'parent_evidence', 'request_id', 'resource_id',
@@ -51,19 +51,17 @@
     file_name (str): Original name of the file.
     ticked_id (str): ID of the current ticket
   
   Returns:
     file_path (str): Path where the file will be saved.
   """
   try:
-    file_name = os.path.splitext(file_name)[0]
-    file_extension = os.path.splitext(file_name)[1]
-    file_extension = '.' + file_extension if file_extension else ''
+    file_name_without_ext, file_extension = os.path.splitext(file_name)
     current_time = datetime.now().strftime(turbinia_config.DATETIME_FORMAT)
-    new_name = f'{file_name}_{current_time}{file_extension}'
+    new_name = f'{file_name_without_ext}_{current_time}{file_extension}'
     os.makedirs(
         f'{turbinia_config.API_EVIDENCE_UPLOAD_DIR}/{ticket_id}', exist_ok=True)
     return os.path.join(
         turbinia_config.API_EVIDENCE_UPLOAD_DIR, ticket_id, new_name)
   except OSError as exception:
     raise TurbiniaException(
         f'Failed in setting path for file {file_name} in ticket '
@@ -253,13 +251,14 @@
           file_info.get('hash')):
         warning_message = (
             f'File {file.filename} was uploaded before, check {evidence_key}')
     if warning_message:
       evidences.append(warning_message)
       log.error(warning_message)
       try:
+        file_path = await get_file_path(file.filename, ticket_id)
         os.remove(file_path)
       except OSError as exception:
         log.error(f'Could not remove file {file_path}: {exception}')
     else:
       evidences.append(file_info)
   return JSONResponse(content=evidences, status_code=200)
```

### Comparing `turbinia-20240313/turbinia/api/routes/jobs.py` & `turbinia-20240412.1/turbinia/api/routes/jobs.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from fastapi import HTTPException, APIRouter
 from fastapi.responses import JSONResponse
 from fastapi.requests import Request
 
 from turbinia import config as turbinia_config
 from turbinia.jobs import manager as jobs_manager
 
-log = logging.getLogger('turbinia')
+log = logging.getLogger(__name__)
 
 router = APIRouter(prefix='/jobs', tags=['Turbinia Jobs'])
 
 
 @router.get('/')
 async def read_jobs(request: Request):
   """Return enabled jobs from the current Turbinia config."""
```

### Comparing `turbinia-20240313/turbinia/api/routes/logs.py` & `turbinia-20240412.1/turbinia/api/routes/logs.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 import logging
 
 from fastapi import APIRouter
 from fastapi.responses import JSONResponse
 from fastapi.requests import Request
 
-log = logging.getLogger('turbinia')
+log = logging.getLogger(__name__)
 
 router = APIRouter(prefix='/logs', tags=['Turbinia Logs'])
 
 
 @router.get('/{query}')
 async def get_logs(request: Request, query: str):
   """Retrieve log data."""
```

### Comparing `turbinia-20240313/turbinia/api/routes/request.py` & `turbinia-20240412.1/turbinia/api/routes/request.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 from pydantic import ValidationError
 from turbinia import TurbiniaException, client as turbinia_client
 from turbinia import evidence
 from turbinia.lib import recipe_helpers
 from turbinia.api.schemas import request as turbinia_request
 from turbinia.api.models import request_status
 
-log = logging.getLogger('turbinia')
+log = logging.getLogger(__name__)
 
 router = APIRouter(prefix='/request', tags=['Turbinia Requests'])
 
 
 @router.get('/summary')
 async def get_requests_summary(request: Request):
   """Retrieves a summary of all Turbinia requests.
```

### Comparing `turbinia-20240313/turbinia/api/routes/result.py` & `turbinia-20240412.1/turbinia/api/routes/result.py`

 * *Files 22% similar despite different names*

```diff
@@ -11,28 +11,27 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Turbinia API - Result router"""
 
 import logging
+import os
 
 from fastapi import HTTPException, APIRouter
-from fastapi.responses import StreamingResponse
+from fastapi.responses import StreamingResponse, FileResponse
 from fastapi.requests import Request
 
-from turbinia import config as turbinia_config
-from turbinia import state_manager
 from turbinia.api import utils as api_utils
 
-log = logging.getLogger('turbinia')
+log = logging.getLogger(__name__)
 
 router = APIRouter(prefix='/result', tags=['Turbinia Request Results'])
 
-_ATTACHMENT_RESPONSE = {
+ATTACHMENT_RESPONSE = {
     '200': {
         'content': {
             'application/octet-stream': {
                 'schema': {
                     'type': 'string',
                     'format': 'binary'
                 }
@@ -40,48 +39,67 @@
         }
     }
 }
 
 
 @router.get(
     '/task/{task_id}', response_class=StreamingResponse,
-    responses=_ATTACHMENT_RESPONSE)
-async def get_task_output(request: Request, task_id: str):
+    responses=ATTACHMENT_RESPONSE)
+async def get_task_output(request: Request, task_id: str) -> StreamingResponse:
   """Retrieves a task's output files."""
   # Get the request_id for the task. This is needed to find the right path.
-  data = None
-  _state_manager = state_manager.get_state_manager()
-  tasks = _state_manager.get_task_data(
-      instance=turbinia_config.INSTANCE_ID, task_id=task_id)
-  if not tasks:
-    raise HTTPException(status_code=404, detail=f'Task {task_id:s} not found.')
+  if not task_id:
+    raise HTTPException(status_code=400, detail='Task identifier not provided.')
 
+  tasks = api_utils.get_task_objects(task_id)
   request_id = tasks[0].get('request_id')
   output_path = api_utils.get_task_output_path(request_id, task_id)
 
   if request_id and output_path:
-    data: bytes = api_utils.create_tarball(output_path)
-
-  if not data:
+    return StreamingResponse(
+        api_utils.create_tarball(output_path), headers={
+            'Content-Disposition': f'attachment;filename={task_id}.tgz',
+            'Transfer-Encoding': 'chunked'
+        })
+  else:
     raise HTTPException(
-        status_code=500, detail='Unable to retrieve task output files.')
-  return StreamingResponse(
-      data,
-      headers={"Content-Disposition": f'attachment;filename={task_id}.tgz'})
+        status_code=404, detail='The requested file was not found.')
 
 
 @router.get(
     '/request/{request_id}', response_class=StreamingResponse,
-    responses=_ATTACHMENT_RESPONSE)
-async def get_request_output(request: Request, request_id: str):
+    responses=ATTACHMENT_RESPONSE)
+async def get_request_output(
+    request: Request, request_id: str) -> StreamingResponse:
   """Retrieve request output."""
-  data = None
+  if not request_id:
+    raise HTTPException(
+        status_code=404, detail='Request identifier not provided.')
+
   request_output_path = api_utils.get_request_output_path(request_id)
   if request_output_path:
-    data: bytes = api_utils.create_tarball(request_output_path)
-
-  if not data:
+    return StreamingResponse(
+        api_utils.create_tarball(request_output_path), headers={
+            'Content-Disposition': f'attachment;filename={request_id}.tgz',
+            'Transfer-Encoding': 'chunked'
+        })
+  else:
     raise HTTPException(
-        status_code=500, detail='Unable to retrieve task output files.')
-  return StreamingResponse(
-      data,
-      headers={"Content-Disposition": f'attachment;filename={request_id}.tgz'})
+        status_code=404, detail='The requested file was not found.')
+
+
+@router.get(
+    '/plasofile/{task_id}', response_class=FileResponse,
+    responses=ATTACHMENT_RESPONSE)
+async def get_plaso_file(request: Request, task_id: str) -> FileResponse:
+  """Retrieves a task's Plaso file."""
+  if not task_id:
+    raise HTTPException(status_code=400, detail='Task identifier not provided.')
+
+  plaso_file_path = api_utils.get_plaso_file_path(task_id)
+  filename = f'{task_id}.plaso'
+
+  if os.path.exists(plaso_file_path):
+    log.info(f'Sending {plaso_file_path} to client.')
+    return FileResponse(plaso_file_path, filename=filename)
+  raise HTTPException(
+      status_code=404, detail=f'File {filename} could not be found.')
```

### Comparing `turbinia-20240313/turbinia/api/routes/router.py` & `turbinia-20240412.1/turbinia/api/routes/router.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,25 +9,28 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Turbinia API server."""
+import logging
 
 from fastapi import APIRouter
 
 from turbinia.api.routes import config
 from turbinia.api.routes import evidence
 from turbinia.api.routes import jobs
 from turbinia.api.routes import logs
 from turbinia.api.routes import request
 from turbinia.api.routes import result
 from turbinia.api.routes import task
 
+log = logging.getLogger('turbinia')
+
 # Prefix API endpoints with /api/
 api_router = APIRouter(prefix='/api')
 
 # Register all API endpoints.
 api_router.include_router(config.router)
 api_router.include_router(evidence.router)
 api_router.include_router(jobs.router)
```

### Comparing `turbinia-20240313/turbinia/api/routes/task.py` & `turbinia-20240412.1/turbinia/api/routes/task.py`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/api/routes/ui.py` & `turbinia-20240412.1/turbinia/api/routes/ui.py`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/api/schemas/__init__.py` & `turbinia-20240412.1/turbinia/api/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/api/schemas/request.py` & `turbinia-20240412.1/turbinia/api/schemas/request.py`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/api/schemas/request_options.py` & `turbinia-20240412.1/turbinia/api/schemas/request_options.py`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/api/utils.py` & `turbinia-20240412.1/turbinia/api/utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -14,18 +14,38 @@
 # limitations under the License.
 """Turbinia API Server helper methods."""
 
 import logging
 import os
 import tarfile
 import io
+
+from typing import Any, AsyncGenerator, List
+
 from fastapi import HTTPException
+from turbinia import TurbiniaException
 from turbinia import config as turbinia_config
+from turbinia import state_manager
+
+log = logging.getLogger(__name__)
 
-log = logging.getLogger('turbinia')
+
+def get_task_objects(task_id: str) -> List[Any]:
+  """Returns a list of Turbinia tasks.
+  
+  Riases:
+    HTTPException: if the specified task was not found.
+  """
+  _state_manager = state_manager.get_state_manager()
+  tasks = _state_manager.get_task_data(
+      instance=turbinia_config.INSTANCE_ID, task_id=task_id)
+
+  if not tasks:
+    raise HTTPException(status_code=404, detail=f'Task {task_id:s} not found.')
+  return tasks
 
 
 def get_request_output_path(request_id: str) -> str:
   """Returns the output path for a request_id."""
   log_path = turbinia_config.toDict().get('OUTPUT_DIR')
   request_output_path = os.path.join(log_path, request_id)
   if not os.path.exists(request_output_path):
@@ -35,28 +55,49 @@
     raise HTTPException(status_code=404, detail=message)
   return request_output_path
 
 
 def get_task_output_path(request_id: str, task_id: str) -> str:
   """Returns the output path for a task_id."""
   request_output_path = get_request_output_path(request_id)
+  task_output_path = request_output_path
   if task_id:
     try:
       request_dirs = os.listdir(request_output_path)
     except FileNotFoundError as exception:
       message = 'Output path {0:s} for task {1:s} could not be found.'.format(
           request_output_path, task_id)
       log.error(message)
       raise HTTPException(status_code=404, detail=message) from exception
 
-    for request_dir in request_dirs:
-      if task_id in request_dir:
-        request_output_path = os.path.join(request_output_path, request_dir)
-        break
-    return request_output_path
+    latest_timestamp = 0
+    for task_dir in request_dirs:
+      # We'll check the timestamp that's part of the directory name
+      # to make sure we grab the most recent directory for the task
+      # in case there are more than one.
+      if task_id in task_dir:
+        timestamp = int(task_dir.split('-')[0])
+        if timestamp > latest_timestamp:
+          latest_timestamp = timestamp
+          task_output_path = os.path.join(request_output_path, task_dir)
+
+    return task_output_path
+
+
+def get_plaso_file_path(task_id: str) -> str:
+  """Returns the saved_path for a specific Plaso task."""
+  task = get_task_objects(task_id)[0]
+  output_dir = turbinia_config.toDict().get('OUTPUT_DIR')
+
+  if not task or not task.get('name').startswith('Plaso'):
+    raise TurbiniaException(f'Task {task_id} not found or is not a Plaso task.')
+
+  for saved_path in task.get('saved_paths'):
+    if saved_path.startswith(output_dir) and saved_path.endswith('.plaso'):
+      return saved_path
 
 
 class ByteStream:
   """A writeable in-memory stream used to create tgz files."""
 
   def __init__(self):
     """Initialize the object."""
@@ -91,15 +132,15 @@
     """
     data = self.buffer.getvalue()
     self.buffer.seek(0)
     self.buffer.truncate()
     return data
 
 
-async def create_tarball(output_path: str) -> bytes:
+async def create_tarball(output_path: str) -> AsyncGenerator[bytes, Any]:
   """Creates an in-memory TGZ file from output_path contents.
 
   Partially inspired by the StreamingTarGenerator class from Google's GRR.
 
   Reference:
       https://github.com/google/grr/blob/master/grr/core/grr_response_core/lib/utils.py
 
@@ -109,16 +150,18 @@
   Yields:
     bytes: tgz file chunk.
   """
   file_paths = []
   for root, _, filenames in os.walk(output_path):
     for filename in filenames:
       file_path = os.path.join(root, filename)
-      log.info(f'Adding {file_path} to tarball.')
-      file_paths.append(file_path)
+      # skip empty files
+      if os.stat(file_path).st_size > 0:
+        log.info(f'Adding {file_path} to tarball.')
+        file_paths.append(file_path)
 
   with ByteStream() as stream:
     with tarfile.TarFile.open(fileobj=stream, mode='w:gz',
                               compresslevel=1) as tar:
       for file_path in file_paths:
         tar_info = tar.gettarinfo(name=file_path)
         tar.addfile(tar_info)
```

### Comparing `turbinia-20240313/turbinia/client.py` & `turbinia-20240412.1/turbinia/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 
 config.LoadConfig()
 if config.CLOUD_PROVIDER.lower() == 'gcp':
   from libcloudforensics.providers.gcp.internal import function as gcp_function
 if config.TASK_MANAGER.lower() == 'celery':
   from turbinia.state_manager import RedisStateManager
 
-log = logging.getLogger('turbinia')
+log = logging.getLogger(__name__)
 
 
 def setup(is_client=False):
   config.LoadConfig()
   if is_client:
     logger.setup(need_file_handler=False)
   else:
```

### Comparing `turbinia-20240313/turbinia/client_stats_test.py` & `turbinia-20240412.1/turbinia/client_stats_test.py`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/client_test.py` & `turbinia-20240412.1/turbinia/client_test.py`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/config/__init__.py` & `turbinia-20240412.1/turbinia/config/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -129,15 +129,15 @@
 ]
 
 # Environment variable to look for path data in
 ENVCONFIGVAR = 'TURBINIA_CONFIG_PATH'
 
 CONFIG = None
 
-log = logging.getLogger('turbinia')
+log = logging.getLogger(__name__)
 
 
 def LoadConfig(config_file=None):
   """Finds Turbinia config file and loads it.
 
   Args:
     config_file(str): full path to config file
```

### Comparing `turbinia-20240313/turbinia/config/logger.py` & `turbinia-20240412.1/turbinia/config/logger.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,17 +12,16 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Sets up logging."""
 
 from __future__ import unicode_literals
 import logging
-
-import warnings
 import logging.handlers
+import warnings
 import os
 import sys
 
 from turbinia import config
 from turbinia import TurbiniaException
 
 # Environment variable to look for node name in
@@ -75,22 +74,23 @@
       log_name = os.uname().nodename
       # Check if NODE_NAME available for GKE setups
       if ENVNODENAME in os.environ:
         log_name = log_name + f'.{os.environ[ENVNODENAME]!s}'
       log_file_path = os.path.join(config.LOG_DIR, log_name) + '.log'
 
     file_handler = logging.FileHandler(log_file_path)
-    formatter = logging.Formatter('%(asctime)s:%(levelname)s:%(message)s')
+    formatter = logging.Formatter(
+        '%(asctime)s [%(levelname)s] %(name)s | %(message)s')
     file_handler.setFormatter(formatter)
     file_handler.setLevel(logging.DEBUG)
     logger.addHandler(file_handler)
 
   console_handler = logging.StreamHandler(sys.stdout)
   formatter = logging.Formatter(
-      '%(asctime)s [%(levelname)s] %(message)s', "%Y-%m-%d %H:%M:%S")
+      '%(asctime)s [%(levelname)s] %(name)s | %(message)s', '%Y-%m-%d %H:%M:%S')
   console_handler.setFormatter(formatter)
   if need_stream_handler:
     logger.addHandler(console_handler)
 
   # Configure the root logger to use exactly our handlers because other modules
   # like PSQ use this, and we want to see log messages from it when executing
   # from CLI.
@@ -98,8 +98,8 @@
   for handler in root_log.handlers:
     root_log.removeHandler(handler)
   root_log.addHandler(console_handler)
   if need_file_handler:
     root_log.addHandler(file_handler)
 
   # Set filelock logging to ERROR due to log spam
-  logging.getLogger("filelock").setLevel(logging.ERROR)
+  logging.getLogger('filelock').setLevel(logging.ERROR)
```

### Comparing `turbinia-20240313/turbinia/config/recipes/all.yaml` & `turbinia-20240412.1/turbinia/config/recipes/all.yaml`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/config/recipes/triage-linux-extended.yaml` & `turbinia-20240412.1/turbinia/config/recipes/triage-linux-extended.yaml`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/config/recipes/triage-linux.yaml` & `turbinia-20240412.1/turbinia/config/recipes/triage-linux.yaml`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/config/recipes/triage-macos.yml` & `turbinia-20240412.1/turbinia/config/recipes/triage-macos.yml`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/config/recipes/triage-windows.yaml` & `turbinia-20240412.1/turbinia/config/recipes/triage-windows.yaml`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/config/rules/redis_replicaof.yar` & `turbinia-20240412.1/turbinia/config/rules/redis_replicaof.yar`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/config/rules/suspicious_cron.yar` & `turbinia-20240412.1/turbinia/config/rules/suspicious_cron.yar`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/config/turbinia_config_test.py` & `turbinia-20240412.1/turbinia/config/turbinia_config_test.py`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/config/turbinia_config_tmpl.py` & `turbinia-20240412.1/turbinia/config/turbinia_config_tmpl.py`

 * *Files 0% similar despite different names*

```diff
@@ -186,15 +186,15 @@
 }, {
     'job': 'FileArtifactExtractionJob',
     'programs': ['image_export'],
     'docker_image': None,
     'timeout': 1200
 }, {
     'job': 'FileSystemTimelineJob',
-    'programs': ['list_file_entries.py'],
+    'programs': ['list_file_entries'],
     'docker_image': None,
     'timeout': 1800
 }, {
     'job': 'FsstatJob',
     'programs': ['fsstat'],
     'docker_image': None,
     'timeout': 1800
```

### Comparing `turbinia-20240313/turbinia/e2e/run-e2e-gke.sh` & `turbinia-20240412.1/turbinia/e2e/run-e2e-gke.sh`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/evidence.py` & `turbinia-20240412.1/turbinia/evidence.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 from turbinia.config import DATETIME_FORMAT
 from datetime import datetime
 
 config.LoadConfig()
 if config.CLOUD_PROVIDER.lower() == 'gcp':
   from turbinia.processors import google_cloud
 
-log = logging.getLogger('turbinia')
+log = logging.getLogger(__name__)
 
 
 def evidence_class_names(all_classes=False):
   """Returns a list of class names for the evidence module.
 
   Args:
     all_classes (bool): Flag to determine whether to include all classes
@@ -101,15 +101,15 @@
       # Add optional attributes.
       for optional_attribute in Evidence.OPTIONAL_ATTRIBUTES:
         object_attribute_mapping[class_name][optional_attribute] = {
             'required': False,
             'type': 'str'
         }
     except ValueError as exception:
-      log.info(exception)
+      log.debug(exception)
   return object_attribute_mapping
 
 
 def evidence_decode(evidence_dict, strict=False):
   """Decode JSON into appropriate Evidence object.
 
   Args:
```

### Comparing `turbinia-20240313/turbinia/evidence_test.py` & `turbinia-20240412.1/turbinia/evidence_test.py`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/job_utils.py` & `turbinia-20240412.1/turbinia/job_utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 """Job utility methods for Turbinia."""
 
 import logging
 
 from turbinia import config
 from turbinia.jobs import manager as job_manager
 
-log = logging.getLogger('turbinia')
+log = logging.getLogger(__name__)
 
 config.LoadConfig()
 
 
 def register_job_timeouts(dependencies):
   """Registers a timeout for each job.
```

### Comparing `turbinia-20240313/turbinia/jobs/__init__.py` & `turbinia-20240412.1/turbinia/jobs/__init__.py`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/jobs/binary_extractor.py` & `turbinia-20240412.1/turbinia/jobs/binary_extractor.py`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/jobs/bulk_extractor.py` & `turbinia-20240412.1/turbinia/jobs/bulk_extractor.py`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/jobs/containerd.py` & `turbinia-20240412.1/turbinia/jobs/containerd.py`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/jobs/dfdewey.py` & `turbinia-20240412.1/turbinia/jobs/dfdewey.py`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/jobs/docker.py` & `turbinia-20240412.1/turbinia/jobs/docker.py`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/jobs/file_system_timeline.py` & `turbinia-20240412.1/turbinia/jobs/file_system_timeline.py`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/jobs/finalize_request.py` & `turbinia-20240412.1/turbinia/jobs/finalize_request.py`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/jobs/fsstat.py` & `turbinia-20240412.1/turbinia/jobs/fsstat.py`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/jobs/grep.py` & `turbinia-20240412.1/turbinia/jobs/grep.py`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/jobs/hindsight.py` & `turbinia-20240412.1/turbinia/jobs/hindsight.py`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/jobs/http_access_logs.py` & `turbinia-20240412.1/turbinia/jobs/http_access_logs.py`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/jobs/imports_test.py` & `turbinia-20240412.1/turbinia/jobs/imports_test.py`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/jobs/interface.py` & `turbinia-20240412.1/turbinia/jobs/interface.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 """Interface for Jobs."""
 import uuid
 
 import logging
 
 from turbinia.evidence import EvidenceCollection
 
-log = logging.getLogger('turbinia')
+log = logging.getLogger(__name__)
 
 
 class TurbiniaJob:
   """Base class for Turbinia Jobs.
 
   Attributes:
     name (str): Name of Job
```

### Comparing `turbinia-20240313/turbinia/jobs/interface_test.py` & `turbinia-20240412.1/turbinia/jobs/interface_test.py`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/jobs/jenkins.py` & `turbinia-20240412.1/turbinia/jobs/jenkins.py`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/jobs/jupyter.py` & `turbinia-20240412.1/turbinia/jobs/jupyter.py`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/jobs/linux_acct.py` & `turbinia-20240412.1/turbinia/jobs/linux_acct.py`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/jobs/llm_artifacts_analyzer.py` & `turbinia-20240412.1/turbinia/jobs/llm_artifacts_analyzer.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,16 @@
 from turbinia import config as turbinia_config
 from turbinia import evidence as evidence_module
 from turbinia import workers
 from turbinia.jobs import interface
 from turbinia.jobs import manager
 from turbinia.workers.analysis import llm_analyzer as llm_analyzer_module
 
-log = logging.getLogger('turbinia')
+log = logging.getLogger(__name__)
+
 LLM_ARTIFACTS = [
     # Keep sorted
     'ApacheAccessLogs',
     'ApacheConfigurationFolder',
     'BashShellConfigurationFile',
     'BashShellHistoryFile',
     'BashShellSessionFile',
```

### Comparing `turbinia-20240313/turbinia/jobs/manager.py` & `turbinia-20240412.1/turbinia/jobs/manager.py`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/jobs/manager_test.py` & `turbinia-20240412.1/turbinia/jobs/manager_test.py`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/jobs/partitions.py` & `turbinia-20240412.1/turbinia/jobs/partitions.py`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/jobs/photorec.py` & `turbinia-20240412.1/turbinia/jobs/photorec.py`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/jobs/plaso.py` & `turbinia-20240412.1/turbinia/jobs/plaso.py`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/jobs/postgres_acct.py` & `turbinia-20240412.1/turbinia/jobs/postgres_acct.py`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/jobs/psort.py` & `turbinia-20240412.1/turbinia/jobs/psort.py`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/jobs/redis.py` & `turbinia-20240412.1/turbinia/jobs/redis.py`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/jobs/ssh_analyzer.py` & `turbinia-20240412.1/turbinia/jobs/ssh_analyzer.py`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/jobs/sshd.py` & `turbinia-20240412.1/turbinia/jobs/sshd.py`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/jobs/strings.py` & `turbinia-20240412.1/turbinia/jobs/strings.py`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/jobs/tomcat.py` & `turbinia-20240412.1/turbinia/jobs/tomcat.py`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/jobs/volatility.py` & `turbinia-20240412.1/turbinia/jobs/volatility.py`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/jobs/windows_acct.py` & `turbinia-20240412.1/turbinia/jobs/windows_acct.py`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/jobs/wordpress_creds.py` & `turbinia-20240412.1/turbinia/jobs/wordpress_creds.py`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/jobs/worker_stat.py` & `turbinia-20240412.1/turbinia/jobs/worker_stat.py`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/jobs/yara.py` & `turbinia-20240412.1/turbinia/jobs/yara.py`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/lib/docker_manager.py` & `turbinia-20240412.1/turbinia/lib/docker_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import os
 import stat
 import json
 import docker
 
 from turbinia import TurbiniaException
 
-log = logging.getLogger('turbinia')
+log = logging.getLogger(__name__)
 checked_image_list = []
 
 
 def IsBlockDevice(path):
   """Checks path to determine whether it is a block device.
 
   Args:
```

### Comparing `turbinia-20240313/turbinia/lib/dockermanager_test.py` & `turbinia-20240412.1/turbinia/lib/dockermanager_test.py`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/lib/file_helpers.py` & `turbinia-20240412.1/turbinia/lib/file_helpers.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # limitations under the License.
 """Library containing file helpers."""
 
 import os
 import logging
 from tempfile import NamedTemporaryFile
 
-log = logging.getLogger('turbinia')
+log = logging.getLogger(__name__)
 
 
 def file_to_str(file_path):
   """Read file to variable
 
   Args:
     file_path(str): Path to file to be read into variable.
```

### Comparing `turbinia-20240313/turbinia/lib/google_cloud.py` & `turbinia-20240412.1/turbinia/lib/google_cloud.py`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/lib/google_cloud_test.py` & `turbinia-20240412.1/turbinia/lib/google_cloud_test.py`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/lib/llm_libs/llm_client.py` & `turbinia-20240412.1/turbinia/lib/llm_libs/llm_client.py`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/lib/llm_libs/llm_lib_base.py` & `turbinia-20240412.1/turbinia/lib/llm_libs/llm_lib_base.py`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/lib/llm_libs/vertex_ai_lib.py` & `turbinia-20240412.1/turbinia/lib/llm_libs/vertex_ai_lib.py`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/lib/llm_libs/vertex_ai_lib_test.py` & `turbinia-20240412.1/turbinia/lib/llm_libs/vertex_ai_lib_test.py`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/lib/recipe_helpers.py` & `turbinia-20240412.1/turbinia/lib/recipe_helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 from yaml import Loader
 from yaml import load
 from turbinia import TurbiniaException, config
 from turbinia.lib.file_helpers import file_to_str
 from turbinia.lib.file_helpers import file_to_list
 from turbinia.task_utils import TaskLoader
 
-log = logging.getLogger('turbinia')
+log = logging.getLogger(__name__)
 
 #Attributes allowed on the 'globals' task recipe
 DEFAULT_GLOBALS_RECIPE = {
     'debug_tasks': False,
     'jobs_allowlist': [],
     'jobs_denylist': [],
     'yara_rules': '',
```

### Comparing `turbinia-20240313/turbinia/lib/recipe_helpers_test.py` & `turbinia-20240412.1/turbinia/lib/recipe_helpers_test.py`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/lib/text_formatter.py` & `turbinia-20240412.1/turbinia/lib/text_formatter.py`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/lib/text_formatter_test.py` & `turbinia-20240412.1/turbinia/lib/text_formatter_test.py`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/lib/utils.py` & `turbinia-20240412.1/turbinia/lib/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import subprocess
 import tempfile
 import threading
 
 from turbinia import config
 from turbinia import TurbiniaException
 
-log = logging.getLogger('turbinia')
+log = logging.getLogger(__name__)
 
 DEFAULT_TIMEOUT = 7200
 
 
 def _image_export(command, output_dir, disk_path, timeout=DEFAULT_TIMEOUT):
   """Runs image_export command.
```

### Comparing `turbinia-20240313/turbinia/message.py` & `turbinia-20240412.1/turbinia/message.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 import uuid
 import logging
 import six
 
 from turbinia import evidence
 from turbinia import TurbiniaException
 
-log = logging.getLogger('turbinia')
+log = logging.getLogger(__name__)
 
 
 class TurbiniaRequest:
   """An object to request evidence to be processed.
 
   Attributes:
     request_id(str): A client specified ID for this request.
```

### Comparing `turbinia-20240313/turbinia/notify.py` & `turbinia-20240412.1/turbinia/notify.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 import logging
 import smtplib
 from email.mime.multipart import MIMEMultipart
 from email.mime.text import MIMEText
 from turbinia import config
 
-log = logging.getLogger('turbinia')
+log = logging.getLogger(__name__)
 
 
 #Sends notifications via email
 def sendmail(address, subject, message):
   """Sends an Email notification via SMTP
      Args:
          address: This is the address that the email will be sent to
```

### Comparing `turbinia-20240313/turbinia/notify_test.py` & `turbinia-20240412.1/turbinia/notify_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -55,49 +55,49 @@
     # Test that email is not sent when EMAIL_PASSWORD is not defined
     mock_smtp.reset_mock()
     self.config.EMAIL_PASSWORD = ''
     with self.assertLogs('turbinia', level='INFO') as turbinia_info_log:
       notify.sendmail('test@example.com', 'Test Subject', 'Test Message')
       self.assertEqual(
           turbinia_info_log.output[0],
-          'INFO:turbinia:Email password is blank, attempting to continue '
+          'INFO:turbinia.notify:Email password is blank, attempting to continue '
           'without logging in')
       mock_smtp.assert_called_once()
     self.config.EMAIL_PASSWORD = 'testpassword'
 
     # Test that email is not sent when SMTP raises an exception
     mock_smtp.reset_mock()
     mock_smtp.side_effect = SMTPException()
     with self.assertLogs('turbinia', level='ERROR') as turbinia_error_log:
       try:
         notify.sendmail('test@example.com', 'Test Subject', 'Test Message')
       except Exception:
         pass
       self.assertEqual(
           turbinia_error_log.output[1],
-          'ERROR:turbinia:Email failed to send, SMTP has raised an error, '
+          'ERROR:turbinia.notify:Email failed to send, SMTP has raised an error, '
           'this likely means that there is a problem with the config')
 
     # Test that email is not sent when SMTP raises a TypeError
     mock_smtp.side_effect = TypeError()
     with self.assertLogs('turbinia', level='ERROR') as turbinia_error_log:
       try:
         notify.sendmail('test@example.com', 'Test Subject', 'Test Message')
       except Exception:
         pass
       self.assertEqual(
           turbinia_error_log.output[0],
-          'ERROR:turbinia:Email failed to send, there is likely a problem '
+          'ERROR:turbinia.notify:Email failed to send, there is likely a problem '
           'with the config')
 
     # Test that email is not sent when SMTP raises a NameError
     mock_smtp.reset_mock()
     mock_smtp.side_effect = NameError()
     with self.assertLogs('turbinia', level='INFO') as turbinia_info_log:
       try:
         notify.sendmail('test@example.com', 'Test Subject', 'Test Message')
       except Exception:
         pass
       self.assertEqual(
           turbinia_info_log.output[0],
-          'ERROR:turbinia:Email failed to send, A value which is required '
+          'ERROR:turbinia.notify:Email failed to send, A value which is required '
           'for email notifications is not defined in the config')
```

### Comparing `turbinia-20240313/turbinia/output_manager.py` & `turbinia-20240412.1/turbinia/output_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 from turbinia import TurbiniaException
 
 config.LoadConfig()
 if config.GCS_OUTPUT_PATH and config.GCS_OUTPUT_PATH.lower() != 'none':
   from google.cloud import storage
   from google.cloud import exceptions
 
-log = logging.getLogger('turbinia')
+log = logging.getLogger(__name__)
 
 
 class OutputManager:
   """Manages output data.
 
   Manages the configured output writers.  Also saves and retrieves evidence data
   as well as other files that are created when running tasks.
```

### Comparing `turbinia-20240313/turbinia/output_manager_test.py` & `turbinia-20240412.1/turbinia/output_manager_test.py`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/processors/archive.py` & `turbinia-20240412.1/turbinia/processors/archive.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 import os
 import tarfile
 import logging
 
 from time import time
 from turbinia import TurbiniaException
 
-log = logging.getLogger('turbinia')
+log = logging.getLogger(__name__)
 
 
 def ValidateTarFile(compressed_directory):
   """ Validates a given compressed directory path.
 
   Performs a check to determine if the path exists and if
   the file extension is in the list of accepted extensions.
```

### Comparing `turbinia-20240313/turbinia/processors/archive_test.py` & `turbinia-20240412.1/turbinia/processors/archive_test.py`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/processors/containerd.py` & `turbinia-20240412.1/turbinia/processors/containerd.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 import os
 import subprocess
 import tempfile
 
 from turbinia import config
 from turbinia import TurbiniaException
 
-log = logging.getLogger('turbinia')
+log = logging.getLogger(__name__)
 
 
 def PreprocessMountContainerdFS(image_path, namespace, container_id):
   """Mounts a containerd container filesystem locally.
 
   Args:
     image_path (str): Path where evidence disk is mounted.
```

### Comparing `turbinia-20240313/turbinia/processors/docker.py` & `turbinia-20240412.1/turbinia/processors/docker.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import subprocess
 import tempfile
 
 from turbinia import config
 from turbinia import TurbiniaException
 from turbinia.lib import utils
 
-log = logging.getLogger('turbinia')
+log = logging.getLogger(__name__)
 
 
 def PreprocessMountDockerFS(docker_dir, container_id):
   """Mounts a Docker container Filesystem locally.
 
   We use subprocess to run the DockerExplorer script, instead of using the
   Python module, because we need to make sure all DockerExplorer code runs
```

### Comparing `turbinia-20240313/turbinia/processors/google_cloud.py` & `turbinia-20240412.1/turbinia/processors/google_cloud.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 from six.moves import urllib
 
 from libcloudforensics.providers.gcp.internal import project as gcp_project
 from prometheus_client import Counter
 from turbinia import config
 from turbinia import TurbiniaException
 
-log = logging.getLogger('turbinia')
+log = logging.getLogger(__name__)
 
 RETRY_MAX = 10
 ATTACH_SLEEP_TIME = 3
 DETACH_SLEEP_TIME = 5
 
 turbinia_nonexisting_disk_path = Counter(
     'turbinia_nonexisting_disk_path',
```

### Comparing `turbinia-20240313/turbinia/processors/mount_local.py` & `turbinia-20240412.1/turbinia/processors/mount_local.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 import filelock
 import re
 
 from prometheus_client import Counter
 from turbinia import config
 from turbinia import TurbiniaException
 
-log = logging.getLogger('turbinia')
+log = logging.getLogger(__name__)
 
 RETRY_MAX = 10
 
 turbinia_failed_loop_device_detach = Counter(
     'turbinia_failed_loop_device_detach',
     'Total number of loop devices failed to detach')
```

### Comparing `turbinia-20240313/turbinia/processors/mount_local_test.py` & `turbinia-20240412.1/turbinia/processors/mount_local_test.py`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/processors/partitions.py` & `turbinia-20240412.1/turbinia/processors/partitions.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 from dfvfs.helpers import volume_scanner
 from dfvfs.lib import definitions as dfvfs_definitions
 from dfvfs.lib import errors as dfvfs_errors
 
 from turbinia import TurbiniaException
 
-log = logging.getLogger('turbinia')
+log = logging.getLogger(__name__)
 
 
 def Enumerate(evidence, location=None):
   """Uses dfVFS to enumerate partitions in a disk / image.
 
   Args:
     evidence: Evidence object to be scanned.
@@ -59,16 +59,16 @@
   try:
     # Setting the volume scanner mediator to None will cause the volume scanner
     # to operate in unattended mode
     scanner = volume_scanner.VolumeScanner(mediator=None)
     path_specs = scanner.GetBasePathSpecs(evidence.local_path, options=options)
   except dfvfs_errors.ScannerError as exception:
     raise TurbiniaException(
-        f'Could not enumerate partitions [{evidence.local_path!s}]: {exception!s}'
-    )
+        f'Could not enumerate partitions [{evidence.local_path!s}]: '
+        f'{exception!s}') from exception
 
   return path_specs
 
 
 def GetPartitionEncryptionType(path_spec):
   """Checks a partition for encryption.
 
@@ -81,10 +81,11 @@
   encryption_type = None
 
   if not path_spec or not path_spec.HasParent():
     return None
 
   if path_spec.parent.type_indicator == dfvfs_definitions.TYPE_INDICATOR_BDE:
     encryption_type = 'BDE'
-  elif path_spec.parent.type_indicator == dfvfs_definitions.TYPE_INDICATOR_LUKSDE:
+  elif path_spec.parent.type_indicator == (
+      dfvfs_definitions.TYPE_INDICATOR_LUKSDE):
     encryption_type = 'LUKSDE'
   return encryption_type
```

### Comparing `turbinia-20240313/turbinia/processors/partitions_test.py` & `turbinia-20240412.1/turbinia/processors/partitions_test.py`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/processors/resource_manager.py` & `turbinia-20240412.1/turbinia/processors/resource_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 import os
 import json
 
 from turbinia import config
 from turbinia import TurbiniaException
 
 config.LoadConfig()
-log = logging.getLogger('turbinia')
+log = logging.getLogger(__name__)
 
 
 def RetrieveResourceState():
   """Creates a resource file if it doesn't exist and load resource state into a json object.
   
     Returns:
       json_load(dict): The resource state json object.
```

### Comparing `turbinia-20240313/turbinia/processors/resource_manager_test.py` & `turbinia-20240412.1/turbinia/processors/resource_manager_test.py`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/server.py` & `turbinia-20240412.1/turbinia/server.py`

 * *Files 3% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 
     Args:
       jobs_denylist (Optional[list[str]]): Jobs we will exclude from running
       jobs_allowlist (Optional[list[str]]): The only Jobs we will include to run
     """
     setup()
     self.task_manager = task_manager.get_task_manager()
-    self.task_manager.setup(jobs_denylist, jobs_allowlist)
+    self.task_manager.setup(jobs_denylist, jobs_allowlist, server=True)
 
   def start(self):
     """Start Turbinia Server."""
     if config.PROMETHEUS_ENABLED:
       if config.PROMETHEUS_PORT and config.PROMETHEUS_ADDR:
         log.info('Starting Prometheus endpoint.')
         start_http_server(
```

### Comparing `turbinia-20240313/turbinia/server_test.py` & `turbinia-20240412.1/turbinia/server_test.py`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/state_manager.py` & `turbinia-20240412.1/turbinia/state_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
   import redis
 else:
   msg = f'State Manager type "{config.STATE_MANAGER:s}" not implemented'
   raise TurbiniaException(msg)
 
 EMPTY_JSON_VALUES = ('null', '{}', '[]')
 MAX_DATASTORE_STRLEN = 1500
-log = logging.getLogger('turbinia')
+log = logging.getLogger(__name__)
 
 
 def get_state_manager():
   """Return state manager object based on config.
 
   Returns:
     Initialized StateManager object.
```

### Comparing `turbinia-20240313/turbinia/state_manager_test.py` & `turbinia-20240412.1/turbinia/state_manager_test.py`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/task_manager.py` & `turbinia-20240412.1/turbinia/task_manager.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 
 config.LoadConfig()
 
 if config.TASK_MANAGER.lower() == 'celery':
   from celery import states as celery_states
   from turbinia import tcelery as turbinia_celery
 
-log = logging.getLogger('turbinia')
+log = logging.getLogger(__name__)
 
 # The amount of time in seconds that the Server will wait in addition to the
 # Job/Task timeout value before it times out a given Task. This is to make sure
 # that the Server doesn't time out the Task before the Worker has a chance to
 # and should account for the Task scheduling and setup time that happens before
 # the Task starts.
 SERVER_TASK_TIMEOUT_BUFFER = 86400
@@ -128,40 +128,44 @@
   def setup(self, jobs_denylist=None, jobs_allowlist=None, *args, **kwargs):
     """Does setup of Task manager and its dependencies.
 
     Args:
       jobs_denylist (list): Jobs that will be excluded from running
       jobs_allowlist (list): The only Jobs will be included to run
     """
+    # Both client and server isntances of the task  manager require backends.
     self._backend_setup(*args, **kwargs)
+    # Only server instances of the task manager need to set up jobs.
+    if kwargs.get('server') is False:
+      return
     job_names = jobs_manager.JobsManager.GetJobNames()
     if jobs_denylist or jobs_allowlist:
       selected_jobs = jobs_denylist or jobs_allowlist
       for job in selected_jobs:
         if job.lower() not in job_names:
           msg = (
-              'Error creating server. Job {0!s} is not found in registered '
-              'jobs {1!s}.'.format(job, job_names))
+              f'Error creating server. Job {job} is not found in registered'
+              f' jobs {job_names}')
           log.error(msg)
           raise TurbiniaException(msg)
       log.info(
-          'Filtering Jobs with allowlist {0!s} and denylist {1!s}'.format(
-              jobs_allowlist, jobs_denylist))
+          f'Filtering Jobs with allowlist {jobs_allowlist} and denylist '
+          f'{jobs_denylist}')
       job_names = jobs_manager.JobsManager.FilterJobNames(
           job_names, jobs_denylist, jobs_allowlist)
 
     # Disable any jobs from the config that were not previously allowlisted.
     disabled_jobs = list(config.DISABLED_JOBS) if config.DISABLED_JOBS else []
     disabled_jobs = [j.lower() for j in disabled_jobs]
     if jobs_allowlist:
       disabled_jobs = list(set(disabled_jobs) - set(jobs_allowlist))
     if disabled_jobs:
       log.info(
-          'Disabling non-allowlisted jobs configured to be disabled in the '
-          'config file: {0:s}'.format(', '.join(disabled_jobs)))
+          f'Disabling non-allowlisted jobs configured to be disabled in '
+          f'the config file: {", ".join(disabled_jobs)}')
       job_names = jobs_manager.JobsManager.FilterJobNames(
           job_names, disabled_jobs, [])
 
     self.jobs = [job for _, job in jobs_manager.JobsManager.GetJobs(job_names)]
     dependencies = config.ParseDependencies()
     job_utils.register_job_timeouts(dependencies)
     log.debug(f'Registered job list: {str(job_names):s}')
@@ -179,15 +183,16 @@
       requester(str): The username of the requester.
       evidence_name(str): Name of the Evidence requested to be processed.
       message(str): The error message to abort the request with.
     """
     abort_task = AbortTask(request_id=request_id, requester=requester)
     result = workers.TurbiniaTaskResult(
         request_id=request_id, no_output_manager=True)
-    result.status = f'Processing request for {evidence_name:s} aborted: {message:s}'
+    result.status = (
+        f'Processing request for {evidence_name:s} aborted: {message:s}')
     result.successful = False
     abort_task.result = result
     self.state_manager.update_task(abort_task)
 
   def add_evidence(self, evidence_):
     """Adds new evidence and creates tasks to process it.
 
@@ -206,16 +211,16 @@
     job_count = 0
     jobs_list = []
 
     jobs_allowlist = evidence_.config['globals'].get('jobs_allowlist', [])
     jobs_denylist = evidence_.config['globals'].get('jobs_denylist', [])
     if jobs_denylist or jobs_allowlist:
       log.info(
-          'Filtering Jobs with allowlist {0!s} and denylist {1!s}'.format(
-              jobs_allowlist, jobs_denylist))
+          f'Filtering Jobs with allowlist {jobs_allowlist} and denylist '
+          f'{jobs_denylist}')
       jobs_list = jobs_manager.JobsManager.FilterJobObjects(
           self.jobs, jobs_denylist, jobs_allowlist)
     else:
       jobs_list = self.jobs
 
     # TODO(aarontp): Add some kind of loop detection in here so that jobs can
     # register for Evidence(), or or other evidence types that may be a super
@@ -248,18 +253,17 @@
       except TurbiniaException as exception:
         log.error(f'Error writing new evidence to redis: {exception}')
       else:
         self.state_manager.write_evidence(evidence_.serialize(json_values=True))
 
     if not job_count:
       log.warning(
-          'No Jobs/Tasks were created for Evidence [{0:s}]. '
-          'Request or recipe parsing may have failed, or Jobs may need to be '
-          'configured to allow this type of Evidence as input'.format(
-              str(evidence_)))
+          f'No Jobs/Tasks were created for Evidence {str(evidence_)}. '
+          f'Request or recipe parsing may have failed, or Jobs may need to be '
+          f'configured to allow this type of Evidence as input')
 
   def check_done(self):
     """Checks if we have any outstanding tasks.
 
     Returns:
       bool: Indicating whether we are done.
     """
@@ -362,16 +366,16 @@
       job (TurbiniaJob): The last Job that was run for this request.
     """
     request_id = job.request_id
     final_job = jobs_manager.JobsManager.GetJobInstance('FinalizeRequestJob')
     final_job.request_id = request_id
     final_job.evidence.config = job.evidence.config
     log.debug(
-        'Request {0:s} done, but not finalized, creating FinalizeRequestJob '
-        '{1:s}'.format(request_id, final_job.id))
+        f'Request {request_id} done, but not finalized, creating '
+        f'FinalizeRequestJob{final_job.id}')
 
     # Finalize tasks use EvidenceCollection with all evidence created by the
     # request or job.
     final_evidence = evidence.EvidenceCollection()
     final_evidence.request_id = request_id
     self.running_jobs.append(final_job)
     turbinia_jobs_total.inc()
@@ -393,16 +397,16 @@
     """
     if evidence_.request_id:
       task.request_id = evidence_.request_id
     elif job and job.request_id:
       task.request_id = job.request_id
     else:
       log.error(
-          'Request ID not found in Evidence {0!s} or Task {1!s}. Not adding '
-          'new Task because of undefined state'.format(evidence_, task))
+          f'Request ID not found in Evidence {evidence_} or Task {task}.'
+          f' Not adding new Task because of undefined state')
       return
 
     evidence_.config = job.evidence.config
     task.evidence_name = evidence_.name
     task.base_output_dir = config.OUTPUT_DIR
     task.requester = evidence_.config.get('globals', {}).get('requester')
     task.group_name = evidence_.config.get('globals', {}).get('group_name')
@@ -423,16 +427,16 @@
     """Removes the all Jobs for the given request ID.
 
     Args:
       request_id (str): The ID of the request we want to remove jobs for.
     """
     remove_jobs = [j for j in self.running_jobs if j.request_id == request_id]
     log.debug(
-        'Removing {0:d} completed Job(s) for request ID {1:s}.'.format(
-            len(remove_jobs), request_id))
+        f'Removing {len(remove_jobs)} completed Job(s) for request ID '
+        f'{request_id}.')
     # pylint: disable=expression-not-assigned
     [self.remove_job(j.id) for j in remove_jobs]
 
   def remove_job(self, job_id):
     """Removes a Job from the running jobs list.
 
     Args:
@@ -475,63 +479,61 @@
       task_result: The TurbiniaTaskResult object
 
     Returns:
       TurbiniaJob|None: The Job for the processed task, else None
     """
     if task_result.successful is None:
       log.error(
-          'Task {0:s} from {1:s} returned invalid success status "None". '
-          'Setting this to False so the client knows the Task is complete. '
-          'Usually this means that the Task returning the TurbiniaTaskResult '
-          'did not call the close() method on it.'.format(
-              task_result.task_name, task_result.worker_name))
+          f'''Task {task_result.task_name} from {task_result.worker_name}  
+          returned invalid success status "None". Setting this to False 
+          so the client knows the Task is complete. Usually this means 
+          that the Task returning the TurbiniaTaskResult did not call 
+          the close() method on it.
+        ''')
       turbinia_result_success_invalid.inc()
       task_result.successful = False
       if task_result.status:
         task_result.status = (
             task_result.status + ' (Success status forcefully set to False)')
 
     if not task_result.successful:
       log.error(
-          'Task {0:s} from {1:s} was not successful'.format(
-              task_result.task_name, task_result.worker_name))
+          f'Task {task_result.task_name} from {task_result.worker_name} '
+          f'was not successful')
     else:
       log.info(
-          'Task {0:s} from {1:s} executed with status [{2:s}]'.format(
-              task_result.task_name, task_result.worker_name,
-              task_result.status))
+          f'Task {task_result.task_name} from {task_result.worker_name} '
+          f'executed with status [{task_result.status}]')
 
     if not isinstance(task_result.evidence, list):
       log.warning(
-          'Task {0:s} from {1:s} did not return evidence list'.format(
-              task_result.task_name, task_result.worker_name))
+          f'Task {task_result.task_name} from {task_result.worker_name} '
+          f'did not return evidence list')
       task_result.evidence = []
 
     job = self.get_job(task_result.job_id)
     if not job:
       log.warning(
-          f'Received task results for unknown Job from Task ID {task_result.task_id:s}'
-      )
+          f'Received task results for unknown Job from Task ID '
+          f'{task_result.task_id:s}')
 
     # Reprocess new evidence and save instance for later consumption by finalize
     # tasks.
     for evidence_ in task_result.evidence:
       if isinstance(evidence_, evidence.Evidence):
         log.info(
-            'Task {0:s} from {1:s} returned Evidence {2:s}'.format(
-                task_result.task_name, task_result.worker_name, evidence_.name))
+            f'Task {task_result.task_name} from {task_result.worker_name} '
+            f'returned Evidence {evidence_.name}')
         self.add_evidence(evidence_)
         if job:
           job.evidence.add_evidence(evidence_)
       else:
         log.error(
-            'Task {0:s} from {1:s} returned non-Evidence output type '
-            '{2:s}'.format(
-                task_result.task_name, task_result.worker_name,
-                type(task_result.evidence)))
+            f'Task {task_result.task_name} from {task_result.worker_name} '
+            f'returned non-Evidence output type {type(task_result.evidence)}')
 
     return job
 
   def process_job(self, job, task):
     """Processes the Job after Task completes.
 
     This removes the Task from the running Job and generates the "finalize"
@@ -610,16 +612,16 @@
       TurbiniaTask: The updated Task.
     """
     result = workers.TurbiniaTaskResult(
         request_id=task.request_id, no_output_manager=True,
         no_state_manager=True)
     result.setup(task)
     result.status = (
-        'Task {0:s} timed out on the Server and was auto-closed after '
-        '{1:d} seconds'.format(task.name, timeout))
+        f'Task {task.name} timed out on the Server and was '
+        f'auto-closed after {timeout} seconds')
     result.successful = False
     result.closed = True
     task.result = result
     turbinia_server_task_timeout_total.inc()
 
     return task
 
@@ -637,20 +639,21 @@
     self.celery = None
     self.kombu = None
     self.celery_runner = None
     config.LoadConfig()
     super(CeleryTaskManager, self).__init__()
 
   def _backend_setup(self, *args, **kwargs):
-    self.celery = turbinia_celery.TurbiniaCelery()
-    self.celery.setup()
     self.kombu = turbinia_celery.TurbiniaKombu(config.KOMBU_CHANNEL)
     self.kombu.setup()
-    self.celery_runner = self.celery.app.task(
-        task_utils.task_runner, name="task_runner")
+    if kwargs.get('server') is True:
+      self.celery = turbinia_celery.TurbiniaCelery()
+      self.celery.setup()
+      self.celery_runner = self.celery.app.task(
+          task_utils.task_runner, name='task_runner')
 
   def process_tasks(self):
     """Determine the current state of our tasks.
 
     Returns:
       list[TurbiniaTask]: all completed tasks
     """
@@ -676,16 +679,16 @@
 
       # For certain Task states we want to check whether the Task has timed out
       # or not.
       if check_timeout:
         timeout = self.check_task_timeout(task)
         if timeout:
           log.warning(
-              'Task {0:s} timed out on server after {1:d} seconds. '
-              'Auto-closing Task.'.format(celery_task.id, timeout))
+              f'Task {celery_task.id} timed out on server after '
+              f'{timeout} seconds. Auto-closing Task')
           task = self.timeout_task(task, timeout)
           completed_tasks.append(task)
 
     outstanding_task_count = len(self.tasks) - len(completed_tasks)
     if outstanding_task_count > 0:
       log.info(f'{outstanding_task_count:d} Tasks still outstanding.')
     return completed_tasks
@@ -732,11 +735,11 @@
           evidence_list.append(evidence_)
       turbinia_server_request_total.inc()
 
     return evidence_list
 
   def enqueue_task(self, task, evidence_):
     log.info(
-        f'Adding Celery task {task.name:s} with evidence {evidence_.name:s} to queue'
-    )
+        f'Adding Celery task {task.name:s} with evidence  {evidence_.name:s}'
+        f' to queue')
     task.stub = self.celery_runner.delay(
         task.serialize(), evidence_.serialize())
```

### Comparing `turbinia-20240313/turbinia/task_manager_test.py` & `turbinia-20240412.1/turbinia/task_manager_test.py`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/task_utils.py` & `turbinia-20240412.1/turbinia/task_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 import logging
 import filelock
 
 from turbinia import config
 from turbinia.config import DATETIME_FORMAT
 from turbinia import TurbiniaException
 
-log = logging.getLogger('turbinia')
+log = logging.getLogger(__name__)
 
 config.LoadConfig()
 
 
 class TaskLoader():
   """Utility class for handling Task loading/checking/deserialization.
```

### Comparing `turbinia-20240313/turbinia/task_utils_test.py` & `turbinia-20240412.1/turbinia/task_utils_test.py`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/tcelery.py` & `turbinia-20240412.1/turbinia/tcelery.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 import kombu
 from kombu.exceptions import OperationalError
 from amqp.exceptions import ChannelError
 
 from turbinia import config
 from turbinia.message import TurbiniaMessageBase
 
-log = logging.getLogger('turbinia')
+log = logging.getLogger(__name__)
 
 
 class TurbiniaCelery:
   """Celery app object.
 
   Attributes:
     app (Celery): The Celery app itself.
@@ -52,15 +52,14 @@
     config.LoadConfig()
     self.app = celery.Celery(
         'turbinia', broker=config.CELERY_BROKER, backend=config.CELERY_BACKEND)
     self.app.conf.update(
         broker_connection_retry_on_startup=True,
         task_default_queue=config.INSTANCE_ID,
         accept_content=['json'],
-        task_acks_late=True,
         worker_cancel_long_running_tasks_on_connection_loss=True,
         worker_concurrency=1,
         worker_prefetch_multiplier=1,
     )
 
 
 class TurbiniaKombu(TurbiniaMessageBase):
```

### Comparing `turbinia-20240313/turbinia/worker.py` & `turbinia-20240412.1/turbinia/worker.py`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/worker_test.py` & `turbinia-20240412.1/turbinia/worker_test.py`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/workers/__init__.py` & `turbinia-20240412.1/turbinia/workers/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 # Set the maximum size that the report can be before truncating it.  This is a
 # best effort estimate and not a guarantee and comes from the limit for
 # datastore entities[1] less some overhead for the rest of the attributes that
 # will be saved in the response.
 # [1]https://cloud.google.com/datastore/docs/concepts/limits
 REPORT_MAXSIZE = int(1048572 * 0.75)
 
-log = logging.getLogger('turbinia')
+log = logging.getLogger(__name__)
 
 registry = CollectorRegistry()
 turbinia_worker_tasks_started_total = Counter(
     'turbinia_worker_tasks_started_total',
     'Total number of started worker tasks', registry=registry)
 turbinia_worker_tasks_completed_total = Counter(
     'turbinia_worker_tasks_completed_total',
```

### Comparing `turbinia-20240313/turbinia/workers/abort.py` & `turbinia-20240412.1/turbinia/workers/abort.py`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/workers/analysis/analyzer_output.py` & `turbinia-20240412.1/turbinia/workers/analysis/analyzer_output.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # limitations under the License.
 """A class to store analyzer output"""
 
 import logging
 
 from turbinia import TurbiniaException
 
-log = logging.getLogger('turbinia')
+log = logging.getLogger(__name__)
 
 
 class AnalyzerOutput:
   """A class to record analyzer output.
 
   Attributes:
     platform (str): [Required] Analyzer platfrom.
```

### Comparing `turbinia-20240313/turbinia/workers/analysis/auth.py` & `turbinia-20240412.1/turbinia/workers/analysis/auth.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from datetime import datetime, timezone
 from typing import List, Tuple
 
 from turbinia import TurbiniaException
 from turbinia.workers import Priority
 from turbinia.workers.analysis.analyzer_output import AnalyzerOutput
 
-log = logging.getLogger('turbinia')
+log = logging.getLogger(__name__)
 
 
 class LoginRecord:
   """Successful login record.
   
   Attributes:
     timestamp (int): Timestamp of successful login event in seconds.
```

### Comparing `turbinia-20240313/turbinia/workers/analysis/auth_test.py` & `turbinia-20240412.1/turbinia/workers/analysis/auth_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 from turbinia.workers.analysis.analyzer_output import AnalyzerOutput
 from turbinia.workers.analysis.auth import AuthAnalyzer
 from turbinia.workers.analysis.auth import AuthSummaryData
 from turbinia.workers.analysis.auth import BruteForceAnalyzer
 from turbinia.workers.analysis.auth import LoginRecord
 from turbinia.workers.analysis.ssh_analyzer import LinuxSSHAnalysisTask
 
-log = logging.getLogger('turbinia')
+log = logging.getLogger(__name__)
 log.addHandler(logging.StreamHandler(sys.stdout))
 log.setLevel(logging.DEBUG)
 
 
 def load_test_dataframe() -> pd.DataFrame:
   """Loads SSH log file and returns dataframe."""
   log_file = os.path.join('test_data', 'secure')
```

### Comparing `turbinia-20240313/turbinia/workers/analysis/jenkins.py` & `turbinia-20240412.1/turbinia/workers/analysis/jenkins.py`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/workers/analysis/jenkins_test.py` & `turbinia-20240412.1/turbinia/workers/analysis/jenkins_test.py`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/workers/analysis/jupyter.py` & `turbinia-20240412.1/turbinia/workers/analysis/jupyter.py`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/workers/analysis/jupyter_test.py` & `turbinia-20240412.1/turbinia/workers/analysis/jupyter_test.py`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/workers/analysis/linux_acct.py` & `turbinia-20240412.1/turbinia/workers/analysis/linux_acct.py`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/workers/analysis/linux_acct_test.py` & `turbinia-20240412.1/turbinia/workers/analysis/linux_acct_test.py`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/workers/analysis/llm_analyzer.py` & `turbinia-20240412.1/turbinia/workers/analysis/llm_analyzer.py`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/workers/analysis/llm_analyzer_test.py` & `turbinia-20240412.1/turbinia/workers/analysis/llm_analyzer_test.py`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/workers/analysis/postgresql_acct.py` & `turbinia-20240412.1/turbinia/workers/analysis/postgresql_acct.py`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/workers/analysis/postgresql_acct_test.py` & `turbinia-20240412.1/turbinia/workers/analysis/postgresql_acct_test.py`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/workers/analysis/redis.py` & `turbinia-20240412.1/turbinia/workers/analysis/redis.py`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/workers/analysis/redis_test.py` & `turbinia-20240412.1/turbinia/workers/analysis/redis_test.py`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/workers/analysis/ssh_analyzer.py` & `turbinia-20240412.1/turbinia/workers/analysis/ssh_analyzer.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 from turbinia.evidence import ReportText
 from turbinia.lib.utils import extract_artifacts
 from turbinia.workers import Priority
 from turbinia.workers import TurbiniaTask
 from turbinia.workers import TurbiniaTaskResult
 from turbinia.workers.analysis.auth import BruteForceAnalyzer
 
-log = logging.getLogger('turbinia')
+log = logging.getLogger(__name__)
 
 
 class SSHEventData:
   """SSH authentication event."""
 
   def __init__(
       self, timestamp: int, date: str, time: str, hostname: str, pid: int,
```

### Comparing `turbinia-20240313/turbinia/workers/analysis/ssh_analyzer_test.py` & `turbinia-20240412.1/turbinia/workers/analysis/ssh_analyzer_test.py`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/workers/analysis/sshd.py` & `turbinia-20240412.1/turbinia/workers/analysis/sshd.py`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/workers/analysis/sshd_test.py` & `turbinia-20240412.1/turbinia/workers/analysis/sshd_test.py`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/workers/analysis/tomcat.py` & `turbinia-20240412.1/turbinia/workers/analysis/tomcat.py`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/workers/analysis/tomcat_test.py` & `turbinia-20240412.1/turbinia/workers/analysis/tomcat_test.py`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/workers/analysis/windows_acct.py` & `turbinia-20240412.1/turbinia/workers/analysis/windows_acct.py`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/workers/analysis/windows_acct_test.py` & `turbinia-20240412.1/turbinia/workers/analysis/windows_acct_test.py`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/workers/analysis/wordpress_access.py` & `turbinia-20240412.1/turbinia/workers/analysis/wordpress_access.py`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/workers/analysis/wordpress_access_test.py` & `turbinia-20240412.1/turbinia/workers/analysis/wordpress_access_test.py`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/workers/analysis/wordpress_creds.py` & `turbinia-20240412.1/turbinia/workers/analysis/wordpress_creds.py`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/workers/analysis/wordpress_creds_test.py` & `turbinia-20240412.1/turbinia/workers/analysis/wordpress_creds_test.py`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/workers/analysis/yara.py` & `turbinia-20240412.1/turbinia/workers/analysis/yara.py`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/workers/analysis/yara_test.py` & `turbinia-20240412.1/turbinia/workers/analysis/yara_test.py`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/workers/artifact.py` & `turbinia-20240412.1/turbinia/workers/artifact.py`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/workers/binary_extractor.py` & `turbinia-20240412.1/turbinia/workers/binary_extractor.py`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/workers/binary_extractor_test.py` & `turbinia-20240412.1/turbinia/workers/binary_extractor_test.py`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/workers/bulk_extractor.py` & `turbinia-20240412.1/turbinia/workers/bulk_extractor.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from turbinia import TurbiniaException
 from turbinia import config
 from turbinia.evidence import BulkExtractorOutput
 from turbinia.evidence import EvidenceState as state
 from turbinia.lib import text_formatter as fmt
 from turbinia.workers import TurbiniaTask
 
-log = logging.getLogger('turbinia')
+log = logging.getLogger(__name__)
 
 REPORT_FILENAME = "report.md"
 
 
 class BulkExtractorTask(TurbiniaTask):
   """Task to generate Bulk Extractor output."""
```

### Comparing `turbinia-20240313/turbinia/workers/bulk_extractor_test.py` & `turbinia-20240412.1/turbinia/workers/bulk_extractor_test.py`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/workers/containerd.py` & `turbinia-20240412.1/turbinia/workers/containerd.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 from turbinia import config
 from turbinia import TurbiniaException
 from turbinia.evidence import ContainerdContainer
 from turbinia.evidence import EvidenceState as state
 from turbinia.workers import Priority
 from turbinia.workers import TurbiniaTask
 
-log = logging.getLogger('turbinia')
+log = logging.getLogger(__name__)
 
 CE_BINARY = '/opt/container-explorer/bin/ce'
 CE_SUPPORT_FILE = '/opt/container-explorer/etc/supportcontainer.yaml'
 POD_NAME_LABEL = 'io.kubernetes.pod.name'
 
 
 class ContainerdEnumerationTask(TurbiniaTask):
```

### Comparing `turbinia-20240313/turbinia/workers/containerd_test.py` & `turbinia-20240412.1/turbinia/workers/containerd_test.py`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/workers/dfdewey.py` & `turbinia-20240412.1/turbinia/workers/dfdewey.py`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/workers/dfdewey_test.py` & `turbinia-20240412.1/turbinia/workers/dfdewey_test.py`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/workers/docker.py` & `turbinia-20240412.1/turbinia/workers/docker.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 from turbinia.evidence import DockerContainer
 from turbinia.evidence import EvidenceState as state
 from turbinia.lib import utils
 from turbinia.workers import Priority
 from turbinia.workers import TurbiniaTask
 from turbinia import config
 
-log = logging.getLogger('turbinia')
+log = logging.getLogger(__name__)
 
 
 class DockerContainersEnumerationTask(TurbiniaTask):
   """Enumerates Docker containers on Linux"""
 
   REQUIRED_STATES = [state.ATTACHED, state.MOUNTED]
```

### Comparing `turbinia-20240313/turbinia/workers/docker_test.py` & `turbinia-20240412.1/turbinia/workers/docker_test.py`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/workers/file_system_timeline.py` & `turbinia-20240412.1/turbinia/workers/file_system_timeline.py`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/workers/file_system_timeline_test.py` & `turbinia-20240412.1/turbinia/workers/file_system_timeline_test.py`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/workers/finalize_request.py` & `turbinia-20240412.1/turbinia/workers/finalize_request.py`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/workers/fsstat.py` & `turbinia-20240412.1/turbinia/workers/fsstat.py`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/workers/fsstat_test.py` & `turbinia-20240412.1/turbinia/workers/fsstat_test.py`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/workers/grep.py` & `turbinia-20240412.1/turbinia/workers/grep.py`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/workers/hindsight.py` & `turbinia-20240412.1/turbinia/workers/hindsight.py`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/workers/partitions.py` & `turbinia-20240412.1/turbinia/workers/partitions.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
     from turbinia.processors import mount_local
     from turbinia.processors import partitions
   except ImportError as exception:
     message = f'Could not import dfVFS libraries: {exception!s}'
     raise TurbiniaException(message)
 
-log = logging.getLogger('turbinia')
+log = logging.getLogger(__name__)
 
 
 class PartitionEnumerationTask(TurbiniaTask):
   """Task to enumerate partitions in a disk."""
 
   REQUIRED_STATES = [EvidenceState.ATTACHED]
```

### Comparing `turbinia-20240313/turbinia/workers/partitions_test.py` & `turbinia-20240412.1/turbinia/workers/partitions_test.py`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/workers/photorec.py` & `turbinia-20240412.1/turbinia/workers/photorec.py`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/workers/photorec_test.py` & `turbinia-20240412.1/turbinia/workers/photorec_test.py`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/workers/plaso.py` & `turbinia-20240412.1/turbinia/workers/plaso.py`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/workers/plaso_test.py` & `turbinia-20240412.1/turbinia/workers/plaso_test.py`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/workers/psort.py` & `turbinia-20240412.1/turbinia/workers/psort.py`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/workers/strings.py` & `turbinia-20240412.1/turbinia/workers/strings.py`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/workers/volatility.py` & `turbinia-20240412.1/turbinia/workers/volatility.py`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/workers/volatility_test.py` & `turbinia-20240412.1/turbinia/workers/volatility_test.py`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/workers/worker_stat.py` & `turbinia-20240412.1/turbinia/workers/worker_stat.py`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/workers/workers_test.py` & `turbinia-20240412.1/turbinia/workers/workers_test.py`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/turbinia/yapf_test.py` & `turbinia-20240412.1/turbinia/yapf_test.py`

 * *Files identical despite different names*

### Comparing `turbinia-20240313/PKG-INFO` & `turbinia-20240412.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: turbinia
-Version: 20240313
+Version: 20240412.1
 Summary: Automation and Scaling of Digital Forensics Tools
 Home-page: https://github.com/google/turbinia
 License: Apache-2.0
 Author: Turbinia Developers
 Author-email: turbinia-dev@googlegroups.com
 Maintainer: Turbinia Developers
 Maintainer-email: turbinia-dev@googlegroups.com
@@ -13,22 +13,23 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: worker
 Requires-Dist: backoff (>=2.2.1)
 Requires-Dist: celery (>=5.2.2,<6.0.0)
-Requires-Dist: dfDewey (>=20220603,<20220604) ; extra == "worker"
-Requires-Dist: dfimagetools (>=20230806,<20230807) ; extra == "worker"
+Requires-Dist: dfDewey (>=20231016,<20231017) ; extra == "worker"
+Requires-Dist: dfimagetools (>=20240301,<20240302) ; extra == "worker"
 Requires-Dist: docker (>=6.1.3,<7.0.0)
 Requires-Dist: fastapi[all] (>=0.75.0,<0.99.0)
 Requires-Dist: filelock
 Requires-Dist: google-api-core (<3.0.0)
 Requires-Dist: google-generativeai (>=0.3.2)
-Requires-Dist: libcloudforensics (==20240214)
+Requires-Dist: libcloudforensics (>=20240325,<20240326)
+Requires-Dist: opensearch-py (==2.4.2)
 Requires-Dist: pandas (>=2.1.0,<3.0.0)
 Requires-Dist: plaso (==20240308) ; extra == "worker"
 Requires-Dist: prometheus_client (>=0.17.1,<0.18.0)
 Requires-Dist: protobuf (>=3.19.0)
 Requires-Dist: pydantic (>=1.10.5,<2.0.0)
 Requires-Dist: pyglove (>=0.4.4)
 Requires-Dist: pyhindsight (>=20230327.0,<20230328.0) ; extra == "worker"
@@ -37,14 +38,15 @@
 Requires-Dist: urllib3 (>=1.25.4,<1.27) ; python_version < "3.10"
 Requires-Dist: urllib3 (>=1.25.4,<2.1) ; python_version >= "3.10"
 Project-URL: Documentation, https://turbinia.readthedocs.io/en/latest/
 Project-URL: Repository, https://github.com/google/turbinia
 Description-Content-Type: text/markdown
 
 # Turbinia
+![Unit tests](https://github.com/google/turbinia/actions/workflows/actions.yml/badge.svg) ![e2e tests](https://github.com/google/turbinia/actions/workflows/e2e.yml/badge.svg)
 
 ## Summary
 
 Turbinia is an open-source framework for deploying, managing, and running
 distributed forensic workloads. It is intended to automate running of common
 forensic processing tools (i.e. Plaso, TSK, strings, etc) to help with
 processing evidence in the Cloud, scaling the processing of large amounts of
```


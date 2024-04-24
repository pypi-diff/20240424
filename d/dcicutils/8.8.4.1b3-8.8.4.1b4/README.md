# Comparing `tmp/dcicutils-8.8.4.1b3.tar.gz` & `tmp/dcicutils-8.8.4.1b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcicutils-8.8.4.1b3.tar", max compression
+gzip compressed data, was "dcicutils-8.8.4.1b4.tar", max compression
```

## Comparing `dcicutils-8.8.4.1b3.tar` & `dcicutils-8.8.4.1b4.tar`

### file list

```diff
@@ -1,79 +1,79 @@
--rw-r--r--   0        0        0     1102 2024-04-24 13:43:25.075500 dcicutils-8.8.4.1b3/LICENSE.txt
--rw-r--r--   0        0        0     1166 2024-04-24 13:43:25.075500 dcicutils-8.8.4.1b3/README.rst
--rw-r--r--   0        0        0        0 2024-04-24 13:43:25.075500 dcicutils-8.8.4.1b3/dcicutils/__init__.py
--rw-r--r--   0        0        0     5115 2024-04-24 13:43:25.075500 dcicutils-8.8.4.1b3/dcicutils/base.py
--rwxr-xr-x   0        0        0    51434 2024-04-24 13:43:25.075500 dcicutils-8.8.4.1b3/dcicutils/beanstalk_utils.py
--rw-r--r--   0        0        0    34669 2024-04-24 13:43:25.075500 dcicutils-8.8.4.1b3/dcicutils/bundle_utils.py
--rw-r--r--   0        0        0     3295 2024-04-24 13:43:25.075500 dcicutils-8.8.4.1b3/dcicutils/captured_output.py
--rw-r--r--   0        0        0    13786 2024-04-24 13:43:25.075500 dcicutils-8.8.4.1b3/dcicutils/cloudformation_utils.py
--rw-r--r--   0        0        0     1155 2024-04-24 13:43:25.075500 dcicutils-8.8.4.1b3/dcicutils/codebuild_utils.py
--rw-r--r--   0        0        0    15285 2024-04-24 13:43:25.075500 dcicutils-8.8.4.1b3/dcicutils/command_utils.py
--rw-r--r--   0        0        0     3955 2024-04-24 13:43:25.075500 dcicutils-8.8.4.1b3/dcicutils/common.py
--rw-r--r--   0        0        0     2015 2024-04-24 13:43:25.075500 dcicutils-8.8.4.1b3/dcicutils/contribution_scripts.py
--rw-r--r--   0        0        0    25653 2024-04-24 13:43:25.075500 dcicutils-8.8.4.1b3/dcicutils/contribution_utils.py
--rw-r--r--   0        0        0    11113 2024-04-24 13:43:25.075500 dcicutils-8.8.4.1b3/dcicutils/creds_utils.py
--rw-r--r--   0        0        0     7626 2024-04-24 13:43:25.075500 dcicutils-8.8.4.1b3/dcicutils/data_readers.py
--rw-r--r--   0        0        0     3098 2024-04-24 13:43:25.075500 dcicutils-8.8.4.1b3/dcicutils/data_utils.py
--rw-r--r--   0        0        0    13499 2024-04-24 13:43:25.075500 dcicutils-8.8.4.1b3/dcicutils/datetime_utils.py
--rw-r--r--   0        0        0    69908 2024-04-24 13:43:25.075500 dcicutils-8.8.4.1b3/dcicutils/deployment_utils.py
--rw-r--r--   0        0        0     8118 2024-04-24 13:43:25.075500 dcicutils-8.8.4.1b3/dcicutils/diff_utils.py
--rw-r--r--   0        0        0     1747 2024-04-24 13:43:25.075500 dcicutils-8.8.4.1b3/dcicutils/docker_utils.py
--rw-r--r--   0        0        0    19474 2024-04-24 13:43:25.075500 dcicutils-8.8.4.1b3/dcicutils/ecr_scripts.py
--rw-r--r--   0        0        0    13079 2024-04-24 13:43:25.075500 dcicutils-8.8.4.1b3/dcicutils/ecr_utils.py
--rw-r--r--   0        0        0     3590 2024-04-24 13:43:25.075500 dcicutils-8.8.4.1b3/dcicutils/ecs_utils.py
--rw-r--r--   0        0        0     6356 2024-04-24 13:43:25.075500 dcicutils-8.8.4.1b3/dcicutils/env_base.py
--rw-r--r--   0        0        0     9444 2024-04-24 13:43:25.075500 dcicutils-8.8.4.1b3/dcicutils/env_manager.py
--rw-r--r--   0        0        0     3909 2024-04-24 13:43:25.075500 dcicutils-8.8.4.1b3/dcicutils/env_scripts.py
--rw-r--r--   0        0        0    46970 2024-04-24 13:43:25.075500 dcicutils-8.8.4.1b3/dcicutils/env_utils.py
--rw-r--r--   0        0        0    29032 2024-04-24 13:43:25.075500 dcicutils-8.8.4.1b3/dcicutils/env_utils_legacy.py
--rw-r--r--   0        0        0     7541 2024-04-24 13:43:25.075500 dcicutils-8.8.4.1b3/dcicutils/es_utils.py
--rw-r--r--   0        0        0     9931 2024-04-24 13:43:25.075500 dcicutils-8.8.4.1b3/dcicutils/exceptions.py
--rw-r--r--   0        0        0    36918 2024-04-24 13:43:25.075500 dcicutils-8.8.4.1b3/dcicutils/ff_mocks.py
--rw-r--r--   0        0        0    73123 2024-04-24 13:43:25.079500 dcicutils-8.8.4.1b3/dcicutils/ff_utils.py
--rw-r--r--   0        0        0     3277 2024-04-24 13:43:25.079500 dcicutils-8.8.4.1b3/dcicutils/file_utils.py
--rw-r--r--   0        0        0    10026 2024-04-24 13:43:25.079500 dcicutils-8.8.4.1b3/dcicutils/function_cache_decorator.py
--rw-r--r--   0        0        0    34149 2024-04-24 13:43:25.079500 dcicutils-8.8.4.1b3/dcicutils/glacier_utils.py
--rw-r--r--   0        0        0      549 2024-04-24 13:43:25.079500 dcicutils-8.8.4.1b3/dcicutils/http_utils.py
--rw-r--r--   0        0        0    11502 2024-04-24 13:43:25.079500 dcicutils-8.8.4.1b3/dcicutils/jh_utils.py
--rw-r--r--   0        0        0    16225 2024-04-24 13:43:25.079500 dcicutils-8.8.4.1b3/dcicutils/kibana/dashboards.json
--rw-r--r--   0        0        0     2164 2024-04-24 13:43:25.079500 dcicutils-8.8.4.1b3/dcicutils/kibana/readme.md
--rw-r--r--   0        0        0    28151 2024-04-24 13:43:25.079500 dcicutils-8.8.4.1b3/dcicutils/lang_utils.py
--rw-r--r--   0        0        0      278 2024-04-24 13:43:25.079500 dcicutils-8.8.4.1b3/dcicutils/license_policies/c4-infrastructure.jsonc
--rw-r--r--   0        0        0      296 2024-04-24 13:43:25.079500 dcicutils-8.8.4.1b3/dcicutils/license_policies/c4-python-infrastructure.jsonc
--rw-r--r--   0        0        0     5790 2024-04-24 13:43:25.079500 dcicutils-8.8.4.1b3/dcicutils/license_policies/park-lab-common-server.jsonc
--rw-r--r--   0        0        0    18864 2024-04-24 13:43:25.079500 dcicutils-8.8.4.1b3/dcicutils/license_policies/park-lab-common.jsonc
--rw-r--r--   0        0        0     3260 2024-04-24 13:43:25.079500 dcicutils-8.8.4.1b3/dcicutils/license_policies/park-lab-gpl-pipeline.jsonc
--rw-r--r--   0        0        0      283 2024-04-24 13:43:25.079500 dcicutils-8.8.4.1b3/dcicutils/license_policies/park-lab-pipeline.jsonc
--rw-r--r--   0        0        0    46978 2024-04-24 13:43:25.079500 dcicutils-8.8.4.1b3/dcicutils/license_utils.py
--rw-r--r--   0        0        0    10883 2024-04-24 13:43:25.079500 dcicutils-8.8.4.1b3/dcicutils/log_utils.py
--rw-r--r--   0        0        0   105041 2024-04-24 13:43:25.079500 dcicutils-8.8.4.1b3/dcicutils/misc_utils.py
--rw-r--r--   0        0        0     5963 2024-04-24 13:43:25.079500 dcicutils-8.8.4.1b3/dcicutils/obfuscation_utils.py
--rw-r--r--   0        0        0     1017 2024-04-24 13:43:25.079500 dcicutils-8.8.4.1b3/dcicutils/opensearch_utils.py
--rw-r--r--   0        0        0    15422 2024-04-24 13:43:25.079500 dcicutils-8.8.4.1b3/dcicutils/portal_object_utils.py
--rw-r--r--   0        0        0    30779 2024-04-24 13:43:25.079500 dcicutils-8.8.4.1b3/dcicutils/portal_utils.py
--rw-r--r--   0        0        0    19468 2024-04-24 13:43:25.079500 dcicutils-8.8.4.1b3/dcicutils/progress_bar.py
--rw-r--r--   0        0        0    31250 2024-04-24 13:43:25.079500 dcicutils-8.8.4.1b3/dcicutils/project_utils.py
--rw-r--r--   0        0        0    20534 2024-04-24 13:43:25.079500 dcicutils-8.8.4.1b3/dcicutils/qa_checkers.py
--rw-r--r--   0        0        0   160208 2024-04-24 13:43:25.079500 dcicutils-8.8.4.1b3/dcicutils/qa_utils.py
--rw-r--r--   0        0        0     7055 2024-04-24 13:43:25.079500 dcicutils-8.8.4.1b3/dcicutils/redis_tools.py
--rw-r--r--   0        0        0     6462 2024-04-24 13:43:25.079500 dcicutils-8.8.4.1b3/dcicutils/redis_utils.py
--rw-r--r--   0        0        0    28868 2024-04-24 13:43:25.079500 dcicutils-8.8.4.1b3/dcicutils/s3_utils.py
--rw-r--r--   0        0        0    10095 2024-04-24 13:43:25.079500 dcicutils-8.8.4.1b3/dcicutils/schema_utils.py
--rw-r--r--   0        0        0    13889 2024-04-24 13:43:25.079500 dcicutils-8.8.4.1b3/dcicutils/scripts/publish_to_pypi.py
--rw-r--r--   0        0        0     4184 2024-04-24 13:43:25.079500 dcicutils-8.8.4.1b3/dcicutils/scripts/run_license_checker.py
--rw-r--r--   0        0        0    26262 2024-04-24 13:43:25.079500 dcicutils-8.8.4.1b3/dcicutils/scripts/view_portal_object.py
--rw-r--r--   0        0        0    19745 2024-04-24 13:43:25.079500 dcicutils-8.8.4.1b3/dcicutils/secrets_utils.py
--rw-r--r--   0        0        0    33629 2024-04-24 13:43:25.079500 dcicutils-8.8.4.1b3/dcicutils/sheet_utils.py
--rw-r--r--   0        0        0    22961 2024-04-24 13:43:25.079500 dcicutils-8.8.4.1b3/dcicutils/snapshot_utils.py
--rw-r--r--   0        0        0     9707 2024-04-24 13:43:25.079500 dcicutils-8.8.4.1b3/dcicutils/ssl_certificate_utils.py
--rw-r--r--   0        0        0    61238 2024-04-24 13:43:25.079500 dcicutils-8.8.4.1b3/dcicutils/structured_data.py
--rw-r--r--   0        0        0     2895 2024-04-24 13:43:25.079500 dcicutils-8.8.4.1b3/dcicutils/submitr/progress_constants.py
--rw-r--r--   0        0        0     3467 2024-04-24 13:43:25.079500 dcicutils-8.8.4.1b3/dcicutils/submitr/ref_lookup_strategy.py
--rw-r--r--   0        0        0     8082 2024-04-24 13:43:25.079500 dcicutils-8.8.4.1b3/dcicutils/task_utils.py
--rw-r--r--   0        0        0     1403 2024-04-24 13:43:25.079500 dcicutils-8.8.4.1b3/dcicutils/tmpfile_utils.py
--rw-r--r--   0        0        0     1769 2024-04-24 13:43:25.083500 dcicutils-8.8.4.1b3/dcicutils/trace_utils.py
--rw-r--r--   0        0        0    14797 2024-04-24 13:43:25.083500 dcicutils-8.8.4.1b3/dcicutils/validation_utils.py
--rw-r--r--   0        0        0     4343 2024-04-24 13:43:25.083500 dcicutils-8.8.4.1b3/dcicutils/variant_utils.py
--rw-r--r--   0        0        0     2994 2024-04-24 13:43:25.083500 dcicutils-8.8.4.1b3/dcicutils/zip_utils.py
--rw-r--r--   0        0        0     4733 2024-04-24 13:43:25.083500 dcicutils-8.8.4.1b3/pyproject.toml
--rw-r--r--   0        0        0     3396 1970-01-01 00:00:00.000000 dcicutils-8.8.4.1b3/PKG-INFO
+-rw-r--r--   0        0        0     1102 2024-04-24 14:44:50.581010 dcicutils-8.8.4.1b4/LICENSE.txt
+-rw-r--r--   0        0        0     1166 2024-04-24 14:44:50.581010 dcicutils-8.8.4.1b4/README.rst
+-rw-r--r--   0        0        0        0 2024-04-24 14:44:50.581010 dcicutils-8.8.4.1b4/dcicutils/__init__.py
+-rw-r--r--   0        0        0     5115 2024-04-24 14:44:50.581010 dcicutils-8.8.4.1b4/dcicutils/base.py
+-rwxr-xr-x   0        0        0    51434 2024-04-24 14:44:50.581010 dcicutils-8.8.4.1b4/dcicutils/beanstalk_utils.py
+-rw-r--r--   0        0        0    34669 2024-04-24 14:44:50.581010 dcicutils-8.8.4.1b4/dcicutils/bundle_utils.py
+-rw-r--r--   0        0        0     3295 2024-04-24 14:44:50.581010 dcicutils-8.8.4.1b4/dcicutils/captured_output.py
+-rw-r--r--   0        0        0    13786 2024-04-24 14:44:50.581010 dcicutils-8.8.4.1b4/dcicutils/cloudformation_utils.py
+-rw-r--r--   0        0        0     1155 2024-04-24 14:44:50.581010 dcicutils-8.8.4.1b4/dcicutils/codebuild_utils.py
+-rw-r--r--   0        0        0    15285 2024-04-24 14:44:50.581010 dcicutils-8.8.4.1b4/dcicutils/command_utils.py
+-rw-r--r--   0        0        0     3955 2024-04-24 14:44:50.581010 dcicutils-8.8.4.1b4/dcicutils/common.py
+-rw-r--r--   0        0        0     2015 2024-04-24 14:44:50.581010 dcicutils-8.8.4.1b4/dcicutils/contribution_scripts.py
+-rw-r--r--   0        0        0    25653 2024-04-24 14:44:50.581010 dcicutils-8.8.4.1b4/dcicutils/contribution_utils.py
+-rw-r--r--   0        0        0    11113 2024-04-24 14:44:50.581010 dcicutils-8.8.4.1b4/dcicutils/creds_utils.py
+-rw-r--r--   0        0        0     7626 2024-04-24 14:44:50.581010 dcicutils-8.8.4.1b4/dcicutils/data_readers.py
+-rw-r--r--   0        0        0     3098 2024-04-24 14:44:50.581010 dcicutils-8.8.4.1b4/dcicutils/data_utils.py
+-rw-r--r--   0        0        0    13499 2024-04-24 14:44:50.581010 dcicutils-8.8.4.1b4/dcicutils/datetime_utils.py
+-rw-r--r--   0        0        0    69908 2024-04-24 14:44:50.581010 dcicutils-8.8.4.1b4/dcicutils/deployment_utils.py
+-rw-r--r--   0        0        0     8118 2024-04-24 14:44:50.581010 dcicutils-8.8.4.1b4/dcicutils/diff_utils.py
+-rw-r--r--   0        0        0     1747 2024-04-24 14:44:50.581010 dcicutils-8.8.4.1b4/dcicutils/docker_utils.py
+-rw-r--r--   0        0        0    19474 2024-04-24 14:44:50.581010 dcicutils-8.8.4.1b4/dcicutils/ecr_scripts.py
+-rw-r--r--   0        0        0    13079 2024-04-24 14:44:50.581010 dcicutils-8.8.4.1b4/dcicutils/ecr_utils.py
+-rw-r--r--   0        0        0     3590 2024-04-24 14:44:50.581010 dcicutils-8.8.4.1b4/dcicutils/ecs_utils.py
+-rw-r--r--   0        0        0     6356 2024-04-24 14:44:50.581010 dcicutils-8.8.4.1b4/dcicutils/env_base.py
+-rw-r--r--   0        0        0     9444 2024-04-24 14:44:50.581010 dcicutils-8.8.4.1b4/dcicutils/env_manager.py
+-rw-r--r--   0        0        0     3909 2024-04-24 14:44:50.581010 dcicutils-8.8.4.1b4/dcicutils/env_scripts.py
+-rw-r--r--   0        0        0    46970 2024-04-24 14:44:50.581010 dcicutils-8.8.4.1b4/dcicutils/env_utils.py
+-rw-r--r--   0        0        0    29032 2024-04-24 14:44:50.581010 dcicutils-8.8.4.1b4/dcicutils/env_utils_legacy.py
+-rw-r--r--   0        0        0     7541 2024-04-24 14:44:50.581010 dcicutils-8.8.4.1b4/dcicutils/es_utils.py
+-rw-r--r--   0        0        0     9931 2024-04-24 14:44:50.581010 dcicutils-8.8.4.1b4/dcicutils/exceptions.py
+-rw-r--r--   0        0        0    36918 2024-04-24 14:44:50.581010 dcicutils-8.8.4.1b4/dcicutils/ff_mocks.py
+-rw-r--r--   0        0        0    73123 2024-04-24 14:44:50.581010 dcicutils-8.8.4.1b4/dcicutils/ff_utils.py
+-rw-r--r--   0        0        0     3653 2024-04-24 14:44:50.581010 dcicutils-8.8.4.1b4/dcicutils/file_utils.py
+-rw-r--r--   0        0        0    10026 2024-04-24 14:44:50.581010 dcicutils-8.8.4.1b4/dcicutils/function_cache_decorator.py
+-rw-r--r--   0        0        0    34149 2024-04-24 14:44:50.581010 dcicutils-8.8.4.1b4/dcicutils/glacier_utils.py
+-rw-r--r--   0        0        0      807 2024-04-24 14:44:50.581010 dcicutils-8.8.4.1b4/dcicutils/http_utils.py
+-rw-r--r--   0        0        0    11502 2024-04-24 14:44:50.581010 dcicutils-8.8.4.1b4/dcicutils/jh_utils.py
+-rw-r--r--   0        0        0    16225 2024-04-24 14:44:50.581010 dcicutils-8.8.4.1b4/dcicutils/kibana/dashboards.json
+-rw-r--r--   0        0        0     2164 2024-04-24 14:44:50.581010 dcicutils-8.8.4.1b4/dcicutils/kibana/readme.md
+-rw-r--r--   0        0        0    28151 2024-04-24 14:44:50.585010 dcicutils-8.8.4.1b4/dcicutils/lang_utils.py
+-rw-r--r--   0        0        0      278 2024-04-24 14:44:50.585010 dcicutils-8.8.4.1b4/dcicutils/license_policies/c4-infrastructure.jsonc
+-rw-r--r--   0        0        0      296 2024-04-24 14:44:50.585010 dcicutils-8.8.4.1b4/dcicutils/license_policies/c4-python-infrastructure.jsonc
+-rw-r--r--   0        0        0     5790 2024-04-24 14:44:50.585010 dcicutils-8.8.4.1b4/dcicutils/license_policies/park-lab-common-server.jsonc
+-rw-r--r--   0        0        0    18864 2024-04-24 14:44:50.585010 dcicutils-8.8.4.1b4/dcicutils/license_policies/park-lab-common.jsonc
+-rw-r--r--   0        0        0     3260 2024-04-24 14:44:50.585010 dcicutils-8.8.4.1b4/dcicutils/license_policies/park-lab-gpl-pipeline.jsonc
+-rw-r--r--   0        0        0      283 2024-04-24 14:44:50.585010 dcicutils-8.8.4.1b4/dcicutils/license_policies/park-lab-pipeline.jsonc
+-rw-r--r--   0        0        0    46978 2024-04-24 14:44:50.585010 dcicutils-8.8.4.1b4/dcicutils/license_utils.py
+-rw-r--r--   0        0        0    10883 2024-04-24 14:44:50.585010 dcicutils-8.8.4.1b4/dcicutils/log_utils.py
+-rw-r--r--   0        0        0   105516 2024-04-24 14:44:50.585010 dcicutils-8.8.4.1b4/dcicutils/misc_utils.py
+-rw-r--r--   0        0        0     5963 2024-04-24 14:44:50.585010 dcicutils-8.8.4.1b4/dcicutils/obfuscation_utils.py
+-rw-r--r--   0        0        0     1017 2024-04-24 14:44:50.585010 dcicutils-8.8.4.1b4/dcicutils/opensearch_utils.py
+-rw-r--r--   0        0        0    15422 2024-04-24 14:44:50.585010 dcicutils-8.8.4.1b4/dcicutils/portal_object_utils.py
+-rw-r--r--   0        0        0    30779 2024-04-24 14:44:50.585010 dcicutils-8.8.4.1b4/dcicutils/portal_utils.py
+-rw-r--r--   0        0        0    19468 2024-04-24 14:44:50.585010 dcicutils-8.8.4.1b4/dcicutils/progress_bar.py
+-rw-r--r--   0        0        0    31250 2024-04-24 14:44:50.585010 dcicutils-8.8.4.1b4/dcicutils/project_utils.py
+-rw-r--r--   0        0        0    20534 2024-04-24 14:44:50.585010 dcicutils-8.8.4.1b4/dcicutils/qa_checkers.py
+-rw-r--r--   0        0        0   160208 2024-04-24 14:44:50.585010 dcicutils-8.8.4.1b4/dcicutils/qa_utils.py
+-rw-r--r--   0        0        0     7055 2024-04-24 14:44:50.585010 dcicutils-8.8.4.1b4/dcicutils/redis_tools.py
+-rw-r--r--   0        0        0     6462 2024-04-24 14:44:50.585010 dcicutils-8.8.4.1b4/dcicutils/redis_utils.py
+-rw-r--r--   0        0        0    28868 2024-04-24 14:44:50.585010 dcicutils-8.8.4.1b4/dcicutils/s3_utils.py
+-rw-r--r--   0        0        0    10095 2024-04-24 14:44:50.585010 dcicutils-8.8.4.1b4/dcicutils/schema_utils.py
+-rw-r--r--   0        0        0    13889 2024-04-24 14:44:50.585010 dcicutils-8.8.4.1b4/dcicutils/scripts/publish_to_pypi.py
+-rw-r--r--   0        0        0     4184 2024-04-24 14:44:50.585010 dcicutils-8.8.4.1b4/dcicutils/scripts/run_license_checker.py
+-rw-r--r--   0        0        0    26262 2024-04-24 14:44:50.585010 dcicutils-8.8.4.1b4/dcicutils/scripts/view_portal_object.py
+-rw-r--r--   0        0        0    19745 2024-04-24 14:44:50.585010 dcicutils-8.8.4.1b4/dcicutils/secrets_utils.py
+-rw-r--r--   0        0        0    33629 2024-04-24 14:44:50.585010 dcicutils-8.8.4.1b4/dcicutils/sheet_utils.py
+-rw-r--r--   0        0        0    22961 2024-04-24 14:44:50.585010 dcicutils-8.8.4.1b4/dcicutils/snapshot_utils.py
+-rw-r--r--   0        0        0     9707 2024-04-24 14:44:50.585010 dcicutils-8.8.4.1b4/dcicutils/ssl_certificate_utils.py
+-rw-r--r--   0        0        0    61238 2024-04-24 14:44:50.585010 dcicutils-8.8.4.1b4/dcicutils/structured_data.py
+-rw-r--r--   0        0        0     2895 2024-04-24 14:44:50.585010 dcicutils-8.8.4.1b4/dcicutils/submitr/progress_constants.py
+-rw-r--r--   0        0        0     3467 2024-04-24 14:44:50.585010 dcicutils-8.8.4.1b4/dcicutils/submitr/ref_lookup_strategy.py
+-rw-r--r--   0        0        0     8082 2024-04-24 14:44:50.585010 dcicutils-8.8.4.1b4/dcicutils/task_utils.py
+-rw-r--r--   0        0        0     1403 2024-04-24 14:44:50.585010 dcicutils-8.8.4.1b4/dcicutils/tmpfile_utils.py
+-rw-r--r--   0        0        0     1769 2024-04-24 14:44:50.585010 dcicutils-8.8.4.1b4/dcicutils/trace_utils.py
+-rw-r--r--   0        0        0    14797 2024-04-24 14:44:50.585010 dcicutils-8.8.4.1b4/dcicutils/validation_utils.py
+-rw-r--r--   0        0        0     4343 2024-04-24 14:44:50.585010 dcicutils-8.8.4.1b4/dcicutils/variant_utils.py
+-rw-r--r--   0        0        0     3265 2024-04-24 14:44:50.585010 dcicutils-8.8.4.1b4/dcicutils/zip_utils.py
+-rw-r--r--   0        0        0     4733 2024-04-24 14:44:50.589010 dcicutils-8.8.4.1b4/pyproject.toml
+-rw-r--r--   0        0        0     3396 1970-01-01 00:00:00.000000 dcicutils-8.8.4.1b4/PKG-INFO
```

### Comparing `dcicutils-8.8.4.1b3/LICENSE.txt` & `dcicutils-8.8.4.1b4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b3/README.rst` & `dcicutils-8.8.4.1b4/README.rst`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b3/dcicutils/base.py` & `dcicutils-8.8.4.1b4/dcicutils/base.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b3/dcicutils/beanstalk_utils.py` & `dcicutils-8.8.4.1b4/dcicutils/beanstalk_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b3/dcicutils/bundle_utils.py` & `dcicutils-8.8.4.1b4/dcicutils/bundle_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b3/dcicutils/captured_output.py` & `dcicutils-8.8.4.1b4/dcicutils/captured_output.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b3/dcicutils/cloudformation_utils.py` & `dcicutils-8.8.4.1b4/dcicutils/cloudformation_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b3/dcicutils/codebuild_utils.py` & `dcicutils-8.8.4.1b4/dcicutils/codebuild_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b3/dcicutils/command_utils.py` & `dcicutils-8.8.4.1b4/dcicutils/command_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b3/dcicutils/common.py` & `dcicutils-8.8.4.1b4/dcicutils/common.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b3/dcicutils/contribution_scripts.py` & `dcicutils-8.8.4.1b4/dcicutils/contribution_scripts.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b3/dcicutils/contribution_utils.py` & `dcicutils-8.8.4.1b4/dcicutils/contribution_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b3/dcicutils/creds_utils.py` & `dcicutils-8.8.4.1b4/dcicutils/creds_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b3/dcicutils/data_readers.py` & `dcicutils-8.8.4.1b4/dcicutils/data_readers.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b3/dcicutils/data_utils.py` & `dcicutils-8.8.4.1b4/dcicutils/data_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b3/dcicutils/datetime_utils.py` & `dcicutils-8.8.4.1b4/dcicutils/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b3/dcicutils/deployment_utils.py` & `dcicutils-8.8.4.1b4/dcicutils/deployment_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b3/dcicutils/diff_utils.py` & `dcicutils-8.8.4.1b4/dcicutils/diff_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b3/dcicutils/docker_utils.py` & `dcicutils-8.8.4.1b4/dcicutils/docker_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b3/dcicutils/ecr_scripts.py` & `dcicutils-8.8.4.1b4/dcicutils/ecr_scripts.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b3/dcicutils/ecr_utils.py` & `dcicutils-8.8.4.1b4/dcicutils/ecr_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b3/dcicutils/ecs_utils.py` & `dcicutils-8.8.4.1b4/dcicutils/ecs_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b3/dcicutils/env_base.py` & `dcicutils-8.8.4.1b4/dcicutils/env_base.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b3/dcicutils/env_manager.py` & `dcicutils-8.8.4.1b4/dcicutils/env_manager.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b3/dcicutils/env_scripts.py` & `dcicutils-8.8.4.1b4/dcicutils/env_scripts.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b3/dcicutils/env_utils.py` & `dcicutils-8.8.4.1b4/dcicutils/env_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b3/dcicutils/env_utils_legacy.py` & `dcicutils-8.8.4.1b4/dcicutils/env_utils_legacy.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b3/dcicutils/es_utils.py` & `dcicutils-8.8.4.1b4/dcicutils/es_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b3/dcicutils/exceptions.py` & `dcicutils-8.8.4.1b4/dcicutils/exceptions.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b3/dcicutils/ff_mocks.py` & `dcicutils-8.8.4.1b4/dcicutils/ff_mocks.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b3/dcicutils/ff_utils.py` & `dcicutils-8.8.4.1b4/dcicutils/ff_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b3/dcicutils/file_utils.py` & `dcicutils-8.8.4.1b4/dcicutils/file_utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -54,19 +54,25 @@
                         if file_found not in files_found:
                             files_found.append(file_found)
         if files_found:
             return files_found[0] if single else files_found
         return None if single else []
 
 
-def normalize_file_path(path: str, including_home_directory: bool = False) -> str:
+def normalize_file_path(path: str, home_directory: bool = True) -> str:
+    """
+    Normalizes the given file path name and returns. Does things like remove multiple
+    consecutive slashes and redundant/unnecessary parent paths; if the home_directory
+    argument is True (the default) then also handles the special tilde home directory
+    component/convention and uses this in the result if applicable.
+    """
     if not isinstance(path, str) or not path:
         path = os.getcwd()
     path = os.path.normpath(path)
-    home_directory = os.path.expanduser("~")
-    if path.startswith("~"):
+    home_directory = os.path.expanduser("~") if home_directory is True else None
+    if home_directory and path.startswith("~"):
         path = os.path.join(home_directory, path[2 if path.startswith("~/") else 1:])
     path = os.path.abspath(path)
-    if including_home_directory and (os.name == "posix"):
+    if home_directory and (os.name == "posix"):
         if path.startswith(home_directory) and path != home_directory:
             path = "~/" + pathlib.Path(path).relative_to(home_directory).as_posix()
     return path
```

### Comparing `dcicutils-8.8.4.1b3/dcicutils/function_cache_decorator.py` & `dcicutils-8.8.4.1b4/dcicutils/function_cache_decorator.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b3/dcicutils/glacier_utils.py` & `dcicutils-8.8.4.1b4/dcicutils/glacier_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b3/dcicutils/jh_utils.py` & `dcicutils-8.8.4.1b4/dcicutils/jh_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b3/dcicutils/kibana/dashboards.json` & `dcicutils-8.8.4.1b4/dcicutils/kibana/dashboards.json`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b3/dcicutils/kibana/readme.md` & `dcicutils-8.8.4.1b4/dcicutils/kibana/readme.md`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b3/dcicutils/lang_utils.py` & `dcicutils-8.8.4.1b4/dcicutils/lang_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b3/dcicutils/license_policies/park-lab-common-server.jsonc` & `dcicutils-8.8.4.1b4/dcicutils/license_policies/park-lab-common-server.jsonc`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b3/dcicutils/license_policies/park-lab-common.jsonc` & `dcicutils-8.8.4.1b4/dcicutils/license_policies/park-lab-common.jsonc`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b3/dcicutils/license_policies/park-lab-gpl-pipeline.jsonc` & `dcicutils-8.8.4.1b4/dcicutils/license_policies/park-lab-gpl-pipeline.jsonc`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b3/dcicutils/license_utils.py` & `dcicutils-8.8.4.1b4/dcicutils/license_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b3/dcicutils/log_utils.py` & `dcicutils-8.8.4.1b4/dcicutils/log_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b3/dcicutils/misc_utils.py` & `dcicutils-8.8.4.1b4/dcicutils/misc_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 import hashlib
 import inspect
 import io
 import json
 import logging
 import math
 import os
+import platform
 import pytz
 import re
 import rfc3986.validators
 import rfc3986.exceptions
 import time
 import uuid
 import warnings
@@ -2678,7 +2679,22 @@
     Returns the standard system application specific directory:
     - On MacOS this directory: is: ~/Library/Application Support
     - On Linux this directory is: ~/.local/share
     - On Windows this directory is: %USERPROFILE%\AppData\Local  # noqa
     N.B. This is has been tested on MacOS and Linux but not on Windows.
     """
     return appdirs.user_data_dir()
+
+
+def get_os_name() -> str:
+    if os_name := platform.system():
+        if os_name == "Darwin": return "osx"  # noqa
+        elif os_name == "Linux": return "linux"  # noqa
+        elif os_name == "Windows": return "windows"  # noqa
+    return ""
+
+
+def get_cpu_architecture_name() -> str:
+    if os_architecture_name := platform.machine():
+        if os_architecture_name == "x86_64": return "amd64"  # noqa
+        return os_architecture_name
+    return ""
```

### Comparing `dcicutils-8.8.4.1b3/dcicutils/obfuscation_utils.py` & `dcicutils-8.8.4.1b4/dcicutils/obfuscation_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b3/dcicutils/opensearch_utils.py` & `dcicutils-8.8.4.1b4/dcicutils/opensearch_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b3/dcicutils/portal_object_utils.py` & `dcicutils-8.8.4.1b4/dcicutils/portal_object_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b3/dcicutils/portal_utils.py` & `dcicutils-8.8.4.1b4/dcicutils/portal_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b3/dcicutils/progress_bar.py` & `dcicutils-8.8.4.1b4/dcicutils/progress_bar.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b3/dcicutils/project_utils.py` & `dcicutils-8.8.4.1b4/dcicutils/project_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b3/dcicutils/qa_checkers.py` & `dcicutils-8.8.4.1b4/dcicutils/qa_checkers.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b3/dcicutils/qa_utils.py` & `dcicutils-8.8.4.1b4/dcicutils/qa_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b3/dcicutils/redis_tools.py` & `dcicutils-8.8.4.1b4/dcicutils/redis_tools.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b3/dcicutils/redis_utils.py` & `dcicutils-8.8.4.1b4/dcicutils/redis_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b3/dcicutils/s3_utils.py` & `dcicutils-8.8.4.1b4/dcicutils/s3_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b3/dcicutils/schema_utils.py` & `dcicutils-8.8.4.1b4/dcicutils/schema_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b3/dcicutils/scripts/publish_to_pypi.py` & `dcicutils-8.8.4.1b4/dcicutils/scripts/publish_to_pypi.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b3/dcicutils/scripts/run_license_checker.py` & `dcicutils-8.8.4.1b4/dcicutils/scripts/run_license_checker.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b3/dcicutils/scripts/view_portal_object.py` & `dcicutils-8.8.4.1b4/dcicutils/scripts/view_portal_object.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b3/dcicutils/secrets_utils.py` & `dcicutils-8.8.4.1b4/dcicutils/secrets_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b3/dcicutils/sheet_utils.py` & `dcicutils-8.8.4.1b4/dcicutils/sheet_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b3/dcicutils/snapshot_utils.py` & `dcicutils-8.8.4.1b4/dcicutils/snapshot_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b3/dcicutils/ssl_certificate_utils.py` & `dcicutils-8.8.4.1b4/dcicutils/ssl_certificate_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b3/dcicutils/structured_data.py` & `dcicutils-8.8.4.1b4/dcicutils/structured_data.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b3/dcicutils/submitr/progress_constants.py` & `dcicutils-8.8.4.1b4/dcicutils/submitr/progress_constants.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b3/dcicutils/submitr/ref_lookup_strategy.py` & `dcicutils-8.8.4.1b4/dcicutils/submitr/ref_lookup_strategy.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b3/dcicutils/task_utils.py` & `dcicutils-8.8.4.1b4/dcicutils/task_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b3/dcicutils/tmpfile_utils.py` & `dcicutils-8.8.4.1b4/dcicutils/tmpfile_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b3/dcicutils/trace_utils.py` & `dcicutils-8.8.4.1b4/dcicutils/trace_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b3/dcicutils/validation_utils.py` & `dcicutils-8.8.4.1b4/dcicutils/validation_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b3/dcicutils/variant_utils.py` & `dcicutils-8.8.4.1b4/dcicutils/variant_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b3/dcicutils/zip_utils.py` & `dcicutils-8.8.4.1b4/dcicutils/zip_utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -47,14 +47,19 @@
                     outputf.write(inputf.read())
                     outputf.close()
                     yield tmp_file_name
 
 
 def extract_file_from_zip(zip_file: str, file_to_extract: str,
                           destination_file: str, raise_exception: bool = True) -> bool:
+    """
+    Extracts from the given zip file, the given file to extract, writing it to the
+    given destination file. Returns True if all is well, otherwise False, or if the
+    raise_exception argument is True (the default), then raises and exception on error.
+    """
     try:
         if not (destination_directory := os.path.dirname(destination_file)):
             destination_directory = os.getcwd()
             destination_file = os.path.join(destination_directory, destination_file)
         with tempfile.TemporaryDirectory() as tmp_directory_name:
             with zipfile.ZipFile(zip_file, "r") as zipf:
                 if file_to_extract not in zipf.namelist():
```

### Comparing `dcicutils-8.8.4.1b3/pyproject.toml` & `dcicutils-8.8.4.1b4/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dcicutils"
-version = "8.8.4.1b3"  # TODO: To become 8.8.5
+version = "8.8.4.1b4"  # TODO: To become 8.8.5
 description = "Utility package for interacting with the 4DN Data Portal and other 4DN resources"
 authors = ["4DN-DCIC Team <support@4dnucleome.org>"]
 license = "MIT"
 readme = "README.rst"
 homepage = "https://github.com/4dn-dcic/utils"
 repository = "https://github.com/4dn-dcic/utils"
 packages = [
@@ -33,17 +33,17 @@
     'Programming Language :: Python :: 3.9',
     'Programming Language :: Python :: 3.10',
     'Programming Language :: Python :: 3.11'
 ]
 
 
 [tool.poetry.dependencies]
-python = ">=3.8,<3.12"
-boto3 = "^1.28.57"
-botocore = "^1.31.57"
+python = ">=3.8,<3.13"
+boto3 = "^1.34.90"
+botocore = "^1.34.90"
 # The DCIC portals (cgap-portal and fourfront) are very particular about which ElasticSearch version.
 # This value is intentionally pinned and must not be changed casually.
 elasticsearch = "7.13.4"
 appdirs = "^1.4.4"
 aws-requests-auth = ">=0.4.2,<1"
 chardet = "^5.2.0"
 docker = "^4.4.4"
@@ -66,16 +66,16 @@
 tqdm = "^4.66.2"
 typing-extensions = ">=3.8"  # Fourfront uses 3.8
 urllib3 = "^1.26.6"
 webtest = "^2.0.34"
 
 
 [tool.poetry.dev-dependencies]
-boto3-stubs = "^1.28.57"
-botocore-stubs = "^1.31.57"
+boto3-stubs = "^1.34.90"
+botocore-stubs = "^1.34.90"
 coverage = ">=7.2.3"
 # Loaded manually in GA workflow for coverage because a dependency on 2to3
 # in its docopts dependency makes a problem for laoding it here in poetry. -kmp 7-Apr-2023
 # coveralls = ">=3.3.1"
 flake8 = ">=3.9.2"
 flaky = ">=3.7.0"
 pip-licenses = "^4.3.3"
```

### Comparing `dcicutils-8.8.4.1b3/PKG-INFO` & `dcicutils-8.8.4.1b4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: dcicutils
-Version: 8.8.4.1b3
+Version: 8.8.4.1b4
 Summary: Utility package for interacting with the 4DN Data Portal and other 4DN resources
 Home-page: https://github.com/4dn-dcic/utils
 License: MIT
 Author: 4DN-DCIC Team
 Author-email: support@4dnucleome.org
-Requires-Python: >=3.8,<3.12
+Requires-Python: >=3.8,<3.13
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -22,16 +22,16 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Database :: Database Engines/Servers
 Requires-Dist: PyJWT (>=2.6.0,<3.0.0)
 Requires-Dist: PyYAML (>=6.0.1,<7.0.0)
 Requires-Dist: appdirs (>=1.4.4,<2.0.0)
 Requires-Dist: aws-requests-auth (>=0.4.2,<1)
-Requires-Dist: boto3 (>=1.28.57,<2.0.0)
-Requires-Dist: botocore (>=1.31.57,<2.0.0)
+Requires-Dist: boto3 (>=1.34.90,<2.0.0)
+Requires-Dist: botocore (>=1.34.90,<2.0.0)
 Requires-Dist: chardet (>=5.2.0,<6.0.0)
 Requires-Dist: docker (>=4.4.4,<5.0.0)
 Requires-Dist: elasticsearch (==7.13.4)
 Requires-Dist: gitpython (>=3.1.2,<4.0.0)
 Requires-Dist: jsonc-parser (>=1.1.5,<2.0.0)
 Requires-Dist: jsonschema (>=4.19.0,<5.0.0)
 Requires-Dist: openpyxl (>=3.1.2,<4.0.0)
```


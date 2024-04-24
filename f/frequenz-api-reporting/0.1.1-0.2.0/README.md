# Comparing `tmp/frequenz-api-reporting-0.1.1.tar.gz` & `tmp/frequenz-api-reporting-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frequenz-api-reporting-0.1.1.tar", last modified: Thu Dec 14 12:31:40 2023, max compression
+gzip compressed data, was "frequenz-api-reporting-0.2.0.tar", last modified: Wed Apr 24 12:47:26 2024, max compression
```

## Comparing `frequenz-api-reporting-0.1.1.tar` & `frequenz-api-reporting-0.2.0.tar`

### file list

```diff
@@ -1,128 +1,139 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 12:31:40.637527 frequenz-api-reporting-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2023-12-14 12:31:22.000000 frequenz-api-reporting-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      376 2023-12-14 12:31:22.000000 frequenz-api-reporting-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4801 2023-12-14 12:31:40.637527 frequenz-api-reporting-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3428 2023-12-14 12:31:22.000000 frequenz-api-reporting-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      437 2023-12-14 12:31:22.000000 frequenz-api-reporting-0.1.1/RELEASE_NOTES.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 12:31:40.621527 frequenz-api-reporting-0.1.1/proto/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 12:31:40.621527 frequenz-api-reporting-0.1.1/proto/frequenz/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 12:31:40.621527 frequenz-api-reporting-0.1.1/proto/frequenz/api/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 12:31:40.621527 frequenz-api-reporting-0.1.1/proto/frequenz/api/reporting/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 12:31:40.625527 frequenz-api-reporting-0.1.1/proto/frequenz/api/reporting/v1/
--rw-r--r--   0 runner    (1001) docker     (127)    22127 2023-12-14 12:31:22.000000 frequenz-api-reporting-0.1.1/proto/frequenz/api/reporting/v1/reporting.proto
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 12:31:40.621527 frequenz-api-reporting-0.1.1/py/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 12:31:40.621527 frequenz-api-reporting-0.1.1/py/frequenz/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 12:31:40.621527 frequenz-api-reporting-0.1.1/py/frequenz/api/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 12:31:40.625527 frequenz-api-reporting-0.1.1/py/frequenz/api/reporting/
--rw-r--r--   0 runner    (1001) docker     (127)      140 2023-12-14 12:31:22.000000 frequenz-api-reporting-0.1.1/py/frequenz/api/reporting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      409 2023-12-14 12:31:22.000000 frequenz-api-reporting-0.1.1/py/frequenz/api/reporting/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-14 12:31:22.000000 frequenz-api-reporting-0.1.1/py/frequenz/api/reporting/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 12:31:40.625527 frequenz-api-reporting-0.1.1/py/frequenz/api/reporting/v1/
--rw-r--r--   0 runner    (1001) docker     (127)      140 2023-12-14 12:31:22.000000 frequenz-api-reporting-0.1.1/py/frequenz/api/reporting/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 12:31:40.629527 frequenz-api-reporting-0.1.1/py/frequenz_api_reporting.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4801 2023-12-14 12:31:40.000000 frequenz-api-reporting-0.1.1/py/frequenz_api_reporting.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5098 2023-12-14 12:31:40.000000 frequenz-api-reporting-0.1.1/py/frequenz_api_reporting.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-14 12:31:40.000000 frequenz-api-reporting-0.1.1/py/frequenz_api_reporting.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      935 2023-12-14 12:31:40.000000 frequenz-api-reporting-0.1.1/py/frequenz_api_reporting.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2023-12-14 12:31:40.000000 frequenz-api-reporting-0.1.1/py/frequenz_api_reporting.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4863 2023-12-14 12:31:22.000000 frequenz-api-reporting-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-14 12:31:40.637527 frequenz-api-reporting-0.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 12:31:40.625527 frequenz-api-reporting-0.1.1/submodules/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 12:31:40.621527 frequenz-api-reporting-0.1.1/submodules/api-common-protos/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 12:31:40.625527 frequenz-api-reporting-0.1.1/submodules/api-common-protos/google/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 12:31:40.633527 frequenz-api-reporting-0.1.1/submodules/api-common-protos/google/api/
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2023-12-14 12:31:23.000000 frequenz-api-reporting-0.1.1/submodules/api-common-protos/google/api/annotations.proto
--rw-r--r--   0 runner    (1001) docker     (127)     7374 2023-12-14 12:31:23.000000 frequenz-api-reporting-0.1.1/submodules/api-common-protos/google/api/auth.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1808 2023-12-14 12:31:23.000000 frequenz-api-reporting-0.1.1/submodules/api-common-protos/google/api/backend.proto
--rw-r--r--   0 runner    (1001) docker     (127)     2504 2023-12-14 12:31:23.000000 frequenz-api-reporting-0.1.1/submodules/api-common-protos/google/api/billing.proto
--rw-r--r--   0 runner    (1001) docker     (127)     3392 2023-12-14 12:31:23.000000 frequenz-api-reporting-0.1.1/submodules/api-common-protos/google/api/client.proto
--rw-r--r--   0 runner    (1001) docker     (127)     3169 2023-12-14 12:31:23.000000 frequenz-api-reporting-0.1.1/submodules/api-common-protos/google/api/config_change.proto
--rw-r--r--   0 runner    (1001) docker     (127)     2719 2023-12-14 12:31:23.000000 frequenz-api-reporting-0.1.1/submodules/api-common-protos/google/api/consumer.proto
--rw-r--r--   0 runner    (1001) docker     (127)     2008 2023-12-14 12:31:23.000000 frequenz-api-reporting-0.1.1/submodules/api-common-protos/google/api/context.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1225 2023-12-14 12:31:23.000000 frequenz-api-reporting-0.1.1/submodules/api-common-protos/google/api/control.proto
--rw-r--r--   0 runner    (1001) docker     (127)     8657 2023-12-14 12:31:23.000000 frequenz-api-reporting-0.1.1/submodules/api-common-protos/google/api/distribution.proto
--rw-r--r--   0 runner    (1001) docker     (127)     6132 2023-12-14 12:31:23.000000 frequenz-api-reporting-0.1.1/submodules/api-common-protos/google/api/documentation.proto
--rw-r--r--   0 runner    (1001) docker     (127)     2824 2023-12-14 12:31:23.000000 frequenz-api-reporting-0.1.1/submodules/api-common-protos/google/api/endpoint.proto
--rw-r--r--   0 runner    (1001) docker     (127)     3318 2023-12-14 12:31:23.000000 frequenz-api-reporting-0.1.1/submodules/api-common-protos/google/api/field_behavior.proto
--rw-r--r--   0 runner    (1001) docker     (127)    12099 2023-12-14 12:31:23.000000 frequenz-api-reporting-0.1.1/submodules/api-common-protos/google/api/http.proto
--rw-r--r--   0 runner    (1001) docker     (127)     2605 2023-12-14 12:31:23.000000 frequenz-api-reporting-0.1.1/submodules/api-common-protos/google/api/httpbody.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1391 2023-12-14 12:31:23.000000 frequenz-api-reporting-0.1.1/submodules/api-common-protos/google/api/label.proto
--rw-r--r--   0 runner    (1001) docker     (127)     2910 2023-12-14 12:31:23.000000 frequenz-api-reporting-0.1.1/submodules/api-common-protos/google/api/launch_stage.proto
--rw-r--r--   0 runner    (1001) docker     (127)     2045 2023-12-14 12:31:23.000000 frequenz-api-reporting-0.1.1/submodules/api-common-protos/google/api/log.proto
--rw-r--r--   0 runner    (1001) docker     (127)     3209 2023-12-14 12:31:23.000000 frequenz-api-reporting-0.1.1/submodules/api-common-protos/google/api/logging.proto
--rw-r--r--   0 runner    (1001) docker     (127)     6628 2023-12-14 12:31:23.000000 frequenz-api-reporting-0.1.1/submodules/api-common-protos/google/api/metric.proto
--rw-r--r--   0 runner    (1001) docker     (127)     5512 2023-12-14 12:31:23.000000 frequenz-api-reporting-0.1.1/submodules/api-common-protos/google/api/monitored_resource.proto
--rw-r--r--   0 runner    (1001) docker     (127)     3524 2023-12-14 12:31:23.000000 frequenz-api-reporting-0.1.1/submodules/api-common-protos/google/api/monitoring.proto
--rw-r--r--   0 runner    (1001) docker     (127)    10854 2023-12-14 12:31:23.000000 frequenz-api-reporting-0.1.1/submodules/api-common-protos/google/api/quota.proto
--rw-r--r--   0 runner    (1001) docker     (127)    11347 2023-12-14 12:31:23.000000 frequenz-api-reporting-0.1.1/submodules/api-common-protos/google/api/resource.proto
--rw-r--r--   0 runner    (1001) docker     (127)    14929 2023-12-14 12:31:23.000000 frequenz-api-reporting-0.1.1/submodules/api-common-protos/google/api/routing.proto
--rw-r--r--   0 runner    (1001) docker     (127)     6099 2023-12-14 12:31:23.000000 frequenz-api-reporting-0.1.1/submodules/api-common-protos/google/api/service.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2023-12-14 12:31:23.000000 frequenz-api-reporting-0.1.1/submodules/api-common-protos/google/api/source_info.proto
--rw-r--r--   0 runner    (1001) docker     (127)     3472 2023-12-14 12:31:23.000000 frequenz-api-reporting-0.1.1/submodules/api-common-protos/google/api/system_parameter.proto
--rw-r--r--   0 runner    (1001) docker     (127)     3513 2023-12-14 12:31:23.000000 frequenz-api-reporting-0.1.1/submodules/api-common-protos/google/api/usage.proto
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 12:31:40.633527 frequenz-api-reporting-0.1.1/submodules/api-common-protos/google/cloud/
--rw-r--r--   0 runner    (1001) docker     (127)     6308 2023-12-14 12:31:23.000000 frequenz-api-reporting-0.1.1/submodules/api-common-protos/google/cloud/extended_operations.proto
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 12:31:40.625527 frequenz-api-reporting-0.1.1/submodules/api-common-protos/google/iam/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 12:31:40.625527 frequenz-api-reporting-0.1.1/submodules/api-common-protos/google/iam/admin/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 12:31:40.633527 frequenz-api-reporting-0.1.1/submodules/api-common-protos/google/iam/admin/v1/
--rw-r--r--   0 runner    (1001) docker     (127)    41483 2023-12-14 12:31:23.000000 frequenz-api-reporting-0.1.1/submodules/api-common-protos/google/iam/admin/v1/iam.proto
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 12:31:40.633527 frequenz-api-reporting-0.1.1/submodules/api-common-protos/google/iam/v1/
--rw-r--r--   0 runner    (1001) docker     (127)     5482 2023-12-14 12:31:23.000000 frequenz-api-reporting-0.1.1/submodules/api-common-protos/google/iam/v1/iam_policy.proto
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 12:31:40.633527 frequenz-api-reporting-0.1.1/submodules/api-common-protos/google/iam/v1/logging/
--rw-r--r--   0 runner    (1001) docker     (127)     1287 2023-12-14 12:31:23.000000 frequenz-api-reporting-0.1.1/submodules/api-common-protos/google/iam/v1/logging/audit_data.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1470 2023-12-14 12:31:23.000000 frequenz-api-reporting-0.1.1/submodules/api-common-protos/google/iam/v1/options.proto
--rw-r--r--   0 runner    (1001) docker     (127)     8659 2023-12-14 12:31:23.000000 frequenz-api-reporting-0.1.1/submodules/api-common-protos/google/iam/v1/policy.proto
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 12:31:40.625527 frequenz-api-reporting-0.1.1/submodules/api-common-protos/google/logging/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 12:31:40.633527 frequenz-api-reporting-0.1.1/submodules/api-common-protos/google/logging/type/
--rw-r--r--   0 runner    (1001) docker     (127)     3389 2023-12-14 12:31:23.000000 frequenz-api-reporting-0.1.1/submodules/api-common-protos/google/logging/type/http_request.proto
--rw-r--r--   0 runner    (1001) docker     (127)     2508 2023-12-14 12:31:23.000000 frequenz-api-reporting-0.1.1/submodules/api-common-protos/google/logging/type/log_severity.proto
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 12:31:40.633527 frequenz-api-reporting-0.1.1/submodules/api-common-protos/google/longrunning/
--rw-r--r--   0 runner    (1001) docker     (127)    10515 2023-12-14 12:31:23.000000 frequenz-api-reporting-0.1.1/submodules/api-common-protos/google/longrunning/operations.proto
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 12:31:40.633527 frequenz-api-reporting-0.1.1/submodules/api-common-protos/google/rpc/
--rw-r--r--   0 runner    (1001) docker     (127)     7125 2023-12-14 12:31:23.000000 frequenz-api-reporting-0.1.1/submodules/api-common-protos/google/rpc/code.proto
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 12:31:40.633527 frequenz-api-reporting-0.1.1/submodules/api-common-protos/google/rpc/context/
--rw-r--r--   0 runner    (1001) docker     (127)    12015 2023-12-14 12:31:23.000000 frequenz-api-reporting-0.1.1/submodules/api-common-protos/google/rpc/context/attribute_context.proto
--rw-r--r--   0 runner    (1001) docker     (127)     9504 2023-12-14 12:31:23.000000 frequenz-api-reporting-0.1.1/submodules/api-common-protos/google/rpc/error_details.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1924 2023-12-14 12:31:23.000000 frequenz-api-reporting-0.1.1/submodules/api-common-protos/google/rpc/status.proto
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 12:31:40.633527 frequenz-api-reporting-0.1.1/submodules/api-common-protos/google/type/
--rw-r--r--   0 runner    (1001) docker     (127)     1766 2023-12-14 12:31:23.000000 frequenz-api-reporting-0.1.1/submodules/api-common-protos/google/type/calendar_period.proto
--rw-r--r--   0 runner    (1001) docker     (127)     6193 2023-12-14 12:31:23.000000 frequenz-api-reporting-0.1.1/submodules/api-common-protos/google/type/color.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1933 2023-12-14 12:31:23.000000 frequenz-api-reporting-0.1.1/submodules/api-common-protos/google/type/date.proto
--rw-r--r--   0 runner    (1001) docker     (127)     3508 2023-12-14 12:31:23.000000 frequenz-api-reporting-0.1.1/submodules/api-common-protos/google/type/datetime.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1337 2023-12-14 12:31:23.000000 frequenz-api-reporting-0.1.1/submodules/api-common-protos/google/type/dayofweek.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1834 2023-12-14 12:31:23.000000 frequenz-api-reporting-0.1.1/submodules/api-common-protos/google/type/expr.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1176 2023-12-14 12:31:23.000000 frequenz-api-reporting-0.1.1/submodules/api-common-protos/google/type/fraction.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1447 2023-12-14 12:31:23.000000 frequenz-api-reporting-0.1.1/submodules/api-common-protos/google/type/latlng.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1603 2023-12-14 12:31:23.000000 frequenz-api-reporting-0.1.1/submodules/api-common-protos/google/type/money.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1482 2023-12-14 12:31:23.000000 frequenz-api-reporting-0.1.1/submodules/api-common-protos/google/type/month.proto
--rw-r--r--   0 runner    (1001) docker     (127)     6239 2023-12-14 12:31:23.000000 frequenz-api-reporting-0.1.1/submodules/api-common-protos/google/type/postal_address.proto
--rw-r--r--   0 runner    (1001) docker     (127)     3795 2023-12-14 12:31:23.000000 frequenz-api-reporting-0.1.1/submodules/api-common-protos/google/type/quaternion.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1668 2023-12-14 12:31:23.000000 frequenz-api-reporting-0.1.1/submodules/api-common-protos/google/type/timeofday.proto
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 12:31:40.625527 frequenz-api-reporting-0.1.1/submodules/frequenz-api-common/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 12:31:40.625527 frequenz-api-reporting-0.1.1/submodules/frequenz-api-common/proto/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 12:31:40.625527 frequenz-api-reporting-0.1.1/submodules/frequenz-api-common/proto/frequenz/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 12:31:40.625527 frequenz-api-reporting-0.1.1/submodules/frequenz-api-common/proto/frequenz/api/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 12:31:40.625527 frequenz-api-reporting-0.1.1/submodules/frequenz-api-common/proto/frequenz/api/common/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 12:31:40.633527 frequenz-api-reporting-0.1.1/submodules/frequenz-api-common/proto/frequenz/api/common/v1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 12:31:40.633527 frequenz-api-reporting-0.1.1/submodules/frequenz-api-common/proto/frequenz/api/common/v1/grid/
--rw-r--r--   0 runner    (1001) docker     (127)     2537 2023-12-14 12:31:24.000000 frequenz-api-reporting-0.1.1/submodules/frequenz-api-common/proto/frequenz/api/common/v1/grid/delivery_area.proto
--rw-r--r--   0 runner    (1001) docker     (127)      582 2023-12-14 12:31:24.000000 frequenz-api-reporting-0.1.1/submodules/frequenz-api-common/proto/frequenz/api/common/v1/location.proto
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 12:31:40.637527 frequenz-api-reporting-0.1.1/submodules/frequenz-api-common/proto/frequenz/api/common/v1/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)      503 2023-12-14 12:31:24.000000 frequenz-api-reporting-0.1.1/submodules/frequenz-api-common/proto/frequenz/api/common/v1/metrics/bounds.proto
--rw-r--r--   0 runner    (1001) docker     (127)     6989 2023-12-14 12:31:24.000000 frequenz-api-reporting-0.1.1/submodules/frequenz-api-common/proto/frequenz/api/common/v1/metrics/metric_sample.proto
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 12:31:40.637527 frequenz-api-reporting-0.1.1/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 12:31:40.637527 frequenz-api-reporting-0.1.1/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/
--rw-r--r--   0 runner    (1001) docker     (127)      512 2023-12-14 12:31:24.000000 frequenz-api-reporting-0.1.1/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/battery.proto
--rw-r--r--   0 runner    (1001) docker     (127)    16612 2023-12-14 12:31:24.000000 frequenz-api-reporting-0.1.1/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/components.proto
--rw-r--r--   0 runner    (1001) docker     (127)      688 2023-12-14 12:31:24.000000 frequenz-api-reporting-0.1.1/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/ev_charger.proto
--rw-r--r--   0 runner    (1001) docker     (127)      805 2023-12-14 12:31:24.000000 frequenz-api-reporting-0.1.1/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/fuse.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1939 2023-12-14 12:31:24.000000 frequenz-api-reporting-0.1.1/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/grid.proto
--rw-r--r--   0 runner    (1001) docker     (127)      594 2023-12-14 12:31:24.000000 frequenz-api-reporting-0.1.1/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/inverter.proto
--rw-r--r--   0 runner    (1001) docker     (127)      919 2023-12-14 12:31:24.000000 frequenz-api-reporting-0.1.1/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/transformer.proto
--rw-r--r--   0 runner    (1001) docker     (127)      966 2023-12-14 12:31:24.000000 frequenz-api-reporting-0.1.1/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/lifetime.proto
--rw-r--r--   0 runner    (1001) docker     (127)     2399 2023-12-14 12:31:24.000000 frequenz-api-reporting-0.1.1/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/microgrid.proto
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 12:31:40.637527 frequenz-api-reporting-0.1.1/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/sensors/
--rw-r--r--   0 runner    (1001) docker     (127)     5595 2023-12-14 12:31:24.000000 frequenz-api-reporting-0.1.1/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/sensors/sensors.proto
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 12:31:40.637527 frequenz-api-reporting-0.1.1/submodules/frequenz-api-common/proto/frequenz/api/common/v1/pagination/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2023-12-14 12:31:24.000000 frequenz-api-reporting-0.1.1/submodules/frequenz-api-common/proto/frequenz/api/common/v1/pagination/pagination_info.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1046 2023-12-14 12:31:24.000000 frequenz-api-reporting-0.1.1/submodules/frequenz-api-common/proto/frequenz/api/common/v1/pagination/pagination_params.proto
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:47:26.661279 frequenz-api-reporting-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-04-24 12:47:07.000000 frequenz-api-reporting-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-24 12:47:07.000000 frequenz-api-reporting-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4801 2024-04-24 12:47:26.657279 frequenz-api-reporting-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3428 2024-04-24 12:47:07.000000 frequenz-api-reporting-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-24 12:47:07.000000 frequenz-api-reporting-0.2.0/RELEASE_NOTES.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:47:26.641279 frequenz-api-reporting-0.2.0/proto/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:47:26.641279 frequenz-api-reporting-0.2.0/proto/frequenz/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:47:26.641279 frequenz-api-reporting-0.2.0/proto/frequenz/api/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:47:26.641279 frequenz-api-reporting-0.2.0/proto/frequenz/api/reporting/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:47:26.645279 frequenz-api-reporting-0.2.0/proto/frequenz/api/reporting/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)    22178 2024-04-24 12:47:07.000000 frequenz-api-reporting-0.2.0/proto/frequenz/api/reporting/v1/reporting.proto
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:47:26.641279 frequenz-api-reporting-0.2.0/py/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:47:26.641279 frequenz-api-reporting-0.2.0/py/frequenz/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:47:26.641279 frequenz-api-reporting-0.2.0/py/frequenz/api/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:47:26.645279 frequenz-api-reporting-0.2.0/py/frequenz/api/reporting/
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-24 12:47:07.000000 frequenz-api-reporting-0.2.0/py/frequenz/api/reporting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-24 12:47:07.000000 frequenz-api-reporting-0.2.0/py/frequenz/api/reporting/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 12:47:07.000000 frequenz-api-reporting-0.2.0/py/frequenz/api/reporting/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:47:26.645279 frequenz-api-reporting-0.2.0/py/frequenz/api/reporting/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-24 12:47:07.000000 frequenz-api-reporting-0.2.0/py/frequenz/api/reporting/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:47:26.649279 frequenz-api-reporting-0.2.0/py/frequenz_api_reporting.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4801 2024-04-24 12:47:26.000000 frequenz-api-reporting-0.2.0/py/frequenz_api_reporting.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5725 2024-04-24 12:47:26.000000 frequenz-api-reporting-0.2.0/py/frequenz_api_reporting.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 12:47:26.000000 frequenz-api-reporting-0.2.0/py/frequenz_api_reporting.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-24 12:47:26.000000 frequenz-api-reporting-0.2.0/py/frequenz_api_reporting.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-24 12:47:26.000000 frequenz-api-reporting-0.2.0/py/frequenz_api_reporting.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4863 2024-04-24 12:47:07.000000 frequenz-api-reporting-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 12:47:26.661279 frequenz-api-reporting-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:47:26.645279 frequenz-api-reporting-0.2.0/submodules/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:47:26.641279 frequenz-api-reporting-0.2.0/submodules/api-common-protos/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:47:26.645279 frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:47:26.653279 frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/api/
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-04-24 12:47:07.000000 frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/api/annotations.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     7374 2024-04-24 12:47:07.000000 frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/api/auth.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-04-24 12:47:07.000000 frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/api/backend.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-04-24 12:47:07.000000 frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/api/billing.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-04-24 12:47:07.000000 frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/api/client.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     3169 2024-04-24 12:47:07.000000 frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/api/config_change.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     2719 2024-04-24 12:47:07.000000 frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/api/consumer.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-04-24 12:47:07.000000 frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/api/context.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-04-24 12:47:07.000000 frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/api/control.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     8657 2024-04-24 12:47:07.000000 frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/api/distribution.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     6132 2024-04-24 12:47:07.000000 frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/api/documentation.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     2824 2024-04-24 12:47:07.000000 frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/api/endpoint.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     3318 2024-04-24 12:47:07.000000 frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/api/field_behavior.proto
+-rw-r--r--   0 runner    (1001) docker     (127)    12099 2024-04-24 12:47:07.000000 frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/api/http.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     2605 2024-04-24 12:47:07.000000 frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/api/httpbody.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-04-24 12:47:07.000000 frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/api/label.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-04-24 12:47:07.000000 frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/api/launch_stage.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-04-24 12:47:07.000000 frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/api/log.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-04-24 12:47:07.000000 frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/api/logging.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     6628 2024-04-24 12:47:07.000000 frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/api/metric.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     5512 2024-04-24 12:47:07.000000 frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/api/monitored_resource.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     3524 2024-04-24 12:47:07.000000 frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/api/monitoring.proto
+-rw-r--r--   0 runner    (1001) docker     (127)    10854 2024-04-24 12:47:07.000000 frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/api/quota.proto
+-rw-r--r--   0 runner    (1001) docker     (127)    11347 2024-04-24 12:47:07.000000 frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/api/resource.proto
+-rw-r--r--   0 runner    (1001) docker     (127)    14929 2024-04-24 12:47:07.000000 frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/api/routing.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     6099 2024-04-24 12:47:07.000000 frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/api/service.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-04-24 12:47:07.000000 frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/api/source_info.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     3472 2024-04-24 12:47:07.000000 frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/api/system_parameter.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     3513 2024-04-24 12:47:07.000000 frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/api/usage.proto
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:47:26.653279 frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/cloud/
+-rw-r--r--   0 runner    (1001) docker     (127)     6308 2024-04-24 12:47:07.000000 frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/cloud/extended_operations.proto
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:47:26.641279 frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/iam/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:47:26.641279 frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/iam/admin/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:47:26.653279 frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/iam/admin/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)    41483 2024-04-24 12:47:07.000000 frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/iam/admin/v1/iam.proto
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:47:26.653279 frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/iam/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)     5482 2024-04-24 12:47:07.000000 frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/iam/v1/iam_policy.proto
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:47:26.653279 frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/iam/v1/logging/
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-04-24 12:47:07.000000 frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/iam/v1/logging/audit_data.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-04-24 12:47:07.000000 frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/iam/v1/options.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     8659 2024-04-24 12:47:07.000000 frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/iam/v1/policy.proto
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:47:26.641279 frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/logging/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:47:26.653279 frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/logging/type/
+-rw-r--r--   0 runner    (1001) docker     (127)     3389 2024-04-24 12:47:07.000000 frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/logging/type/http_request.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-04-24 12:47:07.000000 frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/logging/type/log_severity.proto
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:47:26.653279 frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/longrunning/
+-rw-r--r--   0 runner    (1001) docker     (127)    10515 2024-04-24 12:47:07.000000 frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/longrunning/operations.proto
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:47:26.653279 frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/rpc/
+-rw-r--r--   0 runner    (1001) docker     (127)     7125 2024-04-24 12:47:07.000000 frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/rpc/code.proto
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:47:26.653279 frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/rpc/context/
+-rw-r--r--   0 runner    (1001) docker     (127)    12015 2024-04-24 12:47:07.000000 frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/rpc/context/attribute_context.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     9504 2024-04-24 12:47:07.000000 frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/rpc/error_details.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-04-24 12:47:07.000000 frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/rpc/status.proto
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:47:26.657279 frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/type/
+-rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-04-24 12:47:07.000000 frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/type/calendar_period.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     6193 2024-04-24 12:47:07.000000 frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/type/color.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-04-24 12:47:07.000000 frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/type/date.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     3508 2024-04-24 12:47:07.000000 frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/type/datetime.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-04-24 12:47:07.000000 frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/type/dayofweek.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-04-24 12:47:07.000000 frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/type/expr.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-04-24 12:47:07.000000 frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/type/fraction.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-04-24 12:47:07.000000 frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/type/latlng.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-04-24 12:47:07.000000 frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/type/money.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-04-24 12:47:07.000000 frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/type/month.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     6239 2024-04-24 12:47:07.000000 frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/type/postal_address.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     3795 2024-04-24 12:47:07.000000 frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/type/quaternion.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-04-24 12:47:07.000000 frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/type/timeofday.proto
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:47:26.645279 frequenz-api-reporting-0.2.0/submodules/frequenz-api-common/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:47:26.645279 frequenz-api-reporting-0.2.0/submodules/frequenz-api-common/proto/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:47:26.645279 frequenz-api-reporting-0.2.0/submodules/frequenz-api-common/proto/frequenz/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:47:26.645279 frequenz-api-reporting-0.2.0/submodules/frequenz-api-common/proto/frequenz/api/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:47:26.657279 frequenz-api-reporting-0.2.0/submodules/frequenz-api-common/proto/frequenz/api/common/
+-rw-r--r--   0 runner    (1001) docker     (127)     3557 2024-04-24 12:47:08.000000 frequenz-api-reporting-0.2.0/submodules/frequenz-api-common/proto/frequenz/api/common/components.proto
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-24 12:47:08.000000 frequenz-api-reporting-0.2.0/submodules/frequenz-api-common/proto/frequenz/api/common/location.proto
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:47:26.657279 frequenz-api-reporting-0.2.0/submodules/frequenz-api-common/proto/frequenz/api/common/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)     6191 2024-04-24 12:47:08.000000 frequenz-api-reporting-0.2.0/submodules/frequenz-api-common/proto/frequenz/api/common/metrics/electrical.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     7405 2024-04-24 12:47:08.000000 frequenz-api-reporting-0.2.0/submodules/frequenz-api-common/proto/frequenz/api/common/metrics.proto
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:47:26.657279 frequenz-api-reporting-0.2.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:47:26.657279 frequenz-api-reporting-0.2.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/grid/
+-rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-04-24 12:47:08.000000 frequenz-api-reporting-0.2.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/grid/delivery_area.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-04-24 12:47:08.000000 frequenz-api-reporting-0.2.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/grid/delivery_duration.proto
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-24 12:47:08.000000 frequenz-api-reporting-0.2.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/location.proto
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:47:26.657279 frequenz-api-reporting-0.2.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/market/
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-04-24 12:47:08.000000 frequenz-api-reporting-0.2.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/market/energy.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-04-24 12:47:08.000000 frequenz-api-reporting-0.2.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/market/price.proto
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:47:26.657279 frequenz-api-reporting-0.2.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-24 12:47:08.000000 frequenz-api-reporting-0.2.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/metrics/bounds.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     8186 2024-04-24 12:47:08.000000 frequenz-api-reporting-0.2.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/metrics/metric_sample.proto
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:47:26.657279 frequenz-api-reporting-0.2.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:47:26.657279 frequenz-api-reporting-0.2.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-04-24 12:47:08.000000 frequenz-api-reporting-0.2.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/battery.proto
+-rw-r--r--   0 runner    (1001) docker     (127)    17511 2024-04-24 12:47:08.000000 frequenz-api-reporting-0.2.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/components.proto
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-24 12:47:08.000000 frequenz-api-reporting-0.2.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/ev_charger.proto
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-04-24 12:47:08.000000 frequenz-api-reporting-0.2.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/fuse.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-04-24 12:47:08.000000 frequenz-api-reporting-0.2.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/grid.proto
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-24 12:47:08.000000 frequenz-api-reporting-0.2.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/inverter.proto
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-04-24 12:47:08.000000 frequenz-api-reporting-0.2.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/transformer.proto
+-rw-r--r--   0 runner    (1001) docker     (127)      966 2024-04-24 12:47:08.000000 frequenz-api-reporting-0.2.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/lifetime.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-04-24 12:47:08.000000 frequenz-api-reporting-0.2.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/microgrid.proto
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:47:26.657279 frequenz-api-reporting-0.2.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/sensors/
+-rw-r--r--   0 runner    (1001) docker     (127)     5691 2024-04-24 12:47:08.000000 frequenz-api-reporting-0.2.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/sensors/sensors.proto
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:47:26.657279 frequenz-api-reporting-0.2.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/pagination/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-24 12:47:08.000000 frequenz-api-reporting-0.2.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/pagination/pagination_info.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-04-24 12:47:08.000000 frequenz-api-reporting-0.2.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/pagination/pagination_params.proto
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:47:26.657279 frequenz-api-reporting-0.2.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/types/
+-rw-r--r--   0 runner    (1001) docker     (127)      823 2024-04-24 12:47:08.000000 frequenz-api-reporting-0.2.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/types/decimal.proto
```

### Comparing `frequenz-api-reporting-0.1.1/LICENSE` & `frequenz-api-reporting-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `frequenz-api-reporting-0.1.1/PKG-INFO` & `frequenz-api-reporting-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frequenz-api-reporting
-Version: 0.1.1
+Version: 0.2.0
 Summary: Frequenz gRPC API to aggregate component data from microgrids
 Author-email: Frequenz Energy-as-a-Service GmbH <floss@frequenz.com>
 License: MIT
 Project-URL: Documentation, https://frequenz-floss.github.io/frequenz-api-reporting/
 Project-URL: Changelog, https://github.com/frequenz-floss/frequenz-api-reporting/releases
 Project-URL: Issues, https://github.com/frequenz-floss/frequenz-api-reporting/issues
 Project-URL: Repository, https://github.com/frequenz-floss/frequenz-api-reporting
```

### Comparing `frequenz-api-reporting-0.1.1/README.md` & `frequenz-api-reporting-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `frequenz-api-reporting-0.1.1/proto/frequenz/api/reporting/v1/reporting.proto` & `frequenz-api-reporting-0.2.0/proto/frequenz/api/reporting/v1/reporting.proto`

 * *Files 2% similar despite different names*

```diff
@@ -91,16 +91,16 @@
   google.protobuf.Timestamp end = 2;
 }
 
 // Resampling options for aggregated microgrid components data.
 // If data is resampled, all samples that fall in a left-closed time interval
 // determined by the resolution will be aggregated.
 // At the moment only mean aggregation is supported.
-// The timestamp of the aggregated sample corresponds to the oldest
-// possible timestamp of the time interval.
+// The timestamp for each aggregated sample represents the beginning of its corresponding
+// time interval, marking the earliest point from which data was aggregated.
 message ResamplingOptions {
   // Optional resampling resolution for the data, represented in seconds.
   // If omitted, data will be returned in its original resolution.
   optional uint32 resolution = 1;
 }
 
 // Include options for filtering microgrid components data.
@@ -166,24 +166,24 @@
 //
 // This message serves to encapsulate aggregate metrics derived from multiple component
 // measurements. It is particularly useful in scenarios where an overall metric needs to be
 // calculated for a set of components. For instance, you could use it to represent the average
 // voltage across multiple sources within a microgrid or to calculate the average state of
 // charge of several batteries.
 //
-message SimpleAggregatedMetricSample {
+message SimpleAggregatedMetricValue {
   // The UTC sample timestamp for the aggregated metrics.
   //
   // !!! info
   //     This is the original timestamp of the samples that were aggregated.
   google.protobuf.Timestamp sampled_at = 1;
 
   // The aggregated value of the metric.
   // float value = 2;
-  frequenz.api.common.v1.metrics.SimpleMetricSample sample = 2;
+  frequenz.api.common.v1.metrics.SimpleMetricValue sample = 2;
 }
 
 // Message defining the request format for fetching historical metrics, such as electrical
 // measurements, and other information for individual microgrid components.
 //
 // !!! note
 //     In addition to the raw metrics, the API can also return additional information
@@ -464,15 +464,15 @@
 message ListAggregatedMicrogridComponentsDataResponse {
   // Encapsulates the result of aggregating a metric.
   message AggregatedResult {
     // Metric and related formula provided for aggregation.
     AggregationConfig aggregation_config = 1;
 
     // A list of aggregated metrics.
-    repeated SimpleAggregatedMetricSample samples = 2;
+    repeated SimpleAggregatedMetricValue samples = 2;
   }
 
   // List of aggregated results, each corresponding to a metric and custom aggregation
   // formula.
   //
   // !!! note
   //     Each entry in this list contains the aggregation formula config and the
@@ -534,9 +534,9 @@
 //     ```
 //
 message ReceiveAggregatedMicrogridComponentsDataStreamResponse {
   // The metric and formula that has been used to aggregate the sample.
   AggregationConfig aggregation_config = 1;
 
   // Aggregated sample value and corresponding UTC timestamp when it was sampled.
-  SimpleAggregatedMetricSample sample = 2;
+  SimpleAggregatedMetricValue sample = 2;
 }
```

### Comparing `frequenz-api-reporting-0.1.1/py/frequenz_api_reporting.egg-info/PKG-INFO` & `frequenz-api-reporting-0.2.0/py/frequenz_api_reporting.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frequenz-api-reporting
-Version: 0.1.1
+Version: 0.2.0
 Summary: Frequenz gRPC API to aggregate component data from microgrids
 Author-email: Frequenz Energy-as-a-Service GmbH <floss@frequenz.com>
 License: MIT
 Project-URL: Documentation, https://frequenz-floss.github.io/frequenz-api-reporting/
 Project-URL: Changelog, https://github.com/frequenz-floss/frequenz-api-reporting/releases
 Project-URL: Issues, https://github.com/frequenz-floss/frequenz-api-reporting/issues
 Project-URL: Repository, https://github.com/frequenz-floss/frequenz-api-reporting
```

### Comparing `frequenz-api-reporting-0.1.1/py/frequenz_api_reporting.egg-info/SOURCES.txt` & `frequenz-api-reporting-0.2.0/py/frequenz_api_reporting.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -64,23 +64,31 @@
 submodules/api-common-protos/google/type/fraction.proto
 submodules/api-common-protos/google/type/latlng.proto
 submodules/api-common-protos/google/type/money.proto
 submodules/api-common-protos/google/type/month.proto
 submodules/api-common-protos/google/type/postal_address.proto
 submodules/api-common-protos/google/type/quaternion.proto
 submodules/api-common-protos/google/type/timeofday.proto
+submodules/frequenz-api-common/proto/frequenz/api/common/components.proto
+submodules/frequenz-api-common/proto/frequenz/api/common/location.proto
+submodules/frequenz-api-common/proto/frequenz/api/common/metrics.proto
+submodules/frequenz-api-common/proto/frequenz/api/common/metrics/electrical.proto
 submodules/frequenz-api-common/proto/frequenz/api/common/v1/location.proto
 submodules/frequenz-api-common/proto/frequenz/api/common/v1/grid/delivery_area.proto
+submodules/frequenz-api-common/proto/frequenz/api/common/v1/grid/delivery_duration.proto
+submodules/frequenz-api-common/proto/frequenz/api/common/v1/market/energy.proto
+submodules/frequenz-api-common/proto/frequenz/api/common/v1/market/price.proto
 submodules/frequenz-api-common/proto/frequenz/api/common/v1/metrics/bounds.proto
 submodules/frequenz-api-common/proto/frequenz/api/common/v1/metrics/metric_sample.proto
 submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/lifetime.proto
 submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/microgrid.proto
 submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/battery.proto
 submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/components.proto
 submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/ev_charger.proto
 submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/fuse.proto
 submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/grid.proto
 submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/inverter.proto
 submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/transformer.proto
 submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/sensors/sensors.proto
 submodules/frequenz-api-common/proto/frequenz/api/common/v1/pagination/pagination_info.proto
-submodules/frequenz-api-common/proto/frequenz/api/common/v1/pagination/pagination_params.proto
+submodules/frequenz-api-common/proto/frequenz/api/common/v1/pagination/pagination_params.proto
+submodules/frequenz-api-common/proto/frequenz/api/common/v1/types/decimal.proto
```

### Comparing `frequenz-api-reporting-0.1.1/py/frequenz_api_reporting.egg-info/requires.txt` & `frequenz-api-reporting-0.2.0/py/frequenz_api_reporting.egg-info/requires.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-frequenz-api-common<0.6.0,>=0.5.1
-googleapis-common-protos<2,>=1.56.2
+frequenz-api-common<0.7.0,>=0.6.0
+googleapis-common-protos<2,>=1.56.3
 grpcio<2,>=1.51.1
 
 [dev]
 frequenz-api-reporting[dev-flake8,dev-formatting,dev-mkdocs,dev-mypy,dev-noxfile,dev-pylint,dev-pytest]
 
 [dev-flake8]
 flake8==6.1.0
```

### Comparing `frequenz-api-reporting-0.1.1/pyproject.toml` & `frequenz-api-reporting-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -22,16 +22,16 @@
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3 :: Only",
   "Topic :: Software Development :: Libraries",
   "Typing :: Typed",
 ]
 requires-python = ">= 3.11, < 4"
 dependencies = [
-  "frequenz-api-common >= 0.5.1, < 0.6.0",
-  "googleapis-common-protos >= 1.56.2, < 2",
+  "frequenz-api-common >= 0.6.0, < 0.7.0",
+  "googleapis-common-protos >= 1.56.3, < 2",
   "grpcio >= 1.51.1, < 2",
 ]
 dynamic = ["version"]
 
 [[project.authors]]
 name = "Frequenz Energy-as-a-Service GmbH"
 email = "floss@frequenz.com"
```

### Comparing `frequenz-api-reporting-0.1.1/submodules/api-common-protos/google/api/annotations.proto` & `frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/api/annotations.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-reporting-0.1.1/submodules/api-common-protos/google/api/auth.proto` & `frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/api/auth.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-reporting-0.1.1/submodules/api-common-protos/google/api/backend.proto` & `frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/api/backend.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-reporting-0.1.1/submodules/api-common-protos/google/api/billing.proto` & `frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/api/billing.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-reporting-0.1.1/submodules/api-common-protos/google/api/client.proto` & `frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/api/client.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-reporting-0.1.1/submodules/api-common-protos/google/api/config_change.proto` & `frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/api/config_change.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-reporting-0.1.1/submodules/api-common-protos/google/api/consumer.proto` & `frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/api/consumer.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-reporting-0.1.1/submodules/api-common-protos/google/api/context.proto` & `frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/api/context.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-reporting-0.1.1/submodules/api-common-protos/google/api/control.proto` & `frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/api/control.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-reporting-0.1.1/submodules/api-common-protos/google/api/distribution.proto` & `frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/api/distribution.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-reporting-0.1.1/submodules/api-common-protos/google/api/documentation.proto` & `frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/api/documentation.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-reporting-0.1.1/submodules/api-common-protos/google/api/endpoint.proto` & `frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/api/endpoint.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-reporting-0.1.1/submodules/api-common-protos/google/api/field_behavior.proto` & `frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/api/field_behavior.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-reporting-0.1.1/submodules/api-common-protos/google/api/http.proto` & `frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/api/http.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-reporting-0.1.1/submodules/api-common-protos/google/api/httpbody.proto` & `frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/api/httpbody.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-reporting-0.1.1/submodules/api-common-protos/google/api/label.proto` & `frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/api/label.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-reporting-0.1.1/submodules/api-common-protos/google/api/launch_stage.proto` & `frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/api/launch_stage.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-reporting-0.1.1/submodules/api-common-protos/google/api/log.proto` & `frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/api/log.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-reporting-0.1.1/submodules/api-common-protos/google/api/logging.proto` & `frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/api/logging.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-reporting-0.1.1/submodules/api-common-protos/google/api/metric.proto` & `frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/api/metric.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-reporting-0.1.1/submodules/api-common-protos/google/api/monitored_resource.proto` & `frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/api/monitored_resource.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-reporting-0.1.1/submodules/api-common-protos/google/api/monitoring.proto` & `frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/api/monitoring.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-reporting-0.1.1/submodules/api-common-protos/google/api/quota.proto` & `frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/api/quota.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-reporting-0.1.1/submodules/api-common-protos/google/api/resource.proto` & `frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/api/resource.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-reporting-0.1.1/submodules/api-common-protos/google/api/routing.proto` & `frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/api/routing.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-reporting-0.1.1/submodules/api-common-protos/google/api/service.proto` & `frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/api/service.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-reporting-0.1.1/submodules/api-common-protos/google/api/source_info.proto` & `frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/api/source_info.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-reporting-0.1.1/submodules/api-common-protos/google/api/system_parameter.proto` & `frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/api/system_parameter.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-reporting-0.1.1/submodules/api-common-protos/google/api/usage.proto` & `frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/api/usage.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-reporting-0.1.1/submodules/api-common-protos/google/cloud/extended_operations.proto` & `frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/cloud/extended_operations.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-reporting-0.1.1/submodules/api-common-protos/google/iam/admin/v1/iam.proto` & `frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/iam/admin/v1/iam.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-reporting-0.1.1/submodules/api-common-protos/google/iam/v1/iam_policy.proto` & `frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/iam/v1/iam_policy.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-reporting-0.1.1/submodules/api-common-protos/google/iam/v1/logging/audit_data.proto` & `frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/iam/v1/logging/audit_data.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-reporting-0.1.1/submodules/api-common-protos/google/iam/v1/options.proto` & `frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/iam/v1/options.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-reporting-0.1.1/submodules/api-common-protos/google/iam/v1/policy.proto` & `frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/iam/v1/policy.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-reporting-0.1.1/submodules/api-common-protos/google/logging/type/http_request.proto` & `frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/logging/type/http_request.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-reporting-0.1.1/submodules/api-common-protos/google/logging/type/log_severity.proto` & `frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/logging/type/log_severity.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-reporting-0.1.1/submodules/api-common-protos/google/longrunning/operations.proto` & `frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/longrunning/operations.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-reporting-0.1.1/submodules/api-common-protos/google/rpc/code.proto` & `frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/rpc/code.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-reporting-0.1.1/submodules/api-common-protos/google/rpc/context/attribute_context.proto` & `frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/rpc/context/attribute_context.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-reporting-0.1.1/submodules/api-common-protos/google/rpc/error_details.proto` & `frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/rpc/error_details.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-reporting-0.1.1/submodules/api-common-protos/google/rpc/status.proto` & `frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/rpc/status.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-reporting-0.1.1/submodules/api-common-protos/google/type/calendar_period.proto` & `frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/type/calendar_period.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-reporting-0.1.1/submodules/api-common-protos/google/type/color.proto` & `frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/type/color.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-reporting-0.1.1/submodules/api-common-protos/google/type/date.proto` & `frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/type/date.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-reporting-0.1.1/submodules/api-common-protos/google/type/datetime.proto` & `frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/type/datetime.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-reporting-0.1.1/submodules/api-common-protos/google/type/dayofweek.proto` & `frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/type/dayofweek.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-reporting-0.1.1/submodules/api-common-protos/google/type/expr.proto` & `frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/type/expr.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-reporting-0.1.1/submodules/api-common-protos/google/type/fraction.proto` & `frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/type/fraction.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-reporting-0.1.1/submodules/api-common-protos/google/type/latlng.proto` & `frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/type/latlng.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-reporting-0.1.1/submodules/api-common-protos/google/type/money.proto` & `frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/type/money.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-reporting-0.1.1/submodules/api-common-protos/google/type/month.proto` & `frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/type/month.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-reporting-0.1.1/submodules/api-common-protos/google/type/postal_address.proto` & `frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/type/postal_address.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-reporting-0.1.1/submodules/api-common-protos/google/type/quaternion.proto` & `frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/type/quaternion.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-reporting-0.1.1/submodules/api-common-protos/google/type/timeofday.proto` & `frequenz-api-reporting-0.2.0/submodules/api-common-protos/google/type/timeofday.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-reporting-0.1.1/submodules/frequenz-api-common/proto/frequenz/api/common/v1/grid/delivery_area.proto` & `frequenz-api-reporting-0.2.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/grid/delivery_area.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-reporting-0.1.1/submodules/frequenz-api-common/proto/frequenz/api/common/v1/location.proto` & `frequenz-api-reporting-0.2.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/location.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-reporting-0.1.1/submodules/frequenz-api-common/proto/frequenz/api/common/v1/metrics/metric_sample.proto` & `frequenz-api-reporting-0.2.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/metrics/metric_sample.proto`

 * *Files 16% similar despite different names*

```diff
@@ -12,57 +12,57 @@
 
 import "frequenz/api/common/v1/metrics/bounds.proto";
 
 import "google/protobuf/timestamp.proto";
 
 // Represents a single sample of a specific metric, the value of which is either
 // measured or derived at a particular time.
-message SimpleMetricSample {
+message SimpleMetricValue {
   // The value of the metric, which could be either measured or derived.
   float value = 2;
 }
 
 // Encapsulates derived statistical summaries of a single metric.
 //
 // The message allows for the reporting of statistical summaries — minimum,
 // maximum, and average values - as well as the complete list of individual
 // samples if available.
 //
 // This message represents derived metrics and contains fields for statistical
 // summaries—minimum, maximum, and average values. Individual measurements are
 // are optional, accommodating scenarios where only subsets of this information
 // are available.
-message AggregatedMetricSample {
+message AggregatedMetricValue {
   // The derived average value of the metric.
   float avg_value = 2;
 
   // The minimum measured value of the metric.
   optional float min_value = 3;
 
   // The maximum measured value of the metric.
   optional float max_value = 4;
 
   // Optional array of all the raw individual values.
   repeated float raw_values = 5;
 }
 
-// MetricSampleVariant serves as a union type that can encapsulate either a
-// `SimpleMetricSample` or an `AggregatedMetricSample`.
+// `MetricValueVariant` serves as a union type that can encapsulate either a
+// `SimpleMetricValue` or an `AggregatedMetricValue`.
 //
 // This message is designed to offer flexibility in capturing different
 // granularities of metric samples—either a simple single-point measurement
 // or an aggregated set of measurements for a metric.
 //
-// A `MetricSampleVariant` can hold either a `SimpleMetricSample` or an
-// `AggregatedMetricSample`, but not both simultaneously. Setting one will
+// A `MetricValueVariant` can hold either a `SimpleMetricValue` or an
+// `AggregatedMetricValue`, but not both simultaneously. Setting one will
 // nullify the other.
-message MetricSampleVariant {
-  oneof metric_sample_type {
-    SimpleMetricSample simple_metric = 1;
-    AggregatedMetricSample aggregated_metric = 2;
+message MetricValueVariant {
+  oneof metric_value_variant {
+    SimpleMetricValue simple_metric = 1;
+    AggregatedMetricValue aggregated_metric = 2;
   }
 }
 
 // List of supported metrics.
 enum Metric {
   // Default value.
   METRIC_UNSPECIFIED = 0;
@@ -71,35 +71,38 @@
   METRIC_DC_VOLTAGE = 1;
   METRIC_DC_CURRENT = 2;
   METRIC_DC_POWER = 3;
 
   // General AC electricity metrics
   METRIC_AC_FREQUENCY = 10;
   METRIC_AC_VOLTAGE = 11;
-  METRIC_AC_VOLTAGE_PHASE_1 = 12;
-  METRIC_AC_VOLTAGE_PHASE_2 = 13;
-  METRIC_AC_VOLTAGE_PHASE_3 = 14;
-  METRIC_AC_APPARENT_CURRENT = 15;
-  METRIC_AC_APPARENT_CURRENT_PHASE_1 = 16;
-  METRIC_AC_APPARENT_CURRENT_PHASE_2 = 17;
-  METRIC_AC_APPARENT_CURRENT_PHASE_3 = 18;
+  METRIC_AC_VOLTAGE_PHASE_1_N = 12;
+  METRIC_AC_VOLTAGE_PHASE_2_N = 13;
+  METRIC_AC_VOLTAGE_PHASE_3_N = 14;
+  METRIC_AC_VOLTAGE_PHASE_1_PHASE_2 = 15;
+  METRIC_AC_VOLTAGE_PHASE_2_PHASE_3 = 16;
+  METRIC_AC_VOLTAGE_PHASE_3_PHASE_1 = 17;
+  METRIC_AC_CURRENT = 18;
+  METRIC_AC_CURRENT_PHASE_1 = 19;
+  METRIC_AC_CURRENT_PHASE_2 = 20;
+  METRIC_AC_CURRENT_PHASE_3 = 21;
 
   // AC power metrics
-  METRIC_AC_APPARENT_POWER = 20;
-  METRIC_AC_APPARENT_POWER_PHASE_1 = 21;
-  METRIC_AC_APPARENT_POWER_PHASE_2 = 22;
-  METRIC_AC_APPARENT_POWER_PHASE_3 = 23;
-  METRIC_AC_ACTIVE_POWER = 24;
-  METRIC_AC_ACTIVE_POWER_PHASE_1 = 25;
-  METRIC_AC_ACTIVE_POWER_PHASE_2 = 26;
-  METRIC_AC_ACTIVE_POWER_PHASE_3 = 27;
-  METRIC_AC_REACTIVE_POWER = 28;
-  METRIC_AC_REACTIVE_POWER_PHASE_1 = 29;
-  METRIC_AC_REACTIVE_POWER_PHASE_2 = 30;
-  METRIC_AC_REACTIVE_POWER_PHASE_3 = 31;
+  METRIC_AC_APPARENT_POWER = 22;
+  METRIC_AC_APPARENT_POWER_PHASE_1 = 23;
+  METRIC_AC_APPARENT_POWER_PHASE_2 = 24;
+  METRIC_AC_APPARENT_POWER_PHASE_3 = 25;
+  METRIC_AC_ACTIVE_POWER = 26;
+  METRIC_AC_ACTIVE_POWER_PHASE_1 = 27;
+  METRIC_AC_ACTIVE_POWER_PHASE_2 = 28;
+  METRIC_AC_ACTIVE_POWER_PHASE_3 = 29;
+  METRIC_AC_REACTIVE_POWER = 30;
+  METRIC_AC_REACTIVE_POWER_PHASE_1 = 31;
+  METRIC_AC_REACTIVE_POWER_PHASE_2 = 32;
+  METRIC_AC_REACTIVE_POWER_PHASE_3 = 33;
 
   // AC Power factor
   METRIC_AC_POWER_FACTOR = 40;
   METRIC_AC_POWER_FACTOR_PHASE_1 = 41;
   METRIC_AC_POWER_FACTOR_PHASE_2 = 42;
   METRIC_AC_POWER_FACTOR_PHASE_3 = 43;
 
@@ -122,26 +125,29 @@
   METRIC_AC_ACTIVE_ENERGY_DELIVERED_PHASE_3 = 65;
   METRIC_AC_REACTIVE_ENERGY = 66;
   METRIC_AC_REACTIVE_ENERGY_PHASE_1 = 67;
   METRIC_AC_REACTIVE_ENERGY_PHASE_2 = 69;
   METRIC_AC_REACTIVE_ENERGY_PHASE_3 = 70;
 
   // AC harmonics
-  METRIC_AC_THD_CURRENT = 80;
-  METRIC_AC_THD_CURRENT_PHASE_1 = 81;
-  METRIC_AC_THD_CURRENT_PHASE_2 = 82;
-  METRIC_AC_THD_CURRENT_PHASE_3 = 83;
+  METRIC_AC_TOTAL_HARMONIC_DISTORTION_CURRENT = 80;
+  METRIC_AC_TOTAL_HARMONIC_DISTORTION_CURRENT_PHASE_1 = 81;
+  METRIC_AC_TOTAL_HARMONIC_DISTORTION_CURRENT_PHASE_2 = 82;
+  METRIC_AC_TOTAL_HARMONIC_DISTORTION_CURRENT_PHASE_3 = 83;
 
   // General BMS metrics.
   METRIC_BATTERY_CAPACITY = 101;
   METRIC_BATTERY_SOC_PCT = 102;
   METRIC_BATTERY_TEMPERATURE = 103;
 
   // General inverter metrics.
   METRIC_INVERTER_TEMPERATURE = 120;
+  METRIC_INVERTER_TEMPERATURE_CABINET = 121;
+  METRIC_INVERTER_TEMPERATURE_HEATSINK = 122;
+  METRIC_INVERTER_TEMPERATURE_TRANSFORMER = 123;
 
   // EV charging station metrics.
   METRIC_EV_CHARGER_TEMPERATURE = 140;
 
   // General sensor metrics
   METRIC_SENSOR_WIND_SPEED = 160;
   METRIC_SENSOR_WIND_DIRECTION = 162;
@@ -168,15 +174,15 @@
   // The UTC timestamp of when the metric was sampled.
   google.protobuf.Timestamp sampled_at = 1;
 
   // The metric that was sampled.
   Metric metric = 2;
 
   // The value of the sampled metric.
-  MetricSampleVariant sample = 3;
+  MetricValueVariant value = 3;
 
   // List of bounds that apply to the metric sample.
   //
   // These bounds adapt in real-time to reflect the operating conditions at the
   // time of aggregation or derivation.
   //
   // #### Multiple Bounds
@@ -197,8 +203,24 @@
   //      bound[0].lower                         bound[1].upper
   // <-------|============|------------------|============|--------->
   //                bound[0].upper      bound[1].lower
   // ```
   // ---- values here are disallowed and will be rejected
   // ==== values here are allowed and will be accepted
   repeated Bounds bounds = 4;
+
+  // An optional string that can be used to identify the source of the metric.
+  //
+  // This is expected to be populated when the same `Metric` variant can be
+  // obtained from multiple sensors in the component. Knowing the source of the
+  // metric can help in certain control and monitoring applications.
+  //
+  // E.g., a hybrid inverter can have a DC string for a battery and another DC
+  // string for a PV array. The source names could resemble, say,
+  // `dc_battery_0` and ``dc_pv_0`. A metric like DC voltage can be obtained
+  // from both sources. For an application to determine the SoC of the battery
+  // using the battery voltage, the source of the voltage metric is important.
+  //
+  // In cases where the component has just one source for a metric, then this
+  // field is not expected to be present, because the source is implicit.
+  optional string source = 5;
 }
```

### Comparing `frequenz-api-reporting-0.1.1/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/battery.proto` & `frequenz-api-reporting-0.2.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/battery.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-reporting-0.1.1/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/components.proto` & `frequenz-api-reporting-0.2.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/components.proto`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 // License:
 // MIT
 
 syntax = "proto3";
 
 package frequenz.api.common.v1.microgrid.components;
 
+import "frequenz/api/common/v1/metrics/bounds.proto";
 import "frequenz/api/common/v1/metrics/metric_sample.proto";
 import "frequenz/api/common/v1/microgrid/components/battery.proto";
 import "frequenz/api/common/v1/microgrid/components/ev_charger.proto";
 import "frequenz/api/common/v1/microgrid/components/fuse.proto";
 import "frequenz/api/common/v1/microgrid/components/grid.proto";
 import "frequenz/api/common/v1/microgrid/components/inverter.proto";
 import "frequenz/api/common/v1/microgrid/components/transformer.proto";
@@ -137,14 +138,34 @@
   string model_name = 7;
 
   // The status of the component.
   ComponentStatus status = 8;
 
   // The operational lifetime of the component.
   frequenz.api.common.v1.microgrid.Lifetime operational_lifetime = 9;
+
+  // List of rated bounds present for the component identified by Metric.
+  repeated MetricConfigBounds metric_config_bounds = 10;
+}
+
+// MetricConfigBounds describes a set of limits for a specific metric consisting
+// of a lower and upper bound for said metric.
+//
+// This can be used for example to specify an allowed range of power output
+// for a component.
+message MetricConfigBounds {
+  // Metric type the config bounds are for
+  frequenz.api.common.v1.metrics.Metric metric = 1;
+
+  // The set of bounds for the specified metric.
+  //
+  // This contains the lower and upper bounds for said metric.
+  // Sources these may be derived from include the component configuration,
+  // manufacturers limits, and limits of other devices.
+  frequenz.api.common.v1.metrics.Bounds config_bounds = 2;
 }
 
 // ComponentConnection describes a single electrical link between two components
 // within a microgrid, effectively representing the physical wiring as viewed
 // from the grid connection point, if one exists, or from the islanding point,
 // in case of an islanded microgrids.
 //
@@ -189,34 +210,36 @@
 //    {
 //      component_id: 13,
 //      metric_samples: [
 //        /* list of metrics for multiple timestamps */
 //        {
 //          sampled_at: "2023-10-01T00:00:00Z",
 //          metric: "DC_VOLTAGE_V",
-//          sample: {},
+//          value: {},
 //          bounds: {},
 //        },
 //        {
 //          sampled_at: "2023-10-01T00:00:00Z",
 //          metric: "DC_VOLTAGE_V",
-//          sample: {},
+//          value: {},
 //          bounds: {},
 //        }
 //      ],
 //      states: [
 //        /* list of states for multiple timestamps */
 //        {
 //          sampled_at: "2023-10-01T00:00:00Z",
 //          states: [],
+//          warnings: [],
 //          errors: [],
 //        },
 //        {
 //          sampled_at: "2023-10-01T00:00:00Z",
 //          states: [],
+//          warnings: [],
 //          errors: [],
 //        },
 //      ]
 //    }
 //  ```
 message ComponentData {
   // The ID of the microgrid component.
```

### Comparing `frequenz-api-reporting-0.1.1/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/ev_charger.proto` & `frequenz-api-reporting-0.2.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/ev_charger.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-reporting-0.1.1/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/fuse.proto` & `frequenz-api-reporting-0.2.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/fuse.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-reporting-0.1.1/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/grid.proto` & `frequenz-api-reporting-0.2.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/grid.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-reporting-0.1.1/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/inverter.proto` & `frequenz-api-reporting-0.2.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/inverter.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-reporting-0.1.1/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/transformer.proto` & `frequenz-api-reporting-0.2.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/transformer.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-reporting-0.1.1/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/lifetime.proto` & `frequenz-api-reporting-0.2.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/lifetime.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-reporting-0.1.1/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/microgrid.proto` & `frequenz-api-reporting-0.2.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/microgrid.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-reporting-0.1.1/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/sensors/sensors.proto` & `frequenz-api-reporting-0.2.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/sensors/sensors.proto`

 * *Files 8% similar despite different names*

```diff
@@ -103,37 +103,43 @@
   // Dew point.
   // The temperature at which the air becomes saturated with water vapor.
   //
   // In Celsius (°C).
   SENSOR_METRIC_DEW_POINT = 8;
 }
 
-// ComponentData message aggregates multiple metrics, operational states, and
-// errors, related to a specific microgrid component.
+// SensorData message aggregates multiple metrics, operational states, and
+// errors, related to a specific microgrid sensor.
 //
 // !!! example
 //   Example output of a component data message:
 //   ```
 //    {
-//      component_id: 13,
+//      sensor_id: 13,
 //      metric_samples: [
 //        /* list of metrics for multiple timestamps */
 //        {
 //          sampled_at: "2023-10-01T00:00:00Z",
 //          metric: "METRIC_SENSOR_TEMPERATURE",
-//          sample: metric_sample_type: {simple_metric: {value: 23.5},
-//          bounds: {},
+//          value: metric_value_variant: {simple_metric: {value: 23.5},
 //        },
 //        {
 //          sampled_at: "2023-10-01T00:00:00Z",
 //          metric: "METRIC_SENSOR_RELATIVE_HUMIDITY",
-//          sample: metric_sample_type: {simple_metric: {value: 23.5},
-//          bounds: {},
+//          value: metric_value_variant: {simple_metric: {value: 23.5},
 //        }
+//      ],
+//      states: [
+//        {
+//          sampled_at: "2023-10-01T00:00:00Z",
+//          states: [],
+//          errors: [],
+//        },
 //      ]
+//
 //    }
 //  ```
 message SensorData {
   // The ID of the microgrid sensors.
   uint64 sensor_id = 1;
 
   // List of measurements for a metric of the specific microgrid sensor.
@@ -199,9 +205,9 @@
   // The UTC timestamp of when the metric was sampled.
   google.protobuf.Timestamp sampled_at = 1;
 
   // The metric that was sampled.
   frequenz.api.common.v1.metrics.Metric metric = 2;
 
   // The value of the sampled metric.
-  frequenz.api.common.v1.metrics.MetricSampleVariant sample = 3;
+  frequenz.api.common.v1.metrics.MetricValueVariant value = 3;
 }
```

### Comparing `frequenz-api-reporting-0.1.1/submodules/frequenz-api-common/proto/frequenz/api/common/v1/pagination/pagination_info.proto` & `frequenz-api-reporting-0.2.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/pagination/pagination_info.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-reporting-0.1.1/submodules/frequenz-api-common/proto/frequenz/api/common/v1/pagination/pagination_params.proto` & `frequenz-api-reporting-0.2.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/pagination/pagination_params.proto`

 * *Files identical despite different names*


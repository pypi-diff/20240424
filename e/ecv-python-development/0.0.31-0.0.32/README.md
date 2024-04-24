# Comparing `tmp/ecv-python-development-0.0.31.tar.gz` & `tmp/ecv-python-development-0.0.32.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecv-python-development-0.0.31.tar", last modified: Wed Apr 24 11:46:56 2024, max compression
+gzip compressed data, was "ecv-python-development-0.0.32.tar", last modified: Wed Apr 24 12:20:04 2024, max compression
```

## Comparing `ecv-python-development-0.0.31.tar` & `ecv-python-development-0.0.32.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-04-24 11:46:56.656287 ecv-python-development-0.0.31/
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     1082 2024-04-22 17:32:49.000000 ecv-python-development-0.0.31/LICENSE
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)       39 2024-04-22 17:32:49.000000 ecv-python-development-0.0.31/MANIFEST.in
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      698 2024-04-24 11:46:56.656287 ecv-python-development-0.0.31/PKG-INFO
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      297 2024-04-22 17:32:49.000000 ecv-python-development-0.0.31/README.md
-drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-04-24 11:46:56.626287 ecv-python-development-0.0.31/ecv_python_development/
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      169 2024-04-22 17:32:49.000000 ecv-python-development-0.0.31/ecv_python_development/__init__.py
-drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-04-24 11:46:56.626287 ecv-python-development-0.0.31/ecv_python_development/aws_cloud_native/
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      420 2024-04-22 17:32:49.000000 ecv-python-development-0.0.31/ecv_python_development/aws_cloud_native/__init__.py
-drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-04-24 11:46:56.626287 ecv-python-development-0.0.31/ecv_python_development/aws_cloud_native/events_module/
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)       53 2024-04-22 17:32:49.000000 ecv-python-development-0.0.31/ecv_python_development/aws_cloud_native/events_module/__init__.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     3065 2024-04-22 17:56:33.000000 ecv-python-development-0.0.31/ecv_python_development/aws_cloud_native/events_module/base.py
-drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-04-24 11:46:56.636287 ecv-python-development-0.0.31/ecv_python_development/aws_cloud_native/lambda_module/
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      846 2024-04-22 17:32:49.000000 ecv-python-development-0.0.31/ecv_python_development/aws_cloud_native/lambda_module/__init__.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     1231 2024-04-22 17:32:49.000000 ecv-python-development-0.0.31/ecv_python_development/aws_cloud_native/lambda_module/exceptions.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     1583 2024-04-22 17:32:49.000000 ecv-python-development-0.0.31/ecv_python_development/aws_cloud_native/lambda_module/handler.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      406 2024-04-22 17:32:49.000000 ecv-python-development-0.0.31/ecv_python_development/aws_cloud_native/lambda_module/logger.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      255 2024-04-22 17:32:49.000000 ecv-python-development-0.0.31/ecv_python_development/aws_cloud_native/lambda_module/metrics.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     1471 2024-04-22 17:32:49.000000 ecv-python-development-0.0.31/ecv_python_development/aws_cloud_native/lambda_module/response.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      109 2024-04-22 17:32:49.000000 ecv-python-development-0.0.31/ecv_python_development/aws_cloud_native/lambda_module/tracer.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     3447 2024-04-22 17:32:49.000000 ecv-python-development-0.0.31/ecv_python_development/aws_cloud_native/lambda_module/validator.py
-drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-04-24 11:46:56.646287 ecv-python-development-0.0.31/ecv_python_development/aws_cloud_native/services/
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      169 2024-04-22 17:59:36.000000 ecv-python-development-0.0.31/ecv_python_development/aws_cloud_native/services/__init__.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      616 2024-04-22 17:32:49.000000 ecv-python-development-0.0.31/ecv_python_development/aws_cloud_native/services/aws_service.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     4599 2024-04-22 17:32:49.000000 ecv-python-development-0.0.31/ecv_python_development/aws_cloud_native/services/cognito_service.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     7693 2024-04-22 17:32:49.000000 ecv-python-development-0.0.31/ecv_python_development/aws_cloud_native/services/dynamodb_service.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      683 2024-04-22 17:32:49.000000 ecv-python-development-0.0.31/ecv_python_development/aws_cloud_native/services/eventbridge_service.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)       87 2024-04-22 17:32:49.000000 ecv-python-development-0.0.31/ecv_python_development/aws_cloud_native/services/exceptions.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      986 2024-04-22 17:32:49.000000 ecv-python-development-0.0.31/ecv_python_development/aws_cloud_native/services/kms_service.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     1452 2024-04-22 17:32:49.000000 ecv-python-development-0.0.31/ecv_python_development/aws_cloud_native/services/lambda_service.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     2339 2024-04-22 17:32:49.000000 ecv-python-development-0.0.31/ecv_python_development/aws_cloud_native/services/s3_service.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      806 2024-04-22 17:32:49.000000 ecv-python-development-0.0.31/ecv_python_development/aws_cloud_native/services/secretsmanager_service.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     1090 2024-04-22 17:32:49.000000 ecv-python-development-0.0.31/ecv_python_development/aws_cloud_native/services/ses_service.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      578 2024-04-22 17:32:49.000000 ecv-python-development-0.0.31/ecv_python_development/aws_cloud_native/services/sns_service.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     3232 2024-04-22 17:32:49.000000 ecv-python-development-0.0.31/ecv_python_development/aws_cloud_native/services/sqs_service.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      830 2024-04-22 17:32:49.000000 ecv-python-development-0.0.31/ecv_python_development/aws_cloud_native/services/ssm_service.py
-drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-04-24 11:46:56.646287 ecv-python-development-0.0.31/ecv_python_development/database/
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      267 2024-04-23 12:38:43.000000 ecv-python-development-0.0.31/ecv_python_development/database/__init__.py
-drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-04-24 11:46:56.646287 ecv-python-development-0.0.31/ecv_python_development/database/_pynamodb/
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      121 2024-04-23 10:40:28.000000 ecv-python-development-0.0.31/ecv_python_development/database/_pynamodb/__init__.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      486 2024-04-23 10:36:40.000000 ecv-python-development-0.0.31/ecv_python_development/database/_pynamodb/base.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     5796 2024-04-24 11:46:40.000000 ecv-python-development-0.0.31/ecv_python_development/database/base_model.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-04-22 17:32:49.000000 ecv-python-development-0.0.31/ecv_python_development/database/py.typed
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     1194 2024-04-24 07:19:46.000000 ecv-python-development-0.0.31/ecv_python_development/database/test.py
-drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-04-24 11:46:56.646287 ecv-python-development-0.0.31/ecv_python_development/helpers/
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      308 2024-04-22 17:32:49.000000 ecv-python-development-0.0.31/ecv_python_development/helpers/__init__.py
-drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-04-24 11:46:56.646287 ecv-python-development-0.0.31/ecv_python_development/helpers/datetime/
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)       55 2024-04-22 17:32:49.000000 ecv-python-development-0.0.31/ecv_python_development/helpers/datetime/__init__.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     2458 2024-04-22 17:32:49.000000 ecv-python-development-0.0.31/ecv_python_development/helpers/datetime/standard.py
-drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-04-24 11:46:56.646287 ecv-python-development-0.0.31/ecv_python_development/helpers/debugger/
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)       48 2024-04-22 17:32:49.000000 ecv-python-development-0.0.31/ecv_python_development/helpers/debugger/__init__.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      128 2024-04-22 17:32:49.000000 ecv-python-development-0.0.31/ecv_python_development/helpers/debugger/debugging.py
-drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-04-24 11:46:56.656287 ecv-python-development-0.0.31/ecv_python_development/helpers/files/
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)       43 2024-04-22 17:32:49.000000 ecv-python-development-0.0.31/ecv_python_development/helpers/files/__init__.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      477 2024-04-22 17:32:49.000000 ecv-python-development-0.0.31/ecv_python_development/helpers/files/file.py
-drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-04-24 11:46:56.656287 ecv-python-development-0.0.31/ecv_python_development/helpers/formatter/
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      576 2024-04-22 17:32:49.000000 ecv-python-development-0.0.31/ecv_python_development/helpers/formatter/__init__.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     2658 2024-04-22 17:32:49.000000 ecv-python-development-0.0.31/ecv_python_development/helpers/formatter/formatter.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      149 2024-04-22 17:32:49.000000 ecv-python-development-0.0.31/ecv_python_development/helpers/formatter/regex.py
-drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-04-24 11:46:56.656287 ecv-python-development-0.0.31/ecv_python_development/helpers/http/
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      111 2024-04-22 17:32:49.000000 ecv-python-development-0.0.31/ecv_python_development/helpers/http/__init__.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      729 2024-04-22 17:32:49.000000 ecv-python-development-0.0.31/ecv_python_development/helpers/http/requests.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-04-22 17:32:49.000000 ecv-python-development-0.0.31/ecv_python_development/helpers/py.typed
-drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-04-24 11:46:56.656287 ecv-python-development-0.0.31/ecv_python_development/helpers/strings/
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      123 2024-04-22 17:32:49.000000 ecv-python-development-0.0.31/ecv_python_development/helpers/strings/__init__.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      932 2024-04-22 17:32:49.000000 ecv-python-development-0.0.31/ecv_python_development/helpers/strings/passwords.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)       71 2024-04-22 17:32:49.000000 ecv-python-development-0.0.31/ecv_python_development/helpers/strings/uuid.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-04-22 17:32:49.000000 ecv-python-development-0.0.31/ecv_python_development/py.typed
-drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-04-24 11:46:56.626287 ecv-python-development-0.0.31/ecv_python_development.egg-info/
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      698 2024-04-24 11:46:56.000000 ecv-python-development-0.0.31/ecv_python_development.egg-info/PKG-INFO
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     3025 2024-04-24 11:46:56.000000 ecv-python-development-0.0.31/ecv_python_development.egg-info/SOURCES.txt
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)        1 2024-04-24 11:46:56.000000 ecv-python-development-0.0.31/ecv_python_development.egg-info/dependency_links.txt
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      592 2024-04-24 11:46:56.000000 ecv-python-development-0.0.31/ecv_python_development.egg-info/requires.txt
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)       23 2024-04-24 11:46:56.000000 ecv-python-development-0.0.31/ecv_python_development.egg-info/top_level.txt
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)       38 2024-04-24 11:46:56.656287 ecv-python-development-0.0.31/setup.cfg
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     1708 2024-04-24 11:46:54.000000 ecv-python-development-0.0.31/setup.py
+drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-04-24 12:20:04.236152 ecv-python-development-0.0.32/
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     1082 2024-04-22 17:32:49.000000 ecv-python-development-0.0.32/LICENSE
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)       39 2024-04-22 17:32:49.000000 ecv-python-development-0.0.32/MANIFEST.in
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      698 2024-04-24 12:20:04.236152 ecv-python-development-0.0.32/PKG-INFO
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      297 2024-04-22 17:32:49.000000 ecv-python-development-0.0.32/README.md
+drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-04-24 12:20:04.206152 ecv-python-development-0.0.32/ecv_python_development/
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      169 2024-04-22 17:32:49.000000 ecv-python-development-0.0.32/ecv_python_development/__init__.py
+drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-04-24 12:20:04.216152 ecv-python-development-0.0.32/ecv_python_development/aws_cloud_native/
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      420 2024-04-22 17:32:49.000000 ecv-python-development-0.0.32/ecv_python_development/aws_cloud_native/__init__.py
+drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-04-24 12:20:04.216152 ecv-python-development-0.0.32/ecv_python_development/aws_cloud_native/events_module/
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)       53 2024-04-22 17:32:49.000000 ecv-python-development-0.0.32/ecv_python_development/aws_cloud_native/events_module/__init__.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     3065 2024-04-22 17:56:33.000000 ecv-python-development-0.0.32/ecv_python_development/aws_cloud_native/events_module/base.py
+drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-04-24 12:20:04.216152 ecv-python-development-0.0.32/ecv_python_development/aws_cloud_native/lambda_module/
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      846 2024-04-22 17:32:49.000000 ecv-python-development-0.0.32/ecv_python_development/aws_cloud_native/lambda_module/__init__.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     1231 2024-04-22 17:32:49.000000 ecv-python-development-0.0.32/ecv_python_development/aws_cloud_native/lambda_module/exceptions.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     1583 2024-04-22 17:32:49.000000 ecv-python-development-0.0.32/ecv_python_development/aws_cloud_native/lambda_module/handler.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      406 2024-04-22 17:32:49.000000 ecv-python-development-0.0.32/ecv_python_development/aws_cloud_native/lambda_module/logger.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      255 2024-04-22 17:32:49.000000 ecv-python-development-0.0.32/ecv_python_development/aws_cloud_native/lambda_module/metrics.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     1471 2024-04-22 17:32:49.000000 ecv-python-development-0.0.32/ecv_python_development/aws_cloud_native/lambda_module/response.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      109 2024-04-22 17:32:49.000000 ecv-python-development-0.0.32/ecv_python_development/aws_cloud_native/lambda_module/tracer.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     3447 2024-04-22 17:32:49.000000 ecv-python-development-0.0.32/ecv_python_development/aws_cloud_native/lambda_module/validator.py
+drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-04-24 12:20:04.226152 ecv-python-development-0.0.32/ecv_python_development/aws_cloud_native/services/
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      169 2024-04-22 17:59:36.000000 ecv-python-development-0.0.32/ecv_python_development/aws_cloud_native/services/__init__.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      616 2024-04-22 17:32:49.000000 ecv-python-development-0.0.32/ecv_python_development/aws_cloud_native/services/aws_service.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     4599 2024-04-22 17:32:49.000000 ecv-python-development-0.0.32/ecv_python_development/aws_cloud_native/services/cognito_service.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     7693 2024-04-22 17:32:49.000000 ecv-python-development-0.0.32/ecv_python_development/aws_cloud_native/services/dynamodb_service.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      683 2024-04-22 17:32:49.000000 ecv-python-development-0.0.32/ecv_python_development/aws_cloud_native/services/eventbridge_service.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)       87 2024-04-22 17:32:49.000000 ecv-python-development-0.0.32/ecv_python_development/aws_cloud_native/services/exceptions.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      986 2024-04-22 17:32:49.000000 ecv-python-development-0.0.32/ecv_python_development/aws_cloud_native/services/kms_service.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     1452 2024-04-22 17:32:49.000000 ecv-python-development-0.0.32/ecv_python_development/aws_cloud_native/services/lambda_service.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     2339 2024-04-22 17:32:49.000000 ecv-python-development-0.0.32/ecv_python_development/aws_cloud_native/services/s3_service.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      806 2024-04-22 17:32:49.000000 ecv-python-development-0.0.32/ecv_python_development/aws_cloud_native/services/secretsmanager_service.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     1090 2024-04-22 17:32:49.000000 ecv-python-development-0.0.32/ecv_python_development/aws_cloud_native/services/ses_service.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      578 2024-04-22 17:32:49.000000 ecv-python-development-0.0.32/ecv_python_development/aws_cloud_native/services/sns_service.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     3232 2024-04-22 17:32:49.000000 ecv-python-development-0.0.32/ecv_python_development/aws_cloud_native/services/sqs_service.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      830 2024-04-22 17:32:49.000000 ecv-python-development-0.0.32/ecv_python_development/aws_cloud_native/services/ssm_service.py
+drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-04-24 12:20:04.226152 ecv-python-development-0.0.32/ecv_python_development/database/
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      267 2024-04-23 12:38:43.000000 ecv-python-development-0.0.32/ecv_python_development/database/__init__.py
+drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-04-24 12:20:04.226152 ecv-python-development-0.0.32/ecv_python_development/database/_pynamodb/
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      121 2024-04-23 10:40:28.000000 ecv-python-development-0.0.32/ecv_python_development/database/_pynamodb/__init__.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      486 2024-04-23 10:36:40.000000 ecv-python-development-0.0.32/ecv_python_development/database/_pynamodb/base.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     5759 2024-04-24 12:19:29.000000 ecv-python-development-0.0.32/ecv_python_development/database/base_model.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-04-22 17:32:49.000000 ecv-python-development-0.0.32/ecv_python_development/database/py.typed
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     1196 2024-04-24 12:18:58.000000 ecv-python-development-0.0.32/ecv_python_development/database/test.py
+drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-04-24 12:20:04.226152 ecv-python-development-0.0.32/ecv_python_development/helpers/
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      308 2024-04-22 17:32:49.000000 ecv-python-development-0.0.32/ecv_python_development/helpers/__init__.py
+drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-04-24 12:20:04.226152 ecv-python-development-0.0.32/ecv_python_development/helpers/datetime/
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)       55 2024-04-22 17:32:49.000000 ecv-python-development-0.0.32/ecv_python_development/helpers/datetime/__init__.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     2458 2024-04-22 17:32:49.000000 ecv-python-development-0.0.32/ecv_python_development/helpers/datetime/standard.py
+drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-04-24 12:20:04.226152 ecv-python-development-0.0.32/ecv_python_development/helpers/debugger/
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)       48 2024-04-22 17:32:49.000000 ecv-python-development-0.0.32/ecv_python_development/helpers/debugger/__init__.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      128 2024-04-22 17:32:49.000000 ecv-python-development-0.0.32/ecv_python_development/helpers/debugger/debugging.py
+drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-04-24 12:20:04.226152 ecv-python-development-0.0.32/ecv_python_development/helpers/files/
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)       43 2024-04-22 17:32:49.000000 ecv-python-development-0.0.32/ecv_python_development/helpers/files/__init__.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      477 2024-04-22 17:32:49.000000 ecv-python-development-0.0.32/ecv_python_development/helpers/files/file.py
+drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-04-24 12:20:04.236152 ecv-python-development-0.0.32/ecv_python_development/helpers/formatter/
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      576 2024-04-22 17:32:49.000000 ecv-python-development-0.0.32/ecv_python_development/helpers/formatter/__init__.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     2658 2024-04-22 17:32:49.000000 ecv-python-development-0.0.32/ecv_python_development/helpers/formatter/formatter.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      149 2024-04-22 17:32:49.000000 ecv-python-development-0.0.32/ecv_python_development/helpers/formatter/regex.py
+drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-04-24 12:20:04.236152 ecv-python-development-0.0.32/ecv_python_development/helpers/http/
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      111 2024-04-22 17:32:49.000000 ecv-python-development-0.0.32/ecv_python_development/helpers/http/__init__.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      729 2024-04-22 17:32:49.000000 ecv-python-development-0.0.32/ecv_python_development/helpers/http/requests.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-04-22 17:32:49.000000 ecv-python-development-0.0.32/ecv_python_development/helpers/py.typed
+drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-04-24 12:20:04.236152 ecv-python-development-0.0.32/ecv_python_development/helpers/strings/
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      123 2024-04-22 17:32:49.000000 ecv-python-development-0.0.32/ecv_python_development/helpers/strings/__init__.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      932 2024-04-22 17:32:49.000000 ecv-python-development-0.0.32/ecv_python_development/helpers/strings/passwords.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)       71 2024-04-22 17:32:49.000000 ecv-python-development-0.0.32/ecv_python_development/helpers/strings/uuid.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-04-22 17:32:49.000000 ecv-python-development-0.0.32/ecv_python_development/py.typed
+drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-04-24 12:20:04.216152 ecv-python-development-0.0.32/ecv_python_development.egg-info/
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      698 2024-04-24 12:20:03.000000 ecv-python-development-0.0.32/ecv_python_development.egg-info/PKG-INFO
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     3025 2024-04-24 12:20:03.000000 ecv-python-development-0.0.32/ecv_python_development.egg-info/SOURCES.txt
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)        1 2024-04-24 12:20:03.000000 ecv-python-development-0.0.32/ecv_python_development.egg-info/dependency_links.txt
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      592 2024-04-24 12:20:03.000000 ecv-python-development-0.0.32/ecv_python_development.egg-info/requires.txt
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)       23 2024-04-24 12:20:03.000000 ecv-python-development-0.0.32/ecv_python_development.egg-info/top_level.txt
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)       38 2024-04-24 12:20:04.236152 ecv-python-development-0.0.32/setup.cfg
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     1708 2024-04-24 12:19:55.000000 ecv-python-development-0.0.32/setup.py
```

### Comparing `ecv-python-development-0.0.31/LICENSE` & `ecv-python-development-0.0.32/LICENSE`

 * *Files identical despite different names*

### Comparing `ecv-python-development-0.0.31/PKG-INFO` & `ecv-python-development-0.0.32/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecv-python-development
-Version: 0.0.31
+Version: 0.0.32
 Summary: ECV Python Development Package
 Home-page: https://git-codecommit.ap-southeast-1.amazonaws.com/v1/repos/ecv-python-development
 Author: Warren Ezra Bruce Jaudian
 Author-email: warren.jaudian@ecloudvalley.com
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3.9
```

### Comparing `ecv-python-development-0.0.31/ecv_python_development/aws_cloud_native/events_module/base.py` & `ecv-python-development-0.0.32/ecv_python_development/aws_cloud_native/events_module/base.py`

 * *Files identical despite different names*

### Comparing `ecv-python-development-0.0.31/ecv_python_development/aws_cloud_native/lambda_module/__init__.py` & `ecv-python-development-0.0.32/ecv_python_development/aws_cloud_native/lambda_module/__init__.py`

 * *Files identical despite different names*

### Comparing `ecv-python-development-0.0.31/ecv_python_development/aws_cloud_native/lambda_module/exceptions.py` & `ecv-python-development-0.0.32/ecv_python_development/aws_cloud_native/lambda_module/exceptions.py`

 * *Files identical despite different names*

### Comparing `ecv-python-development-0.0.31/ecv_python_development/aws_cloud_native/lambda_module/handler.py` & `ecv-python-development-0.0.32/ecv_python_development/aws_cloud_native/lambda_module/handler.py`

 * *Files identical despite different names*

### Comparing `ecv-python-development-0.0.31/ecv_python_development/aws_cloud_native/lambda_module/response.py` & `ecv-python-development-0.0.32/ecv_python_development/aws_cloud_native/lambda_module/response.py`

 * *Files identical despite different names*

### Comparing `ecv-python-development-0.0.31/ecv_python_development/aws_cloud_native/lambda_module/validator.py` & `ecv-python-development-0.0.32/ecv_python_development/aws_cloud_native/lambda_module/validator.py`

 * *Files identical despite different names*

### Comparing `ecv-python-development-0.0.31/ecv_python_development/aws_cloud_native/services/aws_service.py` & `ecv-python-development-0.0.32/ecv_python_development/aws_cloud_native/services/aws_service.py`

 * *Files identical despite different names*

### Comparing `ecv-python-development-0.0.31/ecv_python_development/aws_cloud_native/services/cognito_service.py` & `ecv-python-development-0.0.32/ecv_python_development/aws_cloud_native/services/cognito_service.py`

 * *Files identical despite different names*

### Comparing `ecv-python-development-0.0.31/ecv_python_development/aws_cloud_native/services/dynamodb_service.py` & `ecv-python-development-0.0.32/ecv_python_development/aws_cloud_native/services/dynamodb_service.py`

 * *Files identical despite different names*

### Comparing `ecv-python-development-0.0.31/ecv_python_development/aws_cloud_native/services/eventbridge_service.py` & `ecv-python-development-0.0.32/ecv_python_development/aws_cloud_native/services/eventbridge_service.py`

 * *Files identical despite different names*

### Comparing `ecv-python-development-0.0.31/ecv_python_development/aws_cloud_native/services/kms_service.py` & `ecv-python-development-0.0.32/ecv_python_development/aws_cloud_native/services/kms_service.py`

 * *Files identical despite different names*

### Comparing `ecv-python-development-0.0.31/ecv_python_development/aws_cloud_native/services/lambda_service.py` & `ecv-python-development-0.0.32/ecv_python_development/aws_cloud_native/services/lambda_service.py`

 * *Files identical despite different names*

### Comparing `ecv-python-development-0.0.31/ecv_python_development/aws_cloud_native/services/s3_service.py` & `ecv-python-development-0.0.32/ecv_python_development/aws_cloud_native/services/s3_service.py`

 * *Files identical despite different names*

### Comparing `ecv-python-development-0.0.31/ecv_python_development/aws_cloud_native/services/secretsmanager_service.py` & `ecv-python-development-0.0.32/ecv_python_development/aws_cloud_native/services/secretsmanager_service.py`

 * *Files identical despite different names*

### Comparing `ecv-python-development-0.0.31/ecv_python_development/aws_cloud_native/services/ses_service.py` & `ecv-python-development-0.0.32/ecv_python_development/aws_cloud_native/services/ses_service.py`

 * *Files identical despite different names*

### Comparing `ecv-python-development-0.0.31/ecv_python_development/aws_cloud_native/services/sns_service.py` & `ecv-python-development-0.0.32/ecv_python_development/aws_cloud_native/services/sns_service.py`

 * *Files identical despite different names*

### Comparing `ecv-python-development-0.0.31/ecv_python_development/aws_cloud_native/services/sqs_service.py` & `ecv-python-development-0.0.32/ecv_python_development/aws_cloud_native/services/sqs_service.py`

 * *Files identical despite different names*

### Comparing `ecv-python-development-0.0.31/ecv_python_development/aws_cloud_native/services/ssm_service.py` & `ecv-python-development-0.0.32/ecv_python_development/aws_cloud_native/services/ssm_service.py`

 * *Files identical despite different names*

### Comparing `ecv-python-development-0.0.31/ecv_python_development/database/base_model.py` & `ecv-python-development-0.0.32/ecv_python_development/database/base_model.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
 import os
-from typing import Any, Callable, List, Literal, Optional, Pattern
+from typing import Any, Callable, ClassVar, List, Literal, Optional, Pattern
 
 from pydantic import BaseModel as PydanticBaseModel
 from pydantic import (
     Field,
     PrivateAttr,
     StrictBool,
     StrictFloat,
@@ -104,31 +104,31 @@
     created_by: str = field(frozen=True)
     updated_at: str = field(
         default_factory=DateTime.get_current_datetime,
         pattern=r"^\d{4}-\d{2}-\d{2} \d{2}:\d{2}:\d{2}$",
     )
     updated_by: str = field()
 
+    database_model: ClassVar[PynamoDBBaseModel]
+
     def __init__(
         self,
-        db_type: Literal["dynamodb", "rds", "mongodb", "temporary"] = "dynamodb",
+        db_type: Literal["dynamodb", "rds", "mongodb"] = "dynamodb",
         table_name: Optional[str] = os.environ.get("METADATA_TABLE", None),
         **data,
-    ):
+    ) -> None:
         super().__init__(**data)
 
         if db_type == "dynamodb":
-            self.__PynamoDBModel__: PynamoDBBaseModel = None
-        elif db_type == "temporary":
-            pass
+            self.__class__.set_pynamodb_model()
         else:
             raise Exception("Other database not yet supported")
 
     @classmethod
-    def get_pynamodb_model(cls, table_name: Optional[str] = None):
+    def set_pynamodb_model(cls, table_name: Optional[str] = None):
         attributes: dict = {}
 
         for field_name, field_info in cls.model_fields.items():
 
             metadata = field_info.json_schema_extra["json_extra_schema"]
             if "__hash_key__" in metadata or "__range_key__" in metadata:
                 if metadata.get("__hash_key__", False):
@@ -140,22 +140,20 @@
                     field_info.annotation, UnicodeAttribute
                 )(null=field_info.exclude)
 
         model_name = f"{cls.__name__}PynamoDBModel"
         PynamoDBBaseModel.Meta.table_name = table_name
         PynamoDBModel = type(model_name, (PynamoDBBaseModel,), attributes)
 
-        cls.__PynamoDBModel__ = PynamoDBModel
-
-        return PynamoDBModel
+        cls.database_model = PynamoDBModel
 
     def to_pynamodb_model(
         self, include: Optional[list | str] = "all", exclude: Optional[list] = []
-    ) -> PynamoDBBaseModel:
-        return self.__PynamoDBModel__(
+    ) -> type[PynamoDBBaseModel]:
+        return self.database_model(
             **self.model_serialize(
                 include=include,
                 exclude=exclude,
                 serialization_alias=False,
             )
         )
 
@@ -170,15 +168,15 @@
             exclude=set(exclude),
             by_alias=serialization_alias,
         )
 
     @classmethod
     def transform(
         cls, include: Optional[list | str] = "all", exclude: Optional[list] = []
-    ) -> BaseModel:
+    ) -> type[BaseModel]:
         base_fields = {}
 
         for field_name, field_info in cls.model_fields.items():
             if include == "all":
                 base_fields = {**cls.model_fields}
                 break
```

### Comparing `ecv-python-development-0.0.31/ecv_python_development/database/test.py` & `ecv-python-development-0.0.32/ecv_python_development/database/test.py`

 * *Files 24% similar despite different names*

```diff
@@ -16,21 +16,20 @@
     "datetime": "2012-12-01 02:01:02",
     "check": "1",
     "created_by": "a",
     "updated_by": "a",
     "non_defined": "test",
 }
 
-pynamodb_m = UserModel.get_pynamodb_model()
-print(pynamodb_m)
 temp_model = UserModel.transform(include=["username"])
 temp = temp_model(database="dynamodb", table_name="test", **user_data)
 print(temp)
-print(temp.get_pynamodb_model())
+print(temp.database_model.get_attributes())
 pydantic_user = UserModel(database="dynamodb", table_name="test", **user_data)
 print(pydantic_user)
+print(pydantic_user.database_model.get_attributes())
 pynamo_db_model = pydantic_user.to_pynamodb_model()
 print(pynamo_db_model.serialize())
 print(pydantic_user.model_serialize())
 print(temp.model_serialize())
 
 pydantic_user.test_frozen = "new"
```

### Comparing `ecv-python-development-0.0.31/ecv_python_development/helpers/datetime/standard.py` & `ecv-python-development-0.0.32/ecv_python_development/helpers/datetime/standard.py`

 * *Files identical despite different names*

### Comparing `ecv-python-development-0.0.31/ecv_python_development/helpers/formatter/__init__.py` & `ecv-python-development-0.0.32/ecv_python_development/helpers/formatter/__init__.py`

 * *Files identical despite different names*

### Comparing `ecv-python-development-0.0.31/ecv_python_development/helpers/formatter/formatter.py` & `ecv-python-development-0.0.32/ecv_python_development/helpers/formatter/formatter.py`

 * *Files identical despite different names*

### Comparing `ecv-python-development-0.0.31/ecv_python_development/helpers/http/requests.py` & `ecv-python-development-0.0.32/ecv_python_development/helpers/http/requests.py`

 * *Files identical despite different names*

### Comparing `ecv-python-development-0.0.31/ecv_python_development/helpers/strings/passwords.py` & `ecv-python-development-0.0.32/ecv_python_development/helpers/strings/passwords.py`

 * *Files identical despite different names*

### Comparing `ecv-python-development-0.0.31/ecv_python_development.egg-info/PKG-INFO` & `ecv-python-development-0.0.32/ecv_python_development.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecv-python-development
-Version: 0.0.31
+Version: 0.0.32
 Summary: ECV Python Development Package
 Home-page: https://git-codecommit.ap-southeast-1.amazonaws.com/v1/repos/ecv-python-development
 Author: Warren Ezra Bruce Jaudian
 Author-email: warren.jaudian@ecloudvalley.com
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3.9
```

### Comparing `ecv-python-development-0.0.31/ecv_python_development.egg-info/SOURCES.txt` & `ecv-python-development-0.0.32/ecv_python_development.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ecv-python-development-0.0.31/ecv_python_development.egg-info/requires.txt` & `ecv-python-development-0.0.32/ecv_python_development.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `ecv-python-development-0.0.31/setup.py` & `ecv-python-development-0.0.32/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as fh:
     description = fh.read()
 
 setup(
     name="ecv-python-development",
-    version="0.0.31",
+    version="0.0.32",
     author="Warren Ezra Bruce Jaudian",
     author_email="warren.jaudian@ecloudvalley.com",
     packages=find_packages(),
     description="ECV Python Development Package",
     long_description=description,
     long_description_content_type="text/markdown",
     url="https://git-codecommit.ap-southeast-1.amazonaws.com/v1/repos/ecv-python-development",
```


# Comparing `tmp/boto3-stubs-1.34.9.tar.gz` & `tmp/boto3_stubs-1.34.90.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "boto3-stubs-1.34.9.tar", last modified: Wed Dec 27 20:32:15 2023, max compression
+gzip compressed data, was "boto3_stubs-1.34.90.tar", last modified: Tue Apr 23 19:34:17 2024, max compression
```

## Comparing `boto3-stubs-1.34.9.tar` & `boto3_stubs-1.34.90.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 20:32:15.743775 boto3-stubs-1.34.9/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-27 20:31:56.000000 boto3-stubs-1.34.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    80681 2023-12-27 20:32:15.743775 boto3-stubs-1.34.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    68428 2023-12-27 20:31:56.000000 boto3-stubs-1.34.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 20:32:15.739776 boto3-stubs-1.34.9/boto3-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)   202084 2023-12-27 20:32:03.000000 boto3-stubs-1.34.9/boto3-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      151 2023-12-27 20:31:56.000000 boto3-stubs-1.34.9/boto3-stubs/compat.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      839 2023-12-27 20:31:56.000000 boto3-stubs-1.34.9/boto3-stubs/crt.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 20:32:15.739776 boto3-stubs-1.34.9/boto3-stubs/docs/
--rw-r--r--   0 runner    (1001) docker     (127)       99 2023-12-27 20:31:56.000000 boto3-stubs-1.34.9/boto3-stubs/docs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      934 2023-12-27 20:31:56.000000 boto3-stubs-1.34.9/boto3-stubs/docs/utils.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 20:32:15.739776 boto3-stubs-1.34.9/boto3-stubs/dynamodb/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-27 20:31:56.000000 boto3-stubs-1.34.9/boto3-stubs/dynamodb/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5463 2023-12-27 20:31:56.000000 boto3-stubs-1.34.9/boto3-stubs/dynamodb/conditions.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      995 2023-12-27 20:31:56.000000 boto3-stubs-1.34.9/boto3-stubs/dynamodb/table.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1705 2023-12-27 20:31:56.000000 boto3-stubs-1.34.9/boto3-stubs/dynamodb/transform.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1426 2023-12-27 20:31:56.000000 boto3-stubs-1.34.9/boto3-stubs/dynamodb/types.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 20:32:15.739776 boto3-stubs-1.34.9/boto3-stubs/ec2/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-27 20:31:56.000000 boto3-stubs-1.34.9/boto3-stubs/ec2/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      235 2023-12-27 20:31:56.000000 boto3-stubs-1.34.9/boto3-stubs/ec2/createtags.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      204 2023-12-27 20:31:56.000000 boto3-stubs-1.34.9/boto3-stubs/ec2/deletetags.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2023-12-27 20:31:56.000000 boto3-stubs-1.34.9/boto3-stubs/exceptions.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-27 20:32:03.000000 boto3-stubs-1.34.9/boto3-stubs/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 20:32:15.739776 boto3-stubs-1.34.9/boto3-stubs/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-27 20:31:56.000000 boto3-stubs-1.34.9/boto3-stubs/resources/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1546 2023-12-27 20:31:56.000000 boto3-stubs-1.34.9/boto3-stubs/resources/action.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2023-12-27 20:31:56.000000 boto3-stubs-1.34.9/boto3-stubs/resources/base.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1922 2023-12-27 20:31:56.000000 boto3-stubs-1.34.9/boto3-stubs/resources/collection.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      496 2023-12-27 20:31:56.000000 boto3-stubs-1.34.9/boto3-stubs/resources/factory.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3703 2023-12-27 20:31:56.000000 boto3-stubs-1.34.9/boto3-stubs/resources/model.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      565 2023-12-27 20:31:56.000000 boto3-stubs-1.34.9/boto3-stubs/resources/params.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1607 2023-12-27 20:31:56.000000 boto3-stubs-1.34.9/boto3-stubs/resources/response.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 20:32:15.739776 boto3-stubs-1.34.9/boto3-stubs/s3/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-27 20:31:56.000000 boto3-stubs-1.34.9/boto3-stubs/s3/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       75 2023-12-27 20:31:56.000000 boto3-stubs-1.34.9/boto3-stubs/s3/constants.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4577 2023-12-27 20:31:56.000000 boto3-stubs-1.34.9/boto3-stubs/s3/inject.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2508 2023-12-27 20:31:56.000000 boto3-stubs-1.34.9/boto3-stubs/s3/transfer.pyi
--rw-r--r--   0 runner    (1001) docker     (127)   228670 2023-12-27 20:31:59.000000 boto3-stubs-1.34.9/boto3-stubs/session.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      779 2023-12-27 20:31:56.000000 boto3-stubs-1.34.9/boto3-stubs/utils.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 20:32:15.739776 boto3-stubs-1.34.9/boto3_stubs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    80681 2023-12-27 20:32:15.000000 boto3-stubs-1.34.9/boto3_stubs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2023-12-27 20:32:15.000000 boto3-stubs-1.34.9/boto3_stubs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-27 20:32:15.000000 boto3-stubs-1.34.9/boto3_stubs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-27 20:32:15.000000 boto3-stubs-1.34.9/boto3_stubs.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)    35996 2023-12-27 20:32:15.000000 boto3-stubs-1.34.9/boto3_stubs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2023-12-27 20:32:15.000000 boto3-stubs-1.34.9/boto3_stubs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-27 20:32:15.743775 boto3-stubs-1.34.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)    49534 2023-12-27 20:31:56.000000 boto3-stubs-1.34.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:34:17.640536 boto3_stubs-1.34.90/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-23 19:32:57.000000 boto3_stubs-1.34.90/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)   140009 2024-04-23 19:34:17.640536 boto3_stubs-1.34.90/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    69482 2024-04-23 19:32:57.000000 boto3_stubs-1.34.90/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:34:17.540535 boto3_stubs-1.34.90/boto3-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)   205730 2024-04-23 19:33:01.000000 boto3_stubs-1.34.90/boto3-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-23 19:32:56.000000 boto3_stubs-1.34.90/boto3-stubs/compat.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-04-23 19:32:56.000000 boto3_stubs-1.34.90/boto3-stubs/crt.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:34:17.540535 boto3_stubs-1.34.90/boto3-stubs/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-23 19:32:56.000000 boto3_stubs-1.34.90/boto3-stubs/docs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-23 19:32:56.000000 boto3_stubs-1.34.90/boto3-stubs/docs/utils.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:34:17.540535 boto3_stubs-1.34.90/boto3-stubs/dynamodb/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:32:56.000000 boto3_stubs-1.34.90/boto3-stubs/dynamodb/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5463 2024-04-23 19:32:56.000000 boto3_stubs-1.34.90/boto3-stubs/dynamodb/conditions.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-04-23 19:32:56.000000 boto3_stubs-1.34.90/boto3-stubs/dynamodb/table.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-04-23 19:32:56.000000 boto3_stubs-1.34.90/boto3-stubs/dynamodb/transform.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-04-23 19:32:56.000000 boto3_stubs-1.34.90/boto3-stubs/dynamodb/types.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:34:17.540535 boto3_stubs-1.34.90/boto3-stubs/ec2/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:32:56.000000 boto3_stubs-1.34.90/boto3-stubs/ec2/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-23 19:32:56.000000 boto3_stubs-1.34.90/boto3-stubs/ec2/createtags.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-23 19:32:56.000000 boto3_stubs-1.34.90/boto3-stubs/ec2/deletetags.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-04-23 19:32:56.000000 boto3_stubs-1.34.90/boto3-stubs/exceptions.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:33:01.000000 boto3_stubs-1.34.90/boto3-stubs/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:34:17.540535 boto3_stubs-1.34.90/boto3-stubs/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:32:56.000000 boto3_stubs-1.34.90/boto3-stubs/resources/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-04-23 19:32:56.000000 boto3_stubs-1.34.90/boto3-stubs/resources/action.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-23 19:32:56.000000 boto3_stubs-1.34.90/boto3-stubs/resources/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-04-23 19:32:56.000000 boto3_stubs-1.34.90/boto3-stubs/resources/collection.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-04-23 19:32:56.000000 boto3_stubs-1.34.90/boto3-stubs/resources/factory.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3703 2024-04-23 19:32:56.000000 boto3_stubs-1.34.90/boto3-stubs/resources/model.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-23 19:32:56.000000 boto3_stubs-1.34.90/boto3-stubs/resources/params.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-04-23 19:32:56.000000 boto3_stubs-1.34.90/boto3-stubs/resources/response.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:34:17.540535 boto3_stubs-1.34.90/boto3-stubs/s3/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:32:56.000000 boto3_stubs-1.34.90/boto3-stubs/s3/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-23 19:32:56.000000 boto3_stubs-1.34.90/boto3-stubs/s3/constants.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4577 2024-04-23 19:32:56.000000 boto3_stubs-1.34.90/boto3-stubs/s3/inject.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-04-23 19:32:56.000000 boto3_stubs-1.34.90/boto3-stubs/s3/transfer.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)   232778 2024-04-23 19:33:05.000000 boto3_stubs-1.34.90/boto3-stubs/session.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-04-23 19:32:56.000000 boto3_stubs-1.34.90/boto3-stubs/utils.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:34:17.544535 boto3_stubs-1.34.90/boto3_stubs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)   140009 2024-04-23 19:34:17.000000 boto3_stubs-1.34.90/boto3_stubs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-23 19:34:17.000000 boto3_stubs-1.34.90/boto3_stubs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 19:34:17.000000 boto3_stubs-1.34.90/boto3_stubs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 19:34:17.000000 boto3_stubs-1.34.90/boto3_stubs.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)    36667 2024-04-23 19:34:17.000000 boto3_stubs-1.34.90/boto3_stubs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-23 19:34:17.000000 boto3_stubs-1.34.90/boto3_stubs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 19:34:17.640536 boto3_stubs-1.34.90/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)    50417 2024-04-23 19:32:57.000000 boto3_stubs-1.34.90/setup.py
```

### Comparing `boto3-stubs-1.34.9/LICENSE` & `boto3_stubs-1.34.90/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 Vlad Emelianov
+Copyright (c) 2024 Vlad Emelianov
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `boto3-stubs-1.34.9/PKG-INFO` & `boto3_stubs-1.34.90/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,440 +1,29 @@
-Metadata-Version: 2.1
-Name: boto3-stubs
-Version: 1.34.9
-Summary: Type annotations for boto3 1.34.9 generated with mypy-boto3-builder 7.23.0
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 type-annotations boto3-stubs mypy typeshed autocomplete
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Environment :: Console
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Programming Language :: Python :: 3.13
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Typing :: Stubs Only
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: all
-Provides-Extra: essential
-Provides-Extra: boto3
-Provides-Extra: accessanalyzer
-Provides-Extra: account
-Provides-Extra: acm
-Provides-Extra: acm-pca
-Provides-Extra: alexaforbusiness
-Provides-Extra: amp
-Provides-Extra: amplify
-Provides-Extra: amplifybackend
-Provides-Extra: amplifyuibuilder
-Provides-Extra: apigateway
-Provides-Extra: apigatewaymanagementapi
-Provides-Extra: apigatewayv2
-Provides-Extra: appconfig
-Provides-Extra: appconfigdata
-Provides-Extra: appfabric
-Provides-Extra: appflow
-Provides-Extra: appintegrations
-Provides-Extra: application-autoscaling
-Provides-Extra: application-insights
-Provides-Extra: applicationcostprofiler
-Provides-Extra: appmesh
-Provides-Extra: apprunner
-Provides-Extra: appstream
-Provides-Extra: appsync
-Provides-Extra: arc-zonal-shift
-Provides-Extra: athena
-Provides-Extra: auditmanager
-Provides-Extra: autoscaling
-Provides-Extra: autoscaling-plans
-Provides-Extra: b2bi
-Provides-Extra: backup
-Provides-Extra: backup-gateway
-Provides-Extra: backupstorage
-Provides-Extra: batch
-Provides-Extra: bcm-data-exports
-Provides-Extra: bedrock
-Provides-Extra: bedrock-agent
-Provides-Extra: bedrock-agent-runtime
-Provides-Extra: bedrock-runtime
-Provides-Extra: billingconductor
-Provides-Extra: braket
-Provides-Extra: budgets
-Provides-Extra: ce
-Provides-Extra: chime
-Provides-Extra: chime-sdk-identity
-Provides-Extra: chime-sdk-media-pipelines
-Provides-Extra: chime-sdk-meetings
-Provides-Extra: chime-sdk-messaging
-Provides-Extra: chime-sdk-voice
-Provides-Extra: cleanrooms
-Provides-Extra: cleanroomsml
-Provides-Extra: cloud9
-Provides-Extra: cloudcontrol
-Provides-Extra: clouddirectory
-Provides-Extra: cloudformation
-Provides-Extra: cloudfront
-Provides-Extra: cloudfront-keyvaluestore
-Provides-Extra: cloudhsm
-Provides-Extra: cloudhsmv2
-Provides-Extra: cloudsearch
-Provides-Extra: cloudsearchdomain
-Provides-Extra: cloudtrail
-Provides-Extra: cloudtrail-data
-Provides-Extra: cloudwatch
-Provides-Extra: codeartifact
-Provides-Extra: codebuild
-Provides-Extra: codecatalyst
-Provides-Extra: codecommit
-Provides-Extra: codedeploy
-Provides-Extra: codeguru-reviewer
-Provides-Extra: codeguru-security
-Provides-Extra: codeguruprofiler
-Provides-Extra: codepipeline
-Provides-Extra: codestar
-Provides-Extra: codestar-connections
-Provides-Extra: codestar-notifications
-Provides-Extra: cognito-identity
-Provides-Extra: cognito-idp
-Provides-Extra: cognito-sync
-Provides-Extra: comprehend
-Provides-Extra: comprehendmedical
-Provides-Extra: compute-optimizer
-Provides-Extra: config
-Provides-Extra: connect
-Provides-Extra: connect-contact-lens
-Provides-Extra: connectcampaigns
-Provides-Extra: connectcases
-Provides-Extra: connectparticipant
-Provides-Extra: controltower
-Provides-Extra: cost-optimization-hub
-Provides-Extra: cur
-Provides-Extra: customer-profiles
-Provides-Extra: databrew
-Provides-Extra: dataexchange
-Provides-Extra: datapipeline
-Provides-Extra: datasync
-Provides-Extra: datazone
-Provides-Extra: dax
-Provides-Extra: detective
-Provides-Extra: devicefarm
-Provides-Extra: devops-guru
-Provides-Extra: directconnect
-Provides-Extra: discovery
-Provides-Extra: dlm
-Provides-Extra: dms
-Provides-Extra: docdb
-Provides-Extra: docdb-elastic
-Provides-Extra: drs
-Provides-Extra: ds
-Provides-Extra: dynamodb
-Provides-Extra: dynamodbstreams
-Provides-Extra: ebs
-Provides-Extra: ec2
-Provides-Extra: ec2-instance-connect
-Provides-Extra: ecr
-Provides-Extra: ecr-public
-Provides-Extra: ecs
-Provides-Extra: efs
-Provides-Extra: eks
-Provides-Extra: eks-auth
-Provides-Extra: elastic-inference
-Provides-Extra: elasticache
-Provides-Extra: elasticbeanstalk
-Provides-Extra: elastictranscoder
-Provides-Extra: elb
-Provides-Extra: elbv2
-Provides-Extra: emr
-Provides-Extra: emr-containers
-Provides-Extra: emr-serverless
-Provides-Extra: entityresolution
-Provides-Extra: es
-Provides-Extra: events
-Provides-Extra: evidently
-Provides-Extra: finspace
-Provides-Extra: finspace-data
-Provides-Extra: firehose
-Provides-Extra: fis
-Provides-Extra: fms
-Provides-Extra: forecast
-Provides-Extra: forecastquery
-Provides-Extra: frauddetector
-Provides-Extra: freetier
-Provides-Extra: fsx
-Provides-Extra: gamelift
-Provides-Extra: glacier
-Provides-Extra: globalaccelerator
-Provides-Extra: glue
-Provides-Extra: grafana
-Provides-Extra: greengrass
-Provides-Extra: greengrassv2
-Provides-Extra: groundstation
-Provides-Extra: guardduty
-Provides-Extra: health
-Provides-Extra: healthlake
-Provides-Extra: honeycode
-Provides-Extra: iam
-Provides-Extra: identitystore
-Provides-Extra: imagebuilder
-Provides-Extra: importexport
-Provides-Extra: inspector
-Provides-Extra: inspector-scan
-Provides-Extra: inspector2
-Provides-Extra: internetmonitor
-Provides-Extra: iot
-Provides-Extra: iot-data
-Provides-Extra: iot-jobs-data
-Provides-Extra: iot-roborunner
-Provides-Extra: iot1click-devices
-Provides-Extra: iot1click-projects
-Provides-Extra: iotanalytics
-Provides-Extra: iotdeviceadvisor
-Provides-Extra: iotevents
-Provides-Extra: iotevents-data
-Provides-Extra: iotfleethub
-Provides-Extra: iotfleetwise
-Provides-Extra: iotsecuretunneling
-Provides-Extra: iotsitewise
-Provides-Extra: iotthingsgraph
-Provides-Extra: iottwinmaker
-Provides-Extra: iotwireless
-Provides-Extra: ivs
-Provides-Extra: ivs-realtime
-Provides-Extra: ivschat
-Provides-Extra: kafka
-Provides-Extra: kafkaconnect
-Provides-Extra: kendra
-Provides-Extra: kendra-ranking
-Provides-Extra: keyspaces
-Provides-Extra: kinesis
-Provides-Extra: kinesis-video-archived-media
-Provides-Extra: kinesis-video-media
-Provides-Extra: kinesis-video-signaling
-Provides-Extra: kinesis-video-webrtc-storage
-Provides-Extra: kinesisanalytics
-Provides-Extra: kinesisanalyticsv2
-Provides-Extra: kinesisvideo
-Provides-Extra: kms
-Provides-Extra: lakeformation
-Provides-Extra: lambda
-Provides-Extra: launch-wizard
-Provides-Extra: lex-models
-Provides-Extra: lex-runtime
-Provides-Extra: lexv2-models
-Provides-Extra: lexv2-runtime
-Provides-Extra: license-manager
-Provides-Extra: license-manager-linux-subscriptions
-Provides-Extra: license-manager-user-subscriptions
-Provides-Extra: lightsail
-Provides-Extra: location
-Provides-Extra: logs
-Provides-Extra: lookoutequipment
-Provides-Extra: lookoutmetrics
-Provides-Extra: lookoutvision
-Provides-Extra: m2
-Provides-Extra: machinelearning
-Provides-Extra: macie2
-Provides-Extra: managedblockchain
-Provides-Extra: managedblockchain-query
-Provides-Extra: marketplace-agreement
-Provides-Extra: marketplace-catalog
-Provides-Extra: marketplace-deployment
-Provides-Extra: marketplace-entitlement
-Provides-Extra: marketplacecommerceanalytics
-Provides-Extra: mediaconnect
-Provides-Extra: mediaconvert
-Provides-Extra: medialive
-Provides-Extra: mediapackage
-Provides-Extra: mediapackage-vod
-Provides-Extra: mediapackagev2
-Provides-Extra: mediastore
-Provides-Extra: mediastore-data
-Provides-Extra: mediatailor
-Provides-Extra: medical-imaging
-Provides-Extra: memorydb
-Provides-Extra: meteringmarketplace
-Provides-Extra: mgh
-Provides-Extra: mgn
-Provides-Extra: migration-hub-refactor-spaces
-Provides-Extra: migrationhub-config
-Provides-Extra: migrationhuborchestrator
-Provides-Extra: migrationhubstrategy
-Provides-Extra: mobile
-Provides-Extra: mq
-Provides-Extra: mturk
-Provides-Extra: mwaa
-Provides-Extra: neptune
-Provides-Extra: neptune-graph
-Provides-Extra: neptunedata
-Provides-Extra: network-firewall
-Provides-Extra: networkmanager
-Provides-Extra: networkmonitor
-Provides-Extra: nimble
-Provides-Extra: oam
-Provides-Extra: omics
-Provides-Extra: opensearch
-Provides-Extra: opensearchserverless
-Provides-Extra: opsworks
-Provides-Extra: opsworkscm
-Provides-Extra: organizations
-Provides-Extra: osis
-Provides-Extra: outposts
-Provides-Extra: panorama
-Provides-Extra: payment-cryptography
-Provides-Extra: payment-cryptography-data
-Provides-Extra: pca-connector-ad
-Provides-Extra: personalize
-Provides-Extra: personalize-events
-Provides-Extra: personalize-runtime
-Provides-Extra: pi
-Provides-Extra: pinpoint
-Provides-Extra: pinpoint-email
-Provides-Extra: pinpoint-sms-voice
-Provides-Extra: pinpoint-sms-voice-v2
-Provides-Extra: pipes
-Provides-Extra: polly
-Provides-Extra: pricing
-Provides-Extra: privatenetworks
-Provides-Extra: proton
-Provides-Extra: qbusiness
-Provides-Extra: qconnect
-Provides-Extra: qldb
-Provides-Extra: qldb-session
-Provides-Extra: quicksight
-Provides-Extra: ram
-Provides-Extra: rbin
-Provides-Extra: rds
-Provides-Extra: rds-data
-Provides-Extra: redshift
-Provides-Extra: redshift-data
-Provides-Extra: redshift-serverless
-Provides-Extra: rekognition
-Provides-Extra: repostspace
-Provides-Extra: resiliencehub
-Provides-Extra: resource-explorer-2
-Provides-Extra: resource-groups
-Provides-Extra: resourcegroupstaggingapi
-Provides-Extra: robomaker
-Provides-Extra: rolesanywhere
-Provides-Extra: route53
-Provides-Extra: route53-recovery-cluster
-Provides-Extra: route53-recovery-control-config
-Provides-Extra: route53-recovery-readiness
-Provides-Extra: route53domains
-Provides-Extra: route53resolver
-Provides-Extra: rum
-Provides-Extra: s3
-Provides-Extra: s3control
-Provides-Extra: s3outposts
-Provides-Extra: sagemaker
-Provides-Extra: sagemaker-a2i-runtime
-Provides-Extra: sagemaker-edge
-Provides-Extra: sagemaker-featurestore-runtime
-Provides-Extra: sagemaker-geospatial
-Provides-Extra: sagemaker-metrics
-Provides-Extra: sagemaker-runtime
-Provides-Extra: savingsplans
-Provides-Extra: scheduler
-Provides-Extra: schemas
-Provides-Extra: sdb
-Provides-Extra: secretsmanager
-Provides-Extra: securityhub
-Provides-Extra: securitylake
-Provides-Extra: serverlessrepo
-Provides-Extra: service-quotas
-Provides-Extra: servicecatalog
-Provides-Extra: servicecatalog-appregistry
-Provides-Extra: servicediscovery
-Provides-Extra: ses
-Provides-Extra: sesv2
-Provides-Extra: shield
-Provides-Extra: signer
-Provides-Extra: simspaceweaver
-Provides-Extra: sms
-Provides-Extra: sms-voice
-Provides-Extra: snow-device-management
-Provides-Extra: snowball
-Provides-Extra: sns
-Provides-Extra: sqs
-Provides-Extra: ssm
-Provides-Extra: ssm-contacts
-Provides-Extra: ssm-incidents
-Provides-Extra: ssm-sap
-Provides-Extra: sso
-Provides-Extra: sso-admin
-Provides-Extra: sso-oidc
-Provides-Extra: stepfunctions
-Provides-Extra: storagegateway
-Provides-Extra: sts
-Provides-Extra: support
-Provides-Extra: support-app
-Provides-Extra: swf
-Provides-Extra: synthetics
-Provides-Extra: textract
-Provides-Extra: timestream-query
-Provides-Extra: timestream-write
-Provides-Extra: tnb
-Provides-Extra: transcribe
-Provides-Extra: transfer
-Provides-Extra: translate
-Provides-Extra: trustedadvisor
-Provides-Extra: verifiedpermissions
-Provides-Extra: voice-id
-Provides-Extra: vpc-lattice
-Provides-Extra: waf
-Provides-Extra: waf-regional
-Provides-Extra: wafv2
-Provides-Extra: wellarchitected
-Provides-Extra: wisdom
-Provides-Extra: workdocs
-Provides-Extra: worklink
-Provides-Extra: workmail
-Provides-Extra: workmailmessageflow
-Provides-Extra: workspaces
-Provides-Extra: workspaces-thin-client
-Provides-Extra: workspaces-web
-Provides-Extra: xray
-License-File: LICENSE
-
 <a id="boto3-stubs"></a>
 
 # boto3-stubs
 
 [![PyPI - boto3-stubs](https://img.shields.io/pypi/v/boto3-stubs.svg?color=blue)](https://pypi.org/project/boto3-stubs)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/boto3-stubs.svg?color=blue)](https://pypi.org/project/boto3-stubs)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/boto3-stubs)](https://pepy.tech/project/boto3-stubs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3 1.34.9](https://boto3.amazonaws.com/v1/documentation/api/1.34.9/index.html)
+[boto3 1.34.90](https://boto3.amazonaws.com/v1/documentation/api/1.34.90/index.html)
 compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.23.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found in
 [boto3-stubs docs](https://youtype.github.io/boto3_stubs_docs/).
 
 See how it helps to find and fix potential bugs:
 
 ![boto3-stubs demo](https://github.com/youtype/mypy_boto3_builder/raw/main/demo.gif)
@@ -799,15 +388,15 @@
 in [mypy-boto3-builder](https://github.com/youtype/mypy_boto3_builder/issues/)
 repository.
 
 <a id="submodules"></a>
 
 ## Submodules
 
-- `boto3-stubs[all]` - Type annotations for all 376 services.
+- `boto3-stubs[all]` - Type annotations for all 383 services.
 - `boto3-stubs[essential]` - Type annotations for
   [CloudFormation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/),
   [DynamoDB](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/),
   [EC2](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/),
   [Lambda](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/),
   [RDS](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rds/),
   [S3](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/) and
@@ -883,14 +472,17 @@
   service.
 - `boto3-stubs[appsync]` - Type annotations for
   [AppSync](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appsync/)
   service.
 - `boto3-stubs[arc-zonal-shift]` - Type annotations for
   [ARCZonalShift](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_arc_zonal_shift/)
   service.
+- `boto3-stubs[artifact]` - Type annotations for
+  [Artifact](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_artifact/)
+  service.
 - `boto3-stubs[athena]` - Type annotations for
   [Athena](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/)
   service.
 - `boto3-stubs[auditmanager]` - Type annotations for
   [AuditManager](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_auditmanager/)
   service.
 - `boto3-stubs[autoscaling]` - Type annotations for
@@ -936,14 +528,17 @@
   service.
 - `boto3-stubs[budgets]` - Type annotations for
   [Budgets](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/)
   service.
 - `boto3-stubs[ce]` - Type annotations for
   [CostExplorer](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/)
   service.
+- `boto3-stubs[chatbot]` - Type annotations for
+  [Chatbot](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chatbot/)
+  service.
 - `boto3-stubs[chime]` - Type annotations for
   [Chime](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime/)
   service.
 - `boto3-stubs[chime-sdk-identity]` - Type annotations for
   [ChimeSDKIdentity](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_identity/)
   service.
 - `boto3-stubs[chime-sdk-media-pipelines]` - Type annotations for
@@ -1011,14 +606,17 @@
   service.
 - `boto3-stubs[codecatalyst]` - Type annotations for
   [CodeCatalyst](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/)
   service.
 - `boto3-stubs[codecommit]` - Type annotations for
   [CodeCommit](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecommit/)
   service.
+- `boto3-stubs[codeconnections]` - Type annotations for
+  [CodeConnections](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeconnections/)
+  service.
 - `boto3-stubs[codedeploy]` - Type annotations for
   [CodeDeploy](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codedeploy/)
   service.
 - `boto3-stubs[codeguru-reviewer]` - Type annotations for
   [CodeGuruReviewer](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguru_reviewer/)
   service.
 - `boto3-stubs[codeguru-security]` - Type annotations for
@@ -1071,14 +669,17 @@
   service.
 - `boto3-stubs[connectcases]` - Type annotations for
   [ConnectCases](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/)
   service.
 - `boto3-stubs[connectparticipant]` - Type annotations for
   [ConnectParticipant](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectparticipant/)
   service.
+- `boto3-stubs[controlcatalog]` - Type annotations for
+  [ControlCatalog](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_controlcatalog/)
+  service.
 - `boto3-stubs[controltower]` - Type annotations for
   [ControlTower](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_controltower/)
   service.
 - `boto3-stubs[cost-optimization-hub]` - Type annotations for
   [CostOptimizationHub](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cost_optimization_hub/)
   service.
 - `boto3-stubs[cur]` - Type annotations for
@@ -1100,14 +701,17 @@
   [DataSync](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/)
   service.
 - `boto3-stubs[datazone]` - Type annotations for
   [DataZone](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datazone/)
   service.
 - `boto3-stubs[dax]` - Type annotations for
   [DAX](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dax/) service.
+- `boto3-stubs[deadline]` - Type annotations for
+  [DeadlineCloud](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_deadline/)
+  service.
 - `boto3-stubs[detective]` - Type annotations for
   [Detective](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_detective/)
   service.
 - `boto3-stubs[devicefarm]` - Type annotations for
   [DeviceFarm](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/)
   service.
 - `boto3-stubs[devops-guru]` - Type annotations for
@@ -1289,17 +893,14 @@
   [IoT](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/) service.
 - `boto3-stubs[iot-data]` - Type annotations for
   [IoTDataPlane](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot_data/)
   service.
 - `boto3-stubs[iot-jobs-data]` - Type annotations for
   [IoTJobsDataPlane](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot_jobs_data/)
   service.
-- `boto3-stubs[iot-roborunner]` - Type annotations for
-  [IoTRoboRunner](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot_roborunner/)
-  service.
 - `boto3-stubs[iot1click-devices]` - Type annotations for
   [IoT1ClickDevicesService](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot1click_devices/)
   service.
 - `boto3-stubs[iot1click-projects]` - Type annotations for
   [IoT1ClickProjects](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot1click_projects/)
   service.
 - `boto3-stubs[iotanalytics]` - Type annotations for
@@ -1691,14 +1292,17 @@
   service.
 - `boto3-stubs[route53-recovery-readiness]` - Type annotations for
   [Route53RecoveryReadiness](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_readiness/)
   service.
 - `boto3-stubs[route53domains]` - Type annotations for
   [Route53Domains](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/)
   service.
+- `boto3-stubs[route53profiles]` - Type annotations for
+  [Route53Profiles](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53profiles/)
+  service.
 - `boto3-stubs[route53resolver]` - Type annotations for
   [Route53Resolver](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/)
   service.
 - `boto3-stubs[rum]` - Type annotations for
   [CloudWatchRUM](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rum/)
   service.
 - `boto3-stubs[s3]` - Type annotations for
@@ -1818,28 +1422,34 @@
   [SFN](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/)
   service.
 - `boto3-stubs[storagegateway]` - Type annotations for
   [StorageGateway](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/)
   service.
 - `boto3-stubs[sts]` - Type annotations for
   [STS](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sts/) service.
+- `boto3-stubs[supplychain]` - Type annotations for
+  [SupplyChain](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_supplychain/)
+  service.
 - `boto3-stubs[support]` - Type annotations for
   [Support](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_support/)
   service.
 - `boto3-stubs[support-app]` - Type annotations for
   [SupportApp](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_support_app/)
   service.
 - `boto3-stubs[swf]` - Type annotations for
   [SWF](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_swf/) service.
 - `boto3-stubs[synthetics]` - Type annotations for
   [Synthetics](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_synthetics/)
   service.
 - `boto3-stubs[textract]` - Type annotations for
   [Textract](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_textract/)
   service.
+- `boto3-stubs[timestream-influxdb]` - Type annotations for
+  [TimestreamInfluxDB](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_influxdb/)
+  service.
 - `boto3-stubs[timestream-query]` - Type annotations for
   [TimestreamQuery](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_query/)
   service.
 - `boto3-stubs[timestream-write]` - Type annotations for
   [TimestreamWrite](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_write/)
   service.
 - `boto3-stubs[tnb]` - Type annotations for
```

### Comparing `boto3-stubs-1.34.9/boto3-stubs/__init__.pyi` & `boto3_stubs-1.34.90/boto3-stubs/__init__.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 from mypy_boto3_application_insights.client import ApplicationInsightsClient
 from mypy_boto3_applicationcostprofiler.client import ApplicationCostProfilerClient
 from mypy_boto3_appmesh.client import AppMeshClient
 from mypy_boto3_apprunner.client import AppRunnerClient
 from mypy_boto3_appstream.client import AppStreamClient
 from mypy_boto3_appsync.client import AppSyncClient
 from mypy_boto3_arc_zonal_shift.client import ARCZonalShiftClient
+from mypy_boto3_artifact.client import ArtifactClient
 from mypy_boto3_athena.client import AthenaClient
 from mypy_boto3_auditmanager.client import AuditManagerClient
 from mypy_boto3_autoscaling.client import AutoScalingClient
 from mypy_boto3_autoscaling_plans.client import AutoScalingPlansClient
 from mypy_boto3_b2bi.client import B2BIClient
 from mypy_boto3_backup.client import BackupClient
 from mypy_boto3_backup_gateway.client import BackupGatewayClient
@@ -45,14 +46,15 @@
 from mypy_boto3_bedrock_agent.client import AgentsforBedrockClient
 from mypy_boto3_bedrock_agent_runtime.client import AgentsforBedrockRuntimeClient
 from mypy_boto3_bedrock_runtime.client import BedrockRuntimeClient
 from mypy_boto3_billingconductor.client import BillingConductorClient
 from mypy_boto3_braket.client import BraketClient
 from mypy_boto3_budgets.client import BudgetsClient
 from mypy_boto3_ce.client import CostExplorerClient
+from mypy_boto3_chatbot.client import ChatbotClient
 from mypy_boto3_chime.client import ChimeClient
 from mypy_boto3_chime_sdk_identity.client import ChimeSDKIdentityClient
 from mypy_boto3_chime_sdk_media_pipelines.client import ChimeSDKMediaPipelinesClient
 from mypy_boto3_chime_sdk_meetings.client import ChimeSDKMeetingsClient
 from mypy_boto3_chime_sdk_messaging.client import ChimeSDKMessagingClient
 from mypy_boto3_chime_sdk_voice.client import ChimeSDKVoiceClient
 from mypy_boto3_cleanrooms.client import CleanRoomsServiceClient
@@ -72,14 +74,15 @@
 from mypy_boto3_cloudtrail_data.client import CloudTrailDataServiceClient
 from mypy_boto3_cloudwatch.client import CloudWatchClient
 from mypy_boto3_cloudwatch.service_resource import CloudWatchServiceResource
 from mypy_boto3_codeartifact.client import CodeArtifactClient
 from mypy_boto3_codebuild.client import CodeBuildClient
 from mypy_boto3_codecatalyst.client import CodeCatalystClient
 from mypy_boto3_codecommit.client import CodeCommitClient
+from mypy_boto3_codeconnections.client import CodeConnectionsClient
 from mypy_boto3_codedeploy.client import CodeDeployClient
 from mypy_boto3_codeguru_reviewer.client import CodeGuruReviewerClient
 from mypy_boto3_codeguru_security.client import CodeGuruSecurityClient
 from mypy_boto3_codeguruprofiler.client import CodeGuruProfilerClient
 from mypy_boto3_codepipeline.client import CodePipelineClient
 from mypy_boto3_codestar.client import CodeStarClient
 from mypy_boto3_codestar_connections.client import CodeStarconnectionsClient
@@ -92,24 +95,26 @@
 from mypy_boto3_compute_optimizer.client import ComputeOptimizerClient
 from mypy_boto3_config.client import ConfigServiceClient
 from mypy_boto3_connect.client import ConnectClient
 from mypy_boto3_connect_contact_lens.client import ConnectContactLensClient
 from mypy_boto3_connectcampaigns.client import ConnectCampaignServiceClient
 from mypy_boto3_connectcases.client import ConnectCasesClient
 from mypy_boto3_connectparticipant.client import ConnectParticipantClient
+from mypy_boto3_controlcatalog.client import ControlCatalogClient
 from mypy_boto3_controltower.client import ControlTowerClient
 from mypy_boto3_cost_optimization_hub.client import CostOptimizationHubClient
 from mypy_boto3_cur.client import CostandUsageReportServiceClient
 from mypy_boto3_customer_profiles.client import CustomerProfilesClient
 from mypy_boto3_databrew.client import GlueDataBrewClient
 from mypy_boto3_dataexchange.client import DataExchangeClient
 from mypy_boto3_datapipeline.client import DataPipelineClient
 from mypy_boto3_datasync.client import DataSyncClient
 from mypy_boto3_datazone.client import DataZoneClient
 from mypy_boto3_dax.client import DAXClient
+from mypy_boto3_deadline.client import DeadlineCloudClient
 from mypy_boto3_detective.client import DetectiveClient
 from mypy_boto3_devicefarm.client import DeviceFarmClient
 from mypy_boto3_devops_guru.client import DevOpsGuruClient
 from mypy_boto3_directconnect.client import DirectConnectClient
 from mypy_boto3_discovery.client import ApplicationDiscoveryServiceClient
 from mypy_boto3_dlm.client import DLMClient
 from mypy_boto3_dms.client import DatabaseMigrationServiceClient
@@ -176,15 +181,14 @@
 from mypy_boto3_inspector_scan.client import inspectorscanClient
 from mypy_boto3_internetmonitor.client import CloudWatchInternetMonitorClient
 from mypy_boto3_iot1click_devices.client import IoT1ClickDevicesServiceClient
 from mypy_boto3_iot1click_projects.client import IoT1ClickProjectsClient
 from mypy_boto3_iot.client import IoTClient
 from mypy_boto3_iot_data.client import IoTDataPlaneClient
 from mypy_boto3_iot_jobs_data.client import IoTJobsDataPlaneClient
-from mypy_boto3_iot_roborunner.client import IoTRoboRunnerClient
 from mypy_boto3_iotanalytics.client import IoTAnalyticsClient
 from mypy_boto3_iotdeviceadvisor.client import IoTDeviceAdvisorClient
 from mypy_boto3_iotevents.client import IoTEventsClient
 from mypy_boto3_iotevents_data.client import IoTEventsDataClient
 from mypy_boto3_iotfleethub.client import IoTFleetHubClient
 from mypy_boto3_iotfleetwise.client import IoTFleetWiseClient
 from mypy_boto3_iotsecuretunneling.client import IoTSecureTunnelingClient
@@ -316,14 +320,15 @@
 from mypy_boto3_robomaker.client import RoboMakerClient
 from mypy_boto3_rolesanywhere.client import IAMRolesAnywhereClient
 from mypy_boto3_route53.client import Route53Client
 from mypy_boto3_route53_recovery_cluster.client import Route53RecoveryClusterClient
 from mypy_boto3_route53_recovery_control_config.client import Route53RecoveryControlConfigClient
 from mypy_boto3_route53_recovery_readiness.client import Route53RecoveryReadinessClient
 from mypy_boto3_route53domains.client import Route53DomainsClient
+from mypy_boto3_route53profiles.client import Route53ProfilesClient
 from mypy_boto3_route53resolver.client import Route53ResolverClient
 from mypy_boto3_rum.client import CloudWatchRUMClient
 from mypy_boto3_s3.client import S3Client
 from mypy_boto3_s3.service_resource import S3ServiceResource
 from mypy_boto3_s3control.client import S3ControlClient
 from mypy_boto3_s3outposts.client import S3OutpostsClient
 from mypy_boto3_sagemaker.client import SageMakerClient
@@ -364,19 +369,21 @@
 from mypy_boto3_ssm_sap.client import SsmSapClient
 from mypy_boto3_sso.client import SSOClient
 from mypy_boto3_sso_admin.client import SSOAdminClient
 from mypy_boto3_sso_oidc.client import SSOOIDCClient
 from mypy_boto3_stepfunctions.client import SFNClient
 from mypy_boto3_storagegateway.client import StorageGatewayClient
 from mypy_boto3_sts.client import STSClient
+from mypy_boto3_supplychain.client import SupplyChainClient
 from mypy_boto3_support.client import SupportClient
 from mypy_boto3_support_app.client import SupportAppClient
 from mypy_boto3_swf.client import SWFClient
 from mypy_boto3_synthetics.client import SyntheticsClient
 from mypy_boto3_textract.client import TextractClient
+from mypy_boto3_timestream_influxdb.client import TimestreamInfluxDBClient
 from mypy_boto3_timestream_query.client import TimestreamQueryClient
 from mypy_boto3_timestream_write.client import TimestreamWriteClient
 from mypy_boto3_tnb.client import TelcoNetworkBuilderClient
 from mypy_boto3_transcribe.client import TranscribeServiceClient
 from mypy_boto3_transfer.client import TransferClient
 from mypy_boto3_translate.client import TranslateClient
 from mypy_boto3_trustedadvisor.client import TrustedAdvisorPublicAPIClient
@@ -746,14 +753,27 @@
     aws_access_key_id: Optional[str] = ...,
     aws_secret_access_key: Optional[str] = ...,
     aws_session_token: Optional[str] = ...,
     config: Optional[Config] = ...,
 ) -> ARCZonalShiftClient: ...
 @overload
 def client(
+    service_name: Literal["artifact"],
+    region_name: Optional[str] = ...,
+    api_version: Optional[str] = ...,
+    use_ssl: Optional[bool] = ...,
+    verify: Union[bool, str, None] = ...,
+    endpoint_url: Optional[str] = ...,
+    aws_access_key_id: Optional[str] = ...,
+    aws_secret_access_key: Optional[str] = ...,
+    aws_session_token: Optional[str] = ...,
+    config: Optional[Config] = ...,
+) -> ArtifactClient: ...
+@overload
+def client(
     service_name: Literal["athena"],
     region_name: Optional[str] = ...,
     api_version: Optional[str] = ...,
     use_ssl: Optional[bool] = ...,
     verify: Union[bool, str, None] = ...,
     endpoint_url: Optional[str] = ...,
     aws_access_key_id: Optional[str] = ...,
@@ -980,14 +1000,27 @@
     aws_access_key_id: Optional[str] = ...,
     aws_secret_access_key: Optional[str] = ...,
     aws_session_token: Optional[str] = ...,
     config: Optional[Config] = ...,
 ) -> CostExplorerClient: ...
 @overload
 def client(
+    service_name: Literal["chatbot"],
+    region_name: Optional[str] = ...,
+    api_version: Optional[str] = ...,
+    use_ssl: Optional[bool] = ...,
+    verify: Union[bool, str, None] = ...,
+    endpoint_url: Optional[str] = ...,
+    aws_access_key_id: Optional[str] = ...,
+    aws_secret_access_key: Optional[str] = ...,
+    aws_session_token: Optional[str] = ...,
+    config: Optional[Config] = ...,
+) -> ChatbotClient: ...
+@overload
+def client(
     service_name: Literal["chime"],
     region_name: Optional[str] = ...,
     api_version: Optional[str] = ...,
     use_ssl: Optional[bool] = ...,
     verify: Union[bool, str, None] = ...,
     endpoint_url: Optional[str] = ...,
     aws_access_key_id: Optional[str] = ...,
@@ -1305,14 +1338,27 @@
     aws_access_key_id: Optional[str] = ...,
     aws_secret_access_key: Optional[str] = ...,
     aws_session_token: Optional[str] = ...,
     config: Optional[Config] = ...,
 ) -> CodeCommitClient: ...
 @overload
 def client(
+    service_name: Literal["codeconnections"],
+    region_name: Optional[str] = ...,
+    api_version: Optional[str] = ...,
+    use_ssl: Optional[bool] = ...,
+    verify: Union[bool, str, None] = ...,
+    endpoint_url: Optional[str] = ...,
+    aws_access_key_id: Optional[str] = ...,
+    aws_secret_access_key: Optional[str] = ...,
+    aws_session_token: Optional[str] = ...,
+    config: Optional[Config] = ...,
+) -> CodeConnectionsClient: ...
+@overload
+def client(
     service_name: Literal["codedeploy"],
     region_name: Optional[str] = ...,
     api_version: Optional[str] = ...,
     use_ssl: Optional[bool] = ...,
     verify: Union[bool, str, None] = ...,
     endpoint_url: Optional[str] = ...,
     aws_access_key_id: Optional[str] = ...,
@@ -1565,14 +1611,27 @@
     aws_access_key_id: Optional[str] = ...,
     aws_secret_access_key: Optional[str] = ...,
     aws_session_token: Optional[str] = ...,
     config: Optional[Config] = ...,
 ) -> ConnectParticipantClient: ...
 @overload
 def client(
+    service_name: Literal["controlcatalog"],
+    region_name: Optional[str] = ...,
+    api_version: Optional[str] = ...,
+    use_ssl: Optional[bool] = ...,
+    verify: Union[bool, str, None] = ...,
+    endpoint_url: Optional[str] = ...,
+    aws_access_key_id: Optional[str] = ...,
+    aws_secret_access_key: Optional[str] = ...,
+    aws_session_token: Optional[str] = ...,
+    config: Optional[Config] = ...,
+) -> ControlCatalogClient: ...
+@overload
+def client(
     service_name: Literal["controltower"],
     region_name: Optional[str] = ...,
     api_version: Optional[str] = ...,
     use_ssl: Optional[bool] = ...,
     verify: Union[bool, str, None] = ...,
     endpoint_url: Optional[str] = ...,
     aws_access_key_id: Optional[str] = ...,
@@ -1695,14 +1754,27 @@
     aws_access_key_id: Optional[str] = ...,
     aws_secret_access_key: Optional[str] = ...,
     aws_session_token: Optional[str] = ...,
     config: Optional[Config] = ...,
 ) -> DAXClient: ...
 @overload
 def client(
+    service_name: Literal["deadline"],
+    region_name: Optional[str] = ...,
+    api_version: Optional[str] = ...,
+    use_ssl: Optional[bool] = ...,
+    verify: Union[bool, str, None] = ...,
+    endpoint_url: Optional[str] = ...,
+    aws_access_key_id: Optional[str] = ...,
+    aws_secret_access_key: Optional[str] = ...,
+    aws_session_token: Optional[str] = ...,
+    config: Optional[Config] = ...,
+) -> DeadlineCloudClient: ...
+@overload
+def client(
     service_name: Literal["detective"],
     region_name: Optional[str] = ...,
     api_version: Optional[str] = ...,
     use_ssl: Optional[bool] = ...,
     verify: Union[bool, str, None] = ...,
     endpoint_url: Optional[str] = ...,
     aws_access_key_id: Optional[str] = ...,
@@ -2579,27 +2651,14 @@
     aws_access_key_id: Optional[str] = ...,
     aws_secret_access_key: Optional[str] = ...,
     aws_session_token: Optional[str] = ...,
     config: Optional[Config] = ...,
 ) -> IoTJobsDataPlaneClient: ...
 @overload
 def client(
-    service_name: Literal["iot-roborunner"],
-    region_name: Optional[str] = ...,
-    api_version: Optional[str] = ...,
-    use_ssl: Optional[bool] = ...,
-    verify: Union[bool, str, None] = ...,
-    endpoint_url: Optional[str] = ...,
-    aws_access_key_id: Optional[str] = ...,
-    aws_secret_access_key: Optional[str] = ...,
-    aws_session_token: Optional[str] = ...,
-    config: Optional[Config] = ...,
-) -> IoTRoboRunnerClient: ...
-@overload
-def client(
     service_name: Literal["iot1click-devices"],
     region_name: Optional[str] = ...,
     api_version: Optional[str] = ...,
     use_ssl: Optional[bool] = ...,
     verify: Union[bool, str, None] = ...,
     endpoint_url: Optional[str] = ...,
     aws_access_key_id: Optional[str] = ...,
@@ -4360,14 +4419,27 @@
     aws_access_key_id: Optional[str] = ...,
     aws_secret_access_key: Optional[str] = ...,
     aws_session_token: Optional[str] = ...,
     config: Optional[Config] = ...,
 ) -> Route53DomainsClient: ...
 @overload
 def client(
+    service_name: Literal["route53profiles"],
+    region_name: Optional[str] = ...,
+    api_version: Optional[str] = ...,
+    use_ssl: Optional[bool] = ...,
+    verify: Union[bool, str, None] = ...,
+    endpoint_url: Optional[str] = ...,
+    aws_access_key_id: Optional[str] = ...,
+    aws_secret_access_key: Optional[str] = ...,
+    aws_session_token: Optional[str] = ...,
+    config: Optional[Config] = ...,
+) -> Route53ProfilesClient: ...
+@overload
+def client(
     service_name: Literal["route53resolver"],
     region_name: Optional[str] = ...,
     api_version: Optional[str] = ...,
     use_ssl: Optional[bool] = ...,
     verify: Union[bool, str, None] = ...,
     endpoint_url: Optional[str] = ...,
     aws_access_key_id: Optional[str] = ...,
@@ -4945,14 +5017,27 @@
     aws_access_key_id: Optional[str] = ...,
     aws_secret_access_key: Optional[str] = ...,
     aws_session_token: Optional[str] = ...,
     config: Optional[Config] = ...,
 ) -> STSClient: ...
 @overload
 def client(
+    service_name: Literal["supplychain"],
+    region_name: Optional[str] = ...,
+    api_version: Optional[str] = ...,
+    use_ssl: Optional[bool] = ...,
+    verify: Union[bool, str, None] = ...,
+    endpoint_url: Optional[str] = ...,
+    aws_access_key_id: Optional[str] = ...,
+    aws_secret_access_key: Optional[str] = ...,
+    aws_session_token: Optional[str] = ...,
+    config: Optional[Config] = ...,
+) -> SupplyChainClient: ...
+@overload
+def client(
     service_name: Literal["support"],
     region_name: Optional[str] = ...,
     api_version: Optional[str] = ...,
     use_ssl: Optional[bool] = ...,
     verify: Union[bool, str, None] = ...,
     endpoint_url: Optional[str] = ...,
     aws_access_key_id: Optional[str] = ...,
@@ -5010,14 +5095,27 @@
     aws_access_key_id: Optional[str] = ...,
     aws_secret_access_key: Optional[str] = ...,
     aws_session_token: Optional[str] = ...,
     config: Optional[Config] = ...,
 ) -> TextractClient: ...
 @overload
 def client(
+    service_name: Literal["timestream-influxdb"],
+    region_name: Optional[str] = ...,
+    api_version: Optional[str] = ...,
+    use_ssl: Optional[bool] = ...,
+    verify: Union[bool, str, None] = ...,
+    endpoint_url: Optional[str] = ...,
+    aws_access_key_id: Optional[str] = ...,
+    aws_secret_access_key: Optional[str] = ...,
+    aws_session_token: Optional[str] = ...,
+    config: Optional[Config] = ...,
+) -> TimestreamInfluxDBClient: ...
+@overload
+def client(
     service_name: Literal["timestream-query"],
     region_name: Optional[str] = ...,
     api_version: Optional[str] = ...,
     use_ssl: Optional[bool] = ...,
     verify: Union[bool, str, None] = ...,
     endpoint_url: Optional[str] = ...,
     aws_access_key_id: Optional[str] = ...,
```

### Comparing `boto3-stubs-1.34.9/boto3-stubs/crt.pyi` & `boto3_stubs-1.34.90/boto3-stubs/crt.pyi`

 * *Files identical despite different names*

### Comparing `boto3-stubs-1.34.9/boto3-stubs/docs/utils.pyi` & `boto3_stubs-1.34.90/boto3-stubs/docs/utils.pyi`

 * *Files identical despite different names*

### Comparing `boto3-stubs-1.34.9/boto3-stubs/dynamodb/conditions.pyi` & `boto3_stubs-1.34.90/boto3-stubs/dynamodb/conditions.pyi`

 * *Files identical despite different names*

### Comparing `boto3-stubs-1.34.9/boto3-stubs/dynamodb/table.pyi` & `boto3_stubs-1.34.90/boto3-stubs/dynamodb/table.pyi`

 * *Files identical despite different names*

### Comparing `boto3-stubs-1.34.9/boto3-stubs/dynamodb/transform.pyi` & `boto3_stubs-1.34.90/boto3-stubs/dynamodb/transform.pyi`

 * *Files identical despite different names*

### Comparing `boto3-stubs-1.34.9/boto3-stubs/dynamodb/types.pyi` & `boto3_stubs-1.34.90/boto3-stubs/dynamodb/types.pyi`

 * *Files identical despite different names*

### Comparing `boto3-stubs-1.34.9/boto3-stubs/exceptions.pyi` & `boto3_stubs-1.34.90/boto3-stubs/exceptions.pyi`

 * *Files identical despite different names*

### Comparing `boto3-stubs-1.34.9/boto3-stubs/resources/action.pyi` & `boto3_stubs-1.34.90/boto3-stubs/resources/action.pyi`

 * *Files identical despite different names*

### Comparing `boto3-stubs-1.34.9/boto3-stubs/resources/base.pyi` & `boto3_stubs-1.34.90/boto3-stubs/resources/base.pyi`

 * *Files identical despite different names*

### Comparing `boto3-stubs-1.34.9/boto3-stubs/resources/collection.pyi` & `boto3_stubs-1.34.90/boto3-stubs/resources/collection.pyi`

 * *Files identical despite different names*

### Comparing `boto3-stubs-1.34.9/boto3-stubs/resources/model.pyi` & `boto3_stubs-1.34.90/boto3-stubs/resources/model.pyi`

 * *Files identical despite different names*

### Comparing `boto3-stubs-1.34.9/boto3-stubs/resources/params.pyi` & `boto3_stubs-1.34.90/boto3-stubs/resources/params.pyi`

 * *Files identical despite different names*

### Comparing `boto3-stubs-1.34.9/boto3-stubs/resources/response.pyi` & `boto3_stubs-1.34.90/boto3-stubs/resources/response.pyi`

 * *Files identical despite different names*

### Comparing `boto3-stubs-1.34.9/boto3-stubs/s3/inject.pyi` & `boto3_stubs-1.34.90/boto3-stubs/s3/inject.pyi`

 * *Files identical despite different names*

### Comparing `boto3-stubs-1.34.9/boto3-stubs/s3/transfer.pyi` & `boto3_stubs-1.34.90/boto3-stubs/s3/transfer.pyi`

 * *Files identical despite different names*

### Comparing `boto3-stubs-1.34.9/boto3-stubs/session.pyi` & `boto3_stubs-1.34.90/boto3-stubs/session.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 from mypy_boto3_application_insights.client import ApplicationInsightsClient
 from mypy_boto3_applicationcostprofiler.client import ApplicationCostProfilerClient
 from mypy_boto3_appmesh.client import AppMeshClient
 from mypy_boto3_apprunner.client import AppRunnerClient
 from mypy_boto3_appstream.client import AppStreamClient
 from mypy_boto3_appsync.client import AppSyncClient
 from mypy_boto3_arc_zonal_shift.client import ARCZonalShiftClient
+from mypy_boto3_artifact.client import ArtifactClient
 from mypy_boto3_athena.client import AthenaClient
 from mypy_boto3_auditmanager.client import AuditManagerClient
 from mypy_boto3_autoscaling.client import AutoScalingClient
 from mypy_boto3_autoscaling_plans.client import AutoScalingPlansClient
 from mypy_boto3_b2bi.client import B2BIClient
 from mypy_boto3_backup.client import BackupClient
 from mypy_boto3_backup_gateway.client import BackupGatewayClient
@@ -51,14 +52,15 @@
 from mypy_boto3_bedrock_agent.client import AgentsforBedrockClient
 from mypy_boto3_bedrock_agent_runtime.client import AgentsforBedrockRuntimeClient
 from mypy_boto3_bedrock_runtime.client import BedrockRuntimeClient
 from mypy_boto3_billingconductor.client import BillingConductorClient
 from mypy_boto3_braket.client import BraketClient
 from mypy_boto3_budgets.client import BudgetsClient
 from mypy_boto3_ce.client import CostExplorerClient
+from mypy_boto3_chatbot.client import ChatbotClient
 from mypy_boto3_chime.client import ChimeClient
 from mypy_boto3_chime_sdk_identity.client import ChimeSDKIdentityClient
 from mypy_boto3_chime_sdk_media_pipelines.client import ChimeSDKMediaPipelinesClient
 from mypy_boto3_chime_sdk_meetings.client import ChimeSDKMeetingsClient
 from mypy_boto3_chime_sdk_messaging.client import ChimeSDKMessagingClient
 from mypy_boto3_chime_sdk_voice.client import ChimeSDKVoiceClient
 from mypy_boto3_cleanrooms.client import CleanRoomsServiceClient
@@ -78,14 +80,15 @@
 from mypy_boto3_cloudtrail_data.client import CloudTrailDataServiceClient
 from mypy_boto3_cloudwatch.client import CloudWatchClient
 from mypy_boto3_cloudwatch.service_resource import CloudWatchServiceResource
 from mypy_boto3_codeartifact.client import CodeArtifactClient
 from mypy_boto3_codebuild.client import CodeBuildClient
 from mypy_boto3_codecatalyst.client import CodeCatalystClient
 from mypy_boto3_codecommit.client import CodeCommitClient
+from mypy_boto3_codeconnections.client import CodeConnectionsClient
 from mypy_boto3_codedeploy.client import CodeDeployClient
 from mypy_boto3_codeguru_reviewer.client import CodeGuruReviewerClient
 from mypy_boto3_codeguru_security.client import CodeGuruSecurityClient
 from mypy_boto3_codeguruprofiler.client import CodeGuruProfilerClient
 from mypy_boto3_codepipeline.client import CodePipelineClient
 from mypy_boto3_codestar.client import CodeStarClient
 from mypy_boto3_codestar_connections.client import CodeStarconnectionsClient
@@ -98,24 +101,26 @@
 from mypy_boto3_compute_optimizer.client import ComputeOptimizerClient
 from mypy_boto3_config.client import ConfigServiceClient
 from mypy_boto3_connect.client import ConnectClient
 from mypy_boto3_connect_contact_lens.client import ConnectContactLensClient
 from mypy_boto3_connectcampaigns.client import ConnectCampaignServiceClient
 from mypy_boto3_connectcases.client import ConnectCasesClient
 from mypy_boto3_connectparticipant.client import ConnectParticipantClient
+from mypy_boto3_controlcatalog.client import ControlCatalogClient
 from mypy_boto3_controltower.client import ControlTowerClient
 from mypy_boto3_cost_optimization_hub.client import CostOptimizationHubClient
 from mypy_boto3_cur.client import CostandUsageReportServiceClient
 from mypy_boto3_customer_profiles.client import CustomerProfilesClient
 from mypy_boto3_databrew.client import GlueDataBrewClient
 from mypy_boto3_dataexchange.client import DataExchangeClient
 from mypy_boto3_datapipeline.client import DataPipelineClient
 from mypy_boto3_datasync.client import DataSyncClient
 from mypy_boto3_datazone.client import DataZoneClient
 from mypy_boto3_dax.client import DAXClient
+from mypy_boto3_deadline.client import DeadlineCloudClient
 from mypy_boto3_detective.client import DetectiveClient
 from mypy_boto3_devicefarm.client import DeviceFarmClient
 from mypy_boto3_devops_guru.client import DevOpsGuruClient
 from mypy_boto3_directconnect.client import DirectConnectClient
 from mypy_boto3_discovery.client import ApplicationDiscoveryServiceClient
 from mypy_boto3_dlm.client import DLMClient
 from mypy_boto3_dms.client import DatabaseMigrationServiceClient
@@ -182,15 +187,14 @@
 from mypy_boto3_inspector_scan.client import inspectorscanClient
 from mypy_boto3_internetmonitor.client import CloudWatchInternetMonitorClient
 from mypy_boto3_iot1click_devices.client import IoT1ClickDevicesServiceClient
 from mypy_boto3_iot1click_projects.client import IoT1ClickProjectsClient
 from mypy_boto3_iot.client import IoTClient
 from mypy_boto3_iot_data.client import IoTDataPlaneClient
 from mypy_boto3_iot_jobs_data.client import IoTJobsDataPlaneClient
-from mypy_boto3_iot_roborunner.client import IoTRoboRunnerClient
 from mypy_boto3_iotanalytics.client import IoTAnalyticsClient
 from mypy_boto3_iotdeviceadvisor.client import IoTDeviceAdvisorClient
 from mypy_boto3_iotevents.client import IoTEventsClient
 from mypy_boto3_iotevents_data.client import IoTEventsDataClient
 from mypy_boto3_iotfleethub.client import IoTFleetHubClient
 from mypy_boto3_iotfleetwise.client import IoTFleetWiseClient
 from mypy_boto3_iotsecuretunneling.client import IoTSecureTunnelingClient
@@ -322,14 +326,15 @@
 from mypy_boto3_robomaker.client import RoboMakerClient
 from mypy_boto3_rolesanywhere.client import IAMRolesAnywhereClient
 from mypy_boto3_route53.client import Route53Client
 from mypy_boto3_route53_recovery_cluster.client import Route53RecoveryClusterClient
 from mypy_boto3_route53_recovery_control_config.client import Route53RecoveryControlConfigClient
 from mypy_boto3_route53_recovery_readiness.client import Route53RecoveryReadinessClient
 from mypy_boto3_route53domains.client import Route53DomainsClient
+from mypy_boto3_route53profiles.client import Route53ProfilesClient
 from mypy_boto3_route53resolver.client import Route53ResolverClient
 from mypy_boto3_rum.client import CloudWatchRUMClient
 from mypy_boto3_s3.client import S3Client
 from mypy_boto3_s3.service_resource import S3ServiceResource
 from mypy_boto3_s3control.client import S3ControlClient
 from mypy_boto3_s3outposts.client import S3OutpostsClient
 from mypy_boto3_sagemaker.client import SageMakerClient
@@ -370,19 +375,21 @@
 from mypy_boto3_ssm_sap.client import SsmSapClient
 from mypy_boto3_sso.client import SSOClient
 from mypy_boto3_sso_admin.client import SSOAdminClient
 from mypy_boto3_sso_oidc.client import SSOOIDCClient
 from mypy_boto3_stepfunctions.client import SFNClient
 from mypy_boto3_storagegateway.client import StorageGatewayClient
 from mypy_boto3_sts.client import STSClient
+from mypy_boto3_supplychain.client import SupplyChainClient
 from mypy_boto3_support.client import SupportClient
 from mypy_boto3_support_app.client import SupportAppClient
 from mypy_boto3_swf.client import SWFClient
 from mypy_boto3_synthetics.client import SyntheticsClient
 from mypy_boto3_textract.client import TextractClient
+from mypy_boto3_timestream_influxdb.client import TimestreamInfluxDBClient
 from mypy_boto3_timestream_query.client import TimestreamQueryClient
 from mypy_boto3_timestream_write.client import TimestreamWriteClient
 from mypy_boto3_tnb.client import TelcoNetworkBuilderClient
 from mypy_boto3_transcribe.client import TranscribeServiceClient
 from mypy_boto3_transfer.client import TransferClient
 from mypy_boto3_translate.client import TranslateClient
 from mypy_boto3_trustedadvisor.client import TrustedAdvisorPublicAPIClient
@@ -793,14 +800,28 @@
         aws_secret_access_key: Optional[str] = ...,
         aws_session_token: Optional[str] = ...,
         config: Optional[Config] = ...,
     ) -> ARCZonalShiftClient: ...
     @overload
     def client(
         self,
+        service_name: Literal["artifact"],
+        region_name: Optional[str] = ...,
+        api_version: Optional[str] = ...,
+        use_ssl: Optional[bool] = ...,
+        verify: Union[bool, str, None] = ...,
+        endpoint_url: Optional[str] = ...,
+        aws_access_key_id: Optional[str] = ...,
+        aws_secret_access_key: Optional[str] = ...,
+        aws_session_token: Optional[str] = ...,
+        config: Optional[Config] = ...,
+    ) -> ArtifactClient: ...
+    @overload
+    def client(
+        self,
         service_name: Literal["athena"],
         region_name: Optional[str] = ...,
         api_version: Optional[str] = ...,
         use_ssl: Optional[bool] = ...,
         verify: Union[bool, str, None] = ...,
         endpoint_url: Optional[str] = ...,
         aws_access_key_id: Optional[str] = ...,
@@ -1045,14 +1066,28 @@
         aws_secret_access_key: Optional[str] = ...,
         aws_session_token: Optional[str] = ...,
         config: Optional[Config] = ...,
     ) -> CostExplorerClient: ...
     @overload
     def client(
         self,
+        service_name: Literal["chatbot"],
+        region_name: Optional[str] = ...,
+        api_version: Optional[str] = ...,
+        use_ssl: Optional[bool] = ...,
+        verify: Union[bool, str, None] = ...,
+        endpoint_url: Optional[str] = ...,
+        aws_access_key_id: Optional[str] = ...,
+        aws_secret_access_key: Optional[str] = ...,
+        aws_session_token: Optional[str] = ...,
+        config: Optional[Config] = ...,
+    ) -> ChatbotClient: ...
+    @overload
+    def client(
+        self,
         service_name: Literal["chime"],
         region_name: Optional[str] = ...,
         api_version: Optional[str] = ...,
         use_ssl: Optional[bool] = ...,
         verify: Union[bool, str, None] = ...,
         endpoint_url: Optional[str] = ...,
         aws_access_key_id: Optional[str] = ...,
@@ -1395,14 +1430,28 @@
         aws_secret_access_key: Optional[str] = ...,
         aws_session_token: Optional[str] = ...,
         config: Optional[Config] = ...,
     ) -> CodeCommitClient: ...
     @overload
     def client(
         self,
+        service_name: Literal["codeconnections"],
+        region_name: Optional[str] = ...,
+        api_version: Optional[str] = ...,
+        use_ssl: Optional[bool] = ...,
+        verify: Union[bool, str, None] = ...,
+        endpoint_url: Optional[str] = ...,
+        aws_access_key_id: Optional[str] = ...,
+        aws_secret_access_key: Optional[str] = ...,
+        aws_session_token: Optional[str] = ...,
+        config: Optional[Config] = ...,
+    ) -> CodeConnectionsClient: ...
+    @overload
+    def client(
+        self,
         service_name: Literal["codedeploy"],
         region_name: Optional[str] = ...,
         api_version: Optional[str] = ...,
         use_ssl: Optional[bool] = ...,
         verify: Union[bool, str, None] = ...,
         endpoint_url: Optional[str] = ...,
         aws_access_key_id: Optional[str] = ...,
@@ -1675,14 +1724,28 @@
         aws_secret_access_key: Optional[str] = ...,
         aws_session_token: Optional[str] = ...,
         config: Optional[Config] = ...,
     ) -> ConnectParticipantClient: ...
     @overload
     def client(
         self,
+        service_name: Literal["controlcatalog"],
+        region_name: Optional[str] = ...,
+        api_version: Optional[str] = ...,
+        use_ssl: Optional[bool] = ...,
+        verify: Union[bool, str, None] = ...,
+        endpoint_url: Optional[str] = ...,
+        aws_access_key_id: Optional[str] = ...,
+        aws_secret_access_key: Optional[str] = ...,
+        aws_session_token: Optional[str] = ...,
+        config: Optional[Config] = ...,
+    ) -> ControlCatalogClient: ...
+    @overload
+    def client(
+        self,
         service_name: Literal["controltower"],
         region_name: Optional[str] = ...,
         api_version: Optional[str] = ...,
         use_ssl: Optional[bool] = ...,
         verify: Union[bool, str, None] = ...,
         endpoint_url: Optional[str] = ...,
         aws_access_key_id: Optional[str] = ...,
@@ -1815,14 +1878,28 @@
         aws_secret_access_key: Optional[str] = ...,
         aws_session_token: Optional[str] = ...,
         config: Optional[Config] = ...,
     ) -> DAXClient: ...
     @overload
     def client(
         self,
+        service_name: Literal["deadline"],
+        region_name: Optional[str] = ...,
+        api_version: Optional[str] = ...,
+        use_ssl: Optional[bool] = ...,
+        verify: Union[bool, str, None] = ...,
+        endpoint_url: Optional[str] = ...,
+        aws_access_key_id: Optional[str] = ...,
+        aws_secret_access_key: Optional[str] = ...,
+        aws_session_token: Optional[str] = ...,
+        config: Optional[Config] = ...,
+    ) -> DeadlineCloudClient: ...
+    @overload
+    def client(
+        self,
         service_name: Literal["detective"],
         region_name: Optional[str] = ...,
         api_version: Optional[str] = ...,
         use_ssl: Optional[bool] = ...,
         verify: Union[bool, str, None] = ...,
         endpoint_url: Optional[str] = ...,
         aws_access_key_id: Optional[str] = ...,
@@ -2767,28 +2844,14 @@
         aws_secret_access_key: Optional[str] = ...,
         aws_session_token: Optional[str] = ...,
         config: Optional[Config] = ...,
     ) -> IoTJobsDataPlaneClient: ...
     @overload
     def client(
         self,
-        service_name: Literal["iot-roborunner"],
-        region_name: Optional[str] = ...,
-        api_version: Optional[str] = ...,
-        use_ssl: Optional[bool] = ...,
-        verify: Union[bool, str, None] = ...,
-        endpoint_url: Optional[str] = ...,
-        aws_access_key_id: Optional[str] = ...,
-        aws_secret_access_key: Optional[str] = ...,
-        aws_session_token: Optional[str] = ...,
-        config: Optional[Config] = ...,
-    ) -> IoTRoboRunnerClient: ...
-    @overload
-    def client(
-        self,
         service_name: Literal["iot1click-devices"],
         region_name: Optional[str] = ...,
         api_version: Optional[str] = ...,
         use_ssl: Optional[bool] = ...,
         verify: Union[bool, str, None] = ...,
         endpoint_url: Optional[str] = ...,
         aws_access_key_id: Optional[str] = ...,
@@ -4685,14 +4748,28 @@
         aws_secret_access_key: Optional[str] = ...,
         aws_session_token: Optional[str] = ...,
         config: Optional[Config] = ...,
     ) -> Route53DomainsClient: ...
     @overload
     def client(
         self,
+        service_name: Literal["route53profiles"],
+        region_name: Optional[str] = ...,
+        api_version: Optional[str] = ...,
+        use_ssl: Optional[bool] = ...,
+        verify: Union[bool, str, None] = ...,
+        endpoint_url: Optional[str] = ...,
+        aws_access_key_id: Optional[str] = ...,
+        aws_secret_access_key: Optional[str] = ...,
+        aws_session_token: Optional[str] = ...,
+        config: Optional[Config] = ...,
+    ) -> Route53ProfilesClient: ...
+    @overload
+    def client(
+        self,
         service_name: Literal["route53resolver"],
         region_name: Optional[str] = ...,
         api_version: Optional[str] = ...,
         use_ssl: Optional[bool] = ...,
         verify: Union[bool, str, None] = ...,
         endpoint_url: Optional[str] = ...,
         aws_access_key_id: Optional[str] = ...,
@@ -5315,14 +5392,28 @@
         aws_secret_access_key: Optional[str] = ...,
         aws_session_token: Optional[str] = ...,
         config: Optional[Config] = ...,
     ) -> STSClient: ...
     @overload
     def client(
         self,
+        service_name: Literal["supplychain"],
+        region_name: Optional[str] = ...,
+        api_version: Optional[str] = ...,
+        use_ssl: Optional[bool] = ...,
+        verify: Union[bool, str, None] = ...,
+        endpoint_url: Optional[str] = ...,
+        aws_access_key_id: Optional[str] = ...,
+        aws_secret_access_key: Optional[str] = ...,
+        aws_session_token: Optional[str] = ...,
+        config: Optional[Config] = ...,
+    ) -> SupplyChainClient: ...
+    @overload
+    def client(
+        self,
         service_name: Literal["support"],
         region_name: Optional[str] = ...,
         api_version: Optional[str] = ...,
         use_ssl: Optional[bool] = ...,
         verify: Union[bool, str, None] = ...,
         endpoint_url: Optional[str] = ...,
         aws_access_key_id: Optional[str] = ...,
@@ -5385,14 +5476,28 @@
         aws_secret_access_key: Optional[str] = ...,
         aws_session_token: Optional[str] = ...,
         config: Optional[Config] = ...,
     ) -> TextractClient: ...
     @overload
     def client(
         self,
+        service_name: Literal["timestream-influxdb"],
+        region_name: Optional[str] = ...,
+        api_version: Optional[str] = ...,
+        use_ssl: Optional[bool] = ...,
+        verify: Union[bool, str, None] = ...,
+        endpoint_url: Optional[str] = ...,
+        aws_access_key_id: Optional[str] = ...,
+        aws_secret_access_key: Optional[str] = ...,
+        aws_session_token: Optional[str] = ...,
+        config: Optional[Config] = ...,
+    ) -> TimestreamInfluxDBClient: ...
+    @overload
+    def client(
+        self,
         service_name: Literal["timestream-query"],
         region_name: Optional[str] = ...,
         api_version: Optional[str] = ...,
         use_ssl: Optional[bool] = ...,
         verify: Union[bool, str, None] = ...,
         endpoint_url: Optional[str] = ...,
         aws_access_key_id: Optional[str] = ...,
```

### Comparing `boto3-stubs-1.34.9/boto3-stubs/utils.pyi` & `boto3_stubs-1.34.90/boto3-stubs/utils.pyi`

 * *Files identical despite different names*

### Comparing `boto3-stubs-1.34.9/boto3_stubs.egg-info/SOURCES.txt` & `boto3_stubs-1.34.90/boto3_stubs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `boto3-stubs-1.34.9/boto3_stubs.egg-info/requires.txt` & `boto3_stubs-1.34.90/boto3_stubs.egg-info/requires.txt`

 * *Files 0% similar despite different names*

```diff
@@ -41,14 +41,15 @@
 mypy-boto3-application-insights<1.35.0,>=1.34.0
 mypy-boto3-applicationcostprofiler<1.35.0,>=1.34.0
 mypy-boto3-appmesh<1.35.0,>=1.34.0
 mypy-boto3-apprunner<1.35.0,>=1.34.0
 mypy-boto3-appstream<1.35.0,>=1.34.0
 mypy-boto3-appsync<1.35.0,>=1.34.0
 mypy-boto3-arc-zonal-shift<1.35.0,>=1.34.0
+mypy-boto3-artifact<1.35.0,>=1.34.0
 mypy-boto3-athena<1.35.0,>=1.34.0
 mypy-boto3-auditmanager<1.35.0,>=1.34.0
 mypy-boto3-autoscaling<1.35.0,>=1.34.0
 mypy-boto3-autoscaling-plans<1.35.0,>=1.34.0
 mypy-boto3-b2bi<1.35.0,>=1.34.0
 mypy-boto3-backup<1.35.0,>=1.34.0
 mypy-boto3-backup-gateway<1.35.0,>=1.34.0
@@ -59,14 +60,15 @@
 mypy-boto3-bedrock-agent<1.35.0,>=1.34.0
 mypy-boto3-bedrock-agent-runtime<1.35.0,>=1.34.0
 mypy-boto3-bedrock-runtime<1.35.0,>=1.34.0
 mypy-boto3-billingconductor<1.35.0,>=1.34.0
 mypy-boto3-braket<1.35.0,>=1.34.0
 mypy-boto3-budgets<1.35.0,>=1.34.0
 mypy-boto3-ce<1.35.0,>=1.34.0
+mypy-boto3-chatbot<1.35.0,>=1.34.0
 mypy-boto3-chime<1.35.0,>=1.34.0
 mypy-boto3-chime-sdk-identity<1.35.0,>=1.34.0
 mypy-boto3-chime-sdk-media-pipelines<1.35.0,>=1.34.0
 mypy-boto3-chime-sdk-meetings<1.35.0,>=1.34.0
 mypy-boto3-chime-sdk-messaging<1.35.0,>=1.34.0
 mypy-boto3-chime-sdk-voice<1.35.0,>=1.34.0
 mypy-boto3-cleanrooms<1.35.0,>=1.34.0
@@ -84,14 +86,15 @@
 mypy-boto3-cloudtrail<1.35.0,>=1.34.0
 mypy-boto3-cloudtrail-data<1.35.0,>=1.34.0
 mypy-boto3-cloudwatch<1.35.0,>=1.34.0
 mypy-boto3-codeartifact<1.35.0,>=1.34.0
 mypy-boto3-codebuild<1.35.0,>=1.34.0
 mypy-boto3-codecatalyst<1.35.0,>=1.34.0
 mypy-boto3-codecommit<1.35.0,>=1.34.0
+mypy-boto3-codeconnections<1.35.0,>=1.34.0
 mypy-boto3-codedeploy<1.35.0,>=1.34.0
 mypy-boto3-codeguru-reviewer<1.35.0,>=1.34.0
 mypy-boto3-codeguru-security<1.35.0,>=1.34.0
 mypy-boto3-codeguruprofiler<1.35.0,>=1.34.0
 mypy-boto3-codepipeline<1.35.0,>=1.34.0
 mypy-boto3-codestar<1.35.0,>=1.34.0
 mypy-boto3-codestar-connections<1.35.0,>=1.34.0
@@ -104,24 +107,26 @@
 mypy-boto3-compute-optimizer<1.35.0,>=1.34.0
 mypy-boto3-config<1.35.0,>=1.34.0
 mypy-boto3-connect<1.35.0,>=1.34.0
 mypy-boto3-connect-contact-lens<1.35.0,>=1.34.0
 mypy-boto3-connectcampaigns<1.35.0,>=1.34.0
 mypy-boto3-connectcases<1.35.0,>=1.34.0
 mypy-boto3-connectparticipant<1.35.0,>=1.34.0
+mypy-boto3-controlcatalog<1.35.0,>=1.34.0
 mypy-boto3-controltower<1.35.0,>=1.34.0
 mypy-boto3-cost-optimization-hub<1.35.0,>=1.34.0
 mypy-boto3-cur<1.35.0,>=1.34.0
 mypy-boto3-customer-profiles<1.35.0,>=1.34.0
 mypy-boto3-databrew<1.35.0,>=1.34.0
 mypy-boto3-dataexchange<1.35.0,>=1.34.0
 mypy-boto3-datapipeline<1.35.0,>=1.34.0
 mypy-boto3-datasync<1.35.0,>=1.34.0
 mypy-boto3-datazone<1.35.0,>=1.34.0
 mypy-boto3-dax<1.35.0,>=1.34.0
+mypy-boto3-deadline<1.35.0,>=1.34.0
 mypy-boto3-detective<1.35.0,>=1.34.0
 mypy-boto3-devicefarm<1.35.0,>=1.34.0
 mypy-boto3-devops-guru<1.35.0,>=1.34.0
 mypy-boto3-directconnect<1.35.0,>=1.34.0
 mypy-boto3-discovery<1.35.0,>=1.34.0
 mypy-boto3-dlm<1.35.0,>=1.34.0
 mypy-boto3-dms<1.35.0,>=1.34.0
@@ -182,15 +187,14 @@
 mypy-boto3-inspector<1.35.0,>=1.34.0
 mypy-boto3-inspector-scan<1.35.0,>=1.34.0
 mypy-boto3-inspector2<1.35.0,>=1.34.0
 mypy-boto3-internetmonitor<1.35.0,>=1.34.0
 mypy-boto3-iot<1.35.0,>=1.34.0
 mypy-boto3-iot-data<1.35.0,>=1.34.0
 mypy-boto3-iot-jobs-data<1.35.0,>=1.34.0
-mypy-boto3-iot-roborunner<1.35.0,>=1.34.0
 mypy-boto3-iot1click-devices<1.35.0,>=1.34.0
 mypy-boto3-iot1click-projects<1.35.0,>=1.34.0
 mypy-boto3-iotanalytics<1.35.0,>=1.34.0
 mypy-boto3-iotdeviceadvisor<1.35.0,>=1.34.0
 mypy-boto3-iotevents<1.35.0,>=1.34.0
 mypy-boto3-iotevents-data<1.35.0,>=1.34.0
 mypy-boto3-iotfleethub<1.35.0,>=1.34.0
@@ -319,14 +323,15 @@
 mypy-boto3-robomaker<1.35.0,>=1.34.0
 mypy-boto3-rolesanywhere<1.35.0,>=1.34.0
 mypy-boto3-route53<1.35.0,>=1.34.0
 mypy-boto3-route53-recovery-cluster<1.35.0,>=1.34.0
 mypy-boto3-route53-recovery-control-config<1.35.0,>=1.34.0
 mypy-boto3-route53-recovery-readiness<1.35.0,>=1.34.0
 mypy-boto3-route53domains<1.35.0,>=1.34.0
+mypy-boto3-route53profiles<1.35.0,>=1.34.0
 mypy-boto3-route53resolver<1.35.0,>=1.34.0
 mypy-boto3-rum<1.35.0,>=1.34.0
 mypy-boto3-s3<1.35.0,>=1.34.0
 mypy-boto3-s3control<1.35.0,>=1.34.0
 mypy-boto3-s3outposts<1.35.0,>=1.34.0
 mypy-boto3-sagemaker<1.35.0,>=1.34.0
 mypy-boto3-sagemaker-a2i-runtime<1.35.0,>=1.34.0
@@ -364,19 +369,21 @@
 mypy-boto3-ssm-sap<1.35.0,>=1.34.0
 mypy-boto3-sso<1.35.0,>=1.34.0
 mypy-boto3-sso-admin<1.35.0,>=1.34.0
 mypy-boto3-sso-oidc<1.35.0,>=1.34.0
 mypy-boto3-stepfunctions<1.35.0,>=1.34.0
 mypy-boto3-storagegateway<1.35.0,>=1.34.0
 mypy-boto3-sts<1.35.0,>=1.34.0
+mypy-boto3-supplychain<1.35.0,>=1.34.0
 mypy-boto3-support<1.35.0,>=1.34.0
 mypy-boto3-support-app<1.35.0,>=1.34.0
 mypy-boto3-swf<1.35.0,>=1.34.0
 mypy-boto3-synthetics<1.35.0,>=1.34.0
 mypy-boto3-textract<1.35.0,>=1.34.0
+mypy-boto3-timestream-influxdb<1.35.0,>=1.34.0
 mypy-boto3-timestream-query<1.35.0,>=1.34.0
 mypy-boto3-timestream-write<1.35.0,>=1.34.0
 mypy-boto3-tnb<1.35.0,>=1.34.0
 mypy-boto3-transcribe<1.35.0,>=1.34.0
 mypy-boto3-transfer<1.35.0,>=1.34.0
 mypy-boto3-translate<1.35.0,>=1.34.0
 mypy-boto3-trustedadvisor<1.35.0,>=1.34.0
@@ -453,14 +460,17 @@
 
 [appsync]
 mypy-boto3-appsync<1.35.0,>=1.34.0
 
 [arc-zonal-shift]
 mypy-boto3-arc-zonal-shift<1.35.0,>=1.34.0
 
+[artifact]
+mypy-boto3-artifact<1.35.0,>=1.34.0
+
 [athena]
 mypy-boto3-athena<1.35.0,>=1.34.0
 
 [auditmanager]
 mypy-boto3-auditmanager<1.35.0,>=1.34.0
 
 [autoscaling]
@@ -499,26 +509,29 @@
 [bedrock-runtime]
 mypy-boto3-bedrock-runtime<1.35.0,>=1.34.0
 
 [billingconductor]
 mypy-boto3-billingconductor<1.35.0,>=1.34.0
 
 [boto3]
-boto3==1.34.9
-botocore==1.34.9
+boto3==1.34.90
+botocore==1.34.90
 
 [braket]
 mypy-boto3-braket<1.35.0,>=1.34.0
 
 [budgets]
 mypy-boto3-budgets<1.35.0,>=1.34.0
 
 [ce]
 mypy-boto3-ce<1.35.0,>=1.34.0
 
+[chatbot]
+mypy-boto3-chatbot<1.35.0,>=1.34.0
+
 [chime]
 mypy-boto3-chime<1.35.0,>=1.34.0
 
 [chime-sdk-identity]
 mypy-boto3-chime-sdk-identity<1.35.0,>=1.34.0
 
 [chime-sdk-media-pipelines]
@@ -586,14 +599,17 @@
 
 [codecatalyst]
 mypy-boto3-codecatalyst<1.35.0,>=1.34.0
 
 [codecommit]
 mypy-boto3-codecommit<1.35.0,>=1.34.0
 
+[codeconnections]
+mypy-boto3-codeconnections<1.35.0,>=1.34.0
+
 [codedeploy]
 mypy-boto3-codedeploy<1.35.0,>=1.34.0
 
 [codeguru-reviewer]
 mypy-boto3-codeguru-reviewer<1.35.0,>=1.34.0
 
 [codeguru-security]
@@ -646,14 +662,17 @@
 
 [connectcases]
 mypy-boto3-connectcases<1.35.0,>=1.34.0
 
 [connectparticipant]
 mypy-boto3-connectparticipant<1.35.0,>=1.34.0
 
+[controlcatalog]
+mypy-boto3-controlcatalog<1.35.0,>=1.34.0
+
 [controltower]
 mypy-boto3-controltower<1.35.0,>=1.34.0
 
 [cost-optimization-hub]
 mypy-boto3-cost-optimization-hub<1.35.0,>=1.34.0
 
 [cur]
@@ -676,14 +695,17 @@
 
 [datazone]
 mypy-boto3-datazone<1.35.0,>=1.34.0
 
 [dax]
 mypy-boto3-dax<1.35.0,>=1.34.0
 
+[deadline]
+mypy-boto3-deadline<1.35.0,>=1.34.0
+
 [detective]
 mypy-boto3-detective<1.35.0,>=1.34.0
 
 [devicefarm]
 mypy-boto3-devicefarm<1.35.0,>=1.34.0
 
 [devops-guru]
@@ -889,17 +911,14 @@
 
 [iot-data]
 mypy-boto3-iot-data<1.35.0,>=1.34.0
 
 [iot-jobs-data]
 mypy-boto3-iot-jobs-data<1.35.0,>=1.34.0
 
-[iot-roborunner]
-mypy-boto3-iot-roborunner<1.35.0,>=1.34.0
-
 [iot1click-devices]
 mypy-boto3-iot1click-devices<1.35.0,>=1.34.0
 
 [iot1click-projects]
 mypy-boto3-iot1click-projects<1.35.0,>=1.34.0
 
 [iotanalytics]
@@ -1300,14 +1319,17 @@
 
 [route53-recovery-readiness]
 mypy-boto3-route53-recovery-readiness<1.35.0,>=1.34.0
 
 [route53domains]
 mypy-boto3-route53domains<1.35.0,>=1.34.0
 
+[route53profiles]
+mypy-boto3-route53profiles<1.35.0,>=1.34.0
+
 [route53resolver]
 mypy-boto3-route53resolver<1.35.0,>=1.34.0
 
 [rum]
 mypy-boto3-rum<1.35.0,>=1.34.0
 
 [s3]
@@ -1435,14 +1457,17 @@
 
 [storagegateway]
 mypy-boto3-storagegateway<1.35.0,>=1.34.0
 
 [sts]
 mypy-boto3-sts<1.35.0,>=1.34.0
 
+[supplychain]
+mypy-boto3-supplychain<1.35.0,>=1.34.0
+
 [support]
 mypy-boto3-support<1.35.0,>=1.34.0
 
 [support-app]
 mypy-boto3-support-app<1.35.0,>=1.34.0
 
 [swf]
@@ -1450,14 +1475,17 @@
 
 [synthetics]
 mypy-boto3-synthetics<1.35.0,>=1.34.0
 
 [textract]
 mypy-boto3-textract<1.35.0,>=1.34.0
 
+[timestream-influxdb]
+mypy-boto3-timestream-influxdb<1.35.0,>=1.34.0
+
 [timestream-query]
 mypy-boto3-timestream-query<1.35.0,>=1.34.0
 
 [timestream-write]
 mypy-boto3-timestream-write<1.35.0,>=1.34.0
 
 [tnb]
```

### Comparing `boto3-stubs-1.34.9/setup.py` & `boto3_stubs-1.34.90/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="boto3-stubs",
-    version="1.34.9",
+    version="1.34.90",
     packages=["boto3-stubs"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description="Type annotations for boto3 1.34.9 generated with mypy-boto3-builder 7.23.0",
+    description="Type annotations for boto3 1.34.90 generated with mypy-boto3-builder 7.23.2",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
@@ -74,14 +74,15 @@
             "mypy-boto3-application-insights>=1.34.0, <1.35.0",
             "mypy-boto3-applicationcostprofiler>=1.34.0, <1.35.0",
             "mypy-boto3-appmesh>=1.34.0, <1.35.0",
             "mypy-boto3-apprunner>=1.34.0, <1.35.0",
             "mypy-boto3-appstream>=1.34.0, <1.35.0",
             "mypy-boto3-appsync>=1.34.0, <1.35.0",
             "mypy-boto3-arc-zonal-shift>=1.34.0, <1.35.0",
+            "mypy-boto3-artifact>=1.34.0, <1.35.0",
             "mypy-boto3-athena>=1.34.0, <1.35.0",
             "mypy-boto3-auditmanager>=1.34.0, <1.35.0",
             "mypy-boto3-autoscaling>=1.34.0, <1.35.0",
             "mypy-boto3-autoscaling-plans>=1.34.0, <1.35.0",
             "mypy-boto3-b2bi>=1.34.0, <1.35.0",
             "mypy-boto3-backup>=1.34.0, <1.35.0",
             "mypy-boto3-backup-gateway>=1.34.0, <1.35.0",
@@ -92,14 +93,15 @@
             "mypy-boto3-bedrock-agent>=1.34.0, <1.35.0",
             "mypy-boto3-bedrock-agent-runtime>=1.34.0, <1.35.0",
             "mypy-boto3-bedrock-runtime>=1.34.0, <1.35.0",
             "mypy-boto3-billingconductor>=1.34.0, <1.35.0",
             "mypy-boto3-braket>=1.34.0, <1.35.0",
             "mypy-boto3-budgets>=1.34.0, <1.35.0",
             "mypy-boto3-ce>=1.34.0, <1.35.0",
+            "mypy-boto3-chatbot>=1.34.0, <1.35.0",
             "mypy-boto3-chime>=1.34.0, <1.35.0",
             "mypy-boto3-chime-sdk-identity>=1.34.0, <1.35.0",
             "mypy-boto3-chime-sdk-media-pipelines>=1.34.0, <1.35.0",
             "mypy-boto3-chime-sdk-meetings>=1.34.0, <1.35.0",
             "mypy-boto3-chime-sdk-messaging>=1.34.0, <1.35.0",
             "mypy-boto3-chime-sdk-voice>=1.34.0, <1.35.0",
             "mypy-boto3-cleanrooms>=1.34.0, <1.35.0",
@@ -117,14 +119,15 @@
             "mypy-boto3-cloudtrail>=1.34.0, <1.35.0",
             "mypy-boto3-cloudtrail-data>=1.34.0, <1.35.0",
             "mypy-boto3-cloudwatch>=1.34.0, <1.35.0",
             "mypy-boto3-codeartifact>=1.34.0, <1.35.0",
             "mypy-boto3-codebuild>=1.34.0, <1.35.0",
             "mypy-boto3-codecatalyst>=1.34.0, <1.35.0",
             "mypy-boto3-codecommit>=1.34.0, <1.35.0",
+            "mypy-boto3-codeconnections>=1.34.0, <1.35.0",
             "mypy-boto3-codedeploy>=1.34.0, <1.35.0",
             "mypy-boto3-codeguru-reviewer>=1.34.0, <1.35.0",
             "mypy-boto3-codeguru-security>=1.34.0, <1.35.0",
             "mypy-boto3-codeguruprofiler>=1.34.0, <1.35.0",
             "mypy-boto3-codepipeline>=1.34.0, <1.35.0",
             "mypy-boto3-codestar>=1.34.0, <1.35.0",
             "mypy-boto3-codestar-connections>=1.34.0, <1.35.0",
@@ -137,24 +140,26 @@
             "mypy-boto3-compute-optimizer>=1.34.0, <1.35.0",
             "mypy-boto3-config>=1.34.0, <1.35.0",
             "mypy-boto3-connect>=1.34.0, <1.35.0",
             "mypy-boto3-connect-contact-lens>=1.34.0, <1.35.0",
             "mypy-boto3-connectcampaigns>=1.34.0, <1.35.0",
             "mypy-boto3-connectcases>=1.34.0, <1.35.0",
             "mypy-boto3-connectparticipant>=1.34.0, <1.35.0",
+            "mypy-boto3-controlcatalog>=1.34.0, <1.35.0",
             "mypy-boto3-controltower>=1.34.0, <1.35.0",
             "mypy-boto3-cost-optimization-hub>=1.34.0, <1.35.0",
             "mypy-boto3-cur>=1.34.0, <1.35.0",
             "mypy-boto3-customer-profiles>=1.34.0, <1.35.0",
             "mypy-boto3-databrew>=1.34.0, <1.35.0",
             "mypy-boto3-dataexchange>=1.34.0, <1.35.0",
             "mypy-boto3-datapipeline>=1.34.0, <1.35.0",
             "mypy-boto3-datasync>=1.34.0, <1.35.0",
             "mypy-boto3-datazone>=1.34.0, <1.35.0",
             "mypy-boto3-dax>=1.34.0, <1.35.0",
+            "mypy-boto3-deadline>=1.34.0, <1.35.0",
             "mypy-boto3-detective>=1.34.0, <1.35.0",
             "mypy-boto3-devicefarm>=1.34.0, <1.35.0",
             "mypy-boto3-devops-guru>=1.34.0, <1.35.0",
             "mypy-boto3-directconnect>=1.34.0, <1.35.0",
             "mypy-boto3-discovery>=1.34.0, <1.35.0",
             "mypy-boto3-dlm>=1.34.0, <1.35.0",
             "mypy-boto3-dms>=1.34.0, <1.35.0",
@@ -215,15 +220,14 @@
             "mypy-boto3-inspector>=1.34.0, <1.35.0",
             "mypy-boto3-inspector-scan>=1.34.0, <1.35.0",
             "mypy-boto3-inspector2>=1.34.0, <1.35.0",
             "mypy-boto3-internetmonitor>=1.34.0, <1.35.0",
             "mypy-boto3-iot>=1.34.0, <1.35.0",
             "mypy-boto3-iot-data>=1.34.0, <1.35.0",
             "mypy-boto3-iot-jobs-data>=1.34.0, <1.35.0",
-            "mypy-boto3-iot-roborunner>=1.34.0, <1.35.0",
             "mypy-boto3-iot1click-devices>=1.34.0, <1.35.0",
             "mypy-boto3-iot1click-projects>=1.34.0, <1.35.0",
             "mypy-boto3-iotanalytics>=1.34.0, <1.35.0",
             "mypy-boto3-iotdeviceadvisor>=1.34.0, <1.35.0",
             "mypy-boto3-iotevents>=1.34.0, <1.35.0",
             "mypy-boto3-iotevents-data>=1.34.0, <1.35.0",
             "mypy-boto3-iotfleethub>=1.34.0, <1.35.0",
@@ -352,14 +356,15 @@
             "mypy-boto3-robomaker>=1.34.0, <1.35.0",
             "mypy-boto3-rolesanywhere>=1.34.0, <1.35.0",
             "mypy-boto3-route53>=1.34.0, <1.35.0",
             "mypy-boto3-route53-recovery-cluster>=1.34.0, <1.35.0",
             "mypy-boto3-route53-recovery-control-config>=1.34.0, <1.35.0",
             "mypy-boto3-route53-recovery-readiness>=1.34.0, <1.35.0",
             "mypy-boto3-route53domains>=1.34.0, <1.35.0",
+            "mypy-boto3-route53profiles>=1.34.0, <1.35.0",
             "mypy-boto3-route53resolver>=1.34.0, <1.35.0",
             "mypy-boto3-rum>=1.34.0, <1.35.0",
             "mypy-boto3-s3>=1.34.0, <1.35.0",
             "mypy-boto3-s3control>=1.34.0, <1.35.0",
             "mypy-boto3-s3outposts>=1.34.0, <1.35.0",
             "mypy-boto3-sagemaker>=1.34.0, <1.35.0",
             "mypy-boto3-sagemaker-a2i-runtime>=1.34.0, <1.35.0",
@@ -397,19 +402,21 @@
             "mypy-boto3-ssm-sap>=1.34.0, <1.35.0",
             "mypy-boto3-sso>=1.34.0, <1.35.0",
             "mypy-boto3-sso-admin>=1.34.0, <1.35.0",
             "mypy-boto3-sso-oidc>=1.34.0, <1.35.0",
             "mypy-boto3-stepfunctions>=1.34.0, <1.35.0",
             "mypy-boto3-storagegateway>=1.34.0, <1.35.0",
             "mypy-boto3-sts>=1.34.0, <1.35.0",
+            "mypy-boto3-supplychain>=1.34.0, <1.35.0",
             "mypy-boto3-support>=1.34.0, <1.35.0",
             "mypy-boto3-support-app>=1.34.0, <1.35.0",
             "mypy-boto3-swf>=1.34.0, <1.35.0",
             "mypy-boto3-synthetics>=1.34.0, <1.35.0",
             "mypy-boto3-textract>=1.34.0, <1.35.0",
+            "mypy-boto3-timestream-influxdb>=1.34.0, <1.35.0",
             "mypy-boto3-timestream-query>=1.34.0, <1.35.0",
             "mypy-boto3-timestream-write>=1.34.0, <1.35.0",
             "mypy-boto3-tnb>=1.34.0, <1.35.0",
             "mypy-boto3-transcribe>=1.34.0, <1.35.0",
             "mypy-boto3-transfer>=1.34.0, <1.35.0",
             "mypy-boto3-translate>=1.34.0, <1.35.0",
             "mypy-boto3-trustedadvisor>=1.34.0, <1.35.0",
@@ -435,15 +442,15 @@
             "mypy-boto3-dynamodb>=1.34.0, <1.35.0",
             "mypy-boto3-ec2>=1.34.0, <1.35.0",
             "mypy-boto3-lambda>=1.34.0, <1.35.0",
             "mypy-boto3-rds>=1.34.0, <1.35.0",
             "mypy-boto3-s3>=1.34.0, <1.35.0",
             "mypy-boto3-sqs>=1.34.0, <1.35.0",
         ],
-        "boto3": ["boto3==1.34.9", "botocore==1.34.9"],
+        "boto3": ["boto3==1.34.90", "botocore==1.34.90"],
         "accessanalyzer": ["mypy-boto3-accessanalyzer>=1.34.0, <1.35.0"],
         "account": ["mypy-boto3-account>=1.34.0, <1.35.0"],
         "acm": ["mypy-boto3-acm>=1.34.0, <1.35.0"],
         "acm-pca": ["mypy-boto3-acm-pca>=1.34.0, <1.35.0"],
         "alexaforbusiness": ["mypy-boto3-alexaforbusiness>=1.34.0, <1.35.0"],
         "amp": ["mypy-boto3-amp>=1.34.0, <1.35.0"],
         "amplify": ["mypy-boto3-amplify>=1.34.0, <1.35.0"],
@@ -461,14 +468,15 @@
         "application-insights": ["mypy-boto3-application-insights>=1.34.0, <1.35.0"],
         "applicationcostprofiler": ["mypy-boto3-applicationcostprofiler>=1.34.0, <1.35.0"],
         "appmesh": ["mypy-boto3-appmesh>=1.34.0, <1.35.0"],
         "apprunner": ["mypy-boto3-apprunner>=1.34.0, <1.35.0"],
         "appstream": ["mypy-boto3-appstream>=1.34.0, <1.35.0"],
         "appsync": ["mypy-boto3-appsync>=1.34.0, <1.35.0"],
         "arc-zonal-shift": ["mypy-boto3-arc-zonal-shift>=1.34.0, <1.35.0"],
+        "artifact": ["mypy-boto3-artifact>=1.34.0, <1.35.0"],
         "athena": ["mypy-boto3-athena>=1.34.0, <1.35.0"],
         "auditmanager": ["mypy-boto3-auditmanager>=1.34.0, <1.35.0"],
         "autoscaling": ["mypy-boto3-autoscaling>=1.34.0, <1.35.0"],
         "autoscaling-plans": ["mypy-boto3-autoscaling-plans>=1.34.0, <1.35.0"],
         "b2bi": ["mypy-boto3-b2bi>=1.34.0, <1.35.0"],
         "backup": ["mypy-boto3-backup>=1.34.0, <1.35.0"],
         "backup-gateway": ["mypy-boto3-backup-gateway>=1.34.0, <1.35.0"],
@@ -479,14 +487,15 @@
         "bedrock-agent": ["mypy-boto3-bedrock-agent>=1.34.0, <1.35.0"],
         "bedrock-agent-runtime": ["mypy-boto3-bedrock-agent-runtime>=1.34.0, <1.35.0"],
         "bedrock-runtime": ["mypy-boto3-bedrock-runtime>=1.34.0, <1.35.0"],
         "billingconductor": ["mypy-boto3-billingconductor>=1.34.0, <1.35.0"],
         "braket": ["mypy-boto3-braket>=1.34.0, <1.35.0"],
         "budgets": ["mypy-boto3-budgets>=1.34.0, <1.35.0"],
         "ce": ["mypy-boto3-ce>=1.34.0, <1.35.0"],
+        "chatbot": ["mypy-boto3-chatbot>=1.34.0, <1.35.0"],
         "chime": ["mypy-boto3-chime>=1.34.0, <1.35.0"],
         "chime-sdk-identity": ["mypy-boto3-chime-sdk-identity>=1.34.0, <1.35.0"],
         "chime-sdk-media-pipelines": ["mypy-boto3-chime-sdk-media-pipelines>=1.34.0, <1.35.0"],
         "chime-sdk-meetings": ["mypy-boto3-chime-sdk-meetings>=1.34.0, <1.35.0"],
         "chime-sdk-messaging": ["mypy-boto3-chime-sdk-messaging>=1.34.0, <1.35.0"],
         "chime-sdk-voice": ["mypy-boto3-chime-sdk-voice>=1.34.0, <1.35.0"],
         "cleanrooms": ["mypy-boto3-cleanrooms>=1.34.0, <1.35.0"],
@@ -504,14 +513,15 @@
         "cloudtrail": ["mypy-boto3-cloudtrail>=1.34.0, <1.35.0"],
         "cloudtrail-data": ["mypy-boto3-cloudtrail-data>=1.34.0, <1.35.0"],
         "cloudwatch": ["mypy-boto3-cloudwatch>=1.34.0, <1.35.0"],
         "codeartifact": ["mypy-boto3-codeartifact>=1.34.0, <1.35.0"],
         "codebuild": ["mypy-boto3-codebuild>=1.34.0, <1.35.0"],
         "codecatalyst": ["mypy-boto3-codecatalyst>=1.34.0, <1.35.0"],
         "codecommit": ["mypy-boto3-codecommit>=1.34.0, <1.35.0"],
+        "codeconnections": ["mypy-boto3-codeconnections>=1.34.0, <1.35.0"],
         "codedeploy": ["mypy-boto3-codedeploy>=1.34.0, <1.35.0"],
         "codeguru-reviewer": ["mypy-boto3-codeguru-reviewer>=1.34.0, <1.35.0"],
         "codeguru-security": ["mypy-boto3-codeguru-security>=1.34.0, <1.35.0"],
         "codeguruprofiler": ["mypy-boto3-codeguruprofiler>=1.34.0, <1.35.0"],
         "codepipeline": ["mypy-boto3-codepipeline>=1.34.0, <1.35.0"],
         "codestar": ["mypy-boto3-codestar>=1.34.0, <1.35.0"],
         "codestar-connections": ["mypy-boto3-codestar-connections>=1.34.0, <1.35.0"],
@@ -524,24 +534,26 @@
         "compute-optimizer": ["mypy-boto3-compute-optimizer>=1.34.0, <1.35.0"],
         "config": ["mypy-boto3-config>=1.34.0, <1.35.0"],
         "connect": ["mypy-boto3-connect>=1.34.0, <1.35.0"],
         "connect-contact-lens": ["mypy-boto3-connect-contact-lens>=1.34.0, <1.35.0"],
         "connectcampaigns": ["mypy-boto3-connectcampaigns>=1.34.0, <1.35.0"],
         "connectcases": ["mypy-boto3-connectcases>=1.34.0, <1.35.0"],
         "connectparticipant": ["mypy-boto3-connectparticipant>=1.34.0, <1.35.0"],
+        "controlcatalog": ["mypy-boto3-controlcatalog>=1.34.0, <1.35.0"],
         "controltower": ["mypy-boto3-controltower>=1.34.0, <1.35.0"],
         "cost-optimization-hub": ["mypy-boto3-cost-optimization-hub>=1.34.0, <1.35.0"],
         "cur": ["mypy-boto3-cur>=1.34.0, <1.35.0"],
         "customer-profiles": ["mypy-boto3-customer-profiles>=1.34.0, <1.35.0"],
         "databrew": ["mypy-boto3-databrew>=1.34.0, <1.35.0"],
         "dataexchange": ["mypy-boto3-dataexchange>=1.34.0, <1.35.0"],
         "datapipeline": ["mypy-boto3-datapipeline>=1.34.0, <1.35.0"],
         "datasync": ["mypy-boto3-datasync>=1.34.0, <1.35.0"],
         "datazone": ["mypy-boto3-datazone>=1.34.0, <1.35.0"],
         "dax": ["mypy-boto3-dax>=1.34.0, <1.35.0"],
+        "deadline": ["mypy-boto3-deadline>=1.34.0, <1.35.0"],
         "detective": ["mypy-boto3-detective>=1.34.0, <1.35.0"],
         "devicefarm": ["mypy-boto3-devicefarm>=1.34.0, <1.35.0"],
         "devops-guru": ["mypy-boto3-devops-guru>=1.34.0, <1.35.0"],
         "directconnect": ["mypy-boto3-directconnect>=1.34.0, <1.35.0"],
         "discovery": ["mypy-boto3-discovery>=1.34.0, <1.35.0"],
         "dlm": ["mypy-boto3-dlm>=1.34.0, <1.35.0"],
         "dms": ["mypy-boto3-dms>=1.34.0, <1.35.0"],
@@ -602,15 +614,14 @@
         "inspector": ["mypy-boto3-inspector>=1.34.0, <1.35.0"],
         "inspector-scan": ["mypy-boto3-inspector-scan>=1.34.0, <1.35.0"],
         "inspector2": ["mypy-boto3-inspector2>=1.34.0, <1.35.0"],
         "internetmonitor": ["mypy-boto3-internetmonitor>=1.34.0, <1.35.0"],
         "iot": ["mypy-boto3-iot>=1.34.0, <1.35.0"],
         "iot-data": ["mypy-boto3-iot-data>=1.34.0, <1.35.0"],
         "iot-jobs-data": ["mypy-boto3-iot-jobs-data>=1.34.0, <1.35.0"],
-        "iot-roborunner": ["mypy-boto3-iot-roborunner>=1.34.0, <1.35.0"],
         "iot1click-devices": ["mypy-boto3-iot1click-devices>=1.34.0, <1.35.0"],
         "iot1click-projects": ["mypy-boto3-iot1click-projects>=1.34.0, <1.35.0"],
         "iotanalytics": ["mypy-boto3-iotanalytics>=1.34.0, <1.35.0"],
         "iotdeviceadvisor": ["mypy-boto3-iotdeviceadvisor>=1.34.0, <1.35.0"],
         "iotevents": ["mypy-boto3-iotevents>=1.34.0, <1.35.0"],
         "iotevents-data": ["mypy-boto3-iotevents-data>=1.34.0, <1.35.0"],
         "iotfleethub": ["mypy-boto3-iotfleethub>=1.34.0, <1.35.0"],
@@ -753,14 +764,15 @@
         "route53": ["mypy-boto3-route53>=1.34.0, <1.35.0"],
         "route53-recovery-cluster": ["mypy-boto3-route53-recovery-cluster>=1.34.0, <1.35.0"],
         "route53-recovery-control-config": [
             "mypy-boto3-route53-recovery-control-config>=1.34.0, <1.35.0"
         ],
         "route53-recovery-readiness": ["mypy-boto3-route53-recovery-readiness>=1.34.0, <1.35.0"],
         "route53domains": ["mypy-boto3-route53domains>=1.34.0, <1.35.0"],
+        "route53profiles": ["mypy-boto3-route53profiles>=1.34.0, <1.35.0"],
         "route53resolver": ["mypy-boto3-route53resolver>=1.34.0, <1.35.0"],
         "rum": ["mypy-boto3-rum>=1.34.0, <1.35.0"],
         "s3": ["mypy-boto3-s3>=1.34.0, <1.35.0"],
         "s3control": ["mypy-boto3-s3control>=1.34.0, <1.35.0"],
         "s3outposts": ["mypy-boto3-s3outposts>=1.34.0, <1.35.0"],
         "sagemaker": ["mypy-boto3-sagemaker>=1.34.0, <1.35.0"],
         "sagemaker-a2i-runtime": ["mypy-boto3-sagemaker-a2i-runtime>=1.34.0, <1.35.0"],
@@ -800,19 +812,21 @@
         "ssm-sap": ["mypy-boto3-ssm-sap>=1.34.0, <1.35.0"],
         "sso": ["mypy-boto3-sso>=1.34.0, <1.35.0"],
         "sso-admin": ["mypy-boto3-sso-admin>=1.34.0, <1.35.0"],
         "sso-oidc": ["mypy-boto3-sso-oidc>=1.34.0, <1.35.0"],
         "stepfunctions": ["mypy-boto3-stepfunctions>=1.34.0, <1.35.0"],
         "storagegateway": ["mypy-boto3-storagegateway>=1.34.0, <1.35.0"],
         "sts": ["mypy-boto3-sts>=1.34.0, <1.35.0"],
+        "supplychain": ["mypy-boto3-supplychain>=1.34.0, <1.35.0"],
         "support": ["mypy-boto3-support>=1.34.0, <1.35.0"],
         "support-app": ["mypy-boto3-support-app>=1.34.0, <1.35.0"],
         "swf": ["mypy-boto3-swf>=1.34.0, <1.35.0"],
         "synthetics": ["mypy-boto3-synthetics>=1.34.0, <1.35.0"],
         "textract": ["mypy-boto3-textract>=1.34.0, <1.35.0"],
+        "timestream-influxdb": ["mypy-boto3-timestream-influxdb>=1.34.0, <1.35.0"],
         "timestream-query": ["mypy-boto3-timestream-query>=1.34.0, <1.35.0"],
         "timestream-write": ["mypy-boto3-timestream-write>=1.34.0, <1.35.0"],
         "tnb": ["mypy-boto3-tnb>=1.34.0, <1.35.0"],
         "transcribe": ["mypy-boto3-transcribe>=1.34.0, <1.35.0"],
         "transfer": ["mypy-boto3-transfer>=1.34.0, <1.35.0"],
         "translate": ["mypy-boto3-translate>=1.34.0, <1.35.0"],
         "trustedadvisor": ["mypy-boto3-trustedadvisor>=1.34.0, <1.35.0"],
```


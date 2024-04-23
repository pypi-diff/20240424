# Comparing `tmp/gantry-logger-0.0.2a5.tar.gz` & `tmp/gantry_logger-0.0.2a6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gantry-logger-0.0.2a5.tar", last modified: Fri Mar 29 17:34:52 2024, max compression
+gzip compressed data, was "gantry_logger-0.0.2a6.tar", last modified: Tue Apr 23 23:48:47 2024, max compression
```

## Comparing `gantry-logger-0.0.2a5.tar` & `gantry_logger-0.0.2a6.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 17:34:52.070348 gantry-logger-0.0.2a5/
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-03-29 17:34:52.070348 gantry-logger-0.0.2a5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-03-29 17:34:44.000000 gantry-logger-0.0.2a5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-03-29 17:34:52.070348 gantry-logger-0.0.2a5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-03-29 17:34:44.000000 gantry-logger-0.0.2a5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 17:34:52.054347 gantry-logger-0.0.2a5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 17:34:52.058348 gantry-logger-0.0.2a5/src/gantry/
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-03-29 17:34:44.000000 gantry-logger-0.0.2a5/src/gantry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6435 2024-03-29 17:34:44.000000 gantry-logger-0.0.2a5/src/gantry/evaluations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 17:34:52.058348 gantry-logger-0.0.2a5/src/gantry/logger/
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-03-29 17:34:44.000000 gantry-logger-0.0.2a5/src/gantry/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5087 2024-03-29 17:34:44.000000 gantry-logger-0.0.2a5/src/gantry/logger/consumer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4776 2024-03-29 17:34:44.000000 gantry-logger-0.0.2a5/src/gantry/logger/eval_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-03-29 17:34:44.000000 gantry-logger-0.0.2a5/src/gantry/logger/eval_reports.py
--rw-r--r--   0 runner    (1001) docker     (127)     8014 2024-03-29 17:34:44.000000 gantry-logger-0.0.2a5/src/gantry/logger/langchain_callback.py
--rw-r--r--   0 runner    (1001) docker     (127)     5689 2024-03-29 17:34:44.000000 gantry-logger-0.0.2a5/src/gantry/logger/log_location.py
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-03-29 17:34:44.000000 gantry-logger-0.0.2a5/src/gantry/logger/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2528 2024-03-29 17:34:44.000000 gantry-logger-0.0.2a5/src/gantry/logs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 17:34:52.058348 gantry-logger-0.0.2a5/src/gantry/models/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-03-29 17:34:44.000000 gantry-logger-0.0.2a5/src/gantry/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 17:34:52.066348 gantry-logger-0.0.2a5/src/gantry/models/components/
--rw-r--r--   0 runner    (1001) docker     (127)     2412 2024-03-29 17:34:44.000000 gantry-logger-0.0.2a5/src/gantry/models/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-03-29 17:34:44.000000 gantry-logger-0.0.2a5/src/gantry/models/components/createragevaluationrequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-03-29 17:34:44.000000 gantry-logger-0.0.2a5/src/gantry/models/components/criteriafeedback.py
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-03-29 17:34:44.000000 gantry-logger-0.0.2a5/src/gantry/models/components/criteriaresultcapture.py
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-03-29 17:34:44.000000 gantry-logger-0.0.2a5/src/gantry/models/components/criteriastats.py
--rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-03-29 17:34:44.000000 gantry-logger-0.0.2a5/src/gantry/models/components/criteriastatuscount.py
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-03-29 17:34:44.000000 gantry-logger-0.0.2a5/src/gantry/models/components/customstep.py
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-03-29 17:34:44.000000 gantry-logger-0.0.2a5/src/gantry/models/components/document.py
--rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-03-29 17:34:44.000000 gantry-logger-0.0.2a5/src/gantry/models/components/evalcriteria.py
--rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-03-29 17:34:44.000000 gantry-logger-0.0.2a5/src/gantry/models/components/evalstats.py
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-03-29 17:34:44.000000 gantry-logger-0.0.2a5/src/gantry/models/components/evaluationcriteriastatus.py
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-03-29 17:34:44.000000 gantry-logger-0.0.2a5/src/gantry/models/components/evaluationrecordstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     3836 2024-03-29 17:34:44.000000 gantry-logger-0.0.2a5/src/gantry/models/components/evaluationrun.py
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-03-29 17:34:44.000000 gantry-logger-0.0.2a5/src/gantry/models/components/evaluationrunjobstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-03-29 17:34:44.000000 gantry-logger-0.0.2a5/src/gantry/models/components/evaluationrunpreupload.py
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-03-29 17:34:44.000000 gantry-logger-0.0.2a5/src/gantry/models/components/evaluationrunpreuploadresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-03-29 17:34:44.000000 gantry-logger-0.0.2a5/src/gantry/models/components/evaluationrunresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-03-29 17:34:44.000000 gantry-logger-0.0.2a5/src/gantry/models/components/functionstep.py
--rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-03-29 17:34:44.000000 gantry-logger-0.0.2a5/src/gantry/models/components/getlogssummaryrequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-03-29 17:34:44.000000 gantry-logger-0.0.2a5/src/gantry/models/components/getragevaluationresultsresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-03-29 17:34:44.000000 gantry-logger-0.0.2a5/src/gantry/models/components/getragevaluationresultsresponseresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-03-29 17:34:44.000000 gantry-logger-0.0.2a5/src/gantry/models/components/llmevaluationcriteriatype.py
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-03-29 17:34:44.000000 gantry-logger-0.0.2a5/src/gantry/models/components/llmevaluationerrortype.py
--rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-03-29 17:34:44.000000 gantry-logger-0.0.2a5/src/gantry/models/components/llmstep.py
--rw-r--r--   0 runner    (1001) docker     (127)      855 2024-03-29 17:34:44.000000 gantry-logger-0.0.2a5/src/gantry/models/components/logragrecordrequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-03-29 17:34:44.000000 gantry-logger-0.0.2a5/src/gantry/models/components/logragrecordresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      817 2024-03-29 17:34:44.000000 gantry-logger-0.0.2a5/src/gantry/models/components/logragrecordresponseresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-03-29 17:34:44.000000 gantry-logger-0.0.2a5/src/gantry/models/components/message.py
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-03-29 17:34:44.000000 gantry-logger-0.0.2a5/src/gantry/models/components/organizationtier.py
--rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-03-29 17:34:44.000000 gantry-logger-0.0.2a5/src/gantry/models/components/orguser.py
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-03-29 17:34:44.000000 gantry-logger-0.0.2a5/src/gantry/models/components/passfailunsurerubricscalevalues.py
--rw-r--r--   0 runner    (1001) docker     (127)     3451 2024-03-29 17:34:44.000000 gantry-logger-0.0.2a5/src/gantry/models/components/ragcriteriaresult.py
--rw-r--r--   0 runner    (1001) docker     (127)     2080 2024-03-29 17:34:44.000000 gantry-logger-0.0.2a5/src/gantry/models/components/ragevaluationresult.py
--rw-r--r--   0 runner    (1001) docker     (127)     1871 2024-03-29 17:34:44.000000 gantry-logger-0.0.2a5/src/gantry/models/components/ragrecord.py
--rw-r--r--   0 runner    (1001) docker     (127)      860 2024-03-29 17:34:44.000000 gantry-logger-0.0.2a5/src/gantry/models/components/recordstatuscount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-03-29 17:34:44.000000 gantry-logger-0.0.2a5/src/gantry/models/components/retrievalstep.py
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-03-29 17:34:44.000000 gantry-logger-0.0.2a5/src/gantry/models/components/security.py
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-03-29 17:34:44.000000 gantry-logger-0.0.2a5/src/gantry/models/components/stepformat.py
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-03-29 17:34:44.000000 gantry-logger-0.0.2a5/src/gantry/models/components/summarynotesresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-03-29 17:34:44.000000 gantry-logger-0.0.2a5/src/gantry/models/components/topicstats.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 17:34:52.066348 gantry-logger-0.0.2a5/src/gantry/models/errors/
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-03-29 17:34:44.000000 gantry-logger-0.0.2a5/src/gantry/models/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-03-29 17:34:44.000000 gantry-logger-0.0.2a5/src/gantry/models/errors/sdkerror.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 17:34:52.070348 gantry-logger-0.0.2a5/src/gantry/models/operations/
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-03-29 17:34:44.000000 gantry-logger-0.0.2a5/src/gantry/models/operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      876 2024-03-29 17:34:44.000000 gantry-logger-0.0.2a5/src/gantry/models/operations/create_evaluation_run_pre_upload.py
--rw-r--r--   0 runner    (1001) docker     (127)      823 2024-03-29 17:34:44.000000 gantry-logger-0.0.2a5/src/gantry/models/operations/create_rag_evaluation_run.py
--rw-r--r--   0 runner    (1001) docker     (127)     1979 2024-03-29 17:34:44.000000 gantry-logger-0.0.2a5/src/gantry/models/operations/get_rag_evaluation_results.py
--rw-r--r--   0 runner    (1001) docker     (127)      851 2024-03-29 17:34:44.000000 gantry-logger-0.0.2a5/src/gantry/models/operations/log_rag_records.py
--rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-03-29 17:34:44.000000 gantry-logger-0.0.2a5/src/gantry/sdk.py
--rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-03-29 17:34:44.000000 gantry-logger-0.0.2a5/src/gantry/sdkconfiguration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 17:34:52.070348 gantry-logger-0.0.2a5/src/gantry/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-03-29 17:34:44.000000 gantry-logger-0.0.2a5/src/gantry/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3786 2024-03-29 17:34:44.000000 gantry-logger-0.0.2a5/src/gantry/utils/retries.py
--rw-r--r--   0 runner    (1001) docker     (127)    29680 2024-03-29 17:34:44.000000 gantry-logger-0.0.2a5/src/gantry/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 17:34:52.070348 gantry-logger-0.0.2a5/src/gantry_logger.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-03-29 17:34:52.000000 gantry-logger-0.0.2a5/src/gantry_logger.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3059 2024-03-29 17:34:52.000000 gantry-logger-0.0.2a5/src/gantry_logger.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 17:34:52.000000 gantry-logger-0.0.2a5/src/gantry_logger.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-03-29 17:34:52.000000 gantry-logger-0.0.2a5/src/gantry_logger.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-29 17:34:52.000000 gantry-logger-0.0.2a5/src/gantry_logger.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:48:47.426418 gantry_logger-0.0.2a6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-04-23 23:48:47.426418 gantry_logger-0.0.2a6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-23 23:48:40.000000 gantry_logger-0.0.2a6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-23 23:48:47.426418 gantry_logger-0.0.2a6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-04-23 23:48:40.000000 gantry_logger-0.0.2a6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:48:47.414418 gantry_logger-0.0.2a6/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:48:47.414418 gantry_logger-0.0.2a6/src/gantry/
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-23 23:48:40.000000 gantry_logger-0.0.2a6/src/gantry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6435 2024-04-23 23:48:40.000000 gantry_logger-0.0.2a6/src/gantry/evaluations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:48:47.414418 gantry_logger-0.0.2a6/src/gantry/logger/
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-23 23:48:40.000000 gantry_logger-0.0.2a6/src/gantry/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5087 2024-04-23 23:48:40.000000 gantry_logger-0.0.2a6/src/gantry/logger/consumer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4954 2024-04-23 23:48:40.000000 gantry_logger-0.0.2a6/src/gantry/logger/eval_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-23 23:48:40.000000 gantry_logger-0.0.2a6/src/gantry/logger/eval_reports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8014 2024-04-23 23:48:40.000000 gantry_logger-0.0.2a6/src/gantry/logger/langchain_callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5689 2024-04-23 23:48:40.000000 gantry_logger-0.0.2a6/src/gantry/logger/log_location.py
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-23 23:48:40.000000 gantry_logger-0.0.2a6/src/gantry/logger/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2528 2024-04-23 23:48:40.000000 gantry_logger-0.0.2a6/src/gantry/logs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:48:47.414418 gantry_logger-0.0.2a6/src/gantry/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-23 23:48:40.000000 gantry_logger-0.0.2a6/src/gantry/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:48:47.422418 gantry_logger-0.0.2a6/src/gantry/models/components/
+-rw-r--r--   0 runner    (1001) docker     (127)     2412 2024-04-23 23:48:40.000000 gantry_logger-0.0.2a6/src/gantry/models/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-04-23 23:48:40.000000 gantry_logger-0.0.2a6/src/gantry/models/components/createragevaluationrequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-04-23 23:48:40.000000 gantry_logger-0.0.2a6/src/gantry/models/components/criteriafeedback.py
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-23 23:48:40.000000 gantry_logger-0.0.2a6/src/gantry/models/components/criteriaresultcapture.py
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-04-23 23:48:40.000000 gantry_logger-0.0.2a6/src/gantry/models/components/criteriastats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-04-23 23:48:40.000000 gantry_logger-0.0.2a6/src/gantry/models/components/criteriastatuscount.py
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-23 23:48:40.000000 gantry_logger-0.0.2a6/src/gantry/models/components/customstep.py
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-23 23:48:40.000000 gantry_logger-0.0.2a6/src/gantry/models/components/document.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-04-23 23:48:40.000000 gantry_logger-0.0.2a6/src/gantry/models/components/evalcriteria.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-04-23 23:48:40.000000 gantry_logger-0.0.2a6/src/gantry/models/components/evalstats.py
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-23 23:48:40.000000 gantry_logger-0.0.2a6/src/gantry/models/components/evaluationcriteriastatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-23 23:48:40.000000 gantry_logger-0.0.2a6/src/gantry/models/components/evaluationrecordstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3836 2024-04-23 23:48:40.000000 gantry_logger-0.0.2a6/src/gantry/models/components/evaluationrun.py
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-23 23:48:40.000000 gantry_logger-0.0.2a6/src/gantry/models/components/evaluationrunjobstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-04-23 23:48:40.000000 gantry_logger-0.0.2a6/src/gantry/models/components/evaluationrunpreupload.py
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-23 23:48:40.000000 gantry_logger-0.0.2a6/src/gantry/models/components/evaluationrunpreuploadresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-23 23:48:40.000000 gantry_logger-0.0.2a6/src/gantry/models/components/evaluationrunresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-04-23 23:48:40.000000 gantry_logger-0.0.2a6/src/gantry/models/components/functionstep.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-04-23 23:48:40.000000 gantry_logger-0.0.2a6/src/gantry/models/components/getlogssummaryrequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-04-23 23:48:40.000000 gantry_logger-0.0.2a6/src/gantry/models/components/getragevaluationresultsresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-04-23 23:48:40.000000 gantry_logger-0.0.2a6/src/gantry/models/components/getragevaluationresultsresponseresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-23 23:48:40.000000 gantry_logger-0.0.2a6/src/gantry/models/components/llmevaluationcriteriatype.py
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-23 23:48:40.000000 gantry_logger-0.0.2a6/src/gantry/models/components/llmevaluationerrortype.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-04-23 23:48:40.000000 gantry_logger-0.0.2a6/src/gantry/models/components/llmstep.py
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-04-23 23:48:40.000000 gantry_logger-0.0.2a6/src/gantry/models/components/logragrecordrequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-04-23 23:48:40.000000 gantry_logger-0.0.2a6/src/gantry/models/components/logragrecordresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-04-23 23:48:40.000000 gantry_logger-0.0.2a6/src/gantry/models/components/logragrecordresponseresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-04-23 23:48:40.000000 gantry_logger-0.0.2a6/src/gantry/models/components/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-23 23:48:40.000000 gantry_logger-0.0.2a6/src/gantry/models/components/organizationtier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-04-23 23:48:40.000000 gantry_logger-0.0.2a6/src/gantry/models/components/orguser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-23 23:48:40.000000 gantry_logger-0.0.2a6/src/gantry/models/components/passfailunsurerubricscalevalues.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3451 2024-04-23 23:48:40.000000 gantry_logger-0.0.2a6/src/gantry/models/components/ragcriteriaresult.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2080 2024-04-23 23:48:40.000000 gantry_logger-0.0.2a6/src/gantry/models/components/ragevaluationresult.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1871 2024-04-23 23:48:40.000000 gantry_logger-0.0.2a6/src/gantry/models/components/ragrecord.py
+-rw-r--r--   0 runner    (1001) docker     (127)      860 2024-04-23 23:48:40.000000 gantry_logger-0.0.2a6/src/gantry/models/components/recordstatuscount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-04-23 23:48:40.000000 gantry_logger-0.0.2a6/src/gantry/models/components/retrievalstep.py
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-23 23:48:40.000000 gantry_logger-0.0.2a6/src/gantry/models/components/security.py
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-23 23:48:40.000000 gantry_logger-0.0.2a6/src/gantry/models/components/stepformat.py
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-04-23 23:48:40.000000 gantry_logger-0.0.2a6/src/gantry/models/components/summarynotesresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-23 23:48:40.000000 gantry_logger-0.0.2a6/src/gantry/models/components/topicstats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:48:47.422418 gantry_logger-0.0.2a6/src/gantry/models/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-23 23:48:40.000000 gantry_logger-0.0.2a6/src/gantry/models/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-23 23:48:40.000000 gantry_logger-0.0.2a6/src/gantry/models/errors/sdkerror.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:48:47.426418 gantry_logger-0.0.2a6/src/gantry/models/operations/
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-23 23:48:40.000000 gantry_logger-0.0.2a6/src/gantry/models/operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      876 2024-04-23 23:48:40.000000 gantry_logger-0.0.2a6/src/gantry/models/operations/create_evaluation_run_pre_upload.py
+-rw-r--r--   0 runner    (1001) docker     (127)      823 2024-04-23 23:48:40.000000 gantry_logger-0.0.2a6/src/gantry/models/operations/create_rag_evaluation_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1979 2024-04-23 23:48:40.000000 gantry_logger-0.0.2a6/src/gantry/models/operations/get_rag_evaluation_results.py
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-04-23 23:48:40.000000 gantry_logger-0.0.2a6/src/gantry/models/operations/log_rag_records.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-04-23 23:48:40.000000 gantry_logger-0.0.2a6/src/gantry/sdk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-04-23 23:48:40.000000 gantry_logger-0.0.2a6/src/gantry/sdkconfiguration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:48:47.426418 gantry_logger-0.0.2a6/src/gantry/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-23 23:48:40.000000 gantry_logger-0.0.2a6/src/gantry/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3786 2024-04-23 23:48:40.000000 gantry_logger-0.0.2a6/src/gantry/utils/retries.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29680 2024-04-23 23:48:40.000000 gantry_logger-0.0.2a6/src/gantry/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:48:47.426418 gantry_logger-0.0.2a6/src/gantry_logger.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-04-23 23:48:47.000000 gantry_logger-0.0.2a6/src/gantry_logger.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3059 2024-04-23 23:48:47.000000 gantry_logger-0.0.2a6/src/gantry_logger.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 23:48:47.000000 gantry_logger-0.0.2a6/src/gantry_logger.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-23 23:48:47.000000 gantry_logger-0.0.2a6/src/gantry_logger.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-23 23:48:47.000000 gantry_logger-0.0.2a6/src/gantry_logger.egg-info/top_level.txt
```

### Comparing `gantry-logger-0.0.2a5/PKG-INFO` & `gantry_logger-0.0.2a6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gantry-logger
-Version: 0.0.2a5
+Version: 0.0.2a6
 Summary: Gantry Python Library
 Author: Gantry Systems, Inc.
 Author-email: oss@gantry.io
 License: Apache Software License v2
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `gantry-logger-0.0.2a5/setup.py` & `gantry_logger-0.0.2a6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import setuptools
 
-version = "0.0.2a5"
+version = "0.0.2a6"
 
 
 install_requires = [
     "pydantic",
     "certifi>=2023.7.22",
     "charset-normalizer>=3.2.0",
     "dataclasses-json>=0.6.1",
```

### Comparing `gantry-logger-0.0.2a5/src/gantry/evaluations.py` & `gantry_logger-0.0.2a6/src/gantry/evaluations.py`

 * *Files identical despite different names*

### Comparing `gantry-logger-0.0.2a5/src/gantry/logger/consumer.py` & `gantry_logger-0.0.2a6/src/gantry/logger/consumer.py`

 * *Files identical despite different names*

### Comparing `gantry-logger-0.0.2a5/src/gantry/logger/eval_logger.py` & `gantry_logger-0.0.2a6/src/gantry/logger/eval_logger.py`

 * *Files 9% similar despite different names*

```diff
@@ -38,22 +38,27 @@
                 "name": name,
                 "args": args,
                 "output": output,
             }
         )
 
     def add_llm_step(
-        self, messages: List[Dict], response: str, params: Optional[Dict] = None
+        self,
+        messages: List[Dict],
+        response: str,
+        params: Optional[Dict] = None,
+        usage: Optional[Dict] = None,
     ):
         self.steps.append(
             {
                 "type": "llm",
                 "messages": list(messages),  # make a copy
                 "response": response,
                 "params": params,
+                "usage": usage,
             }
         )
 
     def add_custom_step(self, data: Dict):
         self.steps.append(
             {
                 "type": "custom",
@@ -108,17 +113,21 @@
     def add_retrieval_step(self, query: str, documents: List[Dict]):
         self._record.add_retrieval_step(query, documents)
 
     def add_function_step(self, name: str, args: Dict, output: str):
         self._record.add_function_step(name, args, output)
 
     def add_llm_step(
-        self, messages: List[Dict], response: str, params: Optional[Dict] = None
+        self,
+        messages: List[Dict],
+        response: str,
+        params: Optional[Dict] = None,
+        usage: Optional[Dict] = None,
     ):
-        self._record.add_llm_step(messages, response, params)
+        self._record.add_llm_step(messages, response, params=params, usage=usage)
 
     def add_custom_step(self, data: Dict):
         self._record.add_custom_step(data)
 
     def end_record(self, response: str, **kwargs):
         if not isinstance(response, str):
             raise TypeError(f"response must be a string, not {type(response)}")
```

### Comparing `gantry-logger-0.0.2a5/src/gantry/logger/eval_reports.py` & `gantry_logger-0.0.2a6/src/gantry/logger/eval_reports.py`

 * *Files identical despite different names*

### Comparing `gantry-logger-0.0.2a5/src/gantry/logger/langchain_callback.py` & `gantry_logger-0.0.2a6/src/gantry/logger/langchain_callback.py`

 * *Files identical despite different names*

### Comparing `gantry-logger-0.0.2a5/src/gantry/logger/log_location.py` & `gantry_logger-0.0.2a6/src/gantry/logger/log_location.py`

 * *Files identical despite different names*

### Comparing `gantry-logger-0.0.2a5/src/gantry/logger/utils.py` & `gantry_logger-0.0.2a6/src/gantry/logger/utils.py`

 * *Files identical despite different names*

### Comparing `gantry-logger-0.0.2a5/src/gantry/logs.py` & `gantry_logger-0.0.2a6/src/gantry/logs.py`

 * *Files identical despite different names*

### Comparing `gantry-logger-0.0.2a5/src/gantry/models/components/__init__.py` & `gantry_logger-0.0.2a6/src/gantry/models/components/__init__.py`

 * *Files identical despite different names*

### Comparing `gantry-logger-0.0.2a5/src/gantry/models/components/createragevaluationrequest.py` & `gantry_logger-0.0.2a6/src/gantry/models/components/createragevaluationrequest.py`

 * *Files identical despite different names*

### Comparing `gantry-logger-0.0.2a5/src/gantry/models/components/criteriafeedback.py` & `gantry_logger-0.0.2a6/src/gantry/models/components/criteriafeedback.py`

 * *Files identical despite different names*

### Comparing `gantry-logger-0.0.2a5/src/gantry/models/components/criteriaresultcapture.py` & `gantry_logger-0.0.2a6/src/gantry/models/components/criteriaresultcapture.py`

 * *Files identical despite different names*

### Comparing `gantry-logger-0.0.2a5/src/gantry/models/components/criteriastats.py` & `gantry_logger-0.0.2a6/src/gantry/models/components/criteriastats.py`

 * *Files identical despite different names*

### Comparing `gantry-logger-0.0.2a5/src/gantry/models/components/criteriastatuscount.py` & `gantry_logger-0.0.2a6/src/gantry/models/components/criteriastatuscount.py`

 * *Files identical despite different names*

### Comparing `gantry-logger-0.0.2a5/src/gantry/models/components/customstep.py` & `gantry_logger-0.0.2a6/src/gantry/models/components/customstep.py`

 * *Files identical despite different names*

### Comparing `gantry-logger-0.0.2a5/src/gantry/models/components/document.py` & `gantry_logger-0.0.2a6/src/gantry/models/components/document.py`

 * *Files identical despite different names*

### Comparing `gantry-logger-0.0.2a5/src/gantry/models/components/evalcriteria.py` & `gantry_logger-0.0.2a6/src/gantry/models/components/evalcriteria.py`

 * *Files identical despite different names*

### Comparing `gantry-logger-0.0.2a5/src/gantry/models/components/evalstats.py` & `gantry_logger-0.0.2a6/src/gantry/models/components/evalstats.py`

 * *Files identical despite different names*

### Comparing `gantry-logger-0.0.2a5/src/gantry/models/components/evaluationrun.py` & `gantry_logger-0.0.2a6/src/gantry/models/components/evaluationrun.py`

 * *Files identical despite different names*

### Comparing `gantry-logger-0.0.2a5/src/gantry/models/components/evaluationrunpreupload.py` & `gantry_logger-0.0.2a6/src/gantry/models/components/evaluationrunpreupload.py`

 * *Files identical despite different names*

### Comparing `gantry-logger-0.0.2a5/src/gantry/models/components/evaluationrunpreuploadresponse.py` & `gantry_logger-0.0.2a6/src/gantry/models/components/evaluationrunpreuploadresponse.py`

 * *Files identical despite different names*

### Comparing `gantry-logger-0.0.2a5/src/gantry/models/components/evaluationrunresponse.py` & `gantry_logger-0.0.2a6/src/gantry/models/components/evaluationrunresponse.py`

 * *Files identical despite different names*

### Comparing `gantry-logger-0.0.2a5/src/gantry/models/components/functionstep.py` & `gantry_logger-0.0.2a6/src/gantry/models/components/functionstep.py`

 * *Files identical despite different names*

### Comparing `gantry-logger-0.0.2a5/src/gantry/models/components/getlogssummaryrequest.py` & `gantry_logger-0.0.2a6/src/gantry/models/components/getlogssummaryrequest.py`

 * *Files identical despite different names*

### Comparing `gantry-logger-0.0.2a5/src/gantry/models/components/getragevaluationresultsresponse.py` & `gantry_logger-0.0.2a6/src/gantry/models/components/getragevaluationresultsresponse.py`

 * *Files identical despite different names*

### Comparing `gantry-logger-0.0.2a5/src/gantry/models/components/getragevaluationresultsresponseresponse.py` & `gantry_logger-0.0.2a6/src/gantry/models/components/getragevaluationresultsresponseresponse.py`

 * *Files identical despite different names*

### Comparing `gantry-logger-0.0.2a5/src/gantry/models/components/llmstep.py` & `gantry_logger-0.0.2a6/src/gantry/models/components/llmstep.py`

 * *Files identical despite different names*

### Comparing `gantry-logger-0.0.2a5/src/gantry/models/components/logragrecordrequest.py` & `gantry_logger-0.0.2a6/src/gantry/models/components/logragrecordrequest.py`

 * *Files identical despite different names*

### Comparing `gantry-logger-0.0.2a5/src/gantry/models/components/logragrecordresponse.py` & `gantry_logger-0.0.2a6/src/gantry/models/components/logragrecordresponse.py`

 * *Files identical despite different names*

### Comparing `gantry-logger-0.0.2a5/src/gantry/models/components/logragrecordresponseresponse.py` & `gantry_logger-0.0.2a6/src/gantry/models/components/logragrecordresponseresponse.py`

 * *Files identical despite different names*

### Comparing `gantry-logger-0.0.2a5/src/gantry/models/components/message.py` & `gantry_logger-0.0.2a6/src/gantry/models/components/message.py`

 * *Files identical despite different names*

### Comparing `gantry-logger-0.0.2a5/src/gantry/models/components/orguser.py` & `gantry_logger-0.0.2a6/src/gantry/models/components/orguser.py`

 * *Files identical despite different names*

### Comparing `gantry-logger-0.0.2a5/src/gantry/models/components/ragcriteriaresult.py` & `gantry_logger-0.0.2a6/src/gantry/models/components/ragcriteriaresult.py`

 * *Files identical despite different names*

### Comparing `gantry-logger-0.0.2a5/src/gantry/models/components/ragevaluationresult.py` & `gantry_logger-0.0.2a6/src/gantry/models/components/ragevaluationresult.py`

 * *Files identical despite different names*

### Comparing `gantry-logger-0.0.2a5/src/gantry/models/components/ragrecord.py` & `gantry_logger-0.0.2a6/src/gantry/models/components/ragrecord.py`

 * *Files identical despite different names*

### Comparing `gantry-logger-0.0.2a5/src/gantry/models/components/recordstatuscount.py` & `gantry_logger-0.0.2a6/src/gantry/models/components/recordstatuscount.py`

 * *Files identical despite different names*

### Comparing `gantry-logger-0.0.2a5/src/gantry/models/components/retrievalstep.py` & `gantry_logger-0.0.2a6/src/gantry/models/components/retrievalstep.py`

 * *Files identical despite different names*

### Comparing `gantry-logger-0.0.2a5/src/gantry/models/components/summarynotesresponse.py` & `gantry_logger-0.0.2a6/src/gantry/models/components/summarynotesresponse.py`

 * *Files identical despite different names*

### Comparing `gantry-logger-0.0.2a5/src/gantry/models/components/topicstats.py` & `gantry_logger-0.0.2a6/src/gantry/models/components/topicstats.py`

 * *Files identical despite different names*

### Comparing `gantry-logger-0.0.2a5/src/gantry/models/errors/sdkerror.py` & `gantry_logger-0.0.2a6/src/gantry/models/errors/sdkerror.py`

 * *Files identical despite different names*

### Comparing `gantry-logger-0.0.2a5/src/gantry/models/operations/create_evaluation_run_pre_upload.py` & `gantry_logger-0.0.2a6/src/gantry/models/operations/create_evaluation_run_pre_upload.py`

 * *Files identical despite different names*

### Comparing `gantry-logger-0.0.2a5/src/gantry/models/operations/create_rag_evaluation_run.py` & `gantry_logger-0.0.2a6/src/gantry/models/operations/create_rag_evaluation_run.py`

 * *Files identical despite different names*

### Comparing `gantry-logger-0.0.2a5/src/gantry/models/operations/get_rag_evaluation_results.py` & `gantry_logger-0.0.2a6/src/gantry/models/operations/get_rag_evaluation_results.py`

 * *Files identical despite different names*

### Comparing `gantry-logger-0.0.2a5/src/gantry/models/operations/log_rag_records.py` & `gantry_logger-0.0.2a6/src/gantry/models/operations/log_rag_records.py`

 * *Files identical despite different names*

### Comparing `gantry-logger-0.0.2a5/src/gantry/sdk.py` & `gantry_logger-0.0.2a6/src/gantry/sdk.py`

 * *Files identical despite different names*

### Comparing `gantry-logger-0.0.2a5/src/gantry/sdkconfiguration.py` & `gantry_logger-0.0.2a6/src/gantry/sdkconfiguration.py`

 * *Files identical despite different names*

### Comparing `gantry-logger-0.0.2a5/src/gantry/utils/retries.py` & `gantry_logger-0.0.2a6/src/gantry/utils/retries.py`

 * *Files identical despite different names*

### Comparing `gantry-logger-0.0.2a5/src/gantry/utils/utils.py` & `gantry_logger-0.0.2a6/src/gantry/utils/utils.py`

 * *Files identical despite different names*

### Comparing `gantry-logger-0.0.2a5/src/gantry_logger.egg-info/PKG-INFO` & `gantry_logger-0.0.2a6/src/gantry_logger.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gantry-logger
-Version: 0.0.2a5
+Version: 0.0.2a6
 Summary: Gantry Python Library
 Author: Gantry Systems, Inc.
 Author-email: oss@gantry.io
 License: Apache Software License v2
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `gantry-logger-0.0.2a5/src/gantry_logger.egg-info/SOURCES.txt` & `gantry_logger-0.0.2a6/src/gantry_logger.egg-info/SOURCES.txt`

 * *Files identical despite different names*


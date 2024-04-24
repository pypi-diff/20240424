# Comparing `tmp/bullmq-2.7.2.tar.gz` & `tmp/bullmq-2.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bullmq-2.7.2.tar", last modified: Sat Apr 20 05:32:55 2024, max compression
+gzip compressed data, was "bullmq-2.7.3.tar", last modified: Wed Apr 24 04:34:30 2024, max compression
```

## Comparing `bullmq-2.7.2.tar` & `bullmq-2.7.3.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 05:32:55.263938 bullmq-2.7.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-04-20 05:32:55.263938 bullmq-2.7.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      999 2024-04-20 05:31:28.000000 bullmq-2.7.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 05:32:55.251938 bullmq-2.7.2/bullmq/
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-20 05:32:53.000000 bullmq-2.7.2/bullmq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-04-20 05:31:28.000000 bullmq-2.7.2/bullmq/backoffs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 05:32:55.259938 bullmq-2.7.2/bullmq/commands/
--rw-r--r--   0 runner    (1001) docker     (127)    10913 2024-04-20 05:32:27.000000 bullmq-2.7.2/bullmq/commands/addDelayedJob-6.lua
--rw-r--r--   0 runner    (1001) docker     (127)    10334 2024-04-20 05:32:27.000000 bullmq-2.7.2/bullmq/commands/addParentJob-4.lua
--rw-r--r--   0 runner    (1001) docker     (127)    10691 2024-04-20 05:32:27.000000 bullmq-2.7.2/bullmq/commands/addPrioritizedJob-7.lua
--rw-r--r--   0 runner    (1001) docker     (127)    10780 2024-04-20 05:32:27.000000 bullmq-2.7.2/bullmq/commands/addStandardJob-7.lua
--rw-r--r--   0 runner    (1001) docker     (127)     2400 2024-04-20 05:32:27.000000 bullmq-2.7.2/bullmq/commands/changeDelay-4.lua
--rw-r--r--   0 runner    (1001) docker     (127)     2242 2024-04-20 05:32:27.000000 bullmq-2.7.2/bullmq/commands/changePriority-6.lua
--rw-r--r--   0 runner    (1001) docker     (127)     9965 2024-04-20 05:32:27.000000 bullmq-2.7.2/bullmq/commands/cleanJobsInSet-2.lua
--rw-r--r--   0 runner    (1001) docker     (127)     6412 2024-04-20 05:32:27.000000 bullmq-2.7.2/bullmq/commands/drain-4.lua
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-04-20 05:32:27.000000 bullmq-2.7.2/bullmq/commands/extendLock-2.lua
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-20 05:32:27.000000 bullmq-2.7.2/bullmq/commands/getCounts-1.lua
--rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-04-20 05:32:27.000000 bullmq-2.7.2/bullmq/commands/getRanges-1.lua
--rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-04-20 05:32:27.000000 bullmq-2.7.2/bullmq/commands/getState-8.lua
--rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-04-20 05:32:27.000000 bullmq-2.7.2/bullmq/commands/getStateV2-8.lua
--rw-r--r--   0 runner    (1001) docker     (127)      897 2024-04-20 05:32:27.000000 bullmq-2.7.2/bullmq/commands/isFinished-3.lua
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-20 05:32:27.000000 bullmq-2.7.2/bullmq/commands/isJobInList-1.lua
--rw-r--r--   0 runner    (1001) docker     (127)     2706 2024-04-20 05:32:27.000000 bullmq-2.7.2/bullmq/commands/moveJobFromActiveToWait-10.lua
--rw-r--r--   0 runner    (1001) docker     (127)     2931 2024-04-20 05:32:27.000000 bullmq-2.7.2/bullmq/commands/moveJobsToWait-7.lua
--rw-r--r--   0 runner    (1001) docker     (127)    17377 2024-04-20 05:32:27.000000 bullmq-2.7.2/bullmq/commands/moveStalledJobsToWait-9.lua
--rw-r--r--   0 runner    (1001) docker     (127)     7295 2024-04-20 05:32:27.000000 bullmq-2.7.2/bullmq/commands/moveToActive-11.lua
--rw-r--r--   0 runner    (1001) docker     (127)     3439 2024-04-20 05:32:27.000000 bullmq-2.7.2/bullmq/commands/moveToDelayed-8.lua
--rw-r--r--   0 runner    (1001) docker     (127)    25897 2024-04-20 05:32:27.000000 bullmq-2.7.2/bullmq/commands/moveToFinished-14.lua
--rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-04-20 05:32:27.000000 bullmq-2.7.2/bullmq/commands/moveToWaitingChildren-5.lua
--rw-r--r--   0 runner    (1001) docker     (127)     8393 2024-04-20 05:32:27.000000 bullmq-2.7.2/bullmq/commands/obliterate-2.lua
--rw-r--r--   0 runner    (1001) docker     (127)     3742 2024-04-20 05:32:27.000000 bullmq-2.7.2/bullmq/commands/paginate-1.lua
--rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-04-20 05:32:27.000000 bullmq-2.7.2/bullmq/commands/pause-7.lua
--rw-r--r--   0 runner    (1001) docker     (127)     2673 2024-04-20 05:32:27.000000 bullmq-2.7.2/bullmq/commands/promote-8.lua
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-20 05:32:27.000000 bullmq-2.7.2/bullmq/commands/releaseLock-1.lua
--rw-r--r--   0 runner    (1001) docker     (127)     4903 2024-04-20 05:32:27.000000 bullmq-2.7.2/bullmq/commands/removeChildDependency-1.lua
--rw-r--r--   0 runner    (1001) docker     (127)     9216 2024-04-20 05:32:27.000000 bullmq-2.7.2/bullmq/commands/removeJob-1.lua
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-20 05:32:27.000000 bullmq-2.7.2/bullmq/commands/removeRepeatable-2.lua
--rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-04-20 05:32:27.000000 bullmq-2.7.2/bullmq/commands/reprocessJob-7.lua
--rw-r--r--   0 runner    (1001) docker     (127)     4917 2024-04-20 05:32:27.000000 bullmq-2.7.2/bullmq/commands/retryJob-11.lua
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-20 05:32:27.000000 bullmq-2.7.2/bullmq/commands/saveStacktrace-1.lua
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-20 05:32:27.000000 bullmq-2.7.2/bullmq/commands/updateData-1.lua
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-04-20 05:32:27.000000 bullmq-2.7.2/bullmq/commands/updateProgress-3.lua
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 05:32:55.259938 bullmq-2.7.2/bullmq/custom_errors/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-20 05:31:28.000000 bullmq-2.7.2/bullmq/custom_errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-20 05:31:28.000000 bullmq-2.7.2/bullmq/custom_errors/waiting_children_error.py
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-20 05:31:28.000000 bullmq-2.7.2/bullmq/error_code.py
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-20 05:31:28.000000 bullmq-2.7.2/bullmq/event_emitter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4621 2024-04-20 05:31:28.000000 bullmq-2.7.2/bullmq/flow_producer.py
--rw-r--r--   0 runner    (1001) docker     (127)    10416 2024-04-20 05:31:28.000000 bullmq-2.7.2/bullmq/job.py
--rw-r--r--   0 runner    (1001) docker     (127)    10683 2024-04-20 05:31:28.000000 bullmq-2.7.2/bullmq/queue.py
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-20 05:31:28.000000 bullmq-2.7.2/bullmq/queue_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-04-20 05:31:28.000000 bullmq-2.7.2/bullmq/redis_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)    24556 2024-04-20 05:31:28.000000 bullmq-2.7.2/bullmq/scripts.py
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-04-20 05:31:28.000000 bullmq-2.7.2/bullmq/timer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 05:32:55.263938 bullmq-2.7.2/bullmq/types/
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-20 05:31:28.000000 bullmq-2.7.2/bullmq/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-20 05:31:28.000000 bullmq-2.7.2/bullmq/types/backoff_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-04-20 05:31:28.000000 bullmq-2.7.2/bullmq/types/job_options.py
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-20 05:31:28.000000 bullmq-2.7.2/bullmq/types/keep_jobs.py
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-20 05:31:28.000000 bullmq-2.7.2/bullmq/types/promote_jobs_options.py
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-20 05:31:28.000000 bullmq-2.7.2/bullmq/types/queue_options.py
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-20 05:31:28.000000 bullmq-2.7.2/bullmq/types/retry_jobs_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-04-20 05:31:28.000000 bullmq-2.7.2/bullmq/types/worker_options.py
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-20 05:31:28.000000 bullmq-2.7.2/bullmq/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10296 2024-04-20 05:31:28.000000 bullmq-2.7.2/bullmq/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 05:32:55.263938 bullmq-2.7.2/bullmq.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-04-20 05:32:55.000000 bullmq-2.7.2/bullmq.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-04-20 05:32:55.000000 bullmq-2.7.2/bullmq.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 05:32:55.000000 bullmq-2.7.2/bullmq.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-20 05:32:55.000000 bullmq-2.7.2/bullmq.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-20 05:32:55.000000 bullmq-2.7.2/bullmq.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-04-20 05:32:53.000000 bullmq-2.7.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 05:32:55.263938 bullmq-2.7.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-20 05:31:28.000000 bullmq-2.7.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:34:30.614724 bullmq-2.7.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-04-24 04:34:30.614724 bullmq-2.7.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-04-24 04:32:50.000000 bullmq-2.7.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:34:30.606724 bullmq-2.7.3/bullmq/
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-24 04:34:28.000000 bullmq-2.7.3/bullmq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-04-24 04:32:50.000000 bullmq-2.7.3/bullmq/backoffs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:34:30.610724 bullmq-2.7.3/bullmq/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)    10913 2024-04-24 04:34:01.000000 bullmq-2.7.3/bullmq/commands/addDelayedJob-6.lua
+-rw-r--r--   0 runner    (1001) docker     (127)    10334 2024-04-24 04:34:01.000000 bullmq-2.7.3/bullmq/commands/addParentJob-4.lua
+-rw-r--r--   0 runner    (1001) docker     (127)    10691 2024-04-24 04:34:01.000000 bullmq-2.7.3/bullmq/commands/addPrioritizedJob-7.lua
+-rw-r--r--   0 runner    (1001) docker     (127)    10780 2024-04-24 04:34:01.000000 bullmq-2.7.3/bullmq/commands/addStandardJob-7.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     2400 2024-04-24 04:34:01.000000 bullmq-2.7.3/bullmq/commands/changeDelay-4.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     2242 2024-04-24 04:34:01.000000 bullmq-2.7.3/bullmq/commands/changePriority-6.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     9965 2024-04-24 04:34:01.000000 bullmq-2.7.3/bullmq/commands/cleanJobsInSet-2.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     6412 2024-04-24 04:34:01.000000 bullmq-2.7.3/bullmq/commands/drain-4.lua
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-04-24 04:34:01.000000 bullmq-2.7.3/bullmq/commands/extendLock-2.lua
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-24 04:34:01.000000 bullmq-2.7.3/bullmq/commands/getCounts-1.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-04-24 04:34:01.000000 bullmq-2.7.3/bullmq/commands/getRanges-1.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-04-24 04:34:01.000000 bullmq-2.7.3/bullmq/commands/getState-8.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-04-24 04:34:01.000000 bullmq-2.7.3/bullmq/commands/getStateV2-8.lua
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-04-24 04:34:01.000000 bullmq-2.7.3/bullmq/commands/isFinished-3.lua
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-24 04:34:01.000000 bullmq-2.7.3/bullmq/commands/isJobInList-1.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     2706 2024-04-24 04:34:01.000000 bullmq-2.7.3/bullmq/commands/moveJobFromActiveToWait-10.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     2931 2024-04-24 04:34:01.000000 bullmq-2.7.3/bullmq/commands/moveJobsToWait-7.lua
+-rw-r--r--   0 runner    (1001) docker     (127)    18137 2024-04-24 04:34:01.000000 bullmq-2.7.3/bullmq/commands/moveStalledJobsToWait-9.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     7295 2024-04-24 04:34:01.000000 bullmq-2.7.3/bullmq/commands/moveToActive-11.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     3439 2024-04-24 04:34:01.000000 bullmq-2.7.3/bullmq/commands/moveToDelayed-8.lua
+-rw-r--r--   0 runner    (1001) docker     (127)    26012 2024-04-24 04:34:01.000000 bullmq-2.7.3/bullmq/commands/moveToFinished-14.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-04-24 04:34:01.000000 bullmq-2.7.3/bullmq/commands/moveToWaitingChildren-5.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     8393 2024-04-24 04:34:01.000000 bullmq-2.7.3/bullmq/commands/obliterate-2.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     3742 2024-04-24 04:34:01.000000 bullmq-2.7.3/bullmq/commands/paginate-1.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-04-24 04:34:01.000000 bullmq-2.7.3/bullmq/commands/pause-7.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     2673 2024-04-24 04:34:01.000000 bullmq-2.7.3/bullmq/commands/promote-8.lua
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-24 04:34:01.000000 bullmq-2.7.3/bullmq/commands/releaseLock-1.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     4903 2024-04-24 04:34:01.000000 bullmq-2.7.3/bullmq/commands/removeChildDependency-1.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     9216 2024-04-24 04:34:01.000000 bullmq-2.7.3/bullmq/commands/removeJob-1.lua
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-24 04:34:01.000000 bullmq-2.7.3/bullmq/commands/removeRepeatable-2.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-04-24 04:34:01.000000 bullmq-2.7.3/bullmq/commands/reprocessJob-7.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     4917 2024-04-24 04:34:01.000000 bullmq-2.7.3/bullmq/commands/retryJob-11.lua
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-24 04:34:01.000000 bullmq-2.7.3/bullmq/commands/saveStacktrace-1.lua
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-24 04:34:01.000000 bullmq-2.7.3/bullmq/commands/updateData-1.lua
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-04-24 04:34:01.000000 bullmq-2.7.3/bullmq/commands/updateProgress-3.lua
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:34:30.614724 bullmq-2.7.3/bullmq/custom_errors/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-24 04:32:50.000000 bullmq-2.7.3/bullmq/custom_errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-24 04:32:50.000000 bullmq-2.7.3/bullmq/custom_errors/waiting_children_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-24 04:32:50.000000 bullmq-2.7.3/bullmq/error_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-24 04:32:50.000000 bullmq-2.7.3/bullmq/event_emitter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4621 2024-04-24 04:32:50.000000 bullmq-2.7.3/bullmq/flow_producer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10457 2024-04-24 04:32:50.000000 bullmq-2.7.3/bullmq/job.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10683 2024-04-24 04:32:50.000000 bullmq-2.7.3/bullmq/queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-24 04:32:50.000000 bullmq-2.7.3/bullmq/queue_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-04-24 04:32:50.000000 bullmq-2.7.3/bullmq/redis_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24462 2024-04-24 04:32:50.000000 bullmq-2.7.3/bullmq/scripts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-04-24 04:32:50.000000 bullmq-2.7.3/bullmq/timer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:34:30.614724 bullmq-2.7.3/bullmq/types/
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-24 04:32:50.000000 bullmq-2.7.3/bullmq/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-24 04:32:50.000000 bullmq-2.7.3/bullmq/types/backoff_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-04-24 04:32:50.000000 bullmq-2.7.3/bullmq/types/job_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-24 04:32:50.000000 bullmq-2.7.3/bullmq/types/keep_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-24 04:32:50.000000 bullmq-2.7.3/bullmq/types/promote_jobs_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-24 04:32:50.000000 bullmq-2.7.3/bullmq/types/queue_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-24 04:32:50.000000 bullmq-2.7.3/bullmq/types/retry_jobs_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-04-24 04:32:50.000000 bullmq-2.7.3/bullmq/types/worker_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-24 04:32:50.000000 bullmq-2.7.3/bullmq/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10296 2024-04-24 04:32:50.000000 bullmq-2.7.3/bullmq/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:34:30.614724 bullmq-2.7.3/bullmq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-04-24 04:34:30.000000 bullmq-2.7.3/bullmq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-04-24 04:34:30.000000 bullmq-2.7.3/bullmq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 04:34:30.000000 bullmq-2.7.3/bullmq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-24 04:34:30.000000 bullmq-2.7.3/bullmq.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-24 04:34:30.000000 bullmq-2.7.3/bullmq.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-04-24 04:34:28.000000 bullmq-2.7.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 04:34:30.614724 bullmq-2.7.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-24 04:32:50.000000 bullmq-2.7.3/setup.py
```

### Comparing `bullmq-2.7.2/PKG-INFO` & `bullmq-2.7.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bullmq
-Version: 2.7.2
+Version: 2.7.3
 Summary: BullMQ for Python
 Author-email: "Taskforce.sh Inc." <manast@taskforce.sh>
 Project-URL: Homepage, https://bullmq.io
 Project-URL: Bug Tracker, https://github.com/taskforcesh/bullmq/issues
 Keywords: python,bullmq,queues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `bullmq-2.7.2/README.md` & `bullmq-2.7.3/README.md`

 * *Files identical despite different names*

### Comparing `bullmq-2.7.2/bullmq/backoffs.py` & `bullmq-2.7.3/bullmq/backoffs.py`

 * *Files identical despite different names*

### Comparing `bullmq-2.7.2/bullmq/commands/addDelayedJob-6.lua` & `bullmq-2.7.3/bullmq/commands/addDelayedJob-6.lua`

 * *Files identical despite different names*

### Comparing `bullmq-2.7.2/bullmq/commands/addParentJob-4.lua` & `bullmq-2.7.3/bullmq/commands/addParentJob-4.lua`

 * *Files identical despite different names*

### Comparing `bullmq-2.7.2/bullmq/commands/addPrioritizedJob-7.lua` & `bullmq-2.7.3/bullmq/commands/addPrioritizedJob-7.lua`

 * *Files identical despite different names*

### Comparing `bullmq-2.7.2/bullmq/commands/addStandardJob-7.lua` & `bullmq-2.7.3/bullmq/commands/addStandardJob-7.lua`

 * *Files identical despite different names*

### Comparing `bullmq-2.7.2/bullmq/commands/changeDelay-4.lua` & `bullmq-2.7.3/bullmq/commands/changeDelay-4.lua`

 * *Files identical despite different names*

### Comparing `bullmq-2.7.2/bullmq/commands/changePriority-6.lua` & `bullmq-2.7.3/bullmq/commands/changePriority-6.lua`

 * *Files identical despite different names*

### Comparing `bullmq-2.7.2/bullmq/commands/cleanJobsInSet-2.lua` & `bullmq-2.7.3/bullmq/commands/cleanJobsInSet-2.lua`

 * *Files identical despite different names*

### Comparing `bullmq-2.7.2/bullmq/commands/drain-4.lua` & `bullmq-2.7.3/bullmq/commands/drain-4.lua`

 * *Files identical despite different names*

### Comparing `bullmq-2.7.2/bullmq/commands/getCounts-1.lua` & `bullmq-2.7.3/bullmq/commands/getCounts-1.lua`

 * *Files identical despite different names*

### Comparing `bullmq-2.7.2/bullmq/commands/getRanges-1.lua` & `bullmq-2.7.3/bullmq/commands/getRanges-1.lua`

 * *Files identical despite different names*

### Comparing `bullmq-2.7.2/bullmq/commands/getState-8.lua` & `bullmq-2.7.3/bullmq/commands/getState-8.lua`

 * *Files identical despite different names*

### Comparing `bullmq-2.7.2/bullmq/commands/getStateV2-8.lua` & `bullmq-2.7.3/bullmq/commands/getStateV2-8.lua`

 * *Files identical despite different names*

### Comparing `bullmq-2.7.2/bullmq/commands/isFinished-3.lua` & `bullmq-2.7.3/bullmq/commands/isFinished-3.lua`

 * *Files identical despite different names*

### Comparing `bullmq-2.7.2/bullmq/commands/moveJobFromActiveToWait-10.lua` & `bullmq-2.7.3/bullmq/commands/moveJobFromActiveToWait-10.lua`

 * *Files identical despite different names*

### Comparing `bullmq-2.7.2/bullmq/commands/moveJobsToWait-7.lua` & `bullmq-2.7.3/bullmq/commands/moveJobsToWait-7.lua`

 * *Files identical despite different names*

### Comparing `bullmq-2.7.2/bullmq/commands/moveStalledJobsToWait-9.lua` & `bullmq-2.7.3/bullmq/commands/moveStalledJobsToWait-9.lua`

 * *Files 3% similar despite different names*

```diff
@@ -382,14 +382,24 @@
                             moveParentFromWaitingChildrenToFailed(
                                 parentData['queueKey'],
                                 parentData['queueKey'] .. ':' .. parentData['id'],
                                 parentData['id'],
                                 jobKey,
                                 timestamp
                             )
+                        elseif opts['idof'] then
+                            local parentData = cjson.decode(rawParentData)
+                            local parentKey = parentData['queueKey'] .. ':' .. parentData['id']
+                            local dependenciesSet = parentKey .. ":dependencies"
+                            if rcall("SREM", dependenciesSet, jobKey) == 1 then
+                                moveParentToWaitIfNeeded(parentData['queueKey'], dependenciesSet,
+                                                         parentKey, parentData['id'], timestamp)
+                                local failedSet = parentKey .. ":failed"
+                                rcall("HSET", failedSet, jobKey, failedReason)
+                            end
                         end
                         if removeOnFailType == "number" then
                             removeJobsByMaxCount(opts["removeOnFail"],
                                                   failedKey, queueKeyPrefix)
                         elseif removeOnFailType == "boolean" then
                             if opts["removeOnFail"] then
                                 removeJob(jobId, false, queueKeyPrefix)
```

### Comparing `bullmq-2.7.2/bullmq/commands/moveToActive-11.lua` & `bullmq-2.7.3/bullmq/commands/moveToActive-11.lua`

 * *Files identical despite different names*

### Comparing `bullmq-2.7.2/bullmq/commands/moveToDelayed-8.lua` & `bullmq-2.7.3/bullmq/commands/moveToDelayed-8.lua`

 * *Files identical despite different names*

### Comparing `bullmq-2.7.2/bullmq/commands/moveToFinished-14.lua` & `bullmq-2.7.3/bullmq/commands/moveToFinished-14.lua`

 * *Files 1% similar despite different names*

```diff
@@ -453,14 +453,33 @@
   local start = maxCount
   local jobIds = rcall("ZREVRANGE", targetSet, start, -1)
   for i, jobId in ipairs(jobIds) do
     removeJob(jobId, false, prefix)
   end
   rcall("ZREMRANGEBYRANK", targetSet, 0, -(maxCount + 1))
 end
+local function removeLock(jobKey, stalledKey, token, jobId)
+  if token ~= "0" then
+    local lockKey = jobKey .. ':lock'
+    local lockToken = rcall("GET", lockKey)
+    if lockToken == token then
+      rcall("DEL", lockKey)
+      rcall("SREM", stalledKey, jobId)
+    else
+      if lockToken then
+        -- Lock exists but token does not match
+        return -6
+      else
+        -- Lock is missing completely
+        return -2
+      end
+    end
+  end
+  return 0
+end
 --[[
   Function to trim events, default 10000.
 ]]
 -- Includes
 --[[
   Function to get max events value or set by default 10000.
 ]]
@@ -490,34 +509,22 @@
   rcall("HSET", processedSet, jobIdKey, returnvalue)
   moveParentToWaitIfNeeded(parentQueueKey, parentDependenciesKey, parentKey, parentId, timestamp)
 end
 local jobIdKey = KEYS[12]
 if rcall("EXISTS", jobIdKey) == 1 then -- // Make sure job exists
     local opts = cmsgpack.unpack(ARGV[8])
     local token = opts['token']
+    local errorCode = removeLock(jobIdKey, KEYS[5], token, ARGV[1])
+    if errorCode < 0 then
+        return errorCode
+    end
     local attempts = opts['attempts']
     local maxMetricsSize = opts['maxMetricsSize']
     local maxCount = opts['keepJobs']['count']
     local maxAge = opts['keepJobs']['age']
-    if token ~= "0" then
-        local lockKey = jobIdKey .. ':lock'
-        local lockToken = rcall("GET", lockKey)
-        if lockToken == token then
-            rcall("DEL", lockKey)
-            rcall("SREM", KEYS[5], ARGV[1])
-        else
-            if lockToken then
-                -- Lock exists but token does not match
-                return -6
-            else
-                -- Lock is missing completely
-                return -2
-            end
-        end
-    end
     if rcall("SCARD", jobIdKey .. ":dependencies") ~= 0 then -- // Make sure it does not have pending dependencies
         return -4
     end
     local parentReferences = rcall("HMGET", jobIdKey, "parentKey", "parent")
     local parentKey = parentReferences[1] or ""
     local parentId = ""
     local parentQueueKey = ""
```

### Comparing `bullmq-2.7.2/bullmq/commands/moveToWaitingChildren-5.lua` & `bullmq-2.7.3/bullmq/commands/moveToWaitingChildren-5.lua`

 * *Files identical despite different names*

### Comparing `bullmq-2.7.2/bullmq/commands/obliterate-2.lua` & `bullmq-2.7.3/bullmq/commands/obliterate-2.lua`

 * *Files identical despite different names*

### Comparing `bullmq-2.7.2/bullmq/commands/paginate-1.lua` & `bullmq-2.7.3/bullmq/commands/paginate-1.lua`

 * *Files identical despite different names*

### Comparing `bullmq-2.7.2/bullmq/commands/pause-7.lua` & `bullmq-2.7.3/bullmq/commands/pause-7.lua`

 * *Files identical despite different names*

### Comparing `bullmq-2.7.2/bullmq/commands/promote-8.lua` & `bullmq-2.7.3/bullmq/commands/promote-8.lua`

 * *Files identical despite different names*

### Comparing `bullmq-2.7.2/bullmq/commands/removeChildDependency-1.lua` & `bullmq-2.7.3/bullmq/commands/removeChildDependency-1.lua`

 * *Files identical despite different names*

### Comparing `bullmq-2.7.2/bullmq/commands/removeJob-1.lua` & `bullmq-2.7.3/bullmq/commands/removeJob-1.lua`

 * *Files identical despite different names*

### Comparing `bullmq-2.7.2/bullmq/commands/removeRepeatable-2.lua` & `bullmq-2.7.3/bullmq/commands/removeRepeatable-2.lua`

 * *Files identical despite different names*

### Comparing `bullmq-2.7.2/bullmq/commands/reprocessJob-7.lua` & `bullmq-2.7.3/bullmq/commands/reprocessJob-7.lua`

 * *Files identical despite different names*

### Comparing `bullmq-2.7.2/bullmq/commands/retryJob-11.lua` & `bullmq-2.7.3/bullmq/commands/retryJob-11.lua`

 * *Files identical despite different names*

### Comparing `bullmq-2.7.2/bullmq/commands/updateProgress-3.lua` & `bullmq-2.7.3/bullmq/commands/updateProgress-3.lua`

 * *Files identical despite different names*

### Comparing `bullmq-2.7.2/bullmq/event_emitter.py` & `bullmq-2.7.3/bullmq/event_emitter.py`

 * *Files identical despite different names*

### Comparing `bullmq-2.7.2/bullmq/flow_producer.py` & `bullmq-2.7.3/bullmq/flow_producer.py`

 * *Files identical despite different names*

### Comparing `bullmq-2.7.2/bullmq/job.py` & `bullmq-2.7.3/bullmq/job.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 import json
 import time
 import traceback
 
 
 optsDecodeMap = {
     'fpof': 'failParentOnFailure',
+    'idof': 'ignoreDependencyOnFailure',
     'kl': 'keepLogs',
 }
 
 optsEncodeMap = {v: k for k, v in optsDecodeMap.items()}
 
 
 class Job:
```

### Comparing `bullmq-2.7.2/bullmq/queue.py` & `bullmq-2.7.3/bullmq/queue.py`

 * *Files identical despite different names*

### Comparing `bullmq-2.7.2/bullmq/queue_keys.py` & `bullmq-2.7.3/bullmq/queue_keys.py`

 * *Files identical despite different names*

### Comparing `bullmq-2.7.2/bullmq/redis_connection.py` & `bullmq-2.7.3/bullmq/redis_connection.py`

 * *Files identical despite different names*

### Comparing `bullmq-2.7.2/bullmq/scripts.py` & `bullmq-2.7.3/bullmq/scripts.py`

 * *Files 1% similar despite different names*

```diff
@@ -508,30 +508,26 @@
 
         def getMetricsSize(opts: dict):
             metrics = opts.get("metrics")
             if metrics is not None:
                 return metrics.get("maxDataPoints", "")
             return ""
 
-        def getFailParentOnFailure(job: Job):
-            opts = job.opts
-            if opts is not None:
-                return opts.get("failParentOnFailure", False)
-
         keepJobs = getKeepJobs(shouldRemove)
 
         packedOpts = msgpack.packb({
             "token": token,
             "keepJobs": keepJobs,
             "limiter": opts.get("limiter"),
             "lockDuration": opts.get("lockDuration"),
             "attempts": job.attempts,
             "attemptsMade": job.attemptsMade,
             "maxMetricsSize": getMetricsSize(opts),
-            "fpof": getFailParentOnFailure(job),
+            "fpof": opts.get("failParentOnFailure", False),
+            "idof": opts.get("ignoreDependencyOnFailure", False)
         }, use_bin_type=True)
 
         args = [job.id, timestamp, propVal, transformed_value or "", target,
                 fetchNext and "1" or "", self.keys[''], packedOpts]
         return (keys, args)
 
     def moveToFailedArgs(self, job: Job, failed_reason: str, shouldRemove, token: str, opts: dict, fetchNext=True):
```

### Comparing `bullmq-2.7.2/bullmq/timer.py` & `bullmq-2.7.3/bullmq/timer.py`

 * *Files identical despite different names*

### Comparing `bullmq-2.7.2/bullmq/types/job_options.py` & `bullmq-2.7.3/bullmq/types/job_options.py`

 * *Files identical despite different names*

### Comparing `bullmq-2.7.2/bullmq/types/worker_options.py` & `bullmq-2.7.3/bullmq/types/worker_options.py`

 * *Files identical despite different names*

### Comparing `bullmq-2.7.2/bullmq/utils.py` & `bullmq-2.7.3/bullmq/utils.py`

 * *Files identical despite different names*

### Comparing `bullmq-2.7.2/bullmq/worker.py` & `bullmq-2.7.3/bullmq/worker.py`

 * *Files identical despite different names*

### Comparing `bullmq-2.7.2/bullmq.egg-info/PKG-INFO` & `bullmq-2.7.3/bullmq.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bullmq
-Version: 2.7.2
+Version: 2.7.3
 Summary: BullMQ for Python
 Author-email: "Taskforce.sh Inc." <manast@taskforce.sh>
 Project-URL: Homepage, https://bullmq.io
 Project-URL: Bug Tracker, https://github.com/taskforcesh/bullmq/issues
 Keywords: python,bullmq,queues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `bullmq-2.7.2/bullmq.egg-info/SOURCES.txt` & `bullmq-2.7.3/bullmq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bullmq-2.7.2/pyproject.toml` & `bullmq-2.7.3/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "bullmq"
-version = "2.7.2"
+version = "2.7.3"
 description='BullMQ for Python'
 readme="README.md"
 authors = [
     {name = "Taskforce.sh Inc.", email = "manast@taskforce.sh"},
 ]
 requires-python = ">=3.10.0"
 classifiers=[
```


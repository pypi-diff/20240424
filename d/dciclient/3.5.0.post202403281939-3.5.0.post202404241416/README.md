# Comparing `tmp/dciclient-3.5.0.post202403281939.tar.gz` & `tmp/dciclient-3.5.0.post202404241416.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dciclient-3.5.0.post202403281939.tar", last modified: Tue Apr  9 09:54:46 2024, max compression
+gzip compressed data, was "dciclient-3.5.0.post202404241416.tar", last modified: Wed Apr 24 15:27:05 2024, max compression
```

## Comparing `dciclient-3.5.0.post202403281939.tar` & `dciclient-3.5.0.post202404241416.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 09:54:46.882608 dciclient-3.5.0.post202403281939/
--rw-r--r--   0 root         (0) root         (0)    10142 2024-04-09 09:53:47.000000 dciclient-3.5.0.post202403281939/LICENSE
--rw-r--r--   0 root         (0) root         (0)       79 2024-04-09 09:53:47.000000 dciclient-3.5.0.post202403281939/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    10749 2024-04-09 09:54:46.882608 dciclient-3.5.0.post202403281939/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    10025 2024-04-09 09:53:47.000000 dciclient-3.5.0.post202403281939/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 09:54:46.877608 dciclient-3.5.0.post202403281939/dciclient/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-09 09:53:47.000000 dciclient-3.5.0.post202403281939/dciclient/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4876 2024-04-09 09:53:47.000000 dciclient-3.5.0.post202403281939/dciclient/create_component.py
--rw-r--r--   0 root         (0) root         (0)     6198 2024-04-09 09:53:47.000000 dciclient-3.5.0.post202403281939/dciclient/create_job.py
--rw-r--r--   0 root         (0) root         (0)     5376 2024-04-09 09:53:47.000000 dciclient-3.5.0.post202403281939/dciclient/diff_jobs.py
--rw-r--r--   0 root         (0) root         (0)     5317 2024-04-09 09:53:47.000000 dciclient-3.5.0.post202403281939/dciclient/find_latest_component.py
--rw-r--r--   0 root         (0) root         (0)     4068 2024-04-09 09:53:47.000000 dciclient-3.5.0.post202403281939/dciclient/printer.py
--rw-r--r--   0 root         (0) root         (0)     4128 2024-04-09 09:53:47.000000 dciclient-3.5.0.post202403281939/dciclient/rhel_kernel.py
--rwxr-xr-x   0 root         (0) root         (0)     1236 2024-04-09 09:53:47.000000 dciclient-3.5.0.post202403281939/dciclient/shell.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 09:54:46.878608 dciclient-3.5.0.post202403281939/dciclient/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-09 09:53:47.000000 dciclient-3.5.0.post202403281939/dciclient/v1/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 09:54:46.880608 dciclient-3.5.0.post202403281939/dciclient/v1/api/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-09 09:53:47.000000 dciclient-3.5.0.post202403281939/dciclient/v1/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5338 2024-04-09 09:53:47.000000 dciclient-3.5.0.post202403281939/dciclient/v1/api/base.py
--rw-r--r--   0 root         (0) root         (0)     2841 2024-04-09 09:53:47.000000 dciclient-3.5.0.post202403281939/dciclient/v1/api/component.py
--rw-r--r--   0 root         (0) root         (0)     7447 2024-04-09 09:53:47.000000 dciclient-3.5.0.post202403281939/dciclient/v1/api/context.py
--rw-r--r--   0 root         (0) root         (0)     1314 2024-04-09 09:53:47.000000 dciclient-3.5.0.post202403281939/dciclient/v1/api/feeder.py
--rw-r--r--   0 root         (0) root         (0)     3473 2024-04-09 09:53:47.000000 dciclient-3.5.0.post202403281939/dciclient/v1/api/file.py
--rw-r--r--   0 root         (0) root         (0)     1109 2024-04-09 09:53:47.000000 dciclient-3.5.0.post202403281939/dciclient/v1/api/identity.py
--rw-r--r--   0 root         (0) root         (0)     4333 2024-04-09 09:53:47.000000 dciclient-3.5.0.post202403281939/dciclient/v1/api/job.py
--rw-r--r--   0 root         (0) root         (0)     1896 2024-04-09 09:53:47.000000 dciclient-3.5.0.post202403281939/dciclient/v1/api/jobs_events.py
--rw-r--r--   0 root         (0) root         (0)      973 2024-04-09 09:53:47.000000 dciclient-3.5.0.post202403281939/dciclient/v1/api/jobstate.py
--rw-r--r--   0 root         (0) root         (0)     1362 2024-04-09 09:53:47.000000 dciclient-3.5.0.post202403281939/dciclient/v1/api/pipeline.py
--rw-r--r--   0 root         (0) root         (0)     1800 2024-04-09 09:53:47.000000 dciclient-3.5.0.post202403281939/dciclient/v1/api/product.py
--rw-r--r--   0 root         (0) root         (0)     2030 2024-04-09 09:53:47.000000 dciclient-3.5.0.post202403281939/dciclient/v1/api/remoteci.py
--rw-r--r--   0 root         (0) root         (0)     1403 2024-04-09 09:53:47.000000 dciclient-3.5.0.post202403281939/dciclient/v1/api/tag.py
--rw-r--r--   0 root         (0) root         (0)     1205 2024-04-09 09:53:47.000000 dciclient-3.5.0.post202403281939/dciclient/v1/api/team.py
--rw-r--r--   0 root         (0) root         (0)     2438 2024-04-09 09:53:47.000000 dciclient-3.5.0.post202403281939/dciclient/v1/api/topic.py
--rw-r--r--   0 root         (0) root         (0)     1670 2024-04-09 09:53:47.000000 dciclient-3.5.0.post202403281939/dciclient/v1/api/user.py
--rw-r--r--   0 root         (0) root         (0)      862 2024-04-09 09:53:47.000000 dciclient-3.5.0.post202403281939/dciclient/v1/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 09:54:46.881608 dciclient-3.5.0.post202403281939/dciclient/v1/shell_commands/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-09 09:53:47.000000 dciclient-3.5.0.post202403281939/dciclient/v1/shell_commands/__init__.py
--rw-r--r--   0 root         (0) root         (0)    28064 2024-04-09 09:53:47.000000 dciclient-3.5.0.post202403281939/dciclient/v1/shell_commands/cli.py
--rw-r--r--   0 root         (0) root         (0)     1412 2024-04-09 09:53:47.000000 dciclient-3.5.0.post202403281939/dciclient/v1/shell_commands/columns.py
--rw-r--r--   0 root         (0) root         (0)     2785 2024-04-09 09:53:47.000000 dciclient-3.5.0.post202403281939/dciclient/v1/shell_commands/component.py
--rw-r--r--   0 root         (0) root         (0)     3905 2024-04-09 09:53:47.000000 dciclient-3.5.0.post202403281939/dciclient/v1/shell_commands/context.py
--rw-r--r--   0 root         (0) root         (0)     1506 2024-04-09 09:53:47.000000 dciclient-3.5.0.post202403281939/dciclient/v1/shell_commands/feeder.py
--rw-r--r--   0 root         (0) root         (0)      996 2024-04-09 09:53:47.000000 dciclient-3.5.0.post202403281939/dciclient/v1/shell_commands/file.py
--rw-r--r--   0 root         (0) root         (0)     3168 2024-04-09 09:53:47.000000 dciclient-3.5.0.post202403281939/dciclient/v1/shell_commands/job.py
--rw-r--r--   0 root         (0) root         (0)      822 2024-04-09 09:53:47.000000 dciclient-3.5.0.post202403281939/dciclient/v1/shell_commands/jobstate.py
--rw-r--r--   0 root         (0) root         (0)     1558 2024-04-09 09:53:47.000000 dciclient-3.5.0.post202403281939/dciclient/v1/shell_commands/pipeline.py
--rw-r--r--   0 root         (0) root         (0)     1942 2024-04-09 09:53:47.000000 dciclient-3.5.0.post202403281939/dciclient/v1/shell_commands/product.py
--rw-r--r--   0 root         (0) root         (0)     2426 2024-04-09 09:53:47.000000 dciclient-3.5.0.post202403281939/dciclient/v1/shell_commands/purge.py
--rw-r--r--   0 root         (0) root         (0)     2316 2024-04-09 09:53:47.000000 dciclient-3.5.0.post202403281939/dciclient/v1/shell_commands/remoteci.py
--rw-r--r--   0 root         (0) root         (0)     4084 2024-04-09 09:53:47.000000 dciclient-3.5.0.post202403281939/dciclient/v1/shell_commands/runner.py
--rw-r--r--   0 root         (0) root         (0)     1574 2024-04-09 09:53:47.000000 dciclient-3.5.0.post202403281939/dciclient/v1/shell_commands/team.py
--rw-r--r--   0 root         (0) root         (0)     2037 2024-04-09 09:53:47.000000 dciclient-3.5.0.post202403281939/dciclient/v1/shell_commands/topic.py
--rw-r--r--   0 root         (0) root         (0)     1827 2024-04-09 09:53:47.000000 dciclient-3.5.0.post202403281939/dciclient/v1/shell_commands/user.py
--rw-r--r--   0 root         (0) root         (0)     1868 2024-04-09 09:53:47.000000 dciclient-3.5.0.post202403281939/dciclient/v1/utils.py
--rw-r--r--   0 root         (0) root         (0)     1544 2024-04-09 09:53:47.000000 dciclient-3.5.0.post202403281939/dciclient/vault.py
--rw-r--r--   0 root         (0) root         (0)     1838 2024-04-09 09:53:47.000000 dciclient-3.5.0.post202403281939/dciclient/vault_client.py
--rw-r--r--   0 root         (0) root         (0)       51 2024-04-09 09:54:46.000000 dciclient-3.5.0.post202403281939/dciclient/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 09:54:46.877608 dciclient-3.5.0.post202403281939/dciclient.egg-info/
--rw-r--r--   0 root         (0) root         (0)    10749 2024-04-09 09:54:46.000000 dciclient-3.5.0.post202403281939/dciclient.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1716 2024-04-09 09:54:46.000000 dciclient-3.5.0.post202403281939/dciclient.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-09 09:54:46.000000 dciclient-3.5.0.post202403281939/dciclient.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      392 2024-04-09 09:54:46.000000 dciclient-3.5.0.post202403281939/dciclient.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       60 2024-04-09 09:54:46.000000 dciclient-3.5.0.post202403281939/dciclient.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2024-04-09 09:54:46.000000 dciclient-3.5.0.post202403281939/dciclient.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       63 2024-04-09 09:53:47.000000 dciclient-3.5.0.post202403281939/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-09 09:54:46.882608 dciclient-3.5.0.post202403281939/setup.cfg
--rwxr-xr-x   0 root         (0) root         (0)     3218 2024-04-09 09:53:47.000000 dciclient-3.5.0.post202403281939/setup.py
--rwxr-xr-x   0 root         (0) root         (0)     1222 2024-04-09 09:53:47.000000 dciclient-3.5.0.post202403281939/start_db.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:27:05.035430 dciclient-3.5.0.post202404241416/
+-rw-r--r--   0 root         (0) root         (0)    10142 2024-04-24 15:26:04.000000 dciclient-3.5.0.post202404241416/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       79 2024-04-24 15:26:04.000000 dciclient-3.5.0.post202404241416/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    10749 2024-04-24 15:27:05.034430 dciclient-3.5.0.post202404241416/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    10025 2024-04-24 15:26:04.000000 dciclient-3.5.0.post202404241416/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:27:05.029430 dciclient-3.5.0.post202404241416/dciclient/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-24 15:26:04.000000 dciclient-3.5.0.post202404241416/dciclient/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4876 2024-04-24 15:26:04.000000 dciclient-3.5.0.post202404241416/dciclient/create_component.py
+-rw-r--r--   0 root         (0) root         (0)     6198 2024-04-24 15:26:04.000000 dciclient-3.5.0.post202404241416/dciclient/create_job.py
+-rw-r--r--   0 root         (0) root         (0)     5376 2024-04-24 15:26:04.000000 dciclient-3.5.0.post202404241416/dciclient/diff_jobs.py
+-rw-r--r--   0 root         (0) root         (0)     5317 2024-04-24 15:26:04.000000 dciclient-3.5.0.post202404241416/dciclient/find_latest_component.py
+-rw-r--r--   0 root         (0) root         (0)     4068 2024-04-24 15:26:04.000000 dciclient-3.5.0.post202404241416/dciclient/printer.py
+-rw-r--r--   0 root         (0) root         (0)     4128 2024-04-24 15:26:04.000000 dciclient-3.5.0.post202404241416/dciclient/rhel_kernel.py
+-rwxr-xr-x   0 root         (0) root         (0)     1236 2024-04-24 15:26:04.000000 dciclient-3.5.0.post202404241416/dciclient/shell.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:27:05.030430 dciclient-3.5.0.post202404241416/dciclient/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-24 15:26:04.000000 dciclient-3.5.0.post202404241416/dciclient/v1/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:27:05.032430 dciclient-3.5.0.post202404241416/dciclient/v1/api/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-24 15:26:04.000000 dciclient-3.5.0.post202404241416/dciclient/v1/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5338 2024-04-24 15:26:04.000000 dciclient-3.5.0.post202404241416/dciclient/v1/api/base.py
+-rw-r--r--   0 root         (0) root         (0)     2841 2024-04-24 15:26:04.000000 dciclient-3.5.0.post202404241416/dciclient/v1/api/component.py
+-rw-r--r--   0 root         (0) root         (0)     7447 2024-04-24 15:26:04.000000 dciclient-3.5.0.post202404241416/dciclient/v1/api/context.py
+-rw-r--r--   0 root         (0) root         (0)     1314 2024-04-24 15:26:04.000000 dciclient-3.5.0.post202404241416/dciclient/v1/api/feeder.py
+-rw-r--r--   0 root         (0) root         (0)     3473 2024-04-24 15:26:04.000000 dciclient-3.5.0.post202404241416/dciclient/v1/api/file.py
+-rw-r--r--   0 root         (0) root         (0)     1109 2024-04-24 15:26:04.000000 dciclient-3.5.0.post202404241416/dciclient/v1/api/identity.py
+-rw-r--r--   0 root         (0) root         (0)     4333 2024-04-24 15:26:04.000000 dciclient-3.5.0.post202404241416/dciclient/v1/api/job.py
+-rw-r--r--   0 root         (0) root         (0)     1896 2024-04-24 15:26:04.000000 dciclient-3.5.0.post202404241416/dciclient/v1/api/jobs_events.py
+-rw-r--r--   0 root         (0) root         (0)      973 2024-04-24 15:26:04.000000 dciclient-3.5.0.post202404241416/dciclient/v1/api/jobstate.py
+-rw-r--r--   0 root         (0) root         (0)     1362 2024-04-24 15:26:04.000000 dciclient-3.5.0.post202404241416/dciclient/v1/api/pipeline.py
+-rw-r--r--   0 root         (0) root         (0)     1800 2024-04-24 15:26:04.000000 dciclient-3.5.0.post202404241416/dciclient/v1/api/product.py
+-rw-r--r--   0 root         (0) root         (0)     2030 2024-04-24 15:26:04.000000 dciclient-3.5.0.post202404241416/dciclient/v1/api/remoteci.py
+-rw-r--r--   0 root         (0) root         (0)     1403 2024-04-24 15:26:04.000000 dciclient-3.5.0.post202404241416/dciclient/v1/api/tag.py
+-rw-r--r--   0 root         (0) root         (0)     1205 2024-04-24 15:26:04.000000 dciclient-3.5.0.post202404241416/dciclient/v1/api/team.py
+-rw-r--r--   0 root         (0) root         (0)     2438 2024-04-24 15:26:04.000000 dciclient-3.5.0.post202404241416/dciclient/v1/api/topic.py
+-rw-r--r--   0 root         (0) root         (0)     1670 2024-04-24 15:26:04.000000 dciclient-3.5.0.post202404241416/dciclient/v1/api/user.py
+-rw-r--r--   0 root         (0) root         (0)      862 2024-04-24 15:26:04.000000 dciclient-3.5.0.post202404241416/dciclient/v1/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:27:05.034430 dciclient-3.5.0.post202404241416/dciclient/v1/shell_commands/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-24 15:26:04.000000 dciclient-3.5.0.post202404241416/dciclient/v1/shell_commands/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    28064 2024-04-24 15:26:04.000000 dciclient-3.5.0.post202404241416/dciclient/v1/shell_commands/cli.py
+-rw-r--r--   0 root         (0) root         (0)     1412 2024-04-24 15:26:04.000000 dciclient-3.5.0.post202404241416/dciclient/v1/shell_commands/columns.py
+-rw-r--r--   0 root         (0) root         (0)     2785 2024-04-24 15:26:04.000000 dciclient-3.5.0.post202404241416/dciclient/v1/shell_commands/component.py
+-rw-r--r--   0 root         (0) root         (0)     3905 2024-04-24 15:26:04.000000 dciclient-3.5.0.post202404241416/dciclient/v1/shell_commands/context.py
+-rw-r--r--   0 root         (0) root         (0)     1506 2024-04-24 15:26:04.000000 dciclient-3.5.0.post202404241416/dciclient/v1/shell_commands/feeder.py
+-rw-r--r--   0 root         (0) root         (0)      996 2024-04-24 15:26:04.000000 dciclient-3.5.0.post202404241416/dciclient/v1/shell_commands/file.py
+-rw-r--r--   0 root         (0) root         (0)     3168 2024-04-24 15:26:04.000000 dciclient-3.5.0.post202404241416/dciclient/v1/shell_commands/job.py
+-rw-r--r--   0 root         (0) root         (0)      822 2024-04-24 15:26:04.000000 dciclient-3.5.0.post202404241416/dciclient/v1/shell_commands/jobstate.py
+-rw-r--r--   0 root         (0) root         (0)     1558 2024-04-24 15:26:04.000000 dciclient-3.5.0.post202404241416/dciclient/v1/shell_commands/pipeline.py
+-rw-r--r--   0 root         (0) root         (0)     1942 2024-04-24 15:26:04.000000 dciclient-3.5.0.post202404241416/dciclient/v1/shell_commands/product.py
+-rw-r--r--   0 root         (0) root         (0)     2426 2024-04-24 15:26:04.000000 dciclient-3.5.0.post202404241416/dciclient/v1/shell_commands/purge.py
+-rw-r--r--   0 root         (0) root         (0)     2316 2024-04-24 15:26:04.000000 dciclient-3.5.0.post202404241416/dciclient/v1/shell_commands/remoteci.py
+-rw-r--r--   0 root         (0) root         (0)     4084 2024-04-24 15:26:04.000000 dciclient-3.5.0.post202404241416/dciclient/v1/shell_commands/runner.py
+-rw-r--r--   0 root         (0) root         (0)     1574 2024-04-24 15:26:04.000000 dciclient-3.5.0.post202404241416/dciclient/v1/shell_commands/team.py
+-rw-r--r--   0 root         (0) root         (0)     2037 2024-04-24 15:26:04.000000 dciclient-3.5.0.post202404241416/dciclient/v1/shell_commands/topic.py
+-rw-r--r--   0 root         (0) root         (0)     1827 2024-04-24 15:26:04.000000 dciclient-3.5.0.post202404241416/dciclient/v1/shell_commands/user.py
+-rw-r--r--   0 root         (0) root         (0)     1868 2024-04-24 15:26:04.000000 dciclient-3.5.0.post202404241416/dciclient/v1/utils.py
+-rw-r--r--   0 root         (0) root         (0)     1544 2024-04-24 15:26:04.000000 dciclient-3.5.0.post202404241416/dciclient/vault.py
+-rw-r--r--   0 root         (0) root         (0)     1838 2024-04-24 15:26:04.000000 dciclient-3.5.0.post202404241416/dciclient/vault_client.py
+-rw-r--r--   0 root         (0) root         (0)       51 2024-04-24 15:27:04.000000 dciclient-3.5.0.post202404241416/dciclient/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 15:27:05.030430 dciclient-3.5.0.post202404241416/dciclient.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    10749 2024-04-24 15:27:04.000000 dciclient-3.5.0.post202404241416/dciclient.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1716 2024-04-24 15:27:04.000000 dciclient-3.5.0.post202404241416/dciclient.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-24 15:27:04.000000 dciclient-3.5.0.post202404241416/dciclient.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      392 2024-04-24 15:27:04.000000 dciclient-3.5.0.post202404241416/dciclient.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       60 2024-04-24 15:27:04.000000 dciclient-3.5.0.post202404241416/dciclient.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2024-04-24 15:27:04.000000 dciclient-3.5.0.post202404241416/dciclient.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       63 2024-04-24 15:26:04.000000 dciclient-3.5.0.post202404241416/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-24 15:27:05.035430 dciclient-3.5.0.post202404241416/setup.cfg
+-rwxr-xr-x   0 root         (0) root         (0)     3218 2024-04-24 15:26:04.000000 dciclient-3.5.0.post202404241416/setup.py
+-rwxr-xr-x   0 root         (0) root         (0)     1222 2024-04-24 15:26:04.000000 dciclient-3.5.0.post202404241416/start_db.sh
```

### Comparing `dciclient-3.5.0.post202403281939/LICENSE` & `dciclient-3.5.0.post202404241416/LICENSE`

 * *Files identical despite different names*

### Comparing `dciclient-3.5.0.post202403281939/PKG-INFO` & `dciclient-3.5.0.post202404241416/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dciclient
-Version: 3.5.0.post202403281939
+Version: 3.5.0.post202404241416
 Summary: Python client for DCI Control Server
 Home-page: https://github.com/redhat-cip/python-dciclient
 Author: Distributed CI team
 Author-email: distributed-ci@redhat.com
 License: Apache v2.0
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

### Comparing `dciclient-3.5.0.post202403281939/README.md` & `dciclient-3.5.0.post202404241416/README.md`

 * *Files identical despite different names*

### Comparing `dciclient-3.5.0.post202403281939/dciclient/create_component.py` & `dciclient-3.5.0.post202404241416/dciclient/create_component.py`

 * *Files identical despite different names*

### Comparing `dciclient-3.5.0.post202403281939/dciclient/create_job.py` & `dciclient-3.5.0.post202404241416/dciclient/create_job.py`

 * *Files identical despite different names*

### Comparing `dciclient-3.5.0.post202403281939/dciclient/diff_jobs.py` & `dciclient-3.5.0.post202404241416/dciclient/diff_jobs.py`

 * *Files identical despite different names*

### Comparing `dciclient-3.5.0.post202403281939/dciclient/find_latest_component.py` & `dciclient-3.5.0.post202404241416/dciclient/find_latest_component.py`

 * *Files identical despite different names*

### Comparing `dciclient-3.5.0.post202403281939/dciclient/printer.py` & `dciclient-3.5.0.post202404241416/dciclient/printer.py`

 * *Files identical despite different names*

### Comparing `dciclient-3.5.0.post202403281939/dciclient/rhel_kernel.py` & `dciclient-3.5.0.post202404241416/dciclient/rhel_kernel.py`

 * *Files identical despite different names*

### Comparing `dciclient-3.5.0.post202403281939/dciclient/shell.py` & `dciclient-3.5.0.post202404241416/dciclient/shell.py`

 * *Files identical despite different names*

### Comparing `dciclient-3.5.0.post202403281939/dciclient/v1/api/base.py` & `dciclient-3.5.0.post202404241416/dciclient/v1/api/base.py`

 * *Files identical despite different names*

### Comparing `dciclient-3.5.0.post202403281939/dciclient/v1/api/component.py` & `dciclient-3.5.0.post202404241416/dciclient/v1/api/component.py`

 * *Files identical despite different names*

### Comparing `dciclient-3.5.0.post202403281939/dciclient/v1/api/context.py` & `dciclient-3.5.0.post202404241416/dciclient/v1/api/context.py`

 * *Files identical despite different names*

### Comparing `dciclient-3.5.0.post202403281939/dciclient/v1/api/feeder.py` & `dciclient-3.5.0.post202404241416/dciclient/v1/api/feeder.py`

 * *Files identical despite different names*

### Comparing `dciclient-3.5.0.post202403281939/dciclient/v1/api/file.py` & `dciclient-3.5.0.post202404241416/dciclient/v1/api/file.py`

 * *Files identical despite different names*

### Comparing `dciclient-3.5.0.post202403281939/dciclient/v1/api/identity.py` & `dciclient-3.5.0.post202404241416/dciclient/v1/api/identity.py`

 * *Files identical despite different names*

### Comparing `dciclient-3.5.0.post202403281939/dciclient/v1/api/job.py` & `dciclient-3.5.0.post202404241416/dciclient/v1/api/job.py`

 * *Files identical despite different names*

### Comparing `dciclient-3.5.0.post202403281939/dciclient/v1/api/jobs_events.py` & `dciclient-3.5.0.post202404241416/dciclient/v1/api/jobs_events.py`

 * *Files identical despite different names*

### Comparing `dciclient-3.5.0.post202403281939/dciclient/v1/api/jobstate.py` & `dciclient-3.5.0.post202404241416/dciclient/v1/api/jobstate.py`

 * *Files identical despite different names*

### Comparing `dciclient-3.5.0.post202403281939/dciclient/v1/api/pipeline.py` & `dciclient-3.5.0.post202404241416/dciclient/v1/api/pipeline.py`

 * *Files identical despite different names*

### Comparing `dciclient-3.5.0.post202403281939/dciclient/v1/api/product.py` & `dciclient-3.5.0.post202404241416/dciclient/v1/api/product.py`

 * *Files identical despite different names*

### Comparing `dciclient-3.5.0.post202403281939/dciclient/v1/api/remoteci.py` & `dciclient-3.5.0.post202404241416/dciclient/v1/api/remoteci.py`

 * *Files identical despite different names*

### Comparing `dciclient-3.5.0.post202403281939/dciclient/v1/api/tag.py` & `dciclient-3.5.0.post202404241416/dciclient/v1/api/tag.py`

 * *Files identical despite different names*

### Comparing `dciclient-3.5.0.post202403281939/dciclient/v1/api/team.py` & `dciclient-3.5.0.post202404241416/dciclient/v1/api/team.py`

 * *Files identical despite different names*

### Comparing `dciclient-3.5.0.post202403281939/dciclient/v1/api/topic.py` & `dciclient-3.5.0.post202404241416/dciclient/v1/api/topic.py`

 * *Files identical despite different names*

### Comparing `dciclient-3.5.0.post202403281939/dciclient/v1/api/user.py` & `dciclient-3.5.0.post202404241416/dciclient/v1/api/user.py`

 * *Files identical despite different names*

### Comparing `dciclient-3.5.0.post202403281939/dciclient/v1/exceptions.py` & `dciclient-3.5.0.post202404241416/dciclient/v1/exceptions.py`

 * *Files identical despite different names*

### Comparing `dciclient-3.5.0.post202403281939/dciclient/v1/shell_commands/cli.py` & `dciclient-3.5.0.post202404241416/dciclient/v1/shell_commands/cli.py`

 * *Files identical despite different names*

### Comparing `dciclient-3.5.0.post202403281939/dciclient/v1/shell_commands/columns.py` & `dciclient-3.5.0.post202404241416/dciclient/v1/shell_commands/columns.py`

 * *Files identical despite different names*

### Comparing `dciclient-3.5.0.post202403281939/dciclient/v1/shell_commands/component.py` & `dciclient-3.5.0.post202404241416/dciclient/v1/shell_commands/component.py`

 * *Files identical despite different names*

### Comparing `dciclient-3.5.0.post202403281939/dciclient/v1/shell_commands/context.py` & `dciclient-3.5.0.post202404241416/dciclient/v1/shell_commands/context.py`

 * *Files identical despite different names*

### Comparing `dciclient-3.5.0.post202403281939/dciclient/v1/shell_commands/feeder.py` & `dciclient-3.5.0.post202404241416/dciclient/v1/shell_commands/feeder.py`

 * *Files identical despite different names*

### Comparing `dciclient-3.5.0.post202403281939/dciclient/v1/shell_commands/file.py` & `dciclient-3.5.0.post202404241416/dciclient/v1/shell_commands/file.py`

 * *Files identical despite different names*

### Comparing `dciclient-3.5.0.post202403281939/dciclient/v1/shell_commands/job.py` & `dciclient-3.5.0.post202404241416/dciclient/v1/shell_commands/job.py`

 * *Files identical despite different names*

### Comparing `dciclient-3.5.0.post202403281939/dciclient/v1/shell_commands/jobstate.py` & `dciclient-3.5.0.post202404241416/dciclient/v1/shell_commands/jobstate.py`

 * *Files identical despite different names*

### Comparing `dciclient-3.5.0.post202403281939/dciclient/v1/shell_commands/pipeline.py` & `dciclient-3.5.0.post202404241416/dciclient/v1/shell_commands/pipeline.py`

 * *Files identical despite different names*

### Comparing `dciclient-3.5.0.post202403281939/dciclient/v1/shell_commands/product.py` & `dciclient-3.5.0.post202404241416/dciclient/v1/shell_commands/product.py`

 * *Files identical despite different names*

### Comparing `dciclient-3.5.0.post202403281939/dciclient/v1/shell_commands/purge.py` & `dciclient-3.5.0.post202404241416/dciclient/v1/shell_commands/purge.py`

 * *Files identical despite different names*

### Comparing `dciclient-3.5.0.post202403281939/dciclient/v1/shell_commands/remoteci.py` & `dciclient-3.5.0.post202404241416/dciclient/v1/shell_commands/remoteci.py`

 * *Files identical despite different names*

### Comparing `dciclient-3.5.0.post202403281939/dciclient/v1/shell_commands/runner.py` & `dciclient-3.5.0.post202404241416/dciclient/v1/shell_commands/runner.py`

 * *Files identical despite different names*

### Comparing `dciclient-3.5.0.post202403281939/dciclient/v1/shell_commands/team.py` & `dciclient-3.5.0.post202404241416/dciclient/v1/shell_commands/team.py`

 * *Files identical despite different names*

### Comparing `dciclient-3.5.0.post202403281939/dciclient/v1/shell_commands/topic.py` & `dciclient-3.5.0.post202404241416/dciclient/v1/shell_commands/topic.py`

 * *Files identical despite different names*

### Comparing `dciclient-3.5.0.post202403281939/dciclient/v1/shell_commands/user.py` & `dciclient-3.5.0.post202404241416/dciclient/v1/shell_commands/user.py`

 * *Files identical despite different names*

### Comparing `dciclient-3.5.0.post202403281939/dciclient/v1/utils.py` & `dciclient-3.5.0.post202404241416/dciclient/v1/utils.py`

 * *Files identical despite different names*

### Comparing `dciclient-3.5.0.post202403281939/dciclient/vault.py` & `dciclient-3.5.0.post202404241416/dciclient/vault.py`

 * *Files identical despite different names*

### Comparing `dciclient-3.5.0.post202403281939/dciclient/vault_client.py` & `dciclient-3.5.0.post202404241416/dciclient/vault_client.py`

 * *Files identical despite different names*

### Comparing `dciclient-3.5.0.post202403281939/dciclient.egg-info/PKG-INFO` & `dciclient-3.5.0.post202404241416/dciclient.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dciclient
-Version: 3.5.0.post202403281939
+Version: 3.5.0.post202404241416
 Summary: Python client for DCI Control Server
 Home-page: https://github.com/redhat-cip/python-dciclient
 Author: Distributed CI team
 Author-email: distributed-ci@redhat.com
 License: Apache v2.0
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

### Comparing `dciclient-3.5.0.post202403281939/dciclient.egg-info/SOURCES.txt` & `dciclient-3.5.0.post202404241416/dciclient.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dciclient-3.5.0.post202403281939/setup.py` & `dciclient-3.5.0.post202404241416/setup.py`

 * *Files identical despite different names*

### Comparing `dciclient-3.5.0.post202403281939/start_db.sh` & `dciclient-3.5.0.post202404241416/start_db.sh`

 * *Files identical despite different names*


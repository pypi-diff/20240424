# Comparing `tmp/opentaskpy-24.8.0.tar.gz` & `tmp/opentaskpy-24.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opentaskpy-24.8.0.tar", last modified: Wed Feb 21 14:21:16 2024, max compression
+gzip compressed data, was "opentaskpy-24.9.0.tar", last modified: Sat Mar  2 16:55:37 2024, max compression
```

## Comparing `opentaskpy-24.8.0.tar` & `opentaskpy-24.9.0.tar`

### file list

```diff
@@ -1,118 +1,118 @@
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-02-21 14:21:16.528947 opentaskpy-24.8.0/
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)       72 2024-01-29 14:21:30.000000 opentaskpy-24.8.0/AUTHORS
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)    35149 2024-01-29 14:21:30.000000 opentaskpy-24.8.0/LICENSE
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)       44 2024-01-29 14:21:30.000000 opentaskpy-24.8.0/MANIFEST.in
--rw-r--r--   0 vscode    (1000) vscode    (1000)    22911 2024-02-21 14:21:16.528947 opentaskpy-24.8.0/PKG-INFO
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)    21238 2024-02-21 13:56:48.000000 opentaskpy-24.8.0/README.md
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)    14640 2024-02-21 14:21:05.000000 opentaskpy-24.8.0/pyproject.toml
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)       38 2024-02-21 14:21:16.528947 opentaskpy-24.8.0/setup.cfg
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-02-21 14:21:16.496947 opentaskpy-24.8.0/src/
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-02-21 14:21:16.504947 opentaskpy-24.8.0/src/opentaskpy/
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-02-21 14:21:16.504947 opentaskpy-24.8.0/src/opentaskpy/cli/
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     3733 2024-02-21 13:50:29.000000 opentaskpy-24.8.0/src/opentaskpy/cli/batch_validator.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     4596 2024-02-19 17:54:38.000000 opentaskpy-24.8.0/src/opentaskpy/cli/task_run.py
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-02-21 14:21:16.504947 opentaskpy-24.8.0/src/opentaskpy/config/
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)        0 2024-01-29 14:21:30.000000 opentaskpy-24.8.0/src/opentaskpy/config/__init__.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)    13622 2024-02-19 17:49:36.000000 opentaskpy-24.8.0/src/opentaskpy/config/loader.py
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-02-21 14:21:16.500947 opentaskpy-24.8.0/src/opentaskpy/config/schemas/
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-02-21 14:21:16.504947 opentaskpy-24.8.0/src/opentaskpy/config/schemas/batch/
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1754 2024-01-29 14:21:30.000000 opentaskpy-24.8.0/src/opentaskpy/config/schemas/batch/tasks.json
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-02-21 14:21:16.500947 opentaskpy-24.8.0/src/opentaskpy/config/schemas/execution/
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-02-21 14:21:16.508947 opentaskpy-24.8.0/src/opentaskpy/config/schemas/execution/local/
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)      444 2024-01-29 14:21:30.000000 opentaskpy-24.8.0/src/opentaskpy/config/schemas/execution/local/local.json
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)      291 2024-01-29 14:21:30.000000 opentaskpy-24.8.0/src/opentaskpy/config/schemas/execution/local/protocol.json
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-02-21 14:21:16.508947 opentaskpy-24.8.0/src/opentaskpy/config/schemas/execution/ssh/
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)      616 2024-01-29 14:21:30.000000 opentaskpy-24.8.0/src/opentaskpy/config/schemas/execution/ssh/protocol.json
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)      546 2024-01-29 14:21:30.000000 opentaskpy-24.8.0/src/opentaskpy/config/schemas/execution/ssh/ssh.json
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-02-21 14:21:16.508947 opentaskpy-24.8.0/src/opentaskpy/config/schemas/transfer/
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-02-21 14:21:16.508947 opentaskpy-24.8.0/src/opentaskpy/config/schemas/transfer/email/
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)      833 2024-01-29 14:21:30.000000 opentaskpy-24.8.0/src/opentaskpy/config/schemas/transfer/email/protocol.json
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)      517 2024-01-29 14:21:30.000000 opentaskpy-24.8.0/src/opentaskpy/config/schemas/transfer/email_destination.json
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-02-21 14:21:16.512947 opentaskpy-24.8.0/src/opentaskpy/config/schemas/transfer/local_destination/
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)      282 2024-01-29 14:21:30.000000 opentaskpy-24.8.0/src/opentaskpy/config/schemas/transfer/local_destination/flags.json
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)      256 2024-01-29 14:21:30.000000 opentaskpy-24.8.0/src/opentaskpy/config/schemas/transfer/local_destination/permissions.json
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)      302 2024-01-29 14:21:30.000000 opentaskpy-24.8.0/src/opentaskpy/config/schemas/transfer/local_destination/protocol.json
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)      331 2024-01-29 14:21:30.000000 opentaskpy-24.8.0/src/opentaskpy/config/schemas/transfer/local_destination/rename.json
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)      910 2024-01-29 14:21:30.000000 opentaskpy-24.8.0/src/opentaskpy/config/schemas/transfer/local_destination.json
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-02-21 14:21:16.512947 opentaskpy-24.8.0/src/opentaskpy/config/schemas/transfer/local_source/
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)      899 2024-01-29 14:21:30.000000 opentaskpy-24.8.0/src/opentaskpy/config/schemas/transfer/local_source/conditionals.json
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)      401 2024-01-29 14:21:30.000000 opentaskpy-24.8.0/src/opentaskpy/config/schemas/transfer/local_source/fileWatch.json
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1238 2024-01-29 14:21:30.000000 opentaskpy-24.8.0/src/opentaskpy/config/schemas/transfer/local_source/postCopyAction.json
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)      297 2024-01-29 14:21:30.000000 opentaskpy-24.8.0/src/opentaskpy/config/schemas/transfer/local_source/protocol.json
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)      791 2024-01-29 14:21:30.000000 opentaskpy-24.8.0/src/opentaskpy/config/schemas/transfer/local_source.json
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-02-21 14:21:16.512947 opentaskpy-24.8.0/src/opentaskpy/config/schemas/transfer/sftp_destination/
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)      281 2024-01-29 14:21:30.000000 opentaskpy-24.8.0/src/opentaskpy/config/schemas/transfer/sftp_destination/flags.json
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)      255 2024-01-29 14:21:30.000000 opentaskpy-24.8.0/src/opentaskpy/config/schemas/transfer/sftp_destination/permissions.json
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1242 2024-02-15 17:36:32.000000 opentaskpy-24.8.0/src/opentaskpy/config/schemas/transfer/sftp_destination/protocol.json
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)      330 2024-01-29 14:21:30.000000 opentaskpy-24.8.0/src/opentaskpy/config/schemas/transfer/sftp_destination/rename.json
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)      763 2024-01-29 14:21:30.000000 opentaskpy-24.8.0/src/opentaskpy/config/schemas/transfer/sftp_destination.json
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-02-21 14:21:16.512947 opentaskpy-24.8.0/src/opentaskpy/config/schemas/transfer/sftp_source/
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)      898 2024-01-29 14:21:30.000000 opentaskpy-24.8.0/src/opentaskpy/config/schemas/transfer/sftp_source/conditionals.json
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)      400 2024-01-29 14:21:30.000000 opentaskpy-24.8.0/src/opentaskpy/config/schemas/transfer/sftp_source/fileWatch.json
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1237 2024-01-29 14:21:30.000000 opentaskpy-24.8.0/src/opentaskpy/config/schemas/transfer/sftp_source/postCopyAction.json
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)      739 2024-02-15 17:36:32.000000 opentaskpy-24.8.0/src/opentaskpy/config/schemas/transfer/sftp_source/protocol.json
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)      846 2024-01-29 14:21:30.000000 opentaskpy-24.8.0/src/opentaskpy/config/schemas/transfer/sftp_source.json
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-02-21 14:21:16.516947 opentaskpy-24.8.0/src/opentaskpy/config/schemas/transfer/ssh_destination/
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)      280 2024-01-29 14:21:30.000000 opentaskpy-24.8.0/src/opentaskpy/config/schemas/transfer/ssh_destination/flags.json
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)      344 2024-01-29 14:21:30.000000 opentaskpy-24.8.0/src/opentaskpy/config/schemas/transfer/ssh_destination/permissions.json
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1180 2024-02-15 17:36:32.000000 opentaskpy-24.8.0/src/opentaskpy/config/schemas/transfer/ssh_destination/protocol.json
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)      329 2024-01-29 14:21:30.000000 opentaskpy-24.8.0/src/opentaskpy/config/schemas/transfer/ssh_destination/rename.json
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)      960 2024-01-29 14:21:30.000000 opentaskpy-24.8.0/src/opentaskpy/config/schemas/transfer/ssh_destination.json
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-02-21 14:21:16.516947 opentaskpy-24.8.0/src/opentaskpy/config/schemas/transfer/ssh_source/
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)      897 2024-01-29 14:21:30.000000 opentaskpy-24.8.0/src/opentaskpy/config/schemas/transfer/ssh_source/conditionals.json
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)      398 2024-01-29 14:21:30.000000 opentaskpy-24.8.0/src/opentaskpy/config/schemas/transfer/ssh_source/fileWatch.json
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)      491 2024-01-29 14:21:30.000000 opentaskpy-24.8.0/src/opentaskpy/config/schemas/transfer/ssh_source/logWatch.json
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1236 2024-01-29 14:21:30.000000 opentaskpy-24.8.0/src/opentaskpy/config/schemas/transfer/ssh_source/postCopyAction.json
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)      677 2024-02-15 17:36:32.000000 opentaskpy-24.8.0/src/opentaskpy/config/schemas/transfer/ssh_source/protocol.json
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)      933 2024-01-29 14:21:30.000000 opentaskpy-24.8.0/src/opentaskpy/config/schemas/transfer/ssh_source.json
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)    11964 2024-02-15 17:36:32.000000 opentaskpy-24.8.0/src/opentaskpy/config/schemas.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     2400 2024-02-15 17:36:32.000000 opentaskpy-24.8.0/src/opentaskpy/exceptions.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)    10124 2024-02-15 17:36:32.000000 opentaskpy-24.8.0/src/opentaskpy/otflogging.py
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-02-21 14:21:16.500947 opentaskpy-24.8.0/src/opentaskpy/plugins/
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-02-21 14:21:16.516947 opentaskpy-24.8.0/src/opentaskpy/plugins/lookup/
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1415 2024-02-15 17:36:32.000000 opentaskpy-24.8.0/src/opentaskpy/plugins/lookup/file.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1905 2024-02-15 17:36:32.000000 opentaskpy-24.8.0/src/opentaskpy/plugins/lookup/http_json.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1110 2024-02-15 17:36:32.000000 opentaskpy-24.8.0/src/opentaskpy/plugins/lookup/random_number.py
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-02-21 14:21:16.520947 opentaskpy-24.8.0/src/opentaskpy/remotehandlers/
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)        0 2024-01-29 14:21:30.000000 opentaskpy-24.8.0/src/opentaskpy/remotehandlers/__init__.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     5747 2024-02-15 17:36:32.000000 opentaskpy-24.8.0/src/opentaskpy/remotehandlers/email.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)    17410 2024-02-15 17:36:32.000000 opentaskpy-24.8.0/src/opentaskpy/remotehandlers/local.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     4423 2024-02-15 17:36:32.000000 opentaskpy-24.8.0/src/opentaskpy/remotehandlers/remotehandler.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)    18080 2024-02-15 17:36:32.000000 opentaskpy-24.8.0/src/opentaskpy/remotehandlers/sftp.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)    42099 2024-02-15 17:36:32.000000 opentaskpy-24.8.0/src/opentaskpy/remotehandlers/ssh.py
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-02-21 14:21:16.520947 opentaskpy-24.8.0/src/opentaskpy/taskhandlers/
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)        0 2024-01-29 14:21:30.000000 opentaskpy-24.8.0/src/opentaskpy/taskhandlers/__init__.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)    19724 2024-02-21 13:51:42.000000 opentaskpy-24.8.0/src/opentaskpy/taskhandlers/batch.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     8696 2024-02-15 17:36:32.000000 opentaskpy-24.8.0/src/opentaskpy/taskhandlers/execution.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     4666 2024-02-15 17:36:32.000000 opentaskpy-24.8.0/src/opentaskpy/taskhandlers/taskhandler.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)    25010 2024-01-29 14:28:45.000000 opentaskpy-24.8.0/src/opentaskpy/taskhandlers/transfer.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     4723 2024-02-21 11:36:16.000000 opentaskpy-24.8.0/src/opentaskpy/taskrun.py
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-02-21 14:21:16.528947 opentaskpy-24.8.0/src/opentaskpy.egg-info/
--rw-r--r--   0 vscode    (1000) vscode    (1000)    22911 2024-02-21 14:21:16.000000 opentaskpy-24.8.0/src/opentaskpy.egg-info/PKG-INFO
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     4289 2024-02-21 14:21:16.000000 opentaskpy-24.8.0/src/opentaskpy.egg-info/SOURCES.txt
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)        1 2024-02-21 14:21:16.000000 opentaskpy-24.8.0/src/opentaskpy.egg-info/dependency_links.txt
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)      116 2024-02-21 14:21:16.000000 opentaskpy-24.8.0/src/opentaskpy.egg-info/entry_points.txt
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)      277 2024-02-21 14:21:16.000000 opentaskpy-24.8.0/src/opentaskpy.egg-info/requires.txt
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)       11 2024-02-21 14:21:16.000000 opentaskpy-24.8.0/src/opentaskpy.egg-info/top_level.txt
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-02-21 14:21:16.528947 opentaskpy-24.8.0/tests/
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1483 2024-01-29 14:21:30.000000 opentaskpy-24.8.0/tests/test_batch_schema_validate.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     3485 2024-02-21 14:14:12.000000 opentaskpy-24.8.0/tests/test_batch_validator.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)    16708 2024-02-15 17:36:32.000000 opentaskpy-24.8.0/tests/test_config_loader.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     6928 2024-01-29 14:21:30.000000 opentaskpy-24.8.0/tests/test_docker_task_run.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)      989 2024-01-29 14:21:30.000000 opentaskpy-24.8.0/tests/test_email_transfer_schema_validate.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)      852 2024-01-29 14:21:30.000000 opentaskpy-24.8.0/tests/test_file_helper.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     8070 2024-01-29 14:21:30.000000 opentaskpy-24.8.0/tests/test_logging.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)      942 2024-01-29 14:21:30.000000 opentaskpy-24.8.0/tests/test_plugin_file.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1146 2024-01-29 14:21:30.000000 opentaskpy-24.8.0/tests/test_plugin_http_json.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     2270 2024-01-29 14:21:30.000000 opentaskpy-24.8.0/tests/test_schema_validate.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     3555 2024-01-29 14:21:30.000000 opentaskpy-24.8.0/tests/test_ssh_dest_schema_validate.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1080 2024-01-29 14:21:30.000000 opentaskpy-24.8.0/tests/test_ssh_execution_schema_validate.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     5894 2024-01-29 14:21:30.000000 opentaskpy-24.8.0/tests/test_ssh_source_schema_validate.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)    15825 2024-02-21 13:12:32.000000 opentaskpy-24.8.0/tests/test_task_run.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)    15367 2024-01-29 14:21:30.000000 opentaskpy-24.8.0/tests/test_taskhandler_batch.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     2718 2024-01-29 14:21:30.000000 opentaskpy-24.8.0/tests/test_taskhandler_execution_local.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     4337 2024-01-29 14:21:30.000000 opentaskpy-24.8.0/tests/test_taskhandler_execution_ssh.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     4921 2024-01-29 14:21:30.000000 opentaskpy-24.8.0/tests/test_taskhandler_transfer_email.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)    17809 2024-01-29 14:21:30.000000 opentaskpy-24.8.0/tests/test_taskhandler_transfer_local.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)    21097 2024-02-15 17:36:32.000000 opentaskpy-24.8.0/tests/test_taskhandler_transfer_sftp.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)    18844 2024-02-15 17:36:32.000000 opentaskpy-24.8.0/tests/test_taskhandler_transfer_ssh.py
+drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-03-02 16:55:37.260736 opentaskpy-24.9.0/
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)       72 2024-01-29 14:21:30.000000 opentaskpy-24.9.0/AUTHORS
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)    35149 2024-01-29 14:21:30.000000 opentaskpy-24.9.0/LICENSE
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)       44 2024-01-29 14:21:30.000000 opentaskpy-24.9.0/MANIFEST.in
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    22942 2024-03-02 16:55:37.260736 opentaskpy-24.9.0/PKG-INFO
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)    21238 2024-03-02 13:05:49.000000 opentaskpy-24.9.0/README.md
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)    14665 2024-03-02 16:55:26.000000 opentaskpy-24.9.0/pyproject.toml
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)       38 2024-03-02 16:55:37.260736 opentaskpy-24.9.0/setup.cfg
+drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-03-02 16:55:37.200736 opentaskpy-24.9.0/src/
+drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-03-02 16:55:37.216736 opentaskpy-24.9.0/src/opentaskpy/
+drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-03-02 16:55:37.220736 opentaskpy-24.9.0/src/opentaskpy/cli/
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     3733 2024-03-02 13:05:49.000000 opentaskpy-24.9.0/src/opentaskpy/cli/batch_validator.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     4596 2024-03-02 13:05:49.000000 opentaskpy-24.9.0/src/opentaskpy/cli/task_run.py
+drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-03-02 16:55:37.220736 opentaskpy-24.9.0/src/opentaskpy/config/
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)        0 2024-01-29 14:21:30.000000 opentaskpy-24.9.0/src/opentaskpy/config/__init__.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)    13622 2024-03-02 13:05:49.000000 opentaskpy-24.9.0/src/opentaskpy/config/loader.py
+drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-03-02 16:55:37.204736 opentaskpy-24.9.0/src/opentaskpy/config/schemas/
+drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-03-02 16:55:37.220736 opentaskpy-24.9.0/src/opentaskpy/config/schemas/batch/
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1754 2024-01-29 14:21:30.000000 opentaskpy-24.9.0/src/opentaskpy/config/schemas/batch/tasks.json
+drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-03-02 16:55:37.204736 opentaskpy-24.9.0/src/opentaskpy/config/schemas/execution/
+drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-03-02 16:55:37.224737 opentaskpy-24.9.0/src/opentaskpy/config/schemas/execution/local/
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)      444 2024-01-29 14:21:30.000000 opentaskpy-24.9.0/src/opentaskpy/config/schemas/execution/local/local.json
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)      291 2024-01-29 14:21:30.000000 opentaskpy-24.9.0/src/opentaskpy/config/schemas/execution/local/protocol.json
+drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-03-02 16:55:37.228736 opentaskpy-24.9.0/src/opentaskpy/config/schemas/execution/ssh/
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)      616 2024-01-29 14:21:30.000000 opentaskpy-24.9.0/src/opentaskpy/config/schemas/execution/ssh/protocol.json
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)      546 2024-01-29 14:21:30.000000 opentaskpy-24.9.0/src/opentaskpy/config/schemas/execution/ssh/ssh.json
+drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-03-02 16:55:37.232736 opentaskpy-24.9.0/src/opentaskpy/config/schemas/transfer/
+drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-03-02 16:55:37.232736 opentaskpy-24.9.0/src/opentaskpy/config/schemas/transfer/email/
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)      833 2024-01-29 14:21:30.000000 opentaskpy-24.9.0/src/opentaskpy/config/schemas/transfer/email/protocol.json
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)      517 2024-01-29 14:21:30.000000 opentaskpy-24.9.0/src/opentaskpy/config/schemas/transfer/email_destination.json
+drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-03-02 16:55:37.236736 opentaskpy-24.9.0/src/opentaskpy/config/schemas/transfer/local_destination/
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)      282 2024-01-29 14:21:30.000000 opentaskpy-24.9.0/src/opentaskpy/config/schemas/transfer/local_destination/flags.json
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)      256 2024-01-29 14:21:30.000000 opentaskpy-24.9.0/src/opentaskpy/config/schemas/transfer/local_destination/permissions.json
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)      302 2024-01-29 14:21:30.000000 opentaskpy-24.9.0/src/opentaskpy/config/schemas/transfer/local_destination/protocol.json
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)      331 2024-01-29 14:21:30.000000 opentaskpy-24.9.0/src/opentaskpy/config/schemas/transfer/local_destination/rename.json
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)      910 2024-01-29 14:21:30.000000 opentaskpy-24.9.0/src/opentaskpy/config/schemas/transfer/local_destination.json
+drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-03-02 16:55:37.236736 opentaskpy-24.9.0/src/opentaskpy/config/schemas/transfer/local_source/
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)      899 2024-01-29 14:21:30.000000 opentaskpy-24.9.0/src/opentaskpy/config/schemas/transfer/local_source/conditionals.json
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)      401 2024-01-29 14:21:30.000000 opentaskpy-24.9.0/src/opentaskpy/config/schemas/transfer/local_source/fileWatch.json
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1238 2024-01-29 14:21:30.000000 opentaskpy-24.9.0/src/opentaskpy/config/schemas/transfer/local_source/postCopyAction.json
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)      297 2024-01-29 14:21:30.000000 opentaskpy-24.9.0/src/opentaskpy/config/schemas/transfer/local_source/protocol.json
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)      791 2024-01-29 14:21:30.000000 opentaskpy-24.9.0/src/opentaskpy/config/schemas/transfer/local_source.json
+drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-03-02 16:55:37.236736 opentaskpy-24.9.0/src/opentaskpy/config/schemas/transfer/sftp_destination/
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)      281 2024-01-29 14:21:30.000000 opentaskpy-24.9.0/src/opentaskpy/config/schemas/transfer/sftp_destination/flags.json
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)      255 2024-01-29 14:21:30.000000 opentaskpy-24.9.0/src/opentaskpy/config/schemas/transfer/sftp_destination/permissions.json
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1242 2024-02-15 17:36:32.000000 opentaskpy-24.9.0/src/opentaskpy/config/schemas/transfer/sftp_destination/protocol.json
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)      330 2024-01-29 14:21:30.000000 opentaskpy-24.9.0/src/opentaskpy/config/schemas/transfer/sftp_destination/rename.json
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)      763 2024-01-29 14:21:30.000000 opentaskpy-24.9.0/src/opentaskpy/config/schemas/transfer/sftp_destination.json
+drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-03-02 16:55:37.240736 opentaskpy-24.9.0/src/opentaskpy/config/schemas/transfer/sftp_source/
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)      898 2024-01-29 14:21:30.000000 opentaskpy-24.9.0/src/opentaskpy/config/schemas/transfer/sftp_source/conditionals.json
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)      400 2024-01-29 14:21:30.000000 opentaskpy-24.9.0/src/opentaskpy/config/schemas/transfer/sftp_source/fileWatch.json
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1237 2024-01-29 14:21:30.000000 opentaskpy-24.9.0/src/opentaskpy/config/schemas/transfer/sftp_source/postCopyAction.json
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)      739 2024-02-15 17:36:32.000000 opentaskpy-24.9.0/src/opentaskpy/config/schemas/transfer/sftp_source/protocol.json
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)      846 2024-01-29 14:21:30.000000 opentaskpy-24.9.0/src/opentaskpy/config/schemas/transfer/sftp_source.json
+drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-03-02 16:55:37.240736 opentaskpy-24.9.0/src/opentaskpy/config/schemas/transfer/ssh_destination/
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)      280 2024-01-29 14:21:30.000000 opentaskpy-24.9.0/src/opentaskpy/config/schemas/transfer/ssh_destination/flags.json
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)      344 2024-01-29 14:21:30.000000 opentaskpy-24.9.0/src/opentaskpy/config/schemas/transfer/ssh_destination/permissions.json
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1180 2024-02-15 17:36:32.000000 opentaskpy-24.9.0/src/opentaskpy/config/schemas/transfer/ssh_destination/protocol.json
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)      329 2024-01-29 14:21:30.000000 opentaskpy-24.9.0/src/opentaskpy/config/schemas/transfer/ssh_destination/rename.json
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)      960 2024-01-29 14:21:30.000000 opentaskpy-24.9.0/src/opentaskpy/config/schemas/transfer/ssh_destination.json
+drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-03-02 16:55:37.244737 opentaskpy-24.9.0/src/opentaskpy/config/schemas/transfer/ssh_source/
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)      897 2024-01-29 14:21:30.000000 opentaskpy-24.9.0/src/opentaskpy/config/schemas/transfer/ssh_source/conditionals.json
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)      398 2024-01-29 14:21:30.000000 opentaskpy-24.9.0/src/opentaskpy/config/schemas/transfer/ssh_source/fileWatch.json
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)      491 2024-01-29 14:21:30.000000 opentaskpy-24.9.0/src/opentaskpy/config/schemas/transfer/ssh_source/logWatch.json
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1236 2024-01-29 14:21:30.000000 opentaskpy-24.9.0/src/opentaskpy/config/schemas/transfer/ssh_source/postCopyAction.json
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)      677 2024-02-15 17:36:32.000000 opentaskpy-24.9.0/src/opentaskpy/config/schemas/transfer/ssh_source/protocol.json
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)      933 2024-01-29 14:21:30.000000 opentaskpy-24.9.0/src/opentaskpy/config/schemas/transfer/ssh_source.json
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)    11964 2024-02-15 17:36:32.000000 opentaskpy-24.9.0/src/opentaskpy/config/schemas.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     2400 2024-02-15 17:36:32.000000 opentaskpy-24.9.0/src/opentaskpy/exceptions.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)    10122 2024-03-02 16:55:26.000000 opentaskpy-24.9.0/src/opentaskpy/otflogging.py
+drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-03-02 16:55:37.208737 opentaskpy-24.9.0/src/opentaskpy/plugins/
+drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-03-02 16:55:37.244737 opentaskpy-24.9.0/src/opentaskpy/plugins/lookup/
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1415 2024-02-15 17:36:32.000000 opentaskpy-24.9.0/src/opentaskpy/plugins/lookup/file.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1905 2024-02-15 17:36:32.000000 opentaskpy-24.9.0/src/opentaskpy/plugins/lookup/http_json.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1110 2024-02-15 17:36:32.000000 opentaskpy-24.9.0/src/opentaskpy/plugins/lookup/random_number.py
+drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-03-02 16:55:37.248736 opentaskpy-24.9.0/src/opentaskpy/remotehandlers/
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)        0 2024-01-29 14:21:30.000000 opentaskpy-24.9.0/src/opentaskpy/remotehandlers/__init__.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     5747 2024-02-15 17:36:32.000000 opentaskpy-24.9.0/src/opentaskpy/remotehandlers/email.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)    16764 2024-03-02 16:55:26.000000 opentaskpy-24.9.0/src/opentaskpy/remotehandlers/local.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     4423 2024-02-15 17:36:32.000000 opentaskpy-24.9.0/src/opentaskpy/remotehandlers/remotehandler.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)    18698 2024-03-02 16:55:26.000000 opentaskpy-24.9.0/src/opentaskpy/remotehandlers/sftp.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)    42486 2024-03-02 16:55:26.000000 opentaskpy-24.9.0/src/opentaskpy/remotehandlers/ssh.py
+drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-03-02 16:55:37.248736 opentaskpy-24.9.0/src/opentaskpy/taskhandlers/
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)        0 2024-01-29 14:21:30.000000 opentaskpy-24.9.0/src/opentaskpy/taskhandlers/__init__.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)    19816 2024-03-02 16:55:26.000000 opentaskpy-24.9.0/src/opentaskpy/taskhandlers/batch.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     8696 2024-02-15 17:36:32.000000 opentaskpy-24.9.0/src/opentaskpy/taskhandlers/execution.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     4666 2024-02-15 17:36:32.000000 opentaskpy-24.9.0/src/opentaskpy/taskhandlers/taskhandler.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)    25753 2024-03-02 16:55:26.000000 opentaskpy-24.9.0/src/opentaskpy/taskhandlers/transfer.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     4723 2024-03-02 13:05:49.000000 opentaskpy-24.9.0/src/opentaskpy/taskrun.py
+drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-03-02 16:55:37.260736 opentaskpy-24.9.0/src/opentaskpy.egg-info/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    22942 2024-03-02 16:55:37.000000 opentaskpy-24.9.0/src/opentaskpy.egg-info/PKG-INFO
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     4289 2024-03-02 16:55:37.000000 opentaskpy-24.9.0/src/opentaskpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)        1 2024-03-02 16:55:37.000000 opentaskpy-24.9.0/src/opentaskpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)      116 2024-03-02 16:55:37.000000 opentaskpy-24.9.0/src/opentaskpy.egg-info/entry_points.txt
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)      293 2024-03-02 16:55:37.000000 opentaskpy-24.9.0/src/opentaskpy.egg-info/requires.txt
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)       11 2024-03-02 16:55:37.000000 opentaskpy-24.9.0/src/opentaskpy.egg-info/top_level.txt
+drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-03-02 16:55:37.256736 opentaskpy-24.9.0/tests/
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1483 2024-01-29 14:21:30.000000 opentaskpy-24.9.0/tests/test_batch_schema_validate.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     3485 2024-03-02 13:05:49.000000 opentaskpy-24.9.0/tests/test_batch_validator.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)    16708 2024-02-15 17:36:32.000000 opentaskpy-24.9.0/tests/test_config_loader.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     6928 2024-01-29 14:21:30.000000 opentaskpy-24.9.0/tests/test_docker_task_run.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)      989 2024-01-29 14:21:30.000000 opentaskpy-24.9.0/tests/test_email_transfer_schema_validate.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)      852 2024-01-29 14:21:30.000000 opentaskpy-24.9.0/tests/test_file_helper.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     8070 2024-01-29 14:21:30.000000 opentaskpy-24.9.0/tests/test_logging.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)      942 2024-01-29 14:21:30.000000 opentaskpy-24.9.0/tests/test_plugin_file.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1146 2024-01-29 14:21:30.000000 opentaskpy-24.9.0/tests/test_plugin_http_json.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     2270 2024-01-29 14:21:30.000000 opentaskpy-24.9.0/tests/test_schema_validate.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     3555 2024-01-29 14:21:30.000000 opentaskpy-24.9.0/tests/test_ssh_dest_schema_validate.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1080 2024-01-29 14:21:30.000000 opentaskpy-24.9.0/tests/test_ssh_execution_schema_validate.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     5894 2024-01-29 14:21:30.000000 opentaskpy-24.9.0/tests/test_ssh_source_schema_validate.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)    16246 2024-03-02 16:55:26.000000 opentaskpy-24.9.0/tests/test_task_run.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)    16777 2024-03-02 16:55:26.000000 opentaskpy-24.9.0/tests/test_taskhandler_batch.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     2718 2024-01-29 14:21:30.000000 opentaskpy-24.9.0/tests/test_taskhandler_execution_local.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     4337 2024-01-29 14:21:30.000000 opentaskpy-24.9.0/tests/test_taskhandler_execution_ssh.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     4921 2024-01-29 14:21:30.000000 opentaskpy-24.9.0/tests/test_taskhandler_transfer_email.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)    17809 2024-03-02 15:56:18.000000 opentaskpy-24.9.0/tests/test_taskhandler_transfer_local.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)    21097 2024-02-15 17:36:32.000000 opentaskpy-24.9.0/tests/test_taskhandler_transfer_sftp.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)    18844 2024-02-15 17:36:32.000000 opentaskpy-24.9.0/tests/test_taskhandler_transfer_ssh.py
```

### Comparing `opentaskpy-24.8.0/LICENSE` & `opentaskpy-24.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `opentaskpy-24.8.0/PKG-INFO` & `opentaskpy-24.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentaskpy
-Version: 24.8.0
+Version: 24.9.0
 Summary: A framework for automation execution of commands and transferring files between hosts
 Author-email: Adam McDonagh <adam@elitemonkey.net>
 License: GPLv3
 Project-URL: Homepage, https://github.com/adammcdonagh/open-task-framework
 Project-URL: Bug Tracker, https://github.com/adammcdonagh/open-task-framework/issues
 Project-URL: Changelog, https://github.com/adammcdonagh/open-task-framework/blob/main/CHANGELOG.md
 Keywords: automation,task,framework,scheduling,ssh,sftp,remote,execution,command
@@ -17,14 +17,15 @@
 License-File: AUTHORS
 Requires-Dist: jinja2>=3.1
 Requires-Dist: jsonpath-ng>=1.5
 Requires-Dist: jsonschema>=4.17
 Requires-Dist: paramiko>=3.0
 Requires-Dist: requests>=2.28
 Requires-Dist: referencing>=0.29.1
+Requires-Dist: tenacity>=8.2.3
 Provides-Extra: dev
 Requires-Dist: types-requests>=2.28; extra == "dev"
 Requires-Dist: types-paramiko>=3.0; extra == "dev"
 Requires-Dist: black==24.1.1; extra == "dev"
 Requires-Dist: isort; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: bumpver; extra == "dev"
```

### Comparing `opentaskpy-24.8.0/README.md` & `opentaskpy-24.9.0/README.md`

 * *Files identical despite different names*

### Comparing `opentaskpy-24.8.0/pyproject.toml` & `opentaskpy-24.9.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "opentaskpy"
-version = "v24.8.0"
+version = "v24.9.0"
 authors = [{ name = "Adam McDonagh", email = "adam@elitemonkey.net" }]
 license = { text = "GPLv3" }
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: POSIX",
 ]
@@ -26,14 +26,15 @@
 dependencies = [
     "jinja2 >= 3.1",
     "jsonpath-ng >= 1.5",
     "jsonschema >= 4.17",
     "paramiko >= 3.0",
     "requests >= 2.28",
     "referencing >= 0.29.1",
+    "tenacity >= 8.2.3",
 ]
 description = "A framework for automation execution of commands and transferring files between hosts"
 readme = "README.md"
 requires-python = ">=3.11"
 
 [project.optional-dependencies]
 dev = [
@@ -63,15 +64,15 @@
 task-run = "opentaskpy.cli.task_run:main"
 otf-batch-validator = "opentaskpy.cli.batch_validator:main"
 
 [tool.isort]
 profile = 'black'
 
 [tool.bumpver]
-current_version = "v24.8.0"
+current_version = "v24.9.0"
 version_pattern = "vYY.WW.PATCH[-TAG]"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `opentaskpy-24.8.0/src/opentaskpy/cli/batch_validator.py` & `opentaskpy-24.9.0/src/opentaskpy/cli/batch_validator.py`

 * *Files identical despite different names*

### Comparing `opentaskpy-24.8.0/src/opentaskpy/cli/task_run.py` & `opentaskpy-24.9.0/src/opentaskpy/cli/task_run.py`

 * *Files identical despite different names*

### Comparing `opentaskpy-24.8.0/src/opentaskpy/config/loader.py` & `opentaskpy-24.9.0/src/opentaskpy/config/loader.py`

 * *Files identical despite different names*

### Comparing `opentaskpy-24.8.0/src/opentaskpy/config/schemas/batch/tasks.json` & `opentaskpy-24.9.0/src/opentaskpy/config/schemas/batch/tasks.json`

 * *Files identical despite different names*

### Comparing `opentaskpy-24.8.0/src/opentaskpy/config/schemas/execution/ssh/protocol.json` & `opentaskpy-24.9.0/src/opentaskpy/config/schemas/execution/ssh/protocol.json`

 * *Files identical despite different names*

### Comparing `opentaskpy-24.8.0/src/opentaskpy/config/schemas/execution/ssh/ssh.json` & `opentaskpy-24.9.0/src/opentaskpy/config/schemas/execution/ssh/ssh.json`

 * *Files identical despite different names*

### Comparing `opentaskpy-24.8.0/src/opentaskpy/config/schemas/transfer/email/protocol.json` & `opentaskpy-24.9.0/src/opentaskpy/config/schemas/transfer/email/protocol.json`

 * *Files identical despite different names*

### Comparing `opentaskpy-24.8.0/src/opentaskpy/config/schemas/transfer/email_destination.json` & `opentaskpy-24.9.0/src/opentaskpy/config/schemas/transfer/email_destination.json`

 * *Files identical despite different names*

### Comparing `opentaskpy-24.8.0/src/opentaskpy/config/schemas/transfer/local_destination.json` & `opentaskpy-24.9.0/src/opentaskpy/config/schemas/transfer/local_destination.json`

 * *Files identical despite different names*

### Comparing `opentaskpy-24.8.0/src/opentaskpy/config/schemas/transfer/local_source/conditionals.json` & `opentaskpy-24.9.0/src/opentaskpy/config/schemas/transfer/local_source/conditionals.json`

 * *Files identical despite different names*

### Comparing `opentaskpy-24.8.0/src/opentaskpy/config/schemas/transfer/local_source/postCopyAction.json` & `opentaskpy-24.9.0/src/opentaskpy/config/schemas/transfer/local_source/postCopyAction.json`

 * *Files identical despite different names*

### Comparing `opentaskpy-24.8.0/src/opentaskpy/config/schemas/transfer/local_source.json` & `opentaskpy-24.9.0/src/opentaskpy/config/schemas/transfer/local_source.json`

 * *Files identical despite different names*

### Comparing `opentaskpy-24.8.0/src/opentaskpy/config/schemas/transfer/sftp_destination/protocol.json` & `opentaskpy-24.9.0/src/opentaskpy/config/schemas/transfer/sftp_destination/protocol.json`

 * *Files identical despite different names*

### Comparing `opentaskpy-24.8.0/src/opentaskpy/config/schemas/transfer/sftp_destination.json` & `opentaskpy-24.9.0/src/opentaskpy/config/schemas/transfer/sftp_destination.json`

 * *Files identical despite different names*

### Comparing `opentaskpy-24.8.0/src/opentaskpy/config/schemas/transfer/sftp_source/conditionals.json` & `opentaskpy-24.9.0/src/opentaskpy/config/schemas/transfer/sftp_source/conditionals.json`

 * *Files identical despite different names*

### Comparing `opentaskpy-24.8.0/src/opentaskpy/config/schemas/transfer/sftp_source/postCopyAction.json` & `opentaskpy-24.9.0/src/opentaskpy/config/schemas/transfer/sftp_source/postCopyAction.json`

 * *Files identical despite different names*

### Comparing `opentaskpy-24.8.0/src/opentaskpy/config/schemas/transfer/sftp_source/protocol.json` & `opentaskpy-24.9.0/src/opentaskpy/config/schemas/transfer/sftp_source/protocol.json`

 * *Files identical despite different names*

### Comparing `opentaskpy-24.8.0/src/opentaskpy/config/schemas/transfer/sftp_source.json` & `opentaskpy-24.9.0/src/opentaskpy/config/schemas/transfer/sftp_source.json`

 * *Files identical despite different names*

### Comparing `opentaskpy-24.8.0/src/opentaskpy/config/schemas/transfer/ssh_destination/protocol.json` & `opentaskpy-24.9.0/src/opentaskpy/config/schemas/transfer/ssh_destination/protocol.json`

 * *Files identical despite different names*

### Comparing `opentaskpy-24.8.0/src/opentaskpy/config/schemas/transfer/ssh_destination.json` & `opentaskpy-24.9.0/src/opentaskpy/config/schemas/transfer/ssh_destination.json`

 * *Files identical despite different names*

### Comparing `opentaskpy-24.8.0/src/opentaskpy/config/schemas/transfer/ssh_source/conditionals.json` & `opentaskpy-24.9.0/src/opentaskpy/config/schemas/transfer/ssh_source/conditionals.json`

 * *Files identical despite different names*

### Comparing `opentaskpy-24.8.0/src/opentaskpy/config/schemas/transfer/ssh_source/postCopyAction.json` & `opentaskpy-24.9.0/src/opentaskpy/config/schemas/transfer/ssh_source/postCopyAction.json`

 * *Files identical despite different names*

### Comparing `opentaskpy-24.8.0/src/opentaskpy/config/schemas/transfer/ssh_source/protocol.json` & `opentaskpy-24.9.0/src/opentaskpy/config/schemas/transfer/ssh_source/protocol.json`

 * *Files identical despite different names*

### Comparing `opentaskpy-24.8.0/src/opentaskpy/config/schemas/transfer/ssh_source.json` & `opentaskpy-24.9.0/src/opentaskpy/config/schemas/transfer/ssh_source.json`

 * *Files identical despite different names*

### Comparing `opentaskpy-24.8.0/src/opentaskpy/config/schemas.py` & `opentaskpy-24.9.0/src/opentaskpy/config/schemas.py`

 * *Files identical despite different names*

### Comparing `opentaskpy-24.8.0/src/opentaskpy/exceptions.py` & `opentaskpy-24.9.0/src/opentaskpy/exceptions.py`

 * *Files identical despite different names*

### Comparing `opentaskpy-24.8.0/src/opentaskpy/otflogging.py` & `opentaskpy-24.9.0/src/opentaskpy/otflogging.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import json
 import logging
 import os
 import re
 from datetime import datetime
 
 OTF_LOG_FORMAT = (
-    "%(asctime)s — %(name)s - %(filename)s:%(lineno)s [%(threadName)s] — %(levelname)s"
+    "%(asctime)s — %(levelname)s - %(name)s - %(filename)s:%(lineno)s [%(threadName)s]"
     " — %(message)s"
 )
 LOG_DIRECTORY = (
     "logs"
     if os.environ.get("OTF_LOG_DIRECTORY") is None
     else os.environ.get("OTF_LOG_DIRECTORY")
 )
```

### Comparing `opentaskpy-24.8.0/src/opentaskpy/plugins/lookup/file.py` & `opentaskpy-24.9.0/src/opentaskpy/plugins/lookup/file.py`

 * *Files identical despite different names*

### Comparing `opentaskpy-24.8.0/src/opentaskpy/plugins/lookup/http_json.py` & `opentaskpy-24.9.0/src/opentaskpy/plugins/lookup/http_json.py`

 * *Files identical despite different names*

### Comparing `opentaskpy-24.8.0/src/opentaskpy/plugins/lookup/random_number.py` & `opentaskpy-24.9.0/src/opentaskpy/plugins/lookup/random_number.py`

 * *Files identical despite different names*

### Comparing `opentaskpy-24.8.0/src/opentaskpy/remotehandlers/email.py` & `opentaskpy-24.9.0/src/opentaskpy/remotehandlers/email.py`

 * *Files identical despite different names*

### Comparing `opentaskpy-24.8.0/src/opentaskpy/remotehandlers/local.py` & `opentaskpy-24.9.0/src/opentaskpy/remotehandlers/local.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,45 +101,29 @@
         return result
 
     def pull_files_to_worker(
         self, files: list[str], local_staging_directory: str
     ) -> int:
         """Pull files to the worker.
 
-        Moves files from a local location, to the staging directory. This will be used
-        for uploading files to the destination server.
+        This is not applicable for a local transfer, since the files are local already.
+        The files will not be transferred as they'll just fill up the worker's disk for
+        no reason.
+
+        All args are not used because this function literally does nothing.
 
         Args:
             files (list): A list of files to download.
             local_staging_directory (str): The local staging directory to move the files
             into.
 
         Returns:
-            int: 0 if successful, 1 if not.
+            int: Always returns 0
         """
-        result = 0
-
-        # Create the staging directory locally
-        if not os.path.exists(local_staging_directory):
-            os.makedirs(local_staging_directory)
-
-        # Download the files via SFTP
-        for file in files:
-            self.logger.info(
-                f"[LOCALHOST] Copying file {file} to {local_staging_directory}"
-            )
-            file_name = os.path.basename(file)
-            try:
-                # Move file on disk
-                shutil.copy2(file, f"{local_staging_directory}/{file_name}")
-            except Exception as ex:  # pylint: disable=broad-exception-caught
-                self.logger.error(f"[LOCALHOST] Failed to copy file locally: {ex}")
-                result = 1
-
-        return result
+        return 0
 
     def push_files_from_worker(self, local_staging_directory: str) -> int:
         """Push files from the worker to another local directory.
 
         Moves files from a local staging directory, to another local destination folder.
 
         Args:
@@ -196,15 +180,14 @@
                 file_name = re.sub(rename_regex, rename_sub, file_name)
                 final_destination = f"{destination_directory}/{file_name}"
 
             mode = self.spec["mode"] if "mode" in self.spec else None
 
             try:
                 shutil.copy(file, final_destination)
-                os.remove(file)
                 if mode:
                     os.chmod(final_destination, int(mode, base=8))
             except Exception as ex:  # pylint: disable=broad-exception-caught
                 self.logger.error(f"[LOCALHOST] Failed to move file: {ex}")
                 result = 1
 
         return result
```

### Comparing `opentaskpy-24.8.0/src/opentaskpy/remotehandlers/remotehandler.py` & `opentaskpy-24.9.0/src/opentaskpy/remotehandlers/remotehandler.py`

 * *Files identical despite different names*

### Comparing `opentaskpy-24.8.0/src/opentaskpy/remotehandlers/sftp.py` & `opentaskpy-24.9.0/src/opentaskpy/remotehandlers/sftp.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import os
 import re
 import stat
 from io import StringIO
 from shlex import quote
 
 from paramiko import AutoAddPolicy, Channel, RSAKey, SFTPClient, SSHClient
+from tenacity import retry, stop_after_attempt, wait_exponential
 
 import opentaskpy.otflogging
 from opentaskpy.remotehandlers.remotehandler import RemoteTransferHandler
 
 SSH_OPTIONS: str = "-o StrictHostKeyChecking=no -o BatchMode=yes -o ConnectTimeout=5"
 REMOTE_SCRIPT_BASE_DIR: str = "/tmp"  # nosec B108
 
@@ -64,15 +65,16 @@
 
         client_kwargs = {
             "hostname": hostname,
             "port": (
                 self.spec["protocol"]["port"] if "port" in self.spec["protocol"] else 22
             ),
             "username": self.spec["protocol"]["credentials"]["username"],
-            "timeout": 5,
+            "timeout": 3,
+            "allow_agent": False,
         }
 
         # If a custom key is set via env vars, then set that
         if (
             os.environ.get("OTF_SSH_KEY")
             and os.path.exists(str(os.environ.get("OTF_SSH_KEY")))
         ) and "keyFile" not in self.spec["protocol"]["credentials"]:
@@ -95,28 +97,46 @@
             )
             client_kwargs["pkey"] = key
 
         # If a password has been defined, then use that
         elif "password" in self.spec["protocol"]["credentials"]:
             client_kwargs["password"] = self.spec["protocol"]["credentials"]["password"]
 
+        self.connect_with_retry(client_kwargs)
+
+    @retry(
+        reraise=True,
+        stop=stop_after_attempt(3),
+        wait=wait_exponential(multiplier=1, min=4, max=10),
+    )
+    def connect_with_retry(self, client_kwargs: dict) -> SSHClient:
+        """Connect to the remote host with retry.
+
+        Args:
+            client_kwargs (dict): The kwargs to use for the SSH client.
+
+        Returns:
+            SSHClient: The SSH client.
+        """
         try:
             ssh_client = SSHClient()
             ssh_client.set_log_channel(
                 f"{__name__}.{os.environ.get('OTF_TASK_ID')}.paramiko.transport"
             )
             ssh_client.set_missing_host_key_policy(AutoAddPolicy())
-            self.logger.info(f"Connecting to {hostname}")
+            self.logger.info(f"Connecting to {client_kwargs['hostname']}")
             ssh_client.connect(**client_kwargs)
             self.sftp_client = ssh_client.open_sftp()
 
         except Exception as ex:
-            self.logger.error(f"Unable to connect to {hostname}: {ex}")
+            self.logger.error(f"Unable to connect to {client_kwargs['hostname']}: {ex}")
             raise ex
 
+        return ssh_client
+
     def tidy(self) -> None:
         """Tidy up the SFTP connection.
 
         Shut down the SFTP connection and remove the remote transfer script from the
         remote host.
         """
         # Close connection
```

### Comparing `opentaskpy-24.8.0/src/opentaskpy/remotehandlers/ssh.py` & `opentaskpy-24.9.0/src/opentaskpy/remotehandlers/ssh.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 import stat
 import time
 from io import StringIO
 from shlex import quote
 
 from paramiko import AutoAddPolicy, RSAKey, SFTPClient, SSHClient, Transport
 from paramiko.channel import ChannelFile, ChannelStderrFile
+from tenacity import retry, stop_after_attempt, wait_exponential
 
 import opentaskpy.otflogging
 from opentaskpy.exceptions import SSHClientError
 from opentaskpy.remotehandlers.remotehandler import (
     RemoteExecutionHandler,
     RemoteTransferHandler,
 )
@@ -84,66 +85,80 @@
             raise SSHClientError("SSH Client not initialised")
 
         if ssh_client.get_transport() and ssh_client.get_transport().is_active():  # type: ignore[union-attr]
             self.logger.debug(
                 f"[{self.spec['hostname']}] SSH connection to {hostname} already active"
             )
             return
-        try:
-            kwargs = {
-                "hostname": hostname,
-                "port": (
-                    self.spec["protocol"]["port"]
-                    if "port" in self.spec["protocol"]
-                    else 22
-                ),
-                "username": self.spec["protocol"]["credentials"]["username"],
-                "timeout": 5,
-            }
-            # If a custom key is set via env vars, then set that
-            if (
-                os.environ.get("OTF_SSH_KEY")
-                and os.path.exists(str(os.environ.get("OTF_SSH_KEY")))
-            ) and "keyFile" not in self.spec["protocol"]["credentials"]:
-                self.logger.info(
-                    "Loading custom private SSH key from OTF_SSH_KEY env var"
-                )
-                key = RSAKey.from_private_key_file(str(os.environ.get("OTF_SSH_KEY")))
-                kwargs["pkey"] = key
-
-            # If a specific key file has been defined, then use that
-            elif "keyFile" in self.spec["protocol"]["credentials"]:
-                self.logger.info("Using key file from task spec")
-                kwargs["key_filename"] = self.spec["protocol"]["credentials"]["keyFile"]
-
-            # If a private key has been defined as a string, then use that instead
-            elif "key" in self.spec["protocol"]["credentials"]:
-                self.logger.info("Using private key from task spec")
-                key = RSAKey.from_private_key(
-                    StringIO(self.spec["protocol"]["credentials"]["key"])
-                )
-                kwargs["pkey"] = key
 
-            self.logger.info(f"Connecting to {hostname}")
-            ssh_client.connect(**kwargs)
-            _, stdout, _ = ssh_client.exec_command("uname -a")  # nosec B601
-            with stdout as stdout_fh:
-                self.logger.log(
-                    11,
-                    f"[{self.spec['hostname']}] Remote uname:"
-                    f" {stdout_fh.read().decode('UTF-8')}",
-                )
+        kwargs = {
+            "hostname": hostname,
+            "port": (
+                self.spec["protocol"]["port"] if "port" in self.spec["protocol"] else 22
+            ),
+            "username": self.spec["protocol"]["credentials"]["username"],
+            "timeout": 3,
+            "allow_agent": False,
+        }
+        # If a custom key is set via env vars, then set that
+        if (
+            os.environ.get("OTF_SSH_KEY")
+            and os.path.exists(str(os.environ.get("OTF_SSH_KEY")))
+        ) and "keyFile" not in self.spec["protocol"]["credentials"]:
+            self.logger.info("Loading custom private SSH key from OTF_SSH_KEY env var")
+            key = RSAKey.from_private_key_file(str(os.environ.get("OTF_SSH_KEY")))
+            kwargs["pkey"] = key
+
+        # If a specific key file has been defined, then use that
+        elif "keyFile" in self.spec["protocol"]["credentials"]:
+            self.logger.info("Using key file from task spec")
+            kwargs["key_filename"] = self.spec["protocol"]["credentials"]["keyFile"]
+
+        # If a private key has been defined as a string, then use that instead
+        elif "key" in self.spec["protocol"]["credentials"]:
+            self.logger.info("Using private key from task spec")
+            key = RSAKey.from_private_key(
+                StringIO(self.spec["protocol"]["credentials"]["key"])
+            )
+            kwargs["pkey"] = key
+
+        self.connect_with_retry(ssh_client, kwargs)
+
+        _, stdout, _ = ssh_client.exec_command("uname -a")  # nosec B601
+        with stdout as stdout_fh:
+            self.logger.log(
+                11,
+                f"[{self.spec['hostname']}] Remote uname:"
+                f" {stdout_fh.read().decode('UTF-8')}",
+            )
+
+        sftp = ssh_client.open_sftp()
 
-            sftp = ssh_client.open_sftp()
+        if not is_remote_host:
+            self.sftp_connection = sftp
+
+    @retry(
+        reraise=True,
+        stop=stop_after_attempt(3),
+        wait=wait_exponential(multiplier=1, min=4, max=10),
+    )
+    def connect_with_retry(self, ssh_client: SSHClient, kwargs: dict) -> None:
+        """Connect to the remote host with retry.
+
+        Args:
+            ssh_client (SSHClient): The SSH client to use.
+            kwargs (dict): The keyword arguments to use to connect to the remote host.
+        """
+        try:
+            self.logger.info(f"Connecting to {kwargs['hostname']}")
+            ssh_client.connect(**kwargs)
 
-            if not is_remote_host:
-                self.sftp_connection = sftp
         except Exception as ex:
             self.logger.error(
-                f"[{self.spec['hostname']}] Unable to connect to {hostname}: {ex}"
+                f"[{self.spec['hostname']}] Unable to connect to {kwargs['hostname']}: {ex}"
             )
             raise ex
 
     def tidy(self) -> None:
         """Tidy up the SSH connection.
 
         Shut down the SSH connection and remove the remote transfer script from the
```

### Comparing `opentaskpy-24.8.0/src/opentaskpy/taskhandlers/batch.py` & `opentaskpy-24.9.0/src/opentaskpy/taskhandlers/batch.py`

 * *Files 1% similar despite different names*

```diff
@@ -465,13 +465,15 @@
     def _execute(
         self, task_handler: TaskHandler, event: threading.Event | None = None
     ) -> bool:  #
         result = False
         try:
             result = task_handler.run(kill_event=event)
         except Exception as ex:  # pylint: disable=broad-exception-caught
+            task_handler.return_result(1, str(ex), ex)
             self.logger.error(f"[{task_handler.task_id}] Failed to run task")
-            self.logger.error(ex)
+            # Log the call stack
+            self.logger.exception(ex)
             result = False
 
         self.logger.info(f"[{task_handler.task_id}] Returned {result}")
         return result
```

### Comparing `opentaskpy-24.8.0/src/opentaskpy/taskhandlers/execution.py` & `opentaskpy-24.9.0/src/opentaskpy/taskhandlers/execution.py`

 * *Files identical despite different names*

### Comparing `opentaskpy-24.8.0/src/opentaskpy/taskhandlers/taskhandler.py` & `opentaskpy-24.9.0/src/opentaskpy/taskhandlers/taskhandler.py`

 * *Files identical despite different names*

### Comparing `opentaskpy-24.8.0/src/opentaskpy/taskhandlers/transfer.py` & `opentaskpy-24.9.0/src/opentaskpy/taskhandlers/transfer.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,15 +67,15 @@
 
         # Set up the local staging directory
         # Allow for a custom staging directory to be set via environment variable
         staging_dir_name = f"OTF_STAGING_{getpid()}.{random.randint(0, 1000000)}"
         if "OTF_STAGING_DIR" in environ:
             self.local_staging_dir = f"{environ['OTF_STAGING_DIR']}/{staging_dir_name}"
         else:
-            self.local_staging_dir = f"/{DEFAULT_STAGING_DIR_BASE}/{staging_dir_name}"
+            self.local_staging_dir = f"{DEFAULT_STAGING_DIR_BASE}/{staging_dir_name}"
 
         self.logger = opentaskpy.otflogging.init_logging(
             "opentaskpy.taskhandlers.transfer", self.task_id, TASK_TYPE
         )
 
         super().__init__(global_config)
 
@@ -100,22 +100,33 @@
             self.logger.log(12, "Closing source connection")
             self.source_remote_handler.tidy()
         if self.dest_remote_handlers:
             for remote_handler in self.dest_remote_handlers:
                 self.logger.log(12, f"Closing dest connection for {remote_handler}")
                 remote_handler.tidy()
 
-        # Remove local staging directory if it exists
-        if path.exists(self.local_staging_dir):
+        # Remove local staging directory if it exists (and this isn't a local transfer)
+        if (
+            path.exists(self.local_staging_dir)
+            and self.local_staging_dir != self.source_file_spec["directory"]
+        ):
             self.logger.log(
                 12, f"Removing local staging directory {self.local_staging_dir}"
             )
             shutil.rmtree(self.local_staging_dir)
+        else:
+            self.logger.log(
+                12,
+                "Local staging directory is the same as source directory. Not removing",
+            )
 
         # Call super to do the rest
+        # Log the exception
+        if exception:
+            self.logger.exception(exception)
         return super().return_result(status, message, exception)  # type: ignore[no-any-return]
 
     def _get_default_class(self, protocol_name: str) -> type:
         class_name = DEFAULT_PROTOCOL_MAP[protocol_name].class_
         module_name = DEFAULT_PROTOCOL_MAP[protocol_name].module
 
         # Load module
@@ -291,14 +302,17 @@
 
                 # If the sleep time is longer than the time remaining, sleep for that long instead
                 if remaining_seconds < sleep_seconds:
                     actual_sleep_seconds = remaining_seconds
                 else:
                     actual_sleep_seconds = sleep_seconds
 
+                # Prevent negative sleep times
+                actual_sleep_seconds = max(actual_sleep_seconds, 0)
+
                 self.logger.info(
                     f"No files found. Sleeping for {sleep_seconds} secs."
                     f" {remaining_seconds} seconds remain"
                 )
                 time.sleep(actual_sleep_seconds)
 
             if (
@@ -462,16 +476,19 @@
                     different_protocols
                     or (
                         "transferType" in dest_file_spec
                         and dest_file_spec["transferType"] == "proxy"
                     )
                     or not self.source_remote_handler.supports_direct_transfer()
                 ):
-                    # Create local staging dir
-                    makedirs(self.local_staging_dir, exist_ok=True)
+                    # Create local staging dir (if this isn't using the local protocol)
+                    if self.source_file_spec["protocol"]["name"] != "local":
+                        makedirs(self.local_staging_dir, exist_ok=True)
+                    else:
+                        self.local_staging_dir = self.source_file_spec["directory"]
                     transfer_result = self.source_remote_handler.pull_files_to_worker(
                         remote_files, self.local_staging_dir
                     )
                     if transfer_result != 0:
                         return self.return_result(
                             1,
                             "Pull to worker from remote source errored",
```

### Comparing `opentaskpy-24.8.0/src/opentaskpy/taskrun.py` & `opentaskpy-24.9.0/src/opentaskpy/taskrun.py`

 * *Files identical despite different names*

### Comparing `opentaskpy-24.8.0/src/opentaskpy.egg-info/PKG-INFO` & `opentaskpy-24.9.0/src/opentaskpy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentaskpy
-Version: 24.8.0
+Version: 24.9.0
 Summary: A framework for automation execution of commands and transferring files between hosts
 Author-email: Adam McDonagh <adam@elitemonkey.net>
 License: GPLv3
 Project-URL: Homepage, https://github.com/adammcdonagh/open-task-framework
 Project-URL: Bug Tracker, https://github.com/adammcdonagh/open-task-framework/issues
 Project-URL: Changelog, https://github.com/adammcdonagh/open-task-framework/blob/main/CHANGELOG.md
 Keywords: automation,task,framework,scheduling,ssh,sftp,remote,execution,command
@@ -17,14 +17,15 @@
 License-File: AUTHORS
 Requires-Dist: jinja2>=3.1
 Requires-Dist: jsonpath-ng>=1.5
 Requires-Dist: jsonschema>=4.17
 Requires-Dist: paramiko>=3.0
 Requires-Dist: requests>=2.28
 Requires-Dist: referencing>=0.29.1
+Requires-Dist: tenacity>=8.2.3
 Provides-Extra: dev
 Requires-Dist: types-requests>=2.28; extra == "dev"
 Requires-Dist: types-paramiko>=3.0; extra == "dev"
 Requires-Dist: black==24.1.1; extra == "dev"
 Requires-Dist: isort; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: bumpver; extra == "dev"
```

### Comparing `opentaskpy-24.8.0/src/opentaskpy.egg-info/SOURCES.txt` & `opentaskpy-24.9.0/src/opentaskpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `opentaskpy-24.8.0/tests/test_batch_schema_validate.py` & `opentaskpy-24.9.0/tests/test_batch_schema_validate.py`

 * *Files identical despite different names*

### Comparing `opentaskpy-24.8.0/tests/test_batch_validator.py` & `opentaskpy-24.9.0/tests/test_batch_validator.py`

 * *Files identical despite different names*

### Comparing `opentaskpy-24.8.0/tests/test_config_loader.py` & `opentaskpy-24.9.0/tests/test_config_loader.py`

 * *Files identical despite different names*

### Comparing `opentaskpy-24.8.0/tests/test_docker_task_run.py` & `opentaskpy-24.9.0/tests/test_docker_task_run.py`

 * *Files identical despite different names*

### Comparing `opentaskpy-24.8.0/tests/test_email_transfer_schema_validate.py` & `opentaskpy-24.9.0/tests/test_email_transfer_schema_validate.py`

 * *Files identical despite different names*

### Comparing `opentaskpy-24.8.0/tests/test_file_helper.py` & `opentaskpy-24.9.0/tests/test_file_helper.py`

 * *Files identical despite different names*

### Comparing `opentaskpy-24.8.0/tests/test_logging.py` & `opentaskpy-24.9.0/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `opentaskpy-24.8.0/tests/test_plugin_file.py` & `opentaskpy-24.9.0/tests/test_plugin_file.py`

 * *Files identical despite different names*

### Comparing `opentaskpy-24.8.0/tests/test_plugin_http_json.py` & `opentaskpy-24.9.0/tests/test_plugin_http_json.py`

 * *Files identical despite different names*

### Comparing `opentaskpy-24.8.0/tests/test_schema_validate.py` & `opentaskpy-24.9.0/tests/test_schema_validate.py`

 * *Files identical despite different names*

### Comparing `opentaskpy-24.8.0/tests/test_ssh_dest_schema_validate.py` & `opentaskpy-24.9.0/tests/test_ssh_dest_schema_validate.py`

 * *Files identical despite different names*

### Comparing `opentaskpy-24.8.0/tests/test_ssh_execution_schema_validate.py` & `opentaskpy-24.9.0/tests/test_ssh_execution_schema_validate.py`

 * *Files identical despite different names*

### Comparing `opentaskpy-24.8.0/tests/test_ssh_source_schema_validate.py` & `opentaskpy-24.9.0/tests/test_ssh_source_schema_validate.py`

 * *Files identical despite different names*

### Comparing `opentaskpy-24.8.0/tests/test_task_run.py` & `opentaskpy-24.9.0/tests/test_task_run.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,14 +105,25 @@
     fs.create_files(
         [{f"{root_dir}/testFiles/ssh_1/src/test.txt": {"content": "test1234"}}]
     )
 
     assert run_task_run("batch-basic")["returncode"] == 0
 
 
+def test_transfer_local_binary(env_vars, root_dir):
+    # Create a test_basic_local.txt file in /tmp/src
+    fs.create_files([{"/tmp/src/test_basic_local.txt": {"content": "test1234"}}])
+    # Ensure /tmp/dest exists
+    if not os.path.exists("/tmp/dest"):
+        os.makedirs("/tmp/dest")
+
+    # Use the "binary" to trigger the job with command line arguments
+    assert run_task_run("local-basic")["returncode"] == 0
+
+
 def test_batch_execution_invalid_host(env_vars, setup_ssh_keys, root_dir):
     # Use the "binary" to trigger the job with command line arguments
 
     assert run_task_run("batch-basic-invalid-execution-host")["returncode"] == 1
 
 
 def test_binary_invalid_config_file(env_vars, setup_ssh_keys, root_dir):
```

### Comparing `opentaskpy-24.8.0/tests/test_taskhandler_batch.py` & `opentaskpy-24.9.0/tests/test_taskhandler_batch.py`

 * *Files 4% similar despite different names*

```diff
@@ -84,14 +84,60 @@
         {
             "order_id": 2,
             "task_id": "fail-command",
         },
     ],
 }
 
+parallel_batch_many_definition = {
+    "type": "batch",
+    "tasks": [
+        {
+            "order_id": 1,
+            "task_id": "sleep-5",
+        },
+        {
+            "order_id": 2,
+            "task_id": "sleep-5",
+        },
+        {
+            "order_id": 3,
+            "task_id": "sleep-5",
+        },
+        {
+            "order_id": 4,
+            "task_id": "sleep-5",
+        },
+        {
+            "order_id": 5,
+            "task_id": "sleep-5",
+        },
+        {
+            "order_id": 6,
+            "task_id": "sleep-5",
+        },
+        {
+            "order_id": 7,
+            "task_id": "sleep-5",
+        },
+        {
+            "order_id": 8,
+            "task_id": "sleep-5",
+        },
+        {
+            "order_id": 9,
+            "task_id": "sleep-5",
+        },
+        {
+            "order_id": 10,
+            "task_id": "sleep-5",
+        },
+    ],
+}
+
 dependent_batch_definition = {
     "type": "batch",
     "tasks": [
         {
             "order_id": 1,
             "task_id": "touch",
         },
@@ -415,14 +461,27 @@
 
     # Check that all exist, with the right status
     assert os.path.exists(log_file_name_batch.replace("_running", "_failed"))
     assert os.path.exists(log_file_name_touch_task.replace("_running", ""))
     assert os.path.exists(log_file_name_failed_task.replace("_running", "_failed"))
 
 
+def test_batch_parallel_many(setup_ssh_keys, env_vars, root_dir, clear_logs):
+    # Forcing a prefix makes it easy to identify log files, as well as
+    # ensuring that any rerun logic doesn't get hit
+    os.environ["OTF_LOG_RUN_PREFIX"] = f"testbatch_many_parallel_{RANDOM}"
+
+    config_loader = ConfigLoader("test/cfg")
+    batch_obj = batch.Batch(
+        None, f"parallel-many-{RANDOM}", parallel_batch_many_definition, config_loader
+    )
+    # Run and expect a true status
+    assert batch_obj.run()
+
+
 def test_batch_continue_on_failure(setup_ssh_keys, env_vars, root_dir, clear_logs):
     task_id = f"dependency-continue-on-fail-1-{RANDOM}"
     # Ensure there are no logs for this batch
     shutil.rmtree(
         f"{opentaskpy.otflogging.LOG_DIRECTORY}/{task_id}", ignore_errors=True
     )
```

### Comparing `opentaskpy-24.8.0/tests/test_taskhandler_execution_local.py` & `opentaskpy-24.9.0/tests/test_taskhandler_execution_local.py`

 * *Files identical despite different names*

### Comparing `opentaskpy-24.8.0/tests/test_taskhandler_execution_ssh.py` & `opentaskpy-24.9.0/tests/test_taskhandler_execution_ssh.py`

 * *Files identical despite different names*

### Comparing `opentaskpy-24.8.0/tests/test_taskhandler_transfer_email.py` & `opentaskpy-24.9.0/tests/test_taskhandler_transfer_email.py`

 * *Files identical despite different names*

### Comparing `opentaskpy-24.8.0/tests/test_taskhandler_transfer_local.py` & `opentaskpy-24.9.0/tests/test_taskhandler_transfer_local.py`

 * *Files identical despite different names*

### Comparing `opentaskpy-24.8.0/tests/test_taskhandler_transfer_sftp.py` & `opentaskpy-24.9.0/tests/test_taskhandler_transfer_sftp.py`

 * *Files identical despite different names*

### Comparing `opentaskpy-24.8.0/tests/test_taskhandler_transfer_ssh.py` & `opentaskpy-24.9.0/tests/test_taskhandler_transfer_ssh.py`

 * *Files identical despite different names*


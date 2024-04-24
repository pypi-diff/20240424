# Comparing `tmp/fractal_server-2.0.0a8.tar.gz` & `tmp/fractal_server-2.0.0a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fractal_server-2.0.0a8.tar", max compression
+gzip compressed data, was "fractal_server-2.0.0a9.tar", max compression
```

## Comparing `fractal_server-2.0.0a8.tar` & `fractal_server-2.0.0a9.tar`

### file list

```diff
@@ -1,165 +1,165 @@
--rw-r--r--   0        0        0     1576 2024-04-16 09:44:55.210574 fractal_server-2.0.0a8/LICENSE
--rw-r--r--   0        0        0     2466 2024-04-16 09:44:55.210574 fractal_server-2.0.0a8/README.md
--rw-r--r--   0        0        0       24 2024-04-16 09:44:55.214574 fractal_server-2.0.0a8/fractal_server/__init__.py
--rw-r--r--   0        0        0     4958 2024-04-16 09:44:55.214574 fractal_server-2.0.0a8/fractal_server/__main__.py
--rw-r--r--   0        0        0     3153 2024-04-16 09:44:55.214574 fractal_server-2.0.0a8/fractal_server/alembic.ini
--rw-r--r--   0        0        0        0 2024-04-16 09:44:55.214574 fractal_server-2.0.0a8/fractal_server/app/__init__.py
--rw-r--r--   0        0        0     4042 2024-04-16 09:44:55.214574 fractal_server-2.0.0a8/fractal_server/app/db/__init__.py
--rw-r--r--   0        0        0      183 2024-04-16 09:44:55.214574 fractal_server-2.0.0a8/fractal_server/app/models/__init__.py
--rw-r--r--   0        0        0      567 2024-04-16 09:44:55.214574 fractal_server-2.0.0a8/fractal_server/app/models/linkuserproject.py
--rw-r--r--   0        0        0     3378 2024-04-16 09:44:55.214574 fractal_server-2.0.0a8/fractal_server/app/models/security.py
--rw-r--r--   0        0        0     1090 2024-04-16 09:44:55.214574 fractal_server-2.0.0a8/fractal_server/app/models/state.py
--rw-r--r--   0        0        0      413 2024-04-16 09:44:55.214574 fractal_server-2.0.0a8/fractal_server/app/models/v1/__init__.py
--rw-r--r--   0        0        0     2017 2024-04-16 09:44:55.214574 fractal_server-2.0.0a8/fractal_server/app/models/v1/dataset.py
--rw-r--r--   0        0        0     3304 2024-04-16 09:44:55.214574 fractal_server-2.0.0a8/fractal_server/app/models/v1/job.py
--rw-r--r--   0        0        0      859 2024-04-16 09:44:55.214574 fractal_server-2.0.0a8/fractal_server/app/models/v1/project.py
--rw-r--r--   0        0        0     2782 2024-04-16 09:44:55.214574 fractal_server-2.0.0a8/fractal_server/app/models/v1/task.py
--rw-r--r--   0        0        0     3950 2024-04-16 09:44:55.214574 fractal_server-2.0.0a8/fractal_server/app/models/v1/workflow.py
--rw-r--r--   0        0        0      400 2024-04-16 09:44:55.214574 fractal_server-2.0.0a8/fractal_server/app/models/v2/__init__.py
--rw-r--r--   0        0        0     1455 2024-04-16 09:44:55.214574 fractal_server-2.0.0a8/fractal_server/app/models/v2/dataset.py
--rw-r--r--   0        0        0     1535 2024-04-16 09:44:55.214574 fractal_server-2.0.0a8/fractal_server/app/models/v2/job.py
--rw-r--r--   0        0        0      817 2024-04-16 09:44:55.214574 fractal_server-2.0.0a8/fractal_server/app/models/v2/project.py
--rw-r--r--   0        0        0     3257 2024-04-16 09:44:55.214574 fractal_server-2.0.0a8/fractal_server/app/models/v2/task.py
--rw-r--r--   0        0        0     1256 2024-04-16 09:44:55.214574 fractal_server-2.0.0a8/fractal_server/app/models/v2/workflow.py
--rw-r--r--   0        0        0     2727 2024-04-16 09:44:55.214574 fractal_server-2.0.0a8/fractal_server/app/models/v2/workflowtask.py
--rw-r--r--   0        0        0        0 2024-04-16 09:44:55.214574 fractal_server-2.0.0a8/fractal_server/app/routes/__init__.py
--rw-r--r--   0        0        0        0 2024-04-16 09:44:55.214574 fractal_server-2.0.0a8/fractal_server/app/routes/admin/__init__.py
--rw-r--r--   0        0        0    13981 2024-04-16 09:44:55.214574 fractal_server-2.0.0a8/fractal_server/app/routes/admin/v1.py
--rw-r--r--   0        0        0     9826 2024-04-16 09:44:55.214574 fractal_server-2.0.0a8/fractal_server/app/routes/admin/v2.py
--rw-r--r--   0        0        0      315 2024-04-16 09:44:55.214574 fractal_server-2.0.0a8/fractal_server/app/routes/api/__init__.py
--rw-r--r--   0        0        0      958 2024-04-16 09:44:55.214574 fractal_server-2.0.0a8/fractal_server/app/routes/api/v1/__init__.py
--rw-r--r--   0        0        0    11955 2024-04-16 09:44:55.214574 fractal_server-2.0.0a8/fractal_server/app/routes/api/v1/_aux_functions.py
--rw-r--r--   0        0        0    16911 2024-04-16 09:44:55.214574 fractal_server-2.0.0a8/fractal_server/app/routes/api/v1/dataset.py
--rw-r--r--   0        0        0     5436 2024-04-16 09:44:55.214574 fractal_server-2.0.0a8/fractal_server/app/routes/api/v1/job.py
--rw-r--r--   0        0        0    15765 2024-04-16 09:44:55.214574 fractal_server-2.0.0a8/fractal_server/app/routes/api/v1/project.py
--rw-r--r--   0        0        0     6123 2024-04-16 09:44:55.214574 fractal_server-2.0.0a8/fractal_server/app/routes/api/v1/task.py
--rw-r--r--   0        0        0     8873 2024-04-16 09:44:55.214574 fractal_server-2.0.0a8/fractal_server/app/routes/api/v1/task_collection.py
--rw-r--r--   0        0        0    10930 2024-04-16 09:44:55.214574 fractal_server-2.0.0a8/fractal_server/app/routes/api/v1/workflow.py
--rw-r--r--   0        0        0     5579 2024-04-16 09:44:55.214574 fractal_server-2.0.0a8/fractal_server/app/routes/api/v1/workflowtask.py
--rw-r--r--   0        0        0     1373 2024-04-16 09:44:55.214574 fractal_server-2.0.0a8/fractal_server/app/routes/api/v2/__init__.py
--rw-r--r--   0        0        0    14301 2024-04-16 09:44:55.214574 fractal_server-2.0.0a8/fractal_server/app/routes/api/v2/_aux_functions.py
--rw-r--r--   0        0        0    10008 2024-04-16 09:44:55.214574 fractal_server-2.0.0a8/fractal_server/app/routes/api/v2/dataset.py
--rw-r--r--   0        0        0     7589 2024-04-16 09:44:55.214574 fractal_server-2.0.0a8/fractal_server/app/routes/api/v2/images.py
--rw-r--r--   0        0        0     5334 2024-04-16 09:44:55.214574 fractal_server-2.0.0a8/fractal_server/app/routes/api/v2/job.py
--rw-r--r--   0        0        0     6024 2024-04-16 09:44:55.214574 fractal_server-2.0.0a8/fractal_server/app/routes/api/v2/project.py
--rw-r--r--   0        0        0     6901 2024-04-16 09:44:55.214574 fractal_server-2.0.0a8/fractal_server/app/routes/api/v2/submit.py
--rw-r--r--   0        0        0     7130 2024-04-16 09:44:55.214574 fractal_server-2.0.0a8/fractal_server/app/routes/api/v2/task.py
--rw-r--r--   0        0        0     8904 2024-04-16 09:44:55.214574 fractal_server-2.0.0a8/fractal_server/app/routes/api/v2/task_collection.py
--rw-r--r--   0        0        0     1628 2024-04-16 09:44:55.214574 fractal_server-2.0.0a8/fractal_server/app/routes/api/v2/task_legacy.py
--rw-r--r--   0        0        0    11845 2024-04-16 09:44:55.214574 fractal_server-2.0.0a8/fractal_server/app/routes/api/v2/workflow.py
--rw-r--r--   0        0        0     8414 2024-04-16 09:44:55.214574 fractal_server-2.0.0a8/fractal_server/app/routes/api/v2/workflowtask.py
--rw-r--r--   0        0        0     4885 2024-04-16 09:44:55.214574 fractal_server-2.0.0a8/fractal_server/app/routes/auth.py
--rw-r--r--   0        0        0        0 2024-04-16 09:44:55.214574 fractal_server-2.0.0a8/fractal_server/app/routes/aux/__init__.py
--rw-r--r--   0        0        0     1248 2024-04-16 09:44:55.214574 fractal_server-2.0.0a8/fractal_server/app/routes/aux/_job.py
--rw-r--r--   0        0        0      675 2024-04-16 09:44:55.214574 fractal_server-2.0.0a8/fractal_server/app/routes/aux/_runner.py
--rw-r--r--   0        0        0       16 2024-04-16 09:44:55.218574 fractal_server-2.0.0a8/fractal_server/app/runner/.gitignore
--rw-r--r--   0        0        0        0 2024-04-16 09:44:55.218574 fractal_server-2.0.0a8/fractal_server/app/runner/__init__.py
--rw-r--r--   0        0        0      829 2024-04-16 09:44:55.218574 fractal_server-2.0.0a8/fractal_server/app/runner/async_wrap.py
--rw-r--r--   0        0        0      119 2024-04-16 09:44:55.218574 fractal_server-2.0.0a8/fractal_server/app/runner/components.py
--rw-r--r--   0        0        0     4159 2024-04-16 09:44:55.218574 fractal_server-2.0.0a8/fractal_server/app/runner/exceptions.py
--rw-r--r--   0        0        0        0 2024-04-16 09:44:55.218574 fractal_server-2.0.0a8/fractal_server/app/runner/executors/__init__.py
--rw-r--r--   0        0        0       65 2024-04-16 09:44:55.218574 fractal_server-2.0.0a8/fractal_server/app/runner/executors/slurm/__init__.py
--rw-r--r--   0        0        0     8841 2024-04-16 09:44:55.218574 fractal_server-2.0.0a8/fractal_server/app/runner/executors/slurm/_batching.py
--rw-r--r--   0        0        0     1908 2024-04-16 09:44:55.218574 fractal_server-2.0.0a8/fractal_server/app/runner/executors/slurm/_check_jobs_status.py
--rw-r--r--   0        0        0     4421 2024-04-16 09:44:55.218574 fractal_server-2.0.0a8/fractal_server/app/runner/executors/slurm/_executor_wait_thread.py
--rw-r--r--   0        0        0    15552 2024-04-16 09:44:55.218574 fractal_server-2.0.0a8/fractal_server/app/runner/executors/slurm/_slurm_config.py
--rw-r--r--   0        0        0     5123 2024-04-16 09:44:55.218574 fractal_server-2.0.0a8/fractal_server/app/runner/executors/slurm/_subprocess_run_as_user.py
--rw-r--r--   0        0        0    44451 2024-04-16 09:44:55.218574 fractal_server-2.0.0a8/fractal_server/app/runner/executors/slurm/executor.py
--rw-r--r--   0        0        0     5852 2024-04-16 09:44:55.218574 fractal_server-2.0.0a8/fractal_server/app/runner/executors/slurm/remote.py
--rw-r--r--   0        0        0      206 2024-04-16 09:44:55.218574 fractal_server-2.0.0a8/fractal_server/app/runner/filenames.py
--rw-r--r--   0        0        0     1254 2024-04-16 09:44:55.218574 fractal_server-2.0.0a8/fractal_server/app/runner/set_start_and_last_task_index.py
--rw-r--r--   0        0        0     3219 2024-04-16 09:44:55.218574 fractal_server-2.0.0a8/fractal_server/app/runner/task_files.py
--rw-r--r--   0        0        0    13608 2024-04-16 09:44:55.218574 fractal_server-2.0.0a8/fractal_server/app/runner/v1/__init__.py
--rw-r--r--   0        0        0    21240 2024-04-16 09:44:55.218574 fractal_server-2.0.0a8/fractal_server/app/runner/v1/_common.py
--rw-r--r--   0        0        0     6926 2024-04-16 09:44:55.218574 fractal_server-2.0.0a8/fractal_server/app/runner/v1/_local/__init__.py
--rw-r--r--   0        0        0     3147 2024-04-16 09:44:55.218574 fractal_server-2.0.0a8/fractal_server/app/runner/v1/_local/_local_config.py
--rw-r--r--   0        0        0     1493 2024-04-16 09:44:55.218574 fractal_server-2.0.0a8/fractal_server/app/runner/v1/_local/_submit_setup.py
--rw-r--r--   0        0        0     3620 2024-04-16 09:44:55.218574 fractal_server-2.0.0a8/fractal_server/app/runner/v1/_local/executor.py
--rw-r--r--   0        0        0    10853 2024-04-16 09:44:55.218574 fractal_server-2.0.0a8/fractal_server/app/runner/v1/_slurm/__init__.py
--rw-r--r--   0        0        0     2738 2024-04-16 09:44:55.218574 fractal_server-2.0.0a8/fractal_server/app/runner/v1/_slurm/_submit_setup.py
--rw-r--r--   0        0        0     5977 2024-04-16 09:44:55.218574 fractal_server-2.0.0a8/fractal_server/app/runner/v1/_slurm/get_slurm_config.py
--rw-r--r--   0        0        0     3294 2024-04-16 09:44:55.218574 fractal_server-2.0.0a8/fractal_server/app/runner/v1/common.py
--rw-r--r--   0        0        0     4684 2024-04-16 09:44:55.218574 fractal_server-2.0.0a8/fractal_server/app/runner/v1/handle_failed_job.py
--rw-r--r--   0        0        0    12482 2024-04-16 09:44:55.218574 fractal_server-2.0.0a8/fractal_server/app/runner/v2/__init__.py
--rw-r--r--   0        0        0     5881 2024-04-16 09:44:55.218574 fractal_server-2.0.0a8/fractal_server/app/runner/v2/_local/__init__.py
--rw-r--r--   0        0        0     3630 2024-04-16 09:44:55.218574 fractal_server-2.0.0a8/fractal_server/app/runner/v2/_local/_local_config.py
--rw-r--r--   0        0        0     1614 2024-04-16 09:44:55.218574 fractal_server-2.0.0a8/fractal_server/app/runner/v2/_local/_submit_setup.py
--rw-r--r--   0        0        0     3620 2024-04-16 09:44:55.218574 fractal_server-2.0.0a8/fractal_server/app/runner/v2/_local/executor.py
--rw-r--r--   0        0        0     4409 2024-04-16 09:44:55.218574 fractal_server-2.0.0a8/fractal_server/app/runner/v2/_slurm/__init__.py
--rw-r--r--   0        0        0     2793 2024-04-16 09:44:55.218574 fractal_server-2.0.0a8/fractal_server/app/runner/v2/_slurm/_submit_setup.py
--rw-r--r--   0        0        0     6621 2024-04-16 09:44:55.218574 fractal_server-2.0.0a8/fractal_server/app/runner/v2/_slurm/get_slurm_config.py
--rw-r--r--   0        0        0      639 2024-04-16 09:44:55.218574 fractal_server-2.0.0a8/fractal_server/app/runner/v2/deduplicate_list.py
--rw-r--r--   0        0        0     5202 2024-04-16 09:44:55.218574 fractal_server-2.0.0a8/fractal_server/app/runner/v2/handle_failed_job.py
--rw-r--r--   0        0        0     1281 2024-04-16 09:44:55.218574 fractal_server-2.0.0a8/fractal_server/app/runner/v2/merge_outputs.py
--rw-r--r--   0        0        0    11784 2024-04-16 09:44:55.218574 fractal_server-2.0.0a8/fractal_server/app/runner/v2/runner.py
--rw-r--r--   0        0        0    10087 2024-04-16 09:44:55.218574 fractal_server-2.0.0a8/fractal_server/app/runner/v2/runner_functions.py
--rw-r--r--   0        0        0     3845 2024-04-16 09:44:55.218574 fractal_server-2.0.0a8/fractal_server/app/runner/v2/runner_functions_low_level.py
--rw-r--r--   0        0        0     1746 2024-04-16 09:44:55.218574 fractal_server-2.0.0a8/fractal_server/app/runner/v2/task_interface.py
--rw-r--r--   0        0        0      511 2024-04-16 09:44:55.218574 fractal_server-2.0.0a8/fractal_server/app/runner/v2/v1_compat.py
--rw-r--r--   0        0        0      157 2024-04-16 09:44:55.218574 fractal_server-2.0.0a8/fractal_server/app/schemas/__init__.py
--rw-r--r--   0        0        0     3461 2024-04-16 09:44:55.218574 fractal_server-2.0.0a8/fractal_server/app/schemas/_validators.py
--rw-r--r--   0        0        0      692 2024-04-16 09:44:55.218574 fractal_server-2.0.0a8/fractal_server/app/schemas/state.py
--rw-r--r--   0        0        0     3113 2024-04-16 09:44:55.218574 fractal_server-2.0.0a8/fractal_server/app/schemas/user.py
--rw-r--r--   0        0        0     2078 2024-04-16 09:44:55.218574 fractal_server-2.0.0a8/fractal_server/app/schemas/v1/__init__.py
--rw-r--r--   0        0        0     4302 2024-04-16 09:44:55.218574 fractal_server-2.0.0a8/fractal_server/app/schemas/v1/applyworkflow.py
--rw-r--r--   0        0        0     3444 2024-04-16 09:44:55.218574 fractal_server-2.0.0a8/fractal_server/app/schemas/v1/dataset.py
--rw-r--r--   0        0        0     1274 2024-04-16 09:44:55.218574 fractal_server-2.0.0a8/fractal_server/app/schemas/v1/dumps.py
--rw-r--r--   0        0        0     3829 2024-04-16 09:44:55.218574 fractal_server-2.0.0a8/fractal_server/app/schemas/v1/manifest.py
--rw-r--r--   0        0        0     1218 2024-04-16 09:44:55.218574 fractal_server-2.0.0a8/fractal_server/app/schemas/v1/project.py
--rw-r--r--   0        0        0     3704 2024-04-16 09:44:55.218574 fractal_server-2.0.0a8/fractal_server/app/schemas/v1/task.py
--rw-r--r--   0        0        0     3057 2024-04-16 09:44:55.218574 fractal_server-2.0.0a8/fractal_server/app/schemas/v1/task_collection.py
--rw-r--r--   0        0        0     4618 2024-04-16 09:44:55.218574 fractal_server-2.0.0a8/fractal_server/app/schemas/v1/workflow.py
--rw-r--r--   0        0        0     1752 2024-04-16 09:44:55.218574 fractal_server-2.0.0a8/fractal_server/app/schemas/v2/__init__.py
--rw-r--r--   0        0        0     2086 2024-04-16 09:44:55.218574 fractal_server-2.0.0a8/fractal_server/app/schemas/v2/dataset.py
--rw-r--r--   0        0        0     1997 2024-04-16 09:44:55.218574 fractal_server-2.0.0a8/fractal_server/app/schemas/v2/dumps.py
--rw-r--r--   0        0        0     3250 2024-04-16 09:44:55.218574 fractal_server-2.0.0a8/fractal_server/app/schemas/v2/job.py
--rw-r--r--   0        0        0     6243 2024-04-16 09:44:55.218574 fractal_server-2.0.0a8/fractal_server/app/schemas/v2/manifest.py
--rw-r--r--   0        0        0      736 2024-04-16 09:44:55.222575 fractal_server-2.0.0a8/fractal_server/app/schemas/v2/project.py
--rw-r--r--   0        0        0     4672 2024-04-16 09:44:55.222575 fractal_server-2.0.0a8/fractal_server/app/schemas/v2/task.py
--rw-r--r--   0        0        0     3171 2024-04-16 09:44:55.222575 fractal_server-2.0.0a8/fractal_server/app/schemas/v2/task_collection.py
--rw-r--r--   0        0        0     1827 2024-04-16 09:44:55.222575 fractal_server-2.0.0a8/fractal_server/app/schemas/v2/workflow.py
--rw-r--r--   0        0        0     5051 2024-04-16 09:44:55.222575 fractal_server-2.0.0a8/fractal_server/app/schemas/v2/workflowtask.py
--rw-r--r--   0        0        0    11203 2024-04-16 09:44:55.222575 fractal_server-2.0.0a8/fractal_server/app/security/__init__.py
--rw-r--r--   0        0        0    15080 2024-04-16 09:44:55.222575 fractal_server-2.0.0a8/fractal_server/config.py
--rw-r--r--   0        0        0      398 2024-04-16 09:44:55.222575 fractal_server-2.0.0a8/fractal_server/data_migrations/README.md
--rw-r--r--   0        0        0      196 2024-04-16 09:44:55.222575 fractal_server-2.0.0a8/fractal_server/images/__init__.py
--rw-r--r--   0        0        0     4167 2024-04-16 09:44:55.222575 fractal_server-2.0.0a8/fractal_server/images/models.py
--rw-r--r--   0        0        0     2234 2024-04-16 09:44:55.222575 fractal_server-2.0.0a8/fractal_server/images/tools.py
--rw-r--r--   0        0        0     3924 2024-04-16 09:44:55.222575 fractal_server-2.0.0a8/fractal_server/logger.py
--rw-r--r--   0        0        0     3001 2024-04-16 09:44:55.222575 fractal_server-2.0.0a8/fractal_server/main.py
--rw-r--r--   0        0        0       59 2024-04-16 09:44:55.222575 fractal_server-2.0.0a8/fractal_server/migrations/README
--rw-r--r--   0        0        0     2630 2024-04-16 09:44:55.222575 fractal_server-2.0.0a8/fractal_server/migrations/env.py
--rw-r--r--   0        0        0      526 2024-04-16 09:44:55.222575 fractal_server-2.0.0a8/fractal_server/migrations/script.py.mako
--rw-r--r--   0        0        0      954 2024-04-16 09:44:55.222575 fractal_server-2.0.0a8/fractal_server/migrations/versions/4c308bcaea2b_add_task_args_schema_and_task_args_.py
--rw-r--r--   0        0        0     1157 2024-04-16 09:44:55.222575 fractal_server-2.0.0a8/fractal_server/migrations/versions/4cedeb448a53_workflowtask_foreign_keys_not_nullables.py
--rw-r--r--   0        0        0     8770 2024-04-16 09:44:55.222575 fractal_server-2.0.0a8/fractal_server/migrations/versions/50a13d6138fd_initial_schema.py
--rw-r--r--   0        0        0     1632 2024-04-16 09:44:55.222575 fractal_server-2.0.0a8/fractal_server/migrations/versions/70e77f1c38b0_add_applyworkflow_first_task_index_and_.py
--rw-r--r--   0        0        0     1353 2024-04-16 09:44:55.222575 fractal_server-2.0.0a8/fractal_server/migrations/versions/71eefd1dd202_add_slurm_accounts.py
--rw-r--r--   0        0        0     8116 2024-04-16 09:44:55.222575 fractal_server-2.0.0a8/fractal_server/migrations/versions/80e12e1bc4fd_v2.py
--rw-r--r--   0        0        0     2684 2024-04-16 09:44:55.222575 fractal_server-2.0.0a8/fractal_server/migrations/versions/84bf0fffde30_add_dumps_to_applyworkflow.py
--rw-r--r--   0        0        0     1115 2024-04-16 09:44:55.222575 fractal_server-2.0.0a8/fractal_server/migrations/versions/8f79bd162e35_add_docs_info_and_docs_link_to_task_.py
--rw-r--r--   0        0        0     1057 2024-04-16 09:44:55.222575 fractal_server-2.0.0a8/fractal_server/migrations/versions/97f444d47249_add_applyworkflow_project_dump.py
--rw-r--r--   0        0        0      883 2024-04-16 09:44:55.222575 fractal_server-2.0.0a8/fractal_server/migrations/versions/99ea79d9e5d2_add_dataset_history.py
--rw-r--r--   0        0        0     1849 2024-04-16 09:44:55.222575 fractal_server-2.0.0a8/fractal_server/migrations/versions/9fd26a2b0de4_add_workflow_timestamp_created.py
--rw-r--r--   0        0        0      867 2024-04-16 09:44:55.222575 fractal_server-2.0.0a8/fractal_server/migrations/versions/a7f4d6137b53_add_workflow_dump_to_applyworkflow.py
--rw-r--r--   0        0        0      949 2024-04-16 09:44:55.222575 fractal_server-2.0.0a8/fractal_server/migrations/versions/d4fe3708d309_make_applyworkflow_workflow_dump_non_.py
--rw-r--r--   0        0        0      963 2024-04-16 09:44:55.222575 fractal_server-2.0.0a8/fractal_server/migrations/versions/e75cac726012_make_applyworkflow_start_timestamp_not_.py
--rw-r--r--   0        0        0     1221 2024-04-16 09:44:55.222575 fractal_server-2.0.0a8/fractal_server/migrations/versions/efa89c30e0a4_add_project_timestamp_created.py
--rw-r--r--   0        0        0      746 2024-04-16 09:44:55.222575 fractal_server-2.0.0a8/fractal_server/migrations/versions/f384e1c0cf5d_drop_task_default_args_columns.py
--rw-r--r--   0        0        0        0 2024-04-16 09:44:55.222575 fractal_server-2.0.0a8/fractal_server/py.typed
--rw-r--r--   0        0        0     2786 2024-04-16 09:44:55.222575 fractal_server-2.0.0a8/fractal_server/syringe.py
--rw-r--r--   0        0        0       23 2024-04-16 09:44:55.222575 fractal_server-2.0.0a8/fractal_server/tasks/__init__.py
--rw-r--r--   0        0        0     5379 2024-04-16 09:44:55.222575 fractal_server-2.0.0a8/fractal_server/tasks/endpoint_operations.py
--rw-r--r--   0        0        0     3278 2024-04-16 09:44:55.222575 fractal_server-2.0.0a8/fractal_server/tasks/utils.py
--rw-r--r--   0        0        0     3775 2024-04-16 09:44:55.222575 fractal_server-2.0.0a8/fractal_server/tasks/v1/_TaskCollectPip.py
--rw-r--r--   0        0        0        0 2024-04-16 09:44:55.222575 fractal_server-2.0.0a8/fractal_server/tasks/v1/__init__.py
--rw-r--r--   0        0        0    11725 2024-04-16 09:44:55.222575 fractal_server-2.0.0a8/fractal_server/tasks/v1/background_operations.py
--rw-r--r--   0        0        0      502 2024-04-16 09:44:55.222575 fractal_server-2.0.0a8/fractal_server/tasks/v1/get_collection_data.py
--rw-r--r--   0        0        0     3775 2024-04-16 09:44:55.222575 fractal_server-2.0.0a8/fractal_server/tasks/v2/_TaskCollectPip.py
--rw-r--r--   0        0        0        0 2024-04-16 09:44:55.222575 fractal_server-2.0.0a8/fractal_server/tasks/v2/__init__.py
--rw-r--r--   0        0        0    12803 2024-04-16 09:44:55.222575 fractal_server-2.0.0a8/fractal_server/tasks/v2/background_operations.py
--rw-r--r--   0        0        0      502 2024-04-16 09:44:55.222575 fractal_server-2.0.0a8/fractal_server/tasks/v2/get_collection_data.py
--rw-r--r--   0        0        0      448 2024-04-16 09:44:55.222575 fractal_server-2.0.0a8/fractal_server/urls.py
--rw-r--r--   0        0        0     2115 2024-04-16 09:44:55.222575 fractal_server-2.0.0a8/fractal_server/utils.py
--rw-r--r--   0        0        0     2999 2024-04-16 09:44:55.226575 fractal_server-2.0.0a8/pyproject.toml
--rw-r--r--   0        0        0     4204 1970-01-01 00:00:00.000000 fractal_server-2.0.0a8/PKG-INFO
+-rw-r--r--   0        0        0     1576 2024-04-17 14:14:34.354496 fractal_server-2.0.0a9/LICENSE
+-rw-r--r--   0        0        0     2466 2024-04-17 14:14:34.354496 fractal_server-2.0.0a9/README.md
+-rw-r--r--   0        0        0       24 2024-04-17 14:14:34.358496 fractal_server-2.0.0a9/fractal_server/__init__.py
+-rw-r--r--   0        0        0     4958 2024-04-17 14:14:34.358496 fractal_server-2.0.0a9/fractal_server/__main__.py
+-rw-r--r--   0        0        0     3153 2024-04-17 14:14:34.358496 fractal_server-2.0.0a9/fractal_server/alembic.ini
+-rw-r--r--   0        0        0        0 2024-04-17 14:14:34.358496 fractal_server-2.0.0a9/fractal_server/app/__init__.py
+-rw-r--r--   0        0        0     4042 2024-04-17 14:14:34.358496 fractal_server-2.0.0a9/fractal_server/app/db/__init__.py
+-rw-r--r--   0        0        0      183 2024-04-17 14:14:34.358496 fractal_server-2.0.0a9/fractal_server/app/models/__init__.py
+-rw-r--r--   0        0        0      567 2024-04-17 14:14:34.358496 fractal_server-2.0.0a9/fractal_server/app/models/linkuserproject.py
+-rw-r--r--   0        0        0     3378 2024-04-17 14:14:34.358496 fractal_server-2.0.0a9/fractal_server/app/models/security.py
+-rw-r--r--   0        0        0     1090 2024-04-17 14:14:34.358496 fractal_server-2.0.0a9/fractal_server/app/models/state.py
+-rw-r--r--   0        0        0      413 2024-04-17 14:14:34.358496 fractal_server-2.0.0a9/fractal_server/app/models/v1/__init__.py
+-rw-r--r--   0        0        0     2017 2024-04-17 14:14:34.358496 fractal_server-2.0.0a9/fractal_server/app/models/v1/dataset.py
+-rw-r--r--   0        0        0     3304 2024-04-17 14:14:34.358496 fractal_server-2.0.0a9/fractal_server/app/models/v1/job.py
+-rw-r--r--   0        0        0      859 2024-04-17 14:14:34.358496 fractal_server-2.0.0a9/fractal_server/app/models/v1/project.py
+-rw-r--r--   0        0        0     2782 2024-04-17 14:14:34.358496 fractal_server-2.0.0a9/fractal_server/app/models/v1/task.py
+-rw-r--r--   0        0        0     3950 2024-04-17 14:14:34.358496 fractal_server-2.0.0a9/fractal_server/app/models/v1/workflow.py
+-rw-r--r--   0        0        0      400 2024-04-17 14:14:34.358496 fractal_server-2.0.0a9/fractal_server/app/models/v2/__init__.py
+-rw-r--r--   0        0        0     1455 2024-04-17 14:14:34.358496 fractal_server-2.0.0a9/fractal_server/app/models/v2/dataset.py
+-rw-r--r--   0        0        0     1535 2024-04-17 14:14:34.358496 fractal_server-2.0.0a9/fractal_server/app/models/v2/job.py
+-rw-r--r--   0        0        0      817 2024-04-17 14:14:34.358496 fractal_server-2.0.0a9/fractal_server/app/models/v2/project.py
+-rw-r--r--   0        0        0     3257 2024-04-17 14:14:34.358496 fractal_server-2.0.0a9/fractal_server/app/models/v2/task.py
+-rw-r--r--   0        0        0     1069 2024-04-17 14:14:34.358496 fractal_server-2.0.0a9/fractal_server/app/models/v2/workflow.py
+-rw-r--r--   0        0        0     2695 2024-04-17 14:14:34.358496 fractal_server-2.0.0a9/fractal_server/app/models/v2/workflowtask.py
+-rw-r--r--   0        0        0        0 2024-04-17 14:14:34.358496 fractal_server-2.0.0a9/fractal_server/app/routes/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-17 14:14:34.358496 fractal_server-2.0.0a9/fractal_server/app/routes/admin/__init__.py
+-rw-r--r--   0        0        0    13981 2024-04-17 14:14:34.358496 fractal_server-2.0.0a9/fractal_server/app/routes/admin/v1.py
+-rw-r--r--   0        0        0     9826 2024-04-17 14:14:34.358496 fractal_server-2.0.0a9/fractal_server/app/routes/admin/v2.py
+-rw-r--r--   0        0        0      315 2024-04-17 14:14:34.358496 fractal_server-2.0.0a9/fractal_server/app/routes/api/__init__.py
+-rw-r--r--   0        0        0      958 2024-04-17 14:14:34.358496 fractal_server-2.0.0a9/fractal_server/app/routes/api/v1/__init__.py
+-rw-r--r--   0        0        0    11955 2024-04-17 14:14:34.358496 fractal_server-2.0.0a9/fractal_server/app/routes/api/v1/_aux_functions.py
+-rw-r--r--   0        0        0    16911 2024-04-17 14:14:34.358496 fractal_server-2.0.0a9/fractal_server/app/routes/api/v1/dataset.py
+-rw-r--r--   0        0        0     5436 2024-04-17 14:14:34.358496 fractal_server-2.0.0a9/fractal_server/app/routes/api/v1/job.py
+-rw-r--r--   0        0        0    15765 2024-04-17 14:14:34.358496 fractal_server-2.0.0a9/fractal_server/app/routes/api/v1/project.py
+-rw-r--r--   0        0        0     6123 2024-04-17 14:14:34.358496 fractal_server-2.0.0a9/fractal_server/app/routes/api/v1/task.py
+-rw-r--r--   0        0        0     8873 2024-04-17 14:14:34.358496 fractal_server-2.0.0a9/fractal_server/app/routes/api/v1/task_collection.py
+-rw-r--r--   0        0        0    10930 2024-04-17 14:14:34.358496 fractal_server-2.0.0a9/fractal_server/app/routes/api/v1/workflow.py
+-rw-r--r--   0        0        0     5579 2024-04-17 14:14:34.358496 fractal_server-2.0.0a9/fractal_server/app/routes/api/v1/workflowtask.py
+-rw-r--r--   0        0        0     1373 2024-04-17 14:14:34.358496 fractal_server-2.0.0a9/fractal_server/app/routes/api/v2/__init__.py
+-rw-r--r--   0        0        0    14301 2024-04-17 14:14:34.358496 fractal_server-2.0.0a9/fractal_server/app/routes/api/v2/_aux_functions.py
+-rw-r--r--   0        0        0    11573 2024-04-17 14:14:34.358496 fractal_server-2.0.0a9/fractal_server/app/routes/api/v2/dataset.py
+-rw-r--r--   0        0        0     7894 2024-04-17 14:14:34.358496 fractal_server-2.0.0a9/fractal_server/app/routes/api/v2/images.py
+-rw-r--r--   0        0        0     5334 2024-04-17 14:14:34.358496 fractal_server-2.0.0a9/fractal_server/app/routes/api/v2/job.py
+-rw-r--r--   0        0        0     6024 2024-04-17 14:14:34.358496 fractal_server-2.0.0a9/fractal_server/app/routes/api/v2/project.py
+-rw-r--r--   0        0        0     6901 2024-04-17 14:14:34.358496 fractal_server-2.0.0a9/fractal_server/app/routes/api/v2/submit.py
+-rw-r--r--   0        0        0     7130 2024-04-17 14:14:34.358496 fractal_server-2.0.0a9/fractal_server/app/routes/api/v2/task.py
+-rw-r--r--   0        0        0     8904 2024-04-17 14:14:34.358496 fractal_server-2.0.0a9/fractal_server/app/routes/api/v2/task_collection.py
+-rw-r--r--   0        0        0     1628 2024-04-17 14:14:34.358496 fractal_server-2.0.0a9/fractal_server/app/routes/api/v2/task_legacy.py
+-rw-r--r--   0        0        0    11845 2024-04-17 14:14:34.358496 fractal_server-2.0.0a9/fractal_server/app/routes/api/v2/workflow.py
+-rw-r--r--   0        0        0     8720 2024-04-17 14:14:34.358496 fractal_server-2.0.0a9/fractal_server/app/routes/api/v2/workflowtask.py
+-rw-r--r--   0        0        0     4885 2024-04-17 14:14:34.358496 fractal_server-2.0.0a9/fractal_server/app/routes/auth.py
+-rw-r--r--   0        0        0        0 2024-04-17 14:14:34.358496 fractal_server-2.0.0a9/fractal_server/app/routes/aux/__init__.py
+-rw-r--r--   0        0        0     1248 2024-04-17 14:14:34.358496 fractal_server-2.0.0a9/fractal_server/app/routes/aux/_job.py
+-rw-r--r--   0        0        0      675 2024-04-17 14:14:34.358496 fractal_server-2.0.0a9/fractal_server/app/routes/aux/_runner.py
+-rw-r--r--   0        0        0       16 2024-04-17 14:14:34.358496 fractal_server-2.0.0a9/fractal_server/app/runner/.gitignore
+-rw-r--r--   0        0        0        0 2024-04-17 14:14:34.358496 fractal_server-2.0.0a9/fractal_server/app/runner/__init__.py
+-rw-r--r--   0        0        0      829 2024-04-17 14:14:34.358496 fractal_server-2.0.0a9/fractal_server/app/runner/async_wrap.py
+-rw-r--r--   0        0        0      119 2024-04-17 14:14:34.358496 fractal_server-2.0.0a9/fractal_server/app/runner/components.py
+-rw-r--r--   0        0        0     4159 2024-04-17 14:14:34.358496 fractal_server-2.0.0a9/fractal_server/app/runner/exceptions.py
+-rw-r--r--   0        0        0        0 2024-04-17 14:14:34.358496 fractal_server-2.0.0a9/fractal_server/app/runner/executors/__init__.py
+-rw-r--r--   0        0        0       65 2024-04-17 14:14:34.358496 fractal_server-2.0.0a9/fractal_server/app/runner/executors/slurm/__init__.py
+-rw-r--r--   0        0        0     8841 2024-04-17 14:14:34.358496 fractal_server-2.0.0a9/fractal_server/app/runner/executors/slurm/_batching.py
+-rw-r--r--   0        0        0     1908 2024-04-17 14:14:34.358496 fractal_server-2.0.0a9/fractal_server/app/runner/executors/slurm/_check_jobs_status.py
+-rw-r--r--   0        0        0     4421 2024-04-17 14:14:34.362496 fractal_server-2.0.0a9/fractal_server/app/runner/executors/slurm/_executor_wait_thread.py
+-rw-r--r--   0        0        0    15552 2024-04-17 14:14:34.362496 fractal_server-2.0.0a9/fractal_server/app/runner/executors/slurm/_slurm_config.py
+-rw-r--r--   0        0        0     5123 2024-04-17 14:14:34.362496 fractal_server-2.0.0a9/fractal_server/app/runner/executors/slurm/_subprocess_run_as_user.py
+-rw-r--r--   0        0        0    44451 2024-04-17 14:14:34.362496 fractal_server-2.0.0a9/fractal_server/app/runner/executors/slurm/executor.py
+-rw-r--r--   0        0        0     5852 2024-04-17 14:14:34.362496 fractal_server-2.0.0a9/fractal_server/app/runner/executors/slurm/remote.py
+-rw-r--r--   0        0        0      206 2024-04-17 14:14:34.362496 fractal_server-2.0.0a9/fractal_server/app/runner/filenames.py
+-rw-r--r--   0        0        0     1254 2024-04-17 14:14:34.362496 fractal_server-2.0.0a9/fractal_server/app/runner/set_start_and_last_task_index.py
+-rw-r--r--   0        0        0     3219 2024-04-17 14:14:34.362496 fractal_server-2.0.0a9/fractal_server/app/runner/task_files.py
+-rw-r--r--   0        0        0    13608 2024-04-17 14:14:34.362496 fractal_server-2.0.0a9/fractal_server/app/runner/v1/__init__.py
+-rw-r--r--   0        0        0    21240 2024-04-17 14:14:34.362496 fractal_server-2.0.0a9/fractal_server/app/runner/v1/_common.py
+-rw-r--r--   0        0        0     6926 2024-04-17 14:14:34.362496 fractal_server-2.0.0a9/fractal_server/app/runner/v1/_local/__init__.py
+-rw-r--r--   0        0        0     3147 2024-04-17 14:14:34.362496 fractal_server-2.0.0a9/fractal_server/app/runner/v1/_local/_local_config.py
+-rw-r--r--   0        0        0     1493 2024-04-17 14:14:34.362496 fractal_server-2.0.0a9/fractal_server/app/runner/v1/_local/_submit_setup.py
+-rw-r--r--   0        0        0     3620 2024-04-17 14:14:34.362496 fractal_server-2.0.0a9/fractal_server/app/runner/v1/_local/executor.py
+-rw-r--r--   0        0        0    10853 2024-04-17 14:14:34.362496 fractal_server-2.0.0a9/fractal_server/app/runner/v1/_slurm/__init__.py
+-rw-r--r--   0        0        0     2738 2024-04-17 14:14:34.362496 fractal_server-2.0.0a9/fractal_server/app/runner/v1/_slurm/_submit_setup.py
+-rw-r--r--   0        0        0     5977 2024-04-17 14:14:34.362496 fractal_server-2.0.0a9/fractal_server/app/runner/v1/_slurm/get_slurm_config.py
+-rw-r--r--   0        0        0     3294 2024-04-17 14:14:34.362496 fractal_server-2.0.0a9/fractal_server/app/runner/v1/common.py
+-rw-r--r--   0        0        0     4684 2024-04-17 14:14:34.362496 fractal_server-2.0.0a9/fractal_server/app/runner/v1/handle_failed_job.py
+-rw-r--r--   0        0        0    12482 2024-04-17 14:14:34.362496 fractal_server-2.0.0a9/fractal_server/app/runner/v2/__init__.py
+-rw-r--r--   0        0        0     5881 2024-04-17 14:14:34.362496 fractal_server-2.0.0a9/fractal_server/app/runner/v2/_local/__init__.py
+-rw-r--r--   0        0        0     3630 2024-04-17 14:14:34.362496 fractal_server-2.0.0a9/fractal_server/app/runner/v2/_local/_local_config.py
+-rw-r--r--   0        0        0     1614 2024-04-17 14:14:34.362496 fractal_server-2.0.0a9/fractal_server/app/runner/v2/_local/_submit_setup.py
+-rw-r--r--   0        0        0     3620 2024-04-17 14:14:34.362496 fractal_server-2.0.0a9/fractal_server/app/runner/v2/_local/executor.py
+-rw-r--r--   0        0        0     4409 2024-04-17 14:14:34.362496 fractal_server-2.0.0a9/fractal_server/app/runner/v2/_slurm/__init__.py
+-rw-r--r--   0        0        0     2793 2024-04-17 14:14:34.362496 fractal_server-2.0.0a9/fractal_server/app/runner/v2/_slurm/_submit_setup.py
+-rw-r--r--   0        0        0     6726 2024-04-17 14:14:34.362496 fractal_server-2.0.0a9/fractal_server/app/runner/v2/_slurm/get_slurm_config.py
+-rw-r--r--   0        0        0      639 2024-04-17 14:14:34.362496 fractal_server-2.0.0a9/fractal_server/app/runner/v2/deduplicate_list.py
+-rw-r--r--   0        0        0     5415 2024-04-17 14:14:34.362496 fractal_server-2.0.0a9/fractal_server/app/runner/v2/handle_failed_job.py
+-rw-r--r--   0        0        0     1281 2024-04-17 14:14:34.362496 fractal_server-2.0.0a9/fractal_server/app/runner/v2/merge_outputs.py
+-rw-r--r--   0        0        0    12599 2024-04-17 14:14:34.362496 fractal_server-2.0.0a9/fractal_server/app/runner/v2/runner.py
+-rw-r--r--   0        0        0    10171 2024-04-17 14:14:34.362496 fractal_server-2.0.0a9/fractal_server/app/runner/v2/runner_functions.py
+-rw-r--r--   0        0        0     3947 2024-04-17 14:14:34.362496 fractal_server-2.0.0a9/fractal_server/app/runner/v2/runner_functions_low_level.py
+-rw-r--r--   0        0        0     1746 2024-04-17 14:14:34.362496 fractal_server-2.0.0a9/fractal_server/app/runner/v2/task_interface.py
+-rw-r--r--   0        0        0      912 2024-04-17 14:14:34.362496 fractal_server-2.0.0a9/fractal_server/app/runner/v2/v1_compat.py
+-rw-r--r--   0        0        0      157 2024-04-17 14:14:34.362496 fractal_server-2.0.0a9/fractal_server/app/schemas/__init__.py
+-rw-r--r--   0        0        0     3461 2024-04-17 14:14:34.362496 fractal_server-2.0.0a9/fractal_server/app/schemas/_validators.py
+-rw-r--r--   0        0        0      692 2024-04-17 14:14:34.362496 fractal_server-2.0.0a9/fractal_server/app/schemas/state.py
+-rw-r--r--   0        0        0     3113 2024-04-17 14:14:34.362496 fractal_server-2.0.0a9/fractal_server/app/schemas/user.py
+-rw-r--r--   0        0        0     2078 2024-04-17 14:14:34.362496 fractal_server-2.0.0a9/fractal_server/app/schemas/v1/__init__.py
+-rw-r--r--   0        0        0     4302 2024-04-17 14:14:34.362496 fractal_server-2.0.0a9/fractal_server/app/schemas/v1/applyworkflow.py
+-rw-r--r--   0        0        0     3444 2024-04-17 14:14:34.362496 fractal_server-2.0.0a9/fractal_server/app/schemas/v1/dataset.py
+-rw-r--r--   0        0        0     1274 2024-04-17 14:14:34.362496 fractal_server-2.0.0a9/fractal_server/app/schemas/v1/dumps.py
+-rw-r--r--   0        0        0     3829 2024-04-17 14:14:34.362496 fractal_server-2.0.0a9/fractal_server/app/schemas/v1/manifest.py
+-rw-r--r--   0        0        0     1218 2024-04-17 14:14:34.362496 fractal_server-2.0.0a9/fractal_server/app/schemas/v1/project.py
+-rw-r--r--   0        0        0     3704 2024-04-17 14:14:34.362496 fractal_server-2.0.0a9/fractal_server/app/schemas/v1/task.py
+-rw-r--r--   0        0        0     3057 2024-04-17 14:14:34.362496 fractal_server-2.0.0a9/fractal_server/app/schemas/v1/task_collection.py
+-rw-r--r--   0        0        0     4618 2024-04-17 14:14:34.362496 fractal_server-2.0.0a9/fractal_server/app/schemas/v1/workflow.py
+-rw-r--r--   0        0        0     1752 2024-04-17 14:14:34.362496 fractal_server-2.0.0a9/fractal_server/app/schemas/v2/__init__.py
+-rw-r--r--   0        0        0     2737 2024-04-17 14:14:34.362496 fractal_server-2.0.0a9/fractal_server/app/schemas/v2/dataset.py
+-rw-r--r--   0        0        0     2023 2024-04-17 14:14:34.362496 fractal_server-2.0.0a9/fractal_server/app/schemas/v2/dumps.py
+-rw-r--r--   0        0        0     3250 2024-04-17 14:14:34.362496 fractal_server-2.0.0a9/fractal_server/app/schemas/v2/job.py
+-rw-r--r--   0        0        0     6243 2024-04-17 14:14:34.362496 fractal_server-2.0.0a9/fractal_server/app/schemas/v2/manifest.py
+-rw-r--r--   0        0        0      736 2024-04-17 14:14:34.362496 fractal_server-2.0.0a9/fractal_server/app/schemas/v2/project.py
+-rw-r--r--   0        0        0     4672 2024-04-17 14:14:34.362496 fractal_server-2.0.0a9/fractal_server/app/schemas/v2/task.py
+-rw-r--r--   0        0        0     3171 2024-04-17 14:14:34.362496 fractal_server-2.0.0a9/fractal_server/app/schemas/v2/task_collection.py
+-rw-r--r--   0        0        0     1827 2024-04-17 14:14:34.362496 fractal_server-2.0.0a9/fractal_server/app/schemas/v2/workflow.py
+-rw-r--r--   0        0        0     5051 2024-04-17 14:14:34.362496 fractal_server-2.0.0a9/fractal_server/app/schemas/v2/workflowtask.py
+-rw-r--r--   0        0        0    11203 2024-04-17 14:14:34.362496 fractal_server-2.0.0a9/fractal_server/app/security/__init__.py
+-rw-r--r--   0        0        0    15080 2024-04-17 14:14:34.362496 fractal_server-2.0.0a9/fractal_server/config.py
+-rw-r--r--   0        0        0      398 2024-04-17 14:14:34.362496 fractal_server-2.0.0a9/fractal_server/data_migrations/README.md
+-rw-r--r--   0        0        0      196 2024-04-17 14:14:34.362496 fractal_server-2.0.0a9/fractal_server/images/__init__.py
+-rw-r--r--   0        0        0     4167 2024-04-17 14:14:34.362496 fractal_server-2.0.0a9/fractal_server/images/models.py
+-rw-r--r--   0        0        0     2234 2024-04-17 14:14:34.362496 fractal_server-2.0.0a9/fractal_server/images/tools.py
+-rw-r--r--   0        0        0     3924 2024-04-17 14:14:34.366496 fractal_server-2.0.0a9/fractal_server/logger.py
+-rw-r--r--   0        0        0     3001 2024-04-17 14:14:34.366496 fractal_server-2.0.0a9/fractal_server/main.py
+-rw-r--r--   0        0        0       59 2024-04-17 14:14:34.366496 fractal_server-2.0.0a9/fractal_server/migrations/README
+-rw-r--r--   0        0        0     2630 2024-04-17 14:14:34.366496 fractal_server-2.0.0a9/fractal_server/migrations/env.py
+-rw-r--r--   0        0        0      526 2024-04-17 14:14:34.366496 fractal_server-2.0.0a9/fractal_server/migrations/script.py.mako
+-rw-r--r--   0        0        0      954 2024-04-17 14:14:34.366496 fractal_server-2.0.0a9/fractal_server/migrations/versions/4c308bcaea2b_add_task_args_schema_and_task_args_.py
+-rw-r--r--   0        0        0     1157 2024-04-17 14:14:34.366496 fractal_server-2.0.0a9/fractal_server/migrations/versions/4cedeb448a53_workflowtask_foreign_keys_not_nullables.py
+-rw-r--r--   0        0        0     8770 2024-04-17 14:14:34.366496 fractal_server-2.0.0a9/fractal_server/migrations/versions/50a13d6138fd_initial_schema.py
+-rw-r--r--   0        0        0     1632 2024-04-17 14:14:34.366496 fractal_server-2.0.0a9/fractal_server/migrations/versions/70e77f1c38b0_add_applyworkflow_first_task_index_and_.py
+-rw-r--r--   0        0        0     1353 2024-04-17 14:14:34.366496 fractal_server-2.0.0a9/fractal_server/migrations/versions/71eefd1dd202_add_slurm_accounts.py
+-rw-r--r--   0        0        0     8116 2024-04-17 14:14:34.366496 fractal_server-2.0.0a9/fractal_server/migrations/versions/80e12e1bc4fd_v2.py
+-rw-r--r--   0        0        0     2684 2024-04-17 14:14:34.366496 fractal_server-2.0.0a9/fractal_server/migrations/versions/84bf0fffde30_add_dumps_to_applyworkflow.py
+-rw-r--r--   0        0        0     1115 2024-04-17 14:14:34.366496 fractal_server-2.0.0a9/fractal_server/migrations/versions/8f79bd162e35_add_docs_info_and_docs_link_to_task_.py
+-rw-r--r--   0        0        0     1057 2024-04-17 14:14:34.366496 fractal_server-2.0.0a9/fractal_server/migrations/versions/97f444d47249_add_applyworkflow_project_dump.py
+-rw-r--r--   0        0        0      883 2024-04-17 14:14:34.366496 fractal_server-2.0.0a9/fractal_server/migrations/versions/99ea79d9e5d2_add_dataset_history.py
+-rw-r--r--   0        0        0     1849 2024-04-17 14:14:34.366496 fractal_server-2.0.0a9/fractal_server/migrations/versions/9fd26a2b0de4_add_workflow_timestamp_created.py
+-rw-r--r--   0        0        0      867 2024-04-17 14:14:34.366496 fractal_server-2.0.0a9/fractal_server/migrations/versions/a7f4d6137b53_add_workflow_dump_to_applyworkflow.py
+-rw-r--r--   0        0        0      949 2024-04-17 14:14:34.366496 fractal_server-2.0.0a9/fractal_server/migrations/versions/d4fe3708d309_make_applyworkflow_workflow_dump_non_.py
+-rw-r--r--   0        0        0      963 2024-04-17 14:14:34.366496 fractal_server-2.0.0a9/fractal_server/migrations/versions/e75cac726012_make_applyworkflow_start_timestamp_not_.py
+-rw-r--r--   0        0        0     1221 2024-04-17 14:14:34.366496 fractal_server-2.0.0a9/fractal_server/migrations/versions/efa89c30e0a4_add_project_timestamp_created.py
+-rw-r--r--   0        0        0      746 2024-04-17 14:14:34.366496 fractal_server-2.0.0a9/fractal_server/migrations/versions/f384e1c0cf5d_drop_task_default_args_columns.py
+-rw-r--r--   0        0        0        0 2024-04-17 14:14:34.366496 fractal_server-2.0.0a9/fractal_server/py.typed
+-rw-r--r--   0        0        0     2786 2024-04-17 14:14:34.366496 fractal_server-2.0.0a9/fractal_server/syringe.py
+-rw-r--r--   0        0        0       23 2024-04-17 14:14:34.366496 fractal_server-2.0.0a9/fractal_server/tasks/__init__.py
+-rw-r--r--   0        0        0     5379 2024-04-17 14:14:34.366496 fractal_server-2.0.0a9/fractal_server/tasks/endpoint_operations.py
+-rw-r--r--   0        0        0     3278 2024-04-17 14:14:34.366496 fractal_server-2.0.0a9/fractal_server/tasks/utils.py
+-rw-r--r--   0        0        0     3775 2024-04-17 14:14:34.366496 fractal_server-2.0.0a9/fractal_server/tasks/v1/_TaskCollectPip.py
+-rw-r--r--   0        0        0        0 2024-04-17 14:14:34.366496 fractal_server-2.0.0a9/fractal_server/tasks/v1/__init__.py
+-rw-r--r--   0        0        0    11725 2024-04-17 14:14:34.366496 fractal_server-2.0.0a9/fractal_server/tasks/v1/background_operations.py
+-rw-r--r--   0        0        0      502 2024-04-17 14:14:34.366496 fractal_server-2.0.0a9/fractal_server/tasks/v1/get_collection_data.py
+-rw-r--r--   0        0        0     3775 2024-04-17 14:14:34.366496 fractal_server-2.0.0a9/fractal_server/tasks/v2/_TaskCollectPip.py
+-rw-r--r--   0        0        0        0 2024-04-17 14:14:34.366496 fractal_server-2.0.0a9/fractal_server/tasks/v2/__init__.py
+-rw-r--r--   0        0        0    12803 2024-04-17 14:14:34.366496 fractal_server-2.0.0a9/fractal_server/tasks/v2/background_operations.py
+-rw-r--r--   0        0        0      502 2024-04-17 14:14:34.366496 fractal_server-2.0.0a9/fractal_server/tasks/v2/get_collection_data.py
+-rw-r--r--   0        0        0      448 2024-04-17 14:14:34.366496 fractal_server-2.0.0a9/fractal_server/urls.py
+-rw-r--r--   0        0        0     2115 2024-04-17 14:14:34.366496 fractal_server-2.0.0a9/fractal_server/utils.py
+-rw-r--r--   0        0        0     3004 2024-04-17 14:14:34.366496 fractal_server-2.0.0a9/pyproject.toml
+-rw-r--r--   0        0        0     4200 1970-01-01 00:00:00.000000 fractal_server-2.0.0a9/PKG-INFO
```

### Comparing `fractal_server-2.0.0a8/LICENSE` & `fractal_server-2.0.0a9/LICENSE`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a8/README.md` & `fractal_server-2.0.0a9/README.md`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a8/fractal_server/__main__.py` & `fractal_server-2.0.0a9/fractal_server/__main__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a8/fractal_server/alembic.ini` & `fractal_server-2.0.0a9/fractal_server/alembic.ini`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a8/fractal_server/app/db/__init__.py` & `fractal_server-2.0.0a9/fractal_server/app/db/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a8/fractal_server/app/models/linkuserproject.py` & `fractal_server-2.0.0a9/fractal_server/app/models/linkuserproject.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a8/fractal_server/app/models/security.py` & `fractal_server-2.0.0a9/fractal_server/app/models/security.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a8/fractal_server/app/models/state.py` & `fractal_server-2.0.0a9/fractal_server/app/models/state.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a8/fractal_server/app/models/v1/dataset.py` & `fractal_server-2.0.0a9/fractal_server/app/models/v1/dataset.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a8/fractal_server/app/models/v1/job.py` & `fractal_server-2.0.0a9/fractal_server/app/models/v1/job.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a8/fractal_server/app/models/v1/project.py` & `fractal_server-2.0.0a9/fractal_server/app/models/v1/project.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a8/fractal_server/app/models/v1/task.py` & `fractal_server-2.0.0a9/fractal_server/app/models/v1/task.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a8/fractal_server/app/models/v1/workflow.py` & `fractal_server-2.0.0a9/fractal_server/app/models/v1/workflow.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a8/fractal_server/app/models/v2/dataset.py` & `fractal_server-2.0.0a9/fractal_server/app/models/v2/dataset.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a8/fractal_server/app/models/v2/job.py` & `fractal_server-2.0.0a9/fractal_server/app/models/v2/job.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a8/fractal_server/app/models/v2/project.py` & `fractal_server-2.0.0a9/fractal_server/app/models/v2/project.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a8/fractal_server/app/models/v2/task.py` & `fractal_server-2.0.0a9/fractal_server/app/models/v2/task.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a8/fractal_server/app/models/v2/workflow.py` & `fractal_server-2.0.0a9/fractal_server/app/models/v2/workflow.py`

 * *Files 12% similar despite different names*

```diff
@@ -29,15 +29,7 @@
             cascade="all, delete-orphan",
         ),
     )
     timestamp_created: datetime = Field(
         default_factory=get_timestamp,
         sa_column=Column(DateTime(timezone=True), nullable=False),
     )
-
-    @property
-    def input_types(self):
-        return self.task_list[0].task.input_types
-
-    @property
-    def output_types(self):
-        return self.task_list[-1].task.output_types
```

### Comparing `fractal_server-2.0.0a8/fractal_server/app/models/v2/workflowtask.py` & `fractal_server-2.0.0a9/fractal_server/app/models/v2/workflowtask.py`

 * *Files 13% similar despite different names*

```diff
@@ -47,42 +47,40 @@
     task_legacy_id: Optional[int] = Field(foreign_key="task.id")
     task_legacy: Optional[Task] = Relationship(
         sa_relationship_kwargs=dict(lazy="selectin")
     )
 
     @validator("args_non_parallel")
     def validate_args_non_parallel(cls, value):
-        """
-        FIXME V2 this requires an update
-        """
         if value is None:
             return
         forbidden_args_keys = {
-            "metadata",
-            "component",
+            "zarr_dir",
+            "zarr_url",
+            "zarr_urls",
+            "init_args",
         }
         args_keys = set(value.keys())
         intersect_keys = forbidden_args_keys.intersection(args_keys)
         if intersect_keys:
             raise ValueError(
                 "`args` contains the following forbidden keys: "
                 f"{intersect_keys}"
             )
         return value
 
     @validator("args_parallel")
     def validate_args_parallel(cls, value):
-        """
-        FIXME V2 this requires an update
-        """
         if value is None:
             return
         forbidden_args_keys = {
-            "metadata",
-            "component",
+            "zarr_dir",
+            "zarr_url",
+            "zarr_urls",
+            "init_args",
         }
         args_keys = set(value.keys())
         intersect_keys = forbidden_args_keys.intersection(args_keys)
         if intersect_keys:
             raise ValueError(
                 "`args` contains the following forbidden keys: "
                 f"{intersect_keys}"
```

### Comparing `fractal_server-2.0.0a8/fractal_server/app/routes/admin/v1.py` & `fractal_server-2.0.0a9/fractal_server/app/routes/admin/v1.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a8/fractal_server/app/routes/admin/v2.py` & `fractal_server-2.0.0a9/fractal_server/app/routes/admin/v2.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a8/fractal_server/app/routes/api/v1/__init__.py` & `fractal_server-2.0.0a9/fractal_server/app/routes/api/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a8/fractal_server/app/routes/api/v1/_aux_functions.py` & `fractal_server-2.0.0a9/fractal_server/app/routes/api/v1/_aux_functions.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a8/fractal_server/app/routes/api/v1/dataset.py` & `fractal_server-2.0.0a9/fractal_server/app/routes/api/v1/dataset.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a8/fractal_server/app/routes/api/v1/job.py` & `fractal_server-2.0.0a9/fractal_server/app/routes/api/v1/job.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a8/fractal_server/app/routes/api/v1/project.py` & `fractal_server-2.0.0a9/fractal_server/app/routes/api/v1/project.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a8/fractal_server/app/routes/api/v1/task.py` & `fractal_server-2.0.0a9/fractal_server/app/routes/api/v1/task.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a8/fractal_server/app/routes/api/v1/task_collection.py` & `fractal_server-2.0.0a9/fractal_server/app/routes/api/v1/task_collection.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a8/fractal_server/app/routes/api/v1/workflow.py` & `fractal_server-2.0.0a9/fractal_server/app/routes/api/v1/workflow.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a8/fractal_server/app/routes/api/v1/workflowtask.py` & `fractal_server-2.0.0a9/fractal_server/app/routes/api/v1/workflowtask.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a8/fractal_server/app/routes/api/v2/__init__.py` & `fractal_server-2.0.0a9/fractal_server/app/routes/api/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a8/fractal_server/app/routes/api/v2/_aux_functions.py` & `fractal_server-2.0.0a9/fractal_server/app/routes/api/v2/_aux_functions.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a8/fractal_server/app/routes/api/v2/dataset.py` & `fractal_server-2.0.0a9/fractal_server/app/routes/api/v2/dataset.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,14 +13,16 @@
 from ....db import get_async_db
 from ....models.v2 import DatasetV2
 from ....models.v2 import JobV2
 from ....models.v2 import ProjectV2
 from ....schemas.v2 import DatasetCreateV2
 from ....schemas.v2 import DatasetReadV2
 from ....schemas.v2 import DatasetUpdateV2
+from ....schemas.v2.dataset import DatasetExportV2
+from ....schemas.v2.dataset import DatasetImportV2
 from ....schemas.v2.dataset import DatasetStatusReadV2
 from ....schemas.v2.dataset import WorkflowTaskStatusTypeV2
 from ....security import current_active_user
 from ....security import User
 from ._aux_functions import _get_dataset_check_owner
 from ._aux_functions import _get_project_check_owner
 from ._aux_functions import _get_submitted_jobs_statement
@@ -311,7 +313,71 @@
         for history_item in history:
             wftask_id = history_item["workflowtask"]["id"]
             wftask_status = history_item["status"]
             workflow_tasks_status_dict[wftask_id] = wftask_status
 
     response_body = DatasetStatusReadV2(status=workflow_tasks_status_dict)
     return response_body
+
+
+# /api/v2/project/{project_id}/dataset/{dataset_id}/export/
+
+
+@router.get(
+    "/project/{project_id}/dataset/{dataset_id}/export/",
+    response_model=DatasetExportV2,
+)
+async def export_dataset(
+    project_id: int,
+    dataset_id: int,
+    user: User = Depends(current_active_user),
+    db: AsyncSession = Depends(get_async_db),
+) -> Optional[DatasetExportV2]:
+    """
+    Export an existing dataset
+    """
+    dict_dataset_project = await _get_dataset_check_owner(
+        project_id=project_id,
+        dataset_id=dataset_id,
+        user_id=user.id,
+        db=db,
+    )
+    await db.close()
+
+    dataset = dict_dataset_project["dataset"]
+
+    return dataset
+
+
+@router.post(
+    "/project/{project_id}/dataset/import/",
+    response_model=DatasetReadV2,
+    status_code=status.HTTP_201_CREATED,
+)
+async def import_dataset(
+    project_id: int,
+    dataset: DatasetImportV2,
+    user: User = Depends(current_active_user),
+    db: AsyncSession = Depends(get_async_db),
+) -> Optional[DatasetReadV2]:
+    """
+    Import an existing dataset into a project
+    """
+
+    # Preliminary checks
+    await _get_project_check_owner(
+        project_id=project_id,
+        user_id=user.id,
+        db=db,
+    )
+
+    # Create new Dataset
+    db_dataset = DatasetV2(
+        project_id=project_id,
+        **dataset.dict(exclude_none=True),
+    )
+    db.add(db_dataset)
+    await db.commit()
+    await db.refresh(db_dataset)
+    await db.close()
+
+    return db_dataset
```

### Comparing `fractal_server-2.0.0a8/fractal_server/app/routes/api/v2/images.py` & `fractal_server-2.0.0a9/fractal_server/app/routes/api/v2/images.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,14 +62,22 @@
         raise HTTPException(
             status_code=status.HTTP_422_UNPROCESSABLE_ENTITY,
             detail=(
                 "Cannot create image with zarr_url which is not relative to "
                 f"{dataset.zarr_dir}."
             ),
         )
+    elif new_image.zarr_url == dataset.zarr_dir:
+        raise HTTPException(
+            status_code=status.HTTP_422_UNPROCESSABLE_ENTITY,
+            detail=(
+                "`SingleImage.zarr_url` cannot be equal to `Dataset.zarr_dir`:"
+                f" {dataset.zarr_dir}"
+            ),
+        )
 
     if new_image.zarr_url in dataset.image_zarr_urls:
         raise HTTPException(
             status_code=status.HTTP_422_UNPROCESSABLE_ENTITY,
             detail=(
                 f"Image with zarr_url '{new_image.zarr_url}' "
                 f"already in DatasetV2 {dataset_id}",
```

### Comparing `fractal_server-2.0.0a8/fractal_server/app/routes/api/v2/job.py` & `fractal_server-2.0.0a9/fractal_server/app/routes/api/v2/job.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a8/fractal_server/app/routes/api/v2/project.py` & `fractal_server-2.0.0a9/fractal_server/app/routes/api/v2/project.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a8/fractal_server/app/routes/api/v2/submit.py` & `fractal_server-2.0.0a9/fractal_server/app/routes/api/v2/submit.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a8/fractal_server/app/routes/api/v2/task.py` & `fractal_server-2.0.0a9/fractal_server/app/routes/api/v2/task.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a8/fractal_server/app/routes/api/v2/task_collection.py` & `fractal_server-2.0.0a9/fractal_server/app/routes/api/v2/task_collection.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a8/fractal_server/app/routes/api/v2/task_legacy.py` & `fractal_server-2.0.0a9/fractal_server/app/routes/api/v2/task_legacy.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a8/fractal_server/app/routes/api/v2/workflow.py` & `fractal_server-2.0.0a9/fractal_server/app/routes/api/v2/workflow.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a8/fractal_server/app/routes/api/v2/workflowtask.py` & `fractal_server-2.0.0a9/fractal_server/app/routes/api/v2/workflowtask.py`

 * *Files 4% similar despite different names*

```diff
@@ -196,17 +196,23 @@
                 for k, v in value.items():
                     actual_args[k] = v
             if not actual_args:
                 actual_args = None
             setattr(db_wf_task, key, actual_args)
         elif key == "args_non_parallel":
             # Get default arguments via a Task property method
-            default_args = deepcopy(
-                db_wf_task.task.default_args_non_parallel_from_args_schema
-            )
+            if db_wf_task.is_legacy_task:
+                # This is only needed so that we don't have to modify the rest
+                # of this block, but legacy task cannot take any non-parallel
+                # args (see checks above).
+                default_args = {}
+            else:
+                default_args = deepcopy(
+                    db_wf_task.task.default_args_non_parallel_from_args_schema
+                )
             # Override default_args with args value items
             actual_args = default_args.copy()
             if value is not None:
                 for k, v in value.items():
                     actual_args[k] = v
             if not actual_args:
                 actual_args = None
```

### Comparing `fractal_server-2.0.0a8/fractal_server/app/routes/auth.py` & `fractal_server-2.0.0a9/fractal_server/app/routes/auth.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a8/fractal_server/app/routes/aux/_job.py` & `fractal_server-2.0.0a9/fractal_server/app/routes/aux/_job.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a8/fractal_server/app/routes/aux/_runner.py` & `fractal_server-2.0.0a9/fractal_server/app/routes/aux/_runner.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a8/fractal_server/app/runner/async_wrap.py` & `fractal_server-2.0.0a9/fractal_server/app/runner/async_wrap.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a8/fractal_server/app/runner/exceptions.py` & `fractal_server-2.0.0a9/fractal_server/app/runner/exceptions.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a8/fractal_server/app/runner/executors/slurm/_batching.py` & `fractal_server-2.0.0a9/fractal_server/app/runner/executors/slurm/_batching.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a8/fractal_server/app/runner/executors/slurm/_check_jobs_status.py` & `fractal_server-2.0.0a9/fractal_server/app/runner/executors/slurm/_check_jobs_status.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a8/fractal_server/app/runner/executors/slurm/_executor_wait_thread.py` & `fractal_server-2.0.0a9/fractal_server/app/runner/executors/slurm/_executor_wait_thread.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a8/fractal_server/app/runner/executors/slurm/_slurm_config.py` & `fractal_server-2.0.0a9/fractal_server/app/runner/executors/slurm/_slurm_config.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a8/fractal_server/app/runner/executors/slurm/_subprocess_run_as_user.py` & `fractal_server-2.0.0a9/fractal_server/app/runner/executors/slurm/_subprocess_run_as_user.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a8/fractal_server/app/runner/executors/slurm/executor.py` & `fractal_server-2.0.0a9/fractal_server/app/runner/executors/slurm/executor.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a8/fractal_server/app/runner/executors/slurm/remote.py` & `fractal_server-2.0.0a9/fractal_server/app/runner/executors/slurm/remote.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a8/fractal_server/app/runner/set_start_and_last_task_index.py` & `fractal_server-2.0.0a9/fractal_server/app/runner/set_start_and_last_task_index.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a8/fractal_server/app/runner/task_files.py` & `fractal_server-2.0.0a9/fractal_server/app/runner/task_files.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a8/fractal_server/app/runner/v1/__init__.py` & `fractal_server-2.0.0a9/fractal_server/app/runner/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a8/fractal_server/app/runner/v1/_common.py` & `fractal_server-2.0.0a9/fractal_server/app/runner/v1/_common.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a8/fractal_server/app/runner/v1/_local/__init__.py` & `fractal_server-2.0.0a9/fractal_server/app/runner/v1/_local/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a8/fractal_server/app/runner/v1/_local/_local_config.py` & `fractal_server-2.0.0a9/fractal_server/app/runner/v1/_local/_local_config.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a8/fractal_server/app/runner/v1/_local/_submit_setup.py` & `fractal_server-2.0.0a9/fractal_server/app/runner/v1/_local/_submit_setup.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a8/fractal_server/app/runner/v1/_local/executor.py` & `fractal_server-2.0.0a9/fractal_server/app/runner/v1/_local/executor.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a8/fractal_server/app/runner/v1/_slurm/__init__.py` & `fractal_server-2.0.0a9/fractal_server/app/runner/v1/_slurm/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a8/fractal_server/app/runner/v1/_slurm/_submit_setup.py` & `fractal_server-2.0.0a9/fractal_server/app/runner/v1/_slurm/_submit_setup.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a8/fractal_server/app/runner/v1/_slurm/get_slurm_config.py` & `fractal_server-2.0.0a9/fractal_server/app/runner/v1/_slurm/get_slurm_config.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a8/fractal_server/app/runner/v1/common.py` & `fractal_server-2.0.0a9/fractal_server/app/runner/v1/common.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a8/fractal_server/app/runner/v1/handle_failed_job.py` & `fractal_server-2.0.0a9/fractal_server/app/runner/v1/handle_failed_job.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a8/fractal_server/app/runner/v2/__init__.py` & `fractal_server-2.0.0a9/fractal_server/app/runner/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a8/fractal_server/app/runner/v2/_local/__init__.py` & `fractal_server-2.0.0a9/fractal_server/app/runner/v2/_local/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a8/fractal_server/app/runner/v2/_local/_local_config.py` & `fractal_server-2.0.0a9/fractal_server/app/runner/v2/_local/_local_config.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a8/fractal_server/app/runner/v2/_local/_submit_setup.py` & `fractal_server-2.0.0a9/fractal_server/app/runner/v2/_local/_submit_setup.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a8/fractal_server/app/runner/v2/_local/executor.py` & `fractal_server-2.0.0a9/fractal_server/app/runner/v2/_local/executor.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a8/fractal_server/app/runner/v2/_slurm/__init__.py` & `fractal_server-2.0.0a9/fractal_server/app/runner/v2/_slurm/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a8/fractal_server/app/runner/v2/_slurm/_submit_setup.py` & `fractal_server-2.0.0a9/fractal_server/app/runner/v2/_slurm/_submit_setup.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a8/fractal_server/app/runner/v2/_slurm/get_slurm_config.py` & `fractal_server-2.0.0a9/fractal_server/app/runner/v2/_slurm/get_slurm_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -121,15 +121,18 @@
     # Required memory per task, in MB
     if wftask_meta is not None and "mem" in wftask_meta:
         raw_mem = wftask_meta["mem"]
         mem_per_task_MB = _parse_mem_value(raw_mem)
         slurm_dict["mem_per_task_MB"] = mem_per_task_MB
 
     # Job name
-    job_name = wftask.task.name.replace(" ", "_")
+    if wftask.is_legacy_task:
+        job_name = wftask.task_legacy.name.replace(" ", "_")
+    else:
+        job_name = wftask.task.name.replace(" ", "_")
     slurm_dict["job_name"] = job_name
 
     # Optional SLURM arguments and extra lines
     if wftask_meta is not None:
         account = wftask_meta.get("account", None)
         if account is not None:
             error_msg = (
```

### Comparing `fractal_server-2.0.0a8/fractal_server/app/runner/v2/deduplicate_list.py` & `fractal_server-2.0.0a9/fractal_server/app/runner/v2/deduplicate_list.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a8/fractal_server/app/runner/v2/handle_failed_job.py` & `fractal_server-2.0.0a9/fractal_server/app/runner/v2/handle_failed_job.py`

 * *Files 4% similar despite different names*

```diff
@@ -92,16 +92,23 @@
             )
             logger.error("Failed task not appended to history.")
         else:
             failed_wftask = job_wftasks[len(tmp_file_wftasks)]
 
     # Part 3/B: Append failed task to history
     if failed_wftask is not None:
-        failed_wftask_dump = failed_wftask.model_dump(exclude={"task"})
-        failed_wftask_dump["task"] = failed_wftask.task.model_dump()
+        failed_wftask_dump = failed_wftask.model_dump(
+            exclude={"task", "task_legacy"}
+        )
+        if failed_wftask.is_legacy_task:
+            failed_wftask_dump[
+                "task_legacy"
+            ] = failed_wftask.task_legacy.model_dump()
+        else:
+            failed_wftask_dump["task"] = failed_wftask.task.model_dump()
         new_history_item = dict(
             workflowtask=failed_wftask_dump,
             status=WorkflowTaskStatusTypeV2.FAILED,
             parallelization=dict(),  # FIXME: re-include parallelization
         )
         new_history.append(new_history_item)
```

### Comparing `fractal_server-2.0.0a8/fractal_server/app/runner/v2/merge_outputs.py` & `fractal_server-2.0.0a9/fractal_server/app/runner/v2/merge_outputs.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a8/fractal_server/app/runner/v2/runner.py` & `fractal_server-2.0.0a9/fractal_server/app/runner/v2/runner.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import json
+import logging
 from concurrent.futures import ThreadPoolExecutor
 from copy import copy
 from copy import deepcopy
 from pathlib import Path
 from typing import Callable
 from typing import Optional
 
@@ -33,25 +34,30 @@
     executor: ThreadPoolExecutor,
     workflow_dir: Path,
     workflow_dir_user: Optional[Path] = None,
     logger_name: Optional[str] = None,
     submit_setup_call: Callable = no_op_submit_setup_call,
 ) -> DatasetV2:
 
+    logger = logging.getLogger(logger_name)
+
     if not workflow_dir.exists():  # FIXME: this should have already happened
         workflow_dir.mkdir()
 
     # Initialize local dataset attributes
     zarr_dir = dataset.zarr_dir
     tmp_images = deepcopy(dataset.images)
     tmp_filters = deepcopy(dataset.filters)
     tmp_history = []
 
     for wftask in wf_task_list:
         task = wftask.task
+        task_legacy = wftask.task_legacy
+        task_name = task_legacy.name if wftask.is_legacy_task else task.name
+        logger.debug(f'SUBMIT {wftask.order}-th task (name="{task_name}")')
 
         # PRE TASK EXECUTION
 
         # Get filtered images
         pre_filters = dict(
             types=copy(tmp_filters["types"]),
             attributes=copy(tmp_filters["attributes"]),
@@ -59,68 +65,71 @@
         pre_filters["types"].update(wftask.input_filters["types"])
         pre_filters["attributes"].update(wftask.input_filters["attributes"])
         filtered_images = filter_image_list(
             images=tmp_images,
             filters=Filters(**pre_filters),
         )
         # Verify that filtered images comply with task input_types
-        for image in filtered_images:
-            if not match_filter(image, Filters(types=task.input_types)):
-                raise ValueError(
-                    f"Filtered images include {image}, which does "
-                    f"not comply with {task.input_types=}."
-                )
+        if not wftask.is_legacy_task:
+            for image in filtered_images:
+                if not match_filter(image, Filters(types=task.input_types)):
+                    raise ValueError(
+                        f"Filtered images include {image}, which does "
+                        f"not comply with {task.input_types=}."
+                    )
 
         # TASK EXECUTION (V2)
         if not wftask.is_legacy_task:
             if task.type == "non_parallel":
                 current_task_output = run_v2_task_non_parallel(
                     images=filtered_images,
                     zarr_dir=zarr_dir,
                     wftask=wftask,
-                    task=wftask.task,
+                    task=task,
                     workflow_dir=workflow_dir,
                     workflow_dir_user=workflow_dir_user,
                     executor=executor,
                     logger_name=logger_name,
                     submit_setup_call=submit_setup_call,
                 )
             elif task.type == "parallel":
                 current_task_output = run_v2_task_parallel(
                     images=filtered_images,
                     wftask=wftask,
-                    task=wftask.task,
+                    task=task,
                     workflow_dir=workflow_dir,
                     workflow_dir_user=workflow_dir_user,
                     executor=executor,
                     logger_name=logger_name,
                     submit_setup_call=submit_setup_call,
                 )
             elif task.type == "compound":
                 current_task_output = run_v2_task_compound(
                     images=filtered_images,
                     zarr_dir=zarr_dir,
                     wftask=wftask,
-                    task=wftask.task,
+                    task=task,
                     workflow_dir=workflow_dir,
                     workflow_dir_user=workflow_dir_user,
                     executor=executor,
                     logger_name=logger_name,
                     submit_setup_call=submit_setup_call,
                 )
             else:
                 raise ValueError(f"Invalid {task.type=}.")
         # TASK EXECUTION (V1)
         else:
             current_task_output = run_v1_task_parallel(
                 images=filtered_images,
                 wftask=wftask,
-                task_legacy=wftask.task_legacy,
+                task_legacy=task_legacy,
                 executor=executor,
                 logger_name=logger_name,
+                workflow_dir=workflow_dir,
+                workflow_dir_user=workflow_dir_user,
                 submit_setup_call=submit_setup_call,
             )
 
         # POST TASK EXECUTION
 
         # Update image list
         current_task_output.check_zarr_urls_are_unique()
@@ -151,15 +160,16 @@
                 original_index = img_search["index"]
                 updated_attributes = copy(original_img["attributes"])
                 updated_types = copy(original_img["types"])
 
                 # Update image attributes/types with task output and manifest
                 updated_attributes.update(image["attributes"])
                 updated_types.update(image["types"])
-                updated_types.update(task.output_types)
+                if not wftask.is_legacy_task:
+                    updated_types.update(task.output_types)
 
                 # Unset attributes with None value
                 updated_attributes = {
                     key: value
                     for key, value in updated_attributes.items()
                     if value is not None
                 }
@@ -178,14 +188,19 @@
             else:
                 # Check that image['zarr_url'] is relative to zarr_dir
                 if not image["zarr_url"].startswith(zarr_dir):
                     raise ValueError(
                         f"{zarr_dir} is not a parent directory of "
                         f"{image['zarr_url']}"
                     )
+                # Check that image['zarr_url'] is not equal to zarr_dir
+                if image["zarr_url"] == zarr_dir:
+                    raise ValueError(
+                        "image['zarr_url'] cannot be equal to zarr_dir"
+                    )
                 # Propagate attributes and types from `origin` (if any)
                 updated_attributes = {}
                 updated_types = {}
                 if image["origin"] is not None:
                     img_search = find_image_by_zarr_url(
                         images=tmp_images,
                         zarr_url=image["origin"],
@@ -198,15 +213,16 @@
                 updated_attributes.update(image["attributes"])
                 updated_attributes = {
                     key: value
                     for key, value in updated_attributes.items()
                     if value is not None
                 }
                 updated_types.update(image["types"])
-                updated_types.update(task.output_types)
+                if not wftask.is_legacy_task:
+                    updated_types.update(task.output_types)
                 new_image = dict(
                     zarr_url=image["zarr_url"],
                     origin=image["origin"],
                     attributes=updated_attributes,
                     types=updated_types,
                 )
                 # Validate new image
@@ -273,14 +289,16 @@
         with open(workflow_dir / HISTORY_FILENAME, "w") as f:
             json.dump(tmp_history, f, indent=2)
         with open(workflow_dir / FILTERS_FILENAME, "w") as f:
             json.dump(tmp_filters, f, indent=2)
         with open(workflow_dir / IMAGES_FILENAME, "w") as f:
             json.dump(tmp_images, f, indent=2)
 
+        logger.debug(f'END    {wftask.order}-th task (name="{task_name}")')
+
     # NOTE: tmp_history only contains the newly-added history items (to be
     # appended to the original history), while tmp_filters and tmp_images
     # represent the new attributes (to replace the original ones)
     result = dict(
         history=tmp_history,
         filters=tmp_filters,
         images=tmp_images,
```

### Comparing `fractal_server-2.0.0a8/fractal_server/app/runner/v2/runner_functions.py` & `fractal_server-2.0.0a9/fractal_server/app/runner/v2/runner_functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -309,18 +309,19 @@
         which_type="parallel",
     )
 
     list_function_kwargs = []
     for ind, image in enumerate(images):
         list_function_kwargs.append(
             convert_v2_args_into_v1(
-                dict(
+                kwargs_v2=dict(
                     zarr_url=image["zarr_url"],
                     **(wftask.args_parallel or {}),
-                )
+                ),
+                parallelization_level=task_legacy.parallelization_level,
             ),
         )
         list_function_kwargs[-1][_COMPONENT_KEY_] = _index_to_component(ind)
 
     results_iterator = executor.map(
         functools.partial(
             run_single_task,
```

### Comparing `fractal_server-2.0.0a8/fractal_server/app/runner/v2/runner_functions_low_level.py` & `fractal_server-2.0.0a9/fractal_server/app/runner/v2/runner_functions_low_level.py`

 * *Files 2% similar despite different names*

```diff
@@ -112,15 +112,18 @@
         _call_command_wrapper(
             full_command,
             log_path=task_files.log,
         )
     except TaskExecutionError as e:
         e.workflow_task_order = wftask.order
         e.workflow_task_id = wftask.id
-        e.task_name = wftask.task.name
+        if wftask.is_legacy_task:
+            e.task_name = wftask.task_legacy.name
+        else:
+            e.task_name = wftask.task.name
         raise e
 
     try:
         with task_files.metadiff.open("r") as f:
             out_meta = json.load(f)
     except FileNotFoundError as e:
         logger.debug(
```

### Comparing `fractal_server-2.0.0a8/fractal_server/app/runner/v2/task_interface.py` & `fractal_server-2.0.0a9/fractal_server/app/runner/v2/task_interface.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a8/fractal_server/app/schemas/_validators.py` & `fractal_server-2.0.0a9/fractal_server/app/schemas/_validators.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a8/fractal_server/app/schemas/state.py` & `fractal_server-2.0.0a9/fractal_server/app/schemas/state.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a8/fractal_server/app/schemas/user.py` & `fractal_server-2.0.0a9/fractal_server/app/schemas/user.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a8/fractal_server/app/schemas/v1/__init__.py` & `fractal_server-2.0.0a9/fractal_server/app/schemas/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a8/fractal_server/app/schemas/v1/applyworkflow.py` & `fractal_server-2.0.0a9/fractal_server/app/schemas/v1/applyworkflow.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a8/fractal_server/app/schemas/v1/dataset.py` & `fractal_server-2.0.0a9/fractal_server/app/schemas/v1/dataset.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a8/fractal_server/app/schemas/v1/dumps.py` & `fractal_server-2.0.0a9/fractal_server/app/schemas/v1/dumps.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a8/fractal_server/app/schemas/v1/manifest.py` & `fractal_server-2.0.0a9/fractal_server/app/schemas/v1/manifest.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a8/fractal_server/app/schemas/v1/project.py` & `fractal_server-2.0.0a9/fractal_server/app/schemas/v1/project.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a8/fractal_server/app/schemas/v1/task.py` & `fractal_server-2.0.0a9/fractal_server/app/schemas/v1/task.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a8/fractal_server/app/schemas/v1/task_collection.py` & `fractal_server-2.0.0a9/fractal_server/app/schemas/v1/task_collection.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a8/fractal_server/app/schemas/v1/workflow.py` & `fractal_server-2.0.0a9/fractal_server/app/schemas/v1/workflow.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a8/fractal_server/app/schemas/v2/__init__.py` & `fractal_server-2.0.0a9/fractal_server/app/schemas/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a8/fractal_server/app/schemas/v2/dataset.py` & `fractal_server-2.0.0a9/fractal_server/app/schemas/v2/dataset.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 from .._validators import valstr
 from .._validators import valutc
 from .dumps import WorkflowTaskDumpV2
 from .project import ProjectReadV2
 from .workflowtask import WorkflowTaskStatusTypeV2
 from fractal_server.images import Filters
+from fractal_server.images import SingleImage
 from fractal_server.urls import normalize_url
 
 
 class _DatasetHistoryItemV2(BaseModel):
     """
     Class for an item of `Dataset.history`.
     """
@@ -91,7 +92,44 @@
     @validator("zarr_dir")
     def normalize_zarr_dir(cls, v: Optional[str]) -> Optional[str]:
         if v is not None:
             return normalize_url(v)
         return v
 
     _name = validator("name", allow_reuse=True)(valstr("name"))
+
+
+class DatasetImportV2(BaseModel):
+    """
+    Class for `Dataset` import.
+
+    Attributes:
+        name:
+        zarr_dir:
+        images:
+        filters:
+    """
+
+    class Config:
+        extra = "forbid"
+
+    name: str
+    zarr_dir: str
+    images: list[SingleImage] = Field(default_factory=[])
+    filters: Filters = Field(default_factory=Filters)
+
+
+class DatasetExportV2(BaseModel):
+    """
+    Class for `Dataset` export.
+
+    Attributes:
+        name:
+        zarr_dir:
+        images:
+        filters:
+    """
+
+    name: str
+    zarr_dir: str
+    images: list[SingleImage]
+    filters: Filters
```

### Comparing `fractal_server-2.0.0a8/fractal_server/app/schemas/v2/dumps.py` & `fractal_server-2.0.0a9/fractal_server/app/schemas/v2/dumps.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,14 +41,16 @@
 
 
 class WorkflowTaskDumpV2(BaseModel):
     id: int
     workflow_id: int
     order: Optional[int]
 
+    is_legacy_task: bool
+
     input_filters: Filters
 
     task_id: Optional[int]
     task: Optional[TaskDumpV2]
     task_legacy_id: Optional[int]
     task_legacy: Optional[TaskDumpV1]
```

### Comparing `fractal_server-2.0.0a8/fractal_server/app/schemas/v2/job.py` & `fractal_server-2.0.0a9/fractal_server/app/schemas/v2/job.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a8/fractal_server/app/schemas/v2/manifest.py` & `fractal_server-2.0.0a9/fractal_server/app/schemas/v2/manifest.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a8/fractal_server/app/schemas/v2/project.py` & `fractal_server-2.0.0a9/fractal_server/app/schemas/v2/project.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a8/fractal_server/app/schemas/v2/task.py` & `fractal_server-2.0.0a9/fractal_server/app/schemas/v2/task.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a8/fractal_server/app/schemas/v2/task_collection.py` & `fractal_server-2.0.0a9/fractal_server/app/schemas/v2/task_collection.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a8/fractal_server/app/schemas/v2/workflow.py` & `fractal_server-2.0.0a9/fractal_server/app/schemas/v2/workflow.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a8/fractal_server/app/schemas/v2/workflowtask.py` & `fractal_server-2.0.0a9/fractal_server/app/schemas/v2/workflowtask.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a8/fractal_server/app/security/__init__.py` & `fractal_server-2.0.0a9/fractal_server/app/security/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a8/fractal_server/config.py` & `fractal_server-2.0.0a9/fractal_server/config.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a8/fractal_server/images/models.py` & `fractal_server-2.0.0a9/fractal_server/images/models.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a8/fractal_server/images/tools.py` & `fractal_server-2.0.0a9/fractal_server/images/tools.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a8/fractal_server/logger.py` & `fractal_server-2.0.0a9/fractal_server/logger.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a8/fractal_server/main.py` & `fractal_server-2.0.0a9/fractal_server/main.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a8/fractal_server/migrations/env.py` & `fractal_server-2.0.0a9/fractal_server/migrations/env.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a8/fractal_server/migrations/script.py.mako` & `fractal_server-2.0.0a9/fractal_server/migrations/script.py.mako`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a8/fractal_server/migrations/versions/4c308bcaea2b_add_task_args_schema_and_task_args_.py` & `fractal_server-2.0.0a9/fractal_server/migrations/versions/4c308bcaea2b_add_task_args_schema_and_task_args_.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a8/fractal_server/migrations/versions/4cedeb448a53_workflowtask_foreign_keys_not_nullables.py` & `fractal_server-2.0.0a9/fractal_server/migrations/versions/4cedeb448a53_workflowtask_foreign_keys_not_nullables.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a8/fractal_server/migrations/versions/50a13d6138fd_initial_schema.py` & `fractal_server-2.0.0a9/fractal_server/migrations/versions/50a13d6138fd_initial_schema.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a8/fractal_server/migrations/versions/70e77f1c38b0_add_applyworkflow_first_task_index_and_.py` & `fractal_server-2.0.0a9/fractal_server/migrations/versions/70e77f1c38b0_add_applyworkflow_first_task_index_and_.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a8/fractal_server/migrations/versions/71eefd1dd202_add_slurm_accounts.py` & `fractal_server-2.0.0a9/fractal_server/migrations/versions/71eefd1dd202_add_slurm_accounts.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a8/fractal_server/migrations/versions/80e12e1bc4fd_v2.py` & `fractal_server-2.0.0a9/fractal_server/migrations/versions/80e12e1bc4fd_v2.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a8/fractal_server/migrations/versions/84bf0fffde30_add_dumps_to_applyworkflow.py` & `fractal_server-2.0.0a9/fractal_server/migrations/versions/84bf0fffde30_add_dumps_to_applyworkflow.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a8/fractal_server/migrations/versions/8f79bd162e35_add_docs_info_and_docs_link_to_task_.py` & `fractal_server-2.0.0a9/fractal_server/migrations/versions/8f79bd162e35_add_docs_info_and_docs_link_to_task_.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a8/fractal_server/migrations/versions/97f444d47249_add_applyworkflow_project_dump.py` & `fractal_server-2.0.0a9/fractal_server/migrations/versions/97f444d47249_add_applyworkflow_project_dump.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a8/fractal_server/migrations/versions/99ea79d9e5d2_add_dataset_history.py` & `fractal_server-2.0.0a9/fractal_server/migrations/versions/99ea79d9e5d2_add_dataset_history.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a8/fractal_server/migrations/versions/9fd26a2b0de4_add_workflow_timestamp_created.py` & `fractal_server-2.0.0a9/fractal_server/migrations/versions/9fd26a2b0de4_add_workflow_timestamp_created.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a8/fractal_server/migrations/versions/a7f4d6137b53_add_workflow_dump_to_applyworkflow.py` & `fractal_server-2.0.0a9/fractal_server/migrations/versions/a7f4d6137b53_add_workflow_dump_to_applyworkflow.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a8/fractal_server/migrations/versions/d4fe3708d309_make_applyworkflow_workflow_dump_non_.py` & `fractal_server-2.0.0a9/fractal_server/migrations/versions/d4fe3708d309_make_applyworkflow_workflow_dump_non_.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a8/fractal_server/migrations/versions/e75cac726012_make_applyworkflow_start_timestamp_not_.py` & `fractal_server-2.0.0a9/fractal_server/migrations/versions/e75cac726012_make_applyworkflow_start_timestamp_not_.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a8/fractal_server/migrations/versions/efa89c30e0a4_add_project_timestamp_created.py` & `fractal_server-2.0.0a9/fractal_server/migrations/versions/efa89c30e0a4_add_project_timestamp_created.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a8/fractal_server/migrations/versions/f384e1c0cf5d_drop_task_default_args_columns.py` & `fractal_server-2.0.0a9/fractal_server/migrations/versions/f384e1c0cf5d_drop_task_default_args_columns.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a8/fractal_server/syringe.py` & `fractal_server-2.0.0a9/fractal_server/syringe.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a8/fractal_server/tasks/endpoint_operations.py` & `fractal_server-2.0.0a9/fractal_server/tasks/endpoint_operations.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a8/fractal_server/tasks/utils.py` & `fractal_server-2.0.0a9/fractal_server/tasks/utils.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a8/fractal_server/tasks/v1/_TaskCollectPip.py` & `fractal_server-2.0.0a9/fractal_server/tasks/v1/_TaskCollectPip.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a8/fractal_server/tasks/v1/background_operations.py` & `fractal_server-2.0.0a9/fractal_server/tasks/v1/background_operations.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a8/fractal_server/tasks/v2/_TaskCollectPip.py` & `fractal_server-2.0.0a9/fractal_server/tasks/v2/_TaskCollectPip.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a8/fractal_server/tasks/v2/background_operations.py` & `fractal_server-2.0.0a9/fractal_server/tasks/v2/background_operations.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a8/fractal_server/utils.py` & `fractal_server-2.0.0a9/fractal_server/utils.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a8/pyproject.toml` & `fractal_server-2.0.0a9/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fractal-server"
-version = "2.0.0a8"
+version = "2.0.0a9"
 description = "Server component of the Fractal analytics platform"
 authors = [
     "Jacopo Nespolo <jacopo.nespolo@exact-lab.it>",
     "Marco Franzon <marco.franzon@exact-lab.it>",
     "Tommaso Comparin <tommaso.comparin@exact-lab.it>",
 ]
 readme = "README.md"
@@ -36,15 +36,15 @@
 bcrypt = "4.0.1"
 packaging = "^23.2"
 clusterfutures = "^0.5"
 cloudpickle = ">=3.0.0,<3.1.0"
 
 asyncpg = { version = "^0.29.0", optional = true }
 psycopg2 = { version = "^2.9.5", optional = true }
-gunicorn = { version = "^21.2.0", optional = true }
+gunicorn = { version = ">=21.2,<23.0", optional = true }
 
 [tool.poetry.extras]
 postgres = ["asyncpg", "psycopg2"]
 gunicorn = ["gunicorn"]
 
 [tool.poetry.group.dev.dependencies]
 asgi-lifespan = "^2"
@@ -82,15 +82,15 @@
 asyncio_mode = "auto"
 filterwarnings = [
     "error::RuntimeWarning",
     "error::pytest.PytestUnraisableExceptionWarning",
 ]
 
 [tool.bumpver]
-current_version = "2.0.0a8"
+current_version = "2.0.0a9"
 version_pattern = "MAJOR.MINOR.PATCH[PYTAGNUM]"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `fractal_server-2.0.0a8/PKG-INFO` & `fractal_server-2.0.0a9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fractal-server
-Version: 2.0.0a8
+Version: 2.0.0a9
 Summary: Server component of the Fractal analytics platform
 Home-page: https://github.com/fractal-analytics-platform/fractal-server
 License: BSD-3-Clause
 Author: Jacopo Nespolo
 Author-email: jacopo.nespolo@exact-lab.it
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: BSD License
@@ -19,15 +19,15 @@
 Requires-Dist: alembic (>=1.13.1,<2.0.0)
 Requires-Dist: asyncpg (>=0.29.0,<0.30.0) ; extra == "postgres"
 Requires-Dist: bcrypt (==4.0.1)
 Requires-Dist: cloudpickle (>=3.0.0,<3.1.0)
 Requires-Dist: clusterfutures (>=0.5,<0.6)
 Requires-Dist: fastapi (>=0.110.0,<0.111.0)
 Requires-Dist: fastapi-users[oauth] (>=12.1.0,<13.0.0)
-Requires-Dist: gunicorn (>=21.2.0,<22.0.0) ; extra == "gunicorn"
+Requires-Dist: gunicorn (>=21.2,<23.0) ; extra == "gunicorn"
 Requires-Dist: packaging (>=23.2,<24.0)
 Requires-Dist: psycopg2 (>=2.9.5,<3.0.0) ; extra == "postgres"
 Requires-Dist: pydantic (>=1.10.8,<2)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: sqlalchemy[asyncio] (>=2.0.23,<2.1)
 Requires-Dist: sqlmodel (>=0.0.16,<0.0.17)
 Requires-Dist: uvicorn (>=0.29.0,<0.30.0)
```


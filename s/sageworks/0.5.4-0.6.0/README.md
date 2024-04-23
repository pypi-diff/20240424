# Comparing `tmp/sageworks-0.5.4.tar.gz` & `tmp/sageworks-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sageworks-0.5.4.tar", last modified: Wed Apr  3 19:02:27 2024, max compression
+gzip compressed data, was "sageworks-0.6.0.tar", last modified: Tue Apr 23 16:58:06 2024, max compression
```

## Comparing `sageworks-0.5.4.tar` & `sageworks-0.6.0.tar`

### file list

```diff
@@ -1,512 +1,540 @@
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.720978 sageworks-0.5.4/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.665006 sageworks-0.5.4/.github/
--rw-r--r--   0 briford    (501) staff       (20)     1338 2024-03-28 17:23:43.000000 sageworks-0.5.4/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 briford    (501) staff       (20)      499 2023-12-24 17:18:24.000000 sageworks-0.5.4/.github/dependabot.yml
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.665257 sageworks-0.5.4/.github/workflows/
--rw-r--r--   0 briford    (501) staff       (20)      598 2024-01-10 18:45:51.000000 sageworks-0.5.4/.github/workflows/deploy-docs.yml
--rw-r--r--   0 briford    (501) staff       (20)      556 2024-01-23 15:36:53.000000 sageworks-0.5.4/.github/workflows/python-lint.yml
--rw-r--r--   0 briford    (501) staff       (20)     2008 2023-12-24 17:18:24.000000 sageworks-0.5.4/.gitignore
--rw-r--r--   0 briford    (501) staff       (20)      444 2024-03-28 17:23:43.000000 sageworks-0.5.4/CONTRIBUTING.md
--rw-r--r--   0 briford    (501) staff       (20)      102 2024-03-28 17:23:43.000000 sageworks-0.5.4/Dockerfile
--rw-r--r--   0 briford    (501) staff       (20)     1080 2024-03-28 17:23:43.000000 sageworks-0.5.4/LICENSE
--rw-r--r--   0 briford    (501) staff       (20)     1426 2023-12-24 17:18:24.000000 sageworks-0.5.4/Makefile
--rw-r--r--   0 briford    (501) staff       (20)     4118 2024-04-03 19:02:27.720896 sageworks-0.5.4/PKG-INFO
--rw-r--r--   0 briford    (501) staff       (20)     2695 2024-03-28 17:23:43.000000 sageworks-0.5.4/README.md
--rw-r--r--   0 briford    (501) staff       (20)      463 2023-12-24 17:18:24.000000 sageworks-0.5.4/SECURITY.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.655807 sageworks-0.5.4/applications/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.666406 sageworks-0.5.4/applications/aws_dashboard/
--rw-r--r--   0 briford    (501) staff       (20)     1071 2024-04-02 13:06:54.000000 sageworks-0.5.4/applications/aws_dashboard/Dockerfile
--rw-r--r--   0 briford    (501) staff       (20)      331 2024-03-28 17:23:43.000000 sageworks-0.5.4/applications/aws_dashboard/Dockerfile_plugins
--rw-r--r--   0 briford    (501) staff       (20)      841 2024-01-10 18:45:51.000000 sageworks-0.5.4/applications/aws_dashboard/README.md
--rw-r--r--   0 briford    (501) staff       (20)     1526 2024-04-02 16:53:34.000000 sageworks-0.5.4/applications/aws_dashboard/app.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.667116 sageworks-0.5.4/applications/aws_dashboard/assets/
--rw-r--r--   0 briford    (501) staff       (20)   232839 2024-04-02 13:06:54.000000 sageworks-0.5.4/applications/aws_dashboard/assets/bootstrap_darkly.min.css
--rw-r--r--   0 briford    (501) staff       (20)    14995 2024-04-02 13:06:54.000000 sageworks-0.5.4/applications/aws_dashboard/assets/default.css
--rw-r--r--   0 briford    (501) staff       (20)      318 2023-12-24 17:18:24.000000 sageworks-0.5.4/applications/aws_dashboard/assets/favicon.ico
--rw-r--r--   0 briford    (501) staff       (20)      732 2023-12-24 17:18:24.000000 sageworks-0.5.4/applications/aws_dashboard/assets/trash.png
--rwxr-xr-x   0 briford    (501) staff       (20)      637 2024-04-02 15:05:11.000000 sageworks-0.5.4/applications/aws_dashboard/dashboard
--rw-r--r--   0 briford    (501) staff       (20)      205 2023-12-24 17:18:24.000000 sageworks-0.5.4/applications/aws_dashboard/nginx.conf
--rw-r--r--   0 briford    (501) staff       (20)      684 2024-03-28 17:23:43.000000 sageworks-0.5.4/applications/aws_dashboard/open_source_config.json
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.655732 sageworks-0.5.4/applications/aws_dashboard/pages/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.667560 sageworks-0.5.4/applications/aws_dashboard/pages/data_sources/
--rw-r--r--   0 briford    (501) staff       (20)    11696 2024-03-30 22:43:51.000000 sageworks-0.5.4/applications/aws_dashboard/pages/data_sources/callbacks.py
--rw-r--r--   0 briford    (501) staff       (20)     2756 2024-03-28 17:23:43.000000 sageworks-0.5.4/applications/aws_dashboard/pages/data_sources/layout.py
--rw-r--r--   0 briford    (501) staff       (20)     2555 2024-03-28 17:23:43.000000 sageworks-0.5.4/applications/aws_dashboard/pages/data_sources/page.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.667958 sageworks-0.5.4/applications/aws_dashboard/pages/endpoints/
--rw-r--r--   0 briford    (501) staff       (20)     3975 2024-03-30 22:43:51.000000 sageworks-0.5.4/applications/aws_dashboard/pages/endpoints/callbacks.py
--rw-r--r--   0 briford    (501) staff       (20)     2565 2024-03-28 17:23:43.000000 sageworks-0.5.4/applications/aws_dashboard/pages/endpoints/layout.py
--rw-r--r--   0 briford    (501) staff       (20)     2465 2024-03-28 17:23:43.000000 sageworks-0.5.4/applications/aws_dashboard/pages/endpoints/page.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.668398 sageworks-0.5.4/applications/aws_dashboard/pages/feature_sets/
--rw-r--r--   0 briford    (501) staff       (20)    11610 2024-03-30 22:43:51.000000 sageworks-0.5.4/applications/aws_dashboard/pages/feature_sets/callbacks.py
--rw-r--r--   0 briford    (501) staff       (20)     2438 2024-03-28 17:23:43.000000 sageworks-0.5.4/applications/aws_dashboard/pages/feature_sets/layout.py
--rw-r--r--   0 briford    (501) staff       (20)     2505 2024-03-28 17:23:43.000000 sageworks-0.5.4/applications/aws_dashboard/pages/feature_sets/page.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.668822 sageworks-0.5.4/applications/aws_dashboard/pages/main/
--rw-r--r--   0 briford    (501) staff       (20)     4899 2024-03-30 22:43:51.000000 sageworks-0.5.4/applications/aws_dashboard/pages/main/callbacks.py
--rw-r--r--   0 briford    (501) staff       (20)     2899 2024-03-28 17:23:43.000000 sageworks-0.5.4/applications/aws_dashboard/pages/main/layout.py
--rw-r--r--   0 briford    (501) staff       (20)     1844 2024-03-28 17:23:43.000000 sageworks-0.5.4/applications/aws_dashboard/pages/main/page.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.669240 sageworks-0.5.4/applications/aws_dashboard/pages/models/
--rw-r--r--   0 briford    (501) staff       (20)     3760 2024-04-03 18:28:10.000000 sageworks-0.5.4/applications/aws_dashboard/pages/models/callbacks.py
--rw-r--r--   0 briford    (501) staff       (20)     2020 2024-03-28 17:23:43.000000 sageworks-0.5.4/applications/aws_dashboard/pages/models/layout.py
--rw-r--r--   0 briford    (501) staff       (20)     2341 2024-03-28 17:23:43.000000 sageworks-0.5.4/applications/aws_dashboard/pages/models/page.py
--rw-r--r--   0 briford    (501) staff       (20)      394 2024-04-02 13:06:54.000000 sageworks-0.5.4/applications/aws_dashboard/requirements.txt
--rw-r--r--   0 briford    (501) staff       (20)      457 2023-12-24 17:18:24.000000 sageworks-0.5.4/applications/aws_dashboard/supervisord.conf
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.655867 sageworks-0.5.4/applications/experiments/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.670057 sageworks-0.5.4/applications/experiments/compound_explorer/
--rw-r--r--   0 briford    (501) staff       (20)      181 2023-12-24 17:18:24.000000 sageworks-0.5.4/applications/experiments/compound_explorer/Dockerfile
--rw-r--r--   0 briford    (501) staff       (20)      360 2023-12-24 17:18:24.000000 sageworks-0.5.4/applications/experiments/compound_explorer/README.md
--rw-r--r--   0 briford    (501) staff       (20)     3082 2024-04-02 16:53:34.000000 sageworks-0.5.4/applications/experiments/compound_explorer/app.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.670304 sageworks-0.5.4/applications/experiments/compound_explorer/assets/
--rw-r--r--   0 briford    (501) staff       (20)    12861 2023-12-24 17:18:24.000000 sageworks-0.5.4/applications/experiments/compound_explorer/assets/custom.css
--rw-r--r--   0 briford    (501) staff       (20)      318 2023-12-24 17:18:24.000000 sageworks-0.5.4/applications/experiments/compound_explorer/assets/favicon.ico
--rw-r--r--   0 briford    (501) staff       (20)     7676 2024-03-30 22:43:51.000000 sageworks-0.5.4/applications/experiments/compound_explorer/callbacks.py
--rw-r--r--   0 briford    (501) staff       (20)     4860 2024-03-28 17:23:43.000000 sageworks-0.5.4/applications/experiments/compound_explorer/layout.py
--rw-r--r--   0 briford    (501) staff       (20)       94 2023-12-24 17:18:24.000000 sageworks-0.5.4/applications/experiments/compound_explorer/requirements.txt
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.670695 sageworks-0.5.4/aws_setup/
--rw-r--r--   0 briford    (501) staff       (20)     3582 2024-03-28 17:23:43.000000 sageworks-0.5.4/aws_setup/aws_account_check.py
--rw-r--r--   0 briford    (501) staff       (20)     1403 2024-03-28 17:23:43.000000 sageworks-0.5.4/aws_setup/aws_identity_check.py
--rw-r--r--   0 briford    (501) staff       (20)     2629 2024-03-28 17:23:43.000000 sageworks-0.5.4/aws_setup/build_ml_pipeline.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.670820 sageworks-0.5.4/aws_setup/event_bridge/
--rw-r--r--   0 briford    (501) staff       (20)       60 2023-12-24 17:18:24.000000 sageworks-0.5.4/aws_setup/event_bridge/Readme.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.671354 sageworks-0.5.4/aws_setup/event_bridge/dynamic_docker/
--rw-r--r--   0 briford    (501) staff       (20)       60 2023-12-24 17:18:24.000000 sageworks-0.5.4/aws_setup/event_bridge/dynamic_docker/Readme.md
--rw-r--r--   0 briford    (501) staff       (20)     1007 2023-12-24 17:18:24.000000 sageworks-0.5.4/aws_setup/event_bridge/dynamic_docker/app.py
--rw-r--r--   0 briford    (501) staff       (20)     2567 2023-12-24 17:18:24.000000 sageworks-0.5.4/aws_setup/event_bridge/dynamic_docker/cdk.json
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.671484 sageworks-0.5.4/aws_setup/event_bridge/dynamic_docker/lambda/
--rw-r--r--   0 briford    (501) staff       (20)     1812 2024-01-10 18:45:51.000000 sageworks-0.5.4/aws_setup/event_bridge/dynamic_docker/lambda/lambda_replace_task.py
--rw-r--r--   0 briford    (501) staff       (20)     2599 2024-03-27 20:43:31.000000 sageworks-0.5.4/aws_setup/event_bridge/dynamic_docker/sageworks_image_update_stack.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.672386 sageworks-0.5.4/aws_setup/sageworks_core/
--rw-r--r--   0 briford    (501) staff       (20)      119 2023-12-24 17:18:24.000000 sageworks-0.5.4/aws_setup/sageworks_core/.gitignore
--rw-r--r--   0 briford    (501) staff       (20)     1028 2023-12-24 17:18:24.000000 sageworks-0.5.4/aws_setup/sageworks_core/README.md
--rw-r--r--   0 briford    (501) staff       (20)     1403 2024-03-28 17:23:43.000000 sageworks-0.5.4/aws_setup/sageworks_core/app.py
--rw-r--r--   0 briford    (501) staff       (20)     1998 2023-12-24 17:18:24.000000 sageworks-0.5.4/aws_setup/sageworks_core/cdk.json
--rw-r--r--   0 briford    (501) staff       (20)       14 2023-12-24 17:18:24.000000 sageworks-0.5.4/aws_setup/sageworks_core/requirements-dev.txt
--rw-r--r--   0 briford    (501) staff       (20)       53 2024-01-10 18:45:51.000000 sageworks-0.5.4/aws_setup/sageworks_core/requirements.txt
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.672609 sageworks-0.5.4/aws_setup/sageworks_core/sageworks_core/
--rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.5.4/aws_setup/sageworks_core/sageworks_core/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)    23575 2024-03-28 17:23:43.000000 sageworks-0.5.4/aws_setup/sageworks_core/sageworks_core/sageworks_core_stack.py
--rw-r--r--   0 briford    (501) staff       (20)      437 2023-12-24 17:18:24.000000 sageworks-0.5.4/aws_setup/sageworks_core/source.bat
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.672758 sageworks-0.5.4/aws_setup/sageworks_core/tests/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-12-24 17:18:24.000000 sageworks-0.5.4/aws_setup/sageworks_core/tests/__init__.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.672953 sageworks-0.5.4/aws_setup/sageworks_core/tests/unit/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-12-24 17:18:24.000000 sageworks-0.5.4/aws_setup/sageworks_core/tests/unit/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)      720 2023-12-24 17:18:24.000000 sageworks-0.5.4/aws_setup/sageworks_core/tests/unit/test_sageworks_sandbox_stack.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.673884 sageworks-0.5.4/aws_setup/sageworks_dashboard_full/
--rw-r--r--   0 briford    (501) staff       (20)      119 2023-12-24 17:18:24.000000 sageworks-0.5.4/aws_setup/sageworks_dashboard_full/.gitignore
--rw-r--r--   0 briford    (501) staff       (20)     1778 2024-03-28 17:23:43.000000 sageworks-0.5.4/aws_setup/sageworks_dashboard_full/README.md
--rw-r--r--   0 briford    (501) staff       (20)     1907 2024-03-28 17:23:43.000000 sageworks-0.5.4/aws_setup/sageworks_dashboard_full/app.py
--rw-r--r--   0 briford    (501) staff       (20)     2567 2023-12-24 17:18:24.000000 sageworks-0.5.4/aws_setup/sageworks_dashboard_full/cdk.json
--rw-r--r--   0 briford    (501) staff       (20)       14 2023-12-24 17:18:24.000000 sageworks-0.5.4/aws_setup/sageworks_dashboard_full/requirements-dev.txt
--rw-r--r--   0 briford    (501) staff       (20)       47 2023-12-24 17:18:24.000000 sageworks-0.5.4/aws_setup/sageworks_dashboard_full/requirements.txt
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.674115 sageworks-0.5.4/aws_setup/sageworks_dashboard_full/sageworks_dashboard_full/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-12-24 17:18:24.000000 sageworks-0.5.4/aws_setup/sageworks_dashboard_full/sageworks_dashboard_full/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)     7022 2024-04-02 13:06:54.000000 sageworks-0.5.4/aws_setup/sageworks_dashboard_full/sageworks_dashboard_full/sageworks_dashboard_stack.py
--rw-r--r--   0 briford    (501) staff       (20)      437 2023-12-24 17:18:24.000000 sageworks-0.5.4/aws_setup/sageworks_dashboard_full/source.bat
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.674258 sageworks-0.5.4/aws_setup/sageworks_dashboard_full/tests/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-12-24 17:18:24.000000 sageworks-0.5.4/aws_setup/sageworks_dashboard_full/tests/__init__.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.674452 sageworks-0.5.4/aws_setup/sageworks_dashboard_full/tests/unit/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-12-24 17:18:24.000000 sageworks-0.5.4/aws_setup/sageworks_dashboard_full/tests/unit/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)      565 2023-12-24 17:18:24.000000 sageworks-0.5.4/aws_setup/sageworks_dashboard_full/tests/unit/test_sageworks_dashboard_stack.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.675075 sageworks-0.5.4/aws_setup/sageworks_dashboard_lite/
--rw-r--r--   0 briford    (501) staff       (20)      119 2024-03-28 17:23:43.000000 sageworks-0.5.4/aws_setup/sageworks_dashboard_lite/.gitignore
--rw-r--r--   0 briford    (501) staff       (20)     1778 2024-03-28 17:23:43.000000 sageworks-0.5.4/aws_setup/sageworks_dashboard_lite/README.md
--rw-r--r--   0 briford    (501) staff       (20)     1928 2024-03-28 17:23:43.000000 sageworks-0.5.4/aws_setup/sageworks_dashboard_lite/app.py
--rw-r--r--   0 briford    (501) staff       (20)     2567 2024-03-28 17:23:43.000000 sageworks-0.5.4/aws_setup/sageworks_dashboard_lite/cdk.json
--rw-r--r--   0 briford    (501) staff       (20)       47 2024-03-28 17:23:43.000000 sageworks-0.5.4/aws_setup/sageworks_dashboard_lite/requirements.txt
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.675309 sageworks-0.5.4/aws_setup/sageworks_dashboard_lite/sageworks_dashboard_lite/
--rw-r--r--   0 briford    (501) staff       (20)        0 2024-03-28 17:23:43.000000 sageworks-0.5.4/aws_setup/sageworks_dashboard_lite/sageworks_dashboard_lite/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)     6849 2024-04-02 13:06:54.000000 sageworks-0.5.4/aws_setup/sageworks_dashboard_lite/sageworks_dashboard_lite/sageworks_dashboard_stack.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.675970 sageworks-0.5.4/data/
--rw-r--r--   0 briford    (501) staff       (20)   191978 2023-12-24 17:18:24.000000 sageworks-0.5.4/data/abalone.csv
--rw-r--r--   0 briford    (501) staff       (20)     1515 2023-12-24 17:18:24.000000 sageworks-0.5.4/data/test_data.csv
--rw-r--r--   0 briford    (501) staff       (20)     2270 2023-12-24 17:18:24.000000 sageworks-0.5.4/data/test_data.json
--rw-r--r--   0 briford    (501) staff       (20)    12977 2024-01-10 18:45:51.000000 sageworks-0.5.4/data/wine_dataset.csv
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.676200 sageworks-0.5.4/docs/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.676513 sageworks-0.5.4/docs/admin/
--rw-r--r--   0 briford    (501) staff       (20)     1825 2024-03-28 17:23:43.000000 sageworks-0.5.4/docs/admin/docker_push.md
--rw-r--r--   0 briford    (501) staff       (20)     1633 2024-01-10 18:45:51.000000 sageworks-0.5.4/docs/admin/pypi_release.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.677585 sageworks-0.5.4/docs/api_classes/
--rw-r--r--   0 briford    (501) staff       (20)     3595 2024-01-23 15:36:53.000000 sageworks-0.5.4/docs/api_classes/data_source.md
--rw-r--r--   0 briford    (501) staff       (20)     5199 2024-03-28 17:23:43.000000 sageworks-0.5.4/docs/api_classes/endpoint.md
--rw-r--r--   0 briford    (501) staff       (20)     6299 2024-03-28 17:23:43.000000 sageworks-0.5.4/docs/api_classes/feature_set.md
--rw-r--r--   0 briford    (501) staff       (20)     5350 2024-03-30 23:05:32.000000 sageworks-0.5.4/docs/api_classes/meta.md
--rw-r--r--   0 briford    (501) staff       (20)     4356 2024-01-10 18:45:51.000000 sageworks-0.5.4/docs/api_classes/model.md
--rw-r--r--   0 briford    (501) staff       (20)     2218 2024-01-10 18:45:51.000000 sageworks-0.5.4/docs/api_classes/monitor.md
--rw-r--r--   0 briford    (501) staff       (20)     3549 2024-01-10 18:45:51.000000 sageworks-0.5.4/docs/api_classes/overview.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.678278 sageworks-0.5.4/docs/aws_setup/
--rw-r--r--   0 briford    (501) staff       (20)     1121 2024-03-28 17:23:43.000000 sageworks-0.5.4/docs/aws_setup/aws_access_management.md
--rw-r--r--   0 briford    (501) staff       (20)     7836 2024-01-23 15:36:53.000000 sageworks-0.5.4/docs/aws_setup/aws_tips_and_tricks.md
--rw-r--r--   0 briford    (501) staff       (20)     4229 2024-03-28 17:23:43.000000 sageworks-0.5.4/docs/aws_setup/core_stack.md
--rw-r--r--   0 briford    (501) staff       (20)     2075 2024-03-28 17:23:43.000000 sageworks-0.5.4/docs/aws_setup/dashboard_stack.md
--rw-r--r--   0 briford    (501) staff       (20)     2540 2024-01-23 15:36:53.000000 sageworks-0.5.4/docs/aws_setup/full_pipeline.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.678409 sageworks-0.5.4/docs/concepts/
--rw-r--r--   0 briford    (501) staff       (20)      907 2024-01-23 15:36:53.000000 sageworks-0.5.4/docs/concepts/model_monitoring.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.678538 sageworks-0.5.4/docs/core_classes/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.679573 sageworks-0.5.4/docs/core_classes/artifacts/
--rw-r--r--   0 briford    (501) staff       (20)      464 2024-01-23 15:36:53.000000 sageworks-0.5.4/docs/core_classes/artifacts/artifact.md
--rw-r--r--   0 briford    (501) staff       (20)      290 2024-01-10 18:45:51.000000 sageworks-0.5.4/docs/core_classes/artifacts/athena_source.md
--rw-r--r--   0 briford    (501) staff       (20)      479 2024-01-23 15:36:53.000000 sageworks-0.5.4/docs/core_classes/artifacts/data_source_abstract.md
--rw-r--r--   0 briford    (501) staff       (20)      292 2024-01-10 18:45:51.000000 sageworks-0.5.4/docs/core_classes/artifacts/endpoint_core.md
--rw-r--r--   0 briford    (501) staff       (20)      294 2024-01-10 18:45:51.000000 sageworks-0.5.4/docs/core_classes/artifacts/feature_set_core.md
--rw-r--r--   0 briford    (501) staff       (20)      281 2024-01-10 18:45:51.000000 sageworks-0.5.4/docs/core_classes/artifacts/model_core.md
--rw-r--r--   0 briford    (501) staff       (20)      289 2024-01-10 18:45:51.000000 sageworks-0.5.4/docs/core_classes/artifacts/monitor_core.md
--rw-r--r--   0 briford    (501) staff       (20)      861 2024-01-10 18:45:51.000000 sageworks-0.5.4/docs/core_classes/artifacts/overview.md
--rw-r--r--   0 briford    (501) staff       (20)     2119 2024-01-10 18:45:51.000000 sageworks-0.5.4/docs/core_classes/overview.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.680637 sageworks-0.5.4/docs/core_classes/transforms/
--rw-r--r--   0 briford    (501) staff       (20)      352 2024-01-10 18:45:51.000000 sageworks-0.5.4/docs/core_classes/transforms/data_loaders_heavy.md
--rw-r--r--   0 briford    (501) staff       (20)      396 2024-01-10 18:45:51.000000 sageworks-0.5.4/docs/core_classes/transforms/data_loaders_light.md
--rw-r--r--   0 briford    (501) staff       (20)      349 2024-03-28 17:23:43.000000 sageworks-0.5.4/docs/core_classes/transforms/data_to_features.md
--rw-r--r--   0 briford    (501) staff       (20)      265 2024-01-10 18:45:51.000000 sageworks-0.5.4/docs/core_classes/transforms/features_to_model.md
--rw-r--r--   0 briford    (501) staff       (20)      264 2024-01-10 18:45:51.000000 sageworks-0.5.4/docs/core_classes/transforms/model_to_endpoint.md
--rw-r--r--   0 briford    (501) staff       (20)     1177 2024-01-10 18:45:51.000000 sageworks-0.5.4/docs/core_classes/transforms/overview.md
--rw-r--r--   0 briford    (501) staff       (20)      970 2024-01-23 15:36:53.000000 sageworks-0.5.4/docs/core_classes/transforms/pandas_transforms.md
--rw-r--r--   0 briford    (501) staff       (20)      521 2024-01-23 15:36:53.000000 sageworks-0.5.4/docs/core_classes/transforms/transform.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.680781 sageworks-0.5.4/docs/glue/
--rw-r--r--   0 briford    (501) staff       (20)     4837 2024-03-28 17:23:43.000000 sageworks-0.5.4/docs/glue/index.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.683011 sageworks-0.5.4/docs/images/
--rw-r--r--   0 briford    (501) staff       (20)   605827 2023-12-24 17:18:24.000000 sageworks-0.5.4/docs/images/big_spider.png
--rw-r--r--   0 briford    (501) staff       (20)    32320 2023-12-24 17:18:24.000000 sageworks-0.5.4/docs/images/graph_representation.png
--rw-r--r--   0 briford    (501) staff       (20)    15549 2023-12-24 17:18:24.000000 sageworks-0.5.4/docs/images/powered_aws_dark_blue.png
--rw-r--r--   0 briford    (501) staff       (20)    10003 2023-12-24 17:18:24.000000 sageworks-0.5.4/docs/images/powered_aws_transparent.png
--rw-r--r--   0 briford    (501) staff       (20)     6435 2023-12-24 17:18:24.000000 sageworks-0.5.4/docs/images/powered_aws_white.png
--rw-r--r--   0 briford    (501) staff       (20)    21174 2023-12-24 17:18:24.000000 sageworks-0.5.4/docs/images/powered_aws_with_tm_grey.png
--rw-r--r--   0 briford    (501) staff       (20)    51137 2023-12-24 17:18:24.000000 sageworks-0.5.4/docs/images/sageworks.png
--rw-r--r--   0 briford    (501) staff       (20)   489672 2023-12-24 17:18:24.000000 sageworks-0.5.4/docs/images/sageworks_concepts.png
--rw-r--r--   0 briford    (501) staff       (20)    30017 2023-12-24 17:18:24.000000 sageworks-0.5.4/docs/images/scp.png
--rw-r--r--   0 briford    (501) staff       (20)   139307 2023-12-24 17:18:24.000000 sageworks-0.5.4/docs/images/scp_labs.png
--rw-r--r--   0 briford    (501) staff       (20)   381209 2023-12-24 17:18:24.000000 sageworks-0.5.4/docs/images/small_spider.png
--rw-r--r--   0 briford    (501) staff       (20)     3417 2024-03-28 17:23:43.000000 sageworks-0.5.4/docs/index.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.683704 sageworks-0.5.4/docs/misc/
--rw-r--r--   0 briford    (501) staff       (20)     2791 2024-03-28 17:23:43.000000 sageworks-0.5.4/docs/misc/faq.md
--rw-r--r--   0 briford    (501) staff       (20)     5069 2024-01-10 18:45:51.000000 sageworks-0.5.4/docs/misc/general_info.md
--rw-r--r--   0 briford    (501) staff       (20)      667 2024-01-10 18:45:51.000000 sageworks-0.5.4/docs/misc/sageworks_classes_concepts.md
--rw-r--r--   0 briford    (501) staff       (20)     1873 2024-01-10 18:45:51.000000 sageworks-0.5.4/docs/misc/scp_consulting.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.683967 sageworks-0.5.4/docs/plugins/
--rw-r--r--   0 briford    (501) staff       (20)     3221 2024-04-03 13:42:22.000000 sageworks-0.5.4/docs/plugins/index.md
--rw-r--r--   0 briford    (501) staff       (20)      750 2024-03-31 15:49:43.000000 sageworks-0.5.4/docs/plugins/plugin_api_changes.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.684091 sageworks-0.5.4/docs/repl/
--rw-r--r--   0 briford    (501) staff       (20)     2081 2024-03-28 17:23:43.000000 sageworks-0.5.4/docs/repl/index.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.684337 sageworks-0.5.4/docs/research/
--rw-r--r--   0 briford    (501) staff       (20)      912 2024-03-28 17:23:43.000000 sageworks-0.5.4/docs/research/eda.md
--rw-r--r--   0 briford    (501) staff       (20)     2017 2024-03-28 17:23:43.000000 sageworks-0.5.4/docs/research/htg.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.687286 sageworks-0.5.4/examples/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.687422 sageworks-0.5.4/examples/ag-grid/
--rw-r--r--   0 briford    (501) staff       (20)      496 2024-04-02 13:06:54.000000 sageworks-0.5.4/examples/ag-grid/hello_world.py
--rw-r--r--   0 briford    (501) staff       (20)      326 2024-01-10 18:45:51.000000 sageworks-0.5.4/examples/datasource_from_df.py
--rw-r--r--   0 briford    (501) staff       (20)      332 2024-01-10 18:45:51.000000 sageworks-0.5.4/examples/datasource_from_s3.py
--rw-r--r--   0 briford    (501) staff       (20)      536 2024-01-23 15:36:53.000000 sageworks-0.5.4/examples/datasource_query.py
--rw-r--r--   0 briford    (501) staff       (20)      680 2024-01-23 15:36:53.000000 sageworks-0.5.4/examples/datasource_stats.py
--rw-r--r--   0 briford    (501) staff       (20)      223 2024-01-10 18:45:51.000000 sageworks-0.5.4/examples/datasource_to_featureset.py
--rw-r--r--   0 briford    (501) staff       (20)      199 2024-01-10 18:45:51.000000 sageworks-0.5.4/examples/endpoint_details.py
--rw-r--r--   0 briford    (501) staff       (20)      834 2024-03-28 17:23:43.000000 sageworks-0.5.4/examples/endpoint_inference.py
--rw-r--r--   0 briford    (501) staff       (20)      481 2024-01-10 18:45:51.000000 sageworks-0.5.4/examples/endpoint_metrics.py
--rw-r--r--   0 briford    (501) staff       (20)      744 2024-01-10 18:45:51.000000 sageworks-0.5.4/examples/featureset_eda.py
--rw-r--r--   0 briford    (501) staff       (20)      560 2024-03-28 17:23:43.000000 sageworks-0.5.4/examples/featureset_query.py
--rw-r--r--   0 briford    (501) staff       (20)      421 2024-03-27 20:32:26.000000 sageworks-0.5.4/examples/featureset_to_model.py
--rw-r--r--   0 briford    (501) staff       (20)     1534 2024-03-28 17:23:43.000000 sageworks-0.5.4/examples/full_ml_pipeline.py
--rw-r--r--   0 briford    (501) staff       (20)      580 2024-01-23 15:36:53.000000 sageworks-0.5.4/examples/glue_hello_world.py
--rw-r--r--   0 briford    (501) staff       (20)      942 2024-01-23 15:36:53.000000 sageworks-0.5.4/examples/glue_hello_world_with_log.py
--rw-r--r--   0 briford    (501) staff       (20)      686 2024-01-23 15:36:53.000000 sageworks-0.5.4/examples/glue_load_s3_bucket.py
--rw-r--r--   0 briford    (501) staff       (20)      363 2024-03-30 22:43:51.000000 sageworks-0.5.4/examples/meta_list_endpoints.py
--rw-r--r--   0 briford    (501) staff       (20)      328 2024-03-30 22:43:51.000000 sageworks-0.5.4/examples/meta_list_models.py
--rw-r--r--   0 briford    (501) staff       (20)      659 2024-03-30 22:43:51.000000 sageworks-0.5.4/examples/meta_model_metrics.py
--rw-r--r--   0 briford    (501) staff       (20)      548 2024-03-28 17:23:43.000000 sageworks-0.5.4/examples/model_metrics.py
--rw-r--r--   0 briford    (501) staff       (20)      312 2024-03-27 20:32:26.000000 sageworks-0.5.4/examples/model_to_endpoint.py
--rw-r--r--   0 briford    (501) staff       (20)      400 2024-01-10 18:45:51.000000 sageworks-0.5.4/examples/monitor_setup.py
--rw-r--r--   0 briford    (501) staff       (20)      765 2024-01-10 18:45:51.000000 sageworks-0.5.4/examples/monitor_usage.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.658584 sageworks-0.5.4/examples/plugins/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.687948 sageworks-0.5.4/examples/plugins/pages/
--rw-r--r--   0 briford    (501) staff       (20)     2467 2024-04-02 16:53:34.000000 sageworks-0.5.4/examples/plugins/pages/my_plugin_page.py
--rw-r--r--   0 briford    (501) staff       (20)     1621 2024-04-02 17:39:18.000000 sageworks-0.5.4/examples/plugins/pages/plugin_page_1.py
--rw-r--r--   0 briford    (501) staff       (20)     2461 2024-04-02 17:39:30.000000 sageworks-0.5.4/examples/plugins/pages/plugin_page_2.py
--rw-r--r--   0 briford    (501) staff       (20)     4473 2024-04-02 17:39:18.000000 sageworks-0.5.4/examples/plugins/pages/plugin_page_3.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.688212 sageworks-0.5.4/examples/plugins/views/
--rw-r--r--   0 briford    (501) staff       (20)     1588 2024-04-02 13:46:33.000000 sageworks-0.5.4/examples/plugins/views/model_plugin_view.py
--rw-r--r--   0 briford    (501) staff       (20)     1264 2024-04-02 13:06:54.000000 sageworks-0.5.4/examples/plugins/views/my_view_plugin.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.688763 sageworks-0.5.4/examples/plugins/web_components/
--rw-r--r--   0 briford    (501) staff       (20)     1576 2024-04-02 13:46:33.000000 sageworks-0.5.4/examples/plugins/web_components/custom_plugin.py
--rw-r--r--   0 briford    (501) staff       (20)     1666 2024-04-02 13:06:54.000000 sageworks-0.5.4/examples/plugins/web_components/endpoint_plugin.py
--rw-r--r--   0 briford    (501) staff       (20)     3600 2024-04-02 13:46:33.000000 sageworks-0.5.4/examples/plugins/web_components/endpoint_turbo.py
--rw-r--r--   0 briford    (501) staff       (20)     1942 2024-04-02 13:06:54.000000 sageworks-0.5.4/examples/plugins/web_components/model_plugin.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.689207 sageworks-0.5.4/examples/sagemaker_pipelines/
--rw-r--r--   0 briford    (501) staff       (20)      854 2024-03-28 17:23:43.000000 sageworks-0.5.4/examples/sagemaker_pipelines/all_steps.py
--rw-r--r--   0 briford    (501) staff       (20)       40 2024-03-28 17:23:43.000000 sageworks-0.5.4/examples/sagemaker_pipelines/hello.py
--rw-r--r--   0 briford    (501) staff       (20)     1487 2024-03-28 17:23:43.000000 sageworks-0.5.4/examples/sagemaker_pipelines/ml_pipeline.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.658797 sageworks-0.5.4/examples/sagemaker_pipelines/storage/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.689986 sageworks-0.5.4/examples/sagemaker_pipelines/storage/full_pipeline_experiment/
--rw-r--r--   0 briford    (501) staff       (20)      854 2024-03-28 17:23:43.000000 sageworks-0.5.4/examples/sagemaker_pipelines/storage/full_pipeline_experiment/data_source.py
--rw-r--r--   0 briford    (501) staff       (20)      203 2024-03-28 17:23:43.000000 sageworks-0.5.4/examples/sagemaker_pipelines/storage/full_pipeline_experiment/endpoint.py
--rw-r--r--   0 briford    (501) staff       (20)      160 2024-03-28 17:23:43.000000 sageworks-0.5.4/examples/sagemaker_pipelines/storage/full_pipeline_experiment/feature_set.py
--rw-r--r--   0 briford    (501) staff       (20)     1599 2024-03-28 17:23:43.000000 sageworks-0.5.4/examples/sagemaker_pipelines/storage/full_pipeline_experiment/ml_pipeline.py
--rw-r--r--   0 briford    (501) staff       (20)      367 2024-03-28 17:23:43.000000 sageworks-0.5.4/examples/sagemaker_pipelines/storage/full_pipeline_experiment/model.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.690804 sageworks-0.5.4/examples/storage/
--rw-r--r--   0 briford    (501) staff       (20)     1222 2024-03-27 20:40:53.000000 sageworks-0.5.4/examples/storage/data_to_data.py
--rw-r--r--   0 briford    (501) staff       (20)      856 2024-03-27 20:40:53.000000 sageworks-0.5.4/examples/storage/data_to_features.py
--rw-r--r--   0 briford    (501) staff       (20)     1371 2024-03-28 17:23:43.000000 sageworks-0.5.4/examples/storage/endpoint_inference.py
--rw-r--r--   0 briford    (501) staff       (20)     1847 2024-03-28 17:23:43.000000 sageworks-0.5.4/examples/storage/hello_world_pipeline.py
--rw-r--r--   0 briford    (501) staff       (20)     4378 2024-04-02 13:06:34.000000 sageworks-0.5.4/examples/storage/plugin_page_example.py
--rw-r--r--   0 briford    (501) staff       (20)     2750 2024-03-31 15:47:34.000000 sageworks-0.5.4/mkdocs.yml
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.691312 sageworks-0.5.4/notebooks/
--rw-r--r--   0 briford    (501) staff       (20)   185443 2024-03-28 17:23:43.000000 sageworks-0.5.4/notebooks/ML_Pipeline_with_SageWorks.ipynb
--rw-r--r--   0 briford    (501) staff       (20)    36405 2024-03-28 17:23:43.000000 sageworks-0.5.4/notebooks/ML_Pipeline_with_SageWorks_2.ipynb
--rw-r--r--   0 briford    (501) staff       (20)   511134 2024-03-28 17:23:43.000000 sageworks-0.5.4/notebooks/Outliers_in_SageWorks.ipynb
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.692865 sageworks-0.5.4/notebooks/images/
--rw-r--r--   0 briford    (501) staff       (20)   142099 2023-12-24 17:18:24.000000 sageworks-0.5.4/notebooks/images/athena_query_aqsol.png
--rw-r--r--   0 briford    (501) staff       (20)   191022 2023-12-24 17:18:24.000000 sageworks-0.5.4/notebooks/images/aws_dashboard_aqsol.png
--rw-r--r--   0 briford    (501) staff       (20)   222686 2023-12-24 17:18:24.000000 sageworks-0.5.4/notebooks/images/dashboard_aqsol_features.png
--rw-r--r--   0 briford    (501) staff       (20)   171441 2023-12-24 17:18:24.000000 sageworks-0.5.4/notebooks/images/model_screenshot.png
--rw-r--r--   0 briford    (501) staff       (20)   489672 2023-12-24 17:18:24.000000 sageworks-0.5.4/notebooks/images/sageworks_concepts.png
--rw-r--r--   0 briford    (501) staff       (20)   139307 2023-12-24 17:18:24.000000 sageworks-0.5.4/notebooks/images/scp_labs.png
--rw-r--r--   0 briford    (501) staff       (20)      431 2024-04-02 13:06:54.000000 sageworks-0.5.4/requirements.txt
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.693960 sageworks-0.5.4/scripts/
--rw-r--r--   0 briford    (501) staff       (20)     2290 2024-03-28 17:23:43.000000 sageworks-0.5.4/scripts/athena_ddl_mixed_case.py
--rw-r--r--   0 briford    (501) staff       (20)     2178 2024-03-27 20:32:26.000000 sageworks-0.5.4/scripts/copy_data_catalog_db.py
--rw-r--r--   0 briford    (501) staff       (20)      706 2024-01-10 18:45:51.000000 sageworks-0.5.4/scripts/delete_redis_keys.py
--rw-r--r--   0 briford    (501) staff       (20)     1761 2024-03-28 17:23:43.000000 sageworks-0.5.4/scripts/glue_mixed_case.py
--rw-r--r--   0 briford    (501) staff       (20)     5544 2024-03-28 17:23:43.000000 sageworks-0.5.4/scripts/model_endpoint_sanity_check.py
--rw-r--r--   0 briford    (501) staff       (20)      715 2024-03-28 17:23:43.000000 sageworks-0.5.4/scripts/onboard_endpoints.py
--rw-r--r--   0 briford    (501) staff       (20)      694 2024-03-28 17:23:43.000000 sageworks-0.5.4/scripts/onboard_models.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.694299 sageworks-0.5.4/scripts/storage/
--rw-r--r--   0 briford    (501) staff       (20)     1003 2024-03-27 20:32:27.000000 sageworks-0.5.4/scripts/storage/dns_data_to_features.py
--rw-r--r--   0 briford    (501) staff       (20)     1723 2024-03-30 22:43:51.000000 sageworks-0.5.4/scripts/storage/generate_jsonl_data.py
--rw-r--r--   0 briford    (501) staff       (20)      955 2024-03-28 17:23:43.000000 sageworks-0.5.4/scripts/test_feature_resolution.py
--rw-r--r--   0 briford    (501) staff       (20)      533 2024-04-03 19:02:27.721338 sageworks-0.5.4/setup.cfg
--rw-r--r--   0 briford    (501) staff       (20)     1663 2024-03-27 20:32:27.000000 sageworks-0.5.4/setup.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.659354 sageworks-0.5.4/src/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.694447 sageworks-0.5.4/src/sageworks/
--rw-r--r--   0 briford    (501) staff       (20)     1091 2024-01-10 18:45:51.000000 sageworks-0.5.4/src/sageworks/__init__.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.695744 sageworks-0.5.4/src/sageworks/algorithms/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-12-24 17:18:24.000000 sageworks-0.5.4/src/sageworks/algorithms/__init__.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.696700 sageworks-0.5.4/src/sageworks/algorithms/dataframe/
--rw-r--r--   0 briford    (501) staff       (20)      378 2023-12-24 17:18:24.000000 sageworks-0.5.4/src/sageworks/algorithms/dataframe/Readme.md
--rw-r--r--   0 briford    (501) staff       (20)     2852 2024-03-28 17:23:43.000000 sageworks-0.5.4/src/sageworks/algorithms/dataframe/aggregation.py
--rw-r--r--   0 briford    (501) staff       (20)     1606 2024-03-28 17:23:43.000000 sageworks-0.5.4/src/sageworks/algorithms/dataframe/data_source_eda.py
--rw-r--r--   0 briford    (501) staff       (20)     5388 2024-03-28 17:23:43.000000 sageworks-0.5.4/src/sageworks/algorithms/dataframe/dimensionality_reduction.py
--rw-r--r--   0 briford    (501) staff       (20)     9406 2024-03-28 17:23:43.000000 sageworks-0.5.4/src/sageworks/algorithms/dataframe/feature_resolution.py
--rw-r--r--   0 briford    (501) staff       (20)    12309 2024-03-28 17:23:43.000000 sageworks-0.5.4/src/sageworks/algorithms/dataframe/feature_spider.py
--rw-r--r--   0 briford    (501) staff       (20)     4968 2024-03-28 17:23:43.000000 sageworks-0.5.4/src/sageworks/algorithms/dataframe/row_tagger.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.659713 sageworks-0.5.4/src/sageworks/algorithms/graph/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.696845 sageworks-0.5.4/src/sageworks/algorithms/graph/heavy/
--rw-r--r--   0 briford    (501) staff       (20)       96 2023-12-24 17:18:24.000000 sageworks-0.5.4/src/sageworks/algorithms/graph/heavy/Readme.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.696974 sageworks-0.5.4/src/sageworks/algorithms/graph/light/
--rw-r--r--   0 briford    (501) staff       (20)      122 2023-12-24 17:18:24.000000 sageworks-0.5.4/src/sageworks/algorithms/graph/light/Readme.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.697097 sageworks-0.5.4/src/sageworks/algorithms/spark/
--rw-r--r--   0 briford    (501) staff       (20)      615 2023-12-24 17:18:24.000000 sageworks-0.5.4/src/sageworks/algorithms/spark/Readme.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.698141 sageworks-0.5.4/src/sageworks/algorithms/sql/
--rw-r--r--   0 briford    (501) staff       (20)      685 2023-12-24 17:18:24.000000 sageworks-0.5.4/src/sageworks/algorithms/sql/Readme.md
--rw-r--r--   0 briford    (501) staff       (20)     6192 2024-03-28 17:23:43.000000 sageworks-0.5.4/src/sageworks/algorithms/sql/column_stats.py
--rw-r--r--   0 briford    (501) staff       (20)     3645 2024-03-28 17:23:43.000000 sageworks-0.5.4/src/sageworks/algorithms/sql/correlations.py
--rw-r--r--   0 briford    (501) staff       (20)     3622 2024-03-28 17:23:43.000000 sageworks-0.5.4/src/sageworks/algorithms/sql/descriptive_stats.py
--rw-r--r--   0 briford    (501) staff       (20)    10174 2024-03-28 17:23:43.000000 sageworks-0.5.4/src/sageworks/algorithms/sql/outliers.py
--rw-r--r--   0 briford    (501) staff       (20)     2352 2024-03-28 17:23:43.000000 sageworks-0.5.4/src/sageworks/algorithms/sql/sample_rows.py
--rw-r--r--   0 briford    (501) staff       (20)     3437 2024-03-28 17:23:43.000000 sageworks-0.5.4/src/sageworks/algorithms/sql/value_counts.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.699053 sageworks-0.5.4/src/sageworks/api/
--rw-r--r--   0 briford    (501) staff       (20)      708 2024-03-30 22:43:51.000000 sageworks-0.5.4/src/sageworks/api/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)     7811 2024-03-28 17:23:43.000000 sageworks-0.5.4/src/sageworks/api/data_source.py
--rw-r--r--   0 briford    (501) staff       (20)     2505 2024-03-28 17:23:43.000000 sageworks-0.5.4/src/sageworks/api/endpoint.py
--rw-r--r--   0 briford    (501) staff       (20)     4242 2024-03-28 17:23:43.000000 sageworks-0.5.4/src/sageworks/api/feature_set.py
--rw-r--r--   0 briford    (501) staff       (20)    15642 2024-03-30 22:43:51.000000 sageworks-0.5.4/src/sageworks/api/meta.py
--rw-r--r--   0 briford    (501) staff       (20)     2577 2024-03-28 17:23:43.000000 sageworks-0.5.4/src/sageworks/api/model.py
--rw-r--r--   0 briford    (501) staff       (20)     5261 2024-03-28 17:23:43.000000 sageworks-0.5.4/src/sageworks/api/monitor.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.699349 sageworks-0.5.4/src/sageworks/aws_service_broker/
--rw-r--r--   0 briford    (501) staff       (20)     9393 2024-03-28 17:23:43.000000 sageworks-0.5.4/src/sageworks/aws_service_broker/aws_account_clamp.py
--rw-r--r--   0 briford    (501) staff       (20)    10908 2024-03-30 22:43:51.000000 sageworks-0.5.4/src/sageworks/aws_service_broker/aws_service_broker.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.700396 sageworks-0.5.4/src/sageworks/aws_service_broker/aws_service_connectors/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-12-24 17:18:24.000000 sageworks-0.5.4/src/sageworks/aws_service_broker/aws_service_connectors/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)     1834 2024-03-28 17:23:43.000000 sageworks-0.5.4/src/sageworks/aws_service_broker/aws_service_connectors/connector.py
--rw-r--r--   0 briford    (501) staff       (20)     3258 2024-03-28 17:23:43.000000 sageworks-0.5.4/src/sageworks/aws_service_broker/aws_service_connectors/data_catalog.py
--rw-r--r--   0 briford    (501) staff       (20)     4055 2024-03-28 17:23:43.000000 sageworks-0.5.4/src/sageworks/aws_service_broker/aws_service_connectors/endpoints.py
--rw-r--r--   0 briford    (501) staff       (20)     5238 2024-03-28 17:23:43.000000 sageworks-0.5.4/src/sageworks/aws_service_broker/aws_service_connectors/feature_store.py
--rw-r--r--   0 briford    (501) staff       (20)     3712 2024-03-28 17:23:43.000000 sageworks-0.5.4/src/sageworks/aws_service_broker/aws_service_connectors/glue_jobs.py
--rw-r--r--   0 briford    (501) staff       (20)     3889 2024-03-28 17:23:43.000000 sageworks-0.5.4/src/sageworks/aws_service_broker/aws_service_connectors/model_registry.py
--rw-r--r--   0 briford    (501) staff       (20)     3736 2024-03-28 17:23:43.000000 sageworks-0.5.4/src/sageworks/aws_service_broker/aws_service_connectors/s3_bucket.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.700525 sageworks-0.5.4/src/sageworks/core/
--rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.5.4/src/sageworks/core/__init__.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.701722 sageworks-0.5.4/src/sageworks/core/artifacts/
--rw-r--r--   0 briford    (501) staff       (20)      941 2024-03-28 17:23:43.000000 sageworks-0.5.4/src/sageworks/core/artifacts/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)    17938 2024-03-30 22:43:51.000000 sageworks-0.5.4/src/sageworks/core/artifacts/artifact.py
--rw-r--r--   0 briford    (501) staff       (20)    22432 2024-03-30 22:43:51.000000 sageworks-0.5.4/src/sageworks/core/artifacts/athena_source.py
--rw-r--r--   0 briford    (501) staff       (20)    12683 2024-03-28 17:23:43.000000 sageworks-0.5.4/src/sageworks/core/artifacts/data_source_abstract.py
--rw-r--r--   0 briford    (501) staff       (20)     2447 2024-03-28 17:23:43.000000 sageworks-0.5.4/src/sageworks/core/artifacts/data_source_factory.py
--rw-r--r--   0 briford    (501) staff       (20)    36414 2024-03-28 17:23:43.000000 sageworks-0.5.4/src/sageworks/core/artifacts/endpoint_core.py
--rw-r--r--   0 briford    (501) staff       (20)    29123 2024-03-28 17:23:43.000000 sageworks-0.5.4/src/sageworks/core/artifacts/feature_set_core.py
--rw-r--r--   0 briford    (501) staff       (20)    35018 2024-03-29 21:27:39.000000 sageworks-0.5.4/src/sageworks/core/artifacts/model_core.py
--rw-r--r--   0 briford    (501) staff       (20)    21029 2024-03-28 17:23:43.000000 sageworks-0.5.4/src/sageworks/core/artifacts/monitor_core.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.702133 sageworks-0.5.4/src/sageworks/core/transforms/
--rw-r--r--   0 briford    (501) staff       (20)     1432 2024-01-10 18:45:51.000000 sageworks-0.5.4/src/sageworks/core/transforms/Readme.md
--rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.5.4/src/sageworks/core/transforms/__init__.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.702419 sageworks-0.5.4/src/sageworks/core/transforms/data_loaders/
--rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.5.4/src/sageworks/core/transforms/data_loaders/__init__.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.702700 sageworks-0.5.4/src/sageworks/core/transforms/data_loaders/heavy/
--rw-r--r--   0 briford    (501) staff       (20)      298 2024-03-28 17:23:43.000000 sageworks-0.5.4/src/sageworks/core/transforms/data_loaders/heavy/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)     9866 2024-03-28 17:23:43.000000 sageworks-0.5.4/src/sageworks/core/transforms/data_loaders/heavy/s3_heavy_to_data_source.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.703441 sageworks-0.5.4/src/sageworks/core/transforms/data_loaders/light/
--rw-r--r--   0 briford    (501) staff       (20)      543 2024-03-28 17:23:43.000000 sageworks-0.5.4/src/sageworks/core/transforms/data_loaders/light/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)     3011 2024-03-28 17:23:43.000000 sageworks-0.5.4/src/sageworks/core/transforms/data_loaders/light/csv_to_data_source.py
--rw-r--r--   0 briford    (501) staff       (20)     2927 2024-03-28 17:23:43.000000 sageworks-0.5.4/src/sageworks/core/transforms/data_loaders/light/json_to_data_source.py
--rw-r--r--   0 briford    (501) staff       (20)     4225 2024-03-28 17:23:43.000000 sageworks-0.5.4/src/sageworks/core/transforms/data_loaders/light/s3_to_data_source_light.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.703603 sageworks-0.5.4/src/sageworks/core/transforms/data_to_data/
--rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.5.4/src/sageworks/core/transforms/data_to_data/__init__.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.703715 sageworks-0.5.4/src/sageworks/core/transforms/data_to_data/heavy/
--rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.5.4/src/sageworks/core/transforms/data_to_data/heavy/__init__.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.703824 sageworks-0.5.4/src/sageworks/core/transforms/data_to_data/heavy/emr/
--rw-r--r--   0 briford    (501) staff       (20)       68 2024-01-10 18:45:51.000000 sageworks-0.5.4/src/sageworks/core/transforms/data_to_data/heavy/emr/Readme.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.703962 sageworks-0.5.4/src/sageworks/core/transforms/data_to_data/heavy/glue/
--rw-r--r--   0 briford    (501) staff       (20)       48 2024-01-10 18:45:51.000000 sageworks-0.5.4/src/sageworks/core/transforms/data_to_data/heavy/glue/Readme.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.704335 sageworks-0.5.4/src/sageworks/core/transforms/data_to_data/light/
--rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.5.4/src/sageworks/core/transforms/data_to_data/light/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)     2237 2024-03-27 20:40:53.000000 sageworks-0.5.4/src/sageworks/core/transforms/data_to_data/light/clean_data.py
--rw-r--r--   0 briford    (501) staff       (20)     2687 2024-03-27 20:40:53.000000 sageworks-0.5.4/src/sageworks/core/transforms/data_to_data/light/data_to_data_light.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.704481 sageworks-0.5.4/src/sageworks/core/transforms/data_to_features/
--rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.5.4/src/sageworks/core/transforms/data_to_features/__init__.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.704582 sageworks-0.5.4/src/sageworks/core/transforms/data_to_features/heavy/
--rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.5.4/src/sageworks/core/transforms/data_to_features/heavy/__init__.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.704777 sageworks-0.5.4/src/sageworks/core/transforms/data_to_features/heavy/chunk/
--rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.5.4/src/sageworks/core/transforms/data_to_features/heavy/chunk/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)     4551 2024-03-28 17:23:43.000000 sageworks-0.5.4/src/sageworks/core/transforms/data_to_features/heavy/chunk/data_to_features_chunk.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.704931 sageworks-0.5.4/src/sageworks/core/transforms/data_to_features/heavy/emr/
--rw-r--r--   0 briford    (501) staff       (20)       68 2024-01-10 18:45:51.000000 sageworks-0.5.4/src/sageworks/core/transforms/data_to_features/heavy/emr/Readme.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.705069 sageworks-0.5.4/src/sageworks/core/transforms/data_to_features/heavy/glue/
--rw-r--r--   0 briford    (501) staff       (20)       48 2024-01-10 18:45:51.000000 sageworks-0.5.4/src/sageworks/core/transforms/data_to_features/heavy/glue/Readme.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.705209 sageworks-0.5.4/src/sageworks/core/transforms/data_to_features/heavy/storage/
--rw-r--r--   0 briford    (501) staff       (20)     6702 2024-03-28 17:23:43.000000 sageworks-0.5.4/src/sageworks/core/transforms/data_to_features/heavy/storage/data_to_features_heavy_old.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.705591 sageworks-0.5.4/src/sageworks/core/transforms/data_to_features/light/
--rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.5.4/src/sageworks/core/transforms/data_to_features/light/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)     3827 2024-03-28 17:23:43.000000 sageworks-0.5.4/src/sageworks/core/transforms/data_to_features/light/data_to_features_light.py
--rw-r--r--   0 briford    (501) staff       (20)     4778 2024-03-28 17:23:43.000000 sageworks-0.5.4/src/sageworks/core/transforms/data_to_features/light/molecular_descriptors.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.705743 sageworks-0.5.4/src/sageworks/core/transforms/features_to_features/
--rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.5.4/src/sageworks/core/transforms/features_to_features/__init__.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.661755 sageworks-0.5.4/src/sageworks/core/transforms/features_to_features/heavy/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.705841 sageworks-0.5.4/src/sageworks/core/transforms/features_to_features/heavy/emr/
--rw-r--r--   0 briford    (501) staff       (20)       68 2024-01-10 18:45:51.000000 sageworks-0.5.4/src/sageworks/core/transforms/features_to_features/heavy/emr/Readme.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.705980 sageworks-0.5.4/src/sageworks/core/transforms/features_to_features/heavy/glue/
--rw-r--r--   0 briford    (501) staff       (20)       48 2024-01-10 18:45:51.000000 sageworks-0.5.4/src/sageworks/core/transforms/features_to_features/heavy/glue/Readme.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.706212 sageworks-0.5.4/src/sageworks/core/transforms/features_to_model/
--rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.5.4/src/sageworks/core/transforms/features_to_model/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)    13050 2024-03-28 17:23:43.000000 sageworks-0.5.4/src/sageworks/core/transforms/features_to_model/features_to_model.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.706477 sageworks-0.5.4/src/sageworks/core/transforms/features_to_model/light_model_harness/
--rw-r--r--   0 briford    (501) staff       (20)       19 2024-02-27 23:40:48.000000 sageworks-0.5.4/src/sageworks/core/transforms/features_to_model/light_model_harness/requirements.txt
--rw-r--r--   0 briford    (501) staff       (20)    10806 2024-03-28 17:23:43.000000 sageworks-0.5.4/src/sageworks/core/transforms/features_to_model/light_model_harness/xgb_model.template
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.706730 sageworks-0.5.4/src/sageworks/core/transforms/model_to_endpoint/
--rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.5.4/src/sageworks/core/transforms/model_to_endpoint/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)     8185 2024-03-28 17:23:43.000000 sageworks-0.5.4/src/sageworks/core/transforms/model_to_endpoint/model_to_endpoint.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.707585 sageworks-0.5.4/src/sageworks/core/transforms/pandas_transforms/
--rw-r--r--   0 briford    (501) staff       (20)      894 2024-03-28 17:23:43.000000 sageworks-0.5.4/src/sageworks/core/transforms/pandas_transforms/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)     3615 2024-03-28 17:23:43.000000 sageworks-0.5.4/src/sageworks/core/transforms/pandas_transforms/data_to_pandas.py
--rw-r--r--   0 briford    (501) staff       (20)     3445 2024-03-28 17:23:43.000000 sageworks-0.5.4/src/sageworks/core/transforms/pandas_transforms/features_to_pandas.py
--rw-r--r--   0 briford    (501) staff       (20)     8604 2024-03-30 22:43:51.000000 sageworks-0.5.4/src/sageworks/core/transforms/pandas_transforms/pandas_to_data.py
--rw-r--r--   0 briford    (501) staff       (20)    18139 2024-03-30 22:43:51.000000 sageworks-0.5.4/src/sageworks/core/transforms/pandas_transforms/pandas_to_features.py
--rw-r--r--   0 briford    (501) staff       (20)     4440 2024-03-28 17:23:43.000000 sageworks-0.5.4/src/sageworks/core/transforms/pandas_transforms/pandas_to_features_chunked.py
--rw-r--r--   0 briford    (501) staff       (20)     5391 2024-03-28 17:23:43.000000 sageworks-0.5.4/src/sageworks/core/transforms/transform.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.707750 sageworks-0.5.4/src/sageworks/experiments/
--rw-r--r--   0 briford    (501) staff       (20)    10658 2024-03-28 17:23:43.000000 sageworks-0.5.4/src/sageworks/experiments/view_manager.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.708028 sageworks-0.5.4/src/sageworks/repl/
--rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.5.4/src/sageworks/repl/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)    14538 2024-03-30 22:43:51.000000 sageworks-0.5.4/src/sageworks/repl/sageworks_shell.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.708309 sageworks-0.5.4/src/sageworks/resources/
--rw-r--r--   0 briford    (501) staff       (20)      361 2024-01-23 15:36:53.000000 sageworks-0.5.4/src/sageworks/resources/open_source_api.key
--rw-r--r--   0 briford    (501) staff       (20)      272 2024-01-10 18:45:51.000000 sageworks-0.5.4/src/sageworks/resources/signature_verify_pub.pem
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.712096 sageworks-0.5.4/src/sageworks/utils/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-12-24 17:18:24.000000 sageworks-0.5.4/src/sageworks/utils/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)    15587 2024-03-30 22:43:51.000000 sageworks-0.5.4/src/sageworks/utils/aws_utils.py
--rw-r--r--   0 briford    (501) staff       (20)     5455 2024-03-28 17:23:43.000000 sageworks-0.5.4/src/sageworks/utils/cache.py
--rw-r--r--   0 briford    (501) staff       (20)      722 2024-03-28 17:23:43.000000 sageworks-0.5.4/src/sageworks/utils/chem_utils.py
--rw-r--r--   0 briford    (501) staff       (20)    16234 2024-03-28 17:23:43.000000 sageworks-0.5.4/src/sageworks/utils/config_manager.py
--rw-r--r--   0 briford    (501) staff       (20)     7392 2024-03-28 17:23:43.000000 sageworks-0.5.4/src/sageworks/utils/dashboard_metrics.py
--rw-r--r--   0 briford    (501) staff       (20)     4194 2024-03-30 22:43:51.000000 sageworks-0.5.4/src/sageworks/utils/datetime_utils.py
--rw-r--r--   0 briford    (501) staff       (20)     5292 2024-03-28 17:23:43.000000 sageworks-0.5.4/src/sageworks/utils/df_to_endpoint.py
--rw-r--r--   0 briford    (501) staff       (20)     1681 2024-03-28 17:23:43.000000 sageworks-0.5.4/src/sageworks/utils/docker_utils.py
--rw-r--r--   0 briford    (501) staff       (20)     2866 2024-03-27 20:43:31.000000 sageworks-0.5.4/src/sageworks/utils/ecs_info.py
--rw-r--r--   0 briford    (501) staff       (20)     7657 2024-03-28 17:23:43.000000 sageworks-0.5.4/src/sageworks/utils/endpoint_metrics.py
--rw-r--r--   0 briford    (501) staff       (20)     3097 2024-03-28 17:23:43.000000 sageworks-0.5.4/src/sageworks/utils/endpoint_utils.py
--rw-r--r--   0 briford    (501) staff       (20)     6979 2024-03-28 17:23:43.000000 sageworks-0.5.4/src/sageworks/utils/extract_model_artifact.py
--rw-r--r--   0 briford    (501) staff       (20)     1131 2024-03-28 17:23:43.000000 sageworks-0.5.4/src/sageworks/utils/glue_utils.py
--rw-r--r--   0 briford    (501) staff       (20)     5757 2024-03-28 17:23:43.000000 sageworks-0.5.4/src/sageworks/utils/license_manager.py
--rw-r--r--   0 briford    (501) staff       (20)     1439 2024-03-28 17:32:59.000000 sageworks-0.5.4/src/sageworks/utils/markdown_utils.py
--rw-r--r--   0 briford    (501) staff       (20)    13241 2024-03-28 17:23:43.000000 sageworks-0.5.4/src/sageworks/utils/pandas_utils.py
--rw-r--r--   0 briford    (501) staff       (20)    12681 2024-04-02 13:06:54.000000 sageworks-0.5.4/src/sageworks/utils/plugin_manager.py
--rw-r--r--   0 briford    (501) staff       (20)     9533 2024-03-30 22:43:51.000000 sageworks-0.5.4/src/sageworks/utils/redis_cache.py
--rw-r--r--   0 briford    (501) staff       (20)     4166 2024-03-28 17:23:43.000000 sageworks-0.5.4/src/sageworks/utils/repl_utils.py
--rw-r--r--   0 briford    (501) staff       (20)     2089 2024-03-28 17:23:43.000000 sageworks-0.5.4/src/sageworks/utils/s3_utils.py
--rw-r--r--   0 briford    (501) staff       (20)     2163 2024-03-28 17:23:43.000000 sageworks-0.5.4/src/sageworks/utils/sageworks_cache.py
--rw-r--r--   0 briford    (501) staff       (20)     3474 2024-03-28 17:23:43.000000 sageworks-0.5.4/src/sageworks/utils/sageworks_event_bridge.py
--rw-r--r--   0 briford    (501) staff       (20)     5359 2024-03-28 17:23:43.000000 sageworks-0.5.4/src/sageworks/utils/sageworks_logging.py
--rw-r--r--   0 briford    (501) staff       (20)     2120 2024-03-28 17:23:43.000000 sageworks-0.5.4/src/sageworks/utils/sageworks_sqs.py
--rw-r--r--   0 briford    (501) staff       (20)     1108 2024-01-10 18:45:51.000000 sageworks-0.5.4/src/sageworks/utils/symbols.py
--rw-r--r--   0 briford    (501) staff       (20)     6414 2024-03-28 17:23:43.000000 sageworks-0.5.4/src/sageworks/utils/test_data_generator.py
--rw-r--r--   0 briford    (501) staff       (20)     2092 2024-03-27 20:43:31.000000 sageworks-0.5.4/src/sageworks/utils/trace_calls.py
--rw-r--r--   0 briford    (501) staff       (20)     1470 2024-03-28 17:23:43.000000 sageworks-0.5.4/src/sageworks/utils/type_abbrev.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.712991 sageworks-0.5.4/src/sageworks/views/
--rw-r--r--   0 briford    (501) staff       (20)     3318 2024-03-30 22:43:51.000000 sageworks-0.5.4/src/sageworks/views/artifacts_text_view.py
--rw-r--r--   0 briford    (501) staff       (20)     7008 2024-03-30 22:43:51.000000 sageworks-0.5.4/src/sageworks/views/artifacts_web_view.py
--rw-r--r--   0 briford    (501) staff       (20)     3158 2024-03-30 22:43:51.000000 sageworks-0.5.4/src/sageworks/views/data_source_web_view.py
--rw-r--r--   0 briford    (501) staff       (20)     2150 2024-03-30 22:43:51.000000 sageworks-0.5.4/src/sageworks/views/endpoint_web_view.py
--rw-r--r--   0 briford    (501) staff       (20)     3206 2024-03-30 22:43:51.000000 sageworks-0.5.4/src/sageworks/views/feature_set_web_view.py
--rw-r--r--   0 briford    (501) staff       (20)     2029 2024-03-30 22:43:51.000000 sageworks-0.5.4/src/sageworks/views/model_web_view.py
--rw-r--r--   0 briford    (501) staff       (20)     1092 2024-03-28 17:23:43.000000 sageworks-0.5.4/src/sageworks/views/view.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.715432 sageworks-0.5.4/src/sageworks/web_components/
--rw-r--r--   0 briford    (501) staff       (20)      837 2023-12-24 17:18:24.000000 sageworks-0.5.4/src/sageworks/web_components/color_maps.py
--rw-r--r--   0 briford    (501) staff       (20)     4902 2024-03-31 15:44:39.000000 sageworks-0.5.4/src/sageworks/web_components/component_interface.py
--rw-r--r--   0 briford    (501) staff       (20)     3521 2024-03-30 22:43:51.000000 sageworks-0.5.4/src/sageworks/web_components/confusion_matrix.py
--rw-r--r--   0 briford    (501) staff       (20)     5850 2024-03-30 22:43:51.000000 sageworks-0.5.4/src/sageworks/web_components/correlation_matrix.py
--rw-r--r--   0 briford    (501) staff       (20)     2970 2024-03-30 22:43:51.000000 sageworks-0.5.4/src/sageworks/web_components/dashboard_metric_plots.py
--rw-r--r--   0 briford    (501) staff       (20)     9328 2024-04-02 16:53:34.000000 sageworks-0.5.4/src/sageworks/web_components/data_details_markdown.py
--rw-r--r--   0 briford    (501) staff       (20)     4558 2024-04-02 16:53:34.000000 sageworks-0.5.4/src/sageworks/web_components/endpoint_details.py
--rw-r--r--   0 briford    (501) staff       (20)     3064 2024-03-30 22:43:51.000000 sageworks-0.5.4/src/sageworks/web_components/endpoint_metric_plots.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.716035 sageworks-0.5.4/src/sageworks/web_components/experiments/
--rw-r--r--   0 briford    (501) staff       (20)     1633 2024-03-28 17:23:43.000000 sageworks-0.5.4/src/sageworks/web_components/experiments/compound_details.py
--rw-r--r--   0 briford    (501) staff       (20)     1183 2024-03-28 17:23:43.000000 sageworks-0.5.4/src/sageworks/web_components/experiments/histogram.py
--rw-r--r--   0 briford    (501) staff       (20)     3680 2024-03-28 17:23:43.000000 sageworks-0.5.4/src/sageworks/web_components/experiments/outlier_plot.py
--rw-r--r--   0 briford    (501) staff       (20)     2279 2024-03-28 17:23:43.000000 sageworks-0.5.4/src/sageworks/web_components/experiments/scatter_plot.py
--rw-r--r--   0 briford    (501) staff       (20)      838 2024-03-28 17:23:43.000000 sageworks-0.5.4/src/sageworks/web_components/line_chart.py
--rw-r--r--   0 briford    (501) staff       (20)     8731 2024-04-03 14:14:37.000000 sageworks-0.5.4/src/sageworks/web_components/model_details.py
--rw-r--r--   0 briford    (501) staff       (20)     2270 2024-03-30 22:43:51.000000 sageworks-0.5.4/src/sageworks/web_components/model_plot.py
--rw-r--r--   0 briford    (501) staff       (20)     6737 2024-04-03 18:50:52.000000 sageworks-0.5.4/src/sageworks/web_components/plugin_interface.py
--rw-r--r--   0 briford    (501) staff       (20)     2941 2024-03-30 22:43:51.000000 sageworks-0.5.4/src/sageworks/web_components/regression_plot.py
--rw-r--r--   0 briford    (501) staff       (20)     6535 2024-03-28 17:23:43.000000 sageworks-0.5.4/src/sageworks/web_components/table.py
--rw-r--r--   0 briford    (501) staff       (20)     5181 2024-03-30 22:43:51.000000 sageworks-0.5.4/src/sageworks/web_components/violin_plots.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.720468 sageworks-0.5.4/src/sageworks.egg-info/
--rw-r--r--   0 briford    (501) staff       (20)     4118 2024-04-03 19:02:27.000000 sageworks-0.5.4/src/sageworks.egg-info/PKG-INFO
--rw-r--r--   0 briford    (501) staff       (20)    17380 2024-04-03 19:02:27.000000 sageworks-0.5.4/src/sageworks.egg-info/SOURCES.txt
--rw-r--r--   0 briford    (501) staff       (20)        1 2024-04-03 19:02:27.000000 sageworks-0.5.4/src/sageworks.egg-info/dependency_links.txt
--rw-r--r--   0 briford    (501) staff       (20)       74 2024-04-03 19:02:27.000000 sageworks-0.5.4/src/sageworks.egg-info/entry_points.txt
--rw-r--r--   0 briford    (501) staff       (20)      408 2024-04-03 19:02:27.000000 sageworks-0.5.4/src/sageworks.egg-info/requires.txt
--rw-r--r--   0 briford    (501) staff       (20)       10 2024-04-03 19:02:27.000000 sageworks-0.5.4/src/sageworks.egg-info/top_level.txt
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.716911 sageworks-0.5.4/tests/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.717492 sageworks-0.5.4/tests/artifacts/
--rw-r--r--   0 briford    (501) staff       (20)     1548 2024-03-30 19:27:28.000000 sageworks-0.5.4/tests/artifacts/data_source_tests.py
--rw-r--r--   0 briford    (501) staff       (20)     2442 2024-03-28 17:23:43.000000 sageworks-0.5.4/tests/artifacts/endpoint_tests.py
--rw-r--r--   0 briford    (501) staff       (20)     1160 2024-03-28 17:23:43.000000 sageworks-0.5.4/tests/artifacts/feature_set_tests.py
--rw-r--r--   0 briford    (501) staff       (20)      805 2024-03-28 17:23:43.000000 sageworks-0.5.4/tests/artifacts/model_tests.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.717764 sageworks-0.5.4/tests/aws_account/
--rw-r--r--   0 briford    (501) staff       (20)      962 2023-12-24 17:18:24.000000 sageworks-0.5.4/tests/aws_account/aws_account_clamp_tests.py
--rw-r--r--   0 briford    (501) staff       (20)      642 2023-12-24 17:18:24.000000 sageworks-0.5.4/tests/aws_account/aws_service_broker_tests.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.718595 sageworks-0.5.4/tests/connectors/
--rw-r--r--   0 briford    (501) staff       (20)      725 2024-03-28 17:23:43.000000 sageworks-0.5.4/tests/connectors/data_catalog.py
--rw-r--r--   0 briford    (501) staff       (20)      737 2024-03-28 17:23:43.000000 sageworks-0.5.4/tests/connectors/endpoints.py
--rw-r--r--   0 briford    (501) staff       (20)      702 2024-03-28 17:23:43.000000 sageworks-0.5.4/tests/connectors/feature_store.py
--rw-r--r--   0 briford    (501) staff       (20)      644 2024-03-28 17:23:43.000000 sageworks-0.5.4/tests/connectors/glue_jobs.py
--rw-r--r--   0 briford    (501) staff       (20)      799 2024-03-28 17:23:43.000000 sageworks-0.5.4/tests/connectors/model_registry.py
--rw-r--r--   0 briford    (501) staff       (20)     1008 2024-03-28 17:23:43.000000 sageworks-0.5.4/tests/connectors/s3_bucket.py
--rw-r--r--   0 briford    (501) staff       (20)     5408 2024-03-28 17:23:43.000000 sageworks-0.5.4/tests/create_aqsol_artifacts.py
--rw-r--r--   0 briford    (501) staff       (20)     3217 2024-03-28 17:23:43.000000 sageworks-0.5.4/tests/create_basic_test_artifacts.py
--rw-r--r--   0 briford    (501) staff       (20)      870 2024-03-28 17:23:43.000000 sageworks-0.5.4/tests/create_realtime_endpoint.py
--rw-r--r--   0 briford    (501) staff       (20)     2379 2024-03-28 17:23:43.000000 sageworks-0.5.4/tests/create_training_adjusted_artifacts.py
--rw-r--r--   0 briford    (501) staff       (20)     2096 2024-03-28 17:23:43.000000 sageworks-0.5.4/tests/create_wine_artifacts.py
--rw-r--r--   0 briford    (501) staff       (20)     4310 2024-03-28 17:23:43.000000 sageworks-0.5.4/tests/delete_test_artifacts.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.718727 sageworks-0.5.4/tests/plugin_tests/
--rw-r--r--   0 briford    (501) staff       (20)     1888 2024-03-30 22:43:51.000000 sageworks-0.5.4/tests/plugin_tests/crashing_plugin.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.719001 sageworks-0.5.4/tests/specific/
--rw-r--r--   0 briford    (501) staff       (20)      639 2024-03-28 17:23:43.000000 sageworks-0.5.4/tests/specific/capital_tests.py
--rw-r--r--   0 briford    (501) staff       (20)     1513 2024-03-28 17:23:43.000000 sageworks-0.5.4/tests/specific/deletion_tests.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.719869 sageworks-0.5.4/tests/transforms/
--rw-r--r--   0 briford    (501) staff       (20)      592 2024-03-28 17:23:43.000000 sageworks-0.5.4/tests/transforms/data_to_data_tests.py
--rw-r--r--   0 briford    (501) staff       (20)     1025 2024-03-28 17:23:43.000000 sageworks-0.5.4/tests/transforms/data_to_features_tests.py
--rw-r--r--   0 briford    (501) staff       (20)      773 2024-03-28 17:23:43.000000 sageworks-0.5.4/tests/transforms/features_to_model_tests.py
--rw-r--r--   0 briford    (501) staff       (20)     4864 2024-03-28 17:23:43.000000 sageworks-0.5.4/tests/transforms/model_metrics_tests.py
--rw-r--r--   0 briford    (501) staff       (20)      795 2024-03-28 17:23:43.000000 sageworks-0.5.4/tests/transforms/model_to_endpoint_tests.py
--rw-r--r--   0 briford    (501) staff       (20)      633 2024-03-27 20:40:53.000000 sageworks-0.5.4/tests/transforms/pandas_to_data_tests.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.720255 sageworks-0.5.4/tests/web_components/
--rw-r--r--   0 briford    (501) staff       (20)      679 2024-03-30 22:43:51.000000 sageworks-0.5.4/tests/web_components/confusion_matrix_test.py
--rw-r--r--   0 briford    (501) staff       (20)      675 2024-03-30 22:43:51.000000 sageworks-0.5.4/tests/web_components/correlation_matrix_test.py
--rw-r--r--   0 briford    (501) staff       (20)     5210 2024-03-30 22:43:51.000000 sageworks-0.5.4/tests/web_components/plugin_interface_test.py
--rw-r--r--   0 briford    (501) staff       (20)     1115 2024-03-27 20:43:31.000000 sageworks-0.5.4/tox.ini
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 16:58:06.573610 sageworks-0.6.0/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 16:58:06.469787 sageworks-0.6.0/.github/
+-rw-r--r--   0 briford    (501) staff       (20)     1338 2024-03-28 17:23:43.000000 sageworks-0.6.0/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 briford    (501) staff       (20)      499 2023-12-24 17:18:24.000000 sageworks-0.6.0/.github/dependabot.yml
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 16:58:06.470269 sageworks-0.6.0/.github/workflows/
+-rw-r--r--   0 briford    (501) staff       (20)      598 2024-01-10 18:45:51.000000 sageworks-0.6.0/.github/workflows/deploy-docs.yml
+-rw-r--r--   0 briford    (501) staff       (20)      556 2024-01-23 15:36:53.000000 sageworks-0.6.0/.github/workflows/python-lint.yml
+-rw-r--r--   0 briford    (501) staff       (20)     2008 2023-12-24 17:18:24.000000 sageworks-0.6.0/.gitignore
+-rw-r--r--   0 briford    (501) staff       (20)      791 2024-04-16 15:58:18.000000 sageworks-0.6.0/CONTRIBUTING.md
+-rw-r--r--   0 briford    (501) staff       (20)      102 2024-03-28 17:23:43.000000 sageworks-0.6.0/Dockerfile
+-rw-r--r--   0 briford    (501) staff       (20)     1080 2024-03-28 17:23:43.000000 sageworks-0.6.0/LICENSE
+-rw-r--r--   0 briford    (501) staff       (20)     1426 2023-12-24 17:18:24.000000 sageworks-0.6.0/Makefile
+-rw-r--r--   0 briford    (501) staff       (20)     4117 2024-04-23 16:58:06.573547 sageworks-0.6.0/PKG-INFO
+-rw-r--r--   0 briford    (501) staff       (20)     2694 2024-04-16 15:58:18.000000 sageworks-0.6.0/README.md
+-rw-r--r--   0 briford    (501) staff       (20)      463 2023-12-24 17:18:24.000000 sageworks-0.6.0/SECURITY.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 16:58:06.458821 sageworks-0.6.0/applications/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 16:58:06.472319 sageworks-0.6.0/applications/aws_dashboard/
+-rw-r--r--   0 briford    (501) staff       (20)     1071 2024-04-16 15:58:18.000000 sageworks-0.6.0/applications/aws_dashboard/Dockerfile
+-rw-r--r--   0 briford    (501) staff       (20)      331 2024-03-28 17:23:43.000000 sageworks-0.6.0/applications/aws_dashboard/Dockerfile_plugins
+-rw-r--r--   0 briford    (501) staff       (20)      841 2024-01-10 18:45:51.000000 sageworks-0.6.0/applications/aws_dashboard/README.md
+-rw-r--r--   0 briford    (501) staff       (20)     1526 2024-04-09 14:37:33.000000 sageworks-0.6.0/applications/aws_dashboard/app.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 16:58:06.473741 sageworks-0.6.0/applications/aws_dashboard/assets/
+-rw-r--r--   0 briford    (501) staff       (20)   232839 2024-04-06 16:51:44.000000 sageworks-0.6.0/applications/aws_dashboard/assets/bootstrap_darkly.min.css
+-rw-r--r--   0 briford    (501) staff       (20)    14995 2024-04-06 16:51:44.000000 sageworks-0.6.0/applications/aws_dashboard/assets/default.css
+-rw-r--r--   0 briford    (501) staff       (20)    10375 2024-04-16 15:58:18.000000 sageworks-0.6.0/applications/aws_dashboard/assets/favicon.ico
+-rw-r--r--   0 briford    (501) staff       (20)      732 2023-12-24 17:18:24.000000 sageworks-0.6.0/applications/aws_dashboard/assets/trash.png
+-rwxr-xr-x   0 briford    (501) staff       (20)      637 2024-04-06 16:51:44.000000 sageworks-0.6.0/applications/aws_dashboard/dashboard
+-rw-r--r--   0 briford    (501) staff       (20)      205 2023-12-24 17:18:24.000000 sageworks-0.6.0/applications/aws_dashboard/nginx.conf
+-rw-r--r--   0 briford    (501) staff       (20)      684 2024-03-28 17:23:43.000000 sageworks-0.6.0/applications/aws_dashboard/open_source_config.json
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 16:58:06.458749 sageworks-0.6.0/applications/aws_dashboard/pages/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 16:58:06.474335 sageworks-0.6.0/applications/aws_dashboard/pages/data_sources/
+-rw-r--r--   0 briford    (501) staff       (20)    11700 2024-04-16 15:58:18.000000 sageworks-0.6.0/applications/aws_dashboard/pages/data_sources/callbacks.py
+-rw-r--r--   0 briford    (501) staff       (20)     2756 2024-03-28 17:23:43.000000 sageworks-0.6.0/applications/aws_dashboard/pages/data_sources/layout.py
+-rw-r--r--   0 briford    (501) staff       (20)     2555 2024-03-28 17:23:43.000000 sageworks-0.6.0/applications/aws_dashboard/pages/data_sources/page.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 16:58:06.474937 sageworks-0.6.0/applications/aws_dashboard/pages/endpoints/
+-rw-r--r--   0 briford    (501) staff       (20)     4212 2024-04-16 15:58:18.000000 sageworks-0.6.0/applications/aws_dashboard/pages/endpoints/callbacks.py
+-rw-r--r--   0 briford    (501) staff       (20)     2677 2024-04-16 15:58:18.000000 sageworks-0.6.0/applications/aws_dashboard/pages/endpoints/layout.py
+-rw-r--r--   0 briford    (501) staff       (20)     2442 2024-04-16 15:58:18.000000 sageworks-0.6.0/applications/aws_dashboard/pages/endpoints/page.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 16:58:06.475584 sageworks-0.6.0/applications/aws_dashboard/pages/feature_sets/
+-rw-r--r--   0 briford    (501) staff       (20)    11614 2024-04-16 15:58:18.000000 sageworks-0.6.0/applications/aws_dashboard/pages/feature_sets/callbacks.py
+-rw-r--r--   0 briford    (501) staff       (20)     2438 2024-03-28 17:23:43.000000 sageworks-0.6.0/applications/aws_dashboard/pages/feature_sets/layout.py
+-rw-r--r--   0 briford    (501) staff       (20)     2505 2024-03-28 17:23:43.000000 sageworks-0.6.0/applications/aws_dashboard/pages/feature_sets/page.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 16:58:06.476260 sageworks-0.6.0/applications/aws_dashboard/pages/main/
+-rw-r--r--   0 briford    (501) staff       (20)     4899 2024-04-06 16:51:44.000000 sageworks-0.6.0/applications/aws_dashboard/pages/main/callbacks.py
+-rw-r--r--   0 briford    (501) staff       (20)     2899 2024-03-28 17:23:43.000000 sageworks-0.6.0/applications/aws_dashboard/pages/main/layout.py
+-rw-r--r--   0 briford    (501) staff       (20)     1844 2024-03-28 17:23:43.000000 sageworks-0.6.0/applications/aws_dashboard/pages/main/page.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 16:58:06.477005 sageworks-0.6.0/applications/aws_dashboard/pages/models/
+-rw-r--r--   0 briford    (501) staff       (20)     4446 2024-04-16 15:58:18.000000 sageworks-0.6.0/applications/aws_dashboard/pages/models/callbacks.py
+-rw-r--r--   0 briford    (501) staff       (20)     2132 2024-04-16 15:58:18.000000 sageworks-0.6.0/applications/aws_dashboard/pages/models/layout.py
+-rw-r--r--   0 briford    (501) staff       (20)     2136 2024-04-16 15:58:18.000000 sageworks-0.6.0/applications/aws_dashboard/pages/models/page.py
+-rw-r--r--   0 briford    (501) staff       (20)      394 2024-04-06 16:51:44.000000 sageworks-0.6.0/applications/aws_dashboard/requirements.txt
+-rw-r--r--   0 briford    (501) staff       (20)      457 2023-12-24 17:18:24.000000 sageworks-0.6.0/applications/aws_dashboard/supervisord.conf
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 16:58:06.458874 sageworks-0.6.0/applications/experiments/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 16:58:06.478367 sageworks-0.6.0/applications/experiments/compound_explorer/
+-rw-r--r--   0 briford    (501) staff       (20)      181 2023-12-24 17:18:24.000000 sageworks-0.6.0/applications/experiments/compound_explorer/Dockerfile
+-rw-r--r--   0 briford    (501) staff       (20)      360 2023-12-24 17:18:24.000000 sageworks-0.6.0/applications/experiments/compound_explorer/README.md
+-rw-r--r--   0 briford    (501) staff       (20)     3082 2024-04-06 16:51:44.000000 sageworks-0.6.0/applications/experiments/compound_explorer/app.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 16:58:06.478891 sageworks-0.6.0/applications/experiments/compound_explorer/assets/
+-rw-r--r--   0 briford    (501) staff       (20)    12861 2023-12-24 17:18:24.000000 sageworks-0.6.0/applications/experiments/compound_explorer/assets/custom.css
+-rw-r--r--   0 briford    (501) staff       (20)      318 2023-12-24 17:18:24.000000 sageworks-0.6.0/applications/experiments/compound_explorer/assets/favicon.ico
+-rw-r--r--   0 briford    (501) staff       (20)     7678 2024-04-16 15:58:18.000000 sageworks-0.6.0/applications/experiments/compound_explorer/callbacks.py
+-rw-r--r--   0 briford    (501) staff       (20)     4860 2024-03-28 17:23:43.000000 sageworks-0.6.0/applications/experiments/compound_explorer/layout.py
+-rw-r--r--   0 briford    (501) staff       (20)       94 2023-12-24 17:18:24.000000 sageworks-0.6.0/applications/experiments/compound_explorer/requirements.txt
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 16:58:06.479569 sageworks-0.6.0/aws_setup/
+-rw-r--r--   0 briford    (501) staff       (20)     3582 2024-03-28 17:23:43.000000 sageworks-0.6.0/aws_setup/aws_account_check.py
+-rw-r--r--   0 briford    (501) staff       (20)     1403 2024-03-28 17:23:43.000000 sageworks-0.6.0/aws_setup/aws_identity_check.py
+-rw-r--r--   0 briford    (501) staff       (20)     2629 2024-03-28 17:23:43.000000 sageworks-0.6.0/aws_setup/build_ml_pipeline.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 16:58:06.479989 sageworks-0.6.0/aws_setup/event_bridge/
+-rw-r--r--   0 briford    (501) staff       (20)       60 2023-12-24 17:18:24.000000 sageworks-0.6.0/aws_setup/event_bridge/Readme.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 16:58:06.480664 sageworks-0.6.0/aws_setup/event_bridge/dynamic_docker/
+-rw-r--r--   0 briford    (501) staff       (20)       60 2023-12-24 17:18:24.000000 sageworks-0.6.0/aws_setup/event_bridge/dynamic_docker/Readme.md
+-rw-r--r--   0 briford    (501) staff       (20)     1007 2023-12-24 17:18:24.000000 sageworks-0.6.0/aws_setup/event_bridge/dynamic_docker/app.py
+-rw-r--r--   0 briford    (501) staff       (20)     2567 2023-12-24 17:18:24.000000 sageworks-0.6.0/aws_setup/event_bridge/dynamic_docker/cdk.json
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 16:58:06.480894 sageworks-0.6.0/aws_setup/event_bridge/dynamic_docker/lambda/
+-rw-r--r--   0 briford    (501) staff       (20)     1812 2024-01-10 18:45:51.000000 sageworks-0.6.0/aws_setup/event_bridge/dynamic_docker/lambda/lambda_replace_task.py
+-rw-r--r--   0 briford    (501) staff       (20)     2599 2024-03-27 20:43:31.000000 sageworks-0.6.0/aws_setup/event_bridge/dynamic_docker/sageworks_image_update_stack.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 16:58:06.482052 sageworks-0.6.0/aws_setup/sageworks_core/
+-rw-r--r--   0 briford    (501) staff       (20)      119 2023-12-24 17:18:24.000000 sageworks-0.6.0/aws_setup/sageworks_core/.gitignore
+-rw-r--r--   0 briford    (501) staff       (20)     1028 2023-12-24 17:18:24.000000 sageworks-0.6.0/aws_setup/sageworks_core/README.md
+-rw-r--r--   0 briford    (501) staff       (20)     1403 2024-03-28 17:23:43.000000 sageworks-0.6.0/aws_setup/sageworks_core/app.py
+-rw-r--r--   0 briford    (501) staff       (20)     1998 2023-12-24 17:18:24.000000 sageworks-0.6.0/aws_setup/sageworks_core/cdk.json
+-rw-r--r--   0 briford    (501) staff       (20)       14 2023-12-24 17:18:24.000000 sageworks-0.6.0/aws_setup/sageworks_core/requirements-dev.txt
+-rw-r--r--   0 briford    (501) staff       (20)       53 2024-01-10 18:45:51.000000 sageworks-0.6.0/aws_setup/sageworks_core/requirements.txt
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 16:58:06.482326 sageworks-0.6.0/aws_setup/sageworks_core/sageworks_core/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.0/aws_setup/sageworks_core/sageworks_core/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)    23575 2024-03-28 17:23:43.000000 sageworks-0.6.0/aws_setup/sageworks_core/sageworks_core/sageworks_core_stack.py
+-rw-r--r--   0 briford    (501) staff       (20)      437 2023-12-24 17:18:24.000000 sageworks-0.6.0/aws_setup/sageworks_core/source.bat
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 16:58:06.482736 sageworks-0.6.0/aws_setup/sageworks_core/tests/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-12-24 17:18:24.000000 sageworks-0.6.0/aws_setup/sageworks_core/tests/__init__.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 16:58:06.482929 sageworks-0.6.0/aws_setup/sageworks_core/tests/unit/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-12-24 17:18:24.000000 sageworks-0.6.0/aws_setup/sageworks_core/tests/unit/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)      720 2023-12-24 17:18:24.000000 sageworks-0.6.0/aws_setup/sageworks_core/tests/unit/test_sageworks_sandbox_stack.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 16:58:06.484378 sageworks-0.6.0/aws_setup/sageworks_dashboard_full/
+-rw-r--r--   0 briford    (501) staff       (20)      119 2023-12-24 17:18:24.000000 sageworks-0.6.0/aws_setup/sageworks_dashboard_full/.gitignore
+-rw-r--r--   0 briford    (501) staff       (20)     1778 2024-03-28 17:23:43.000000 sageworks-0.6.0/aws_setup/sageworks_dashboard_full/README.md
+-rw-r--r--   0 briford    (501) staff       (20)     1907 2024-03-28 17:23:43.000000 sageworks-0.6.0/aws_setup/sageworks_dashboard_full/app.py
+-rw-r--r--   0 briford    (501) staff       (20)     2567 2023-12-24 17:18:24.000000 sageworks-0.6.0/aws_setup/sageworks_dashboard_full/cdk.json
+-rw-r--r--   0 briford    (501) staff       (20)       14 2023-12-24 17:18:24.000000 sageworks-0.6.0/aws_setup/sageworks_dashboard_full/requirements-dev.txt
+-rw-r--r--   0 briford    (501) staff       (20)       47 2023-12-24 17:18:24.000000 sageworks-0.6.0/aws_setup/sageworks_dashboard_full/requirements.txt
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 16:58:06.484617 sageworks-0.6.0/aws_setup/sageworks_dashboard_full/sageworks_dashboard_full/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-12-24 17:18:24.000000 sageworks-0.6.0/aws_setup/sageworks_dashboard_full/sageworks_dashboard_full/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)     7022 2024-04-16 15:58:18.000000 sageworks-0.6.0/aws_setup/sageworks_dashboard_full/sageworks_dashboard_full/sageworks_dashboard_stack.py
+-rw-r--r--   0 briford    (501) staff       (20)      437 2023-12-24 17:18:24.000000 sageworks-0.6.0/aws_setup/sageworks_dashboard_full/source.bat
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 16:58:06.484873 sageworks-0.6.0/aws_setup/sageworks_dashboard_full/tests/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-12-24 17:18:24.000000 sageworks-0.6.0/aws_setup/sageworks_dashboard_full/tests/__init__.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 16:58:06.485066 sageworks-0.6.0/aws_setup/sageworks_dashboard_full/tests/unit/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-12-24 17:18:24.000000 sageworks-0.6.0/aws_setup/sageworks_dashboard_full/tests/unit/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)      565 2023-12-24 17:18:24.000000 sageworks-0.6.0/aws_setup/sageworks_dashboard_full/tests/unit/test_sageworks_dashboard_stack.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 16:58:06.485758 sageworks-0.6.0/aws_setup/sageworks_dashboard_lite/
+-rw-r--r--   0 briford    (501) staff       (20)      119 2024-03-28 17:23:43.000000 sageworks-0.6.0/aws_setup/sageworks_dashboard_lite/.gitignore
+-rw-r--r--   0 briford    (501) staff       (20)     1778 2024-03-28 17:23:43.000000 sageworks-0.6.0/aws_setup/sageworks_dashboard_lite/README.md
+-rw-r--r--   0 briford    (501) staff       (20)     1928 2024-03-28 17:23:43.000000 sageworks-0.6.0/aws_setup/sageworks_dashboard_lite/app.py
+-rw-r--r--   0 briford    (501) staff       (20)     2567 2024-03-28 17:23:43.000000 sageworks-0.6.0/aws_setup/sageworks_dashboard_lite/cdk.json
+-rw-r--r--   0 briford    (501) staff       (20)       47 2024-03-28 17:23:43.000000 sageworks-0.6.0/aws_setup/sageworks_dashboard_lite/requirements.txt
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 16:58:06.486014 sageworks-0.6.0/aws_setup/sageworks_dashboard_lite/sageworks_dashboard_lite/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2024-03-28 17:23:43.000000 sageworks-0.6.0/aws_setup/sageworks_dashboard_lite/sageworks_dashboard_lite/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)     6849 2024-04-16 15:58:18.000000 sageworks-0.6.0/aws_setup/sageworks_dashboard_lite/sageworks_dashboard_lite/sageworks_dashboard_stack.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 16:58:06.487218 sageworks-0.6.0/data/
+-rw-r--r--   0 briford    (501) staff       (20)   191978 2023-12-24 17:18:24.000000 sageworks-0.6.0/data/abalone.csv
+-rw-r--r--   0 briford    (501) staff       (20)     1515 2023-12-24 17:18:24.000000 sageworks-0.6.0/data/test_data.csv
+-rw-r--r--   0 briford    (501) staff       (20)     2270 2023-12-24 17:18:24.000000 sageworks-0.6.0/data/test_data.json
+-rw-r--r--   0 briford    (501) staff       (20)    12977 2024-01-10 18:45:51.000000 sageworks-0.6.0/data/wine_dataset.csv
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 16:58:06.487516 sageworks-0.6.0/docs/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 16:58:06.487884 sageworks-0.6.0/docs/admin/
+-rw-r--r--   0 briford    (501) staff       (20)     2176 2024-04-16 15:58:18.000000 sageworks-0.6.0/docs/admin/docker_push.md
+-rw-r--r--   0 briford    (501) staff       (20)     1633 2024-01-10 18:45:51.000000 sageworks-0.6.0/docs/admin/pypi_release.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 16:58:06.489778 sageworks-0.6.0/docs/api_classes/
+-rw-r--r--   0 briford    (501) staff       (20)     3595 2024-01-23 15:36:53.000000 sageworks-0.6.0/docs/api_classes/data_source.md
+-rw-r--r--   0 briford    (501) staff       (20)     5199 2024-03-28 17:23:43.000000 sageworks-0.6.0/docs/api_classes/endpoint.md
+-rw-r--r--   0 briford    (501) staff       (20)     6299 2024-03-28 17:23:43.000000 sageworks-0.6.0/docs/api_classes/feature_set.md
+-rw-r--r--   0 briford    (501) staff       (20)     5350 2024-04-06 16:51:44.000000 sageworks-0.6.0/docs/api_classes/meta.md
+-rw-r--r--   0 briford    (501) staff       (20)     4356 2024-01-10 18:45:51.000000 sageworks-0.6.0/docs/api_classes/model.md
+-rw-r--r--   0 briford    (501) staff       (20)     2218 2024-01-10 18:45:51.000000 sageworks-0.6.0/docs/api_classes/monitor.md
+-rw-r--r--   0 briford    (501) staff       (20)     3549 2024-01-10 18:45:51.000000 sageworks-0.6.0/docs/api_classes/overview.md
+-rw-r--r--   0 briford    (501) staff       (20)     4894 2024-04-19 15:50:50.000000 sageworks-0.6.0/docs/api_classes/pipelines.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 16:58:06.491146 sageworks-0.6.0/docs/aws_setup/
+-rw-r--r--   0 briford    (501) staff       (20)     1121 2024-03-28 17:23:43.000000 sageworks-0.6.0/docs/aws_setup/aws_access_management.md
+-rw-r--r--   0 briford    (501) staff       (20)     7836 2024-01-23 15:36:53.000000 sageworks-0.6.0/docs/aws_setup/aws_tips_and_tricks.md
+-rw-r--r--   0 briford    (501) staff       (20)     4229 2024-03-28 17:23:43.000000 sageworks-0.6.0/docs/aws_setup/core_stack.md
+-rw-r--r--   0 briford    (501) staff       (20)     2075 2024-03-28 17:23:43.000000 sageworks-0.6.0/docs/aws_setup/dashboard_stack.md
+-rw-r--r--   0 briford    (501) staff       (20)     2540 2024-01-23 15:36:53.000000 sageworks-0.6.0/docs/aws_setup/full_pipeline.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 16:58:06.491402 sageworks-0.6.0/docs/concepts/
+-rw-r--r--   0 briford    (501) staff       (20)      907 2024-01-23 15:36:53.000000 sageworks-0.6.0/docs/concepts/model_monitoring.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 16:58:06.491651 sageworks-0.6.0/docs/core_classes/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 16:58:06.493254 sageworks-0.6.0/docs/core_classes/artifacts/
+-rw-r--r--   0 briford    (501) staff       (20)      464 2024-01-23 15:36:53.000000 sageworks-0.6.0/docs/core_classes/artifacts/artifact.md
+-rw-r--r--   0 briford    (501) staff       (20)      290 2024-01-10 18:45:51.000000 sageworks-0.6.0/docs/core_classes/artifacts/athena_source.md
+-rw-r--r--   0 briford    (501) staff       (20)      479 2024-01-23 15:36:53.000000 sageworks-0.6.0/docs/core_classes/artifacts/data_source_abstract.md
+-rw-r--r--   0 briford    (501) staff       (20)      292 2024-01-10 18:45:51.000000 sageworks-0.6.0/docs/core_classes/artifacts/endpoint_core.md
+-rw-r--r--   0 briford    (501) staff       (20)      294 2024-01-10 18:45:51.000000 sageworks-0.6.0/docs/core_classes/artifacts/feature_set_core.md
+-rw-r--r--   0 briford    (501) staff       (20)      281 2024-01-10 18:45:51.000000 sageworks-0.6.0/docs/core_classes/artifacts/model_core.md
+-rw-r--r--   0 briford    (501) staff       (20)      289 2024-01-10 18:45:51.000000 sageworks-0.6.0/docs/core_classes/artifacts/monitor_core.md
+-rw-r--r--   0 briford    (501) staff       (20)      861 2024-01-10 18:45:51.000000 sageworks-0.6.0/docs/core_classes/artifacts/overview.md
+-rw-r--r--   0 briford    (501) staff       (20)     2119 2024-01-10 18:45:51.000000 sageworks-0.6.0/docs/core_classes/overview.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 16:58:06.494807 sageworks-0.6.0/docs/core_classes/transforms/
+-rw-r--r--   0 briford    (501) staff       (20)      352 2024-01-10 18:45:51.000000 sageworks-0.6.0/docs/core_classes/transforms/data_loaders_heavy.md
+-rw-r--r--   0 briford    (501) staff       (20)      396 2024-01-10 18:45:51.000000 sageworks-0.6.0/docs/core_classes/transforms/data_loaders_light.md
+-rw-r--r--   0 briford    (501) staff       (20)      349 2024-03-28 17:23:43.000000 sageworks-0.6.0/docs/core_classes/transforms/data_to_features.md
+-rw-r--r--   0 briford    (501) staff       (20)      265 2024-01-10 18:45:51.000000 sageworks-0.6.0/docs/core_classes/transforms/features_to_model.md
+-rw-r--r--   0 briford    (501) staff       (20)      264 2024-01-10 18:45:51.000000 sageworks-0.6.0/docs/core_classes/transforms/model_to_endpoint.md
+-rw-r--r--   0 briford    (501) staff       (20)     1177 2024-01-10 18:45:51.000000 sageworks-0.6.0/docs/core_classes/transforms/overview.md
+-rw-r--r--   0 briford    (501) staff       (20)      970 2024-01-23 15:36:53.000000 sageworks-0.6.0/docs/core_classes/transforms/pandas_transforms.md
+-rw-r--r--   0 briford    (501) staff       (20)      521 2024-01-23 15:36:53.000000 sageworks-0.6.0/docs/core_classes/transforms/transform.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 16:58:06.495099 sageworks-0.6.0/docs/glue/
+-rw-r--r--   0 briford    (501) staff       (20)     4837 2024-03-28 17:23:43.000000 sageworks-0.6.0/docs/glue/index.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 16:58:06.500386 sageworks-0.6.0/docs/images/
+-rw-r--r--   0 briford    (501) staff       (20)   605827 2023-12-24 17:18:24.000000 sageworks-0.6.0/docs/images/big_spider.png
+-rw-r--r--   0 briford    (501) staff       (20)    32320 2023-12-24 17:18:24.000000 sageworks-0.6.0/docs/images/graph_representation.png
+-rw-r--r--   0 briford    (501) staff       (20)    15549 2023-12-24 17:18:24.000000 sageworks-0.6.0/docs/images/powered_aws_dark_blue.png
+-rw-r--r--   0 briford    (501) staff       (20)    10003 2023-12-24 17:18:24.000000 sageworks-0.6.0/docs/images/powered_aws_transparent.png
+-rw-r--r--   0 briford    (501) staff       (20)     6435 2023-12-24 17:18:24.000000 sageworks-0.6.0/docs/images/powered_aws_white.png
+-rw-r--r--   0 briford    (501) staff       (20)    21174 2023-12-24 17:18:24.000000 sageworks-0.6.0/docs/images/powered_aws_with_tm_grey.png
+-rw-r--r--   0 briford    (501) staff       (20)    51137 2023-12-24 17:18:24.000000 sageworks-0.6.0/docs/images/sageworks.png
+-rw-r--r--   0 briford    (501) staff       (20)   489672 2023-12-24 17:18:24.000000 sageworks-0.6.0/docs/images/sageworks_concepts.png
+-rw-r--r--   0 briford    (501) staff       (20)    30017 2023-12-24 17:18:24.000000 sageworks-0.6.0/docs/images/scp.png
+-rw-r--r--   0 briford    (501) staff       (20)   139307 2023-12-24 17:18:24.000000 sageworks-0.6.0/docs/images/scp_labs.png
+-rw-r--r--   0 briford    (501) staff       (20)   381209 2023-12-24 17:18:24.000000 sageworks-0.6.0/docs/images/small_spider.png
+-rw-r--r--   0 briford    (501) staff       (20)     3417 2024-03-28 17:23:43.000000 sageworks-0.6.0/docs/index.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 16:58:06.501827 sageworks-0.6.0/docs/misc/
+-rw-r--r--   0 briford    (501) staff       (20)     2791 2024-03-28 17:23:43.000000 sageworks-0.6.0/docs/misc/faq.md
+-rw-r--r--   0 briford    (501) staff       (20)     5069 2024-01-10 18:45:51.000000 sageworks-0.6.0/docs/misc/general_info.md
+-rw-r--r--   0 briford    (501) staff       (20)      667 2024-01-10 18:45:51.000000 sageworks-0.6.0/docs/misc/sageworks_classes_concepts.md
+-rw-r--r--   0 briford    (501) staff       (20)     1873 2024-01-10 18:45:51.000000 sageworks-0.6.0/docs/misc/scp_consulting.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 16:58:06.502251 sageworks-0.6.0/docs/plugins/
+-rw-r--r--   0 briford    (501) staff       (20)     3361 2024-04-16 15:58:18.000000 sageworks-0.6.0/docs/plugins/index.md
+-rw-r--r--   0 briford    (501) staff       (20)      750 2024-04-06 16:51:44.000000 sageworks-0.6.0/docs/plugins/plugin_api_changes.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 16:58:06.502502 sageworks-0.6.0/docs/repl/
+-rw-r--r--   0 briford    (501) staff       (20)     2081 2024-03-28 17:23:43.000000 sageworks-0.6.0/docs/repl/index.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 16:58:06.502899 sageworks-0.6.0/docs/research/
+-rw-r--r--   0 briford    (501) staff       (20)      912 2024-03-28 17:23:43.000000 sageworks-0.6.0/docs/research/eda.md
+-rw-r--r--   0 briford    (501) staff       (20)     2017 2024-03-28 17:23:43.000000 sageworks-0.6.0/docs/research/htg.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 16:58:06.503395 sageworks-0.6.0/examples/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 16:58:06.503558 sageworks-0.6.0/examples/ag-grid/
+-rw-r--r--   0 briford    (501) staff       (20)      496 2024-04-06 16:51:44.000000 sageworks-0.6.0/examples/ag-grid/hello_world.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 16:58:06.504657 sageworks-0.6.0/examples/datasource/
+-rw-r--r--   0 briford    (501) staff       (20)      326 2024-01-10 18:45:51.000000 sageworks-0.6.0/examples/datasource/datasource_from_df.py
+-rw-r--r--   0 briford    (501) staff       (20)      332 2024-01-10 18:45:51.000000 sageworks-0.6.0/examples/datasource/datasource_from_s3.py
+-rw-r--r--   0 briford    (501) staff       (20)      536 2024-01-23 15:36:53.000000 sageworks-0.6.0/examples/datasource/datasource_query.py
+-rw-r--r--   0 briford    (501) staff       (20)      680 2024-01-23 15:36:53.000000 sageworks-0.6.0/examples/datasource/datasource_stats.py
+-rw-r--r--   0 briford    (501) staff       (20)      223 2024-01-10 18:45:51.000000 sageworks-0.6.0/examples/datasource/datasource_to_featureset.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 16:58:06.505079 sageworks-0.6.0/examples/endpoint/
+-rw-r--r--   0 briford    (501) staff       (20)      199 2024-01-10 18:45:51.000000 sageworks-0.6.0/examples/endpoint/endpoint_details.py
+-rw-r--r--   0 briford    (501) staff       (20)      834 2024-03-28 17:23:43.000000 sageworks-0.6.0/examples/endpoint/endpoint_inference.py
+-rw-r--r--   0 briford    (501) staff       (20)      481 2024-01-10 18:45:51.000000 sageworks-0.6.0/examples/endpoint/endpoint_metrics.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 16:58:06.505500 sageworks-0.6.0/examples/featureset/
+-rw-r--r--   0 briford    (501) staff       (20)      744 2024-01-10 18:45:51.000000 sageworks-0.6.0/examples/featureset/featureset_eda.py
+-rw-r--r--   0 briford    (501) staff       (20)      560 2024-03-28 17:23:43.000000 sageworks-0.6.0/examples/featureset/featureset_query.py
+-rw-r--r--   0 briford    (501) staff       (20)      421 2024-03-27 20:32:26.000000 sageworks-0.6.0/examples/featureset/featureset_to_model.py
+-rw-r--r--   0 briford    (501) staff       (20)     1534 2024-03-28 17:23:43.000000 sageworks-0.6.0/examples/full_ml_pipeline.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 16:58:06.506332 sageworks-0.6.0/examples/glue/
+-rw-r--r--   0 briford    (501) staff       (20)      580 2024-01-23 15:36:53.000000 sageworks-0.6.0/examples/glue/glue_hello_world.py
+-rw-r--r--   0 briford    (501) staff       (20)      942 2024-01-23 15:36:53.000000 sageworks-0.6.0/examples/glue/glue_hello_world_with_log.py
+-rw-r--r--   0 briford    (501) staff       (20)      686 2024-01-23 15:36:53.000000 sageworks-0.6.0/examples/glue/glue_load_s3_bucket.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 16:58:06.506941 sageworks-0.6.0/examples/meta/
+-rw-r--r--   0 briford    (501) staff       (20)      363 2024-04-06 16:51:44.000000 sageworks-0.6.0/examples/meta/meta_list_endpoints.py
+-rw-r--r--   0 briford    (501) staff       (20)      328 2024-04-06 16:51:44.000000 sageworks-0.6.0/examples/meta/meta_list_models.py
+-rw-r--r--   0 briford    (501) staff       (20)      659 2024-04-06 16:51:44.000000 sageworks-0.6.0/examples/meta/meta_model_metrics.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 16:58:06.507873 sageworks-0.6.0/examples/model/
+-rw-r--r--   0 briford    (501) staff       (20)      548 2024-03-28 17:23:43.000000 sageworks-0.6.0/examples/model/model_metrics.py
+-rw-r--r--   0 briford    (501) staff       (20)      312 2024-03-27 20:32:26.000000 sageworks-0.6.0/examples/model/model_to_endpoint.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 16:58:06.508240 sageworks-0.6.0/examples/monitor/
+-rw-r--r--   0 briford    (501) staff       (20)      400 2024-01-10 18:45:51.000000 sageworks-0.6.0/examples/monitor/monitor_setup.py
+-rw-r--r--   0 briford    (501) staff       (20)      765 2024-01-10 18:45:51.000000 sageworks-0.6.0/examples/monitor/monitor_usage.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 16:58:06.509836 sageworks-0.6.0/examples/pipelines/
+-rw-r--r--   0 briford    (501) staff       (20)     1000 2024-04-19 14:53:32.000000 sageworks-0.6.0/examples/pipelines/abalone_pipeline_v1.json
+-rw-r--r--   0 briford    (501) staff       (20)     1073 2024-04-19 19:42:10.000000 sageworks-0.6.0/examples/pipelines/abalone_pipeline_v2.json
+-rw-r--r--   0 briford    (501) staff       (20)     4435 2024-04-20 17:35:29.000000 sageworks-0.6.0/examples/pipelines/aqsol_pipeline_v1.json
+-rw-r--r--   0 briford    (501) staff       (20)      142 2024-04-19 14:55:38.000000 sageworks-0.6.0/examples/pipelines/pipeline_details.py
+-rw-r--r--   0 briford    (501) staff       (20)      324 2024-04-19 14:55:38.000000 sageworks-0.6.0/examples/pipelines/pipeline_execute.py
+-rw-r--r--   0 briford    (501) staff       (20)      556 2024-04-19 14:51:51.000000 sageworks-0.6.0/examples/pipelines/pipeline_manager.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 16:58:06.462296 sageworks-0.6.0/examples/plugins/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 16:58:06.510817 sageworks-0.6.0/examples/plugins/pages/
+-rw-r--r--   0 briford    (501) staff       (20)     2467 2024-04-09 15:13:19.000000 sageworks-0.6.0/examples/plugins/pages/my_plugin_page.py
+-rw-r--r--   0 briford    (501) staff       (20)     1635 2024-04-16 15:58:18.000000 sageworks-0.6.0/examples/plugins/pages/plugin_page_1.py
+-rw-r--r--   0 briford    (501) staff       (20)     2464 2024-04-16 15:58:18.000000 sageworks-0.6.0/examples/plugins/pages/plugin_page_2.py
+-rw-r--r--   0 briford    (501) staff       (20)     4528 2024-04-16 15:58:18.000000 sageworks-0.6.0/examples/plugins/pages/plugin_page_3.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 16:58:06.511192 sageworks-0.6.0/examples/plugins/views/
+-rw-r--r--   0 briford    (501) staff       (20)     1588 2024-04-06 16:51:44.000000 sageworks-0.6.0/examples/plugins/views/model_plugin_view.py
+-rw-r--r--   0 briford    (501) staff       (20)     1264 2024-04-06 16:51:44.000000 sageworks-0.6.0/examples/plugins/views/my_view_plugin.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 16:58:06.511892 sageworks-0.6.0/examples/plugins/web_components/
+-rw-r--r--   0 briford    (501) staff       (20)     1733 2024-04-16 15:58:18.000000 sageworks-0.6.0/examples/plugins/web_components/custom_plugin.py
+-rw-r--r--   0 briford    (501) staff       (20)     2029 2024-04-16 15:58:18.000000 sageworks-0.6.0/examples/plugins/web_components/endpoint_plugin.py
+-rw-r--r--   0 briford    (501) staff       (20)     3660 2024-04-16 15:58:18.000000 sageworks-0.6.0/examples/plugins/web_components/endpoint_turbo.py
+-rw-r--r--   0 briford    (501) staff       (20)     2596 2024-04-16 15:58:18.000000 sageworks-0.6.0/examples/plugins/web_components/model_markdown.py
+-rw-r--r--   0 briford    (501) staff       (20)     2238 2024-04-16 15:58:18.000000 sageworks-0.6.0/examples/plugins/web_components/model_plugin.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 16:58:06.513031 sageworks-0.6.0/examples/storage/
+-rw-r--r--   0 briford    (501) staff       (20)     1222 2024-03-27 20:40:53.000000 sageworks-0.6.0/examples/storage/data_to_data.py
+-rw-r--r--   0 briford    (501) staff       (20)      856 2024-03-27 20:40:53.000000 sageworks-0.6.0/examples/storage/data_to_features.py
+-rw-r--r--   0 briford    (501) staff       (20)     1371 2024-03-28 17:23:43.000000 sageworks-0.6.0/examples/storage/endpoint_inference.py
+-rw-r--r--   0 briford    (501) staff       (20)     1847 2024-03-28 17:23:43.000000 sageworks-0.6.0/examples/storage/hello_world_pipeline.py
+-rw-r--r--   0 briford    (501) staff       (20)     4380 2024-04-16 15:58:18.000000 sageworks-0.6.0/examples/storage/plugin_page_example.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 16:58:06.513558 sageworks-0.6.0/examples/storage/sagemaker_pipelines/
+-rw-r--r--   0 briford    (501) staff       (20)      854 2024-03-28 17:23:43.000000 sageworks-0.6.0/examples/storage/sagemaker_pipelines/all_steps.py
+-rw-r--r--   0 briford    (501) staff       (20)       40 2024-03-28 17:23:43.000000 sageworks-0.6.0/examples/storage/sagemaker_pipelines/hello.py
+-rw-r--r--   0 briford    (501) staff       (20)     1487 2024-03-28 17:23:43.000000 sageworks-0.6.0/examples/storage/sagemaker_pipelines/ml_pipeline.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 16:58:06.462567 sageworks-0.6.0/examples/storage/sagemaker_pipelines/storage/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 16:58:06.514275 sageworks-0.6.0/examples/storage/sagemaker_pipelines/storage/full_pipeline_experiment/
+-rw-r--r--   0 briford    (501) staff       (20)      854 2024-03-28 17:23:43.000000 sageworks-0.6.0/examples/storage/sagemaker_pipelines/storage/full_pipeline_experiment/data_source.py
+-rw-r--r--   0 briford    (501) staff       (20)      203 2024-03-28 17:23:43.000000 sageworks-0.6.0/examples/storage/sagemaker_pipelines/storage/full_pipeline_experiment/endpoint.py
+-rw-r--r--   0 briford    (501) staff       (20)      160 2024-03-28 17:23:43.000000 sageworks-0.6.0/examples/storage/sagemaker_pipelines/storage/full_pipeline_experiment/feature_set.py
+-rw-r--r--   0 briford    (501) staff       (20)     1599 2024-03-28 17:23:43.000000 sageworks-0.6.0/examples/storage/sagemaker_pipelines/storage/full_pipeline_experiment/ml_pipeline.py
+-rw-r--r--   0 briford    (501) staff       (20)      367 2024-03-28 17:23:43.000000 sageworks-0.6.0/examples/storage/sagemaker_pipelines/storage/full_pipeline_experiment/model.py
+-rw-r--r--   0 briford    (501) staff       (20)     2792 2024-04-16 21:08:28.000000 sageworks-0.6.0/mkdocs.yml
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 16:58:06.515179 sageworks-0.6.0/notebooks/
+-rw-r--r--   0 briford    (501) staff       (20)   185443 2024-03-28 17:23:43.000000 sageworks-0.6.0/notebooks/ML_Pipeline_with_SageWorks.ipynb
+-rw-r--r--   0 briford    (501) staff       (20)    36405 2024-03-28 17:23:43.000000 sageworks-0.6.0/notebooks/ML_Pipeline_with_SageWorks_2.ipynb
+-rw-r--r--   0 briford    (501) staff       (20)   511134 2024-03-28 17:23:43.000000 sageworks-0.6.0/notebooks/Outliers_in_SageWorks.ipynb
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 16:58:06.524336 sageworks-0.6.0/notebooks/images/
+-rw-r--r--   0 briford    (501) staff       (20)   142099 2023-12-24 17:18:24.000000 sageworks-0.6.0/notebooks/images/athena_query_aqsol.png
+-rw-r--r--   0 briford    (501) staff       (20)   191022 2023-12-24 17:18:24.000000 sageworks-0.6.0/notebooks/images/aws_dashboard_aqsol.png
+-rw-r--r--   0 briford    (501) staff       (20)   222686 2023-12-24 17:18:24.000000 sageworks-0.6.0/notebooks/images/dashboard_aqsol_features.png
+-rw-r--r--   0 briford    (501) staff       (20)   171441 2023-12-24 17:18:24.000000 sageworks-0.6.0/notebooks/images/model_screenshot.png
+-rw-r--r--   0 briford    (501) staff       (20)   489672 2023-12-24 17:18:24.000000 sageworks-0.6.0/notebooks/images/sageworks_concepts.png
+-rw-r--r--   0 briford    (501) staff       (20)   139307 2023-12-24 17:18:24.000000 sageworks-0.6.0/notebooks/images/scp_labs.png
+-rw-r--r--   0 briford    (501) staff       (20)      431 2024-04-06 16:51:44.000000 sageworks-0.6.0/requirements.txt
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 16:58:06.528538 sageworks-0.6.0/scripts/
+-rw-r--r--   0 briford    (501) staff       (20)     1710 2024-04-16 15:58:18.000000 sageworks-0.6.0/scripts/ag_table_row_selection.py
+-rw-r--r--   0 briford    (501) staff       (20)     2290 2024-03-28 17:23:43.000000 sageworks-0.6.0/scripts/athena_ddl_mixed_case.py
+-rw-r--r--   0 briford    (501) staff       (20)     2178 2024-03-27 20:32:26.000000 sageworks-0.6.0/scripts/copy_data_catalog_db.py
+-rw-r--r--   0 briford    (501) staff       (20)     1222 2024-04-16 15:58:18.000000 sageworks-0.6.0/scripts/create_glue_workflow_with_trigger.py
+-rw-r--r--   0 briford    (501) staff       (20)      706 2024-01-10 18:45:51.000000 sageworks-0.6.0/scripts/delete_redis_keys.py
+-rw-r--r--   0 briford    (501) staff       (20)     1761 2024-03-28 17:23:43.000000 sageworks-0.6.0/scripts/glue_mixed_case.py
+-rw-r--r--   0 briford    (501) staff       (20)     5544 2024-03-28 17:23:43.000000 sageworks-0.6.0/scripts/model_endpoint_sanity_check.py
+-rw-r--r--   0 briford    (501) staff       (20)      715 2024-03-28 17:23:43.000000 sageworks-0.6.0/scripts/onboard_endpoints.py
+-rw-r--r--   0 briford    (501) staff       (20)      694 2024-03-28 17:23:43.000000 sageworks-0.6.0/scripts/onboard_models.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 16:58:06.529148 sageworks-0.6.0/scripts/storage/
+-rw-r--r--   0 briford    (501) staff       (20)     1003 2024-03-27 20:32:27.000000 sageworks-0.6.0/scripts/storage/dns_data_to_features.py
+-rw-r--r--   0 briford    (501) staff       (20)     1723 2024-04-06 16:51:44.000000 sageworks-0.6.0/scripts/storage/generate_jsonl_data.py
+-rw-r--r--   0 briford    (501) staff       (20)      955 2024-03-28 17:23:43.000000 sageworks-0.6.0/scripts/test_feature_resolution.py
+-rw-r--r--   0 briford    (501) staff       (20)      533 2024-04-23 16:58:06.573947 sageworks-0.6.0/setup.cfg
+-rw-r--r--   0 briford    (501) staff       (20)     1663 2024-03-27 20:32:27.000000 sageworks-0.6.0/setup.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 16:58:06.463054 sageworks-0.6.0/src/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 16:58:06.529422 sageworks-0.6.0/src/sageworks/
+-rw-r--r--   0 briford    (501) staff       (20)     1091 2024-01-10 18:45:51.000000 sageworks-0.6.0/src/sageworks/__init__.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 16:58:06.530374 sageworks-0.6.0/src/sageworks/algorithms/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-12-24 17:18:24.000000 sageworks-0.6.0/src/sageworks/algorithms/__init__.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 16:58:06.532151 sageworks-0.6.0/src/sageworks/algorithms/dataframe/
+-rw-r--r--   0 briford    (501) staff       (20)      378 2023-12-24 17:18:24.000000 sageworks-0.6.0/src/sageworks/algorithms/dataframe/Readme.md
+-rw-r--r--   0 briford    (501) staff       (20)     2852 2024-03-28 17:23:43.000000 sageworks-0.6.0/src/sageworks/algorithms/dataframe/aggregation.py
+-rw-r--r--   0 briford    (501) staff       (20)     1606 2024-03-28 17:23:43.000000 sageworks-0.6.0/src/sageworks/algorithms/dataframe/data_source_eda.py
+-rw-r--r--   0 briford    (501) staff       (20)     5388 2024-03-28 17:23:43.000000 sageworks-0.6.0/src/sageworks/algorithms/dataframe/dimensionality_reduction.py
+-rw-r--r--   0 briford    (501) staff       (20)     9406 2024-03-28 17:23:43.000000 sageworks-0.6.0/src/sageworks/algorithms/dataframe/feature_resolution.py
+-rw-r--r--   0 briford    (501) staff       (20)    12309 2024-03-28 17:23:43.000000 sageworks-0.6.0/src/sageworks/algorithms/dataframe/feature_spider.py
+-rw-r--r--   0 briford    (501) staff       (20)     4968 2024-03-28 17:23:43.000000 sageworks-0.6.0/src/sageworks/algorithms/dataframe/row_tagger.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 16:58:06.463405 sageworks-0.6.0/src/sageworks/algorithms/graph/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 16:58:06.532397 sageworks-0.6.0/src/sageworks/algorithms/graph/heavy/
+-rw-r--r--   0 briford    (501) staff       (20)       96 2023-12-24 17:18:24.000000 sageworks-0.6.0/src/sageworks/algorithms/graph/heavy/Readme.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 16:58:06.532642 sageworks-0.6.0/src/sageworks/algorithms/graph/light/
+-rw-r--r--   0 briford    (501) staff       (20)      122 2023-12-24 17:18:24.000000 sageworks-0.6.0/src/sageworks/algorithms/graph/light/Readme.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 16:58:06.532915 sageworks-0.6.0/src/sageworks/algorithms/spark/
+-rw-r--r--   0 briford    (501) staff       (20)      615 2023-12-24 17:18:24.000000 sageworks-0.6.0/src/sageworks/algorithms/spark/Readme.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 16:58:06.534601 sageworks-0.6.0/src/sageworks/algorithms/sql/
+-rw-r--r--   0 briford    (501) staff       (20)      685 2023-12-24 17:18:24.000000 sageworks-0.6.0/src/sageworks/algorithms/sql/Readme.md
+-rw-r--r--   0 briford    (501) staff       (20)     6192 2024-03-28 17:23:43.000000 sageworks-0.6.0/src/sageworks/algorithms/sql/column_stats.py
+-rw-r--r--   0 briford    (501) staff       (20)     3645 2024-03-28 17:23:43.000000 sageworks-0.6.0/src/sageworks/algorithms/sql/correlations.py
+-rw-r--r--   0 briford    (501) staff       (20)     3622 2024-03-28 17:23:43.000000 sageworks-0.6.0/src/sageworks/algorithms/sql/descriptive_stats.py
+-rw-r--r--   0 briford    (501) staff       (20)    10174 2024-03-28 17:23:43.000000 sageworks-0.6.0/src/sageworks/algorithms/sql/outliers.py
+-rw-r--r--   0 briford    (501) staff       (20)     2352 2024-03-28 17:23:43.000000 sageworks-0.6.0/src/sageworks/algorithms/sql/sample_rows.py
+-rw-r--r--   0 briford    (501) staff       (20)     3437 2024-03-28 17:23:43.000000 sageworks-0.6.0/src/sageworks/algorithms/sql/value_counts.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 16:58:06.536835 sageworks-0.6.0/src/sageworks/api/
+-rw-r--r--   0 briford    (501) staff       (20)      708 2024-04-18 20:46:23.000000 sageworks-0.6.0/src/sageworks/api/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)     7811 2024-03-28 17:23:43.000000 sageworks-0.6.0/src/sageworks/api/data_source.py
+-rw-r--r--   0 briford    (501) staff       (20)     2505 2024-03-28 17:23:43.000000 sageworks-0.6.0/src/sageworks/api/endpoint.py
+-rw-r--r--   0 briford    (501) staff       (20)     4242 2024-03-28 17:23:43.000000 sageworks-0.6.0/src/sageworks/api/feature_set.py
+-rw-r--r--   0 briford    (501) staff       (20)    16482 2024-04-21 15:28:58.000000 sageworks-0.6.0/src/sageworks/api/meta.py
+-rw-r--r--   0 briford    (501) staff       (20)     2595 2024-04-16 15:58:18.000000 sageworks-0.6.0/src/sageworks/api/model.py
+-rw-r--r--   0 briford    (501) staff       (20)     5261 2024-03-28 17:23:43.000000 sageworks-0.6.0/src/sageworks/api/monitor.py
+-rw-r--r--   0 briford    (501) staff       (20)     7016 2024-04-22 20:46:36.000000 sageworks-0.6.0/src/sageworks/api/pipeline.py
+-rw-r--r--   0 briford    (501) staff       (20)     6731 2024-04-19 14:53:21.000000 sageworks-0.6.0/src/sageworks/api/pipeline_manager.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 16:58:06.537583 sageworks-0.6.0/src/sageworks/aws_service_broker/
+-rw-r--r--   0 briford    (501) staff       (20)     9393 2024-03-28 17:23:43.000000 sageworks-0.6.0/src/sageworks/aws_service_broker/aws_account_clamp.py
+-rw-r--r--   0 briford    (501) staff       (20)    10908 2024-04-06 16:51:44.000000 sageworks-0.6.0/src/sageworks/aws_service_broker/aws_service_broker.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 16:58:06.538976 sageworks-0.6.0/src/sageworks/aws_service_broker/aws_service_connectors/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-12-24 17:18:24.000000 sageworks-0.6.0/src/sageworks/aws_service_broker/aws_service_connectors/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)     1834 2024-03-28 17:23:43.000000 sageworks-0.6.0/src/sageworks/aws_service_broker/aws_service_connectors/connector.py
+-rw-r--r--   0 briford    (501) staff       (20)     3258 2024-03-28 17:23:43.000000 sageworks-0.6.0/src/sageworks/aws_service_broker/aws_service_connectors/data_catalog.py
+-rw-r--r--   0 briford    (501) staff       (20)     4055 2024-03-28 17:23:43.000000 sageworks-0.6.0/src/sageworks/aws_service_broker/aws_service_connectors/endpoints.py
+-rw-r--r--   0 briford    (501) staff       (20)     5238 2024-03-28 17:23:43.000000 sageworks-0.6.0/src/sageworks/aws_service_broker/aws_service_connectors/feature_store.py
+-rw-r--r--   0 briford    (501) staff       (20)     3712 2024-03-28 17:23:43.000000 sageworks-0.6.0/src/sageworks/aws_service_broker/aws_service_connectors/glue_jobs.py
+-rw-r--r--   0 briford    (501) staff       (20)     3889 2024-03-28 17:23:43.000000 sageworks-0.6.0/src/sageworks/aws_service_broker/aws_service_connectors/model_registry.py
+-rw-r--r--   0 briford    (501) staff       (20)     3736 2024-03-28 17:23:43.000000 sageworks-0.6.0/src/sageworks/aws_service_broker/aws_service_connectors/s3_bucket.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 16:58:06.539125 sageworks-0.6.0/src/sageworks/core/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.0/src/sageworks/core/__init__.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 16:58:06.542029 sageworks-0.6.0/src/sageworks/core/artifacts/
+-rw-r--r--   0 briford    (501) staff       (20)      941 2024-03-28 17:23:43.000000 sageworks-0.6.0/src/sageworks/core/artifacts/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)    17938 2024-04-15 22:06:08.000000 sageworks-0.6.0/src/sageworks/core/artifacts/artifact.py
+-rw-r--r--   0 briford    (501) staff       (20)    22432 2024-04-06 16:51:44.000000 sageworks-0.6.0/src/sageworks/core/artifacts/athena_source.py
+-rw-r--r--   0 briford    (501) staff       (20)    12683 2024-03-28 17:23:43.000000 sageworks-0.6.0/src/sageworks/core/artifacts/data_source_abstract.py
+-rw-r--r--   0 briford    (501) staff       (20)     2447 2024-03-28 17:23:43.000000 sageworks-0.6.0/src/sageworks/core/artifacts/data_source_factory.py
+-rw-r--r--   0 briford    (501) staff       (20)    36630 2024-04-21 18:44:59.000000 sageworks-0.6.0/src/sageworks/core/artifacts/endpoint_core.py
+-rw-r--r--   0 briford    (501) staff       (20)    29698 2024-04-22 20:46:36.000000 sageworks-0.6.0/src/sageworks/core/artifacts/feature_set_core.py
+-rw-r--r--   0 briford    (501) staff       (20)    35498 2024-04-22 20:58:40.000000 sageworks-0.6.0/src/sageworks/core/artifacts/model_core.py
+-rw-r--r--   0 briford    (501) staff       (20)    21029 2024-03-28 17:23:43.000000 sageworks-0.6.0/src/sageworks/core/artifacts/monitor_core.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 16:58:06.542528 sageworks-0.6.0/src/sageworks/core/pipelines/
+-rw-r--r--   0 briford    (501) staff       (20)     6928 2024-04-22 20:46:36.000000 sageworks-0.6.0/src/sageworks/core/pipelines/pipeline_executor.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 16:58:06.543244 sageworks-0.6.0/src/sageworks/core/transforms/
+-rw-r--r--   0 briford    (501) staff       (20)     1432 2024-01-10 18:45:51.000000 sageworks-0.6.0/src/sageworks/core/transforms/Readme.md
+-rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.0/src/sageworks/core/transforms/__init__.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 16:58:06.543580 sageworks-0.6.0/src/sageworks/core/transforms/data_loaders/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.0/src/sageworks/core/transforms/data_loaders/__init__.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 16:58:06.543936 sageworks-0.6.0/src/sageworks/core/transforms/data_loaders/heavy/
+-rw-r--r--   0 briford    (501) staff       (20)      298 2024-03-28 17:23:43.000000 sageworks-0.6.0/src/sageworks/core/transforms/data_loaders/heavy/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)     9866 2024-03-28 17:23:43.000000 sageworks-0.6.0/src/sageworks/core/transforms/data_loaders/heavy/s3_heavy_to_data_source.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 16:58:06.545111 sageworks-0.6.0/src/sageworks/core/transforms/data_loaders/light/
+-rw-r--r--   0 briford    (501) staff       (20)      543 2024-03-28 17:23:43.000000 sageworks-0.6.0/src/sageworks/core/transforms/data_loaders/light/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)     3011 2024-03-28 17:23:43.000000 sageworks-0.6.0/src/sageworks/core/transforms/data_loaders/light/csv_to_data_source.py
+-rw-r--r--   0 briford    (501) staff       (20)     2927 2024-03-28 17:23:43.000000 sageworks-0.6.0/src/sageworks/core/transforms/data_loaders/light/json_to_data_source.py
+-rw-r--r--   0 briford    (501) staff       (20)     4225 2024-03-28 17:23:43.000000 sageworks-0.6.0/src/sageworks/core/transforms/data_loaders/light/s3_to_data_source_light.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 16:58:06.545366 sageworks-0.6.0/src/sageworks/core/transforms/data_to_data/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.0/src/sageworks/core/transforms/data_to_data/__init__.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 16:58:06.545468 sageworks-0.6.0/src/sageworks/core/transforms/data_to_data/heavy/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.0/src/sageworks/core/transforms/data_to_data/heavy/__init__.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 16:58:06.545570 sageworks-0.6.0/src/sageworks/core/transforms/data_to_data/heavy/emr/
+-rw-r--r--   0 briford    (501) staff       (20)       68 2024-01-10 18:45:51.000000 sageworks-0.6.0/src/sageworks/core/transforms/data_to_data/heavy/emr/Readme.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 16:58:06.545801 sageworks-0.6.0/src/sageworks/core/transforms/data_to_data/heavy/glue/
+-rw-r--r--   0 briford    (501) staff       (20)       48 2024-01-10 18:45:51.000000 sageworks-0.6.0/src/sageworks/core/transforms/data_to_data/heavy/glue/Readme.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 16:58:06.546333 sageworks-0.6.0/src/sageworks/core/transforms/data_to_data/light/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.0/src/sageworks/core/transforms/data_to_data/light/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)     2237 2024-03-27 20:40:53.000000 sageworks-0.6.0/src/sageworks/core/transforms/data_to_data/light/clean_data.py
+-rw-r--r--   0 briford    (501) staff       (20)     2687 2024-03-27 20:40:53.000000 sageworks-0.6.0/src/sageworks/core/transforms/data_to_data/light/data_to_data_light.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 16:58:06.546561 sageworks-0.6.0/src/sageworks/core/transforms/data_to_features/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.0/src/sageworks/core/transforms/data_to_features/__init__.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 16:58:06.546669 sageworks-0.6.0/src/sageworks/core/transforms/data_to_features/heavy/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.0/src/sageworks/core/transforms/data_to_features/heavy/__init__.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 16:58:06.546879 sageworks-0.6.0/src/sageworks/core/transforms/data_to_features/heavy/chunk/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.0/src/sageworks/core/transforms/data_to_features/heavy/chunk/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)     4551 2024-03-28 17:23:43.000000 sageworks-0.6.0/src/sageworks/core/transforms/data_to_features/heavy/chunk/data_to_features_chunk.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 16:58:06.547116 sageworks-0.6.0/src/sageworks/core/transforms/data_to_features/heavy/emr/
+-rw-r--r--   0 briford    (501) staff       (20)       68 2024-01-10 18:45:51.000000 sageworks-0.6.0/src/sageworks/core/transforms/data_to_features/heavy/emr/Readme.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 16:58:06.547265 sageworks-0.6.0/src/sageworks/core/transforms/data_to_features/heavy/glue/
+-rw-r--r--   0 briford    (501) staff       (20)       48 2024-01-10 18:45:51.000000 sageworks-0.6.0/src/sageworks/core/transforms/data_to_features/heavy/glue/Readme.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 16:58:06.547406 sageworks-0.6.0/src/sageworks/core/transforms/data_to_features/heavy/storage/
+-rw-r--r--   0 briford    (501) staff       (20)     6702 2024-03-28 17:23:43.000000 sageworks-0.6.0/src/sageworks/core/transforms/data_to_features/heavy/storage/data_to_features_heavy_old.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 16:58:06.547917 sageworks-0.6.0/src/sageworks/core/transforms/data_to_features/light/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.0/src/sageworks/core/transforms/data_to_features/light/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)     3827 2024-03-28 17:23:43.000000 sageworks-0.6.0/src/sageworks/core/transforms/data_to_features/light/data_to_features_light.py
+-rw-r--r--   0 briford    (501) staff       (20)     5674 2024-04-23 15:16:38.000000 sageworks-0.6.0/src/sageworks/core/transforms/data_to_features/light/molecular_descriptors.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 16:58:06.548174 sageworks-0.6.0/src/sageworks/core/transforms/features_to_features/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.0/src/sageworks/core/transforms/features_to_features/__init__.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 16:58:06.465431 sageworks-0.6.0/src/sageworks/core/transforms/features_to_features/heavy/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 16:58:06.548274 sageworks-0.6.0/src/sageworks/core/transforms/features_to_features/heavy/emr/
+-rw-r--r--   0 briford    (501) staff       (20)       68 2024-01-10 18:45:51.000000 sageworks-0.6.0/src/sageworks/core/transforms/features_to_features/heavy/emr/Readme.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 16:58:06.548428 sageworks-0.6.0/src/sageworks/core/transforms/features_to_features/heavy/glue/
+-rw-r--r--   0 briford    (501) staff       (20)       48 2024-01-10 18:45:51.000000 sageworks-0.6.0/src/sageworks/core/transforms/features_to_features/heavy/glue/Readme.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 16:58:06.548678 sageworks-0.6.0/src/sageworks/core/transforms/features_to_model/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.0/src/sageworks/core/transforms/features_to_model/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)    13050 2024-03-28 17:23:43.000000 sageworks-0.6.0/src/sageworks/core/transforms/features_to_model/features_to_model.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 16:58:06.549264 sageworks-0.6.0/src/sageworks/core/transforms/features_to_model/light_model_harness/
+-rw-r--r--   0 briford    (501) staff       (20)       19 2024-02-27 23:40:48.000000 sageworks-0.6.0/src/sageworks/core/transforms/features_to_model/light_model_harness/requirements.txt
+-rw-r--r--   0 briford    (501) staff       (20)    10806 2024-03-28 17:23:43.000000 sageworks-0.6.0/src/sageworks/core/transforms/features_to_model/light_model_harness/xgb_model.template
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 16:58:06.549668 sageworks-0.6.0/src/sageworks/core/transforms/model_to_endpoint/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.0/src/sageworks/core/transforms/model_to_endpoint/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)     8185 2024-03-28 17:23:43.000000 sageworks-0.6.0/src/sageworks/core/transforms/model_to_endpoint/model_to_endpoint.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 16:58:06.550932 sageworks-0.6.0/src/sageworks/core/transforms/pandas_transforms/
+-rw-r--r--   0 briford    (501) staff       (20)      894 2024-03-28 17:23:43.000000 sageworks-0.6.0/src/sageworks/core/transforms/pandas_transforms/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)     3615 2024-03-28 17:23:43.000000 sageworks-0.6.0/src/sageworks/core/transforms/pandas_transforms/data_to_pandas.py
+-rw-r--r--   0 briford    (501) staff       (20)     3445 2024-03-28 17:23:43.000000 sageworks-0.6.0/src/sageworks/core/transforms/pandas_transforms/features_to_pandas.py
+-rw-r--r--   0 briford    (501) staff       (20)     8604 2024-04-06 16:51:44.000000 sageworks-0.6.0/src/sageworks/core/transforms/pandas_transforms/pandas_to_data.py
+-rw-r--r--   0 briford    (501) staff       (20)    18139 2024-04-06 16:51:44.000000 sageworks-0.6.0/src/sageworks/core/transforms/pandas_transforms/pandas_to_features.py
+-rw-r--r--   0 briford    (501) staff       (20)     4440 2024-03-28 17:23:43.000000 sageworks-0.6.0/src/sageworks/core/transforms/pandas_transforms/pandas_to_features_chunked.py
+-rw-r--r--   0 briford    (501) staff       (20)     5391 2024-03-28 17:23:43.000000 sageworks-0.6.0/src/sageworks/core/transforms/transform.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 16:58:06.551099 sageworks-0.6.0/src/sageworks/experiments/
+-rw-r--r--   0 briford    (501) staff       (20)    10658 2024-03-28 17:23:43.000000 sageworks-0.6.0/src/sageworks/experiments/view_manager.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 16:58:06.551483 sageworks-0.6.0/src/sageworks/repl/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.0/src/sageworks/repl/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)    15486 2024-04-21 15:35:25.000000 sageworks-0.6.0/src/sageworks/repl/sageworks_shell.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 16:58:06.551994 sageworks-0.6.0/src/sageworks/resources/
+-rw-r--r--   0 briford    (501) staff       (20)      361 2024-01-23 15:36:53.000000 sageworks-0.6.0/src/sageworks/resources/open_source_api.key
+-rw-r--r--   0 briford    (501) staff       (20)      272 2024-01-10 18:45:51.000000 sageworks-0.6.0/src/sageworks/resources/signature_verify_pub.pem
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 16:58:06.559277 sageworks-0.6.0/src/sageworks/utils/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-12-24 17:18:24.000000 sageworks-0.6.0/src/sageworks/utils/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)    15587 2024-04-06 16:51:44.000000 sageworks-0.6.0/src/sageworks/utils/aws_utils.py
+-rw-r--r--   0 briford    (501) staff       (20)     5447 2024-04-16 15:58:18.000000 sageworks-0.6.0/src/sageworks/utils/cache.py
+-rw-r--r--   0 briford    (501) staff       (20)      722 2024-03-28 17:23:43.000000 sageworks-0.6.0/src/sageworks/utils/chem_utils.py
+-rw-r--r--   0 briford    (501) staff       (20)    16543 2024-04-16 15:58:18.000000 sageworks-0.6.0/src/sageworks/utils/config_manager.py
+-rw-r--r--   0 briford    (501) staff       (20)     7392 2024-03-28 17:23:43.000000 sageworks-0.6.0/src/sageworks/utils/dashboard_metrics.py
+-rw-r--r--   0 briford    (501) staff       (20)     4194 2024-04-06 16:51:44.000000 sageworks-0.6.0/src/sageworks/utils/datetime_utils.py
+-rw-r--r--   0 briford    (501) staff       (20)     5292 2024-03-28 17:23:43.000000 sageworks-0.6.0/src/sageworks/utils/df_to_endpoint.py
+-rw-r--r--   0 briford    (501) staff       (20)     1681 2024-03-28 17:23:43.000000 sageworks-0.6.0/src/sageworks/utils/docker_utils.py
+-rw-r--r--   0 briford    (501) staff       (20)     2866 2024-03-27 20:43:31.000000 sageworks-0.6.0/src/sageworks/utils/ecs_info.py
+-rw-r--r--   0 briford    (501) staff       (20)     7657 2024-03-28 17:23:43.000000 sageworks-0.6.0/src/sageworks/utils/endpoint_metrics.py
+-rw-r--r--   0 briford    (501) staff       (20)     3097 2024-03-28 17:23:43.000000 sageworks-0.6.0/src/sageworks/utils/endpoint_utils.py
+-rw-r--r--   0 briford    (501) staff       (20)     6979 2024-03-28 17:23:43.000000 sageworks-0.6.0/src/sageworks/utils/extract_model_artifact.py
+-rw-r--r--   0 briford    (501) staff       (20)     1131 2024-03-28 17:23:43.000000 sageworks-0.6.0/src/sageworks/utils/glue_utils.py
+-rw-r--r--   0 briford    (501) staff       (20)     5757 2024-03-28 17:23:43.000000 sageworks-0.6.0/src/sageworks/utils/license_manager.py
+-rw-r--r--   0 briford    (501) staff       (20)     1439 2024-04-06 16:51:44.000000 sageworks-0.6.0/src/sageworks/utils/markdown_utils.py
+-rw-r--r--   0 briford    (501) staff       (20)    15517 2024-04-22 20:45:19.000000 sageworks-0.6.0/src/sageworks/utils/pandas_utils.py
+-rw-r--r--   0 briford    (501) staff       (20)    12684 2024-04-16 15:58:18.000000 sageworks-0.6.0/src/sageworks/utils/plugin_manager.py
+-rw-r--r--   0 briford    (501) staff       (20)     9533 2024-04-06 16:51:44.000000 sageworks-0.6.0/src/sageworks/utils/redis_cache.py
+-rw-r--r--   0 briford    (501) staff       (20)     4166 2024-03-28 17:23:43.000000 sageworks-0.6.0/src/sageworks/utils/repl_utils.py
+-rw-r--r--   0 briford    (501) staff       (20)     2089 2024-03-28 17:23:43.000000 sageworks-0.6.0/src/sageworks/utils/s3_utils.py
+-rw-r--r--   0 briford    (501) staff       (20)     2163 2024-03-28 17:23:43.000000 sageworks-0.6.0/src/sageworks/utils/sageworks_cache.py
+-rw-r--r--   0 briford    (501) staff       (20)     3474 2024-03-28 17:23:43.000000 sageworks-0.6.0/src/sageworks/utils/sageworks_event_bridge.py
+-rw-r--r--   0 briford    (501) staff       (20)     5359 2024-03-28 17:23:43.000000 sageworks-0.6.0/src/sageworks/utils/sageworks_logging.py
+-rw-r--r--   0 briford    (501) staff       (20)     2120 2024-03-28 17:23:43.000000 sageworks-0.6.0/src/sageworks/utils/sageworks_sqs.py
+-rw-r--r--   0 briford    (501) staff       (20)     1108 2024-01-10 18:45:51.000000 sageworks-0.6.0/src/sageworks/utils/symbols.py
+-rw-r--r--   0 briford    (501) staff       (20)     6414 2024-03-28 17:23:43.000000 sageworks-0.6.0/src/sageworks/utils/test_data_generator.py
+-rw-r--r--   0 briford    (501) staff       (20)     2092 2024-03-27 20:43:31.000000 sageworks-0.6.0/src/sageworks/utils/trace_calls.py
+-rw-r--r--   0 briford    (501) staff       (20)     1470 2024-03-28 17:23:43.000000 sageworks-0.6.0/src/sageworks/utils/type_abbrev.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 16:58:06.561128 sageworks-0.6.0/src/sageworks/views/
+-rw-r--r--   0 briford    (501) staff       (20)     3517 2024-04-16 22:29:17.000000 sageworks-0.6.0/src/sageworks/views/artifacts_text_view.py
+-rw-r--r--   0 briford    (501) staff       (20)     7008 2024-04-06 16:51:44.000000 sageworks-0.6.0/src/sageworks/views/artifacts_web_view.py
+-rw-r--r--   0 briford    (501) staff       (20)     3158 2024-04-06 16:51:44.000000 sageworks-0.6.0/src/sageworks/views/data_source_web_view.py
+-rw-r--r--   0 briford    (501) staff       (20)     2150 2024-04-06 16:51:44.000000 sageworks-0.6.0/src/sageworks/views/endpoint_web_view.py
+-rw-r--r--   0 briford    (501) staff       (20)     3206 2024-04-06 16:51:44.000000 sageworks-0.6.0/src/sageworks/views/feature_set_web_view.py
+-rw-r--r--   0 briford    (501) staff       (20)     2029 2024-04-06 16:51:44.000000 sageworks-0.6.0/src/sageworks/views/model_web_view.py
+-rw-r--r--   0 briford    (501) staff       (20)     1092 2024-03-28 17:23:43.000000 sageworks-0.6.0/src/sageworks/views/view.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 16:58:06.564485 sageworks-0.6.0/src/sageworks/web_components/
+-rw-r--r--   0 briford    (501) staff       (20)     5862 2024-04-16 15:58:18.000000 sageworks-0.6.0/src/sageworks/web_components/component_interface.py
+-rw-r--r--   0 briford    (501) staff       (20)     3525 2024-04-16 15:58:18.000000 sageworks-0.6.0/src/sageworks/web_components/confusion_matrix.py
+-rw-r--r--   0 briford    (501) staff       (20)     5854 2024-04-16 15:58:18.000000 sageworks-0.6.0/src/sageworks/web_components/correlation_matrix.py
+-rw-r--r--   0 briford    (501) staff       (20)     9328 2024-04-06 16:51:44.000000 sageworks-0.6.0/src/sageworks/web_components/data_details_markdown.py
+-rw-r--r--   0 briford    (501) staff       (20)     4558 2024-04-06 16:51:44.000000 sageworks-0.6.0/src/sageworks/web_components/endpoint_details.py
+-rw-r--r--   0 briford    (501) staff       (20)     3068 2024-04-16 15:58:18.000000 sageworks-0.6.0/src/sageworks/web_components/endpoint_metric_plots.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 16:58:06.566405 sageworks-0.6.0/src/sageworks/web_components/experiments/
+-rw-r--r--   0 briford    (501) staff       (20)      837 2024-04-16 15:58:18.000000 sageworks-0.6.0/src/sageworks/web_components/experiments/color_maps.py
+-rw-r--r--   0 briford    (501) staff       (20)     1633 2024-03-28 17:23:43.000000 sageworks-0.6.0/src/sageworks/web_components/experiments/compound_details.py
+-rw-r--r--   0 briford    (501) staff       (20)     2974 2024-04-16 15:58:18.000000 sageworks-0.6.0/src/sageworks/web_components/experiments/dashboard_metric_plots.py
+-rw-r--r--   0 briford    (501) staff       (20)     2240 2024-04-16 15:58:18.000000 sageworks-0.6.0/src/sageworks/web_components/experiments/data_table.py
+-rw-r--r--   0 briford    (501) staff       (20)     1183 2024-03-28 17:23:43.000000 sageworks-0.6.0/src/sageworks/web_components/experiments/histogram.py
+-rw-r--r--   0 briford    (501) staff       (20)      838 2024-04-16 15:58:18.000000 sageworks-0.6.0/src/sageworks/web_components/experiments/line_chart.py
+-rw-r--r--   0 briford    (501) staff       (20)     3680 2024-03-28 17:23:43.000000 sageworks-0.6.0/src/sageworks/web_components/experiments/outlier_plot.py
+-rw-r--r--   0 briford    (501) staff       (20)     2373 2024-04-16 15:58:18.000000 sageworks-0.6.0/src/sageworks/web_components/experiments/plugin_callbacks.py
+-rw-r--r--   0 briford    (501) staff       (20)     2279 2024-03-28 17:23:43.000000 sageworks-0.6.0/src/sageworks/web_components/experiments/scatter_plot.py
+-rw-r--r--   0 briford    (501) staff       (20)     8690 2024-04-16 15:58:18.000000 sageworks-0.6.0/src/sageworks/web_components/model_details.py
+-rw-r--r--   0 briford    (501) staff       (20)     2278 2024-04-16 15:58:18.000000 sageworks-0.6.0/src/sageworks/web_components/model_plot.py
+-rw-r--r--   0 briford    (501) staff       (20)     7079 2024-04-16 15:58:18.000000 sageworks-0.6.0/src/sageworks/web_components/plugin_interface.py
+-rw-r--r--   0 briford    (501) staff       (20)     3155 2024-04-19 21:25:54.000000 sageworks-0.6.0/src/sageworks/web_components/plugin_unit_test.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 16:58:06.566687 sageworks-0.6.0/src/sageworks/web_components/plugins/
+-rw-r--r--   0 briford    (501) staff       (20)     2862 2024-04-16 15:58:18.000000 sageworks-0.6.0/src/sageworks/web_components/plugins/ag_table.py
+-rw-r--r--   0 briford    (501) staff       (20)     9653 2024-04-15 13:43:00.000000 sageworks-0.6.0/src/sageworks/web_components/plugins/model_details.py
+-rw-r--r--   0 briford    (501) staff       (20)     2945 2024-04-16 15:58:18.000000 sageworks-0.6.0/src/sageworks/web_components/regression_plot.py
+-rw-r--r--   0 briford    (501) staff       (20)     6547 2024-04-16 15:58:18.000000 sageworks-0.6.0/src/sageworks/web_components/table.py
+-rw-r--r--   0 briford    (501) staff       (20)     5185 2024-04-16 15:58:18.000000 sageworks-0.6.0/src/sageworks/web_components/violin_plots.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 16:58:06.573166 sageworks-0.6.0/src/sageworks.egg-info/
+-rw-r--r--   0 briford    (501) staff       (20)     4117 2024-04-23 16:58:06.000000 sageworks-0.6.0/src/sageworks.egg-info/PKG-INFO
+-rw-r--r--   0 briford    (501) staff       (20)    18445 2024-04-23 16:58:06.000000 sageworks-0.6.0/src/sageworks.egg-info/SOURCES.txt
+-rw-r--r--   0 briford    (501) staff       (20)        1 2024-04-23 16:58:06.000000 sageworks-0.6.0/src/sageworks.egg-info/dependency_links.txt
+-rw-r--r--   0 briford    (501) staff       (20)       74 2024-04-23 16:58:06.000000 sageworks-0.6.0/src/sageworks.egg-info/entry_points.txt
+-rw-r--r--   0 briford    (501) staff       (20)      408 2024-04-23 16:58:06.000000 sageworks-0.6.0/src/sageworks.egg-info/requires.txt
+-rw-r--r--   0 briford    (501) staff       (20)       10 2024-04-23 16:58:06.000000 sageworks-0.6.0/src/sageworks.egg-info/top_level.txt
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 16:58:06.568009 sageworks-0.6.0/tests/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 16:58:06.568777 sageworks-0.6.0/tests/artifacts/
+-rw-r--r--   0 briford    (501) staff       (20)     1548 2024-03-30 19:27:28.000000 sageworks-0.6.0/tests/artifacts/data_source_tests.py
+-rw-r--r--   0 briford    (501) staff       (20)     2442 2024-03-28 17:23:43.000000 sageworks-0.6.0/tests/artifacts/endpoint_tests.py
+-rw-r--r--   0 briford    (501) staff       (20)     1160 2024-03-28 17:23:43.000000 sageworks-0.6.0/tests/artifacts/feature_set_tests.py
+-rw-r--r--   0 briford    (501) staff       (20)      805 2024-03-28 17:23:43.000000 sageworks-0.6.0/tests/artifacts/model_tests.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 16:58:06.569176 sageworks-0.6.0/tests/aws_account/
+-rw-r--r--   0 briford    (501) staff       (20)      962 2023-12-24 17:18:24.000000 sageworks-0.6.0/tests/aws_account/aws_account_clamp_tests.py
+-rw-r--r--   0 briford    (501) staff       (20)      642 2023-12-24 17:18:24.000000 sageworks-0.6.0/tests/aws_account/aws_service_broker_tests.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 16:58:06.570581 sageworks-0.6.0/tests/connectors/
+-rw-r--r--   0 briford    (501) staff       (20)      725 2024-03-28 17:23:43.000000 sageworks-0.6.0/tests/connectors/data_catalog.py
+-rw-r--r--   0 briford    (501) staff       (20)      737 2024-03-28 17:23:43.000000 sageworks-0.6.0/tests/connectors/endpoints.py
+-rw-r--r--   0 briford    (501) staff       (20)      702 2024-03-28 17:23:43.000000 sageworks-0.6.0/tests/connectors/feature_store.py
+-rw-r--r--   0 briford    (501) staff       (20)      644 2024-03-28 17:23:43.000000 sageworks-0.6.0/tests/connectors/glue_jobs.py
+-rw-r--r--   0 briford    (501) staff       (20)      799 2024-03-28 17:23:43.000000 sageworks-0.6.0/tests/connectors/model_registry.py
+-rw-r--r--   0 briford    (501) staff       (20)     1008 2024-03-28 17:23:43.000000 sageworks-0.6.0/tests/connectors/s3_bucket.py
+-rw-r--r--   0 briford    (501) staff       (20)     5408 2024-03-28 17:23:43.000000 sageworks-0.6.0/tests/create_aqsol_artifacts.py
+-rw-r--r--   0 briford    (501) staff       (20)     3217 2024-03-28 17:23:43.000000 sageworks-0.6.0/tests/create_basic_test_artifacts.py
+-rw-r--r--   0 briford    (501) staff       (20)      870 2024-03-28 17:23:43.000000 sageworks-0.6.0/tests/create_realtime_endpoint.py
+-rw-r--r--   0 briford    (501) staff       (20)     2378 2024-04-22 20:46:36.000000 sageworks-0.6.0/tests/create_training_adjusted_artifacts.py
+-rw-r--r--   0 briford    (501) staff       (20)     2096 2024-03-28 17:23:43.000000 sageworks-0.6.0/tests/create_wine_artifacts.py
+-rw-r--r--   0 briford    (501) staff       (20)     4448 2024-04-16 15:58:18.000000 sageworks-0.6.0/tests/delete_test_artifacts.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 16:58:06.570732 sageworks-0.6.0/tests/plugin_tests/
+-rw-r--r--   0 briford    (501) staff       (20)     1885 2024-04-16 15:58:18.000000 sageworks-0.6.0/tests/plugin_tests/crashing_plugin.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 16:58:06.571023 sageworks-0.6.0/tests/specific/
+-rw-r--r--   0 briford    (501) staff       (20)      639 2024-03-28 17:23:43.000000 sageworks-0.6.0/tests/specific/capital_tests.py
+-rw-r--r--   0 briford    (501) staff       (20)     1513 2024-03-28 17:23:43.000000 sageworks-0.6.0/tests/specific/deletion_tests.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 16:58:06.572340 sageworks-0.6.0/tests/transforms/
+-rw-r--r--   0 briford    (501) staff       (20)      592 2024-03-28 17:23:43.000000 sageworks-0.6.0/tests/transforms/data_to_data_tests.py
+-rw-r--r--   0 briford    (501) staff       (20)     1025 2024-03-28 17:23:43.000000 sageworks-0.6.0/tests/transforms/data_to_features_tests.py
+-rw-r--r--   0 briford    (501) staff       (20)      773 2024-03-28 17:23:43.000000 sageworks-0.6.0/tests/transforms/features_to_model_tests.py
+-rw-r--r--   0 briford    (501) staff       (20)     5142 2024-04-20 00:25:37.000000 sageworks-0.6.0/tests/transforms/model_metrics_tests.py
+-rw-r--r--   0 briford    (501) staff       (20)      795 2024-03-28 17:23:43.000000 sageworks-0.6.0/tests/transforms/model_to_endpoint_tests.py
+-rw-r--r--   0 briford    (501) staff       (20)      633 2024-03-27 20:40:53.000000 sageworks-0.6.0/tests/transforms/pandas_to_data_tests.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 16:58:06.572850 sageworks-0.6.0/tests/web_components/
+-rw-r--r--   0 briford    (501) staff       (20)      681 2024-04-16 15:58:18.000000 sageworks-0.6.0/tests/web_components/confusion_matrix_test.py
+-rw-r--r--   0 briford    (501) staff       (20)      677 2024-04-16 15:58:18.000000 sageworks-0.6.0/tests/web_components/correlation_matrix_test.py
+-rw-r--r--   0 briford    (501) staff       (20)     5269 2024-04-16 15:58:18.000000 sageworks-0.6.0/tests/web_components/plugin_interface_test.py
+-rw-r--r--   0 briford    (501) staff       (20)     1115 2024-03-27 20:43:31.000000 sageworks-0.6.0/tox.ini
```

### Comparing `sageworks-0.5.4/.github/PULL_REQUEST_TEMPLATE.md` & `sageworks-0.6.0/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/.github/workflows/deploy-docs.yml` & `sageworks-0.6.0/.github/workflows/deploy-docs.yml`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/.github/workflows/python-lint.yml` & `sageworks-0.6.0/.github/workflows/python-lint.yml`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/.gitignore` & `sageworks-0.6.0/.gitignore`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/LICENSE` & `sageworks-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/Makefile` & `sageworks-0.6.0/Makefile`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/PKG-INFO` & `sageworks-0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sageworks
-Version: 0.5.4
+Version: 0.6.0
 Summary: SageWorks: A Python WorkBench for creating and deploying AWS SageMaker Models
 Home-page: https://github.com/SuperCowPowers/sageworks
 Author: SuperCowPowers LLC
 Author-email: support@supercowpowers.com
 License: MIT
 Keywords: SageMaker,Machine Learning,AWS,Python,Utilities
 Classifier: Development Status :: 4 - Beta
@@ -81,8 +81,8 @@
 Using SageWorks will minimize the time and manpower needed to incorporate AWS ML into your organization. If your company would like to be a SageWorks Beta Tester, contact us at [sageworks@supercowpowers.com](mailto:sageworks@supercowpowers.com).
 
 ### Contributions
 If you'd like to contribute to the SageWorks project, you're more than welcome. All contributions will fall under the existing project [license](https://github.com/SuperCowPowers/sageworks/blob/main/LICENSE). If you are interested in contributing or have questions please feel free to contact us at [sageworks@supercowpowers.com](mailto:sageworks@supercowpowers.com).
 
 <img align="right" src="docs/images/scp.png" width="180">
 
-® Amazon Web Services, AWS, the Powered by AWS logo, are trademarks of Amazon.com, Inc. or its affiliates.
+® Amazon Web Services, AWS, the Powered by AWS logo, are trademarks of Amazon.com, Inc. or its affiliates
```

### Comparing `sageworks-0.5.4/README.md` & `sageworks-0.6.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -41,8 +41,8 @@
 Using SageWorks will minimize the time and manpower needed to incorporate AWS ML into your organization. If your company would like to be a SageWorks Beta Tester, contact us at [sageworks@supercowpowers.com](mailto:sageworks@supercowpowers.com).
 
 ### Contributions
 If you'd like to contribute to the SageWorks project, you're more than welcome. All contributions will fall under the existing project [license](https://github.com/SuperCowPowers/sageworks/blob/main/LICENSE). If you are interested in contributing or have questions please feel free to contact us at [sageworks@supercowpowers.com](mailto:sageworks@supercowpowers.com).
 
 <img align="right" src="docs/images/scp.png" width="180">
 
-® Amazon Web Services, AWS, the Powered by AWS logo, are trademarks of Amazon.com, Inc. or its affiliates.
+® Amazon Web Services, AWS, the Powered by AWS logo, are trademarks of Amazon.com, Inc. or its affiliates
```

### Comparing `sageworks-0.5.4/applications/aws_dashboard/Dockerfile` & `sageworks-0.6.0/applications/aws_dashboard/Dockerfile`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 RUN pip install --no-cache-dir -r requirements.txt
 
 # Copy the Nginx and Supervisor configuration files
 COPY nginx.conf /etc/nginx/sites-available/default
 COPY supervisord.conf /etc/supervisor/conf.d/supervisord.conf
 
 # Install Sageworks (changes often)
-RUN pip install --no-cache-dir sageworks==0.5.3
+RUN pip install --no-cache-dir sageworks==0.5.4
 
 # Copy the current directory contents into the container at /app
 COPY . /app
 
 # Grab the config file from build args, copy, and set ENV var
 ARG SAGEWORKS_CONFIG
 COPY $SAGEWORKS_CONFIG /app/sageworks_config.json
```

### Comparing `sageworks-0.5.4/applications/aws_dashboard/README.md` & `sageworks-0.6.0/applications/aws_dashboard/README.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/applications/aws_dashboard/app.py` & `sageworks-0.6.0/applications/aws_dashboard/app.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/applications/aws_dashboard/assets/bootstrap_darkly.min.css` & `sageworks-0.6.0/applications/aws_dashboard/assets/bootstrap_darkly.min.css`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/applications/aws_dashboard/assets/default.css` & `sageworks-0.6.0/applications/aws_dashboard/assets/default.css`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/applications/aws_dashboard/assets/trash.png` & `sageworks-0.6.0/applications/aws_dashboard/assets/trash.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/applications/aws_dashboard/dashboard` & `sageworks-0.6.0/applications/aws_dashboard/dashboard`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/applications/aws_dashboard/open_source_config.json` & `sageworks-0.6.0/applications/aws_dashboard/open_source_config.json`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/applications/aws_dashboard/pages/data_sources/callbacks.py` & `sageworks-0.6.0/applications/aws_dashboard/pages/data_sources/callbacks.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,15 +83,15 @@
         data_details = data_source_web_view.data_source_details(data_source_uuid)
         details_markdown = data_details_markdown.DataDetailsMarkdown().generate_markdown(data_details)
 
         # Set the Header Text
         header = f"Details: {data_source_uuid}"
 
         # Generate a new correlation matrix figure
-        corr_figure = correlation_matrix.CorrelationMatrix().update_contents(data_details)
+        corr_figure = correlation_matrix.CorrelationMatrix().update_properties(data_details)
 
         # Return the details/markdown for these data details
         return [header, details_markdown, corr_figure]
 
 
 def update_data_source_sample_rows(app: Dash, data_source_web_view: DataSourceWebView):
     @app.callback(
@@ -131,15 +131,15 @@
             style_cells = table.Table().style_data_conditional()
         else:
             unique_categories = smart_sample_rows[color_column].unique().tolist()
             unique_categories = [x for x in unique_categories if x != "sample"]
             style_cells = table.Table().style_data_conditional(color_column, unique_categories)
 
         # Update the Violin Plot with the new smart sample rows
-        violin_figure = violin_plots.ViolinPlots().update_contents(
+        violin_figure = violin_plots.ViolinPlots().update_properties(
             smart_sample_rows,
             figure_args={
                 "box_visible": True,
                 "meanline_visible": True,
                 "showlegend": False,
                 "points": "all",
                 "spanmode": "hard",
```

### Comparing `sageworks-0.5.4/applications/aws_dashboard/pages/data_sources/layout.py` & `sageworks-0.6.0/applications/aws_dashboard/pages/data_sources/layout.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/applications/aws_dashboard/pages/data_sources/page.py` & `sageworks-0.6.0/applications/aws_dashboard/pages/data_sources/page.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/applications/aws_dashboard/pages/endpoints/callbacks.py` & `sageworks-0.6.0/applications/aws_dashboard/pages/endpoints/callbacks.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,23 @@
 """Callbacks for the Endpoints Subpage Web User Interface"""
 
-from dash import Dash, no_update
+import logging
+from dash import Dash, callback, no_update
+from dash.exceptions import PreventUpdate
 from dash.dependencies import Input, Output, State
 
 # SageWorks Imports
 from sageworks.views.endpoint_web_view import EndpointWebView
 from sageworks.web_components import table, endpoint_metric_plots
 from sageworks.utils.pandas_utils import deserialize_aws_broker_data
 from sageworks.api.endpoint import Endpoint
 
+# Get the SageWorks logger
+log = logging.getLogger("sageworks")
+
 
 def update_endpoints_table(app: Dash):
     @app.callback(
         [
             Output("endpoints_table", "columns"),
             Output("endpoints_table", "data"),
         ],
@@ -70,35 +75,40 @@
         endpoint_uuid = selected_row_data["uuid"]
         print(f"Endpoint UUID: {endpoint_uuid}")
 
         # Endpoint Details
         endpoint_details = endpoint_web_view.endpoint_details(endpoint_uuid)
 
         # Endpoint Metrics
-        endpoint_metrics_figure = endpoint_metric_plots.EndpointMetricPlots().update_contents(endpoint_details)
+        endpoint_metrics_figure = endpoint_metric_plots.EndpointMetricPlots().update_properties(endpoint_details)
 
         # Return the details/markdown for these data details
         return endpoint_metrics_figure
 
 
-# Updates the plugin component when a endpoint row is selected
-def update_plugin(app: Dash, plugin, endpoint_web_view: EndpointWebView):
-    @app.callback(
-        Output(plugin.component_id(), "figure"),
+# Set up the plugin callbacks that take an endpoint
+def setup_plugin_callbacks(plugins):
+    @callback(
+        # Aggregate plugin outputs
+        [Output(component_id, prop) for p in plugins for component_id, prop in p.properties],
         Input("endpoints_table", "derived_viewport_selected_row_ids"),
         State("endpoints_table", "data"),
-        prevent_initial_call=True,
     )
-    def update_callback(selected_rows, table_data):
+    def update_all_plugin_properties(selected_rows, table_data):
         # Check for no selected rows
         if not selected_rows or selected_rows[0] is None:
-            return no_update
+            raise PreventUpdate
 
         # Get the selected row data and grab the uuid
         selected_row_data = table_data[selected_rows[0]]
-        endpoint_uuid = selected_row_data["uuid"]
+        object_uuid = selected_row_data["uuid"]
+
+        # Create the Endpoint object
+        endpoint = Endpoint(object_uuid, legacy=True)
 
-        # Instantiate the Endpoint and send it to the plugin
-        endpoint = Endpoint(endpoint_uuid, legacy=True)
+        # Update all the properties for each plugin
+        all_props = []
+        for p in plugins:
+            all_props.extend(p.update_properties(endpoint))
 
-        # Instantiate the Endpoint and send it to the plugin
-        return plugin.update_contents(endpoint)
+        # Return all the updated properties
+        return all_props
```

### Comparing `sageworks-0.5.4/applications/aws_dashboard/pages/endpoints/layout.py` & `sageworks-0.6.0/applications/aws_dashboard/pages/endpoints/layout.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     ]
     layout = html.Div(
         children=[
             dbc.Row(
                 [
                     html.H2("SageWorks: Endpoints"),
                     dbc.Row(style={"padding": "30px 0px 0px 0px"}),
+                    html.Div(id="dev_null", style={"display": "none"}),  # Output for callbacks without outputs
                 ]
             ),
             # A table that lists out all the Models
             dbc.Row(endpoints_table),
             # Model Details, and Plugins
             dbc.Row(
                 [
```

### Comparing `sageworks-0.5.4/applications/aws_dashboard/pages/endpoints/page.py` & `sageworks-0.6.0/applications/aws_dashboard/pages/endpoints/page.py`

 * *Files 14% similar despite different names*

```diff
@@ -48,25 +48,24 @@
 
 # Load any web components plugins of type 'endpoint'
 pm = PluginManager()
 plugins = pm.get_list_of_web_plugins(plugin_page=PluginPage.ENDPOINT)
 
 # Add the plugins to the components dictionary
 for plugin in plugins:
-    component_id = plugin.component_id()
+    component_id = plugin.generate_component_id()
     components[component_id] = plugin.create_component(component_id)
 
 # Set up our layout (Dash looks for a var called layout)
 layout = endpoints_layout(**components)
 
 # Setup our callbacks/connections
 app = dash.get_app()
 callbacks.update_endpoints_table(app)
 endpoint_details.register_callbacks("endpoints_table")
 
 # Callback for the endpoints table
 callbacks.table_row_select(app, "endpoints_table")
 callbacks.update_endpoint_metrics(app, endpoint_broker)
 
-# For each plugin, set up a callback to update the plugin figure
-for plugin in plugins:
-    callbacks.update_plugin(app, plugin, endpoint_broker)
+# For all the plugins we have we'll call their update_properties method
+callbacks.setup_plugin_callbacks(plugins)
```

### Comparing `sageworks-0.5.4/applications/aws_dashboard/pages/feature_sets/callbacks.py` & `sageworks-0.6.0/applications/aws_dashboard/pages/feature_sets/callbacks.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,15 +78,15 @@
         header = f"Details: {feature_set_uuid}"
 
         # FeatureSet Details
         feature_details = feature_set_web_view.feature_set_details(feature_set_uuid)
         feature_details_markdown = data_details_markdown.DataDetailsMarkdown().generate_markdown(feature_details)
 
         # Generate a new correlation matrix figure
-        corr_figure = correlation_matrix.CorrelationMatrix().update_contents(feature_details)
+        corr_figure = correlation_matrix.CorrelationMatrix().update_properties(feature_details)
 
         # Return the details/markdown for these data details
         return [header, feature_details_markdown, corr_figure]
 
 
 def update_feature_set_sample_rows(app: Dash, feature_set_web_view: FeatureSetWebView):
     @app.callback(
@@ -126,15 +126,15 @@
             style_cells = table.Table().style_data_conditional()
         else:
             unique_categories = smart_sample_rows[color_column].unique().tolist()
             unique_categories = [x for x in unique_categories if x != "sample"]
             style_cells = table.Table().style_data_conditional(color_column, unique_categories)
 
         # Update the Violin Plot with the new smart sample rows
-        violin_figure = violin_plots.ViolinPlots().update_contents(
+        violin_figure = violin_plots.ViolinPlots().update_properties(
             smart_sample_rows,
             figure_args={
                 "box_visible": True,
                 "meanline_visible": True,
                 "showlegend": False,
                 "points": "all",
                 "spanmode": "hard",
```

### Comparing `sageworks-0.5.4/applications/aws_dashboard/pages/feature_sets/layout.py` & `sageworks-0.6.0/applications/aws_dashboard/pages/feature_sets/layout.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/applications/aws_dashboard/pages/feature_sets/page.py` & `sageworks-0.6.0/applications/aws_dashboard/pages/feature_sets/page.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/applications/aws_dashboard/pages/main/callbacks.py` & `sageworks-0.6.0/applications/aws_dashboard/pages/main/callbacks.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/applications/aws_dashboard/pages/main/layout.py` & `sageworks-0.6.0/applications/aws_dashboard/pages/main/layout.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/applications/aws_dashboard/pages/main/page.py` & `sageworks-0.6.0/applications/aws_dashboard/pages/main/page.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/applications/aws_dashboard/pages/models/callbacks.py` & `sageworks-0.6.0/applications/aws_dashboard/pages/models/callbacks.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 """Callbacks for the Model Subpage Web User Interface"""
 
-from dash import Dash, no_update
+import logging
+from dash import Dash, callback, no_update
+from dash.exceptions import PreventUpdate
 from dash.dependencies import Input, Output, State
 
 # SageWorks Imports
-from sageworks.views.model_web_view import ModelWebView
-from sageworks.web_components import (
-    table,
-    model_plot,
-)
+from sageworks.web_components import table, model_plot
 from sageworks.utils.pandas_utils import deserialize_aws_broker_data
 from sageworks.api.model import Model
 
+# Get the SageWorks logger
+log = logging.getLogger("sageworks")
+
 
 def update_models_table(app: Dash):
     @app.callback(
         [Output("models_table", "columns"), Output("models_table", "data")],
         Input("aws-broker-data", "data"),
     )
     def models_update(serialized_aws_broker_data):
@@ -67,33 +68,56 @@
 
         # Get the selected row data and grab the uuid
         selected_row_data = table_data[selected_rows[0]]
         model_uuid = selected_row_data["uuid"]
         m = Model(model_uuid, legacy=True)
 
         # Model Details Markdown component
-        model_plot_fig = model_plot.ModelPlot().update_contents(m, inference_run)
+        model_plot_fig = model_plot.ModelPlot().update_properties(m, inference_run)
 
         # Return the details/markdown for these data details
         return model_plot_fig
 
 
-# Updates the plugin component when a model row is selected
-def update_plugin(app: Dash, plugin, model_web_view: ModelWebView):
-    @app.callback(
-        Output(plugin.component_id(), "figure"),
-        [Input("model_details-dropdown", "value"), Input("models_table", "derived_viewport_selected_row_ids")],
+"""
+# Register the plugin callbacks for the model subpage
+def register_plugin_callbacks(plugins):
+    # Setup the inputs for the plugins and register the callbacks
+    model_inputs = [
+        Input("model_details-dropdown", "value"),
+        Input("models_table", "derived_viewport_selected_row_ids"),
+        State("models_table", "data"),
+    ]
+
+    # Sanity check that we have some plugins
+    if plugins:
+        plugin_callbacks.register_callbacks(plugins, model_inputs, "model")
+"""
+
+
+def setup_plugin_callbacks(plugins):
+    @callback(
+        # Aggregate plugin outputs
+        [Output(component_id, prop) for p in plugins for component_id, prop in p.properties],
+        Input("model_details-dropdown", "value"),
+        Input("models_table", "derived_viewport_selected_row_ids"),
         State("models_table", "data"),
-        prevent_initial_call=True,
     )
-    def update_plugin_figure(inference_run, selected_rows, table_data):
+    def update_all_plugin_properties(inference_run, selected_rows, table_data):
         # Check for no selected rows
         if not selected_rows or selected_rows[0] is None:
-            return no_update
+            raise PreventUpdate
 
         # Get the selected row data and grab the uuid
         selected_row_data = table_data[selected_rows[0]]
-        model_uuid = selected_row_data["uuid"]
+        object_uuid = selected_row_data["uuid"]
+
+        # Create the Model object
+        model = Model(object_uuid, legacy=True)
+
+        # Update all the properties for each plugin
+        all_props = []
+        for p in plugins:
+            all_props.extend(p.update_properties(model, inference_run=inference_run))
 
-        # Instantiate the Model and send it to the plugin
-        model = Model(model_uuid, legacy=True)
-        return plugin.update_contents(model, inference_run=inference_run)
+        # Return all the updated properties
+        return all_props
```

### Comparing `sageworks-0.5.4/applications/aws_dashboard/pages/models/layout.py` & `sageworks-0.6.0/applications/aws_dashboard/pages/models/layout.py`

 * *Files 11% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     ]
     layout = html.Div(
         children=[
             dbc.Row(
                 [
                     html.H2("SageWorks: Models"),
                     dbc.Row(style={"padding": "30px 0px 0px 0px"}),
+                    html.Div(id="dev_null", style={"display": "none"}),  # Output for callbacks without outputs
                 ]
             ),
             # A table that lists out all the Models
             dbc.Row(models_table),
             # Model Details, and Plugins
             dbc.Row(
                 [
```

### Comparing `sageworks-0.5.4/applications/aws_dashboard/pages/models/page.py` & `sageworks-0.6.0/applications/aws_dashboard/pages/models/page.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,30 +11,26 @@
 # SageWorks Imports
 from sageworks.web_components import (
     table,
     model_details,
     model_plot,
 )
 from sageworks.web_components.plugin_interface import PluginPage
-from sageworks.views.model_web_view import ModelWebView
 from sageworks.utils.plugin_manager import PluginManager
 
 # Register this page with Dash
 register_page(
     __name__,
     path="/models",
     name="SageWorks - Models",
 )
 
 # Put the components into 'dark' mode
 load_figure_template("darkly")
 
-# Grab a view that gives us a summary of the Models in SageWorks
-model_broker = ModelWebView()
-
 # Create a table to display the models
 models_table = table.Table().create_component(
     "models_table", header_color="rgb(60, 100, 60)", row_select="single", max_height=270
 )
 
 # Create a Markdown component to display the model details
 model_details = model_details.ModelDetails()
@@ -52,25 +48,24 @@
 
 # Load any web components plugins of type 'model'
 pm = PluginManager()
 plugins = pm.get_list_of_web_plugins(plugin_page=PluginPage.MODEL)
 
 # Add the plugins to the components dictionary
 for plugin in plugins:
-    component_id = plugin.component_id()
+    component_id = plugin.generate_component_id()
     components[component_id] = plugin.create_component(component_id)
 
 # Set up our layout (Dash looks for a var called layout)
 layout = models_layout(**components)
 
 # Setup our callbacks/connections
 app = dash.get_app()
 callbacks.update_models_table(app)
 model_details.register_callbacks("models_table")
 
 # Callback for the model table
 callbacks.table_row_select(app, "models_table")
 callbacks.update_model_plot_component(app)
 
-# For each plugin, set up a callback to update the plugin figure
-for plugin in plugins:
-    callbacks.update_plugin(app, plugin, model_broker)
+# Set up callbacks for all the plugins
+callbacks.setup_plugin_callbacks(plugins)
```

### Comparing `sageworks-0.5.4/applications/experiments/compound_explorer/app.py` & `sageworks-0.6.0/applications/experiments/compound_explorer/app.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/applications/experiments/compound_explorer/assets/custom.css` & `sageworks-0.6.0/applications/experiments/compound_explorer/assets/custom.css`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/applications/experiments/compound_explorer/callbacks.py` & `sageworks-0.6.0/applications/experiments/compound_explorer/callbacks.py`

 * *Files 0% similar despite different names*

```diff
@@ -192,15 +192,15 @@
         prevent_initial_call=True,
     )
     def generate_new_violin_plot(selected_rows):
         print(f"Selected Rows: {selected_rows}")
         if not selected_rows or selected_rows[0] is None:
             return dash.no_update
         smart_sample_rows = data_source_web_view.data_source_smart_sample(selected_rows[0])
-        return violin_plots.ViolinPlots().update_contents(
+        return violin_plots.ViolinPlots().update_properties(
             smart_sample_rows,
             figure_args={
                 "box_visible": True,
                 "meanline_visible": True,
                 "showlegend": False,
                 "points": "all",
             },
```

### Comparing `sageworks-0.5.4/applications/experiments/compound_explorer/layout.py` & `sageworks-0.6.0/applications/experiments/compound_explorer/layout.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/aws_setup/aws_account_check.py` & `sageworks-0.6.0/aws_setup/aws_account_check.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/aws_setup/aws_identity_check.py` & `sageworks-0.6.0/aws_setup/aws_identity_check.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/aws_setup/build_ml_pipeline.py` & `sageworks-0.6.0/aws_setup/build_ml_pipeline.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/aws_setup/event_bridge/dynamic_docker/app.py` & `sageworks-0.6.0/aws_setup/event_bridge/dynamic_docker/app.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/aws_setup/event_bridge/dynamic_docker/cdk.json` & `sageworks-0.6.0/aws_setup/event_bridge/dynamic_docker/cdk.json`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/aws_setup/event_bridge/dynamic_docker/lambda/lambda_replace_task.py` & `sageworks-0.6.0/aws_setup/event_bridge/dynamic_docker/lambda/lambda_replace_task.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/aws_setup/event_bridge/dynamic_docker/sageworks_image_update_stack.py` & `sageworks-0.6.0/aws_setup/event_bridge/dynamic_docker/sageworks_image_update_stack.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/aws_setup/sageworks_core/README.md` & `sageworks-0.6.0/aws_setup/sageworks_core/README.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/aws_setup/sageworks_core/app.py` & `sageworks-0.6.0/aws_setup/sageworks_core/app.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/aws_setup/sageworks_core/cdk.json` & `sageworks-0.6.0/aws_setup/sageworks_core/cdk.json`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/aws_setup/sageworks_core/sageworks_core/sageworks_core_stack.py` & `sageworks-0.6.0/aws_setup/sageworks_core/sageworks_core/sageworks_core_stack.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/aws_setup/sageworks_core/tests/unit/test_sageworks_sandbox_stack.py` & `sageworks-0.6.0/aws_setup/sageworks_core/tests/unit/test_sageworks_sandbox_stack.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/aws_setup/sageworks_dashboard_full/README.md` & `sageworks-0.6.0/aws_setup/sageworks_dashboard_full/README.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/aws_setup/sageworks_dashboard_full/app.py` & `sageworks-0.6.0/aws_setup/sageworks_dashboard_full/app.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/aws_setup/sageworks_dashboard_full/cdk.json` & `sageworks-0.6.0/aws_setup/sageworks_dashboard_full/cdk.json`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/aws_setup/sageworks_dashboard_full/sageworks_dashboard_full/sageworks_dashboard_stack.py` & `sageworks-0.6.0/aws_setup/sageworks_dashboard_full/sageworks_dashboard_full/sageworks_dashboard_stack.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 )
 from aws_cdk.aws_ec2 import Subnet
 from aws_cdk.aws_certificatemanager import Certificate
 from aws_cdk.aws_ecs_patterns import ApplicationLoadBalancedFargateService
 from constructs import Construct
 
 # When you want a different version change this line
-dashboard_image = "public.ecr.aws/m6i5k1r2/sageworks_dashboard:v0_5_3_amd64"
+dashboard_image = "public.ecr.aws/m6i5k1r2/sageworks_dashboard:v0_5_4_amd64"
 
 
 class SageworksDashboardStackProps(StackProps):
     def __init__(
         self,
         sageworks_bucket: str,
         sageworks_api_key: str,
```

### Comparing `sageworks-0.5.4/aws_setup/sageworks_dashboard_full/tests/unit/test_sageworks_dashboard_stack.py` & `sageworks-0.6.0/aws_setup/sageworks_dashboard_full/tests/unit/test_sageworks_dashboard_stack.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/aws_setup/sageworks_dashboard_lite/README.md` & `sageworks-0.6.0/aws_setup/sageworks_dashboard_lite/README.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/aws_setup/sageworks_dashboard_lite/app.py` & `sageworks-0.6.0/aws_setup/sageworks_dashboard_lite/app.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/aws_setup/sageworks_dashboard_lite/cdk.json` & `sageworks-0.6.0/aws_setup/sageworks_dashboard_lite/cdk.json`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/aws_setup/sageworks_dashboard_lite/sageworks_dashboard_lite/sageworks_dashboard_stack.py` & `sageworks-0.6.0/aws_setup/sageworks_dashboard_lite/sageworks_dashboard_lite/sageworks_dashboard_stack.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     aws_logs as logs,
 )
 from aws_cdk.aws_certificatemanager import Certificate
 from aws_cdk.aws_ecs_patterns import ApplicationLoadBalancedFargateService
 from constructs import Construct
 
 # When you want a different version change this line
-dashboard_image = "public.ecr.aws/m6i5k1r2/sageworks_dashboard:v0_5_0_amd64"
+dashboard_image = "public.ecr.aws/m6i5k1r2/sageworks_dashboard:v0_5_4_amd64"
 
 
 class SageworksDashboardStackProps(StackProps):
     def __init__(
         self,
         sageworks_bucket: str,
         sageworks_api_key: str,
```

### Comparing `sageworks-0.5.4/data/abalone.csv` & `sageworks-0.6.0/data/abalone.csv`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/data/test_data.csv` & `sageworks-0.6.0/data/test_data.csv`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/data/test_data.json` & `sageworks-0.6.0/data/test_data.json`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/data/wine_dataset.csv` & `sageworks-0.6.0/data/wine_dataset.csv`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/docs/admin/docker_push.md` & `sageworks-0.6.0/docs/admin/docker_push.md`

 * *Files 19% similar despite different names*

```diff
@@ -46,11 +46,22 @@
 docker tag public.ecr.aws/m6i5k1r2/sageworks_dashboard:v0_4_13_amd64 \
 public.ecr.aws/m6i5k1r2/sageworks_dashboard:latest
 ```
 ```
 docker push public.ecr.aws/m6i5k1r2/sageworks_dashboard:latest
 ```
 
+### Update the 'stable' tag
+This is obviously only when you want to mark a version as stable. Meaning that it seems to 'be good and stable (ish)' :)
+
+```
+docker tag public.ecr.aws/m6i5k1r2/sageworks_dashboard:v0_5_4_amd64 \
+public.ecr.aws/m6i5k1r2/sageworks_dashboard:stable
+```
+```
+docker push public.ecr.aws/m6i5k1r2/sageworks_dashboard:stable
+```
+
 ### Test the ECR Image
 You have a `docker_ecr_dashboard` alias in your `~/.zshrc` :)
```

### Comparing `sageworks-0.5.4/docs/admin/pypi_release.md` & `sageworks-0.6.0/docs/admin/pypi_release.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/docs/api_classes/data_source.md` & `sageworks-0.6.0/docs/api_classes/data_source.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/docs/api_classes/endpoint.md` & `sageworks-0.6.0/docs/api_classes/endpoint.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/docs/api_classes/feature_set.md` & `sageworks-0.6.0/docs/api_classes/feature_set.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/docs/api_classes/meta.md` & `sageworks-0.6.0/docs/api_classes/meta.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/docs/api_classes/model.md` & `sageworks-0.6.0/docs/api_classes/model.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/docs/api_classes/monitor.md` & `sageworks-0.6.0/docs/api_classes/monitor.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/docs/api_classes/overview.md` & `sageworks-0.6.0/docs/api_classes/overview.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/docs/aws_setup/aws_access_management.md` & `sageworks-0.6.0/docs/aws_setup/aws_access_management.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/docs/aws_setup/aws_tips_and_tricks.md` & `sageworks-0.6.0/docs/aws_setup/aws_tips_and_tricks.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/docs/aws_setup/core_stack.md` & `sageworks-0.6.0/docs/aws_setup/core_stack.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/docs/aws_setup/dashboard_stack.md` & `sageworks-0.6.0/docs/aws_setup/dashboard_stack.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/docs/aws_setup/full_pipeline.md` & `sageworks-0.6.0/docs/aws_setup/full_pipeline.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/docs/concepts/model_monitoring.md` & `sageworks-0.6.0/docs/concepts/model_monitoring.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/docs/core_classes/artifacts/overview.md` & `sageworks-0.6.0/docs/core_classes/artifacts/overview.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/docs/core_classes/overview.md` & `sageworks-0.6.0/docs/core_classes/overview.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/docs/core_classes/transforms/overview.md` & `sageworks-0.6.0/docs/core_classes/transforms/overview.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/docs/core_classes/transforms/pandas_transforms.md` & `sageworks-0.6.0/docs/core_classes/transforms/pandas_transforms.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/docs/core_classes/transforms/transform.md` & `sageworks-0.6.0/docs/core_classes/transforms/transform.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/docs/glue/index.md` & `sageworks-0.6.0/docs/glue/index.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/docs/images/big_spider.png` & `sageworks-0.6.0/docs/images/big_spider.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/docs/images/graph_representation.png` & `sageworks-0.6.0/docs/images/graph_representation.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/docs/images/powered_aws_dark_blue.png` & `sageworks-0.6.0/docs/images/powered_aws_dark_blue.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/docs/images/powered_aws_transparent.png` & `sageworks-0.6.0/docs/images/powered_aws_transparent.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/docs/images/powered_aws_white.png` & `sageworks-0.6.0/docs/images/powered_aws_white.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/docs/images/powered_aws_with_tm_grey.png` & `sageworks-0.6.0/docs/images/powered_aws_with_tm_grey.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/docs/images/sageworks.png` & `sageworks-0.6.0/docs/images/sageworks.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/docs/images/sageworks_concepts.png` & `sageworks-0.6.0/docs/images/sageworks_concepts.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/docs/images/scp.png` & `sageworks-0.6.0/docs/images/scp.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/docs/images/scp_labs.png` & `sageworks-0.6.0/docs/images/scp_labs.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/docs/images/small_spider.png` & `sageworks-0.6.0/docs/images/small_spider.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/docs/index.md` & `sageworks-0.6.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/docs/misc/faq.md` & `sageworks-0.6.0/docs/misc/faq.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/docs/misc/general_info.md` & `sageworks-0.6.0/docs/misc/general_info.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/docs/misc/sageworks_classes_concepts.md` & `sageworks-0.6.0/docs/misc/sageworks_classes_concepts.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/docs/misc/scp_consulting.md` & `sageworks-0.6.0/docs/misc/scp_consulting.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/docs/plugins/index.md` & `sageworks-0.6.0/docs/plugins/index.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 !!! tip inline end "SageWorks Plugins"
     The SageWorks toolkit provides a flexible plugin architecture to expand, enhance, or even replace the [Dashboard](../aws_setup/dashboard_stack.md). Make custom UI components, views, and entire pages with the plugin classes described here.
 
 The SageWorks Plugin system allows clients to customize how their AWS Machine Learning Pipeline is displayed, analyzed, and visualized. Our easy to use Python API enables developers to make new [Dash/Plotly](https://plotly.com/) components, data views, and entirely new web pages focused on business use cases.
 
 ### Concept Docs
 Many classes in SageWorks need additional high-level material that covers class design and illustrates class usage. Here's the Concept Docs for Plugins:
- 
-- [Getting Started]( https://docs.google.com/presentation/d/1S_-XapmyTsXIkO6od9AVkTbEU2nqS-mEZwFrtUucUME/edit?usp=sharing) 
+
+- [Plugin Concepts: Read First!](https://docs.google.com/presentation/d/1RjpMmJW1i9auPztn2xXYmYKXsZjsnG7vVaCQQ4FLIMM/edit?usp=sharing)
+- [How to Write a Plugin]( https://docs.google.com/presentation/d/1S_-XapmyTsXIkO6od9AVkTbEU2nqS-mEZwFrtUucUME/edit?usp=sharing) 
 - [Plugin Pages](https://docs.google.com/presentation/d/1Yp4ka8DGPdRs8WfsAAUTnc0SHzkkcdJY2TABKxD_CPo/edit?usp=sharing)
 - [Plugins Advanced](https://docs.google.com/presentation/d/1sByTnZa24lY6d4INRMm7OHmQndIZmLbTxOyTeAJol20/edit?usp=sharing)
 
 ## Make a plugin
 
 Each plugin class inherits from the SageWorks PluginInterface class and needs to set two attributes and implement two methods. These requirements are set so that each Plugin will conform to the Sageworks infrastructure; if the required attributes and methods aren’t included in the class definition, errors will be raised during tests and at runtime.
```

### Comparing `sageworks-0.5.4/docs/plugins/plugin_api_changes.md` & `sageworks-0.6.0/docs/plugins/plugin_api_changes.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/docs/repl/index.md` & `sageworks-0.6.0/docs/repl/index.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/docs/research/eda.md` & `sageworks-0.6.0/docs/research/eda.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/docs/research/htg.md` & `sageworks-0.6.0/docs/research/htg.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/examples/datasource_query.py` & `sageworks-0.6.0/examples/datasource/datasource_query.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/examples/datasource_stats.py` & `sageworks-0.6.0/examples/datasource/datasource_stats.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/examples/endpoint_inference.py` & `sageworks-0.6.0/examples/endpoint/endpoint_inference.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/examples/featureset_eda.py` & `sageworks-0.6.0/examples/featureset/featureset_eda.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/examples/featureset_query.py` & `sageworks-0.6.0/examples/featureset/featureset_query.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/examples/full_ml_pipeline.py` & `sageworks-0.6.0/examples/full_ml_pipeline.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/examples/glue_hello_world.py` & `sageworks-0.6.0/examples/glue/glue_hello_world.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/examples/glue_hello_world_with_log.py` & `sageworks-0.6.0/examples/glue/glue_hello_world_with_log.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/examples/glue_load_s3_bucket.py` & `sageworks-0.6.0/examples/glue/glue_load_s3_bucket.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/examples/meta_model_metrics.py` & `sageworks-0.6.0/examples/meta/meta_model_metrics.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/examples/model_metrics.py` & `sageworks-0.6.0/examples/model/model_metrics.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/examples/monitor_usage.py` & `sageworks-0.6.0/examples/monitor/monitor_usage.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/examples/plugins/pages/my_plugin_page.py` & `sageworks-0.6.0/examples/plugins/pages/my_plugin_page.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/examples/plugins/pages/plugin_page_1.py` & `sageworks-0.6.0/examples/plugins/pages/plugin_page_1.py`

 * *Files 17% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         self.page_name = "Hello World"
 
     def page_setup(self, app: dash.Dash):
         """Required function to set up the page"""
 
         # Register this page with Dash and set up the layout (required)
         register_page(
-            __name__,
+            __file__,
             path="/plugin_1",
             name=self.page_name,
             layout=self.page_layout(),
         )
 
     def page_layout(self) -> dash.html.Div:
         """Set up the layout for the page"""
@@ -30,27 +30,27 @@
 
 
 # Unit Test for your Plugin Page
 if __name__ == "__main__":
     import webbrowser
 
     # Create our Dash Application
-    app = dash.Dash(
+    my_app = dash.Dash(
         __name__,
         title="SageWorks Dashboard",
         use_pages=True,
         pages_folder="",
         external_stylesheets=[dbc.themes.DARKLY],
     )
 
     # For Multi-Page Applications, we need to create a 'page container' to hold all the pages
-    app.layout = html.Div([page_container])
+    my_app.layout = html.Div([page_container])
 
     # Create the Plugin Page and call page_setup
     plugin_page = PluginPage1()
-    plugin_page.page_setup(app)
+    plugin_page.page_setup(my_app)
 
     # Open the browser to the plugin page
     webbrowser.open("http://localhost:8000/plugin_1")
 
     # Note: This 'main' is purely for running/testing locally
-    app.run(host="0.0.0.0", port=8000, debug=True)
+    my_app.run(host="localhost", port=8000, debug=True)
```

### Comparing `sageworks-0.5.4/examples/plugins/pages/plugin_page_2.py` & `sageworks-0.6.0/examples/plugins/pages/plugin_page_2.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # SageWorks Imports
 from sageworks.web_components import table
 from sageworks.api.meta import Meta
 
 
 class PluginPage2:
-    """Plugin Page:  A SageWorks Plugin Web Interface"""
+    """Plugin Page: A SageWorks Plugin Page Interface"""
 
     def __init__(self):
         """Initialize the Plugin Page"""
         self.page_name = "Hello World"
         self.models_table = table.Table()
         self.table_component = None
         self.meta = Meta()
@@ -23,17 +23,17 @@
         """Required function to set up the page"""
 
         # Create a table to display the models
         self.table_component = self.models_table.create_component(
             "my_model_table", header_color="rgb(60, 60, 60)", row_select="single", max_height=400
         )
 
-        # Register this page with Dash and set up the layout (required)
+        # Register this page with Dash and set up the layout
         register_page(
-            __name__,
+            __file__,
             path="/plugin_2",
             name=self.page_name,
             layout=self.page_layout(),
         )
 
         # Populate the models table with data
         models = self.meta.models()
@@ -54,27 +54,27 @@
 
 
 # Unit Test for your Plugin Page
 if __name__ == "__main__":
     import webbrowser
 
     # Create our Dash Application
-    app = dash.Dash(
+    my_app = dash.Dash(
         __name__,
         title="SageWorks Dashboard",
         use_pages=True,
         pages_folder="",
         external_stylesheets=[dbc.themes.DARKLY],
     )
 
     # For Multi-Page Applications, we need to create a 'page container' to hold all the pages
-    app.layout = html.Div([page_container])
+    my_app.layout = html.Div([page_container])
 
     # Create the Plugin Page and call page_setup
     plugin_page = PluginPage2()
-    plugin_page.page_setup(app)
+    plugin_page.page_setup(my_app)
 
     # Open the browser to the plugin page
     webbrowser.open("http://localhost:8000/plugin_2")
 
     # Note: This 'main' is purely for running/testing locally
-    app.run(host="0.0.0.0", port=8000, debug=True)
+    my_app.run(host="localhost", port=8000, debug=True)
```

### Comparing `sageworks-0.5.4/examples/plugins/pages/plugin_page_3.py` & `sageworks-0.6.0/examples/plugins/pages/plugin_page_3.py`

 * *Files 7% similar despite different names*

```diff
@@ -27,39 +27,39 @@
         self.meta = Meta()
 
     def page_setup(self, app: dash.Dash):
         """Required function to set up the page"""
 
         # Create a table to display the models
         self.table_component = self.models_table.create_component(
-            "my_model_table", header_color="rgb(60, 60, 60)", row_select="single", max_height=400
+            "plugin_3_model_table", header_color="rgb(60, 60, 60)", row_select="single", max_height=400
         )
 
         # Create a model details panel and model plot
-        self.details_component = self.model_details.create_component("my_model_details")
-        self.plot_component = self.model_plot.create_component("my_model_plot")
+        self.details_component = self.model_details.create_component("plugin_3_model_details")
+        self.plot_component = self.model_plot.create_component("plugin_3_model_plot")
 
-        # Register this page with Dash and set up the layout (required)
+        # Register this page with Dash and set up the layout
         register_page(
-            __name__,
+            __file__,
             path="/plugin_3",
             name=self.page_name,
             layout=self.page_layout(),
         )
 
         # Populate the models table with data
         models = self.meta.models()
         models["uuid"] = models["Model Group"]
         models["id"] = range(len(models))
         self.table_component.columns = self.models_table.column_setup(models)
         self.table_component.data = models.to_dict("records")
 
         # Register the callbacks
-        self.register_callbacks()
-        self.model_details.register_callbacks("my_model_table")
+        self.register_app_callbacks(app)
+        self.model_details.register_callbacks("plugin_3_model_table")
 
     def page_layout(self) -> dash.html.Div:
         """Set up the layout for the page"""
         layout = dash.html.Div(
             children=[
                 dash.html.H1(self.page_name),
                 dbc.Row(self.table_component),
@@ -69,59 +69,57 @@
                         dbc.Col(self.plot_component, width=7),
                     ]
                 ),
             ]
         )
         return layout
 
-    def register_callbacks(self):
+    def register_app_callbacks(self, app: dash.Dash):
         """Register the callbacks for the page"""
 
-        @callback(
-            Output("my_model_plot", "figure"),
-            Input("my_model_details-dropdown", "value"),
-            [State("my_model_table", "data"), State("my_model_table", "derived_viewport_selected_row_ids")],
+        @app.callback(
+            Output("plugin_3_model_plot", "figure"),
+            [
+                Input("plugin_3_model_details-dropdown", "value"),
+                Input("plugin_3_model_table", "derived_viewport_selected_row_ids"),
+            ],
+            State("plugin_3_model_table", "data"),
             prevent_initial_call=True,
         )
-        def generate_model_plot_figure(inference_run, table_data, selected_rows):
+        def generate_model_plot_figure(inference_run, selected_rows, table_data):
             # Check for no selected rows
             if not selected_rows or selected_rows[0] is None:
                 return no_update
 
             # Get the selected row data and grab the uuid
             selected_row_data = table_data[selected_rows[0]]
             model_uuid = selected_row_data["uuid"]
             model = Model(model_uuid, legacy=True)
 
             # Model Details Markdown component
-            model_plot_fig = self.model_plot.update_contents(model, inference_run)
+            model_plot_fig = self.model_plot.update_properties(model, inference_run)
 
             # Return the details/markdown for these data details
             return model_plot_fig
 
 
 # Unit Test for your Plugin Page
 if __name__ == "__main__":
     import webbrowser
 
     # Create our Dash Application
-    app = dash.Dash(
-        __name__,
-        title="SageWorks Dashboard",
-        use_pages=True,
-        pages_folder="",
-        external_stylesheets=[dbc.themes.DARKLY],
-        suppress_callback_exceptions=True,
+    my_app = dash.Dash(
+        __name__, title="SageWorks Dashboard", use_pages=True, pages_folder="", external_stylesheets=[dbc.themes.DARKLY]
     )
 
     # For Multi-Page Applications, we need to create a 'page container' to hold all the pages
-    app.layout = html.Div([page_container])
+    my_app.layout = html.Div([page_container])
 
     # Create the Plugin Page and call page_setup
     plugin_page = PluginPage3()
-    plugin_page.page_setup(app)
+    plugin_page.page_setup(my_app)
 
     # Open the browser to the plugin page
     webbrowser.open("http://localhost:8000/plugin_3")
 
     # Note: This 'main' is purely for running/testing locally
-    app.run(host="0.0.0.0", port=8000, debug=True)
+    my_app.run(host="localhost", port=8000, debug=True)
```

### Comparing `sageworks-0.5.4/examples/plugins/views/model_plugin_view.py` & `sageworks-0.6.0/examples/plugins/views/model_plugin_view.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/examples/plugins/views/my_view_plugin.py` & `sageworks-0.6.0/examples/plugins/views/my_view_plugin.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/examples/plugins/web_components/custom_plugin.py` & `sageworks-0.6.0/examples/plugins/web_components/endpoint_plugin.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,55 +1,62 @@
-"""A Custom plugin component"""
+"""An example Endpoint plugin component"""
 
+import logging
 from dash import dcc
-import plotly.graph_objects as go
 
 
 # SageWorks Imports
 from sageworks.web_components.plugin_interface import PluginInterface, PluginPage, PluginInputType
-from sageworks.api.model import Model
+from sageworks.api.endpoint import Endpoint
 
 
-class CustomPlugin(PluginInterface):
-    """CustomPlugin Component"""
+# Get the SageWorks logger
+log = logging.getLogger("sageworks")
+
+
+class MyEndpointPlugin(PluginInterface):
+    """MyEndpointPlugin Component"""
 
     """Initialize this Plugin Component Class with required attributes"""
-    plugin_page = PluginPage.CUSTOM
-    plugin_input_type = PluginInputType.MODEL
+    auto_load_page = PluginPage.ENDPOINT
+    plugin_input_type = PluginInputType.ENDPOINT
 
     def create_component(self, component_id: str) -> dcc.Graph:
         """Create a CustomPlugin Component without any data.
         Args:
             component_id (str): The ID of the web component
         Returns:
             dcc.Graph: The EndpointTurbo Component
         """
-        return dcc.Graph(id=component_id, figure=self.display_text("Waiting for Data..."))
+        self.component_id = component_id
+        self.container = dcc.Graph(id=component_id, figure=self.display_text("Waiting for Data..."))
 
-    def update_contents(self, model: Model) -> go.Figure:
-        """Create a CustomPlugin Figure
-        Args:
-            model (Model): An instantiated Endpoint object
-        Returns:
-            go.Figure: A Plotly Figure object
-        """
-        model_name = f"Model: {model.uuid}"
-        return self.display_text(model_name)
+        # Fill in plugin properties
+        self.properties = [(self.component_id, "figure")]
 
+        # Return the container
+        return self.container
 
-if __name__ == "__main__":
-    # This class takes in a model object
+    def update_properties(self, endpoint: Endpoint, **kwargs) -> list:
+        """Create a Endpoint Plugin Figure
 
-    # Instantiate an Endpoint
-    my_model = Model("abalone-regression")
+        Args:
+            endpoint (Endpoint): An instantiated Endpoint object
+            **kwargs: Additional keyword arguments (unused)
 
-    # Instantiate the EndpointTurbo class
-    plugin = CustomPlugin()
+        Returns:
+            list: A list of the updated property values for the plugin
+        """
+        log.important(f"Updating Model Plugin with Model: {endpoint.uuid} and kwargs: {kwargs}")
+        endpoint_name = f"Endpoint: {endpoint.uuid}"
+        text_figure = self.display_text(endpoint_name, figure_height=100)
 
-    # Generate the figure
-    fig = plugin.update_contents(my_model)
+        # Return the updated property values
+        return [text_figure]
 
-    # Apply dark theme
-    fig.update_layout(template="plotly_dark")
 
-    # Show the figure
-    fig.show()
+if __name__ == "__main__":
+    # A Unit Test for the Plugin
+    from sageworks.web_components.plugin_unit_test import PluginUnitTest
+
+    # Run the Unit Test on the Plugin
+    PluginUnitTest(MyEndpointPlugin, test_type="endpoint").run()
```

### Comparing `sageworks-0.5.4/examples/plugins/web_components/endpoint_turbo.py` & `sageworks-0.6.0/examples/plugins/web_components/endpoint_turbo.py`

 * *Files 17% similar despite different names*

```diff
@@ -9,37 +9,44 @@
 from sageworks.api.endpoint import Endpoint
 
 
 class EndpointTurbo(PluginInterface):
     """EndpointTurbo Component"""
 
     """Initialize this Plugin Component Class with required attributes"""
-    plugin_page = PluginPage.ENDPOINT
+    auto_load_page = PluginPage.ENDPOINT
     plugin_input_type = PluginInputType.ENDPOINT
 
     def create_component(self, component_id: str) -> dcc.Graph:
         """Create a EndpointTurbo Component without any data.
         Args:
             component_id (str): The ID of the web component
         Returns:
             dcc.Graph: The EndpointTurbo Component
         """
-        return dcc.Graph(id=component_id, figure=self.display_text("Waiting for Data..."))
+        self.component_id = component_id
+        self.container = dcc.Graph(id=component_id, figure=self.display_text("Waiting for Data..."))
+
+        # Fill in plugin properties
+        self.properties = [(self.component_id, "figure")]
+
+        # Return the container
+        return self.container
+
+    def update_properties(self, endpoint: Endpoint, **kwargs) -> list:
+        """Update the properties for the plugin.
 
-    def update_contents(self, endpoint: Endpoint) -> go.Figure:
-        """Create a EndpointTurbo Figure for the numeric columns in the dataframe.
         Args:
-            endpoint (Endpoint): An instantiated Endpoint object
+            endpoint (Endpoint): An instantiated Model object
+            **kwargs: Additional keyword arguments (unused)
+
         Returns:
-            go.Figure: A Plotly Figure object
+            list: A list of the updated property values for the plugin
         """
 
-        # Just to make sure we have the right endpoint object
-        print(endpoint.summary())
-
         data = [  # Portfolio (inner donut)
             # Inner ring
             go.Pie(
                 values=[20, 40],
                 labels=["Reds", "Blues"],
                 domain={"x": [0.05, 0.45], "y": [0.2, 0.8]},
                 hole=0.5,
@@ -78,31 +85,22 @@
                 sort=False,
                 marker={"colors": ["#668866", "#779977", "#EEA540", "#FFC060"]},
                 showlegend=False,
             ),
         ]
 
         # Create the nested pie chart plot with custom settings
-        fig = go.Figure(data=data)
-        fig.update_layout(margin={"t": 10, "b": 10, "r": 10, "l": 10, "pad": 10}, height=400)
+        endpoint_name = f"Endpoint: {endpoint.uuid}"
+        turbo_figure = go.Figure(data=data)
+        turbo_figure.update_layout(
+            margin={"t": 30, "b": 10, "r": 10, "l": 10, "pad": 10}, title=endpoint_name, height=400
+        )
 
-        return fig
+        # Return the updated property values
+        return [turbo_figure]
 
 
 if __name__ == "__main__":
-    # This class takes in model details and generates a EndpointTurbo
-    from sageworks.api.endpoint import Endpoint
-
-    # Instantiate an Endpoint
-    end = Endpoint("abalone-regression-end")
-
-    # Instantiate the EndpointTurbo class
-    pie = EndpointTurbo()
-
-    # Generate the figure
-    fig = pie.update_contents(end)
-
-    # Apply dark theme
-    fig.update_layout(template="plotly_dark")
+    from sageworks.web_components.plugin_unit_test import PluginUnitTest
 
-    # Show the figure
-    fig.show()
+    # Run the Unit Test on the Plugin
+    PluginUnitTest(EndpointTurbo).run()
```

### Comparing `sageworks-0.5.4/examples/plugins/web_components/model_plugin.py` & `sageworks-0.6.0/examples/plugins/web_components/model_markdown.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,63 +1,84 @@
-"""An Example Model plugin component"""
+"""A Markdown Plugin Example for details/information about Models"""
 
-from dash import dcc
-import plotly.graph_objects as go
-import random
+import logging
 
+# Dash Imports
+from dash import html, dcc
 
 # SageWorks Imports
+from sageworks.api import Model
 from sageworks.web_components.plugin_interface import PluginInterface, PluginPage, PluginInputType
-from sageworks.api.model import Model
 
+# Get the SageWorks logger
+log = logging.getLogger("sageworks")
 
-class MyModelPlugin(PluginInterface):
-    """MyModelPlugin Component"""
+
+class MyModelMarkdown(PluginInterface):
+    """MyModelMarkdown Component"""
 
     """Initialize this Plugin Component Class with required attributes"""
-    plugin_page = PluginPage.MODEL
+    auto_load_page = PluginPage.MODEL
     plugin_input_type = PluginInputType.MODEL
 
-    def create_component(self, component_id: str) -> dcc.Graph:
-        """Create a EndpointTurbo Component without any data.
+    def create_component(self, component_id: str) -> html.Div:
+        """Create a Model Markdown Component without any data
+
         Args:
             component_id (str): The ID of the web component
         Returns:
             dcc.Graph: The EndpointTurbo Component
         """
-        return dcc.Graph(id=component_id, figure=self.display_text("Waiting for Data..."))
+        self.component_id = component_id
+        self.container = html.Div(
+            id=self.component_id,
+            children=[
+                html.H3(id=f"{self.component_id}-header", children="Model: Loading..."),
+                dcc.Markdown(id=f"{self.component_id}-details"),
+            ],
+        )
+
+        # Fill in plugin properties
+        self.properties = [
+            (f"{self.component_id}-header", "children"),
+            (f"{self.component_id}-details", "children"),
+        ]
+
+        # Return the container
+        return self.container
+
+    def update_properties(self, model: Model, **kwargs) -> list:
+        """Update the properties for this plugin component
 
-    def update_contents(self, model: Model) -> go.Figure:
-        """Create a Figure for the plugin.
         Args:
             model (Model): An instantiated Model object
+            **kwargs: Additional keyword arguments (unused)
+
         Returns:
-            go.Figure: A Plotly Figure object
+            list: A list of the updated property values for the plugin
         """
-        model_name = f"Model: {model.uuid}"
-
-        # Generate random values for the pie chart
-        pie_values = [random.randint(10, 30) for _ in range(3)]
+        log.important(f"Updating Model Markdown Plugin with Model: {model.uuid} and kwargs: {kwargs}")
 
-        # Create a pie chart with the endpoint name as the title
-        fig = go.Figure(data=[go.Pie(labels=["A", "B", "C"], values=pie_values)], layout=go.Layout(title=model_name))
-        return fig
+        # Update the html header
+        header = f"Model: {model.uuid}"
 
+        # Make Markdown for the model summary
+        summary = model.summary()
+        markdown = ""
+        for key, value in summary.items():
 
-if __name__ == "__main__":
-    # This class takes in model details and generates a pie chart
-    from sageworks.api.model import Model
+            # Chop off the "sageworks_" prefix
+            key = key.replace("sageworks_", "")
 
-    # Instantiate an Endpoint
-    model = Model("abalone-regression")
+            # Add to markdown string
+            markdown += f"**{key}:** {value}  \n"
 
-    # Instantiate the EndpointTurbo class
-    my_plugin = MyModelPlugin()
+        # Return the updated property values for the plugin
+        return [header, markdown]
 
-    # Generate the figure
-    fig = my_plugin.update_contents(model)
 
-    # Apply dark theme
-    fig.update_layout(template="plotly_dark")
+# Unit Test for the Plugin
+if __name__ == "__main__":
+    from sageworks.web_components.plugin_unit_test import PluginUnitTest
 
-    # Show the figure
-    fig.show()
+    # Run the Unit Test on the Plugin
+    PluginUnitTest(MyModelMarkdown).run()
```

### Comparing `sageworks-0.5.4/examples/sagemaker_pipelines/all_steps.py` & `sageworks-0.6.0/examples/storage/sagemaker_pipelines/all_steps.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/examples/sagemaker_pipelines/ml_pipeline.py` & `sageworks-0.6.0/examples/storage/sagemaker_pipelines/ml_pipeline.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/examples/sagemaker_pipelines/storage/full_pipeline_experiment/data_source.py` & `sageworks-0.6.0/examples/storage/sagemaker_pipelines/storage/full_pipeline_experiment/data_source.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/examples/sagemaker_pipelines/storage/full_pipeline_experiment/ml_pipeline.py` & `sageworks-0.6.0/examples/storage/sagemaker_pipelines/storage/full_pipeline_experiment/ml_pipeline.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/examples/storage/data_to_data.py` & `sageworks-0.6.0/examples/storage/data_to_data.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/examples/storage/data_to_features.py` & `sageworks-0.6.0/examples/storage/data_to_features.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/examples/storage/endpoint_inference.py` & `sageworks-0.6.0/examples/storage/endpoint_inference.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/examples/storage/hello_world_pipeline.py` & `sageworks-0.6.0/examples/storage/hello_world_pipeline.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/examples/storage/plugin_page_example.py` & `sageworks-0.6.0/examples/storage/plugin_page_example.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,8 +117,8 @@
 
             # Get the selected row data and grab the uuid
             selected_row_data = table_data[selected_rows[0]]
             model_uuid = selected_row_data["uuid"]
 
             # Instantiate the Model and send it to the plugin
             model = Model(model_uuid)
-            return plugin.update_contents(model)
+            return plugin.update_properties(model)
```

### Comparing `sageworks-0.5.4/mkdocs.yml` & `sageworks-0.6.0/mkdocs.yml`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
   - API Classes: 
     - OverView: api_classes/overview.md
     - Meta: api_classes/meta.md
     - DataSource: api_classes/data_source.md
     - FeatureSet: api_classes/feature_set.md
     - Model: api_classes/model.md
     - Endpoint: api_classes/endpoint.md
+    - Pipelines: api_classes/pipelines.md
     - Monitor: api_classes/monitor.md
   - Core Classes: 
     - OverView: core_classes/overview.md
     - Artifacts: 
       - OverView: core_classes/artifacts/overview.md
       - AthenaSource: core_classes/artifacts/athena_source.md
       - FeatureSetCore: core_classes/artifacts/feature_set_core.md
```

### Comparing `sageworks-0.5.4/notebooks/ML_Pipeline_with_SageWorks.ipynb` & `sageworks-0.6.0/notebooks/ML_Pipeline_with_SageWorks.ipynb`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/notebooks/ML_Pipeline_with_SageWorks_2.ipynb` & `sageworks-0.6.0/notebooks/ML_Pipeline_with_SageWorks_2.ipynb`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/notebooks/Outliers_in_SageWorks.ipynb` & `sageworks-0.6.0/notebooks/Outliers_in_SageWorks.ipynb`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/notebooks/images/athena_query_aqsol.png` & `sageworks-0.6.0/notebooks/images/athena_query_aqsol.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/notebooks/images/aws_dashboard_aqsol.png` & `sageworks-0.6.0/notebooks/images/aws_dashboard_aqsol.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/notebooks/images/dashboard_aqsol_features.png` & `sageworks-0.6.0/notebooks/images/dashboard_aqsol_features.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/notebooks/images/model_screenshot.png` & `sageworks-0.6.0/notebooks/images/model_screenshot.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/notebooks/images/sageworks_concepts.png` & `sageworks-0.6.0/notebooks/images/sageworks_concepts.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/notebooks/images/scp_labs.png` & `sageworks-0.6.0/notebooks/images/scp_labs.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/scripts/athena_ddl_mixed_case.py` & `sageworks-0.6.0/scripts/athena_ddl_mixed_case.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/scripts/copy_data_catalog_db.py` & `sageworks-0.6.0/scripts/copy_data_catalog_db.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/scripts/delete_redis_keys.py` & `sageworks-0.6.0/scripts/delete_redis_keys.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/scripts/glue_mixed_case.py` & `sageworks-0.6.0/scripts/glue_mixed_case.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/scripts/model_endpoint_sanity_check.py` & `sageworks-0.6.0/scripts/model_endpoint_sanity_check.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/scripts/onboard_endpoints.py` & `sageworks-0.6.0/scripts/onboard_endpoints.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/scripts/onboard_models.py` & `sageworks-0.6.0/scripts/onboard_models.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/scripts/storage/dns_data_to_features.py` & `sageworks-0.6.0/scripts/storage/dns_data_to_features.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/scripts/storage/generate_jsonl_data.py` & `sageworks-0.6.0/scripts/storage/generate_jsonl_data.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/scripts/test_feature_resolution.py` & `sageworks-0.6.0/scripts/test_feature_resolution.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/setup.cfg` & `sageworks-0.6.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/setup.py` & `sageworks-0.6.0/setup.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/src/sageworks/__init__.py` & `sageworks-0.6.0/src/sageworks/__init__.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/src/sageworks/algorithms/dataframe/aggregation.py` & `sageworks-0.6.0/src/sageworks/algorithms/dataframe/aggregation.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/src/sageworks/algorithms/dataframe/data_source_eda.py` & `sageworks-0.6.0/src/sageworks/algorithms/dataframe/data_source_eda.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/src/sageworks/algorithms/dataframe/dimensionality_reduction.py` & `sageworks-0.6.0/src/sageworks/algorithms/dataframe/dimensionality_reduction.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/src/sageworks/algorithms/dataframe/feature_resolution.py` & `sageworks-0.6.0/src/sageworks/algorithms/dataframe/feature_resolution.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/src/sageworks/algorithms/dataframe/feature_spider.py` & `sageworks-0.6.0/src/sageworks/algorithms/dataframe/feature_spider.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/src/sageworks/algorithms/dataframe/row_tagger.py` & `sageworks-0.6.0/src/sageworks/algorithms/dataframe/row_tagger.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/src/sageworks/algorithms/spark/Readme.md` & `sageworks-0.6.0/src/sageworks/algorithms/spark/Readme.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/src/sageworks/algorithms/sql/Readme.md` & `sageworks-0.6.0/src/sageworks/algorithms/sql/Readme.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/src/sageworks/algorithms/sql/column_stats.py` & `sageworks-0.6.0/src/sageworks/algorithms/sql/column_stats.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/src/sageworks/algorithms/sql/correlations.py` & `sageworks-0.6.0/src/sageworks/algorithms/sql/correlations.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/src/sageworks/algorithms/sql/descriptive_stats.py` & `sageworks-0.6.0/src/sageworks/algorithms/sql/descriptive_stats.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/src/sageworks/algorithms/sql/outliers.py` & `sageworks-0.6.0/src/sageworks/algorithms/sql/outliers.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/src/sageworks/algorithms/sql/sample_rows.py` & `sageworks-0.6.0/src/sageworks/algorithms/sql/sample_rows.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/src/sageworks/algorithms/sql/value_counts.py` & `sageworks-0.6.0/src/sageworks/algorithms/sql/value_counts.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/src/sageworks/api/__init__.py` & `sageworks-0.6.0/src/sageworks/api/__init__.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/src/sageworks/api/data_source.py` & `sageworks-0.6.0/src/sageworks/api/data_source.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/src/sageworks/api/endpoint.py` & `sageworks-0.6.0/src/sageworks/api/endpoint.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/src/sageworks/api/feature_set.py` & `sageworks-0.6.0/src/sageworks/api/feature_set.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/src/sageworks/api/meta.py` & `sageworks-0.6.0/src/sageworks/api/meta.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 
 # SageWorks Imports
 from sageworks.aws_service_broker.aws_account_clamp import AWSAccountClamp
 from sageworks.aws_service_broker.aws_service_broker import AWSServiceBroker, ServiceCategory
 from sageworks.utils.config_manager import ConfigManager
 from sageworks.utils.datetime_utils import datetime_string
 from sageworks.utils.aws_utils import num_columns_ds, num_columns_fs, aws_url
+from sageworks.api.pipeline_manager import PipelineManager
 
 
 class Meta:
     """Meta: A class that provides Metadata for a broad set of AWS Artifacts
 
     Common Usage:
     ```
@@ -33,14 +34,17 @@
         self.log = logging.getLogger("sageworks")
 
         # Account and Service Brokers
         self.aws_account_clamp = AWSAccountClamp()
         self.aws_broker = AWSServiceBroker()
         self.cm = ConfigManager()
 
+        # Pipeline Manager
+        self.pipeline_manager = PipelineManager()
+
     def account(self) -> dict:
         """Print out the AWS Account Info
 
         Returns:
             dict: The AWS Account Info
         """
         return self.aws_account_clamp.get_aws_account_info()
@@ -340,26 +344,44 @@
             refresh (bool, optional): Force a refresh of the metadata. Defaults to False.
 
         Returns:
             dict: A summary of the Endpoints in AWS
         """
         return self.aws_broker.get_metadata(ServiceCategory.ENDPOINTS, force_refresh=refresh)
 
+    def pipelines(self, refresh: bool = False) -> pd.DataFrame:
+        """Get a summary of the SageWorks Pipelines
+
+        Args:
+            refresh (bool, optional): Force a refresh of the metadata. Defaults to False.
+
+        Returns:
+            pd.DataFrame: A summary of the SageWorks Pipelines
+        """
+        data = self.pipeline_manager.list_pipelines()
+
+        # Return the pipelines summary as a DataFrame
+        return pd.DataFrame(data)
+
     def _remove_sageworks_meta(self, data: dict) -> dict:
         """Internal: Recursively remove any keys with 'sageworks_' in them"""
 
         # Recursively exclude any keys with 'sageworks_' in them
         summary_data = {}
         for key, value in data.items():
             if isinstance(value, dict):
                 summary_data[key] = self._remove_sageworks_meta(value)
             elif not key.startswith("sageworks_"):
                 summary_data[key] = value
         return summary_data
 
+    def refresh_all_aws_meta(self) -> None:
+        """Force a refresh of all the metadata"""
+        self.aws_broker.get_all_metadata(force_refresh=True)
+
 
 if __name__ == "__main__":
     """Exercise the SageWorks Meta Class"""
     from pprint import pprint
 
     # Create the class
     meta = Meta()
@@ -396,14 +418,18 @@
     print("\n\n*** Models ***")
     pprint(meta.models())
 
     # Get the Endpoints
     print("\n\n*** Endpoints ***")
     pprint(meta.endpoints())
 
+    # Get the Pipelines
+    print("\n\n*** Pipelines ***")
+    pprint(meta.pipelines())
+
     # Now do a deep dive on all the Artifacts
     print("\n\n#")
     print("# Deep Dives ***")
     print("#")
 
     # Get the Data Sources
     print("\n\n*** Data Sources ***")
```

### Comparing `sageworks-0.5.4/src/sageworks/api/model.py` & `sageworks-0.6.0/src/sageworks/api/model.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,40 +1,42 @@
 """Model: Manages AWS Model Package/Group creation and management.
+
 Models are automatically set up and provisioned for deployment into AWS.
 Models can be viewed in the AWS Sagemaker interfaces or in the SageWorks
-Dashboard UI, which provides additional model details and performance metrics"""
+Dashboard UI, which provides additional model details and performance metrics
+"""
 
 # SageWorks Imports
 from sageworks.core.artifacts.artifact import Artifact
 from sageworks.core.artifacts.model_core import ModelCore, ModelType  # noqa: F401
 from sageworks.core.transforms.model_to_endpoint.model_to_endpoint import ModelToEndpoint
 from sageworks.api.endpoint import Endpoint
 
 
 class Model(ModelCore):
-    """Model: SageWorks Model API Class
+    """Model: SageWorks Model API Class.
 
     Common Usage:
         ```
         my_features = Model(name)
         my_features.details()
         my_features.to_endpoint()
         ```
     """
 
     def details(self, **kwargs) -> dict:
-        """Model Details
+        """Retrieve the Model Details.
 
         Returns:
             dict: A dictionary of details about the Model
         """
         return super().details(**kwargs)
 
     def to_endpoint(self, name: str = None, tags: list = None, serverless: bool = True) -> Endpoint:
-        """Create an Endpoint from the Model
+        """Create an Endpoint from the Model.
 
         Args:
             name (str): Set the name for the endpoint. If not specified, an automatic name will be generated
             tags (list): Set the tags for the endpoint. If not specified automatic tags will be generated.
             serverless (bool): Set the endpoint to be serverless (default: True)
 
         Returns:
```

### Comparing `sageworks-0.5.4/src/sageworks/api/monitor.py` & `sageworks-0.6.0/src/sageworks/api/monitor.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/src/sageworks/aws_service_broker/aws_account_clamp.py` & `sageworks-0.6.0/src/sageworks/aws_service_broker/aws_account_clamp.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/src/sageworks/aws_service_broker/aws_service_broker.py` & `sageworks-0.6.0/src/sageworks/aws_service_broker/aws_service_broker.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/src/sageworks/aws_service_broker/aws_service_connectors/connector.py` & `sageworks-0.6.0/src/sageworks/aws_service_broker/aws_service_connectors/connector.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/src/sageworks/aws_service_broker/aws_service_connectors/data_catalog.py` & `sageworks-0.6.0/src/sageworks/aws_service_broker/aws_service_connectors/data_catalog.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/src/sageworks/aws_service_broker/aws_service_connectors/endpoints.py` & `sageworks-0.6.0/src/sageworks/aws_service_broker/aws_service_connectors/endpoints.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/src/sageworks/aws_service_broker/aws_service_connectors/feature_store.py` & `sageworks-0.6.0/src/sageworks/aws_service_broker/aws_service_connectors/feature_store.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/src/sageworks/aws_service_broker/aws_service_connectors/glue_jobs.py` & `sageworks-0.6.0/src/sageworks/aws_service_broker/aws_service_connectors/glue_jobs.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/src/sageworks/aws_service_broker/aws_service_connectors/model_registry.py` & `sageworks-0.6.0/src/sageworks/aws_service_broker/aws_service_connectors/model_registry.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/src/sageworks/aws_service_broker/aws_service_connectors/s3_bucket.py` & `sageworks-0.6.0/src/sageworks/aws_service_broker/aws_service_connectors/s3_bucket.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/src/sageworks/core/artifacts/__init__.py` & `sageworks-0.6.0/src/sageworks/core/artifacts/__init__.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/src/sageworks/core/artifacts/artifact.py` & `sageworks-0.6.0/src/sageworks/core/artifacts/artifact.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/src/sageworks/core/artifacts/athena_source.py` & `sageworks-0.6.0/src/sageworks/core/artifacts/athena_source.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/src/sageworks/core/artifacts/data_source_abstract.py` & `sageworks-0.6.0/src/sageworks/core/artifacts/data_source_abstract.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/src/sageworks/core/artifacts/data_source_factory.py` & `sageworks-0.6.0/src/sageworks/core/artifacts/data_source_factory.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/src/sageworks/core/artifacts/endpoint_core.py` & `sageworks-0.6.0/src/sageworks/core/artifacts/endpoint_core.py`

 * *Files 2% similar despite different names*

```diff
@@ -723,22 +723,26 @@
             pd.DataFrame: DataFrame with the confusion matrix
         """
 
         y_true = prediction_df[target_column]
         prediction_col = "prediction" if "prediction" in prediction_df.columns else "predictions"
         y_pred = prediction_df[prediction_col]
 
-        # Compute the confusion matrix
-        conf_mtx = confusion_matrix(y_true, y_pred)
+        # Special case for low, medium, high classes
+        if (set(y_true) | set(y_pred)) == {"low", "medium", "high"}:
+            labels = ["low", "medium", "high"]
+        else:
+            labels = sorted(list(set(y_true) | set(y_pred)))
 
-        # Get unique labels
-        labels = sorted(list(set(y_true) | set(y_pred)))
+        # Compute the confusion matrix
+        conf_mtx = confusion_matrix(y_true, y_pred, labels=labels)
 
         # Create a DataFrame
         conf_mtx_df = pd.DataFrame(conf_mtx, index=labels, columns=labels)
+        conf_mtx_df.index.name = "labels"
         return conf_mtx_df
 
     def endpoint_config_name(self) -> str:
         # Grab the Endpoint Config Name from the AWS
         details = self.sm_client.describe_endpoint(EndpointName=self.endpoint_name)
         return details["EndpointConfigName"]
```

### Comparing `sageworks-0.5.4/src/sageworks/core/artifacts/feature_set_core.py` & `sageworks-0.6.0/src/sageworks/core/artifacts/feature_set_core.py`

 * *Files 2% similar despite different names*

```diff
@@ -235,41 +235,60 @@
             str: The full path/file for the CSV file created by Feature Store create_dataset()
         """
 
         # Set up the S3 Query results path
         date_time = datetime.now(timezone.utc).strftime("%Y-%m-%d_%H:%M:%S")
         s3_output_path = self.feature_sets_s3_path + f"/{self.uuid}/datasets/all_{date_time}"
 
+        # Get the training data query
+        query = self.get_training_data_query()
+
+        # Make the query
+        athena_query = FeatureGroup(name=self.uuid, sagemaker_session=self.sm_session).athena_query()
+        athena_query.run(query, output_location=s3_output_path)
+        athena_query.wait()
+        query_execution = athena_query.get_query_execution()
+
+        # Get the full path to the S3 files with the results
+        full_s3_path = s3_output_path + f"/{query_execution['QueryExecution']['QueryExecutionId']}.csv"
+        return full_s3_path
+
+    def get_training_data_query(self) -> str:
+        """Get the training data query for this FeatureSet
+
+        Returns:
+            str: The training data query for this FeatureSet
+        """
+
         # Do we have a training view?
         training_view = self.get_training_view_table()
         if training_view:
-            self.log.important(f"Creating S3 Training Data from Training View {training_view}...")
+            self.log.important(f"Pulling Data from Training View {training_view}...")
             table_name = training_view
         else:
             self.log.warning(f"No Training View found for {self.uuid}, using FeatureSet directly...")
             table_name = self.athena_table
 
         # Make a query that gets all the data from the FeatureSet
-        query = f"SELECT * FROM {table_name}"
+        return f"SELECT * FROM {table_name}"
 
-        """
-        Note: We're going to circle back to this
-        # Get the snapshot query
-        query = self.snapshot_query(table_name=table_name)
+    def get_training_data(self, limit=50000) -> pd.DataFrame:
+        """Get the training data for this FeatureSet
+
+        Args:
+            limit (int): The number of rows to limit the query to (default: 1000)
+        Returns:
+            pd.DataFrame: The training data for this FeatureSet
         """
 
-        # Make the query
-        athena_query = FeatureGroup(name=self.uuid, sagemaker_session=self.sm_session).athena_query()
-        athena_query.run(query, output_location=s3_output_path)
-        athena_query.wait()
-        query_execution = athena_query.get_query_execution()
+        # Get the training data query (put a limit on it for now)
+        query = self.get_training_data_query() + f" LIMIT {limit}"
 
-        # Get the full path to the S3 files with the results
-        full_s3_path = s3_output_path + f"/{query_execution['QueryExecution']['QueryExecutionId']}.csv"
-        return full_s3_path
+        # Make the query
+        return self.query(query)
 
     def snapshot_query(self, table_name: str = None) -> str:
         """An Athena query to get the latest snapshot of features
 
         Args:
             table_name (str): The name of the table to query (default: None)
 
@@ -403,68 +422,68 @@
             END AS training
             FROM {self.athena_table}
             """
 
         # Execute the CREATE VIEW query
         self.data_source.execute_statement(create_view_query)
 
-    def create_training_view(self, id_column: str, hold_out_ids: list[str]):
+    def create_training_view(self, id_column: str, holdout_ids: list[str]):
         """Create a view in Athena that marks hold out ids for this FeatureSet
 
         Args:
             id_column (str): The name of the id column in the output DataFrame.
-            hold_out_ids (list[str]): The list of hold out ids.
+            holdout_ids (list[str]): The list of hold out ids.
         """
 
         # Create the view name
         view_name = f"{self.athena_table}_training"
         self.log.important(f"Creating Training View {view_name}...")
 
         # Format the list of hold out ids for SQL IN clause
-        if hold_out_ids and all(isinstance(id, str) for id in hold_out_ids):
-            formatted_hold_out_ids = ", ".join(f"'{id}'" for id in hold_out_ids)
+        if holdout_ids and all(isinstance(id, str) for id in holdout_ids):
+            formatted_holdout_ids = ", ".join(f"'{id}'" for id in holdout_ids)
         else:
-            formatted_hold_out_ids = ", ".join(map(str, hold_out_ids))
+            formatted_holdout_ids = ", ".join(map(str, holdout_ids))
 
         # Construct the CREATE VIEW query
         create_view_query = f"""
         CREATE OR REPLACE VIEW {view_name} AS
         SELECT *, CASE
-            WHEN {id_column} IN ({formatted_hold_out_ids}) THEN 0
+            WHEN {id_column} IN ({formatted_holdout_ids}) THEN 0
             ELSE 1
         END AS training
         FROM {self.athena_table}
         """
 
         # Execute the CREATE VIEW query
         self.data_source.execute_statement(create_view_query)
 
-    def set_hold_out_ids(self, id_column: str, hold_out_ids: list[str]):
+    def set_holdout_ids(self, id_column: str, holdout_ids: list[str]):
         """Set the hold out ids for this FeatureSet
 
         Args:
             id_column (str): The name of the id column in the output DataFrame.
-            hold_out_ids (list[str]): The list of hold out ids.
+            holdout_ids (list[str]): The list of hold out ids.
         """
-        self.create_training_view(id_column, hold_out_ids)
+        self.create_training_view(id_column, holdout_ids)
 
-    def get_hold_out_ids(self, id_column: str) -> list[str]:
+    def get_holdout_ids(self, id_column: str) -> list[str]:
         """Get the hold out ids for this FeatureSet
 
         Args:
             id_column (str): The name of the id column in the output DataFrame.
 
         Returns:
             list[str]: The list of hold out ids.
         """
         training_view_table = self.get_training_view_table(create=False)
         if training_view_table is not None:
             query = f"SELECT {id_column} FROM {training_view_table} WHERE training = 0"
-            hold_out_ids = self.query(query)[id_column].tolist()
-            return hold_out_ids
+            holdout_ids = self.query(query)[id_column].tolist()
+            return holdout_ids
         else:
             return []
 
     def get_training_view_table(self, create: bool = True) -> Union[str, None]:
         """Get the name of the training view for this FeatureSet
         Args:
             create (bool): Create the training view if it doesn't exist (default=True)
@@ -698,27 +717,27 @@
     print("Creating default training view...")
     my_features.create_default_training_view()
 
     # Test the hold out set functionality with ints
     print("Setting hold out ids...")
     table = my_features.get_training_view_table()
     df = my_features.query(f"SELECT id, name FROM {table}")
-    my_hold_out_ids = [id for id in df["id"] if id < 20]
-    my_features.create_training_view("id", my_hold_out_ids)
+    my_holdout_ids = [id for id in df["id"] if id < 20]
+    my_features.create_training_view("id", my_holdout_ids)
 
     # Convenience methods to set and get the hold out ids
     print("Setting hold out ids...")
-    my_features.set_hold_out_ids("id", my_hold_out_ids)
+    my_features.set_holdout_ids("id", my_holdout_ids)
     print("Getting hold out ids...")
-    hold_output = my_features.get_hold_out_ids("id")
-    print(hold_output)
-    assert set(hold_output) == set(my_hold_out_ids)
+    holdoutput = my_features.get_holdout_ids("id")
+    print(holdoutput)
+    assert set(holdoutput) == set(my_holdout_ids)
 
     # Test the hold out set functionality with strings
     print("Setting hold out ids (strings)...")
-    my_hold_out_ids = [name for name in df["name"] if int(name.split(" ")[1]) > 80]
-    my_features.create_training_view("name", my_hold_out_ids)
+    my_holdout_ids = [name for name in df["name"] if int(name.split(" ")[1]) > 80]
+    my_features.create_training_view("name", my_holdout_ids)
 
     # Now delete the AWS artifacts associated with this Feature Set
     # print('Deleting SageWorks Feature Set...')
     # my_features.delete()
     print("Done")
```

### Comparing `sageworks-0.5.4/src/sageworks/core/artifacts/model_core.py` & `sageworks-0.6.0/src/sageworks/core/artifacts/model_core.py`

 * *Files 2% similar despite different names*

```diff
@@ -373,14 +373,15 @@
         storage_key = f"model:{self.uuid}:details"
         cached_details = self.data_storage.get(storage_key)
         if cached_details and not recompute:
             return cached_details
 
         self.log.info("Recomputing Model Details...")
         details = self.summary()
+        details["pipeline"] = self.get_pipeline()
         details["model_type"] = self.model_type.value
         details["model_package_group_arn"] = self.group_arn()
         details["model_package_arn"] = self.model_package_arn()
         aws_meta = self.aws_meta()
         details["description"] = aws_meta.get("ModelPackageDescription", "-")
         details["version"] = aws_meta["ModelPackageVersion"]
         details["status"] = aws_meta["ModelPackageStatus"]
@@ -410,14 +411,27 @@
 
         # Cache the details
         self.data_storage.set(storage_key, details)
 
         # Return the details
         return details
 
+    # Pipeline for this model
+    def get_pipeline(self) -> str:
+        """Get the pipeline for this model"""
+        return self.sageworks_meta().get("sageworks_pipeline")
+
+    def set_pipeline(self, pipeline: str):
+        """Set the pipeline for this model
+
+        Args:
+            pipeline (str): Pipeline that was used to create this model
+        """
+        self.upsert_sageworks_meta({"sageworks_pipeline": pipeline})
+
     def expected_meta(self) -> list[str]:
         """Metadata we expect to see for this Model when it's ready
         Returns:
             list[str]: List of expected metadata keys
         """
         # Our current list of expected metadata, we can add to this as needed
         return ["sageworks_status", "sageworks_training_metrics", "sageworks_training_cm"]
```

### Comparing `sageworks-0.5.4/src/sageworks/core/artifacts/monitor_core.py` & `sageworks-0.6.0/src/sageworks/core/artifacts/monitor_core.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/src/sageworks/core/transforms/Readme.md` & `sageworks-0.6.0/src/sageworks/core/transforms/Readme.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/src/sageworks/core/transforms/data_loaders/heavy/s3_heavy_to_data_source.py` & `sageworks-0.6.0/src/sageworks/core/transforms/data_loaders/heavy/s3_heavy_to_data_source.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/src/sageworks/core/transforms/data_loaders/light/__init__.py` & `sageworks-0.6.0/src/sageworks/core/transforms/data_loaders/light/__init__.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/src/sageworks/core/transforms/data_loaders/light/csv_to_data_source.py` & `sageworks-0.6.0/src/sageworks/core/transforms/data_loaders/light/csv_to_data_source.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/src/sageworks/core/transforms/data_loaders/light/json_to_data_source.py` & `sageworks-0.6.0/src/sageworks/core/transforms/data_loaders/light/json_to_data_source.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/src/sageworks/core/transforms/data_loaders/light/s3_to_data_source_light.py` & `sageworks-0.6.0/src/sageworks/core/transforms/data_loaders/light/s3_to_data_source_light.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/src/sageworks/core/transforms/data_to_data/light/clean_data.py` & `sageworks-0.6.0/src/sageworks/core/transforms/data_to_data/light/clean_data.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/src/sageworks/core/transforms/data_to_data/light/data_to_data_light.py` & `sageworks-0.6.0/src/sageworks/core/transforms/data_to_data/light/data_to_data_light.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/src/sageworks/core/transforms/data_to_features/heavy/chunk/data_to_features_chunk.py` & `sageworks-0.6.0/src/sageworks/core/transforms/data_to_features/heavy/chunk/data_to_features_chunk.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/src/sageworks/core/transforms/data_to_features/heavy/storage/data_to_features_heavy_old.py` & `sageworks-0.6.0/src/sageworks/core/transforms/data_to_features/heavy/storage/data_to_features_heavy_old.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/src/sageworks/core/transforms/data_to_features/light/data_to_features_light.py` & `sageworks-0.6.0/src/sageworks/core/transforms/data_to_features/light/data_to_features_light.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/src/sageworks/core/transforms/data_to_features/light/molecular_descriptors.py` & `sageworks-0.6.0/src/sageworks/core/transforms/data_to_features/light/molecular_descriptors.py`

 * *Files 18% similar despite different names*

```diff
@@ -55,19 +55,36 @@
     def transform_impl(self, **kwargs):
         """Compute a Feature Set based on RDKit Descriptors"""
 
         # Check the input DataFrame has the required columns
         if "smiles" not in self.input_df.columns:
             raise ValueError("Input DataFrame must have a 'smiles' column")
 
+        # There are certain smiles that cause Mordred to crash
+        # We'll replace them with 'equivalent' smiles (these need to be verified)
+        self.input_df["smiles"] = self.input_df["smiles"].replace(
+            "[O-]C([O-])=O.[NH4+]CCO.[NH4+]CCO", "[O]C([O])=O.[N]CCO.[N]CCO"
+        )
+        self.input_df["smiles"] = self.input_df["smiles"].replace(
+            "[NH4+]CCO.[NH4+]CCO.[O-]C([O-])=O", "[N]CCO.[N]CCO.[O]C([O])=O"
+        )
+        self.input_df["smiles"] = self.input_df["smiles"].replace(
+            "O=S(=O)(Nn1c-nnc1)C1=CC=CC=C1", "O=S(=O)(NN(C=N1)C=N1)C(C=CC1)=CC=1"
+        )
+
         # Compute/add all the Molecular Descriptors
         self.output_df = self.compute_molecular_descriptors(self.input_df)
 
+        # Get the columns that are descriptors
+        desc_columns = set(self.output_df.columns) - set(self.input_df.columns)
+
         # Drop any NaNs (and INFs)
-        self.output_df = pandas_utils.drop_nans(self.output_df, how="all")
+        current_rows = self.output_df.shape[0]
+        self.output_df = pandas_utils.drop_nans(self.output_df, how="any", subset=desc_columns)
+        self.log.warning(f"Dropped {current_rows - self.output_df.shape[0]} NaN rows")
 
     def compute_molecular_descriptors(self, process_df: pd.DataFrame) -> pd.DataFrame:
         """Compute and add all the Molecular Descriptors
         Args:
             process_df(pd.DataFrame): The DataFrame to process and generate RDKit Descriptors
         Returns:
             pd.DataFrame: The input DataFrame with all the RDKit Descriptors added
```

### Comparing `sageworks-0.5.4/src/sageworks/core/transforms/features_to_model/features_to_model.py` & `sageworks-0.6.0/src/sageworks/core/transforms/features_to_model/features_to_model.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/src/sageworks/core/transforms/features_to_model/light_model_harness/xgb_model.template` & `sageworks-0.6.0/src/sageworks/core/transforms/features_to_model/light_model_harness/xgb_model.template`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/src/sageworks/core/transforms/model_to_endpoint/model_to_endpoint.py` & `sageworks-0.6.0/src/sageworks/core/transforms/model_to_endpoint/model_to_endpoint.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/src/sageworks/core/transforms/pandas_transforms/__init__.py` & `sageworks-0.6.0/src/sageworks/core/transforms/pandas_transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/src/sageworks/core/transforms/pandas_transforms/data_to_pandas.py` & `sageworks-0.6.0/src/sageworks/core/transforms/pandas_transforms/data_to_pandas.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/src/sageworks/core/transforms/pandas_transforms/features_to_pandas.py` & `sageworks-0.6.0/src/sageworks/core/transforms/pandas_transforms/features_to_pandas.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/src/sageworks/core/transforms/pandas_transforms/pandas_to_data.py` & `sageworks-0.6.0/src/sageworks/core/transforms/pandas_transforms/pandas_to_data.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/src/sageworks/core/transforms/pandas_transforms/pandas_to_features.py` & `sageworks-0.6.0/src/sageworks/core/transforms/pandas_transforms/pandas_to_features.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/src/sageworks/core/transforms/pandas_transforms/pandas_to_features_chunked.py` & `sageworks-0.6.0/src/sageworks/core/transforms/pandas_transforms/pandas_to_features_chunked.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/src/sageworks/core/transforms/transform.py` & `sageworks-0.6.0/src/sageworks/core/transforms/transform.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/src/sageworks/experiments/view_manager.py` & `sageworks-0.6.0/src/sageworks/experiments/view_manager.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/src/sageworks/repl/sageworks_shell.py` & `sageworks-0.6.0/src/sageworks/repl/sageworks_shell.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     pass
 
 
 # SageWorks Imports
 from sageworks.utils.repl_utils import cprint, Spinner
 from sageworks.utils.sageworks_logging import IMPORTANT_LEVEL_NUM
 from sageworks.utils.config_manager import ConfigManager
+from sageworks.api.meta import Meta
 
 logging.getLogger("sageworks").setLevel(IMPORTANT_LEVEL_NUM)
 
 
 class CustomPromptStyle(Style):
     styles = {
         Token.SageWorks: "#ff69b4",  # Pink color for SageWorks
@@ -72,14 +73,15 @@
 
         # Perform AWS connection test and other checks
         self.commands = dict()
         self.artifacts_text_view = None
         self.aws_status = self.check_aws_account()
         self.redis_status = self.check_redis()
         self.open_source_api_key = self.check_open_source_api_key()
+        self.meta = Meta()
         if self.aws_status:
             self.import_sageworks()
 
         # Set up the Prompt and the IPython shell
         config = InteractiveShellEmbed.instance().config
         config.TerminalInteractiveShell.autocall = 2
         config.TerminalInteractiveShell.prompts_class = SageWorksPrompt
@@ -92,24 +94,26 @@
         self.commands["summary"] = self.summary
         self.commands["incoming_data"] = self.incoming_data
         self.commands["glue_jobs"] = self.glue_jobs
         self.commands["data_sources"] = self.data_sources
         self.commands["feature_sets"] = self.feature_sets
         self.commands["models"] = self.models
         self.commands["endpoints"] = self.endpoints
+        self.commands["pipelines"] = self.pipelines
         self.commands["log_debug"] = self.log_debug
         self.commands["log_info"] = self.log_info
         self.commands["log_important"] = self.log_important
         self.commands["log_warning"] = self.log_warning
+        self.commands["aws_refresh"] = self.aws_refresh
         self.commands["config"] = self.show_config
         self.commands["status"] = self.status_description
 
     def start(self):
         """Start the SageWorks IPython shell"""
-        cprint("magenta", "Welcome to SageWorks!")
+        cprint("magenta", "\nWelcome to SageWorks!")
         if self.aws_status is False:
             cprint("red", "AWS Account Connection Failed...Review/Fix the SageWorks Config:")
             cprint("red", f"Path: {self.cm.site_config_path}")
             self.show_config()
         else:
             self.help()
             self.summary()
@@ -205,14 +209,16 @@
         self.commands["DataSource"] = importlib.import_module("sageworks.api.data_source").DataSource
         self.commands["FeatureSet"] = importlib.import_module("sageworks.api.feature_set").FeatureSet
         self.commands["Model"] = importlib.import_module("sageworks.api.model").Model
         self.commands["ModelType"] = importlib.import_module("sageworks.api.model").ModelType
         self.commands["Endpoint"] = importlib.import_module("sageworks.api.endpoint").Endpoint
         self.commands["Monitor"] = importlib.import_module("sageworks.api.monitor").Monitor
         self.commands["Meta"] = importlib.import_module("sageworks.api.meta").Meta
+        self.commands["Pipeline"] = importlib.import_module("sageworks.api.pipeline").Pipeline
+        self.commands["PipelineManager"] = importlib.import_module("sageworks.api.pipeline_manager").PipelineManager
         self.commands["PluginManager"] = importlib.import_module("sageworks.utils.plugin_manager").PluginManager
 
         # These are 'nice to have' imports
         self.commands["pd"] = importlib.import_module("pandas")
         self.commands["pprint"] = importlib.import_module("pprint").pprint
 
     def help(self, *args):
@@ -237,16 +243,18 @@
         - summary: Show a summary of all the AWS Artifacts
         - incoming_data: List all the incoming S3 data
         - glue_jobs: List all the Glue Jobs in AWS
         - data_sources: List all the DataSources in AWS
         - feature_sets: List all the FeatureSets in AWS
         - models: List all the Models in AWS
         - endpoints: List all the Endpoints in AWS
+        - pipelines: List all the SageWorks Pipelines
         - config: Show the current SageWorks Config
         - status: Show the current SageWorks Status
+        - aws_refresh: Force a refresh of all AWS Meta Data
         - log_(debug/info/important/warning): Set the SageWorks log level
         - exit: Exit SageWorks REPL"""
         return help_msg
 
     def spinner_start(self, text: str, color: str = "lightpurple") -> Spinner:
         # Import all the SageWorks modules
         spinner = Spinner(color, text)
@@ -255,25 +263,38 @@
 
     @staticmethod
     def doc_browser():
         """Open a browser and start the Dash app and open a browser."""
         url = "https://supercowpowers.github.io/sageworks/"
         webbrowser.open(url)
 
+    def aws_refresh(self):
+        """Refresh the AWS Meta Data"""
+        spinner = self.spinner_start("Refreshing AWS Meta Data:")
+        try:
+            self.meta.refresh_all_aws_meta()
+        finally:
+            spinner.stop()
+
     def summary(self):
         cprint("yellow", "\nAWS Artifacts Summary:")
         view_data = self.artifacts_text_view.view_data()
         for name, df in view_data.items():
             # Pad the name to 15 characters
             name = (name + " " * 15)[:15]
 
+            # Sanity check the dataframe
+            if df.empty:
+                examples = ""
+
             # Get the first three items in the first column
-            examples = ", ".join(df.iloc[:, 0].tolist())
-            if len(examples) > 70:
-                examples = examples[:70] + "..."
+            else:
+                examples = ", ".join(df.iloc[:, 0].tolist())
+                if len(examples) > 70:
+                    examples = examples[:70] + "..."
 
             # Print the summary
             cprint(["lightpurple", "\t" + name, "lightgreen", str(df.shape[0]) + "  ", "purple_blue", examples])
 
     def incoming_data(self):
         return self.artifacts_text_view.incoming_data_summary()
 
@@ -288,14 +309,17 @@
 
     def models(self):
         return self.artifacts_text_view.models_summary()
 
     def endpoints(self):
         return self.artifacts_text_view.endpoints_summary()
 
+    def pipelines(self):
+        return self.artifacts_text_view.pipelines_summary()
+
     @staticmethod
     def log_debug():
         logging.getLogger("sageworks").setLevel(logging.DEBUG)
 
     @staticmethod
     def log_info():
         logging.getLogger("sageworks").setLevel(logging.INFO)
```

### Comparing `sageworks-0.5.4/src/sageworks/utils/aws_utils.py` & `sageworks-0.6.0/src/sageworks/utils/aws_utils.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/src/sageworks/utils/cache.py` & `sageworks-0.6.0/src/sageworks/utils/cache.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Cache class for key/value pairs"""
 
 import time
 from collections import OrderedDict
 import atexit
 
 
-class Cache(object):
+class Cache:
     """In process memory cache. Not thread safe.
     Usage:
          cache = Cache(max_size=5, expire=10)
          cache.set('foo', 'bar')
          cache.get('foo')
          > bar
          time.sleep(11)
```

### Comparing `sageworks-0.5.4/src/sageworks/utils/chem_utils.py` & `sageworks-0.6.0/src/sageworks/utils/chem_utils.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/src/sageworks/utils/config_manager.py` & `sageworks-0.6.0/src/sageworks/utils/config_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -311,19 +311,24 @@
                 return self.get_config_from_aws_parameter_store()
             except Exception:
                 self.log.error("Failed to load config from AWS Parameter Store")
                 return self._load_default_config()
 
         # Load site specified configuration file
         try:
+            # Normalize the path
+            self.site_config_path = os.path.normpath(self.site_config_path)
             self.log.info(f"Loading site configuration from {self.site_config_path}...")
             with open(self.site_config_path, "r") as file:
                 return json.load(file)
-        except (FileNotFoundError, json.JSONDecodeError):
-            self.log.error(f"Failed to load config from {self.site_config_path}")
+        except FileNotFoundError:
+            self.log.error(f"Config file not found at {self.site_config_path}. Loading default config.")
+            return self._load_default_config()
+        except json.JSONDecodeError as e:
+            self.log.error(f"Failed to decode JSON from {self.site_config_path}: {e}. Loading default config.")
             return self._load_default_config()
 
     @staticmethod
     def _load_bootstrap_config() -> Dict[str, Any]:
         """Internal: Load the bootstrap configuration from the package resources.
 
         Returns:
```

### Comparing `sageworks-0.5.4/src/sageworks/utils/dashboard_metrics.py` & `sageworks-0.6.0/src/sageworks/utils/dashboard_metrics.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/src/sageworks/utils/datetime_utils.py` & `sageworks-0.6.0/src/sageworks/utils/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/src/sageworks/utils/df_to_endpoint.py` & `sageworks-0.6.0/src/sageworks/utils/df_to_endpoint.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/src/sageworks/utils/docker_utils.py` & `sageworks-0.6.0/src/sageworks/utils/docker_utils.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/src/sageworks/utils/ecs_info.py` & `sageworks-0.6.0/src/sageworks/utils/ecs_info.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/src/sageworks/utils/endpoint_metrics.py` & `sageworks-0.6.0/src/sageworks/utils/endpoint_metrics.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/src/sageworks/utils/endpoint_utils.py` & `sageworks-0.6.0/src/sageworks/utils/endpoint_utils.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/src/sageworks/utils/extract_model_artifact.py` & `sageworks-0.6.0/src/sageworks/utils/extract_model_artifact.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/src/sageworks/utils/glue_utils.py` & `sageworks-0.6.0/src/sageworks/utils/glue_utils.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/src/sageworks/utils/license_manager.py` & `sageworks-0.6.0/src/sageworks/utils/license_manager.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/src/sageworks/utils/markdown_utils.py` & `sageworks-0.6.0/src/sageworks/utils/markdown_utils.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/src/sageworks/utils/pandas_utils.py` & `sageworks-0.6.0/src/sageworks/utils/pandas_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -85,17 +85,23 @@
 
 
 def numeric_stats(df):
     """Simple function to get the numeric stats for a dataframe"""
     return df.describe().round(2).T.drop("count", axis=1)
 
 
-def drop_nans(input_df: pd.DataFrame, how: str = "all", nan_drop_percent: float = 50) -> pd.DataFrame:
-    """Dropping NaNs in rows and columns. Obviously lots of ways to do this, so picked some reasonable defaults,
-    we can certainly change this later with a more formal set of operations and arguments
+def drop_nans(
+    input_df: pd.DataFrame, how: str = "all", nan_drop_percent: float = 50, subset: list = None
+) -> pd.DataFrame:
+    """Dropping NaNs in rows and columns. Optionally, focus on specific columns.
+    Args:
+        input_df (pd.DataFrame): Input data frame.
+        how (str): 'all' to drop rows where all values are NaN, 'any' to drop rows where any value is NaN.
+        nan_drop_percent (float): Percentage threshold to drop columns with missing values exceeding this rate.
+        subset (list): Specific subset of columns to check for NaNs when dropping rows.
     """
 
     # Grab input number of rows
     orig_num_rows = len(input_df)
 
     # First replace any INF/-INF with NaN
     output_df = input_df.replace([np.inf, -np.inf], np.nan)
@@ -107,20 +113,25 @@
 
     # Report on Dropped Columns
     nan_warn_percent = 0
     for name, percent in column_nan_percent.items():
         if percent > nan_warn_percent:
             log.important(f"Column ({name}) has {percent}% NaN Values")
         if percent > nan_drop_percent:
-            log.warning(f"Dropping Column ({name}) with {percent}% NaN Values!")
+            log.warning(f"Column ({name}) with {percent}% NaN Values!")
+
+    # Conditionally drop rows based on NaNs in specified columns
+    if subset is not None:
+        output_df.dropna(axis=0, how=how, subset=subset, inplace=True)
+    else:
+        output_df.dropna(axis=0, how=how, inplace=True)
 
-    # Drop Rows that have NaNs in them
-    output_df.dropna(axis=0, how=how, inplace=True)
     if len(output_df) != orig_num_rows:
-        log.important(f"Dropping {orig_num_rows - len(output_df)} rows that have a NaN in them")
+        dropped_rows = orig_num_rows - len(output_df)
+        log.important(f"Dropping {dropped_rows} rows that have a NaN in them")
         output_df.reset_index(drop=True, inplace=True)
 
     return output_df
 
 
 def drop_duplicates(input_df: pd.DataFrame) -> pd.DataFrame:
     """Drop duplicate rows from a dataframe
@@ -361,14 +372,60 @@
     df = df.reset_index(drop=True)
 
     # Concatenate the new columns with the original DataFrame
     df = pd.concat([df, proba_df], axis=1)
     return df
 
 
+def stratified_split(df, column_name, test_size=0.2, random_state=42):
+    """
+    Stratified train-test split based on a categorical column, including handling NaNs as a separate category.
+
+    Args:
+        df (pd.DataFrame): DataFrame to split
+        column_name (str): Column name to stratify the split on
+        test_size (float): Proportion of the test set
+        random_state (int): Random seed for reproducibility
+
+    Returns:
+        pd.DataFrame, pd.DataFrame: Train and Test DataFrames
+
+    """
+    # Temporarily replace NaNs with a placeholder to treat them as a category
+    df_temp = df.copy()
+    df_temp.loc[:, column_name] = df_temp[column_name].fillna("NaN")  # Use .loc to avoid SettingWithCopyWarning
+
+    # Determine minimum number of samples per group in the test set
+    min_test_samples = 1
+
+    # Calculate the number of samples each group should ideally have in the test set
+    group_counts = df_temp[column_name].value_counts()
+
+    # This ensures at least one sample per group
+    test_counts = (group_counts * test_size).clip(lower=min_test_samples).astype(int)
+
+    # Create a mask to identify test samples
+    test_mask = pd.Series(False, index=df_temp.index)
+
+    # Assign samples to test set ensuring each group has at least one sample
+    grouped = df_temp.groupby(column_name)
+    for name, group in grouped:
+        test_indices = group.sample(n=test_counts[name], random_state=random_state).index
+        test_mask.loc[test_indices] = True
+
+    train_df = df_temp[~test_mask]
+    test_df = df_temp[test_mask]
+
+    # Convert 'NaN' placeholders back to actual NaNs, using .loc to ensure direct modification
+    train_df.loc[:, column_name] = train_df[column_name].replace("NaN", np.nan)
+    test_df.loc[:, column_name] = test_df[column_name].replace("NaN", np.nan)
+
+    return train_df, test_df
+
+
 if __name__ == "__main__":
     """Exercise the Pandas Utility Methods"""
     from sageworks.utils.test_data_generator import TestDataGenerator
 
     # Setup Pandas output options
     pd.set_option("display.max_colwidth", 35)
     pd.set_option("display.max_columns", 15)
```

### Comparing `sageworks-0.5.4/src/sageworks/utils/plugin_manager.py` & `sageworks-0.6.0/src/sageworks/utils/plugin_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -163,15 +163,15 @@
 
         Returns:
             List[Any]: A list of INSTANTIATED plugin classes for the requested page.
         """
         plugin_classes = [
             self.plugins["web_components"][x]
             for x in self.plugins["web_components"]
-            if self.plugins["web_components"][x].plugin_page == plugin_page
+            if self.plugins["web_components"][x].auto_load_page == plugin_page
         ]
         return [x() for x in plugin_classes]
 
     def get_web_plugin(self, plugin_name: str) -> PluginInterface:
         """
         Retrieve a specific web plugin by name
```

### Comparing `sageworks-0.5.4/src/sageworks/utils/redis_cache.py` & `sageworks-0.6.0/src/sageworks/utils/redis_cache.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/src/sageworks/utils/repl_utils.py` & `sageworks-0.6.0/src/sageworks/utils/repl_utils.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/src/sageworks/utils/s3_utils.py` & `sageworks-0.6.0/src/sageworks/utils/s3_utils.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/src/sageworks/utils/sageworks_cache.py` & `sageworks-0.6.0/src/sageworks/utils/sageworks_cache.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/src/sageworks/utils/sageworks_event_bridge.py` & `sageworks-0.6.0/src/sageworks/utils/sageworks_event_bridge.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/src/sageworks/utils/sageworks_logging.py` & `sageworks-0.6.0/src/sageworks/utils/sageworks_logging.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/src/sageworks/utils/sageworks_sqs.py` & `sageworks-0.6.0/src/sageworks/utils/sageworks_sqs.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/src/sageworks/utils/symbols.py` & `sageworks-0.6.0/src/sageworks/utils/symbols.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/src/sageworks/utils/test_data_generator.py` & `sageworks-0.6.0/src/sageworks/utils/test_data_generator.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/src/sageworks/utils/trace_calls.py` & `sageworks-0.6.0/src/sageworks/utils/trace_calls.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/src/sageworks/utils/type_abbrev.py` & `sageworks-0.6.0/src/sageworks/utils/type_abbrev.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/src/sageworks/views/artifacts_text_view.py` & `sageworks-0.6.0/src/sageworks/views/artifacts_text_view.py`

 * *Files 6% similar despite different names*

```diff
@@ -37,14 +37,15 @@
         summary_data = {
             "INCOMING_DATA": self.incoming_data_summary(),
             "GLUE_JOBS": self.glue_jobs_summary(),
             "DATA_SOURCES": self.data_sources_summary(),
             "FEATURE_SETS": self.feature_sets_summary(),
             "MODELS": self.models_summary(),
             "ENDPOINTS": self.endpoints_summary(),
+            "PIPELINES": self.pipelines_summary(),
         }
         return summary_data
 
     def summary(self) -> None:
         """Give a summary of all the Artifact data to stdout"""
         for name, df in self.view_data().items():
             print(f"\n{name}")
@@ -75,14 +76,18 @@
         """Get summary data about the SageWorks Models"""
         return self.meta.models()
 
     def endpoints_summary(self) -> pd.DataFrame:
         """Get summary data about the SageWorks Endpoints"""
         return self.meta.endpoints()
 
+    def pipelines_summary(self) -> pd.DataFrame:
+        """Get summary data about the SageWorks Pipelines"""
+        return self.meta.pipelines()
+
 
 if __name__ == "__main__":
     import time
 
     # Create the class and get the AWS Model Registry details
     artifacts = ArtifactsTextView()
```

### Comparing `sageworks-0.5.4/src/sageworks/views/artifacts_web_view.py` & `sageworks-0.6.0/src/sageworks/views/artifacts_web_view.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/src/sageworks/views/data_source_web_view.py` & `sageworks-0.6.0/src/sageworks/views/data_source_web_view.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/src/sageworks/views/endpoint_web_view.py` & `sageworks-0.6.0/src/sageworks/views/endpoint_web_view.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/src/sageworks/views/feature_set_web_view.py` & `sageworks-0.6.0/src/sageworks/views/feature_set_web_view.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/src/sageworks/views/model_web_view.py` & `sageworks-0.6.0/src/sageworks/views/model_web_view.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/src/sageworks/views/view.py` & `sageworks-0.6.0/src/sageworks/views/view.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/src/sageworks/web_components/color_maps.py` & `sageworks-0.6.0/src/sageworks/web_components/experiments/color_maps.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/src/sageworks/web_components/component_interface.py` & `sageworks-0.6.0/src/sageworks/web_components/component_interface.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,64 +1,77 @@
 """An abstract class that defines the web component interface for SageWorks"""
 
+import logging
 from abc import ABC, abstractmethod
 from typing import Any, Union
+import textwrap
 import re
 from functools import wraps
-import logging
 import plotly.graph_objects as go
-from dash import dcc, html, dash_table
+import pandas as pd
+from dash import dcc
+from dash.development.base_component import Component
 
 # SageWorks Imports
 from sageworks.api import DataSource, FeatureSet, Model, Endpoint
 
+log = logging.getLogger("sageworks")
+
 
 class ComponentInterface(ABC):
     """A Abstract Web Component Interface
     Notes:
       - The 'create_container' method create a gcc.Graph, html.Div, etc
-      - The 'update_contents' method generates the contents (figure, markdown, etc)
+      - The 'update_properties' method generates the property values
     """
 
     log = logging.getLogger("sageworks")
 
-    SageworksObject = Union[DataSource, FeatureSet, Model, Endpoint]
-    ComponentTypes = Union[dcc.Graph, dash_table.DataTable, dcc.Markdown, html.Div]
-    ContentTypes = Union[go.Figure, str]  # str is used for dcc.Markdown
+    SageworksObject = Union[DataSource, FeatureSet, Model, Endpoint, pd.DataFrame]
+
+    def __init__(self):
+        self.component_id = None
+        self.container = None
+        self.properties = []
+        self.signals = []
 
     def __init_subclass__(cls, **kwargs):
         super().__init_subclass__(**kwargs)
 
-        # Automatically apply the error handling decorator to the create_component and update_contents methods
+        # Automatically apply the error handling decorator to the create_component and update_properties methods
         if hasattr(cls, "create_component") and callable(cls.create_component):
             cls.create_component = create_component_handler(cls.create_component)
-        if hasattr(cls, "update_contents") and callable(cls.update_contents):
-            cls.update_contents = update_contents_handler(cls.update_contents)
+        if hasattr(cls, "update_properties") and callable(cls.update_properties):
+            cls.update_properties = update_properties_handler(cls.update_properties)
 
     @abstractmethod
-    def create_component(self, component_id: str, **kwargs: Any) -> ComponentTypes:
+    def create_component(self, component_id: str, **kwargs: Any) -> Component:
         """Create a Dash Component/Container without any data.
+
         Args:
             component_id (str): The ID of the web component
             kwargs (Any): Any additional arguments to pass to the component
+
         Returns:
-            Union[dcc.Graph, dash_table.DataTable, dcc.Markdown, html.Div]: The Dash Web component
+           Component: A Dash Base Component
         """
         pass
 
-    def update_contents(self, data_object: SageworksObject) -> ContentTypes:
-        """Update the contents of the component/container
+    def update_properties(self, data_object: SageworksObject) -> list:
+        """Update the properties of the component/container
+
         Args:
-            data_object (sageworks_object): The instantiated data object for the plugin type.
+            data_object (sageworks_object/dataframe): A SageWorks object or DataFrame
+
         Returns:
-            Union[go.Figure, str]: A Plotly Figure or a Markdown string
+            list: A list of the updated property values for the component
         """
         pass
 
-    def component_id(self) -> str:
+    def generate_component_id(self) -> str:
         """This helper method returns the component ID for the component
         Returns:
             str: An auto generated component ID
         """
 
         # Get the plugin class name
         plugin_class_name = self.__class__.__name__
@@ -102,25 +115,43 @@
     def wrapper(*args, **kwargs):
         try:
             return func(*args, **kwargs)
         except Exception as e:
             # Get the class name of the plugin
             class_name = args[0].__class__.__name__ if args else "UnknownPlugin"
             error_info = f"{class_name} Crashed: {e.__class__.__name__}: {e}"
-            figure = ComponentInterface.display_text(error_info, figure_height=100, font_size=16)
+            error_info = "<br>".join(textwrap.wrap(error_info, width=120))
+            figure = ComponentInterface.display_text(error_info, figure_height=200, font_size=14)
             return dcc.Graph(id="error", figure=figure)
 
     return wrapper
 
 
-def update_contents_handler(func):
+def update_properties_handler(func):
     @wraps(func)
-    def wrapper(*args, **kwargs):
+    def wrapper(self, *args, **kwargs):
         try:
-            return func(*args, **kwargs)
+            return func(self, *args, **kwargs)
         except Exception as e:
             # Get the class name of the plugin
-            class_name = args[0].__class__.__name__ if args else "UnknownPlugin"
+            class_name = self.__class__.__name__
             error_info = f"{class_name} Crashed: {e.__class__.__name__}: {e}"
-            return ComponentInterface.display_text(error_info, figure_height=100, font_size=16)
+            log.critical(error_info)
+            error_info = "<br>".join(textwrap.wrap(error_info, width=120))
+            figure = ComponentInterface.display_text(error_info, figure_height=200, font_size=14)
+
+            # Prepare the error output to match the properties format
+            error_output = []
+            for component_id, property in self.properties:
+                if property == "figure":
+                    error_output.append(figure)
+                elif property in ["children", "value", "data"]:
+                    error_output.append(error_info)
+                elif property == "columnDefs":
+                    error_output.append([{"headerName": "Crash", "field": "Crash"}])
+                elif property == "rowData":
+                    error_output.append([{"Crash": error_info}])
+                else:
+                    error_output.append(None)  # Fallback for other properties
+            return error_output
 
     return wrapper
```

### Comparing `sageworks-0.5.4/src/sageworks/web_components/confusion_matrix.py` & `sageworks-0.6.0/src/sageworks/web_components/confusion_matrix.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         Args:
             component_id (str): The ID of the web component
         Returns:
             dcc.Graph: The Confusion Matrix Component
         """
         return dcc.Graph(id=component_id, figure=self.display_text("Waiting for Data..."))
 
-    def update_contents(self, model: Model, inference_run: str) -> go.Figure:
+    def update_properties(self, model: Model, inference_run: str) -> go.Figure:
         """Create a Confusion Matrix Figure for the numeric columns in the dataframe.
         Args:
             model (Model): Sageworks Model object
             inference_run (str): Inference capture UUID
         Returns:
             plotly.graph_objs.Figure: A Figure object containing the confusion matrix.
         """
@@ -87,14 +87,14 @@
     m = Model("wine-classification")
     inference_run = "training_holdout"
 
     # Instantiate the ConfusionMatrix class
     cm = ConfusionMatrix()
 
     # Generate the figure
-    fig = cm.update_contents(m, inference_run)
+    fig = cm.update_properties(m, inference_run)
 
     # Apply dark theme
     fig.update_layout(template="plotly_dark")
 
     # Show the figure
     fig.show()
```

### Comparing `sageworks-0.5.4/src/sageworks/web_components/correlation_matrix.py` & `sageworks-0.6.0/src/sageworks/web_components/correlation_matrix.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         Args:
             component_id (str): The ID of the web component
         Returns:
             dcc.Graph: The Correlation Matrix Component
         """
         return dcc.Graph(id=component_id, figure=self.display_text("Waiting for Data..."))
 
-    def update_contents(self, data_source_details: dict) -> go.Figure:
+    def update_properties(self, data_source_details: dict) -> go.Figure:
         """Create a Correlation Matrix Figure for the numeric columns in the dataframe.
         Args:
             data_source_details (dict): A dictionary containing DataSource details.
         Returns:
             plotly.graph_objs.Figure: A Figure object containing the correlation matrix.
         """
 
@@ -137,14 +137,14 @@
     ds = DataSource("test_data")
     ds_details = ds.details()
 
     # Instantiate the CorrelationMatrix class
     corr_plot = CorrelationMatrix()
 
     # Generate the figure
-    fig = corr_plot.update_contents(ds_details)
+    fig = corr_plot.update_properties(ds_details)
 
     # Apply dark theme
     fig.update_layout(template="plotly_dark")
 
     # Show the figure
     fig.show()
```

### Comparing `sageworks-0.5.4/src/sageworks/web_components/dashboard_metric_plots.py` & `sageworks-0.6.0/src/sageworks/web_components/experiments/dashboard_metric_plots.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         Args:
             component_id (str): The ID of the web component
         Returns:
             dcc.Graph: The Dashboard Metrics Component
         """
         return dcc.Graph(id=component_id, figure=self.display_text("Waiting for Data..."))
 
-    def update_contents(self, metrics_df: pd.DataFrame) -> go.Figure:
+    def update_properties(self, metrics_df: pd.DataFrame) -> go.Figure:
         """Create a Dashboard Metric Plots Figure.
         Args:
             metrics_df (pd.DataFrame): The dashboard metrics dataframe
         Returns:
             plotly.graph_objs.Figure: A Figure object containing the Dashboard metrics.
         """
 
@@ -72,14 +72,14 @@
     # Grab our Dashboard Metrics
     dashboard_metrics = DashboardMetrics().get_metrics()
 
     # Instantiate the DashboardMetricPlots class
     dashboard_metric_plots = DashboardMetricPlots()
 
     # Generate the figure
-    fig = dashboard_metric_plots.update_contents(dashboard_metrics)
+    fig = dashboard_metric_plots.update_properties(dashboard_metrics)
 
     # Apply dark theme
     fig.update_layout(template="plotly_dark")
 
     # Show the figure
     fig.show()
```

### Comparing `sageworks-0.5.4/src/sageworks/web_components/data_details_markdown.py` & `sageworks-0.6.0/src/sageworks/web_components/data_details_markdown.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/src/sageworks/web_components/endpoint_details.py` & `sageworks-0.6.0/src/sageworks/web_components/endpoint_details.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/src/sageworks/web_components/endpoint_metric_plots.py` & `sageworks-0.6.0/src/sageworks/web_components/endpoint_metric_plots.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         Args:
             component_id (str): The ID of the web component
         Returns:
             dcc.Graph: The Endpoint Metrics Component
         """
         return dcc.Graph(id=component_id, figure=self.display_text("Waiting for Data..."))
 
-    def update_contents(self, endpoint_details: dict) -> go.Figure:
+    def update_properties(self, endpoint_details: dict) -> go.Figure:
         """Create a Endpoint Metrics Figure for the numeric columns in the dataframe.
         Args:
             endpoint_details (dict): The model details dictionary
         Returns:
             plotly.graph_objs.Figure: A Figure object containing the Endpoint metrics.
         """
 
@@ -72,14 +72,14 @@
     end = EndpointCore("abalone-regression-end-rt")
     end_details = end.details(recompute=True)
 
     # Instantiate the EndpointMetricPlots class
     endpoint_metric_plots = EndpointMetricPlots()
 
     # Generate the figure
-    fig = endpoint_metric_plots.update_contents(end_details)
+    fig = endpoint_metric_plots.update_properties(end_details)
 
     # Apply dark theme
     fig.update_layout(template="plotly_dark")
 
     # Show the figure
     fig.show()
```

### Comparing `sageworks-0.5.4/src/sageworks/web_components/experiments/compound_details.py` & `sageworks-0.6.0/src/sageworks/web_components/experiments/compound_details.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/src/sageworks/web_components/experiments/histogram.py` & `sageworks-0.6.0/src/sageworks/web_components/experiments/histogram.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/src/sageworks/web_components/experiments/outlier_plot.py` & `sageworks-0.6.0/src/sageworks/web_components/experiments/outlier_plot.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/src/sageworks/web_components/experiments/scatter_plot.py` & `sageworks-0.6.0/src/sageworks/web_components/experiments/scatter_plot.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/src/sageworks/web_components/line_chart.py` & `sageworks-0.6.0/src/sageworks/web_components/experiments/line_chart.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/src/sageworks/web_components/model_details.py` & `sageworks-0.6.0/src/sageworks/web_components/model_details.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,15 +94,15 @@
 
     def model_summary(self):
         """Construct the markdown string for the model summary
 
         Returns:
             str: A markdown string
         """
-        # Get these fields from the model
+
         # Get these fields from the model
         show_fields = [
             "health_tags",
             "input",
             "sageworks_registered_endpoints",
             "sageworks_model_type",
             "sageworks_tags",
```

### Comparing `sageworks-0.5.4/src/sageworks/web_components/model_plot.py` & `sageworks-0.6.0/src/sageworks/web_components/model_plot.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 class ModelPlot(ComponentInterface):
     """Model Metrics Components"""
 
     def create_component(self, component_id: str) -> dcc.Graph:
         # Initialize an empty plot figure
         return dcc.Graph(id=component_id, figure=self.display_text("Waiting for Data..."))
 
-    def update_contents(self, model: Model, inference_run: str) -> go.Figure:
+    def update_properties(self, model: Model, inference_run: str) -> go.Figure:
         """Create a Model Plot Figure based on the model type.
         Args:
             model (Model): Sageworks Model object
             inference_run (str): Inference run capture UUID
         Returns:
             plotly.graph_objs.Figure: A Figure object containing the model metrics.
         """
@@ -34,17 +34,17 @@
         # If the model details are empty then return a message
         if model_details is None:
             return self.display_text("Model Details are Empty")
 
         # Based on the model type, we'll generate a different plot
         model_type = model_details.get("model_type")
         if model_type == "classifier":
-            return ConfusionMatrix().update_contents(model, inference_run)
+            return ConfusionMatrix().update_properties(model, inference_run)
         elif model_type == "regressor":
-            return RegressionPlot().update_contents(model, inference_run)
+            return RegressionPlot().update_properties(model, inference_run)
         else:
             return self.display_text("Unknown Model Type")
 
 
 if __name__ == "__main__":
     # This class takes in model details and generates a Confusion Matrix
     from sageworks.api.model import Model
@@ -52,14 +52,14 @@
     m = Model("abalone-regression")
     inference_run = "model_training"
 
     # Instantiate the ModelPlot class
     model_plot = ModelPlot()
 
     # Generate the figure
-    fig = model_plot.update_contents(m, inference_run)
+    fig = model_plot.update_properties(m, inference_run)
 
     # Apply dark theme
     fig.update_layout(template="plotly_dark")
 
     # Show the figure
     fig.show()
```

### Comparing `sageworks-0.5.4/src/sageworks/web_components/plugin_interface.py` & `sageworks-0.6.0/src/sageworks/web_components/plugin_interface.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,88 +1,90 @@
 """An abstract class that defines the web component interface for SageWorks"""
 
 from abc import abstractmethod
 from inspect import signature
 from typing import Union, get_args
 from enum import Enum
+from dash.development.base_component import Component
 
 # Local Imports
 from sageworks.web_components.component_interface import ComponentInterface
 
 
 class PluginPage(Enum):
-    """Plugin Page: Specify which page will autoload the plugin (CUSTOM = Don't autoload)"""
+    """Plugin Page: Specify which page will AUTO load the plugin (CUSTOM/NONE = Don't autoload)"""
 
     DATA_SOURCE = "data_source"
     FEATURE_SET = "feature_set"
     MODEL = "model"
     ENDPOINT = "endpoint"
     CUSTOM = "custom"
+    NONE = "none"
 
 
 class PluginInputType(Enum):
     """Plugin Input Type: Specify the type of object that the plugin will receive as input"""
 
     DATA_SOURCE = "data_source"
     FEATURE_SET = "feature_set"
     MODEL = "model"
     ENDPOINT = "endpoint"
+    MODEL_TABLE = "model_table"
 
 
 class PluginInterface(ComponentInterface):
     """A Web Plugin Interface
     Notes:
-      - These methods are ^stateless^, all data should be passed through the
-        arguments and the implementations should not reference 'self' variables
       - The 'create_component' method must be implemented by the child class
-      - The 'update_contents' method must be implemented by the child class
+      - The 'update_properties' method must be implemented by the child class
     """
 
     @abstractmethod
-    def create_component(self, component_id: str) -> ComponentInterface.ComponentTypes:
+    def create_component(self, component_id: str) -> Component:
         """Create a Dash Component without any data.
+
         Args:
             component_id (str): The ID of the web component
+
         Returns:
-            Union[dcc.Graph, dash_table.DataTable, dcc.Markdown, html.Div] The Dash Web component
+           Component: A Dash Base Component
         """
         pass
 
     @abstractmethod
-    def update_contents(
-        self, data_object: ComponentInterface.SageworksObject, **kwargs
-    ) -> ComponentInterface.ContentTypes:
-        """Generate a figure from the data in the given dataframe.
+    def update_properties(self, data_object: ComponentInterface.SageworksObject, **kwargs) -> list:
+        """Update the property values for the plugin component
         Args:
             data_object (sageworks_object): The instantiated data object for the plugin type.
+            **kwargs: Additional keyword arguments (plugins can define their own arguments)
         Returns:
-            Union[go.Figure, str]: A Plotly Figure or a Markdown string
+            list: A list of the updated properties values for the plugin
         """
         pass
 
     #
     # Internal Methods: These methods are used to validate the plugin interface at runtime
     #
     def __init_subclass__(cls, **kwargs):
         super().__init_subclass__(**kwargs)
 
-        # Ensure the subclass defines the required plugin_page and plugin_input_type
-        if not hasattr(cls, "plugin_page") or not isinstance(cls.plugin_page, PluginPage):
-            raise TypeError("Subclasses must define a 'plugin_page' of type PluginPage")
+        # Ensure the subclass defines the required auto_load_page and plugin_input_type
+        if not hasattr(cls, "auto_load_page") or not isinstance(cls.auto_load_page, PluginPage):
+            raise TypeError("Subclasses must define a 'auto_load_page' of type PluginPage")
         if not hasattr(cls, "plugin_input_type") or not isinstance(cls.plugin_input_type, PluginInputType):
             raise TypeError("Subclasses must define a 'plugin_input_type' of type PluginInputType")
 
-    # If any base class method or parameter is missing from a subclass, or if a subclass method parameter is not
-    # correctly typed a call of issubclass(subclass, cls) will return False, allowing runtime checks for plugins
-    # The plugin loader calls issubclass(subclass, cls) to determine if the subclass is a valid plugin
+    # This subclass check ensures that a subclass of PluginInterface has all required attributes, methods,
+    # and signatures. It returns False any thing is incorrect enabling runtime validation for plugins.
+    # The plugin loader uses issubclass(subclass, cls) to verify plugin subclasses.
     @classmethod
     def __subclasshook__(cls, subclass):
         if cls is PluginInterface:
             # Check if the subclass has all the required attributes
-            if not all(hasattr(subclass, attr) for attr in ("plugin_page", "plugin_input_type")):
+            if not all(hasattr(subclass, attr) for attr in ("auto_load_page", "plugin_input_type")):
                 cls.log.warning(f"Subclass {subclass.__name__} is missing required attributes")
                 return False
 
             # Check if the subclass has all the required methods with correct signatures
             required_methods = set(cls.__abstractmethods__)
             for method in required_methods:
                 # Check for the presence of the method
@@ -129,18 +131,28 @@
                 # Check if the actual type is a subtype of any of the expected types
                 if not any(issubclass(actual, exp) for exp in expected_types):
                     return f"Expected argument types {expected_types} do not include the actual argument type {actual}"
             else:
                 # Direct comparison for non-Union types
                 if expected != actual:
                     return f"Expected argument type {expected} does not match actual argument type {actual}"
+
         return None
 
     @classmethod
     def _check_return_type(cls, base_class_method, subclass_method):
-        return_annotation = base_class_method.__annotations__["return"]
-        expected_return_types = get_args(return_annotation)
-        return_type = signature(subclass_method).return_annotation
+        method_name = base_class_method.__name__
+        actual_return_type = subclass_method.__annotations__.get("return", None)
+
+        if actual_return_type is None:
+            return "Missing return type annotation in subclass method."
+
+        if method_name == "create_component":
+            if not issubclass(actual_return_type, Component):
+                return (
+                    f"Incorrect return type for {method_name} (expected Component, got {actual_return_type.__name__})"
+                )
+        elif method_name == "update_properties":
+            if not (actual_return_type == list or (getattr(actual_return_type, "__origin__", None) is list)):
+                return f"Incorrect return type for {method_name} (expected list, got {actual_return_type.__name__})"
 
-        if return_type not in expected_return_types:
-            return f"Incorrect return type (expected one of {expected_return_types}, got {return_type})"
         return None
```

### Comparing `sageworks-0.5.4/src/sageworks/web_components/regression_plot.py` & `sageworks-0.6.0/src/sageworks/web_components/regression_plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 class RegressionPlot(ComponentInterface):
     """Regression Plot Component"""
 
     def create_component(self, component_id: str) -> dcc.Graph:
         # Initialize an empty scatter plot figure
         return dcc.Graph(id=component_id, figure=self.display_text("Waiting for Data..."))
 
-    def update_contents(self, model: Model, inference_run: str = None) -> go.Figure:
+    def update_properties(self, model: Model, inference_run: str = None) -> go.Figure:
         # Get predictions for specific inference
         df = model.predictions(inference_run)
 
         if df is None:
             return self.display_text("No Data")
 
         # Get the name of the actual field value column
@@ -80,14 +80,14 @@
     m = Model("abalone-regression")
     my_inference_run = "model_training"
 
     # Instantiate the ConfusionMatrix class
     reg_plot = RegressionPlot()
 
     # Generate the figure
-    fig = reg_plot.update_contents(m, my_inference_run)
+    fig = reg_plot.update_properties(m, my_inference_run)
 
     # Apply dark theme
     fig.update_layout(template="plotly_dark")
 
     # Show the figure
     fig.show()
```

### Comparing `sageworks-0.5.4/src/sageworks/web_components/table.py` & `sageworks-0.6.0/src/sageworks/web_components/table.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from dash import dash_table
 from dash.dash_table.Format import Format
 import plotly.express as px
 import pandas as pd
 
 # Local imports
-from sageworks.web_components.color_maps import color_map_add_alpha
+from sageworks.web_components.experiments.color_maps import color_map_add_alpha
 
 # SageWorks Imports
 from sageworks.web_components.component_interface import ComponentInterface
 
 
 class Table(ComponentInterface):
     """Data Details Markdown Component"""
```

### Comparing `sageworks-0.5.4/src/sageworks/web_components/violin_plots.py` & `sageworks-0.6.0/src/sageworks/web_components/violin_plots.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         Args:
             component_id (str): The ID of the web component
         Returns:
             dcc.Graph: The Violin Plot Component
         """
         return dcc.Graph(id=component_id, figure=self.display_text("Waiting for Data..."))
 
-    def update_contents(self, df: pd.DataFrame, figure_args: dict, max_plots: int = 40) -> go.Figure:
+    def update_properties(self, df: pd.DataFrame, figure_args: dict, max_plots: int = 40) -> go.Figure:
         """Create a set of violin plots for the numeric columns in the dataframe.
         Args:
             df (pd.DataFrame): The dataframe containing the data.
             figure_args (dict): A dictionary of arguments to pass to the plot object.
                 For violin plot arguments, refer to: https://plotly.com/python/reference/violin/
             max_plots (int): The maximum number of plots to create (default: 40).
         Returns:
@@ -125,15 +125,15 @@
     ds = DataSource("abalone_data")
     smart_sample_rows = ds.smart_sample()
 
     # Instantiate the ViolinPlots class
     v_plots = ViolinPlots()
 
     # Generate the figure
-    fig = v_plots.update_contents(
+    fig = v_plots.update_properties(
         smart_sample_rows,
         figure_args={
             "box_visible": True,
             "meanline_visible": True,
             "showlegend": False,
             "points": "all",
             "spanmode": "hard",
```

### Comparing `sageworks-0.5.4/src/sageworks.egg-info/PKG-INFO` & `sageworks-0.6.0/src/sageworks.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sageworks
-Version: 0.5.4
+Version: 0.6.0
 Summary: SageWorks: A Python WorkBench for creating and deploying AWS SageMaker Models
 Home-page: https://github.com/SuperCowPowers/sageworks
 Author: SuperCowPowers LLC
 Author-email: support@supercowpowers.com
 License: MIT
 Keywords: SageMaker,Machine Learning,AWS,Python,Utilities
 Classifier: Development Status :: 4 - Beta
@@ -81,8 +81,8 @@
 Using SageWorks will minimize the time and manpower needed to incorporate AWS ML into your organization. If your company would like to be a SageWorks Beta Tester, contact us at [sageworks@supercowpowers.com](mailto:sageworks@supercowpowers.com).
 
 ### Contributions
 If you'd like to contribute to the SageWorks project, you're more than welcome. All contributions will fall under the existing project [license](https://github.com/SuperCowPowers/sageworks/blob/main/LICENSE). If you are interested in contributing or have questions please feel free to contact us at [sageworks@supercowpowers.com](mailto:sageworks@supercowpowers.com).
 
 <img align="right" src="docs/images/scp.png" width="180">
 
-® Amazon Web Services, AWS, the Powered by AWS logo, are trademarks of Amazon.com, Inc. or its affiliates.
+® Amazon Web Services, AWS, the Powered by AWS logo, are trademarks of Amazon.com, Inc. or its affiliates
```

### Comparing `sageworks-0.5.4/src/sageworks.egg-info/SOURCES.txt` & `sageworks-0.6.0/src/sageworks.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -100,14 +100,15 @@
 docs/api_classes/data_source.md
 docs/api_classes/endpoint.md
 docs/api_classes/feature_set.md
 docs/api_classes/meta.md
 docs/api_classes/model.md
 docs/api_classes/monitor.md
 docs/api_classes/overview.md
+docs/api_classes/pipelines.md
 docs/aws_setup/aws_access_management.md
 docs/aws_setup/aws_tips_and_tricks.md
 docs/aws_setup/core_stack.md
 docs/aws_setup/dashboard_stack.md
 docs/aws_setup/full_pipeline.md
 docs/concepts/model_monitoring.md
 docs/core_classes/overview.md
@@ -144,71 +145,80 @@
 docs/misc/sageworks_classes_concepts.md
 docs/misc/scp_consulting.md
 docs/plugins/index.md
 docs/plugins/plugin_api_changes.md
 docs/repl/index.md
 docs/research/eda.md
 docs/research/htg.md
-examples/datasource_from_df.py
-examples/datasource_from_s3.py
-examples/datasource_query.py
-examples/datasource_stats.py
-examples/datasource_to_featureset.py
-examples/endpoint_details.py
-examples/endpoint_inference.py
-examples/endpoint_metrics.py
-examples/featureset_eda.py
-examples/featureset_query.py
-examples/featureset_to_model.py
 examples/full_ml_pipeline.py
-examples/glue_hello_world.py
-examples/glue_hello_world_with_log.py
-examples/glue_load_s3_bucket.py
-examples/meta_list_endpoints.py
-examples/meta_list_models.py
-examples/meta_model_metrics.py
-examples/model_metrics.py
-examples/model_to_endpoint.py
-examples/monitor_setup.py
-examples/monitor_usage.py
 examples/ag-grid/hello_world.py
+examples/datasource/datasource_from_df.py
+examples/datasource/datasource_from_s3.py
+examples/datasource/datasource_query.py
+examples/datasource/datasource_stats.py
+examples/datasource/datasource_to_featureset.py
+examples/endpoint/endpoint_details.py
+examples/endpoint/endpoint_inference.py
+examples/endpoint/endpoint_metrics.py
+examples/featureset/featureset_eda.py
+examples/featureset/featureset_query.py
+examples/featureset/featureset_to_model.py
+examples/glue/glue_hello_world.py
+examples/glue/glue_hello_world_with_log.py
+examples/glue/glue_load_s3_bucket.py
+examples/meta/meta_list_endpoints.py
+examples/meta/meta_list_models.py
+examples/meta/meta_model_metrics.py
+examples/model/model_metrics.py
+examples/model/model_to_endpoint.py
+examples/monitor/monitor_setup.py
+examples/monitor/monitor_usage.py
+examples/pipelines/abalone_pipeline_v1.json
+examples/pipelines/abalone_pipeline_v2.json
+examples/pipelines/aqsol_pipeline_v1.json
+examples/pipelines/pipeline_details.py
+examples/pipelines/pipeline_execute.py
+examples/pipelines/pipeline_manager.py
 examples/plugins/pages/my_plugin_page.py
 examples/plugins/pages/plugin_page_1.py
 examples/plugins/pages/plugin_page_2.py
 examples/plugins/pages/plugin_page_3.py
 examples/plugins/views/model_plugin_view.py
 examples/plugins/views/my_view_plugin.py
 examples/plugins/web_components/custom_plugin.py
 examples/plugins/web_components/endpoint_plugin.py
 examples/plugins/web_components/endpoint_turbo.py
+examples/plugins/web_components/model_markdown.py
 examples/plugins/web_components/model_plugin.py
-examples/sagemaker_pipelines/all_steps.py
-examples/sagemaker_pipelines/hello.py
-examples/sagemaker_pipelines/ml_pipeline.py
-examples/sagemaker_pipelines/storage/full_pipeline_experiment/data_source.py
-examples/sagemaker_pipelines/storage/full_pipeline_experiment/endpoint.py
-examples/sagemaker_pipelines/storage/full_pipeline_experiment/feature_set.py
-examples/sagemaker_pipelines/storage/full_pipeline_experiment/ml_pipeline.py
-examples/sagemaker_pipelines/storage/full_pipeline_experiment/model.py
 examples/storage/data_to_data.py
 examples/storage/data_to_features.py
 examples/storage/endpoint_inference.py
 examples/storage/hello_world_pipeline.py
 examples/storage/plugin_page_example.py
+examples/storage/sagemaker_pipelines/all_steps.py
+examples/storage/sagemaker_pipelines/hello.py
+examples/storage/sagemaker_pipelines/ml_pipeline.py
+examples/storage/sagemaker_pipelines/storage/full_pipeline_experiment/data_source.py
+examples/storage/sagemaker_pipelines/storage/full_pipeline_experiment/endpoint.py
+examples/storage/sagemaker_pipelines/storage/full_pipeline_experiment/feature_set.py
+examples/storage/sagemaker_pipelines/storage/full_pipeline_experiment/ml_pipeline.py
+examples/storage/sagemaker_pipelines/storage/full_pipeline_experiment/model.py
 notebooks/ML_Pipeline_with_SageWorks.ipynb
 notebooks/ML_Pipeline_with_SageWorks_2.ipynb
 notebooks/Outliers_in_SageWorks.ipynb
 notebooks/images/athena_query_aqsol.png
 notebooks/images/aws_dashboard_aqsol.png
 notebooks/images/dashboard_aqsol_features.png
 notebooks/images/model_screenshot.png
 notebooks/images/sageworks_concepts.png
 notebooks/images/scp_labs.png
+scripts/ag_table_row_selection.py
 scripts/athena_ddl_mixed_case.py
 scripts/copy_data_catalog_db.py
+scripts/create_glue_workflow_with_trigger.py
 scripts/delete_redis_keys.py
 scripts/glue_mixed_case.py
 scripts/model_endpoint_sanity_check.py
 scripts/onboard_endpoints.py
 scripts/onboard_models.py
 scripts/test_feature_resolution.py
 scripts/storage/dns_data_to_features.py
@@ -241,14 +251,16 @@
 src/sageworks/api/__init__.py
 src/sageworks/api/data_source.py
 src/sageworks/api/endpoint.py
 src/sageworks/api/feature_set.py
 src/sageworks/api/meta.py
 src/sageworks/api/model.py
 src/sageworks/api/monitor.py
+src/sageworks/api/pipeline.py
+src/sageworks/api/pipeline_manager.py
 src/sageworks/aws_service_broker/aws_account_clamp.py
 src/sageworks/aws_service_broker/aws_service_broker.py
 src/sageworks/aws_service_broker/aws_service_connectors/__init__.py
 src/sageworks/aws_service_broker/aws_service_connectors/connector.py
 src/sageworks/aws_service_broker/aws_service_connectors/data_catalog.py
 src/sageworks/aws_service_broker/aws_service_connectors/endpoints.py
 src/sageworks/aws_service_broker/aws_service_connectors/feature_store.py
@@ -261,14 +273,15 @@
 src/sageworks/core/artifacts/athena_source.py
 src/sageworks/core/artifacts/data_source_abstract.py
 src/sageworks/core/artifacts/data_source_factory.py
 src/sageworks/core/artifacts/endpoint_core.py
 src/sageworks/core/artifacts/feature_set_core.py
 src/sageworks/core/artifacts/model_core.py
 src/sageworks/core/artifacts/monitor_core.py
+src/sageworks/core/pipelines/pipeline_executor.py
 src/sageworks/core/transforms/Readme.md
 src/sageworks/core/transforms/__init__.py
 src/sageworks/core/transforms/transform.py
 src/sageworks/core/transforms/data_loaders/__init__.py
 src/sageworks/core/transforms/data_loaders/heavy/__init__.py
 src/sageworks/core/transforms/data_loaders/heavy/s3_heavy_to_data_source.py
 src/sageworks/core/transforms/data_loaders/light/__init__.py
@@ -344,33 +357,38 @@
 src/sageworks/views/artifacts_text_view.py
 src/sageworks/views/artifacts_web_view.py
 src/sageworks/views/data_source_web_view.py
 src/sageworks/views/endpoint_web_view.py
 src/sageworks/views/feature_set_web_view.py
 src/sageworks/views/model_web_view.py
 src/sageworks/views/view.py
-src/sageworks/web_components/color_maps.py
 src/sageworks/web_components/component_interface.py
 src/sageworks/web_components/confusion_matrix.py
 src/sageworks/web_components/correlation_matrix.py
-src/sageworks/web_components/dashboard_metric_plots.py
 src/sageworks/web_components/data_details_markdown.py
 src/sageworks/web_components/endpoint_details.py
 src/sageworks/web_components/endpoint_metric_plots.py
-src/sageworks/web_components/line_chart.py
 src/sageworks/web_components/model_details.py
 src/sageworks/web_components/model_plot.py
 src/sageworks/web_components/plugin_interface.py
+src/sageworks/web_components/plugin_unit_test.py
 src/sageworks/web_components/regression_plot.py
 src/sageworks/web_components/table.py
 src/sageworks/web_components/violin_plots.py
+src/sageworks/web_components/experiments/color_maps.py
 src/sageworks/web_components/experiments/compound_details.py
+src/sageworks/web_components/experiments/dashboard_metric_plots.py
+src/sageworks/web_components/experiments/data_table.py
 src/sageworks/web_components/experiments/histogram.py
+src/sageworks/web_components/experiments/line_chart.py
 src/sageworks/web_components/experiments/outlier_plot.py
+src/sageworks/web_components/experiments/plugin_callbacks.py
 src/sageworks/web_components/experiments/scatter_plot.py
+src/sageworks/web_components/plugins/ag_table.py
+src/sageworks/web_components/plugins/model_details.py
 tests/create_aqsol_artifacts.py
 tests/create_basic_test_artifacts.py
 tests/create_realtime_endpoint.py
 tests/create_training_adjusted_artifacts.py
 tests/create_wine_artifacts.py
 tests/delete_test_artifacts.py
 tests/artifacts/data_source_tests.py
```

### Comparing `sageworks-0.5.4/tests/artifacts/data_source_tests.py` & `sageworks-0.6.0/tests/artifacts/data_source_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/tests/artifacts/endpoint_tests.py` & `sageworks-0.6.0/tests/artifacts/endpoint_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/tests/artifacts/feature_set_tests.py` & `sageworks-0.6.0/tests/artifacts/feature_set_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/tests/artifacts/model_tests.py` & `sageworks-0.6.0/tests/artifacts/model_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/tests/aws_account/aws_account_clamp_tests.py` & `sageworks-0.6.0/tests/aws_account/aws_account_clamp_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/tests/aws_account/aws_service_broker_tests.py` & `sageworks-0.6.0/tests/aws_account/aws_service_broker_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/tests/connectors/data_catalog.py` & `sageworks-0.6.0/tests/connectors/data_catalog.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/tests/connectors/endpoints.py` & `sageworks-0.6.0/tests/connectors/endpoints.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/tests/connectors/feature_store.py` & `sageworks-0.6.0/tests/connectors/feature_store.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/tests/connectors/glue_jobs.py` & `sageworks-0.6.0/tests/connectors/glue_jobs.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/tests/connectors/model_registry.py` & `sageworks-0.6.0/tests/connectors/model_registry.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/tests/connectors/s3_bucket.py` & `sageworks-0.6.0/tests/connectors/s3_bucket.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/tests/create_aqsol_artifacts.py` & `sageworks-0.6.0/tests/create_aqsol_artifacts.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/tests/create_basic_test_artifacts.py` & `sageworks-0.6.0/tests/create_basic_test_artifacts.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/tests/create_realtime_endpoint.py` & `sageworks-0.6.0/tests/create_realtime_endpoint.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/tests/create_training_adjusted_artifacts.py` & `sageworks-0.6.0/tests/create_training_adjusted_artifacts.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
     # Recreate Flag in case you want to recreate the artifacts
     recreate = False
 
     # Create a training view of the test_features
     log.important("Creating training view for abalone_features...")
     fs = FeatureSetCore("abalone_features")
-    fs.create_training_view("id", hold_out_ids=range(100))  # Just the first 100 ids
+    fs.create_training_view("id", holdout_ids=range(100))  # Just the first 100 ids
 
     # Create the abalone_regression Model
     if recreate or not ModelCore("abalone-regression-100").exists():
         features_to_model = FeaturesToModel(
             "abalone_features", "abalone-regression-100", model_type=ModelType.REGRESSOR
         )
         features_to_model.set_output_tags(["abalone", "regression"])
```

### Comparing `sageworks-0.5.4/tests/create_wine_artifacts.py` & `sageworks-0.6.0/tests/create_wine_artifacts.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/tests/delete_test_artifacts.py` & `sageworks-0.6.0/tests/delete_test_artifacts.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,14 +59,18 @@
     if fs.exists():
         print("Deleting abalone_features...")
         fs.delete()
     m = Model("abalone-regression")
     if m.exists():
         print("Deleting abalone-regression model...")
         m.delete()
+    m = Model("abalone-regression-full")
+    if m.exists():
+        print("Deleting abalone-regression-full model...")
+        m.delete()
     end = Endpoint("abalone-regression-end")
     if end.exists():
         print("Deleting abalone-regression-end...")
         end.delete()
     end = Endpoint("abalone-regression-end-rt")
     if end.exists():
         print("Deleting abalone-regression-end-rt...")
```

### Comparing `sageworks-0.5.4/tests/plugin_tests/crashing_plugin.py` & `sageworks-0.6.0/tests/plugin_tests/crashing_plugin.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,42 +2,43 @@
 
 from dash import dcc
 import plotly.graph_objects as go
 
 
 # SageWorks Imports
 from sageworks.web_components.plugin_interface import PluginInterface, PluginPage, PluginInputType
+from sageworks.api.model import Model
 
 
 class CrashingPlugin(PluginInterface):
     """CrashingPlugin Component"""
 
     """Initialize this Plugin Component Class with required attributes"""
-    plugin_page = PluginPage.MODEL
+    auto_load_page = PluginPage.MODEL
     plugin_input_type = PluginInputType.MODEL
 
     def create_component(self, component_id: str) -> dcc.Graph:
         """Create a CrashingPlugin Component without any data.
         Args:
             component_id (str): The ID of the web component
         Returns:
             dcc.Graph: The CrashingPlugin Component
         """
         return dcc.Graph(id=component_id, figure=self.display_text("Waiting for Data..."))
 
-    def update_contents(self, model_details: dict) -> go.Figure:
+    def update_properties(self, model: Model) -> go.Figure:
         """Create a CrashingPlugin Figure for the numeric columns in the dataframe.
         Args:
-            model_details (dict): The model details dictionary (see Model.details())
+            model (Model): A Model Object
         Returns:
             go.Figure: A Figure object containing the confusion matrix.
         """
 
         # This is where the plugin crashes
-        my_bad = model_details["bad_key"]
+        my_bad = model.summary()["bad_key"]
 
         # Create the nested pie chart plot with custom settings
         fig = go.Figure(my_bad)
         fig.update_layout(margin={"t": 10, "b": 10, "r": 10, "l": 10, "pad": 10}, height=400)
 
         return fig
 
@@ -46,14 +47,14 @@
     # This class takes in model details and generates a CrashingPlugin
 
     # Instantiate the CrashingPlugin class
     bad_plugin = CrashingPlugin()
 
     # Generate the figure
     my_model_details = {"key": "value"}
-    fig = bad_plugin.update_contents(my_model_details)
+    fig = bad_plugin.update_properties(my_model_details)
 
     # Apply dark theme
     fig.update_layout(template="plotly_dark")
 
     # Show the figure
     fig.show()
```

### Comparing `sageworks-0.5.4/tests/specific/capital_tests.py` & `sageworks-0.6.0/tests/specific/capital_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/tests/specific/deletion_tests.py` & `sageworks-0.6.0/tests/specific/deletion_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/tests/transforms/data_to_data_tests.py` & `sageworks-0.6.0/tests/transforms/data_to_data_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/tests/transforms/data_to_features_tests.py` & `sageworks-0.6.0/tests/transforms/data_to_features_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/tests/transforms/features_to_model_tests.py` & `sageworks-0.6.0/tests/transforms/features_to_model_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/tests/transforms/model_metrics_tests.py` & `sageworks-0.6.0/tests/transforms/model_metrics_tests.py`

 * *Files 3% similar despite different names*

```diff
@@ -49,15 +49,21 @@
     print("\n\n*** Validation Predictions ***")
     pprint(model_reg.validation_predictions().head())
     pprint(model_class.validation_predictions().head())
 
 
 def test_inference_predictions():
     print("\n\n*** Inference Predictions ***")
+    if model_reg.inference_predictions() is None:
+        print(f"Model {model_reg.uuid} has no inference predictions!")
+        exit(1)
     pprint(model_reg.inference_predictions().head())
+    if model_class.inference_predictions() is None:
+        print(f"Model {model_class.uuid} has no inference predictions!")
+        exit(1)
     pprint(model_class.inference_predictions().head())
 
 
 def test_confusion_matrix():
     print("\n\n*** Confusion Matrix ***")
     pprint(model_reg.confusion_matrix())
     pprint(model_class.confusion_matrix())
```

### Comparing `sageworks-0.5.4/tests/transforms/model_to_endpoint_tests.py` & `sageworks-0.6.0/tests/transforms/model_to_endpoint_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/tests/transforms/pandas_to_data_tests.py` & `sageworks-0.6.0/tests/transforms/pandas_to_data_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.4/tests/web_components/confusion_matrix_test.py` & `sageworks-0.6.0/tests/web_components/confusion_matrix_test.py`

 * *Files 21% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     m = Model("wine-classification")
     inference_run = "training_holdout"
 
     # Instantiate the ConfusionMatrix class
     cm = ConfusionMatrix()
 
     # Generate the figure
-    fig = cm.update_contents(m, inference_run)
+    fig = cm.update_properties(m, inference_run)
 
     # Apply dark theme
     fig.update_layout(template="plotly_dark")
 
     # Show the figure
     fig.show()
```

### Comparing `sageworks-0.5.4/tests/web_components/correlation_matrix_test.py` & `sageworks-0.6.0/tests/web_components/correlation_matrix_test.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     ds = DataSource("test_data")
     ds_details = ds.details()
 
     # Instantiate the CorrelationMatrix class
     corr_plot = CorrelationMatrix()
 
     # Generate the figure
-    fig = corr_plot.update_contents(ds_details)
+    fig = corr_plot.update_properties(ds_details)
 
     # Apply dark theme
     fig.update_layout(template="plotly_dark")
 
     # Show the figure
     fig.show()
```

### Comparing `sageworks-0.5.4/tests/web_components/plugin_interface_test.py` & `sageworks-0.6.0/tests/web_components/plugin_interface_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,42 +9,44 @@
 from sageworks.api.model import Model
 
 
 class CorrectPlugin(PluginInterface):
     """Subclass of PluginInterface with correct inputs and returns."""
 
     """Initialize this Plugin Component Class with required attributes"""
-    plugin_page = PluginPage.MODEL
+    auto_load_page = PluginPage.MODEL
     plugin_input_type = PluginInputType.MODEL
 
+    def __init__(self):
+        self.container = None
+
     def create_component(self, component_id: str) -> dcc.Graph:
         """Create a Confusion Matrix Component without any data.
         Args:
             component_id (str): The ID of the web component
         Returns:
             dcc.Graph: The Confusion Matrix Component
         """
-        return dcc.Graph(id=component_id, figure=self.waiting_figure())
+        self.container = dcc.Graph(id=component_id, figure=self.waiting_figure())
 
-    def update_contents(self, model: Model) -> go.Figure:
+    def update_properties(self, model: Model) -> list:
         """Create a Confusion Matrix Figure for the numeric columns in the dataframe.
         Args:
              model (Model): An instantiated Model object
-        Returns:
-             go.Figure: A Plotly Figure object
         """
-        return PluginInterface.display_text("I'm a good plugin...")
+        text_figure = PluginInterface.display_text("I'm a good plugin...")
+        return [text_figure]
 
 
 class IncorrectMethods(PluginInterface):
     """Subclass of PluginInterface with incorrect methods
-    they have create_component but forgot to implement update_contents"""
+    they have create_component but forgot to implement update_properties"""
 
     """Initialize this Plugin Component Class with required attributes"""
-    plugin_page = PluginPage.MODEL
+    auto_load_page = PluginPage.MODEL
     plugin_input_type = PluginInputType.MODEL
 
     def create_component(self, component_id: str) -> dcc.Graph:
         """Create a Confusion Matrix Component without any data.
         Args:
             component_id (str): The ID of the web component
         Returns:
@@ -53,61 +55,61 @@
         return dcc.Graph(id=component_id, figure=self.waiting_figure())
 
 
 class IncorrectArgTypes(PluginInterface):
     """Subclass of PluginInterface with an incorrectly typed argument."""
 
     """Initialize this Plugin Component Class with required attributes"""
-    plugin_page = PluginPage.MODEL
+    auto_load_page = PluginPage.MODEL
     plugin_input_type = PluginInputType.MODEL
 
     # Component is an incorrectly named keyword argument
     def create_component(self, component_id: str) -> dcc.Graph:
         """Create a Component without any data.
         Args:
             component_id (str): The ID of the web component
         Returns:
             dcc.Graph: A Dash Component
         """
         return dcc.Graph(id=component_id, figure=self.waiting_figure())
 
-    def update_contents(self, model: list) -> go.Figure:
+    def update_properties(self, model: list) -> go.Figure:
         """Create a Plotly Figure
         Args:
             model (list): An incorrect argument type
         Returns:
             go.Figure: A Figure object
         """
         return PluginInterface.display_text("I'm a bad plugin...")
 
 
 class IncorrectReturnType(PluginInterface):
     """Subclass of PluginInterface with incorrect return type."""
 
     """Initialize this Plugin Component Class with required attributes"""
-    plugin_page = PluginPage.MODEL
+    auto_load_page = PluginPage.MODEL
     plugin_input_type = PluginInputType.MODEL
 
     def create_component(self, component_id: str) -> dcc.Graph:
         """Create a Confusion Matrix Component without any data.
         Args:
             component_id (str): The ID of the web component
         Returns:
             dcc.Graph: The Confusion Matrix Component
         """
         return dcc.Graph(id=component_id, figure=self.waiting_figure())
 
-    def update_contents(self, model: Model) -> list:
+    def update_properties(self, model: Model) -> go.Figure:
         """Create a Figure but give the wrong return type.
         Args:
             model (Model): An instantiated Model object
         Returns:
             list: An incorrect return type
         """
-        return [1, 2, 3]  # Incorrect return type
+        return go.Figure()  # Incorrect return type
 
 
 def test_incorrect_methods():
     """Test if incorrect methods are caught by the PluginInterface"""
     subclass_cond = issubclass(IncorrectMethods, PluginInterface)
     print(f"Incorrect Methods is a subclass of PluginInterface?: {subclass_cond}")
     print("\n")
```

### Comparing `sageworks-0.5.4/tox.ini` & `sageworks-0.6.0/tox.ini`

 * *Files identical despite different names*


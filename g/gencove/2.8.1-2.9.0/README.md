# Comparing `tmp/gencove-2.8.1.tar.gz` & `tmp/gencove-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/gencove-2.8.1.tar", last modified: Fri Nov  3 21:24:10 2023, max compression
+gzip compressed data, was "dist/gencove-2.9.0.tar", last modified: Mon Nov 13 17:09:53 2023, max compression
```

## Comparing `gencove-2.8.1.tar` & `gencove-2.9.0.tar`

### file list

```diff
@@ -1,341 +1,344 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-03 21:24:10.000000 gencove-2.8.1/
--rw-r--r--   0 root         (0) root         (0)     2387 2023-11-03 21:24:10.000000 gencove-2.8.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2143 2023-11-03 21:23:38.000000 gencove-2.8.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-03 21:24:10.000000 gencove-2.8.1/gencove/
--rw-rw-rw-   0 root         (0) root         (0)       56 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1264 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/cli.py
--rw-rw-rw-   0 root         (0) root         (0)    35488 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-03 21:24:10.000000 gencove-2.8.1/gencove/command/
--rw-rw-rw-   0 root         (0) root         (0)       61 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6009 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-03 21:24:10.000000 gencove-2.8.1/gencove/command/basespace/
--rw-rw-rw-   0 root         (0) root         (0)       78 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/basespace/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-03 21:24:10.000000 gencove-2.8.1/gencove/command/basespace/autoimports/
--rw-rw-rw-   0 root         (0) root         (0)       92 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/basespace/autoimports/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-03 21:24:10.000000 gencove-2.8.1/gencove/command/basespace/autoimports/autoimport_list/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/basespace/autoimports/autoimport_list/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      793 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/basespace/autoimports/autoimport_list/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     1966 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/basespace/autoimports/autoimport_list/main.py
--rw-rw-rw-   0 root         (0) root         (0)      522 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/basespace/autoimports/autoimport_list/utils.py
--rw-rw-rw-   0 root         (0) root         (0)      343 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/basespace/autoimports/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-03 21:24:10.000000 gencove-2.8.1/gencove/command/basespace/autoimports/create/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/basespace/autoimports/create/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1990 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/basespace/autoimports/create/cli.py
--rw-rw-rw-   0 root         (0) root         (0)      247 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/basespace/autoimports/create/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     2398 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/basespace/autoimports/create/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-03 21:24:10.000000 gencove-2.8.1/gencove/command/basespace/biosamples/
--rw-rw-rw-   0 root         (0) root         (0)       90 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/basespace/biosamples/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-03 21:24:10.000000 gencove-2.8.1/gencove/command/basespace/biosamples/biosamples_list/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/basespace/biosamples/biosamples_list/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      947 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/basespace/biosamples/biosamples_list/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     2212 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/basespace/biosamples/biosamples_list/main.py
--rw-rw-rw-   0 root         (0) root         (0)      547 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/basespace/biosamples/biosamples_list/utils.py
--rw-rw-rw-   0 root         (0) root         (0)      277 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/basespace/biosamples/cli.py
--rw-rw-rw-   0 root         (0) root         (0)      393 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/basespace/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-03 21:24:10.000000 gencove-2.8.1/gencove/command/basespace/projects/
--rw-rw-rw-   0 root         (0) root         (0)       86 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/basespace/projects/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-03 21:24:10.000000 gencove-2.8.1/gencove/command/basespace/projects/basespace_import/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/basespace/projects/basespace_import/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2144 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/basespace/projects/basespace_import/cli.py
--rw-rw-rw-   0 root         (0) root         (0)      235 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/basespace/projects/basespace_import/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     2151 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/basespace/projects/basespace_import/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-03 21:24:10.000000 gencove-2.8.1/gencove/command/basespace/projects/basespace_list/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/basespace/projects/basespace_list/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      634 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/basespace/projects/basespace_list/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     1987 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/basespace/projects/basespace_list/main.py
--rw-rw-rw-   0 root         (0) root         (0)      571 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/basespace/projects/basespace_list/utils.py
--rw-rw-rw-   0 root         (0) root         (0)      358 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/basespace/projects/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     1548 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/common_cli_options.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-03 21:24:10.000000 gencove-2.8.1/gencove/command/download/
--rw-rw-rw-   0 root         (0) root         (0)       99 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/download/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3834 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/download/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     2104 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/download/constants.py
--rw-rw-rw-   0 root         (0) root         (0)      206 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/download/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)    14841 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/download/main.py
--rw-rw-rw-   0 root         (0) root         (0)    10605 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/download/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-03 21:24:10.000000 gencove-2.8.1/gencove/command/files/
--rw-rw-rw-   0 root         (0) root         (0)       79 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/files/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      630 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/files/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     1888 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/files/main.py
--rw-rw-rw-   0 root         (0) root         (0)      390 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/files/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-03 21:24:10.000000 gencove-2.8.1/gencove/command/projects/
--rw-rw-rw-   0 root         (0) root         (0)       75 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/projects/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1970 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/projects/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-03 21:24:10.000000 gencove-2.8.1/gencove/command/projects/create/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/projects/create/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      935 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/projects/create/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     1439 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/projects/create/main.py
--rw-rw-rw-   0 root         (0) root         (0)      505 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/projects/create/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-03 21:24:10.000000 gencove-2.8.1/gencove/command/projects/create_batch/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/projects/create_batch/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1359 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/projects/create_batch/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     2433 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/projects/create_batch/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-03 21:24:10.000000 gencove-2.8.1/gencove/command/projects/create_merged_vcf/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/projects/create_merged_vcf/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      730 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/projects/create_merged_vcf/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     1436 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/projects/create_merged_vcf/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-03 21:24:10.000000 gencove-2.8.1/gencove/command/projects/create_sample_manifest/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/projects/create_sample_manifest/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1015 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/projects/create_sample_manifest/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     2219 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/projects/create_sample_manifest/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-03 21:24:10.000000 gencove-2.8.1/gencove/command/projects/delete/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/projects/delete/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      978 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/projects/delete/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     1709 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/projects/delete/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-03 21:24:10.000000 gencove-2.8.1/gencove/command/projects/delete_samples/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/projects/delete_samples/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1073 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/projects/delete_samples/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     1931 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/projects/delete_samples/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-03 21:24:10.000000 gencove-2.8.1/gencove/command/projects/get_batch/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/projects/get_batch/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      977 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/projects/get_batch/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     2769 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/projects/get_batch/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-03 21:24:10.000000 gencove-2.8.1/gencove/command/projects/get_merged_vcf/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/projects/get_merged_vcf/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1105 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/projects/get_merged_vcf/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     2147 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/projects/get_merged_vcf/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-03 21:24:10.000000 gencove-2.8.1/gencove/command/projects/get_sample_manifests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/projects/get_sample_manifests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1013 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/projects/get_sample_manifests/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     2518 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/projects/get_sample_manifests/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-03 21:24:10.000000 gencove-2.8.1/gencove/command/projects/import_existing_samples/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/projects/import_existing_samples/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1918 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/projects/import_existing_samples/cli.py
--rw-rw-rw-   0 root         (0) root         (0)      295 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/projects/import_existing_samples/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     2191 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/projects/import_existing_samples/main.py
--rw-rw-rw-   0 root         (0) root         (0)      442 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/projects/import_existing_samples/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-03 21:24:10.000000 gencove-2.8.1/gencove/command/projects/list/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/projects/list/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      646 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/projects/list/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     3051 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/projects/list/main.py
--rw-rw-rw-   0 root         (0) root         (0)      699 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/projects/list/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-03 21:24:10.000000 gencove-2.8.1/gencove/command/projects/list_batch_types/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/projects/list_batch_types/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      731 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/projects/list_batch_types/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     2264 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/projects/list_batch_types/main.py
--rw-rw-rw-   0 root         (0) root         (0)      403 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/projects/list_batch_types/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-03 21:24:10.000000 gencove-2.8.1/gencove/command/projects/list_batches/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/projects/list_batches/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      709 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/projects/list_batches/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     2182 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/projects/list_batches/main.py
--rw-rw-rw-   0 root         (0) root         (0)      499 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/projects/list_batches/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-03 21:24:10.000000 gencove-2.8.1/gencove/command/projects/list_pipeline_capabilities/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/projects/list_pipeline_capabilities/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      781 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/projects/list_pipeline_capabilities/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     1668 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/projects/list_pipeline_capabilities/main.py
--rw-rw-rw-   0 root         (0) root         (0)      448 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/projects/list_pipeline_capabilities/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-03 21:24:10.000000 gencove-2.8.1/gencove/command/projects/list_pipelines/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/projects/list_pipelines/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      554 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/projects/list_pipelines/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     1842 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/projects/list_pipelines/main.py
--rw-rw-rw-   0 root         (0) root         (0)      391 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/projects/list_pipelines/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-03 21:24:10.000000 gencove-2.8.1/gencove/command/projects/restore_samples/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/projects/restore_samples/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1159 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/projects/restore_samples/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     1823 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/projects/restore_samples/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-03 21:24:10.000000 gencove-2.8.1/gencove/command/projects/run_prefix/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/projects/run_prefix/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2075 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/projects/run_prefix/cli.py
--rw-rw-rw-   0 root         (0) root         (0)      327 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/projects/run_prefix/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     4918 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/projects/run_prefix/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-03 21:24:10.000000 gencove-2.8.1/gencove/command/projects/samples/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/projects/samples/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1646 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/projects/samples/cli.py
--rw-rw-rw-   0 root         (0) root         (0)      343 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/projects/samples/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     2454 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/projects/samples/main.py
--rw-rw-rw-   0 root         (0) root         (0)      735 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/projects/samples/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-03 21:24:10.000000 gencove-2.8.1/gencove/command/projects/status_merged_vcf/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/projects/status_merged_vcf/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      748 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/projects/status_merged_vcf/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     1813 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/projects/status_merged_vcf/main.py
--rw-rw-rw-   0 root         (0) root         (0)      470 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/projects/status_merged_vcf/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-03 21:24:10.000000 gencove-2.8.1/gencove/command/reports/
--rw-rw-rw-   0 root         (0) root         (0)       62 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/reports/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      322 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/reports/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-03 21:24:10.000000 gencove-2.8.1/gencove/command/reports/monthly_usage/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/reports/monthly_usage/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1450 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/reports/monthly_usage/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     2470 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/reports/monthly_usage/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-03 21:24:10.000000 gencove-2.8.1/gencove/command/reports/project_qc/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/reports/project_qc/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1251 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/reports/project_qc/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     2588 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/reports/project_qc/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-03 21:24:10.000000 gencove-2.8.1/gencove/command/s3_imports/
--rw-rw-rw-   0 root         (0) root         (0)       72 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/s3_imports/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-03 21:24:10.000000 gencove-2.8.1/gencove/command/s3_imports/autoimports/
--rw-rw-rw-   0 root         (0) root         (0)       85 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/s3_imports/autoimports/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-03 21:24:10.000000 gencove-2.8.1/gencove/command/s3_imports/autoimports/autoimport_list/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/s3_imports/autoimports/autoimport_list/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      660 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/s3_imports/autoimports/autoimport_list/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     1744 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/s3_imports/autoimports/autoimport_list/main.py
--rw-rw-rw-   0 root         (0) root         (0)      462 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/s3_imports/autoimports/autoimport_list/utils.py
--rw-rw-rw-   0 root         (0) root         (0)      336 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/s3_imports/autoimports/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-03 21:24:10.000000 gencove-2.8.1/gencove/command/s3_imports/autoimports/create/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/s3_imports/autoimports/create/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1686 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/s3_imports/autoimports/create/cli.py
--rw-rw-rw-   0 root         (0) root         (0)      226 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/s3_imports/autoimports/create/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     2314 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/s3_imports/autoimports/create/main.py
--rw-rw-rw-   0 root         (0) root         (0)      392 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/s3_imports/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-03 21:24:10.000000 gencove-2.8.1/gencove/command/s3_imports/s3_import/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/s3_imports/s3_import/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1523 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/s3_imports/s3_import/cli.py
--rw-rw-rw-   0 root         (0) root         (0)      214 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/s3_imports/s3_import/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     1916 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/s3_imports/s3_import/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-03 21:24:10.000000 gencove-2.8.1/gencove/command/sample_manifests/
--rw-rw-rw-   0 root         (0) root         (0)       80 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/sample_manifests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      296 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/sample_manifests/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-03 21:24:10.000000 gencove-2.8.1/gencove/command/sample_manifests/get_sample_manifest/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/sample_manifests/get_sample_manifest/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      991 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/sample_manifests/get_sample_manifest/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     2181 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/sample_manifests/get_sample_manifest/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-03 21:24:10.000000 gencove-2.8.1/gencove/command/samples/
--rw-rw-rw-   0 root         (0) root         (0)       79 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/samples/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      370 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/samples/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-03 21:24:10.000000 gencove-2.8.1/gencove/command/samples/download_file/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/samples/download_file/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2825 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/samples/download_file/cli.py
--rw-rw-rw-   0 root         (0) root         (0)      141 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/samples/download_file/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     5345 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/samples/download_file/main.py
--rw-rw-rw-   0 root         (0) root         (0)     3051 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/samples/download_file/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-03 21:24:10.000000 gencove-2.8.1/gencove/command/samples/get_metadata/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/samples/get_metadata/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      870 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/samples/get_metadata/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     2348 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/samples/get_metadata/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-03 21:24:10.000000 gencove-2.8.1/gencove/command/samples/set_metadata/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/samples/set_metadata/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      818 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/samples/set_metadata/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     1981 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/samples/set_metadata/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-03 21:24:10.000000 gencove-2.8.1/gencove/command/upload/
--rw-rw-rw-   0 root         (0) root         (0)       97 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/upload/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1973 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/upload/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     1529 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/upload/constants.py
--rw-rw-rw-   0 root         (0) root         (0)      258 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/upload/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)    17222 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/upload/main.py
--rw-rw-rw-   0 root         (0) root         (0)     3028 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/upload/multi_file_reader.py
--rw-rw-rw-   0 root         (0) root         (0)     9443 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/upload/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-03 21:24:10.000000 gencove-2.8.1/gencove/command/uploads/
--rw-rw-rw-   0 root         (0) root         (0)       84 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/uploads/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      213 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/uploads/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-03 21:24:10.000000 gencove-2.8.1/gencove/command/uploads/list/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/uploads/list/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      934 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/uploads/list/cli.py
--rw-rw-rw-   0 root         (0) root         (0)      277 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/uploads/list/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     2113 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/uploads/list/main.py
--rw-rw-rw-   0 root         (0) root         (0)      573 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/uploads/list/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     4334 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-03 21:24:10.000000 gencove-2.8.1/gencove/command/webhook/
--rw-rw-rw-   0 root         (0) root         (0)       72 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/webhook/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      198 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/webhook/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-03 21:24:10.000000 gencove-2.8.1/gencove/command/webhook/verify/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/webhook/verify/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      777 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/webhook/verify/cli.py
--rw-rw-rw-   0 root         (0) root         (0)      999 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/command/webhook/verify/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     4119 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-03 21:24:10.000000 gencove-2.8.1/gencove/description/
--rw-rw-rw-   0 root         (0) root         (0)     1811 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/description/pypi_readme.md
--rw-rw-rw-   0 root         (0) root         (0)      508 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     3205 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/logger.py
--rw-rw-rw-   0 root         (0) root         (0)     8467 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-03 21:24:10.000000 gencove-2.8.1/gencove/tests/
--rw-rw-rw-   0 root         (0) root         (0)       32 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-03 21:24:10.000000 gencove-2.8.1/gencove/tests/basespace/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/tests/basespace/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6374 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/tests/basespace/test_basespace_autoimports_create.py
--rw-rw-rw-   0 root         (0) root         (0)     4249 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/tests/basespace/test_basespace_autoimports_list.py
--rw-rw-rw-   0 root         (0) root         (0)     7257 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/tests/basespace/test_basespace_biosamples_list.py
--rw-rw-rw-   0 root         (0) root         (0)     6334 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/tests/basespace/test_basespace_projects_import.py
--rw-rw-rw-   0 root         (0) root         (0)     5955 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/tests/basespace/test_basespace_projects_list.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-03 21:24:10.000000 gencove-2.8.1/gencove/tests/basespace/vcr/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/tests/basespace/vcr/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5184 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/tests/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)     3328 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/tests/decorators.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-03 21:24:10.000000 gencove-2.8.1/gencove/tests/download/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/tests/download/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    41021 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/tests/download/test_cli_download.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-03 21:24:10.000000 gencove-2.8.1/gencove/tests/download/vcr/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/tests/download/vcr/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      932 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/tests/download/vcr/filters.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-03 21:24:10.000000 gencove-2.8.1/gencove/tests/files/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/tests/files/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4371 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/tests/files/test_file_types_list.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-03 21:24:10.000000 gencove-2.8.1/gencove/tests/files/vcr/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/tests/files/vcr/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5527 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/tests/filters.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-03 21:24:10.000000 gencove-2.8.1/gencove/tests/projects/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/tests/projects/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6781 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/tests/projects/test_projects_batch_get.py
--rw-rw-rw-   0 root         (0) root         (0)     4502 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/tests/projects/test_projects_batch_types_list.py
--rw-rw-rw-   0 root         (0) root         (0)     8945 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/tests/projects/test_projects_batches_create.py
--rw-rw-rw-   0 root         (0) root         (0)     4601 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/tests/projects/test_projects_batches_list.py
--rw-rw-rw-   0 root         (0) root         (0)     4380 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/tests/projects/test_projects_create.py
--rw-rw-rw-   0 root         (0) root         (0)     9108 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/tests/projects/test_projects_create_merged_vcf.py
--rw-rw-rw-   0 root         (0) root         (0)     4693 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/tests/projects/test_projects_create_sample_manifest.py
--rw-rw-rw-   0 root         (0) root         (0)     5626 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/tests/projects/test_projects_delete.py
--rw-rw-rw-   0 root         (0) root         (0)     8901 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/tests/projects/test_projects_delete_samples.py
--rw-rw-rw-   0 root         (0) root         (0)    12016 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/tests/projects/test_projects_get_merged_vcf.py
--rw-rw-rw-   0 root         (0) root         (0)     6459 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/tests/projects/test_projects_get_sample_manifests.py
--rw-rw-rw-   0 root         (0) root         (0)     6286 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/tests/projects/test_projects_import_existing_samples.py
--rw-rw-rw-   0 root         (0) root         (0)    12079 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/tests/projects/test_projects_list.py
--rw-rw-rw-   0 root         (0) root         (0)     6511 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/tests/projects/test_projects_pipeline_capabilities_list.py
--rw-rw-rw-   0 root         (0) root         (0)     3899 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/tests/projects/test_projects_pipelines_list.py
--rw-rw-rw-   0 root         (0) root         (0)     7212 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/tests/projects/test_projects_restore_samples.py
--rw-rw-rw-   0 root         (0) root         (0)    13390 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/tests/projects/test_projects_run_prefix.py
--rw-rw-rw-   0 root         (0) root         (0)     7184 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/tests/projects/test_projects_samples_list.py
--rw-rw-rw-   0 root         (0) root         (0)     6468 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/tests/projects/test_projects_status_merged_vcf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-03 21:24:10.000000 gencove-2.8.1/gencove/tests/projects/vcr/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/tests/projects/vcr/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    13811 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/tests/projects/vcr/filters.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-03 21:24:10.000000 gencove-2.8.1/gencove/tests/reports/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/tests/reports/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6034 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/tests/reports/test_reports_monthly_usage.py
--rw-rw-rw-   0 root         (0) root         (0)     6903 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/tests/reports/test_reports_project_qc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-03 21:24:10.000000 gencove-2.8.1/gencove/tests/s3_imports/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/tests/s3_imports/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6422 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/tests/s3_imports/test_s3_autoimports_create.py
--rw-rw-rw-   0 root         (0) root         (0)     4163 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/tests/s3_imports/test_s3_autoimports_list.py
--rw-rw-rw-   0 root         (0) root         (0)     5269 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/tests/s3_imports/test_s3_uri_import.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-03 21:24:10.000000 gencove-2.8.1/gencove/tests/s3_imports/vcr/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/tests/s3_imports/vcr/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-03 21:24:10.000000 gencove-2.8.1/gencove/tests/sample_manifests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/tests/sample_manifests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5289 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/tests/sample_manifests/test_sample_manifests_get_sample_manifest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-03 21:24:10.000000 gencove-2.8.1/gencove/tests/samples/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/tests/samples/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10756 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/tests/samples/test_samples_download_file.py
--rw-rw-rw-   0 root         (0) root         (0)     7024 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/tests/samples/test_samples_get_metadata.py
--rw-rw-rw-   0 root         (0) root         (0)     3433 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/tests/samples/test_samples_set_metadata.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-03 21:24:10.000000 gencove-2.8.1/gencove/tests/samples/vcr/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/tests/samples/vcr/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      700 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/tests/samples/vcr/filters.py
--rw-rw-rw-   0 root         (0) root         (0)      660 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/tests/test_logger.py
--rw-rw-rw-   0 root         (0) root         (0)    24076 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/tests/test_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-03 21:24:10.000000 gencove-2.8.1/gencove/tests/upload/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/tests/upload/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    44376 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/tests/upload/test_cli_upload.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-03 21:24:10.000000 gencove-2.8.1/gencove/tests/upload/vcr/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/tests/upload/vcr/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5281 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/tests/upload/vcr/filters.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-03 21:24:10.000000 gencove-2.8.1/gencove/tests/uploads/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/tests/uploads/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4357 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/tests/uploads/test_uploads_list.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-03 21:24:10.000000 gencove-2.8.1/gencove/tests/uploads/vcr/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/tests/uploads/vcr/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1435 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/tests/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-03 21:24:10.000000 gencove-2.8.1/gencove/tests/webhook/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/tests/webhook/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3430 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/tests/webhook/test_webhook_verify.py
--rw-rw-rw-   0 root         (0) root         (0)     6163 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-03 21:24:10.000000 gencove-2.8.1/gencove/version/
--rw-rw-rw-   0 root         (0) root         (0)        2 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/version/A-major
--rw-rw-rw-   0 root         (0) root         (0)        2 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/version/B-minor
--rw-rw-rw-   0 root         (0) root         (0)        2 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/version/C-patch
--rw-rw-rw-   0 root         (0) root         (0)      400 2023-11-03 21:23:38.000000 gencove-2.8.1/gencove/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-03 21:24:10.000000 gencove-2.8.1/gencove.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2387 2023-11-03 21:24:10.000000 gencove-2.8.1/gencove.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    11746 2023-11-03 21:24:10.000000 gencove-2.8.1/gencove.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-11-03 21:24:10.000000 gencove-2.8.1/gencove.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       63 2023-11-03 21:24:10.000000 gencove-2.8.1/gencove.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      127 2023-11-03 21:24:10.000000 gencove-2.8.1/gencove.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-11-03 21:24:10.000000 gencove-2.8.1/gencove.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      135 2023-11-03 21:24:10.000000 gencove-2.8.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1866 2023-11-03 21:23:38.000000 gencove-2.8.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-13 17:09:53.000000 gencove-2.9.0/
+-rw-r--r--   0 root         (0) root         (0)     2387 2023-11-13 17:09:53.000000 gencove-2.9.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2143 2023-11-13 17:09:20.000000 gencove-2.9.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-13 17:09:53.000000 gencove-2.9.0/gencove/
+-rw-rw-rw-   0 root         (0) root         (0)       56 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1336 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)    35488 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-13 17:09:53.000000 gencove-2.9.0/gencove/command/
+-rw-rw-rw-   0 root         (0) root         (0)       61 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6009 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-13 17:09:53.000000 gencove-2.9.0/gencove/command/basespace/
+-rw-rw-rw-   0 root         (0) root         (0)       78 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/basespace/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-13 17:09:53.000000 gencove-2.9.0/gencove/command/basespace/autoimports/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/basespace/autoimports/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-13 17:09:53.000000 gencove-2.9.0/gencove/command/basespace/autoimports/autoimport_list/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/basespace/autoimports/autoimport_list/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      793 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/basespace/autoimports/autoimport_list/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     1966 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/basespace/autoimports/autoimport_list/main.py
+-rw-rw-rw-   0 root         (0) root         (0)      522 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/basespace/autoimports/autoimport_list/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      343 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/basespace/autoimports/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-13 17:09:53.000000 gencove-2.9.0/gencove/command/basespace/autoimports/create/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/basespace/autoimports/create/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1990 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/basespace/autoimports/create/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)      247 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/basespace/autoimports/create/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     2398 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/basespace/autoimports/create/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-13 17:09:53.000000 gencove-2.9.0/gencove/command/basespace/biosamples/
+-rw-rw-rw-   0 root         (0) root         (0)       90 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/basespace/biosamples/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-13 17:09:53.000000 gencove-2.9.0/gencove/command/basespace/biosamples/biosamples_list/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/basespace/biosamples/biosamples_list/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      947 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/basespace/biosamples/biosamples_list/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     2212 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/basespace/biosamples/biosamples_list/main.py
+-rw-rw-rw-   0 root         (0) root         (0)      547 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/basespace/biosamples/biosamples_list/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      277 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/basespace/biosamples/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)      393 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/basespace/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-13 17:09:53.000000 gencove-2.9.0/gencove/command/basespace/projects/
+-rw-rw-rw-   0 root         (0) root         (0)       86 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/basespace/projects/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-13 17:09:53.000000 gencove-2.9.0/gencove/command/basespace/projects/basespace_import/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/basespace/projects/basespace_import/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2144 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/basespace/projects/basespace_import/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)      235 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/basespace/projects/basespace_import/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     2151 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/basespace/projects/basespace_import/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-13 17:09:53.000000 gencove-2.9.0/gencove/command/basespace/projects/basespace_list/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/basespace/projects/basespace_list/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      634 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/basespace/projects/basespace_list/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     1987 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/basespace/projects/basespace_list/main.py
+-rw-rw-rw-   0 root         (0) root         (0)      571 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/basespace/projects/basespace_list/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      358 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/basespace/projects/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     1548 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/common_cli_options.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-13 17:09:53.000000 gencove-2.9.0/gencove/command/download/
+-rw-rw-rw-   0 root         (0) root         (0)       99 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/download/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3834 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/download/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     2104 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/download/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)      206 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/download/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    14841 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/download/main.py
+-rw-rw-rw-   0 root         (0) root         (0)    10605 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/download/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-13 17:09:53.000000 gencove-2.9.0/gencove/command/explorer/
+-rw-rw-rw-   0 root         (0) root         (0)       99 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/explorer/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1389 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/explorer/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-13 17:09:53.000000 gencove-2.9.0/gencove/command/files/
+-rw-rw-rw-   0 root         (0) root         (0)       79 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/files/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      630 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/files/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     1888 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/files/main.py
+-rw-rw-rw-   0 root         (0) root         (0)      390 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/files/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-13 17:09:53.000000 gencove-2.9.0/gencove/command/projects/
+-rw-rw-rw-   0 root         (0) root         (0)       75 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/projects/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1970 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/projects/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-13 17:09:53.000000 gencove-2.9.0/gencove/command/projects/create/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/projects/create/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      935 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/projects/create/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     1439 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/projects/create/main.py
+-rw-rw-rw-   0 root         (0) root         (0)      505 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/projects/create/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-13 17:09:53.000000 gencove-2.9.0/gencove/command/projects/create_batch/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/projects/create_batch/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1359 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/projects/create_batch/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     2433 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/projects/create_batch/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-13 17:09:53.000000 gencove-2.9.0/gencove/command/projects/create_merged_vcf/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/projects/create_merged_vcf/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      730 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/projects/create_merged_vcf/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     1436 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/projects/create_merged_vcf/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-13 17:09:53.000000 gencove-2.9.0/gencove/command/projects/create_sample_manifest/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/projects/create_sample_manifest/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1015 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/projects/create_sample_manifest/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     2219 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/projects/create_sample_manifest/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-13 17:09:53.000000 gencove-2.9.0/gencove/command/projects/delete/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/projects/delete/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      978 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/projects/delete/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     1709 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/projects/delete/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-13 17:09:53.000000 gencove-2.9.0/gencove/command/projects/delete_samples/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/projects/delete_samples/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1073 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/projects/delete_samples/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     1931 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/projects/delete_samples/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-13 17:09:53.000000 gencove-2.9.0/gencove/command/projects/get_batch/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/projects/get_batch/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      977 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/projects/get_batch/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     2769 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/projects/get_batch/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-13 17:09:53.000000 gencove-2.9.0/gencove/command/projects/get_merged_vcf/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/projects/get_merged_vcf/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1105 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/projects/get_merged_vcf/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     2147 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/projects/get_merged_vcf/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-13 17:09:53.000000 gencove-2.9.0/gencove/command/projects/get_sample_manifests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/projects/get_sample_manifests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1013 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/projects/get_sample_manifests/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     2518 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/projects/get_sample_manifests/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-13 17:09:53.000000 gencove-2.9.0/gencove/command/projects/import_existing_samples/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/projects/import_existing_samples/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1918 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/projects/import_existing_samples/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)      295 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/projects/import_existing_samples/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     2191 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/projects/import_existing_samples/main.py
+-rw-rw-rw-   0 root         (0) root         (0)      442 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/projects/import_existing_samples/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-13 17:09:53.000000 gencove-2.9.0/gencove/command/projects/list/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/projects/list/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      646 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/projects/list/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     3051 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/projects/list/main.py
+-rw-rw-rw-   0 root         (0) root         (0)      699 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/projects/list/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-13 17:09:53.000000 gencove-2.9.0/gencove/command/projects/list_batch_types/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/projects/list_batch_types/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      731 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/projects/list_batch_types/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     2264 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/projects/list_batch_types/main.py
+-rw-rw-rw-   0 root         (0) root         (0)      403 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/projects/list_batch_types/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-13 17:09:53.000000 gencove-2.9.0/gencove/command/projects/list_batches/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/projects/list_batches/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      709 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/projects/list_batches/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     2182 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/projects/list_batches/main.py
+-rw-rw-rw-   0 root         (0) root         (0)      499 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/projects/list_batches/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-13 17:09:53.000000 gencove-2.9.0/gencove/command/projects/list_pipeline_capabilities/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/projects/list_pipeline_capabilities/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      781 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/projects/list_pipeline_capabilities/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     1668 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/projects/list_pipeline_capabilities/main.py
+-rw-rw-rw-   0 root         (0) root         (0)      448 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/projects/list_pipeline_capabilities/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-13 17:09:53.000000 gencove-2.9.0/gencove/command/projects/list_pipelines/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/projects/list_pipelines/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      554 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/projects/list_pipelines/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     1842 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/projects/list_pipelines/main.py
+-rw-rw-rw-   0 root         (0) root         (0)      391 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/projects/list_pipelines/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-13 17:09:53.000000 gencove-2.9.0/gencove/command/projects/restore_samples/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/projects/restore_samples/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1159 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/projects/restore_samples/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     1823 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/projects/restore_samples/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-13 17:09:53.000000 gencove-2.9.0/gencove/command/projects/run_prefix/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/projects/run_prefix/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2075 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/projects/run_prefix/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)      327 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/projects/run_prefix/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     4918 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/projects/run_prefix/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-13 17:09:53.000000 gencove-2.9.0/gencove/command/projects/samples/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/projects/samples/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1646 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/projects/samples/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)      343 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/projects/samples/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     2454 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/projects/samples/main.py
+-rw-rw-rw-   0 root         (0) root         (0)      735 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/projects/samples/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-13 17:09:53.000000 gencove-2.9.0/gencove/command/projects/status_merged_vcf/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/projects/status_merged_vcf/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      748 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/projects/status_merged_vcf/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     1813 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/projects/status_merged_vcf/main.py
+-rw-rw-rw-   0 root         (0) root         (0)      470 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/projects/status_merged_vcf/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-13 17:09:53.000000 gencove-2.9.0/gencove/command/reports/
+-rw-rw-rw-   0 root         (0) root         (0)       62 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/reports/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      322 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/reports/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-13 17:09:53.000000 gencove-2.9.0/gencove/command/reports/monthly_usage/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/reports/monthly_usage/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1450 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/reports/monthly_usage/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     2470 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/reports/monthly_usage/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-13 17:09:53.000000 gencove-2.9.0/gencove/command/reports/project_qc/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/reports/project_qc/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1251 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/reports/project_qc/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     2588 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/reports/project_qc/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-13 17:09:53.000000 gencove-2.9.0/gencove/command/s3_imports/
+-rw-rw-rw-   0 root         (0) root         (0)       72 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/s3_imports/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-13 17:09:53.000000 gencove-2.9.0/gencove/command/s3_imports/autoimports/
+-rw-rw-rw-   0 root         (0) root         (0)       85 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/s3_imports/autoimports/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-13 17:09:53.000000 gencove-2.9.0/gencove/command/s3_imports/autoimports/autoimport_list/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/s3_imports/autoimports/autoimport_list/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      660 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/s3_imports/autoimports/autoimport_list/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     1744 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/s3_imports/autoimports/autoimport_list/main.py
+-rw-rw-rw-   0 root         (0) root         (0)      462 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/s3_imports/autoimports/autoimport_list/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      336 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/s3_imports/autoimports/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-13 17:09:53.000000 gencove-2.9.0/gencove/command/s3_imports/autoimports/create/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/s3_imports/autoimports/create/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1686 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/s3_imports/autoimports/create/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)      226 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/s3_imports/autoimports/create/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     2314 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/s3_imports/autoimports/create/main.py
+-rw-rw-rw-   0 root         (0) root         (0)      392 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/s3_imports/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-13 17:09:53.000000 gencove-2.9.0/gencove/command/s3_imports/s3_import/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/s3_imports/s3_import/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1523 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/s3_imports/s3_import/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)      214 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/s3_imports/s3_import/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     1916 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/s3_imports/s3_import/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-13 17:09:53.000000 gencove-2.9.0/gencove/command/sample_manifests/
+-rw-rw-rw-   0 root         (0) root         (0)       80 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/sample_manifests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      296 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/sample_manifests/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-13 17:09:53.000000 gencove-2.9.0/gencove/command/sample_manifests/get_sample_manifest/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/sample_manifests/get_sample_manifest/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      991 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/sample_manifests/get_sample_manifest/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     2181 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/sample_manifests/get_sample_manifest/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-13 17:09:53.000000 gencove-2.9.0/gencove/command/samples/
+-rw-rw-rw-   0 root         (0) root         (0)       79 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/samples/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      370 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/samples/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-13 17:09:53.000000 gencove-2.9.0/gencove/command/samples/download_file/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/samples/download_file/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2825 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/samples/download_file/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)      141 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/samples/download_file/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     5345 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/samples/download_file/main.py
+-rw-rw-rw-   0 root         (0) root         (0)     3051 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/samples/download_file/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-13 17:09:53.000000 gencove-2.9.0/gencove/command/samples/get_metadata/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/samples/get_metadata/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      870 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/samples/get_metadata/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     2348 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/samples/get_metadata/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-13 17:09:53.000000 gencove-2.9.0/gencove/command/samples/set_metadata/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/samples/set_metadata/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      818 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/samples/set_metadata/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     1981 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/samples/set_metadata/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-13 17:09:53.000000 gencove-2.9.0/gencove/command/upload/
+-rw-rw-rw-   0 root         (0) root         (0)       97 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/upload/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1973 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/upload/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     1529 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/upload/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)      258 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/upload/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    17222 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/upload/main.py
+-rw-rw-rw-   0 root         (0) root         (0)     3028 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/upload/multi_file_reader.py
+-rw-rw-rw-   0 root         (0) root         (0)     9443 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/upload/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-13 17:09:53.000000 gencove-2.9.0/gencove/command/uploads/
+-rw-rw-rw-   0 root         (0) root         (0)       84 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/uploads/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      213 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/uploads/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-13 17:09:53.000000 gencove-2.9.0/gencove/command/uploads/list/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/uploads/list/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      934 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/uploads/list/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)      277 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/uploads/list/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     2113 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/uploads/list/main.py
+-rw-rw-rw-   0 root         (0) root         (0)      573 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/uploads/list/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     4334 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-13 17:09:53.000000 gencove-2.9.0/gencove/command/webhook/
+-rw-rw-rw-   0 root         (0) root         (0)       72 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/webhook/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      198 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/webhook/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-13 17:09:53.000000 gencove-2.9.0/gencove/command/webhook/verify/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/webhook/verify/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      777 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/webhook/verify/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)      999 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/command/webhook/verify/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     4119 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-13 17:09:53.000000 gencove-2.9.0/gencove/description/
+-rw-rw-rw-   0 root         (0) root         (0)     1811 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/description/pypi_readme.md
+-rw-rw-rw-   0 root         (0) root         (0)      508 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     3205 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/logger.py
+-rw-rw-rw-   0 root         (0) root         (0)     8467 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-13 17:09:53.000000 gencove-2.9.0/gencove/tests/
+-rw-rw-rw-   0 root         (0) root         (0)       32 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-13 17:09:53.000000 gencove-2.9.0/gencove/tests/basespace/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/tests/basespace/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6374 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/tests/basespace/test_basespace_autoimports_create.py
+-rw-rw-rw-   0 root         (0) root         (0)     4249 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/tests/basespace/test_basespace_autoimports_list.py
+-rw-rw-rw-   0 root         (0) root         (0)     7257 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/tests/basespace/test_basespace_biosamples_list.py
+-rw-rw-rw-   0 root         (0) root         (0)     6334 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/tests/basespace/test_basespace_projects_import.py
+-rw-rw-rw-   0 root         (0) root         (0)     5955 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/tests/basespace/test_basespace_projects_list.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-13 17:09:53.000000 gencove-2.9.0/gencove/tests/basespace/vcr/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/tests/basespace/vcr/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5184 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/tests/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)     3328 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/tests/decorators.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-13 17:09:53.000000 gencove-2.9.0/gencove/tests/download/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/tests/download/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    41021 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/tests/download/test_cli_download.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-13 17:09:53.000000 gencove-2.9.0/gencove/tests/download/vcr/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/tests/download/vcr/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      932 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/tests/download/vcr/filters.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-13 17:09:53.000000 gencove-2.9.0/gencove/tests/files/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/tests/files/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4371 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/tests/files/test_file_types_list.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-13 17:09:53.000000 gencove-2.9.0/gencove/tests/files/vcr/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/tests/files/vcr/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5527 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/tests/filters.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-13 17:09:53.000000 gencove-2.9.0/gencove/tests/projects/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/tests/projects/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6781 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/tests/projects/test_projects_batch_get.py
+-rw-rw-rw-   0 root         (0) root         (0)     4502 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/tests/projects/test_projects_batch_types_list.py
+-rw-rw-rw-   0 root         (0) root         (0)     8945 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/tests/projects/test_projects_batches_create.py
+-rw-rw-rw-   0 root         (0) root         (0)     4601 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/tests/projects/test_projects_batches_list.py
+-rw-rw-rw-   0 root         (0) root         (0)     4380 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/tests/projects/test_projects_create.py
+-rw-rw-rw-   0 root         (0) root         (0)     9108 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/tests/projects/test_projects_create_merged_vcf.py
+-rw-rw-rw-   0 root         (0) root         (0)     4693 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/tests/projects/test_projects_create_sample_manifest.py
+-rw-rw-rw-   0 root         (0) root         (0)     5626 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/tests/projects/test_projects_delete.py
+-rw-rw-rw-   0 root         (0) root         (0)     8901 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/tests/projects/test_projects_delete_samples.py
+-rw-rw-rw-   0 root         (0) root         (0)    12016 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/tests/projects/test_projects_get_merged_vcf.py
+-rw-rw-rw-   0 root         (0) root         (0)     6459 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/tests/projects/test_projects_get_sample_manifests.py
+-rw-rw-rw-   0 root         (0) root         (0)     6286 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/tests/projects/test_projects_import_existing_samples.py
+-rw-rw-rw-   0 root         (0) root         (0)    12079 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/tests/projects/test_projects_list.py
+-rw-rw-rw-   0 root         (0) root         (0)     6511 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/tests/projects/test_projects_pipeline_capabilities_list.py
+-rw-rw-rw-   0 root         (0) root         (0)     3899 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/tests/projects/test_projects_pipelines_list.py
+-rw-rw-rw-   0 root         (0) root         (0)     7212 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/tests/projects/test_projects_restore_samples.py
+-rw-rw-rw-   0 root         (0) root         (0)    13390 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/tests/projects/test_projects_run_prefix.py
+-rw-rw-rw-   0 root         (0) root         (0)     7184 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/tests/projects/test_projects_samples_list.py
+-rw-rw-rw-   0 root         (0) root         (0)     6468 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/tests/projects/test_projects_status_merged_vcf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-13 17:09:53.000000 gencove-2.9.0/gencove/tests/projects/vcr/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/tests/projects/vcr/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    13811 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/tests/projects/vcr/filters.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-13 17:09:53.000000 gencove-2.9.0/gencove/tests/reports/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/tests/reports/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6034 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/tests/reports/test_reports_monthly_usage.py
+-rw-rw-rw-   0 root         (0) root         (0)     6903 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/tests/reports/test_reports_project_qc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-13 17:09:53.000000 gencove-2.9.0/gencove/tests/s3_imports/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/tests/s3_imports/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6422 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/tests/s3_imports/test_s3_autoimports_create.py
+-rw-rw-rw-   0 root         (0) root         (0)     4163 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/tests/s3_imports/test_s3_autoimports_list.py
+-rw-rw-rw-   0 root         (0) root         (0)     5269 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/tests/s3_imports/test_s3_uri_import.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-13 17:09:53.000000 gencove-2.9.0/gencove/tests/s3_imports/vcr/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/tests/s3_imports/vcr/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-13 17:09:53.000000 gencove-2.9.0/gencove/tests/sample_manifests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/tests/sample_manifests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5289 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/tests/sample_manifests/test_sample_manifests_get_sample_manifest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-13 17:09:53.000000 gencove-2.9.0/gencove/tests/samples/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/tests/samples/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10756 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/tests/samples/test_samples_download_file.py
+-rw-rw-rw-   0 root         (0) root         (0)     7024 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/tests/samples/test_samples_get_metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)     3433 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/tests/samples/test_samples_set_metadata.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-13 17:09:53.000000 gencove-2.9.0/gencove/tests/samples/vcr/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/tests/samples/vcr/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      700 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/tests/samples/vcr/filters.py
+-rw-rw-rw-   0 root         (0) root         (0)      660 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/tests/test_logger.py
+-rw-rw-rw-   0 root         (0) root         (0)    24076 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/tests/test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-13 17:09:53.000000 gencove-2.9.0/gencove/tests/upload/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/tests/upload/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    44376 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/tests/upload/test_cli_upload.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-13 17:09:53.000000 gencove-2.9.0/gencove/tests/upload/vcr/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/tests/upload/vcr/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5281 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/tests/upload/vcr/filters.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-13 17:09:53.000000 gencove-2.9.0/gencove/tests/uploads/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/tests/uploads/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4357 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/tests/uploads/test_uploads_list.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-13 17:09:53.000000 gencove-2.9.0/gencove/tests/uploads/vcr/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/tests/uploads/vcr/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1435 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/tests/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-13 17:09:53.000000 gencove-2.9.0/gencove/tests/webhook/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/tests/webhook/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3430 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/tests/webhook/test_webhook_verify.py
+-rw-rw-rw-   0 root         (0) root         (0)     6163 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-13 17:09:53.000000 gencove-2.9.0/gencove/version/
+-rw-rw-rw-   0 root         (0) root         (0)        2 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/version/A-major
+-rw-rw-rw-   0 root         (0) root         (0)        2 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/version/B-minor
+-rw-rw-rw-   0 root         (0) root         (0)        2 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/version/C-patch
+-rw-rw-rw-   0 root         (0) root         (0)      400 2023-11-13 17:09:20.000000 gencove-2.9.0/gencove/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-13 17:09:53.000000 gencove-2.9.0/gencove.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2387 2023-11-13 17:09:53.000000 gencove-2.9.0/gencove.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    11815 2023-11-13 17:09:53.000000 gencove-2.9.0/gencove.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-11-13 17:09:53.000000 gencove-2.9.0/gencove.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       63 2023-11-13 17:09:53.000000 gencove-2.9.0/gencove.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      165 2023-11-13 17:09:53.000000 gencove-2.9.0/gencove.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-11-13 17:09:53.000000 gencove-2.9.0/gencove.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      135 2023-11-13 17:09:53.000000 gencove-2.9.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1926 2023-11-13 17:09:20.000000 gencove-2.9.0/setup.py
```

### Comparing `gencove-2.8.1/PKG-INFO` & `gencove-2.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gencove
-Version: 2.8.1
+Version: 2.9.0
 Summary: Gencove API and CLI tool
 Home-page: http://docs.gencove.com
 Author: Tomaz Berisa
 License: Apache 2.0
 Description: # The Gencove CLI
         
         [![PyPI Latest Release](https://img.shields.io/pypi/v/gencove.svg)](https://pypi.org/project/gencove/)
```

### Comparing `gencove-2.8.1/README.md` & `gencove-2.9.0/README.md`

 * *Files identical despite different names*

### Comparing `gencove-2.8.1/gencove/cli.py` & `gencove-2.9.0/gencove/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Python library which enables you to use Gencoves' research backend."""
 import click
 
 from gencove import version
 from gencove.command.basespace import basespace
 from gencove.command.download import download
+from gencove.command.explorer import explorer
 from gencove.command.files import list_file_types
 from gencove.command.projects import projects
 from gencove.command.reports import reports
 from gencove.command.s3_imports import s3
 from gencove.command.sample_manifests import sample_manifests
 from gencove.command.samples import samples
 from gencove.command.upload import upload
@@ -26,14 +27,15 @@
 def cli():
     """Gencove's command line interface."""
 
 
 announcements()
 cli.add_command(basespace)
 cli.add_command(download)
+cli.add_command(explorer)
 cli.add_command(list_file_types)
 cli.add_command(upload)
 cli.add_command(uploads)
 cli.add_command(projects)
 cli.add_command(reports)
 cli.add_command(samples)
 cli.add_command(sample_manifests)
```

### Comparing `gencove-2.8.1/gencove/client.py` & `gencove-2.9.0/gencove/client.py`

 * *Files identical despite different names*

### Comparing `gencove-2.8.1/gencove/command/base.py` & `gencove-2.9.0/gencove/command/base.py`

 * *Files identical despite different names*

### Comparing `gencove-2.8.1/gencove/command/basespace/autoimports/autoimport_list/cli.py` & `gencove-2.9.0/gencove/command/basespace/autoimports/autoimport_list/cli.py`

 * *Files identical despite different names*

### Comparing `gencove-2.8.1/gencove/command/basespace/autoimports/autoimport_list/main.py` & `gencove-2.9.0/gencove/command/basespace/autoimports/autoimport_list/main.py`

 * *Files identical despite different names*

### Comparing `gencove-2.8.1/gencove/command/basespace/autoimports/autoimport_list/utils.py` & `gencove-2.9.0/gencove/command/basespace/autoimports/autoimport_list/utils.py`

 * *Files identical despite different names*

### Comparing `gencove-2.8.1/gencove/command/basespace/autoimports/create/cli.py` & `gencove-2.9.0/gencove/command/basespace/autoimports/create/cli.py`

 * *Files identical despite different names*

### Comparing `gencove-2.8.1/gencove/command/basespace/autoimports/create/main.py` & `gencove-2.9.0/gencove/command/basespace/autoimports/create/main.py`

 * *Files identical despite different names*

### Comparing `gencove-2.8.1/gencove/command/basespace/biosamples/biosamples_list/cli.py` & `gencove-2.9.0/gencove/command/basespace/biosamples/biosamples_list/cli.py`

 * *Files identical despite different names*

### Comparing `gencove-2.8.1/gencove/command/basespace/biosamples/biosamples_list/main.py` & `gencove-2.9.0/gencove/command/basespace/biosamples/biosamples_list/main.py`

 * *Files identical despite different names*

### Comparing `gencove-2.8.1/gencove/command/basespace/biosamples/biosamples_list/utils.py` & `gencove-2.9.0/gencove/command/basespace/biosamples/biosamples_list/utils.py`

 * *Files identical despite different names*

### Comparing `gencove-2.8.1/gencove/command/basespace/projects/basespace_import/cli.py` & `gencove-2.9.0/gencove/command/basespace/projects/basespace_import/cli.py`

 * *Files identical despite different names*

### Comparing `gencove-2.8.1/gencove/command/basespace/projects/basespace_import/main.py` & `gencove-2.9.0/gencove/command/basespace/projects/basespace_import/main.py`

 * *Files identical despite different names*

### Comparing `gencove-2.8.1/gencove/command/basespace/projects/basespace_list/cli.py` & `gencove-2.9.0/gencove/command/basespace/projects/basespace_list/cli.py`

 * *Files identical despite different names*

### Comparing `gencove-2.8.1/gencove/command/basespace/projects/basespace_list/main.py` & `gencove-2.9.0/gencove/command/basespace/projects/basespace_list/main.py`

 * *Files identical despite different names*

### Comparing `gencove-2.8.1/gencove/command/basespace/projects/basespace_list/utils.py` & `gencove-2.9.0/gencove/command/basespace/projects/basespace_list/utils.py`

 * *Files identical despite different names*

### Comparing `gencove-2.8.1/gencove/command/common_cli_options.py` & `gencove-2.9.0/gencove/command/common_cli_options.py`

 * *Files identical despite different names*

### Comparing `gencove-2.8.1/gencove/command/download/cli.py` & `gencove-2.9.0/gencove/command/download/cli.py`

 * *Files identical despite different names*

### Comparing `gencove-2.8.1/gencove/command/download/constants.py` & `gencove-2.9.0/gencove/command/download/constants.py`

 * *Files identical despite different names*

### Comparing `gencove-2.8.1/gencove/command/download/main.py` & `gencove-2.9.0/gencove/command/download/main.py`

 * *Files identical despite different names*

### Comparing `gencove-2.8.1/gencove/command/download/utils.py` & `gencove-2.9.0/gencove/command/download/utils.py`

 * *Files identical despite different names*

### Comparing `gencove-2.8.1/gencove/command/files/cli.py` & `gencove-2.9.0/gencove/command/files/cli.py`

 * *Files identical despite different names*

### Comparing `gencove-2.8.1/gencove/command/files/main.py` & `gencove-2.9.0/gencove/command/files/main.py`

 * *Files identical despite different names*

### Comparing `gencove-2.8.1/gencove/command/projects/cli.py` & `gencove-2.9.0/gencove/command/projects/cli.py`

 * *Files identical despite different names*

### Comparing `gencove-2.8.1/gencove/command/projects/create/cli.py` & `gencove-2.9.0/gencove/command/projects/create/cli.py`

 * *Files identical despite different names*

### Comparing `gencove-2.8.1/gencove/command/projects/create/main.py` & `gencove-2.9.0/gencove/command/projects/create/main.py`

 * *Files identical despite different names*

### Comparing `gencove-2.8.1/gencove/command/projects/create_batch/cli.py` & `gencove-2.9.0/gencove/command/projects/create_batch/cli.py`

 * *Files identical despite different names*

### Comparing `gencove-2.8.1/gencove/command/projects/create_batch/main.py` & `gencove-2.9.0/gencove/command/projects/create_batch/main.py`

 * *Files identical despite different names*

### Comparing `gencove-2.8.1/gencove/command/projects/create_merged_vcf/cli.py` & `gencove-2.9.0/gencove/command/projects/create_merged_vcf/cli.py`

 * *Files identical despite different names*

### Comparing `gencove-2.8.1/gencove/command/projects/create_merged_vcf/main.py` & `gencove-2.9.0/gencove/command/projects/create_merged_vcf/main.py`

 * *Files identical despite different names*

### Comparing `gencove-2.8.1/gencove/command/projects/create_sample_manifest/cli.py` & `gencove-2.9.0/gencove/command/projects/create_sample_manifest/cli.py`

 * *Files identical despite different names*

### Comparing `gencove-2.8.1/gencove/command/projects/create_sample_manifest/main.py` & `gencove-2.9.0/gencove/command/projects/create_sample_manifest/main.py`

 * *Files identical despite different names*

### Comparing `gencove-2.8.1/gencove/command/projects/delete/cli.py` & `gencove-2.9.0/gencove/command/projects/delete/cli.py`

 * *Files identical despite different names*

### Comparing `gencove-2.8.1/gencove/command/projects/delete/main.py` & `gencove-2.9.0/gencove/command/projects/delete/main.py`

 * *Files identical despite different names*

### Comparing `gencove-2.8.1/gencove/command/projects/delete_samples/cli.py` & `gencove-2.9.0/gencove/command/projects/delete_samples/cli.py`

 * *Files identical despite different names*

### Comparing `gencove-2.8.1/gencove/command/projects/delete_samples/main.py` & `gencove-2.9.0/gencove/command/projects/delete_samples/main.py`

 * *Files identical despite different names*

### Comparing `gencove-2.8.1/gencove/command/projects/get_batch/cli.py` & `gencove-2.9.0/gencove/command/projects/get_batch/cli.py`

 * *Files identical despite different names*

### Comparing `gencove-2.8.1/gencove/command/projects/get_batch/main.py` & `gencove-2.9.0/gencove/command/projects/get_batch/main.py`

 * *Files identical despite different names*

### Comparing `gencove-2.8.1/gencove/command/projects/get_merged_vcf/cli.py` & `gencove-2.9.0/gencove/command/projects/get_merged_vcf/cli.py`

 * *Files identical despite different names*

### Comparing `gencove-2.8.1/gencove/command/projects/get_merged_vcf/main.py` & `gencove-2.9.0/gencove/command/projects/get_merged_vcf/main.py`

 * *Files identical despite different names*

### Comparing `gencove-2.8.1/gencove/command/projects/get_sample_manifests/cli.py` & `gencove-2.9.0/gencove/command/projects/get_sample_manifests/cli.py`

 * *Files identical despite different names*

### Comparing `gencove-2.8.1/gencove/command/projects/get_sample_manifests/main.py` & `gencove-2.9.0/gencove/command/projects/get_sample_manifests/main.py`

 * *Files identical despite different names*

### Comparing `gencove-2.8.1/gencove/command/projects/import_existing_samples/cli.py` & `gencove-2.9.0/gencove/command/projects/import_existing_samples/cli.py`

 * *Files identical despite different names*

### Comparing `gencove-2.8.1/gencove/command/projects/import_existing_samples/main.py` & `gencove-2.9.0/gencove/command/projects/import_existing_samples/main.py`

 * *Files identical despite different names*

### Comparing `gencove-2.8.1/gencove/command/projects/list/cli.py` & `gencove-2.9.0/gencove/command/projects/list/cli.py`

 * *Files identical despite different names*

### Comparing `gencove-2.8.1/gencove/command/projects/list/main.py` & `gencove-2.9.0/gencove/command/projects/list/main.py`

 * *Files identical despite different names*

### Comparing `gencove-2.8.1/gencove/command/projects/list/utils.py` & `gencove-2.9.0/gencove/command/projects/list/utils.py`

 * *Files identical despite different names*

### Comparing `gencove-2.8.1/gencove/command/projects/list_batch_types/cli.py` & `gencove-2.9.0/gencove/command/projects/list_batch_types/cli.py`

 * *Files identical despite different names*

### Comparing `gencove-2.8.1/gencove/command/projects/list_batch_types/main.py` & `gencove-2.9.0/gencove/command/projects/list_batch_types/main.py`

 * *Files identical despite different names*

### Comparing `gencove-2.8.1/gencove/command/projects/list_batches/cli.py` & `gencove-2.9.0/gencove/command/projects/list_batches/cli.py`

 * *Files identical despite different names*

### Comparing `gencove-2.8.1/gencove/command/projects/list_batches/main.py` & `gencove-2.9.0/gencove/command/projects/list_batches/main.py`

 * *Files identical despite different names*

### Comparing `gencove-2.8.1/gencove/command/projects/list_pipeline_capabilities/cli.py` & `gencove-2.9.0/gencove/command/projects/list_pipeline_capabilities/cli.py`

 * *Files identical despite different names*

### Comparing `gencove-2.8.1/gencove/command/projects/list_pipeline_capabilities/main.py` & `gencove-2.9.0/gencove/command/projects/list_pipeline_capabilities/main.py`

 * *Files identical despite different names*

### Comparing `gencove-2.8.1/gencove/command/projects/list_pipelines/cli.py` & `gencove-2.9.0/gencove/command/projects/list_pipelines/cli.py`

 * *Files identical despite different names*

### Comparing `gencove-2.8.1/gencove/command/projects/list_pipelines/main.py` & `gencove-2.9.0/gencove/command/projects/list_pipelines/main.py`

 * *Files identical despite different names*

### Comparing `gencove-2.8.1/gencove/command/projects/restore_samples/cli.py` & `gencove-2.9.0/gencove/command/projects/restore_samples/cli.py`

 * *Files identical despite different names*

### Comparing `gencove-2.8.1/gencove/command/projects/restore_samples/main.py` & `gencove-2.9.0/gencove/command/projects/restore_samples/main.py`

 * *Files identical despite different names*

### Comparing `gencove-2.8.1/gencove/command/projects/run_prefix/cli.py` & `gencove-2.9.0/gencove/command/projects/run_prefix/cli.py`

 * *Files identical despite different names*

### Comparing `gencove-2.8.1/gencove/command/projects/run_prefix/main.py` & `gencove-2.9.0/gencove/command/projects/run_prefix/main.py`

 * *Files identical despite different names*

### Comparing `gencove-2.8.1/gencove/command/projects/samples/cli.py` & `gencove-2.9.0/gencove/command/projects/samples/cli.py`

 * *Files identical despite different names*

### Comparing `gencove-2.8.1/gencove/command/projects/samples/main.py` & `gencove-2.9.0/gencove/command/projects/samples/main.py`

 * *Files identical despite different names*

### Comparing `gencove-2.8.1/gencove/command/projects/samples/utils.py` & `gencove-2.9.0/gencove/command/projects/samples/utils.py`

 * *Files identical despite different names*

### Comparing `gencove-2.8.1/gencove/command/projects/status_merged_vcf/cli.py` & `gencove-2.9.0/gencove/command/projects/status_merged_vcf/cli.py`

 * *Files identical despite different names*

### Comparing `gencove-2.8.1/gencove/command/projects/status_merged_vcf/main.py` & `gencove-2.9.0/gencove/command/projects/status_merged_vcf/main.py`

 * *Files identical despite different names*

### Comparing `gencove-2.8.1/gencove/command/reports/monthly_usage/cli.py` & `gencove-2.9.0/gencove/command/reports/monthly_usage/cli.py`

 * *Files identical despite different names*

### Comparing `gencove-2.8.1/gencove/command/reports/monthly_usage/main.py` & `gencove-2.9.0/gencove/command/reports/monthly_usage/main.py`

 * *Files identical despite different names*

### Comparing `gencove-2.8.1/gencove/command/reports/project_qc/cli.py` & `gencove-2.9.0/gencove/command/reports/project_qc/cli.py`

 * *Files identical despite different names*

### Comparing `gencove-2.8.1/gencove/command/reports/project_qc/main.py` & `gencove-2.9.0/gencove/command/reports/project_qc/main.py`

 * *Files identical despite different names*

### Comparing `gencove-2.8.1/gencove/command/s3_imports/autoimports/autoimport_list/cli.py` & `gencove-2.9.0/gencove/command/s3_imports/autoimports/autoimport_list/cli.py`

 * *Files identical despite different names*

### Comparing `gencove-2.8.1/gencove/command/s3_imports/autoimports/autoimport_list/main.py` & `gencove-2.9.0/gencove/command/s3_imports/autoimports/autoimport_list/main.py`

 * *Files identical despite different names*

### Comparing `gencove-2.8.1/gencove/command/s3_imports/autoimports/create/cli.py` & `gencove-2.9.0/gencove/command/s3_imports/autoimports/create/cli.py`

 * *Files identical despite different names*

### Comparing `gencove-2.8.1/gencove/command/s3_imports/autoimports/create/main.py` & `gencove-2.9.0/gencove/command/s3_imports/autoimports/create/main.py`

 * *Files identical despite different names*

### Comparing `gencove-2.8.1/gencove/command/s3_imports/s3_import/cli.py` & `gencove-2.9.0/gencove/command/s3_imports/s3_import/cli.py`

 * *Files identical despite different names*

### Comparing `gencove-2.8.1/gencove/command/s3_imports/s3_import/main.py` & `gencove-2.9.0/gencove/command/s3_imports/s3_import/main.py`

 * *Files identical despite different names*

### Comparing `gencove-2.8.1/gencove/command/sample_manifests/get_sample_manifest/cli.py` & `gencove-2.9.0/gencove/command/sample_manifests/get_sample_manifest/cli.py`

 * *Files identical despite different names*

### Comparing `gencove-2.8.1/gencove/command/sample_manifests/get_sample_manifest/main.py` & `gencove-2.9.0/gencove/command/sample_manifests/get_sample_manifest/main.py`

 * *Files identical despite different names*

### Comparing `gencove-2.8.1/gencove/command/samples/download_file/cli.py` & `gencove-2.9.0/gencove/command/samples/download_file/cli.py`

 * *Files identical despite different names*

### Comparing `gencove-2.8.1/gencove/command/samples/download_file/main.py` & `gencove-2.9.0/gencove/command/samples/download_file/main.py`

 * *Files identical despite different names*

### Comparing `gencove-2.8.1/gencove/command/samples/download_file/utils.py` & `gencove-2.9.0/gencove/command/samples/download_file/utils.py`

 * *Files identical despite different names*

### Comparing `gencove-2.8.1/gencove/command/samples/get_metadata/cli.py` & `gencove-2.9.0/gencove/command/samples/get_metadata/cli.py`

 * *Files identical despite different names*

### Comparing `gencove-2.8.1/gencove/command/samples/get_metadata/main.py` & `gencove-2.9.0/gencove/command/samples/get_metadata/main.py`

 * *Files identical despite different names*

### Comparing `gencove-2.8.1/gencove/command/samples/set_metadata/cli.py` & `gencove-2.9.0/gencove/command/samples/set_metadata/cli.py`

 * *Files identical despite different names*

### Comparing `gencove-2.8.1/gencove/command/samples/set_metadata/main.py` & `gencove-2.9.0/gencove/command/samples/set_metadata/main.py`

 * *Files identical despite different names*

### Comparing `gencove-2.8.1/gencove/command/upload/cli.py` & `gencove-2.9.0/gencove/command/upload/cli.py`

 * *Files identical despite different names*

### Comparing `gencove-2.8.1/gencove/command/upload/constants.py` & `gencove-2.9.0/gencove/command/upload/constants.py`

 * *Files identical despite different names*

### Comparing `gencove-2.8.1/gencove/command/upload/main.py` & `gencove-2.9.0/gencove/command/upload/main.py`

 * *Files identical despite different names*

### Comparing `gencove-2.8.1/gencove/command/upload/multi_file_reader.py` & `gencove-2.9.0/gencove/command/upload/multi_file_reader.py`

 * *Files identical despite different names*

### Comparing `gencove-2.8.1/gencove/command/upload/utils.py` & `gencove-2.9.0/gencove/command/upload/utils.py`

 * *Files identical despite different names*

### Comparing `gencove-2.8.1/gencove/command/uploads/list/cli.py` & `gencove-2.9.0/gencove/command/uploads/list/cli.py`

 * *Files identical despite different names*

### Comparing `gencove-2.8.1/gencove/command/uploads/list/main.py` & `gencove-2.9.0/gencove/command/uploads/list/main.py`

 * *Files identical despite different names*

### Comparing `gencove-2.8.1/gencove/command/uploads/list/utils.py` & `gencove-2.9.0/gencove/command/uploads/list/utils.py`

 * *Files identical despite different names*

### Comparing `gencove-2.8.1/gencove/command/utils.py` & `gencove-2.9.0/gencove/command/utils.py`

 * *Files identical despite different names*

### Comparing `gencove-2.8.1/gencove/command/webhook/verify/cli.py` & `gencove-2.9.0/gencove/command/webhook/verify/cli.py`

 * *Files identical despite different names*

### Comparing `gencove-2.8.1/gencove/command/webhook/verify/utils.py` & `gencove-2.9.0/gencove/command/webhook/verify/utils.py`

 * *Files identical despite different names*

### Comparing `gencove-2.8.1/gencove/constants.py` & `gencove-2.9.0/gencove/constants.py`

 * *Files identical despite different names*

### Comparing `gencove-2.8.1/gencove/description/pypi_readme.md` & `gencove-2.9.0/gencove/description/pypi_readme.md`

 * *Files identical despite different names*

### Comparing `gencove-2.8.1/gencove/logger.py` & `gencove-2.9.0/gencove/logger.py`

 * *Files identical despite different names*

### Comparing `gencove-2.8.1/gencove/models.py` & `gencove-2.9.0/gencove/models.py`

 * *Files identical despite different names*

### Comparing `gencove-2.8.1/gencove/tests/basespace/test_basespace_autoimports_create.py` & `gencove-2.9.0/gencove/tests/basespace/test_basespace_autoimports_create.py`

 * *Files identical despite different names*

### Comparing `gencove-2.8.1/gencove/tests/basespace/test_basespace_autoimports_list.py` & `gencove-2.9.0/gencove/tests/basespace/test_basespace_autoimports_list.py`

 * *Files identical despite different names*

### Comparing `gencove-2.8.1/gencove/tests/basespace/test_basespace_biosamples_list.py` & `gencove-2.9.0/gencove/tests/basespace/test_basespace_biosamples_list.py`

 * *Files identical despite different names*

### Comparing `gencove-2.8.1/gencove/tests/basespace/test_basespace_projects_import.py` & `gencove-2.9.0/gencove/tests/basespace/test_basespace_projects_import.py`

 * *Files identical despite different names*

### Comparing `gencove-2.8.1/gencove/tests/basespace/test_basespace_projects_list.py` & `gencove-2.9.0/gencove/tests/basespace/test_basespace_projects_list.py`

 * *Files identical despite different names*

### Comparing `gencove-2.8.1/gencove/tests/conftest.py` & `gencove-2.9.0/gencove/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `gencove-2.8.1/gencove/tests/decorators.py` & `gencove-2.9.0/gencove/tests/decorators.py`

 * *Files identical despite different names*

### Comparing `gencove-2.8.1/gencove/tests/download/test_cli_download.py` & `gencove-2.9.0/gencove/tests/download/test_cli_download.py`

 * *Files identical despite different names*

### Comparing `gencove-2.8.1/gencove/tests/download/vcr/filters.py` & `gencove-2.9.0/gencove/tests/download/vcr/filters.py`

 * *Files identical despite different names*

### Comparing `gencove-2.8.1/gencove/tests/files/test_file_types_list.py` & `gencove-2.9.0/gencove/tests/files/test_file_types_list.py`

 * *Files identical despite different names*

### Comparing `gencove-2.8.1/gencove/tests/filters.py` & `gencove-2.9.0/gencove/tests/filters.py`

 * *Files identical despite different names*

### Comparing `gencove-2.8.1/gencove/tests/projects/test_projects_batch_get.py` & `gencove-2.9.0/gencove/tests/projects/test_projects_batch_get.py`

 * *Files identical despite different names*

### Comparing `gencove-2.8.1/gencove/tests/projects/test_projects_batch_types_list.py` & `gencove-2.9.0/gencove/tests/projects/test_projects_batch_types_list.py`

 * *Files identical despite different names*

### Comparing `gencove-2.8.1/gencove/tests/projects/test_projects_batches_create.py` & `gencove-2.9.0/gencove/tests/projects/test_projects_batches_create.py`

 * *Files identical despite different names*

### Comparing `gencove-2.8.1/gencove/tests/projects/test_projects_batches_list.py` & `gencove-2.9.0/gencove/tests/projects/test_projects_batches_list.py`

 * *Files identical despite different names*

### Comparing `gencove-2.8.1/gencove/tests/projects/test_projects_create.py` & `gencove-2.9.0/gencove/tests/projects/test_projects_create.py`

 * *Files identical despite different names*

### Comparing `gencove-2.8.1/gencove/tests/projects/test_projects_create_merged_vcf.py` & `gencove-2.9.0/gencove/tests/projects/test_projects_create_merged_vcf.py`

 * *Files identical despite different names*

### Comparing `gencove-2.8.1/gencove/tests/projects/test_projects_create_sample_manifest.py` & `gencove-2.9.0/gencove/tests/projects/test_projects_create_sample_manifest.py`

 * *Files identical despite different names*

### Comparing `gencove-2.8.1/gencove/tests/projects/test_projects_delete.py` & `gencove-2.9.0/gencove/tests/projects/test_projects_delete.py`

 * *Files identical despite different names*

### Comparing `gencove-2.8.1/gencove/tests/projects/test_projects_delete_samples.py` & `gencove-2.9.0/gencove/tests/projects/test_projects_delete_samples.py`

 * *Files identical despite different names*

### Comparing `gencove-2.8.1/gencove/tests/projects/test_projects_get_merged_vcf.py` & `gencove-2.9.0/gencove/tests/projects/test_projects_get_merged_vcf.py`

 * *Files identical despite different names*

### Comparing `gencove-2.8.1/gencove/tests/projects/test_projects_get_sample_manifests.py` & `gencove-2.9.0/gencove/tests/projects/test_projects_get_sample_manifests.py`

 * *Files identical despite different names*

### Comparing `gencove-2.8.1/gencove/tests/projects/test_projects_import_existing_samples.py` & `gencove-2.9.0/gencove/tests/projects/test_projects_import_existing_samples.py`

 * *Files identical despite different names*

### Comparing `gencove-2.8.1/gencove/tests/projects/test_projects_list.py` & `gencove-2.9.0/gencove/tests/projects/test_projects_list.py`

 * *Files identical despite different names*

### Comparing `gencove-2.8.1/gencove/tests/projects/test_projects_pipeline_capabilities_list.py` & `gencove-2.9.0/gencove/tests/projects/test_projects_pipeline_capabilities_list.py`

 * *Files identical despite different names*

### Comparing `gencove-2.8.1/gencove/tests/projects/test_projects_pipelines_list.py` & `gencove-2.9.0/gencove/tests/projects/test_projects_pipelines_list.py`

 * *Files identical despite different names*

### Comparing `gencove-2.8.1/gencove/tests/projects/test_projects_restore_samples.py` & `gencove-2.9.0/gencove/tests/projects/test_projects_restore_samples.py`

 * *Files identical despite different names*

### Comparing `gencove-2.8.1/gencove/tests/projects/test_projects_run_prefix.py` & `gencove-2.9.0/gencove/tests/projects/test_projects_run_prefix.py`

 * *Files identical despite different names*

### Comparing `gencove-2.8.1/gencove/tests/projects/test_projects_samples_list.py` & `gencove-2.9.0/gencove/tests/projects/test_projects_samples_list.py`

 * *Files identical despite different names*

### Comparing `gencove-2.8.1/gencove/tests/projects/test_projects_status_merged_vcf.py` & `gencove-2.9.0/gencove/tests/projects/test_projects_status_merged_vcf.py`

 * *Files identical despite different names*

### Comparing `gencove-2.8.1/gencove/tests/projects/vcr/filters.py` & `gencove-2.9.0/gencove/tests/projects/vcr/filters.py`

 * *Files identical despite different names*

### Comparing `gencove-2.8.1/gencove/tests/reports/test_reports_monthly_usage.py` & `gencove-2.9.0/gencove/tests/reports/test_reports_monthly_usage.py`

 * *Files identical despite different names*

### Comparing `gencove-2.8.1/gencove/tests/reports/test_reports_project_qc.py` & `gencove-2.9.0/gencove/tests/reports/test_reports_project_qc.py`

 * *Files identical despite different names*

### Comparing `gencove-2.8.1/gencove/tests/s3_imports/test_s3_autoimports_create.py` & `gencove-2.9.0/gencove/tests/s3_imports/test_s3_autoimports_create.py`

 * *Files identical despite different names*

### Comparing `gencove-2.8.1/gencove/tests/s3_imports/test_s3_autoimports_list.py` & `gencove-2.9.0/gencove/tests/s3_imports/test_s3_autoimports_list.py`

 * *Files identical despite different names*

### Comparing `gencove-2.8.1/gencove/tests/s3_imports/test_s3_uri_import.py` & `gencove-2.9.0/gencove/tests/s3_imports/test_s3_uri_import.py`

 * *Files identical despite different names*

### Comparing `gencove-2.8.1/gencove/tests/sample_manifests/test_sample_manifests_get_sample_manifest.py` & `gencove-2.9.0/gencove/tests/sample_manifests/test_sample_manifests_get_sample_manifest.py`

 * *Files identical despite different names*

### Comparing `gencove-2.8.1/gencove/tests/samples/test_samples_download_file.py` & `gencove-2.9.0/gencove/tests/samples/test_samples_download_file.py`

 * *Files identical despite different names*

### Comparing `gencove-2.8.1/gencove/tests/samples/test_samples_get_metadata.py` & `gencove-2.9.0/gencove/tests/samples/test_samples_get_metadata.py`

 * *Files identical despite different names*

### Comparing `gencove-2.8.1/gencove/tests/samples/test_samples_set_metadata.py` & `gencove-2.9.0/gencove/tests/samples/test_samples_set_metadata.py`

 * *Files identical despite different names*

### Comparing `gencove-2.8.1/gencove/tests/samples/vcr/filters.py` & `gencove-2.9.0/gencove/tests/samples/vcr/filters.py`

 * *Files identical despite different names*

### Comparing `gencove-2.8.1/gencove/tests/test_logger.py` & `gencove-2.9.0/gencove/tests/test_logger.py`

 * *Files identical despite different names*

### Comparing `gencove-2.8.1/gencove/tests/test_utils.py` & `gencove-2.9.0/gencove/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `gencove-2.8.1/gencove/tests/upload/test_cli_upload.py` & `gencove-2.9.0/gencove/tests/upload/test_cli_upload.py`

 * *Files identical despite different names*

### Comparing `gencove-2.8.1/gencove/tests/upload/vcr/filters.py` & `gencove-2.9.0/gencove/tests/upload/vcr/filters.py`

 * *Files identical despite different names*

### Comparing `gencove-2.8.1/gencove/tests/uploads/test_uploads_list.py` & `gencove-2.9.0/gencove/tests/uploads/test_uploads_list.py`

 * *Files identical despite different names*

### Comparing `gencove-2.8.1/gencove/tests/utils.py` & `gencove-2.9.0/gencove/tests/utils.py`

 * *Files identical despite different names*

### Comparing `gencove-2.8.1/gencove/tests/webhook/test_webhook_verify.py` & `gencove-2.9.0/gencove/tests/webhook/test_webhook_verify.py`

 * *Files identical despite different names*

### Comparing `gencove-2.8.1/gencove/utils.py` & `gencove-2.9.0/gencove/utils.py`

 * *Files identical despite different names*

### Comparing `gencove-2.8.1/gencove.egg-info/PKG-INFO` & `gencove-2.9.0/gencove.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gencove
-Version: 2.8.1
+Version: 2.9.0
 Summary: Gencove API and CLI tool
 Home-page: http://docs.gencove.com
 Author: Tomaz Berisa
 License: Apache 2.0
 Description: # The Gencove CLI
         
         [![PyPI Latest Release](https://img.shields.io/pypi/v/gencove.svg)](https://pypi.org/project/gencove/)
```

### Comparing `gencove-2.8.1/gencove.egg-info/SOURCES.txt` & `gencove-2.9.0/gencove.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -50,14 +50,16 @@
 gencove/command/basespace/projects/basespace_list/utils.py
 gencove/command/download/__init__.py
 gencove/command/download/cli.py
 gencove/command/download/constants.py
 gencove/command/download/exceptions.py
 gencove/command/download/main.py
 gencove/command/download/utils.py
+gencove/command/explorer/__init__.py
+gencove/command/explorer/cli.py
 gencove/command/files/__init__.py
 gencove/command/files/cli.py
 gencove/command/files/main.py
 gencove/command/files/utils.py
 gencove/command/projects/__init__.py
 gencove/command/projects/cli.py
 gencove/command/projects/create/__init__.py
```

### Comparing `gencove-2.8.1/setup.py` & `gencove-2.9.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -43,14 +43,16 @@
         "six>=1.5",
         "Click>=7.0",
         "requests>=2.19.1",
         "boto3>=1.17.97",
         "progressbar2==3.55.0",
         "backoff<=2.2.1",
         "pydantic==1.9.2",
+        "click-default-group>=1.2.4",
+        "sh>=1.14.3",
     ],
     setup_requires=["pytest-runner"],
     tests_require=["pytest", "pytest-mock"],
     entry_points="""
         [console_scripts]
         gencove=gencove.cli:cli
     """,
```


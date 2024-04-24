# Comparing `tmp/dyff-audit-0.3.0.tar.gz` & `tmp/dyff_audit-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dyff-audit-0.3.0.tar", last modified: Fri Apr 12 05:12:25 2024, max compression
+gzip compressed data, was "dyff_audit-0.3.1.tar", last modified: Wed Apr 24 05:33:46 2024, max compression
```

## Comparing `dyff-audit-0.3.0.tar` & `dyff_audit-0.3.1.tar`

### file list

```diff
@@ -1,49 +1,71 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 05:12:25.832653 dyff-audit-0.3.0/
--rw-rw-rw-   0 root         (0) root         (0)      504 2024-04-12 05:12:19.000000 dyff-audit-0.3.0/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     1794 2024-04-12 05:12:19.000000 dyff-audit-0.3.0/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)      375 2024-04-12 05:12:19.000000 dyff-audit-0.3.0/.licenserc.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1800 2024-04-12 05:12:19.000000 dyff-audit-0.3.0/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)      122 2024-04-12 05:12:19.000000 dyff-audit-0.3.0/.prettierignore
--rw-rw-rw-   0 root         (0) root         (0)     2192 2024-04-12 05:12:19.000000 dyff-audit-0.3.0/.secrets.baseline
--rw-rw-rw-   0 root         (0) root         (0)     5503 2024-04-12 05:12:19.000000 dyff-audit-0.3.0/CODE_OF_CONDUCT.md
--rw-rw-rw-   0 root         (0) root         (0)    11357 2024-04-12 05:12:19.000000 dyff-audit-0.3.0/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       49 2024-04-12 05:12:19.000000 dyff-audit-0.3.0/NOTICE
--rw-r--r--   0 root         (0) root         (0)     3438 2024-04-12 05:12:25.831653 dyff-audit-0.3.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2309 2024-04-12 05:12:19.000000 dyff-audit-0.3.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 05:12:25.821653 dyff-audit-0.3.0/dyff/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 05:12:25.826653 dyff-audit-0.3.0/dyff/audit/
--rw-rw-rw-   0 root         (0) root         (0)       92 2024-04-12 05:12:19.000000 dyff-audit-0.3.0/dyff/audit/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 05:12:25.827653 dyff-audit-0.3.0/dyff/audit/analysis/
--rw-rw-rw-   0 root         (0) root         (0)      349 2024-04-12 05:12:19.000000 dyff-audit-0.3.0/dyff/audit/analysis/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6108 2024-04-12 05:12:19.000000 dyff-audit-0.3.0/dyff/audit/analysis/context.py
--rw-rw-rw-   0 root         (0) root         (0)     1689 2024-04-12 05:12:19.000000 dyff-audit-0.3.0/dyff/audit/analysis/jupyter.py
--rw-rw-rw-   0 root         (0) root         (0)     1197 2024-04-12 05:12:19.000000 dyff-audit-0.3.0/dyff/audit/analysis/legacy.py
--rw-rw-rw-   0 root         (0) root         (0)     2842 2024-04-12 05:12:19.000000 dyff-audit-0.3.0/dyff/audit/analysis/python.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 05:12:25.827653 dyff-audit-0.3.0/dyff/audit/data/
--rw-rw-rw-   0 root         (0) root         (0)      217 2024-04-12 05:12:19.000000 dyff-audit-0.3.0/dyff/audit/data/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2368 2024-04-12 05:12:19.000000 dyff-audit-0.3.0/dyff/audit/data/text.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 05:12:25.828653 dyff-audit-0.3.0/dyff/audit/local/
--rw-rw-rw-   0 root         (0) root         (0)      173 2024-04-12 05:12:19.000000 dyff-audit-0.3.0/dyff/audit/local/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    22979 2024-04-12 05:12:19.000000 dyff-audit-0.3.0/dyff/audit/local/platform.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 05:12:25.828653 dyff-audit-0.3.0/dyff/audit/metrics/
--rw-rw-rw-   0 root         (0) root         (0)      233 2024-04-12 05:12:19.000000 dyff-audit-0.3.0/dyff/audit/metrics/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1071 2024-04-12 05:12:19.000000 dyff-audit-0.3.0/dyff/audit/metrics/base.py
--rw-rw-rw-   0 root         (0) root         (0)     4359 2024-04-12 05:12:19.000000 dyff-audit-0.3.0/dyff/audit/metrics/text.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 05:12:25.829653 dyff-audit-0.3.0/dyff/audit/scoring/
--rw-rw-rw-   0 root         (0) root         (0)      261 2024-04-12 05:12:19.000000 dyff-audit-0.3.0/dyff/audit/scoring/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1217 2024-04-12 05:12:19.000000 dyff-audit-0.3.0/dyff/audit/scoring/base.py
--rw-rw-rw-   0 root         (0) root         (0)     3949 2024-04-12 05:12:19.000000 dyff-audit-0.3.0/dyff/audit/scoring/classification.py
--rw-rw-rw-   0 root         (0) root         (0)     1787 2024-04-12 05:12:19.000000 dyff-audit-0.3.0/dyff/audit/scoring/example.py
--rw-rw-rw-   0 root         (0) root         (0)    11999 2024-04-12 05:12:19.000000 dyff-audit-0.3.0/dyff/audit/scoring/text.py
--rw-rw-rw-   0 root         (0) root         (0)     5756 2024-04-12 05:12:19.000000 dyff-audit-0.3.0/dyff/audit/workflows.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 05:12:25.831653 dyff-audit-0.3.0/dyff_audit.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3438 2024-04-12 05:12:25.000000 dyff-audit-0.3.0/dyff_audit.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      905 2024-04-12 05:12:25.000000 dyff-audit-0.3.0/dyff_audit.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-12 05:12:25.000000 dyff-audit-0.3.0/dyff_audit.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       50 2024-04-12 05:12:25.000000 dyff-audit-0.3.0/dyff_audit.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2024-04-12 05:12:25.000000 dyff-audit-0.3.0/dyff_audit.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      526 2024-04-12 05:12:19.000000 dyff-audit-0.3.0/makefile
--rw-rw-rw-   0 root         (0) root         (0)     1755 2024-04-12 05:12:19.000000 dyff-audit-0.3.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-12 05:12:25.832653 dyff-audit-0.3.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 05:12:25.831653 dyff-audit-0.3.0/tests/
--rw-rw-rw-   0 root         (0) root         (0)      661 2024-04-12 05:12:19.000000 dyff-audit-0.3.0/tests/test_import.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 05:33:46.486544 dyff_audit-0.3.1/
+-rw-rw-rw-   0 root         (0) root         (0)      504 2024-04-24 05:33:40.000000 dyff_audit-0.3.1/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     1839 2024-04-24 05:33:40.000000 dyff_audit-0.3.1/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)      396 2024-04-24 05:33:40.000000 dyff_audit-0.3.1/.licenserc.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1800 2024-04-24 05:33:40.000000 dyff_audit-0.3.1/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      122 2024-04-24 05:33:40.000000 dyff_audit-0.3.1/.prettierignore
+-rw-rw-rw-   0 root         (0) root         (0)     2192 2024-04-24 05:33:40.000000 dyff_audit-0.3.1/.secrets.baseline
+-rw-rw-rw-   0 root         (0) root         (0)     5503 2024-04-24 05:33:40.000000 dyff_audit-0.3.1/CODE_OF_CONDUCT.md
+-rw-rw-rw-   0 root         (0) root         (0)    11357 2024-04-24 05:33:40.000000 dyff_audit-0.3.1/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       49 2024-04-24 05:33:40.000000 dyff_audit-0.3.1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     3690 2024-04-24 05:33:46.486544 dyff_audit-0.3.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2309 2024-04-24 05:33:40.000000 dyff_audit-0.3.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 05:33:46.469545 dyff_audit-0.3.1/dyff/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 05:33:46.476544 dyff_audit-0.3.1/dyff/audit/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2024-04-24 05:33:40.000000 dyff_audit-0.3.1/dyff/audit/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 05:33:46.477544 dyff_audit-0.3.1/dyff/audit/analysis/
+-rw-rw-rw-   0 root         (0) root         (0)      295 2024-04-24 05:33:40.000000 dyff_audit-0.3.1/dyff/audit/analysis/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6108 2024-04-24 05:33:40.000000 dyff_audit-0.3.1/dyff/audit/analysis/context.py
+-rw-rw-rw-   0 root         (0) root         (0)     1689 2024-04-24 05:33:40.000000 dyff_audit-0.3.1/dyff/audit/analysis/jupyter.py
+-rw-rw-rw-   0 root         (0) root         (0)     1179 2024-04-24 05:33:40.000000 dyff_audit-0.3.1/dyff/audit/analysis/legacy.py
+-rw-rw-rw-   0 root         (0) root         (0)     2814 2024-04-24 05:33:40.000000 dyff_audit-0.3.1/dyff/audit/analysis/python.py
+-rw-rw-rw-   0 root         (0) root         (0)     3401 2024-04-24 05:33:40.000000 dyff_audit-0.3.1/dyff/audit/analysis/runner.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 05:33:46.478545 dyff_audit-0.3.1/dyff/audit/data/
+-rw-rw-rw-   0 root         (0) root         (0)      217 2024-04-24 05:33:40.000000 dyff_audit-0.3.1/dyff/audit/data/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2368 2024-04-24 05:33:40.000000 dyff_audit-0.3.1/dyff/audit/data/text.py
+-rw-rw-rw-   0 root         (0) root         (0)      485 2024-04-24 05:33:40.000000 dyff_audit-0.3.1/dyff/audit/dynamic_import.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 05:33:46.478545 dyff_audit-0.3.1/dyff/audit/local/
+-rw-rw-rw-   0 root         (0) root         (0)      173 2024-04-24 05:33:40.000000 dyff_audit-0.3.1/dyff/audit/local/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    24096 2024-04-24 05:33:40.000000 dyff_audit-0.3.1/dyff/audit/local/platform.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 05:33:46.479544 dyff_audit-0.3.1/dyff/audit/metrics/
+-rw-rw-rw-   0 root         (0) root         (0)      233 2024-04-24 05:33:40.000000 dyff_audit-0.3.1/dyff/audit/metrics/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1071 2024-04-24 05:33:40.000000 dyff_audit-0.3.1/dyff/audit/metrics/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     4359 2024-04-24 05:33:40.000000 dyff_audit-0.3.1/dyff/audit/metrics/text.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 05:33:46.481544 dyff_audit-0.3.1/dyff/audit/scoring/
+-rw-rw-rw-   0 root         (0) root         (0)      261 2024-04-24 05:33:40.000000 dyff_audit-0.3.1/dyff/audit/scoring/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1217 2024-04-24 05:33:40.000000 dyff_audit-0.3.1/dyff/audit/scoring/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     3949 2024-04-24 05:33:40.000000 dyff_audit-0.3.1/dyff/audit/scoring/classification.py
+-rw-rw-rw-   0 root         (0) root         (0)     1787 2024-04-24 05:33:40.000000 dyff_audit-0.3.1/dyff/audit/scoring/example.py
+-rw-rw-rw-   0 root         (0) root         (0)    11999 2024-04-24 05:33:40.000000 dyff_audit-0.3.1/dyff/audit/scoring/text.py
+-rw-rw-rw-   0 root         (0) root         (0)     5994 2024-04-24 05:33:40.000000 dyff_audit-0.3.1/dyff/audit/workflows.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 05:33:46.485544 dyff_audit-0.3.1/dyff_audit.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3690 2024-04-24 05:33:46.000000 dyff_audit-0.3.1/dyff_audit.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1411 2024-04-24 05:33:46.000000 dyff_audit-0.3.1/dyff_audit.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-24 05:33:46.000000 dyff_audit-0.3.1/dyff_audit.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      136 2024-04-24 05:33:46.000000 dyff_audit-0.3.1/dyff_audit.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2024-04-24 05:33:46.000000 dyff_audit-0.3.1/dyff_audit.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      526 2024-04-24 05:33:40.000000 dyff_audit-0.3.1/makefile
+-rw-rw-rw-   0 root         (0) root         (0)     1911 2024-04-24 05:33:40.000000 dyff_audit-0.3.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-24 05:33:46.486544 dyff_audit-0.3.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 05:33:46.482545 dyff_audit-0.3.1/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      193 2024-04-24 05:33:40.000000 dyff_audit-0.3.1/tests/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 05:33:46.472545 dyff_audit-0.3.1/tests/data/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 05:33:46.483544 dyff_audit-0.3.1/tests/data/dataset/
+-rw-rw-rw-   0 root         (0) root         (0)     1196 2024-04-24 05:33:40.000000 dyff_audit-0.3.1/tests/data/dataset/part-0.parquet
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 05:33:46.483544 dyff_audit-0.3.1/tests/data/evaluation/
+-rw-rw-rw-   0 root         (0) root         (0)     2990 2024-04-24 05:33:40.000000 dyff_audit-0.3.1/tests/data/evaluation/part-0.parquet
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 05:33:46.483544 dyff_audit-0.3.1/tests/data/module_jupyter_notebook/
+-rw-rw-rw-   0 root         (0) root         (0)      139 2024-04-24 05:33:40.000000 dyff_audit-0.3.1/tests/data/module_jupyter_notebook/notebook_dependency.py
+-rw-rw-rw-   0 root         (0) root         (0)     5740 2024-04-24 05:33:40.000000 dyff_audit-0.3.1/tests/data/module_jupyter_notebook/test-notebook.ipynb
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 05:33:46.472545 dyff_audit-0.3.1/tests/data/module_python_function/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 05:33:46.472545 dyff_audit-0.3.1/tests/data/module_python_function/dyff/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 05:33:46.484544 dyff_audit-0.3.1/tests/data/module_python_function/dyff/fake/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2024-04-24 05:33:40.000000 dyff_audit-0.3.1/tests/data/module_python_function/dyff/fake/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1974 2024-04-24 05:33:40.000000 dyff_audit-0.3.1/tests/data/module_python_function/dyff/fake/method.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 05:33:46.472545 dyff_audit-0.3.1/tests/data/module_python_rubric/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 05:33:46.472545 dyff_audit-0.3.1/tests/data/module_python_rubric/dyff/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 05:33:46.484544 dyff_audit-0.3.1/tests/data/module_python_rubric/dyff/fake/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2024-04-24 05:33:40.000000 dyff_audit-0.3.1/tests/data/module_python_rubric/dyff/fake/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1726 2024-04-24 05:33:40.000000 dyff_audit-0.3.1/tests/data/module_python_rubric/dyff/fake/rubric.py
+-rw-rw-rw-   0 root         (0) root         (0)      948 2024-04-24 05:33:40.000000 dyff_audit-0.3.1/tests/test_import.py
+-rw-rw-rw-   0 root         (0) root         (0)    10808 2024-04-24 05:33:40.000000 dyff_audit-0.3.1/tests/test_local_platform.py
```

### Comparing `dyff-audit-0.3.0/.gitlab-ci.yml` & `dyff_audit-0.3.1/.gitlab-ci.yml`

 * *Files 10% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 include:
   - project: buildgarden/pipelines/gitlab
     ref: 0.2.2
     file:
       - gitlab-release.yml
   - project: buildgarden/pipelines/detect-secrets
-    ref: 0.1.0
+    ref: 0.2.1
     file:
       - detect-secrets.yml
   - project: buildgarden/pipelines/prettier
     ref: 0.3.2
     file:
       - prettier.yml
   - project: buildgarden/pipelines/python
@@ -44,14 +44,16 @@
       - python-docformatter.yml
   - project: buildgarden/pipelines/skywalking-eyes
     ref: 0.2.0
     file:
       - license-eye-header-check.yml
 
 python-pytest:
+  variables:
+    PYTHON_REQUIREMENTS: .[dev]
   parallel:
     matrix:
       - PYTHON_VERSION: ['3.9', '3.10', '3.11', '3.12']
 
 dyff-audit-install-test:
   stage: test
   image: ${CONTAINER_PROXY}python:3.9-bookworm
```

### Comparing `dyff-audit-0.3.0/.pre-commit-config.yaml` & `dyff_audit-0.3.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dyff-audit-0.3.0/.secrets.baseline` & `dyff_audit-0.3.1/.secrets.baseline`

 * *Files identical despite different names*

### Comparing `dyff-audit-0.3.0/CODE_OF_CONDUCT.md` & `dyff_audit-0.3.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `dyff-audit-0.3.0/LICENSE` & `dyff_audit-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dyff-audit-0.3.0/PKG-INFO` & `dyff_audit-0.3.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dyff-audit
-Version: 0.3.0
+Version: 0.3.1
 Summary: Audit tools for the Dyff AI auditing platform.
 Author-email: Digital Safety Research Institute <contact@dsri.org>
 License: Apache-2.0
 Project-URL: Home, https://gitlab.com/dyff/packages/dyff-audit
 Project-URL: Issues, https://gitlab.com/dyff/packages/dyff-audit/-/issues
 Keywords: ai,audit,safety,evaluation
 Classifier: Development Status :: 3 - Alpha
@@ -19,17 +19,25 @@
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: NOTICE
 Requires-Dist: dyff-client
 Requires-Dist: dyff-schema
+Requires-Dist: nbconvert
+Requires-Dist: nbformat
+Requires-Dist: notebook
 Requires-Dist: pandas
 Requires-Dist: pyarrow
 Requires-Dist: pydantic<2
+Requires-Dist: ruamel.yaml
+Provides-Extra: dev
+Requires-Dist: pytest; extra == "dev"
+Requires-Dist: pytest-datafiles; extra == "dev"
+Requires-Dist: pytest-depends; extra == "dev"
 
 # dyff-audit
 
 <!-- BADGIE TIME -->
 
 [![pipeline status](https://img.shields.io/gitlab/pipeline-status/dyff/packages/dyff-audit?branch=main)](https://gitlab.com/dyff/packages/dyff-audit/-/commits/main)
 [![coverage report](https://img.shields.io/gitlab/pipeline-coverage/dyff/packages/dyff-audit?branch=main)](https://gitlab.com/dyff/packages/dyff-audit/-/commits/main)
```

### Comparing `dyff-audit-0.3.0/README.md` & `dyff_audit-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `dyff-audit-0.3.0/dyff/audit/analysis/context.py` & `dyff_audit-0.3.1/dyff/audit/analysis/context.py`

 * *Files identical despite different names*

### Comparing `dyff-audit-0.3.0/dyff/audit/analysis/jupyter.py` & `dyff_audit-0.3.1/dyff/audit/analysis/jupyter.py`

 * *Files identical despite different names*

### Comparing `dyff-audit-0.3.0/dyff/audit/analysis/legacy.py` & `dyff_audit-0.3.1/dyff/audit/analysis/legacy.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 # SPDX-FileCopyrightText: 2024 UL Research Institutes
 # SPDX-License-Identifier: Apache-2.0
 
 # mypy: disable-error-code="import-untyped"
 import sys
 from typing import Optional
 
-from dyff.audit.scoring import Rubric
 from dyff.schema.dataset import arrow
-from dyff.storage import dynamic_import
+
+from .. import dynamic_import
+from ..scoring import Rubric
 
 
 def run_python_rubric(
     *,
     rubric: str,
     dataset_path: str,
     evaluation_path: str,
```

### Comparing `dyff-audit-0.3.0/dyff/audit/analysis/python.py` & `dyff_audit-0.3.1/dyff/audit/analysis/python.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # SPDX-FileCopyrightText: 2024 UL Research Institutes
 # SPDX-License-Identifier: Apache-2.0
 
-
-from dyff.audit.analysis import AnalysisContext
-from dyff.audit.scoring import Rubric
 from dyff.schema.dataset import arrow
 from dyff.schema.platform import (
     MeasurementLevel,
     MethodImplementationKind,
     MethodOutputKind,
 )
-from dyff.storage import dynamic_import
+
+from .. import dynamic_import
+from ..analysis import AnalysisContext
+from ..scoring import Rubric
 
 
 def run_python_function():
     ctx = AnalysisContext()
     implementation = ctx.analysis.method.implementation
     if (
         implementation.kind != MethodImplementationKind.PythonFunction
```

### Comparing `dyff-audit-0.3.0/dyff/audit/data/text.py` & `dyff_audit-0.3.1/dyff/audit/data/text.py`

 * *Files identical despite different names*

### Comparing `dyff-audit-0.3.0/dyff/audit/local/platform.py` & `dyff_audit-0.3.1/dyff/audit/local/platform.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,49 +1,54 @@
 # SPDX-FileCopyrightText: 2024 UL Research Institutes
 # SPDX-License-Identifier: Apache-2.0
 
 # mypy: disable-error-code="import-untyped"
 from __future__ import annotations
 
 import json
-import os
-import sys
 from datetime import datetime
 from pathlib import Path
-from typing import Iterable, Optional, TypeVar
+from typing import Any, Iterable, Optional, TypeVar
 
 import pyarrow
 import ruamel.yaml
 
 from dyff.client import Client
 from dyff.schema import ids
 from dyff.schema.dataset import arrow, binary
 from dyff.schema.platform import (
     Analysis,
     Artifact,
     DataSchema,
     Dataset,
     Digest,
     EntityStatus,
+    Evaluation,
+    ForeignInferenceService,
     ForeignMethod,
+    InferenceInterface,
+    InferenceSessionSpec,
     Measurement,
     Method,
-    MethodImplementationKind,
     MethodInputKind,
     Module,
+    Report,
     SafetyCase,
 )
 from dyff.schema.requests import (
     AnalysisCreateRequest,
     DatasetCreateRequest,
+    EvaluationCreateRequest,
     MethodCreateRequest,
     ModuleCreateRequest,
+    ReportCreateRequest,
 )
 
-from ..analysis import run_jupyter_notebook, run_python_function, run_python_rubric
+from ..analysis import run_analysis, run_report
+from ..workflows import local_evaluation
 
 T = TypeVar("T")
 
 
 def _once(x: T) -> Iterable[T]:
     yield x
 
@@ -57,24 +62,22 @@
         dataset_dict = dataset_request.dict()
         dataset_dict["id"] = id
         dataset_dict["account"] = self._platform.account
         dataset_dict["status"] = EntityStatus.ready
         dataset_dict["creationTime"] = datetime.now()
         dataset = Dataset.parse_obj(dataset_dict)
 
-        cache_dir = self._platform.storage_root / id
-        if cache_dir.exists():
-            raise ValueError(f"directory exists: {cache_dir}")
+        cache_dir = self._platform.entity_path(id)
         cache_dir.mkdir()
         with open(cache_dir / ".dataset.json", "w") as fout:
             fout.write(dataset.json())
         return dataset
 
     def get(self, id: str) -> Dataset:
-        file = self._platform.storage_root / id / ".dataset.json"
+        file = self._platform.entity_path(id) / ".dataset.json"
         return Dataset.parse_file(file)
 
     def create_arrow_dataset(
         self, dataset_directory: str, *, account: str, name: str
     ) -> Dataset:
         """Create a Dataset resource describing an existing Arrow dataset.
 
@@ -149,28 +152,70 @@
                     fout.write(fin.read())
 
 
 class _Evaluations:
     def __init__(self, platform: DyffLocalPlatform):
         self._platform = platform
 
-    def import_data(self, dataset_directory: str) -> str:
+    def import_data(
+        self,
+        dataset_directory: Path | str,
+        *,
+        id: Optional[str] = None,
+        evaluation_request: Optional[EvaluationCreateRequest] = None,
+    ) -> Evaluation:
         """Imports existing data into the local cache under a newly-generated ID. Useful
         when you already have evaluation data and you want to make it available to other
         workflows using the local platform.
 
         :param dataset_directory: The root directory of the Arrow dataset.
         :type dataset_directory: str
         :returns: The ID of the imported data in the local platform.
         :rtype: str
         """
-        id = ids.generate_entity_id()
         dataset_path = Path(dataset_directory)
         ds = arrow.open_dataset(str(dataset_path))
         file_paths = list(ds.files)
+
+        replications = set()
+        for row in ds.to_table().to_pylist():
+            replications.add(row["_replication_"])
+
+        evaluation_dict: dict[str, Any] = {}
+        evaluation_dict["id"] = id or ids.generate_entity_id()
+        evaluation_dict["account"] = (
+            evaluation_request and evaluation_request.account
+        ) or ids.null_id()
+        evaluation_dict["dataset"] = (
+            evaluation_request and evaluation_request.dataset
+        ) or ids.null_id()
+        evaluation_dict["replications"] = len(replications)
+
+        service_id = (
+            evaluation_request and evaluation_request.inferenceSession.inferenceService
+        ) or ids.null_id()
+        session_spec = InferenceSessionSpec(
+            inferenceService=ForeignInferenceService(
+                id=service_id,
+                name="",
+                account=ids.null_id(),
+                interface=InferenceInterface(
+                    endpoint="",
+                    outputSchema=DataSchema(arrowSchema=arrow.encode_schema(ds.schema)),
+                ),
+            )
+        )
+        evaluation_dict["inferenceSession"] = session_spec.dict()
+        evaluation = Evaluation.parse_obj(evaluation_dict)
+
+        cache_dir = self._platform.entity_path(evaluation.id)
+        cache_dir.mkdir()
+        with open(cache_dir / ".evaluation.json", "w") as fout:
+            fout.write(evaluation.json())
+
         artifact_paths = [
             str(Path(file_path).relative_to(dataset_path)) for file_path in file_paths
         ]
         artifacts = [
             Artifact(
                 kind="parquet",
                 path=artifact_path,
@@ -179,100 +224,94 @@
                 ),
             )
             for file_path, artifact_path in zip(file_paths, artifact_paths)
         ]
         for artifact in artifacts:
             assert artifact.digest.md5 is not None
             file_path = Path(dataset_directory) / artifact.path
-            cache_path = self._platform.storage_root / id / artifact.path
+            cache_path = self._platform.entity_path(evaluation.id) / artifact.path
             cache_path.parent.mkdir(parents=True, exist_ok=True)
             with open(file_path, "rb") as fin:
                 with open(cache_path, "wb") as fout:
                     fout.write(fin.read())
-        return id
+        return evaluation
+
+    def local_evaluation(self, *, dataset: str, inferencesession: str) -> str:
+        client = self._platform._require_client()
+        session = client.inferencesessions.get(inferencesession)
+        id = ids.generate_entity_id()
+        return local_evaluation(
+            client,
+            session,
+            input_dataset_path=self._platform.entity_path(dataset),
+            # workflows.local_evaluation() creates an /id subdirectory for the output
+            output_dataset_path=self._platform.storage_root,
+            id=id,
+        )
+
+    def get(self, id: str) -> Evaluation:
+        file = self._platform.entity_path(id) / ".evaluation.json"
+        return Evaluation.parse_file(file)
 
 
 class _Measurements:
     def __init__(self, platform: DyffLocalPlatform):
         self._platform = platform
 
     def create(self, analysis_request: AnalysisCreateRequest) -> Measurement:
         id = ids.generate_entity_id()
-        print(f"Measurement.id: {id}")
 
         method_id = analysis_request.method
         method = self._platform.methods.get(method_id)
 
         # Create an entity representing the output of the Analysis
         measurement_spec = method.output.measurement
         if measurement_spec is None:
             raise ValueError("Method spec violates constraints")
 
         measurement = Measurement(
             account=analysis_request.account,
             id=id,
             creationTime=datetime.now(),
-            status=EntityStatus.ready,
+            status=EntityStatus.complete,
             scope=analysis_request.scope,
             method=ForeignMethod.parse_obj(method.dict()),
             arguments=analysis_request.arguments,
             inputs=analysis_request.inputs,
             **measurement_spec.dict(),
         )
 
-        cache_dir = self._platform.storage_root / id
-        if cache_dir.exists():
-            raise ValueError(f"directory exists: {cache_dir}")
+        cache_dir = self._platform.entity_path(id)
         cache_dir.mkdir()
         with open(cache_dir / ".measurement.json", "w") as fout:
             fout.write(measurement.json())
 
         analysis = Analysis.parse_obj(measurement.dict())
         # This fixes some things that YAML can't parse (like Enums)
         analysis_dict = json.loads(analysis.json())
         analysis_dict["id"] = id
         # Code expects a full k8s manifest
         # TODO: Should only pass the 'spec' part in the first place from
         # dyff-operator, but that requires figuring out how to manipulate YAML in Go
         analysis_dict = {"spec": analysis_dict}
+        config_file = cache_dir / ".analysis.yaml"
         yaml = ruamel.yaml.YAML()
-        with open(cache_dir / ".analysis.yaml", "w") as fout:
+        with open(config_file, "w") as fout:
             yaml.dump(analysis_dict, fout)
 
-        old_path = sys.path.copy()
-        old_environ = os.environ.copy()
-
-        try:
-            for module in method.modules:
-                sys.path.append(str(self._platform.storage_root / module))
-
-            os.environ["DYFF_AUDIT_LOCAL_STORAGE_ROOT"] = str(
-                self._platform.storage_root
-            )
-            os.environ["DYFF_AUDIT_ANALYSIS_CONFIG_FILE"] = str(
-                cache_dir / ".analysis.yaml"
-            )
-
-            if method.implementation.kind == MethodImplementationKind.PythonFunction:
-                run_python_function()
-            elif method.implementation.kind == MethodImplementationKind.PythonRubric:
-                run_python_rubric()
-            else:
-                raise NotImplementedError(
-                    f"method.implementation.kind = {method.implementation.kind}"
-                )
-        finally:
-            sys.path = old_path
-            os.environ.clear()
-            os.environ.update(old_environ)
+        run_analysis(
+            method,
+            storage_root=self._platform.storage_root,
+            config_file=config_file,
+        )
 
         return measurement
 
     def get(self, id: str) -> Measurement:
-        file = self._platform.storage_root / id / ".measurement.json"
+        file = self._platform.entity_path(id) / ".measurement.json"
         return Measurement.parse_file(file)
 
 
 class _Methods:
     def __init__(self, platform: DyffLocalPlatform):
         self._platform = platform
 
@@ -281,24 +320,22 @@
         method_dict = method_request.dict()
         method_dict["id"] = id
         method_dict["account"] = self._platform.account
         method_dict["status"] = EntityStatus.ready
         method_dict["creationTime"] = datetime.now()
         method = Method.parse_obj(method_dict)
 
-        cache_dir = self._platform.storage_root / id
-        if cache_dir.exists():
-            raise ValueError(f"directory exists: {cache_dir}")
+        cache_dir = self._platform.entity_path(id)
         cache_dir.mkdir()
         with open(cache_dir / ".method.json", "w") as fout:
             fout.write(method.json())
         return method
 
     def get(self, id: str) -> Method:
-        file = self._platform.storage_root / id / ".method.json"
+        file = self._platform.entity_path(id) / ".method.json"
         return Method.parse_file(file)
 
 
 class _Modules:
     def __init__(self, platform: DyffLocalPlatform):
         self._platform = platform
 
@@ -307,24 +344,22 @@
         module_dict = module_request.dict()
         module_dict["id"] = id
         module_dict["account"] = self._platform.account
         module_dict["status"] = EntityStatus.ready
         module_dict["creationTime"] = datetime.now()
         module = Module.parse_obj(module_dict)
 
-        cache_dir = self._platform.storage_root / id
-        if cache_dir.exists():
-            raise ValueError(f"directory exists: {cache_dir}")
+        cache_dir = self._platform.entity_path(id)
         cache_dir.mkdir()
         with open(cache_dir / ".module.json", "w") as fout:
             fout.write(module.json())
         return module
 
     def get(self, id: str) -> Module:
-        file = self._platform.storage_root / id / ".module.json"
+        file = self._platform.entity_path(id) / ".module.json"
         return Module.parse_file(file)
 
     def create_package(
         self, package_directory: str, *, account: str, name: str
     ) -> Module:
         """Create a Module resource describing a package structured as a directory tree.
 
@@ -395,91 +430,104 @@
             cache_path = self._platform.storage_root / module.id / artifact.path
             cache_path.parent.mkdir(parents=True, exist_ok=True)
             with open(file_path, "rb") as fin:
                 with open(cache_path, "wb") as fout:
                     fout.write(fin.read())
 
 
+class _Reports:
+    def __init__(self, platform: DyffLocalPlatform):
+        self._platform = platform
+
+    def create(self, report_request: ReportCreateRequest) -> Report:
+        id = ids.generate_entity_id()
+        report_dict = report_request.dict()
+        report_dict["id"] = id
+        report_dict["account"] = self._platform.account
+        report_dict["status"] = EntityStatus.ready
+        report_dict["creationTime"] = datetime.now()
+
+        evaluation = self._platform.evaluations.get(report_request.evaluation)
+        report_dict["dataset"] = evaluation.dataset
+        report_dict["inferenceService"] = (
+            evaluation.inferenceSession.inferenceService.id
+        )
+
+        report = Report.parse_obj(report_dict)
+
+        cache_dir = self._platform.entity_path(id)
+        cache_dir.mkdir()
+        with open(cache_dir / ".report.json", "w") as fout:
+            fout.write(report.json())
+
+        run_report(report, storage_root=self._platform.storage_root)
+
+        return report
+
+    def get(self, id: str) -> Module:
+        file = self._platform.entity_path(id) / ".module.json"
+        return Module.parse_file(file)
+
+
 class _SafetyCases:
     def __init__(self, platform: DyffLocalPlatform):
         self._platform = platform
 
     def create(self, analysis_request: AnalysisCreateRequest) -> SafetyCase:
         id = ids.generate_entity_id()
-        print(f"SafetyCase.id: {id}")
 
         method_id = analysis_request.method
         method = self._platform.methods.get(method_id)
 
         # Create an entity representing the output of the Analysis
         safetycase_spec = method.output.safetyCase
         if safetycase_spec is None:
             raise ValueError("Method spec violates constraints")
 
         safetycase = SafetyCase(
             account=analysis_request.account,
             id=id,
             creationTime=datetime.now(),
-            status=EntityStatus.ready,
+            status=EntityStatus.complete,
             scope=analysis_request.scope,
             method=ForeignMethod.parse_obj(method.dict()),
             arguments=analysis_request.arguments,
             inputs=analysis_request.inputs,
             # This covers: .name, .description
             **safetycase_spec.dict(),
         )
 
-        cache_dir = self._platform.storage_root / id
-        if cache_dir.exists():
-            raise ValueError(f"directory exists: {cache_dir}")
+        cache_dir = self._platform.entity_path(id)
         cache_dir.mkdir()
         with open(cache_dir / ".safetycase.json", "w") as fout:
             fout.write(safetycase.json())
 
         analysis = Analysis.parse_obj(safetycase.dict())
         # This fixes some things that YAML can't parse (like Enums)
         analysis_dict = json.loads(analysis.json())
         analysis_dict["id"] = id
         # Code expects a full k8s manifest
         # TODO: Should only pass the 'spec' part in the first place from
         # dyff-operator, but that requires figuring out how to manipulate YAML in Go
         analysis_dict = {"spec": analysis_dict}
+        config_file = cache_dir / ".analysis.yaml"
         yaml = ruamel.yaml.YAML()
-        with open(cache_dir / ".analysis.yaml", "w") as fout:
+        with open(config_file, "w") as fout:
             yaml.dump(analysis_dict, fout)
 
-        old_path = sys.path.copy()
-        old_environ = os.environ.copy()
-
-        try:
-            for module in method.modules:
-                sys.path.append(str(self._platform.storage_root / module))
-
-            os.environ["DYFF_AUDIT_LOCAL_STORAGE_ROOT"] = str(
-                self._platform.storage_root
-            )
-            os.environ["DYFF_AUDIT_ANALYSIS_CONFIG_FILE"] = str(
-                cache_dir / ".analysis.yaml"
-            )
-
-            if method.implementation.kind == MethodImplementationKind.JupyterNotebook:
-                run_jupyter_notebook()
-            else:
-                raise NotImplementedError(
-                    f"method.implementation.kind = {method.implementation.kind}"
-                )
-        finally:
-            sys.path = old_path
-            os.environ.clear()
-            os.environ.update(old_environ)
+        run_analysis(
+            method,
+            storage_root=self._platform.storage_root,
+            config_file=config_file,
+        )
 
         return safetycase
 
     def get(self, id: str) -> SafetyCase:
-        file = self._platform.storage_root / id / ".safetycase.json"
+        file = self._platform.entity_path(id) / ".safetycase.json"
         return SafetyCase.parse_file(file)
 
 
 class DyffLocalPlatform:
     """Emulates a subset of Dyff Platform operations locally.
 
     This class is intended to aid in local development and debugging of code
@@ -492,52 +540,39 @@
     instance if the requested entity is not available locally. API calls that
     modify the platform state are **never** forwarded to a remote instance.
     """
 
     def __init__(
         self,
         storage_root: Path,
-        use_remote: bool = False,
-        api_endpoint: Optional[str] = None,
-        api_token: Optional[str] = None,
-        insecure: bool = False,
+        *,
+        remote_client: Optional[Client] = None,
     ):
         self._storage_root = storage_root
-
-        self._use_remote = use_remote
-        if self._use_remote:
-            raise NotImplementedError("forwarding to remote not implemented yet")
-
-        self._api_endpoint = (
-            api_endpoint
-            or os.environ.get("DYFF_API_ENDPOINT")
-            or "https://api.dyff.io/v0"
-        )
-        self._api_token = api_token or os.environ.get("DYFF_API_TOKEN")
-        self._insecure = insecure or (os.environ.get("DYFF_API_INSECURE") == "1")
-
-        self._client: Optional[Client] = None
-        if self._use_remote:
-            if self._api_token is None:
-                raise ValueError(
-                    "API token not specified; set use_remote=False to disable remote access"
-                )
-            self._client = Client(
-                api_key=self._api_token,
-                endpoint=self._api_endpoint,
-                verify_ssl_certificates=(not insecure),
-            )
+        self._client = remote_client
 
         self._datasets = _Datasets(self)
         self._evaluations = _Evaluations(self)
         self._measurements = _Measurements(self)
         self._methods = _Methods(self)
         self._modules = _Modules(self)
+        self._reports = _Reports(self)
         self._safetycases = _SafetyCases(self)
 
+        self._storage_root.mkdir(exist_ok=True)
+
+    def _require_client(self) -> Client:
+        if not self._client:
+            raise ValueError("remote client not available")
+        return self._client
+
+    @property
+    def remote(self) -> Client | None:
+        return self._client
+
     @property
     def datasets(self) -> _Datasets:
         return self._datasets
 
     @property
     def evaluations(self) -> _Evaluations:
         return self._evaluations
@@ -551,25 +586,34 @@
         return self._methods
 
     @property
     def modules(self) -> _Modules:
         return self._modules
 
     @property
+    def reports(self) -> _Reports:
+        return self._reports
+
+    @property
     def safetycases(self) -> _SafetyCases:
         return self._safetycases
 
     @property
     def storage_root(self) -> Path:
         return self._storage_root
 
     @property
     def account(self) -> str:
         return "local"
 
+    def entity_path(self, id: str) -> Path:
+        """Returns the path to the local directory that stores information about the
+        entity with the given ID."""
+        return self.storage_root / id
+
     def link_entity(self, package: Path, id: Optional[str] = None) -> str:
         """Creates a symlink in the local storage tree pointing to a directory on the
         file system. You can either provide an ID or let the platform generate one.
         Returns the assigned ID.
 
         This can be used to create an "editable" package so that you can refer to the
         package at a stable ID while still changing the contents of the files in it.
```

### Comparing `dyff-audit-0.3.0/dyff/audit/metrics/base.py` & `dyff_audit-0.3.1/dyff/audit/metrics/base.py`

 * *Files identical despite different names*

### Comparing `dyff-audit-0.3.0/dyff/audit/metrics/text.py` & `dyff_audit-0.3.1/dyff/audit/metrics/text.py`

 * *Files identical despite different names*

### Comparing `dyff-audit-0.3.0/dyff/audit/scoring/base.py` & `dyff_audit-0.3.1/dyff/audit/scoring/base.py`

 * *Files identical despite different names*

### Comparing `dyff-audit-0.3.0/dyff/audit/scoring/classification.py` & `dyff_audit-0.3.1/dyff/audit/scoring/classification.py`

 * *Files identical despite different names*

### Comparing `dyff-audit-0.3.0/dyff/audit/scoring/example.py` & `dyff_audit-0.3.1/dyff/audit/scoring/example.py`

 * *Files identical despite different names*

### Comparing `dyff-audit-0.3.0/dyff/audit/scoring/text.py` & `dyff_audit-0.3.1/dyff/audit/scoring/text.py`

 * *Files identical despite different names*

### Comparing `dyff-audit-0.3.0/dyff/audit/workflows.py` & `dyff_audit-0.3.1/dyff/audit/workflows.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # SPDX-FileCopyrightText: 2024 UL Research Institutes
 # SPDX-License-Identifier: Apache-2.0
 
 # mypy: disable-error-code="import-untyped"
 from __future__ import annotations
 
 from pathlib import Path
-from typing import Iterable
+from typing import Iterable, Optional
 
 import pyarrow
 
 from dyff.client import Client
 from dyff.schema import ids
 from dyff.schema.dataset import arrow
 from dyff.schema.platform import InferenceSession
@@ -20,14 +20,15 @@
 def local_evaluation(
     client: Client,
     session: InferenceSession,
     *,
     input_dataset_path: Path | str,
     output_dataset_path: Path | str,
     replications: int = 1,
+    id: Optional[str] = None,
 ) -> str:
     """Emulate an Evaluation workflow by feeding data from a local Arrow dataset to an
     InferenceSession running on the Dyff platform.
 
     The output dataset will have the same schema as the outputs from an
     Evaluation run on the platform, including fields added by the platform
     -- ``_index_``, ``_replication_``, etc.
@@ -47,25 +48,29 @@
     :keyword output_dataset_path: The directory where the Arrow output dataset
         should be created. A subdirectory named with the ID of the simulated
         evaluation will be created.
     :type output_dataset_path: Path | str
     :keyword replications: The number of replications to run. Equivalent to the
         ``EvaluationCreateRequest.replications`` parameter.
     :type replications: int
-    :returns: An ID for the simulated evaluation. This will not correspond to
+    :keyword id: If specified, use this ID for the evaluation. Otherwise,
+        generate a new ID.
+    :type id: str
+    :returns: An ID for the simulated evaluation, either the ID provided as
+        an argument, or a newly-generated one. This will not correspond to
         an entity in the Dyff datastore, but it can be used to derive the IDs
         of replications in the output dataset.
     :rtype: str
     """
     session_token = client.inferencesessions.token(session.id)
     interface = session.inferenceService.interface
     inference_client = client.inferencesessions.client(
         session.id, session_token, interface=interface
     )
-    evaluation_id = ids.generate_entity_id()
+    evaluation_id = id or ids.generate_entity_id()
     replication_ids = [
         ids.replication_id(evaluation_id, i) for i in range(replications)
     ]
     feature_schema = arrow.decode_schema(interface.outputSchema.arrowSchema)
     partition_schema = arrow.subset_schema(feature_schema, ["_replication_"])
 
     def output_generator() -> Iterable[pyarrow.RecordBatch]:
```

### Comparing `dyff-audit-0.3.0/dyff_audit.egg-info/PKG-INFO` & `dyff_audit-0.3.1/dyff_audit.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dyff-audit
-Version: 0.3.0
+Version: 0.3.1
 Summary: Audit tools for the Dyff AI auditing platform.
 Author-email: Digital Safety Research Institute <contact@dsri.org>
 License: Apache-2.0
 Project-URL: Home, https://gitlab.com/dyff/packages/dyff-audit
 Project-URL: Issues, https://gitlab.com/dyff/packages/dyff-audit/-/issues
 Keywords: ai,audit,safety,evaluation
 Classifier: Development Status :: 3 - Alpha
@@ -19,17 +19,25 @@
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: NOTICE
 Requires-Dist: dyff-client
 Requires-Dist: dyff-schema
+Requires-Dist: nbconvert
+Requires-Dist: nbformat
+Requires-Dist: notebook
 Requires-Dist: pandas
 Requires-Dist: pyarrow
 Requires-Dist: pydantic<2
+Requires-Dist: ruamel.yaml
+Provides-Extra: dev
+Requires-Dist: pytest; extra == "dev"
+Requires-Dist: pytest-datafiles; extra == "dev"
+Requires-Dist: pytest-depends; extra == "dev"
 
 # dyff-audit
 
 <!-- BADGIE TIME -->
 
 [![pipeline status](https://img.shields.io/gitlab/pipeline-status/dyff/packages/dyff-audit?branch=main)](https://gitlab.com/dyff/packages/dyff-audit/-/commits/main)
 [![coverage report](https://img.shields.io/gitlab/pipeline-coverage/dyff/packages/dyff-audit?branch=main)](https://gitlab.com/dyff/packages/dyff-audit/-/commits/main)
```

### Comparing `dyff-audit-0.3.0/makefile` & `dyff_audit-0.3.1/makefile`

 * *Files identical despite different names*

### Comparing `dyff-audit-0.3.0/pyproject.toml` & `dyff_audit-0.3.1/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -29,17 +29,21 @@
     "Programming Language :: Python :: 3.12",
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
 ]
 
 dependencies = [
     "dyff-client",
     "dyff-schema",
+    "nbconvert",
+    "nbformat",
+    "notebook",
     "pandas",
     "pyarrow",
     "pydantic<2",
+    "ruamel.yaml",
 ]
 
 dynamic = ["version"]
 
 keywords = [
     "ai",
     "audit",
@@ -49,14 +53,17 @@
 
 license = {text = "Apache-2.0"}
 
 readme = "README.md"
 
 requires-python = ">=3.9"
 
+[project.optional-dependencies]
+dev = ["pytest", "pytest-datafiles", "pytest-depends"]
+
 [project.urls]
 "Home" = "https://gitlab.com/dyff/packages/dyff-audit"
 "Issues" = "https://gitlab.com/dyff/packages/dyff-audit/-/issues"
 
 [tool.setuptools.packages.find]
 where = ["."]
 include = [
```

### Comparing `dyff-audit-0.3.0/tests/test_import.py` & `dyff_audit-0.3.1/tests/test_import.py`

 * *Files 25% similar despite different names*

```diff
@@ -6,16 +6,24 @@
 import pytest
 
 
 @pytest.mark.parametrize(
     "module_name",
     [
         "dyff.audit",
+        "dyff.audit.analysis",
+        "dyff.audit.analysis.context",
+        "dyff.audit.analysis.jupyter",
+        "dyff.audit.analysis.legacy",
+        "dyff.audit.analysis.python",
         "dyff.audit.data",
         "dyff.audit.data.text",
+        "dyff.audit.dynamic_import",
+        "dyff.audit.local",
+        "dyff.audit.local.platform",
         "dyff.audit.metrics.base",
         "dyff.audit.metrics.text",
         "dyff.audit.metrics",
         "dyff.audit.scoring.base",
         "dyff.audit.scoring.example",
         "dyff.audit.scoring.text",
         "dyff.audit.scoring",
```


# Comparing `tmp/dvclive-3.5.0.tar.gz` & `tmp/dvclive-3.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dvclive-3.5.0.tar", last modified: Thu Dec 21 18:46:46 2023, max compression
+gzip compressed data, was "dvclive-3.5.1.tar", last modified: Fri Dec 22 18:29:03 2023, max compression
```

## Comparing `dvclive-3.5.0.tar` & `dvclive-3.5.1.tar`

### file list

```diff
@@ -1,102 +1,102 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 18:46:46.225991 dvclive-3.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)      700 2023-12-21 18:46:35.000000 dvclive-3.5.0/.cruft.json
--rw-r--r--   0 runner    (1001) docker     (127)       19 2023-12-21 18:46:35.000000 dvclive-3.5.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 18:46:46.201991 dvclive-3.5.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      412 2023-12-21 18:46:35.000000 dvclive-3.5.0/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (127)      737 2023-12-21 18:46:35.000000 dvclive-3.5.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 18:46:46.201991 dvclive-3.5.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      791 2023-12-21 18:46:35.000000 dvclive-3.5.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2192 2023-12-21 18:46:35.000000 dvclive-3.5.0/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)      298 2023-12-21 18:46:35.000000 dvclive-3.5.0/.github/workflows/update-template.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2085 2023-12-21 18:46:35.000000 dvclive-3.5.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      995 2023-12-21 18:46:35.000000 dvclive-3.5.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5392 2023-12-21 18:46:35.000000 dvclive-3.5.0/CODE_OF_CONDUCT.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2733 2023-12-21 18:46:35.000000 dvclive-3.5.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)    11340 2023-12-21 18:46:35.000000 dvclive-3.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10715 2023-12-21 18:46:46.225991 dvclive-3.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7748 2023-12-21 18:46:35.000000 dvclive-3.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 18:46:46.205991 dvclive-3.5.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)   321138 2023-12-21 18:46:35.000000 dvclive-3.5.0/docs/dvc_plots_diff.png
--rw-r--r--   0 runner    (1001) docker     (127)   676021 2023-12-21 18:46:35.000000 dvclive-3.5.0/docs/studio_compare.png
--rw-r--r--   0 runner    (1001) docker     (127)   501824 2023-12-21 18:46:35.000000 dvclive-3.5.0/docs/vscode_experiments.png
--rw-r--r--   0 runner    (1001) docker     (127)   627561 2023-12-21 18:46:35.000000 dvclive-3.5.0/docs/vscode_plots.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 18:46:46.209991 dvclive-3.5.0/examples/
--rw-r--r--   0 runner    (1001) docker     (127)   306756 2023-12-21 18:46:35.000000 dvclive-3.5.0/examples/DVCLive-Evidently.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    11395 2023-12-21 18:46:35.000000 dvclive-3.5.0/examples/DVCLive-Fabric.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     8857 2023-12-21 18:46:35.000000 dvclive-3.5.0/examples/DVCLive-HuggingFace.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     7460 2023-12-21 18:46:35.000000 dvclive-3.5.0/examples/DVCLive-PyTorch-Lightning.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    10015 2023-12-21 18:46:35.000000 dvclive-3.5.0/examples/DVCLive-Quickstart.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     3169 2023-12-21 18:46:35.000000 dvclive-3.5.0/examples/DVCLive-YOLO.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     4243 2023-12-21 18:46:35.000000 dvclive-3.5.0/examples/DVCLive-scikit-learn.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1749 2023-12-21 18:46:35.000000 dvclive-3.5.0/noxfile.py
--rw-r--r--   0 runner    (1001) docker     (127)     3745 2023-12-21 18:46:35.000000 dvclive-3.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-21 18:46:46.225991 dvclive-3.5.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 18:46:46.201991 dvclive-3.5.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 18:46:46.213991 dvclive-3.5.0/src/dvclive/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2023-12-21 18:46:35.000000 dvclive-3.5.0/src/dvclive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2023-12-21 18:46:46.000000 dvclive-3.5.0/src/dvclive/_dvclive_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      758 2023-12-21 18:46:35.000000 dvclive-3.5.0/src/dvclive/catalyst.py
--rw-r--r--   0 runner    (1001) docker     (127)     5589 2023-12-21 18:46:35.000000 dvclive-3.5.0/src/dvclive/dvc.py
--rw-r--r--   0 runner    (1001) docker     (127)      230 2023-12-21 18:46:35.000000 dvclive-3.5.0/src/dvclive/env.py
--rw-r--r--   0 runner    (1001) docker     (127)     1032 2023-12-21 18:46:35.000000 dvclive-3.5.0/src/dvclive/error.py
--rw-r--r--   0 runner    (1001) docker     (127)     4456 2023-12-21 18:46:35.000000 dvclive-3.5.0/src/dvclive/fabric.py
--rw-r--r--   0 runner    (1001) docker     (127)     2586 2023-12-21 18:46:35.000000 dvclive-3.5.0/src/dvclive/fastai.py
--rw-r--r--   0 runner    (1001) docker     (127)     2143 2023-12-21 18:46:35.000000 dvclive-3.5.0/src/dvclive/huggingface.py
--rw-r--r--   0 runner    (1001) docker     (127)      822 2023-12-21 18:46:35.000000 dvclive-3.5.0/src/dvclive/keras.py
--rw-r--r--   0 runner    (1001) docker     (127)      593 2023-12-21 18:46:35.000000 dvclive-3.5.0/src/dvclive/lgbm.py
--rw-r--r--   0 runner    (1001) docker     (127)     4603 2023-12-21 18:46:35.000000 dvclive-3.5.0/src/dvclive/lightning.py
--rw-r--r--   0 runner    (1001) docker     (127)    21273 2023-12-21 18:46:35.000000 dvclive-3.5.0/src/dvclive/live.py
--rw-r--r--   0 runner    (1001) docker     (127)     1449 2023-12-21 18:46:35.000000 dvclive-3.5.0/src/dvclive/optuna.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 18:46:46.213991 dvclive-3.5.0/src/dvclive/plots/
--rw-r--r--   0 runner    (1001) docker     (127)      439 2023-12-21 18:46:35.000000 dvclive-3.5.0/src/dvclive/plots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      722 2023-12-21 18:46:35.000000 dvclive-3.5.0/src/dvclive/plots/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1387 2023-12-21 18:46:35.000000 dvclive-3.5.0/src/dvclive/plots/custom.py
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2023-12-21 18:46:35.000000 dvclive-3.5.0/src/dvclive/plots/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     1417 2023-12-21 18:46:35.000000 dvclive-3.5.0/src/dvclive/plots/metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     5289 2023-12-21 18:46:35.000000 dvclive-3.5.0/src/dvclive/plots/sklearn.py
--rw-r--r--   0 runner    (1001) docker     (127)      585 2023-12-21 18:46:35.000000 dvclive-3.5.0/src/dvclive/plots/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5102 2023-12-21 18:46:35.000000 dvclive-3.5.0/src/dvclive/report.py
--rw-r--r--   0 runner    (1001) docker     (127)     1443 2023-12-21 18:46:35.000000 dvclive-3.5.0/src/dvclive/serialize.py
--rw-r--r--   0 runner    (1001) docker     (127)     3629 2023-12-21 18:46:35.000000 dvclive-3.5.0/src/dvclive/studio.py
--rw-r--r--   0 runner    (1001) docker     (127)     6566 2023-12-21 18:46:35.000000 dvclive-3.5.0/src/dvclive/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2722 2023-12-21 18:46:35.000000 dvclive-3.5.0/src/dvclive/vscode.py
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2023-12-21 18:46:35.000000 dvclive-3.5.0/src/dvclive/xgb.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 18:46:46.221991 dvclive-3.5.0/src/dvclive.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10715 2023-12-21 18:46:46.000000 dvclive-3.5.0/src/dvclive.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2246 2023-12-21 18:46:46.000000 dvclive-3.5.0/src/dvclive.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-21 18:46:46.000000 dvclive-3.5.0/src/dvclive.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      675 2023-12-21 18:46:46.000000 dvclive-3.5.0/src/dvclive.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2023-12-21 18:46:46.000000 dvclive-3.5.0/src/dvclive.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 18:46:46.217991 dvclive-3.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-21 18:46:35.000000 dvclive-3.5.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1764 2023-12-21 18:46:35.000000 dvclive-3.5.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 18:46:46.217991 dvclive-3.5.0/tests/frameworks/
--rw-r--r--   0 runner    (1001) docker     (127)     2583 2023-12-21 18:46:35.000000 dvclive-3.5.0/tests/frameworks/test_catalyst.py
--rw-r--r--   0 runner    (1001) docker     (127)     1947 2023-12-21 18:46:35.000000 dvclive-3.5.0/tests/frameworks/test_fabric.py
--rw-r--r--   0 runner    (1001) docker     (127)     3670 2023-12-21 18:46:35.000000 dvclive-3.5.0/tests/frameworks/test_fastai.py
--rw-r--r--   0 runner    (1001) docker     (127)     5136 2023-12-21 18:46:35.000000 dvclive-3.5.0/tests/frameworks/test_huggingface.py
--rw-r--r--   0 runner    (1001) docker     (127)     1667 2023-12-21 18:46:35.000000 dvclive-3.5.0/tests/frameworks/test_keras.py
--rw-r--r--   0 runner    (1001) docker     (127)     2479 2023-12-21 18:46:35.000000 dvclive-3.5.0/tests/frameworks/test_lgbm.py
--rw-r--r--   0 runner    (1001) docker     (127)    10583 2023-12-21 18:46:35.000000 dvclive-3.5.0/tests/frameworks/test_lightning.py
--rw-r--r--   0 runner    (1001) docker     (127)      898 2023-12-21 18:46:35.000000 dvclive-3.5.0/tests/frameworks/test_optuna.py
--rw-r--r--   0 runner    (1001) docker     (127)     2323 2023-12-21 18:46:35.000000 dvclive-3.5.0/tests/frameworks/test_xgboost.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 18:46:46.221991 dvclive-3.5.0/tests/plots/
--rw-r--r--   0 runner    (1001) docker     (127)      762 2023-12-21 18:46:35.000000 dvclive-3.5.0/tests/plots/test_custom.py
--rw-r--r--   0 runner    (1001) docker     (127)     3428 2023-12-21 18:46:35.000000 dvclive-3.5.0/tests/plots/test_image.py
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2023-12-21 18:46:35.000000 dvclive-3.5.0/tests/plots/test_metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     5297 2023-12-21 18:46:35.000000 dvclive-3.5.0/tests/plots/test_sklearn.py
--rw-r--r--   0 runner    (1001) docker     (127)     1215 2023-12-21 18:46:35.000000 dvclive-3.5.0/tests/test_cleanup.py
--rw-r--r--   0 runner    (1001) docker     (127)      716 2023-12-21 18:46:35.000000 dvclive-3.5.0/tests/test_context_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     7966 2023-12-21 18:46:35.000000 dvclive-3.5.0/tests/test_dvc.py
--rw-r--r--   0 runner    (1001) docker     (127)     9812 2023-12-21 18:46:35.000000 dvclive-3.5.0/tests/test_log_artifact.py
--rw-r--r--   0 runner    (1001) docker     (127)     2956 2023-12-21 18:46:35.000000 dvclive-3.5.0/tests/test_log_metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     2120 2023-12-21 18:46:35.000000 dvclive-3.5.0/tests/test_log_param.py
--rw-r--r--   0 runner    (1001) docker     (127)      551 2023-12-21 18:46:35.000000 dvclive-3.5.0/tests/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)    13992 2023-12-21 18:46:35.000000 dvclive-3.5.0/tests/test_make_dvcyaml.py
--rw-r--r--   0 runner    (1001) docker     (127)     6998 2023-12-21 18:46:35.000000 dvclive-3.5.0/tests/test_make_report.py
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2023-12-21 18:46:35.000000 dvclive-3.5.0/tests/test_make_summary.py
--rw-r--r--   0 runner    (1001) docker     (127)    11266 2023-12-21 18:46:35.000000 dvclive-3.5.0/tests/test_post_to_studio.py
--rw-r--r--   0 runner    (1001) docker     (127)     1331 2023-12-21 18:46:35.000000 dvclive-3.5.0/tests/test_resume.py
--rw-r--r--   0 runner    (1001) docker     (127)     2151 2023-12-21 18:46:35.000000 dvclive-3.5.0/tests/test_step.py
--rw-r--r--   0 runner    (1001) docker     (127)     1649 2023-12-21 18:46:35.000000 dvclive-3.5.0/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2688 2023-12-21 18:46:35.000000 dvclive-3.5.0/tests/test_vscode.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 18:29:03.170470 dvclive-3.5.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2023-12-22 18:28:50.000000 dvclive-3.5.1/.cruft.json
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2023-12-22 18:28:50.000000 dvclive-3.5.1/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 18:29:03.150469 dvclive-3.5.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2023-12-22 18:28:50.000000 dvclive-3.5.1/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2023-12-22 18:28:50.000000 dvclive-3.5.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 18:29:03.150469 dvclive-3.5.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2023-12-22 18:28:50.000000 dvclive-3.5.1/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2192 2023-12-22 18:28:50.000000 dvclive-3.5.1/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2023-12-22 18:28:50.000000 dvclive-3.5.1/.github/workflows/update-template.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2085 2023-12-22 18:28:50.000000 dvclive-3.5.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2023-12-22 18:28:50.000000 dvclive-3.5.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5392 2023-12-22 18:28:50.000000 dvclive-3.5.1/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2733 2023-12-22 18:28:50.000000 dvclive-3.5.1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11340 2023-12-22 18:28:50.000000 dvclive-3.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10785 2023-12-22 18:29:03.170470 dvclive-3.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7748 2023-12-22 18:28:50.000000 dvclive-3.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 18:29:03.154469 dvclive-3.5.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)   321138 2023-12-22 18:28:50.000000 dvclive-3.5.1/docs/dvc_plots_diff.png
+-rw-r--r--   0 runner    (1001) docker     (127)   676021 2023-12-22 18:28:50.000000 dvclive-3.5.1/docs/studio_compare.png
+-rw-r--r--   0 runner    (1001) docker     (127)   501824 2023-12-22 18:28:50.000000 dvclive-3.5.1/docs/vscode_experiments.png
+-rw-r--r--   0 runner    (1001) docker     (127)   627561 2023-12-22 18:28:50.000000 dvclive-3.5.1/docs/vscode_plots.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 18:29:03.158470 dvclive-3.5.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)   306756 2023-12-22 18:28:50.000000 dvclive-3.5.1/examples/DVCLive-Evidently.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    11395 2023-12-22 18:28:50.000000 dvclive-3.5.1/examples/DVCLive-Fabric.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     8857 2023-12-22 18:28:50.000000 dvclive-3.5.1/examples/DVCLive-HuggingFace.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     7460 2023-12-22 18:28:50.000000 dvclive-3.5.1/examples/DVCLive-PyTorch-Lightning.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    10015 2023-12-22 18:28:50.000000 dvclive-3.5.1/examples/DVCLive-Quickstart.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     3169 2023-12-22 18:28:50.000000 dvclive-3.5.1/examples/DVCLive-YOLO.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     4243 2023-12-22 18:28:50.000000 dvclive-3.5.1/examples/DVCLive-scikit-learn.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1749 2023-12-22 18:28:50.000000 dvclive-3.5.1/noxfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3781 2023-12-22 18:28:50.000000 dvclive-3.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-22 18:29:03.170470 dvclive-3.5.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 18:29:03.150469 dvclive-3.5.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 18:29:03.158470 dvclive-3.5.1/src/dvclive/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2023-12-22 18:28:50.000000 dvclive-3.5.1/src/dvclive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2023-12-22 18:29:03.000000 dvclive-3.5.1/src/dvclive/_dvclive_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2023-12-22 18:28:50.000000 dvclive-3.5.1/src/dvclive/catalyst.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5589 2023-12-22 18:28:50.000000 dvclive-3.5.1/src/dvclive/dvc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2023-12-22 18:28:50.000000 dvclive-3.5.1/src/dvclive/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2023-12-22 18:28:50.000000 dvclive-3.5.1/src/dvclive/error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4456 2023-12-22 18:28:50.000000 dvclive-3.5.1/src/dvclive/fabric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2586 2023-12-22 18:28:50.000000 dvclive-3.5.1/src/dvclive/fastai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2143 2023-12-22 18:28:50.000000 dvclive-3.5.1/src/dvclive/huggingface.py
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2023-12-22 18:28:50.000000 dvclive-3.5.1/src/dvclive/keras.py
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2023-12-22 18:28:50.000000 dvclive-3.5.1/src/dvclive/lgbm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4603 2023-12-22 18:28:50.000000 dvclive-3.5.1/src/dvclive/lightning.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21273 2023-12-22 18:28:50.000000 dvclive-3.5.1/src/dvclive/live.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1449 2023-12-22 18:28:50.000000 dvclive-3.5.1/src/dvclive/optuna.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 18:29:03.162469 dvclive-3.5.1/src/dvclive/plots/
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2023-12-22 18:28:50.000000 dvclive-3.5.1/src/dvclive/plots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      722 2023-12-22 18:28:50.000000 dvclive-3.5.1/src/dvclive/plots/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1387 2023-12-22 18:28:50.000000 dvclive-3.5.1/src/dvclive/plots/custom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2023-12-22 18:28:50.000000 dvclive-3.5.1/src/dvclive/plots/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1417 2023-12-22 18:28:50.000000 dvclive-3.5.1/src/dvclive/plots/metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5289 2023-12-22 18:28:50.000000 dvclive-3.5.1/src/dvclive/plots/sklearn.py
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2023-12-22 18:28:50.000000 dvclive-3.5.1/src/dvclive/plots/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5102 2023-12-22 18:28:50.000000 dvclive-3.5.1/src/dvclive/report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1443 2023-12-22 18:28:50.000000 dvclive-3.5.1/src/dvclive/serialize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3629 2023-12-22 18:28:50.000000 dvclive-3.5.1/src/dvclive/studio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6566 2023-12-22 18:28:50.000000 dvclive-3.5.1/src/dvclive/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2722 2023-12-22 18:28:50.000000 dvclive-3.5.1/src/dvclive/vscode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2023-12-22 18:28:50.000000 dvclive-3.5.1/src/dvclive/xgb.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 18:29:03.166469 dvclive-3.5.1/src/dvclive.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10785 2023-12-22 18:29:03.000000 dvclive-3.5.1/src/dvclive.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2246 2023-12-22 18:29:03.000000 dvclive-3.5.1/src/dvclive.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-22 18:29:03.000000 dvclive-3.5.1/src/dvclive.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2023-12-22 18:29:03.000000 dvclive-3.5.1/src/dvclive.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2023-12-22 18:29:03.000000 dvclive-3.5.1/src/dvclive.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 18:29:03.166469 dvclive-3.5.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-22 18:28:50.000000 dvclive-3.5.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1764 2023-12-22 18:28:50.000000 dvclive-3.5.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 18:29:03.166469 dvclive-3.5.1/tests/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (127)     2583 2023-12-22 18:28:50.000000 dvclive-3.5.1/tests/frameworks/test_catalyst.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1947 2023-12-22 18:28:50.000000 dvclive-3.5.1/tests/frameworks/test_fabric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3670 2023-12-22 18:28:50.000000 dvclive-3.5.1/tests/frameworks/test_fastai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5136 2023-12-22 18:28:50.000000 dvclive-3.5.1/tests/frameworks/test_huggingface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1667 2023-12-22 18:28:50.000000 dvclive-3.5.1/tests/frameworks/test_keras.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2479 2023-12-22 18:28:50.000000 dvclive-3.5.1/tests/frameworks/test_lgbm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10583 2023-12-22 18:28:50.000000 dvclive-3.5.1/tests/frameworks/test_lightning.py
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2023-12-22 18:28:50.000000 dvclive-3.5.1/tests/frameworks/test_optuna.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2323 2023-12-22 18:28:50.000000 dvclive-3.5.1/tests/frameworks/test_xgboost.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 18:29:03.166469 dvclive-3.5.1/tests/plots/
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2023-12-22 18:28:50.000000 dvclive-3.5.1/tests/plots/test_custom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3428 2023-12-22 18:28:50.000000 dvclive-3.5.1/tests/plots/test_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2023-12-22 18:28:50.000000 dvclive-3.5.1/tests/plots/test_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5297 2023-12-22 18:28:50.000000 dvclive-3.5.1/tests/plots/test_sklearn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1215 2023-12-22 18:28:50.000000 dvclive-3.5.1/tests/test_cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2023-12-22 18:28:50.000000 dvclive-3.5.1/tests/test_context_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7966 2023-12-22 18:28:50.000000 dvclive-3.5.1/tests/test_dvc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9812 2023-12-22 18:28:50.000000 dvclive-3.5.1/tests/test_log_artifact.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2956 2023-12-22 18:28:50.000000 dvclive-3.5.1/tests/test_log_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2120 2023-12-22 18:28:50.000000 dvclive-3.5.1/tests/test_log_param.py
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2023-12-22 18:28:50.000000 dvclive-3.5.1/tests/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13992 2023-12-22 18:28:50.000000 dvclive-3.5.1/tests/test_make_dvcyaml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6998 2023-12-22 18:28:50.000000 dvclive-3.5.1/tests/test_make_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2023-12-22 18:28:50.000000 dvclive-3.5.1/tests/test_make_summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11266 2023-12-22 18:28:50.000000 dvclive-3.5.1/tests/test_post_to_studio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1331 2023-12-22 18:28:50.000000 dvclive-3.5.1/tests/test_resume.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2637 2023-12-22 18:28:50.000000 dvclive-3.5.1/tests/test_step.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1649 2023-12-22 18:28:50.000000 dvclive-3.5.1/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2688 2023-12-22 18:28:50.000000 dvclive-3.5.1/tests/test_vscode.py
```

### Comparing `dvclive-3.5.0/.cruft.json` & `dvclive-3.5.1/.cruft.json`

 * *Files identical despite different names*

### Comparing `dvclive-3.5.0/.github/dependabot.yml` & `dvclive-3.5.1/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `dvclive-3.5.0/.github/workflows/release.yml` & `dvclive-3.5.1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `dvclive-3.5.0/.github/workflows/tests.yml` & `dvclive-3.5.1/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `dvclive-3.5.0/.gitignore` & `dvclive-3.5.1/.gitignore`

 * *Files identical despite different names*

### Comparing `dvclive-3.5.0/.pre-commit-config.yaml` & `dvclive-3.5.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dvclive-3.5.0/CODE_OF_CONDUCT.rst` & `dvclive-3.5.1/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `dvclive-3.5.0/CONTRIBUTING.rst` & `dvclive-3.5.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `dvclive-3.5.0/LICENSE` & `dvclive-3.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dvclive-3.5.0/PKG-INFO` & `dvclive-3.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dvclive
-Version: 3.5.0
+Version: 3.5.1
 Summary: Experiments logger for ML projects.
 Author-email: Iterative <support@dvc.org>
 Maintainer-email: Iterative <support@dvc.org>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/iterative/dvclive
 Project-URL: Documentation, https://dvc.org/doc/dvclive
 Project-URL: Repository, https://github.com/iterative/dvclive
@@ -64,14 +64,15 @@
 Provides-Extra: catalyst
 Requires-Dist: catalyst>22; extra == "catalyst"
 Provides-Extra: fastai
 Requires-Dist: fastai; extra == "fastai"
 Provides-Extra: lightning
 Requires-Dist: lightning>=2.0; extra == "lightning"
 Requires-Dist: torch; extra == "lightning"
+Requires-Dist: jsonargparse[signatures]>=4.26.1; extra == "lightning"
 Provides-Extra: optuna
 Requires-Dist: optuna; extra == "optuna"
 Provides-Extra: all
 Requires-Dist: dvclive[catalyst,fastai,huggingface,image,lgbm,lightning,markdown,mmcv,optuna,plots,tf,xgb]; extra == "all"
 
 # DVCLive
```

### Comparing `dvclive-3.5.0/README.md` & `dvclive-3.5.1/README.md`

 * *Files identical despite different names*

### Comparing `dvclive-3.5.0/docs/dvc_plots_diff.png` & `dvclive-3.5.1/docs/dvc_plots_diff.png`

 * *Files identical despite different names*

### Comparing `dvclive-3.5.0/docs/studio_compare.png` & `dvclive-3.5.1/docs/studio_compare.png`

 * *Files identical despite different names*

### Comparing `dvclive-3.5.0/docs/vscode_experiments.png` & `dvclive-3.5.1/docs/vscode_experiments.png`

 * *Files identical despite different names*

### Comparing `dvclive-3.5.0/docs/vscode_plots.png` & `dvclive-3.5.1/docs/vscode_plots.png`

 * *Files identical despite different names*

### Comparing `dvclive-3.5.0/examples/DVCLive-Evidently.ipynb` & `dvclive-3.5.1/examples/DVCLive-Evidently.ipynb`

 * *Files identical despite different names*

### Comparing `dvclive-3.5.0/examples/DVCLive-Fabric.ipynb` & `dvclive-3.5.1/examples/DVCLive-Fabric.ipynb`

 * *Files identical despite different names*

### Comparing `dvclive-3.5.0/examples/DVCLive-HuggingFace.ipynb` & `dvclive-3.5.1/examples/DVCLive-HuggingFace.ipynb`

 * *Files identical despite different names*

### Comparing `dvclive-3.5.0/examples/DVCLive-PyTorch-Lightning.ipynb` & `dvclive-3.5.1/examples/DVCLive-PyTorch-Lightning.ipynb`

 * *Files identical despite different names*

### Comparing `dvclive-3.5.0/examples/DVCLive-Quickstart.ipynb` & `dvclive-3.5.1/examples/DVCLive-Quickstart.ipynb`

 * *Files identical despite different names*

### Comparing `dvclive-3.5.0/examples/DVCLive-YOLO.ipynb` & `dvclive-3.5.1/examples/DVCLive-YOLO.ipynb`

 * *Files identical despite different names*

### Comparing `dvclive-3.5.0/examples/DVCLive-scikit-learn.ipynb` & `dvclive-3.5.1/examples/DVCLive-scikit-learn.ipynb`

 * *Files identical despite different names*

### Comparing `dvclive-3.5.0/noxfile.py` & `dvclive-3.5.1/noxfile.py`

 * *Files identical despite different names*

### Comparing `dvclive-3.5.0/pyproject.toml` & `dvclive-3.5.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
 mmcv = ["mmcv"]
 tf = ["tensorflow"]
 xgb = ["xgboost"]
 lgbm = ["lightgbm"]
 huggingface = ["transformers", "datasets"]
 catalyst = ["catalyst>22"]
 fastai = ["fastai"]
-lightning = ["lightning>=2.0", "torch"]
+lightning = ["lightning>=2.0", "torch", "jsonargparse[signatures]>=4.26.1"]
 optuna = ["optuna"]
 all = [
    "dvclive[image,mmcv,tf,xgb,lgbm,huggingface,catalyst,fastai,lightning,optuna,plots,markdown]"
 ]
 
 [project.urls]
 Homepage = "https://github.com/iterative/dvclive"
```

### Comparing `dvclive-3.5.0/src/dvclive/catalyst.py` & `dvclive-3.5.1/src/dvclive/catalyst.py`

 * *Files identical despite different names*

### Comparing `dvclive-3.5.0/src/dvclive/dvc.py` & `dvclive-3.5.1/src/dvclive/dvc.py`

 * *Files identical despite different names*

### Comparing `dvclive-3.5.0/src/dvclive/error.py` & `dvclive-3.5.1/src/dvclive/error.py`

 * *Files identical despite different names*

### Comparing `dvclive-3.5.0/src/dvclive/fabric.py` & `dvclive-3.5.1/src/dvclive/fabric.py`

 * *Files identical despite different names*

### Comparing `dvclive-3.5.0/src/dvclive/fastai.py` & `dvclive-3.5.1/src/dvclive/fastai.py`

 * *Files identical despite different names*

### Comparing `dvclive-3.5.0/src/dvclive/huggingface.py` & `dvclive-3.5.1/src/dvclive/huggingface.py`

 * *Files identical despite different names*

### Comparing `dvclive-3.5.0/src/dvclive/keras.py` & `dvclive-3.5.1/src/dvclive/keras.py`

 * *Files identical despite different names*

### Comparing `dvclive-3.5.0/src/dvclive/lgbm.py` & `dvclive-3.5.1/src/dvclive/lgbm.py`

 * *Files identical despite different names*

### Comparing `dvclive-3.5.0/src/dvclive/lightning.py` & `dvclive-3.5.1/src/dvclive/lightning.py`

 * *Files identical despite different names*

### Comparing `dvclive-3.5.0/src/dvclive/live.py` & `dvclive-3.5.1/src/dvclive/live.py`

 * *Files 0% similar despite different names*

```diff
@@ -582,15 +582,15 @@
             return
 
         if self._images and self._cache_images:
             images_path = Path(self.plots_dir) / Image.subfolder
             self.cache(images_path)
 
         # If next_step called before end, don't want to update step number
-        if self._step is not None:
+        if "step" in self.summary:
             self.step = self.summary["step"]
         self.sync()
 
         if self._inside_dvc_exp and self._dvc_repo:
             catch_and_warn(DvcException, logger)(ensure_dir_is_tracked)(
                 self.dir, self._dvc_repo
             )
```

### Comparing `dvclive-3.5.0/src/dvclive/optuna.py` & `dvclive-3.5.1/src/dvclive/optuna.py`

 * *Files identical despite different names*

### Comparing `dvclive-3.5.0/src/dvclive/plots/base.py` & `dvclive-3.5.1/src/dvclive/plots/base.py`

 * *Files identical despite different names*

### Comparing `dvclive-3.5.0/src/dvclive/plots/custom.py` & `dvclive-3.5.1/src/dvclive/plots/custom.py`

 * *Files identical despite different names*

### Comparing `dvclive-3.5.0/src/dvclive/plots/image.py` & `dvclive-3.5.1/src/dvclive/plots/image.py`

 * *Files identical despite different names*

### Comparing `dvclive-3.5.0/src/dvclive/plots/metric.py` & `dvclive-3.5.1/src/dvclive/plots/metric.py`

 * *Files identical despite different names*

### Comparing `dvclive-3.5.0/src/dvclive/plots/sklearn.py` & `dvclive-3.5.1/src/dvclive/plots/sklearn.py`

 * *Files identical despite different names*

### Comparing `dvclive-3.5.0/src/dvclive/plots/utils.py` & `dvclive-3.5.1/src/dvclive/plots/utils.py`

 * *Files identical despite different names*

### Comparing `dvclive-3.5.0/src/dvclive/report.py` & `dvclive-3.5.1/src/dvclive/report.py`

 * *Files identical despite different names*

### Comparing `dvclive-3.5.0/src/dvclive/serialize.py` & `dvclive-3.5.1/src/dvclive/serialize.py`

 * *Files identical despite different names*

### Comparing `dvclive-3.5.0/src/dvclive/studio.py` & `dvclive-3.5.1/src/dvclive/studio.py`

 * *Files identical despite different names*

### Comparing `dvclive-3.5.0/src/dvclive/utils.py` & `dvclive-3.5.1/src/dvclive/utils.py`

 * *Files identical despite different names*

### Comparing `dvclive-3.5.0/src/dvclive/vscode.py` & `dvclive-3.5.1/src/dvclive/vscode.py`

 * *Files identical despite different names*

### Comparing `dvclive-3.5.0/src/dvclive/xgb.py` & `dvclive-3.5.1/src/dvclive/xgb.py`

 * *Files identical despite different names*

### Comparing `dvclive-3.5.0/src/dvclive.egg-info/PKG-INFO` & `dvclive-3.5.1/src/dvclive.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dvclive
-Version: 3.5.0
+Version: 3.5.1
 Summary: Experiments logger for ML projects.
 Author-email: Iterative <support@dvc.org>
 Maintainer-email: Iterative <support@dvc.org>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/iterative/dvclive
 Project-URL: Documentation, https://dvc.org/doc/dvclive
 Project-URL: Repository, https://github.com/iterative/dvclive
@@ -64,14 +64,15 @@
 Provides-Extra: catalyst
 Requires-Dist: catalyst>22; extra == "catalyst"
 Provides-Extra: fastai
 Requires-Dist: fastai; extra == "fastai"
 Provides-Extra: lightning
 Requires-Dist: lightning>=2.0; extra == "lightning"
 Requires-Dist: torch; extra == "lightning"
+Requires-Dist: jsonargparse[signatures]>=4.26.1; extra == "lightning"
 Provides-Extra: optuna
 Requires-Dist: optuna; extra == "optuna"
 Provides-Extra: all
 Requires-Dist: dvclive[catalyst,fastai,huggingface,image,lgbm,lightning,markdown,mmcv,optuna,plots,tf,xgb]; extra == "all"
 
 # DVCLive
```

### Comparing `dvclive-3.5.0/src/dvclive.egg-info/SOURCES.txt` & `dvclive-3.5.1/src/dvclive.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dvclive-3.5.0/src/dvclive.egg-info/requires.txt` & `dvclive-3.5.1/src/dvclive.egg-info/requires.txt`

 * *Files 13% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 
 [lgbm]
 lightgbm
 
 [lightning]
 lightning>=2.0
 torch
+jsonargparse[signatures]>=4.26.1
 
 [markdown]
 matplotlib
 
 [mmcv]
 mmcv
```

### Comparing `dvclive-3.5.0/tests/conftest.py` & `dvclive-3.5.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dvclive-3.5.0/tests/frameworks/test_catalyst.py` & `dvclive-3.5.1/tests/frameworks/test_catalyst.py`

 * *Files identical despite different names*

### Comparing `dvclive-3.5.0/tests/frameworks/test_fabric.py` & `dvclive-3.5.1/tests/frameworks/test_fabric.py`

 * *Files identical despite different names*

### Comparing `dvclive-3.5.0/tests/frameworks/test_fastai.py` & `dvclive-3.5.1/tests/frameworks/test_fastai.py`

 * *Files identical despite different names*

### Comparing `dvclive-3.5.0/tests/frameworks/test_huggingface.py` & `dvclive-3.5.1/tests/frameworks/test_huggingface.py`

 * *Files identical despite different names*

### Comparing `dvclive-3.5.0/tests/frameworks/test_keras.py` & `dvclive-3.5.1/tests/frameworks/test_keras.py`

 * *Files identical despite different names*

### Comparing `dvclive-3.5.0/tests/frameworks/test_lgbm.py` & `dvclive-3.5.1/tests/frameworks/test_lgbm.py`

 * *Files identical despite different names*

### Comparing `dvclive-3.5.0/tests/frameworks/test_lightning.py` & `dvclive-3.5.1/tests/frameworks/test_lightning.py`

 * *Files identical despite different names*

### Comparing `dvclive-3.5.0/tests/frameworks/test_optuna.py` & `dvclive-3.5.1/tests/frameworks/test_optuna.py`

 * *Files identical despite different names*

### Comparing `dvclive-3.5.0/tests/frameworks/test_xgboost.py` & `dvclive-3.5.1/tests/frameworks/test_xgboost.py`

 * *Files identical despite different names*

### Comparing `dvclive-3.5.0/tests/plots/test_custom.py` & `dvclive-3.5.1/tests/plots/test_custom.py`

 * *Files identical despite different names*

### Comparing `dvclive-3.5.0/tests/plots/test_image.py` & `dvclive-3.5.1/tests/plots/test_image.py`

 * *Files identical despite different names*

### Comparing `dvclive-3.5.0/tests/plots/test_metric.py` & `dvclive-3.5.1/tests/plots/test_metric.py`

 * *Files identical despite different names*

### Comparing `dvclive-3.5.0/tests/plots/test_sklearn.py` & `dvclive-3.5.1/tests/plots/test_sklearn.py`

 * *Files identical despite different names*

### Comparing `dvclive-3.5.0/tests/test_cleanup.py` & `dvclive-3.5.1/tests/test_cleanup.py`

 * *Files identical despite different names*

### Comparing `dvclive-3.5.0/tests/test_context_manager.py` & `dvclive-3.5.1/tests/test_context_manager.py`

 * *Files identical despite different names*

### Comparing `dvclive-3.5.0/tests/test_dvc.py` & `dvclive-3.5.1/tests/test_dvc.py`

 * *Files identical despite different names*

### Comparing `dvclive-3.5.0/tests/test_log_artifact.py` & `dvclive-3.5.1/tests/test_log_artifact.py`

 * *Files identical despite different names*

### Comparing `dvclive-3.5.0/tests/test_log_metric.py` & `dvclive-3.5.1/tests/test_log_metric.py`

 * *Files identical despite different names*

### Comparing `dvclive-3.5.0/tests/test_log_param.py` & `dvclive-3.5.1/tests/test_log_param.py`

 * *Files identical despite different names*

### Comparing `dvclive-3.5.0/tests/test_logging.py` & `dvclive-3.5.1/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `dvclive-3.5.0/tests/test_make_dvcyaml.py` & `dvclive-3.5.1/tests/test_make_dvcyaml.py`

 * *Files identical despite different names*

### Comparing `dvclive-3.5.0/tests/test_make_report.py` & `dvclive-3.5.1/tests/test_make_report.py`

 * *Files identical despite different names*

### Comparing `dvclive-3.5.0/tests/test_make_summary.py` & `dvclive-3.5.1/tests/test_make_summary.py`

 * *Files identical despite different names*

### Comparing `dvclive-3.5.0/tests/test_post_to_studio.py` & `dvclive-3.5.1/tests/test_post_to_studio.py`

 * *Files identical despite different names*

### Comparing `dvclive-3.5.0/tests/test_resume.py` & `dvclive-3.5.1/tests/test_resume.py`

 * *Files identical despite different names*

### Comparing `dvclive-3.5.0/tests/test_step.py` & `dvclive-3.5.1/tests/test_step.py`

 * *Files 5% similar despite different names*

```diff
@@ -82,7 +82,27 @@
     while dvclive.step < 10:
         dvclive.log_metric("i", dvclive.step)
         dvclive.next_step()
 
     steps, values = read_history(dvclive, "i")
     assert steps == list(range(10))
     assert values == [float(x) for x in range(10)]
+
+
+def test_set_step_only(tmp_dir):
+    dvclive = Live()
+    dvclive.step = 1
+    dvclive.end()
+
+    assert dvclive.read_latest() == {"step": 1}
+    assert not os.path.exists(os.path.join(tmp_dir, "dvclive", "plots"))
+
+
+def test_step_on_end(tmp_dir):
+    dvclive = Live()
+    for metric in range(3):
+        dvclive.log_metric("m", metric)
+        dvclive.next_step()
+    dvclive.end()
+    assert dvclive.step == metric
+
+    assert dvclive.read_latest() == {"step": metric, "m": metric}
```

### Comparing `dvclive-3.5.0/tests/test_utils.py` & `dvclive-3.5.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `dvclive-3.5.0/tests/test_vscode.py` & `dvclive-3.5.1/tests/test_vscode.py`

 * *Files identical despite different names*


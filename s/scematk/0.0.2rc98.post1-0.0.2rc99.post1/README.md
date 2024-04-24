# Comparing `tmp/scematk-0.0.2rc98.post1.tar.gz` & `tmp/scematk-0.0.2rc99.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scematk-0.0.2rc98.post1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "scematk-0.0.2rc99.post1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `scematk-0.0.2rc98.post1.tar` & `scematk-0.0.2rc99.post1.tar`

### file list

```diff
@@ -1,75 +1,75 @@
--rw-r--r--   0        0        0      333 2024-03-25 20:12:08.611242 scematk-0.0.2rc98.post1/.devcontainer/Dockerfile
--rw-r--r--   0        0        0     1157 2024-03-25 20:12:08.611242 scematk-0.0.2rc98.post1/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0      417 2024-03-25 20:12:08.611242 scematk-0.0.2rc98.post1/.github/dependabot.yml
--rw-r--r--   0        0        0      418 2024-03-25 20:12:08.611242 scematk-0.0.2rc98.post1/.github/template-sync.yml
--rw-r--r--   0        0        0      476 2024-03-25 20:12:08.611242 scematk-0.0.2rc98.post1/.github/workflows/CI.yml
--rw-r--r--   0        0        0      263 2024-03-25 20:12:08.615242 scematk-0.0.2rc98.post1/.github/workflows/publish.yml
--rw-r--r--   0        0        0      675 2024-03-25 20:12:08.615242 scematk-0.0.2rc98.post1/.github/workflows/schedule-update-actions.yml
--rw-r--r--   0        0        0      318 2024-03-25 20:12:08.615242 scematk-0.0.2rc98.post1/.github/workflows/semantic-pr-check.yml
--rw-r--r--   0        0        0      368 2024-03-25 20:12:08.615242 scematk-0.0.2rc98.post1/.github/workflows/sphinx.yml
--rw-r--r--   0        0        0      307 2024-03-25 20:12:08.615242 scematk-0.0.2rc98.post1/.github/workflows/template-sync.yml
--rw-r--r--   0        0        0     1826 2024-03-25 20:12:08.615242 scematk-0.0.2rc98.post1/.gitignore
--rw-r--r--   0        0        0     1540 2024-03-25 20:12:08.615242 scematk-0.0.2rc98.post1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      158 2024-03-25 20:12:08.615242 scematk-0.0.2rc98.post1/.pypirc
--rw-r--r--   0        0        0      459 2024-03-25 20:12:08.615242 scematk-0.0.2rc98.post1/.vscode/launch.json
--rw-r--r--   0        0        0      817 2024-03-25 20:12:08.615242 scematk-0.0.2rc98.post1/.vscode/settings.json
--rw-r--r--   0        0        0      444 2024-03-25 20:12:08.615242 scematk-0.0.2rc98.post1/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     1141 2024-03-25 20:12:08.615242 scematk-0.0.2rc98.post1/LICENSE
--rw-r--r--   0        0        0    14946 2024-03-25 20:12:08.615242 scematk-0.0.2rc98.post1/README.md
--rw-r--r--   0        0        0     2780 2024-03-25 20:12:08.615242 scematk-0.0.2rc98.post1/SECURITY.md
--rw-r--r--   0        0        0     1308 2024-03-25 20:12:08.615242 scematk-0.0.2rc98.post1/SUPPORT.md
--rw-r--r--   0        0        0      634 2024-03-25 20:12:08.615242 scematk-0.0.2rc98.post1/docs/Makefile
--rw-r--r--   0        0        0     2321 2024-03-25 20:12:08.615242 scematk-0.0.2rc98.post1/docs/conf.py
--rw-r--r--   0        0        0      360 2024-03-25 20:12:08.615242 scematk-0.0.2rc98.post1/docs/devcontainer.md
--rw-r--r--   0        0        0       47 2024-03-25 20:12:08.615242 scematk-0.0.2rc98.post1/docs/developer.md
--rw-r--r--   0        0        0      468 2024-03-25 20:12:08.615242 scematk-0.0.2rc98.post1/docs/index.rst
--rw-r--r--   0        0        0      800 2024-03-25 20:12:08.615242 scematk-0.0.2rc98.post1/docs/make.bat
--rw-r--r--   0        0        0       57 2024-03-25 20:12:08.615242 scematk-0.0.2rc98.post1/docs/modules.rst
--rw-r--r--   0        0        0      471 2024-03-25 20:12:08.615242 scematk-0.0.2rc98.post1/docs/pre-commit-config.md
--rw-r--r--   0        0        0    16088 2024-03-25 20:12:08.615242 scematk-0.0.2rc98.post1/docs/pylint.md
--rw-r--r--   0        0        0      497 2024-03-25 20:12:08.615242 scematk-0.0.2rc98.post1/docs/pyproject.md
--rw-r--r--   0        0        0      437 2024-03-25 20:12:08.615242 scematk-0.0.2rc98.post1/docs/python_package.hello_world.rst
--rw-r--r--   0        0        0      427 2024-03-25 20:12:08.615242 scematk-0.0.2rc98.post1/docs/python_package.rst
--rw-r--r--   0        0        0       42 2024-03-25 20:12:08.615242 scematk-0.0.2rc98.post1/docs/requirements.txt
--rw-r--r--   0        0        0       44 2024-03-25 20:12:08.615242 scematk-0.0.2rc98.post1/docs/vscode.md
--rw-r--r--   0        0        0      208 2024-03-25 20:12:08.615242 scematk-0.0.2rc98.post1/docs/workflows.md
--rw-r--r--   0        0        0     6829 2024-03-25 20:12:08.615242 scematk-0.0.2rc98.post1/pyproject.toml
--rw-r--r--   0        0        0      360 2024-03-25 20:12:22.635061 scematk-0.0.2rc98.post1/src/scematk/__init__.py
--rw-r--r--   0        0        0       92 2024-03-25 20:12:08.615242 scematk-0.0.2rc98.post1/src/scematk/normaliser/__init__.py
--rw-r--r--   0        0        0      942 2024-03-25 20:12:08.615242 scematk-0.0.2rc98.post1/src/scematk/normaliser/_normaliser.py
--rw-r--r--   0        0        0     1904 2024-03-25 20:12:08.615242 scematk-0.0.2rc98.post1/src/scematk/normaliser/_reinhard_normaliser.py
--rw-r--r--   0        0        0       67 2024-03-25 20:12:08.615242 scematk-0.0.2rc98.post1/src/scematk/plot/__init__.py
--rw-r--r--   0        0        0     1234 2024-03-25 20:12:08.615242 scematk-0.0.2rc98.post1/src/scematk/plot/_show_thumb.py
--rw-r--r--   0        0        0      109 2024-03-25 20:12:08.615242 scematk-0.0.2rc98.post1/src/scematk/process/__init__.py
--rw-r--r--   0        0        0      448 2024-03-25 20:12:08.615242 scematk-0.0.2rc98.post1/src/scematk/process/_process.py
--rw-r--r--   0        0        0      755 2024-03-25 20:12:08.615242 scematk-0.0.2rc98.post1/src/scematk/process/_processor.py
--rw-r--r--   0        0        0      252 2024-03-25 20:12:08.615242 scematk-0.0.2rc98.post1/src/scematk/process/colour/__init__.py
--rw-r--r--   0        0        0      762 2024-03-25 20:12:08.615242 scematk-0.0.2rc98.post1/src/scematk/process/colour/_grey_transform.py
--rw-r--r--   0        0        0      642 2024-03-25 20:12:08.615242 scematk-0.0.2rc98.post1/src/scematk/process/colour/_hsv_transform.py
--rw-r--r--   0        0        0      641 2024-03-25 20:12:08.615242 scematk-0.0.2rc98.post1/src/scematk/process/colour/_lab_transform.py
--rw-r--r--   0        0        0     1486 2024-03-25 20:12:08.615242 scematk-0.0.2rc98.post1/src/scematk/process/colour/_od_transform.py
--rw-r--r--   0        0        0      112 2024-03-25 20:12:08.615242 scematk-0.0.2rc98.post1/src/scematk/process/contrast/__init__.py
--rw-r--r--   0        0        0     1231 2024-03-25 20:12:08.615242 scematk-0.0.2rc98.post1/src/scematk/process/contrast/_contrast2d.py
--rw-r--r--   0        0        0       73 2024-03-25 20:12:08.615242 scematk-0.0.2rc98.post1/src/scematk/process/filter/__init__.py
--rw-r--r--   0        0        0      794 2024-03-25 20:12:08.615242 scematk-0.0.2rc98.post1/src/scematk/process/filter/_gaussian.py
--rw-r--r--   0        0        0      124 2024-03-25 20:12:08.615242 scematk-0.0.2rc98.post1/src/scematk/process/luminosity/__init__.py
--rw-r--r--   0        0        0      941 2024-03-25 20:12:08.619242 scematk-0.0.2rc98.post1/src/scematk/process/luminosity/_percentile_standardiser.py
--rw-r--r--   0        0        0      256 2024-03-25 20:12:08.619242 scematk-0.0.2rc98.post1/src/scematk/process/morphology/__init__.py
--rw-r--r--   0        0        0     3933 2024-03-25 20:12:08.619242 scematk-0.0.2rc98.post1/src/scematk/process/morphology/_binary_morphology.py
--rw-r--r--   0        0        0      923 2024-03-25 20:12:08.619242 scematk-0.0.2rc98.post1/src/scematk/process/morphology/_label_morphology.py
--rw-r--r--   0        0        0       56 2024-03-25 20:12:08.619242 scematk-0.0.2rc98.post1/src/scematk/qc/__init__.py
--rw-r--r--   0        0        0      938 2024-03-25 20:12:08.619242 scematk-0.0.2rc98.post1/src/scematk/qc/_qc_step.py
--rw-r--r--   0        0        0     1368 2024-03-25 20:12:08.619242 scematk-0.0.2rc98.post1/src/scematk/qc/folds/_fold_detector.py
--rw-r--r--   0        0        0      317 2024-03-25 20:12:08.619242 scematk-0.0.2rc98.post1/src/scematk/qc/folds/_rules_based.py
--rw-r--r--   0        0        0      161 2024-03-25 20:12:08.619242 scematk-0.0.2rc98.post1/src/scematk/qc/pen/__init__.py
--rw-r--r--   0        0        0      269 2024-03-25 20:12:08.619242 scematk-0.0.2rc98.post1/src/scematk/qc/pen/_pen_detector.py
--rw-r--r--   0        0        0     1320 2024-03-25 20:12:08.619242 scematk-0.0.2rc98.post1/src/scematk/qc/pen/_rules_based_pen_detector.py
--rw-r--r--   0        0        0      197 2024-03-25 20:12:08.619242 scematk-0.0.2rc98.post1/src/scematk/segment/__init__.py
--rw-r--r--   0        0        0     2257 2024-03-25 20:12:08.619242 scematk-0.0.2rc98.post1/src/scematk/segment/_segmenters.py
--rw-r--r--   0        0        0      183 2024-03-25 20:12:08.619242 scematk-0.0.2rc98.post1/src/scematk/segment/tissue/__init__.py
--rw-r--r--   0        0        0     1966 2024-03-25 20:12:08.619242 scematk-0.0.2rc98.post1/src/scematk/segment/tissue/_global_otsu.py
--rw-r--r--   0        0        0     1213 2024-03-25 20:12:08.619242 scematk-0.0.2rc98.post1/src/scematk/segment/tissue/_rules_based.py
--rw-r--r--   0        0        0      989 2024-03-25 20:12:08.619242 scematk-0.0.2rc98.post1/tests/conftest.py
--rw-r--r--   0        0        0      199 2024-03-25 20:12:08.619242 scematk-0.0.2rc98.post1/tests/test_plot.py
--rw-r--r--   0        0        0      435 2024-03-25 20:12:08.619242 scematk-0.0.2rc98.post1/tests/test_process_colour.py
--rw-r--r--   0        0        0    17026 1970-01-01 00:00:00.000000 scematk-0.0.2rc98.post1/PKG-INFO
+-rw-r--r--   0        0        0      333 2024-03-25 21:00:59.546533 scematk-0.0.2rc99.post1/.devcontainer/Dockerfile
+-rw-r--r--   0        0        0     1157 2024-03-25 21:00:59.546533 scematk-0.0.2rc99.post1/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0      417 2024-03-25 21:00:59.546533 scematk-0.0.2rc99.post1/.github/dependabot.yml
+-rw-r--r--   0        0        0      418 2024-03-25 21:00:59.546533 scematk-0.0.2rc99.post1/.github/template-sync.yml
+-rw-r--r--   0        0        0      476 2024-03-25 21:00:59.546533 scematk-0.0.2rc99.post1/.github/workflows/CI.yml
+-rw-r--r--   0        0        0      263 2024-03-25 21:00:59.546533 scematk-0.0.2rc99.post1/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      675 2024-03-25 21:00:59.546533 scematk-0.0.2rc99.post1/.github/workflows/schedule-update-actions.yml
+-rw-r--r--   0        0        0      318 2024-03-25 21:00:59.546533 scematk-0.0.2rc99.post1/.github/workflows/semantic-pr-check.yml
+-rw-r--r--   0        0        0      368 2024-03-25 21:00:59.546533 scematk-0.0.2rc99.post1/.github/workflows/sphinx.yml
+-rw-r--r--   0        0        0      307 2024-03-25 21:00:59.546533 scematk-0.0.2rc99.post1/.github/workflows/template-sync.yml
+-rw-r--r--   0        0        0     1826 2024-03-25 21:00:59.546533 scematk-0.0.2rc99.post1/.gitignore
+-rw-r--r--   0        0        0     1540 2024-03-25 21:00:59.546533 scematk-0.0.2rc99.post1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      158 2024-03-25 21:00:59.546533 scematk-0.0.2rc99.post1/.pypirc
+-rw-r--r--   0        0        0      459 2024-03-25 21:00:59.546533 scematk-0.0.2rc99.post1/.vscode/launch.json
+-rw-r--r--   0        0        0      817 2024-03-25 21:00:59.546533 scematk-0.0.2rc99.post1/.vscode/settings.json
+-rw-r--r--   0        0        0      444 2024-03-25 21:00:59.546533 scematk-0.0.2rc99.post1/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     1141 2024-03-25 21:00:59.546533 scematk-0.0.2rc99.post1/LICENSE
+-rw-r--r--   0        0        0    14946 2024-03-25 21:00:59.546533 scematk-0.0.2rc99.post1/README.md
+-rw-r--r--   0        0        0     2780 2024-03-25 21:00:59.546533 scematk-0.0.2rc99.post1/SECURITY.md
+-rw-r--r--   0        0        0     1308 2024-03-25 21:00:59.546533 scematk-0.0.2rc99.post1/SUPPORT.md
+-rw-r--r--   0        0        0      634 2024-03-25 21:00:59.546533 scematk-0.0.2rc99.post1/docs/Makefile
+-rw-r--r--   0        0        0     2321 2024-03-25 21:00:59.546533 scematk-0.0.2rc99.post1/docs/conf.py
+-rw-r--r--   0        0        0      360 2024-03-25 21:00:59.546533 scematk-0.0.2rc99.post1/docs/devcontainer.md
+-rw-r--r--   0        0        0       47 2024-03-25 21:00:59.546533 scematk-0.0.2rc99.post1/docs/developer.md
+-rw-r--r--   0        0        0      468 2024-03-25 21:00:59.546533 scematk-0.0.2rc99.post1/docs/index.rst
+-rw-r--r--   0        0        0      800 2024-03-25 21:00:59.546533 scematk-0.0.2rc99.post1/docs/make.bat
+-rw-r--r--   0        0        0       57 2024-03-25 21:00:59.546533 scematk-0.0.2rc99.post1/docs/modules.rst
+-rw-r--r--   0        0        0      471 2024-03-25 21:00:59.546533 scematk-0.0.2rc99.post1/docs/pre-commit-config.md
+-rw-r--r--   0        0        0    16088 2024-03-25 21:00:59.550533 scematk-0.0.2rc99.post1/docs/pylint.md
+-rw-r--r--   0        0        0      497 2024-03-25 21:00:59.550533 scematk-0.0.2rc99.post1/docs/pyproject.md
+-rw-r--r--   0        0        0      437 2024-03-25 21:00:59.550533 scematk-0.0.2rc99.post1/docs/python_package.hello_world.rst
+-rw-r--r--   0        0        0      427 2024-03-25 21:00:59.550533 scematk-0.0.2rc99.post1/docs/python_package.rst
+-rw-r--r--   0        0        0       42 2024-03-25 21:00:59.550533 scematk-0.0.2rc99.post1/docs/requirements.txt
+-rw-r--r--   0        0        0       44 2024-03-25 21:00:59.550533 scematk-0.0.2rc99.post1/docs/vscode.md
+-rw-r--r--   0        0        0      208 2024-03-25 21:00:59.550533 scematk-0.0.2rc99.post1/docs/workflows.md
+-rw-r--r--   0        0        0     6829 2024-03-25 21:00:59.550533 scematk-0.0.2rc99.post1/pyproject.toml
+-rw-r--r--   0        0        0      360 2024-03-25 21:01:12.618510 scematk-0.0.2rc99.post1/src/scematk/__init__.py
+-rw-r--r--   0        0        0       92 2024-03-25 21:00:59.550533 scematk-0.0.2rc99.post1/src/scematk/normaliser/__init__.py
+-rw-r--r--   0        0        0      956 2024-03-25 21:00:59.550533 scematk-0.0.2rc99.post1/src/scematk/normaliser/_normaliser.py
+-rw-r--r--   0        0        0     1924 2024-03-25 21:00:59.550533 scematk-0.0.2rc99.post1/src/scematk/normaliser/_reinhard_normaliser.py
+-rw-r--r--   0        0        0       67 2024-03-25 21:00:59.550533 scematk-0.0.2rc99.post1/src/scematk/plot/__init__.py
+-rw-r--r--   0        0        0     1234 2024-03-25 21:00:59.550533 scematk-0.0.2rc99.post1/src/scematk/plot/_show_thumb.py
+-rw-r--r--   0        0        0      109 2024-03-25 21:00:59.550533 scematk-0.0.2rc99.post1/src/scematk/process/__init__.py
+-rw-r--r--   0        0        0      448 2024-03-25 21:00:59.550533 scematk-0.0.2rc99.post1/src/scematk/process/_process.py
+-rw-r--r--   0        0        0      755 2024-03-25 21:00:59.550533 scematk-0.0.2rc99.post1/src/scematk/process/_processor.py
+-rw-r--r--   0        0        0      252 2024-03-25 21:00:59.550533 scematk-0.0.2rc99.post1/src/scematk/process/colour/__init__.py
+-rw-r--r--   0        0        0      762 2024-03-25 21:00:59.550533 scematk-0.0.2rc99.post1/src/scematk/process/colour/_grey_transform.py
+-rw-r--r--   0        0        0      642 2024-03-25 21:00:59.550533 scematk-0.0.2rc99.post1/src/scematk/process/colour/_hsv_transform.py
+-rw-r--r--   0        0        0      641 2024-03-25 21:00:59.550533 scematk-0.0.2rc99.post1/src/scematk/process/colour/_lab_transform.py
+-rw-r--r--   0        0        0     1486 2024-03-25 21:00:59.550533 scematk-0.0.2rc99.post1/src/scematk/process/colour/_od_transform.py
+-rw-r--r--   0        0        0      112 2024-03-25 21:00:59.550533 scematk-0.0.2rc99.post1/src/scematk/process/contrast/__init__.py
+-rw-r--r--   0        0        0     1231 2024-03-25 21:00:59.550533 scematk-0.0.2rc99.post1/src/scematk/process/contrast/_contrast2d.py
+-rw-r--r--   0        0        0       73 2024-03-25 21:00:59.550533 scematk-0.0.2rc99.post1/src/scematk/process/filter/__init__.py
+-rw-r--r--   0        0        0      794 2024-03-25 21:00:59.550533 scematk-0.0.2rc99.post1/src/scematk/process/filter/_gaussian.py
+-rw-r--r--   0        0        0      124 2024-03-25 21:00:59.550533 scematk-0.0.2rc99.post1/src/scematk/process/luminosity/__init__.py
+-rw-r--r--   0        0        0      973 2024-03-25 21:00:59.550533 scematk-0.0.2rc99.post1/src/scematk/process/luminosity/_percentile_standardiser.py
+-rw-r--r--   0        0        0      256 2024-03-25 21:00:59.550533 scematk-0.0.2rc99.post1/src/scematk/process/morphology/__init__.py
+-rw-r--r--   0        0        0     3933 2024-03-25 21:00:59.550533 scematk-0.0.2rc99.post1/src/scematk/process/morphology/_binary_morphology.py
+-rw-r--r--   0        0        0      923 2024-03-25 21:00:59.550533 scematk-0.0.2rc99.post1/src/scematk/process/morphology/_label_morphology.py
+-rw-r--r--   0        0        0       56 2024-03-25 21:00:59.550533 scematk-0.0.2rc99.post1/src/scematk/qc/__init__.py
+-rw-r--r--   0        0        0      938 2024-03-25 21:00:59.550533 scematk-0.0.2rc99.post1/src/scematk/qc/_qc_step.py
+-rw-r--r--   0        0        0     1368 2024-03-25 21:00:59.550533 scematk-0.0.2rc99.post1/src/scematk/qc/folds/_fold_detector.py
+-rw-r--r--   0        0        0      317 2024-03-25 21:00:59.550533 scematk-0.0.2rc99.post1/src/scematk/qc/folds/_rules_based.py
+-rw-r--r--   0        0        0      161 2024-03-25 21:00:59.550533 scematk-0.0.2rc99.post1/src/scematk/qc/pen/__init__.py
+-rw-r--r--   0        0        0      269 2024-03-25 21:00:59.550533 scematk-0.0.2rc99.post1/src/scematk/qc/pen/_pen_detector.py
+-rw-r--r--   0        0        0     1320 2024-03-25 21:00:59.550533 scematk-0.0.2rc99.post1/src/scematk/qc/pen/_rules_based_pen_detector.py
+-rw-r--r--   0        0        0      197 2024-03-25 21:00:59.550533 scematk-0.0.2rc99.post1/src/scematk/segment/__init__.py
+-rw-r--r--   0        0        0     2257 2024-03-25 21:00:59.550533 scematk-0.0.2rc99.post1/src/scematk/segment/_segmenters.py
+-rw-r--r--   0        0        0      183 2024-03-25 21:00:59.550533 scematk-0.0.2rc99.post1/src/scematk/segment/tissue/__init__.py
+-rw-r--r--   0        0        0     1966 2024-03-25 21:00:59.550533 scematk-0.0.2rc99.post1/src/scematk/segment/tissue/_global_otsu.py
+-rw-r--r--   0        0        0     1213 2024-03-25 21:00:59.550533 scematk-0.0.2rc99.post1/src/scematk/segment/tissue/_rules_based.py
+-rw-r--r--   0        0        0      989 2024-03-25 21:00:59.550533 scematk-0.0.2rc99.post1/tests/conftest.py
+-rw-r--r--   0        0        0      199 2024-03-25 21:00:59.550533 scematk-0.0.2rc99.post1/tests/test_plot.py
+-rw-r--r--   0        0        0      435 2024-03-25 21:00:59.550533 scematk-0.0.2rc99.post1/tests/test_process_colour.py
+-rw-r--r--   0        0        0    17026 1970-01-01 00:00:00.000000 scematk-0.0.2rc99.post1/PKG-INFO
```

### Comparing `scematk-0.0.2rc98.post1/.devcontainer/devcontainer.json` & `scematk-0.0.2rc99.post1/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `scematk-0.0.2rc98.post1/.github/workflows/schedule-update-actions.yml` & `scematk-0.0.2rc99.post1/.github/workflows/schedule-update-actions.yml`

 * *Files identical despite different names*

### Comparing `scematk-0.0.2rc98.post1/.gitignore` & `scematk-0.0.2rc99.post1/.gitignore`

 * *Files identical despite different names*

### Comparing `scematk-0.0.2rc98.post1/.pre-commit-config.yaml` & `scematk-0.0.2rc99.post1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `scematk-0.0.2rc98.post1/.vscode/settings.json` & `scematk-0.0.2rc99.post1/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `scematk-0.0.2rc98.post1/LICENSE` & `scematk-0.0.2rc99.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `scematk-0.0.2rc98.post1/README.md` & `scematk-0.0.2rc99.post1/README.md`

 * *Files identical despite different names*

### Comparing `scematk-0.0.2rc98.post1/SECURITY.md` & `scematk-0.0.2rc99.post1/SECURITY.md`

 * *Files identical despite different names*

### Comparing `scematk-0.0.2rc98.post1/SUPPORT.md` & `scematk-0.0.2rc99.post1/SUPPORT.md`

 * *Files identical despite different names*

### Comparing `scematk-0.0.2rc98.post1/docs/Makefile` & `scematk-0.0.2rc99.post1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `scematk-0.0.2rc98.post1/docs/conf.py` & `scematk-0.0.2rc99.post1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `scematk-0.0.2rc98.post1/docs/make.bat` & `scematk-0.0.2rc99.post1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `scematk-0.0.2rc98.post1/docs/pylint.md` & `scematk-0.0.2rc99.post1/docs/pylint.md`

 * *Files identical despite different names*

### Comparing `scematk-0.0.2rc98.post1/pyproject.toml` & `scematk-0.0.2rc99.post1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `scematk-0.0.2rc98.post1/src/scematk/normaliser/_normaliser.py` & `scematk-0.0.2rc99.post1/src/scematk/qc/_qc_step.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from ..process._processor import Processor
 from abc import ABC, abstractmethod
 from dask.array import Array
 
-class Normaliser(ABC):
+class QCStep(ABC):
     def __init__(self, name, preprocessor: Processor = None, postprocessor: Processor = None) -> None:
         self.name = name
         preprocessor = preprocessor or self._default_preprocessor()
         postprocessor = postprocessor or self._default_postprocessor()
         self.preprocessor = preprocessor
         self.postprocessor = postprocessor
         self.fitted = False
```

### Comparing `scematk-0.0.2rc98.post1/src/scematk/normaliser/_reinhard_normaliser.py` & `scematk-0.0.2rc99.post1/src/scematk/normaliser/_reinhard_normaliser.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 
     def fit(self, image: Array) -> None:
         assert isinstance(image, da.Array), "Image must be a dask array"
         assert image.ndim == 3, "Image must have 3 dimensions"
         assert image.shape[2] == 3, "Image must have 3 channels"
         image = self.preprocessor.process(image)
         image = da.map_blocks(rgb2lab, image, dtype="float32")
-        self.means = da.mean(image, axis=(0, 1))
-        self.stds = da.std(image, axis=(0, 1))
+        self.means = da.mean(image, axis=(0, 1)).compute()
+        self.stds = da.std(image, axis=(0, 1)).compute()
         self.fitted = True
 
     def run(self, image: Array) -> Array:
         assert self.fitted, "Normaliser must be fitted before running"
         assert isinstance(image, da.Array), "Image must be a dask array"
         assert image.ndim == 3, "Image must have 3 dimensions"
         assert image.shape[2] == 3, "Image must have 3 channels"
```

### Comparing `scematk-0.0.2rc98.post1/src/scematk/plot/_show_thumb.py` & `scematk-0.0.2rc99.post1/src/scematk/plot/_show_thumb.py`

 * *Files identical despite different names*

### Comparing `scematk-0.0.2rc98.post1/src/scematk/process/_processor.py` & `scematk-0.0.2rc99.post1/src/scematk/process/_processor.py`

 * *Files identical despite different names*

### Comparing `scematk-0.0.2rc98.post1/src/scematk/process/colour/_grey_transform.py` & `scematk-0.0.2rc99.post1/src/scematk/process/colour/_grey_transform.py`

 * *Files identical despite different names*

### Comparing `scematk-0.0.2rc98.post1/src/scematk/process/colour/_hsv_transform.py` & `scematk-0.0.2rc99.post1/src/scematk/process/colour/_hsv_transform.py`

 * *Files identical despite different names*

### Comparing `scematk-0.0.2rc98.post1/src/scematk/process/colour/_lab_transform.py` & `scematk-0.0.2rc99.post1/src/scematk/process/colour/_lab_transform.py`

 * *Files identical despite different names*

### Comparing `scematk-0.0.2rc98.post1/src/scematk/process/colour/_od_transform.py` & `scematk-0.0.2rc99.post1/src/scematk/process/colour/_od_transform.py`

 * *Files identical despite different names*

### Comparing `scematk-0.0.2rc98.post1/src/scematk/process/contrast/_contrast2d.py` & `scematk-0.0.2rc99.post1/src/scematk/process/contrast/_contrast2d.py`

 * *Files identical despite different names*

### Comparing `scematk-0.0.2rc98.post1/src/scematk/process/filter/_gaussian.py` & `scematk-0.0.2rc99.post1/src/scematk/process/filter/_gaussian.py`

 * *Files identical despite different names*

### Comparing `scematk-0.0.2rc98.post1/src/scematk/process/luminosity/_percentile_standardiser.py` & `scematk-0.0.2rc99.post1/src/scematk/process/luminosity/_percentile_standardiser.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,12 +10,13 @@
         assert isinstance(percentile, float), "Percentile must be a float"
         assert 0 < percentile < 1, "Percentile must be between 0 and 1"
         self.percentile = percentile
 
     def process(self, image: Array) -> Array:
         image = da.map_blocks(rgb2lab, image, dtype=float)
         luminosity = image[:, :, 0]
-        luminosity = da.percentile(luminosity.ravel(), self.percentile)
+        percentile = self.percentile
+        luminosity = da.percentile(luminosity.ravel(), percentile)
         image[:, :, 0] = da.clip(image[:, :, 0], 0, luminosity)
         image = da.map_blocks(lab2rgb, image, dtype=float)
         image = da.map_blocks(img_as_ubyte, image, dtype="uint8")
         return image
```

### Comparing `scematk-0.0.2rc98.post1/src/scematk/process/morphology/_binary_morphology.py` & `scematk-0.0.2rc99.post1/src/scematk/process/morphology/_binary_morphology.py`

 * *Files identical despite different names*

### Comparing `scematk-0.0.2rc98.post1/src/scematk/process/morphology/_label_morphology.py` & `scematk-0.0.2rc99.post1/src/scematk/process/morphology/_label_morphology.py`

 * *Files identical despite different names*

### Comparing `scematk-0.0.2rc98.post1/src/scematk/qc/_qc_step.py` & `scematk-0.0.2rc99.post1/src/scematk/normaliser/_normaliser.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 from ..process._processor import Processor
 from abc import ABC, abstractmethod
 from dask.array import Array
 
-class QCStep(ABC):
+class Normaliser(ABC):
     def __init__(self, name, preprocessor: Processor = None, postprocessor: Processor = None) -> None:
         self.name = name
-        preprocessor = preprocessor or self._default_preprocessor()
-        postprocessor = postprocessor or self._default_postprocessor()
+        if preprocessor is None:
+            preprocessor = self._default_preprocessor()
+        if postprocessor is None:
+            postprocessor = self._default_postprocessor()
         self.preprocessor = preprocessor
         self.postprocessor = postprocessor
         self.fitted = False
 
     @abstractmethod
     def fit(self, image: Array) -> None:
         pass
@@ -21,12 +23,12 @@
 
     @abstractmethod
     def fit_and_run(self, image: Array) -> Array:
         pass
 
     @abstractmethod
     def _default_preprocessor(self) -> Processor:
-        return Processor()
+        pass
 
     @abstractmethod
     def _default_postprocessor(self) -> Processor:
-        return Processor()
+        pass
```

### Comparing `scematk-0.0.2rc98.post1/src/scematk/qc/folds/_fold_detector.py` & `scematk-0.0.2rc99.post1/src/scematk/qc/folds/_fold_detector.py`

 * *Files identical despite different names*

### Comparing `scematk-0.0.2rc98.post1/src/scematk/qc/pen/_rules_based_pen_detector.py` & `scematk-0.0.2rc99.post1/src/scematk/qc/pen/_rules_based_pen_detector.py`

 * *Files identical despite different names*

### Comparing `scematk-0.0.2rc98.post1/src/scematk/segment/_segmenters.py` & `scematk-0.0.2rc99.post1/src/scematk/segment/_segmenters.py`

 * *Files identical despite different names*

### Comparing `scematk-0.0.2rc98.post1/src/scematk/segment/tissue/_global_otsu.py` & `scematk-0.0.2rc99.post1/src/scematk/segment/tissue/_global_otsu.py`

 * *Files identical despite different names*

### Comparing `scematk-0.0.2rc98.post1/src/scematk/segment/tissue/_rules_based.py` & `scematk-0.0.2rc99.post1/src/scematk/segment/tissue/_rules_based.py`

 * *Files identical despite different names*

### Comparing `scematk-0.0.2rc98.post1/tests/conftest.py` & `scematk-0.0.2rc99.post1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `scematk-0.0.2rc98.post1/PKG-INFO` & `scematk-0.0.2rc99.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scematk
-Version: 0.0.2rc98.post1
+Version: 0.0.2rc99.post1
 Summary: Sample Python Project for creating a new Python Module
 Author-email: Hugh Warden <hugh.warden@outlook.com>
 Requires-Python: >=3.8.1
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```


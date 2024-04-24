# Comparing `tmp/emtl-0.1.4.dev1.tar.gz` & `tmp/emtl-0.1.5.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emtl-0.1.4.dev1.tar", last modified: Fri Apr 19 01:57:32 2024, max compression
+gzip compressed data, was "emtl-0.1.5.dev1.tar", last modified: Wed Apr 24 03:16:21 2024, max compression
```

## Comparing `emtl-0.1.4.dev1.tar` & `emtl-0.1.5.dev1.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 zhoubo    (1000) zhoubo    (1000)        0 2024-04-19 01:57:32.747393 emtl-0.1.4.dev1/
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)      757 2024-04-19 01:29:59.000000 emtl-0.1.4.dev1/.bumpversion.cfg
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)     1901 2024-04-19 01:29:59.000000 emtl-0.1.4.dev1/.cookiecutterrc
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)      149 2024-04-16 01:27:17.000000 emtl-0.1.4.dev1/.coveragerc
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)      353 2024-04-16 01:27:17.000000 emtl-0.1.4.dev1/.editorconfig
-drwxr-xr-x   0 zhoubo    (1000) zhoubo    (1000)        0 2024-04-19 01:57:32.737393 emtl-0.1.4.dev1/.github/
-drwxr-xr-x   0 zhoubo    (1000) zhoubo    (1000)        0 2024-04-19 01:57:32.747393 emtl-0.1.4.dev1/.github/workflows/
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)      907 2024-04-19 01:18:25.000000 emtl-0.1.4.dev1/.github/workflows/document.yml
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)     3925 2024-04-19 01:32:21.000000 emtl-0.1.4.dev1/.github/workflows/github-actions.yml
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)      734 2024-04-16 01:37:37.000000 emtl-0.1.4.dev1/.gitignore
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)      686 2024-04-16 01:27:59.000000 emtl-0.1.4.dev1/.pre-commit-config.yaml
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)      285 2024-04-17 09:47:16.000000 emtl-0.1.4.dev1/.readthedocs.yml
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)       65 2024-04-16 01:27:17.000000 emtl-0.1.4.dev1/AUTHORS.rst
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)      235 2024-04-19 01:18:25.000000 emtl-0.1.4.dev1/CHANGELOG.rst
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)     2274 2024-04-16 01:27:17.000000 emtl-0.1.4.dev1/CONTRIBUTING.rst
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)     1117 2024-04-16 01:42:17.000000 emtl-0.1.4.dev1/LICENSE
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)     2054 2024-04-19 01:57:32.747393 emtl-0.1.4.dev1/PKG-INFO
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)     2251 2024-04-19 01:29:59.000000 emtl-0.1.4.dev1/README.rst
-drwxr-xr-x   0 zhoubo    (1000) zhoubo    (1000)        0 2024-04-19 01:57:32.747393 emtl-0.1.4.dev1/ci/
--rwxr-xr-x   0 zhoubo    (1000) zhoubo    (1000)     2867 2024-04-16 01:27:17.000000 emtl-0.1.4.dev1/ci/bootstrap.py
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)       72 2024-04-16 01:27:17.000000 emtl-0.1.4.dev1/ci/requirements.txt
-drwxr-xr-x   0 zhoubo    (1000) zhoubo    (1000)        0 2024-04-19 01:57:32.737393 emtl-0.1.4.dev1/ci/templates/
-drwxr-xr-x   0 zhoubo    (1000) zhoubo    (1000)        0 2024-04-19 01:57:32.737393 emtl-0.1.4.dev1/ci/templates/.github/
-drwxr-xr-x   0 zhoubo    (1000) zhoubo    (1000)        0 2024-04-19 01:57:32.747393 emtl-0.1.4.dev1/ci/templates/.github/workflows/
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)     2179 2024-04-16 01:27:17.000000 emtl-0.1.4.dev1/ci/templates/.github/workflows/github-actions.yml
-drwxr-xr-x   0 zhoubo    (1000) zhoubo    (1000)        0 2024-04-19 01:57:32.747393 emtl-0.1.4.dev1/docs/
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)       28 2024-04-16 01:27:17.000000 emtl-0.1.4.dev1/docs/authors.rst
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)       30 2024-04-16 01:27:17.000000 emtl-0.1.4.dev1/docs/changelog.rst
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)     1145 2024-04-19 01:29:59.000000 emtl-0.1.4.dev1/docs/conf.py
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)       33 2024-04-16 01:27:17.000000 emtl-0.1.4.dev1/docs/contributing.rst
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)      244 2024-04-16 01:27:17.000000 emtl-0.1.4.dev1/docs/index.rst
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)       84 2024-04-16 01:27:17.000000 emtl-0.1.4.dev1/docs/installation.rst
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)       27 2024-04-16 01:27:17.000000 emtl-0.1.4.dev1/docs/readme.rst
-drwxr-xr-x   0 zhoubo    (1000) zhoubo    (1000)        0 2024-04-19 01:57:32.747393 emtl-0.1.4.dev1/docs/reference/
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)      146 2024-04-16 01:27:17.000000 emtl-0.1.4.dev1/docs/reference/emtl.rst
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)       56 2024-04-16 01:27:17.000000 emtl-0.1.4.dev1/docs/reference/index.rst
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)       17 2024-04-16 01:27:17.000000 emtl-0.1.4.dev1/docs/requirements.txt
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)      109 2024-04-16 01:27:17.000000 emtl-0.1.4.dev1/docs/spelling_wordlist.txt
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)       98 2024-04-16 01:27:17.000000 emtl-0.1.4.dev1/docs/usage.rst
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)     1381 2024-04-16 01:27:17.000000 emtl-0.1.4.dev1/pyproject.toml
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)     1303 2024-04-16 01:27:17.000000 emtl-0.1.4.dev1/pytest.ini
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)       38 2024-04-19 01:57:32.747393 emtl-0.1.4.dev1/setup.cfg
--rwxr-xr-x   0 zhoubo    (1000) zhoubo    (1000)     3066 2024-04-19 01:29:59.000000 emtl-0.1.4.dev1/setup.py
-drwxr-xr-x   0 zhoubo    (1000) zhoubo    (1000)        0 2024-04-19 01:57:32.747393 emtl-0.1.4.dev1/src/
-drwxr-xr-x   0 zhoubo    (1000) zhoubo    (1000)        0 2024-04-19 01:57:32.747393 emtl-0.1.4.dev1/src/emtl/
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)      183 2024-04-19 01:29:59.000000 emtl-0.1.4.dev1/src/emtl/__init__.py
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)      354 2024-04-16 01:27:17.000000 emtl-0.1.4.dev1/src/emtl/__main__.py
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)      424 2024-04-19 01:57:32.000000 emtl-0.1.4.dev1/src/emtl/_version.py
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)     1003 2024-04-17 00:52:46.000000 emtl-0.1.4.dev1/src/emtl/cli.py
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)     1083 2024-04-17 03:52:39.000000 emtl-0.1.4.dev1/src/emtl/const.py
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)     4310 2024-04-19 01:18:25.000000 emtl-0.1.4.dev1/src/emtl/core.py
-drwxr-xr-x   0 zhoubo    (1000) zhoubo    (1000)        0 2024-04-19 01:57:32.747393 emtl-0.1.4.dev1/src/emtl/tests/
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)        0 2024-04-16 01:27:17.000000 emtl-0.1.4.dev1/src/emtl/tests/__init__.py
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)      133 2024-04-17 01:52:16.000000 emtl-0.1.4.dev1/src/emtl/tests/test_cli.py
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)      624 2024-04-19 01:18:25.000000 emtl-0.1.4.dev1/src/emtl/tests/test_core.py
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)     1585 2024-04-18 02:05:24.000000 emtl-0.1.4.dev1/src/emtl/utils.py
-drwxr-xr-x   0 zhoubo    (1000) zhoubo    (1000)        0 2024-04-19 01:57:32.747393 emtl-0.1.4.dev1/src/emtl.egg-info/
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)     2054 2024-04-19 01:57:32.000000 emtl-0.1.4.dev1/src/emtl.egg-info/PKG-INFO
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)     1045 2024-04-19 01:57:32.000000 emtl-0.1.4.dev1/src/emtl.egg-info/SOURCES.txt
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)        1 2024-04-19 01:57:32.000000 emtl-0.1.4.dev1/src/emtl.egg-info/dependency_links.txt
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)       38 2024-04-19 01:57:32.000000 emtl-0.1.4.dev1/src/emtl.egg-info/entry_points.txt
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)        1 2024-04-16 09:34:21.000000 emtl-0.1.4.dev1/src/emtl.egg-info/not-zip-safe
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)       63 2024-04-19 01:57:32.000000 emtl-0.1.4.dev1/src/emtl.egg-info/requires.txt
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)        5 2024-04-19 01:57:32.000000 emtl-0.1.4.dev1/src/emtl.egg-info/top_level.txt
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)     1593 2024-04-17 08:38:27.000000 emtl-0.1.4.dev1/tox.ini
+drwxr-xr-x   0 zhoubo    (1000) zhoubo    (1000)        0 2024-04-24 03:16:21.076150 emtl-0.1.5.dev1/
+-rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)      757 2024-04-19 03:14:30.000000 emtl-0.1.5.dev1/.bumpversion.cfg
+-rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)     1906 2024-04-19 03:14:30.000000 emtl-0.1.5.dev1/.cookiecutterrc
+-rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)      149 2024-04-16 01:27:17.000000 emtl-0.1.5.dev1/.coveragerc
+-rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)      353 2024-04-16 01:27:17.000000 emtl-0.1.5.dev1/.editorconfig
+drwxr-xr-x   0 zhoubo    (1000) zhoubo    (1000)        0 2024-04-24 03:16:21.056150 emtl-0.1.5.dev1/.github/
+drwxr-xr-x   0 zhoubo    (1000) zhoubo    (1000)        0 2024-04-24 03:16:21.056150 emtl-0.1.5.dev1/.github/workflows/
+-rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)      907 2024-04-19 01:18:25.000000 emtl-0.1.5.dev1/.github/workflows/document.yml
+-rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)     3925 2024-04-19 01:32:21.000000 emtl-0.1.5.dev1/.github/workflows/github-actions.yml
+-rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)      734 2024-04-16 01:37:37.000000 emtl-0.1.5.dev1/.gitignore
+-rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)      686 2024-04-16 01:27:59.000000 emtl-0.1.5.dev1/.pre-commit-config.yaml
+-rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)      285 2024-04-17 09:47:16.000000 emtl-0.1.5.dev1/.readthedocs.yml
+-rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)       65 2024-04-16 01:27:17.000000 emtl-0.1.5.dev1/AUTHORS.rst
+-rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)      296 2024-04-19 03:09:42.000000 emtl-0.1.5.dev1/CHANGELOG.rst
+-rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)     2274 2024-04-16 01:27:17.000000 emtl-0.1.5.dev1/CONTRIBUTING.rst
+-rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)     1117 2024-04-16 01:42:17.000000 emtl-0.1.5.dev1/LICENSE
+-rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)     2115 2024-04-24 03:16:21.076150 emtl-0.1.5.dev1/PKG-INFO
+-rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)     2251 2024-04-19 03:14:30.000000 emtl-0.1.5.dev1/README.rst
+drwxr-xr-x   0 zhoubo    (1000) zhoubo    (1000)        0 2024-04-24 03:16:21.066150 emtl-0.1.5.dev1/ci/
+-rwxr-xr-x   0 zhoubo    (1000) zhoubo    (1000)     2867 2024-04-16 01:27:17.000000 emtl-0.1.5.dev1/ci/bootstrap.py
+-rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)       72 2024-04-16 01:27:17.000000 emtl-0.1.5.dev1/ci/requirements.txt
+drwxr-xr-x   0 zhoubo    (1000) zhoubo    (1000)        0 2024-04-24 03:16:21.056150 emtl-0.1.5.dev1/ci/templates/
+drwxr-xr-x   0 zhoubo    (1000) zhoubo    (1000)        0 2024-04-24 03:16:21.056150 emtl-0.1.5.dev1/ci/templates/.github/
+drwxr-xr-x   0 zhoubo    (1000) zhoubo    (1000)        0 2024-04-24 03:16:21.066150 emtl-0.1.5.dev1/ci/templates/.github/workflows/
+-rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)     2179 2024-04-16 01:27:17.000000 emtl-0.1.5.dev1/ci/templates/.github/workflows/github-actions.yml
+drwxr-xr-x   0 zhoubo    (1000) zhoubo    (1000)        0 2024-04-24 03:16:21.066150 emtl-0.1.5.dev1/docs/
+-rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)       28 2024-04-16 01:27:17.000000 emtl-0.1.5.dev1/docs/authors.rst
+-rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)       30 2024-04-16 01:27:17.000000 emtl-0.1.5.dev1/docs/changelog.rst
+-rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)     1150 2024-04-19 03:14:30.000000 emtl-0.1.5.dev1/docs/conf.py
+-rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)       33 2024-04-16 01:27:17.000000 emtl-0.1.5.dev1/docs/contributing.rst
+-rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)      244 2024-04-16 01:27:17.000000 emtl-0.1.5.dev1/docs/index.rst
+-rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)       84 2024-04-16 01:27:17.000000 emtl-0.1.5.dev1/docs/installation.rst
+-rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)       27 2024-04-16 01:27:17.000000 emtl-0.1.5.dev1/docs/readme.rst
+drwxr-xr-x   0 zhoubo    (1000) zhoubo    (1000)        0 2024-04-24 03:16:21.066150 emtl-0.1.5.dev1/docs/reference/
+-rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)      146 2024-04-16 01:27:17.000000 emtl-0.1.5.dev1/docs/reference/emtl.rst
+-rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)       56 2024-04-16 01:27:17.000000 emtl-0.1.5.dev1/docs/reference/index.rst
+-rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)       14 2024-04-19 02:32:39.000000 emtl-0.1.5.dev1/docs/requirements.txt
+-rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)      109 2024-04-16 01:27:17.000000 emtl-0.1.5.dev1/docs/spelling_wordlist.txt
+-rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)      157 2024-04-19 02:08:08.000000 emtl-0.1.5.dev1/docs/usage.rst
+-rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)     1381 2024-04-16 01:27:17.000000 emtl-0.1.5.dev1/pyproject.toml
+-rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)     1303 2024-04-16 01:27:17.000000 emtl-0.1.5.dev1/pytest.ini
+-rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)       38 2024-04-24 03:16:21.076150 emtl-0.1.5.dev1/setup.cfg
+-rwxr-xr-x   0 zhoubo    (1000) zhoubo    (1000)     3066 2024-04-19 03:14:30.000000 emtl-0.1.5.dev1/setup.py
+drwxr-xr-x   0 zhoubo    (1000) zhoubo    (1000)        0 2024-04-24 03:16:21.056150 emtl-0.1.5.dev1/src/
+drwxr-xr-x   0 zhoubo    (1000) zhoubo    (1000)        0 2024-04-24 03:16:21.066150 emtl-0.1.5.dev1/src/emtl/
+-rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)      183 2024-04-19 03:14:30.000000 emtl-0.1.5.dev1/src/emtl/__init__.py
+-rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)      354 2024-04-16 01:27:17.000000 emtl-0.1.5.dev1/src/emtl/__main__.py
+-rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)      424 2024-04-24 03:16:20.000000 emtl-0.1.5.dev1/src/emtl/_version.py
+-rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)     1003 2024-04-17 00:52:46.000000 emtl-0.1.5.dev1/src/emtl/cli.py
+-rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)     1083 2024-04-17 03:52:39.000000 emtl-0.1.5.dev1/src/emtl/const.py
+-rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)     4376 2024-04-23 11:01:13.000000 emtl-0.1.5.dev1/src/emtl/core.py
+drwxr-xr-x   0 zhoubo    (1000) zhoubo    (1000)        0 2024-04-24 03:16:21.066150 emtl-0.1.5.dev1/src/emtl/tests/
+-rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)        0 2024-04-16 01:27:17.000000 emtl-0.1.5.dev1/src/emtl/tests/__init__.py
+-rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)      133 2024-04-17 01:52:16.000000 emtl-0.1.5.dev1/src/emtl/tests/test_cli.py
+-rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)      624 2024-04-19 01:18:25.000000 emtl-0.1.5.dev1/src/emtl/tests/test_core.py
+-rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)     1585 2024-04-18 02:05:24.000000 emtl-0.1.5.dev1/src/emtl/utils.py
+drwxr-xr-x   0 zhoubo    (1000) zhoubo    (1000)        0 2024-04-24 03:16:21.066150 emtl-0.1.5.dev1/src/emtl.egg-info/
+-rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)     2115 2024-04-24 03:16:20.000000 emtl-0.1.5.dev1/src/emtl.egg-info/PKG-INFO
+-rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)     1045 2024-04-24 03:16:21.000000 emtl-0.1.5.dev1/src/emtl.egg-info/SOURCES.txt
+-rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)        1 2024-04-24 03:16:20.000000 emtl-0.1.5.dev1/src/emtl.egg-info/dependency_links.txt
+-rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)       38 2024-04-24 03:16:20.000000 emtl-0.1.5.dev1/src/emtl.egg-info/entry_points.txt
+-rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)        1 2024-04-16 09:34:21.000000 emtl-0.1.5.dev1/src/emtl.egg-info/not-zip-safe
+-rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)       63 2024-04-24 03:16:20.000000 emtl-0.1.5.dev1/src/emtl.egg-info/requires.txt
+-rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)        5 2024-04-24 03:16:20.000000 emtl-0.1.5.dev1/src/emtl.egg-info/top_level.txt
+-rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)     1593 2024-04-17 08:38:27.000000 emtl-0.1.5.dev1/tox.ini
```

### Comparing `emtl-0.1.4.dev1/.cookiecutterrc` & `emtl-0.1.5.dev1/.cookiecutterrc`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     repo_name: "emtl"
     repo_username: "riiy"
     scrutinizer: "no"
     setup_py_uses_setuptools_scm: "yes"
     sphinx_docs: "yes"
     sphinx_docs_hosting: "https://emtl.readthedocs.io/"
     sphinx_doctest: "no"
-    sphinx_theme: "furo"
+    sphinx_theme: "alabaster"
     test_matrix_separate_coverage: "yes"
     tests_inside_package: "yes"
-    version: "0.1.2"
+    version: "0.1.3"
     version_manager: "bump2version"
     website: "riiy.gihub.io/emtl"
     year_from: "2024"
     year_to: "2025"
```

### Comparing `emtl-0.1.4.dev1/.github/workflows/document.yml` & `emtl-0.1.5.dev1/.github/workflows/document.yml`

 * *Files identical despite different names*

### Comparing `emtl-0.1.4.dev1/.github/workflows/github-actions.yml` & `emtl-0.1.5.dev1/.github/workflows/github-actions.yml`

 * *Files identical despite different names*

### Comparing `emtl-0.1.4.dev1/.gitignore` & `emtl-0.1.5.dev1/.gitignore`

 * *Files identical despite different names*

### Comparing `emtl-0.1.4.dev1/.pre-commit-config.yaml` & `emtl-0.1.5.dev1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `emtl-0.1.4.dev1/CONTRIBUTING.rst` & `emtl-0.1.5.dev1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `emtl-0.1.4.dev1/LICENSE` & `emtl-0.1.5.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `emtl-0.1.4.dev1/PKG-INFO` & `emtl-0.1.5.dev1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emtl
-Version: 0.1.4.dev1
+Version: 0.1.5.dev1
 Summary: 东方财富自动交易系统
 Home-page: https://github.com/riiy/emtl
 Author: Eastmoney Trade Library
 Author-email: riiyzhou@gmail.com
 License: MIT
 Project-URL: Documentation, https://emtl.readthedocs.io/
 Project-URL: Changelog, https://emtl.readthedocs.io/en/latest/changelog.html
@@ -80,23 +80,29 @@
 
             PYTEST_ADDOPTS=--cov-append tox
 
 
 Changelog
 =========
 
-0.1.2 (2024-04-18)
+
+0.1.0 (2024-04-14)
 ------------------
 
-* add login && add asset position
+* First release on PyPI.
 
 0.1.1 (2024-04-16)
 ------------------
 
 * Delete python3.8 python3.9 pypy.
 
-0.1.0 (2024-04-14)
+0.1.2 (2024-04-18)
 ------------------
 
-* First release on PyPI.
+* add login && add asset position
+
+0.1.3 (2024-04-19)
+------------------
+
+* update docs theme
```

### Comparing `emtl-0.1.4.dev1/README.rst` & `emtl-0.1.5.dev1/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -37,17 +37,17 @@
     :alt: Supported versions
     :target: https://pypi.org/project/emtl
 
 .. |supported-implementations| image:: https://img.shields.io/pypi/implementation/emtl.svg
     :alt: Supported implementations
     :target: https://pypi.org/project/emtl
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/riiy/emtl/v0.1.3.svg
+.. |commits-since| image:: https://img.shields.io/github/commits-since/riiy/emtl/v0.1.4.svg
     :alt: Commits since latest release
-    :target: https://github.com/riiy/emtl/compare/v0.1.3...master
+    :target: https://github.com/riiy/emtl/compare/v0.1.4...master
 
 
 
 .. end-badges
 
 东方财富自动交易系统
```

### Comparing `emtl-0.1.4.dev1/ci/bootstrap.py` & `emtl-0.1.5.dev1/ci/bootstrap.py`

 * *Files identical despite different names*

### Comparing `emtl-0.1.4.dev1/ci/templates/.github/workflows/github-actions.yml` & `emtl-0.1.5.dev1/ci/templates/.github/workflows/github-actions.yml`

 * *Files identical despite different names*

### Comparing `emtl-0.1.4.dev1/docs/conf.py` & `emtl-0.1.5.dev1/docs/conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,24 +21,24 @@
     from pkg_resources import get_distribution
 
     version = release = get_distribution("emtl").version
 except Exception:
     import traceback
 
     traceback.print_exc()
-    version = release = "0.1.3"
+    version = release = "0.1.4"
 
 pygments_style = "trac"
 templates_path = ["."]
 extlinks = {
     "issue": ("https://github.com/riiy/emtl/issues/%s", "#%s"),
     "pr": ("https://github.com/riiy/emtl/pull/%s", "PR #%s"),
 }
 
-html_theme = "furo"
+html_theme = "alabaster"
 html_theme_options = {
     "githuburl": "https://github.com/riiy/emtl/",
 }
 
 html_use_smartypants = True
 html_last_updated_fmt = "%b %d, %Y"
 html_split_index = False
```

### Comparing `emtl-0.1.4.dev1/pyproject.toml` & `emtl-0.1.5.dev1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `emtl-0.1.4.dev1/pytest.ini` & `emtl-0.1.5.dev1/pytest.ini`

 * *Files identical despite different names*

### Comparing `emtl-0.1.4.dev1/setup.py` & `emtl-0.1.5.dev1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 
 setup(
     name="emtl",
     use_scm_version={
         "local_scheme": "dirty-tag",
         "write_to": "src/emtl/_version.py",
-        "fallback_version": "0.1.3",
+        "fallback_version": "0.1.4",
     },
     license="MIT",
     description="东方财富自动交易系统",
     long_description="{}\n{}".format(
         re.compile("^.. start-badges.*^.. end-badges", re.M | re.S).sub("", read("README.rst")),
         re.sub(":[a-z]+:`~?(.*?)`", r"``\1``", read("CHANGELOG.rst")),
     ),
```

### Comparing `emtl-0.1.4.dev1/src/emtl/cli.py` & `emtl-0.1.5.dev1/src/emtl/cli.py`

 * *Files identical despite different names*

### Comparing `emtl-0.1.4.dev1/src/emtl/const.py` & `emtl-0.1.5.dev1/src/emtl/const.py`

 * *Files identical despite different names*

### Comparing `emtl-0.1.4.dev1/src/emtl/core.py` & `emtl-0.1.5.dev1/src/emtl/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,18 +90,20 @@
         _em_validatekey = match_result[0].strip()
         global _em_validate_key
         _em_validate_key = _em_validatekey
         return _em_validatekey
 
 
 def login(username: str, password: str, duration: int = 30) -> Optional[str]:
-    """Login.
-    :param username: 用户名
-    :param password: 密码(明文)
-    :param duration: 在线时长(分钟)
+    """登录接口.
+
+    :param str username: 用户名
+    :param str password: 密码(明文)
+    :param duration: 在线时长(分钟), defaults to 30
+    :type duration: int, optional
     :return:
     """
     if (ret := _get_captcha_code()) is None:
         return ""
     random_num, code = ret
     logger.error(code)
     headers = _base_headers.copy()
```

### Comparing `emtl-0.1.4.dev1/src/emtl/tests/test_core.py` & `emtl-0.1.5.dev1/src/emtl/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `emtl-0.1.4.dev1/src/emtl/utils.py` & `emtl-0.1.5.dev1/src/emtl/utils.py`

 * *Files identical despite different names*

### Comparing `emtl-0.1.4.dev1/src/emtl.egg-info/PKG-INFO` & `emtl-0.1.5.dev1/src/emtl.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emtl
-Version: 0.1.4.dev1
+Version: 0.1.5.dev1
 Summary: 东方财富自动交易系统
 Home-page: https://github.com/riiy/emtl
 Author: Eastmoney Trade Library
 Author-email: riiyzhou@gmail.com
 License: MIT
 Project-URL: Documentation, https://emtl.readthedocs.io/
 Project-URL: Changelog, https://emtl.readthedocs.io/en/latest/changelog.html
@@ -80,23 +80,29 @@
 
             PYTEST_ADDOPTS=--cov-append tox
 
 
 Changelog
 =========
 
-0.1.2 (2024-04-18)
+
+0.1.0 (2024-04-14)
 ------------------
 
-* add login && add asset position
+* First release on PyPI.
 
 0.1.1 (2024-04-16)
 ------------------
 
 * Delete python3.8 python3.9 pypy.
 
-0.1.0 (2024-04-14)
+0.1.2 (2024-04-18)
 ------------------
 
-* First release on PyPI.
+* add login && add asset position
+
+0.1.3 (2024-04-19)
+------------------
+
+* update docs theme
```

### Comparing `emtl-0.1.4.dev1/src/emtl.egg-info/SOURCES.txt` & `emtl-0.1.5.dev1/src/emtl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `emtl-0.1.4.dev1/tox.ini` & `emtl-0.1.5.dev1/tox.ini`

 * *Files identical despite different names*


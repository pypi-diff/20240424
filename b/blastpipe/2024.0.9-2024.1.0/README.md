# Comparing `tmp/blastpipe-2024.0.9.tar.gz` & `tmp/blastpipe-2024.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blastpipe-2024.0.9.tar", last modified: Mon Apr 22 21:13:55 2024, max compression
+gzip compressed data, was "blastpipe-2024.1.0.tar", last modified: Tue Apr 23 22:41:26 2024, max compression
```

## Comparing `blastpipe-2024.0.9.tar` & `blastpipe-2024.1.0.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 21:13:55.145464 blastpipe-2024.0.9/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-22 21:07:44.000000 blastpipe-2024.0.9/.github/
--rw-rw-r--   0 runner    (1001) docker     (127)       56 2024-04-22 21:07:44.000000 blastpipe-2024.0.9/.github/.markdownlint.json
--rw-rw-r--   0 runner    (1001) docker     (127)      111 2024-04-22 21:07:44.000000 blastpipe-2024.0.9/.github/dependabot.yml
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-22 21:07:44.000000 blastpipe-2024.0.9/.github/workflows/
--rw-rw-r--   0 runner    (1001) docker     (127)     2886 2024-04-22 21:07:44.000000 blastpipe-2024.0.9/.github/workflows/codeql.yml
--rw-rw-r--   0 runner    (1001) docker     (127)      968 2024-04-22 21:07:44.000000 blastpipe-2024.0.9/.github/workflows/dependency-review.yml
--rw-rw-r--   0 runner    (1001) docker     (127)     5869 2024-04-22 21:07:44.000000 blastpipe-2024.0.9/.github/workflows/ozi.yml
--rw-rw-r--   0 runner    (1001) docker     (127)     3060 2024-04-22 21:07:44.000000 blastpipe-2024.0.9/.github/workflows/scorecards.yml
--rw-rw-r--   0 runner    (1001) docker     (127)     3105 2024-04-22 21:07:44.000000 blastpipe-2024.0.9/.gitignore
--rw-rw-r--   0 runner    (1001) docker     (127)      309 2024-04-22 21:07:44.000000 blastpipe-2024.0.9/.pre-commit-config.yaml
--rw-rw-r--   0 runner    (1001) docker     (127)    77004 2024-04-22 21:07:44.000000 blastpipe-2024.0.9/CHANGELOG.md
--rw-rw-r--   0 runner    (1001) docker     (127)    12501 2024-04-22 21:07:44.000000 blastpipe-2024.0.9/LICENSE.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     2710 2024-04-22 21:07:44.000000 blastpipe-2024.0.9/NOTICE.md
--rw-r--r--   0 runner    (1001) docker     (127)     5477 2024-04-22 21:13:55.145464 blastpipe-2024.0.9/PKG-INFO
--rw-rw-r--   0 runner    (1001) docker     (127)     4528 2024-04-22 21:07:44.000000 blastpipe-2024.0.9/README.rst
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-22 21:07:44.000000 blastpipe-2024.0.9/blastpipe/
--rw-rw-r--   0 runner    (1001) docker     (127)     1279 2024-04-22 21:07:44.000000 blastpipe-2024.0.9/blastpipe/__init__.py
--rw-rw-r--   0 runner    (1001) docker     (127)      138 2024-04-22 21:07:44.000000 blastpipe-2024.0.9/blastpipe/__init__.pyi
--rw-rw-r--   0 runner    (1001) docker     (127)     3202 2024-04-22 21:07:44.000000 blastpipe-2024.0.9/blastpipe/backports.py
--rw-rw-r--   0 runner    (1001) docker     (127)     1006 2024-04-22 21:07:44.000000 blastpipe-2024.0.9/blastpipe/backports.pyi
--rw-rw-r--   0 runner    (1001) docker     (127)     1717 2024-04-22 21:07:44.000000 blastpipe-2024.0.9/blastpipe/buffer.py
--rw-rw-r--   0 runner    (1001) docker     (127)      213 2024-04-22 21:07:44.000000 blastpipe-2024.0.9/blastpipe/buffer.pyi
--rw-rw-r--   0 runner    (1001) docker     (127)     1762 2024-04-22 21:07:44.000000 blastpipe-2024.0.9/blastpipe/loop.py
--rw-rw-r--   0 runner    (1001) docker     (127)      331 2024-04-22 21:07:44.000000 blastpipe-2024.0.9/blastpipe/loop.pyi
--rw-rw-r--   0 runner    (1001) docker     (127)     3316 2024-04-22 21:07:44.000000 blastpipe-2024.0.9/blastpipe/malloc.py
--rw-rw-r--   0 runner    (1001) docker     (127)      301 2024-04-22 21:07:44.000000 blastpipe-2024.0.9/blastpipe/malloc.pyi
--rw-rw-r--   0 runner    (1001) docker     (127)     1235 2024-04-22 21:07:44.000000 blastpipe-2024.0.9/blastpipe/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)     1475 2024-04-22 21:07:44.000000 blastpipe-2024.0.9/blastpipe/mixin.py
--rw-rw-r--   0 runner    (1001) docker     (127)      453 2024-04-22 21:07:44.000000 blastpipe-2024.0.9/blastpipe/mixin.pyi
--rw-rw-r--   0 runner    (1001) docker     (127)        0 2024-04-22 21:07:44.000000 blastpipe-2024.0.9/blastpipe/py.typed
--rw-rw-r--   0 runner    (1001) docker     (127)     1865 2024-04-22 21:07:44.000000 blastpipe-2024.0.9/blastpipe/sequence.py
--rw-rw-r--   0 runner    (1001) docker     (127)      101 2024-04-22 21:07:44.000000 blastpipe-2024.0.9/blastpipe/sequence.pyi
--rw-rw-r--   0 runner    (1001) docker     (127)     1696 2024-04-22 21:07:44.000000 blastpipe-2024.0.9/blastpipe/tailcall.py
--rw-rw-r--   0 runner    (1001) docker     (127)      329 2024-04-22 21:07:44.000000 blastpipe-2024.0.9/blastpipe/tailcall.pyi
--rw-rw-r--   0 runner    (1001) docker     (127)     3291 2024-04-22 21:07:44.000000 blastpipe-2024.0.9/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)     4520 2024-04-22 21:07:44.000000 blastpipe-2024.0.9/meson.options
--rw-rw-r--   0 runner    (1001) docker     (127)     8329 2024-04-22 21:07:44.000000 blastpipe-2024.0.9/pyproject.toml
--rw-rw-r--   0 runner    (1001) docker     (127)        0 2024-04-22 21:07:44.000000 blastpipe-2024.0.9/requirements.in
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-22 21:07:44.000000 blastpipe-2024.0.9/subprojects/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-22 21:07:44.000000 blastpipe-2024.0.9/subprojects/docs/
--rw-rw-r--   0 runner    (1001) docker     (127)    12501 2024-04-22 21:07:44.000000 blastpipe-2024.0.9/subprojects/docs/LICENSE.txt
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-22 21:07:44.000000 blastpipe-2024.0.9/subprojects/docs/_static/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-22 21:07:44.000000 blastpipe-2024.0.9/subprojects/docs/_static/css/
--rw-rw-r--   0 runner    (1001) docker     (127)      767 2024-04-22 21:07:44.000000 blastpipe-2024.0.9/subprojects/docs/_static/css/custom.css
--rw-rw-r--   0 runner    (1001) docker     (127)      693 2024-04-22 21:07:44.000000 blastpipe-2024.0.9/subprojects/docs/_static/css/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)      633 2024-04-22 21:07:44.000000 blastpipe-2024.0.9/subprojects/docs/_static/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-22 21:07:44.000000 blastpipe-2024.0.9/subprojects/docs/_templates/
--rw-rw-r--   0 runner    (1001) docker     (127)     1033 2024-04-22 21:07:44.000000 blastpipe-2024.0.9/subprojects/docs/_templates/layout.html
--rw-rw-r--   0 runner    (1001) docker     (127)      694 2024-04-22 21:07:44.000000 blastpipe-2024.0.9/subprojects/docs/_templates/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)      860 2024-04-22 21:07:44.000000 blastpipe-2024.0.9/subprojects/docs/conf.cfg
--rw-rw-r--   0 runner    (1001) docker     (127)     1751 2024-04-22 21:07:44.000000 blastpipe-2024.0.9/subprojects/docs/index.rst
--rw-rw-r--   0 runner    (1001) docker     (127)     2680 2024-04-22 21:07:44.000000 blastpipe-2024.0.9/subprojects/docs/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)     2058 2024-04-22 21:07:44.000000 blastpipe-2024.0.9/subprojects/docs/meson.options
--rw-rw-r--   0 runner    (1001) docker     (127)      121 2024-04-22 21:07:44.000000 blastpipe-2024.0.9/subprojects/ozi.wrap
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-22 21:07:44.000000 blastpipe-2024.0.9/tests/
--rw-rw-r--   0 runner    (1001) docker     (127)      813 2024-04-22 21:07:44.000000 blastpipe-2024.0.9/tests/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)     1219 2024-04-22 21:07:44.000000 blastpipe-2024.0.9/tests/test_backports.py
--rw-rw-r--   0 runner    (1001) docker     (127)     2583 2024-04-22 21:07:44.000000 blastpipe-2024.0.9/tests/test_fuzz.py
--rw-rw-r--   0 runner    (1001) docker     (127)     1872 2024-04-22 21:07:44.000000 blastpipe-2024.0.9/tests/test_tailcall.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:41:26.224312 blastpipe-2024.1.0/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:34:47.000000 blastpipe-2024.1.0/.github/
+-rw-rw-r--   0 runner    (1001) docker     (127)       56 2024-04-23 22:34:47.000000 blastpipe-2024.1.0/.github/.markdownlint.json
+-rw-rw-r--   0 runner    (1001) docker     (127)      111 2024-04-23 22:34:47.000000 blastpipe-2024.1.0/.github/dependabot.yml
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:34:47.000000 blastpipe-2024.1.0/.github/workflows/
+-rw-rw-r--   0 runner    (1001) docker     (127)     2886 2024-04-23 22:34:47.000000 blastpipe-2024.1.0/.github/workflows/codeql.yml
+-rw-rw-r--   0 runner    (1001) docker     (127)      968 2024-04-23 22:34:47.000000 blastpipe-2024.1.0/.github/workflows/dependency-review.yml
+-rw-rw-r--   0 runner    (1001) docker     (127)     5868 2024-04-23 22:34:47.000000 blastpipe-2024.1.0/.github/workflows/ozi.yml
+-rw-rw-r--   0 runner    (1001) docker     (127)     3060 2024-04-23 22:34:47.000000 blastpipe-2024.1.0/.github/workflows/scorecards.yml
+-rw-rw-r--   0 runner    (1001) docker     (127)     3105 2024-04-23 22:34:47.000000 blastpipe-2024.1.0/.gitignore
+-rw-rw-r--   0 runner    (1001) docker     (127)      309 2024-04-23 22:34:47.000000 blastpipe-2024.1.0/.pre-commit-config.yaml
+-rw-rw-r--   0 runner    (1001) docker     (127)    78145 2024-04-23 22:34:47.000000 blastpipe-2024.1.0/CHANGELOG.md
+-rw-rw-r--   0 runner    (1001) docker     (127)    12501 2024-04-23 22:34:47.000000 blastpipe-2024.1.0/LICENSE.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     2710 2024-04-23 22:34:47.000000 blastpipe-2024.1.0/NOTICE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5477 2024-04-23 22:41:26.224312 blastpipe-2024.1.0/PKG-INFO
+-rw-rw-r--   0 runner    (1001) docker     (127)     4528 2024-04-23 22:34:47.000000 blastpipe-2024.1.0/README.rst
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:34:47.000000 blastpipe-2024.1.0/blastpipe/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1279 2024-04-23 22:34:47.000000 blastpipe-2024.1.0/blastpipe/__init__.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      138 2024-04-23 22:34:47.000000 blastpipe-2024.1.0/blastpipe/__init__.pyi
+-rw-rw-r--   0 runner    (1001) docker     (127)     3202 2024-04-23 22:34:47.000000 blastpipe-2024.1.0/blastpipe/backports.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     1006 2024-04-23 22:34:47.000000 blastpipe-2024.1.0/blastpipe/backports.pyi
+-rw-rw-r--   0 runner    (1001) docker     (127)     1717 2024-04-23 22:34:47.000000 blastpipe-2024.1.0/blastpipe/buffer.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      213 2024-04-23 22:34:47.000000 blastpipe-2024.1.0/blastpipe/buffer.pyi
+-rw-rw-r--   0 runner    (1001) docker     (127)     1762 2024-04-23 22:34:47.000000 blastpipe-2024.1.0/blastpipe/loop.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      331 2024-04-23 22:34:47.000000 blastpipe-2024.1.0/blastpipe/loop.pyi
+-rw-rw-r--   0 runner    (1001) docker     (127)     3316 2024-04-23 22:34:47.000000 blastpipe-2024.1.0/blastpipe/malloc.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      301 2024-04-23 22:34:47.000000 blastpipe-2024.1.0/blastpipe/malloc.pyi
+-rw-rw-r--   0 runner    (1001) docker     (127)     1235 2024-04-23 22:34:47.000000 blastpipe-2024.1.0/blastpipe/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)     1475 2024-04-23 22:34:47.000000 blastpipe-2024.1.0/blastpipe/mixin.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      453 2024-04-23 22:34:47.000000 blastpipe-2024.1.0/blastpipe/mixin.pyi
+-rw-rw-r--   0 runner    (1001) docker     (127)        0 2024-04-23 22:34:47.000000 blastpipe-2024.1.0/blastpipe/py.typed
+-rw-rw-r--   0 runner    (1001) docker     (127)     1865 2024-04-23 22:34:47.000000 blastpipe-2024.1.0/blastpipe/sequence.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      101 2024-04-23 22:34:47.000000 blastpipe-2024.1.0/blastpipe/sequence.pyi
+-rw-rw-r--   0 runner    (1001) docker     (127)     1696 2024-04-23 22:34:47.000000 blastpipe-2024.1.0/blastpipe/tailcall.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      329 2024-04-23 22:34:47.000000 blastpipe-2024.1.0/blastpipe/tailcall.pyi
+-rw-rw-r--   0 runner    (1001) docker     (127)     3291 2024-04-23 22:34:47.000000 blastpipe-2024.1.0/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)     4520 2024-04-23 22:34:47.000000 blastpipe-2024.1.0/meson.options
+-rw-rw-r--   0 runner    (1001) docker     (127)     8329 2024-04-23 22:34:47.000000 blastpipe-2024.1.0/pyproject.toml
+-rw-rw-r--   0 runner    (1001) docker     (127)        0 2024-04-23 22:34:47.000000 blastpipe-2024.1.0/requirements.in
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:34:47.000000 blastpipe-2024.1.0/subprojects/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:34:47.000000 blastpipe-2024.1.0/subprojects/docs/
+-rw-rw-r--   0 runner    (1001) docker     (127)    12501 2024-04-23 22:34:47.000000 blastpipe-2024.1.0/subprojects/docs/LICENSE.txt
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:34:47.000000 blastpipe-2024.1.0/subprojects/docs/_static/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:34:47.000000 blastpipe-2024.1.0/subprojects/docs/_static/css/
+-rw-rw-r--   0 runner    (1001) docker     (127)      767 2024-04-23 22:34:47.000000 blastpipe-2024.1.0/subprojects/docs/_static/css/custom.css
+-rw-rw-r--   0 runner    (1001) docker     (127)      693 2024-04-23 22:34:47.000000 blastpipe-2024.1.0/subprojects/docs/_static/css/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)      633 2024-04-23 22:34:47.000000 blastpipe-2024.1.0/subprojects/docs/_static/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:34:47.000000 blastpipe-2024.1.0/subprojects/docs/_templates/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1033 2024-04-23 22:34:47.000000 blastpipe-2024.1.0/subprojects/docs/_templates/layout.html
+-rw-rw-r--   0 runner    (1001) docker     (127)      694 2024-04-23 22:34:47.000000 blastpipe-2024.1.0/subprojects/docs/_templates/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)      860 2024-04-23 22:34:47.000000 blastpipe-2024.1.0/subprojects/docs/conf.cfg
+-rw-rw-r--   0 runner    (1001) docker     (127)     1751 2024-04-23 22:34:47.000000 blastpipe-2024.1.0/subprojects/docs/index.rst
+-rw-rw-r--   0 runner    (1001) docker     (127)     2680 2024-04-23 22:34:47.000000 blastpipe-2024.1.0/subprojects/docs/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)     2058 2024-04-23 22:34:47.000000 blastpipe-2024.1.0/subprojects/docs/meson.options
+-rw-rw-r--   0 runner    (1001) docker     (127)      121 2024-04-23 22:34:47.000000 blastpipe-2024.1.0/subprojects/ozi.wrap
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:34:47.000000 blastpipe-2024.1.0/tests/
+-rw-rw-r--   0 runner    (1001) docker     (127)      813 2024-04-23 22:34:47.000000 blastpipe-2024.1.0/tests/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)     1219 2024-04-23 22:34:47.000000 blastpipe-2024.1.0/tests/test_backports.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     2583 2024-04-23 22:34:47.000000 blastpipe-2024.1.0/tests/test_fuzz.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     1872 2024-04-23 22:34:47.000000 blastpipe-2024.1.0/tests/test_tailcall.py
```

### Comparing `blastpipe-2024.0.9/.github/workflows/codeql.yml` & `blastpipe-2024.1.0/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.9/.github/workflows/dependency-review.yml` & `blastpipe-2024.1.0/.github/workflows/dependency-review.yml`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.9/.github/workflows/ozi.yml` & `blastpipe-2024.1.0/.github/workflows/ozi.yml`

 * *Files 0% similar despite different names*

```diff
@@ -153,15 +153,15 @@
     name: Generate build provenance
     permissions:
       actions: read # To read the workflow path.
       id-token: write # To sign the provenance.
       contents: write # To add assets to a release.
     # Currently this action needs to be referred by tag. More details at:
     # https://github.com/slsa-framework/slsa-github-generator#verification-of-provenance
-    uses: slsa-framework/slsa-github-generator/.github/workflows/generator_generic_slsa3.yml@v1.10.0
+    uses: slsa-framework/slsa-github-generator/.github/workflows/generator_generic_slsa3.yml@v2.0.0
     with:
       provenance-name: provenance-${{ github.event.repository.name }}-${{ needs.release.outputs.tag }}.intoto.jsonl
       base64-subjects: "${{ needs.release.outputs.hashes }}"
       upload-tag-name: "${{ needs.release.outputs.tag }}"
       upload-assets: true
 
   publish:
```

### Comparing `blastpipe-2024.0.9/.github/workflows/scorecards.yml` & `blastpipe-2024.1.0/.github/workflows/scorecards.yml`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.9/.gitignore` & `blastpipe-2024.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.9/CHANGELOG.md` & `blastpipe-2024.1.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,38 @@
 # CHANGELOG
 
 
 
+## v2024.1.0 (2024-04-23)
+
+### :arrow_up:
+
+* :arrow_up: Bump slsa-framework/slsa-github-generator
+
+Bumps [slsa-framework/slsa-github-generator](https://github.com/slsa-framework/slsa-github-generator) from 1.10.0 to 2.0.0.
+- [Release notes](https://github.com/slsa-framework/slsa-github-generator/releases)
+- [Changelog](https://github.com/slsa-framework/slsa-github-generator/blob/main/CHANGELOG.md)
+- [Commits](https://github.com/slsa-framework/slsa-github-generator/compare/v1.10.0...v2.0.0)
+
+---
+updated-dependencies:
+- dependency-name: slsa-framework/slsa-github-generator
+  dependency-type: direct:production
+  update-type: version-update:semver-major
+...
+
+Signed-off-by: dependabot[bot] &lt;support@github.com&gt; ([`98b3f63`](https://github.com/OZI-Project/blastpipe/commit/98b3f63da24998c356d35d2ffb83db1ab5046995))
+
+### :sparkles:
+
+* :sparkles: Merge pull request #66 from OZI-Project/dependabot/github_actions/slsa-framework/slsa-github-generator-2.0.0
+
+⬆️ Bump slsa-framework/slsa-github-generator from 1.10.0 to 2.0.0 ([`ee91082`](https://github.com/OZI-Project/blastpipe/commit/ee91082a5858f6b9b9b545a683a4977073466489))
+
+
 ## v2024.0.9 (2024-04-22)
 
 ### :arrow_up:
 
 * :arrow_up: Merge pull request #63 from OZI-Project/dependabot/github_actions/OZI-Project/checkpoint-0.1.5
 
 ⬆️ Bump OZI-Project/checkpoint from 0.1.4 to 0.1.5 ([`98bf23f`](https://github.com/OZI-Project/blastpipe/commit/98bf23fd0fb0da343c75239a65790209922c7f4d))
```

### Comparing `blastpipe-2024.0.9/LICENSE.txt` & `blastpipe-2024.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.9/NOTICE.md` & `blastpipe-2024.1.0/NOTICE.md`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.9/PKG-INFO` & `blastpipe-2024.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: blastpipe
-Version: 2024.0.9
+Version: 2024.1.0
 Summary: OZI integrated test library.
 Home-page: https://oziproject.dev
 Author: Eden Ross Duff MSc
 Author-email: help@oziproject.dev
 License: Apache-2.0 WITH LLVM-exception
-Download-URL: https://github.com//blastpipe/archive/refs/tags/2024.0.9.tar.gz
+Download-URL: https://github.com//blastpipe/archive/refs/tags/2024.1.0.tar.gz
 Requires-Python: >=3.10, <3.13
 Keywords: ozi,meson
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Development Status :: 1 - Planning
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `blastpipe-2024.0.9/README.rst` & `blastpipe-2024.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.9/blastpipe/__init__.py` & `blastpipe-2024.1.0/blastpipe/__init__.py`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.9/blastpipe/backports.py` & `blastpipe-2024.1.0/blastpipe/backports.py`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.9/blastpipe/backports.pyi` & `blastpipe-2024.1.0/blastpipe/backports.pyi`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.9/blastpipe/buffer.py` & `blastpipe-2024.1.0/blastpipe/buffer.py`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.9/blastpipe/loop.py` & `blastpipe-2024.1.0/blastpipe/loop.py`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.9/blastpipe/malloc.py` & `blastpipe-2024.1.0/blastpipe/malloc.py`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.9/blastpipe/meson.build` & `blastpipe-2024.1.0/blastpipe/meson.build`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.9/blastpipe/mixin.py` & `blastpipe-2024.1.0/blastpipe/mixin.py`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.9/blastpipe/sequence.py` & `blastpipe-2024.1.0/blastpipe/sequence.py`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.9/blastpipe/tailcall.py` & `blastpipe-2024.1.0/blastpipe/tailcall.py`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.9/meson.build` & `blastpipe-2024.1.0/meson.build`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.9/meson.options` & `blastpipe-2024.1.0/meson.options`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.9/pyproject.toml` & `blastpipe-2024.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.9/subprojects/docs/LICENSE.txt` & `blastpipe-2024.1.0/subprojects/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.9/subprojects/docs/_static/css/custom.css` & `blastpipe-2024.1.0/subprojects/docs/_static/css/custom.css`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.9/subprojects/docs/_static/css/meson.build` & `blastpipe-2024.1.0/subprojects/docs/_static/css/meson.build`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.9/subprojects/docs/_static/meson.build` & `blastpipe-2024.1.0/subprojects/docs/_static/meson.build`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.9/subprojects/docs/_templates/layout.html` & `blastpipe-2024.1.0/subprojects/docs/_templates/layout.html`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.9/subprojects/docs/_templates/meson.build` & `blastpipe-2024.1.0/subprojects/docs/_templates/meson.build`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.9/subprojects/docs/conf.cfg` & `blastpipe-2024.1.0/subprojects/docs/conf.cfg`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.9/subprojects/docs/index.rst` & `blastpipe-2024.1.0/subprojects/docs/index.rst`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.9/subprojects/docs/meson.build` & `blastpipe-2024.1.0/subprojects/docs/meson.build`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.9/subprojects/docs/meson.options` & `blastpipe-2024.1.0/subprojects/docs/meson.options`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.9/tests/meson.build` & `blastpipe-2024.1.0/tests/meson.build`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.9/tests/test_backports.py` & `blastpipe-2024.1.0/tests/test_backports.py`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.9/tests/test_fuzz.py` & `blastpipe-2024.1.0/tests/test_fuzz.py`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.9/tests/test_tailcall.py` & `blastpipe-2024.1.0/tests/test_tailcall.py`

 * *Files identical despite different names*


# Comparing `tmp/blastpipe-2024.1.0.tar.gz` & `tmp/blastpipe-2024.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blastpipe-2024.1.0.tar", last modified: Tue Apr 23 22:41:26 2024, max compression
+gzip compressed data, was "blastpipe-2024.1.1.tar", last modified: Tue Apr 23 23:02:27 2024, max compression
```

## Comparing `blastpipe-2024.1.0.tar` & `blastpipe-2024.1.1.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:41:26.224312 blastpipe-2024.1.0/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:34:47.000000 blastpipe-2024.1.0/.github/
--rw-rw-r--   0 runner    (1001) docker     (127)       56 2024-04-23 22:34:47.000000 blastpipe-2024.1.0/.github/.markdownlint.json
--rw-rw-r--   0 runner    (1001) docker     (127)      111 2024-04-23 22:34:47.000000 blastpipe-2024.1.0/.github/dependabot.yml
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:34:47.000000 blastpipe-2024.1.0/.github/workflows/
--rw-rw-r--   0 runner    (1001) docker     (127)     2886 2024-04-23 22:34:47.000000 blastpipe-2024.1.0/.github/workflows/codeql.yml
--rw-rw-r--   0 runner    (1001) docker     (127)      968 2024-04-23 22:34:47.000000 blastpipe-2024.1.0/.github/workflows/dependency-review.yml
--rw-rw-r--   0 runner    (1001) docker     (127)     5868 2024-04-23 22:34:47.000000 blastpipe-2024.1.0/.github/workflows/ozi.yml
--rw-rw-r--   0 runner    (1001) docker     (127)     3060 2024-04-23 22:34:47.000000 blastpipe-2024.1.0/.github/workflows/scorecards.yml
--rw-rw-r--   0 runner    (1001) docker     (127)     3105 2024-04-23 22:34:47.000000 blastpipe-2024.1.0/.gitignore
--rw-rw-r--   0 runner    (1001) docker     (127)      309 2024-04-23 22:34:47.000000 blastpipe-2024.1.0/.pre-commit-config.yaml
--rw-rw-r--   0 runner    (1001) docker     (127)    78145 2024-04-23 22:34:47.000000 blastpipe-2024.1.0/CHANGELOG.md
--rw-rw-r--   0 runner    (1001) docker     (127)    12501 2024-04-23 22:34:47.000000 blastpipe-2024.1.0/LICENSE.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     2710 2024-04-23 22:34:47.000000 blastpipe-2024.1.0/NOTICE.md
--rw-r--r--   0 runner    (1001) docker     (127)     5477 2024-04-23 22:41:26.224312 blastpipe-2024.1.0/PKG-INFO
--rw-rw-r--   0 runner    (1001) docker     (127)     4528 2024-04-23 22:34:47.000000 blastpipe-2024.1.0/README.rst
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:34:47.000000 blastpipe-2024.1.0/blastpipe/
--rw-rw-r--   0 runner    (1001) docker     (127)     1279 2024-04-23 22:34:47.000000 blastpipe-2024.1.0/blastpipe/__init__.py
--rw-rw-r--   0 runner    (1001) docker     (127)      138 2024-04-23 22:34:47.000000 blastpipe-2024.1.0/blastpipe/__init__.pyi
--rw-rw-r--   0 runner    (1001) docker     (127)     3202 2024-04-23 22:34:47.000000 blastpipe-2024.1.0/blastpipe/backports.py
--rw-rw-r--   0 runner    (1001) docker     (127)     1006 2024-04-23 22:34:47.000000 blastpipe-2024.1.0/blastpipe/backports.pyi
--rw-rw-r--   0 runner    (1001) docker     (127)     1717 2024-04-23 22:34:47.000000 blastpipe-2024.1.0/blastpipe/buffer.py
--rw-rw-r--   0 runner    (1001) docker     (127)      213 2024-04-23 22:34:47.000000 blastpipe-2024.1.0/blastpipe/buffer.pyi
--rw-rw-r--   0 runner    (1001) docker     (127)     1762 2024-04-23 22:34:47.000000 blastpipe-2024.1.0/blastpipe/loop.py
--rw-rw-r--   0 runner    (1001) docker     (127)      331 2024-04-23 22:34:47.000000 blastpipe-2024.1.0/blastpipe/loop.pyi
--rw-rw-r--   0 runner    (1001) docker     (127)     3316 2024-04-23 22:34:47.000000 blastpipe-2024.1.0/blastpipe/malloc.py
--rw-rw-r--   0 runner    (1001) docker     (127)      301 2024-04-23 22:34:47.000000 blastpipe-2024.1.0/blastpipe/malloc.pyi
--rw-rw-r--   0 runner    (1001) docker     (127)     1235 2024-04-23 22:34:47.000000 blastpipe-2024.1.0/blastpipe/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)     1475 2024-04-23 22:34:47.000000 blastpipe-2024.1.0/blastpipe/mixin.py
--rw-rw-r--   0 runner    (1001) docker     (127)      453 2024-04-23 22:34:47.000000 blastpipe-2024.1.0/blastpipe/mixin.pyi
--rw-rw-r--   0 runner    (1001) docker     (127)        0 2024-04-23 22:34:47.000000 blastpipe-2024.1.0/blastpipe/py.typed
--rw-rw-r--   0 runner    (1001) docker     (127)     1865 2024-04-23 22:34:47.000000 blastpipe-2024.1.0/blastpipe/sequence.py
--rw-rw-r--   0 runner    (1001) docker     (127)      101 2024-04-23 22:34:47.000000 blastpipe-2024.1.0/blastpipe/sequence.pyi
--rw-rw-r--   0 runner    (1001) docker     (127)     1696 2024-04-23 22:34:47.000000 blastpipe-2024.1.0/blastpipe/tailcall.py
--rw-rw-r--   0 runner    (1001) docker     (127)      329 2024-04-23 22:34:47.000000 blastpipe-2024.1.0/blastpipe/tailcall.pyi
--rw-rw-r--   0 runner    (1001) docker     (127)     3291 2024-04-23 22:34:47.000000 blastpipe-2024.1.0/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)     4520 2024-04-23 22:34:47.000000 blastpipe-2024.1.0/meson.options
--rw-rw-r--   0 runner    (1001) docker     (127)     8329 2024-04-23 22:34:47.000000 blastpipe-2024.1.0/pyproject.toml
--rw-rw-r--   0 runner    (1001) docker     (127)        0 2024-04-23 22:34:47.000000 blastpipe-2024.1.0/requirements.in
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:34:47.000000 blastpipe-2024.1.0/subprojects/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:34:47.000000 blastpipe-2024.1.0/subprojects/docs/
--rw-rw-r--   0 runner    (1001) docker     (127)    12501 2024-04-23 22:34:47.000000 blastpipe-2024.1.0/subprojects/docs/LICENSE.txt
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:34:47.000000 blastpipe-2024.1.0/subprojects/docs/_static/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:34:47.000000 blastpipe-2024.1.0/subprojects/docs/_static/css/
--rw-rw-r--   0 runner    (1001) docker     (127)      767 2024-04-23 22:34:47.000000 blastpipe-2024.1.0/subprojects/docs/_static/css/custom.css
--rw-rw-r--   0 runner    (1001) docker     (127)      693 2024-04-23 22:34:47.000000 blastpipe-2024.1.0/subprojects/docs/_static/css/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)      633 2024-04-23 22:34:47.000000 blastpipe-2024.1.0/subprojects/docs/_static/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:34:47.000000 blastpipe-2024.1.0/subprojects/docs/_templates/
--rw-rw-r--   0 runner    (1001) docker     (127)     1033 2024-04-23 22:34:47.000000 blastpipe-2024.1.0/subprojects/docs/_templates/layout.html
--rw-rw-r--   0 runner    (1001) docker     (127)      694 2024-04-23 22:34:47.000000 blastpipe-2024.1.0/subprojects/docs/_templates/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)      860 2024-04-23 22:34:47.000000 blastpipe-2024.1.0/subprojects/docs/conf.cfg
--rw-rw-r--   0 runner    (1001) docker     (127)     1751 2024-04-23 22:34:47.000000 blastpipe-2024.1.0/subprojects/docs/index.rst
--rw-rw-r--   0 runner    (1001) docker     (127)     2680 2024-04-23 22:34:47.000000 blastpipe-2024.1.0/subprojects/docs/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)     2058 2024-04-23 22:34:47.000000 blastpipe-2024.1.0/subprojects/docs/meson.options
--rw-rw-r--   0 runner    (1001) docker     (127)      121 2024-04-23 22:34:47.000000 blastpipe-2024.1.0/subprojects/ozi.wrap
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:34:47.000000 blastpipe-2024.1.0/tests/
--rw-rw-r--   0 runner    (1001) docker     (127)      813 2024-04-23 22:34:47.000000 blastpipe-2024.1.0/tests/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)     1219 2024-04-23 22:34:47.000000 blastpipe-2024.1.0/tests/test_backports.py
--rw-rw-r--   0 runner    (1001) docker     (127)     2583 2024-04-23 22:34:47.000000 blastpipe-2024.1.0/tests/test_fuzz.py
--rw-rw-r--   0 runner    (1001) docker     (127)     1872 2024-04-23 22:34:47.000000 blastpipe-2024.1.0/tests/test_tailcall.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:02:27.782684 blastpipe-2024.1.1/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:56:01.000000 blastpipe-2024.1.1/.github/
+-rw-rw-r--   0 runner    (1001) docker     (127)       56 2024-04-23 22:56:01.000000 blastpipe-2024.1.1/.github/.markdownlint.json
+-rw-rw-r--   0 runner    (1001) docker     (127)      111 2024-04-23 22:56:01.000000 blastpipe-2024.1.1/.github/dependabot.yml
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:56:01.000000 blastpipe-2024.1.1/.github/workflows/
+-rw-rw-r--   0 runner    (1001) docker     (127)     2886 2024-04-23 22:56:01.000000 blastpipe-2024.1.1/.github/workflows/codeql.yml
+-rw-rw-r--   0 runner    (1001) docker     (127)      968 2024-04-23 22:56:01.000000 blastpipe-2024.1.1/.github/workflows/dependency-review.yml
+-rw-rw-r--   0 runner    (1001) docker     (127)     5868 2024-04-23 22:56:01.000000 blastpipe-2024.1.1/.github/workflows/ozi.yml
+-rw-rw-r--   0 runner    (1001) docker     (127)     3060 2024-04-23 22:56:01.000000 blastpipe-2024.1.1/.github/workflows/scorecards.yml
+-rw-rw-r--   0 runner    (1001) docker     (127)     3105 2024-04-23 22:56:01.000000 blastpipe-2024.1.1/.gitignore
+-rw-rw-r--   0 runner    (1001) docker     (127)      309 2024-04-23 22:56:01.000000 blastpipe-2024.1.1/.pre-commit-config.yaml
+-rw-rw-r--   0 runner    (1001) docker     (127)    80159 2024-04-23 22:56:01.000000 blastpipe-2024.1.1/CHANGELOG.md
+-rw-rw-r--   0 runner    (1001) docker     (127)    12501 2024-04-23 22:56:01.000000 blastpipe-2024.1.1/LICENSE.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     2710 2024-04-23 22:56:01.000000 blastpipe-2024.1.1/NOTICE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5477 2024-04-23 23:02:27.782684 blastpipe-2024.1.1/PKG-INFO
+-rw-rw-r--   0 runner    (1001) docker     (127)     4528 2024-04-23 22:56:01.000000 blastpipe-2024.1.1/README.rst
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:56:01.000000 blastpipe-2024.1.1/blastpipe/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1279 2024-04-23 22:56:01.000000 blastpipe-2024.1.1/blastpipe/__init__.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      138 2024-04-23 22:56:01.000000 blastpipe-2024.1.1/blastpipe/__init__.pyi
+-rw-rw-r--   0 runner    (1001) docker     (127)     3202 2024-04-23 22:56:01.000000 blastpipe-2024.1.1/blastpipe/backports.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     1006 2024-04-23 22:56:01.000000 blastpipe-2024.1.1/blastpipe/backports.pyi
+-rw-rw-r--   0 runner    (1001) docker     (127)     1717 2024-04-23 22:56:01.000000 blastpipe-2024.1.1/blastpipe/buffer.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      213 2024-04-23 22:56:01.000000 blastpipe-2024.1.1/blastpipe/buffer.pyi
+-rw-rw-r--   0 runner    (1001) docker     (127)     1762 2024-04-23 22:56:01.000000 blastpipe-2024.1.1/blastpipe/loop.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      331 2024-04-23 22:56:01.000000 blastpipe-2024.1.1/blastpipe/loop.pyi
+-rw-rw-r--   0 runner    (1001) docker     (127)     3316 2024-04-23 22:56:01.000000 blastpipe-2024.1.1/blastpipe/malloc.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      301 2024-04-23 22:56:01.000000 blastpipe-2024.1.1/blastpipe/malloc.pyi
+-rw-rw-r--   0 runner    (1001) docker     (127)     1235 2024-04-23 22:56:01.000000 blastpipe-2024.1.1/blastpipe/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)     1475 2024-04-23 22:56:01.000000 blastpipe-2024.1.1/blastpipe/mixin.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      453 2024-04-23 22:56:01.000000 blastpipe-2024.1.1/blastpipe/mixin.pyi
+-rw-rw-r--   0 runner    (1001) docker     (127)        0 2024-04-23 22:56:01.000000 blastpipe-2024.1.1/blastpipe/py.typed
+-rw-rw-r--   0 runner    (1001) docker     (127)     1865 2024-04-23 22:56:01.000000 blastpipe-2024.1.1/blastpipe/sequence.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      101 2024-04-23 22:56:01.000000 blastpipe-2024.1.1/blastpipe/sequence.pyi
+-rw-rw-r--   0 runner    (1001) docker     (127)     1696 2024-04-23 22:56:01.000000 blastpipe-2024.1.1/blastpipe/tailcall.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      329 2024-04-23 22:56:01.000000 blastpipe-2024.1.1/blastpipe/tailcall.pyi
+-rw-rw-r--   0 runner    (1001) docker     (127)     3291 2024-04-23 22:56:01.000000 blastpipe-2024.1.1/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)     4520 2024-04-23 22:56:01.000000 blastpipe-2024.1.1/meson.options
+-rw-rw-r--   0 runner    (1001) docker     (127)     8329 2024-04-23 22:56:01.000000 blastpipe-2024.1.1/pyproject.toml
+-rw-rw-r--   0 runner    (1001) docker     (127)        0 2024-04-23 22:56:01.000000 blastpipe-2024.1.1/requirements.in
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:56:01.000000 blastpipe-2024.1.1/subprojects/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:56:01.000000 blastpipe-2024.1.1/subprojects/docs/
+-rw-rw-r--   0 runner    (1001) docker     (127)    12501 2024-04-23 22:56:01.000000 blastpipe-2024.1.1/subprojects/docs/LICENSE.txt
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:56:01.000000 blastpipe-2024.1.1/subprojects/docs/_static/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:56:01.000000 blastpipe-2024.1.1/subprojects/docs/_static/css/
+-rw-rw-r--   0 runner    (1001) docker     (127)      767 2024-04-23 22:56:01.000000 blastpipe-2024.1.1/subprojects/docs/_static/css/custom.css
+-rw-rw-r--   0 runner    (1001) docker     (127)      693 2024-04-23 22:56:01.000000 blastpipe-2024.1.1/subprojects/docs/_static/css/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)      633 2024-04-23 22:56:01.000000 blastpipe-2024.1.1/subprojects/docs/_static/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:56:01.000000 blastpipe-2024.1.1/subprojects/docs/_templates/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1033 2024-04-23 22:56:01.000000 blastpipe-2024.1.1/subprojects/docs/_templates/layout.html
+-rw-rw-r--   0 runner    (1001) docker     (127)      694 2024-04-23 22:56:01.000000 blastpipe-2024.1.1/subprojects/docs/_templates/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)      860 2024-04-23 22:56:01.000000 blastpipe-2024.1.1/subprojects/docs/conf.cfg
+-rw-rw-r--   0 runner    (1001) docker     (127)     1751 2024-04-23 22:56:01.000000 blastpipe-2024.1.1/subprojects/docs/index.rst
+-rw-rw-r--   0 runner    (1001) docker     (127)     2680 2024-04-23 22:56:01.000000 blastpipe-2024.1.1/subprojects/docs/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)     2058 2024-04-23 22:56:01.000000 blastpipe-2024.1.1/subprojects/docs/meson.options
+-rw-rw-r--   0 runner    (1001) docker     (127)      121 2024-04-23 22:56:01.000000 blastpipe-2024.1.1/subprojects/ozi.wrap
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:56:01.000000 blastpipe-2024.1.1/tests/
+-rw-rw-r--   0 runner    (1001) docker     (127)      813 2024-04-23 22:56:01.000000 blastpipe-2024.1.1/tests/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)     1219 2024-04-23 22:56:01.000000 blastpipe-2024.1.1/tests/test_backports.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     2583 2024-04-23 22:56:01.000000 blastpipe-2024.1.1/tests/test_fuzz.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     1872 2024-04-23 22:56:01.000000 blastpipe-2024.1.1/tests/test_tailcall.py
```

### Comparing `blastpipe-2024.1.0/.github/workflows/codeql.yml` & `blastpipe-2024.1.1/.github/workflows/codeql.yml`

 * *Files 12% similar despite different names*

```diff
@@ -46,33 +46,33 @@
           egress-policy: audit
 
       - name: Checkout repository
         uses: actions/checkout@1d96c772d19495a3b5c517cd2bc0cb401ea0529f # v4.1.3
 
       # Initializes the CodeQL tools for scanning.
       - name: Initialize CodeQL
-        uses: github/codeql-action/init@c7f9125735019aa87cfc361530512d50ea439c71 # v3.25.1
+        uses: github/codeql-action/init@8f596b4ae3cb3c588a5c46780b86dd53fef16c52 # v3.25.2
         with:
           languages: ${{ matrix.language }}
           # If you wish to specify custom queries, you can do so here or in a config file.
           # By default, queries listed here will override any specified in a config file.
           # Prefix the list here with "+" to use these queries and those in the config file.
 
       # Autobuild attempts to build any compiled languages  (C/C++, C#, or Java).
       # If this step fails, then you should remove it and run the build manually (see below)
       - name: Autobuild
-        uses: github/codeql-action/autobuild@c7f9125735019aa87cfc361530512d50ea439c71 # v3.25.1
+        uses: github/codeql-action/autobuild@8f596b4ae3cb3c588a5c46780b86dd53fef16c52 # v3.25.2
 
       # ℹ️ Command-line programs to run using the OS shell.
       # 📚 See https://docs.github.com/en/actions/using-workflows/workflow-syntax-for-github-actions#jobsjob_idstepsrun
 
       #   If the Autobuild fails above, remove it and uncomment the following three lines.
       #   modify them (or add more) to build your code if your project, please refer to the EXAMPLE below for guidance.
 
       # - run: |
       #   echo "Run, Build Application using script"
       #   ./location_of_script_within_repo/buildscript.sh
 
       - name: Perform CodeQL Analysis
-        uses: github/codeql-action/analyze@c7f9125735019aa87cfc361530512d50ea439c71 # v3.25.1
+        uses: github/codeql-action/analyze@8f596b4ae3cb3c588a5c46780b86dd53fef16c52 # v3.25.2
         with:
           category: "/language:${{matrix.language}}"
```

### Comparing `blastpipe-2024.1.0/.github/workflows/dependency-review.yml` & `blastpipe-2024.1.1/.github/workflows/dependency-review.yml`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.1.0/.github/workflows/ozi.yml` & `blastpipe-2024.1.1/.github/workflows/ozi.yml`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.1.0/.github/workflows/scorecards.yml` & `blastpipe-2024.1.1/.github/workflows/scorecards.yml`

 * *Files 10% similar despite different names*

```diff
@@ -59,18 +59,18 @@
           #   - `publish_results` will always be set to `false`, regardless
           #     of the value entered here.
           publish_results: true
 
       # Upload the results as artifacts (optional). Commenting out will disable uploads of run results in SARIF
       # format to the repository Actions tab.
       - name: "Upload artifact"
-        uses: actions/upload-artifact@1746f4ab65b179e0ea60a494b83293b640dd5bba # v4.3.2
+        uses: actions/upload-artifact@65462800fd760344b1a7b4382951275a0abb4808 # v4.3.3
         with:
           name: SARIF file
           path: results.sarif
           retention-days: 5
 
       # Upload the results to GitHub's code scanning dashboard.
       - name: "Upload to code-scanning"
-        uses: github/codeql-action/upload-sarif@c7f9125735019aa87cfc361530512d50ea439c71 # v3.25.1
+        uses: github/codeql-action/upload-sarif@8f596b4ae3cb3c588a5c46780b86dd53fef16c52 # v3.25.2
         with:
           sarif_file: results.sarif
```

### Comparing `blastpipe-2024.1.0/.gitignore` & `blastpipe-2024.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.1.0/CHANGELOG.md` & `blastpipe-2024.1.1/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,24 @@
 # CHANGELOG
 
 
 
+## v2024.1.1 (2024-04-23)
+
+### Other
+
+* Merge pull request #64 from OZI-Project/dependabot/github_actions/github/codeql-action-3.25.2
+
+⬆️ Bump github/codeql-action from 3.25.1 to 3.25.2 ([`255087f`](https://github.com/OZI-Project/blastpipe/commit/255087fafe7964594fa485f2b046ae527560a62c))
+
+* Merge pull request #65 from OZI-Project/dependabot/github_actions/actions/upload-artifact-4.3.3
+
+⬆️ Bump actions/upload-artifact from 4.3.2 to 4.3.3 ([`d2f54ab`](https://github.com/OZI-Project/blastpipe/commit/d2f54ab7ed2f5a37d2b432fbd2f6fbf1805d3e3d))
+
+
 ## v2024.1.0 (2024-04-23)
 
 ### :arrow_up:
 
 * :arrow_up: Bump slsa-framework/slsa-github-generator
 
 Bumps [slsa-framework/slsa-github-generator](https://github.com/slsa-framework/slsa-github-generator) from 1.10.0 to 2.0.0.
@@ -18,14 +31,45 @@
 - dependency-name: slsa-framework/slsa-github-generator
   dependency-type: direct:production
   update-type: version-update:semver-major
 ...
 
 Signed-off-by: dependabot[bot] &lt;support@github.com&gt; ([`98b3f63`](https://github.com/OZI-Project/blastpipe/commit/98b3f63da24998c356d35d2ffb83db1ab5046995))
 
+* :arrow_up: Bump actions/upload-artifact from 4.3.2 to 4.3.3
+
+Bumps [actions/upload-artifact](https://github.com/actions/upload-artifact) from 4.3.2 to 4.3.3.
+- [Release notes](https://github.com/actions/upload-artifact/releases)
+- [Commits](https://github.com/actions/upload-artifact/compare/1746f4ab65b179e0ea60a494b83293b640dd5bba...65462800fd760344b1a7b4382951275a0abb4808)
+
+---
+updated-dependencies:
+- dependency-name: actions/upload-artifact
+  dependency-type: direct:production
+  update-type: version-update:semver-patch
+...
+
+Signed-off-by: dependabot[bot] &lt;support@github.com&gt; ([`df59855`](https://github.com/OZI-Project/blastpipe/commit/df59855b192e4c465ac1e452539bb1a1ea44c54f))
+
+* :arrow_up: Bump github/codeql-action from 3.25.1 to 3.25.2
+
+Bumps [github/codeql-action](https://github.com/github/codeql-action) from 3.25.1 to 3.25.2.
+- [Release notes](https://github.com/github/codeql-action/releases)
+- [Changelog](https://github.com/github/codeql-action/blob/main/CHANGELOG.md)
+- [Commits](https://github.com/github/codeql-action/compare/c7f9125735019aa87cfc361530512d50ea439c71...8f596b4ae3cb3c588a5c46780b86dd53fef16c52)
+
+---
+updated-dependencies:
+- dependency-name: github/codeql-action
+  dependency-type: direct:production
+  update-type: version-update:semver-patch
+...
+
+Signed-off-by: dependabot[bot] &lt;support@github.com&gt; ([`e119b2e`](https://github.com/OZI-Project/blastpipe/commit/e119b2e997ad0e70068fd99ea5dc72fcb2f9dced))
+
 ### :sparkles:
 
 * :sparkles: Merge pull request #66 from OZI-Project/dependabot/github_actions/slsa-framework/slsa-github-generator-2.0.0
 
 ⬆️ Bump slsa-framework/slsa-github-generator from 1.10.0 to 2.0.0 ([`ee91082`](https://github.com/OZI-Project/blastpipe/commit/ee91082a5858f6b9b9b545a683a4977073466489))
```

### Comparing `blastpipe-2024.1.0/LICENSE.txt` & `blastpipe-2024.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.1.0/NOTICE.md` & `blastpipe-2024.1.1/NOTICE.md`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.1.0/PKG-INFO` & `blastpipe-2024.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: blastpipe
-Version: 2024.1.0
+Version: 2024.1.1
 Summary: OZI integrated test library.
 Home-page: https://oziproject.dev
 Author: Eden Ross Duff MSc
 Author-email: help@oziproject.dev
 License: Apache-2.0 WITH LLVM-exception
-Download-URL: https://github.com//blastpipe/archive/refs/tags/2024.1.0.tar.gz
+Download-URL: https://github.com//blastpipe/archive/refs/tags/2024.1.1.tar.gz
 Requires-Python: >=3.10, <3.13
 Keywords: ozi,meson
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Development Status :: 1 - Planning
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `blastpipe-2024.1.0/README.rst` & `blastpipe-2024.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.1.0/blastpipe/__init__.py` & `blastpipe-2024.1.1/blastpipe/__init__.py`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.1.0/blastpipe/backports.py` & `blastpipe-2024.1.1/blastpipe/backports.py`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.1.0/blastpipe/backports.pyi` & `blastpipe-2024.1.1/blastpipe/backports.pyi`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.1.0/blastpipe/buffer.py` & `blastpipe-2024.1.1/blastpipe/buffer.py`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.1.0/blastpipe/loop.py` & `blastpipe-2024.1.1/blastpipe/loop.py`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.1.0/blastpipe/malloc.py` & `blastpipe-2024.1.1/blastpipe/malloc.py`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.1.0/blastpipe/meson.build` & `blastpipe-2024.1.1/blastpipe/meson.build`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.1.0/blastpipe/mixin.py` & `blastpipe-2024.1.1/blastpipe/mixin.py`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.1.0/blastpipe/sequence.py` & `blastpipe-2024.1.1/blastpipe/sequence.py`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.1.0/blastpipe/tailcall.py` & `blastpipe-2024.1.1/blastpipe/tailcall.py`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.1.0/meson.build` & `blastpipe-2024.1.1/meson.build`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.1.0/meson.options` & `blastpipe-2024.1.1/meson.options`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.1.0/pyproject.toml` & `blastpipe-2024.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.1.0/subprojects/docs/LICENSE.txt` & `blastpipe-2024.1.1/subprojects/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.1.0/subprojects/docs/_static/css/custom.css` & `blastpipe-2024.1.1/subprojects/docs/_static/css/custom.css`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.1.0/subprojects/docs/_static/css/meson.build` & `blastpipe-2024.1.1/subprojects/docs/_static/css/meson.build`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.1.0/subprojects/docs/_static/meson.build` & `blastpipe-2024.1.1/subprojects/docs/_static/meson.build`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.1.0/subprojects/docs/_templates/layout.html` & `blastpipe-2024.1.1/subprojects/docs/_templates/layout.html`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.1.0/subprojects/docs/_templates/meson.build` & `blastpipe-2024.1.1/subprojects/docs/_templates/meson.build`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.1.0/subprojects/docs/conf.cfg` & `blastpipe-2024.1.1/subprojects/docs/conf.cfg`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.1.0/subprojects/docs/index.rst` & `blastpipe-2024.1.1/subprojects/docs/index.rst`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.1.0/subprojects/docs/meson.build` & `blastpipe-2024.1.1/subprojects/docs/meson.build`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.1.0/subprojects/docs/meson.options` & `blastpipe-2024.1.1/subprojects/docs/meson.options`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.1.0/tests/meson.build` & `blastpipe-2024.1.1/tests/meson.build`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.1.0/tests/test_backports.py` & `blastpipe-2024.1.1/tests/test_backports.py`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.1.0/tests/test_fuzz.py` & `blastpipe-2024.1.1/tests/test_fuzz.py`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.1.0/tests/test_tailcall.py` & `blastpipe-2024.1.1/tests/test_tailcall.py`

 * *Files identical despite different names*


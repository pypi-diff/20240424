# Comparing `tmp/tclint-0.2.3.tar.gz` & `tmp/tclint-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tclint-0.2.3.tar", last modified: Mon Apr  1 21:49:47 2024, max compression
+gzip compressed data, was "tclint-0.2.4.tar", last modified: Wed Apr 24 03:21:02 2024, max compression
```

## Comparing `tclint-0.2.3.tar` & `tclint-0.2.4.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:49:47.755031 tclint-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-01 21:49:44.000000 tclint-0.2.3/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:49:47.747031 tclint-0.2.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:49:47.747031 tclint-0.2.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-04-01 21:49:44.000000 tclint-0.2.3/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-04-01 21:49:44.000000 tclint-0.2.3/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-01 21:49:44.000000 tclint-0.2.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-04-01 21:49:44.000000 tclint-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3379 2024-04-01 21:49:47.755031 tclint-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2799 2024-04-01 21:49:44.000000 tclint-0.2.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-01 21:49:44.000000 tclint-0.2.3/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-01 21:49:44.000000 tclint-0.2.3/dev-constraints.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:49:47.747031 tclint-0.2.3/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     4568 2024-04-01 21:49:44.000000 tclint-0.2.3/docs/configuration.md
--rw-r--r--   0 runner    (1001) docker     (127)     5211 2024-04-01 21:49:44.000000 tclint-0.2.3/docs/violations.md
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-01 21:49:44.000000 tclint-0.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 21:49:47.755031 tclint-0.2.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:49:47.747031 tclint-0.2.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:49:47.751031 tclint-0.2.3/src/tclint/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 21:49:44.000000 tclint-0.2.3/src/tclint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-01 21:49:47.000000 tclint-0.2.3/src/tclint/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    25942 2024-04-01 21:49:44.000000 tclint-0.2.3/src/tclint/checks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:49:47.751031 tclint-0.2.3/src/tclint/commands/
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-04-01 21:49:44.000000 tclint-0.2.3/src/tclint/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25927 2024-04-01 21:49:44.000000 tclint-0.2.3/src/tclint/commands/builtin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-04-01 21:49:44.000000 tclint-0.2.3/src/tclint/commands/plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)     4109 2024-04-01 21:49:44.000000 tclint-0.2.3/src/tclint/commands/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3019 2024-04-01 21:49:44.000000 tclint-0.2.3/src/tclint/comments.py
--rw-r--r--   0 runner    (1001) docker     (127)    11979 2024-04-01 21:49:44.000000 tclint-0.2.3/src/tclint/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4691 2024-04-01 21:49:44.000000 tclint-0.2.3/src/tclint/lexer.py
--rw-r--r--   0 runner    (1001) docker     (127)    27503 2024-04-01 21:49:44.000000 tclint-0.2.3/src/tclint/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)    10322 2024-04-01 21:49:44.000000 tclint-0.2.3/src/tclint/syntax_tree.py
--rw-r--r--   0 runner    (1001) docker     (127)     7122 2024-04-01 21:49:44.000000 tclint-0.2.3/src/tclint/tclint.py
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-04-01 21:49:44.000000 tclint-0.2.3/src/tclint/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-04-01 21:49:44.000000 tclint-0.2.3/src/tclint/violations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:49:47.755031 tclint-0.2.3/src/tclint.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3379 2024-04-01 21:49:47.000000 tclint-0.2.3/src/tclint.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-04-01 21:49:47.000000 tclint-0.2.3/src/tclint.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 21:49:47.000000 tclint-0.2.3/src/tclint.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-01 21:49:47.000000 tclint-0.2.3/src/tclint.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-01 21:49:47.000000 tclint-0.2.3/src/tclint.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-01 21:49:47.000000 tclint-0.2.3/src/tclint.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:49:47.751031 tclint-0.2.3/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:49:47.755031 tclint-0.2.3/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-01 21:49:44.000000 tclint-0.2.3/tests/data/backslash-spacing.tcl
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-01 21:49:44.000000 tclint-0.2.3/tests/data/backslash-spacing.txt
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-04-01 21:49:44.000000 tclint-0.2.3/tests/data/blank-lines.tcl
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-01 21:49:44.000000 tclint-0.2.3/tests/data/blank-lines.txt
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-01 21:49:44.000000 tclint-0.2.3/tests/data/clean.tcl
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 21:49:44.000000 tclint-0.2.3/tests/data/clean.txt
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-01 21:49:44.000000 tclint-0.2.3/tests/data/dirty.tcl
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-04-01 21:49:44.000000 tclint-0.2.3/tests/data/dirty.txt
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-01 21:49:44.000000 tclint-0.2.3/tests/data/example.tcl
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-01 21:49:44.000000 tclint-0.2.3/tests/data/example.txt
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-01 21:49:44.000000 tclint-0.2.3/tests/data/expr-format.tcl
--rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-01 21:49:44.000000 tclint-0.2.3/tests/data/expr-format.txt
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-01 21:49:44.000000 tclint-0.2.3/tests/data/indent.tcl
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-01 21:49:44.000000 tclint-0.2.3/tests/data/indent.txt
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-04-01 21:49:44.000000 tclint-0.2.3/tests/data/indent_lists.tcl
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-01 21:49:44.000000 tclint-0.2.3/tests/data/indent_lists.txt
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-01 21:49:44.000000 tclint-0.2.3/tests/data/lines.tcl
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-01 21:49:44.000000 tclint-0.2.3/tests/data/lines.txt
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-01 21:49:44.000000 tclint-0.2.3/tests/data/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-01 21:49:44.000000 tclint-0.2.3/tests/data/spaces-in-braces.tcl
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-01 21:49:44.000000 tclint-0.2.3/tests/data/spaces-in-braces.toml
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-01 21:49:44.000000 tclint-0.2.3/tests/data/spaces-in-braces.txt
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-01 21:49:44.000000 tclint-0.2.3/tests/data/special-comments.tcl
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 21:49:44.000000 tclint-0.2.3/tests/data/special-comments.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-01 21:49:44.000000 tclint-0.2.3/tests/data/tclint.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-04-01 21:49:44.000000 tclint-0.2.3/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2930 2024-04-01 21:49:44.000000 tclint-0.2.3/tests/test_lint.py
--rw-r--r--   0 runner    (1001) docker     (127)    17815 2024-04-01 21:49:44.000000 tclint-0.2.3/tests/test_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     5594 2024-04-01 21:49:44.000000 tclint-0.2.3/tests/test_tclint.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:02.636049 tclint-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-24 03:20:54.000000 tclint-0.2.4/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:02.624049 tclint-0.2.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:02.624049 tclint-0.2.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-04-24 03:20:54.000000 tclint-0.2.4/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-04-24 03:20:54.000000 tclint-0.2.4/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-24 03:20:54.000000 tclint-0.2.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-04-24 03:20:54.000000 tclint-0.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3428 2024-04-24 03:21:02.636049 tclint-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-04-24 03:20:54.000000 tclint-0.2.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-24 03:20:54.000000 tclint-0.2.4/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-24 03:20:54.000000 tclint-0.2.4/dev-constraints.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:02.628049 tclint-0.2.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     4733 2024-04-24 03:20:54.000000 tclint-0.2.4/docs/configuration.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5211 2024-04-24 03:20:54.000000 tclint-0.2.4/docs/violations.md
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-04-24 03:20:54.000000 tclint-0.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 03:21:02.636049 tclint-0.2.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:02.624049 tclint-0.2.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:02.628049 tclint-0.2.4/src/tclint/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 03:20:54.000000 tclint-0.2.4/src/tclint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-24 03:21:02.000000 tclint-0.2.4/src/tclint/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25942 2024-04-24 03:20:54.000000 tclint-0.2.4/src/tclint/checks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:02.632049 tclint-0.2.4/src/tclint/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)      820 2024-04-24 03:20:54.000000 tclint-0.2.4/src/tclint/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25927 2024-04-24 03:20:54.000000 tclint-0.2.4/src/tclint/commands/builtin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3260 2024-04-24 03:20:54.000000 tclint-0.2.4/src/tclint/commands/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4109 2024-04-24 03:20:54.000000 tclint-0.2.4/src/tclint/commands/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3019 2024-04-24 03:20:54.000000 tclint-0.2.4/src/tclint/comments.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12392 2024-04-24 03:20:54.000000 tclint-0.2.4/src/tclint/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4691 2024-04-24 03:20:54.000000 tclint-0.2.4/src/tclint/lexer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27503 2024-04-24 03:20:54.000000 tclint-0.2.4/src/tclint/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10322 2024-04-24 03:20:54.000000 tclint-0.2.4/src/tclint/syntax_tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7207 2024-04-24 03:20:54.000000 tclint-0.2.4/src/tclint/tclint.py
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-04-24 03:20:54.000000 tclint-0.2.4/src/tclint/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-04-24 03:20:54.000000 tclint-0.2.4/src/tclint/violations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:02.636049 tclint-0.2.4/src/tclint.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3428 2024-04-24 03:21:02.000000 tclint-0.2.4/src/tclint.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-04-24 03:21:02.000000 tclint-0.2.4/src/tclint.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 03:21:02.000000 tclint-0.2.4/src/tclint.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-24 03:21:02.000000 tclint-0.2.4/src/tclint.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-24 03:21:02.000000 tclint-0.2.4/src/tclint.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-24 03:21:02.000000 tclint-0.2.4/src/tclint.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:02.632049 tclint-0.2.4/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:02.636049 tclint-0.2.4/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-24 03:20:54.000000 tclint-0.2.4/tests/data/backslash-spacing.tcl
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-24 03:20:54.000000 tclint-0.2.4/tests/data/backslash-spacing.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-04-24 03:20:54.000000 tclint-0.2.4/tests/data/blank-lines.tcl
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-24 03:20:54.000000 tclint-0.2.4/tests/data/blank-lines.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-24 03:20:54.000000 tclint-0.2.4/tests/data/clean.tcl
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 03:20:54.000000 tclint-0.2.4/tests/data/clean.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-24 03:20:54.000000 tclint-0.2.4/tests/data/dirty.tcl
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-04-24 03:20:54.000000 tclint-0.2.4/tests/data/dirty.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-24 03:20:54.000000 tclint-0.2.4/tests/data/example.tcl
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-24 03:20:54.000000 tclint-0.2.4/tests/data/example.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-24 03:20:54.000000 tclint-0.2.4/tests/data/expr-format.tcl
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-24 03:20:54.000000 tclint-0.2.4/tests/data/expr-format.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-24 03:20:54.000000 tclint-0.2.4/tests/data/indent.tcl
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-24 03:20:54.000000 tclint-0.2.4/tests/data/indent.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-04-24 03:20:54.000000 tclint-0.2.4/tests/data/indent_lists.tcl
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-24 03:20:54.000000 tclint-0.2.4/tests/data/indent_lists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-24 03:20:54.000000 tclint-0.2.4/tests/data/lines.tcl
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-24 03:20:54.000000 tclint-0.2.4/tests/data/lines.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-24 03:20:54.000000 tclint-0.2.4/tests/data/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-24 03:20:54.000000 tclint-0.2.4/tests/data/spaces-in-braces.tcl
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-24 03:20:54.000000 tclint-0.2.4/tests/data/spaces-in-braces.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-24 03:20:54.000000 tclint-0.2.4/tests/data/spaces-in-braces.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-24 03:20:54.000000 tclint-0.2.4/tests/data/special-comments.tcl
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 03:20:54.000000 tclint-0.2.4/tests/data/special-comments.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-04-24 03:20:54.000000 tclint-0.2.4/tests/data/tclint.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-04-24 03:20:54.000000 tclint-0.2.4/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2930 2024-04-24 03:20:54.000000 tclint-0.2.4/tests/test_lint.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17815 2024-04-24 03:20:54.000000 tclint-0.2.4/tests/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6390 2024-04-24 03:20:54.000000 tclint-0.2.4/tests/test_tclint.py
```

### Comparing `tclint-0.2.3/.github/workflows/ci.yml` & `tclint-0.2.4/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `tclint-0.2.3/.github/workflows/release.yml` & `tclint-0.2.4/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `tclint-0.2.3/LICENSE` & `tclint-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `tclint-0.2.3/PKG-INFO` & `tclint-0.2.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: tclint
-Version: 0.2.3
+Version: 0.2.4
 Summary: A CLI utility for linting and analyzing Tcl code.
 Author-email: Noah Moroze <me@noahmoroze.com>
 License: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: ply==3.11
 Requires-Dist: schema==0.7.5
 Requires-Dist: tomli~=2.0.1; python_version < "3.11"
 Requires-Dist: pathspec==0.11.2
+Requires-Dist: importlib-metadata==6.8.0
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: flake8; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-timeout; extra == "dev"
 
 # tclint &nbsp; [![CI](https://github.com/nmoroze/tclint/actions/workflows/ci.yml/badge.svg)](https://github.com/nmoroze/tclint/actions/workflows/ci.yml)
@@ -60,15 +61,15 @@
 example.tcl:1:1: too many args to puts: got 4, expected no more than 3 [command-args]
 example.tcl:2:1: expected indent of 0 spaces, got 2 [indent]
 example.tcl:3:5: expected 1 space between words, got 3 [spacing]
 ```
 
 ## Usage
 
-`tclint` is a command-line utility. It takes a list of paths as positional arguments, which may either be direct paths to source files, or directories which will be recursively searched for files ending in `.tcl`, `.sdc`, or `.xdc`.
+`tclint` is a command-line utility. It takes a list of paths as positional arguments, which may either be direct paths to source files, or directories which will be recursively searched for files ending in `.tcl`, `.sdc`, `.xdc`, or `.upf`.
 
 Collected files will be checked for lint violations.  See the
 [Violations](docs/violations.md) documentation page for a description of all
 lint violations `tclint` may report.
 
 Aspects of `tclint`'s behavior can be controlled by a configuration file. By default, `tclint` will look for a file named `tclint.toml` or `.tclint` in the current working directory (in that order), but a path to an alternate configuration file can be provided using the `-c` or `--config` flag. See [Configuration](docs/configuration.md) for documentation on the configuration file.
```

### Comparing `tclint-0.2.3/README.md` & `tclint-0.2.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 example.tcl:1:1: too many args to puts: got 4, expected no more than 3 [command-args]
 example.tcl:2:1: expected indent of 0 spaces, got 2 [indent]
 example.tcl:3:5: expected 1 space between words, got 3 [spacing]
 ```
 
 ## Usage
 
-`tclint` is a command-line utility. It takes a list of paths as positional arguments, which may either be direct paths to source files, or directories which will be recursively searched for files ending in `.tcl`, `.sdc`, or `.xdc`.
+`tclint` is a command-line utility. It takes a list of paths as positional arguments, which may either be direct paths to source files, or directories which will be recursively searched for files ending in `.tcl`, `.sdc`, `.xdc`, or `.upf`.
 
 Collected files will be checked for lint violations.  See the
 [Violations](docs/violations.md) documentation page for a description of all
 lint violations `tclint` may report.
 
 Aspects of `tclint`'s behavior can be controlled by a configuration file. By default, `tclint` will look for a file named `tclint.toml` or `.tclint` in the current working directory (in that order), but a path to an alternate configuration file can be provided using the `-c` or `--config` flag. See [Configuration](docs/configuration.md) for documentation on the configuration file.
```

### Comparing `tclint-0.2.3/docs/configuration.md` & `tclint-0.2.4/docs/configuration.md`

 * *Files 3% similar despite different names*

```diff
@@ -11,14 +11,17 @@
 exclude = ["ignore_me/", "ignore*.tcl", "/ignore_from_here"]
 # lint violations to ignore. defaults to empty list.
 # can also supply an inline table with a path and a list of violations to ignore under that path.
 ignore = [
     "spacing",
     { path = "files_with_bad_indent/", rules = ["indent"] }
 ]
+# extensions of files to lint when searching directories. defaults to tcl, sdc,
+# xdc, and upf.
+extensions = ["tcl"]
 
 [style]
 # number of spaces to indent. can also be set to "tab". defaults to 4.
 indent = 2
 # maximum allowed line length. defaults to 80.
 line-length = 100
 # maximum allowed number of consecutive blank lines. defaults to 2.
@@ -30,15 +33,15 @@
 # whether to expect a single space (true) or no spaces (false) surrounding the contents of a braced expression or script argument.
 # defaults to false.
 spaces-in-braces = true
 ```
 
 ## Filesets
 
-The configuration file can define an arbitrary number of sub-configurations that apply to a specific set of paths. These sub-configs support the same set of fields as the global configuration, with the exception of `exclude`.
+The configuration file can define an arbitrary number of sub-configurations that apply to a specific set of paths. These sub-configs support the same set of fields as the global configuration, with the exception of `exclude` and `extensions`.
 
 The following example shows how to add two fileset sub-configs that each override different configuration fields:
 
 ```toml
 [[fileset]]
 paths = ["other_file_group1/"]
 ignore = ["command-args"]
@@ -61,14 +64,15 @@
 
 ```
 configuration arguments:
   --ignore "rule1, rule2, ..."
   --extend-ignore "rule1, rule2, ..."
   --exclude "pattern1, pattern2, ..."
   --extend-exclude "pattern1, pattern2, ..."
+  --extensions "tcl, xdc, ..."
   --style-indent <indent>
   --style-line-length <line_length>
   --style-max-blank-lines <max_blank_lines>
   --style-aligned-sets
   --style-no-aligned-sets
   --style-indent-namespace-eval
   --style-no-indent-namespace-eval
```

### Comparing `tclint-0.2.3/docs/violations.md` & `tclint-0.2.4/docs/violations.md`

 * *Files identical despite different names*

### Comparing `tclint-0.2.3/pyproject.toml` & `tclint-0.2.4/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -12,15 +12,16 @@
 ]
 readme = "README.md"
 requires-python = ">=3.8"
 dependencies = [
     "ply==3.11",
     "schema==0.7.5",
     "tomli~=2.0.1; python_version < '3.11'",
-    "pathspec==0.11.2"
+    "pathspec==0.11.2",
+    "importlib-metadata==6.8.0",
 ]
 
 [project.optional-dependencies]
 dev = [
     "black",
     "flake8",
     "pytest",
```

### Comparing `tclint-0.2.3/src/tclint/checks.py` & `tclint-0.2.4/src/tclint/checks.py`

 * *Files identical despite different names*

### Comparing `tclint-0.2.3/src/tclint/commands/builtin.py` & `tclint-0.2.4/src/tclint/commands/builtin.py`

 * *Files identical despite different names*

### Comparing `tclint-0.2.3/src/tclint/commands/utils.py` & `tclint-0.2.4/src/tclint/commands/utils.py`

 * *Files identical despite different names*

### Comparing `tclint-0.2.3/src/tclint/comments.py` & `tclint-0.2.4/src/tclint/comments.py`

 * *Files identical despite different names*

### Comparing `tclint-0.2.3/src/tclint/config.py` & `tclint-0.2.4/src/tclint/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,14 +24,17 @@
     The type annotations defined here are fairly loose - more specific type
     validation (and normalization) is defined by `validators` below.
     """
 
     exclude: List[Any] = dataclasses.field(default_factory=list)
     ignore: List[Any] = dataclasses.field(default_factory=list)
     command_plugins: List[str] = dataclasses.field(default_factory=list)
+    extensions: List[str] = dataclasses.field(
+        default_factory=lambda: ["tcl", "sdc", "xdc", "upf"]
+    )
     style_indent: Union[str, int] = dataclasses.field(default=4)
     style_line_length: int = dataclasses.field(default=80)
     style_allow_aligned_sets: bool = dataclasses.field(default=False)
     style_max_blank_lines: int = dataclasses.field(default=2)
     style_indent_namespace_eval: bool = dataclasses.field(default=True)
     style_spaces_in_braces: bool = dataclasses.field(default=False)
 
@@ -89,14 +92,15 @@
                         )
                     ],
                 },
             )
         ],
     ),
     "command_plugins": Use(validate_command_plugins),
+    "extensions": Use(_str2list),
     "style_indent": Or(
         lambda v: v == "tab", Use(int), error="indent must be integer or 'tab'"
     ),
     "style_line_length": Use(int, error="line-length must be integer"),
     "style_allow_aligned_sets": Use(bool, error="allow-aligned-sets must be a bool"),
     "style_max_blank_lines": And(
         Use(int),
@@ -129,16 +133,17 @@
                 "style_indent_namespace_eval"
             ],
             Optional("spaces-in-braces"): _VALIDATORS["style_spaces_in_braces"],
         },
     }
 
     schema = Schema({
-        # exclude is special - only has meaning in global context
+        # exclude and extensions can only be used in global context
         Optional("exclude"): _VALIDATORS["exclude"],
+        Optional("extensions"): _VALIDATORS["extensions"],
         **base_config,
         Optional("fileset"): Schema([{"paths": [Use(pathlib.Path)], **base_config}]),
     })
 
     try:
         return schema.validate(config)
     except SchemaError as e:
@@ -181,14 +186,17 @@
     config_group.add_argument(
         "--exclude", type=validator("exclude"), metavar='"path1, path2, ..."'
     )
     config_group.add_argument(
         "--extend-exclude", type=validator("exclude"), metavar='"path1, path2, ..."'
     )
     config_group.add_argument(
+        "--extensions", type=validator("extensions"), metavar='"tcl, xdc, ..."'
+    )
+    config_group.add_argument(
         "--style-indent", type=validator("style_indent"), metavar="<indent>"
     )
     config_group.add_argument(
         "--style-line-length",
         type=validator("style_line_length"),
         metavar="<line_length>",
     )
@@ -248,14 +256,18 @@
         if fileset_configs is not None:
             self._fileset_configs = fileset_configs
 
     @property
     def exclude(self):
         return self._global_config.exclude
 
+    @property
+    def extensions(self):
+        return self._global_config.extensions
+
     @classmethod
     def from_dict(cls, config_dict: dict):
         config_dict = _validate_config(config_dict)
         try:
             fileset_config_dicts = config_dict.pop("fileset")
         except KeyError:
             fileset_config_dicts = []
```

### Comparing `tclint-0.2.3/src/tclint/lexer.py` & `tclint-0.2.4/src/tclint/lexer.py`

 * *Files identical despite different names*

### Comparing `tclint-0.2.3/src/tclint/parser.py` & `tclint-0.2.4/src/tclint/parser.py`

 * *Files identical despite different names*

### Comparing `tclint-0.2.3/src/tclint/syntax_tree.py` & `tclint-0.2.4/src/tclint/syntax_tree.py`

 * *Files identical despite different names*

### Comparing `tclint-0.2.3/src/tclint/tclint.py` & `tclint-0.2.4/src/tclint/tclint.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,30 +26,30 @@
 EXIT_OK = 0
 EXIT_LINT_VIOLATIONS = 1
 EXIT_SYNTAX_ERROR = 2
 EXIT_INPUT_ERROR = 4
 
 
 def resolve_sources(
-    paths: List[pathlib.Path], exclude_patterns: List[str], exclude_root: pathlib.Path
+    paths: List[pathlib.Path],
+    exclude_patterns: List[str],
+    exclude_root: pathlib.Path,
+    extensions: List[str],
 ) -> List[Optional[pathlib.Path]]:
     """Resolves paths passed via CLI to a list of filepaths to lint.
 
     `paths` is a list of paths that may be files or directories. Files are
     returned verbatim if they exist, and directories are recursively searched
-    for files that have the extension .tcl, .xdc, or .sdc. Paths that match a
+    for files that have an extension specified in `extensions`. Paths that match a
     pattern in `exclude_patterns` are ignored (based on gitignore pattern
     format, see https://git-scm.com/docs/gitignore#_pattern_format).
 
     Raises FileNotFoundError if a supplied path does not exist.
     """
-    # Extensions that may indicate tcl files
-    # TODO: make configurable
-    EXTENSIONS = [".tcl", ".xdc", ".sdc"]
-
+    extensions = [f".{ext}" if not ext.startswith(".") else ext for ext in extensions]
     exclude_root = exclude_root.resolve()
     exclude_patterns = [
         re.sub(r"^\s*#", r"\#", pattern) for pattern in exclude_patterns
     ]
     exclude_spec = pathspec.PathSpec.from_lines("gitwildmatch", exclude_patterns)
 
     def is_excluded(path):
@@ -83,15 +83,15 @@
         if not path.is_dir():
             sources.append(path)
             continue
 
         for dirpath, _, filenames in os.walk(path):
             for name in filenames:
                 _, ext = os.path.splitext(name)
-                if ext in EXTENSIONS:
+                if ext.lower() in extensions:
                     child = pathlib.Path(dirpath) / name
                     if not is_excluded(child):
                         sources.append(child)
 
     return sources
 
 
@@ -201,15 +201,18 @@
 
     try:
         # TODO: we should eventually allow tclint to find a config by walking up
         # directories, at which point exclude_root should be the parent dir of
         # the config file, unless -c is used (eslint rules)
         exclude_root = pathlib.Path.cwd()
         sources = resolve_sources(
-            args.source, exclude_patterns=config.exclude, exclude_root=exclude_root
+            args.source,
+            exclude_patterns=config.exclude,
+            exclude_root=exclude_root,
+            extensions=config.extensions,
         )
     except FileNotFoundError as e:
         print(f"Invalid path provided: {e}")
         return EXIT_INPUT_ERROR
 
     retcode = EXIT_OK
```

### Comparing `tclint-0.2.3/src/tclint/violations.py` & `tclint-0.2.4/src/tclint/violations.py`

 * *Files identical despite different names*

### Comparing `tclint-0.2.3/src/tclint.egg-info/PKG-INFO` & `tclint-0.2.4/src/tclint.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: tclint
-Version: 0.2.3
+Version: 0.2.4
 Summary: A CLI utility for linting and analyzing Tcl code.
 Author-email: Noah Moroze <me@noahmoroze.com>
 License: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: ply==3.11
 Requires-Dist: schema==0.7.5
 Requires-Dist: tomli~=2.0.1; python_version < "3.11"
 Requires-Dist: pathspec==0.11.2
+Requires-Dist: importlib-metadata==6.8.0
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: flake8; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-timeout; extra == "dev"
 
 # tclint &nbsp; [![CI](https://github.com/nmoroze/tclint/actions/workflows/ci.yml/badge.svg)](https://github.com/nmoroze/tclint/actions/workflows/ci.yml)
@@ -60,15 +61,15 @@
 example.tcl:1:1: too many args to puts: got 4, expected no more than 3 [command-args]
 example.tcl:2:1: expected indent of 0 spaces, got 2 [indent]
 example.tcl:3:5: expected 1 space between words, got 3 [spacing]
 ```
 
 ## Usage
 
-`tclint` is a command-line utility. It takes a list of paths as positional arguments, which may either be direct paths to source files, or directories which will be recursively searched for files ending in `.tcl`, `.sdc`, or `.xdc`.
+`tclint` is a command-line utility. It takes a list of paths as positional arguments, which may either be direct paths to source files, or directories which will be recursively searched for files ending in `.tcl`, `.sdc`, `.xdc`, or `.upf`.
 
 Collected files will be checked for lint violations.  See the
 [Violations](docs/violations.md) documentation page for a description of all
 lint violations `tclint` may report.
 
 Aspects of `tclint`'s behavior can be controlled by a configuration file. By default, `tclint` will look for a file named `tclint.toml` or `.tclint` in the current working directory (in that order), but a path to an alternate configuration file can be provided using the `-c` or `--config` flag. See [Configuration](docs/configuration.md) for documentation on the configuration file.
```

### Comparing `tclint-0.2.3/src/tclint.egg-info/SOURCES.txt` & `tclint-0.2.4/src/tclint.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tclint-0.2.3/tests/data/blank-lines.txt` & `tclint-0.2.4/tests/data/blank-lines.txt`

 * *Files identical despite different names*

### Comparing `tclint-0.2.3/tests/data/dirty.txt` & `tclint-0.2.4/tests/data/dirty.txt`

 * *Files identical despite different names*

### Comparing `tclint-0.2.3/tests/data/expr-format.txt` & `tclint-0.2.4/tests/data/expr-format.txt`

 * *Files identical despite different names*

### Comparing `tclint-0.2.3/tests/data/indent.txt` & `tclint-0.2.4/tests/data/indent.txt`

 * *Files identical despite different names*

### Comparing `tclint-0.2.3/tests/data/indent_lists.tcl` & `tclint-0.2.4/tests/data/indent_lists.tcl`

 * *Files identical despite different names*

### Comparing `tclint-0.2.3/tests/data/spaces-in-braces.txt` & `tclint-0.2.4/tests/data/spaces-in-braces.txt`

 * *Files identical despite different names*

### Comparing `tclint-0.2.3/tests/data/tclint.toml` & `tclint-0.2.4/tests/data/tclint.toml`

 * *Files 14% similar despite different names*

```diff
@@ -2,14 +2,17 @@
 exclude = ["ignore_me/", "ignore*.tcl", "/ignore_from_here"]
 # lint violations to ignore. defaults to empty list.
 # can also supply an inline table with a path and a list of violations to ignore under that path.
 ignore = [
     "spacing",
     { path = "files_with_bad_indent/", rules = ["indent"] }
 ]
+# extensions of files to lint when searching directories. defaults to tcl, sdc,
+# xdc, and upf.
+extensions = ["tcl"]
 
 [style]
 # number of spaces to indent. can also be set to "tab". defaults to 4.
 indent = 2
 # maximum allowed line length. defaults to 80.
 line-length = 100
 # maximum allowed number of consecutive blank lines. defaults to 2.
```

### Comparing `tclint-0.2.3/tests/test_config.py` & `tclint-0.2.4/tests/test_config.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     global_ = config.get_for_path(pathlib.Path())
 
     assert global_.exclude == ["ignore_me/", "ignore*.tcl", "/ignore_from_here"]
     assert global_.ignore == [
         Rule("spacing"),
         {"path": pathlib.Path("files_with_bad_indent/"), "rules": [Rule("indent")]},
     ]
+    assert global_.extensions == ["tcl"]
 
     assert global_.style_indent == 2
     assert global_.style_line_length == 100
     assert global_.style_allow_aligned_sets is True
     assert global_.style_indent_namespace_eval is False
 
     group1 = config.get_for_path(pathlib.Path("other_file_group1/file.tcl"))
```

### Comparing `tclint-0.2.3/tests/test_lint.py` & `tclint-0.2.4/tests/test_lint.py`

 * *Files identical despite different names*

### Comparing `tclint-0.2.3/tests/test_parser.py` & `tclint-0.2.4/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `tclint-0.2.3/tests/test_tclint.py` & `tclint-0.2.4/tests/test_tclint.py`

 * *Files 22% similar despite different names*

```diff
@@ -125,56 +125,90 @@
     (tmp_path / "src" / "ignore2.tcl").touch()
     to_include = tmp_path / "src" / "foo.tcl"
     to_include.touch()
 
     cwd = os.getcwd()
     os.chdir(tmp_path)
 
+    extensions = ["tcl"]
+
     sources = tclint.resolve_sources(
         [pathlib.Path(".")],
         exclude_patterns=[
             # test bare pattern matches anywhere in tree
             "ignore",
             # test glob
             "ignore*.tcl",
             # test pattern with "/" only matches from root of tree
             "/foo.tcl",
         ],
         exclude_root=tmp_path,
+        extensions=extensions,
     )
 
     assert len(sources) == 1
     assert sources[0] == to_include.relative_to(tmp_path)
 
     # test absolute path outside of exclude_root doesn't get matched by ignore
     # pattern starting with "/"
     other_dir = tmp_path_factory.mktemp("b")
     in_path = other_dir / "foo.tcl"
     in_path.touch()
     sources = tclint.resolve_sources(
-        [in_path], exclude_patterns=[str(in_path)], exclude_root=tmp_path
+        [in_path],
+        exclude_patterns=[str(in_path)],
+        exclude_root=tmp_path,
+        extensions=extensions,
     )
     assert len(sources) == 1
     assert sources[0] == in_path
 
     # test that we can match outside of exclude root with explicit relative path
     top_src = tmp_path / "top.tcl"
     top_src.touch()
     sources = tclint.resolve_sources(
-        [top_src], exclude_patterns=["../top.tcl"], exclude_root=tmp_path / "src"
+        [top_src],
+        exclude_patterns=["../top.tcl"],
+        exclude_root=tmp_path / "src",
+        extensions=extensions,
     )
     assert len(sources) == 0
 
     # test auto-escape leading hash
     other_other_dir = tmp_path_factory.mktemp("c")
     hash_srcs = [other_other_dir / "#foo.tcl", other_other_dir / "#bar.tcl"]
     for src in hash_srcs:
         src.touch()
     sources = tclint.resolve_sources(
         hash_srcs,
         # extra space before #bar.tcl is important to make sure we don't just match ^#
         exclude_patterns=["#foo.tcl", " #bar.tcl"],
         exclude_root=other_other_dir,
+        extensions=extensions,
     )
     assert len(sources) == 0
 
     os.chdir(cwd)
+
+
+def test_resolve_sources_extensions(tmp_path):
+    foo_file = tmp_path / "file.foo"
+    foo_file.touch()
+    bar_file = tmp_path / "file.BAR"
+    bar_file.touch()
+
+    cwd = os.getcwd()
+    os.chdir(tmp_path)
+
+    sources = tclint.resolve_sources(
+        [tmp_path], exclude_patterns=[], exclude_root=tmp_path, extensions=["foo"]
+    )
+    assert len(sources) == 1
+    assert sources[0] == foo_file
+
+    sources = tclint.resolve_sources(
+        [tmp_path], exclude_patterns=[], exclude_root=tmp_path, extensions=["bar"]
+    )
+    assert len(sources) == 1
+    assert sources[0] == bar_file
+
+    os.chdir(cwd)
```


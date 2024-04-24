# Comparing `tmp/flake8-async-24.4.1.tar.gz` & `tmp/flake8_async-24.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flake8-async-24.4.1.tar", last modified: Wed Apr 10 03:09:32 2024, max compression
+gzip compressed data, was "flake8_async-24.4.2.tar", last modified: Wed Apr 24 18:40:17 2024, max compression
```

## Comparing `flake8-async-24.4.1.tar` & `flake8_async-24.4.2.tar`

### file list

```diff
@@ -1,119 +1,120 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:09:32.021136 flake8-async-24.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)     7513 2024-04-10 03:09:20.000000 flake8-async-24.4.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     4889 2024-04-10 03:09:20.000000 flake8-async-24.4.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-10 03:09:20.000000 flake8-async-24.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-10 03:09:20.000000 flake8-async-24.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    21787 2024-04-10 03:09:32.021136 flake8-async-24.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13335 2024-04-10 03:09:29.000000 flake8-async-24.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:09:32.005136 flake8-async-24.4.1/flake8_async/
--rw-r--r--   0 runner    (1001) docker     (127)    14215 2024-04-10 03:09:20.000000 flake8-async-24.4.1/flake8_async/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-10 03:09:20.000000 flake8-async-24.4.1/flake8_async/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3178 2024-04-10 03:09:20.000000 flake8-async-24.4.1/flake8_async/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5052 2024-04-10 03:09:20.000000 flake8-async-24.4.1/flake8_async/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:09:32.005136 flake8-async-24.4.1/flake8_async/visitors/
--rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-04-10 03:09:20.000000 flake8-async-24.4.1/flake8_async/visitors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8896 2024-04-10 03:09:20.000000 flake8-async-24.4.1/flake8_async/visitors/flake8asyncvisitor.py
--rw-r--r--   0 runner    (1001) docker     (127)    13307 2024-04-10 03:09:20.000000 flake8-async-24.4.1/flake8_async/visitors/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2868 2024-04-10 03:09:20.000000 flake8-async-24.4.1/flake8_async/visitors/visitor100.py
--rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-04-10 03:09:20.000000 flake8-async-24.4.1/flake8_async/visitors/visitor101.py
--rw-r--r--   0 runner    (1001) docker     (127)     5699 2024-04-10 03:09:20.000000 flake8-async-24.4.1/flake8_async/visitors/visitor102.py
--rw-r--r--   0 runner    (1001) docker     (127)     8526 2024-04-10 03:09:20.000000 flake8-async-24.4.1/flake8_async/visitors/visitor103_104.py
--rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-04-10 03:09:20.000000 flake8-async-24.4.1/flake8_async/visitors/visitor105.py
--rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-04-10 03:09:20.000000 flake8-async-24.4.1/flake8_async/visitors/visitor111.py
--rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-04-10 03:09:20.000000 flake8-async-24.4.1/flake8_async/visitors/visitor118.py
--rw-r--r--   0 runner    (1001) docker     (127)    14407 2024-04-10 03:09:20.000000 flake8-async-24.4.1/flake8_async/visitors/visitor2xx.py
--rw-r--r--   0 runner    (1001) docker     (127)    32798 2024-04-10 03:09:20.000000 flake8-async-24.4.1/flake8_async/visitors/visitor91x.py
--rw-r--r--   0 runner    (1001) docker     (127)     7340 2024-04-10 03:09:20.000000 flake8-async-24.4.1/flake8_async/visitors/visitor_utility.py
--rw-r--r--   0 runner    (1001) docker     (127)    10743 2024-04-10 03:09:20.000000 flake8-async-24.4.1/flake8_async/visitors/visitors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:09:32.021136 flake8-async-24.4.1/flake8_async.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    21787 2024-04-10 03:09:31.000000 flake8-async-24.4.1/flake8_async.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3440 2024-04-10 03:09:31.000000 flake8-async-24.4.1/flake8_async.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 03:09:31.000000 flake8-async-24.4.1/flake8_async.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-10 03:09:31.000000 flake8-async-24.4.1/flake8_async.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 03:09:31.000000 flake8-async-24.4.1/flake8_async.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-10 03:09:31.000000 flake8-async-24.4.1/flake8_async.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-10 03:09:31.000000 flake8-async-24.4.1/flake8_async.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4188 2024-04-10 03:09:20.000000 flake8-async-24.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 03:09:32.021136 flake8-async-24.4.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     2098 2024-04-10 03:09:20.000000 flake8-async-24.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:09:32.009136 flake8-async-24.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-10 03:09:20.000000 flake8-async-24.4.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:09:32.009136 flake8-async-24.4.1/tests/autofix_files/
--rw-r--r--   0 runner    (1001) docker     (127)     2936 2024-04-10 03:09:20.000000 flake8-async-24.4.1/tests/autofix_files/async100.py
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-04-10 03:09:20.000000 flake8-async-24.4.1/tests/autofix_files/async100_simple_autofix.py
--rw-r--r--   0 runner    (1001) docker     (127)    11981 2024-04-10 03:09:20.000000 flake8-async-24.4.1/tests/autofix_files/async910.py
--rw-r--r--   0 runner    (1001) docker     (127)    28720 2024-04-10 03:09:20.000000 flake8-async-24.4.1/tests/autofix_files/async911.py
--rw-r--r--   0 runner    (1001) docker     (127)     3659 2024-04-10 03:09:20.000000 flake8-async-24.4.1/tests/autofix_files/async91x_autofix.py
--rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-04-10 03:09:20.000000 flake8-async-24.4.1/tests/autofix_files/noqa.py
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-10 03:09:20.000000 flake8-async-24.4.1/tests/autofix_files/noqa_testing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-04-10 03:09:20.000000 flake8-async-24.4.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:09:32.021136 flake8-async-24.4.1/tests/eval_files/
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-10 03:09:20.000000 flake8-async-24.4.1/tests/eval_files/anyio_trio.py
--rw-r--r--   0 runner    (1001) docker     (127)     3571 2024-04-10 03:09:20.000000 flake8-async-24.4.1/tests/eval_files/async100.py
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-10 03:09:20.000000 flake8-async-24.4.1/tests/eval_files/async100_asyncio.py
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-04-10 03:09:20.000000 flake8-async-24.4.1/tests/eval_files/async100_noautofix.py
--rw-r--r--   0 runner    (1001) docker     (127)      987 2024-04-10 03:09:20.000000 flake8-async-24.4.1/tests/eval_files/async100_simple_autofix.py
--rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-04-10 03:09:20.000000 flake8-async-24.4.1/tests/eval_files/async101.py
--rw-r--r--   0 runner    (1001) docker     (127)     7082 2024-04-10 03:09:20.000000 flake8-async-24.4.1/tests/eval_files/async102.py
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-04-10 03:09:20.000000 flake8-async-24.4.1/tests/eval_files/async102_aclose.py
--rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-10 03:09:20.000000 flake8-async-24.4.1/tests/eval_files/async102_aclose_args.py
--rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-04-10 03:09:20.000000 flake8-async-24.4.1/tests/eval_files/async102_anyio.py
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-04-10 03:09:20.000000 flake8-async-24.4.1/tests/eval_files/async102_asyncio.py
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-10 03:09:20.000000 flake8-async-24.4.1/tests/eval_files/async102_trio.py
--rw-r--r--   0 runner    (1001) docker     (127)     5893 2024-04-10 03:09:20.000000 flake8-async-24.4.1/tests/eval_files/async103.py
--rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-04-10 03:09:20.000000 flake8-async-24.4.1/tests/eval_files/async103_all_imported.py
--rw-r--r--   0 runner    (1001) docker     (127)      965 2024-04-10 03:09:20.000000 flake8-async-24.4.1/tests/eval_files/async103_both_imported.py
--rw-r--r--   0 runner    (1001) docker     (127)      461 2024-04-10 03:09:20.000000 flake8-async-24.4.1/tests/eval_files/async103_no_104.py
--rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-04-10 03:09:20.000000 flake8-async-24.4.1/tests/eval_files/async103_trio.py
--rw-r--r--   0 runner    (1001) docker     (127)     3780 2024-04-10 03:09:20.000000 flake8-async-24.4.1/tests/eval_files/async104.py
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-10 03:09:20.000000 flake8-async-24.4.1/tests/eval_files/async104_anyio.py
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-10 03:09:20.000000 flake8-async-24.4.1/tests/eval_files/async104_trio.py
--rw-r--r--   0 runner    (1001) docker     (127)     4747 2024-04-10 03:09:20.000000 flake8-async-24.4.1/tests/eval_files/async105.py
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-10 03:09:20.000000 flake8-async-24.4.1/tests/eval_files/async105_anyio.py
--rw-r--r--   0 runner    (1001) docker     (127)      538 2024-04-10 03:09:20.000000 flake8-async-24.4.1/tests/eval_files/async106.py
--rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-04-10 03:09:20.000000 flake8-async-24.4.1/tests/eval_files/async109.py
--rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-04-10 03:09:20.000000 flake8-async-24.4.1/tests/eval_files/async110.py
--rw-r--r--   0 runner    (1001) docker     (127)    10136 2024-04-10 03:09:20.000000 flake8-async-24.4.1/tests/eval_files/async111.py
--rw-r--r--   0 runner    (1001) docker     (127)     2799 2024-04-10 03:09:20.000000 flake8-async-24.4.1/tests/eval_files/async112.py
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-10 03:09:20.000000 flake8-async-24.4.1/tests/eval_files/async113.py
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-10 03:09:20.000000 flake8-async-24.4.1/tests/eval_files/async113_anyio.py
--rw-r--r--   0 runner    (1001) docker     (127)     4486 2024-04-10 03:09:20.000000 flake8-async-24.4.1/tests/eval_files/async113_trio.py
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-10 03:09:20.000000 flake8-async-24.4.1/tests/eval_files/async114.py
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-10 03:09:20.000000 flake8-async-24.4.1/tests/eval_files/async115.py
--rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-04-10 03:09:20.000000 flake8-async-24.4.1/tests/eval_files/async116.py
--rw-r--r--   0 runner    (1001) docker     (127)      886 2024-04-10 03:09:20.000000 flake8-async-24.4.1/tests/eval_files/async118.py
--rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-04-10 03:09:20.000000 flake8-async-24.4.1/tests/eval_files/async200.py
--rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-04-10 03:09:20.000000 flake8-async-24.4.1/tests/eval_files/async210.py
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-04-10 03:09:20.000000 flake8-async-24.4.1/tests/eval_files/async211.py
--rw-r--r--   0 runner    (1001) docker     (127)     2715 2024-04-10 03:09:20.000000 flake8-async-24.4.1/tests/eval_files/async212.py
--rw-r--r--   0 runner    (1001) docker     (127)     2915 2024-04-10 03:09:20.000000 flake8-async-24.4.1/tests/eval_files/async22x.py
--rw-r--r--   0 runner    (1001) docker     (127)     2967 2024-04-10 03:09:20.000000 flake8-async-24.4.1/tests/eval_files/async22x_asyncio.py
--rw-r--r--   0 runner    (1001) docker     (127)     6230 2024-04-10 03:09:20.000000 flake8-async-24.4.1/tests/eval_files/async232.py
--rw-r--r--   0 runner    (1001) docker     (127)     6255 2024-04-10 03:09:20.000000 flake8-async-24.4.1/tests/eval_files/async232_asyncio.py
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-10 03:09:20.000000 flake8-async-24.4.1/tests/eval_files/async23x.py
--rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-04-10 03:09:20.000000 flake8-async-24.4.1/tests/eval_files/async23x_asyncio.py
--rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-04-10 03:09:20.000000 flake8-async-24.4.1/tests/eval_files/async240.py
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-10 03:09:20.000000 flake8-async-24.4.1/tests/eval_files/async250.py
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-10 03:09:20.000000 flake8-async-24.4.1/tests/eval_files/async250_multi_library.py
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-10 03:09:20.000000 flake8-async-24.4.1/tests/eval_files/async251.py
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-10 03:09:20.000000 flake8-async-24.4.1/tests/eval_files/async251_multi_library.py
--rw-r--r--   0 runner    (1001) docker     (127)      905 2024-04-10 03:09:20.000000 flake8-async-24.4.1/tests/eval_files/async900.py
--rw-r--r--   0 runner    (1001) docker     (127)    10851 2024-04-10 03:09:20.000000 flake8-async-24.4.1/tests/eval_files/async910.py
--rw-r--r--   0 runner    (1001) docker     (127)    23988 2024-04-10 03:09:20.000000 flake8-async-24.4.1/tests/eval_files/async911.py
--rw-r--r--   0 runner    (1001) docker     (127)     3069 2024-04-10 03:09:20.000000 flake8-async-24.4.1/tests/eval_files/async91x_autofix.py
--rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-04-10 03:09:20.000000 flake8-async-24.4.1/tests/eval_files/async91x_noautofix.py
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-10 03:09:20.000000 flake8-async-24.4.1/tests/eval_files/no_library.py
--rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-04-10 03:09:20.000000 flake8-async-24.4.1/tests/eval_files/noqa.py
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-10 03:09:20.000000 flake8-async-24.4.1/tests/eval_files/noqa_no_autofix.py
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-10 03:09:20.000000 flake8-async-24.4.1/tests/eval_files/noqa_testing.py
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-10 03:09:20.000000 flake8-async-24.4.1/tests/eval_files/trio_anyio.py
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-04-10 03:09:20.000000 flake8-async-24.4.1/tests/test_all_visitors_imported.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3604 2024-04-10 03:09:20.000000 flake8-async-24.4.1/tests/test_changelog_and_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    11124 2024-04-10 03:09:20.000000 flake8-async-24.4.1/tests/test_config_and_args.py
--rw-r--r--   0 runner    (1001) docker     (127)     3455 2024-04-10 03:09:20.000000 flake8-async-24.4.1/tests/test_decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-10 03:09:20.000000 flake8-async-24.4.1/tests/test_exception_on_invalid_code.py
--rw-r--r--   0 runner    (1001) docker     (127)    29043 2024-04-10 03:09:20.000000 flake8-async-24.4.1/tests/test_flake8_async.py
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-10 03:09:20.000000 flake8-async-24.4.1/tests/test_formatting.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3407 2024-04-10 03:09:20.000000 flake8-async-24.4.1/tests/test_messages_documented.py
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-10 03:09:20.000000 flake8-async-24.4.1/tests/trio_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-04-10 03:09:20.000000 flake8-async-24.4.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:40:17.211190 flake8_async-24.4.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     7583 2024-04-24 18:40:10.000000 flake8_async-24.4.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4889 2024-04-24 18:40:10.000000 flake8_async-24.4.2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-24 18:40:10.000000 flake8_async-24.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-24 18:40:10.000000 flake8_async-24.4.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    22912 2024-04-24 18:40:17.211190 flake8_async-24.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14390 2024-04-24 18:40:14.000000 flake8_async-24.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:40:17.191189 flake8_async-24.4.2/flake8_async/
+-rw-r--r--   0 runner    (1001) docker     (127)    14215 2024-04-24 18:40:10.000000 flake8_async-24.4.2/flake8_async/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-24 18:40:10.000000 flake8_async-24.4.2/flake8_async/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3178 2024-04-24 18:40:10.000000 flake8_async-24.4.2/flake8_async/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5052 2024-04-24 18:40:10.000000 flake8_async-24.4.2/flake8_async/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:40:17.195190 flake8_async-24.4.2/flake8_async/visitors/
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-04-24 18:40:10.000000 flake8_async-24.4.2/flake8_async/visitors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8896 2024-04-24 18:40:10.000000 flake8_async-24.4.2/flake8_async/visitors/flake8asyncvisitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13307 2024-04-24 18:40:10.000000 flake8_async-24.4.2/flake8_async/visitors/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2868 2024-04-24 18:40:10.000000 flake8_async-24.4.2/flake8_async/visitors/visitor100.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-04-24 18:40:10.000000 flake8_async-24.4.2/flake8_async/visitors/visitor101.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5699 2024-04-24 18:40:10.000000 flake8_async-24.4.2/flake8_async/visitors/visitor102.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8526 2024-04-24 18:40:10.000000 flake8_async-24.4.2/flake8_async/visitors/visitor103_104.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-04-24 18:40:10.000000 flake8_async-24.4.2/flake8_async/visitors/visitor105.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-04-24 18:40:10.000000 flake8_async-24.4.2/flake8_async/visitors/visitor111.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-04-24 18:40:10.000000 flake8_async-24.4.2/flake8_async/visitors/visitor118.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14407 2024-04-24 18:40:10.000000 flake8_async-24.4.2/flake8_async/visitors/visitor2xx.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32798 2024-04-24 18:40:10.000000 flake8_async-24.4.2/flake8_async/visitors/visitor91x.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7340 2024-04-24 18:40:10.000000 flake8_async-24.4.2/flake8_async/visitors/visitor_utility.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12111 2024-04-24 18:40:10.000000 flake8_async-24.4.2/flake8_async/visitors/visitors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:40:17.207190 flake8_async-24.4.2/flake8_async.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    22912 2024-04-24 18:40:17.000000 flake8_async-24.4.2/flake8_async.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3469 2024-04-24 18:40:17.000000 flake8_async-24.4.2/flake8_async.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 18:40:17.000000 flake8_async-24.4.2/flake8_async.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-24 18:40:17.000000 flake8_async-24.4.2/flake8_async.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 18:40:17.000000 flake8_async-24.4.2/flake8_async.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-24 18:40:17.000000 flake8_async-24.4.2/flake8_async.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-24 18:40:17.000000 flake8_async-24.4.2/flake8_async.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4188 2024-04-24 18:40:10.000000 flake8_async-24.4.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 18:40:17.211190 flake8_async-24.4.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2098 2024-04-24 18:40:10.000000 flake8_async-24.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:40:17.199190 flake8_async-24.4.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:40:17.199190 flake8_async-24.4.2/tests/autofix_files/
+-rw-r--r--   0 runner    (1001) docker     (127)     2936 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tests/autofix_files/async100.py
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tests/autofix_files/async100_simple_autofix.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11981 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tests/autofix_files/async910.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28720 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tests/autofix_files/async911.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3659 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tests/autofix_files/async91x_autofix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tests/autofix_files/noqa.py
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tests/autofix_files/noqa_testing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:40:17.207190 flake8_async-24.4.2/tests/eval_files/
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tests/eval_files/anyio_trio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3571 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tests/eval_files/async100.py
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tests/eval_files/async100_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tests/eval_files/async100_noautofix.py
+-rw-r--r--   0 runner    (1001) docker     (127)      987 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tests/eval_files/async100_simple_autofix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tests/eval_files/async101.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7082 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tests/eval_files/async102.py
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tests/eval_files/async102_aclose.py
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tests/eval_files/async102_aclose_args.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tests/eval_files/async102_anyio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tests/eval_files/async102_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tests/eval_files/async102_trio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5893 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tests/eval_files/async103.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tests/eval_files/async103_all_imported.py
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tests/eval_files/async103_both_imported.py
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tests/eval_files/async103_no_104.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tests/eval_files/async103_trio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3780 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tests/eval_files/async104.py
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tests/eval_files/async104_anyio.py
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tests/eval_files/async104_trio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4747 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tests/eval_files/async105.py
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tests/eval_files/async105_anyio.py
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tests/eval_files/async106.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tests/eval_files/async109.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tests/eval_files/async110.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10136 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tests/eval_files/async111.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2799 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tests/eval_files/async112.py
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tests/eval_files/async113.py
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tests/eval_files/async113_anyio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4486 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tests/eval_files/async113_trio.py
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tests/eval_files/async114.py
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tests/eval_files/async115.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tests/eval_files/async116.py
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tests/eval_files/async118.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tests/eval_files/async119.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tests/eval_files/async200.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tests/eval_files/async210.py
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tests/eval_files/async211.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2715 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tests/eval_files/async212.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2915 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tests/eval_files/async22x.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2967 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tests/eval_files/async22x_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6230 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tests/eval_files/async232.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6255 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tests/eval_files/async232_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tests/eval_files/async23x.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tests/eval_files/async23x_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tests/eval_files/async240.py
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tests/eval_files/async250.py
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tests/eval_files/async250_multi_library.py
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tests/eval_files/async251.py
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tests/eval_files/async251_multi_library.py
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tests/eval_files/async900.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10851 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tests/eval_files/async910.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23988 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tests/eval_files/async911.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3069 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tests/eval_files/async91x_autofix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tests/eval_files/async91x_noautofix.py
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tests/eval_files/no_library.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tests/eval_files/noqa.py
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tests/eval_files/noqa_no_autofix.py
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tests/eval_files/noqa_testing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tests/eval_files/trio_anyio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tests/test_all_visitors_imported.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3604 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tests/test_changelog_and_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12107 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tests/test_config_and_args.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3455 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tests/test_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tests/test_exception_on_invalid_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29043 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tests/test_flake8_async.py
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tests/test_formatting.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3407 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tests/test_messages_documented.py
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tests/trio_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tox.ini
```

### Comparing `flake8-async-24.4.1/CHANGELOG.md` & `flake8_async-24.4.2/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 # Changelog
 *[CalVer, YY.month.patch](https://calver.org/)*
 
+## 24.4.2
+- Add ASYNC119: yield in contextmanager in async generator.
 
 ## 24.4.1
 - ASYNC91X fix internal error caused by multiple `try/except` incorrectly sharing state.
 
 ## 24.3.6
 - ASYNC100 no longer triggers if a context manager contains a `yield`.
```

### Comparing `flake8-async-24.4.1/CONTRIBUTING.md` & `flake8_async-24.4.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `flake8-async-24.4.1/LICENSE` & `flake8_async-24.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `flake8-async-24.4.1/PKG-INFO` & `flake8_async-24.4.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flake8-async
-Version: 24.4.1
+Version: 24.4.2
 Summary: A highly opinionated flake8 plugin for Trio-related problems.
 Home-page: https://github.com/python-trio/flake8-async
 Author: Zac Hatfield-Dodds, John Litborn, and Contributors
 Author-email: zac@zhd.dev
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Flake8
@@ -62,14 +62,15 @@
 - **ASYNC111**: Variable, from context manager opened inside nursery, passed to `start[_soon]` might be invalidly accessed while in use, due to context manager closing before the nursery. This is usually a bug, and nurseries should generally be the inner-most context manager.
 - **ASYNC112**: Nursery body with only a call to `nursery.start[_soon]` and not passing itself as a parameter can be replaced with a regular function call.
 - **ASYNC113**: Using `nursery.start_soon` in `__aenter__` doesn't wait for the task to begin. Consider replacing with `nursery.start`.
 - **ASYNC114**: Startable function (i.e. has a `task_status` keyword parameter) not in `--startable-in-context-manager` parameter list, please add it so ASYNC113 can catch errors when using it.
 - **ASYNC115**: Replace `[trio/anyio].sleep(0)` with the more suggestive `[trio/anyio].lowlevel.checkpoint()`.
 - **ASYNC116**: `[trio/anyio].sleep()` with >24 hour interval should usually be `[trio/anyio].sleep_forever()`.
 - **ASYNC118**: Don't assign the value of `anyio.get_cancelled_exc_class()` to a variable, since that breaks linter checks and multi-backend programs.
+- **ASYNC119**: `yield` in context manager in async generator is unsafe, the cleanup may be delayed until `await` is no longer allowed. We strongly encourage you to read PEP-533 and use `async with aclosing(...)`, or better yet avoid async generators entirely (see ASYNC900) in favor of context managers which return an iterable channel/queue.
 
 ### Warnings for blocking sync calls in async functions
 Note: 22X, 23X and 24X has not had asyncio-specific suggestions written.
 - **ASYNC200**: User-configured error for blocking sync calls in async functions. Does nothing by default, see [`async200-blocking-calls`](#async200-blocking-calls) for how to configure it.
 - **ASYNC210**: Sync HTTP call in async function, use `httpx.AsyncClient`. This and the other ASYNC21x checks look for usage of `urllib3` and `httpx.Client`, and recommend using `httpx.AsyncClient` as that's the largest http client supporting anyio/trio.
 - **ASYNC211**: Likely sync HTTP call in async function, use `httpx.AsyncClient`. Looks for `urllib3` method calls on pool objects, but only matching on the method signature and not the object.
 - **ASYNC212**: Blocking sync HTTP call on httpx object, use httpx.AsyncClient.
@@ -105,15 +106,15 @@
 If you use [pre-commit](https://pre-commit.com/), you can use it with flake8-async by
 adding the following to your `.pre-commit-config.yaml`:
 
 ```yaml
 minimum_pre_commit_version: '2.9.0'
 repos:
 - repo: https://github.com/python-trio/flake8-async
-  rev: 24.4.1
+  rev: 24.4.2
   hooks:
     - id: flake8-async
       # args: [--enable=ASYNC, --disable=ASYNC9, --autofix=ASYNC]
 ```
 
 This is often considerably faster for large projects, because `pre-commit`
 can avoid running `flake8-async` on unchanged files.
@@ -144,14 +145,17 @@
 ```
 
 ## Configuration
 [You can configure `flake8` with command-line options](https://flake8.pycqa.org/en/latest/user/configuration.html),
 but we prefer using a config file. The file needs to start with a section marker `[flake8]` and the following options are then parsed using flake8's config parser, and can be used just like any other flake8 options.
 Note that it's not currently possible to use a configuration file when running `flake8-async` standalone.
 
+### `ValueError` when trying to `ignore` error codes in config file
+Error codes with more than three letters are not possible to `ignore` in config files since flake8>=6, as flake8 tries to validate correct configuration with a regex. We have decided not to conform to this, as it would be a breaking change for end-users requiring them to update `noqa`s and configurations, we think the `ASYNC` code is much more readable than e.g. `ASYxxx`, and ruff does not enforce such a limit. The easiest option for users hitting this error is to instead use the `--disable` option as documented [below](#--disable). See further discussion and other workarounds in https://github.com/python-trio/flake8-async/issues/230
+
 ### `--enable`
 Comma-separated list of error codes to enable, similar to flake8 --select but is additionally more performant as it will disable non-enabled visitors from running instead of just silencing their errors.
 
 ### `--disable`
 Comma-separated list of error codes to disable, similar to flake8 --ignore but is additionally more performant as it will disable non-enabled visitors from running instead of just silencing their errors.
 
 ### `--autofix`
@@ -217,14 +221,16 @@
     arbitrary_other_function(my_blocking_call=None)
 ```
 
 
 # Changelog
 *[CalVer, YY.month.patch](https://calver.org/)*
 
+## 24.4.2
+- Add ASYNC119: yield in contextmanager in async generator.
 
 ## 24.4.1
 - ASYNC91X fix internal error caused by multiple `try/except` incorrectly sharing state.
 
 ## 24.3.6
 - ASYNC100 no longer triggers if a context manager contains a `yield`.
```

### Comparing `flake8-async-24.4.1/README.md` & `flake8_async-24.4.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 - **ASYNC111**: Variable, from context manager opened inside nursery, passed to `start[_soon]` might be invalidly accessed while in use, due to context manager closing before the nursery. This is usually a bug, and nurseries should generally be the inner-most context manager.
 - **ASYNC112**: Nursery body with only a call to `nursery.start[_soon]` and not passing itself as a parameter can be replaced with a regular function call.
 - **ASYNC113**: Using `nursery.start_soon` in `__aenter__` doesn't wait for the task to begin. Consider replacing with `nursery.start`.
 - **ASYNC114**: Startable function (i.e. has a `task_status` keyword parameter) not in `--startable-in-context-manager` parameter list, please add it so ASYNC113 can catch errors when using it.
 - **ASYNC115**: Replace `[trio/anyio].sleep(0)` with the more suggestive `[trio/anyio].lowlevel.checkpoint()`.
 - **ASYNC116**: `[trio/anyio].sleep()` with >24 hour interval should usually be `[trio/anyio].sleep_forever()`.
 - **ASYNC118**: Don't assign the value of `anyio.get_cancelled_exc_class()` to a variable, since that breaks linter checks and multi-backend programs.
+- **ASYNC119**: `yield` in context manager in async generator is unsafe, the cleanup may be delayed until `await` is no longer allowed. We strongly encourage you to read PEP-533 and use `async with aclosing(...)`, or better yet avoid async generators entirely (see ASYNC900) in favor of context managers which return an iterable channel/queue.
 
 ### Warnings for blocking sync calls in async functions
 Note: 22X, 23X and 24X has not had asyncio-specific suggestions written.
 - **ASYNC200**: User-configured error for blocking sync calls in async functions. Does nothing by default, see [`async200-blocking-calls`](#async200-blocking-calls) for how to configure it.
 - **ASYNC210**: Sync HTTP call in async function, use `httpx.AsyncClient`. This and the other ASYNC21x checks look for usage of `urllib3` and `httpx.Client`, and recommend using `httpx.AsyncClient` as that's the largest http client supporting anyio/trio.
 - **ASYNC211**: Likely sync HTTP call in async function, use `httpx.AsyncClient`. Looks for `urllib3` method calls on pool objects, but only matching on the method signature and not the object.
 - **ASYNC212**: Blocking sync HTTP call on httpx object, use httpx.AsyncClient.
@@ -80,15 +81,15 @@
 If you use [pre-commit](https://pre-commit.com/), you can use it with flake8-async by
 adding the following to your `.pre-commit-config.yaml`:
 
 ```yaml
 minimum_pre_commit_version: '2.9.0'
 repos:
 - repo: https://github.com/python-trio/flake8-async
-  rev: 24.4.1
+  rev: 24.4.2
   hooks:
     - id: flake8-async
       # args: [--enable=ASYNC, --disable=ASYNC9, --autofix=ASYNC]
 ```
 
 This is often considerably faster for large projects, because `pre-commit`
 can avoid running `flake8-async` on unchanged files.
@@ -119,14 +120,17 @@
 ```
 
 ## Configuration
 [You can configure `flake8` with command-line options](https://flake8.pycqa.org/en/latest/user/configuration.html),
 but we prefer using a config file. The file needs to start with a section marker `[flake8]` and the following options are then parsed using flake8's config parser, and can be used just like any other flake8 options.
 Note that it's not currently possible to use a configuration file when running `flake8-async` standalone.
 
+### `ValueError` when trying to `ignore` error codes in config file
+Error codes with more than three letters are not possible to `ignore` in config files since flake8>=6, as flake8 tries to validate correct configuration with a regex. We have decided not to conform to this, as it would be a breaking change for end-users requiring them to update `noqa`s and configurations, we think the `ASYNC` code is much more readable than e.g. `ASYxxx`, and ruff does not enforce such a limit. The easiest option for users hitting this error is to instead use the `--disable` option as documented [below](#--disable). See further discussion and other workarounds in https://github.com/python-trio/flake8-async/issues/230
+
 ### `--enable`
 Comma-separated list of error codes to enable, similar to flake8 --select but is additionally more performant as it will disable non-enabled visitors from running instead of just silencing their errors.
 
 ### `--disable`
 Comma-separated list of error codes to disable, similar to flake8 --ignore but is additionally more performant as it will disable non-enabled visitors from running instead of just silencing their errors.
 
 ### `--autofix`
```

### Comparing `flake8-async-24.4.1/flake8_async/__init__.py` & `flake8_async-24.4.2/flake8_async/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 
     from flake8.options.manager import OptionManager
 
     from .base import Error
 
 
 # CalVer: YY.month.patch, e.g. first release of July 2022 == "22.7.1"
-__version__ = "24.4.1"
+__version__ = "24.4.2"
 
 
 # taken from https://github.com/Zac-HD/shed
 @functools.lru_cache
 def _get_git_repo_root(cwd: str | None = None) -> str:
     return subprocess.run(
         ["git", "rev-parse", "--show-toplevel"],
```

### Comparing `flake8-async-24.4.1/flake8_async/base.py` & `flake8_async-24.4.2/flake8_async/base.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.4.1/flake8_async/runner.py` & `flake8_async-24.4.2/flake8_async/runner.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.4.1/flake8_async/visitors/__init__.py` & `flake8_async-24.4.2/flake8_async/visitors/__init__.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.4.1/flake8_async/visitors/flake8asyncvisitor.py` & `flake8_async-24.4.2/flake8_async/visitors/flake8asyncvisitor.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.4.1/flake8_async/visitors/helpers.py` & `flake8_async-24.4.2/flake8_async/visitors/helpers.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.4.1/flake8_async/visitors/visitor100.py` & `flake8_async-24.4.2/flake8_async/visitors/visitor100.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.4.1/flake8_async/visitors/visitor101.py` & `flake8_async-24.4.2/flake8_async/visitors/visitor101.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.4.1/flake8_async/visitors/visitor102.py` & `flake8_async-24.4.2/flake8_async/visitors/visitor102.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.4.1/flake8_async/visitors/visitor103_104.py` & `flake8_async-24.4.2/flake8_async/visitors/visitor103_104.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.4.1/flake8_async/visitors/visitor105.py` & `flake8_async-24.4.2/flake8_async/visitors/visitor105.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.4.1/flake8_async/visitors/visitor111.py` & `flake8_async-24.4.2/flake8_async/visitors/visitor111.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.4.1/flake8_async/visitors/visitor118.py` & `flake8_async-24.4.2/flake8_async/visitors/visitor118.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.4.1/flake8_async/visitors/visitor2xx.py` & `flake8_async-24.4.2/flake8_async/visitors/visitor2xx.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.4.1/flake8_async/visitors/visitor91x.py` & `flake8_async-24.4.2/flake8_async/visitors/visitor91x.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.4.1/flake8_async/visitors/visitor_utility.py` & `flake8_async-24.4.2/flake8_async/visitors/visitor_utility.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.4.1/flake8_async/visitors/visitors.py` & `flake8_async-24.4.2/flake8_async/visitors/visitors.py`

 * *Files 14% similar despite different names*

```diff
@@ -278,14 +278,53 @@
                     and arg.value > 86400
                 )
             ):
                 self.error(node, m[2])
 
 
 @error_class
+class Visitor119(Flake8AsyncVisitor):
+    error_codes: Mapping[str, str] = {
+        "ASYNC119": "Yield in contextmanager in async generator might not trigger"
+        " cleanup. Use `@asynccontextmanager` or refactor."
+    }
+
+    def __init__(self, *args: Any, **kwargs: Any):
+        super().__init__(*args, **kwargs)
+        self.unsafe_function: bool = False
+        self.contextmanager: bool = False
+
+    def visit_AsyncFunctionDef(
+        self, node: ast.AsyncFunctionDef | ast.FunctionDef | ast.Lambda
+    ):
+        self.save_state(node, "unsafe_function", "contextmanager")
+        self.contextmanager = False
+        if isinstance(node, ast.AsyncFunctionDef) and not has_decorator(
+            node, "asynccontextmanager"
+        ):
+            self.unsafe_function = True
+        else:
+            self.unsafe_function = False
+
+    def visit_With(self, node: ast.With | ast.AsyncWith):
+        self.save_state(node, "contextmanager")
+        self.contextmanager = True
+
+    def visit_Yield(self, node: ast.Yield):
+        if self.unsafe_function and self.contextmanager:
+            self.error(node)
+
+    visit_AsyncWith = visit_With
+    visit_FunctionDef = visit_AsyncFunctionDef
+    # it's not possible to yield or open context managers in lambda's, so this
+    # one isn't strictly needed afaik.
+    visit_Lambda = visit_AsyncFunctionDef
+
+
+@error_class
 @disabled_by_default
 class Visitor900(Flake8AsyncVisitor):
     error_codes: Mapping[str, str] = {
         "ASYNC900": "Async generator without `@asynccontextmanager` not allowed."
     }
 
     def __init__(self, *args: Any, **kwargs: Any):
```

### Comparing `flake8-async-24.4.1/flake8_async.egg-info/PKG-INFO` & `flake8_async-24.4.2/flake8_async.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flake8-async
-Version: 24.4.1
+Version: 24.4.2
 Summary: A highly opinionated flake8 plugin for Trio-related problems.
 Home-page: https://github.com/python-trio/flake8-async
 Author: Zac Hatfield-Dodds, John Litborn, and Contributors
 Author-email: zac@zhd.dev
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Flake8
@@ -62,14 +62,15 @@
 - **ASYNC111**: Variable, from context manager opened inside nursery, passed to `start[_soon]` might be invalidly accessed while in use, due to context manager closing before the nursery. This is usually a bug, and nurseries should generally be the inner-most context manager.
 - **ASYNC112**: Nursery body with only a call to `nursery.start[_soon]` and not passing itself as a parameter can be replaced with a regular function call.
 - **ASYNC113**: Using `nursery.start_soon` in `__aenter__` doesn't wait for the task to begin. Consider replacing with `nursery.start`.
 - **ASYNC114**: Startable function (i.e. has a `task_status` keyword parameter) not in `--startable-in-context-manager` parameter list, please add it so ASYNC113 can catch errors when using it.
 - **ASYNC115**: Replace `[trio/anyio].sleep(0)` with the more suggestive `[trio/anyio].lowlevel.checkpoint()`.
 - **ASYNC116**: `[trio/anyio].sleep()` with >24 hour interval should usually be `[trio/anyio].sleep_forever()`.
 - **ASYNC118**: Don't assign the value of `anyio.get_cancelled_exc_class()` to a variable, since that breaks linter checks and multi-backend programs.
+- **ASYNC119**: `yield` in context manager in async generator is unsafe, the cleanup may be delayed until `await` is no longer allowed. We strongly encourage you to read PEP-533 and use `async with aclosing(...)`, or better yet avoid async generators entirely (see ASYNC900) in favor of context managers which return an iterable channel/queue.
 
 ### Warnings for blocking sync calls in async functions
 Note: 22X, 23X and 24X has not had asyncio-specific suggestions written.
 - **ASYNC200**: User-configured error for blocking sync calls in async functions. Does nothing by default, see [`async200-blocking-calls`](#async200-blocking-calls) for how to configure it.
 - **ASYNC210**: Sync HTTP call in async function, use `httpx.AsyncClient`. This and the other ASYNC21x checks look for usage of `urllib3` and `httpx.Client`, and recommend using `httpx.AsyncClient` as that's the largest http client supporting anyio/trio.
 - **ASYNC211**: Likely sync HTTP call in async function, use `httpx.AsyncClient`. Looks for `urllib3` method calls on pool objects, but only matching on the method signature and not the object.
 - **ASYNC212**: Blocking sync HTTP call on httpx object, use httpx.AsyncClient.
@@ -105,15 +106,15 @@
 If you use [pre-commit](https://pre-commit.com/), you can use it with flake8-async by
 adding the following to your `.pre-commit-config.yaml`:
 
 ```yaml
 minimum_pre_commit_version: '2.9.0'
 repos:
 - repo: https://github.com/python-trio/flake8-async
-  rev: 24.4.1
+  rev: 24.4.2
   hooks:
     - id: flake8-async
       # args: [--enable=ASYNC, --disable=ASYNC9, --autofix=ASYNC]
 ```
 
 This is often considerably faster for large projects, because `pre-commit`
 can avoid running `flake8-async` on unchanged files.
@@ -144,14 +145,17 @@
 ```
 
 ## Configuration
 [You can configure `flake8` with command-line options](https://flake8.pycqa.org/en/latest/user/configuration.html),
 but we prefer using a config file. The file needs to start with a section marker `[flake8]` and the following options are then parsed using flake8's config parser, and can be used just like any other flake8 options.
 Note that it's not currently possible to use a configuration file when running `flake8-async` standalone.
 
+### `ValueError` when trying to `ignore` error codes in config file
+Error codes with more than three letters are not possible to `ignore` in config files since flake8>=6, as flake8 tries to validate correct configuration with a regex. We have decided not to conform to this, as it would be a breaking change for end-users requiring them to update `noqa`s and configurations, we think the `ASYNC` code is much more readable than e.g. `ASYxxx`, and ruff does not enforce such a limit. The easiest option for users hitting this error is to instead use the `--disable` option as documented [below](#--disable). See further discussion and other workarounds in https://github.com/python-trio/flake8-async/issues/230
+
 ### `--enable`
 Comma-separated list of error codes to enable, similar to flake8 --select but is additionally more performant as it will disable non-enabled visitors from running instead of just silencing their errors.
 
 ### `--disable`
 Comma-separated list of error codes to disable, similar to flake8 --ignore but is additionally more performant as it will disable non-enabled visitors from running instead of just silencing their errors.
 
 ### `--autofix`
@@ -217,14 +221,16 @@
     arbitrary_other_function(my_blocking_call=None)
 ```
 
 
 # Changelog
 *[CalVer, YY.month.patch](https://calver.org/)*
 
+## 24.4.2
+- Add ASYNC119: yield in contextmanager in async generator.
 
 ## 24.4.1
 - ASYNC91X fix internal error caused by multiple `try/except` incorrectly sharing state.
 
 ## 24.3.6
 - ASYNC100 no longer triggers if a context manager contains a `yield`.
```

### Comparing `flake8-async-24.4.1/flake8_async.egg-info/SOURCES.txt` & `flake8_async-24.4.2/flake8_async.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -79,14 +79,15 @@
 tests/eval_files/async113.py
 tests/eval_files/async113_anyio.py
 tests/eval_files/async113_trio.py
 tests/eval_files/async114.py
 tests/eval_files/async115.py
 tests/eval_files/async116.py
 tests/eval_files/async118.py
+tests/eval_files/async119.py
 tests/eval_files/async200.py
 tests/eval_files/async210.py
 tests/eval_files/async211.py
 tests/eval_files/async212.py
 tests/eval_files/async22x.py
 tests/eval_files/async22x_asyncio.py
 tests/eval_files/async232.py
```

### Comparing `flake8-async-24.4.1/pyproject.toml` & `flake8_async-24.4.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `flake8-async-24.4.1/setup.py` & `flake8_async-24.4.2/setup.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.4.1/tests/autofix_files/async100.py` & `flake8_async-24.4.2/tests/autofix_files/async100.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.4.1/tests/autofix_files/async100_simple_autofix.py` & `flake8_async-24.4.2/tests/autofix_files/async100_simple_autofix.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.4.1/tests/autofix_files/async910.py` & `flake8_async-24.4.2/tests/autofix_files/async910.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.4.1/tests/autofix_files/async911.py` & `flake8_async-24.4.2/tests/autofix_files/async911.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.4.1/tests/autofix_files/async91x_autofix.py` & `flake8_async-24.4.2/tests/autofix_files/async91x_autofix.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.4.1/tests/autofix_files/noqa.py` & `flake8_async-24.4.2/tests/autofix_files/noqa.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.4.1/tests/conftest.py` & `flake8_async-24.4.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.4.1/tests/eval_files/async100.py` & `flake8_async-24.4.2/tests/eval_files/async100.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.4.1/tests/eval_files/async100_asyncio.py` & `flake8_async-24.4.2/tests/eval_files/async100_asyncio.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.4.1/tests/eval_files/async100_noautofix.py` & `flake8_async-24.4.2/tests/eval_files/async100_noautofix.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.4.1/tests/eval_files/async100_simple_autofix.py` & `flake8_async-24.4.2/tests/eval_files/async100_simple_autofix.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.4.1/tests/eval_files/async101.py` & `flake8_async-24.4.2/tests/eval_files/async101.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.4.1/tests/eval_files/async102.py` & `flake8_async-24.4.2/tests/eval_files/async102.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.4.1/tests/eval_files/async102_aclose.py` & `flake8_async-24.4.2/tests/eval_files/async102_aclose.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.4.1/tests/eval_files/async102_aclose_args.py` & `flake8_async-24.4.2/tests/eval_files/async102_aclose_args.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.4.1/tests/eval_files/async102_anyio.py` & `flake8_async-24.4.2/tests/eval_files/async102_anyio.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.4.1/tests/eval_files/async102_asyncio.py` & `flake8_async-24.4.2/tests/eval_files/async102_asyncio.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.4.1/tests/eval_files/async102_trio.py` & `flake8_async-24.4.2/tests/eval_files/async102_trio.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.4.1/tests/eval_files/async103.py` & `flake8_async-24.4.2/tests/eval_files/async103.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.4.1/tests/eval_files/async103_all_imported.py` & `flake8_async-24.4.2/tests/eval_files/async103_all_imported.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.4.1/tests/eval_files/async103_both_imported.py` & `flake8_async-24.4.2/tests/eval_files/async103_both_imported.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.4.1/tests/eval_files/async103_trio.py` & `flake8_async-24.4.2/tests/eval_files/async103_trio.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.4.1/tests/eval_files/async104.py` & `flake8_async-24.4.2/tests/eval_files/async104.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.4.1/tests/eval_files/async104_anyio.py` & `flake8_async-24.4.2/tests/eval_files/async104_anyio.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.4.1/tests/eval_files/async105.py` & `flake8_async-24.4.2/tests/eval_files/async105.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.4.1/tests/eval_files/async106.py` & `flake8_async-24.4.2/tests/eval_files/async106.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.4.1/tests/eval_files/async109.py` & `flake8_async-24.4.2/tests/eval_files/async109.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.4.1/tests/eval_files/async110.py` & `flake8_async-24.4.2/tests/eval_files/async110.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.4.1/tests/eval_files/async111.py` & `flake8_async-24.4.2/tests/eval_files/async111.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.4.1/tests/eval_files/async112.py` & `flake8_async-24.4.2/tests/eval_files/async112.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.4.1/tests/eval_files/async113.py` & `flake8_async-24.4.2/tests/eval_files/async113.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.4.1/tests/eval_files/async113_trio.py` & `flake8_async-24.4.2/tests/eval_files/async113_trio.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.4.1/tests/eval_files/async114.py` & `flake8_async-24.4.2/tests/eval_files/async114.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.4.1/tests/eval_files/async115.py` & `flake8_async-24.4.2/tests/eval_files/async115.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.4.1/tests/eval_files/async116.py` & `flake8_async-24.4.2/tests/eval_files/async116.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.4.1/tests/eval_files/async118.py` & `flake8_async-24.4.2/tests/eval_files/async118.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.4.1/tests/eval_files/async200.py` & `flake8_async-24.4.2/tests/eval_files/async200.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.4.1/tests/eval_files/async210.py` & `flake8_async-24.4.2/tests/eval_files/async210.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.4.1/tests/eval_files/async211.py` & `flake8_async-24.4.2/tests/eval_files/async211.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.4.1/tests/eval_files/async212.py` & `flake8_async-24.4.2/tests/eval_files/async212.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.4.1/tests/eval_files/async22x.py` & `flake8_async-24.4.2/tests/eval_files/async22x.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.4.1/tests/eval_files/async22x_asyncio.py` & `flake8_async-24.4.2/tests/eval_files/async22x_asyncio.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.4.1/tests/eval_files/async232.py` & `flake8_async-24.4.2/tests/eval_files/async232.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.4.1/tests/eval_files/async232_asyncio.py` & `flake8_async-24.4.2/tests/eval_files/async232_asyncio.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.4.1/tests/eval_files/async23x.py` & `flake8_async-24.4.2/tests/eval_files/async23x.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.4.1/tests/eval_files/async23x_asyncio.py` & `flake8_async-24.4.2/tests/eval_files/async23x_asyncio.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.4.1/tests/eval_files/async240.py` & `flake8_async-24.4.2/tests/eval_files/async240.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.4.1/tests/eval_files/async900.py` & `flake8_async-24.4.2/tests/eval_files/async900.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.4.1/tests/eval_files/async910.py` & `flake8_async-24.4.2/tests/eval_files/async910.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.4.1/tests/eval_files/async911.py` & `flake8_async-24.4.2/tests/eval_files/async911.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.4.1/tests/eval_files/async91x_autofix.py` & `flake8_async-24.4.2/tests/eval_files/async91x_autofix.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.4.1/tests/eval_files/async91x_noautofix.py` & `flake8_async-24.4.2/tests/eval_files/async91x_noautofix.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.4.1/tests/eval_files/noqa.py` & `flake8_async-24.4.2/tests/eval_files/noqa.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.4.1/tests/test_all_visitors_imported.py` & `flake8_async-24.4.2/tests/test_all_visitors_imported.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.4.1/tests/test_changelog_and_version.py` & `flake8_async-24.4.2/tests/test_changelog_and_version.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.4.1/tests/test_config_and_args.py` & `flake8_async-24.4.2/tests/test_config_and_args.py`

 * *Files 10% similar despite different names*

```diff
@@ -206,14 +206,15 @@
     assert tmp_path.joinpath(".flake8").write_text(
         """
 [flake8]
 trio200-blocking-calls =
   other -> async,
   sync_fns.* -> the_async_equivalent,
 select = ASYNC200
+extend-ignore = E
 """
     )
     assert tmp_path.joinpath("example.py").write_text(
         """
 import sync_fns
 
 async def foo():
@@ -399,7 +400,37 @@
     out, err = capsys.readouterr()
     assert not err
     assert (
         out
         == "./example.py:1:1: ASYNC106 trio must be imported with `import trio` for the"
         " linter to work.\n"
     )
+
+
+@pytest.mark.xfail(reason="flake8>=6 enforces three-letter error codes in config")
+def test_config_ignore_error_code(tmp_path: Path) -> None:
+    assert tmp_path.joinpath(".flake8").write_text(
+        """
+[flake8]
+ignore = ASYNC100
+"""
+    )
+    res = subprocess.run(
+        ["flake8", "--help"], cwd=tmp_path, capture_output=True, check=False
+    )
+    assert not res.stderr
+    assert res.returncode == 0
+
+
+# but make sure we can disable selected codes
+def test_config_disable_error_code(tmp_path: Path) -> None:
+    # select ASYNC200 and create file that induces ASYNC200
+    _test_trio200_from_config_common(tmp_path)
+    # disable ASYNC200
+    with open(tmp_path.joinpath(".flake8"), "a", encoding="utf-8") as file:
+        file.write("disable = ASYNC200")
+
+    # it now returns no errors
+    res = subprocess.run(["flake8"], cwd=tmp_path, capture_output=True, check=True)
+    assert not res.stdout
+    assert not res.stderr
+    assert res.returncode == 0
```

### Comparing `flake8-async-24.4.1/tests/test_decorator.py` & `flake8_async-24.4.2/tests/test_decorator.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.4.1/tests/test_exception_on_invalid_code.py` & `flake8_async-24.4.2/tests/test_exception_on_invalid_code.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.4.1/tests/test_flake8_async.py` & `flake8_async-24.4.2/tests/test_flake8_async.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.4.1/tests/test_messages_documented.py` & `flake8_async-24.4.2/tests/test_messages_documented.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.4.1/tox.ini` & `flake8_async-24.4.2/tox.ini`

 * *Files 19% similar despite different names*

```diff
@@ -16,14 +16,26 @@
     hypothesis
     # 0.3.3 adds py313 support
     hypothesmith >= 0.3.3
     trio
 commands =
     pytest {posargs:-n auto}
 
+[testenv:docs]
+description = Generate docs locally
+deps =
+    sphinx
+    readthedocs-sphinx-ext
+    -r docs/requirements.txt
+allowlist_externals = make
+changedir = docs
+skip_install = True
+commands =
+    make html
+
 # Settings for other tools
 [pytest]
 addopts =
     --tb=native
     --cov=flake8_async
     --cov-branch
     --cov-report=term-missing:skip-covered
```


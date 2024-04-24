# Comparing `tmp/cnlitellm-0.2.0.tar.gz` & `tmp/cnlitellm-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cnlitellm-0.2.0.tar", last modified: Mon Apr 22 09:51:05 2024, max compression
+gzip compressed data, was "cnlitellm-0.2.1.tar", last modified: Wed Apr 24 14:12:37 2024, max compression
```

## Comparing `cnlitellm-0.2.0.tar` & `cnlitellm-0.2.1.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 everfly    (501) staff       (20)        0 2024-04-22 09:51:05.138152 cnlitellm-0.2.0/
--rw-r--r--   0 everfly    (501) staff       (20)       44 2024-03-19 10:47:10.000000 cnlitellm-0.2.0/LICENSE
--rw-r--r--   0 everfly    (501) staff       (20)      448 2024-04-22 09:51:05.137978 cnlitellm-0.2.0/PKG-INFO
--rw-r--r--   0 everfly    (501) staff       (20)       82 2024-03-19 10:47:10.000000 cnlitellm-0.2.0/README.md
-drwxr-xr-x   0 everfly    (501) staff       (20)        0 2024-04-22 09:51:05.132916 cnlitellm-0.2.0/cnlitellm/
--rw-r--r--   0 everfly    (501) staff       (20)        0 2024-03-19 10:47:10.000000 cnlitellm-0.2.0/cnlitellm/__init__.py
-drwxr-xr-x   0 everfly    (501) staff       (20)        0 2024-04-22 09:51:05.133874 cnlitellm-0.2.0/cnlitellm/__pycache__/
--rw-r--r--   0 everfly    (501) staff       (20)      140 2024-03-21 11:21:03.000000 cnlitellm-0.2.0/cnlitellm/__pycache__/__init__.cpython-312.pyc
--rw-r--r--   0 everfly    (501) staff       (20)     1790 2024-03-21 11:21:03.000000 cnlitellm-0.2.0/cnlitellm/__pycache__/models.cpython-312.pyc
--rw-r--r--   0 everfly    (501) staff       (20)    14486 2024-03-29 11:12:45.000000 cnlitellm-0.2.0/cnlitellm/__pycache__/utils.cpython-312.pyc
--rw-r--r--   0 everfly    (501) staff       (20)     1967 2024-04-20 11:21:30.000000 cnlitellm-0.2.0/cnlitellm/api.py
--rw-r--r--   0 everfly    (501) staff       (20)      306 2024-03-19 10:47:10.000000 cnlitellm-0.2.0/cnlitellm/exceptions.py
--rw-r--r--   0 everfly    (501) staff       (20)     1195 2024-03-19 10:47:10.000000 cnlitellm-0.2.0/cnlitellm/models.py
-drwxr-xr-x   0 everfly    (501) staff       (20)        0 2024-04-22 09:51:05.135434 cnlitellm-0.2.0/cnlitellm/providers/
--rw-r--r--   0 everfly    (501) staff       (20)        0 2024-03-19 10:47:10.000000 cnlitellm-0.2.0/cnlitellm/providers/__init__.py
-drwxr-xr-x   0 everfly    (501) staff       (20)        0 2024-04-22 09:51:05.136416 cnlitellm-0.2.0/cnlitellm/providers/__pycache__/
--rw-r--r--   0 everfly    (501) staff       (20)      150 2024-03-21 11:21:03.000000 cnlitellm-0.2.0/cnlitellm/providers/__pycache__/__init__.cpython-312.pyc
--rw-r--r--   0 everfly    (501) staff       (20)     4455 2024-03-29 11:12:45.000000 cnlitellm-0.2.0/cnlitellm/providers/__pycache__/baichuan.cpython-312.pyc
--rw-r--r--   0 everfly    (501) staff       (20)     2682 2024-03-21 11:21:03.000000 cnlitellm-0.2.0/cnlitellm/providers/__pycache__/base_provider.cpython-312.pyc
--rw-r--r--   0 everfly    (501) staff       (20)     4252 2024-03-29 11:12:45.000000 cnlitellm-0.2.0/cnlitellm/providers/__pycache__/minimax.cpython-312.pyc
--rw-r--r--   0 everfly    (501) staff       (20)     4158 2024-03-29 11:12:45.000000 cnlitellm-0.2.0/cnlitellm/providers/__pycache__/moonshot.cpython-312.pyc
--rw-r--r--   0 everfly    (501) staff       (20)     4452 2024-03-29 11:12:45.000000 cnlitellm-0.2.0/cnlitellm/providers/__pycache__/qwen.cpython-312.pyc
--rw-r--r--   0 everfly    (501) staff       (20)     5144 2024-03-29 11:12:45.000000 cnlitellm-0.2.0/cnlitellm/providers/__pycache__/tiangong.cpython-312.pyc
--rw-r--r--   0 everfly    (501) staff       (20)     5051 2024-03-29 11:12:45.000000 cnlitellm-0.2.0/cnlitellm/providers/__pycache__/wenxin.cpython-312.pyc
--rw-r--r--   0 everfly    (501) staff       (20)     3935 2024-03-29 11:12:45.000000 cnlitellm-0.2.0/cnlitellm/providers/__pycache__/zhipu.cpython-312.pyc
--rw-r--r--   0 everfly    (501) staff       (20)      462 2024-03-29 11:12:45.000000 cnlitellm-0.2.0/cnlitellm/providers/a.json
--rw-r--r--   0 everfly    (501) staff       (20)     4622 2024-04-21 23:53:41.000000 cnlitellm-0.2.0/cnlitellm/providers/baichuan.py
--rw-r--r--   0 everfly    (501) staff       (20)     1613 2024-03-19 10:47:10.000000 cnlitellm-0.2.0/cnlitellm/providers/base_provider.py
--rw-r--r--   0 everfly    (501) staff       (20)     8587 2024-04-21 23:32:33.000000 cnlitellm-0.2.0/cnlitellm/providers/coze.py
--rw-r--r--   0 everfly    (501) staff       (20)     6826 2024-04-21 23:46:44.000000 cnlitellm-0.2.0/cnlitellm/providers/dify.py
--rw-r--r--   0 everfly    (501) staff       (20)     6402 2024-04-21 23:32:41.000000 cnlitellm-0.2.0/cnlitellm/providers/fastgpt.py
--rw-r--r--   0 everfly    (501) staff       (20)     4609 2024-04-22 00:05:51.000000 cnlitellm-0.2.0/cnlitellm/providers/minimax.py
--rw-r--r--   0 everfly    (501) staff       (20)     2642 2024-04-22 08:07:48.000000 cnlitellm-0.2.0/cnlitellm/providers/moonshot.py
--rw-r--r--   0 everfly    (501) staff       (20)     5968 2024-04-22 00:06:48.000000 cnlitellm-0.2.0/cnlitellm/providers/qwen.py
--rw-r--r--   0 everfly    (501) staff       (20)     5318 2024-04-22 07:20:13.000000 cnlitellm-0.2.0/cnlitellm/providers/tiangong.py
--rw-r--r--   0 everfly    (501) staff       (20)     5825 2024-04-22 07:25:41.000000 cnlitellm-0.2.0/cnlitellm/providers/wenxin.py
--rw-r--r--   0 everfly    (501) staff       (20)     9369 2024-04-22 07:59:20.000000 cnlitellm-0.2.0/cnlitellm/providers/xunfei.py
--rw-r--r--   0 everfly    (501) staff       (20)     2367 2024-04-17 10:38:01.000000 cnlitellm-0.2.0/cnlitellm/providers/zhipu.py
--rw-r--r--   0 everfly    (501) staff       (20)    11502 2024-04-22 00:20:28.000000 cnlitellm-0.2.0/cnlitellm/utils.py
-drwxr-xr-x   0 everfly    (501) staff       (20)        0 2024-04-22 09:51:05.133541 cnlitellm-0.2.0/cnlitellm.egg-info/
--rw-r--r--   0 everfly    (501) staff       (20)      448 2024-04-22 09:51:05.000000 cnlitellm-0.2.0/cnlitellm.egg-info/PKG-INFO
--rw-r--r--   0 everfly    (501) staff       (20)     1694 2024-04-22 09:51:05.000000 cnlitellm-0.2.0/cnlitellm.egg-info/SOURCES.txt
--rw-r--r--   0 everfly    (501) staff       (20)        1 2024-04-22 09:51:05.000000 cnlitellm-0.2.0/cnlitellm.egg-info/dependency_links.txt
--rw-r--r--   0 everfly    (501) staff       (20)       69 2024-04-22 09:51:05.000000 cnlitellm-0.2.0/cnlitellm.egg-info/requires.txt
--rw-r--r--   0 everfly    (501) staff       (20)       16 2024-04-22 09:51:05.000000 cnlitellm-0.2.0/cnlitellm.egg-info/top_level.txt
-drwxr-xr-x   0 everfly    (501) staff       (20)        0 2024-04-22 09:51:05.136513 cnlitellm-0.2.0/examples/
--rw-r--r--   0 everfly    (501) staff       (20)       48 2024-03-19 10:47:10.000000 cnlitellm-0.2.0/examples/example_usage.py
--rw-r--r--   0 everfly    (501) staff       (20)      406 2024-04-07 09:48:46.000000 cnlitellm-0.2.0/pyproject.toml
--rw-r--r--   0 everfly    (501) staff       (20)      140 2024-04-07 09:38:02.000000 cnlitellm-0.2.0/requirements.txt
--rw-r--r--   0 everfly    (501) staff       (20)       38 2024-04-22 09:51:05.138196 cnlitellm-0.2.0/setup.cfg
--rw-r--r--   0 everfly    (501) staff       (20)      528 2024-04-22 09:48:41.000000 cnlitellm-0.2.0/setup.py
-drwxr-xr-x   0 everfly    (501) staff       (20)        0 2024-04-22 09:51:05.137757 cnlitellm-0.2.0/tests/
--rw-r--r--   0 everfly    (501) staff       (20)        0 2024-03-19 10:47:10.000000 cnlitellm-0.2.0/tests/__init__.py
--rw-r--r--   0 everfly    (501) staff       (20)       65 2024-03-19 10:47:10.000000 cnlitellm-0.2.0/tests/test_api.py
--rw-r--r--   0 everfly    (501) staff       (20)     2000 2024-03-29 11:12:45.000000 cnlitellm-0.2.0/tests/test_baichuan.py
--rw-r--r--   0 everfly    (501) staff       (20)      980 2024-04-20 11:40:33.000000 cnlitellm-0.2.0/tests/test_coze.py
--rw-r--r--   0 everfly    (501) staff       (20)     1416 2024-04-20 10:17:01.000000 cnlitellm-0.2.0/tests/test_fastgpt.py
--rw-r--r--   0 everfly    (501) staff       (20)     2350 2024-03-29 11:12:45.000000 cnlitellm-0.2.0/tests/test_minimax.py
--rw-r--r--   0 everfly    (501) staff       (20)     2882 2024-03-29 11:13:20.000000 cnlitellm-0.2.0/tests/test_moonshot.py
--rw-r--r--   0 everfly    (501) staff       (20)     1693 2024-04-20 03:21:10.000000 cnlitellm-0.2.0/tests/test_moonshot2.py
--rw-r--r--   0 everfly    (501) staff       (20)     1866 2024-03-29 11:12:45.000000 cnlitellm-0.2.0/tests/test_qwen.py
--rw-r--r--   0 everfly    (501) staff       (20)     1947 2024-03-29 11:12:45.000000 cnlitellm-0.2.0/tests/test_tiangong.py
--rw-r--r--   0 everfly    (501) staff       (20)     1911 2024-03-29 11:12:45.000000 cnlitellm-0.2.0/tests/test_wenxin.py
--rw-r--r--   0 everfly    (501) staff       (20)     1555 2024-04-20 09:23:11.000000 cnlitellm-0.2.0/tests/test_zhipu.py
--rw-r--r--   0 everfly    (501) staff       (20)     1405 2024-04-20 09:25:47.000000 cnlitellm-0.2.0/tests/test_zhipu2.py
+drwxr-xr-x   0 everfly    (501) staff       (20)        0 2024-04-24 14:12:37.161248 cnlitellm-0.2.1/
+-rw-r--r--   0 everfly    (501) staff       (20)       44 2024-03-19 10:47:10.000000 cnlitellm-0.2.1/LICENSE
+-rw-r--r--   0 everfly    (501) staff       (20)      448 2024-04-24 14:12:37.161077 cnlitellm-0.2.1/PKG-INFO
+-rw-r--r--   0 everfly    (501) staff       (20)       82 2024-03-19 10:47:10.000000 cnlitellm-0.2.1/README.md
+drwxr-xr-x   0 everfly    (501) staff       (20)        0 2024-04-24 14:12:37.150160 cnlitellm-0.2.1/cnlitellm/
+-rw-r--r--   0 everfly    (501) staff       (20)        0 2024-03-19 10:47:10.000000 cnlitellm-0.2.1/cnlitellm/__init__.py
+drwxr-xr-x   0 everfly    (501) staff       (20)        0 2024-04-24 14:12:37.151633 cnlitellm-0.2.1/cnlitellm/__pycache__/
+-rw-r--r--   0 everfly    (501) staff       (20)      140 2024-03-21 11:21:03.000000 cnlitellm-0.2.1/cnlitellm/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0 everfly    (501) staff       (20)     1790 2024-03-21 11:21:03.000000 cnlitellm-0.2.1/cnlitellm/__pycache__/models.cpython-312.pyc
+-rw-r--r--   0 everfly    (501) staff       (20)    14486 2024-03-29 11:12:45.000000 cnlitellm-0.2.1/cnlitellm/__pycache__/utils.cpython-312.pyc
+-rw-r--r--   0 everfly    (501) staff       (20)     1967 2024-04-20 11:21:30.000000 cnlitellm-0.2.1/cnlitellm/api.py
+-rw-r--r--   0 everfly    (501) staff       (20)      306 2024-03-19 10:47:10.000000 cnlitellm-0.2.1/cnlitellm/exceptions.py
+-rw-r--r--   0 everfly    (501) staff       (20)     1195 2024-03-19 10:47:10.000000 cnlitellm-0.2.1/cnlitellm/models.py
+drwxr-xr-x   0 everfly    (501) staff       (20)        0 2024-04-24 14:12:37.155229 cnlitellm-0.2.1/cnlitellm/providers/
+-rw-r--r--   0 everfly    (501) staff       (20)        0 2024-03-19 10:47:10.000000 cnlitellm-0.2.1/cnlitellm/providers/__init__.py
+drwxr-xr-x   0 everfly    (501) staff       (20)        0 2024-04-24 14:12:37.157216 cnlitellm-0.2.1/cnlitellm/providers/__pycache__/
+-rw-r--r--   0 everfly    (501) staff       (20)      150 2024-03-21 11:21:03.000000 cnlitellm-0.2.1/cnlitellm/providers/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0 everfly    (501) staff       (20)     4455 2024-03-29 11:12:45.000000 cnlitellm-0.2.1/cnlitellm/providers/__pycache__/baichuan.cpython-312.pyc
+-rw-r--r--   0 everfly    (501) staff       (20)     2682 2024-03-21 11:21:03.000000 cnlitellm-0.2.1/cnlitellm/providers/__pycache__/base_provider.cpython-312.pyc
+-rw-r--r--   0 everfly    (501) staff       (20)     4252 2024-03-29 11:12:45.000000 cnlitellm-0.2.1/cnlitellm/providers/__pycache__/minimax.cpython-312.pyc
+-rw-r--r--   0 everfly    (501) staff       (20)     4158 2024-03-29 11:12:45.000000 cnlitellm-0.2.1/cnlitellm/providers/__pycache__/moonshot.cpython-312.pyc
+-rw-r--r--   0 everfly    (501) staff       (20)     4452 2024-03-29 11:12:45.000000 cnlitellm-0.2.1/cnlitellm/providers/__pycache__/qwen.cpython-312.pyc
+-rw-r--r--   0 everfly    (501) staff       (20)     5144 2024-03-29 11:12:45.000000 cnlitellm-0.2.1/cnlitellm/providers/__pycache__/tiangong.cpython-312.pyc
+-rw-r--r--   0 everfly    (501) staff       (20)     5051 2024-03-29 11:12:45.000000 cnlitellm-0.2.1/cnlitellm/providers/__pycache__/wenxin.cpython-312.pyc
+-rw-r--r--   0 everfly    (501) staff       (20)     3935 2024-03-29 11:12:45.000000 cnlitellm-0.2.1/cnlitellm/providers/__pycache__/zhipu.cpython-312.pyc
+-rw-r--r--   0 everfly    (501) staff       (20)      462 2024-03-29 11:12:45.000000 cnlitellm-0.2.1/cnlitellm/providers/a.json
+-rw-r--r--   0 everfly    (501) staff       (20)     4622 2024-04-21 23:53:41.000000 cnlitellm-0.2.1/cnlitellm/providers/baichuan.py
+-rw-r--r--   0 everfly    (501) staff       (20)     1613 2024-03-19 10:47:10.000000 cnlitellm-0.2.1/cnlitellm/providers/base_provider.py
+-rw-r--r--   0 everfly    (501) staff       (20)     8848 2024-04-24 10:18:26.000000 cnlitellm-0.2.1/cnlitellm/providers/coze.py
+-rw-r--r--   0 everfly    (501) staff       (20)     6826 2024-04-21 23:46:44.000000 cnlitellm-0.2.1/cnlitellm/providers/dify.py
+-rw-r--r--   0 everfly    (501) staff       (20)     6402 2024-04-21 23:32:41.000000 cnlitellm-0.2.1/cnlitellm/providers/fastgpt.py
+-rw-r--r--   0 everfly    (501) staff       (20)     4609 2024-04-22 00:05:51.000000 cnlitellm-0.2.1/cnlitellm/providers/minimax.py
+-rw-r--r--   0 everfly    (501) staff       (20)     2642 2024-04-22 08:07:48.000000 cnlitellm-0.2.1/cnlitellm/providers/moonshot.py
+-rw-r--r--   0 everfly    (501) staff       (20)     5968 2024-04-22 00:06:48.000000 cnlitellm-0.2.1/cnlitellm/providers/qwen.py
+-rw-r--r--   0 everfly    (501) staff       (20)     5318 2024-04-22 07:20:13.000000 cnlitellm-0.2.1/cnlitellm/providers/tiangong.py
+-rw-r--r--   0 everfly    (501) staff       (20)     5825 2024-04-22 07:25:41.000000 cnlitellm-0.2.1/cnlitellm/providers/wenxin.py
+-rw-r--r--   0 everfly    (501) staff       (20)     9369 2024-04-22 07:59:20.000000 cnlitellm-0.2.1/cnlitellm/providers/xunfei.py
+-rw-r--r--   0 everfly    (501) staff       (20)     2367 2024-04-17 10:38:01.000000 cnlitellm-0.2.1/cnlitellm/providers/zhipu.py
+-rw-r--r--   0 everfly    (501) staff       (20)    11502 2024-04-22 00:20:28.000000 cnlitellm-0.2.1/cnlitellm/utils.py
+drwxr-xr-x   0 everfly    (501) staff       (20)        0 2024-04-24 14:12:37.151018 cnlitellm-0.2.1/cnlitellm.egg-info/
+-rw-r--r--   0 everfly    (501) staff       (20)      448 2024-04-24 14:12:37.000000 cnlitellm-0.2.1/cnlitellm.egg-info/PKG-INFO
+-rw-r--r--   0 everfly    (501) staff       (20)     1694 2024-04-24 14:12:37.000000 cnlitellm-0.2.1/cnlitellm.egg-info/SOURCES.txt
+-rw-r--r--   0 everfly    (501) staff       (20)        1 2024-04-24 14:12:37.000000 cnlitellm-0.2.1/cnlitellm.egg-info/dependency_links.txt
+-rw-r--r--   0 everfly    (501) staff       (20)       69 2024-04-24 14:12:37.000000 cnlitellm-0.2.1/cnlitellm.egg-info/requires.txt
+-rw-r--r--   0 everfly    (501) staff       (20)       16 2024-04-24 14:12:37.000000 cnlitellm-0.2.1/cnlitellm.egg-info/top_level.txt
+drwxr-xr-x   0 everfly    (501) staff       (20)        0 2024-04-24 14:12:37.157453 cnlitellm-0.2.1/examples/
+-rw-r--r--   0 everfly    (501) staff       (20)       48 2024-03-19 10:47:10.000000 cnlitellm-0.2.1/examples/example_usage.py
+-rw-r--r--   0 everfly    (501) staff       (20)      406 2024-04-07 09:48:46.000000 cnlitellm-0.2.1/pyproject.toml
+-rw-r--r--   0 everfly    (501) staff       (20)      140 2024-04-07 09:38:02.000000 cnlitellm-0.2.1/requirements.txt
+-rw-r--r--   0 everfly    (501) staff       (20)       38 2024-04-24 14:12:37.161282 cnlitellm-0.2.1/setup.cfg
+-rw-r--r--   0 everfly    (501) staff       (20)      528 2024-04-24 14:12:02.000000 cnlitellm-0.2.1/setup.py
+drwxr-xr-x   0 everfly    (501) staff       (20)        0 2024-04-24 14:12:37.160594 cnlitellm-0.2.1/tests/
+-rw-r--r--   0 everfly    (501) staff       (20)        0 2024-03-19 10:47:10.000000 cnlitellm-0.2.1/tests/__init__.py
+-rw-r--r--   0 everfly    (501) staff       (20)       65 2024-03-19 10:47:10.000000 cnlitellm-0.2.1/tests/test_api.py
+-rw-r--r--   0 everfly    (501) staff       (20)     2000 2024-03-29 11:12:45.000000 cnlitellm-0.2.1/tests/test_baichuan.py
+-rw-r--r--   0 everfly    (501) staff       (20)      980 2024-04-20 11:40:33.000000 cnlitellm-0.2.1/tests/test_coze.py
+-rw-r--r--   0 everfly    (501) staff       (20)     1416 2024-04-20 10:17:01.000000 cnlitellm-0.2.1/tests/test_fastgpt.py
+-rw-r--r--   0 everfly    (501) staff       (20)     2350 2024-03-29 11:12:45.000000 cnlitellm-0.2.1/tests/test_minimax.py
+-rw-r--r--   0 everfly    (501) staff       (20)     2882 2024-03-29 11:13:20.000000 cnlitellm-0.2.1/tests/test_moonshot.py
+-rw-r--r--   0 everfly    (501) staff       (20)     1693 2024-04-20 03:21:10.000000 cnlitellm-0.2.1/tests/test_moonshot2.py
+-rw-r--r--   0 everfly    (501) staff       (20)     1866 2024-03-29 11:12:45.000000 cnlitellm-0.2.1/tests/test_qwen.py
+-rw-r--r--   0 everfly    (501) staff       (20)     1947 2024-03-29 11:12:45.000000 cnlitellm-0.2.1/tests/test_tiangong.py
+-rw-r--r--   0 everfly    (501) staff       (20)     1911 2024-03-29 11:12:45.000000 cnlitellm-0.2.1/tests/test_wenxin.py
+-rw-r--r--   0 everfly    (501) staff       (20)     1555 2024-04-20 09:23:11.000000 cnlitellm-0.2.1/tests/test_zhipu.py
+-rw-r--r--   0 everfly    (501) staff       (20)     1405 2024-04-20 09:25:47.000000 cnlitellm-0.2.1/tests/test_zhipu2.py
```

### Comparing `cnlitellm-0.2.0/cnlitellm/__pycache__/models.cpython-312.pyc` & `cnlitellm-0.2.1/cnlitellm/__pycache__/models.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `cnlitellm-0.2.0/cnlitellm/__pycache__/utils.cpython-312.pyc` & `cnlitellm-0.2.1/cnlitellm/__pycache__/utils.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `cnlitellm-0.2.0/cnlitellm/api.py` & `cnlitellm-0.2.1/cnlitellm/api.py`

 * *Files identical despite different names*

### Comparing `cnlitellm-0.2.0/cnlitellm/models.py` & `cnlitellm-0.2.1/cnlitellm/models.py`

 * *Files identical despite different names*

### Comparing `cnlitellm-0.2.0/cnlitellm/providers/__pycache__/baichuan.cpython-312.pyc` & `cnlitellm-0.2.1/cnlitellm/providers/__pycache__/baichuan.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `cnlitellm-0.2.0/cnlitellm/providers/__pycache__/base_provider.cpython-312.pyc` & `cnlitellm-0.2.1/cnlitellm/providers/__pycache__/base_provider.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `cnlitellm-0.2.0/cnlitellm/providers/__pycache__/minimax.cpython-312.pyc` & `cnlitellm-0.2.1/cnlitellm/providers/__pycache__/minimax.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `cnlitellm-0.2.0/cnlitellm/providers/__pycache__/moonshot.cpython-312.pyc` & `cnlitellm-0.2.1/cnlitellm/providers/__pycache__/moonshot.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `cnlitellm-0.2.0/cnlitellm/providers/__pycache__/qwen.cpython-312.pyc` & `cnlitellm-0.2.1/cnlitellm/providers/__pycache__/qwen.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `cnlitellm-0.2.0/cnlitellm/providers/__pycache__/tiangong.cpython-312.pyc` & `cnlitellm-0.2.1/cnlitellm/providers/__pycache__/tiangong.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `cnlitellm-0.2.0/cnlitellm/providers/__pycache__/wenxin.cpython-312.pyc` & `cnlitellm-0.2.1/cnlitellm/providers/__pycache__/wenxin.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `cnlitellm-0.2.0/cnlitellm/providers/__pycache__/zhipu.cpython-312.pyc` & `cnlitellm-0.2.1/cnlitellm/providers/__pycache__/zhipu.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `cnlitellm-0.2.0/cnlitellm/providers/baichuan.py` & `cnlitellm-0.2.1/cnlitellm/providers/baichuan.py`

 * *Files identical despite different names*

### Comparing `cnlitellm-0.2.0/cnlitellm/providers/base_provider.py` & `cnlitellm-0.2.1/cnlitellm/providers/base_provider.py`

 * *Files identical despite different names*

### Comparing `cnlitellm-0.2.0/cnlitellm/providers/coze.py` & `cnlitellm-0.2.1/cnlitellm/providers/coze.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,25 +111,33 @@
         context = []
 
         result_dict = result.json()
         messages = result_dict.get('messages', [])
         results = []
         cotext_pre = []
 
+        print("messages is:",messages)
+
         for message in messages:
             # 根据消息类型处理数据
             if message['role'] == 'assistant' and message['type'] == 'knowledge':
                 # 解析知识型内容
                 content = message['content']
+                print("content is:",content)
+
                 # 假设knowledge类型内容是由"---\nrecall slice X:\n"分隔的
                 slices = content.split('---\n')
                 for slice in slices:
                     if slice.strip().startswith('recall slice'):
                         # 去掉前缀找到JSON部分
                         json_part = slice.strip().split('\n', 1)[-1].strip()
+                        # 如果不是以\"}结尾，则强制添加
+                        if not json_part.endswith('\"}'):
+                            json_part += '\"}'
+
                         try:
                             # 尝试解析JSON数据
                             recall_data = json.loads(json_part)
                             cotext_pre.append(str(recall_data))
                         except json.JSONDecodeError:
                             raise CozeAIError(status_code=500, message=f"Error decoding JSON from slice: {json_part}")
```

### Comparing `cnlitellm-0.2.0/cnlitellm/providers/dify.py` & `cnlitellm-0.2.1/cnlitellm/providers/dify.py`

 * *Files identical despite different names*

### Comparing `cnlitellm-0.2.0/cnlitellm/providers/fastgpt.py` & `cnlitellm-0.2.1/cnlitellm/providers/fastgpt.py`

 * *Files identical despite different names*

### Comparing `cnlitellm-0.2.0/cnlitellm/providers/minimax.py` & `cnlitellm-0.2.1/cnlitellm/providers/minimax.py`

 * *Files identical despite different names*

### Comparing `cnlitellm-0.2.0/cnlitellm/providers/moonshot.py` & `cnlitellm-0.2.1/cnlitellm/providers/moonshot.py`

 * *Files identical despite different names*

### Comparing `cnlitellm-0.2.0/cnlitellm/providers/qwen.py` & `cnlitellm-0.2.1/cnlitellm/providers/qwen.py`

 * *Files identical despite different names*

### Comparing `cnlitellm-0.2.0/cnlitellm/providers/tiangong.py` & `cnlitellm-0.2.1/cnlitellm/providers/tiangong.py`

 * *Files identical despite different names*

### Comparing `cnlitellm-0.2.0/cnlitellm/providers/wenxin.py` & `cnlitellm-0.2.1/cnlitellm/providers/wenxin.py`

 * *Files identical despite different names*

### Comparing `cnlitellm-0.2.0/cnlitellm/providers/xunfei.py` & `cnlitellm-0.2.1/cnlitellm/providers/xunfei.py`

 * *Files identical despite different names*

### Comparing `cnlitellm-0.2.0/cnlitellm/providers/zhipu.py` & `cnlitellm-0.2.1/cnlitellm/providers/zhipu.py`

 * *Files identical despite different names*

### Comparing `cnlitellm-0.2.0/cnlitellm/utils.py` & `cnlitellm-0.2.1/cnlitellm/utils.py`

 * *Files identical despite different names*

### Comparing `cnlitellm-0.2.0/cnlitellm.egg-info/SOURCES.txt` & `cnlitellm-0.2.1/cnlitellm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cnlitellm-0.2.0/setup.py` & `cnlitellm-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='cnlitellm',
-    version='0.2.0',
+    version='0.2.1',
     packages=find_packages(),
     license='MIT',
     description='A Python library for unified access to Chinese domestic large language models.',
     author='everfly',
     author_email='tagriver@gmail.com',
     url='https://github.com/EvalsOne/CNLiteLLM',
     install_requires=[
```

### Comparing `cnlitellm-0.2.0/tests/test_baichuan.py` & `cnlitellm-0.2.1/tests/test_baichuan.py`

 * *Files identical despite different names*

### Comparing `cnlitellm-0.2.0/tests/test_coze.py` & `cnlitellm-0.2.1/tests/test_coze.py`

 * *Files identical despite different names*

### Comparing `cnlitellm-0.2.0/tests/test_fastgpt.py` & `cnlitellm-0.2.1/tests/test_fastgpt.py`

 * *Files identical despite different names*

### Comparing `cnlitellm-0.2.0/tests/test_minimax.py` & `cnlitellm-0.2.1/tests/test_minimax.py`

 * *Files identical despite different names*

### Comparing `cnlitellm-0.2.0/tests/test_moonshot.py` & `cnlitellm-0.2.1/tests/test_moonshot.py`

 * *Files identical despite different names*

### Comparing `cnlitellm-0.2.0/tests/test_moonshot2.py` & `cnlitellm-0.2.1/tests/test_moonshot2.py`

 * *Files identical despite different names*

### Comparing `cnlitellm-0.2.0/tests/test_qwen.py` & `cnlitellm-0.2.1/tests/test_qwen.py`

 * *Files identical despite different names*

### Comparing `cnlitellm-0.2.0/tests/test_tiangong.py` & `cnlitellm-0.2.1/tests/test_tiangong.py`

 * *Files identical despite different names*

### Comparing `cnlitellm-0.2.0/tests/test_wenxin.py` & `cnlitellm-0.2.1/tests/test_wenxin.py`

 * *Files identical despite different names*

### Comparing `cnlitellm-0.2.0/tests/test_zhipu.py` & `cnlitellm-0.2.1/tests/test_zhipu.py`

 * *Files identical despite different names*

### Comparing `cnlitellm-0.2.0/tests/test_zhipu2.py` & `cnlitellm-0.2.1/tests/test_zhipu2.py`

 * *Files identical despite different names*


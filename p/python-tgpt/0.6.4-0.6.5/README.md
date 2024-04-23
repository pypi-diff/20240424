# Comparing `tmp/python_tgpt-0.6.4.tar.gz` & `tmp/python_tgpt-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_tgpt-0.6.4.tar", last modified: Tue Apr 23 10:48:57 2024, max compression
+gzip compressed data, was "python_tgpt-0.6.5.tar", last modified: Tue Apr 23 22:20:13 2024, max compression
```

## Comparing `python_tgpt-0.6.4.tar` & `python_tgpt-0.6.5.tar`

### file list

```diff
@@ -1,94 +1,97 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 10:48:57.814113 python_tgpt-0.6.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-23 10:48:27.000000 python_tgpt-0.6.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    19654 2024-04-23 10:48:57.814113 python_tgpt-0.6.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    16775 2024-04-23 10:48:57.000000 python_tgpt-0.6.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 10:48:57.814113 python_tgpt-0.6.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3179 2024-04-23 10:48:27.000000 python_tgpt-0.6.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 10:48:57.798114 python_tgpt-0.6.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 10:48:57.802114 python_tgpt-0.6.4/src/pytgpt/
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-23 10:48:27.000000 python_tgpt-0.6.4/src/pytgpt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-23 10:48:27.000000 python_tgpt-0.6.4/src/pytgpt/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 10:48:57.802114 python_tgpt-0.6.4/src/pytgpt/api/
--rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-04-23 10:48:27.000000 python_tgpt-0.6.4/src/pytgpt/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-23 10:48:27.000000 python_tgpt-0.6.4/src/pytgpt/api/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-04-23 10:48:27.000000 python_tgpt-0.6.4/src/pytgpt/api/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    12434 2024-04-23 10:48:27.000000 python_tgpt-0.6.4/src/pytgpt/api/v1.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 10:48:57.802114 python_tgpt-0.6.4/src/pytgpt/auto/
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-23 10:48:27.000000 python_tgpt-0.6.4/src/pytgpt/auto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-23 10:48:27.000000 python_tgpt-0.6.4/src/pytgpt/auto/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     7999 2024-04-23 10:48:27.000000 python_tgpt-0.6.4/src/pytgpt/auto/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-04-23 10:48:27.000000 python_tgpt-0.6.4/src/pytgpt/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 10:48:57.802114 python_tgpt-0.6.4/src/pytgpt/blackboxai/
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-23 10:48:27.000000 python_tgpt-0.6.4/src/pytgpt/blackboxai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7753 2024-04-23 10:48:27.000000 python_tgpt-0.6.4/src/pytgpt/blackboxai/main.py
--rw-r--r--   0 runner    (1001) docker     (127)    81305 2024-04-23 10:48:27.000000 python_tgpt-0.6.4/src/pytgpt/console.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 10:48:57.802114 python_tgpt-0.6.4/src/pytgpt/gemini/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-23 10:48:27.000000 python_tgpt-0.6.4/src/pytgpt/gemini/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7460 2024-04-23 10:48:27.000000 python_tgpt-0.6.4/src/pytgpt/gemini/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 10:48:57.802114 python_tgpt-0.6.4/src/pytgpt/gpt4all/
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-23 10:48:27.000000 python_tgpt-0.6.4/src/pytgpt/gpt4all/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7595 2024-04-23 10:48:27.000000 python_tgpt-0.6.4/src/pytgpt/gpt4all/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 10:48:57.802114 python_tgpt-0.6.4/src/pytgpt/gpt4free/
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-23 10:48:27.000000 python_tgpt-0.6.4/src/pytgpt/gpt4free/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9078 2024-04-23 10:48:27.000000 python_tgpt-0.6.4/src/pytgpt/gpt4free/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     7293 2024-04-23 10:48:27.000000 python_tgpt-0.6.4/src/pytgpt/gpt4free/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 10:48:57.802114 python_tgpt-0.6.4/src/pytgpt/groq/
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-23 10:48:27.000000 python_tgpt-0.6.4/src/pytgpt/groq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10062 2024-04-23 10:48:27.000000 python_tgpt-0.6.4/src/pytgpt/groq/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 10:48:57.806114 python_tgpt-0.6.4/src/pytgpt/imager/
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-23 10:48:27.000000 python_tgpt-0.6.4/src/pytgpt/imager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4020 2024-04-23 10:48:27.000000 python_tgpt-0.6.4/src/pytgpt/imager/imager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 10:48:57.806114 python_tgpt-0.6.4/src/pytgpt/koboldai/
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-23 10:48:27.000000 python_tgpt-0.6.4/src/pytgpt/koboldai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7308 2024-04-23 10:48:27.000000 python_tgpt-0.6.4/src/pytgpt/koboldai/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 10:48:57.806114 python_tgpt-0.6.4/src/pytgpt/leo/
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-23 10:48:27.000000 python_tgpt-0.6.4/src/pytgpt/leo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9685 2024-04-23 10:48:27.000000 python_tgpt-0.6.4/src/pytgpt/leo/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 10:48:57.806114 python_tgpt-0.6.4/src/pytgpt/llama2/
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-23 10:48:27.000000 python_tgpt-0.6.4/src/pytgpt/llama2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8180 2024-04-23 10:48:27.000000 python_tgpt-0.6.4/src/pytgpt/llama2/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 10:48:57.806114 python_tgpt-0.6.4/src/pytgpt/openai/
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-23 10:48:27.000000 python_tgpt-0.6.4/src/pytgpt/openai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9597 2024-04-23 10:48:27.000000 python_tgpt-0.6.4/src/pytgpt/openai/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 10:48:57.806114 python_tgpt-0.6.4/src/pytgpt/opengpt/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-23 10:48:27.000000 python_tgpt-0.6.4/src/pytgpt/opengpt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8709 2024-04-23 10:48:27.000000 python_tgpt-0.6.4/src/pytgpt/opengpt/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 10:48:57.806114 python_tgpt-0.6.4/src/pytgpt/perplexity/
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-23 10:48:27.000000 python_tgpt-0.6.4/src/pytgpt/perplexity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7907 2024-04-23 10:48:27.000000 python_tgpt-0.6.4/src/pytgpt/perplexity/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 10:48:57.806114 python_tgpt-0.6.4/src/pytgpt/phind/
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-23 10:48:27.000000 python_tgpt-0.6.4/src/pytgpt/phind/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9139 2024-04-23 10:48:27.000000 python_tgpt-0.6.4/src/pytgpt/phind/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 10:48:57.806114 python_tgpt-0.6.4/src/pytgpt/poe/
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-23 10:48:27.000000 python_tgpt-0.6.4/src/pytgpt/poe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7455 2024-04-23 10:48:27.000000 python_tgpt-0.6.4/src/pytgpt/poe/main.py
--rw-r--r--   0 runner    (1001) docker     (127)    23689 2024-04-23 10:48:27.000000 python_tgpt-0.6.4/src/pytgpt/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 10:48:57.806114 python_tgpt-0.6.4/src/pytgpt/webchatgpt/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-23 10:48:27.000000 python_tgpt-0.6.4/src/pytgpt/webchatgpt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7114 2024-04-23 10:48:27.000000 python_tgpt-0.6.4/src/pytgpt/webchatgpt/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 10:48:57.810114 python_tgpt-0.6.4/src/python_tgpt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    19654 2024-04-23 10:48:57.000000 python_tgpt-0.6.4/src/python_tgpt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1816 2024-04-23 10:48:57.000000 python_tgpt-0.6.4/src/python_tgpt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 10:48:57.000000 python_tgpt-0.6.4/src/python_tgpt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-23 10:48:57.000000 python_tgpt-0.6.4/src/python_tgpt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-04-23 10:48:57.000000 python_tgpt-0.6.4/src/python_tgpt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-23 10:48:57.000000 python_tgpt-0.6.4/src/python_tgpt.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 10:48:57.810114 python_tgpt-0.6.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3342 2024-04-23 10:48:27.000000 python_tgpt-0.6.4/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-23 10:48:27.000000 python_tgpt-0.6.4/tests/test_auto.py
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-23 10:48:27.000000 python_tgpt-0.6.4/tests/test_blackboxai.py
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-23 10:48:27.000000 python_tgpt-0.6.4/tests/test_gemini.py
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-23 10:48:27.000000 python_tgpt-0.6.4/tests/test_gpt4all.py
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-23 10:48:27.000000 python_tgpt-0.6.4/tests/test_gpt4free.py
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-23 10:48:27.000000 python_tgpt-0.6.4/tests/test_groq.py
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-23 10:48:27.000000 python_tgpt-0.6.4/tests/test_imager.py
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-23 10:48:27.000000 python_tgpt-0.6.4/tests/test_koboldai.py
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-23 10:48:27.000000 python_tgpt-0.6.4/tests/test_leo.py
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-23 10:48:27.000000 python_tgpt-0.6.4/tests/test_llama2.py
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-23 10:48:27.000000 python_tgpt-0.6.4/tests/test_openai.py
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-23 10:48:27.000000 python_tgpt-0.6.4/tests/test_opengpt.py
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-23 10:48:27.000000 python_tgpt-0.6.4/tests/test_perplexity.py
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-23 10:48:27.000000 python_tgpt-0.6.4/tests/test_phind.py
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-23 10:48:27.000000 python_tgpt-0.6.4/tests/test_poe.py
--rw-r--r--   0 runner    (1001) docker     (127)     4202 2024-04-23 10:48:27.000000 python_tgpt-0.6.4/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-23 10:48:27.000000 python_tgpt-0.6.4/tests/test_webchatgpt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:20:13.925598 python_tgpt-0.6.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-23 22:19:32.000000 python_tgpt-0.6.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    21581 2024-04-23 22:20:13.925598 python_tgpt-0.6.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    18668 2024-04-23 22:20:13.000000 python_tgpt-0.6.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 22:20:13.925598 python_tgpt-0.6.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3205 2024-04-23 22:19:32.000000 python_tgpt-0.6.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:20:13.909598 python_tgpt-0.6.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:20:13.913598 python_tgpt-0.6.5/src/pytgpt/
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-23 22:19:32.000000 python_tgpt-0.6.5/src/pytgpt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-23 22:19:32.000000 python_tgpt-0.6.5/src/pytgpt/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:20:13.913598 python_tgpt-0.6.5/src/pytgpt/api/
+-rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-04-23 22:19:32.000000 python_tgpt-0.6.5/src/pytgpt/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-23 22:19:32.000000 python_tgpt-0.6.5/src/pytgpt/api/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-04-23 22:19:32.000000 python_tgpt-0.6.5/src/pytgpt/api/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17395 2024-04-23 22:19:32.000000 python_tgpt-0.6.5/src/pytgpt/api/v1.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:20:13.913598 python_tgpt-0.6.5/src/pytgpt/auto/
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-23 22:19:32.000000 python_tgpt-0.6.5/src/pytgpt/auto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-23 22:19:32.000000 python_tgpt-0.6.5/src/pytgpt/auto/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7999 2024-04-23 22:19:32.000000 python_tgpt-0.6.5/src/pytgpt/auto/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-04-23 22:19:32.000000 python_tgpt-0.6.5/src/pytgpt/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:20:13.913598 python_tgpt-0.6.5/src/pytgpt/blackboxai/
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-23 22:19:32.000000 python_tgpt-0.6.5/src/pytgpt/blackboxai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7753 2024-04-23 22:19:32.000000 python_tgpt-0.6.5/src/pytgpt/blackboxai/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    84784 2024-04-23 22:19:32.000000 python_tgpt-0.6.5/src/pytgpt/console.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:20:13.913598 python_tgpt-0.6.5/src/pytgpt/gemini/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-23 22:19:32.000000 python_tgpt-0.6.5/src/pytgpt/gemini/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7460 2024-04-23 22:19:32.000000 python_tgpt-0.6.5/src/pytgpt/gemini/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:20:13.913598 python_tgpt-0.6.5/src/pytgpt/gpt4all/
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-23 22:19:32.000000 python_tgpt-0.6.5/src/pytgpt/gpt4all/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7595 2024-04-23 22:19:32.000000 python_tgpt-0.6.5/src/pytgpt/gpt4all/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:20:13.913598 python_tgpt-0.6.5/src/pytgpt/gpt4free/
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-23 22:19:32.000000 python_tgpt-0.6.5/src/pytgpt/gpt4free/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9078 2024-04-23 22:19:32.000000 python_tgpt-0.6.5/src/pytgpt/gpt4free/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7293 2024-04-23 22:19:32.000000 python_tgpt-0.6.5/src/pytgpt/gpt4free/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:20:13.917598 python_tgpt-0.6.5/src/pytgpt/groq/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-23 22:19:32.000000 python_tgpt-0.6.5/src/pytgpt/groq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10062 2024-04-23 22:19:32.000000 python_tgpt-0.6.5/src/pytgpt/groq/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:20:13.917598 python_tgpt-0.6.5/src/pytgpt/imager/
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-23 22:19:32.000000 python_tgpt-0.6.5/src/pytgpt/imager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8191 2024-04-23 22:19:32.000000 python_tgpt-0.6.5/src/pytgpt/imager/imager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:20:13.917598 python_tgpt-0.6.5/src/pytgpt/koboldai/
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-23 22:19:32.000000 python_tgpt-0.6.5/src/pytgpt/koboldai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7308 2024-04-23 22:19:32.000000 python_tgpt-0.6.5/src/pytgpt/koboldai/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:20:13.917598 python_tgpt-0.6.5/src/pytgpt/leo/
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-23 22:19:32.000000 python_tgpt-0.6.5/src/pytgpt/leo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9685 2024-04-23 22:19:32.000000 python_tgpt-0.6.5/src/pytgpt/leo/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:20:13.917598 python_tgpt-0.6.5/src/pytgpt/llama2/
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-23 22:19:32.000000 python_tgpt-0.6.5/src/pytgpt/llama2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8180 2024-04-23 22:19:32.000000 python_tgpt-0.6.5/src/pytgpt/llama2/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:20:13.917598 python_tgpt-0.6.5/src/pytgpt/openai/
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-23 22:19:32.000000 python_tgpt-0.6.5/src/pytgpt/openai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9597 2024-04-23 22:19:32.000000 python_tgpt-0.6.5/src/pytgpt/openai/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:20:13.917598 python_tgpt-0.6.5/src/pytgpt/opengpt/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-23 22:19:32.000000 python_tgpt-0.6.5/src/pytgpt/opengpt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8709 2024-04-23 22:19:32.000000 python_tgpt-0.6.5/src/pytgpt/opengpt/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:20:13.917598 python_tgpt-0.6.5/src/pytgpt/perplexity/
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-23 22:19:32.000000 python_tgpt-0.6.5/src/pytgpt/perplexity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7907 2024-04-23 22:19:32.000000 python_tgpt-0.6.5/src/pytgpt/perplexity/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:20:13.917598 python_tgpt-0.6.5/src/pytgpt/phind/
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-23 22:19:32.000000 python_tgpt-0.6.5/src/pytgpt/phind/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9139 2024-04-23 22:19:32.000000 python_tgpt-0.6.5/src/pytgpt/phind/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:20:13.917598 python_tgpt-0.6.5/src/pytgpt/poe/
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-23 22:19:32.000000 python_tgpt-0.6.5/src/pytgpt/poe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7455 2024-04-23 22:19:32.000000 python_tgpt-0.6.5/src/pytgpt/poe/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33719 2024-04-23 22:19:32.000000 python_tgpt-0.6.5/src/pytgpt/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:20:13.917598 python_tgpt-0.6.5/src/pytgpt/webchatgpt/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-23 22:19:32.000000 python_tgpt-0.6.5/src/pytgpt/webchatgpt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7114 2024-04-23 22:19:32.000000 python_tgpt-0.6.5/src/pytgpt/webchatgpt/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:20:13.917598 python_tgpt-0.6.5/src/pytgpt/yepchat/
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-23 22:19:32.000000 python_tgpt-0.6.5/src/pytgpt/yepchat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9434 2024-04-23 22:19:32.000000 python_tgpt-0.6.5/src/pytgpt/yepchat/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:20:13.921598 python_tgpt-0.6.5/src/python_tgpt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    21581 2024-04-23 22:20:13.000000 python_tgpt-0.6.5/src/python_tgpt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-04-23 22:20:13.000000 python_tgpt-0.6.5/src/python_tgpt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 22:20:13.000000 python_tgpt-0.6.5/src/python_tgpt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-23 22:20:13.000000 python_tgpt-0.6.5/src/python_tgpt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-23 22:20:13.000000 python_tgpt-0.6.5/src/python_tgpt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-23 22:20:13.000000 python_tgpt-0.6.5/src/python_tgpt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:20:13.921598 python_tgpt-0.6.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3342 2024-04-23 22:19:32.000000 python_tgpt-0.6.5/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-23 22:19:32.000000 python_tgpt-0.6.5/tests/test_auto.py
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-23 22:19:32.000000 python_tgpt-0.6.5/tests/test_blackboxai.py
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-23 22:19:32.000000 python_tgpt-0.6.5/tests/test_gemini.py
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-23 22:19:32.000000 python_tgpt-0.6.5/tests/test_gpt4all.py
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-23 22:19:32.000000 python_tgpt-0.6.5/tests/test_gpt4free.py
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-23 22:19:32.000000 python_tgpt-0.6.5/tests/test_groq.py
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-23 22:19:32.000000 python_tgpt-0.6.5/tests/test_imager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-23 22:19:32.000000 python_tgpt-0.6.5/tests/test_koboldai.py
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-23 22:19:32.000000 python_tgpt-0.6.5/tests/test_leo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-23 22:19:32.000000 python_tgpt-0.6.5/tests/test_llama2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-23 22:19:32.000000 python_tgpt-0.6.5/tests/test_openai.py
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-23 22:19:32.000000 python_tgpt-0.6.5/tests/test_opengpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-23 22:19:32.000000 python_tgpt-0.6.5/tests/test_perplexity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-23 22:19:32.000000 python_tgpt-0.6.5/tests/test_phind.py
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-23 22:19:32.000000 python_tgpt-0.6.5/tests/test_poe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4202 2024-04-23 22:19:32.000000 python_tgpt-0.6.5/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-23 22:19:32.000000 python_tgpt-0.6.5/tests/test_webchatgpt.py
```

### Comparing `python_tgpt-0.6.4/LICENSE` & `python_tgpt-0.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.6.4/PKG-INFO` & `python_tgpt-0.6.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-tgpt
-Version: 0.6.4
+Version: 0.6.5
 Summary: Interact with AI without API key
 Home-page: https://github.com/Simatwa/python-tgpt
 Author: Smartwa
 Author-email: simatwacaleb@proton.me
 Maintainer: Smartwa
 License: MIT
 Project-URL: Bug Report, https://github.com/Simatwa/python-tgpt/issues/new
@@ -36,14 +36,15 @@
 Requires-Dist: pyyaml==6.0.1
 Requires-Dist: webchatgpt==0.3.0
 Requires-Dist: GoogleBard1>=2.1.4
 Requires-Dist: poe-api-wrapper==1.3.6
 Requires-Dist: brotli==1.1.0
 Requires-Dist: g4f>=0.2.6.1
 Requires-Dist: Helpingai-T2==0.3
+Requires-Dist: python-vlc>=3.0.20
 Provides-Extra: cli
 Requires-Dist: click==8.1.3; extra == "cli"
 Requires-Dist: rich==13.3.4; extra == "cli"
 Requires-Dist: clipman==3.1.0; extra == "cli"
 Requires-Dist: pyperclip==1.8.2; extra == "cli"
 Requires-Dist: colorama==0.4.6; extra == "cli"
 Requires-Dist: g4f>=0.2.6.1; extra == "cli"
@@ -147,14 +148,15 @@
 9. [Phind](https://www.phind.com)
 10. [Llama2](https://www.llama2.ai)
 11. [Blackboxai](https://www.blackbox.ai)
 12. [gpt4all](https://gpt4all.io) *(Offline)*
 13. [Poe](https://poe.com) - Poe|Quora *(Session ID required)*
 14. [Groq](https://console.groq.com/playground) *(API Key required)*
 15. [Perplexity](https://www.perplexity.ai)
+16. [YepChat](https://yep.com)
 
 
 <details>
 
 <summary>
 
 41+ providers proudly offered by [gpt4free](https://github.com/xtekky/gpt4free).
@@ -463,14 +465,25 @@
 img.save(img_generator)
 
 # RAM friendly
 ```
 
 </details>
 
+#### Using **Prodia** provider
+
+```python
+from pytgpt.imager import Prodia
+
+img = Prodia()
+
+img_generator = img.generate('Coding bot', amount=3, stream=True)
+
+img.save(img_generator)
+```
 
 </details>
 
 ### Advanced Usage of Placeholders
 
 The `generate` functionality has been enhanced starting from *v0.3.0* to enable comprehensive utilization of the `--with-copied` option and support for accepting piped inputs. This improvement introduces placeholders, offering dynamic values for more versatile interactions.
 
@@ -533,21 +546,59 @@
 
 The environment variables can be overridden by explicitly declaring new value.
 
 > [!TIP]
 > Save the variables in a `.env` file in your current directory or export them in your `~/.zshrc` file.
 > To load previous conversations from a `.txt` file, use the `-fp` or `--filepath` flag. If no flag is passed, the default one will be used. To load context from a file without altering its content, use the `--retain-file` flag.
 
-## Dynamic Provider
+## Dynamic Provider & Further Interfaces
 
 Version **0.4.6** also introduces dynamic provider called `g4fauto`, which represents the fastest working g4f-based provider.
 
 > [!TIP]
-> To launch web interface for g4f-based providers simply run `$ pytgpt gpt4free gui`. 
+> To launch web interface for g4f-based providers simply run `$ pytgpt gpt4free gui`.
 > `$ pytgpt api run` will start the REST-API. Access docs and redoc at */docs* and */redoc* respectively.
+To launch the web interface for g4f-based providers, execute the following command in your terminal:
+
+```bash
+$ pytgpt gpt4free gui
+```
+
+This command initializes the Web-user interface for interacting with g4f-based providers.
+
+To start the REST-API:
+
+```bash
+$ pytgpt api run
+```
+
+This command starts the RESTful API server, enabling you to interact with the service programmatically.
+
+For accessing the documentation and redoc, navigate to the following paths in your web browser:
+- Documentation: `*/docs`
+- ReDoc: `*/redoc`
+
+## Speech Synthesis
+
+To enable speech synthesis of responses, ensure you have either the [VLC player](https://www.videolan.org/vlc/index.html) installed on your system or, if you are a [Termux](https://termux.org) user, the [Termux:API](https://wiki.termux.com/wiki/Termux:API) package.
+
+To activate speech synthesis, use the `--talk-to-me` flag or its shorthand `-ttm` when running your commands. For example:
+```bash
+$ pytgpt generate "Generate an ogre story" --talk-to-me
+```
+or
+```bash
+$ pytgpt interactive -ttm
+```
+This flag instructs the system to audiolize the ai responses and then play them, enhancing the user experience by providing auditory feedback.
+
+> To speech synthesise the responses just ensure you have [vlc player]() in your system or [termux-api](https://wiki.termux.com/wiki/Termux:API) for the case of [Termux](https://termux.org) users.
+> Use the flag `--talk-to-me`, shortform `-ttm`.
+
+Version **0.6.4** introduces another dynamic provider, `auto`, which denotes the working provider **overall**. This relieves you of the workload of manually checking a working provider each time you fire up pytgpt.
 
 <details>
 
 <summary>
 
 For more usage info run `$ pytgpt --help`
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: python-tgpt Version: 0.6.4 Summary: Interact with
+Metadata-Version: 2.1 Name: python-tgpt Version: 0.6.5 Summary: Interact with
 AI without API key Home-page: https://github.com/Simatwa/python-tgpt Author:
 Smartwa Author-email: simatwacaleb@proton.me Maintainer: Smartwa License: MIT
 Project-URL: Bug Report, https://github.com/Simatwa/python-tgpt/issues/new
 Project-URL: Homepage, https://github.com/Simatwa/python-tgpt Project-URL:
 Source Code, https://github.com/Simatwa/python-tgpt Project-URL: Issue Tracker,
 https://github.com/Simatwa/python-tgpt/issues Project-URL: Download, https://
 github.com/Simatwa/python-tgpt/releases Project-URL: Documentation, https://
@@ -20,27 +20,28 @@
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12 Requires-Python: >=3.10
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 requests[socks]==2.31.0 Requires-Dist: appdirs==1.4.4 Requires-Dist:
 pyyaml==6.0.1 Requires-Dist: webchatgpt==0.3.0 Requires-Dist:
 GoogleBard1>=2.1.4 Requires-Dist: poe-api-wrapper==1.3.6 Requires-Dist:
 brotli==1.1.0 Requires-Dist: g4f>=0.2.6.1 Requires-Dist: Helpingai-T2==0.3
-Provides-Extra: cli Requires-Dist: click==8.1.3; extra == "cli" Requires-Dist:
-rich==13.3.4; extra == "cli" Requires-Dist: clipman==3.1.0; extra == "cli"
-Requires-Dist: pyperclip==1.8.2; extra == "cli" Requires-Dist: colorama==0.4.6;
-extra == "cli" Requires-Dist: g4f>=0.2.6.1; extra == "cli" Requires-Dist:
-python-dotenv==1.0.0; extra == "cli" Provides-Extra: api Requires-Dist: fastapi
-[all]==0.110.1; extra == "api" Provides-Extra: all Requires-Dist: g4f
-[all]>=0.2.6.1; extra == "all" Requires-Dist: matplotlib; extra == "all"
-Requires-Dist: gpt4all==2.2.0; extra == "all" Requires-Dist: click==8.1.3;
-extra == "all" Requires-Dist: rich==13.3.4; extra == "all" Requires-Dist:
-clipman==3.1.0; extra == "all" Requires-Dist: pyperclip==1.8.2; extra == "all"
-Requires-Dist: colorama==0.4.6; extra == "all" Requires-Dist: g4f>=0.2.6.1;
-extra == "all" Requires-Dist: python-dotenv==1.0.0; extra == "all" Requires-
-Dist: fastapi[all]==0.110.1; extra == "all"
+Requires-Dist: python-vlc>=3.0.20 Provides-Extra: cli Requires-Dist:
+click==8.1.3; extra == "cli" Requires-Dist: rich==13.3.4; extra == "cli"
+Requires-Dist: clipman==3.1.0; extra == "cli" Requires-Dist: pyperclip==1.8.2;
+extra == "cli" Requires-Dist: colorama==0.4.6; extra == "cli" Requires-Dist:
+g4f>=0.2.6.1; extra == "cli" Requires-Dist: python-dotenv==1.0.0; extra ==
+"cli" Provides-Extra: api Requires-Dist: fastapi[all]==0.110.1; extra == "api"
+Provides-Extra: all Requires-Dist: g4f[all]>=0.2.6.1; extra == "all" Requires-
+Dist: matplotlib; extra == "all" Requires-Dist: gpt4all==2.2.0; extra == "all"
+Requires-Dist: click==8.1.3; extra == "all" Requires-Dist: rich==13.3.4; extra
+== "all" Requires-Dist: clipman==3.1.0; extra == "all" Requires-Dist:
+pyperclip==1.8.2; extra == "all" Requires-Dist: colorama==0.4.6; extra == "all"
+Requires-Dist: g4f>=0.2.6.1; extra == "all" Requires-Dist: python-
+dotenv==1.0.0; extra == "all" Requires-Dist: fastapi[all]==0.110.1; extra ==
+"all"
 [https://github.com/Simatwa/python-tgpt/blob/main/assets/py-tgpt.png?raw=true]
 _[_L_i_c_e_n_s_e_]_[_P_y_t_h_o_n_ _v_e_r_s_i_o_n_]_[_P_y_P_i_]_[_B_l_a_c_k_]_[_P_a_s_s_i_n_g_]_[_P_y_t_h_o_n_ _P_a_c_k_a_g_e_ _f_l_o_w_]_[_c_o_v_e_r_a_g_e_]
    _[_D_o_w_n_l_o_a_d_s_]_[_D_o_w_n_l_o_a_d_s_]_[_D_o_w_n_l_o_a_d_s_]_[_L_a_t_e_s_t_ _r_e_l_e_a_s_e_]_[_r_e_l_e_a_s_e_ _d_a_t_e_]_[_h_t_t_p_s_:_/_/
   _h_i_t_s_._s_e_e_y_o_u_f_a_r_m_._c_o_m_/_a_p_i_/_c_o_u_n_t_/_i_n_c_r_/_b_a_d_g_e_._s_v_g_?_u_r_l_=_h_t_t_p_s_%_3_A_%_2_F_%_2_F_g_i_t_h_u_b_._c_o_m_/
                         _S_i_m_a_t_w_a_/_p_y_t_h_o_n_-_t_g_p_t_]_[_w_a_k_a_t_i_m_e_]
                              ******** ppyytthhoonn--ttggpptt ********
  [https://github.com/Simatwa/python-tgpt/blob/main/assets/demo-1.gif?raw=True]
@@ -69,37 +70,38 @@
 uc.a.run.app/) 4. [OpenAI](https://chat.openai.com) *(API key required)* 5.
 [WebChatGPT](https://github.com/Simatwa/WebChatGPT) - **OpenAI** *(Session ID
 required)* 6. [Gemini](https://github.com/Simatwa/bard) - **Google** *(Session
 ID required)* 9. [Phind](https://www.phind.com) 10. [Llama2](https://
 www.llama2.ai) 11. [Blackboxai](https://www.blackbox.ai) 12. [gpt4all](https://
 gpt4all.io) *(Offline)* 13. [Poe](https://poe.com) - Poe|Quora *(Session ID
 required)* 14. [Groq](https://console.groq.com/playground) *(API Key required)*
-15. [Perplexity](https://www.perplexity.ai) 41+ providers proudly offered by
-[gpt4free](https://github.com/xtekky/gpt4free). - To list working providers
-run: ```sh $ pytgpt gpt4free test -y ``` ## Prerequisites - [x] [Python>=3.10]
-(https://python.org) *(Optional)* ## Installation and Usage ### Installation
-Download binaries for your system from [here.](https://github.com/Simatwa/
-python-tgpt/releases/latest/) Alternatively, you can install non-binaries. *
-(Recommended)* 1. Developers: ```sh pip install --upgrade python-tgpt ``` 2.
-Commandline: ```sh pip install --upgrade "python-tgpt[cli]" ``` 3. Full
-installation: ```sh pip install --upgrade "python-tgpt[all]" ``` > `pip install
--U "python-tgt[api]"` will install REST API dependencies. ## Usage This package
-offers a convenient command-line interface. > [!NOTE] > `phind` is the default
-*provider*. - For a quick response: ```bash python -m pytgpt generate "" ``` -
-For interactive mode: ```bash python -m pytgpt interactive "" ``` Make use of
-flag `--provider` followed by the provider name of your choice. e.g `--provider
-koboldai` > To list all providers offered by gpt4free, use following commands:
-```pytgpt gpt4free list providers``` You can also simply use `pytgpt` instead
-of `python -m pytgpt`. Starting from version 0.2.7, running `$ pytgpt` without
-any other command or option will automatically enter the `interactive` mode.
-Otherwise, you'll need to explicitly declare the desired action, for example,
-by running `$ pytgpt generate`. ### Developer Docs 1. Generate a quick response
-```python from pytgpt.leo import LEO bot = LEO() resp = bot.chat('') print
-(resp) # Output : How may I help you. ``` 2. Get back whole response ```python
-from pytgpt.leo import LEO bot = LEO() resp = bot.ask('
+15. [Perplexity](https://www.perplexity.ai) 16. [YepChat](https://yep.com) 41+
+providers proudly offered by [gpt4free](https://github.com/xtekky/gpt4free). -
+To list working providers run: ```sh $ pytgpt gpt4free test -y ``` ##
+Prerequisites - [x] [Python>=3.10](https://python.org) *(Optional)* ##
+Installation and Usage ### Installation Download binaries for your system from
+[here.](https://github.com/Simatwa/python-tgpt/releases/latest/) Alternatively,
+you can install non-binaries. *(Recommended)* 1. Developers: ```sh pip install
+--upgrade python-tgpt ``` 2. Commandline: ```sh pip install --upgrade "python-
+tgpt[cli]" ``` 3. Full installation: ```sh pip install --upgrade "python-tgpt
+[all]" ``` > `pip install -U "python-tgt[api]"` will install REST API
+dependencies. ## Usage This package offers a convenient command-line interface.
+> [!NOTE] > `phind` is the default *provider*. - For a quick response: ```bash
+python -m pytgpt generate "" ``` - For interactive mode: ```bash python -
+m pytgpt interactive "" ``` Make use of flag `--provider` followed by the
+provider name of your choice. e.g `--provider koboldai` > To list all providers
+offered by gpt4free, use following commands: ```pytgpt gpt4free list
+providers``` You can also simply use `pytgpt` instead of `python -m pytgpt`.
+Starting from version 0.2.7, running `$ pytgpt` without any other command or
+option will automatically enter the `interactive` mode. Otherwise, you'll need
+to explicitly declare the desired action, for example, by running `$ pytgpt
+generate`. ### Developer Docs 1. Generate a quick response ```python from
+pytgpt.leo import LEO bot = LEO() resp = bot.chat('') print(resp) # Output :
+How may I help you. ``` 2. Get back whole response ```python from pytgpt.leo
+import LEO bot = LEO() resp = bot.ask('
  Output """ {'completion': "I'm so excited to share with you the incredible
 experiences...", 'stop_reason': None, 'truncated': False, 'stop': None,
 'model': 'llama-2-13b-chat', 'log_id': 'cmpl-3NmRt5A5Djqo2jXtXLBwJ2',
 'exception': None} """ ``` #### Stream Response Just add parameter `stream`
 with value `true`. 1. Text Generated only ```python from pytgpt.leo import LEO
 bot = LEO() resp = bot.chat('', stream=True) for value in resp: print(value) #
 output """ How may How may I help How may I help you How may I help you today?
@@ -141,25 +143,27 @@
 informed that majority of providers offered by *gpt4free* requires *Google
 Chrome* inorder to function. ### Image Generation This has been made possible
 by [pollinations.ai](https://pollination.ai). ```sh $ pytgpt imager "" # e.g
 pytgpt imager "Coding bot" ``` Developers ```python from pytgpt.imager import
 Imager img = Imager() generated_img = img.generate('Coding bot') # [bytes]
 img.save(generated_img) ``` Download Multiple Images ```python from
 pytgpt.imager import Imager img = Imager() img_generator = img.generate('Coding
-bot', amount=3, stream=True) img.save(img_generator) # RAM friendly ``` ###
-Advanced Usage of Placeholders The `generate` functionality has been enhanced
-starting from *v0.3.0* to enable comprehensive utilization of the `--with-
-copied` option and support for accepting piped inputs. This improvement
-introduces placeholders, offering dynamic values for more versatile
-interactions. | Placeholder | Represents | | ------------ | ----------- | | `{
-{stream}}` | The piped input | | `{{copied}}` | The last copied text | This
-feature is particularly beneficial for intricate operations. For example:
-```bash $ git diff | pytgpt generate "Here is a diff file: {{stream}} Make a
-concise commit message from it, aligning with my commit message history: {
-{copied}}" --shell --new ``` > In this illustration, `{{stream}}` denotes the
+bot', amount=3, stream=True) img.save(img_generator) # RAM friendly ``` ####
+Using **Prodia** provider ```python from pytgpt.imager import Prodia img =
+Prodia() img_generator = img.generate('Coding bot', amount=3, stream=True)
+img.save(img_generator) ``` ### Advanced Usage of Placeholders The `generate`
+functionality has been enhanced starting from *v0.3.0* to enable comprehensive
+utilization of the `--with-copied` option and support for accepting piped
+inputs. This improvement introduces placeholders, offering dynamic values for
+more versatile interactions. | Placeholder | Represents | | ------------ | ----
+------- | | `{{stream}}` | The piped input | | `{{copied}}` | The last copied
+text | This feature is particularly beneficial for intricate operations. For
+example: ```bash $ git diff | pytgpt generate "Here is a diff file: {{stream}}
+Make a concise commit message from it, aligning with my commit message history:
+{{copied}}" --shell --new ``` > In this illustration, `{{stream}}` denotes the
 result of the `$ git diff` operation, while `{{copied}}` signifies the content
 copied from the output of the `$ git log` command. ### Awesome Prompts [These
 prompts](https://github.com/Simatwa/gpt-cli/blob/main/assets/all-
 acts.pdf?raw=True) are designed to guide the AI's behavior or responses in a
 particular direction, encouraging it to exhibit certain characteristics or
 behaviors. The term "awesome-prompt" is not a formal term in AI or machine
 learning literature, but it encapsulates the idea of crafting prompts that are
@@ -192,24 +196,46 @@
 prompt` will take the environment variable `PYTGPT_AWESOME_PROMPT`. > [!NOTE] >
 This is **NOT** limited to any command The environment variables can be
 overridden by explicitly declaring new value. > [!TIP] > Save the variables in
 a `.env` file in your current directory or export them in your `~/.zshrc` file.
 > To load previous conversations from a `.txt` file, use the `-fp` or `--
 filepath` flag. If no flag is passed, the default one will be used. To load
 context from a file without altering its content, use the `--retain-file` flag.
-## Dynamic Provider Version **0.4.6** also introduces dynamic provider called
-`g4fauto`, which represents the fastest working g4f-based provider. > [!TIP] >
-To launch web interface for g4f-based providers simply run `$ pytgpt gpt4free
-gui`. > `$ pytgpt api run` will start the REST-API. Access docs and redoc at */
-docs* and */redoc* respectively. For more usage info run `$ pytgpt --help` ```
-Usage: pytgpt [OPTIONS] COMMAND [ARGS]... Options: -v, --version Show the
-version and exit. -h, --help Show this message and exit. Commands: api FastAPI
-control endpoint awesome Perform CRUD operations on awesome-prompts generate
-Generate a quick response with AI gpt4free Discover gpt4free models, providers
-etc imager Generate images with pollinations.ai interactive Chat with AI
-interactively (Default) utils Utility endpoint for pytgpt webchatgpt Reverse
-Engineered ChatGPT Web-Version ``` ### API Health Status | No. | API | Status |
-|--------|-----|--------| | 1. | [On-render](https://python-tgpt.onrender.com)
-| [cron-job](https://pqfzhmvz.status.cron-job.org/) | ## [CHANGELOG](https://
+## Dynamic Provider & Further Interfaces Version **0.4.6** also introduces
+dynamic provider called `g4fauto`, which represents the fastest working g4f-
+based provider. > [!TIP] > To launch web interface for g4f-based providers
+simply run `$ pytgpt gpt4free gui`. > `$ pytgpt api run` will start the REST-
+API. Access docs and redoc at */docs* and */redoc* respectively. To launch the
+web interface for g4f-based providers, execute the following command in your
+terminal: ```bash $ pytgpt gpt4free gui ``` This command initializes the Web-
+user interface for interacting with g4f-based providers. To start the REST-API:
+```bash $ pytgpt api run ``` This command starts the RESTful API server,
+enabling you to interact with the service programmatically. For accessing the
+documentation and redoc, navigate to the following paths in your web browser: -
+Documentation: `*/docs` - ReDoc: `*/redoc` ## Speech Synthesis To enable speech
+synthesis of responses, ensure you have either the [VLC player](https://
+www.videolan.org/vlc/index.html) installed on your system or, if you are a
+[Termux](https://termux.org) user, the [Termux:API](https://wiki.termux.com/
+wiki/Termux:API) package. To activate speech synthesis, use the `--talk-to-me`
+flag or its shorthand `-ttm` when running your commands. For example: ```bash $
+pytgpt generate "Generate an ogre story" --talk-to-me ``` or ```bash $ pytgpt
+interactive -ttm ``` This flag instructs the system to audiolize the ai
+responses and then play them, enhancing the user experience by providing
+auditory feedback. > To speech synthesise the responses just ensure you have
+[vlc player]() in your system or [termux-api](https://wiki.termux.com/wiki/
+Termux:API) for the case of [Termux](https://termux.org) users. > Use the flag
+`--talk-to-me`, shortform `-ttm`. Version **0.6.4** introduces another dynamic
+provider, `auto`, which denotes the working provider **overall**. This relieves
+you of the workload of manually checking a working provider each time you fire
+up pytgpt. For more usage info run `$ pytgpt --help` ``` Usage: pytgpt
+[OPTIONS] COMMAND [ARGS]... Options: -v, --version Show the version and exit. -
+h, --help Show this message and exit. Commands: api FastAPI control endpoint
+awesome Perform CRUD operations on awesome-prompts generate Generate a quick
+response with AI gpt4free Discover gpt4free models, providers etc imager
+Generate images with pollinations.ai interactive Chat with AI interactively
+(Default) utils Utility endpoint for pytgpt webchatgpt Reverse Engineered
+ChatGPT Web-Version ``` ### API Health Status | No. | API | Status | |--------
+|-----|--------| | 1. | [On-render](https://python-tgpt.onrender.com) | [cron-
+job](https://pqfzhmvz.status.cron-job.org/) | ## [CHANGELOG](https://
 github.com/Simatwa/python-tgpt/blob/main/docs/CHANGELOG.md) ## Acknowledgements
 1. [x] [tgpt](https://github.com/aandrew-me/tgpt) 2. [x] [gpt4free](https://
 github.com/xtekky/gpt4free)
```

### Comparing `python_tgpt-0.6.4/README.md` & `python_tgpt-0.6.5/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -82,14 +82,15 @@
 9. [Phind](https://www.phind.com)
 10. [Llama2](https://www.llama2.ai)
 11. [Blackboxai](https://www.blackbox.ai)
 12. [gpt4all](https://gpt4all.io) *(Offline)*
 13. [Poe](https://poe.com) - Poe|Quora *(Session ID required)*
 14. [Groq](https://console.groq.com/playground) *(API Key required)*
 15. [Perplexity](https://www.perplexity.ai)
+16. [YepChat](https://yep.com)
 
 
 <details>
 
 <summary>
 
 41+ providers proudly offered by [gpt4free](https://github.com/xtekky/gpt4free).
@@ -398,14 +399,25 @@
 img.save(img_generator)
 
 # RAM friendly
 ```
 
 </details>
 
+#### Using **Prodia** provider
+
+```python
+from pytgpt.imager import Prodia
+
+img = Prodia()
+
+img_generator = img.generate('Coding bot', amount=3, stream=True)
+
+img.save(img_generator)
+```
 
 </details>
 
 ### Advanced Usage of Placeholders
 
 The `generate` functionality has been enhanced starting from *v0.3.0* to enable comprehensive utilization of the `--with-copied` option and support for accepting piped inputs. This improvement introduces placeholders, offering dynamic values for more versatile interactions.
 
@@ -468,21 +480,59 @@
 
 The environment variables can be overridden by explicitly declaring new value.
 
 > [!TIP]
 > Save the variables in a `.env` file in your current directory or export them in your `~/.zshrc` file.
 > To load previous conversations from a `.txt` file, use the `-fp` or `--filepath` flag. If no flag is passed, the default one will be used. To load context from a file without altering its content, use the `--retain-file` flag.
 
-## Dynamic Provider
+## Dynamic Provider & Further Interfaces
 
 Version **0.4.6** also introduces dynamic provider called `g4fauto`, which represents the fastest working g4f-based provider.
 
 > [!TIP]
-> To launch web interface for g4f-based providers simply run `$ pytgpt gpt4free gui`. 
+> To launch web interface for g4f-based providers simply run `$ pytgpt gpt4free gui`.
 > `$ pytgpt api run` will start the REST-API. Access docs and redoc at */docs* and */redoc* respectively.
+To launch the web interface for g4f-based providers, execute the following command in your terminal:
+
+```bash
+$ pytgpt gpt4free gui
+```
+
+This command initializes the Web-user interface for interacting with g4f-based providers.
+
+To start the REST-API:
+
+```bash
+$ pytgpt api run
+```
+
+This command starts the RESTful API server, enabling you to interact with the service programmatically.
+
+For accessing the documentation and redoc, navigate to the following paths in your web browser:
+- Documentation: `*/docs`
+- ReDoc: `*/redoc`
+
+## Speech Synthesis
+
+To enable speech synthesis of responses, ensure you have either the [VLC player](https://www.videolan.org/vlc/index.html) installed on your system or, if you are a [Termux](https://termux.org) user, the [Termux:API](https://wiki.termux.com/wiki/Termux:API) package.
+
+To activate speech synthesis, use the `--talk-to-me` flag or its shorthand `-ttm` when running your commands. For example:
+```bash
+$ pytgpt generate "Generate an ogre story" --talk-to-me
+```
+or
+```bash
+$ pytgpt interactive -ttm
+```
+This flag instructs the system to audiolize the ai responses and then play them, enhancing the user experience by providing auditory feedback.
+
+> To speech synthesise the responses just ensure you have [vlc player]() in your system or [termux-api](https://wiki.termux.com/wiki/Termux:API) for the case of [Termux](https://termux.org) users.
+> Use the flag `--talk-to-me`, shortform `-ttm`.
+
+Version **0.6.4** introduces another dynamic provider, `auto`, which denotes the working provider **overall**. This relieves you of the workload of manually checking a working provider each time you fire up pytgpt.
 
 <details>
 
 <summary>
 
 For more usage info run `$ pytgpt --help`
```

#### html2text {}

```diff
@@ -30,37 +30,38 @@
 uc.a.run.app/) 4. [OpenAI](https://chat.openai.com) *(API key required)* 5.
 [WebChatGPT](https://github.com/Simatwa/WebChatGPT) - **OpenAI** *(Session ID
 required)* 6. [Gemini](https://github.com/Simatwa/bard) - **Google** *(Session
 ID required)* 9. [Phind](https://www.phind.com) 10. [Llama2](https://
 www.llama2.ai) 11. [Blackboxai](https://www.blackbox.ai) 12. [gpt4all](https://
 gpt4all.io) *(Offline)* 13. [Poe](https://poe.com) - Poe|Quora *(Session ID
 required)* 14. [Groq](https://console.groq.com/playground) *(API Key required)*
-15. [Perplexity](https://www.perplexity.ai) 41+ providers proudly offered by
-[gpt4free](https://github.com/xtekky/gpt4free). - To list working providers
-run: ```sh $ pytgpt gpt4free test -y ``` ## Prerequisites - [x] [Python>=3.10]
-(https://python.org) *(Optional)* ## Installation and Usage ### Installation
-Download binaries for your system from [here.](https://github.com/Simatwa/
-python-tgpt/releases/latest/) Alternatively, you can install non-binaries. *
-(Recommended)* 1. Developers: ```sh pip install --upgrade python-tgpt ``` 2.
-Commandline: ```sh pip install --upgrade "python-tgpt[cli]" ``` 3. Full
-installation: ```sh pip install --upgrade "python-tgpt[all]" ``` > `pip install
--U "python-tgt[api]"` will install REST API dependencies. ## Usage This package
-offers a convenient command-line interface. > [!NOTE] > `phind` is the default
-*provider*. - For a quick response: ```bash python -m pytgpt generate "" ``` -
-For interactive mode: ```bash python -m pytgpt interactive "" ``` Make use of
-flag `--provider` followed by the provider name of your choice. e.g `--provider
-koboldai` > To list all providers offered by gpt4free, use following commands:
-```pytgpt gpt4free list providers``` You can also simply use `pytgpt` instead
-of `python -m pytgpt`. Starting from version 0.2.7, running `$ pytgpt` without
-any other command or option will automatically enter the `interactive` mode.
-Otherwise, you'll need to explicitly declare the desired action, for example,
-by running `$ pytgpt generate`. ### Developer Docs 1. Generate a quick response
-```python from pytgpt.leo import LEO bot = LEO() resp = bot.chat('') print
-(resp) # Output : How may I help you. ``` 2. Get back whole response ```python
-from pytgpt.leo import LEO bot = LEO() resp = bot.ask('
+15. [Perplexity](https://www.perplexity.ai) 16. [YepChat](https://yep.com) 41+
+providers proudly offered by [gpt4free](https://github.com/xtekky/gpt4free). -
+To list working providers run: ```sh $ pytgpt gpt4free test -y ``` ##
+Prerequisites - [x] [Python>=3.10](https://python.org) *(Optional)* ##
+Installation and Usage ### Installation Download binaries for your system from
+[here.](https://github.com/Simatwa/python-tgpt/releases/latest/) Alternatively,
+you can install non-binaries. *(Recommended)* 1. Developers: ```sh pip install
+--upgrade python-tgpt ``` 2. Commandline: ```sh pip install --upgrade "python-
+tgpt[cli]" ``` 3. Full installation: ```sh pip install --upgrade "python-tgpt
+[all]" ``` > `pip install -U "python-tgt[api]"` will install REST API
+dependencies. ## Usage This package offers a convenient command-line interface.
+> [!NOTE] > `phind` is the default *provider*. - For a quick response: ```bash
+python -m pytgpt generate "" ``` - For interactive mode: ```bash python -
+m pytgpt interactive "" ``` Make use of flag `--provider` followed by the
+provider name of your choice. e.g `--provider koboldai` > To list all providers
+offered by gpt4free, use following commands: ```pytgpt gpt4free list
+providers``` You can also simply use `pytgpt` instead of `python -m pytgpt`.
+Starting from version 0.2.7, running `$ pytgpt` without any other command or
+option will automatically enter the `interactive` mode. Otherwise, you'll need
+to explicitly declare the desired action, for example, by running `$ pytgpt
+generate`. ### Developer Docs 1. Generate a quick response ```python from
+pytgpt.leo import LEO bot = LEO() resp = bot.chat('') print(resp) # Output :
+How may I help you. ``` 2. Get back whole response ```python from pytgpt.leo
+import LEO bot = LEO() resp = bot.ask('
  Output """ {'completion': "I'm so excited to share with you the incredible
 experiences...", 'stop_reason': None, 'truncated': False, 'stop': None,
 'model': 'llama-2-13b-chat', 'log_id': 'cmpl-3NmRt5A5Djqo2jXtXLBwJ2',
 'exception': None} """ ``` #### Stream Response Just add parameter `stream`
 with value `true`. 1. Text Generated only ```python from pytgpt.leo import LEO
 bot = LEO() resp = bot.chat('', stream=True) for value in resp: print(value) #
 output """ How may How may I help How may I help you How may I help you today?
@@ -102,25 +103,27 @@
 informed that majority of providers offered by *gpt4free* requires *Google
 Chrome* inorder to function. ### Image Generation This has been made possible
 by [pollinations.ai](https://pollination.ai). ```sh $ pytgpt imager "" # e.g
 pytgpt imager "Coding bot" ``` Developers ```python from pytgpt.imager import
 Imager img = Imager() generated_img = img.generate('Coding bot') # [bytes]
 img.save(generated_img) ``` Download Multiple Images ```python from
 pytgpt.imager import Imager img = Imager() img_generator = img.generate('Coding
-bot', amount=3, stream=True) img.save(img_generator) # RAM friendly ``` ###
-Advanced Usage of Placeholders The `generate` functionality has been enhanced
-starting from *v0.3.0* to enable comprehensive utilization of the `--with-
-copied` option and support for accepting piped inputs. This improvement
-introduces placeholders, offering dynamic values for more versatile
-interactions. | Placeholder | Represents | | ------------ | ----------- | | `{
-{stream}}` | The piped input | | `{{copied}}` | The last copied text | This
-feature is particularly beneficial for intricate operations. For example:
-```bash $ git diff | pytgpt generate "Here is a diff file: {{stream}} Make a
-concise commit message from it, aligning with my commit message history: {
-{copied}}" --shell --new ``` > In this illustration, `{{stream}}` denotes the
+bot', amount=3, stream=True) img.save(img_generator) # RAM friendly ``` ####
+Using **Prodia** provider ```python from pytgpt.imager import Prodia img =
+Prodia() img_generator = img.generate('Coding bot', amount=3, stream=True)
+img.save(img_generator) ``` ### Advanced Usage of Placeholders The `generate`
+functionality has been enhanced starting from *v0.3.0* to enable comprehensive
+utilization of the `--with-copied` option and support for accepting piped
+inputs. This improvement introduces placeholders, offering dynamic values for
+more versatile interactions. | Placeholder | Represents | | ------------ | ----
+------- | | `{{stream}}` | The piped input | | `{{copied}}` | The last copied
+text | This feature is particularly beneficial for intricate operations. For
+example: ```bash $ git diff | pytgpt generate "Here is a diff file: {{stream}}
+Make a concise commit message from it, aligning with my commit message history:
+{{copied}}" --shell --new ``` > In this illustration, `{{stream}}` denotes the
 result of the `$ git diff` operation, while `{{copied}}` signifies the content
 copied from the output of the `$ git log` command. ### Awesome Prompts [These
 prompts](https://github.com/Simatwa/gpt-cli/blob/main/assets/all-
 acts.pdf?raw=True) are designed to guide the AI's behavior or responses in a
 particular direction, encouraging it to exhibit certain characteristics or
 behaviors. The term "awesome-prompt" is not a formal term in AI or machine
 learning literature, but it encapsulates the idea of crafting prompts that are
@@ -153,24 +156,46 @@
 prompt` will take the environment variable `PYTGPT_AWESOME_PROMPT`. > [!NOTE] >
 This is **NOT** limited to any command The environment variables can be
 overridden by explicitly declaring new value. > [!TIP] > Save the variables in
 a `.env` file in your current directory or export them in your `~/.zshrc` file.
 > To load previous conversations from a `.txt` file, use the `-fp` or `--
 filepath` flag. If no flag is passed, the default one will be used. To load
 context from a file without altering its content, use the `--retain-file` flag.
-## Dynamic Provider Version **0.4.6** also introduces dynamic provider called
-`g4fauto`, which represents the fastest working g4f-based provider. > [!TIP] >
-To launch web interface for g4f-based providers simply run `$ pytgpt gpt4free
-gui`. > `$ pytgpt api run` will start the REST-API. Access docs and redoc at */
-docs* and */redoc* respectively. For more usage info run `$ pytgpt --help` ```
-Usage: pytgpt [OPTIONS] COMMAND [ARGS]... Options: -v, --version Show the
-version and exit. -h, --help Show this message and exit. Commands: api FastAPI
-control endpoint awesome Perform CRUD operations on awesome-prompts generate
-Generate a quick response with AI gpt4free Discover gpt4free models, providers
-etc imager Generate images with pollinations.ai interactive Chat with AI
-interactively (Default) utils Utility endpoint for pytgpt webchatgpt Reverse
-Engineered ChatGPT Web-Version ``` ### API Health Status | No. | API | Status |
-|--------|-----|--------| | 1. | [On-render](https://python-tgpt.onrender.com)
-| [cron-job](https://pqfzhmvz.status.cron-job.org/) | ## [CHANGELOG](https://
+## Dynamic Provider & Further Interfaces Version **0.4.6** also introduces
+dynamic provider called `g4fauto`, which represents the fastest working g4f-
+based provider. > [!TIP] > To launch web interface for g4f-based providers
+simply run `$ pytgpt gpt4free gui`. > `$ pytgpt api run` will start the REST-
+API. Access docs and redoc at */docs* and */redoc* respectively. To launch the
+web interface for g4f-based providers, execute the following command in your
+terminal: ```bash $ pytgpt gpt4free gui ``` This command initializes the Web-
+user interface for interacting with g4f-based providers. To start the REST-API:
+```bash $ pytgpt api run ``` This command starts the RESTful API server,
+enabling you to interact with the service programmatically. For accessing the
+documentation and redoc, navigate to the following paths in your web browser: -
+Documentation: `*/docs` - ReDoc: `*/redoc` ## Speech Synthesis To enable speech
+synthesis of responses, ensure you have either the [VLC player](https://
+www.videolan.org/vlc/index.html) installed on your system or, if you are a
+[Termux](https://termux.org) user, the [Termux:API](https://wiki.termux.com/
+wiki/Termux:API) package. To activate speech synthesis, use the `--talk-to-me`
+flag or its shorthand `-ttm` when running your commands. For example: ```bash $
+pytgpt generate "Generate an ogre story" --talk-to-me ``` or ```bash $ pytgpt
+interactive -ttm ``` This flag instructs the system to audiolize the ai
+responses and then play them, enhancing the user experience by providing
+auditory feedback. > To speech synthesise the responses just ensure you have
+[vlc player]() in your system or [termux-api](https://wiki.termux.com/wiki/
+Termux:API) for the case of [Termux](https://termux.org) users. > Use the flag
+`--talk-to-me`, shortform `-ttm`. Version **0.6.4** introduces another dynamic
+provider, `auto`, which denotes the working provider **overall**. This relieves
+you of the workload of manually checking a working provider each time you fire
+up pytgpt. For more usage info run `$ pytgpt --help` ``` Usage: pytgpt
+[OPTIONS] COMMAND [ARGS]... Options: -v, --version Show the version and exit. -
+h, --help Show this message and exit. Commands: api FastAPI control endpoint
+awesome Perform CRUD operations on awesome-prompts generate Generate a quick
+response with AI gpt4free Discover gpt4free models, providers etc imager
+Generate images with pollinations.ai interactive Chat with AI interactively
+(Default) utils Utility endpoint for pytgpt webchatgpt Reverse Engineered
+ChatGPT Web-Version ``` ### API Health Status | No. | API | Status | |--------
+|-----|--------| | 1. | [On-render](https://python-tgpt.onrender.com) | [cron-
+job](https://pqfzhmvz.status.cron-job.org/) | ## [CHANGELOG](https://
 github.com/Simatwa/python-tgpt/blob/main/docs/CHANGELOG.md) ## Acknowledgements
 1. [x] [tgpt](https://github.com/aandrew-me/tgpt) 2. [x] [gpt4free](https://
 github.com/xtekky/gpt4free)
```

### Comparing `python_tgpt-0.6.4/setup.py` & `python_tgpt-0.6.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     "pyyaml==6.0.1",
     "webchatgpt==0.3.0",
     "GoogleBard1>=2.1.4",
     "poe-api-wrapper==1.3.6",
     "brotli==1.1.0",
     "g4f>=0.2.6.1",
     "Helpingai-T2==0.3",
+    "python-vlc>=3.0.20",
 ]
 
 cli_reqs = [
     "click==8.1.3",
     "rich==13.3.4",
     "clipman==3.1.0",
     "pyperclip==1.8.2",
@@ -42,15 +43,15 @@
 if not PATH.exists():
     with Path.open(DOCS_PATH, encoding="utf-8") as f1:
         with Path.open(PATH, "w+", encoding="utf-8") as f2:
             f2.write(f1.read())
 
 setup(
     name="python-tgpt",
-    version="0.6.4",
+    version="0.6.5",
     license="MIT",
     author="Smartwa",
     maintainer="Smartwa",
     author_email="simatwacaleb@proton.me",
     description="Interact with AI without API key",
     packages=find_packages("src"),
     package_dir={"": "src"},
```

### Comparing `python_tgpt-0.6.4/src/pytgpt/__init__.py` & `python_tgpt-0.6.5/src/pytgpt/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -22,14 +22,15 @@
     "blackboxai",
     "gpt4all",
     "webchatgpt",
     "g4fauto",
     "poe",
     "groq",
     "perplexity",
+    "yepchat",
 ]
 
 gpt4free_providers = [
     provider.__name__ for provider in g4f.Provider.__providers__  # if provider.working
 ]
 
 available_providers = tgpt_providers + gpt4free_providers
```

### Comparing `python_tgpt-0.6.4/src/pytgpt/api/__init__.py` & `python_tgpt-0.6.5/src/pytgpt/api/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,16 +11,19 @@
 from datetime import datetime
 from . import v1
 
 app = FastAPI(
     title="python-tgpt",
     summary="Interact with AI without API key",
     description=(
-        "For **text** and **image** generation."
-        "Full documentation available at official repo : [Simatwa/python-tgpt](https://github.com/Simatwa/python-tgpt)."
+        "For **text** generation, **text-to-image** and **text-to-audio** conversions."
+        "\n\n"
+        "Access redoc at [/redoc](/redoc) endpoint."
+        "\n\n"
+        "Full documentation is available at official repo : [Simatwa/python-tgpt](https://github.com/Simatwa/python-tgpt)."
     ),
     version=__version__,
     contact={
         "name": "Smartwa",
         "email": "simatwacaleb@proton.me",
         "url": "https://simatwa.vercel.app",
     },
```

### Comparing `python_tgpt-0.6.4/src/pytgpt/api/utils.py` & `python_tgpt-0.6.5/src/pytgpt/api/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,16 +19,16 @@
     async def decorator(*args, **kwargs):
         try:
             return await func(*args, **kwargs)
 
         except (ProxyError, InvalidProxyURL, SSLError) as e:
             raise HTTPException(
                 status_code=status.HTTP_400_BAD_REQUEST,
-                detail=f"Proxy related error. {get_exception_string(e)}",
+                detail=dict(message=f"Proxy related error. {get_exception_string(e)}"),
             )
         except Exception as e:
             raise HTTPException(
                 status_code=status.HTTP_500_INTERNAL_SERVER_ERROR,
-                detail=get_exception_string(e),
+                detail=dict(message=get_exception_string(e)),
             )
 
     return decorator
```

### Comparing `python_tgpt-0.6.4/src/pytgpt/api/v1.py` & `python_tgpt-0.6.5/src/pytgpt/api/v1.py`

 * *Files 17% similar despite different names*

```diff
@@ -12,30 +12,36 @@
 from pytgpt.leo import LEO
 from pytgpt.opengpt import OPENGPT
 from pytgpt.koboldai import KOBOLDAI
 from pytgpt.phind import PHIND
 from pytgpt.llama2 import LLAMA2
 from pytgpt.blackboxai import BLACKBOXAI
 from pytgpt.perplexity import PERPLEXITY
+from pytgpt.yepchat import YEPCHAT
 from pytgpt.gpt4free import GPT4FREE
 from pytgpt.auto import AUTO
 from pytgpt.imager import Imager
+from pytgpt.imager import Prodia
+from pytgpt.utils import Audio
 from pytgpt.utils import api_static_image_dir
 
 provider_map = {
     "leo": LEO,
     "opengpt": OPENGPT,
     "koboldai": KOBOLDAI,
     "phind": PHIND,
     "llama2": LLAMA2,
     "blackboxai": BLACKBOXAI,
     "perplexity": PERPLEXITY,
+    "yepchat": YEPCHAT,
     "auto": AUTO,
 }
 
+image_providers = {"default": Imager, "prodia": Prodia}
+
 supported_providers = list(provider_map.keys()) + gpt4free_providers
 
 app = APIRouter()
 
 
 class ProvidersModel(BaseModel):
     tgpt: list[str] = list(provider_map.keys())
@@ -53,15 +59,15 @@
                     ],
                 }
             ]
         }
     }
 
 
-class UserPayload(BaseModel):
+class TextGenerationPayload(BaseModel):
     prompt: str
     provider: str = "auto"
     # is_conversation: bool = False
     whole: bool = False
     max_tokens: PositiveInt = 600
     timeout: PositiveInt = 30
     proxy: Union[dict[str, str], None] = None
@@ -85,15 +91,17 @@
     }
 
     @validator("provider")
     def validate_provider(provider: str) -> object:
         if provider not in supported_providers:
             raise HTTPException(
                 status_code=status.HTTP_400_BAD_REQUEST,
-                detail=f"Provider '{provider}' is not one of [{', '.join(supported_providers)}]",
+                detail=dict(
+                    message=f"Provider '{provider}' is not one of [{', '.join(supported_providers)}]",
+                ),
             )
         return provider
 
 
 class ProviderResponse(BaseModel):
     """
     - `provider` : Provider name that generated response.
@@ -138,26 +146,28 @@
 
 
 class ImagePayload(BaseModel):
     prompt: str
     amount: PositiveInt = 1
     proxy: Union[dict[str, str], None] = None
     timeout: PositiveInt = 30
+    provider: Union[str, None] = None
 
     model_config = {
         "json_schema_extra": {
             "examples": [
                 {
-                    "prompt": "Mount Everest view from ISS",
+                    "prompt": "Sunset view from ISS",
                     "amount": 2,
                     "proxy": {
                         "http": "socks4://54.248.238.110:80",
                         "https": "socks4://54.248.238.110:80",
                     },
                     "timeout": 30,
+                    "provider": "default",
                 },
                 {
                     "prompt": "Developed Nairobi in 3050",
                     "amount": 2,
                     "proxy": None,
                     "timeout": 30,
                 },
@@ -166,40 +176,66 @@
     }
 
     @validator("amount")
     def validate_amount(amount: int) -> PositiveInt:
         if amount > 10:
             raise HTTPException(
                 status_code=status.HTTP_400_BAD_REQUEST,
-                detail=f"Amount {amount} is out of range : 1-10",
+                detail=dict(
+                    message=f"Amount {amount} is out of range : 1-10",
+                ),
             )
         return amount
 
+    @validator("provider")
+    def validate_provider(provider: Union[str, None]) -> str:
+        if provider not in image_providers:
+            raise HTTPException(
+                status_code=status.HTTP_400_BAD_REQUEST,
+                detail=dict(
+                    message=f"Image provider '{provider}' is not one of [{', '.join(list(image_providers.keys()))}]",
+                ),
+            )
+        return "default" if provider is None else provider
+
 
 class ImageBytesPayload(BaseModel):
     prompt: str
     proxy: Union[dict[str, str], None] = None
     timeout: PositiveInt = 30
+    provider: Union[str, None] = None
 
     model_config = {
         "json_schema_extra": {
             "examples": [
                 {
-                    "prompt": "Jay Z performing",
+                    "prompt": "Alan Walker performing",
                     "proxy": {
                         "http": "socks4://199.229.254.129:4145",
                         "https": "socks4://199.229.254.129:4145",
                     },
                     "timeout": 30,
+                    "provider": "default",
                 },
                 {"prompt": "Developed Nairobi in 3050", "proxy": None, "timeout": 30},
             ]
         }
     }
 
+    @validator("provider")
+    def validate_provider(provider: Union[str, None]) -> str:
+        if provider not in image_providers:
+            raise HTTPException(
+                status_code=status.HTTP_400_BAD_REQUEST,
+                detail=dict(
+                    message=f"Image provider '{provider}' is not one of [{', '.join(list(image_providers.keys()))}]",
+                ),
+            )
+        return "default" if provider is None else provider
+
 
 class ImageBytesResponse(BaseModel):
     image: bytes
 
 
 class ImageResponse(BaseModel):
     """
@@ -218,15 +254,62 @@
                     ]
                 }
             ]
         }
     }
 
 
-def init_provider(payload: UserPayload) -> object:
+class TextToAudioPayload(BaseModel):
+    message: str
+    voice: Union[str, None] = "Brian"
+    proxy: Union[dict[str, str], None] = None
+    timeout: int = 30
+    model_config = {
+        "json_schema_extra": {
+            "example": {
+                "message": "There is a place for people like you.",
+                "voice": "Brian",
+                "proxy": {
+                    "http": "socks4://199.229.254.129:4145",
+                    "https": "socks4://199.229.254.129:4145",
+                },
+                "timeout": 30,
+            }
+        }
+    }
+
+    @validator("voice")
+    def validate_voice(voice) -> str:
+        if not voice in Audio.all_voices:
+            raise HTTPException(
+                status_code=status.HTTP_400_BAD_REQUEST,
+                detail=dict(
+                    message=f"Voice '{voice}' is not one of '[{', '.join(Audio.all_voices)}]"
+                ),
+            )
+        return "Brian" if not voice else voice
+
+
+class TextToAudioResponse(BaseModel):
+    """
+    - `url` : Link to generated audio file.
+    """
+
+    url: str
+
+    model_config = {
+        "json_schema_extra": {
+            "example": {
+                "url": " http://localhost:8000/static/audios/f9d4233f-9b78-4d87-bc27-5d2ab928f673.mp3",
+            }
+        }
+    }
+
+
+def init_provider(payload: TextGenerationPayload) -> object:
     return provider_map.get(payload.provider, GPT4FREE)(
         is_conversation=False,  # payload.is_conversation,
         max_tokens=payload.max_tokens,
         timeout=payload.timeout,
         proxies=payload.proxy,
     )
 
@@ -243,15 +326,15 @@
     **Warning** : Not all of *g4f-based* providers are functional.
     """
     return ProvidersModel()
 
 
 @app.post("/chat/nostream", name="no-stream")
 @api_exception_handler
-async def non_stream(payload: UserPayload) -> ProviderResponse:
+async def non_stream(payload: TextGenerationPayload) -> ProviderResponse:
     """No response streaming.
 
     - `prompt` : User query.
     - `provider` : LLM provider name.
     - `whole` : Return whole response body instead of text only.
     - `max_tokens` : Maximum number of tokens to be generated upon completion.
     - `timeout` : Http request timeout.
@@ -270,15 +353,15 @@
             else payload.provider
         ),
         text=ai_generated_text,
         body=provider_obj.last_response if payload.whole else None,
     )
 
 
-def generate_streaming_response(payload: UserPayload) -> Generator:
+def generate_streaming_response(payload: TextGenerationPayload) -> Generator:
     provider_obj: LEO = init_provider(payload)
 
     for text in provider_obj.chat(payload.prompt, stream=True):
         response = ProviderResponse(
             provider=(
                 provider_obj.provider_name
                 if payload.provider == "auto"
@@ -288,15 +371,15 @@
             body=provider_obj.last_response if payload.whole else None,
         )
         yield dumps(jsonable_encoder(response)) + "\n"
 
 
 @app.post("/chat/stream", name="stream", response_model=ProviderResponse)
 @api_exception_handler
-async def stream(payload: UserPayload) -> Any:
+async def stream(payload: TextGenerationPayload) -> Any:
     """Stream back response as received.
 
     - `prompt` : User query.
     - `provider` : LLM provider name.
     - `whole` : Return whole response body instead of text only.
     - `max_tokens` : Maximum number of tokens to be generated upon completion.
     - `timeout` : Http request timeout.
@@ -317,19 +400,22 @@
 async def generate_image(payload: ImagePayload, request: Request) -> ImageResponse:
     """Generate images from prompt
 
     - `prompt` : Image description
     - `amount` : Images to be generated. Maximum of 10.
     - `timeout` : Http request timeout.
     - `proxy` : Http request proxies.
+    - `provider` : Image provider name ie. *[default, prodia]*
 
     **NOTE** : *Ensure `proxy` value is correct otherwise make it `null`*
     """
     host = f"{request.url.scheme}://{request.url.netloc}"
-    image_gen_obj = Imager(timeout=payload.timeout, proxies=payload.proxy)
+    image_gen_obj = image_providers.get(payload.provider)(
+        timeout=payload.timeout, proxies=payload.proxy
+    )
     image_generator = image_gen_obj.generate(
         prompt=payload.prompt, amount=payload.amount, stream=True
     )
     image_urls = image_gen_obj.save(
         image_generator,
         name=uuid4().__str__(),
         dir=api_static_image_dir,
@@ -342,58 +428,125 @@
 @api_exception_handler
 async def generate_image(payload: ImageBytesPayload, request: Request) -> Response:
     """Generate images from prompt and return raw bytes
 
     - `prompt` : Image description
     - `timeout` : Http request timeout.
     - `proxy` : Http request proxies.
+    - `provider` : Image provider name ie. *[default, prodia]*
 
     **Only one image is generated.**
 
     **NOTE** : *Ensure `proxy` value is correct otherwise make it `null`*
     """
-    image_gen_obj = Imager(timeout=payload.timeout, proxies=payload.proxy)
+    image_gen_obj = image_providers.get(payload.provider)(
+        timeout=payload.timeout, proxies=payload.proxy
+    )
     image_list = image_gen_obj.generate(prompt=payload.prompt)
     response = Response(
         image_list[0],
-        media_type="image/jpeg",
+        media_type=f"image/{image_gen_obj.image_extension}",
     )
     response.headers["Content-Disposition"] = (
-        f"attachment; filename={payload.prompt[:25]+'...' if len(payload.prompt)>25 else payload.prompt}.jpeg"
+        f"attachment; filename={payload.prompt[:25]+'...' if len(payload.prompt)>25 else payload.prompt}.{image_gen_obj.image_extension}"
     )
     return response
 
 
 @app.get("/image/bytes", name="prompt-to-image (bytes)")
 @api_exception_handler
-async def redirect_image_generation(
-    prompt: str, proxy: Union[str, None] = None, timeout: int = 30
+async def generate_image_return_bytes(
+    prompt: str,
+    proxy: Union[str, None] = None,
+    timeout: int = 30,
+    provider: str = "default",
 ):
     """Generate images from prompt and return raw bytes
 
     - `prompt` : Image description
     - `timeout` : Http request timeout.
     - `proxy` : Http request proxies.
+    - `provider` : Image provider name ie. *[default, prodia]*
 
     **Only one image is generated.**
 
     **NOTE** : *Ensure `proxy` value is correct otherwise make it `null`*
     """
-    image_gen_obj = Imager(timeout=timeout, proxies={"https": proxy} if proxy else {})
+    image_gen_obj = image_providers.get(provider, "default")(
+        timeout=timeout, proxies={"https": proxy} if proxy else {}
+    )
     image_list = image_gen_obj.generate(prompt=prompt)
     response = Response(
         image_list[0],
-        media_type="image/jpeg",
+        media_type=f"image/{image_gen_obj.image_extension}",
     )
     response.headers["Content-Disposition"] = (
-        f"attachment; filename={prompt[:25]+'...' if len(prompt)>25 else prompt}.jpeg"
+        f"attachment; filename={prompt[:25]+'...' if len(prompt)>25 else prompt}.{image_gen_obj.image_extension}"
     )
     return response
 
 
 @app.get("/image/bytes/redirect", name="prompt-to-image (bytes - redirect) ")
 @api_exception_handler
 async def redirect_image_generation(prompt: str):
     """Redirect image generation request to [pollinations.ai](https://pollinations.ai)"""
     return RedirectResponse(
         f"https://image.pollinations.ai/prompt/{prompt}",
     )
+
+
+@app.post("/audio", name="text-to-audio")
+@api_exception_handler
+async def text_to_audio(
+    payload: TextToAudioPayload, request: Request
+) -> TextToAudioResponse:
+    """Vocalize text
+
+    - `message` : Text to be synthesised.
+    - `voice` :  The voice to use for speech synthesis.
+    - `timeout` : Http request timeout in seconds.
+    - `proxy` : Http request proxy.
+
+    **NOTE** : *Ensure `proxy` value is correct otherwise make it `null`*
+    """
+    host = f"{request.url.scheme}://{request.url.netloc}"
+    filename = uuid4().__str__() + ".mp3"
+    Audio.text_to_audio(
+        message=payload.message,
+        voice=payload.voice,
+        proxies=payload.proxy,
+        timeout=payload.timeout,
+        save_to=Audio.cache_dir.joinpath(filename).as_posix(),
+    )
+    return TextToAudioResponse(url=f"{host}/static/audios/" + filename)
+
+
+@app.get("/audio", name="text-to-audio (bytes)")
+@api_exception_handler
+async def text_to_audio_bytes(
+    message: str,
+    voice: str = "Brian",
+    timeout: int = 30,
+    proxy: Union[str, None] = None,
+):
+    """Return raw audio
+
+    - `message` : Text to be synthesised.
+    - `voice` :  The voice to use for speech synthesis.
+    - `timeout` : Http request timeout in seconds.
+    - `proxy` : Http request proxy.
+
+    **NOTE** : *Ensure `proxy` value is correct otherwise make it `null`*
+    """
+    image_bytes = Audio.text_to_audio(
+        message=message,
+        voice=voice if voice in Audio.all_voices else "Brian",
+        proxies={"https": proxy} if proxy else {},
+        timeout=timeout,
+    )
+    return Response(
+        content=image_bytes,
+        media_type="audio/mpeg",
+        headers={
+            "Content-Disposition": f"attachment; filename={uuid4().__str__()}.mp3"
+        },
+    )
```

### Comparing `python_tgpt-0.6.4/src/pytgpt/auto/main.py` & `python_tgpt-0.6.5/src/pytgpt/auto/main.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.6.4/src/pytgpt/base.py` & `python_tgpt-0.6.5/src/pytgpt/base.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.6.4/src/pytgpt/blackboxai/main.py` & `python_tgpt-0.6.5/src/pytgpt/blackboxai/main.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.6.4/src/pytgpt/console.py` & `python_tgpt-0.6.5/src/pytgpt/console.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,16 @@
 from rich.progress import Progress
 from typing import Iterator
 from pytgpt.utils import Optimizers
 from pytgpt.utils import default_path
 from pytgpt.utils import AwesomePrompts
 from pytgpt.utils import RawDog
 from pytgpt.imager import Imager
+from pytgpt.imager import Prodia
+from pytgpt.utils import Audio
 from WebChatGPT.console import chat as webchatgpt
 from colorama import Fore
 from colorama import init as init_colorama
 from dotenv import load_dotenv
 
 init_colorama(autoreset=True)
 
@@ -62,14 +64,16 @@
 
     default_provider = "auto"
 
     getExc = lambda e: e.args[1] if len(e.args) > 1 else str(e)
 
     context_settings = dict(auto_envvar_prefix="PYTGPT")
 
+    image_providers_map: dict[str, object] = {"default": Imager, "prodia": Prodia}
+
     """Console utils"""
 
     @staticmethod
     def run_system_command(
         command: str, exit_on_error: bool = True, stdout_error: bool = True
     ):
         """Run commands against system
@@ -565,14 +569,34 @@
                     filepath=filepath,
                     update_file=update_file,
                     proxies=proxies,
                     history_offset=history_offset,
                     act=awesome_prompt,
                 )
 
+            elif provider == "yepchat":
+                from pytgpt.yepchat import main as yepchat
+
+                self.bot = yepchat.YEPCHAT(
+                    is_conversation=disable_conversation,
+                    max_tokens=max_tokens,
+                    temperature=temperature,
+                    presence_penalty=top_p,
+                    frequency_penalty=top_k,
+                    top_p=top_p,
+                    model=getOr(model, yepchat.model),
+                    timeout=timeout,
+                    intro=intro,
+                    filepath=filepath,
+                    update_file=update_file,
+                    proxies=proxies,
+                    history_offset=history_offset,
+                    act=awesome_prompt,
+                )
+
             elif provider == "gpt4all":
                 assert auth, (
                     "Path to LLM (.gguf or .bin) file is required. "
                     "Download models from <https://gpt4all.io>. "
                     "Use the flag `--key` or `-k`"
                 )
 
@@ -717,14 +741,17 @@
         self.disable_stream = False
         self.provider = provider
         self.disable_coloring = False
         self.internal_exec = internal_exec
         self.confirm_script = confirm_script
         self.interpreter = interpreter
         self.rawdog = rawdog
+        self.read_aloud = False
+        self.read_aloud_voice = "Brian"
+        self.path_to_last_response_audio = None
         self.__init_time = time.time()
         self.__start_time = time.time()
         self.__end_time = time.time()
 
     @property
     def get_provider(self):
         if self.provider == "auto" and self.bot.provider_name is not None:
@@ -1030,14 +1057,21 @@
         """Show whole last response in json format"""
         self.output_bond(
             "Last Response",
             self.bot.last_response,
             is_json=True,
         )
 
+    @busy_bar.run(help="While rereading aloud", index=3, immediate=True)
+    def do_reread(self, line):
+        """Reread aloud last ai response"""
+        if not self.path_to_last_response_audio:
+            raise Exception("Path to last response audio is null")
+        Audio.play(self.path_to_last_response_audio)
+
     @busy_bar.run()
     def do_exec(self, line):
         """Exec python code in last response with RawDog"""
         last_response = self.bot.get_message(self.bot.last_response)
         assert last_response, "Last response is null"
         assert "```python" in last_response, "Last response has no python code"
         if self.rawdog:
@@ -1140,17 +1174,32 @@
 
             except Exception as e:
                 # logging.exception(e)
                 busy_bar.stop_spinning()
                 logging.error(this.getExc(e))
                 if exit_on_error:
                     sys.exit(1)
+
+            else:
+                self.post_default()
+
             finally:
                 self.__end_time = time.time()
 
+    @busy_bar.run(help="While reading aloud", immediate=True, index=3)
+    def post_default(self):
+        """Actions to be taken after upon successfull complete response generation triggered by `default` function"""
+        last_text: str = self.bot.get_message(self.bot.last_response)
+        if self.read_aloud and last_text is not None:
+            # Talk back to user
+            self.path_to_last_response_audio = Audio.text_to_audio(
+                last_text, voice=self.read_aloud_voice, auto=True
+            )
+            Audio.play(self.path_to_last_response_audio)
+
     def do_sys(self, line):
         """Execute system commands
         shortcut [./<command>]
         Usage:
             sys <System command>
                   or
              ./<System command>
@@ -1399,14 +1448,28 @@
     )
     @click.option(
         "-int",
         "--interpreter",
         default="python",
         help="RawDog : Python's interpreter name",
     )
+    @click.option(
+        "-ttm",
+        "--talk-to-me",
+        is_flag=True,
+        help="Audiolize responses upon complete generation",
+    )
+    @click.option(
+        "-ttmv",
+        "--talk-to-me-voice",
+        help="The voice to use for speech synthesis",
+        type=click.Choice(Audio.all_voices),
+        metavar="|".join(Audio.all_voices[:8]),
+        default="Brian",
+    )
     @click.help_option("-h", "--help")
     def interactive(
         model,
         temperature,
         max_tokens,
         top_p,
         top_k,
@@ -1433,14 +1496,16 @@
         no_coloring,
         chat_completion,
         ignore_working,
         rawdog,
         internal_exec,
         confirm_script,
         interpreter,
+        talk_to_me,
+        talk_to_me_voice,
     ):
         """Chat with AI interactively (Default)"""
         this.clear_history_file(filepath, new)
         bot = Main(
             max_tokens,
             temperature,
             top_k,
@@ -1467,14 +1532,16 @@
         busy_bar.spin_index = busy_bar_index
         bot.code_theme = code_theme
         bot.color = font_color
         bot.disable_coloring = no_coloring
         bot.prettify = prettify
         bot.vertical_overflow = vertical_overflow
         bot.disable_stream = whole
+        bot.read_aloud = talk_to_me
+        bot.read_aloud_voice = talk_to_me_voice
         if prompt:
             if with_copied:
                 prompt = prompt + "\n" + clipman.get()
             bot.default(prompt)
         bot.cmdloop()
 
 
@@ -1681,14 +1748,28 @@
     )
     @click.option(
         "-int",
         "--interpreter",
         default="python",
         help="RawDog : Python's interpreter name",
     )
+    @click.option(
+        "-ttm",
+        "--talk-to-me",
+        is_flag=True,
+        help="Audiolize responses upon complete generation",
+    )
+    @click.option(
+        "-ttmv",
+        "--talk-to-me-voice",
+        help="The voice to use for speech synthesis",
+        type=click.Choice(Audio.all_voices),
+        metavar="|".join(Audio.all_voices[:8]),
+        default="Brian",
+    )
     @click.help_option("-h", "--help")
     def generate(
         model,
         temperature,
         max_tokens,
         top_p,
         top_k,
@@ -1715,14 +1796,16 @@
         new,
         with_copied,
         ignore_working,
         rawdog,
         internal_exec,
         confirm_script,
         interpreter,
+        talk_to_me,
+        talk_to_me_voice,
     ):
         """Generate a quick response with AI"""
         this.clear_history_file(filepath, new)
         bot = Main(
             max_tokens,
             temperature,
             top_k,
@@ -1792,14 +1875,16 @@
             0 if any([quiet, sys.stdout.isatty() == False]) else busy_bar_index
         )
         bot.code_theme = code_theme
         bot.color = font_color
         bot.prettify = prettify
         bot.vertical_overflow = vertical_overflow
         bot.disable_stream = whole
+        bot.read_aloud = talk_to_me
+        bot.read_aloud_voice = talk_to_me_voice
         bot.default(prompt, True, normal_stdout=(sys.stdout.isatty() == False))
 
 
 class Awesome:
     """Awesome commands"""
 
     @staticmethod
@@ -2269,14 +2354,23 @@
 
 class ImageGen:
 
     @staticmethod
     @click.command(context_settings=this.context_settings)
     @click.argument("prompt")
     @click.option(
+        "-p",
+        "--provider",
+        help="Provider name for image generation",
+        type=click.Choice(
+            list(this.image_providers_map.keys()),
+        ),
+        default="default",
+    )
+    @click.option(
         "-d",
         "--directory",
         type=click.Path(exists=True),
         help="Folder for saving the images",
         default=os.getcwd(),
     )
     @click.option(
@@ -2289,34 +2383,35 @@
     @click.option("-n", "--name", help="Name for the generated images")
     @click.option(
         "-t",
         "--timeout",
         type=click.IntRange(5, 300),
         help="Http request timeout in seconds",
     )
-    @click.option("-p", "--proxy", help="Http request proxy")
+    @click.option("-pr", "--proxy", help="Http request proxy")
     @click.option(
         "-nd",
         "--no-additives",
         is_flag=True,
         help="Disable prompt altering for effective image generation",
     )
     @click.option("-q", "--quiet", is_flag=True, help="Suppress progress bar")
     @click.help_option("-h", "--help")
     def generate_image(
-        prompt, directory, amount, name, timeout, proxy, no_additives, quiet
+        prompt, provider, directory, amount, name, timeout, proxy, no_additives, quiet
     ):
         """Generate images with pollinations.ai"""
+        provider_obj = this.image_providers_map.get(provider)
         with Progress() as progress:
             task = progress.add_task(
                 f"[cyan]Generating ...[{amount}]",
                 total=amount,
                 visible=quiet == False,
             )
-            imager = Imager(timeout=timeout, proxies=proxy if proxy else {})
+            imager = provider_obj(timeout=timeout, proxies=proxy if proxy else {})
             for image in imager.generate(
                 prompt=prompt,
                 amount=amount,
                 additives=no_additives == False,
                 stream=True,
             ):
                 imager.save([image], name=name, dir=directory)
@@ -2419,26 +2514,33 @@
         import uvicorn
         from pytgpt.api import app
 
         uvicorn.run(app, host=bind, port=port, log_level=log_level)
 
     @staticmethod
     @click.command(context_settings=this.context_settings)
-    @click.argument("content", required=True, type=click.Choice(["images", "all"]))
+    @click.argument(
+        "content", required=True, type=click.Choice(["images", "audios", "all"])
+    )
     @click.option("-y", "--yes", is_flag=True, help="Okay to all confirmation prompts")
     @click.help_option("-h", "--help")
     def clear(content: str, yes: bool):
         """Delete api's static contents"""
-        from pytgpt.utils import api_static_image_dir, api_static_dir
+        from pytgpt.utils import (
+            api_static_image_dir,
+            api_static_audio_dir,
+            api_static_dir,
+        )
         from pathlib import Path
         import shutil
 
         static_contents_map: dict[str, Path] = {
             "images": api_static_image_dir,
             "all": api_static_dir,
+            "audios": api_static_audio_dir,
         }
         content_path: Path = static_contents_map[content]
         if not yes:
             yess: bool = click.confirm(
                 f"Are you sure to clear {content} '{content_path.as_posix()}'"
             )
             if not yess:
```

### Comparing `python_tgpt-0.6.4/src/pytgpt/gemini/main.py` & `python_tgpt-0.6.5/src/pytgpt/gemini/main.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.6.4/src/pytgpt/gpt4all/main.py` & `python_tgpt-0.6.5/src/pytgpt/gpt4all/main.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.6.4/src/pytgpt/gpt4free/main.py` & `python_tgpt-0.6.5/src/pytgpt/gpt4free/main.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.6.4/src/pytgpt/gpt4free/utils.py` & `python_tgpt-0.6.5/src/pytgpt/gpt4free/utils.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.6.4/src/pytgpt/groq/main.py` & `python_tgpt-0.6.5/src/pytgpt/groq/main.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.6.4/src/pytgpt/koboldai/main.py` & `python_tgpt-0.6.5/src/pytgpt/koboldai/main.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.6.4/src/pytgpt/leo/main.py` & `python_tgpt-0.6.5/src/pytgpt/leo/main.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.6.4/src/pytgpt/llama2/main.py` & `python_tgpt-0.6.5/src/pytgpt/llama2/main.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.6.4/src/pytgpt/openai/main.py` & `python_tgpt-0.6.5/src/pytgpt/openai/main.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.6.4/src/pytgpt/opengpt/main.py` & `python_tgpt-0.6.5/src/pytgpt/opengpt/main.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.6.4/src/pytgpt/perplexity/main.py` & `python_tgpt-0.6.5/src/pytgpt/perplexity/main.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.6.4/src/pytgpt/phind/main.py` & `python_tgpt-0.6.5/src/pytgpt/phind/main.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.6.4/src/pytgpt/poe/main.py` & `python_tgpt-0.6.5/src/pytgpt/poe/main.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.6.4/src/pytgpt/utils.py` & `python_tgpt-0.6.5/src/pytgpt/utils.py`

 * *Files 25% similar despite different names*

```diff
@@ -8,26 +8,34 @@
 import re
 import sys
 import click
 from rich.markdown import Markdown
 from rich.console import Console
 from pathlib import Path
 import os
+from typing import Union
+from typing import NoReturn
+import requests
+import vlc
+from time import sleep as wait
 
 appdir = appdirs.AppDirs("pytgpt", "Smartwa")
 
 default_path = appdir.user_cache_dir
 
 api_static_dir = Path(default_path) / "api"
 
 api_static_image_dir = api_static_dir / "images"
 
+api_static_audio_dir = api_static_dir / "audios"
+
 os.makedirs(default_path, exist_ok=True)
 os.makedirs(api_static_dir.as_posix(), exist_ok=True)
 os.makedirs(api_static_image_dir.as_posix(), exist_ok=True)
+os.makedirs(api_static_audio_dir.as_posix(), exist_ok=True)
 
 
 def run_system_command(
     command: str,
     exit_on_error: bool = True,
     stdout_error: bool = True,
     help: str = None,
@@ -656,7 +664,352 @@
                 except Exception as e:
                     self.log(
                         "Exception occurred while executing script. Responding with error: "
                         f"{e.args[1] if len(e.args)>1 else str(e)}",
                         "error",
                     )
                     return f"PREVIOUS SCRIPT EXCEPTION:\n{str(e)}"
+
+
+class Audio:
+    # Request headers
+    cache_dir: Path = api_static_audio_dir
+    headers: dict[str, str] = {
+        "User-Agent": "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/119.0.0.0 Safari/537.36"
+    }
+    all_voices: list[str] = [
+        "Filiz",
+        "Astrid",
+        "Tatyana",
+        "Maxim",
+        "Carmen",
+        "Ines",
+        "Cristiano",
+        "Vitoria",
+        "Ricardo",
+        "Maja",
+        "Jan",
+        "Jacek",
+        "Ewa",
+        "Ruben",
+        "Lotte",
+        "Liv",
+        "Seoyeon",
+        "Takumi",
+        "Mizuki",
+        "Giorgio",
+        "Carla",
+        "Bianca",
+        "Karl",
+        "Dora",
+        "Mathieu",
+        "Celine",
+        "Chantal",
+        "Penelope",
+        "Miguel",
+        "Mia",
+        "Enrique",
+        "Conchita",
+        "Geraint",
+        "Salli",
+        "Matthew",
+        "Kimberly",
+        "Kendra",
+        "Justin",
+        "Joey",
+        "Joanna",
+        "Ivy",
+        "Raveena",
+        "Aditi",
+        "Emma",
+        "Brian",
+        "Amy",
+        "Russell",
+        "Nicole",
+        "Vicki",
+        "Marlene",
+        "Hans",
+        "Naja",
+        "Mads",
+        "Gwyneth",
+        "Zhiyu",
+        "es-ES-Standard-A",
+        "it-IT-Standard-A",
+        "it-IT-Wavenet-A",
+        "ja-JP-Standard-A",
+        "ja-JP-Wavenet-A",
+        "ko-KR-Standard-A",
+        "ko-KR-Wavenet-A",
+        "pt-BR-Standard-A",
+        "tr-TR-Standard-A",
+        "sv-SE-Standard-A",
+        "nl-NL-Standard-A",
+        "nl-NL-Wavenet-A",
+        "en-US-Wavenet-A",
+        "en-US-Wavenet-B",
+        "en-US-Wavenet-C",
+        "en-US-Wavenet-D",
+        "en-US-Wavenet-E",
+        "en-US-Wavenet-F",
+        "en-GB-Standard-A",
+        "en-GB-Standard-B",
+        "en-GB-Standard-C",
+        "en-GB-Standard-D",
+        "en-GB-Wavenet-A",
+        "en-GB-Wavenet-B",
+        "en-GB-Wavenet-C",
+        "en-GB-Wavenet-D",
+        "en-US-Standard-B",
+        "en-US-Standard-C",
+        "en-US-Standard-D",
+        "en-US-Standard-E",
+        "de-DE-Standard-A",
+        "de-DE-Standard-B",
+        "de-DE-Wavenet-A",
+        "de-DE-Wavenet-B",
+        "de-DE-Wavenet-C",
+        "de-DE-Wavenet-D",
+        "en-AU-Standard-A",
+        "en-AU-Standard-B",
+        "en-AU-Wavenet-A",
+        "en-AU-Wavenet-B",
+        "en-AU-Wavenet-C",
+        "en-AU-Wavenet-D",
+        "en-AU-Standard-C",
+        "en-AU-Standard-D",
+        "fr-CA-Standard-A",
+        "fr-CA-Standard-B",
+        "fr-CA-Standard-C",
+        "fr-CA-Standard-D",
+        "fr-FR-Standard-C",
+        "fr-FR-Standard-D",
+        "fr-FR-Wavenet-A",
+        "fr-FR-Wavenet-B",
+        "fr-FR-Wavenet-C",
+        "fr-FR-Wavenet-D",
+        "da-DK-Wavenet-A",
+        "pl-PL-Wavenet-A",
+        "pl-PL-Wavenet-B",
+        "pl-PL-Wavenet-C",
+        "pl-PL-Wavenet-D",
+        "pt-PT-Wavenet-A",
+        "pt-PT-Wavenet-B",
+        "pt-PT-Wavenet-C",
+        "pt-PT-Wavenet-D",
+        "ru-RU-Wavenet-A",
+        "ru-RU-Wavenet-B",
+        "ru-RU-Wavenet-C",
+        "ru-RU-Wavenet-D",
+        "sk-SK-Wavenet-A",
+        "tr-TR-Wavenet-A",
+        "tr-TR-Wavenet-B",
+        "tr-TR-Wavenet-C",
+        "tr-TR-Wavenet-D",
+        "tr-TR-Wavenet-E",
+        "uk-UA-Wavenet-A",
+        "ar-XA-Wavenet-A",
+        "ar-XA-Wavenet-B",
+        "ar-XA-Wavenet-C",
+        "cs-CZ-Wavenet-A",
+        "nl-NL-Wavenet-B",
+        "nl-NL-Wavenet-C",
+        "nl-NL-Wavenet-D",
+        "nl-NL-Wavenet-E",
+        "en-IN-Wavenet-A",
+        "en-IN-Wavenet-B",
+        "en-IN-Wavenet-C",
+        "fil-PH-Wavenet-A",
+        "fi-FI-Wavenet-A",
+        "el-GR-Wavenet-A",
+        "hi-IN-Wavenet-A",
+        "hi-IN-Wavenet-B",
+        "hi-IN-Wavenet-C",
+        "hu-HU-Wavenet-A",
+        "id-ID-Wavenet-A",
+        "id-ID-Wavenet-B",
+        "id-ID-Wavenet-C",
+        "it-IT-Wavenet-B",
+        "it-IT-Wavenet-C",
+        "it-IT-Wavenet-D",
+        "ja-JP-Wavenet-B",
+        "ja-JP-Wavenet-C",
+        "ja-JP-Wavenet-D",
+        "cmn-CN-Wavenet-A",
+        "cmn-CN-Wavenet-B",
+        "cmn-CN-Wavenet-C",
+        "cmn-CN-Wavenet-D",
+        "nb-no-Wavenet-E",
+        "nb-no-Wavenet-A",
+        "nb-no-Wavenet-B",
+        "nb-no-Wavenet-C",
+        "nb-no-Wavenet-D",
+        "vi-VN-Wavenet-A",
+        "vi-VN-Wavenet-B",
+        "vi-VN-Wavenet-C",
+        "vi-VN-Wavenet-D",
+        "sr-rs-Standard-A",
+        "lv-lv-Standard-A",
+        "is-is-Standard-A",
+        "bg-bg-Standard-A",
+        "af-ZA-Standard-A",
+        "Tracy",
+        "Danny",
+        "Huihui",
+        "Yaoyao",
+        "Kangkang",
+        "HanHan",
+        "Zhiwei",
+        "Asaf",
+        "An",
+        "Stefanos",
+        "Filip",
+        "Ivan",
+        "Heidi",
+        "Herena",
+        "Kalpana",
+        "Hemant",
+        "Matej",
+        "Andika",
+        "Rizwan",
+        "Lado",
+        "Valluvar",
+        "Linda",
+        "Heather",
+        "Sean",
+        "Michael",
+        "Karsten",
+        "Guillaume",
+        "Pattara",
+        "Jakub",
+        "Szabolcs",
+        "Hoda",
+        "Naayf",
+    ]
+
+    @classmethod
+    def text_to_audio(
+        cls,
+        message: str,
+        voice: str = "Brian",
+        proxies: dict[str, str] = {},
+        timeout: int = 30,
+        save_to: Union[Path, str] = None,
+        auto: bool = False,
+    ) -> Union[str, bytes]:
+        """
+        Text to speech using StreamElements API
+
+        Parameters:
+            message (str): The text to convert to speech
+            voice (str, optional): The voice to use for speech synthesis. Defaults to "Brian".
+            proxies (dict, optional): Http request proxies. Default to {}.
+            timeout (int, optional): Http request timeout. Defaults to 30.
+            save_to (bool, optional): Path to save the audio file. Defaults to None.
+            auto (bool, optional): Generate filename for the contents based on `message` and save to `cls.cache_dir`. Defaults to False.
+
+        Returns:
+            result (Union[str, bytes]): Path to saved contents or audio content.
+        """
+        assert (
+            voice in cls.all_voices
+        ), f"Voice '{voice}' not one of [{', '.join(cls.all_voices)}]"
+        # Base URL for provider API
+        url: str = (
+            f"https://api.streamelements.com/kappa/v2/speech?voice={voice}&text={{{message}}}"
+        )
+        resp = requests.get(
+            url=url, headers=cls.headers, stream=True, proxies=proxies, timeout=timeout
+        )
+        if not resp.ok:
+            raise Exception(
+                f"Failed to perform the operation - ({resp.status_code}, {resp.reason}) - {resp.text}"
+            )
+
+        def sanitize_filename(path):
+            trash = [
+                "\\",
+                "/",
+                ":",
+                "*",
+                "?",
+                '"',
+                "<",
+                "|",
+                ">",
+            ]
+            for val in trash:
+                path = path.replace(val, "")
+            return path.strip()
+
+        if auto:
+            filename: str = message + "..." if len(message) <= 40 else message[:40]
+            save_to = cls.cache_dir / sanitize_filename(filename)
+            save_to = save_to.as_posix()
+
+        if save_to:
+            if not save_to.endswith("mp3"):
+                save_to += ".mp3"
+
+            with open(save_to, "wb") as fh:
+                for chunk in resp.iter_content(chunk_size=512):
+                    fh.write(chunk)
+        else:
+            return resp.content
+        return save_to
+
+    @staticmethod
+    def play(path_to_audio_file: Union[Path, str]) -> NoReturn:
+        """Play audio (.mp3) using vlc media player or termux-media-player
+
+        Args:
+            path_to_audio_file (Union[Path, str]): Path to audio file.
+
+        Returns:
+            NoReturn: None
+        """
+        if not Path(path_to_audio_file).is_file():
+            raise FileNotFoundError(f"File does not exist - '{path_to_audio_file}'")
+
+        def play_using_vlc():
+            # create instance
+            instance = vlc.Instance()
+            # Create a Media Player object
+            player = instance.media_player_new()
+            # Load the audio file
+            media = instance.media_new(path_to_audio_file)
+            # Set the media to the player
+            player.set_media(media)
+            # Play the audio file
+            player.play()
+            # Keep the script running until the audio finishes playing
+            while player.get_state() != vlc.State.Ended:
+                pass
+
+        def play_using_termux_media_player():
+            # check if media-player is installed
+            check = run_system_command(
+                "termux-media-player --help",
+                exit_on_error=False,
+                stdout_error=False,
+                help="Install termux-api package in order to play audio files.\n apt update && apt install termux-api",
+            )[1]
+
+            if check.returncode == 127:
+                raise Exception(
+                    "Install termux-api package in order to play audio files.\n apt update && apt install termux-api"
+                )
+            try:
+                run_system_command(f'termux-media-player play "{path_to_audio_file}"')
+                while (
+                    run_system_command("termux-media-player info")[1].stdout.strip()
+                    != "No track currently!"
+                ):
+                    wait(1)
+            except (KeyboardInterrupt, KeyError) as e:
+                logging.debug(f"Stopping termux-media-player due to - {e}")
+                run_system_command("termux-media-player stop")
+
+        (
+            play_using_termux_media_player()
+            if "termux" in os.environ.get("PREFIX", "")
+            else play_using_vlc()
+        )
```

### Comparing `python_tgpt-0.6.4/src/pytgpt/webchatgpt/main.py` & `python_tgpt-0.6.5/src/pytgpt/webchatgpt/main.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.6.4/src/python_tgpt.egg-info/PKG-INFO` & `python_tgpt-0.6.5/src/python_tgpt.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-tgpt
-Version: 0.6.4
+Version: 0.6.5
 Summary: Interact with AI without API key
 Home-page: https://github.com/Simatwa/python-tgpt
 Author: Smartwa
 Author-email: simatwacaleb@proton.me
 Maintainer: Smartwa
 License: MIT
 Project-URL: Bug Report, https://github.com/Simatwa/python-tgpt/issues/new
@@ -36,14 +36,15 @@
 Requires-Dist: pyyaml==6.0.1
 Requires-Dist: webchatgpt==0.3.0
 Requires-Dist: GoogleBard1>=2.1.4
 Requires-Dist: poe-api-wrapper==1.3.6
 Requires-Dist: brotli==1.1.0
 Requires-Dist: g4f>=0.2.6.1
 Requires-Dist: Helpingai-T2==0.3
+Requires-Dist: python-vlc>=3.0.20
 Provides-Extra: cli
 Requires-Dist: click==8.1.3; extra == "cli"
 Requires-Dist: rich==13.3.4; extra == "cli"
 Requires-Dist: clipman==3.1.0; extra == "cli"
 Requires-Dist: pyperclip==1.8.2; extra == "cli"
 Requires-Dist: colorama==0.4.6; extra == "cli"
 Requires-Dist: g4f>=0.2.6.1; extra == "cli"
@@ -147,14 +148,15 @@
 9. [Phind](https://www.phind.com)
 10. [Llama2](https://www.llama2.ai)
 11. [Blackboxai](https://www.blackbox.ai)
 12. [gpt4all](https://gpt4all.io) *(Offline)*
 13. [Poe](https://poe.com) - Poe|Quora *(Session ID required)*
 14. [Groq](https://console.groq.com/playground) *(API Key required)*
 15. [Perplexity](https://www.perplexity.ai)
+16. [YepChat](https://yep.com)
 
 
 <details>
 
 <summary>
 
 41+ providers proudly offered by [gpt4free](https://github.com/xtekky/gpt4free).
@@ -463,14 +465,25 @@
 img.save(img_generator)
 
 # RAM friendly
 ```
 
 </details>
 
+#### Using **Prodia** provider
+
+```python
+from pytgpt.imager import Prodia
+
+img = Prodia()
+
+img_generator = img.generate('Coding bot', amount=3, stream=True)
+
+img.save(img_generator)
+```
 
 </details>
 
 ### Advanced Usage of Placeholders
 
 The `generate` functionality has been enhanced starting from *v0.3.0* to enable comprehensive utilization of the `--with-copied` option and support for accepting piped inputs. This improvement introduces placeholders, offering dynamic values for more versatile interactions.
 
@@ -533,21 +546,59 @@
 
 The environment variables can be overridden by explicitly declaring new value.
 
 > [!TIP]
 > Save the variables in a `.env` file in your current directory or export them in your `~/.zshrc` file.
 > To load previous conversations from a `.txt` file, use the `-fp` or `--filepath` flag. If no flag is passed, the default one will be used. To load context from a file without altering its content, use the `--retain-file` flag.
 
-## Dynamic Provider
+## Dynamic Provider & Further Interfaces
 
 Version **0.4.6** also introduces dynamic provider called `g4fauto`, which represents the fastest working g4f-based provider.
 
 > [!TIP]
-> To launch web interface for g4f-based providers simply run `$ pytgpt gpt4free gui`. 
+> To launch web interface for g4f-based providers simply run `$ pytgpt gpt4free gui`.
 > `$ pytgpt api run` will start the REST-API. Access docs and redoc at */docs* and */redoc* respectively.
+To launch the web interface for g4f-based providers, execute the following command in your terminal:
+
+```bash
+$ pytgpt gpt4free gui
+```
+
+This command initializes the Web-user interface for interacting with g4f-based providers.
+
+To start the REST-API:
+
+```bash
+$ pytgpt api run
+```
+
+This command starts the RESTful API server, enabling you to interact with the service programmatically.
+
+For accessing the documentation and redoc, navigate to the following paths in your web browser:
+- Documentation: `*/docs`
+- ReDoc: `*/redoc`
+
+## Speech Synthesis
+
+To enable speech synthesis of responses, ensure you have either the [VLC player](https://www.videolan.org/vlc/index.html) installed on your system or, if you are a [Termux](https://termux.org) user, the [Termux:API](https://wiki.termux.com/wiki/Termux:API) package.
+
+To activate speech synthesis, use the `--talk-to-me` flag or its shorthand `-ttm` when running your commands. For example:
+```bash
+$ pytgpt generate "Generate an ogre story" --talk-to-me
+```
+or
+```bash
+$ pytgpt interactive -ttm
+```
+This flag instructs the system to audiolize the ai responses and then play them, enhancing the user experience by providing auditory feedback.
+
+> To speech synthesise the responses just ensure you have [vlc player]() in your system or [termux-api](https://wiki.termux.com/wiki/Termux:API) for the case of [Termux](https://termux.org) users.
+> Use the flag `--talk-to-me`, shortform `-ttm`.
+
+Version **0.6.4** introduces another dynamic provider, `auto`, which denotes the working provider **overall**. This relieves you of the workload of manually checking a working provider each time you fire up pytgpt.
 
 <details>
 
 <summary>
 
 For more usage info run `$ pytgpt --help`
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: python-tgpt Version: 0.6.4 Summary: Interact with
+Metadata-Version: 2.1 Name: python-tgpt Version: 0.6.5 Summary: Interact with
 AI without API key Home-page: https://github.com/Simatwa/python-tgpt Author:
 Smartwa Author-email: simatwacaleb@proton.me Maintainer: Smartwa License: MIT
 Project-URL: Bug Report, https://github.com/Simatwa/python-tgpt/issues/new
 Project-URL: Homepage, https://github.com/Simatwa/python-tgpt Project-URL:
 Source Code, https://github.com/Simatwa/python-tgpt Project-URL: Issue Tracker,
 https://github.com/Simatwa/python-tgpt/issues Project-URL: Download, https://
 github.com/Simatwa/python-tgpt/releases Project-URL: Documentation, https://
@@ -20,27 +20,28 @@
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12 Requires-Python: >=3.10
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 requests[socks]==2.31.0 Requires-Dist: appdirs==1.4.4 Requires-Dist:
 pyyaml==6.0.1 Requires-Dist: webchatgpt==0.3.0 Requires-Dist:
 GoogleBard1>=2.1.4 Requires-Dist: poe-api-wrapper==1.3.6 Requires-Dist:
 brotli==1.1.0 Requires-Dist: g4f>=0.2.6.1 Requires-Dist: Helpingai-T2==0.3
-Provides-Extra: cli Requires-Dist: click==8.1.3; extra == "cli" Requires-Dist:
-rich==13.3.4; extra == "cli" Requires-Dist: clipman==3.1.0; extra == "cli"
-Requires-Dist: pyperclip==1.8.2; extra == "cli" Requires-Dist: colorama==0.4.6;
-extra == "cli" Requires-Dist: g4f>=0.2.6.1; extra == "cli" Requires-Dist:
-python-dotenv==1.0.0; extra == "cli" Provides-Extra: api Requires-Dist: fastapi
-[all]==0.110.1; extra == "api" Provides-Extra: all Requires-Dist: g4f
-[all]>=0.2.6.1; extra == "all" Requires-Dist: matplotlib; extra == "all"
-Requires-Dist: gpt4all==2.2.0; extra == "all" Requires-Dist: click==8.1.3;
-extra == "all" Requires-Dist: rich==13.3.4; extra == "all" Requires-Dist:
-clipman==3.1.0; extra == "all" Requires-Dist: pyperclip==1.8.2; extra == "all"
-Requires-Dist: colorama==0.4.6; extra == "all" Requires-Dist: g4f>=0.2.6.1;
-extra == "all" Requires-Dist: python-dotenv==1.0.0; extra == "all" Requires-
-Dist: fastapi[all]==0.110.1; extra == "all"
+Requires-Dist: python-vlc>=3.0.20 Provides-Extra: cli Requires-Dist:
+click==8.1.3; extra == "cli" Requires-Dist: rich==13.3.4; extra == "cli"
+Requires-Dist: clipman==3.1.0; extra == "cli" Requires-Dist: pyperclip==1.8.2;
+extra == "cli" Requires-Dist: colorama==0.4.6; extra == "cli" Requires-Dist:
+g4f>=0.2.6.1; extra == "cli" Requires-Dist: python-dotenv==1.0.0; extra ==
+"cli" Provides-Extra: api Requires-Dist: fastapi[all]==0.110.1; extra == "api"
+Provides-Extra: all Requires-Dist: g4f[all]>=0.2.6.1; extra == "all" Requires-
+Dist: matplotlib; extra == "all" Requires-Dist: gpt4all==2.2.0; extra == "all"
+Requires-Dist: click==8.1.3; extra == "all" Requires-Dist: rich==13.3.4; extra
+== "all" Requires-Dist: clipman==3.1.0; extra == "all" Requires-Dist:
+pyperclip==1.8.2; extra == "all" Requires-Dist: colorama==0.4.6; extra == "all"
+Requires-Dist: g4f>=0.2.6.1; extra == "all" Requires-Dist: python-
+dotenv==1.0.0; extra == "all" Requires-Dist: fastapi[all]==0.110.1; extra ==
+"all"
 [https://github.com/Simatwa/python-tgpt/blob/main/assets/py-tgpt.png?raw=true]
 _[_L_i_c_e_n_s_e_]_[_P_y_t_h_o_n_ _v_e_r_s_i_o_n_]_[_P_y_P_i_]_[_B_l_a_c_k_]_[_P_a_s_s_i_n_g_]_[_P_y_t_h_o_n_ _P_a_c_k_a_g_e_ _f_l_o_w_]_[_c_o_v_e_r_a_g_e_]
    _[_D_o_w_n_l_o_a_d_s_]_[_D_o_w_n_l_o_a_d_s_]_[_D_o_w_n_l_o_a_d_s_]_[_L_a_t_e_s_t_ _r_e_l_e_a_s_e_]_[_r_e_l_e_a_s_e_ _d_a_t_e_]_[_h_t_t_p_s_:_/_/
   _h_i_t_s_._s_e_e_y_o_u_f_a_r_m_._c_o_m_/_a_p_i_/_c_o_u_n_t_/_i_n_c_r_/_b_a_d_g_e_._s_v_g_?_u_r_l_=_h_t_t_p_s_%_3_A_%_2_F_%_2_F_g_i_t_h_u_b_._c_o_m_/
                         _S_i_m_a_t_w_a_/_p_y_t_h_o_n_-_t_g_p_t_]_[_w_a_k_a_t_i_m_e_]
                              ******** ppyytthhoonn--ttggpptt ********
  [https://github.com/Simatwa/python-tgpt/blob/main/assets/demo-1.gif?raw=True]
@@ -69,37 +70,38 @@
 uc.a.run.app/) 4. [OpenAI](https://chat.openai.com) *(API key required)* 5.
 [WebChatGPT](https://github.com/Simatwa/WebChatGPT) - **OpenAI** *(Session ID
 required)* 6. [Gemini](https://github.com/Simatwa/bard) - **Google** *(Session
 ID required)* 9. [Phind](https://www.phind.com) 10. [Llama2](https://
 www.llama2.ai) 11. [Blackboxai](https://www.blackbox.ai) 12. [gpt4all](https://
 gpt4all.io) *(Offline)* 13. [Poe](https://poe.com) - Poe|Quora *(Session ID
 required)* 14. [Groq](https://console.groq.com/playground) *(API Key required)*
-15. [Perplexity](https://www.perplexity.ai) 41+ providers proudly offered by
-[gpt4free](https://github.com/xtekky/gpt4free). - To list working providers
-run: ```sh $ pytgpt gpt4free test -y ``` ## Prerequisites - [x] [Python>=3.10]
-(https://python.org) *(Optional)* ## Installation and Usage ### Installation
-Download binaries for your system from [here.](https://github.com/Simatwa/
-python-tgpt/releases/latest/) Alternatively, you can install non-binaries. *
-(Recommended)* 1. Developers: ```sh pip install --upgrade python-tgpt ``` 2.
-Commandline: ```sh pip install --upgrade "python-tgpt[cli]" ``` 3. Full
-installation: ```sh pip install --upgrade "python-tgpt[all]" ``` > `pip install
--U "python-tgt[api]"` will install REST API dependencies. ## Usage This package
-offers a convenient command-line interface. > [!NOTE] > `phind` is the default
-*provider*. - For a quick response: ```bash python -m pytgpt generate "" ``` -
-For interactive mode: ```bash python -m pytgpt interactive "" ``` Make use of
-flag `--provider` followed by the provider name of your choice. e.g `--provider
-koboldai` > To list all providers offered by gpt4free, use following commands:
-```pytgpt gpt4free list providers``` You can also simply use `pytgpt` instead
-of `python -m pytgpt`. Starting from version 0.2.7, running `$ pytgpt` without
-any other command or option will automatically enter the `interactive` mode.
-Otherwise, you'll need to explicitly declare the desired action, for example,
-by running `$ pytgpt generate`. ### Developer Docs 1. Generate a quick response
-```python from pytgpt.leo import LEO bot = LEO() resp = bot.chat('') print
-(resp) # Output : How may I help you. ``` 2. Get back whole response ```python
-from pytgpt.leo import LEO bot = LEO() resp = bot.ask('
+15. [Perplexity](https://www.perplexity.ai) 16. [YepChat](https://yep.com) 41+
+providers proudly offered by [gpt4free](https://github.com/xtekky/gpt4free). -
+To list working providers run: ```sh $ pytgpt gpt4free test -y ``` ##
+Prerequisites - [x] [Python>=3.10](https://python.org) *(Optional)* ##
+Installation and Usage ### Installation Download binaries for your system from
+[here.](https://github.com/Simatwa/python-tgpt/releases/latest/) Alternatively,
+you can install non-binaries. *(Recommended)* 1. Developers: ```sh pip install
+--upgrade python-tgpt ``` 2. Commandline: ```sh pip install --upgrade "python-
+tgpt[cli]" ``` 3. Full installation: ```sh pip install --upgrade "python-tgpt
+[all]" ``` > `pip install -U "python-tgt[api]"` will install REST API
+dependencies. ## Usage This package offers a convenient command-line interface.
+> [!NOTE] > `phind` is the default *provider*. - For a quick response: ```bash
+python -m pytgpt generate "" ``` - For interactive mode: ```bash python -
+m pytgpt interactive "" ``` Make use of flag `--provider` followed by the
+provider name of your choice. e.g `--provider koboldai` > To list all providers
+offered by gpt4free, use following commands: ```pytgpt gpt4free list
+providers``` You can also simply use `pytgpt` instead of `python -m pytgpt`.
+Starting from version 0.2.7, running `$ pytgpt` without any other command or
+option will automatically enter the `interactive` mode. Otherwise, you'll need
+to explicitly declare the desired action, for example, by running `$ pytgpt
+generate`. ### Developer Docs 1. Generate a quick response ```python from
+pytgpt.leo import LEO bot = LEO() resp = bot.chat('') print(resp) # Output :
+How may I help you. ``` 2. Get back whole response ```python from pytgpt.leo
+import LEO bot = LEO() resp = bot.ask('
  Output """ {'completion': "I'm so excited to share with you the incredible
 experiences...", 'stop_reason': None, 'truncated': False, 'stop': None,
 'model': 'llama-2-13b-chat', 'log_id': 'cmpl-3NmRt5A5Djqo2jXtXLBwJ2',
 'exception': None} """ ``` #### Stream Response Just add parameter `stream`
 with value `true`. 1. Text Generated only ```python from pytgpt.leo import LEO
 bot = LEO() resp = bot.chat('', stream=True) for value in resp: print(value) #
 output """ How may How may I help How may I help you How may I help you today?
@@ -141,25 +143,27 @@
 informed that majority of providers offered by *gpt4free* requires *Google
 Chrome* inorder to function. ### Image Generation This has been made possible
 by [pollinations.ai](https://pollination.ai). ```sh $ pytgpt imager "" # e.g
 pytgpt imager "Coding bot" ``` Developers ```python from pytgpt.imager import
 Imager img = Imager() generated_img = img.generate('Coding bot') # [bytes]
 img.save(generated_img) ``` Download Multiple Images ```python from
 pytgpt.imager import Imager img = Imager() img_generator = img.generate('Coding
-bot', amount=3, stream=True) img.save(img_generator) # RAM friendly ``` ###
-Advanced Usage of Placeholders The `generate` functionality has been enhanced
-starting from *v0.3.0* to enable comprehensive utilization of the `--with-
-copied` option and support for accepting piped inputs. This improvement
-introduces placeholders, offering dynamic values for more versatile
-interactions. | Placeholder | Represents | | ------------ | ----------- | | `{
-{stream}}` | The piped input | | `{{copied}}` | The last copied text | This
-feature is particularly beneficial for intricate operations. For example:
-```bash $ git diff | pytgpt generate "Here is a diff file: {{stream}} Make a
-concise commit message from it, aligning with my commit message history: {
-{copied}}" --shell --new ``` > In this illustration, `{{stream}}` denotes the
+bot', amount=3, stream=True) img.save(img_generator) # RAM friendly ``` ####
+Using **Prodia** provider ```python from pytgpt.imager import Prodia img =
+Prodia() img_generator = img.generate('Coding bot', amount=3, stream=True)
+img.save(img_generator) ``` ### Advanced Usage of Placeholders The `generate`
+functionality has been enhanced starting from *v0.3.0* to enable comprehensive
+utilization of the `--with-copied` option and support for accepting piped
+inputs. This improvement introduces placeholders, offering dynamic values for
+more versatile interactions. | Placeholder | Represents | | ------------ | ----
+------- | | `{{stream}}` | The piped input | | `{{copied}}` | The last copied
+text | This feature is particularly beneficial for intricate operations. For
+example: ```bash $ git diff | pytgpt generate "Here is a diff file: {{stream}}
+Make a concise commit message from it, aligning with my commit message history:
+{{copied}}" --shell --new ``` > In this illustration, `{{stream}}` denotes the
 result of the `$ git diff` operation, while `{{copied}}` signifies the content
 copied from the output of the `$ git log` command. ### Awesome Prompts [These
 prompts](https://github.com/Simatwa/gpt-cli/blob/main/assets/all-
 acts.pdf?raw=True) are designed to guide the AI's behavior or responses in a
 particular direction, encouraging it to exhibit certain characteristics or
 behaviors. The term "awesome-prompt" is not a formal term in AI or machine
 learning literature, but it encapsulates the idea of crafting prompts that are
@@ -192,24 +196,46 @@
 prompt` will take the environment variable `PYTGPT_AWESOME_PROMPT`. > [!NOTE] >
 This is **NOT** limited to any command The environment variables can be
 overridden by explicitly declaring new value. > [!TIP] > Save the variables in
 a `.env` file in your current directory or export them in your `~/.zshrc` file.
 > To load previous conversations from a `.txt` file, use the `-fp` or `--
 filepath` flag. If no flag is passed, the default one will be used. To load
 context from a file without altering its content, use the `--retain-file` flag.
-## Dynamic Provider Version **0.4.6** also introduces dynamic provider called
-`g4fauto`, which represents the fastest working g4f-based provider. > [!TIP] >
-To launch web interface for g4f-based providers simply run `$ pytgpt gpt4free
-gui`. > `$ pytgpt api run` will start the REST-API. Access docs and redoc at */
-docs* and */redoc* respectively. For more usage info run `$ pytgpt --help` ```
-Usage: pytgpt [OPTIONS] COMMAND [ARGS]... Options: -v, --version Show the
-version and exit. -h, --help Show this message and exit. Commands: api FastAPI
-control endpoint awesome Perform CRUD operations on awesome-prompts generate
-Generate a quick response with AI gpt4free Discover gpt4free models, providers
-etc imager Generate images with pollinations.ai interactive Chat with AI
-interactively (Default) utils Utility endpoint for pytgpt webchatgpt Reverse
-Engineered ChatGPT Web-Version ``` ### API Health Status | No. | API | Status |
-|--------|-----|--------| | 1. | [On-render](https://python-tgpt.onrender.com)
-| [cron-job](https://pqfzhmvz.status.cron-job.org/) | ## [CHANGELOG](https://
+## Dynamic Provider & Further Interfaces Version **0.4.6** also introduces
+dynamic provider called `g4fauto`, which represents the fastest working g4f-
+based provider. > [!TIP] > To launch web interface for g4f-based providers
+simply run `$ pytgpt gpt4free gui`. > `$ pytgpt api run` will start the REST-
+API. Access docs and redoc at */docs* and */redoc* respectively. To launch the
+web interface for g4f-based providers, execute the following command in your
+terminal: ```bash $ pytgpt gpt4free gui ``` This command initializes the Web-
+user interface for interacting with g4f-based providers. To start the REST-API:
+```bash $ pytgpt api run ``` This command starts the RESTful API server,
+enabling you to interact with the service programmatically. For accessing the
+documentation and redoc, navigate to the following paths in your web browser: -
+Documentation: `*/docs` - ReDoc: `*/redoc` ## Speech Synthesis To enable speech
+synthesis of responses, ensure you have either the [VLC player](https://
+www.videolan.org/vlc/index.html) installed on your system or, if you are a
+[Termux](https://termux.org) user, the [Termux:API](https://wiki.termux.com/
+wiki/Termux:API) package. To activate speech synthesis, use the `--talk-to-me`
+flag or its shorthand `-ttm` when running your commands. For example: ```bash $
+pytgpt generate "Generate an ogre story" --talk-to-me ``` or ```bash $ pytgpt
+interactive -ttm ``` This flag instructs the system to audiolize the ai
+responses and then play them, enhancing the user experience by providing
+auditory feedback. > To speech synthesise the responses just ensure you have
+[vlc player]() in your system or [termux-api](https://wiki.termux.com/wiki/
+Termux:API) for the case of [Termux](https://termux.org) users. > Use the flag
+`--talk-to-me`, shortform `-ttm`. Version **0.6.4** introduces another dynamic
+provider, `auto`, which denotes the working provider **overall**. This relieves
+you of the workload of manually checking a working provider each time you fire
+up pytgpt. For more usage info run `$ pytgpt --help` ``` Usage: pytgpt
+[OPTIONS] COMMAND [ARGS]... Options: -v, --version Show the version and exit. -
+h, --help Show this message and exit. Commands: api FastAPI control endpoint
+awesome Perform CRUD operations on awesome-prompts generate Generate a quick
+response with AI gpt4free Discover gpt4free models, providers etc imager
+Generate images with pollinations.ai interactive Chat with AI interactively
+(Default) utils Utility endpoint for pytgpt webchatgpt Reverse Engineered
+ChatGPT Web-Version ``` ### API Health Status | No. | API | Status | |--------
+|-----|--------| | 1. | [On-render](https://python-tgpt.onrender.com) | [cron-
+job](https://pqfzhmvz.status.cron-job.org/) | ## [CHANGELOG](https://
 github.com/Simatwa/python-tgpt/blob/main/docs/CHANGELOG.md) ## Acknowledgements
 1. [x] [tgpt](https://github.com/aandrew-me/tgpt) 2. [x] [gpt4free](https://
 github.com/xtekky/gpt4free)
```

### Comparing `python_tgpt-0.6.4/src/python_tgpt.egg-info/SOURCES.txt` & `python_tgpt-0.6.5/src/python_tgpt.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -40,14 +40,16 @@
 src/pytgpt/perplexity/main.py
 src/pytgpt/phind/__init__.py
 src/pytgpt/phind/main.py
 src/pytgpt/poe/__init__.py
 src/pytgpt/poe/main.py
 src/pytgpt/webchatgpt/__init__.py
 src/pytgpt/webchatgpt/main.py
+src/pytgpt/yepchat/__init__.py
+src/pytgpt/yepchat/main.py
 src/python_tgpt.egg-info/PKG-INFO
 src/python_tgpt.egg-info/SOURCES.txt
 src/python_tgpt.egg-info/dependency_links.txt
 src/python_tgpt.egg-info/entry_points.txt
 src/python_tgpt.egg-info/requires.txt
 src/python_tgpt.egg-info/top_level.txt
 tests/test_api.py
```

### Comparing `python_tgpt-0.6.4/tests/test_api.py` & `python_tgpt-0.6.5/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.6.4/tests/test_imager.py` & `python_tgpt-0.6.5/tests/test_imager.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.6.4/tests/test_utils.py` & `python_tgpt-0.6.5/tests/test_utils.py`

 * *Files identical despite different names*


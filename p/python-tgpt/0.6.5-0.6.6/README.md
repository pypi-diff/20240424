# Comparing `tmp/python_tgpt-0.6.5.tar.gz` & `tmp/python_tgpt-0.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_tgpt-0.6.5.tar", last modified: Tue Apr 23 22:20:13 2024, max compression
+gzip compressed data, was "python_tgpt-0.6.6.tar", last modified: Wed Apr 24 16:45:06 2024, max compression
```

## Comparing `python_tgpt-0.6.5.tar` & `python_tgpt-0.6.6.tar`

### file list

```diff
@@ -1,97 +1,97 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:20:13.925598 python_tgpt-0.6.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-23 22:19:32.000000 python_tgpt-0.6.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    21581 2024-04-23 22:20:13.925598 python_tgpt-0.6.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    18668 2024-04-23 22:20:13.000000 python_tgpt-0.6.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 22:20:13.925598 python_tgpt-0.6.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3205 2024-04-23 22:19:32.000000 python_tgpt-0.6.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:20:13.909598 python_tgpt-0.6.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:20:13.913598 python_tgpt-0.6.5/src/pytgpt/
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-23 22:19:32.000000 python_tgpt-0.6.5/src/pytgpt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-23 22:19:32.000000 python_tgpt-0.6.5/src/pytgpt/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:20:13.913598 python_tgpt-0.6.5/src/pytgpt/api/
--rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-04-23 22:19:32.000000 python_tgpt-0.6.5/src/pytgpt/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-23 22:19:32.000000 python_tgpt-0.6.5/src/pytgpt/api/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-04-23 22:19:32.000000 python_tgpt-0.6.5/src/pytgpt/api/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    17395 2024-04-23 22:19:32.000000 python_tgpt-0.6.5/src/pytgpt/api/v1.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:20:13.913598 python_tgpt-0.6.5/src/pytgpt/auto/
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-23 22:19:32.000000 python_tgpt-0.6.5/src/pytgpt/auto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-23 22:19:32.000000 python_tgpt-0.6.5/src/pytgpt/auto/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     7999 2024-04-23 22:19:32.000000 python_tgpt-0.6.5/src/pytgpt/auto/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-04-23 22:19:32.000000 python_tgpt-0.6.5/src/pytgpt/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:20:13.913598 python_tgpt-0.6.5/src/pytgpt/blackboxai/
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-23 22:19:32.000000 python_tgpt-0.6.5/src/pytgpt/blackboxai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7753 2024-04-23 22:19:32.000000 python_tgpt-0.6.5/src/pytgpt/blackboxai/main.py
--rw-r--r--   0 runner    (1001) docker     (127)    84784 2024-04-23 22:19:32.000000 python_tgpt-0.6.5/src/pytgpt/console.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:20:13.913598 python_tgpt-0.6.5/src/pytgpt/gemini/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-23 22:19:32.000000 python_tgpt-0.6.5/src/pytgpt/gemini/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7460 2024-04-23 22:19:32.000000 python_tgpt-0.6.5/src/pytgpt/gemini/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:20:13.913598 python_tgpt-0.6.5/src/pytgpt/gpt4all/
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-23 22:19:32.000000 python_tgpt-0.6.5/src/pytgpt/gpt4all/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7595 2024-04-23 22:19:32.000000 python_tgpt-0.6.5/src/pytgpt/gpt4all/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:20:13.913598 python_tgpt-0.6.5/src/pytgpt/gpt4free/
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-23 22:19:32.000000 python_tgpt-0.6.5/src/pytgpt/gpt4free/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9078 2024-04-23 22:19:32.000000 python_tgpt-0.6.5/src/pytgpt/gpt4free/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     7293 2024-04-23 22:19:32.000000 python_tgpt-0.6.5/src/pytgpt/gpt4free/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:20:13.917598 python_tgpt-0.6.5/src/pytgpt/groq/
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-23 22:19:32.000000 python_tgpt-0.6.5/src/pytgpt/groq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10062 2024-04-23 22:19:32.000000 python_tgpt-0.6.5/src/pytgpt/groq/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:20:13.917598 python_tgpt-0.6.5/src/pytgpt/imager/
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-23 22:19:32.000000 python_tgpt-0.6.5/src/pytgpt/imager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8191 2024-04-23 22:19:32.000000 python_tgpt-0.6.5/src/pytgpt/imager/imager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:20:13.917598 python_tgpt-0.6.5/src/pytgpt/koboldai/
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-23 22:19:32.000000 python_tgpt-0.6.5/src/pytgpt/koboldai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7308 2024-04-23 22:19:32.000000 python_tgpt-0.6.5/src/pytgpt/koboldai/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:20:13.917598 python_tgpt-0.6.5/src/pytgpt/leo/
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-23 22:19:32.000000 python_tgpt-0.6.5/src/pytgpt/leo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9685 2024-04-23 22:19:32.000000 python_tgpt-0.6.5/src/pytgpt/leo/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:20:13.917598 python_tgpt-0.6.5/src/pytgpt/llama2/
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-23 22:19:32.000000 python_tgpt-0.6.5/src/pytgpt/llama2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8180 2024-04-23 22:19:32.000000 python_tgpt-0.6.5/src/pytgpt/llama2/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:20:13.917598 python_tgpt-0.6.5/src/pytgpt/openai/
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-23 22:19:32.000000 python_tgpt-0.6.5/src/pytgpt/openai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9597 2024-04-23 22:19:32.000000 python_tgpt-0.6.5/src/pytgpt/openai/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:20:13.917598 python_tgpt-0.6.5/src/pytgpt/opengpt/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-23 22:19:32.000000 python_tgpt-0.6.5/src/pytgpt/opengpt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8709 2024-04-23 22:19:32.000000 python_tgpt-0.6.5/src/pytgpt/opengpt/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:20:13.917598 python_tgpt-0.6.5/src/pytgpt/perplexity/
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-23 22:19:32.000000 python_tgpt-0.6.5/src/pytgpt/perplexity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7907 2024-04-23 22:19:32.000000 python_tgpt-0.6.5/src/pytgpt/perplexity/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:20:13.917598 python_tgpt-0.6.5/src/pytgpt/phind/
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-23 22:19:32.000000 python_tgpt-0.6.5/src/pytgpt/phind/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9139 2024-04-23 22:19:32.000000 python_tgpt-0.6.5/src/pytgpt/phind/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:20:13.917598 python_tgpt-0.6.5/src/pytgpt/poe/
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-23 22:19:32.000000 python_tgpt-0.6.5/src/pytgpt/poe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7455 2024-04-23 22:19:32.000000 python_tgpt-0.6.5/src/pytgpt/poe/main.py
--rw-r--r--   0 runner    (1001) docker     (127)    33719 2024-04-23 22:19:32.000000 python_tgpt-0.6.5/src/pytgpt/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:20:13.917598 python_tgpt-0.6.5/src/pytgpt/webchatgpt/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-23 22:19:32.000000 python_tgpt-0.6.5/src/pytgpt/webchatgpt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7114 2024-04-23 22:19:32.000000 python_tgpt-0.6.5/src/pytgpt/webchatgpt/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:20:13.917598 python_tgpt-0.6.5/src/pytgpt/yepchat/
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-23 22:19:32.000000 python_tgpt-0.6.5/src/pytgpt/yepchat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9434 2024-04-23 22:19:32.000000 python_tgpt-0.6.5/src/pytgpt/yepchat/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:20:13.921598 python_tgpt-0.6.5/src/python_tgpt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    21581 2024-04-23 22:20:13.000000 python_tgpt-0.6.5/src/python_tgpt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-04-23 22:20:13.000000 python_tgpt-0.6.5/src/python_tgpt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 22:20:13.000000 python_tgpt-0.6.5/src/python_tgpt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-23 22:20:13.000000 python_tgpt-0.6.5/src/python_tgpt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-23 22:20:13.000000 python_tgpt-0.6.5/src/python_tgpt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-23 22:20:13.000000 python_tgpt-0.6.5/src/python_tgpt.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:20:13.921598 python_tgpt-0.6.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3342 2024-04-23 22:19:32.000000 python_tgpt-0.6.5/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-23 22:19:32.000000 python_tgpt-0.6.5/tests/test_auto.py
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-23 22:19:32.000000 python_tgpt-0.6.5/tests/test_blackboxai.py
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-23 22:19:32.000000 python_tgpt-0.6.5/tests/test_gemini.py
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-23 22:19:32.000000 python_tgpt-0.6.5/tests/test_gpt4all.py
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-23 22:19:32.000000 python_tgpt-0.6.5/tests/test_gpt4free.py
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-23 22:19:32.000000 python_tgpt-0.6.5/tests/test_groq.py
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-23 22:19:32.000000 python_tgpt-0.6.5/tests/test_imager.py
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-23 22:19:32.000000 python_tgpt-0.6.5/tests/test_koboldai.py
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-23 22:19:32.000000 python_tgpt-0.6.5/tests/test_leo.py
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-23 22:19:32.000000 python_tgpt-0.6.5/tests/test_llama2.py
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-23 22:19:32.000000 python_tgpt-0.6.5/tests/test_openai.py
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-23 22:19:32.000000 python_tgpt-0.6.5/tests/test_opengpt.py
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-23 22:19:32.000000 python_tgpt-0.6.5/tests/test_perplexity.py
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-23 22:19:32.000000 python_tgpt-0.6.5/tests/test_phind.py
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-23 22:19:32.000000 python_tgpt-0.6.5/tests/test_poe.py
--rw-r--r--   0 runner    (1001) docker     (127)     4202 2024-04-23 22:19:32.000000 python_tgpt-0.6.5/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-23 22:19:32.000000 python_tgpt-0.6.5/tests/test_webchatgpt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:45:06.301255 python_tgpt-0.6.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-24 16:44:33.000000 python_tgpt-0.6.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    21914 2024-04-24 16:45:06.301255 python_tgpt-0.6.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    19001 2024-04-24 16:45:06.000000 python_tgpt-0.6.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 16:45:06.301255 python_tgpt-0.6.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3205 2024-04-24 16:44:33.000000 python_tgpt-0.6.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:45:06.289255 python_tgpt-0.6.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:45:06.289255 python_tgpt-0.6.6/src/pytgpt/
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-24 16:44:33.000000 python_tgpt-0.6.6/src/pytgpt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-24 16:44:33.000000 python_tgpt-0.6.6/src/pytgpt/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:45:06.289255 python_tgpt-0.6.6/src/pytgpt/api/
+-rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-04-24 16:44:33.000000 python_tgpt-0.6.6/src/pytgpt/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-24 16:44:33.000000 python_tgpt-0.6.6/src/pytgpt/api/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-04-24 16:44:33.000000 python_tgpt-0.6.6/src/pytgpt/api/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17394 2024-04-24 16:44:33.000000 python_tgpt-0.6.6/src/pytgpt/api/v1.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:45:06.289255 python_tgpt-0.6.6/src/pytgpt/auto/
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-24 16:44:33.000000 python_tgpt-0.6.6/src/pytgpt/auto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-24 16:44:33.000000 python_tgpt-0.6.6/src/pytgpt/auto/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7999 2024-04-24 16:44:33.000000 python_tgpt-0.6.6/src/pytgpt/auto/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-04-24 16:44:33.000000 python_tgpt-0.6.6/src/pytgpt/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:45:06.289255 python_tgpt-0.6.6/src/pytgpt/blackboxai/
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-24 16:44:33.000000 python_tgpt-0.6.6/src/pytgpt/blackboxai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7753 2024-04-24 16:44:33.000000 python_tgpt-0.6.6/src/pytgpt/blackboxai/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    84784 2024-04-24 16:44:33.000000 python_tgpt-0.6.6/src/pytgpt/console.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:45:06.289255 python_tgpt-0.6.6/src/pytgpt/gemini/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-24 16:44:33.000000 python_tgpt-0.6.6/src/pytgpt/gemini/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7460 2024-04-24 16:44:33.000000 python_tgpt-0.6.6/src/pytgpt/gemini/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:45:06.293255 python_tgpt-0.6.6/src/pytgpt/gpt4all/
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-24 16:44:33.000000 python_tgpt-0.6.6/src/pytgpt/gpt4all/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7595 2024-04-24 16:44:33.000000 python_tgpt-0.6.6/src/pytgpt/gpt4all/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:45:06.293255 python_tgpt-0.6.6/src/pytgpt/gpt4free/
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-24 16:44:33.000000 python_tgpt-0.6.6/src/pytgpt/gpt4free/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9078 2024-04-24 16:44:33.000000 python_tgpt-0.6.6/src/pytgpt/gpt4free/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7293 2024-04-24 16:44:33.000000 python_tgpt-0.6.6/src/pytgpt/gpt4free/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:45:06.293255 python_tgpt-0.6.6/src/pytgpt/groq/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-24 16:44:33.000000 python_tgpt-0.6.6/src/pytgpt/groq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10062 2024-04-24 16:44:33.000000 python_tgpt-0.6.6/src/pytgpt/groq/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:45:06.293255 python_tgpt-0.6.6/src/pytgpt/imager/
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-24 16:44:33.000000 python_tgpt-0.6.6/src/pytgpt/imager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8191 2024-04-24 16:44:33.000000 python_tgpt-0.6.6/src/pytgpt/imager/imager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:45:06.293255 python_tgpt-0.6.6/src/pytgpt/koboldai/
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-24 16:44:33.000000 python_tgpt-0.6.6/src/pytgpt/koboldai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7308 2024-04-24 16:44:33.000000 python_tgpt-0.6.6/src/pytgpt/koboldai/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:45:06.293255 python_tgpt-0.6.6/src/pytgpt/leo/
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-24 16:44:33.000000 python_tgpt-0.6.6/src/pytgpt/leo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9685 2024-04-24 16:44:33.000000 python_tgpt-0.6.6/src/pytgpt/leo/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:45:06.293255 python_tgpt-0.6.6/src/pytgpt/llama2/
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-24 16:44:33.000000 python_tgpt-0.6.6/src/pytgpt/llama2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8180 2024-04-24 16:44:33.000000 python_tgpt-0.6.6/src/pytgpt/llama2/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:45:06.293255 python_tgpt-0.6.6/src/pytgpt/openai/
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-24 16:44:33.000000 python_tgpt-0.6.6/src/pytgpt/openai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9597 2024-04-24 16:44:33.000000 python_tgpt-0.6.6/src/pytgpt/openai/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:45:06.293255 python_tgpt-0.6.6/src/pytgpt/opengpt/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-24 16:44:33.000000 python_tgpt-0.6.6/src/pytgpt/opengpt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8709 2024-04-24 16:44:33.000000 python_tgpt-0.6.6/src/pytgpt/opengpt/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:45:06.293255 python_tgpt-0.6.6/src/pytgpt/perplexity/
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-24 16:44:33.000000 python_tgpt-0.6.6/src/pytgpt/perplexity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7907 2024-04-24 16:44:33.000000 python_tgpt-0.6.6/src/pytgpt/perplexity/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:45:06.293255 python_tgpt-0.6.6/src/pytgpt/phind/
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-24 16:44:33.000000 python_tgpt-0.6.6/src/pytgpt/phind/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9139 2024-04-24 16:44:33.000000 python_tgpt-0.6.6/src/pytgpt/phind/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:45:06.293255 python_tgpt-0.6.6/src/pytgpt/poe/
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-24 16:44:33.000000 python_tgpt-0.6.6/src/pytgpt/poe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7455 2024-04-24 16:44:33.000000 python_tgpt-0.6.6/src/pytgpt/poe/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33863 2024-04-24 16:44:33.000000 python_tgpt-0.6.6/src/pytgpt/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:45:06.297255 python_tgpt-0.6.6/src/pytgpt/webchatgpt/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-24 16:44:33.000000 python_tgpt-0.6.6/src/pytgpt/webchatgpt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7114 2024-04-24 16:44:33.000000 python_tgpt-0.6.6/src/pytgpt/webchatgpt/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:45:06.297255 python_tgpt-0.6.6/src/pytgpt/yepchat/
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-24 16:44:33.000000 python_tgpt-0.6.6/src/pytgpt/yepchat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9434 2024-04-24 16:44:33.000000 python_tgpt-0.6.6/src/pytgpt/yepchat/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:45:06.301255 python_tgpt-0.6.6/src/python_tgpt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    21914 2024-04-24 16:45:06.000000 python_tgpt-0.6.6/src/python_tgpt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-04-24 16:45:06.000000 python_tgpt-0.6.6/src/python_tgpt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 16:45:06.000000 python_tgpt-0.6.6/src/python_tgpt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-24 16:45:06.000000 python_tgpt-0.6.6/src/python_tgpt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-24 16:45:06.000000 python_tgpt-0.6.6/src/python_tgpt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-24 16:45:06.000000 python_tgpt-0.6.6/src/python_tgpt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:45:06.301255 python_tgpt-0.6.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3342 2024-04-24 16:44:33.000000 python_tgpt-0.6.6/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-24 16:44:33.000000 python_tgpt-0.6.6/tests/test_auto.py
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-24 16:44:33.000000 python_tgpt-0.6.6/tests/test_blackboxai.py
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-24 16:44:33.000000 python_tgpt-0.6.6/tests/test_gemini.py
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-24 16:44:33.000000 python_tgpt-0.6.6/tests/test_gpt4all.py
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-24 16:44:33.000000 python_tgpt-0.6.6/tests/test_gpt4free.py
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-24 16:44:33.000000 python_tgpt-0.6.6/tests/test_groq.py
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-24 16:44:33.000000 python_tgpt-0.6.6/tests/test_imager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-24 16:44:33.000000 python_tgpt-0.6.6/tests/test_koboldai.py
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-24 16:44:33.000000 python_tgpt-0.6.6/tests/test_leo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-24 16:44:33.000000 python_tgpt-0.6.6/tests/test_llama2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-24 16:44:33.000000 python_tgpt-0.6.6/tests/test_openai.py
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-24 16:44:33.000000 python_tgpt-0.6.6/tests/test_opengpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-24 16:44:33.000000 python_tgpt-0.6.6/tests/test_perplexity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-24 16:44:33.000000 python_tgpt-0.6.6/tests/test_phind.py
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-24 16:44:33.000000 python_tgpt-0.6.6/tests/test_poe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4202 2024-04-24 16:44:33.000000 python_tgpt-0.6.6/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-24 16:44:33.000000 python_tgpt-0.6.6/tests/test_webchatgpt.py
```

### Comparing `python_tgpt-0.6.5/LICENSE` & `python_tgpt-0.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.6.5/PKG-INFO` & `python_tgpt-0.6.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-tgpt
-Version: 0.6.5
+Version: 0.6.6
 Summary: Interact with AI without API key
 Home-page: https://github.com/Simatwa/python-tgpt
 Author: Smartwa
 Author-email: simatwacaleb@proton.me
 Maintainer: Smartwa
 License: MIT
 Project-URL: Bug Report, https://github.com/Simatwa/python-tgpt/issues/new
@@ -113,32 +113,33 @@
 img.save(generated_images)
 ```
 
 This project enables seamless interaction with over **45 free LLM providers** without requiring an API Key and generating images as well.
 
 The name *python-tgpt* draws inspiration from its parent project [tgpt](https://github.com/aandrew-me/tgpt), which operates on [Golang](https://go.dev/). Through this Python adaptation, users can effortlessly engage with a number of free LLMs available, fostering a smoother AI interaction experience.
 
-
 ### Features
 
 - 🐍 Python package
 - [🌐 FastAPI for web integration](https://python-tgpt.onrender.com)
 - ⌨️ Command-line interface
 - 🧠 Multiple LLM providers - **45+**
 - 🌊 Stream and non-stream response
 - 🚀 Ready to use (No API key required)
 - 🎯 Customizable script generation and execution
 - 🔌 Offline support for Large Language Models
 - 🎨 Image generation capabilities
+- 🎤 Text-to-audio conversion capabilities
 - ⛓️ Chained requests via proxy
 - 🗨️ Enhanced conversational chat experience
 - 💾 Capability to save prompts and responses (Conversation)
 - 🔄 Ability to load previous conversations
 - 🤖 Pass [awesome-chatgpt prompts](https://github.com/f/awesome-chatgpt-prompts) easily
 
+
 ## Providers
 
 These are simply the hosts of the LLMs, which include:
 
 1. [Leo](https://brave.com/leo/) - **Brave**
 2. [Koboldai](https://koboldai-koboldcpp-tiefighter.hf.space)
 3. [OpenGPTs](https://opengpts-example-vz4y4ooboq-uc.a.run.app/)
@@ -406,14 +407,16 @@
 bot = LEO()
 resp = bot.ask('<Your Prompt>', optimizer='code')
 print(resp)
 ```
 
 </details>
 
+</details>
+
 > [!IMPORTANT]
 > Commencing from [v0.1.0](https://github.com/Simatwa/python-tgpt/releases/), the default mode of interaction is conversational. This mode enhances the interactive experience, offering better control over the chat history. By associating previous prompts and responses, it tailors conversations for a more engaging experience.
 
 You can still disable the mode:
 
 ```python
 bot = koboldai.KOBOLDAI(is_conversation=False)
@@ -587,19 +590,20 @@
 ```
 or
 ```bash
 $ pytgpt interactive -ttm
 ```
 This flag instructs the system to audiolize the ai responses and then play them, enhancing the user experience by providing auditory feedback.
 
-> To speech synthesise the responses just ensure you have [vlc player]() in your system or [termux-api](https://wiki.termux.com/wiki/Termux:API) for the case of [Termux](https://termux.org) users.
-> Use the flag `--talk-to-me`, shortform `-ttm`.
-
 Version **0.6.4** introduces another dynamic provider, `auto`, which denotes the working provider **overall**. This relieves you of the workload of manually checking a working provider each time you fire up pytgpt.
 
+## [Telegram Bot](https://github.com/Simatwa/pytgpt-bot)
+
+If you're not satisfied with the existing interfaces, [pytgpt-bot](https://github.com/Simatwa/pytgpt-bot) could be the solution you're seeking. This bot is designed to enhance your experience by offering a wide range of functionalities. Whether you're interested in engaging in AI-driven conversations, creating images and audio from text, or exploring other innovative features, [pytgpt-bot is equipped to meet your needs.](https://github.com/Simatwa/pytgpt-bot)
+
 <details>
 
 <summary>
 
 For more usage info run `$ pytgpt --help`
 
 </summary>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: python-tgpt Version: 0.6.5 Summary: Interact with
+Metadata-Version: 2.1 Name: python-tgpt Version: 0.6.6 Summary: Interact with
 AI without API key Home-page: https://github.com/Simatwa/python-tgpt Author:
 Smartwa Author-email: simatwacaleb@proton.me Maintainer: Smartwa License: MIT
 Project-URL: Bug Report, https://github.com/Simatwa/python-tgpt/issues/new
 Project-URL: Homepage, https://github.com/Simatwa/python-tgpt Project-URL:
 Source Code, https://github.com/Simatwa/python-tgpt Project-URL: Issue Tracker,
 https://github.com/Simatwa/python-tgpt/issues Project-URL: Download, https://
 github.com/Simatwa/python-tgpt/releases Project-URL: Documentation, https://
@@ -56,52 +56,52 @@
 Python adaptation, users can effortlessly engage with a number of free LLMs
 available, fostering a smoother AI interaction experience. ### Features - ð
 Python package - [ð FastAPI for web integration](https://python-
 tgpt.onrender.com) - â¨ï¸ Command-line interface - ð§  Multiple LLM
 providers - **45+** - ð Stream and non-stream response - ð Ready to use
 (No API key required) - ð¯ Customizable script generation and execution -
 ð Offline support for Large Language Models - ð¨ Image generation
-capabilities - âï¸ Chained requests via proxy - ð¨ï¸ Enhanced
-conversational chat experience - ð¾ Capability to save prompts and responses
-(Conversation) - ð Ability to load previous conversations - ð¤ Pass
-[awesome-chatgpt prompts](https://github.com/f/awesome-chatgpt-prompts) easily
-## Providers These are simply the hosts of the LLMs, which include: 1. [Leo]
-(https://brave.com/leo/) - **Brave** 2. [Koboldai](https://koboldai-koboldcpp-
-tiefighter.hf.space) 3. [OpenGPTs](https://opengpts-example-vz4y4ooboq-
-uc.a.run.app/) 4. [OpenAI](https://chat.openai.com) *(API key required)* 5.
-[WebChatGPT](https://github.com/Simatwa/WebChatGPT) - **OpenAI** *(Session ID
-required)* 6. [Gemini](https://github.com/Simatwa/bard) - **Google** *(Session
-ID required)* 9. [Phind](https://www.phind.com) 10. [Llama2](https://
-www.llama2.ai) 11. [Blackboxai](https://www.blackbox.ai) 12. [gpt4all](https://
-gpt4all.io) *(Offline)* 13. [Poe](https://poe.com) - Poe|Quora *(Session ID
-required)* 14. [Groq](https://console.groq.com/playground) *(API Key required)*
-15. [Perplexity](https://www.perplexity.ai) 16. [YepChat](https://yep.com) 41+
-providers proudly offered by [gpt4free](https://github.com/xtekky/gpt4free). -
-To list working providers run: ```sh $ pytgpt gpt4free test -y ``` ##
-Prerequisites - [x] [Python>=3.10](https://python.org) *(Optional)* ##
-Installation and Usage ### Installation Download binaries for your system from
-[here.](https://github.com/Simatwa/python-tgpt/releases/latest/) Alternatively,
-you can install non-binaries. *(Recommended)* 1. Developers: ```sh pip install
---upgrade python-tgpt ``` 2. Commandline: ```sh pip install --upgrade "python-
-tgpt[cli]" ``` 3. Full installation: ```sh pip install --upgrade "python-tgpt
-[all]" ``` > `pip install -U "python-tgt[api]"` will install REST API
-dependencies. ## Usage This package offers a convenient command-line interface.
-> [!NOTE] > `phind` is the default *provider*. - For a quick response: ```bash
-python -m pytgpt generate "" ``` - For interactive mode: ```bash python -
-m pytgpt interactive "" ``` Make use of flag `--provider` followed by the
-provider name of your choice. e.g `--provider koboldai` > To list all providers
-offered by gpt4free, use following commands: ```pytgpt gpt4free list
-providers``` You can also simply use `pytgpt` instead of `python -m pytgpt`.
-Starting from version 0.2.7, running `$ pytgpt` without any other command or
-option will automatically enter the `interactive` mode. Otherwise, you'll need
-to explicitly declare the desired action, for example, by running `$ pytgpt
-generate`. ### Developer Docs 1. Generate a quick response ```python from
-pytgpt.leo import LEO bot = LEO() resp = bot.chat('') print(resp) # Output :
-How may I help you. ``` 2. Get back whole response ```python from pytgpt.leo
-import LEO bot = LEO() resp = bot.ask('
+capabilities - ð¤ Text-to-audio conversion capabilities - âï¸ Chained
+requests via proxy - ð¨ï¸ Enhanced conversational chat experience - ð¾
+Capability to save prompts and responses (Conversation) - ð Ability to load
+previous conversations - ð¤ Pass [awesome-chatgpt prompts](https://
+github.com/f/awesome-chatgpt-prompts) easily ## Providers These are simply the
+hosts of the LLMs, which include: 1. [Leo](https://brave.com/leo/) - **Brave**
+2. [Koboldai](https://koboldai-koboldcpp-tiefighter.hf.space) 3. [OpenGPTs]
+(https://opengpts-example-vz4y4ooboq-uc.a.run.app/) 4. [OpenAI](https://
+chat.openai.com) *(API key required)* 5. [WebChatGPT](https://github.com/
+Simatwa/WebChatGPT) - **OpenAI** *(Session ID required)* 6. [Gemini](https://
+github.com/Simatwa/bard) - **Google** *(Session ID required)* 9. [Phind](https:
+//www.phind.com) 10. [Llama2](https://www.llama2.ai) 11. [Blackboxai](https://
+www.blackbox.ai) 12. [gpt4all](https://gpt4all.io) *(Offline)* 13. [Poe](https:
+//poe.com) - Poe|Quora *(Session ID required)* 14. [Groq](https://
+console.groq.com/playground) *(API Key required)* 15. [Perplexity](https://
+www.perplexity.ai) 16. [YepChat](https://yep.com) 41+ providers proudly offered
+by [gpt4free](https://github.com/xtekky/gpt4free). - To list working providers
+run: ```sh $ pytgpt gpt4free test -y ``` ## Prerequisites - [x] [Python>=3.10]
+(https://python.org) *(Optional)* ## Installation and Usage ### Installation
+Download binaries for your system from [here.](https://github.com/Simatwa/
+python-tgpt/releases/latest/) Alternatively, you can install non-binaries. *
+(Recommended)* 1. Developers: ```sh pip install --upgrade python-tgpt ``` 2.
+Commandline: ```sh pip install --upgrade "python-tgpt[cli]" ``` 3. Full
+installation: ```sh pip install --upgrade "python-tgpt[all]" ``` > `pip install
+-U "python-tgt[api]"` will install REST API dependencies. ## Usage This package
+offers a convenient command-line interface. > [!NOTE] > `phind` is the default
+*provider*. - For a quick response: ```bash python -m pytgpt generate "" ``` -
+For interactive mode: ```bash python -m pytgpt interactive "" ``` Make use of
+flag `--provider` followed by the provider name of your choice. e.g `--provider
+koboldai` > To list all providers offered by gpt4free, use following commands:
+```pytgpt gpt4free list providers``` You can also simply use `pytgpt` instead
+of `python -m pytgpt`. Starting from version 0.2.7, running `$ pytgpt` without
+any other command or option will automatically enter the `interactive` mode.
+Otherwise, you'll need to explicitly declare the desired action, for example,
+by running `$ pytgpt generate`. ### Developer Docs 1. Generate a quick response
+```python from pytgpt.leo import LEO bot = LEO() resp = bot.chat('') print
+(resp) # Output : How may I help you. ``` 2. Get back whole response ```python
+from pytgpt.leo import LEO bot = LEO() resp = bot.ask('
  Output """ {'completion': "I'm so excited to share with you the incredible
 experiences...", 'stop_reason': None, 'truncated': False, 'stop': None,
 'model': 'llama-2-13b-chat', 'log_id': 'cmpl-3NmRt5A5Djqo2jXtXLBwJ2',
 'exception': None} """ ``` #### Stream Response Just add parameter `stream`
 with value `true`. 1. Text Generated only ```python from pytgpt.leo import LEO
 bot = LEO() resp = bot.chat('', stream=True) for value in resp: print(value) #
 output """ How may How may I help How may I help you How may I help you today?
@@ -216,26 +216,30 @@
 www.videolan.org/vlc/index.html) installed on your system or, if you are a
 [Termux](https://termux.org) user, the [Termux:API](https://wiki.termux.com/
 wiki/Termux:API) package. To activate speech synthesis, use the `--talk-to-me`
 flag or its shorthand `-ttm` when running your commands. For example: ```bash $
 pytgpt generate "Generate an ogre story" --talk-to-me ``` or ```bash $ pytgpt
 interactive -ttm ``` This flag instructs the system to audiolize the ai
 responses and then play them, enhancing the user experience by providing
-auditory feedback. > To speech synthesise the responses just ensure you have
-[vlc player]() in your system or [termux-api](https://wiki.termux.com/wiki/
-Termux:API) for the case of [Termux](https://termux.org) users. > Use the flag
-`--talk-to-me`, shortform `-ttm`. Version **0.6.4** introduces another dynamic
-provider, `auto`, which denotes the working provider **overall**. This relieves
-you of the workload of manually checking a working provider each time you fire
-up pytgpt. For more usage info run `$ pytgpt --help` ``` Usage: pytgpt
-[OPTIONS] COMMAND [ARGS]... Options: -v, --version Show the version and exit. -
-h, --help Show this message and exit. Commands: api FastAPI control endpoint
-awesome Perform CRUD operations on awesome-prompts generate Generate a quick
-response with AI gpt4free Discover gpt4free models, providers etc imager
-Generate images with pollinations.ai interactive Chat with AI interactively
-(Default) utils Utility endpoint for pytgpt webchatgpt Reverse Engineered
-ChatGPT Web-Version ``` ### API Health Status | No. | API | Status | |--------
-|-----|--------| | 1. | [On-render](https://python-tgpt.onrender.com) | [cron-
-job](https://pqfzhmvz.status.cron-job.org/) | ## [CHANGELOG](https://
-github.com/Simatwa/python-tgpt/blob/main/docs/CHANGELOG.md) ## Acknowledgements
-1. [x] [tgpt](https://github.com/aandrew-me/tgpt) 2. [x] [gpt4free](https://
-github.com/xtekky/gpt4free)
+auditory feedback. Version **0.6.4** introduces another dynamic provider,
+`auto`, which denotes the working provider **overall**. This relieves you of
+the workload of manually checking a working provider each time you fire up
+pytgpt. ## [Telegram Bot](https://github.com/Simatwa/pytgpt-bot) If you're not
+satisfied with the existing interfaces, [pytgpt-bot](https://github.com/
+Simatwa/pytgpt-bot) could be the solution you're seeking. This bot is designed
+to enhance your experience by offering a wide range of functionalities. Whether
+you're interested in engaging in AI-driven conversations, creating images and
+audio from text, or exploring other innovative features, [pytgpt-bot is
+equipped to meet your needs.](https://github.com/Simatwa/pytgpt-bot) For more
+usage info run `$ pytgpt --help` ``` Usage: pytgpt [OPTIONS] COMMAND [ARGS]...
+Options: -v, --version Show the version and exit. -h, --help Show this message
+and exit. Commands: api FastAPI control endpoint awesome Perform CRUD
+operations on awesome-prompts generate Generate a quick response with AI
+gpt4free Discover gpt4free models, providers etc imager Generate images with
+pollinations.ai interactive Chat with AI interactively (Default) utils Utility
+endpoint for pytgpt webchatgpt Reverse Engineered ChatGPT Web-Version ``` ###
+API Health Status | No. | API | Status | |--------|-----|--------| | 1. | [On-
+render](https://python-tgpt.onrender.com) | [cron-job](https://
+pqfzhmvz.status.cron-job.org/) | ## [CHANGELOG](https://github.com/Simatwa/
+python-tgpt/blob/main/docs/CHANGELOG.md) ## Acknowledgements 1. [x] [tgpt]
+(https://github.com/aandrew-me/tgpt) 2. [x] [gpt4free](https://github.com/
+xtekky/gpt4free)
```

### Comparing `python_tgpt-0.6.5/README.md` & `python_tgpt-0.6.6/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -47,32 +47,33 @@
 img.save(generated_images)
 ```
 
 This project enables seamless interaction with over **45 free LLM providers** without requiring an API Key and generating images as well.
 
 The name *python-tgpt* draws inspiration from its parent project [tgpt](https://github.com/aandrew-me/tgpt), which operates on [Golang](https://go.dev/). Through this Python adaptation, users can effortlessly engage with a number of free LLMs available, fostering a smoother AI interaction experience.
 
-
 ### Features
 
 - 🐍 Python package
 - [🌐 FastAPI for web integration](https://python-tgpt.onrender.com)
 - ⌨️ Command-line interface
 - 🧠 Multiple LLM providers - **45+**
 - 🌊 Stream and non-stream response
 - 🚀 Ready to use (No API key required)
 - 🎯 Customizable script generation and execution
 - 🔌 Offline support for Large Language Models
 - 🎨 Image generation capabilities
+- 🎤 Text-to-audio conversion capabilities
 - ⛓️ Chained requests via proxy
 - 🗨️ Enhanced conversational chat experience
 - 💾 Capability to save prompts and responses (Conversation)
 - 🔄 Ability to load previous conversations
 - 🤖 Pass [awesome-chatgpt prompts](https://github.com/f/awesome-chatgpt-prompts) easily
 
+
 ## Providers
 
 These are simply the hosts of the LLMs, which include:
 
 1. [Leo](https://brave.com/leo/) - **Brave**
 2. [Koboldai](https://koboldai-koboldcpp-tiefighter.hf.space)
 3. [OpenGPTs](https://opengpts-example-vz4y4ooboq-uc.a.run.app/)
@@ -340,14 +341,16 @@
 bot = LEO()
 resp = bot.ask('<Your Prompt>', optimizer='code')
 print(resp)
 ```
 
 </details>
 
+</details>
+
 > [!IMPORTANT]
 > Commencing from [v0.1.0](https://github.com/Simatwa/python-tgpt/releases/), the default mode of interaction is conversational. This mode enhances the interactive experience, offering better control over the chat history. By associating previous prompts and responses, it tailors conversations for a more engaging experience.
 
 You can still disable the mode:
 
 ```python
 bot = koboldai.KOBOLDAI(is_conversation=False)
@@ -521,19 +524,20 @@
 ```
 or
 ```bash
 $ pytgpt interactive -ttm
 ```
 This flag instructs the system to audiolize the ai responses and then play them, enhancing the user experience by providing auditory feedback.
 
-> To speech synthesise the responses just ensure you have [vlc player]() in your system or [termux-api](https://wiki.termux.com/wiki/Termux:API) for the case of [Termux](https://termux.org) users.
-> Use the flag `--talk-to-me`, shortform `-ttm`.
-
 Version **0.6.4** introduces another dynamic provider, `auto`, which denotes the working provider **overall**. This relieves you of the workload of manually checking a working provider each time you fire up pytgpt.
 
+## [Telegram Bot](https://github.com/Simatwa/pytgpt-bot)
+
+If you're not satisfied with the existing interfaces, [pytgpt-bot](https://github.com/Simatwa/pytgpt-bot) could be the solution you're seeking. This bot is designed to enhance your experience by offering a wide range of functionalities. Whether you're interested in engaging in AI-driven conversations, creating images and audio from text, or exploring other innovative features, [pytgpt-bot is equipped to meet your needs.](https://github.com/Simatwa/pytgpt-bot)
+
 <details>
 
 <summary>
 
 For more usage info run `$ pytgpt --help`
 
 </summary>
```

#### html2text {}

```diff
@@ -16,52 +16,52 @@
 Python adaptation, users can effortlessly engage with a number of free LLMs
 available, fostering a smoother AI interaction experience. ### Features - ð
 Python package - [ð FastAPI for web integration](https://python-
 tgpt.onrender.com) - â¨ï¸ Command-line interface - ð§  Multiple LLM
 providers - **45+** - ð Stream and non-stream response - ð Ready to use
 (No API key required) - ð¯ Customizable script generation and execution -
 ð Offline support for Large Language Models - ð¨ Image generation
-capabilities - âï¸ Chained requests via proxy - ð¨ï¸ Enhanced
-conversational chat experience - ð¾ Capability to save prompts and responses
-(Conversation) - ð Ability to load previous conversations - ð¤ Pass
-[awesome-chatgpt prompts](https://github.com/f/awesome-chatgpt-prompts) easily
-## Providers These are simply the hosts of the LLMs, which include: 1. [Leo]
-(https://brave.com/leo/) - **Brave** 2. [Koboldai](https://koboldai-koboldcpp-
-tiefighter.hf.space) 3. [OpenGPTs](https://opengpts-example-vz4y4ooboq-
-uc.a.run.app/) 4. [OpenAI](https://chat.openai.com) *(API key required)* 5.
-[WebChatGPT](https://github.com/Simatwa/WebChatGPT) - **OpenAI** *(Session ID
-required)* 6. [Gemini](https://github.com/Simatwa/bard) - **Google** *(Session
-ID required)* 9. [Phind](https://www.phind.com) 10. [Llama2](https://
-www.llama2.ai) 11. [Blackboxai](https://www.blackbox.ai) 12. [gpt4all](https://
-gpt4all.io) *(Offline)* 13. [Poe](https://poe.com) - Poe|Quora *(Session ID
-required)* 14. [Groq](https://console.groq.com/playground) *(API Key required)*
-15. [Perplexity](https://www.perplexity.ai) 16. [YepChat](https://yep.com) 41+
-providers proudly offered by [gpt4free](https://github.com/xtekky/gpt4free). -
-To list working providers run: ```sh $ pytgpt gpt4free test -y ``` ##
-Prerequisites - [x] [Python>=3.10](https://python.org) *(Optional)* ##
-Installation and Usage ### Installation Download binaries for your system from
-[here.](https://github.com/Simatwa/python-tgpt/releases/latest/) Alternatively,
-you can install non-binaries. *(Recommended)* 1. Developers: ```sh pip install
---upgrade python-tgpt ``` 2. Commandline: ```sh pip install --upgrade "python-
-tgpt[cli]" ``` 3. Full installation: ```sh pip install --upgrade "python-tgpt
-[all]" ``` > `pip install -U "python-tgt[api]"` will install REST API
-dependencies. ## Usage This package offers a convenient command-line interface.
-> [!NOTE] > `phind` is the default *provider*. - For a quick response: ```bash
-python -m pytgpt generate "" ``` - For interactive mode: ```bash python -
-m pytgpt interactive "" ``` Make use of flag `--provider` followed by the
-provider name of your choice. e.g `--provider koboldai` > To list all providers
-offered by gpt4free, use following commands: ```pytgpt gpt4free list
-providers``` You can also simply use `pytgpt` instead of `python -m pytgpt`.
-Starting from version 0.2.7, running `$ pytgpt` without any other command or
-option will automatically enter the `interactive` mode. Otherwise, you'll need
-to explicitly declare the desired action, for example, by running `$ pytgpt
-generate`. ### Developer Docs 1. Generate a quick response ```python from
-pytgpt.leo import LEO bot = LEO() resp = bot.chat('') print(resp) # Output :
-How may I help you. ``` 2. Get back whole response ```python from pytgpt.leo
-import LEO bot = LEO() resp = bot.ask('
+capabilities - ð¤ Text-to-audio conversion capabilities - âï¸ Chained
+requests via proxy - ð¨ï¸ Enhanced conversational chat experience - ð¾
+Capability to save prompts and responses (Conversation) - ð Ability to load
+previous conversations - ð¤ Pass [awesome-chatgpt prompts](https://
+github.com/f/awesome-chatgpt-prompts) easily ## Providers These are simply the
+hosts of the LLMs, which include: 1. [Leo](https://brave.com/leo/) - **Brave**
+2. [Koboldai](https://koboldai-koboldcpp-tiefighter.hf.space) 3. [OpenGPTs]
+(https://opengpts-example-vz4y4ooboq-uc.a.run.app/) 4. [OpenAI](https://
+chat.openai.com) *(API key required)* 5. [WebChatGPT](https://github.com/
+Simatwa/WebChatGPT) - **OpenAI** *(Session ID required)* 6. [Gemini](https://
+github.com/Simatwa/bard) - **Google** *(Session ID required)* 9. [Phind](https:
+//www.phind.com) 10. [Llama2](https://www.llama2.ai) 11. [Blackboxai](https://
+www.blackbox.ai) 12. [gpt4all](https://gpt4all.io) *(Offline)* 13. [Poe](https:
+//poe.com) - Poe|Quora *(Session ID required)* 14. [Groq](https://
+console.groq.com/playground) *(API Key required)* 15. [Perplexity](https://
+www.perplexity.ai) 16. [YepChat](https://yep.com) 41+ providers proudly offered
+by [gpt4free](https://github.com/xtekky/gpt4free). - To list working providers
+run: ```sh $ pytgpt gpt4free test -y ``` ## Prerequisites - [x] [Python>=3.10]
+(https://python.org) *(Optional)* ## Installation and Usage ### Installation
+Download binaries for your system from [here.](https://github.com/Simatwa/
+python-tgpt/releases/latest/) Alternatively, you can install non-binaries. *
+(Recommended)* 1. Developers: ```sh pip install --upgrade python-tgpt ``` 2.
+Commandline: ```sh pip install --upgrade "python-tgpt[cli]" ``` 3. Full
+installation: ```sh pip install --upgrade "python-tgpt[all]" ``` > `pip install
+-U "python-tgt[api]"` will install REST API dependencies. ## Usage This package
+offers a convenient command-line interface. > [!NOTE] > `phind` is the default
+*provider*. - For a quick response: ```bash python -m pytgpt generate "" ``` -
+For interactive mode: ```bash python -m pytgpt interactive "" ``` Make use of
+flag `--provider` followed by the provider name of your choice. e.g `--provider
+koboldai` > To list all providers offered by gpt4free, use following commands:
+```pytgpt gpt4free list providers``` You can also simply use `pytgpt` instead
+of `python -m pytgpt`. Starting from version 0.2.7, running `$ pytgpt` without
+any other command or option will automatically enter the `interactive` mode.
+Otherwise, you'll need to explicitly declare the desired action, for example,
+by running `$ pytgpt generate`. ### Developer Docs 1. Generate a quick response
+```python from pytgpt.leo import LEO bot = LEO() resp = bot.chat('') print
+(resp) # Output : How may I help you. ``` 2. Get back whole response ```python
+from pytgpt.leo import LEO bot = LEO() resp = bot.ask('
  Output """ {'completion': "I'm so excited to share with you the incredible
 experiences...", 'stop_reason': None, 'truncated': False, 'stop': None,
 'model': 'llama-2-13b-chat', 'log_id': 'cmpl-3NmRt5A5Djqo2jXtXLBwJ2',
 'exception': None} """ ``` #### Stream Response Just add parameter `stream`
 with value `true`. 1. Text Generated only ```python from pytgpt.leo import LEO
 bot = LEO() resp = bot.chat('', stream=True) for value in resp: print(value) #
 output """ How may How may I help How may I help you How may I help you today?
@@ -176,26 +176,30 @@
 www.videolan.org/vlc/index.html) installed on your system or, if you are a
 [Termux](https://termux.org) user, the [Termux:API](https://wiki.termux.com/
 wiki/Termux:API) package. To activate speech synthesis, use the `--talk-to-me`
 flag or its shorthand `-ttm` when running your commands. For example: ```bash $
 pytgpt generate "Generate an ogre story" --talk-to-me ``` or ```bash $ pytgpt
 interactive -ttm ``` This flag instructs the system to audiolize the ai
 responses and then play them, enhancing the user experience by providing
-auditory feedback. > To speech synthesise the responses just ensure you have
-[vlc player]() in your system or [termux-api](https://wiki.termux.com/wiki/
-Termux:API) for the case of [Termux](https://termux.org) users. > Use the flag
-`--talk-to-me`, shortform `-ttm`. Version **0.6.4** introduces another dynamic
-provider, `auto`, which denotes the working provider **overall**. This relieves
-you of the workload of manually checking a working provider each time you fire
-up pytgpt. For more usage info run `$ pytgpt --help` ``` Usage: pytgpt
-[OPTIONS] COMMAND [ARGS]... Options: -v, --version Show the version and exit. -
-h, --help Show this message and exit. Commands: api FastAPI control endpoint
-awesome Perform CRUD operations on awesome-prompts generate Generate a quick
-response with AI gpt4free Discover gpt4free models, providers etc imager
-Generate images with pollinations.ai interactive Chat with AI interactively
-(Default) utils Utility endpoint for pytgpt webchatgpt Reverse Engineered
-ChatGPT Web-Version ``` ### API Health Status | No. | API | Status | |--------
-|-----|--------| | 1. | [On-render](https://python-tgpt.onrender.com) | [cron-
-job](https://pqfzhmvz.status.cron-job.org/) | ## [CHANGELOG](https://
-github.com/Simatwa/python-tgpt/blob/main/docs/CHANGELOG.md) ## Acknowledgements
-1. [x] [tgpt](https://github.com/aandrew-me/tgpt) 2. [x] [gpt4free](https://
-github.com/xtekky/gpt4free)
+auditory feedback. Version **0.6.4** introduces another dynamic provider,
+`auto`, which denotes the working provider **overall**. This relieves you of
+the workload of manually checking a working provider each time you fire up
+pytgpt. ## [Telegram Bot](https://github.com/Simatwa/pytgpt-bot) If you're not
+satisfied with the existing interfaces, [pytgpt-bot](https://github.com/
+Simatwa/pytgpt-bot) could be the solution you're seeking. This bot is designed
+to enhance your experience by offering a wide range of functionalities. Whether
+you're interested in engaging in AI-driven conversations, creating images and
+audio from text, or exploring other innovative features, [pytgpt-bot is
+equipped to meet your needs.](https://github.com/Simatwa/pytgpt-bot) For more
+usage info run `$ pytgpt --help` ``` Usage: pytgpt [OPTIONS] COMMAND [ARGS]...
+Options: -v, --version Show the version and exit. -h, --help Show this message
+and exit. Commands: api FastAPI control endpoint awesome Perform CRUD
+operations on awesome-prompts generate Generate a quick response with AI
+gpt4free Discover gpt4free models, providers etc imager Generate images with
+pollinations.ai interactive Chat with AI interactively (Default) utils Utility
+endpoint for pytgpt webchatgpt Reverse Engineered ChatGPT Web-Version ``` ###
+API Health Status | No. | API | Status | |--------|-----|--------| | 1. | [On-
+render](https://python-tgpt.onrender.com) | [cron-job](https://
+pqfzhmvz.status.cron-job.org/) | ## [CHANGELOG](https://github.com/Simatwa/
+python-tgpt/blob/main/docs/CHANGELOG.md) ## Acknowledgements 1. [x] [tgpt]
+(https://github.com/aandrew-me/tgpt) 2. [x] [gpt4free](https://github.com/
+xtekky/gpt4free)
```

### Comparing `python_tgpt-0.6.5/setup.py` & `python_tgpt-0.6.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 if not PATH.exists():
     with Path.open(DOCS_PATH, encoding="utf-8") as f1:
         with Path.open(PATH, "w+", encoding="utf-8") as f2:
             f2.write(f1.read())
 
 setup(
     name="python-tgpt",
-    version="0.6.5",
+    version="0.6.6",
     license="MIT",
     author="Smartwa",
     maintainer="Smartwa",
     author_email="simatwacaleb@proton.me",
     description="Interact with AI without API key",
     packages=find_packages("src"),
     package_dir={"": "src"},
```

### Comparing `python_tgpt-0.6.5/src/pytgpt/__init__.py` & `python_tgpt-0.6.6/src/pytgpt/__init__.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.6.5/src/pytgpt/api/__init__.py` & `python_tgpt-0.6.6/src/pytgpt/api/__init__.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.6.5/src/pytgpt/api/utils.py` & `python_tgpt-0.6.6/src/pytgpt/api/utils.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.6.5/src/pytgpt/api/v1.py` & `python_tgpt-0.6.6/src/pytgpt/api/v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -295,15 +295,15 @@
     """
 
     url: str
 
     model_config = {
         "json_schema_extra": {
             "example": {
-                "url": " http://localhost:8000/static/audios/f9d4233f-9b78-4d87-bc27-5d2ab928f673.mp3",
+                "url": "http://localhost:8000/static/audios/f9d4233f-9b78-4d87-bc27-5d2ab928f673.mp3",
             }
         }
     }
 
 
 def init_provider(payload: TextGenerationPayload) -> object:
     return provider_map.get(payload.provider, GPT4FREE)(
```

### Comparing `python_tgpt-0.6.5/src/pytgpt/auto/main.py` & `python_tgpt-0.6.6/src/pytgpt/auto/main.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.6.5/src/pytgpt/base.py` & `python_tgpt-0.6.6/src/pytgpt/base.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.6.5/src/pytgpt/blackboxai/main.py` & `python_tgpt-0.6.6/src/pytgpt/blackboxai/main.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.6.5/src/pytgpt/console.py` & `python_tgpt-0.6.6/src/pytgpt/console.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.6.5/src/pytgpt/gemini/main.py` & `python_tgpt-0.6.6/src/pytgpt/gemini/main.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.6.5/src/pytgpt/gpt4all/main.py` & `python_tgpt-0.6.6/src/pytgpt/gpt4all/main.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.6.5/src/pytgpt/gpt4free/main.py` & `python_tgpt-0.6.6/src/pytgpt/gpt4free/main.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.6.5/src/pytgpt/gpt4free/utils.py` & `python_tgpt-0.6.6/src/pytgpt/gpt4free/utils.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.6.5/src/pytgpt/groq/main.py` & `python_tgpt-0.6.6/src/pytgpt/groq/main.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.6.5/src/pytgpt/imager/imager.py` & `python_tgpt-0.6.6/src/pytgpt/imager/imager.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.6.5/src/pytgpt/koboldai/main.py` & `python_tgpt-0.6.6/src/pytgpt/koboldai/main.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.6.5/src/pytgpt/leo/main.py` & `python_tgpt-0.6.6/src/pytgpt/leo/main.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.6.5/src/pytgpt/llama2/main.py` & `python_tgpt-0.6.6/src/pytgpt/llama2/main.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.6.5/src/pytgpt/openai/main.py` & `python_tgpt-0.6.6/src/pytgpt/openai/main.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.6.5/src/pytgpt/opengpt/main.py` & `python_tgpt-0.6.6/src/pytgpt/opengpt/main.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.6.5/src/pytgpt/perplexity/main.py` & `python_tgpt-0.6.6/src/pytgpt/perplexity/main.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.6.5/src/pytgpt/phind/main.py` & `python_tgpt-0.6.6/src/pytgpt/phind/main.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.6.5/src/pytgpt/poe/main.py` & `python_tgpt-0.6.6/src/pytgpt/poe/main.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.6.5/src/pytgpt/utils.py` & `python_tgpt-0.6.6/src/pytgpt/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 import datetime
 import re
 import sys
 import click
 from rich.markdown import Markdown
 from rich.console import Console
 from pathlib import Path
-import os
 from typing import Union
 from typing import NoReturn
 import requests
 import vlc
 from time import sleep as wait
 
 appdir = appdirs.AppDirs("pytgpt", "Smartwa")
@@ -182,43 +181,45 @@
         else:
             logging.debug(f"Loading conversation from '{filepath}'")
             with open(filepath) as fh:
                 file_contents = fh.read()
                 # Presume intro prompt is part of the file content
                 self.chat_history = file_contents
 
-    def __trim_chat_history(self, chat_history: str) -> str:
+    def __trim_chat_history(self, chat_history: str, intro: str = None) -> str:
         """Ensures the len(prompt) and max_tokens_to_sample is not > 4096"""
-        len_of_intro = len(self.intro)
+        intro = self.intro if intro is None else intro
+        len_of_intro = len(intro)
         len_of_chat_history = len(chat_history)
         total = (
             self.max_tokens_to_sample + len_of_intro + len_of_chat_history
         )  # + self.max_tokens_to_sample
         if total > self.history_offset:
             truncate_at = (total - self.history_offset) + self.prompt_allowance
             # Remove head of total (n) of chat_history
             new_chat_history = chat_history[truncate_at:]
-            self.chat_history = self.intro + "\n... " + new_chat_history
+            self.chat_history = intro + "\n... " + new_chat_history
             # print(len(self.chat_history))
             return self.chat_history
         # print(len(chat_history))
         return chat_history
 
-    def gen_complete_prompt(self, prompt: str) -> str:
+    def gen_complete_prompt(self, prompt: str, intro: str = None) -> str:
         """Generates a kinda like incomplete conversation
 
         Args:
-            prompt (str): _description_
+            prompt (str): Chat prompt
+            intro (str): Override class' intro. Defaults to None.
 
         Returns:
             str: Updated incomplete chat_history
         """
         if self.status:
             resp = self.chat_history + self.history_format % dict(user=prompt, llm="")
-            return self.__trim_chat_history(resp)
+            return self.__trim_chat_history(resp, intro)
 
         return prompt
 
     def update_chat_history(
         self, prompt: str, response: str, force: bool = False
     ) -> None:
         """Updates chat history
```

### Comparing `python_tgpt-0.6.5/src/pytgpt/webchatgpt/main.py` & `python_tgpt-0.6.6/src/pytgpt/webchatgpt/main.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.6.5/src/pytgpt/yepchat/main.py` & `python_tgpt-0.6.6/src/pytgpt/yepchat/main.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.6.5/src/python_tgpt.egg-info/PKG-INFO` & `python_tgpt-0.6.6/src/python_tgpt.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-tgpt
-Version: 0.6.5
+Version: 0.6.6
 Summary: Interact with AI without API key
 Home-page: https://github.com/Simatwa/python-tgpt
 Author: Smartwa
 Author-email: simatwacaleb@proton.me
 Maintainer: Smartwa
 License: MIT
 Project-URL: Bug Report, https://github.com/Simatwa/python-tgpt/issues/new
@@ -113,32 +113,33 @@
 img.save(generated_images)
 ```
 
 This project enables seamless interaction with over **45 free LLM providers** without requiring an API Key and generating images as well.
 
 The name *python-tgpt* draws inspiration from its parent project [tgpt](https://github.com/aandrew-me/tgpt), which operates on [Golang](https://go.dev/). Through this Python adaptation, users can effortlessly engage with a number of free LLMs available, fostering a smoother AI interaction experience.
 
-
 ### Features
 
 - 🐍 Python package
 - [🌐 FastAPI for web integration](https://python-tgpt.onrender.com)
 - ⌨️ Command-line interface
 - 🧠 Multiple LLM providers - **45+**
 - 🌊 Stream and non-stream response
 - 🚀 Ready to use (No API key required)
 - 🎯 Customizable script generation and execution
 - 🔌 Offline support for Large Language Models
 - 🎨 Image generation capabilities
+- 🎤 Text-to-audio conversion capabilities
 - ⛓️ Chained requests via proxy
 - 🗨️ Enhanced conversational chat experience
 - 💾 Capability to save prompts and responses (Conversation)
 - 🔄 Ability to load previous conversations
 - 🤖 Pass [awesome-chatgpt prompts](https://github.com/f/awesome-chatgpt-prompts) easily
 
+
 ## Providers
 
 These are simply the hosts of the LLMs, which include:
 
 1. [Leo](https://brave.com/leo/) - **Brave**
 2. [Koboldai](https://koboldai-koboldcpp-tiefighter.hf.space)
 3. [OpenGPTs](https://opengpts-example-vz4y4ooboq-uc.a.run.app/)
@@ -406,14 +407,16 @@
 bot = LEO()
 resp = bot.ask('<Your Prompt>', optimizer='code')
 print(resp)
 ```
 
 </details>
 
+</details>
+
 > [!IMPORTANT]
 > Commencing from [v0.1.0](https://github.com/Simatwa/python-tgpt/releases/), the default mode of interaction is conversational. This mode enhances the interactive experience, offering better control over the chat history. By associating previous prompts and responses, it tailors conversations for a more engaging experience.
 
 You can still disable the mode:
 
 ```python
 bot = koboldai.KOBOLDAI(is_conversation=False)
@@ -587,19 +590,20 @@
 ```
 or
 ```bash
 $ pytgpt interactive -ttm
 ```
 This flag instructs the system to audiolize the ai responses and then play them, enhancing the user experience by providing auditory feedback.
 
-> To speech synthesise the responses just ensure you have [vlc player]() in your system or [termux-api](https://wiki.termux.com/wiki/Termux:API) for the case of [Termux](https://termux.org) users.
-> Use the flag `--talk-to-me`, shortform `-ttm`.
-
 Version **0.6.4** introduces another dynamic provider, `auto`, which denotes the working provider **overall**. This relieves you of the workload of manually checking a working provider each time you fire up pytgpt.
 
+## [Telegram Bot](https://github.com/Simatwa/pytgpt-bot)
+
+If you're not satisfied with the existing interfaces, [pytgpt-bot](https://github.com/Simatwa/pytgpt-bot) could be the solution you're seeking. This bot is designed to enhance your experience by offering a wide range of functionalities. Whether you're interested in engaging in AI-driven conversations, creating images and audio from text, or exploring other innovative features, [pytgpt-bot is equipped to meet your needs.](https://github.com/Simatwa/pytgpt-bot)
+
 <details>
 
 <summary>
 
 For more usage info run `$ pytgpt --help`
 
 </summary>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: python-tgpt Version: 0.6.5 Summary: Interact with
+Metadata-Version: 2.1 Name: python-tgpt Version: 0.6.6 Summary: Interact with
 AI without API key Home-page: https://github.com/Simatwa/python-tgpt Author:
 Smartwa Author-email: simatwacaleb@proton.me Maintainer: Smartwa License: MIT
 Project-URL: Bug Report, https://github.com/Simatwa/python-tgpt/issues/new
 Project-URL: Homepage, https://github.com/Simatwa/python-tgpt Project-URL:
 Source Code, https://github.com/Simatwa/python-tgpt Project-URL: Issue Tracker,
 https://github.com/Simatwa/python-tgpt/issues Project-URL: Download, https://
 github.com/Simatwa/python-tgpt/releases Project-URL: Documentation, https://
@@ -56,52 +56,52 @@
 Python adaptation, users can effortlessly engage with a number of free LLMs
 available, fostering a smoother AI interaction experience. ### Features - ð
 Python package - [ð FastAPI for web integration](https://python-
 tgpt.onrender.com) - â¨ï¸ Command-line interface - ð§  Multiple LLM
 providers - **45+** - ð Stream and non-stream response - ð Ready to use
 (No API key required) - ð¯ Customizable script generation and execution -
 ð Offline support for Large Language Models - ð¨ Image generation
-capabilities - âï¸ Chained requests via proxy - ð¨ï¸ Enhanced
-conversational chat experience - ð¾ Capability to save prompts and responses
-(Conversation) - ð Ability to load previous conversations - ð¤ Pass
-[awesome-chatgpt prompts](https://github.com/f/awesome-chatgpt-prompts) easily
-## Providers These are simply the hosts of the LLMs, which include: 1. [Leo]
-(https://brave.com/leo/) - **Brave** 2. [Koboldai](https://koboldai-koboldcpp-
-tiefighter.hf.space) 3. [OpenGPTs](https://opengpts-example-vz4y4ooboq-
-uc.a.run.app/) 4. [OpenAI](https://chat.openai.com) *(API key required)* 5.
-[WebChatGPT](https://github.com/Simatwa/WebChatGPT) - **OpenAI** *(Session ID
-required)* 6. [Gemini](https://github.com/Simatwa/bard) - **Google** *(Session
-ID required)* 9. [Phind](https://www.phind.com) 10. [Llama2](https://
-www.llama2.ai) 11. [Blackboxai](https://www.blackbox.ai) 12. [gpt4all](https://
-gpt4all.io) *(Offline)* 13. [Poe](https://poe.com) - Poe|Quora *(Session ID
-required)* 14. [Groq](https://console.groq.com/playground) *(API Key required)*
-15. [Perplexity](https://www.perplexity.ai) 16. [YepChat](https://yep.com) 41+
-providers proudly offered by [gpt4free](https://github.com/xtekky/gpt4free). -
-To list working providers run: ```sh $ pytgpt gpt4free test -y ``` ##
-Prerequisites - [x] [Python>=3.10](https://python.org) *(Optional)* ##
-Installation and Usage ### Installation Download binaries for your system from
-[here.](https://github.com/Simatwa/python-tgpt/releases/latest/) Alternatively,
-you can install non-binaries. *(Recommended)* 1. Developers: ```sh pip install
---upgrade python-tgpt ``` 2. Commandline: ```sh pip install --upgrade "python-
-tgpt[cli]" ``` 3. Full installation: ```sh pip install --upgrade "python-tgpt
-[all]" ``` > `pip install -U "python-tgt[api]"` will install REST API
-dependencies. ## Usage This package offers a convenient command-line interface.
-> [!NOTE] > `phind` is the default *provider*. - For a quick response: ```bash
-python -m pytgpt generate "" ``` - For interactive mode: ```bash python -
-m pytgpt interactive "" ``` Make use of flag `--provider` followed by the
-provider name of your choice. e.g `--provider koboldai` > To list all providers
-offered by gpt4free, use following commands: ```pytgpt gpt4free list
-providers``` You can also simply use `pytgpt` instead of `python -m pytgpt`.
-Starting from version 0.2.7, running `$ pytgpt` without any other command or
-option will automatically enter the `interactive` mode. Otherwise, you'll need
-to explicitly declare the desired action, for example, by running `$ pytgpt
-generate`. ### Developer Docs 1. Generate a quick response ```python from
-pytgpt.leo import LEO bot = LEO() resp = bot.chat('') print(resp) # Output :
-How may I help you. ``` 2. Get back whole response ```python from pytgpt.leo
-import LEO bot = LEO() resp = bot.ask('
+capabilities - ð¤ Text-to-audio conversion capabilities - âï¸ Chained
+requests via proxy - ð¨ï¸ Enhanced conversational chat experience - ð¾
+Capability to save prompts and responses (Conversation) - ð Ability to load
+previous conversations - ð¤ Pass [awesome-chatgpt prompts](https://
+github.com/f/awesome-chatgpt-prompts) easily ## Providers These are simply the
+hosts of the LLMs, which include: 1. [Leo](https://brave.com/leo/) - **Brave**
+2. [Koboldai](https://koboldai-koboldcpp-tiefighter.hf.space) 3. [OpenGPTs]
+(https://opengpts-example-vz4y4ooboq-uc.a.run.app/) 4. [OpenAI](https://
+chat.openai.com) *(API key required)* 5. [WebChatGPT](https://github.com/
+Simatwa/WebChatGPT) - **OpenAI** *(Session ID required)* 6. [Gemini](https://
+github.com/Simatwa/bard) - **Google** *(Session ID required)* 9. [Phind](https:
+//www.phind.com) 10. [Llama2](https://www.llama2.ai) 11. [Blackboxai](https://
+www.blackbox.ai) 12. [gpt4all](https://gpt4all.io) *(Offline)* 13. [Poe](https:
+//poe.com) - Poe|Quora *(Session ID required)* 14. [Groq](https://
+console.groq.com/playground) *(API Key required)* 15. [Perplexity](https://
+www.perplexity.ai) 16. [YepChat](https://yep.com) 41+ providers proudly offered
+by [gpt4free](https://github.com/xtekky/gpt4free). - To list working providers
+run: ```sh $ pytgpt gpt4free test -y ``` ## Prerequisites - [x] [Python>=3.10]
+(https://python.org) *(Optional)* ## Installation and Usage ### Installation
+Download binaries for your system from [here.](https://github.com/Simatwa/
+python-tgpt/releases/latest/) Alternatively, you can install non-binaries. *
+(Recommended)* 1. Developers: ```sh pip install --upgrade python-tgpt ``` 2.
+Commandline: ```sh pip install --upgrade "python-tgpt[cli]" ``` 3. Full
+installation: ```sh pip install --upgrade "python-tgpt[all]" ``` > `pip install
+-U "python-tgt[api]"` will install REST API dependencies. ## Usage This package
+offers a convenient command-line interface. > [!NOTE] > `phind` is the default
+*provider*. - For a quick response: ```bash python -m pytgpt generate "" ``` -
+For interactive mode: ```bash python -m pytgpt interactive "" ``` Make use of
+flag `--provider` followed by the provider name of your choice. e.g `--provider
+koboldai` > To list all providers offered by gpt4free, use following commands:
+```pytgpt gpt4free list providers``` You can also simply use `pytgpt` instead
+of `python -m pytgpt`. Starting from version 0.2.7, running `$ pytgpt` without
+any other command or option will automatically enter the `interactive` mode.
+Otherwise, you'll need to explicitly declare the desired action, for example,
+by running `$ pytgpt generate`. ### Developer Docs 1. Generate a quick response
+```python from pytgpt.leo import LEO bot = LEO() resp = bot.chat('') print
+(resp) # Output : How may I help you. ``` 2. Get back whole response ```python
+from pytgpt.leo import LEO bot = LEO() resp = bot.ask('
  Output """ {'completion': "I'm so excited to share with you the incredible
 experiences...", 'stop_reason': None, 'truncated': False, 'stop': None,
 'model': 'llama-2-13b-chat', 'log_id': 'cmpl-3NmRt5A5Djqo2jXtXLBwJ2',
 'exception': None} """ ``` #### Stream Response Just add parameter `stream`
 with value `true`. 1. Text Generated only ```python from pytgpt.leo import LEO
 bot = LEO() resp = bot.chat('', stream=True) for value in resp: print(value) #
 output """ How may How may I help How may I help you How may I help you today?
@@ -216,26 +216,30 @@
 www.videolan.org/vlc/index.html) installed on your system or, if you are a
 [Termux](https://termux.org) user, the [Termux:API](https://wiki.termux.com/
 wiki/Termux:API) package. To activate speech synthesis, use the `--talk-to-me`
 flag or its shorthand `-ttm` when running your commands. For example: ```bash $
 pytgpt generate "Generate an ogre story" --talk-to-me ``` or ```bash $ pytgpt
 interactive -ttm ``` This flag instructs the system to audiolize the ai
 responses and then play them, enhancing the user experience by providing
-auditory feedback. > To speech synthesise the responses just ensure you have
-[vlc player]() in your system or [termux-api](https://wiki.termux.com/wiki/
-Termux:API) for the case of [Termux](https://termux.org) users. > Use the flag
-`--talk-to-me`, shortform `-ttm`. Version **0.6.4** introduces another dynamic
-provider, `auto`, which denotes the working provider **overall**. This relieves
-you of the workload of manually checking a working provider each time you fire
-up pytgpt. For more usage info run `$ pytgpt --help` ``` Usage: pytgpt
-[OPTIONS] COMMAND [ARGS]... Options: -v, --version Show the version and exit. -
-h, --help Show this message and exit. Commands: api FastAPI control endpoint
-awesome Perform CRUD operations on awesome-prompts generate Generate a quick
-response with AI gpt4free Discover gpt4free models, providers etc imager
-Generate images with pollinations.ai interactive Chat with AI interactively
-(Default) utils Utility endpoint for pytgpt webchatgpt Reverse Engineered
-ChatGPT Web-Version ``` ### API Health Status | No. | API | Status | |--------
-|-----|--------| | 1. | [On-render](https://python-tgpt.onrender.com) | [cron-
-job](https://pqfzhmvz.status.cron-job.org/) | ## [CHANGELOG](https://
-github.com/Simatwa/python-tgpt/blob/main/docs/CHANGELOG.md) ## Acknowledgements
-1. [x] [tgpt](https://github.com/aandrew-me/tgpt) 2. [x] [gpt4free](https://
-github.com/xtekky/gpt4free)
+auditory feedback. Version **0.6.4** introduces another dynamic provider,
+`auto`, which denotes the working provider **overall**. This relieves you of
+the workload of manually checking a working provider each time you fire up
+pytgpt. ## [Telegram Bot](https://github.com/Simatwa/pytgpt-bot) If you're not
+satisfied with the existing interfaces, [pytgpt-bot](https://github.com/
+Simatwa/pytgpt-bot) could be the solution you're seeking. This bot is designed
+to enhance your experience by offering a wide range of functionalities. Whether
+you're interested in engaging in AI-driven conversations, creating images and
+audio from text, or exploring other innovative features, [pytgpt-bot is
+equipped to meet your needs.](https://github.com/Simatwa/pytgpt-bot) For more
+usage info run `$ pytgpt --help` ``` Usage: pytgpt [OPTIONS] COMMAND [ARGS]...
+Options: -v, --version Show the version and exit. -h, --help Show this message
+and exit. Commands: api FastAPI control endpoint awesome Perform CRUD
+operations on awesome-prompts generate Generate a quick response with AI
+gpt4free Discover gpt4free models, providers etc imager Generate images with
+pollinations.ai interactive Chat with AI interactively (Default) utils Utility
+endpoint for pytgpt webchatgpt Reverse Engineered ChatGPT Web-Version ``` ###
+API Health Status | No. | API | Status | |--------|-----|--------| | 1. | [On-
+render](https://python-tgpt.onrender.com) | [cron-job](https://
+pqfzhmvz.status.cron-job.org/) | ## [CHANGELOG](https://github.com/Simatwa/
+python-tgpt/blob/main/docs/CHANGELOG.md) ## Acknowledgements 1. [x] [tgpt]
+(https://github.com/aandrew-me/tgpt) 2. [x] [gpt4free](https://github.com/
+xtekky/gpt4free)
```

### Comparing `python_tgpt-0.6.5/src/python_tgpt.egg-info/SOURCES.txt` & `python_tgpt-0.6.6/src/python_tgpt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.6.5/tests/test_api.py` & `python_tgpt-0.6.6/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.6.5/tests/test_imager.py` & `python_tgpt-0.6.6/tests/test_imager.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.6.5/tests/test_utils.py` & `python_tgpt-0.6.6/tests/test_utils.py`

 * *Files identical despite different names*


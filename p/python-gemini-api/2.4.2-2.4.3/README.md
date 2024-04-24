# Comparing `tmp/python-gemini-api-2.4.2.tar.gz` & `tmp/python_gemini_api-2.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-gemini-api-2.4.2.tar", last modified: Thu Apr  4 08:41:38 2024, max compression
+gzip compressed data, was "python_gemini_api-2.4.3.tar", last modified: Wed Apr 24 10:21:02 2024, max compression
```

## Comparing `python-gemini-api-2.4.2.tar` & `python_gemini_api-2.4.3.tar`

### file list

```diff
@@ -1,46 +1,48 @@
-drwxrwxrwx   0        0        0        0 2024-04-04 08:41:38.091471 python-gemini-api-2.4.2/
--rw-rw-rw-   0        0        0     1097 2024-02-13 10:03:29.000000 python-gemini-api-2.4.2/LICENSE
--rw-rw-rw-   0        0        0    32655 2024-04-04 08:41:38.089966 python-gemini-api-2.4.2/PKG-INFO
--rw-rw-rw-   0        0        0    31352 2024-03-31 08:34:47.000000 python-gemini-api-2.4.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-04 08:41:38.043139 python-gemini-api-2.4.2/gemini/
--rw-rw-rw-   0        0        0     1140 2024-04-04 08:40:39.000000 python-gemini-api-2.4.2/gemini/__init__.py
--rw-rw-rw-   0        0        0    15192 2024-03-18 04:20:24.000000 python-gemini-api-2.4.2/gemini/async_client.py
--rw-rw-rw-   0        0        0    18814 2024-04-04 08:40:05.000000 python-gemini-api-2.4.2/gemini/client.py
-drwxrwxrwx   0        0        0        0 2024-04-04 08:41:38.045143 python-gemini-api-2.4.2/gemini/src/
--rw-rw-rw-   0        0        0        0 2024-03-05 10:25:37.000000 python-gemini-api-2.4.2/gemini/src/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-04 08:41:38.047144 python-gemini-api-2.4.2/gemini/src/extensions/
--rw-rw-rw-   0        0        0       40 2024-03-16 06:40:55.000000 python-gemini-api-2.4.2/gemini/src/extensions/__init__.py
--rw-rw-rw-   0        0        0      622 2024-03-18 04:30:10.000000 python-gemini-api-2.4.2/gemini/src/extensions/replit.py
-drwxrwxrwx   0        0        0        0 2024-04-04 08:41:38.055691 python-gemini-api-2.4.2/gemini/src/misc/
--rw-rw-rw-   0        0        0      251 2024-03-18 04:18:05.000000 python-gemini-api-2.4.2/gemini/src/misc/__init__.py
--rw-rw-rw-   0        0        0     8623 2024-03-20 05:43:08.000000 python-gemini-api-2.4.2/gemini/src/misc/constants.py
--rw-rw-rw-   0        0        0     3063 2024-03-18 04:29:01.000000 python-gemini-api-2.4.2/gemini/src/misc/decorator.py
--rw-rw-rw-   0        0        0      824 2024-03-11 08:18:15.000000 python-gemini-api-2.4.2/gemini/src/misc/exceptions.py
--rw-rw-rw-   0        0        0     3278 2024-03-18 04:48:49.000000 python-gemini-api-2.4.2/gemini/src/misc/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-04 08:41:38.059702 python-gemini-api-2.4.2/gemini/src/model/
--rw-rw-rw-   0        0        0       88 2024-03-16 06:40:55.000000 python-gemini-api-2.4.2/gemini/src/model/__init__.py
--rw-rw-rw-   0        0        0     8611 2024-03-18 04:29:31.000000 python-gemini-api-2.4.2/gemini/src/model/image.py
--rw-rw-rw-   0        0        0     1858 2024-03-31 11:20:09.000000 python-gemini-api-2.4.2/gemini/src/model/output.py
-drwxrwxrwx   0        0        0        0 2024-04-04 08:41:38.065721 python-gemini-api-2.4.2/gemini/src/model/parser/
--rw-rw-rw-   0        0        0      130 2024-03-17 09:52:54.000000 python-gemini-api-2.4.2/gemini/src/model/parser/__init__.py
--rw-rw-rw-   0        0        0     1490 2024-03-05 10:15:40.000000 python-gemini-api-2.4.2/gemini/src/model/parser/base.py
--rw-rw-rw-   0        0        0     5433 2024-03-31 11:20:09.000000 python-gemini-api-2.4.2/gemini/src/model/parser/custom_parser.py
--rw-rw-rw-   0        0        0     7692 2024-03-31 11:20:09.000000 python-gemini-api-2.4.2/gemini/src/model/parser/response_parser.py
-drwxrwxrwx   0        0        0        0 2024-04-04 08:41:38.067794 python-gemini-api-2.4.2/gemini/src/modules/
--rw-rw-rw-   0        0        0        0 2024-03-29 00:25:32.000000 python-gemini-api-2.4.2/gemini/src/modules/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-04 08:41:38.071297 python-gemini-api-2.4.2/gemini/src/modules/openrouter/
--rw-rw-rw-   0        0        0       31 2024-03-26 07:55:29.000000 python-gemini-api-2.4.2/gemini/src/modules/openrouter/__init__.py
--rw-rw-rw-   0        0        0     5103 2024-03-27 02:57:53.000000 python-gemini-api-2.4.2/gemini/src/modules/openrouter/client.py
-drwxrwxrwx   0        0        0        0 2024-04-04 08:41:38.075564 python-gemini-api-2.4.2/gemini/src/modules/voice/
--rw-rw-rw-   0        0        0       88 2024-03-18 04:18:39.000000 python-gemini-api-2.4.2/gemini/src/modules/voice/__init__.py
--rw-rw-rw-   0        0        0     2441 2024-03-18 04:18:26.000000 python-gemini-api-2.4.2/gemini/src/modules/voice/google.py
--rw-rw-rw-   0        0        0     3144 2024-03-17 14:01:32.000000 python-gemini-api-2.4.2/gemini/src/modules/voice/openai.py
-drwxrwxrwx   0        0        0        0 2024-04-04 08:41:38.088966 python-gemini-api-2.4.2/python_gemini_api.egg-info/
--rw-rw-rw-   0        0        0    32655 2024-04-04 08:41:37.000000 python-gemini-api-2.4.2/python_gemini_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1017 2024-04-04 08:41:38.000000 python-gemini-api-2.4.2/python_gemini_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-04 08:41:37.000000 python-gemini-api-2.4.2/python_gemini_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2024-04-04 08:41:37.000000 python-gemini-api-2.4.2/python_gemini_api.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      111 2024-04-04 08:41:37.000000 python-gemini-api-2.4.2/python_gemini_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-04 08:41:37.000000 python-gemini-api-2.4.2/python_gemini_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-04 08:41:38.092476 python-gemini-api-2.4.2/setup.cfg
--rw-rw-rw-   0        0        0     2184 2024-03-18 04:48:51.000000 python-gemini-api-2.4.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-24 10:21:02.304932 python_gemini_api-2.4.3/
+-rw-rw-rw-   0        0        0    35823 2024-04-24 10:16:55.000000 python_gemini_api-2.4.3/LICENSE
+-rw-rw-rw-   0        0        0    36565 2024-04-24 10:21:02.302935 python_gemini_api-2.4.3/PKG-INFO
+-rw-rw-rw-   0        0        0    35262 2024-04-24 10:16:55.000000 python_gemini_api-2.4.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-24 10:21:02.240656 python_gemini_api-2.4.3/gemini/
+-rw-rw-rw-   0        0        0     1443 2024-04-24 10:20:48.000000 python_gemini_api-2.4.3/gemini/__init__.py
+-rw-rw-rw-   0        0        0    15192 2024-03-18 04:20:24.000000 python_gemini_api-2.4.3/gemini/async_client.py
+-rw-rw-rw-   0        0        0    19096 2024-04-17 13:21:33.000000 python_gemini_api-2.4.3/gemini/client.py
+drwxrwxrwx   0        0        0        0 2024-04-24 10:21:02.242933 python_gemini_api-2.4.3/gemini/src/
+-rw-rw-rw-   0        0        0        0 2024-03-05 10:25:37.000000 python_gemini_api-2.4.3/gemini/src/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 10:21:02.245132 python_gemini_api-2.4.3/gemini/src/extensions/
+-rw-rw-rw-   0        0        0       40 2024-03-16 06:40:55.000000 python_gemini_api-2.4.3/gemini/src/extensions/__init__.py
+-rw-rw-rw-   0        0        0      622 2024-03-18 04:30:10.000000 python_gemini_api-2.4.3/gemini/src/extensions/replit.py
+drwxrwxrwx   0        0        0        0 2024-04-24 10:21:02.255931 python_gemini_api-2.4.3/gemini/src/misc/
+-rw-rw-rw-   0        0        0      265 2024-04-17 09:46:31.000000 python_gemini_api-2.4.3/gemini/src/misc/__init__.py
+-rw-rw-rw-   0        0        0     9279 2024-04-05 10:13:11.000000 python_gemini_api-2.4.3/gemini/src/misc/constants.py
+-rw-rw-rw-   0        0        0     3063 2024-03-18 04:29:01.000000 python_gemini_api-2.4.3/gemini/src/misc/decorator.py
+-rw-rw-rw-   0        0        0     2421 2024-04-20 13:54:53.000000 python_gemini_api-2.4.3/gemini/src/misc/exceptions.py
+-rw-rw-rw-   0        0        0     4487 2024-04-17 09:46:59.000000 python_gemini_api-2.4.3/gemini/src/misc/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-24 10:21:02.261922 python_gemini_api-2.4.3/gemini/src/model/
+-rw-rw-rw-   0        0        0       88 2024-03-16 06:40:55.000000 python_gemini_api-2.4.3/gemini/src/model/__init__.py
+-rw-rw-rw-   0        0        0     8611 2024-03-18 04:29:31.000000 python_gemini_api-2.4.3/gemini/src/model/image.py
+-rw-rw-rw-   0        0        0     1858 2024-03-31 11:20:09.000000 python_gemini_api-2.4.3/gemini/src/model/output.py
+drwxrwxrwx   0        0        0        0 2024-04-24 10:21:02.270196 python_gemini_api-2.4.3/gemini/src/model/parser/
+-rw-rw-rw-   0        0        0      130 2024-03-17 09:52:54.000000 python_gemini_api-2.4.3/gemini/src/model/parser/__init__.py
+-rw-rw-rw-   0        0        0     1490 2024-03-05 10:15:40.000000 python_gemini_api-2.4.3/gemini/src/model/parser/base.py
+-rw-rw-rw-   0        0        0     5433 2024-03-31 11:20:09.000000 python_gemini_api-2.4.3/gemini/src/model/parser/custom_parser.py
+-rw-rw-rw-   0        0        0     7692 2024-03-31 11:20:09.000000 python_gemini_api-2.4.3/gemini/src/model/parser/response_parser.py
+drwxrwxrwx   0        0        0        0 2024-04-24 10:21:02.272285 python_gemini_api-2.4.3/gemini/src/modules/
+-rw-rw-rw-   0        0        0        0 2024-03-29 00:25:32.000000 python_gemini_api-2.4.3/gemini/src/modules/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 10:21:02.281091 python_gemini_api-2.4.3/gemini/src/modules/openrouter/
+-rw-rw-rw-   0        0        0      102 2024-04-21 13:59:49.000000 python_gemini_api-2.4.3/gemini/src/modules/openrouter/__init__.py
+-rw-rw-rw-   0        0        0     3043 2024-04-21 13:58:36.000000 python_gemini_api-2.4.3/gemini/src/modules/openrouter/async_client.py
+-rw-rw-rw-   0        0        0     4748 2024-04-21 13:58:36.000000 python_gemini_api-2.4.3/gemini/src/modules/openrouter/client.py
+-rw-rw-rw-   0        0        0      447 2024-04-21 14:07:31.000000 python_gemini_api-2.4.3/gemini/src/modules/openrouter/const.py
+drwxrwxrwx   0        0        0        0 2024-04-24 10:21:02.287170 python_gemini_api-2.4.3/gemini/src/modules/voice/
+-rw-rw-rw-   0        0        0       88 2024-03-18 04:18:39.000000 python_gemini_api-2.4.3/gemini/src/modules/voice/__init__.py
+-rw-rw-rw-   0        0        0     2441 2024-03-18 04:18:26.000000 python_gemini_api-2.4.3/gemini/src/modules/voice/google.py
+-rw-rw-rw-   0        0        0     3144 2024-03-17 14:01:32.000000 python_gemini_api-2.4.3/gemini/src/modules/voice/openai.py
+drwxrwxrwx   0        0        0        0 2024-04-24 10:21:02.300828 python_gemini_api-2.4.3/python_gemini_api.egg-info/
+-rw-rw-rw-   0        0        0    36565 2024-04-24 10:21:02.000000 python_gemini_api-2.4.3/python_gemini_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1102 2024-04-24 10:21:02.000000 python_gemini_api-2.4.3/python_gemini_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 10:21:02.000000 python_gemini_api-2.4.3/python_gemini_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2024-04-24 10:21:02.000000 python_gemini_api-2.4.3/python_gemini_api.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      111 2024-04-24 10:21:02.000000 python_gemini_api-2.4.3/python_gemini_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-24 10:21:02.000000 python_gemini_api-2.4.3/python_gemini_api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-24 10:21:02.304932 python_gemini_api-2.4.3/setup.cfg
+-rw-rw-rw-   0        0        0     2184 2024-03-18 04:48:51.000000 python_gemini_api-2.4.3/setup.py
```

### Comparing `python-gemini-api-2.4.2/PKG-INFO` & `python_gemini_api-2.4.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,214 +1,201 @@
-Metadata-Version: 2.1
-Name: python-gemini-api
-Version: 2.4.2
-Summary: The python package that returns Response of Google Gemini through API.
-Home-page: https://github.com/dsdanielpark/Gemini-API
-Author: Daniel Park
-Author-email: parkminwoo1991@gmail.com
-Keywords: Python,API,Gemini,Google Gemini,Large Language Model,Chatbot API,Google API,Chatbot
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Intended Audience :: Science/Research
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: httpx[http2]>=0.20.0
-Requires-Dist: requests
-Requires-Dist: browser_cookie3
-Requires-Dist: loguru
-Requires-Dist: pydantic
-Provides-Extra: voice
-Requires-Dist: gTTS; extra == "voice"
-Requires-Dist: SpeechRecognition; extra == "voice"
-Requires-Dist: openai; extra == "voice"
-Requires-Dist: anthropic; extra == "voice"
-
 
 # <img src="https://www.gstatic.com/lamda/images/favicon_v1_150160cddff7f294ce30.svg" width="35px" alt="Gemini Icon" /> Gemini API  <a href="https://pypi.org/project/python-gemini-api/"> <img alt="PyPI" src="https://img.shields.io/pypi/v/python-gemini-api?color=black"></a>
 
 
 <p align="right">
     <a href="https://github.com/dsdanielpark/Gemini-API"><img alt="pip download" src="https://img.shields.io/badge/pip_install-python_gemini_api-black"></a> 
     <a href="https://github.com/psf/black"><img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg"></a>
     <a href="https://hits.seeyoufarm.com"><img src="https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2Fdsdanielpark%2FGemini-API&count_bg=%23000000&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=views&edge_flat=false"/></a>
     <a href="https://pypistats.org/packages/python-gemini-api"><img alt="Downloads" src="https://pepy.tech/badge/python-gemini-api"></a>
 <!-- <a href="https://github.com/dsdanielpark/Gemini-API/stargazers"><img src="https://img.shields.io/github/stars/dsdanielpark/Gemini-API?style=social"></a> -->
 </p>
 
 
+
 https://github.com/dsdanielpark/Gemini-API/assets/81407603/e0c11d4f-3fe1-4cbb-ba79-d9f89b637324
 
 
 
 
 
 
 A *unofficial* Python wrapper, [python-gemini-api](https://pypi.org/project/python-gemini-api/), operates through reverse-engineering, utilizing cookie values to interact with [Google Gemini](https://gemini.google.com) for users struggling with frequent authentication problems or unable to authenticate via [Google Authentication](https://developers.google.com/identity/protocols/oauth2?hl=en).
 
 Collaborated competently with [Antonio Cheong](https://github.com/acheong08).
 
-
-
-
+<br>
 
 <br>
 
 
 > [!TIP]
 > | 2024-03-26 | [[See Code Examples]](https://github.com/dsdanielpark/Gemini-API/blob/main/documents/README_OPENROUTER.md)
 > 
 > Check out temporarily free Open-source LLM APIs with Open Router.  (Free limit: 10 requests/minute) 
 
-<br><br>
+<br>
 
+## Contents
 
 - [ Gemini API   ](#-gemini-api---)
-  - [What is Gemini?](#what-is-gemini)
-  - [Installation](#installation)
-  - [Authentication](#authentication)
-  - [Quick Start](#quick-start)
+  - [What is Gemini? 🔐](#what-is-gemini)
+  - [Installation ✅](#installation-)
+  - [Authentication ✅](#authentication)
+  - [Quick Start ✅](#quick-start)
   - [Usage](#usage)
-    - [# 01. Initialization](#-01-initialization)
+    - [# 01. Initialization ✅](#-01-initialization)
     - [# 02. Generate content](#-02-generate-content)
     - [# 03. Send request](#-03-send-request)
     - [# 04. Text generation](#-04-text-generation)
     - [# 05. Image generation](#-05-image-generation)
     - [# 06. Retrieving Images from Gemini Responses](#-06-retrieving-images-from-gemini-responses)
     - [# 07. Generate content from images](#-07-generate-content-from-images)
     - [# 08. Generate content using Google Services](#-08-generate-content-using-google-services)
-    - [# 09. Fix context setting rcid](#-09-fix-context-setting-rcid)
+    - [# 09. Fix context setting RCID](#-09-fix-context-setting-rcid)
     - [# 10. Changing the Selected Response from 0 to *n*](#-10-changing-the-selected-response-from-0-to-n)
     - [# 11. Generate custom content](#-11-generate-custom-content)
   - [Further](#further)
-  - [Open-source LLM, Gemma](#open-source-llm-gemma)
-    - [How to use Gemma](#how-to-use-gemma)
-  - [Utilize free open-source LLM API through Open Router](#utilize-free-open-source-llm-api-through-open-router)
+  - [Google Open-source LLMs](#google-open-source-llms)
+      - [Open-source LLM, Gemma 🤝](#open-source-llm-gemma)
+      - [Open-source LLM, Code Gemma 🤝](#open-source-llm-code-gemma)
+  - [Utilize free open-source LLM API through Open Router ✅](#utilize-free-open-source-llm-api-through-open-router)
 
 
 
 
 
 
 
 <br>
 
+## What is [Gemini](https://deepmind.google/technologies/gemini/#introduction)?
 
+| [Paper](https://arxiv.org/abs/2312.11805) | [Official Website](https://deepmind.google/technologies/gemini/#introduction) | [Official API](https://aistudio.google.com/) | [API Documents](https://cloud.google.com/vertex-ai/docs/generative-ai/model-reference/gemini) |
 
+Gemini is a family of generative AI models developed by Google DeepMind that is designed for multimodal use cases. The Gemini API gives you access to the Gemini Pro and Gemini Pro Vision models. In February 2024, Google's **Bard** service was changed to **Gemini**.
 
+#### Overview of Google LLMs
 
-## What is [Gemini](https://deepmind.google/technologies/gemini/#introduction)?
+| Model | Type | Access | Details
+|:-------:|:------:|:--------:|---------
+[Gemini](https://huggingface.co/google/gemma-7b) | Proprietary | API <sup>[[13](https://ai.google.dev/tutorials/ai-studio_quickstart)] | A proprietary multimodal AI by Google DeepMind, including advanced models such as Gemini Pro and Gemini Pro Vision. Access is restricted to API usage; additional insights may be obtained through the paper and website. <sup>[[1](https://arxiv.org/abs/2312.11805)][[2](https://deepmind.google/technologies/gemini/#introduction)]</sup>
+[Gemma](https://huggingface.co/google/gemma-7b) | Open Source | [Downloadable](https://huggingface.co/google/gemma-7b) <br>[Free API](https://github.com/dsdanielpark/Gemini-API?tab=readme-ov-file#utilize-free-open-source-llm-api-through-open-router) | An open-source text-to-text language model suitable for tasks like QA and summarization. Weights are downloadable for on-premises use, and detailed documentation is provided via the paper and website. <sup>[[3](https://arxiv.org/abs/2403.08295)][[4](https://ai.google.dev/gemma/docs)]</sup>
+[Code Gemma](https://huggingface.co/google/codegemma-7b-it) | Open Source | [Downloadable](https://huggingface.co/google/codegemma-7b-it) | Designed specifically for programming tasks, this open-source model offers downloadable weights to assist developers with code generation and similar activities. Refer to the associated paper, blog post, and Hugging Face collection for more information. <sup>[[5](https://storage.googleapis.com/deepmind-media/gemma/codegemma_report.pdf?utm_source=substack&utm_medium=email)][[6](https://huggingface.co/blog/codegemma)][[7](https://huggingface.co/collections/google/codegemma-release-66152ac7b683e2667abdee11)]</sup>
 
-| [Paper](https://arxiv.org/abs/2312.11805) | [Official Website](https://deepmind.google/technologies/gemini/#introduction) | [Official API](https://aistudio.google.com/) | [API Documents](https://cloud.google.com/vertex-ai/docs/generative-ai/model-reference/gemini) |
 
-Gemini is a family of generative AI models developed by Google DeepMind that is designed for multimodal use cases. The Gemini API gives you access to the Gemini Pro and Gemini Pro Vision models. In February 2024, Google's **Bard** service was changed to **Gemini**.
+<br>
 
+## What is [Python-Gemini-API](https://github.com/dsdanielpark/Gemini-API)?
 
+This is a Python wrapper derived from the [Bard API](https://github.com/dsdanielpark/Bard-API) project, designed to retrieve responses from Gemini Web in REST format. **Synchronous clients are preferred over asynchronous ones for Gemini because of rate limiting and blocking concerns.**
 
 ## Installation 📦
 ```
 pip install python-gemini-api
 ```
 ```
 pip install git+https://github.com/dsdanielpark/Gemini-API.git
 ```
 For the updated version, use as follows:
 ```
 pip install -q -U python-gemini-api
 ```
+
+
+
 ## Authentication
-> [!NOTE]
-> Cookies can change quickly. Don't reopen the same session or repeat prompts too often; they'll expire faster. If the cookie value doesn't export correctly, refresh the Gemini page and export again. 
+
 1. Visit https://gemini.google.com/ <br>
     With browser open, try auto-collecting cookies first.
     ```python
     from gemini import Gemini
     GeminiClient = Gemini(auto_cookies=True)
 
     # Testing needed as cookies vary by region.
     # GeminiClient = Gemini(auto_cookies=True, target_cookies=["__Secure-1PSID", "__Secure-1PSIDTS"])
+    # GeminiClient = Gemini(auto_cookies=True, target_cookies="all") # You can pass whole cookies
 
     response = GeminiClient.generate_content("Hello, Gemini. What's the weather like in Seoul today?")
     print(response.payload)
     ```
 2. *(Manually)* `F12` for browser console → `Session: Application` → `Cookies` → Copy the value of some working cookie sets. If it doesn't work, go to step 3.
     <details><summary>Some working cookie sets</summary>
     Cookies may vary by account or region. 
       
     First try `__Secure-1PSIDCC` alone. If it doesn't work, use `__Secure-1PSID` and `__Secure-1PSIDTS`. Still no success? Try these four cookies: `__Secure-1PSIDCC`, `__Secure-1PSID`, `__Secure-1PSIDTS`, `NID`. If none work, proceed to step 3 and consider sending the entire cookie file.
     
     </details>
 
 3. *(Recommended)* Export Gemini site cookies via a browser extension. For instance, use Chrome extension [ExportThisCookies](https://chromewebstore.google.com/detail/exportthiscookie/dannllckdimllhkiplchkcaoheibealk), open, and copy the txt file contents.
 
+
+<br>
+
 <details><summary>Further: For manual collection or Required for a few users upon error</summary>
 
 4. For manual cookie collection, refer to [this image](assets/cookies.pdf). Press F12 → Network → Send any prompt to Gemini webui → Click the post address starting with "https://gemini.google.com/_/BardChatUi/data/assistant.lamda.BardFrontendService/StreamGenerate" → Headers → Request Headers → Cookie → Copy and Reformat as JSON manually.
 5. *(Required for a few users upon error)* If errors persist after manually collecting cookies, refresh the Gemini website and collect cookies again. If errors continue, some users may need to manually set the nonce value. To do this: Press F12 → Network → Send any prompt to Gemini webui → Click the post address starting with "https://gemini.google.com/_/BardChatUi/data/assistant.lamda.BardFrontendService/StreamGenerate" → Payload → Form Data → Copy the "at" key value. See [this image](assets/nonce_value.pdf) for reference.
 </details>
 
 
 > [!IMPORTANT] 
->  Try different Google accounts until you find a working cookie. Use a fresh browser to ensure no remaining cookie values. Use secret browsing mode with independent cookies. Results may vary depending on factors like IP and account status. Providing the entire set of cookies seems to fix one cookie per account. Additionally, once successfully connected with that cookie, it seems to work flawlessly for over three weeks without any errors. *Try various methods until you succeed. Experiment in different environments.*
+> Experiment with different Google accounts and browser settings to find a working cookie. Success may vary by IP and account status. Once connected, a cookie typically remains effective over a month. Keep testing until successful.
 
 
 <br>
 
 ## Quick Start
 
-*Simple usage*
-
-Setting Gemini response language (Optional): Check supported languages [here](https://developers.google.com/hotels/hotel-prices/dev-guide/country-codes). Default is English.
-
-```python
-import os
-os.environ["GEMINI_LANGUAGE"] = "KR"
-```
-
-
-
-Generate content: returns parsed response.
+**Generate content:** returns parsed response.
 ```python
 from gemini import Gemini
 
 cookies = {} # Cookies may vary by account or region. Consider sending the entire cookie file.
 GeminiClient = Gemini(cookies=cookies) # You can use various args
 
 response = GeminiClient.generate_content("Hello, Gemini. What's the weather like in Seoul today?")
 response.payload
 ```
 
-Generate content from image: you can use image as input.
+**Generate content from image:** you can use image as input.
 ```python
 from gemini import Gemini
 
 cookies = {} # Cookies may vary by account or region. Consider sending the entire cookie file.
 
 GeminiClient = Gemini(cookies=cookies) # You can use various args
 response = GeminiClient.generate_content("What does the text in this image say?", image='folder/image.jpg')
 response.payload
 ```
 
 > [!NOTE] 
 > If the generate_content method returns an empty payload, try executing it again without reinitializing the Gemini object.
 
-<br>
+<br><br>
 
 ## Usage
 
+*Setting language and Gemini version using environment variables:*
+
+Setting Gemini response language (Optional): Check supported languages [here](https://developers.google.com/hotels/hotel-prices/dev-guide/country-codes). Default is English.
+
+```python
+import os
+os.environ["GEMINI_LANGUAGE"] = "KR"  # Setting Gemini response language (Optional)
+os.environ["GEMINI_ULTRA"] = "1"      # Switch to Gemini-advanced response (Experimental, Optional)
+# In some accounts, access to Gemini Ultra may not be available. If that's the case, please revert it back to "0".
+```
+
+
+
+<br>
 
 ### # 01. Initialization
-Please explicitly declare `cookies` in dict format. You can also enter the path to the file containing the cookie with `cookie_fp`(*.json, *.txt supported). Check this [sample cookie file](https://github.com/dsdanielpark/Gemini-API/blob/main/cookies.txt).
+Please explicitly declare `cookies` in dict format. You can also enter the path to the file containing the cookie with `cookie_fp`(*.json, *.txt supported). Check sample cookie files in [assets](https://github.com/dsdanielpark/Gemini-API/tree/main/assets) folder.
 
 
 
 
 ```python
 from gemini import Gemini
 
@@ -221,53 +208,48 @@
   }
 
 GeminiClient = Gemini(cookies=cookies)
 # GeminiClient = Gemini(cookie_fp="folder/cookie_file.json") # (*.json, *.txt) are supported.
 # GeminiClient = Gemini(auto_cookies=True) # Or use auto_cookies paprameter
 ```
 
-#### Auto Cookie Update
-For `auto_cookie` to be set to `True`, Gemini WebUI must be active in the browser. The [browser_cookie3](https://github.com/borisbabic/browser_cookie3) enables automatic cookie collection, though updates may not be complete yet.
+##### Auto Cookie Update
+For `auto_cookie` to be set to `True`, and adjust `target_cookies`. Gemini WebUI must be active in the browser. The [browser_cookie3](https://github.com/borisbabic/browser_cookie3) enables automatic cookie collection, though updates may not be complete yet.
 
 
-> [!IMPORTANT]
->  **If the session connects successfully and `generate_content` runs well, CLOSE Gemini website.** If Gemini web stays open in the browser, cookies may expire faster.
 
 <br>
 
 ### # 02. Generate content
-Returns Gemini's response, but the first one might be empty. If generate_content yields an empty payload, rerun it without reinitializing Gemini. 
+Returns Gemini's response, but the first one might be empty. 
+
 
-Regardless of model output type, access the response_dict property (renamed to payload after v2.3.0).
-https://github.com/dsdanielpark/Gemini-API/blob/fdf064c57bc1fb47fbbb4b93067618a200e77f62/gemini/core.py#L252
 ```python
 prompt = "Hello, Gemini. What's the weather like in Seoul today?"
 response = GeminiClient.generate_content(prompt)
 print(response.payload)
 ```
+
+
 > [!IMPORTANT]
->  Once connected and generating valid content, **Be sure to CLOSE the Gemini website or CLOSE your browser** for cookie stability. 
+>  DO NOT send same prompt repeatly. **If the session connects successfully and `generate_content` runs well, CLOSE Gemini website.** If Gemini web stays open in the browser, cookies may expire faster. 
 
 <br>
 
-The output of the generate_content function is `GeminiModelOutput`, with the following structure:
-
-**Properties of GeminiModelOutput:**
+The output of the generate_content function is `GeminiModelOutput`, with the following structure: 
 - *rcid*: returns the response candidate id of the chosen candidate.
 - *text*: returns the text of the chosen candidate.
 - *code*: returns the codes of the chosen candidate.
 - *web_images*: returns a list of web images from the chosen candidate.
 - *generated_images*: returns a list of generated images from the chosen candidate.
-- *payload*: returns the response dictionary, if available. (same as *reponse_dict* under v2.3.0)
-
+- *payload*: returns the response dictionary, if available.
 https://github.com/dsdanielpark/Gemini-API/blob/fdf064c57bc1fb47fbbb4b93067618a200e77f62/gemini/src/model/output.py#L16
 
 
-> [!NOTE]
-> If the session fails to connect, works improperly, or terminates, returning an error, it is recommended to manually renew the cookies. The error is likely due to incorrect cookie values. Refresh or log out of Gemini web to renew cookies and try again. 
+
 
 <br>
 
 
 ### # 03. Send request
 Send request: returns the request's payload and status_code, making debugging easier.
 ```python
@@ -275,15 +257,15 @@
 
 cookies = {} # Cookies may vary by account or region. Consider sending the entire cookie file.
 GeminiClient = Gemini(cookies=cookies) # You can use various args
 
 response_text, response_status = GeminiClient.send_request("Hello, Gemini. What's the weather like in Seoul today?")
 print(response_text)
 ```
-
+You can track the total number of requests made by accessing the `request_count` property within the `Gemini` class.
 
 <br>
 
 ### # 04. Text generation
 Returns text generated by Gemini.
 ```python
 prompt = "Hello, Gemini. What's the weather like in Seoul today?"
@@ -292,65 +274,62 @@
 ```
 
 
 <br>
 
 ### # 05. Image generation
 Returns images generated by Gemini.
-https://github.com/dsdanielpark/Gemini-API/blob/fdf064c57bc1fb47fbbb4b93067618a200e77f62/gemini/src/model/image.py#L12
 
-*Sync downloader*
-```python
-from gemini import Gemini, GeminiImage
+*Async downloader*
 
+```python
 response = GeminiClient.generate_content("Create illustrations of Seoul, South Korea.")
-generated_images = response.generated_images # Check generated images [Dict]
 
-GeminiImage.save_sync(generated_images, save_path="save_dir", cookies=cookies)
+generated_images = response.generated_images # Check generated images [Dict]
 
-# You can use byte type image dict for printing images as follow:
-# bytes_images_dict = GeminiImage.fetch_images_dict_sync(generated_images, cookies=cookies) # Get bytes images dict
-# GeminiImage.save_images_sync(bytes_images_dict, path="save_dir", cookies=cookies) # Save to path
+await GeminiImage.save(generated_images, "save_dir", cookies=cookies)
+# image_data_dict = await GeminiImage.fetch_images_dict(generated_images, cookies=cookies)
+# await GeminiImage.save_images(image_data_dict, "save_dir")
 ```
 
-<details><summary>Display images in IPython</summary>
-  
+
+<details><summary>Further</summary>
+
+*Display images in IPython*
   You can display the image or transmit it to another application in byte format.
   
-  ```
+  ```python
   bytes_images_dict = GeminiImage.fetch_images_dict_sync(generated_images, cookies) # Get bytes images dict
   from IPython.display import display, Image
   import io
   
   for image_name, image_bytes in bytes_images_dict.items():
       print(image_name)
       image = Image(data=image_bytes)
       display(image)
   ```
 
-</details>
-
-
-
-*Async downloader*
 
+*Sync downloader*
 ```python
-response = GeminiClient.generate_content("Create illustrations of Seoul, South Korea.")
+from gemini import Gemini, GeminiImage
 
+response = GeminiClient.generate_content("Create illustrations of Seoul, South Korea.")
 generated_images = response.generated_images # Check generated images [Dict]
 
-await GeminiImage.save(generated_images, "save_dir", cookies=cookies)
-# image_data_dict = await GeminiImage.fetch_images_dict(generated_images, cookies=cookies)
-# await GeminiImage.save_images(image_data_dict, "save_dir")
-```
+GeminiImage.save_sync(generated_images, save_path="save_dir", cookies=cookies)
 
+# You can use byte type image dict for printing images as follow:
+# bytes_images_dict = GeminiImage.fetch_images_dict_sync(generated_images, cookies=cookies) # Get bytes images dict
+# GeminiImage.save_images_sync(bytes_images_dict, path="save_dir", cookies=cookies) # Save to path
+```
 
-<details><summary>Async downloader wrapper</summary>
+*Async downloader wrapper*
 
-```
+```python
 import asyncio
 from gemini import Gemini, GeminiImage
 
 async def save_generated_imagse(generated_imagse, save_path="save_dir", cookies=cookies):
     await GeminiImage.save(generated_imagse, save_path=save_path, cookies=cookies)
 
 # Run the async function
@@ -383,41 +362,45 @@
 > Use GeminiImage for image processing. `web_images` works without cookies, but for images like `generated_image` from Gemini, pass cookies. Cookies are needed to download images from Google's storage. Check the response or use existing cookies variable.
 
 <br>
 
 ### # 06. Retrieving Images from Gemini Responses
 Returns images in response of Gemini.
 
-*Sync downloader*
-```python
-from gemini import Gemini, GeminiImage
-
-response = GeminiClient.generate_content("Please recommend a travel itinerary for Seoul.")
-response_images = response.web_images # Check response images [Dict]
 
-GeminiImage.save_sync(response_images, save_path="save_dir")
-
-# You can use byte type image dict as follow:
-# bytes_images_dict = GeminiImage.fetch_bytes_sync(response_images, cookies) # Get bytes images dict
-# GeminiImage.save_images_sync(bytes_images_dict, path="save_dir") # Save to path
-```
 *Async downloader*
 ```python
 response = GeminiClient.generate_content("Create illustrations of Seoul, South Korea.")
 
 response_images = response.web_images # Check generated images [Dict]
 
 await GeminiImage.save(response_images, "save_dir")
 # image_data_dict = await GeminiImage.fetch_images_dict(response_images)
 # await GeminiImage.save_images(image_data_dict, "save_dir")
 ```
 
-<details><summary>Async downloader wrapper</summary>
+<details><summary>Further</summary>
 
+
+*Sync downloader*
+```python
+from gemini import Gemini, GeminiImage
+
+response = GeminiClient.generate_content("Please recommend a travel itinerary for Seoul.")
+response_images = response.web_images # Check response images [Dict]
+
+GeminiImage.save_sync(response_images, save_path="save_dir")
+
+# You can use byte type image dict as follow:
+# bytes_images_dict = GeminiImage.fetch_bytes_sync(response_images, cookies) # Get bytes images dict
+# GeminiImage.save_images_sync(bytes_images_dict, path="save_dir") # Save to path
 ```
+
+*Async downloader wrapper*
+```python
 import asyncio
 from gemini import Gemini, GeminiImage
 
 async def save_response_web_imagse(response_images, save_path="save_dir", cookies=cookies):
     await GeminiImage.save(response_images, save_path=save_path, cookies=cookies)
 
 # Run the async function
@@ -498,59 +481,68 @@
   - Description: Explore YouTube videos and ask questions about what interests you.
   - Features: Problem-solving, generating ideas, search, exploring topics
 </details>
 
 <br>
 
 
-### # 09. Fix context setting rcid
-You can specify a particular response by setting its response candidate id(rcid).
+### # 09. Fix context setting RCID
+You can specify a particular response by setting its Response Candidate ID(RCID).
 
 ```python
 # Generate content for the prompt "Give me some information about the USA."
 response1 = GeminiClient.generate_content("Give me some information about the USA.")
 # After reviewing the responses, choose the one you prefer and copy its RCID.
 GeminiClient.rcid = "rc_xxxx"
 
 # Now, generate content for the next prompt "How long does it take from LA to New York?"
 response2 = GeminiClient.generate_content("How long does it take from LA to New York?")
+
+# However, RCID may not persist. If parsing fails, reset `GeminiClient.rcid` to None.
+# GeminiClient.rcid = None
 ```
 
+
+
 <br>
 
 ### # 10. Changing the Selected Response from 0 to *n*
 In Gemini, generate_content returns the first response. This may vary depending on length or sorting. Therefore, you can specify the index of the chosen response from 0 to *n* as follows. However, if there is only one response, revert it back to 0.
 ```python
 from gemini import GeminiModelOutput
+
 GeminiModelOutput.chosen = 1 # default is 0
-response1 = GeminiClient.generate_content("Give me some information about the USA.")
+response_choice_1 = GeminiClient.generate_content("Give me some information about the USA.")
+
+# If not all Gemini returns are necessarily plural, revert back to 0 in case of errors.
+#  GeminiModelOutput.chosen = 0
 ```
 
 <br>
 
 ### # 11. Generate custom content 
 Parse the response text to extract desired values.
 
-https://github.com/dsdanielpark/Gemini-API/blob/fdf064c57bc1fb47fbbb4b93067618a200e77f62/gemini/core.py#L317
 
 Using `Gemini.generate_custom_content`, specify custom parsing to extract specific values. Utilize ParseMethod1 and ParseMethod2 by default, and you can pass custom parsing methods as arguments if desired. Refer to [custom_parser.py](https://github.com/dsdanielpark/Gemini-API/blob/main/gemini/src/model/parser/custom_parser.py).
 
 ```python
 # You can create a parser method that takes response_text as the input for custom_parser.
 response_text, response_status = GeminiClient.send_request("Give me some information about the USA.")
 
 # Use custom_parser function or class inheriting from BaseParser
 response = GeminiClient.generate_custom_content("Give me some information about the USA.", *custom_parser)
 ```
 
+https://github.com/dsdanielpark/Gemini-API/blob/31b842488bbc5429ad9c74b1d8b00e20d94e8cb1/gemini/client.py#L323
 <br>
 
 ## Further
 
-### Use rotating proxies
+### Use rotating proxies via [Smart Proxy by Crawlbase](https://crawlbase.com/docs/smart-proxy/?utm_source=github_ad&utm_medium=social&utm_campaign=bard_api)
 
 If you want to **avoid blocked requests** and bans, then use [Smart Proxy by Crawlbase](https://crawlbase.com/docs/smart-proxy/?utm_source=github_ad&utm_medium=social&utm_campaign=bard_api). It forwards your connection requests to a **randomly rotating IP address** in a pool of proxies before reaching the target website. The combination of AI and ML make it more effective to avoid CAPTCHAs and blocks.
 
 ```python
 # Get your proxy url at crawlbase https://crawlbase.com/docs/smart-proxy/get/
 proxy_url = "http://xxxxx:@smartproxy.crawlbase.com:8012" 
 proxies = {"http": proxy_url, "https": proxy_url}
@@ -558,16 +550,16 @@
 GeminiClient = Gemini(cookies=cookies, proxies=proxies, timeout=30)
 GeminiClient.generate_content("Hello, Gemini. Give me a beautiful photo of Seoul's scenery.")
 ```
 
 ### Reusable session object
 For standard cases, use Gemini class; for exceptions, use session objects. When creating a new bot Gemini server, adjust Headers.MAIN.
 ```python
-from gemini import Gemini, Headers
 import requests
+from gemini import Gemini, Headers
 
 cookies = {} 
 
 session = requests.Session()
 session.headers = Headers.MAIN
 for key, value in cookies.items():
     session.cookies.update({key: value})
@@ -584,42 +576,66 @@
 ## [More features](https://github.com/dsdanielpark/Gemini-API/blob/main/documents/README_DEV.md)
 Explore additional features in [this document](https://github.com/dsdanielpark/Gemini-API/blob/main/documents/README_DEV.md).
 
 If you want to develop your own simple code, you can start from [this simple code example](https://github.com/dsdanielpark/Gemini-API/blob/main/script/sample.ipynb).  
 
 <br>
 
+## Google Open-source LLMs
+
+If you have sufficient GPU resources, you can download weights directly instead of using the Gemini API to generate content. Consider Gemma and Code Gemma, an open-source models **available for on-premises use**.
+
+
 
-## Open-source LLM, [Gemma](https://huggingface.co/google/gemma-7b)
-If you have sufficient GPU resources, you can download weights directly instead of using the Gemini API to generate content. Consider Gemma, an open-source model **available for on-premises use**.
+### Open-source LLM, [Gemma](https://huggingface.co/google/gemma-7b)
 
-[Gemma](https://huggingface.co/google/gemma-7b) models are Google's lightweight, advanced text-to-text, decoder-only language models, derived from Gemini research. Available in English, they offer open weights and variants, ideal for tasks like question answering and summarization. Their small size enables deployment in resource-limited settings, broadening access to cutting-edge AI. For more infomation, visit [Gemma-7b](https://huggingface.co/google/gemma-7b) model card.
 
-### How to use Gemma
+Gemma models are Google's lightweight, advanced text-to-text, decoder-only language models, derived from Gemini research. Available in English, they offer open weights and variants, ideal for tasks like question answering and summarization. For more infomation, visit [Gemma-7b](https://huggingface.co/google/gemma-7b) model card.
+
+#### How to use Gemma
 ```python
 from transformers import AutoTokenizer, AutoModelForCausalLM
 
 tokenizer = AutoTokenizer.from_pretrained("google/gemma-7b")
 model = AutoModelForCausalLM.from_pretrained("google/gemma-7b")
 
 input_text = "Write me a poem about Machine Learning."
 input_ids = tokenizer(input_text, return_tensors="pt")
 
 outputs = model.generate(**input_ids)
 print(tokenizer.decode(outputs[0]))
 ```
 
+### Open-source LLM, [Code Gemma](https://huggingface.co/collections/google/codegemma-release-66152ac7b683e2667abdee11)
+
+CodeGemma, which is an official release from Google for code LLMs, was released on April 9, 2024. It provides three models specifically designed for generating and interacting with code. You can explore the [Code Gemma models](https://huggingface.co/collections/google/codegemma-release-66152ac7b683e2667abdee11) and view the [model card](https://huggingface.co/google/codegemma-7b-it) for more details.
+
+#### How to use Code Gemma
+```python
+from transformers import GemmaTokenizer, AutoModelForCausalLM
+
+tokenizer = GemmaTokenizer.from_pretrained("google/codegemma-7b-it")
+model = AutoModelForCausalLM.from_pretrained("google/codegemma-7b-it")
+
+input_text = "Write me a Python function to calculate the nth fibonacci number."
+input_ids = tokenizer(input_text, return_tensors="pt")
+
+outputs = model.generate(**input_ids)
+print(tokenizer.decode(outputs[0]))
+```
+
+
+
 <br>
 
 
 ## Utilize free open-source LLM API through [Open Router](https://openrouter.ai/)
-OpenRouter offers temporary free inference for select models. Obtain an API key from [Open Router API](https://openrouter.ai/keys) and check free models at [Open Router models](https://openrouter.ai/docs#models). Use models with a 0-dollar token cost primarily; other models may incur charges. See more [free open-source LLM API guide](https://github.com/dsdanielpark/Gemini-API/blob/main/documents/README_OPENROUTER.md)
+OpenRouter offers temporary free inference for select models. Obtain an API key from [Open Router API](https://openrouter.ai/keys) and check free models at [Open Router models](https://openrouter.ai/docs#models). Use models with a 0-dollar token cost primarily; other models may incur charges. See more at [free open-source LLM API guide](https://github.com/dsdanielpark/Gemini-API/blob/main/documents/README_OPENROUTER.md).
 
-> [!NOTE]
-> You can easily receive responses from open LLMs without this package by following the instructions on [here](https://openrouter.ai/docs#models).
+**Sync client is favored over async for Gemini due to rate limiting and blocking issues**, but OpenRouter offers reliable open-source LLMs for [async implementation](https://github.com/dsdanielpark/Gemini-API/blob/main/documents/README_OPENROUTER.md#openrouter-async-api-client).
 
 ```python
 from gemini import OpenRouter
 
 OPENROUTER_API_KEY = "<your_open_router_api_key>"
 GemmaClient = OpenRouter(api_key=OPENROUTER_API_KEY, model="google/gemma-7b-it:free")
 
@@ -643,28 +659,26 @@
 
 
 
 
 
 <br>
 
+## Sponsor, [Crawlbase](https://crawlbase.com/)
+Use [Crawlbase](https://crawlbase.com/) API for efficient data scraping to train AI models, boasting a 98% success rate and 99.9% uptime. It's quick to start, GDPR/CCPA compliant, supports massive data extraction, and is trusted by 70k+ developers.
+
+<br>
 
 ## [FAQ](https://github.com/dsdanielpark/Gemini-API/blob/main/documents/README_FAQ.md)
 First review [HanaokaYuzu/Gemini-API](https://github.com/HanaokaYuzu/Gemini-API) and the [Official Google Gemini API](https://aistudio.google.com/) before using this package.
 You can find most help on the [FAQ](https://github.com/dsdanielpark/Gemini-API/blob/main/documents/README_FAQ.md) and [Issue](https://github.com/dsdanielpark/Gemini-API/issues) pages. 
-
-
             
 ## [Issues](https://github.com/dsdanielpark/Gemini-API/issues)
 Sincerely grateful for any reports on new features or bugs. Your valuable feedback on the code is highly appreciated. Frequent errors may occur due to changes in Google's service API interface. Both [Issue reports](https://github.com/dsdanielpark/Gemini-API/issues) and [Pull requests](https://github.com/dsdanielpark/Gemini-API/pulls) contributing to improvements are always welcome. We strive to maintain an active and courteous open community.
 
-
-## Sponsor
-Use [Crawlbase](https://crawlbase.com/) API for efficient data scraping to train AI models, boasting a 98% success rate and 99.9% uptime. It's quick to start, GDPR/CCPA compliant, supports massive data extraction, and is trusted by 70k+ developers.
-
 ## Contributors
 We would like to express our sincere gratitude to all the contributors. 
 
 This package aims to re-implement the functionality of the [Bard API](https://github.com/dsdanielpark/Bard-API/), which has been archived for the contributions of the beloved open-source community, despite Gemini's official API already being available.
 
 Contributors to the [Bard API](https://github.com/dsdanielpark/Bard-API/) and [Gemini API](https://github.com/dsdanielpark/Gemini-API/).
 
@@ -696,20 +710,27 @@
 
 
 ## License ©️ 
 [MIT](https://opensource.org/license/mit/) license, 2024. We hereby strongly disclaim any explicit or implicit legal liability related to our works. Users are required to use this package responsibly and at their own risk. This project is a personal initiative and is not affiliated with or endorsed by Google. It is recommended to use Google's official API.
 
 
 ## References
-[1] Github: [acheong08/Bard](https://github.com/acheong08/Bard) <br>
-[2] GitHub: [HanaokaYuzu/Gemini-API](https://github.com/HanaokaYuzu/Gemini-API) <br>
-[3] Github: [dsdanielpark/Bard-API](https://github.com/dsdanielpark/Bard-API) <br>
-[4] Github: [GoogleCloudPlatform/generative-ai](https://github.com/GoogleCloudPlatform/generative-ai) <br>
-[5] Github: [OpenRouter](https://github.com/OpenRouterTeam/openrouter-runner) <br>
-[6] WebSite: [Google AI Studio](https://ai.google.dev/tutorials/ai-studio_quickstart) <br>
+[1]: Paper - [Introducing GEMINI: Multimodal Generative Models](https://arxiv.org/abs/2312.11805) <br>
+[2]: Website - [Google DeepMind :: GEMINI Introduction](https://deepmind.google/technologies/gemini/#introduction) <br>
+[3]: Paper - [GEMMA: A Unified Language Model for Text Generation, Understanding, Translation, Coding, and Math.]() <br>
+[4]: Website - [AI at Google :: GEMS Documentation](https://ai.google.dev/gemma/docs) <br>
+[5]: Report - [CodeGMMA: Large Language Models Can Write Realistic Programming Assignments](https://storage.googleapis.com/deepmind-media/gemma/codegemma_report.pdf?utm_source=substack&utm_medium=email) <br>
+[6]: Blog Post - [Announcing CodeGen: Building Better Developers’ Tools Using LLMs](https://huggingface.co/blog/codegen) <br>
+[7]: Collection - [Google :: CodeGen Release](https://huggingface.co/collections/google/codegen-release-5d0f4c4eaedbc5cefcfdcbdf) <br>
+[8]: Github - [acheong08/Bard](https://github.com/acheong08/Bard) <br>
+[9]: GitHub - [HanaokaYuzu/Gemini-API](https://github.com/HanaokaYuzu/Gemini-API) <br>
+[10]: Github - [dsdanielpark/Bard-API](https://github.com/dsdanielpark/Bard-API) <br>
+[11]: Github - [GoogleCloudPlatform/generative-ai](https://github.com/GoogleCloudPlatform/generative-ai) <br>
+[12]: Github - [OpenRouter](https://github.com/OpenRouterTeam/openrouter-runner) <br>
+[13]: WebSite - [Google AI Studio](https://ai.google.dev/tutorials/ai-studio_quickstart) <br>
 
 
 > *Warning*
 Users assume full legal responsibility for GeminiAPI. Not endorsed by Google. Excessive use may lead to account restrictions. Changes in policies or account status may affect functionality. Utilize issue and discussion pages.
 
 <br>
```

#### html2text {}

```diff
@@ -1,83 +1,94 @@
-Metadata-Version: 2.1 Name: python-gemini-api Version: 2.4.2 Summary: The
-python package that returns Response of Google Gemini through API. Home-page:
-https://github.com/dsdanielpark/Gemini-API Author: Daniel Park Author-email:
-parkminwoo1991@gmail.com Keywords: Python,API,Gemini,Google Gemini,Large
-Language Model,Chatbot API,Google API,Chatbot Classifier: Development Status ::
-2 - Pre-Alpha Classifier: Intended Audience :: Science/Research Classifier:
-Natural Language :: English Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
-Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12 Classifier: License :: OSI
-Approved :: MIT License Classifier: Topic :: Scientific/Engineering ::
-Artificial Intelligence Requires-Python: >=3.9 Description-Content-Type: text/
-markdown License-File: LICENSE Requires-Dist: httpx[http2]>=0.20.0 Requires-
-Dist: requests Requires-Dist: browser_cookie3 Requires-Dist: loguru Requires-
-Dist: pydantic Provides-Extra: voice Requires-Dist: gTTS; extra == "voice"
-Requires-Dist: SpeechRecognition; extra == "voice" Requires-Dist: openai; extra
-== "voice" Requires-Dist: anthropic; extra == "voice" # [Gemini Icon]Gemini API
-_[_P_y_P_I_]
+# [Gemini Icon]Gemini API_[_P_y_P_I_]
   _[_p_i_p_ _d_o_w_n_l_o_a_d_]_[_C_o_d_e_ _s_t_y_l_e_:_ _b_l_a_c_k_]_[_h_t_t_p_s_:_/_/_h_i_t_s_._s_e_e_y_o_u_f_a_r_m_._c_o_m_/_a_p_i_/_c_o_u_n_t_/_i_n_c_r_/
                 _b_a_d_g_e_._s_v_g_?_u_r_l_=_h_t_t_p_s_%_3_A_%_2_F_%_2_F_g_i_t_h_u_b_._c_o_m_%_2_F_d_s_d_a_n_i_e_l_p_a_r_k_%_2_F_G_e_m_i_n_i_-
 _A_P_I_&_c_o_u_n_t___b_g_=_%_2_3_0_0_0_0_0_0_&_t_i_t_l_e___b_g_=_%_2_3_5_5_5_5_5_5_&_i_c_o_n_=_&_i_c_o_n___c_o_l_o_r_=_%_2_3_E_7_E_7_E_7_&_t_i_t_l_e_=_v_i_e_w_s_&_e_d_g_e___f_l_a_t_=_f_a_l_s_e_]
                                                                     _[_D_o_w_n_l_o_a_d_s_]
 https://github.com/dsdanielpark/Gemini-API/assets/81407603/e0c11d4f-3fe1-4cbb-
 ba79-d9f89b637324 A *unofficial* Python wrapper, [python-gemini-api](https://
 pypi.org/project/python-gemini-api/), operates through reverse-engineering,
 utilizing cookie values to interact with [Google Gemini](https://
 gemini.google.com) for users struggling with frequent authentication problems
 or unable to authenticate via [Google Authentication](https://
 developers.google.com/identity/protocols/oauth2?hl=en). Collaborated
 competently with [Antonio Cheong](https://github.com/acheong08).
+
 > [!TIP] > | 2024-03-26 | [[See Code Examples]](https://github.com/
 dsdanielpark/Gemini-API/blob/main/documents/README_OPENROUTER.md) > > Check out
 temporarily free Open-source LLM APIs with Open Router. (Free limit: 10
 requests/minute)
-
-- [ Gemini API ](#-gemini-api---) - [What is Gemini?](#what-is-gemini) -
-[Installation](#installation) - [Authentication](#authentication) - [Quick
-Start](#quick-start) - [Usage](#usage) - [# 01. Initialization](#-01-
-initialization) - [# 02. Generate content](#-02-generate-content) - [# 03. Send
-request](#-03-send-request) - [# 04. Text generation](#-04-text-generation) -
-[# 05. Image generation](#-05-image-generation) - [# 06. Retrieving Images from
-Gemini Responses](#-06-retrieving-images-from-gemini-responses) - [# 07.
-Generate content from images](#-07-generate-content-from-images) - [# 08.
-Generate content using Google Services](#-08-generate-content-using-google-
-services) - [# 09. Fix context setting rcid](#-09-fix-context-setting-rcid) -
-[# 10. Changing the Selected Response from 0 to *n*](#-10-changing-the-
-selected-response-from-0-to-n) - [# 11. Generate custom content](#-11-generate-
-custom-content) - [Further](#further) - [Open-source LLM, Gemma](#open-source-
-llm-gemma) - [How to use Gemma](#how-to-use-gemma) - [Utilize free open-source
-LLM API through Open Router](#utilize-free-open-source-llm-api-through-open-
-router)
+## Contents - [ Gemini API ](#-gemini-api---) - [What is Gemini? ð](#what-
+is-gemini) - [Installation â](#installation-) - [Authentication â]
+(#authentication) - [Quick Start â](#quick-start) - [Usage](#usage) - [# 01.
+Initialization â](#-01-initialization) - [# 02. Generate content](#-02-
+generate-content) - [# 03. Send request](#-03-send-request) - [# 04. Text
+generation](#-04-text-generation) - [# 05. Image generation](#-05-image-
+generation) - [# 06. Retrieving Images from Gemini Responses](#-06-retrieving-
+images-from-gemini-responses) - [# 07. Generate content from images](#-07-
+generate-content-from-images) - [# 08. Generate content using Google Services]
+(#-08-generate-content-using-google-services) - [# 09. Fix context setting
+RCID](#-09-fix-context-setting-rcid) - [# 10. Changing the Selected Response
+from 0 to *n*](#-10-changing-the-selected-response-from-0-to-n) - [# 11.
+Generate custom content](#-11-generate-custom-content) - [Further](#further) -
+[Google Open-source LLMs](#google-open-source-llms) - [Open-source LLM, Gemma
+ð¤](#open-source-llm-gemma) - [Open-source LLM, Code Gemma ð¤](#open-
+source-llm-code-gemma) - [Utilize free open-source LLM API through Open Router
+â](#utilize-free-open-source-llm-api-through-open-router)
 ## What is [Gemini](https://deepmind.google/technologies/gemini/#introduction)?
 | [Paper](https://arxiv.org/abs/2312.11805) | [Official Website](https://
 deepmind.google/technologies/gemini/#introduction) | [Official API](https://
 aistudio.google.com/) | [API Documents](https://cloud.google.com/vertex-ai/
 docs/generative-ai/model-reference/gemini) | Gemini is a family of generative
 AI models developed by Google DeepMind that is designed for multimodal use
 cases. The Gemini API gives you access to the Gemini Pro and Gemini Pro Vision
 models. In February 2024, Google's **Bard** service was changed to **Gemini**.
-## Installation ð¦ ``` pip install python-gemini-api ``` ``` pip install
-git+https://github.com/dsdanielpark/Gemini-API.git ``` For the updated version,
-use as follows: ``` pip install -q -U python-gemini-api ``` ## Authentication >
-[!NOTE] > Cookies can change quickly. Don't reopen the same session or repeat
-prompts too often; they'll expire faster. If the cookie value doesn't export
-correctly, refresh the Gemini page and export again. 1. Visit https://
+#### Overview of Google LLMs | Model | Type | Access | Details |:-------:|:----
+--:|:--------:|--------- [Gemini](https://huggingface.co/google/gemma-7b) |
+Proprietary | API [[13](https://ai.google.dev/tutorials/ai-studio_quickstart)]
+| A proprietary multimodal AI by Google DeepMind, including advanced models
+such as Gemini Pro and Gemini Pro Vision. Access is restricted to API usage;
+additional insights may be obtained through the paper and website. [[1](https:/
+/arxiv.org/abs/2312.11805)][[2](https://deepmind.google/technologies/gemini/
+#introduction)] [Gemma](https://huggingface.co/google/gemma-7b) | Open Source |
+[Downloadable](https://huggingface.co/google/gemma-7b)
+[Free API](https://github.com/dsdanielpark/Gemini-API?tab=readme-ov-
+file#utilize-free-open-source-llm-api-through-open-router) | An open-source
+text-to-text language model suitable for tasks like QA and summarization.
+Weights are downloadable for on-premises use, and detailed documentation is
+provided via the paper and website. [[3](https://arxiv.org/abs/2403.08295)][[4]
+(https://ai.google.dev/gemma/docs)] [Code Gemma](https://huggingface.co/google/
+codegemma-7b-it) | Open Source | [Downloadable](https://huggingface.co/google/
+codegemma-7b-it) | Designed specifically for programming tasks, this open-
+source model offers downloadable weights to assist developers with code
+generation and similar activities. Refer to the associated paper, blog post,
+and Hugging Face collection for more information. [[5](https://
+storage.googleapis.com/deepmind-media/gemma/
+codegemma_report.pdf?utm_source=substack&utm_medium=email)][[6](https://
+huggingface.co/blog/codegemma)][[7](https://huggingface.co/collections/google/
+codegemma-release-66152ac7b683e2667abdee11)]
+## What is [Python-Gemini-API](https://github.com/dsdanielpark/Gemini-API)?
+This is a Python wrapper derived from the [Bard API](https://github.com/
+dsdanielpark/Bard-API) project, designed to retrieve responses from Gemini Web
+in REST format. **Synchronous clients are preferred over asynchronous ones for
+Gemini because of rate limiting and blocking concerns.** ## Installation ð¦
+``` pip install python-gemini-api ``` ``` pip install git+https://github.com/
+dsdanielpark/Gemini-API.git ``` For the updated version, use as follows: ```
+pip install -q -U python-gemini-api ``` ## Authentication 1. Visit https://
 gemini.google.com/
 With browser open, try auto-collecting cookies first. ```python from gemini
 import Gemini GeminiClient = Gemini(auto_cookies=True) # Testing needed as
 cookies vary by region. # GeminiClient = Gemini(auto_cookies=True,
-target_cookies=["__Secure-1PSID", "__Secure-1PSIDTS"]) response =
-GeminiClient.generate_content("Hello, Gemini. What's the weather like in Seoul
-today?") print(response.payload) ``` 2. *(Manually)* `F12` for browser console
-â `Session: Application` â `Cookies` â Copy the value of some working
-cookie sets. If it doesn't work, go to step 3. Some working cookie sets Cookies
-may vary by account or region. First try `__Secure-1PSIDCC` alone. If it
-doesn't work, use `__Secure-1PSID` and `__Secure-1PSIDTS`. Still no success?
+target_cookies=["__Secure-1PSID", "__Secure-1PSIDTS"]) # GeminiClient = Gemini
+(auto_cookies=True, target_cookies="all") # You can pass whole cookies response
+= GeminiClient.generate_content("Hello, Gemini. What's the weather like in
+Seoul today?") print(response.payload) ``` 2. *(Manually)* `F12` for browser
+console â `Session: Application` â `Cookies` â Copy the value of some
+working cookie sets. If it doesn't work, go to step 3. Some working cookie sets
+Cookies may vary by account or region. First try `__Secure-1PSIDCC` alone. If
+it doesn't work, use `__Secure-1PSID` and `__Secure-1PSIDTS`. Still no success?
 Try these four cookies: `__Secure-1PSIDCC`, `__Secure-1PSID`, `__Secure-
 1PSIDTS`, `NID`. If none work, proceed to step 3 and consider sending the
 entire cookie file. 3. *(Recommended)* Export Gemini site cookies via a browser
 extension. For instance, use Chrome extension [ExportThisCookies](https://
 chromewebstore.google.com/detail/exportthiscookie/
 dannllckdimllhkiplchkcaoheibealk), open, and copy the txt file contents.
 Further: For manual collection or Required for a few users upon error 4. For
@@ -89,113 +100,104 @@
 few users upon error)* If errors persist after manually collecting cookies,
 refresh the Gemini website and collect cookies again. If errors continue, some
 users may need to manually set the nonce value. To do this: Press F12 â
 Network â Send any prompt to Gemini webui â Click the post address starting
 with "https://gemini.google.com/_/BardChatUi/data/
 assistant.lamda.BardFrontendService/StreamGenerate" â Payload â Form Data
 â Copy the "at" key value. See [this image](assets/nonce_value.pdf) for
-reference. > [!IMPORTANT] > Try different Google accounts until you find a
-working cookie. Use a fresh browser to ensure no remaining cookie values. Use
-secret browsing mode with independent cookies. Results may vary depending on
-factors like IP and account status. Providing the entire set of cookies seems
-to fix one cookie per account. Additionally, once successfully connected with
-that cookie, it seems to work flawlessly for over three weeks without any
-errors. *Try various methods until you succeed. Experiment in different
-environments.*
-## Quick Start *Simple usage* Setting Gemini response language (Optional):
-Check supported languages [here](https://developers.google.com/hotels/hotel-
-prices/dev-guide/country-codes). Default is English. ```python import os
-os.environ["GEMINI_LANGUAGE"] = "KR" ``` Generate content: returns parsed
-response. ```python from gemini import Gemini cookies = {} # Cookies may vary
-by account or region. Consider sending the entire cookie file. GeminiClient =
-Gemini(cookies=cookies) # You can use various args response =
-GeminiClient.generate_content("Hello, Gemini. What's the weather like in Seoul
-today?") response.payload ``` Generate content from image: you can use image as
-input. ```python from gemini import Gemini cookies = {} # Cookies may vary by
-account or region. Consider sending the entire cookie file. GeminiClient =
-Gemini(cookies=cookies) # You can use various args response =
-GeminiClient.generate_content("What does the text in this image say?",
-image='folder/image.jpg') response.payload ``` > [!NOTE] > If the
-generate_content method returns an empty payload, try executing it again
-without reinitializing the Gemini object.
-## Usage ### # 01. Initialization Please explicitly declare `cookies` in dict
-format. You can also enter the path to the file containing the cookie with
-`cookie_fp`(*.json, *.txt supported). Check this [sample cookie file](https://
-github.com/dsdanielpark/Gemini-API/blob/main/cookies.txt). ```python from
+reference. > [!IMPORTANT] > Experiment with different Google accounts and
+browser settings to find a working cookie. Success may vary by IP and account
+status. Once connected, a cookie typically remains effective over a month. Keep
+testing until successful.
+## Quick Start **Generate content:** returns parsed response. ```python from
+gemini import Gemini cookies = {} # Cookies may vary by account or region.
+Consider sending the entire cookie file. GeminiClient = Gemini(cookies=cookies)
+# You can use various args response = GeminiClient.generate_content("Hello,
+Gemini. What's the weather like in Seoul today?") response.payload ```
+**Generate content from image:** you can use image as input. ```python from
+gemini import Gemini cookies = {} # Cookies may vary by account or region.
+Consider sending the entire cookie file. GeminiClient = Gemini(cookies=cookies)
+# You can use various args response = GeminiClient.generate_content("What does
+the text in this image say?", image='folder/image.jpg') response.payload ``` >
+[!NOTE] > If the generate_content method returns an empty payload, try
+executing it again without reinitializing the Gemini object.
+
+## Usage *Setting language and Gemini version using environment variables:
+* Setting Gemini response language (Optional): Check supported languages [here]
+(https://developers.google.com/hotels/hotel-prices/dev-guide/country-codes).
+Default is English. ```python import os os.environ["GEMINI_LANGUAGE"] = "KR" #
+Setting Gemini response language (Optional) os.environ["GEMINI_ULTRA"] = "1" #
+Switch to Gemini-advanced response (Experimental, Optional) # In some accounts,
+access to Gemini Ultra may not be available. If that's the case, please revert
+it back to "0". ```
+### # 01. Initialization Please explicitly declare `cookies` in dict format.
+You can also enter the path to the file containing the cookie with `cookie_fp`
+(*.json, *.txt supported). Check sample cookie files in [assets](https://
+github.com/dsdanielpark/Gemini-API/tree/main/assets) folder. ```python from
 gemini import Gemini cookies = { "__Secure-1PSIDCC" : "value", "__Secure-1PSID"
 : "value", "__Secure-1PSIDTS" : "value", "NID" : "value", # Cookies may vary by
 account or region. Consider sending the entire cookie file. } GeminiClient =
 Gemini(cookies=cookies) # GeminiClient = Gemini(cookie_fp="folder/
 cookie_file.json") # (*.json, *.txt) are supported. # GeminiClient = Gemini
-(auto_cookies=True) # Or use auto_cookies paprameter ``` #### Auto Cookie
-Update For `auto_cookie` to be set to `True`, Gemini WebUI must be active in
-the browser. The [browser_cookie3](https://github.com/borisbabic/
-browser_cookie3) enables automatic cookie collection, though updates may not be
-complete yet. > [!IMPORTANT] > **If the session connects successfully and
-`generate_content` runs well, CLOSE Gemini website.** If Gemini web stays open
-in the browser, cookies may expire faster.
+(auto_cookies=True) # Or use auto_cookies paprameter ``` ##### Auto Cookie
+Update For `auto_cookie` to be set to `True`, and adjust `target_cookies`.
+Gemini WebUI must be active in the browser. The [browser_cookie3](https://
+github.com/borisbabic/browser_cookie3) enables automatic cookie collection,
+though updates may not be complete yet.
 ### # 02. Generate content Returns Gemini's response, but the first one might
-be empty. If generate_content yields an empty payload, rerun it without
-reinitializing Gemini. Regardless of model output type, access the
-response_dict property (renamed to payload after v2.3.0). https://github.com/
-dsdanielpark/Gemini-API/blob/fdf064c57bc1fb47fbbb4b93067618a200e77f62/gemini/
-core.py#L252 ```python prompt = "Hello, Gemini. What's the weather like in
-Seoul today?" response = GeminiClient.generate_content(prompt) print
-(response.payload) ``` > [!IMPORTANT] > Once connected and generating valid
-content, **Be sure to CLOSE the Gemini website or CLOSE your browser** for
-cookie stability.
+be empty. ```python prompt = "Hello, Gemini. What's the weather like in Seoul
+today?" response = GeminiClient.generate_content(prompt) print
+(response.payload) ``` > [!IMPORTANT] > DO NOT send same prompt repeatly. **If
+the session connects successfully and `generate_content` runs well, CLOSE
+Gemini website.** If Gemini web stays open in the browser, cookies may expire
+faster.
 The output of the generate_content function is `GeminiModelOutput`, with the
-following structure: **Properties of GeminiModelOutput:** - *rcid*: returns the
-response candidate id of the chosen candidate. - *text*: returns the text of
-the chosen candidate. - *code*: returns the codes of the chosen candidate. -
-*web_images*: returns a list of web images from the chosen candidate. -
-*generated_images*: returns a list of generated images from the chosen
-candidate. - *payload*: returns the response dictionary, if available. (same as
-*reponse_dict* under v2.3.0) https://github.com/dsdanielpark/Gemini-API/blob/
-fdf064c57bc1fb47fbbb4b93067618a200e77f62/gemini/src/model/output.py#L16 >
-[!NOTE] > If the session fails to connect, works improperly, or terminates,
-returning an error, it is recommended to manually renew the cookies. The error
-is likely due to incorrect cookie values. Refresh or log out of Gemini web to
-renew cookies and try again.
+following structure: - *rcid*: returns the response candidate id of the chosen
+candidate. - *text*: returns the text of the chosen candidate. - *code*:
+returns the codes of the chosen candidate. - *web_images*: returns a list of
+web images from the chosen candidate. - *generated_images*: returns a list of
+generated images from the chosen candidate. - *payload*: returns the response
+dictionary, if available. https://github.com/dsdanielpark/Gemini-API/blob/
+fdf064c57bc1fb47fbbb4b93067618a200e77f62/gemini/src/model/output.py#L16
 ### # 03. Send request Send request: returns the request's payload and
 status_code, making debugging easier. ```python from gemini import Gemini
 cookies = {} # Cookies may vary by account or region. Consider sending the
 entire cookie file. GeminiClient = Gemini(cookies=cookies) # You can use
 various args response_text, response_status = GeminiClient.send_request("Hello,
-Gemini. What's the weather like in Seoul today?") print(response_text) ```
+Gemini. What's the weather like in Seoul today?") print(response_text) ``` You
+can track the total number of requests made by accessing the `request_count`
+property within the `Gemini` class.
 ### # 04. Text generation Returns text generated by Gemini. ```python prompt =
 "Hello, Gemini. What's the weather like in Seoul today?" response =
 GeminiClient.generate_content(prompt) print(response.text) ```
-### # 05. Image generation Returns images generated by Gemini. https://
-github.com/dsdanielpark/Gemini-API/blob/
-fdf064c57bc1fb47fbbb4b93067618a200e77f62/gemini/src/model/image.py#L12 *Sync
-downloader* ```python from gemini import Gemini, GeminiImage response =
-GeminiClient.generate_content("Create illustrations of Seoul, South Korea.")
-generated_images = response.generated_images # Check generated images [Dict]
-GeminiImage.save_sync(generated_images, save_path="save_dir", cookies=cookies)
-# You can use byte type image dict for printing images as follow: #
-bytes_images_dict = GeminiImage.fetch_images_dict_sync(generated_images,
-cookies=cookies) # Get bytes images dict # GeminiImage.save_images_sync
-(bytes_images_dict, path="save_dir", cookies=cookies) # Save to path ```
-Display images in IPython You can display the image or transmit it to another
-application in byte format. ``` bytes_images_dict =
+### # 05. Image generation Returns images generated by Gemini. *Async
+downloader* ```python response = GeminiClient.generate_content("Create
+illustrations of Seoul, South Korea.") generated_images =
+response.generated_images # Check generated images [Dict] await
+GeminiImage.save(generated_images, "save_dir", cookies=cookies) #
+image_data_dict = await GeminiImage.fetch_images_dict(generated_images,
+cookies=cookies) # await GeminiImage.save_images(image_data_dict, "save_dir")
+``` Further *Display images in IPython* You can display the image or transmit
+it to another application in byte format. ```python bytes_images_dict =
 GeminiImage.fetch_images_dict_sync(generated_images, cookies) # Get bytes
 images dict from IPython.display import display, Image import io for
 image_name, image_bytes in bytes_images_dict.items(): print(image_name) image =
-Image(data=image_bytes) display(image) ``` *Async downloader* ```python
-response = GeminiClient.generate_content("Create illustrations of Seoul, South
-Korea.") generated_images = response.generated_images # Check generated images
-[Dict] await GeminiImage.save(generated_images, "save_dir", cookies=cookies) #
-image_data_dict = await GeminiImage.fetch_images_dict(generated_images,
-cookies=cookies) # await GeminiImage.save_images(image_data_dict, "save_dir")
-``` Async downloader wrapper ``` import asyncio from gemini import Gemini,
-GeminiImage async def save_generated_imagse(generated_imagse,
-save_path="save_dir", cookies=cookies): await GeminiImage.save
-(generated_imagse, save_path=save_path, cookies=cookies) # Run the async
-function if __name__ == "__main__": cookies = {"key" : "value"}
+Image(data=image_bytes) display(image) ``` *Sync downloader* ```python from
+gemini import Gemini, GeminiImage response = GeminiClient.generate_content
+("Create illustrations of Seoul, South Korea.") generated_images =
+response.generated_images # Check generated images [Dict] GeminiImage.save_sync
+(generated_images, save_path="save_dir", cookies=cookies) # You can use byte
+type image dict for printing images as follow: # bytes_images_dict =
+GeminiImage.fetch_images_dict_sync(generated_images, cookies=cookies) # Get
+bytes images dict # GeminiImage.save_images_sync(bytes_images_dict,
+path="save_dir", cookies=cookies) # Save to path ``` *Async downloader wrapper*
+```python import asyncio from gemini import Gemini, GeminiImage async def
+save_generated_imagse(generated_imagse, save_path="save_dir", cookies=cookies):
+await GeminiImage.save(generated_imagse, save_path=save_path, cookies=cookies)
+# Run the async function if __name__ == "__main__": cookies = {"key" : "value"}
 generated_imagse = response.generated_imagse asyncio.run(save_generated_imagse
 (generated_imagse, save_path="save_dir", cookies=cookies)) ```
 `GeminiImage.save` method logic ``` import asyncio from gemini import Gemini,
 GeminiImage async def save_generated_imagse(generated_imagse,
 save_path="save_dir", cookies=cookies): image_data_dict = await
 GeminiImage.fetch_images_dict(generated_imagse, cookies=cookies) # Get bytes
 images dict asynchronously await GeminiImage.save_images(image_data_dict,
@@ -204,38 +206,38 @@
 Check response images [Dict] asyncio.run(save_generated_imagse
 (generated_imagse, save_path="save_dir", cookies=cookies)) ``` > [!NOTE] > Use
 GeminiImage for image processing. `web_images` works without cookies, but for
 images like `generated_image` from Gemini, pass cookies. Cookies are needed to
 download images from Google's storage. Check the response or use existing
 cookies variable.
 ### # 06. Retrieving Images from Gemini Responses Returns images in response of
-Gemini. *Sync downloader* ```python from gemini import Gemini, GeminiImage
-response = GeminiClient.generate_content("Please recommend a travel itinerary
-for Seoul.") response_images = response.web_images # Check response images
-[Dict] GeminiImage.save_sync(response_images, save_path="save_dir") # You can
-use byte type image dict as follow: # bytes_images_dict =
-GeminiImage.fetch_bytes_sync(response_images, cookies) # Get bytes images dict
-# GeminiImage.save_images_sync(bytes_images_dict, path="save_dir") # Save to
-path ``` *Async downloader* ```python response = GeminiClient.generate_content
+Gemini. *Async downloader* ```python response = GeminiClient.generate_content
 ("Create illustrations of Seoul, South Korea.") response_images =
 response.web_images # Check generated images [Dict] await GeminiImage.save
 (response_images, "save_dir") # image_data_dict = await
 GeminiImage.fetch_images_dict(response_images) # await GeminiImage.save_images
-(image_data_dict, "save_dir") ``` Async downloader wrapper ``` import asyncio
-from gemini import Gemini, GeminiImage async def save_response_web_imagse
-(response_images, save_path="save_dir", cookies=cookies): await
-GeminiImage.save(response_images, save_path=save_path, cookies=cookies) # Run
-the async function if __name__ == "__main__": cookies = {"key" : "value"}
-response_images = response.web_images asyncio.run(save_response_web_imagse
-(response_images, save_path="save_dir", cookies=cookies)) ```
-`GeminiImage.save` method logic ``` import asyncio from gemini import Gemini,
-GeminiImage async def save_response_web_imagse(response_images,
-save_path="save_dir", cookies=cookies): image_data_dict = await
-GeminiImage.fetch_images_dict(response_images, cookies=cookies) # Get bytes
-images dict asynchronously await GeminiImage.save_images(image_data_dict,
+(image_data_dict, "save_dir") ``` Further *Sync downloader* ```python from
+gemini import Gemini, GeminiImage response = GeminiClient.generate_content
+("Please recommend a travel itinerary for Seoul.") response_images =
+response.web_images # Check response images [Dict] GeminiImage.save_sync
+(response_images, save_path="save_dir") # You can use byte type image dict as
+follow: # bytes_images_dict = GeminiImage.fetch_bytes_sync(response_images,
+cookies) # Get bytes images dict # GeminiImage.save_images_sync
+(bytes_images_dict, path="save_dir") # Save to path ``` *Async downloader
+wrapper* ```python import asyncio from gemini import Gemini, GeminiImage async
+def save_response_web_imagse(response_images, save_path="save_dir",
+cookies=cookies): await GeminiImage.save(response_images, save_path=save_path,
+cookies=cookies) # Run the async function if __name__ == "__main__": cookies =
+{"key" : "value"} response_images = response.web_images asyncio.run
+(save_response_web_imagse(response_images, save_path="save_dir",
+cookies=cookies)) ``` `GeminiImage.save` method logic ``` import asyncio from
+gemini import Gemini, GeminiImage async def save_response_web_imagse
+(response_images, save_path="save_dir", cookies=cookies): image_data_dict =
+await GeminiImage.fetch_images_dict(response_images, cookies=cookies) # Get
+bytes images dict asynchronously await GeminiImage.save_images(image_data_dict,
 save_path=save_path) # Run the async function if __name__ == "__main__":
 response_images = response.web_images # Check response images [Dict]
 asyncio.run(save_response_web_imagse(response_images, save_path="save_dir",
 cookies=cookies)) ```
 ### # 07. Generate content from images Takes an image as input and returns a
 response. ```python image = 'folder/image.jpg' # image = open('folder/
 image.jpg', 'rb').read() # (jpg, jpeg, png, webp) are supported. response =
@@ -261,93 +263,111 @@
 tailored travel itineraries. - Features: Holiday preparation, price comparison,
 trip planning - Google Hotels - Service: **@Google Hotels** - Description:
 Search for hotels considering what matters most to you, like having a
 conversation with a friend. - Features: Packing for travel, sightseeing,
 special relaxation - YouTube - Service: **@YouTube** - Description: Explore
 YouTube videos and ask questions about what interests you. - Features: Problem-
 solving, generating ideas, search, exploring topics
-### # 09. Fix context setting rcid You can specify a particular response by
-setting its response candidate id(rcid). ```python # Generate content for the
+### # 09. Fix context setting RCID You can specify a particular response by
+setting its Response Candidate ID(RCID). ```python # Generate content for the
 prompt "Give me some information about the USA." response1 =
 GeminiClient.generate_content("Give me some information about the USA.") #
 After reviewing the responses, choose the one you prefer and copy its RCID.
 GeminiClient.rcid = "rc_xxxx" # Now, generate content for the next prompt "How
 long does it take from LA to New York?" response2 =
-GeminiClient.generate_content("How long does it take from LA to New York?") ```
-
+GeminiClient.generate_content("How long does it take from LA to New York?") #
+However, RCID may not persist. If parsing fails, reset `GeminiClient.rcid` to
+None. # GeminiClient.rcid = None ```
 ### # 10. Changing the Selected Response from 0 to *n* In Gemini,
 generate_content returns the first response. This may vary depending on length
 or sorting. Therefore, you can specify the index of the chosen response from 0
 to *n* as follows. However, if there is only one response, revert it back to 0.
 ```python from gemini import GeminiModelOutput GeminiModelOutput.chosen = 1 #
-default is 0 response1 = GeminiClient.generate_content("Give me some
-information about the USA.") ```
+default is 0 response_choice_1 = GeminiClient.generate_content("Give me some
+information about the USA.") # If not all Gemini returns are necessarily
+plural, revert back to 0 in case of errors. # GeminiModelOutput.chosen = 0 ```
 ### # 11. Generate custom content Parse the response text to extract desired
-values. https://github.com/dsdanielpark/Gemini-API/blob/
-fdf064c57bc1fb47fbbb4b93067618a200e77f62/gemini/core.py#L317 Using
-`Gemini.generate_custom_content`, specify custom parsing to extract specific
-values. Utilize ParseMethod1 and ParseMethod2 by default, and you can pass
-custom parsing methods as arguments if desired. Refer to [custom_parser.py]
-(https://github.com/dsdanielpark/Gemini-API/blob/main/gemini/src/model/parser/
-custom_parser.py). ```python # You can create a parser method that takes
-response_text as the input for custom_parser. response_text, response_status =
-GeminiClient.send_request("Give me some information about the USA.") # Use
-custom_parser function or class inheriting from BaseParser response =
-GeminiClient.generate_custom_content("Give me some information about the USA.",
-*custom_parser) ```
-## Further ### Use rotating proxies If you want to **avoid blocked requests**
-and bans, then use [Smart Proxy by Crawlbase](https://crawlbase.com/docs/smart-
-proxy/?utm_source=github_ad&utm_medium=social&utm_campaign=bard_api). It
-forwards your connection requests to a **randomly rotating IP address** in a
-pool of proxies before reaching the target website. The combination of AI and
-ML make it more effective to avoid CAPTCHAs and blocks. ```python # Get your
-proxy url at crawlbase https://crawlbase.com/docs/smart-proxy/get/ proxy_url =
-"http://xxxxx:@smartproxy.crawlbase.com:8012" proxies = {"http": proxy_url,
-"https": proxy_url} GeminiClient = Gemini(cookies=cookies, proxies=proxies,
-timeout=30) GeminiClient.generate_content("Hello, Gemini. Give me a beautiful
-photo of Seoul's scenery.") ``` ### Reusable session object For standard cases,
-use Gemini class; for exceptions, use session objects. When creating a new bot
-Gemini server, adjust Headers.MAIN. ```python from gemini import Gemini,
-Headers import requests cookies = {} session = requests.Session()
+values. Using `Gemini.generate_custom_content`, specify custom parsing to
+extract specific values. Utilize ParseMethod1 and ParseMethod2 by default, and
+you can pass custom parsing methods as arguments if desired. Refer to
+[custom_parser.py](https://github.com/dsdanielpark/Gemini-API/blob/main/gemini/
+src/model/parser/custom_parser.py). ```python # You can create a parser method
+that takes response_text as the input for custom_parser. response_text,
+response_status = GeminiClient.send_request("Give me some information about the
+USA.") # Use custom_parser function or class inheriting from BaseParser
+response = GeminiClient.generate_custom_content("Give me some information about
+the USA.", *custom_parser) ``` https://github.com/dsdanielpark/Gemini-API/blob/
+31b842488bbc5429ad9c74b1d8b00e20d94e8cb1/gemini/client.py#L323
+## Further ### Use rotating proxies via [Smart Proxy by Crawlbase](https://
+crawlbase.com/docs/smart-proxy/
+?utm_source=github_ad&utm_medium=social&utm_campaign=bard_api) If you want to
+**avoid blocked requests** and bans, then use [Smart Proxy by Crawlbase](https:
+//crawlbase.com/docs/smart-proxy/
+?utm_source=github_ad&utm_medium=social&utm_campaign=bard_api). It forwards
+your connection requests to a **randomly rotating IP address** in a pool of
+proxies before reaching the target website. The combination of AI and ML make
+it more effective to avoid CAPTCHAs and blocks. ```python # Get your proxy url
+at crawlbase https://crawlbase.com/docs/smart-proxy/get/ proxy_url = "http://
+xxxxx:@smartproxy.crawlbase.com:8012" proxies = {"http": proxy_url, "https":
+proxy_url} GeminiClient = Gemini(cookies=cookies, proxies=proxies, timeout=30)
+GeminiClient.generate_content("Hello, Gemini. Give me a beautiful photo of
+Seoul's scenery.") ``` ### Reusable session object For standard cases, use
+Gemini class; for exceptions, use session objects. When creating a new bot
+Gemini server, adjust Headers.MAIN. ```python import requests from gemini
+import Gemini, Headers cookies = {} session = requests.Session()
 session.headers = Headers.MAIN for key, value in cookies.items():
 session.cookies.update({key: value}) GeminiClient = Gemini(session=session) #
 You can use various args response = GeminiClient.generate_content("Hello,
 Gemini. What's the weather like in Seoul today?") ```
 ## [More features](https://github.com/dsdanielpark/Gemini-API/blob/main/
 documents/README_DEV.md) Explore additional features in [this document](https:/
 /github.com/dsdanielpark/Gemini-API/blob/main/documents/README_DEV.md). If you
 want to develop your own simple code, you can start from [this simple code
 example](https://github.com/dsdanielpark/Gemini-API/blob/main/script/
 sample.ipynb).
-## Open-source LLM, [Gemma](https://huggingface.co/google/gemma-7b) If you have
-sufficient GPU resources, you can download weights directly instead of using
-the Gemini API to generate content. Consider Gemma, an open-source model
-**available for on-premises use**. [Gemma](https://huggingface.co/google/gemma-
-7b) models are Google's lightweight, advanced text-to-text, decoder-only
-language models, derived from Gemini research. Available in English, they offer
-open weights and variants, ideal for tasks like question answering and
-summarization. Their small size enables deployment in resource-limited
-settings, broadening access to cutting-edge AI. For more infomation, visit
-[Gemma-7b](https://huggingface.co/google/gemma-7b) model card. ### How to use
-Gemma ```python from transformers import AutoTokenizer, AutoModelForCausalLM
-tokenizer = AutoTokenizer.from_pretrained("google/gemma-7b") model =
+## Google Open-source LLMs If you have sufficient GPU resources, you can
+download weights directly instead of using the Gemini API to generate content.
+Consider Gemma and Code Gemma, an open-source models **available for on-
+premises use**. ### Open-source LLM, [Gemma](https://huggingface.co/google/
+gemma-7b) Gemma models are Google's lightweight, advanced text-to-text,
+decoder-only language models, derived from Gemini research. Available in
+English, they offer open weights and variants, ideal for tasks like question
+answering and summarization. For more infomation, visit [Gemma-7b](https://
+huggingface.co/google/gemma-7b) model card. #### How to use Gemma ```python
+from transformers import AutoTokenizer, AutoModelForCausalLM tokenizer =
+AutoTokenizer.from_pretrained("google/gemma-7b") model =
 AutoModelForCausalLM.from_pretrained("google/gemma-7b") input_text = "Write me
 a poem about Machine Learning." input_ids = tokenizer(input_text,
 return_tensors="pt") outputs = model.generate(**input_ids) print
+(tokenizer.decode(outputs[0])) ``` ### Open-source LLM, [Code Gemma](https://
+huggingface.co/collections/google/codegemma-release-66152ac7b683e2667abdee11)
+CodeGemma, which is an official release from Google for code LLMs, was released
+on April 9, 2024. It provides three models specifically designed for generating
+and interacting with code. You can explore the [Code Gemma models](https://
+huggingface.co/collections/google/codegemma-release-66152ac7b683e2667abdee11)
+and view the [model card](https://huggingface.co/google/codegemma-7b-it) for
+more details. #### How to use Code Gemma ```python from transformers import
+GemmaTokenizer, AutoModelForCausalLM tokenizer = GemmaTokenizer.from_pretrained
+("google/codegemma-7b-it") model = AutoModelForCausalLM.from_pretrained
+("google/codegemma-7b-it") input_text = "Write me a Python function to
+calculate the nth fibonacci number." input_ids = tokenizer(input_text,
+return_tensors="pt") outputs = model.generate(**input_ids) print
 (tokenizer.decode(outputs[0])) ```
 ## Utilize free open-source LLM API through [Open Router](https://
 openrouter.ai/) OpenRouter offers temporary free inference for select models.
 Obtain an API key from [Open Router API](https://openrouter.ai/keys) and check
 free models at [Open Router models](https://openrouter.ai/docs#models). Use
 models with a 0-dollar token cost primarily; other models may incur charges.
-See more [free open-source LLM API guide](https://github.com/dsdanielpark/
-Gemini-API/blob/main/documents/README_OPENROUTER.md) > [!NOTE] > You can easily
-receive responses from open LLMs without this package by following the
-instructions on [here](https://openrouter.ai/docs#models). ```python from
-gemini import OpenRouter OPENROUTER_API_KEY = "" GemmaClient = OpenRouter
+See more at [free open-source LLM API guide](https://github.com/dsdanielpark/
+Gemini-API/blob/main/documents/README_OPENROUTER.md). **Sync client is favored
+over async for Gemini due to rate limiting and blocking issues**, but
+OpenRouter offers reliable open-source LLMs for [async implementation](https://
+github.com/dsdanielpark/Gemini-API/blob/main/documents/
+README_OPENROUTER.md#openrouter-async-api-client). ```python from gemini import
+OpenRouter OPENROUTER_API_KEY = "" GemmaClient = OpenRouter
 (api_key=OPENROUTER_API_KEY, model="google/gemma-7b-it:free") prompt = "Do you
 know UCA academy in Korea? https://blog.naver.com/ulsancoding" response =
 GemmaClient.create_chat_completion(prompt) print(response) # payload =
 GemmaClient.generate_content(prompt) # print(payload.json()) ``` The free model
 list includes: - `google/gemma-7b-it:free` - [google/gemma-7b](https://
 huggingface.co/google/gemma-7b) from Google *** - `mistralai/mistral-7b-
 instruct:free` - [mistralai/Mistral-7B-Instruct-v0.1](https://huggingface.co/
@@ -358,38 +378,38 @@
 `openrouter/cinematika-7b:free` - [jondurbin/cinematika-7b-v0.1](https://
 huggingface.co/jondurbin/cinematika-7b-v0.1) - `undi95/toppy-m-7b:free` -
 [Undi95/Toppy-M-7B](https://huggingface.co/Undi95/Toppy-M-7B?not-for-all-
 audiences=true) - `gryphe/mythomist-7b:free` - [Gryphe/MythoMist-7b](https://
 huggingface.co/Gryphe/MythoMist-7b) - `nousresearch/nous-capybara-7b:free` -
 [NousResearch/Nous-Capybara-7B-V1](https://huggingface.co/NousResearch/Nous-
 Capybara-7B-V1) from Nous Research
+## Sponsor, [Crawlbase](https://crawlbase.com/) Use [Crawlbase](https://
+crawlbase.com/) API for efficient data scraping to train AI models, boasting a
+98% success rate and 99.9% uptime. It's quick to start, GDPR/CCPA compliant,
+supports massive data extraction, and is trusted by 70k+ developers.
 ## [FAQ](https://github.com/dsdanielpark/Gemini-API/blob/main/documents/
 README_FAQ.md) First review [HanaokaYuzu/Gemini-API](https://github.com/
 HanaokaYuzu/Gemini-API) and the [Official Google Gemini API](https://
 aistudio.google.com/) before using this package. You can find most help on the
 [FAQ](https://github.com/dsdanielpark/Gemini-API/blob/main/documents/
 README_FAQ.md) and [Issue](https://github.com/dsdanielpark/Gemini-API/issues)
 pages. ## [Issues](https://github.com/dsdanielpark/Gemini-API/issues) Sincerely
 grateful for any reports on new features or bugs. Your valuable feedback on the
 code is highly appreciated. Frequent errors may occur due to changes in
 Google's service API interface. Both [Issue reports](https://github.com/
 dsdanielpark/Gemini-API/issues) and [Pull requests](https://github.com/
 dsdanielpark/Gemini-API/pulls) contributing to improvements are always welcome.
-We strive to maintain an active and courteous open community. ## Sponsor Use
-[Crawlbase](https://crawlbase.com/) API for efficient data scraping to train AI
-models, boasting a 98% success rate and 99.9% uptime. It's quick to start,
-GDPR/CCPA compliant, supports massive data extraction, and is trusted by 70k+
-developers. ## Contributors We would like to express our sincere gratitude to
-all the contributors. This package aims to re-implement the functionality of
-the [Bard API](https://github.com/dsdanielpark/Bard-API/), which has been
-archived for the contributions of the beloved open-source community, despite
-Gemini's official API already being available. Contributors to the [Bard API]
-(https://github.com/dsdanielpark/Bard-API/) and [Gemini API](https://
-github.com/dsdanielpark/Gemini-API/). _[_h_t_t_p_s_:_/_/_c_o_n_t_r_i_b_._r_o_c_k_s_/
-_i_m_a_g_e_?_r_e_p_o_=_d_s_d_a_n_i_e_l_p_a_r_k_/_B_a_r_d___A_P_I_]
+We strive to maintain an active and courteous open community. ## Contributors
+We would like to express our sincere gratitude to all the contributors. This
+package aims to re-implement the functionality of the [Bard API](https://
+github.com/dsdanielpark/Bard-API/), which has been archived for the
+contributions of the beloved open-source community, despite Gemini's official
+API already being available. Contributors to the [Bard API](https://github.com/
+dsdanielpark/Bard-API/) and [Gemini API](https://github.com/dsdanielpark/
+Gemini-API/). _[_h_t_t_p_s_:_/_/_c_o_n_t_r_i_b_._r_o_c_k_s_/_i_m_a_g_e_?_r_e_p_o_=_d_s_d_a_n_i_e_l_p_a_r_k_/_B_a_r_d___A_P_I_]
 Further development potential Modifications to the async client using my logic
 are needed, along with automatic cookie collection via browser_cookie3, and
 implementation of other Bard API features (such as code extraction, export to
 Replit, graph drawing, etc.). Please note that while reviewing automatic cookie
 collection, it appears that cookies expire immediately upon sending a request
 for collection. Efforts to make it more user-friendly were unsuccessful. Also,
 the _sid value seems to work normally even when returned as None. Lastly, if
@@ -401,21 +421,38 @@
 Cheong](https://github.com/acheong08) / teapotv8@proton.me
 - [Daniel Park](https://github.com/DSDanielPark) / parkminwoo1991@gmail.com ##
 License Â©ï¸ [MIT](https://opensource.org/license/mit/) license, 2024. We
 hereby strongly disclaim any explicit or implicit legal liability related to
 our works. Users are required to use this package responsibly and at their own
 risk. This project is a personal initiative and is not affiliated with or
 endorsed by Google. It is recommended to use Google's official API. ##
-References [1] Github: [acheong08/Bard](https://github.com/acheong08/Bard)
-[2] GitHub: [HanaokaYuzu/Gemini-API](https://github.com/HanaokaYuzu/Gemini-API)
-
-[3] Github: [dsdanielpark/Bard-API](https://github.com/dsdanielpark/Bard-API)
-[4] Github: [GoogleCloudPlatform/generative-ai](https://github.com/
+References [1]: Paper - [Introducing GEMINI: Multimodal Generative Models]
+(https://arxiv.org/abs/2312.11805)
+[2]: Website - [Google DeepMind :: GEMINI Introduction](https://
+deepmind.google/technologies/gemini/#introduction)
+[3]: Paper - [GEMMA: A Unified Language Model for Text Generation,
+Understanding, Translation, Coding, and Math.]()
+[4]: Website - [AI at Google :: GEMS Documentation](https://ai.google.dev/
+gemma/docs)
+[5]: Report - [CodeGMMA: Large Language Models Can Write Realistic Programming
+Assignments](https://storage.googleapis.com/deepmind-media/gemma/
+codegemma_report.pdf?utm_source=substack&utm_medium=email)
+[6]: Blog Post - [Announcing CodeGen: Building Better Developersâ Tools Using
+LLMs](https://huggingface.co/blog/codegen)
+[7]: Collection - [Google :: CodeGen Release](https://huggingface.co/
+collections/google/codegen-release-5d0f4c4eaedbc5cefcfdcbdf)
+[8]: Github - [acheong08/Bard](https://github.com/acheong08/Bard)
+[9]: GitHub - [HanaokaYuzu/Gemini-API](https://github.com/HanaokaYuzu/Gemini-
+API)
+[10]: Github - [dsdanielpark/Bard-API](https://github.com/dsdanielpark/Bard-
+API)
+[11]: Github - [GoogleCloudPlatform/generative-ai](https://github.com/
 GoogleCloudPlatform/generative-ai)
-[5] Github: [OpenRouter](https://github.com/OpenRouterTeam/openrouter-runner)
-[6] WebSite: [Google AI Studio](https://ai.google.dev/tutorials/ai-
+[12]: Github - [OpenRouter](https://github.com/OpenRouterTeam/openrouter-
+runner)
+[13]: WebSite - [Google AI Studio](https://ai.google.dev/tutorials/ai-
 studio_quickstart)
 > *Warning* Users assume full legal responsibility for GeminiAPI. Not endorsed
 by Google. Excessive use may lead to account restrictions. Changes in policies
 or account status may affect functionality. Utilize issue and discussion pages.
 
 ## Requirements Python 3.7 or higher.
```

### Comparing `python-gemini-api-2.4.2/README.md` & `python_gemini_api-2.4.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,182 +1,233 @@
+Metadata-Version: 2.1
+Name: python-gemini-api
+Version: 2.4.3
+Summary: The python package that returns Response of Google Gemini through API.
+Home-page: https://github.com/dsdanielpark/Gemini-API
+Author: Daniel Park
+Author-email: parkminwoo1991@gmail.com
+Keywords: Python,API,Gemini,Google Gemini,Large Language Model,Chatbot API,Google API,Chatbot
+Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Intended Audience :: Science/Research
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: httpx[http2]>=0.20.0
+Requires-Dist: requests
+Requires-Dist: browser_cookie3
+Requires-Dist: loguru
+Requires-Dist: pydantic
+Provides-Extra: voice
+Requires-Dist: gTTS; extra == "voice"
+Requires-Dist: SpeechRecognition; extra == "voice"
+Requires-Dist: openai; extra == "voice"
+Requires-Dist: anthropic; extra == "voice"
+
 
 # <img src="https://www.gstatic.com/lamda/images/favicon_v1_150160cddff7f294ce30.svg" width="35px" alt="Gemini Icon" /> Gemini API  <a href="https://pypi.org/project/python-gemini-api/"> <img alt="PyPI" src="https://img.shields.io/pypi/v/python-gemini-api?color=black"></a>
 
 
 <p align="right">
     <a href="https://github.com/dsdanielpark/Gemini-API"><img alt="pip download" src="https://img.shields.io/badge/pip_install-python_gemini_api-black"></a> 
     <a href="https://github.com/psf/black"><img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg"></a>
     <a href="https://hits.seeyoufarm.com"><img src="https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2Fdsdanielpark%2FGemini-API&count_bg=%23000000&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=views&edge_flat=false"/></a>
     <a href="https://pypistats.org/packages/python-gemini-api"><img alt="Downloads" src="https://pepy.tech/badge/python-gemini-api"></a>
 <!-- <a href="https://github.com/dsdanielpark/Gemini-API/stargazers"><img src="https://img.shields.io/github/stars/dsdanielpark/Gemini-API?style=social"></a> -->
 </p>
 
 
+
 https://github.com/dsdanielpark/Gemini-API/assets/81407603/e0c11d4f-3fe1-4cbb-ba79-d9f89b637324
 
 
 
 
 
 
 A *unofficial* Python wrapper, [python-gemini-api](https://pypi.org/project/python-gemini-api/), operates through reverse-engineering, utilizing cookie values to interact with [Google Gemini](https://gemini.google.com) for users struggling with frequent authentication problems or unable to authenticate via [Google Authentication](https://developers.google.com/identity/protocols/oauth2?hl=en).
 
 Collaborated competently with [Antonio Cheong](https://github.com/acheong08).
 
-
-
-
+<br>
 
 <br>
 
 
 > [!TIP]
 > | 2024-03-26 | [[See Code Examples]](https://github.com/dsdanielpark/Gemini-API/blob/main/documents/README_OPENROUTER.md)
 > 
 > Check out temporarily free Open-source LLM APIs with Open Router.  (Free limit: 10 requests/minute) 
 
-<br><br>
+<br>
 
+## Contents
 
 - [ Gemini API   ](#-gemini-api---)
-  - [What is Gemini?](#what-is-gemini)
-  - [Installation](#installation)
-  - [Authentication](#authentication)
-  - [Quick Start](#quick-start)
+  - [What is Gemini? 🔐](#what-is-gemini)
+  - [Installation ✅](#installation-)
+  - [Authentication ✅](#authentication)
+  - [Quick Start ✅](#quick-start)
   - [Usage](#usage)
-    - [# 01. Initialization](#-01-initialization)
+    - [# 01. Initialization ✅](#-01-initialization)
     - [# 02. Generate content](#-02-generate-content)
     - [# 03. Send request](#-03-send-request)
     - [# 04. Text generation](#-04-text-generation)
     - [# 05. Image generation](#-05-image-generation)
     - [# 06. Retrieving Images from Gemini Responses](#-06-retrieving-images-from-gemini-responses)
     - [# 07. Generate content from images](#-07-generate-content-from-images)
     - [# 08. Generate content using Google Services](#-08-generate-content-using-google-services)
-    - [# 09. Fix context setting rcid](#-09-fix-context-setting-rcid)
+    - [# 09. Fix context setting RCID](#-09-fix-context-setting-rcid)
     - [# 10. Changing the Selected Response from 0 to *n*](#-10-changing-the-selected-response-from-0-to-n)
     - [# 11. Generate custom content](#-11-generate-custom-content)
   - [Further](#further)
-  - [Open-source LLM, Gemma](#open-source-llm-gemma)
-    - [How to use Gemma](#how-to-use-gemma)
-  - [Utilize free open-source LLM API through Open Router](#utilize-free-open-source-llm-api-through-open-router)
+  - [Google Open-source LLMs](#google-open-source-llms)
+      - [Open-source LLM, Gemma 🤝](#open-source-llm-gemma)
+      - [Open-source LLM, Code Gemma 🤝](#open-source-llm-code-gemma)
+  - [Utilize free open-source LLM API through Open Router ✅](#utilize-free-open-source-llm-api-through-open-router)
 
 
 
 
 
 
 
 <br>
 
+## What is [Gemini](https://deepmind.google/technologies/gemini/#introduction)?
 
+| [Paper](https://arxiv.org/abs/2312.11805) | [Official Website](https://deepmind.google/technologies/gemini/#introduction) | [Official API](https://aistudio.google.com/) | [API Documents](https://cloud.google.com/vertex-ai/docs/generative-ai/model-reference/gemini) |
 
+Gemini is a family of generative AI models developed by Google DeepMind that is designed for multimodal use cases. The Gemini API gives you access to the Gemini Pro and Gemini Pro Vision models. In February 2024, Google's **Bard** service was changed to **Gemini**.
 
+#### Overview of Google LLMs
 
-## What is [Gemini](https://deepmind.google/technologies/gemini/#introduction)?
+| Model | Type | Access | Details
+|:-------:|:------:|:--------:|---------
+[Gemini](https://huggingface.co/google/gemma-7b) | Proprietary | API <sup>[[13](https://ai.google.dev/tutorials/ai-studio_quickstart)] | A proprietary multimodal AI by Google DeepMind, including advanced models such as Gemini Pro and Gemini Pro Vision. Access is restricted to API usage; additional insights may be obtained through the paper and website. <sup>[[1](https://arxiv.org/abs/2312.11805)][[2](https://deepmind.google/technologies/gemini/#introduction)]</sup>
+[Gemma](https://huggingface.co/google/gemma-7b) | Open Source | [Downloadable](https://huggingface.co/google/gemma-7b) <br>[Free API](https://github.com/dsdanielpark/Gemini-API?tab=readme-ov-file#utilize-free-open-source-llm-api-through-open-router) | An open-source text-to-text language model suitable for tasks like QA and summarization. Weights are downloadable for on-premises use, and detailed documentation is provided via the paper and website. <sup>[[3](https://arxiv.org/abs/2403.08295)][[4](https://ai.google.dev/gemma/docs)]</sup>
+[Code Gemma](https://huggingface.co/google/codegemma-7b-it) | Open Source | [Downloadable](https://huggingface.co/google/codegemma-7b-it) | Designed specifically for programming tasks, this open-source model offers downloadable weights to assist developers with code generation and similar activities. Refer to the associated paper, blog post, and Hugging Face collection for more information. <sup>[[5](https://storage.googleapis.com/deepmind-media/gemma/codegemma_report.pdf?utm_source=substack&utm_medium=email)][[6](https://huggingface.co/blog/codegemma)][[7](https://huggingface.co/collections/google/codegemma-release-66152ac7b683e2667abdee11)]</sup>
 
-| [Paper](https://arxiv.org/abs/2312.11805) | [Official Website](https://deepmind.google/technologies/gemini/#introduction) | [Official API](https://aistudio.google.com/) | [API Documents](https://cloud.google.com/vertex-ai/docs/generative-ai/model-reference/gemini) |
 
-Gemini is a family of generative AI models developed by Google DeepMind that is designed for multimodal use cases. The Gemini API gives you access to the Gemini Pro and Gemini Pro Vision models. In February 2024, Google's **Bard** service was changed to **Gemini**.
+<br>
 
+## What is [Python-Gemini-API](https://github.com/dsdanielpark/Gemini-API)?
 
+This is a Python wrapper derived from the [Bard API](https://github.com/dsdanielpark/Bard-API) project, designed to retrieve responses from Gemini Web in REST format. **Synchronous clients are preferred over asynchronous ones for Gemini because of rate limiting and blocking concerns.**
 
 ## Installation 📦
 ```
 pip install python-gemini-api
 ```
 ```
 pip install git+https://github.com/dsdanielpark/Gemini-API.git
 ```
 For the updated version, use as follows:
 ```
 pip install -q -U python-gemini-api
 ```
+
+
+
 ## Authentication
-> [!NOTE]
-> Cookies can change quickly. Don't reopen the same session or repeat prompts too often; they'll expire faster. If the cookie value doesn't export correctly, refresh the Gemini page and export again. 
+
 1. Visit https://gemini.google.com/ <br>
     With browser open, try auto-collecting cookies first.
     ```python
     from gemini import Gemini
     GeminiClient = Gemini(auto_cookies=True)
 
     # Testing needed as cookies vary by region.
     # GeminiClient = Gemini(auto_cookies=True, target_cookies=["__Secure-1PSID", "__Secure-1PSIDTS"])
+    # GeminiClient = Gemini(auto_cookies=True, target_cookies="all") # You can pass whole cookies
 
     response = GeminiClient.generate_content("Hello, Gemini. What's the weather like in Seoul today?")
     print(response.payload)
     ```
 2. *(Manually)* `F12` for browser console → `Session: Application` → `Cookies` → Copy the value of some working cookie sets. If it doesn't work, go to step 3.
     <details><summary>Some working cookie sets</summary>
     Cookies may vary by account or region. 
       
     First try `__Secure-1PSIDCC` alone. If it doesn't work, use `__Secure-1PSID` and `__Secure-1PSIDTS`. Still no success? Try these four cookies: `__Secure-1PSIDCC`, `__Secure-1PSID`, `__Secure-1PSIDTS`, `NID`. If none work, proceed to step 3 and consider sending the entire cookie file.
     
     </details>
 
 3. *(Recommended)* Export Gemini site cookies via a browser extension. For instance, use Chrome extension [ExportThisCookies](https://chromewebstore.google.com/detail/exportthiscookie/dannllckdimllhkiplchkcaoheibealk), open, and copy the txt file contents.
 
+
+<br>
+
 <details><summary>Further: For manual collection or Required for a few users upon error</summary>
 
 4. For manual cookie collection, refer to [this image](assets/cookies.pdf). Press F12 → Network → Send any prompt to Gemini webui → Click the post address starting with "https://gemini.google.com/_/BardChatUi/data/assistant.lamda.BardFrontendService/StreamGenerate" → Headers → Request Headers → Cookie → Copy and Reformat as JSON manually.
 5. *(Required for a few users upon error)* If errors persist after manually collecting cookies, refresh the Gemini website and collect cookies again. If errors continue, some users may need to manually set the nonce value. To do this: Press F12 → Network → Send any prompt to Gemini webui → Click the post address starting with "https://gemini.google.com/_/BardChatUi/data/assistant.lamda.BardFrontendService/StreamGenerate" → Payload → Form Data → Copy the "at" key value. See [this image](assets/nonce_value.pdf) for reference.
 </details>
 
 
 > [!IMPORTANT] 
->  Try different Google accounts until you find a working cookie. Use a fresh browser to ensure no remaining cookie values. Use secret browsing mode with independent cookies. Results may vary depending on factors like IP and account status. Providing the entire set of cookies seems to fix one cookie per account. Additionally, once successfully connected with that cookie, it seems to work flawlessly for over three weeks without any errors. *Try various methods until you succeed. Experiment in different environments.*
+> Experiment with different Google accounts and browser settings to find a working cookie. Success may vary by IP and account status. Once connected, a cookie typically remains effective over a month. Keep testing until successful.
 
 
 <br>
 
 ## Quick Start
 
-*Simple usage*
-
-Setting Gemini response language (Optional): Check supported languages [here](https://developers.google.com/hotels/hotel-prices/dev-guide/country-codes). Default is English.
-
-```python
-import os
-os.environ["GEMINI_LANGUAGE"] = "KR"
-```
-
-
-
-Generate content: returns parsed response.
+**Generate content:** returns parsed response.
 ```python
 from gemini import Gemini
 
 cookies = {} # Cookies may vary by account or region. Consider sending the entire cookie file.
 GeminiClient = Gemini(cookies=cookies) # You can use various args
 
 response = GeminiClient.generate_content("Hello, Gemini. What's the weather like in Seoul today?")
 response.payload
 ```
 
-Generate content from image: you can use image as input.
+**Generate content from image:** you can use image as input.
 ```python
 from gemini import Gemini
 
 cookies = {} # Cookies may vary by account or region. Consider sending the entire cookie file.
 
 GeminiClient = Gemini(cookies=cookies) # You can use various args
 response = GeminiClient.generate_content("What does the text in this image say?", image='folder/image.jpg')
 response.payload
 ```
 
 > [!NOTE] 
 > If the generate_content method returns an empty payload, try executing it again without reinitializing the Gemini object.
 
-<br>
+<br><br>
 
 ## Usage
 
+*Setting language and Gemini version using environment variables:*
+
+Setting Gemini response language (Optional): Check supported languages [here](https://developers.google.com/hotels/hotel-prices/dev-guide/country-codes). Default is English.
+
+```python
+import os
+os.environ["GEMINI_LANGUAGE"] = "KR"  # Setting Gemini response language (Optional)
+os.environ["GEMINI_ULTRA"] = "1"      # Switch to Gemini-advanced response (Experimental, Optional)
+# In some accounts, access to Gemini Ultra may not be available. If that's the case, please revert it back to "0".
+```
+
+
+
+<br>
 
 ### # 01. Initialization
-Please explicitly declare `cookies` in dict format. You can also enter the path to the file containing the cookie with `cookie_fp`(*.json, *.txt supported). Check this [sample cookie file](https://github.com/dsdanielpark/Gemini-API/blob/main/cookies.txt).
+Please explicitly declare `cookies` in dict format. You can also enter the path to the file containing the cookie with `cookie_fp`(*.json, *.txt supported). Check sample cookie files in [assets](https://github.com/dsdanielpark/Gemini-API/tree/main/assets) folder.
 
 
 
 
 ```python
 from gemini import Gemini
 
@@ -189,53 +240,48 @@
   }
 
 GeminiClient = Gemini(cookies=cookies)
 # GeminiClient = Gemini(cookie_fp="folder/cookie_file.json") # (*.json, *.txt) are supported.
 # GeminiClient = Gemini(auto_cookies=True) # Or use auto_cookies paprameter
 ```
 
-#### Auto Cookie Update
-For `auto_cookie` to be set to `True`, Gemini WebUI must be active in the browser. The [browser_cookie3](https://github.com/borisbabic/browser_cookie3) enables automatic cookie collection, though updates may not be complete yet.
+##### Auto Cookie Update
+For `auto_cookie` to be set to `True`, and adjust `target_cookies`. Gemini WebUI must be active in the browser. The [browser_cookie3](https://github.com/borisbabic/browser_cookie3) enables automatic cookie collection, though updates may not be complete yet.
 
 
-> [!IMPORTANT]
->  **If the session connects successfully and `generate_content` runs well, CLOSE Gemini website.** If Gemini web stays open in the browser, cookies may expire faster.
 
 <br>
 
 ### # 02. Generate content
-Returns Gemini's response, but the first one might be empty. If generate_content yields an empty payload, rerun it without reinitializing Gemini. 
+Returns Gemini's response, but the first one might be empty. 
+
 
-Regardless of model output type, access the response_dict property (renamed to payload after v2.3.0).
-https://github.com/dsdanielpark/Gemini-API/blob/fdf064c57bc1fb47fbbb4b93067618a200e77f62/gemini/core.py#L252
 ```python
 prompt = "Hello, Gemini. What's the weather like in Seoul today?"
 response = GeminiClient.generate_content(prompt)
 print(response.payload)
 ```
+
+
 > [!IMPORTANT]
->  Once connected and generating valid content, **Be sure to CLOSE the Gemini website or CLOSE your browser** for cookie stability. 
+>  DO NOT send same prompt repeatly. **If the session connects successfully and `generate_content` runs well, CLOSE Gemini website.** If Gemini web stays open in the browser, cookies may expire faster. 
 
 <br>
 
-The output of the generate_content function is `GeminiModelOutput`, with the following structure:
-
-**Properties of GeminiModelOutput:**
+The output of the generate_content function is `GeminiModelOutput`, with the following structure: 
 - *rcid*: returns the response candidate id of the chosen candidate.
 - *text*: returns the text of the chosen candidate.
 - *code*: returns the codes of the chosen candidate.
 - *web_images*: returns a list of web images from the chosen candidate.
 - *generated_images*: returns a list of generated images from the chosen candidate.
-- *payload*: returns the response dictionary, if available. (same as *reponse_dict* under v2.3.0)
-
+- *payload*: returns the response dictionary, if available.
 https://github.com/dsdanielpark/Gemini-API/blob/fdf064c57bc1fb47fbbb4b93067618a200e77f62/gemini/src/model/output.py#L16
 
 
-> [!NOTE]
-> If the session fails to connect, works improperly, or terminates, returning an error, it is recommended to manually renew the cookies. The error is likely due to incorrect cookie values. Refresh or log out of Gemini web to renew cookies and try again. 
+
 
 <br>
 
 
 ### # 03. Send request
 Send request: returns the request's payload and status_code, making debugging easier.
 ```python
@@ -243,15 +289,15 @@
 
 cookies = {} # Cookies may vary by account or region. Consider sending the entire cookie file.
 GeminiClient = Gemini(cookies=cookies) # You can use various args
 
 response_text, response_status = GeminiClient.send_request("Hello, Gemini. What's the weather like in Seoul today?")
 print(response_text)
 ```
-
+You can track the total number of requests made by accessing the `request_count` property within the `Gemini` class.
 
 <br>
 
 ### # 04. Text generation
 Returns text generated by Gemini.
 ```python
 prompt = "Hello, Gemini. What's the weather like in Seoul today?"
@@ -260,65 +306,62 @@
 ```
 
 
 <br>
 
 ### # 05. Image generation
 Returns images generated by Gemini.
-https://github.com/dsdanielpark/Gemini-API/blob/fdf064c57bc1fb47fbbb4b93067618a200e77f62/gemini/src/model/image.py#L12
 
-*Sync downloader*
-```python
-from gemini import Gemini, GeminiImage
+*Async downloader*
 
+```python
 response = GeminiClient.generate_content("Create illustrations of Seoul, South Korea.")
-generated_images = response.generated_images # Check generated images [Dict]
 
-GeminiImage.save_sync(generated_images, save_path="save_dir", cookies=cookies)
+generated_images = response.generated_images # Check generated images [Dict]
 
-# You can use byte type image dict for printing images as follow:
-# bytes_images_dict = GeminiImage.fetch_images_dict_sync(generated_images, cookies=cookies) # Get bytes images dict
-# GeminiImage.save_images_sync(bytes_images_dict, path="save_dir", cookies=cookies) # Save to path
+await GeminiImage.save(generated_images, "save_dir", cookies=cookies)
+# image_data_dict = await GeminiImage.fetch_images_dict(generated_images, cookies=cookies)
+# await GeminiImage.save_images(image_data_dict, "save_dir")
 ```
 
-<details><summary>Display images in IPython</summary>
-  
+
+<details><summary>Further</summary>
+
+*Display images in IPython*
   You can display the image or transmit it to another application in byte format.
   
-  ```
+  ```python
   bytes_images_dict = GeminiImage.fetch_images_dict_sync(generated_images, cookies) # Get bytes images dict
   from IPython.display import display, Image
   import io
   
   for image_name, image_bytes in bytes_images_dict.items():
       print(image_name)
       image = Image(data=image_bytes)
       display(image)
   ```
 
-</details>
-
-
-
-*Async downloader*
 
+*Sync downloader*
 ```python
-response = GeminiClient.generate_content("Create illustrations of Seoul, South Korea.")
+from gemini import Gemini, GeminiImage
 
+response = GeminiClient.generate_content("Create illustrations of Seoul, South Korea.")
 generated_images = response.generated_images # Check generated images [Dict]
 
-await GeminiImage.save(generated_images, "save_dir", cookies=cookies)
-# image_data_dict = await GeminiImage.fetch_images_dict(generated_images, cookies=cookies)
-# await GeminiImage.save_images(image_data_dict, "save_dir")
-```
+GeminiImage.save_sync(generated_images, save_path="save_dir", cookies=cookies)
 
+# You can use byte type image dict for printing images as follow:
+# bytes_images_dict = GeminiImage.fetch_images_dict_sync(generated_images, cookies=cookies) # Get bytes images dict
+# GeminiImage.save_images_sync(bytes_images_dict, path="save_dir", cookies=cookies) # Save to path
+```
 
-<details><summary>Async downloader wrapper</summary>
+*Async downloader wrapper*
 
-```
+```python
 import asyncio
 from gemini import Gemini, GeminiImage
 
 async def save_generated_imagse(generated_imagse, save_path="save_dir", cookies=cookies):
     await GeminiImage.save(generated_imagse, save_path=save_path, cookies=cookies)
 
 # Run the async function
@@ -351,41 +394,45 @@
 > Use GeminiImage for image processing. `web_images` works without cookies, but for images like `generated_image` from Gemini, pass cookies. Cookies are needed to download images from Google's storage. Check the response or use existing cookies variable.
 
 <br>
 
 ### # 06. Retrieving Images from Gemini Responses
 Returns images in response of Gemini.
 
-*Sync downloader*
-```python
-from gemini import Gemini, GeminiImage
-
-response = GeminiClient.generate_content("Please recommend a travel itinerary for Seoul.")
-response_images = response.web_images # Check response images [Dict]
 
-GeminiImage.save_sync(response_images, save_path="save_dir")
-
-# You can use byte type image dict as follow:
-# bytes_images_dict = GeminiImage.fetch_bytes_sync(response_images, cookies) # Get bytes images dict
-# GeminiImage.save_images_sync(bytes_images_dict, path="save_dir") # Save to path
-```
 *Async downloader*
 ```python
 response = GeminiClient.generate_content("Create illustrations of Seoul, South Korea.")
 
 response_images = response.web_images # Check generated images [Dict]
 
 await GeminiImage.save(response_images, "save_dir")
 # image_data_dict = await GeminiImage.fetch_images_dict(response_images)
 # await GeminiImage.save_images(image_data_dict, "save_dir")
 ```
 
-<details><summary>Async downloader wrapper</summary>
+<details><summary>Further</summary>
 
+
+*Sync downloader*
+```python
+from gemini import Gemini, GeminiImage
+
+response = GeminiClient.generate_content("Please recommend a travel itinerary for Seoul.")
+response_images = response.web_images # Check response images [Dict]
+
+GeminiImage.save_sync(response_images, save_path="save_dir")
+
+# You can use byte type image dict as follow:
+# bytes_images_dict = GeminiImage.fetch_bytes_sync(response_images, cookies) # Get bytes images dict
+# GeminiImage.save_images_sync(bytes_images_dict, path="save_dir") # Save to path
 ```
+
+*Async downloader wrapper*
+```python
 import asyncio
 from gemini import Gemini, GeminiImage
 
 async def save_response_web_imagse(response_images, save_path="save_dir", cookies=cookies):
     await GeminiImage.save(response_images, save_path=save_path, cookies=cookies)
 
 # Run the async function
@@ -466,59 +513,68 @@
   - Description: Explore YouTube videos and ask questions about what interests you.
   - Features: Problem-solving, generating ideas, search, exploring topics
 </details>
 
 <br>
 
 
-### # 09. Fix context setting rcid
-You can specify a particular response by setting its response candidate id(rcid).
+### # 09. Fix context setting RCID
+You can specify a particular response by setting its Response Candidate ID(RCID).
 
 ```python
 # Generate content for the prompt "Give me some information about the USA."
 response1 = GeminiClient.generate_content("Give me some information about the USA.")
 # After reviewing the responses, choose the one you prefer and copy its RCID.
 GeminiClient.rcid = "rc_xxxx"
 
 # Now, generate content for the next prompt "How long does it take from LA to New York?"
 response2 = GeminiClient.generate_content("How long does it take from LA to New York?")
+
+# However, RCID may not persist. If parsing fails, reset `GeminiClient.rcid` to None.
+# GeminiClient.rcid = None
 ```
 
+
+
 <br>
 
 ### # 10. Changing the Selected Response from 0 to *n*
 In Gemini, generate_content returns the first response. This may vary depending on length or sorting. Therefore, you can specify the index of the chosen response from 0 to *n* as follows. However, if there is only one response, revert it back to 0.
 ```python
 from gemini import GeminiModelOutput
+
 GeminiModelOutput.chosen = 1 # default is 0
-response1 = GeminiClient.generate_content("Give me some information about the USA.")
+response_choice_1 = GeminiClient.generate_content("Give me some information about the USA.")
+
+# If not all Gemini returns are necessarily plural, revert back to 0 in case of errors.
+#  GeminiModelOutput.chosen = 0
 ```
 
 <br>
 
 ### # 11. Generate custom content 
 Parse the response text to extract desired values.
 
-https://github.com/dsdanielpark/Gemini-API/blob/fdf064c57bc1fb47fbbb4b93067618a200e77f62/gemini/core.py#L317
 
 Using `Gemini.generate_custom_content`, specify custom parsing to extract specific values. Utilize ParseMethod1 and ParseMethod2 by default, and you can pass custom parsing methods as arguments if desired. Refer to [custom_parser.py](https://github.com/dsdanielpark/Gemini-API/blob/main/gemini/src/model/parser/custom_parser.py).
 
 ```python
 # You can create a parser method that takes response_text as the input for custom_parser.
 response_text, response_status = GeminiClient.send_request("Give me some information about the USA.")
 
 # Use custom_parser function or class inheriting from BaseParser
 response = GeminiClient.generate_custom_content("Give me some information about the USA.", *custom_parser)
 ```
 
+https://github.com/dsdanielpark/Gemini-API/blob/31b842488bbc5429ad9c74b1d8b00e20d94e8cb1/gemini/client.py#L323
 <br>
 
 ## Further
 
-### Use rotating proxies
+### Use rotating proxies via [Smart Proxy by Crawlbase](https://crawlbase.com/docs/smart-proxy/?utm_source=github_ad&utm_medium=social&utm_campaign=bard_api)
 
 If you want to **avoid blocked requests** and bans, then use [Smart Proxy by Crawlbase](https://crawlbase.com/docs/smart-proxy/?utm_source=github_ad&utm_medium=social&utm_campaign=bard_api). It forwards your connection requests to a **randomly rotating IP address** in a pool of proxies before reaching the target website. The combination of AI and ML make it more effective to avoid CAPTCHAs and blocks.
 
 ```python
 # Get your proxy url at crawlbase https://crawlbase.com/docs/smart-proxy/get/
 proxy_url = "http://xxxxx:@smartproxy.crawlbase.com:8012" 
 proxies = {"http": proxy_url, "https": proxy_url}
@@ -526,16 +582,16 @@
 GeminiClient = Gemini(cookies=cookies, proxies=proxies, timeout=30)
 GeminiClient.generate_content("Hello, Gemini. Give me a beautiful photo of Seoul's scenery.")
 ```
 
 ### Reusable session object
 For standard cases, use Gemini class; for exceptions, use session objects. When creating a new bot Gemini server, adjust Headers.MAIN.
 ```python
-from gemini import Gemini, Headers
 import requests
+from gemini import Gemini, Headers
 
 cookies = {} 
 
 session = requests.Session()
 session.headers = Headers.MAIN
 for key, value in cookies.items():
     session.cookies.update({key: value})
@@ -552,42 +608,66 @@
 ## [More features](https://github.com/dsdanielpark/Gemini-API/blob/main/documents/README_DEV.md)
 Explore additional features in [this document](https://github.com/dsdanielpark/Gemini-API/blob/main/documents/README_DEV.md).
 
 If you want to develop your own simple code, you can start from [this simple code example](https://github.com/dsdanielpark/Gemini-API/blob/main/script/sample.ipynb).  
 
 <br>
 
+## Google Open-source LLMs
+
+If you have sufficient GPU resources, you can download weights directly instead of using the Gemini API to generate content. Consider Gemma and Code Gemma, an open-source models **available for on-premises use**.
+
+
 
-## Open-source LLM, [Gemma](https://huggingface.co/google/gemma-7b)
-If you have sufficient GPU resources, you can download weights directly instead of using the Gemini API to generate content. Consider Gemma, an open-source model **available for on-premises use**.
+### Open-source LLM, [Gemma](https://huggingface.co/google/gemma-7b)
 
-[Gemma](https://huggingface.co/google/gemma-7b) models are Google's lightweight, advanced text-to-text, decoder-only language models, derived from Gemini research. Available in English, they offer open weights and variants, ideal for tasks like question answering and summarization. Their small size enables deployment in resource-limited settings, broadening access to cutting-edge AI. For more infomation, visit [Gemma-7b](https://huggingface.co/google/gemma-7b) model card.
 
-### How to use Gemma
+Gemma models are Google's lightweight, advanced text-to-text, decoder-only language models, derived from Gemini research. Available in English, they offer open weights and variants, ideal for tasks like question answering and summarization. For more infomation, visit [Gemma-7b](https://huggingface.co/google/gemma-7b) model card.
+
+#### How to use Gemma
 ```python
 from transformers import AutoTokenizer, AutoModelForCausalLM
 
 tokenizer = AutoTokenizer.from_pretrained("google/gemma-7b")
 model = AutoModelForCausalLM.from_pretrained("google/gemma-7b")
 
 input_text = "Write me a poem about Machine Learning."
 input_ids = tokenizer(input_text, return_tensors="pt")
 
 outputs = model.generate(**input_ids)
 print(tokenizer.decode(outputs[0]))
 ```
 
+### Open-source LLM, [Code Gemma](https://huggingface.co/collections/google/codegemma-release-66152ac7b683e2667abdee11)
+
+CodeGemma, which is an official release from Google for code LLMs, was released on April 9, 2024. It provides three models specifically designed for generating and interacting with code. You can explore the [Code Gemma models](https://huggingface.co/collections/google/codegemma-release-66152ac7b683e2667abdee11) and view the [model card](https://huggingface.co/google/codegemma-7b-it) for more details.
+
+#### How to use Code Gemma
+```python
+from transformers import GemmaTokenizer, AutoModelForCausalLM
+
+tokenizer = GemmaTokenizer.from_pretrained("google/codegemma-7b-it")
+model = AutoModelForCausalLM.from_pretrained("google/codegemma-7b-it")
+
+input_text = "Write me a Python function to calculate the nth fibonacci number."
+input_ids = tokenizer(input_text, return_tensors="pt")
+
+outputs = model.generate(**input_ids)
+print(tokenizer.decode(outputs[0]))
+```
+
+
+
 <br>
 
 
 ## Utilize free open-source LLM API through [Open Router](https://openrouter.ai/)
-OpenRouter offers temporary free inference for select models. Obtain an API key from [Open Router API](https://openrouter.ai/keys) and check free models at [Open Router models](https://openrouter.ai/docs#models). Use models with a 0-dollar token cost primarily; other models may incur charges. See more [free open-source LLM API guide](https://github.com/dsdanielpark/Gemini-API/blob/main/documents/README_OPENROUTER.md)
+OpenRouter offers temporary free inference for select models. Obtain an API key from [Open Router API](https://openrouter.ai/keys) and check free models at [Open Router models](https://openrouter.ai/docs#models). Use models with a 0-dollar token cost primarily; other models may incur charges. See more at [free open-source LLM API guide](https://github.com/dsdanielpark/Gemini-API/blob/main/documents/README_OPENROUTER.md).
 
-> [!NOTE]
-> You can easily receive responses from open LLMs without this package by following the instructions on [here](https://openrouter.ai/docs#models).
+**Sync client is favored over async for Gemini due to rate limiting and blocking issues**, but OpenRouter offers reliable open-source LLMs for [async implementation](https://github.com/dsdanielpark/Gemini-API/blob/main/documents/README_OPENROUTER.md#openrouter-async-api-client).
 
 ```python
 from gemini import OpenRouter
 
 OPENROUTER_API_KEY = "<your_open_router_api_key>"
 GemmaClient = OpenRouter(api_key=OPENROUTER_API_KEY, model="google/gemma-7b-it:free")
 
@@ -611,28 +691,26 @@
 
 
 
 
 
 <br>
 
+## Sponsor, [Crawlbase](https://crawlbase.com/)
+Use [Crawlbase](https://crawlbase.com/) API for efficient data scraping to train AI models, boasting a 98% success rate and 99.9% uptime. It's quick to start, GDPR/CCPA compliant, supports massive data extraction, and is trusted by 70k+ developers.
+
+<br>
 
 ## [FAQ](https://github.com/dsdanielpark/Gemini-API/blob/main/documents/README_FAQ.md)
 First review [HanaokaYuzu/Gemini-API](https://github.com/HanaokaYuzu/Gemini-API) and the [Official Google Gemini API](https://aistudio.google.com/) before using this package.
 You can find most help on the [FAQ](https://github.com/dsdanielpark/Gemini-API/blob/main/documents/README_FAQ.md) and [Issue](https://github.com/dsdanielpark/Gemini-API/issues) pages. 
-
-
             
 ## [Issues](https://github.com/dsdanielpark/Gemini-API/issues)
 Sincerely grateful for any reports on new features or bugs. Your valuable feedback on the code is highly appreciated. Frequent errors may occur due to changes in Google's service API interface. Both [Issue reports](https://github.com/dsdanielpark/Gemini-API/issues) and [Pull requests](https://github.com/dsdanielpark/Gemini-API/pulls) contributing to improvements are always welcome. We strive to maintain an active and courteous open community.
 
-
-## Sponsor
-Use [Crawlbase](https://crawlbase.com/) API for efficient data scraping to train AI models, boasting a 98% success rate and 99.9% uptime. It's quick to start, GDPR/CCPA compliant, supports massive data extraction, and is trusted by 70k+ developers.
-
 ## Contributors
 We would like to express our sincere gratitude to all the contributors. 
 
 This package aims to re-implement the functionality of the [Bard API](https://github.com/dsdanielpark/Bard-API/), which has been archived for the contributions of the beloved open-source community, despite Gemini's official API already being available.
 
 Contributors to the [Bard API](https://github.com/dsdanielpark/Bard-API/) and [Gemini API](https://github.com/dsdanielpark/Gemini-API/).
 
@@ -664,20 +742,27 @@
 
 
 ## License ©️ 
 [MIT](https://opensource.org/license/mit/) license, 2024. We hereby strongly disclaim any explicit or implicit legal liability related to our works. Users are required to use this package responsibly and at their own risk. This project is a personal initiative and is not affiliated with or endorsed by Google. It is recommended to use Google's official API.
 
 
 ## References
-[1] Github: [acheong08/Bard](https://github.com/acheong08/Bard) <br>
-[2] GitHub: [HanaokaYuzu/Gemini-API](https://github.com/HanaokaYuzu/Gemini-API) <br>
-[3] Github: [dsdanielpark/Bard-API](https://github.com/dsdanielpark/Bard-API) <br>
-[4] Github: [GoogleCloudPlatform/generative-ai](https://github.com/GoogleCloudPlatform/generative-ai) <br>
-[5] Github: [OpenRouter](https://github.com/OpenRouterTeam/openrouter-runner) <br>
-[6] WebSite: [Google AI Studio](https://ai.google.dev/tutorials/ai-studio_quickstart) <br>
+[1]: Paper - [Introducing GEMINI: Multimodal Generative Models](https://arxiv.org/abs/2312.11805) <br>
+[2]: Website - [Google DeepMind :: GEMINI Introduction](https://deepmind.google/technologies/gemini/#introduction) <br>
+[3]: Paper - [GEMMA: A Unified Language Model for Text Generation, Understanding, Translation, Coding, and Math.]() <br>
+[4]: Website - [AI at Google :: GEMS Documentation](https://ai.google.dev/gemma/docs) <br>
+[5]: Report - [CodeGMMA: Large Language Models Can Write Realistic Programming Assignments](https://storage.googleapis.com/deepmind-media/gemma/codegemma_report.pdf?utm_source=substack&utm_medium=email) <br>
+[6]: Blog Post - [Announcing CodeGen: Building Better Developers’ Tools Using LLMs](https://huggingface.co/blog/codegen) <br>
+[7]: Collection - [Google :: CodeGen Release](https://huggingface.co/collections/google/codegen-release-5d0f4c4eaedbc5cefcfdcbdf) <br>
+[8]: Github - [acheong08/Bard](https://github.com/acheong08/Bard) <br>
+[9]: GitHub - [HanaokaYuzu/Gemini-API](https://github.com/HanaokaYuzu/Gemini-API) <br>
+[10]: Github - [dsdanielpark/Bard-API](https://github.com/dsdanielpark/Bard-API) <br>
+[11]: Github - [GoogleCloudPlatform/generative-ai](https://github.com/GoogleCloudPlatform/generative-ai) <br>
+[12]: Github - [OpenRouter](https://github.com/OpenRouterTeam/openrouter-runner) <br>
+[13]: WebSite - [Google AI Studio](https://ai.google.dev/tutorials/ai-studio_quickstart) <br>
 
 
 > *Warning*
 Users assume full legal responsibility for GeminiAPI. Not endorsed by Google. Excessive use may lead to account restrictions. Changes in policies or account status may affect functionality. Utilize issue and discussion pages.
 
 <br>
```

#### html2text {}

```diff
@@ -1,66 +1,111 @@
-# [Gemini Icon]Gemini API_[_P_y_P_I_]
+Metadata-Version: 2.1 Name: python-gemini-api Version: 2.4.3 Summary: The
+python package that returns Response of Google Gemini through API. Home-page:
+https://github.com/dsdanielpark/Gemini-API Author: Daniel Park Author-email:
+parkminwoo1991@gmail.com Keywords: Python,API,Gemini,Google Gemini,Large
+Language Model,Chatbot API,Google API,Chatbot Classifier: Development Status ::
+2 - Pre-Alpha Classifier: Intended Audience :: Science/Research Classifier:
+Natural Language :: English Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
+Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12 Classifier: License :: OSI
+Approved :: MIT License Classifier: Topic :: Scientific/Engineering ::
+Artificial Intelligence Requires-Python: >=3.9 Description-Content-Type: text/
+markdown License-File: LICENSE Requires-Dist: httpx[http2]>=0.20.0 Requires-
+Dist: requests Requires-Dist: browser_cookie3 Requires-Dist: loguru Requires-
+Dist: pydantic Provides-Extra: voice Requires-Dist: gTTS; extra == "voice"
+Requires-Dist: SpeechRecognition; extra == "voice" Requires-Dist: openai; extra
+== "voice" Requires-Dist: anthropic; extra == "voice" # [Gemini Icon]Gemini API
+_[_P_y_P_I_]
   _[_p_i_p_ _d_o_w_n_l_o_a_d_]_[_C_o_d_e_ _s_t_y_l_e_:_ _b_l_a_c_k_]_[_h_t_t_p_s_:_/_/_h_i_t_s_._s_e_e_y_o_u_f_a_r_m_._c_o_m_/_a_p_i_/_c_o_u_n_t_/_i_n_c_r_/
                 _b_a_d_g_e_._s_v_g_?_u_r_l_=_h_t_t_p_s_%_3_A_%_2_F_%_2_F_g_i_t_h_u_b_._c_o_m_%_2_F_d_s_d_a_n_i_e_l_p_a_r_k_%_2_F_G_e_m_i_n_i_-
 _A_P_I_&_c_o_u_n_t___b_g_=_%_2_3_0_0_0_0_0_0_&_t_i_t_l_e___b_g_=_%_2_3_5_5_5_5_5_5_&_i_c_o_n_=_&_i_c_o_n___c_o_l_o_r_=_%_2_3_E_7_E_7_E_7_&_t_i_t_l_e_=_v_i_e_w_s_&_e_d_g_e___f_l_a_t_=_f_a_l_s_e_]
                                                                     _[_D_o_w_n_l_o_a_d_s_]
 https://github.com/dsdanielpark/Gemini-API/assets/81407603/e0c11d4f-3fe1-4cbb-
 ba79-d9f89b637324 A *unofficial* Python wrapper, [python-gemini-api](https://
 pypi.org/project/python-gemini-api/), operates through reverse-engineering,
 utilizing cookie values to interact with [Google Gemini](https://
 gemini.google.com) for users struggling with frequent authentication problems
 or unable to authenticate via [Google Authentication](https://
 developers.google.com/identity/protocols/oauth2?hl=en). Collaborated
 competently with [Antonio Cheong](https://github.com/acheong08).
+
 > [!TIP] > | 2024-03-26 | [[See Code Examples]](https://github.com/
 dsdanielpark/Gemini-API/blob/main/documents/README_OPENROUTER.md) > > Check out
 temporarily free Open-source LLM APIs with Open Router. (Free limit: 10
 requests/minute)
-
-- [ Gemini API ](#-gemini-api---) - [What is Gemini?](#what-is-gemini) -
-[Installation](#installation) - [Authentication](#authentication) - [Quick
-Start](#quick-start) - [Usage](#usage) - [# 01. Initialization](#-01-
-initialization) - [# 02. Generate content](#-02-generate-content) - [# 03. Send
-request](#-03-send-request) - [# 04. Text generation](#-04-text-generation) -
-[# 05. Image generation](#-05-image-generation) - [# 06. Retrieving Images from
-Gemini Responses](#-06-retrieving-images-from-gemini-responses) - [# 07.
-Generate content from images](#-07-generate-content-from-images) - [# 08.
-Generate content using Google Services](#-08-generate-content-using-google-
-services) - [# 09. Fix context setting rcid](#-09-fix-context-setting-rcid) -
-[# 10. Changing the Selected Response from 0 to *n*](#-10-changing-the-
-selected-response-from-0-to-n) - [# 11. Generate custom content](#-11-generate-
-custom-content) - [Further](#further) - [Open-source LLM, Gemma](#open-source-
-llm-gemma) - [How to use Gemma](#how-to-use-gemma) - [Utilize free open-source
-LLM API through Open Router](#utilize-free-open-source-llm-api-through-open-
-router)
+## Contents - [ Gemini API ](#-gemini-api---) - [What is Gemini? ð](#what-
+is-gemini) - [Installation â](#installation-) - [Authentication â]
+(#authentication) - [Quick Start â](#quick-start) - [Usage](#usage) - [# 01.
+Initialization â](#-01-initialization) - [# 02. Generate content](#-02-
+generate-content) - [# 03. Send request](#-03-send-request) - [# 04. Text
+generation](#-04-text-generation) - [# 05. Image generation](#-05-image-
+generation) - [# 06. Retrieving Images from Gemini Responses](#-06-retrieving-
+images-from-gemini-responses) - [# 07. Generate content from images](#-07-
+generate-content-from-images) - [# 08. Generate content using Google Services]
+(#-08-generate-content-using-google-services) - [# 09. Fix context setting
+RCID](#-09-fix-context-setting-rcid) - [# 10. Changing the Selected Response
+from 0 to *n*](#-10-changing-the-selected-response-from-0-to-n) - [# 11.
+Generate custom content](#-11-generate-custom-content) - [Further](#further) -
+[Google Open-source LLMs](#google-open-source-llms) - [Open-source LLM, Gemma
+ð¤](#open-source-llm-gemma) - [Open-source LLM, Code Gemma ð¤](#open-
+source-llm-code-gemma) - [Utilize free open-source LLM API through Open Router
+â](#utilize-free-open-source-llm-api-through-open-router)
 ## What is [Gemini](https://deepmind.google/technologies/gemini/#introduction)?
 | [Paper](https://arxiv.org/abs/2312.11805) | [Official Website](https://
 deepmind.google/technologies/gemini/#introduction) | [Official API](https://
 aistudio.google.com/) | [API Documents](https://cloud.google.com/vertex-ai/
 docs/generative-ai/model-reference/gemini) | Gemini is a family of generative
 AI models developed by Google DeepMind that is designed for multimodal use
 cases. The Gemini API gives you access to the Gemini Pro and Gemini Pro Vision
 models. In February 2024, Google's **Bard** service was changed to **Gemini**.
-## Installation ð¦ ``` pip install python-gemini-api ``` ``` pip install
-git+https://github.com/dsdanielpark/Gemini-API.git ``` For the updated version,
-use as follows: ``` pip install -q -U python-gemini-api ``` ## Authentication >
-[!NOTE] > Cookies can change quickly. Don't reopen the same session or repeat
-prompts too often; they'll expire faster. If the cookie value doesn't export
-correctly, refresh the Gemini page and export again. 1. Visit https://
+#### Overview of Google LLMs | Model | Type | Access | Details |:-------:|:----
+--:|:--------:|--------- [Gemini](https://huggingface.co/google/gemma-7b) |
+Proprietary | API [[13](https://ai.google.dev/tutorials/ai-studio_quickstart)]
+| A proprietary multimodal AI by Google DeepMind, including advanced models
+such as Gemini Pro and Gemini Pro Vision. Access is restricted to API usage;
+additional insights may be obtained through the paper and website. [[1](https:/
+/arxiv.org/abs/2312.11805)][[2](https://deepmind.google/technologies/gemini/
+#introduction)] [Gemma](https://huggingface.co/google/gemma-7b) | Open Source |
+[Downloadable](https://huggingface.co/google/gemma-7b)
+[Free API](https://github.com/dsdanielpark/Gemini-API?tab=readme-ov-
+file#utilize-free-open-source-llm-api-through-open-router) | An open-source
+text-to-text language model suitable for tasks like QA and summarization.
+Weights are downloadable for on-premises use, and detailed documentation is
+provided via the paper and website. [[3](https://arxiv.org/abs/2403.08295)][[4]
+(https://ai.google.dev/gemma/docs)] [Code Gemma](https://huggingface.co/google/
+codegemma-7b-it) | Open Source | [Downloadable](https://huggingface.co/google/
+codegemma-7b-it) | Designed specifically for programming tasks, this open-
+source model offers downloadable weights to assist developers with code
+generation and similar activities. Refer to the associated paper, blog post,
+and Hugging Face collection for more information. [[5](https://
+storage.googleapis.com/deepmind-media/gemma/
+codegemma_report.pdf?utm_source=substack&utm_medium=email)][[6](https://
+huggingface.co/blog/codegemma)][[7](https://huggingface.co/collections/google/
+codegemma-release-66152ac7b683e2667abdee11)]
+## What is [Python-Gemini-API](https://github.com/dsdanielpark/Gemini-API)?
+This is a Python wrapper derived from the [Bard API](https://github.com/
+dsdanielpark/Bard-API) project, designed to retrieve responses from Gemini Web
+in REST format. **Synchronous clients are preferred over asynchronous ones for
+Gemini because of rate limiting and blocking concerns.** ## Installation ð¦
+``` pip install python-gemini-api ``` ``` pip install git+https://github.com/
+dsdanielpark/Gemini-API.git ``` For the updated version, use as follows: ```
+pip install -q -U python-gemini-api ``` ## Authentication 1. Visit https://
 gemini.google.com/
 With browser open, try auto-collecting cookies first. ```python from gemini
 import Gemini GeminiClient = Gemini(auto_cookies=True) # Testing needed as
 cookies vary by region. # GeminiClient = Gemini(auto_cookies=True,
-target_cookies=["__Secure-1PSID", "__Secure-1PSIDTS"]) response =
-GeminiClient.generate_content("Hello, Gemini. What's the weather like in Seoul
-today?") print(response.payload) ``` 2. *(Manually)* `F12` for browser console
-â `Session: Application` â `Cookies` â Copy the value of some working
-cookie sets. If it doesn't work, go to step 3. Some working cookie sets Cookies
-may vary by account or region. First try `__Secure-1PSIDCC` alone. If it
-doesn't work, use `__Secure-1PSID` and `__Secure-1PSIDTS`. Still no success?
+target_cookies=["__Secure-1PSID", "__Secure-1PSIDTS"]) # GeminiClient = Gemini
+(auto_cookies=True, target_cookies="all") # You can pass whole cookies response
+= GeminiClient.generate_content("Hello, Gemini. What's the weather like in
+Seoul today?") print(response.payload) ``` 2. *(Manually)* `F12` for browser
+console â `Session: Application` â `Cookies` â Copy the value of some
+working cookie sets. If it doesn't work, go to step 3. Some working cookie sets
+Cookies may vary by account or region. First try `__Secure-1PSIDCC` alone. If
+it doesn't work, use `__Secure-1PSID` and `__Secure-1PSIDTS`. Still no success?
 Try these four cookies: `__Secure-1PSIDCC`, `__Secure-1PSID`, `__Secure-
 1PSIDTS`, `NID`. If none work, proceed to step 3 and consider sending the
 entire cookie file. 3. *(Recommended)* Export Gemini site cookies via a browser
 extension. For instance, use Chrome extension [ExportThisCookies](https://
 chromewebstore.google.com/detail/exportthiscookie/
 dannllckdimllhkiplchkcaoheibealk), open, and copy the txt file contents.
 Further: For manual collection or Required for a few users upon error 4. For
@@ -72,113 +117,104 @@
 few users upon error)* If errors persist after manually collecting cookies,
 refresh the Gemini website and collect cookies again. If errors continue, some
 users may need to manually set the nonce value. To do this: Press F12 â
 Network â Send any prompt to Gemini webui â Click the post address starting
 with "https://gemini.google.com/_/BardChatUi/data/
 assistant.lamda.BardFrontendService/StreamGenerate" â Payload â Form Data
 â Copy the "at" key value. See [this image](assets/nonce_value.pdf) for
-reference. > [!IMPORTANT] > Try different Google accounts until you find a
-working cookie. Use a fresh browser to ensure no remaining cookie values. Use
-secret browsing mode with independent cookies. Results may vary depending on
-factors like IP and account status. Providing the entire set of cookies seems
-to fix one cookie per account. Additionally, once successfully connected with
-that cookie, it seems to work flawlessly for over three weeks without any
-errors. *Try various methods until you succeed. Experiment in different
-environments.*
-## Quick Start *Simple usage* Setting Gemini response language (Optional):
-Check supported languages [here](https://developers.google.com/hotels/hotel-
-prices/dev-guide/country-codes). Default is English. ```python import os
-os.environ["GEMINI_LANGUAGE"] = "KR" ``` Generate content: returns parsed
-response. ```python from gemini import Gemini cookies = {} # Cookies may vary
-by account or region. Consider sending the entire cookie file. GeminiClient =
-Gemini(cookies=cookies) # You can use various args response =
-GeminiClient.generate_content("Hello, Gemini. What's the weather like in Seoul
-today?") response.payload ``` Generate content from image: you can use image as
-input. ```python from gemini import Gemini cookies = {} # Cookies may vary by
-account or region. Consider sending the entire cookie file. GeminiClient =
-Gemini(cookies=cookies) # You can use various args response =
-GeminiClient.generate_content("What does the text in this image say?",
-image='folder/image.jpg') response.payload ``` > [!NOTE] > If the
-generate_content method returns an empty payload, try executing it again
-without reinitializing the Gemini object.
-## Usage ### # 01. Initialization Please explicitly declare `cookies` in dict
-format. You can also enter the path to the file containing the cookie with
-`cookie_fp`(*.json, *.txt supported). Check this [sample cookie file](https://
-github.com/dsdanielpark/Gemini-API/blob/main/cookies.txt). ```python from
+reference. > [!IMPORTANT] > Experiment with different Google accounts and
+browser settings to find a working cookie. Success may vary by IP and account
+status. Once connected, a cookie typically remains effective over a month. Keep
+testing until successful.
+## Quick Start **Generate content:** returns parsed response. ```python from
+gemini import Gemini cookies = {} # Cookies may vary by account or region.
+Consider sending the entire cookie file. GeminiClient = Gemini(cookies=cookies)
+# You can use various args response = GeminiClient.generate_content("Hello,
+Gemini. What's the weather like in Seoul today?") response.payload ```
+**Generate content from image:** you can use image as input. ```python from
+gemini import Gemini cookies = {} # Cookies may vary by account or region.
+Consider sending the entire cookie file. GeminiClient = Gemini(cookies=cookies)
+# You can use various args response = GeminiClient.generate_content("What does
+the text in this image say?", image='folder/image.jpg') response.payload ``` >
+[!NOTE] > If the generate_content method returns an empty payload, try
+executing it again without reinitializing the Gemini object.
+
+## Usage *Setting language and Gemini version using environment variables:
+* Setting Gemini response language (Optional): Check supported languages [here]
+(https://developers.google.com/hotels/hotel-prices/dev-guide/country-codes).
+Default is English. ```python import os os.environ["GEMINI_LANGUAGE"] = "KR" #
+Setting Gemini response language (Optional) os.environ["GEMINI_ULTRA"] = "1" #
+Switch to Gemini-advanced response (Experimental, Optional) # In some accounts,
+access to Gemini Ultra may not be available. If that's the case, please revert
+it back to "0". ```
+### # 01. Initialization Please explicitly declare `cookies` in dict format.
+You can also enter the path to the file containing the cookie with `cookie_fp`
+(*.json, *.txt supported). Check sample cookie files in [assets](https://
+github.com/dsdanielpark/Gemini-API/tree/main/assets) folder. ```python from
 gemini import Gemini cookies = { "__Secure-1PSIDCC" : "value", "__Secure-1PSID"
 : "value", "__Secure-1PSIDTS" : "value", "NID" : "value", # Cookies may vary by
 account or region. Consider sending the entire cookie file. } GeminiClient =
 Gemini(cookies=cookies) # GeminiClient = Gemini(cookie_fp="folder/
 cookie_file.json") # (*.json, *.txt) are supported. # GeminiClient = Gemini
-(auto_cookies=True) # Or use auto_cookies paprameter ``` #### Auto Cookie
-Update For `auto_cookie` to be set to `True`, Gemini WebUI must be active in
-the browser. The [browser_cookie3](https://github.com/borisbabic/
-browser_cookie3) enables automatic cookie collection, though updates may not be
-complete yet. > [!IMPORTANT] > **If the session connects successfully and
-`generate_content` runs well, CLOSE Gemini website.** If Gemini web stays open
-in the browser, cookies may expire faster.
+(auto_cookies=True) # Or use auto_cookies paprameter ``` ##### Auto Cookie
+Update For `auto_cookie` to be set to `True`, and adjust `target_cookies`.
+Gemini WebUI must be active in the browser. The [browser_cookie3](https://
+github.com/borisbabic/browser_cookie3) enables automatic cookie collection,
+though updates may not be complete yet.
 ### # 02. Generate content Returns Gemini's response, but the first one might
-be empty. If generate_content yields an empty payload, rerun it without
-reinitializing Gemini. Regardless of model output type, access the
-response_dict property (renamed to payload after v2.3.0). https://github.com/
-dsdanielpark/Gemini-API/blob/fdf064c57bc1fb47fbbb4b93067618a200e77f62/gemini/
-core.py#L252 ```python prompt = "Hello, Gemini. What's the weather like in
-Seoul today?" response = GeminiClient.generate_content(prompt) print
-(response.payload) ``` > [!IMPORTANT] > Once connected and generating valid
-content, **Be sure to CLOSE the Gemini website or CLOSE your browser** for
-cookie stability.
+be empty. ```python prompt = "Hello, Gemini. What's the weather like in Seoul
+today?" response = GeminiClient.generate_content(prompt) print
+(response.payload) ``` > [!IMPORTANT] > DO NOT send same prompt repeatly. **If
+the session connects successfully and `generate_content` runs well, CLOSE
+Gemini website.** If Gemini web stays open in the browser, cookies may expire
+faster.
 The output of the generate_content function is `GeminiModelOutput`, with the
-following structure: **Properties of GeminiModelOutput:** - *rcid*: returns the
-response candidate id of the chosen candidate. - *text*: returns the text of
-the chosen candidate. - *code*: returns the codes of the chosen candidate. -
-*web_images*: returns a list of web images from the chosen candidate. -
-*generated_images*: returns a list of generated images from the chosen
-candidate. - *payload*: returns the response dictionary, if available. (same as
-*reponse_dict* under v2.3.0) https://github.com/dsdanielpark/Gemini-API/blob/
-fdf064c57bc1fb47fbbb4b93067618a200e77f62/gemini/src/model/output.py#L16 >
-[!NOTE] > If the session fails to connect, works improperly, or terminates,
-returning an error, it is recommended to manually renew the cookies. The error
-is likely due to incorrect cookie values. Refresh or log out of Gemini web to
-renew cookies and try again.
+following structure: - *rcid*: returns the response candidate id of the chosen
+candidate. - *text*: returns the text of the chosen candidate. - *code*:
+returns the codes of the chosen candidate. - *web_images*: returns a list of
+web images from the chosen candidate. - *generated_images*: returns a list of
+generated images from the chosen candidate. - *payload*: returns the response
+dictionary, if available. https://github.com/dsdanielpark/Gemini-API/blob/
+fdf064c57bc1fb47fbbb4b93067618a200e77f62/gemini/src/model/output.py#L16
 ### # 03. Send request Send request: returns the request's payload and
 status_code, making debugging easier. ```python from gemini import Gemini
 cookies = {} # Cookies may vary by account or region. Consider sending the
 entire cookie file. GeminiClient = Gemini(cookies=cookies) # You can use
 various args response_text, response_status = GeminiClient.send_request("Hello,
-Gemini. What's the weather like in Seoul today?") print(response_text) ```
+Gemini. What's the weather like in Seoul today?") print(response_text) ``` You
+can track the total number of requests made by accessing the `request_count`
+property within the `Gemini` class.
 ### # 04. Text generation Returns text generated by Gemini. ```python prompt =
 "Hello, Gemini. What's the weather like in Seoul today?" response =
 GeminiClient.generate_content(prompt) print(response.text) ```
-### # 05. Image generation Returns images generated by Gemini. https://
-github.com/dsdanielpark/Gemini-API/blob/
-fdf064c57bc1fb47fbbb4b93067618a200e77f62/gemini/src/model/image.py#L12 *Sync
-downloader* ```python from gemini import Gemini, GeminiImage response =
-GeminiClient.generate_content("Create illustrations of Seoul, South Korea.")
-generated_images = response.generated_images # Check generated images [Dict]
-GeminiImage.save_sync(generated_images, save_path="save_dir", cookies=cookies)
-# You can use byte type image dict for printing images as follow: #
-bytes_images_dict = GeminiImage.fetch_images_dict_sync(generated_images,
-cookies=cookies) # Get bytes images dict # GeminiImage.save_images_sync
-(bytes_images_dict, path="save_dir", cookies=cookies) # Save to path ```
-Display images in IPython You can display the image or transmit it to another
-application in byte format. ``` bytes_images_dict =
+### # 05. Image generation Returns images generated by Gemini. *Async
+downloader* ```python response = GeminiClient.generate_content("Create
+illustrations of Seoul, South Korea.") generated_images =
+response.generated_images # Check generated images [Dict] await
+GeminiImage.save(generated_images, "save_dir", cookies=cookies) #
+image_data_dict = await GeminiImage.fetch_images_dict(generated_images,
+cookies=cookies) # await GeminiImage.save_images(image_data_dict, "save_dir")
+``` Further *Display images in IPython* You can display the image or transmit
+it to another application in byte format. ```python bytes_images_dict =
 GeminiImage.fetch_images_dict_sync(generated_images, cookies) # Get bytes
 images dict from IPython.display import display, Image import io for
 image_name, image_bytes in bytes_images_dict.items(): print(image_name) image =
-Image(data=image_bytes) display(image) ``` *Async downloader* ```python
-response = GeminiClient.generate_content("Create illustrations of Seoul, South
-Korea.") generated_images = response.generated_images # Check generated images
-[Dict] await GeminiImage.save(generated_images, "save_dir", cookies=cookies) #
-image_data_dict = await GeminiImage.fetch_images_dict(generated_images,
-cookies=cookies) # await GeminiImage.save_images(image_data_dict, "save_dir")
-``` Async downloader wrapper ``` import asyncio from gemini import Gemini,
-GeminiImage async def save_generated_imagse(generated_imagse,
-save_path="save_dir", cookies=cookies): await GeminiImage.save
-(generated_imagse, save_path=save_path, cookies=cookies) # Run the async
-function if __name__ == "__main__": cookies = {"key" : "value"}
+Image(data=image_bytes) display(image) ``` *Sync downloader* ```python from
+gemini import Gemini, GeminiImage response = GeminiClient.generate_content
+("Create illustrations of Seoul, South Korea.") generated_images =
+response.generated_images # Check generated images [Dict] GeminiImage.save_sync
+(generated_images, save_path="save_dir", cookies=cookies) # You can use byte
+type image dict for printing images as follow: # bytes_images_dict =
+GeminiImage.fetch_images_dict_sync(generated_images, cookies=cookies) # Get
+bytes images dict # GeminiImage.save_images_sync(bytes_images_dict,
+path="save_dir", cookies=cookies) # Save to path ``` *Async downloader wrapper*
+```python import asyncio from gemini import Gemini, GeminiImage async def
+save_generated_imagse(generated_imagse, save_path="save_dir", cookies=cookies):
+await GeminiImage.save(generated_imagse, save_path=save_path, cookies=cookies)
+# Run the async function if __name__ == "__main__": cookies = {"key" : "value"}
 generated_imagse = response.generated_imagse asyncio.run(save_generated_imagse
 (generated_imagse, save_path="save_dir", cookies=cookies)) ```
 `GeminiImage.save` method logic ``` import asyncio from gemini import Gemini,
 GeminiImage async def save_generated_imagse(generated_imagse,
 save_path="save_dir", cookies=cookies): image_data_dict = await
 GeminiImage.fetch_images_dict(generated_imagse, cookies=cookies) # Get bytes
 images dict asynchronously await GeminiImage.save_images(image_data_dict,
@@ -187,38 +223,38 @@
 Check response images [Dict] asyncio.run(save_generated_imagse
 (generated_imagse, save_path="save_dir", cookies=cookies)) ``` > [!NOTE] > Use
 GeminiImage for image processing. `web_images` works without cookies, but for
 images like `generated_image` from Gemini, pass cookies. Cookies are needed to
 download images from Google's storage. Check the response or use existing
 cookies variable.
 ### # 06. Retrieving Images from Gemini Responses Returns images in response of
-Gemini. *Sync downloader* ```python from gemini import Gemini, GeminiImage
-response = GeminiClient.generate_content("Please recommend a travel itinerary
-for Seoul.") response_images = response.web_images # Check response images
-[Dict] GeminiImage.save_sync(response_images, save_path="save_dir") # You can
-use byte type image dict as follow: # bytes_images_dict =
-GeminiImage.fetch_bytes_sync(response_images, cookies) # Get bytes images dict
-# GeminiImage.save_images_sync(bytes_images_dict, path="save_dir") # Save to
-path ``` *Async downloader* ```python response = GeminiClient.generate_content
+Gemini. *Async downloader* ```python response = GeminiClient.generate_content
 ("Create illustrations of Seoul, South Korea.") response_images =
 response.web_images # Check generated images [Dict] await GeminiImage.save
 (response_images, "save_dir") # image_data_dict = await
 GeminiImage.fetch_images_dict(response_images) # await GeminiImage.save_images
-(image_data_dict, "save_dir") ``` Async downloader wrapper ``` import asyncio
-from gemini import Gemini, GeminiImage async def save_response_web_imagse
-(response_images, save_path="save_dir", cookies=cookies): await
-GeminiImage.save(response_images, save_path=save_path, cookies=cookies) # Run
-the async function if __name__ == "__main__": cookies = {"key" : "value"}
-response_images = response.web_images asyncio.run(save_response_web_imagse
-(response_images, save_path="save_dir", cookies=cookies)) ```
-`GeminiImage.save` method logic ``` import asyncio from gemini import Gemini,
-GeminiImage async def save_response_web_imagse(response_images,
-save_path="save_dir", cookies=cookies): image_data_dict = await
-GeminiImage.fetch_images_dict(response_images, cookies=cookies) # Get bytes
-images dict asynchronously await GeminiImage.save_images(image_data_dict,
+(image_data_dict, "save_dir") ``` Further *Sync downloader* ```python from
+gemini import Gemini, GeminiImage response = GeminiClient.generate_content
+("Please recommend a travel itinerary for Seoul.") response_images =
+response.web_images # Check response images [Dict] GeminiImage.save_sync
+(response_images, save_path="save_dir") # You can use byte type image dict as
+follow: # bytes_images_dict = GeminiImage.fetch_bytes_sync(response_images,
+cookies) # Get bytes images dict # GeminiImage.save_images_sync
+(bytes_images_dict, path="save_dir") # Save to path ``` *Async downloader
+wrapper* ```python import asyncio from gemini import Gemini, GeminiImage async
+def save_response_web_imagse(response_images, save_path="save_dir",
+cookies=cookies): await GeminiImage.save(response_images, save_path=save_path,
+cookies=cookies) # Run the async function if __name__ == "__main__": cookies =
+{"key" : "value"} response_images = response.web_images asyncio.run
+(save_response_web_imagse(response_images, save_path="save_dir",
+cookies=cookies)) ``` `GeminiImage.save` method logic ``` import asyncio from
+gemini import Gemini, GeminiImage async def save_response_web_imagse
+(response_images, save_path="save_dir", cookies=cookies): image_data_dict =
+await GeminiImage.fetch_images_dict(response_images, cookies=cookies) # Get
+bytes images dict asynchronously await GeminiImage.save_images(image_data_dict,
 save_path=save_path) # Run the async function if __name__ == "__main__":
 response_images = response.web_images # Check response images [Dict]
 asyncio.run(save_response_web_imagse(response_images, save_path="save_dir",
 cookies=cookies)) ```
 ### # 07. Generate content from images Takes an image as input and returns a
 response. ```python image = 'folder/image.jpg' # image = open('folder/
 image.jpg', 'rb').read() # (jpg, jpeg, png, webp) are supported. response =
@@ -244,93 +280,111 @@
 tailored travel itineraries. - Features: Holiday preparation, price comparison,
 trip planning - Google Hotels - Service: **@Google Hotels** - Description:
 Search for hotels considering what matters most to you, like having a
 conversation with a friend. - Features: Packing for travel, sightseeing,
 special relaxation - YouTube - Service: **@YouTube** - Description: Explore
 YouTube videos and ask questions about what interests you. - Features: Problem-
 solving, generating ideas, search, exploring topics
-### # 09. Fix context setting rcid You can specify a particular response by
-setting its response candidate id(rcid). ```python # Generate content for the
+### # 09. Fix context setting RCID You can specify a particular response by
+setting its Response Candidate ID(RCID). ```python # Generate content for the
 prompt "Give me some information about the USA." response1 =
 GeminiClient.generate_content("Give me some information about the USA.") #
 After reviewing the responses, choose the one you prefer and copy its RCID.
 GeminiClient.rcid = "rc_xxxx" # Now, generate content for the next prompt "How
 long does it take from LA to New York?" response2 =
-GeminiClient.generate_content("How long does it take from LA to New York?") ```
-
+GeminiClient.generate_content("How long does it take from LA to New York?") #
+However, RCID may not persist. If parsing fails, reset `GeminiClient.rcid` to
+None. # GeminiClient.rcid = None ```
 ### # 10. Changing the Selected Response from 0 to *n* In Gemini,
 generate_content returns the first response. This may vary depending on length
 or sorting. Therefore, you can specify the index of the chosen response from 0
 to *n* as follows. However, if there is only one response, revert it back to 0.
 ```python from gemini import GeminiModelOutput GeminiModelOutput.chosen = 1 #
-default is 0 response1 = GeminiClient.generate_content("Give me some
-information about the USA.") ```
+default is 0 response_choice_1 = GeminiClient.generate_content("Give me some
+information about the USA.") # If not all Gemini returns are necessarily
+plural, revert back to 0 in case of errors. # GeminiModelOutput.chosen = 0 ```
 ### # 11. Generate custom content Parse the response text to extract desired
-values. https://github.com/dsdanielpark/Gemini-API/blob/
-fdf064c57bc1fb47fbbb4b93067618a200e77f62/gemini/core.py#L317 Using
-`Gemini.generate_custom_content`, specify custom parsing to extract specific
-values. Utilize ParseMethod1 and ParseMethod2 by default, and you can pass
-custom parsing methods as arguments if desired. Refer to [custom_parser.py]
-(https://github.com/dsdanielpark/Gemini-API/blob/main/gemini/src/model/parser/
-custom_parser.py). ```python # You can create a parser method that takes
-response_text as the input for custom_parser. response_text, response_status =
-GeminiClient.send_request("Give me some information about the USA.") # Use
-custom_parser function or class inheriting from BaseParser response =
-GeminiClient.generate_custom_content("Give me some information about the USA.",
-*custom_parser) ```
-## Further ### Use rotating proxies If you want to **avoid blocked requests**
-and bans, then use [Smart Proxy by Crawlbase](https://crawlbase.com/docs/smart-
-proxy/?utm_source=github_ad&utm_medium=social&utm_campaign=bard_api). It
-forwards your connection requests to a **randomly rotating IP address** in a
-pool of proxies before reaching the target website. The combination of AI and
-ML make it more effective to avoid CAPTCHAs and blocks. ```python # Get your
-proxy url at crawlbase https://crawlbase.com/docs/smart-proxy/get/ proxy_url =
-"http://xxxxx:@smartproxy.crawlbase.com:8012" proxies = {"http": proxy_url,
-"https": proxy_url} GeminiClient = Gemini(cookies=cookies, proxies=proxies,
-timeout=30) GeminiClient.generate_content("Hello, Gemini. Give me a beautiful
-photo of Seoul's scenery.") ``` ### Reusable session object For standard cases,
-use Gemini class; for exceptions, use session objects. When creating a new bot
-Gemini server, adjust Headers.MAIN. ```python from gemini import Gemini,
-Headers import requests cookies = {} session = requests.Session()
+values. Using `Gemini.generate_custom_content`, specify custom parsing to
+extract specific values. Utilize ParseMethod1 and ParseMethod2 by default, and
+you can pass custom parsing methods as arguments if desired. Refer to
+[custom_parser.py](https://github.com/dsdanielpark/Gemini-API/blob/main/gemini/
+src/model/parser/custom_parser.py). ```python # You can create a parser method
+that takes response_text as the input for custom_parser. response_text,
+response_status = GeminiClient.send_request("Give me some information about the
+USA.") # Use custom_parser function or class inheriting from BaseParser
+response = GeminiClient.generate_custom_content("Give me some information about
+the USA.", *custom_parser) ``` https://github.com/dsdanielpark/Gemini-API/blob/
+31b842488bbc5429ad9c74b1d8b00e20d94e8cb1/gemini/client.py#L323
+## Further ### Use rotating proxies via [Smart Proxy by Crawlbase](https://
+crawlbase.com/docs/smart-proxy/
+?utm_source=github_ad&utm_medium=social&utm_campaign=bard_api) If you want to
+**avoid blocked requests** and bans, then use [Smart Proxy by Crawlbase](https:
+//crawlbase.com/docs/smart-proxy/
+?utm_source=github_ad&utm_medium=social&utm_campaign=bard_api). It forwards
+your connection requests to a **randomly rotating IP address** in a pool of
+proxies before reaching the target website. The combination of AI and ML make
+it more effective to avoid CAPTCHAs and blocks. ```python # Get your proxy url
+at crawlbase https://crawlbase.com/docs/smart-proxy/get/ proxy_url = "http://
+xxxxx:@smartproxy.crawlbase.com:8012" proxies = {"http": proxy_url, "https":
+proxy_url} GeminiClient = Gemini(cookies=cookies, proxies=proxies, timeout=30)
+GeminiClient.generate_content("Hello, Gemini. Give me a beautiful photo of
+Seoul's scenery.") ``` ### Reusable session object For standard cases, use
+Gemini class; for exceptions, use session objects. When creating a new bot
+Gemini server, adjust Headers.MAIN. ```python import requests from gemini
+import Gemini, Headers cookies = {} session = requests.Session()
 session.headers = Headers.MAIN for key, value in cookies.items():
 session.cookies.update({key: value}) GeminiClient = Gemini(session=session) #
 You can use various args response = GeminiClient.generate_content("Hello,
 Gemini. What's the weather like in Seoul today?") ```
 ## [More features](https://github.com/dsdanielpark/Gemini-API/blob/main/
 documents/README_DEV.md) Explore additional features in [this document](https:/
 /github.com/dsdanielpark/Gemini-API/blob/main/documents/README_DEV.md). If you
 want to develop your own simple code, you can start from [this simple code
 example](https://github.com/dsdanielpark/Gemini-API/blob/main/script/
 sample.ipynb).
-## Open-source LLM, [Gemma](https://huggingface.co/google/gemma-7b) If you have
-sufficient GPU resources, you can download weights directly instead of using
-the Gemini API to generate content. Consider Gemma, an open-source model
-**available for on-premises use**. [Gemma](https://huggingface.co/google/gemma-
-7b) models are Google's lightweight, advanced text-to-text, decoder-only
-language models, derived from Gemini research. Available in English, they offer
-open weights and variants, ideal for tasks like question answering and
-summarization. Their small size enables deployment in resource-limited
-settings, broadening access to cutting-edge AI. For more infomation, visit
-[Gemma-7b](https://huggingface.co/google/gemma-7b) model card. ### How to use
-Gemma ```python from transformers import AutoTokenizer, AutoModelForCausalLM
-tokenizer = AutoTokenizer.from_pretrained("google/gemma-7b") model =
+## Google Open-source LLMs If you have sufficient GPU resources, you can
+download weights directly instead of using the Gemini API to generate content.
+Consider Gemma and Code Gemma, an open-source models **available for on-
+premises use**. ### Open-source LLM, [Gemma](https://huggingface.co/google/
+gemma-7b) Gemma models are Google's lightweight, advanced text-to-text,
+decoder-only language models, derived from Gemini research. Available in
+English, they offer open weights and variants, ideal for tasks like question
+answering and summarization. For more infomation, visit [Gemma-7b](https://
+huggingface.co/google/gemma-7b) model card. #### How to use Gemma ```python
+from transformers import AutoTokenizer, AutoModelForCausalLM tokenizer =
+AutoTokenizer.from_pretrained("google/gemma-7b") model =
 AutoModelForCausalLM.from_pretrained("google/gemma-7b") input_text = "Write me
 a poem about Machine Learning." input_ids = tokenizer(input_text,
 return_tensors="pt") outputs = model.generate(**input_ids) print
+(tokenizer.decode(outputs[0])) ``` ### Open-source LLM, [Code Gemma](https://
+huggingface.co/collections/google/codegemma-release-66152ac7b683e2667abdee11)
+CodeGemma, which is an official release from Google for code LLMs, was released
+on April 9, 2024. It provides three models specifically designed for generating
+and interacting with code. You can explore the [Code Gemma models](https://
+huggingface.co/collections/google/codegemma-release-66152ac7b683e2667abdee11)
+and view the [model card](https://huggingface.co/google/codegemma-7b-it) for
+more details. #### How to use Code Gemma ```python from transformers import
+GemmaTokenizer, AutoModelForCausalLM tokenizer = GemmaTokenizer.from_pretrained
+("google/codegemma-7b-it") model = AutoModelForCausalLM.from_pretrained
+("google/codegemma-7b-it") input_text = "Write me a Python function to
+calculate the nth fibonacci number." input_ids = tokenizer(input_text,
+return_tensors="pt") outputs = model.generate(**input_ids) print
 (tokenizer.decode(outputs[0])) ```
 ## Utilize free open-source LLM API through [Open Router](https://
 openrouter.ai/) OpenRouter offers temporary free inference for select models.
 Obtain an API key from [Open Router API](https://openrouter.ai/keys) and check
 free models at [Open Router models](https://openrouter.ai/docs#models). Use
 models with a 0-dollar token cost primarily; other models may incur charges.
-See more [free open-source LLM API guide](https://github.com/dsdanielpark/
-Gemini-API/blob/main/documents/README_OPENROUTER.md) > [!NOTE] > You can easily
-receive responses from open LLMs without this package by following the
-instructions on [here](https://openrouter.ai/docs#models). ```python from
-gemini import OpenRouter OPENROUTER_API_KEY = "" GemmaClient = OpenRouter
+See more at [free open-source LLM API guide](https://github.com/dsdanielpark/
+Gemini-API/blob/main/documents/README_OPENROUTER.md). **Sync client is favored
+over async for Gemini due to rate limiting and blocking issues**, but
+OpenRouter offers reliable open-source LLMs for [async implementation](https://
+github.com/dsdanielpark/Gemini-API/blob/main/documents/
+README_OPENROUTER.md#openrouter-async-api-client). ```python from gemini import
+OpenRouter OPENROUTER_API_KEY = "" GemmaClient = OpenRouter
 (api_key=OPENROUTER_API_KEY, model="google/gemma-7b-it:free") prompt = "Do you
 know UCA academy in Korea? https://blog.naver.com/ulsancoding" response =
 GemmaClient.create_chat_completion(prompt) print(response) # payload =
 GemmaClient.generate_content(prompt) # print(payload.json()) ``` The free model
 list includes: - `google/gemma-7b-it:free` - [google/gemma-7b](https://
 huggingface.co/google/gemma-7b) from Google *** - `mistralai/mistral-7b-
 instruct:free` - [mistralai/Mistral-7B-Instruct-v0.1](https://huggingface.co/
@@ -341,38 +395,38 @@
 `openrouter/cinematika-7b:free` - [jondurbin/cinematika-7b-v0.1](https://
 huggingface.co/jondurbin/cinematika-7b-v0.1) - `undi95/toppy-m-7b:free` -
 [Undi95/Toppy-M-7B](https://huggingface.co/Undi95/Toppy-M-7B?not-for-all-
 audiences=true) - `gryphe/mythomist-7b:free` - [Gryphe/MythoMist-7b](https://
 huggingface.co/Gryphe/MythoMist-7b) - `nousresearch/nous-capybara-7b:free` -
 [NousResearch/Nous-Capybara-7B-V1](https://huggingface.co/NousResearch/Nous-
 Capybara-7B-V1) from Nous Research
+## Sponsor, [Crawlbase](https://crawlbase.com/) Use [Crawlbase](https://
+crawlbase.com/) API for efficient data scraping to train AI models, boasting a
+98% success rate and 99.9% uptime. It's quick to start, GDPR/CCPA compliant,
+supports massive data extraction, and is trusted by 70k+ developers.
 ## [FAQ](https://github.com/dsdanielpark/Gemini-API/blob/main/documents/
 README_FAQ.md) First review [HanaokaYuzu/Gemini-API](https://github.com/
 HanaokaYuzu/Gemini-API) and the [Official Google Gemini API](https://
 aistudio.google.com/) before using this package. You can find most help on the
 [FAQ](https://github.com/dsdanielpark/Gemini-API/blob/main/documents/
 README_FAQ.md) and [Issue](https://github.com/dsdanielpark/Gemini-API/issues)
 pages. ## [Issues](https://github.com/dsdanielpark/Gemini-API/issues) Sincerely
 grateful for any reports on new features or bugs. Your valuable feedback on the
 code is highly appreciated. Frequent errors may occur due to changes in
 Google's service API interface. Both [Issue reports](https://github.com/
 dsdanielpark/Gemini-API/issues) and [Pull requests](https://github.com/
 dsdanielpark/Gemini-API/pulls) contributing to improvements are always welcome.
-We strive to maintain an active and courteous open community. ## Sponsor Use
-[Crawlbase](https://crawlbase.com/) API for efficient data scraping to train AI
-models, boasting a 98% success rate and 99.9% uptime. It's quick to start,
-GDPR/CCPA compliant, supports massive data extraction, and is trusted by 70k+
-developers. ## Contributors We would like to express our sincere gratitude to
-all the contributors. This package aims to re-implement the functionality of
-the [Bard API](https://github.com/dsdanielpark/Bard-API/), which has been
-archived for the contributions of the beloved open-source community, despite
-Gemini's official API already being available. Contributors to the [Bard API]
-(https://github.com/dsdanielpark/Bard-API/) and [Gemini API](https://
-github.com/dsdanielpark/Gemini-API/). _[_h_t_t_p_s_:_/_/_c_o_n_t_r_i_b_._r_o_c_k_s_/
-_i_m_a_g_e_?_r_e_p_o_=_d_s_d_a_n_i_e_l_p_a_r_k_/_B_a_r_d___A_P_I_]
+We strive to maintain an active and courteous open community. ## Contributors
+We would like to express our sincere gratitude to all the contributors. This
+package aims to re-implement the functionality of the [Bard API](https://
+github.com/dsdanielpark/Bard-API/), which has been archived for the
+contributions of the beloved open-source community, despite Gemini's official
+API already being available. Contributors to the [Bard API](https://github.com/
+dsdanielpark/Bard-API/) and [Gemini API](https://github.com/dsdanielpark/
+Gemini-API/). _[_h_t_t_p_s_:_/_/_c_o_n_t_r_i_b_._r_o_c_k_s_/_i_m_a_g_e_?_r_e_p_o_=_d_s_d_a_n_i_e_l_p_a_r_k_/_B_a_r_d___A_P_I_]
 Further development potential Modifications to the async client using my logic
 are needed, along with automatic cookie collection via browser_cookie3, and
 implementation of other Bard API features (such as code extraction, export to
 Replit, graph drawing, etc.). Please note that while reviewing automatic cookie
 collection, it appears that cookies expire immediately upon sending a request
 for collection. Efforts to make it more user-friendly were unsuccessful. Also,
 the _sid value seems to work normally even when returned as None. Lastly, if
@@ -384,21 +438,38 @@
 Cheong](https://github.com/acheong08) / teapotv8@proton.me
 - [Daniel Park](https://github.com/DSDanielPark) / parkminwoo1991@gmail.com ##
 License Â©ï¸ [MIT](https://opensource.org/license/mit/) license, 2024. We
 hereby strongly disclaim any explicit or implicit legal liability related to
 our works. Users are required to use this package responsibly and at their own
 risk. This project is a personal initiative and is not affiliated with or
 endorsed by Google. It is recommended to use Google's official API. ##
-References [1] Github: [acheong08/Bard](https://github.com/acheong08/Bard)
-[2] GitHub: [HanaokaYuzu/Gemini-API](https://github.com/HanaokaYuzu/Gemini-API)
-
-[3] Github: [dsdanielpark/Bard-API](https://github.com/dsdanielpark/Bard-API)
-[4] Github: [GoogleCloudPlatform/generative-ai](https://github.com/
+References [1]: Paper - [Introducing GEMINI: Multimodal Generative Models]
+(https://arxiv.org/abs/2312.11805)
+[2]: Website - [Google DeepMind :: GEMINI Introduction](https://
+deepmind.google/technologies/gemini/#introduction)
+[3]: Paper - [GEMMA: A Unified Language Model for Text Generation,
+Understanding, Translation, Coding, and Math.]()
+[4]: Website - [AI at Google :: GEMS Documentation](https://ai.google.dev/
+gemma/docs)
+[5]: Report - [CodeGMMA: Large Language Models Can Write Realistic Programming
+Assignments](https://storage.googleapis.com/deepmind-media/gemma/
+codegemma_report.pdf?utm_source=substack&utm_medium=email)
+[6]: Blog Post - [Announcing CodeGen: Building Better Developersâ Tools Using
+LLMs](https://huggingface.co/blog/codegen)
+[7]: Collection - [Google :: CodeGen Release](https://huggingface.co/
+collections/google/codegen-release-5d0f4c4eaedbc5cefcfdcbdf)
+[8]: Github - [acheong08/Bard](https://github.com/acheong08/Bard)
+[9]: GitHub - [HanaokaYuzu/Gemini-API](https://github.com/HanaokaYuzu/Gemini-
+API)
+[10]: Github - [dsdanielpark/Bard-API](https://github.com/dsdanielpark/Bard-
+API)
+[11]: Github - [GoogleCloudPlatform/generative-ai](https://github.com/
 GoogleCloudPlatform/generative-ai)
-[5] Github: [OpenRouter](https://github.com/OpenRouterTeam/openrouter-runner)
-[6] WebSite: [Google AI Studio](https://ai.google.dev/tutorials/ai-
+[12]: Github - [OpenRouter](https://github.com/OpenRouterTeam/openrouter-
+runner)
+[13]: WebSite - [Google AI Studio](https://ai.google.dev/tutorials/ai-
 studio_quickstart)
 > *Warning* Users assume full legal responsibility for GeminiAPI. Not endorsed
 by Google. Excessive use may lead to account restrictions. Changes in policies
 or account status may affect functionality. Utilize issue and discussion pages.
 
 ## Requirements Python 3.7 or higher.
```

### Comparing `python-gemini-api-2.4.2/gemini/async_client.py` & `python_gemini_api-2.4.3/gemini/async_client.py`

 * *Files identical despite different names*

### Comparing `python-gemini-api-2.4.2/gemini/client.py` & `python_gemini_api-2.4.3/gemini/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,25 +2,28 @@
 import re
 import json
 import random
 import string
 import inspect
 import requests
 import urllib.parse
-from typing import Optional, Tuple, Dict, Union, List
 from requests.exceptions import ConnectionError
+from typing import Optional, Tuple, Dict, Union, List
 
-from .src.model.parser.custom_parser import ParseMethod1, ParseMethod2
+from .src.misc.utils import upload_image, load_cookies
 from .src.model.parser.response_parser import ResponseParser
 from .src.model.output import GeminiCandidate, GeminiModelOutput
-from .src.misc.utils import upload_image
+from .src.model.parser.custom_parser import ParseMethod1, ParseMethod2
+from .src.misc.exceptions import GeminiAPIError
+
 from .src.misc.constants import (
     URLs,
     Headers,
     TARGET_COOKIES,
+    WHOLE_COOKIES,
     SUPPORTED_BROWSERS,
 )
 
 
 class Gemini:
     """
     A class to manage interactions with a web service, handling sessions, cookies, and proxies.
@@ -52,14 +55,15 @@
         target_cookies: List = None,
         timeout: int = 30,
         proxies: Optional[dict] = None,
     ) -> None:
         """
         Initializes the Gemini object with session, cookies, and other configurations.
         """
+        self._request_count = 0
         self._nonce = None  # SNlM0e nonce value
         self._sid = None  # session id
         self._rcid = None  # response candidate id
         self._rid = None  # response id
         self._cid = None  # candidate id
         self._reqid = int("".join(random.choices(string.digits, k=7)))  # request id
         self.auto_cookies = auto_cookies
@@ -69,14 +73,18 @@
         self.proxies = proxies or {}
         self.timeout = timeout
         self.session = session or self._initialize_session()
         self.base_url: str = URLs.BASE_URL.value
         self.parser = ResponseParser(cookies=self.cookies)
 
     @property
+    def request_count(self) -> int:
+        return self._request_count
+
+    @property
     def nonce(self) -> Optional[str]:
         return self._nonce
 
     @nonce.setter
     def nonce(self, value: Optional[str]) -> None:
         if value != self._nonce:
             self._nonce = value
@@ -114,35 +122,31 @@
         self._set_sid_and_nonce()
 
         return session
 
     def _set_cookies_from_file(self, file_path: str) -> None:
         """Loads cookies from a file and updates the session."""
         try:
-            if file_path.endswith(".json"):
-                with open(file_path, "r") as file:
-                    cookies = json.load(file)
-            else:
-                with open(file_path, "r") as file:
-                    content = file.read()
-                    try:
-                        cookies = eval(content)
-                    except NameError:
-                        cookies = json.loads(content.replace("'", '"'))
-            self.session.cookies.update(cookies)
+            cookies = load_cookies(file_path)
         except Exception as e:
-            print(f"Error loading cookie file: {e}")
+            raise Exception(f"Failed to load cookies from {file_path}: {e}")
+
+        self.session.cookies.update(cookies)
 
     def _set_sid_and_nonce(self):
         """
         Retrieves the session ID (SID) and a SNlM0e nonce value from the application page.
         """
         try:
             response = requests.get(f"{URLs.BASE_URL.value}/app", cookies=self.cookies)
-            print(response)
+            if response.status_code != 200:
+                raise GeminiAPIError(
+                    f"Gemini API Error: Response code {response.status_code}\nExcessive connections may have temporarily blocked your account/IP, but web UI should remain accessible."
+                )
+
             response.raise_for_status()
 
             sid_match = re.search(r'"FdrFJe":"([\d-]+)"', response.text)
             nonce_match = re.search(r'"SNlM0e":"(.*?)"', response.text)
 
             if sid_match:
                 self._sid = sid_match.group(1)
@@ -223,14 +227,15 @@
             },
         )
 
     def send_request(
         self, prompt: str, image: Union[bytes, str] = None
     ) -> Tuple[str, int]:
         """Sends a request and returns the response text and status code."""
+        self._request_count += 1
         params = self._construct_params(self._sid)
         data = self._construct_payload(prompt, image, self._nonce)
         response = self.session.post(
             URLs.POST_ENDPOINT.value,
             params=params,
             data=data,
             timeout=self.timeout,
@@ -395,14 +400,15 @@
 
     #     except Exception as e:
     #         raise ConnectionError(
     #             f"Failed to retrive SID or Nonce valuse:\n{e}"
     #         )
 
     # To-Do: Get cookie values automatically.
+
     def _set_cookies_automatically(self) -> None:
         """
         Updates the instance's cookies attribute with Gemini API tokens, either from environment variables or by extracting them from the browser, based on the auto_cookies flag.
         """
         if not self.auto_cookies and self.cookies is not None:
             return
 
@@ -427,20 +433,24 @@
 
         if not self.cookies:
             raise Exception(
                 "Gemini cookies must be provided through environment variables or extracted from the browser with auto_cookies enabled."
             )
 
         # Delete non-target cookies
-        if self.target_cookies == None:
-            self.cookies = {
-                key: value
-                for key, value in self.cookies.items()
-                if key in TARGET_COOKIES
-            }
+        if isinstance(self.target_cookies, list):
+            filter_set = set(self.target_cookies)
+        elif self.target_cookies == "all":
+            filter_set = WHOLE_COOKIES
+        else:
+            filter_set = TARGET_COOKIES
+
+        self.cookies = {
+            key: value for key, value in self.cookies.items() if key in filter_set
+        }
 
     # To-Do: Get cookie values automatically.
     def _update_cookies_from_browser(self) -> dict:
         """
         Attempts to extract specific Gemini cookies from the cookies stored by web browsers on the current system.
 
         This method iterates over a predefined list of supported browsers, attempting to retrieve cookies that match a specific domain (e.g., ".google.com"). If the required cookies are found, they are added to the instance's cookie store. The process supports multiple modern web browsers across different operating systems.
```

### Comparing `python-gemini-api-2.4.2/gemini/src/extensions/replit.py` & `python_gemini_api-2.4.3/gemini/src/extensions/replit.py`

 * *Files identical despite different names*

### Comparing `python-gemini-api-2.4.2/gemini/src/misc/constants.py` & `python_gemini_api-2.4.3/gemini/src/misc/constants.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,42 @@
-from enum import Enum
+from enum import Enum, auto
 import browser_cookie3
 
 
-TARGET_COOKIES = ["__Secure-1PSIDCC", " __Secure-1PSID", "__Secure-1PSIDTS", "NID"]
+class CookieNames(Enum):
+    SEARCH_SAMESITE = auto()
+    SID = auto()
+    SECURE_1PSID = auto()
+    SECURE_3PSID = auto()
+    HSID = auto()
+    SSID = auto()
+    APISID = auto()
+    SAPISID = auto()
+    SECURE_1PAPISID = auto()
+    SECURE_3PAPISID = auto()
+    _GA = auto()
+    AEC = auto()
+    _GA_WC57KJ50ZZ = auto()
+    _1P_JAR = auto()
+    NID = auto()
+    SECURE_1PSIDTS = auto()
+    SECURE_3PSIDTS = auto()
+    SIDCC = auto()
+    SECURE_1PSIDCC = auto()
+    SECURE_3PSIDCC = auto()
+
+
+TARGET_COOKIES = [
+    CookieNames.SECURE_1PSIDCC.name,
+    CookieNames.SECURE_1PSID.name,
+    CookieNames.SECURE_1PSIDTS.name,
+    CookieNames.NID.name,
+]
+
+WHOLE_COOKIES = [cookie.name for cookie in CookieNames]
 
 
 class URLs(Enum):
     BASE_URL = "https://gemini.google.com"
     POST_ENDPOINT = f"{BASE_URL}/_/BardChatUi/data/assistant.lamda.BardFrontendService/StreamGenerate"
     SHARE_ENDPOINT = "https://clients6.google.com/upload/drive/v3/"
     BOT_SERVER = "boq_assistant-bard-web-server_20240227.13_p0"
```

### Comparing `python-gemini-api-2.4.2/gemini/src/misc/decorator.py` & `python_gemini_api-2.4.3/gemini/src/misc/decorator.py`

 * *Files identical despite different names*

### Comparing `python-gemini-api-2.4.2/gemini/src/misc/utils.py` & `python_gemini_api-2.4.3/gemini/src/misc/utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,45 @@
+import json
 import requests
 from typing import Union
 from gemini.src.misc.constants import Headers
 
 
+def load_cookies(file_path):
+    """
+    Reads a text file and tries to parse it into a Python dictionary.
+    Assumes the file might contain a cookies string or is in JSON format.
+
+    :param file_path: Path to the file containing cookie data
+    :return: A dictionary containing cookie data
+    """
+    with open(file_path, "r") as file:
+        content = file.read().strip()
+
+    # If content includes '=', assume it's a cookie string
+    if "=" in content:
+        try:
+            # Split at the first '=' and prepare for JSON parsing
+            json_str = content.split("=", 1)[1].strip()
+            json_str = json_str.replace(
+                "'", '"'
+            )  # Replace single quotes with double quotes
+            cookies_dict = json.loads(json_str)
+        except json.JSONDecodeError:
+            raise ValueError("The cookie string does not have a valid JSON format.")
+    else:
+        try:
+            # Parse the entire content directly as JSON
+            cookies_dict = json.loads(content)
+        except json.JSONDecodeError:
+            raise ValueError("The file content does not have a valid JSON format.")
+
+    return cookies_dict
+
+
 def extract_code(text: str) -> str:
     """
     Extracts code snippets from the given text.
     If only one snippet is found, returns it directly instead of a list.
     If no snippets are found, returns the original text.
 
     Args:
```

### Comparing `python-gemini-api-2.4.2/gemini/src/model/image.py` & `python_gemini_api-2.4.3/gemini/src/model/image.py`

 * *Files identical despite different names*

### Comparing `python-gemini-api-2.4.2/gemini/src/model/output.py` & `python_gemini_api-2.4.3/gemini/src/model/output.py`

 * *Files identical despite different names*

### Comparing `python-gemini-api-2.4.2/gemini/src/model/parser/base.py` & `python_gemini_api-2.4.3/gemini/src/model/parser/base.py`

 * *Files identical despite different names*

### Comparing `python-gemini-api-2.4.2/gemini/src/model/parser/custom_parser.py` & `python_gemini_api-2.4.3/gemini/src/model/parser/custom_parser.py`

 * *Files identical despite different names*

### Comparing `python-gemini-api-2.4.2/gemini/src/model/parser/response_parser.py` & `python_gemini_api-2.4.3/gemini/src/model/parser/response_parser.py`

 * *Files identical despite different names*

### Comparing `python-gemini-api-2.4.2/gemini/src/modules/openrouter/client.py` & `python_gemini_api-2.4.3/gemini/src/modules/openrouter/client.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import requests
+from const import FreeModel
 from typing import List, Optional
 from requests.models import Response
 
 
 class OpenRouter:
     """
     Manages API interactions with OpenRouter for creating chat completions using AI models.
@@ -18,25 +19,14 @@
         generate_content(message, site_url=None, app_name=None): Validates and sends a request to generate content.
         get_model_list(): Returns a list of free model identifiers available.
 
     Raises:
         ValueError: If an API key is not provided or if the message format is incorrect.
     """
 
-    FREE_MODEL_LIST: List[str] = [
-        "google/gemma-7b-it:free",
-        "huggingfaceh4/zephyr-7b-beta:free",
-        "mistralai/mistral-7b-instruct:free",
-        "openrouter/cinematika-7b:free",
-        "undi95/toppy-m-7b:free",
-        "gryphe/mythomist-7b:free",
-        "nousresearch/nous-capybara-7b:free",
-        "openchat/openchat-7b:free",
-    ]
-
     def __init__(self, model: str, api_key: str) -> None:
         """
         Initializes the OpenRouter instance with a specified model and API key.
 
         Parameters:
             model (str): The model identifier for generating chat completions.
             api_key (str): The API key for authentication.
@@ -128,11 +118,11 @@
         if not isinstance(message, str):
             raise ValueError("Message must be a string")
 
     def _validate_model(self, model: str) -> None:
         """
         Checks if the specified model is in the list of free models.
         """
-        if model not in self.FREE_MODEL_LIST:
+        if model not in FreeModel:
             print(
                 "This model may not be free. Please check the following list for costs.\nUsers are responsible for API costs. Visit https://openrouter.ai/docs#models"
             )
```

### Comparing `python-gemini-api-2.4.2/gemini/src/modules/voice/google.py` & `python_gemini_api-2.4.3/gemini/src/modules/voice/google.py`

 * *Files identical despite different names*

### Comparing `python-gemini-api-2.4.2/gemini/src/modules/voice/openai.py` & `python_gemini_api-2.4.3/gemini/src/modules/voice/openai.py`

 * *Files identical despite different names*

### Comparing `python-gemini-api-2.4.2/python_gemini_api.egg-info/PKG-INFO` & `python_gemini_api-2.4.3/python_gemini_api.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-gemini-api
-Version: 2.4.2
+Version: 2.4.3
 Summary: The python package that returns Response of Google Gemini through API.
 Home-page: https://github.com/dsdanielpark/Gemini-API
 Author: Daniel Park
 Author-email: parkminwoo1991@gmail.com
 Keywords: Python,API,Gemini,Google Gemini,Large Language Model,Chatbot API,Google API,Chatbot
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
@@ -39,176 +39,195 @@
     <a href="https://github.com/psf/black"><img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg"></a>
     <a href="https://hits.seeyoufarm.com"><img src="https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2Fdsdanielpark%2FGemini-API&count_bg=%23000000&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=views&edge_flat=false"/></a>
     <a href="https://pypistats.org/packages/python-gemini-api"><img alt="Downloads" src="https://pepy.tech/badge/python-gemini-api"></a>
 <!-- <a href="https://github.com/dsdanielpark/Gemini-API/stargazers"><img src="https://img.shields.io/github/stars/dsdanielpark/Gemini-API?style=social"></a> -->
 </p>
 
 
+
 https://github.com/dsdanielpark/Gemini-API/assets/81407603/e0c11d4f-3fe1-4cbb-ba79-d9f89b637324
 
 
 
 
 
 
 A *unofficial* Python wrapper, [python-gemini-api](https://pypi.org/project/python-gemini-api/), operates through reverse-engineering, utilizing cookie values to interact with [Google Gemini](https://gemini.google.com) for users struggling with frequent authentication problems or unable to authenticate via [Google Authentication](https://developers.google.com/identity/protocols/oauth2?hl=en).
 
 Collaborated competently with [Antonio Cheong](https://github.com/acheong08).
 
-
-
-
+<br>
 
 <br>
 
 
 > [!TIP]
 > | 2024-03-26 | [[See Code Examples]](https://github.com/dsdanielpark/Gemini-API/blob/main/documents/README_OPENROUTER.md)
 > 
 > Check out temporarily free Open-source LLM APIs with Open Router.  (Free limit: 10 requests/minute) 
 
-<br><br>
+<br>
 
+## Contents
 
 - [ Gemini API   ](#-gemini-api---)
-  - [What is Gemini?](#what-is-gemini)
-  - [Installation](#installation)
-  - [Authentication](#authentication)
-  - [Quick Start](#quick-start)
+  - [What is Gemini? 🔐](#what-is-gemini)
+  - [Installation ✅](#installation-)
+  - [Authentication ✅](#authentication)
+  - [Quick Start ✅](#quick-start)
   - [Usage](#usage)
-    - [# 01. Initialization](#-01-initialization)
+    - [# 01. Initialization ✅](#-01-initialization)
     - [# 02. Generate content](#-02-generate-content)
     - [# 03. Send request](#-03-send-request)
     - [# 04. Text generation](#-04-text-generation)
     - [# 05. Image generation](#-05-image-generation)
     - [# 06. Retrieving Images from Gemini Responses](#-06-retrieving-images-from-gemini-responses)
     - [# 07. Generate content from images](#-07-generate-content-from-images)
     - [# 08. Generate content using Google Services](#-08-generate-content-using-google-services)
-    - [# 09. Fix context setting rcid](#-09-fix-context-setting-rcid)
+    - [# 09. Fix context setting RCID](#-09-fix-context-setting-rcid)
     - [# 10. Changing the Selected Response from 0 to *n*](#-10-changing-the-selected-response-from-0-to-n)
     - [# 11. Generate custom content](#-11-generate-custom-content)
   - [Further](#further)
-  - [Open-source LLM, Gemma](#open-source-llm-gemma)
-    - [How to use Gemma](#how-to-use-gemma)
-  - [Utilize free open-source LLM API through Open Router](#utilize-free-open-source-llm-api-through-open-router)
+  - [Google Open-source LLMs](#google-open-source-llms)
+      - [Open-source LLM, Gemma 🤝](#open-source-llm-gemma)
+      - [Open-source LLM, Code Gemma 🤝](#open-source-llm-code-gemma)
+  - [Utilize free open-source LLM API through Open Router ✅](#utilize-free-open-source-llm-api-through-open-router)
 
 
 
 
 
 
 
 <br>
 
+## What is [Gemini](https://deepmind.google/technologies/gemini/#introduction)?
 
+| [Paper](https://arxiv.org/abs/2312.11805) | [Official Website](https://deepmind.google/technologies/gemini/#introduction) | [Official API](https://aistudio.google.com/) | [API Documents](https://cloud.google.com/vertex-ai/docs/generative-ai/model-reference/gemini) |
 
+Gemini is a family of generative AI models developed by Google DeepMind that is designed for multimodal use cases. The Gemini API gives you access to the Gemini Pro and Gemini Pro Vision models. In February 2024, Google's **Bard** service was changed to **Gemini**.
 
+#### Overview of Google LLMs
 
-## What is [Gemini](https://deepmind.google/technologies/gemini/#introduction)?
+| Model | Type | Access | Details
+|:-------:|:------:|:--------:|---------
+[Gemini](https://huggingface.co/google/gemma-7b) | Proprietary | API <sup>[[13](https://ai.google.dev/tutorials/ai-studio_quickstart)] | A proprietary multimodal AI by Google DeepMind, including advanced models such as Gemini Pro and Gemini Pro Vision. Access is restricted to API usage; additional insights may be obtained through the paper and website. <sup>[[1](https://arxiv.org/abs/2312.11805)][[2](https://deepmind.google/technologies/gemini/#introduction)]</sup>
+[Gemma](https://huggingface.co/google/gemma-7b) | Open Source | [Downloadable](https://huggingface.co/google/gemma-7b) <br>[Free API](https://github.com/dsdanielpark/Gemini-API?tab=readme-ov-file#utilize-free-open-source-llm-api-through-open-router) | An open-source text-to-text language model suitable for tasks like QA and summarization. Weights are downloadable for on-premises use, and detailed documentation is provided via the paper and website. <sup>[[3](https://arxiv.org/abs/2403.08295)][[4](https://ai.google.dev/gemma/docs)]</sup>
+[Code Gemma](https://huggingface.co/google/codegemma-7b-it) | Open Source | [Downloadable](https://huggingface.co/google/codegemma-7b-it) | Designed specifically for programming tasks, this open-source model offers downloadable weights to assist developers with code generation and similar activities. Refer to the associated paper, blog post, and Hugging Face collection for more information. <sup>[[5](https://storage.googleapis.com/deepmind-media/gemma/codegemma_report.pdf?utm_source=substack&utm_medium=email)][[6](https://huggingface.co/blog/codegemma)][[7](https://huggingface.co/collections/google/codegemma-release-66152ac7b683e2667abdee11)]</sup>
 
-| [Paper](https://arxiv.org/abs/2312.11805) | [Official Website](https://deepmind.google/technologies/gemini/#introduction) | [Official API](https://aistudio.google.com/) | [API Documents](https://cloud.google.com/vertex-ai/docs/generative-ai/model-reference/gemini) |
 
-Gemini is a family of generative AI models developed by Google DeepMind that is designed for multimodal use cases. The Gemini API gives you access to the Gemini Pro and Gemini Pro Vision models. In February 2024, Google's **Bard** service was changed to **Gemini**.
+<br>
 
+## What is [Python-Gemini-API](https://github.com/dsdanielpark/Gemini-API)?
 
+This is a Python wrapper derived from the [Bard API](https://github.com/dsdanielpark/Bard-API) project, designed to retrieve responses from Gemini Web in REST format. **Synchronous clients are preferred over asynchronous ones for Gemini because of rate limiting and blocking concerns.**
 
 ## Installation 📦
 ```
 pip install python-gemini-api
 ```
 ```
 pip install git+https://github.com/dsdanielpark/Gemini-API.git
 ```
 For the updated version, use as follows:
 ```
 pip install -q -U python-gemini-api
 ```
+
+
+
 ## Authentication
-> [!NOTE]
-> Cookies can change quickly. Don't reopen the same session or repeat prompts too often; they'll expire faster. If the cookie value doesn't export correctly, refresh the Gemini page and export again. 
+
 1. Visit https://gemini.google.com/ <br>
     With browser open, try auto-collecting cookies first.
     ```python
     from gemini import Gemini
     GeminiClient = Gemini(auto_cookies=True)
 
     # Testing needed as cookies vary by region.
     # GeminiClient = Gemini(auto_cookies=True, target_cookies=["__Secure-1PSID", "__Secure-1PSIDTS"])
+    # GeminiClient = Gemini(auto_cookies=True, target_cookies="all") # You can pass whole cookies
 
     response = GeminiClient.generate_content("Hello, Gemini. What's the weather like in Seoul today?")
     print(response.payload)
     ```
 2. *(Manually)* `F12` for browser console → `Session: Application` → `Cookies` → Copy the value of some working cookie sets. If it doesn't work, go to step 3.
     <details><summary>Some working cookie sets</summary>
     Cookies may vary by account or region. 
       
     First try `__Secure-1PSIDCC` alone. If it doesn't work, use `__Secure-1PSID` and `__Secure-1PSIDTS`. Still no success? Try these four cookies: `__Secure-1PSIDCC`, `__Secure-1PSID`, `__Secure-1PSIDTS`, `NID`. If none work, proceed to step 3 and consider sending the entire cookie file.
     
     </details>
 
 3. *(Recommended)* Export Gemini site cookies via a browser extension. For instance, use Chrome extension [ExportThisCookies](https://chromewebstore.google.com/detail/exportthiscookie/dannllckdimllhkiplchkcaoheibealk), open, and copy the txt file contents.
 
+
+<br>
+
 <details><summary>Further: For manual collection or Required for a few users upon error</summary>
 
 4. For manual cookie collection, refer to [this image](assets/cookies.pdf). Press F12 → Network → Send any prompt to Gemini webui → Click the post address starting with "https://gemini.google.com/_/BardChatUi/data/assistant.lamda.BardFrontendService/StreamGenerate" → Headers → Request Headers → Cookie → Copy and Reformat as JSON manually.
 5. *(Required for a few users upon error)* If errors persist after manually collecting cookies, refresh the Gemini website and collect cookies again. If errors continue, some users may need to manually set the nonce value. To do this: Press F12 → Network → Send any prompt to Gemini webui → Click the post address starting with "https://gemini.google.com/_/BardChatUi/data/assistant.lamda.BardFrontendService/StreamGenerate" → Payload → Form Data → Copy the "at" key value. See [this image](assets/nonce_value.pdf) for reference.
 </details>
 
 
 > [!IMPORTANT] 
->  Try different Google accounts until you find a working cookie. Use a fresh browser to ensure no remaining cookie values. Use secret browsing mode with independent cookies. Results may vary depending on factors like IP and account status. Providing the entire set of cookies seems to fix one cookie per account. Additionally, once successfully connected with that cookie, it seems to work flawlessly for over three weeks without any errors. *Try various methods until you succeed. Experiment in different environments.*
+> Experiment with different Google accounts and browser settings to find a working cookie. Success may vary by IP and account status. Once connected, a cookie typically remains effective over a month. Keep testing until successful.
 
 
 <br>
 
 ## Quick Start
 
-*Simple usage*
-
-Setting Gemini response language (Optional): Check supported languages [here](https://developers.google.com/hotels/hotel-prices/dev-guide/country-codes). Default is English.
-
-```python
-import os
-os.environ["GEMINI_LANGUAGE"] = "KR"
-```
-
-
-
-Generate content: returns parsed response.
+**Generate content:** returns parsed response.
 ```python
 from gemini import Gemini
 
 cookies = {} # Cookies may vary by account or region. Consider sending the entire cookie file.
 GeminiClient = Gemini(cookies=cookies) # You can use various args
 
 response = GeminiClient.generate_content("Hello, Gemini. What's the weather like in Seoul today?")
 response.payload
 ```
 
-Generate content from image: you can use image as input.
+**Generate content from image:** you can use image as input.
 ```python
 from gemini import Gemini
 
 cookies = {} # Cookies may vary by account or region. Consider sending the entire cookie file.
 
 GeminiClient = Gemini(cookies=cookies) # You can use various args
 response = GeminiClient.generate_content("What does the text in this image say?", image='folder/image.jpg')
 response.payload
 ```
 
 > [!NOTE] 
 > If the generate_content method returns an empty payload, try executing it again without reinitializing the Gemini object.
 
-<br>
+<br><br>
 
 ## Usage
 
+*Setting language and Gemini version using environment variables:*
+
+Setting Gemini response language (Optional): Check supported languages [here](https://developers.google.com/hotels/hotel-prices/dev-guide/country-codes). Default is English.
+
+```python
+import os
+os.environ["GEMINI_LANGUAGE"] = "KR"  # Setting Gemini response language (Optional)
+os.environ["GEMINI_ULTRA"] = "1"      # Switch to Gemini-advanced response (Experimental, Optional)
+# In some accounts, access to Gemini Ultra may not be available. If that's the case, please revert it back to "0".
+```
+
+
+
+<br>
 
 ### # 01. Initialization
-Please explicitly declare `cookies` in dict format. You can also enter the path to the file containing the cookie with `cookie_fp`(*.json, *.txt supported). Check this [sample cookie file](https://github.com/dsdanielpark/Gemini-API/blob/main/cookies.txt).
+Please explicitly declare `cookies` in dict format. You can also enter the path to the file containing the cookie with `cookie_fp`(*.json, *.txt supported). Check sample cookie files in [assets](https://github.com/dsdanielpark/Gemini-API/tree/main/assets) folder.
 
 
 
 
 ```python
 from gemini import Gemini
 
@@ -221,53 +240,48 @@
   }
 
 GeminiClient = Gemini(cookies=cookies)
 # GeminiClient = Gemini(cookie_fp="folder/cookie_file.json") # (*.json, *.txt) are supported.
 # GeminiClient = Gemini(auto_cookies=True) # Or use auto_cookies paprameter
 ```
 
-#### Auto Cookie Update
-For `auto_cookie` to be set to `True`, Gemini WebUI must be active in the browser. The [browser_cookie3](https://github.com/borisbabic/browser_cookie3) enables automatic cookie collection, though updates may not be complete yet.
+##### Auto Cookie Update
+For `auto_cookie` to be set to `True`, and adjust `target_cookies`. Gemini WebUI must be active in the browser. The [browser_cookie3](https://github.com/borisbabic/browser_cookie3) enables automatic cookie collection, though updates may not be complete yet.
 
 
-> [!IMPORTANT]
->  **If the session connects successfully and `generate_content` runs well, CLOSE Gemini website.** If Gemini web stays open in the browser, cookies may expire faster.
 
 <br>
 
 ### # 02. Generate content
-Returns Gemini's response, but the first one might be empty. If generate_content yields an empty payload, rerun it without reinitializing Gemini. 
+Returns Gemini's response, but the first one might be empty. 
+
 
-Regardless of model output type, access the response_dict property (renamed to payload after v2.3.0).
-https://github.com/dsdanielpark/Gemini-API/blob/fdf064c57bc1fb47fbbb4b93067618a200e77f62/gemini/core.py#L252
 ```python
 prompt = "Hello, Gemini. What's the weather like in Seoul today?"
 response = GeminiClient.generate_content(prompt)
 print(response.payload)
 ```
+
+
 > [!IMPORTANT]
->  Once connected and generating valid content, **Be sure to CLOSE the Gemini website or CLOSE your browser** for cookie stability. 
+>  DO NOT send same prompt repeatly. **If the session connects successfully and `generate_content` runs well, CLOSE Gemini website.** If Gemini web stays open in the browser, cookies may expire faster. 
 
 <br>
 
-The output of the generate_content function is `GeminiModelOutput`, with the following structure:
-
-**Properties of GeminiModelOutput:**
+The output of the generate_content function is `GeminiModelOutput`, with the following structure: 
 - *rcid*: returns the response candidate id of the chosen candidate.
 - *text*: returns the text of the chosen candidate.
 - *code*: returns the codes of the chosen candidate.
 - *web_images*: returns a list of web images from the chosen candidate.
 - *generated_images*: returns a list of generated images from the chosen candidate.
-- *payload*: returns the response dictionary, if available. (same as *reponse_dict* under v2.3.0)
-
+- *payload*: returns the response dictionary, if available.
 https://github.com/dsdanielpark/Gemini-API/blob/fdf064c57bc1fb47fbbb4b93067618a200e77f62/gemini/src/model/output.py#L16
 
 
-> [!NOTE]
-> If the session fails to connect, works improperly, or terminates, returning an error, it is recommended to manually renew the cookies. The error is likely due to incorrect cookie values. Refresh or log out of Gemini web to renew cookies and try again. 
+
 
 <br>
 
 
 ### # 03. Send request
 Send request: returns the request's payload and status_code, making debugging easier.
 ```python
@@ -275,15 +289,15 @@
 
 cookies = {} # Cookies may vary by account or region. Consider sending the entire cookie file.
 GeminiClient = Gemini(cookies=cookies) # You can use various args
 
 response_text, response_status = GeminiClient.send_request("Hello, Gemini. What's the weather like in Seoul today?")
 print(response_text)
 ```
-
+You can track the total number of requests made by accessing the `request_count` property within the `Gemini` class.
 
 <br>
 
 ### # 04. Text generation
 Returns text generated by Gemini.
 ```python
 prompt = "Hello, Gemini. What's the weather like in Seoul today?"
@@ -292,65 +306,62 @@
 ```
 
 
 <br>
 
 ### # 05. Image generation
 Returns images generated by Gemini.
-https://github.com/dsdanielpark/Gemini-API/blob/fdf064c57bc1fb47fbbb4b93067618a200e77f62/gemini/src/model/image.py#L12
 
-*Sync downloader*
-```python
-from gemini import Gemini, GeminiImage
+*Async downloader*
 
+```python
 response = GeminiClient.generate_content("Create illustrations of Seoul, South Korea.")
-generated_images = response.generated_images # Check generated images [Dict]
 
-GeminiImage.save_sync(generated_images, save_path="save_dir", cookies=cookies)
+generated_images = response.generated_images # Check generated images [Dict]
 
-# You can use byte type image dict for printing images as follow:
-# bytes_images_dict = GeminiImage.fetch_images_dict_sync(generated_images, cookies=cookies) # Get bytes images dict
-# GeminiImage.save_images_sync(bytes_images_dict, path="save_dir", cookies=cookies) # Save to path
+await GeminiImage.save(generated_images, "save_dir", cookies=cookies)
+# image_data_dict = await GeminiImage.fetch_images_dict(generated_images, cookies=cookies)
+# await GeminiImage.save_images(image_data_dict, "save_dir")
 ```
 
-<details><summary>Display images in IPython</summary>
-  
+
+<details><summary>Further</summary>
+
+*Display images in IPython*
   You can display the image or transmit it to another application in byte format.
   
-  ```
+  ```python
   bytes_images_dict = GeminiImage.fetch_images_dict_sync(generated_images, cookies) # Get bytes images dict
   from IPython.display import display, Image
   import io
   
   for image_name, image_bytes in bytes_images_dict.items():
       print(image_name)
       image = Image(data=image_bytes)
       display(image)
   ```
 
-</details>
-
-
-
-*Async downloader*
 
+*Sync downloader*
 ```python
-response = GeminiClient.generate_content("Create illustrations of Seoul, South Korea.")
+from gemini import Gemini, GeminiImage
 
+response = GeminiClient.generate_content("Create illustrations of Seoul, South Korea.")
 generated_images = response.generated_images # Check generated images [Dict]
 
-await GeminiImage.save(generated_images, "save_dir", cookies=cookies)
-# image_data_dict = await GeminiImage.fetch_images_dict(generated_images, cookies=cookies)
-# await GeminiImage.save_images(image_data_dict, "save_dir")
-```
+GeminiImage.save_sync(generated_images, save_path="save_dir", cookies=cookies)
 
+# You can use byte type image dict for printing images as follow:
+# bytes_images_dict = GeminiImage.fetch_images_dict_sync(generated_images, cookies=cookies) # Get bytes images dict
+# GeminiImage.save_images_sync(bytes_images_dict, path="save_dir", cookies=cookies) # Save to path
+```
 
-<details><summary>Async downloader wrapper</summary>
+*Async downloader wrapper*
 
-```
+```python
 import asyncio
 from gemini import Gemini, GeminiImage
 
 async def save_generated_imagse(generated_imagse, save_path="save_dir", cookies=cookies):
     await GeminiImage.save(generated_imagse, save_path=save_path, cookies=cookies)
 
 # Run the async function
@@ -383,41 +394,45 @@
 > Use GeminiImage for image processing. `web_images` works without cookies, but for images like `generated_image` from Gemini, pass cookies. Cookies are needed to download images from Google's storage. Check the response or use existing cookies variable.
 
 <br>
 
 ### # 06. Retrieving Images from Gemini Responses
 Returns images in response of Gemini.
 
-*Sync downloader*
-```python
-from gemini import Gemini, GeminiImage
-
-response = GeminiClient.generate_content("Please recommend a travel itinerary for Seoul.")
-response_images = response.web_images # Check response images [Dict]
-
-GeminiImage.save_sync(response_images, save_path="save_dir")
 
-# You can use byte type image dict as follow:
-# bytes_images_dict = GeminiImage.fetch_bytes_sync(response_images, cookies) # Get bytes images dict
-# GeminiImage.save_images_sync(bytes_images_dict, path="save_dir") # Save to path
-```
 *Async downloader*
 ```python
 response = GeminiClient.generate_content("Create illustrations of Seoul, South Korea.")
 
 response_images = response.web_images # Check generated images [Dict]
 
 await GeminiImage.save(response_images, "save_dir")
 # image_data_dict = await GeminiImage.fetch_images_dict(response_images)
 # await GeminiImage.save_images(image_data_dict, "save_dir")
 ```
 
-<details><summary>Async downloader wrapper</summary>
+<details><summary>Further</summary>
+
 
+*Sync downloader*
+```python
+from gemini import Gemini, GeminiImage
+
+response = GeminiClient.generate_content("Please recommend a travel itinerary for Seoul.")
+response_images = response.web_images # Check response images [Dict]
+
+GeminiImage.save_sync(response_images, save_path="save_dir")
+
+# You can use byte type image dict as follow:
+# bytes_images_dict = GeminiImage.fetch_bytes_sync(response_images, cookies) # Get bytes images dict
+# GeminiImage.save_images_sync(bytes_images_dict, path="save_dir") # Save to path
 ```
+
+*Async downloader wrapper*
+```python
 import asyncio
 from gemini import Gemini, GeminiImage
 
 async def save_response_web_imagse(response_images, save_path="save_dir", cookies=cookies):
     await GeminiImage.save(response_images, save_path=save_path, cookies=cookies)
 
 # Run the async function
@@ -498,59 +513,68 @@
   - Description: Explore YouTube videos and ask questions about what interests you.
   - Features: Problem-solving, generating ideas, search, exploring topics
 </details>
 
 <br>
 
 
-### # 09. Fix context setting rcid
-You can specify a particular response by setting its response candidate id(rcid).
+### # 09. Fix context setting RCID
+You can specify a particular response by setting its Response Candidate ID(RCID).
 
 ```python
 # Generate content for the prompt "Give me some information about the USA."
 response1 = GeminiClient.generate_content("Give me some information about the USA.")
 # After reviewing the responses, choose the one you prefer and copy its RCID.
 GeminiClient.rcid = "rc_xxxx"
 
 # Now, generate content for the next prompt "How long does it take from LA to New York?"
 response2 = GeminiClient.generate_content("How long does it take from LA to New York?")
+
+# However, RCID may not persist. If parsing fails, reset `GeminiClient.rcid` to None.
+# GeminiClient.rcid = None
 ```
 
+
+
 <br>
 
 ### # 10. Changing the Selected Response from 0 to *n*
 In Gemini, generate_content returns the first response. This may vary depending on length or sorting. Therefore, you can specify the index of the chosen response from 0 to *n* as follows. However, if there is only one response, revert it back to 0.
 ```python
 from gemini import GeminiModelOutput
+
 GeminiModelOutput.chosen = 1 # default is 0
-response1 = GeminiClient.generate_content("Give me some information about the USA.")
+response_choice_1 = GeminiClient.generate_content("Give me some information about the USA.")
+
+# If not all Gemini returns are necessarily plural, revert back to 0 in case of errors.
+#  GeminiModelOutput.chosen = 0
 ```
 
 <br>
 
 ### # 11. Generate custom content 
 Parse the response text to extract desired values.
 
-https://github.com/dsdanielpark/Gemini-API/blob/fdf064c57bc1fb47fbbb4b93067618a200e77f62/gemini/core.py#L317
 
 Using `Gemini.generate_custom_content`, specify custom parsing to extract specific values. Utilize ParseMethod1 and ParseMethod2 by default, and you can pass custom parsing methods as arguments if desired. Refer to [custom_parser.py](https://github.com/dsdanielpark/Gemini-API/blob/main/gemini/src/model/parser/custom_parser.py).
 
 ```python
 # You can create a parser method that takes response_text as the input for custom_parser.
 response_text, response_status = GeminiClient.send_request("Give me some information about the USA.")
 
 # Use custom_parser function or class inheriting from BaseParser
 response = GeminiClient.generate_custom_content("Give me some information about the USA.", *custom_parser)
 ```
 
+https://github.com/dsdanielpark/Gemini-API/blob/31b842488bbc5429ad9c74b1d8b00e20d94e8cb1/gemini/client.py#L323
 <br>
 
 ## Further
 
-### Use rotating proxies
+### Use rotating proxies via [Smart Proxy by Crawlbase](https://crawlbase.com/docs/smart-proxy/?utm_source=github_ad&utm_medium=social&utm_campaign=bard_api)
 
 If you want to **avoid blocked requests** and bans, then use [Smart Proxy by Crawlbase](https://crawlbase.com/docs/smart-proxy/?utm_source=github_ad&utm_medium=social&utm_campaign=bard_api). It forwards your connection requests to a **randomly rotating IP address** in a pool of proxies before reaching the target website. The combination of AI and ML make it more effective to avoid CAPTCHAs and blocks.
 
 ```python
 # Get your proxy url at crawlbase https://crawlbase.com/docs/smart-proxy/get/
 proxy_url = "http://xxxxx:@smartproxy.crawlbase.com:8012" 
 proxies = {"http": proxy_url, "https": proxy_url}
@@ -558,16 +582,16 @@
 GeminiClient = Gemini(cookies=cookies, proxies=proxies, timeout=30)
 GeminiClient.generate_content("Hello, Gemini. Give me a beautiful photo of Seoul's scenery.")
 ```
 
 ### Reusable session object
 For standard cases, use Gemini class; for exceptions, use session objects. When creating a new bot Gemini server, adjust Headers.MAIN.
 ```python
-from gemini import Gemini, Headers
 import requests
+from gemini import Gemini, Headers
 
 cookies = {} 
 
 session = requests.Session()
 session.headers = Headers.MAIN
 for key, value in cookies.items():
     session.cookies.update({key: value})
@@ -584,42 +608,66 @@
 ## [More features](https://github.com/dsdanielpark/Gemini-API/blob/main/documents/README_DEV.md)
 Explore additional features in [this document](https://github.com/dsdanielpark/Gemini-API/blob/main/documents/README_DEV.md).
 
 If you want to develop your own simple code, you can start from [this simple code example](https://github.com/dsdanielpark/Gemini-API/blob/main/script/sample.ipynb).  
 
 <br>
 
+## Google Open-source LLMs
+
+If you have sufficient GPU resources, you can download weights directly instead of using the Gemini API to generate content. Consider Gemma and Code Gemma, an open-source models **available for on-premises use**.
+
+
+
+### Open-source LLM, [Gemma](https://huggingface.co/google/gemma-7b)
 
-## Open-source LLM, [Gemma](https://huggingface.co/google/gemma-7b)
-If you have sufficient GPU resources, you can download weights directly instead of using the Gemini API to generate content. Consider Gemma, an open-source model **available for on-premises use**.
 
-[Gemma](https://huggingface.co/google/gemma-7b) models are Google's lightweight, advanced text-to-text, decoder-only language models, derived from Gemini research. Available in English, they offer open weights and variants, ideal for tasks like question answering and summarization. Their small size enables deployment in resource-limited settings, broadening access to cutting-edge AI. For more infomation, visit [Gemma-7b](https://huggingface.co/google/gemma-7b) model card.
+Gemma models are Google's lightweight, advanced text-to-text, decoder-only language models, derived from Gemini research. Available in English, they offer open weights and variants, ideal for tasks like question answering and summarization. For more infomation, visit [Gemma-7b](https://huggingface.co/google/gemma-7b) model card.
 
-### How to use Gemma
+#### How to use Gemma
 ```python
 from transformers import AutoTokenizer, AutoModelForCausalLM
 
 tokenizer = AutoTokenizer.from_pretrained("google/gemma-7b")
 model = AutoModelForCausalLM.from_pretrained("google/gemma-7b")
 
 input_text = "Write me a poem about Machine Learning."
 input_ids = tokenizer(input_text, return_tensors="pt")
 
 outputs = model.generate(**input_ids)
 print(tokenizer.decode(outputs[0]))
 ```
 
+### Open-source LLM, [Code Gemma](https://huggingface.co/collections/google/codegemma-release-66152ac7b683e2667abdee11)
+
+CodeGemma, which is an official release from Google for code LLMs, was released on April 9, 2024. It provides three models specifically designed for generating and interacting with code. You can explore the [Code Gemma models](https://huggingface.co/collections/google/codegemma-release-66152ac7b683e2667abdee11) and view the [model card](https://huggingface.co/google/codegemma-7b-it) for more details.
+
+#### How to use Code Gemma
+```python
+from transformers import GemmaTokenizer, AutoModelForCausalLM
+
+tokenizer = GemmaTokenizer.from_pretrained("google/codegemma-7b-it")
+model = AutoModelForCausalLM.from_pretrained("google/codegemma-7b-it")
+
+input_text = "Write me a Python function to calculate the nth fibonacci number."
+input_ids = tokenizer(input_text, return_tensors="pt")
+
+outputs = model.generate(**input_ids)
+print(tokenizer.decode(outputs[0]))
+```
+
+
+
 <br>
 
 
 ## Utilize free open-source LLM API through [Open Router](https://openrouter.ai/)
-OpenRouter offers temporary free inference for select models. Obtain an API key from [Open Router API](https://openrouter.ai/keys) and check free models at [Open Router models](https://openrouter.ai/docs#models). Use models with a 0-dollar token cost primarily; other models may incur charges. See more [free open-source LLM API guide](https://github.com/dsdanielpark/Gemini-API/blob/main/documents/README_OPENROUTER.md)
+OpenRouter offers temporary free inference for select models. Obtain an API key from [Open Router API](https://openrouter.ai/keys) and check free models at [Open Router models](https://openrouter.ai/docs#models). Use models with a 0-dollar token cost primarily; other models may incur charges. See more at [free open-source LLM API guide](https://github.com/dsdanielpark/Gemini-API/blob/main/documents/README_OPENROUTER.md).
 
-> [!NOTE]
-> You can easily receive responses from open LLMs without this package by following the instructions on [here](https://openrouter.ai/docs#models).
+**Sync client is favored over async for Gemini due to rate limiting and blocking issues**, but OpenRouter offers reliable open-source LLMs for [async implementation](https://github.com/dsdanielpark/Gemini-API/blob/main/documents/README_OPENROUTER.md#openrouter-async-api-client).
 
 ```python
 from gemini import OpenRouter
 
 OPENROUTER_API_KEY = "<your_open_router_api_key>"
 GemmaClient = OpenRouter(api_key=OPENROUTER_API_KEY, model="google/gemma-7b-it:free")
 
@@ -643,28 +691,26 @@
 
 
 
 
 
 <br>
 
+## Sponsor, [Crawlbase](https://crawlbase.com/)
+Use [Crawlbase](https://crawlbase.com/) API for efficient data scraping to train AI models, boasting a 98% success rate and 99.9% uptime. It's quick to start, GDPR/CCPA compliant, supports massive data extraction, and is trusted by 70k+ developers.
+
+<br>
 
 ## [FAQ](https://github.com/dsdanielpark/Gemini-API/blob/main/documents/README_FAQ.md)
 First review [HanaokaYuzu/Gemini-API](https://github.com/HanaokaYuzu/Gemini-API) and the [Official Google Gemini API](https://aistudio.google.com/) before using this package.
 You can find most help on the [FAQ](https://github.com/dsdanielpark/Gemini-API/blob/main/documents/README_FAQ.md) and [Issue](https://github.com/dsdanielpark/Gemini-API/issues) pages. 
-
-
             
 ## [Issues](https://github.com/dsdanielpark/Gemini-API/issues)
 Sincerely grateful for any reports on new features or bugs. Your valuable feedback on the code is highly appreciated. Frequent errors may occur due to changes in Google's service API interface. Both [Issue reports](https://github.com/dsdanielpark/Gemini-API/issues) and [Pull requests](https://github.com/dsdanielpark/Gemini-API/pulls) contributing to improvements are always welcome. We strive to maintain an active and courteous open community.
 
-
-## Sponsor
-Use [Crawlbase](https://crawlbase.com/) API for efficient data scraping to train AI models, boasting a 98% success rate and 99.9% uptime. It's quick to start, GDPR/CCPA compliant, supports massive data extraction, and is trusted by 70k+ developers.
-
 ## Contributors
 We would like to express our sincere gratitude to all the contributors. 
 
 This package aims to re-implement the functionality of the [Bard API](https://github.com/dsdanielpark/Bard-API/), which has been archived for the contributions of the beloved open-source community, despite Gemini's official API already being available.
 
 Contributors to the [Bard API](https://github.com/dsdanielpark/Bard-API/) and [Gemini API](https://github.com/dsdanielpark/Gemini-API/).
 
@@ -696,20 +742,27 @@
 
 
 ## License ©️ 
 [MIT](https://opensource.org/license/mit/) license, 2024. We hereby strongly disclaim any explicit or implicit legal liability related to our works. Users are required to use this package responsibly and at their own risk. This project is a personal initiative and is not affiliated with or endorsed by Google. It is recommended to use Google's official API.
 
 
 ## References
-[1] Github: [acheong08/Bard](https://github.com/acheong08/Bard) <br>
-[2] GitHub: [HanaokaYuzu/Gemini-API](https://github.com/HanaokaYuzu/Gemini-API) <br>
-[3] Github: [dsdanielpark/Bard-API](https://github.com/dsdanielpark/Bard-API) <br>
-[4] Github: [GoogleCloudPlatform/generative-ai](https://github.com/GoogleCloudPlatform/generative-ai) <br>
-[5] Github: [OpenRouter](https://github.com/OpenRouterTeam/openrouter-runner) <br>
-[6] WebSite: [Google AI Studio](https://ai.google.dev/tutorials/ai-studio_quickstart) <br>
+[1]: Paper - [Introducing GEMINI: Multimodal Generative Models](https://arxiv.org/abs/2312.11805) <br>
+[2]: Website - [Google DeepMind :: GEMINI Introduction](https://deepmind.google/technologies/gemini/#introduction) <br>
+[3]: Paper - [GEMMA: A Unified Language Model for Text Generation, Understanding, Translation, Coding, and Math.]() <br>
+[4]: Website - [AI at Google :: GEMS Documentation](https://ai.google.dev/gemma/docs) <br>
+[5]: Report - [CodeGMMA: Large Language Models Can Write Realistic Programming Assignments](https://storage.googleapis.com/deepmind-media/gemma/codegemma_report.pdf?utm_source=substack&utm_medium=email) <br>
+[6]: Blog Post - [Announcing CodeGen: Building Better Developers’ Tools Using LLMs](https://huggingface.co/blog/codegen) <br>
+[7]: Collection - [Google :: CodeGen Release](https://huggingface.co/collections/google/codegen-release-5d0f4c4eaedbc5cefcfdcbdf) <br>
+[8]: Github - [acheong08/Bard](https://github.com/acheong08/Bard) <br>
+[9]: GitHub - [HanaokaYuzu/Gemini-API](https://github.com/HanaokaYuzu/Gemini-API) <br>
+[10]: Github - [dsdanielpark/Bard-API](https://github.com/dsdanielpark/Bard-API) <br>
+[11]: Github - [GoogleCloudPlatform/generative-ai](https://github.com/GoogleCloudPlatform/generative-ai) <br>
+[12]: Github - [OpenRouter](https://github.com/OpenRouterTeam/openrouter-runner) <br>
+[13]: WebSite - [Google AI Studio](https://ai.google.dev/tutorials/ai-studio_quickstart) <br>
 
 
 > *Warning*
 Users assume full legal responsibility for GeminiAPI. Not endorsed by Google. Excessive use may lead to account restrictions. Changes in policies or account status may affect functionality. Utilize issue and discussion pages.
 
 <br>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: python-gemini-api Version: 2.4.2 Summary: The
+Metadata-Version: 2.1 Name: python-gemini-api Version: 2.4.3 Summary: The
 python package that returns Response of Google Gemini through API. Home-page:
 https://github.com/dsdanielpark/Gemini-API Author: Daniel Park Author-email:
 parkminwoo1991@gmail.com Keywords: Python,API,Gemini,Google Gemini,Large
 Language Model,Chatbot API,Google API,Chatbot Classifier: Development Status ::
 2 - Pre-Alpha Classifier: Intended Audience :: Science/Research Classifier:
 Natural Language :: English Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
@@ -24,60 +24,88 @@
 ba79-d9f89b637324 A *unofficial* Python wrapper, [python-gemini-api](https://
 pypi.org/project/python-gemini-api/), operates through reverse-engineering,
 utilizing cookie values to interact with [Google Gemini](https://
 gemini.google.com) for users struggling with frequent authentication problems
 or unable to authenticate via [Google Authentication](https://
 developers.google.com/identity/protocols/oauth2?hl=en). Collaborated
 competently with [Antonio Cheong](https://github.com/acheong08).
+
 > [!TIP] > | 2024-03-26 | [[See Code Examples]](https://github.com/
 dsdanielpark/Gemini-API/blob/main/documents/README_OPENROUTER.md) > > Check out
 temporarily free Open-source LLM APIs with Open Router. (Free limit: 10
 requests/minute)
-
-- [ Gemini API ](#-gemini-api---) - [What is Gemini?](#what-is-gemini) -
-[Installation](#installation) - [Authentication](#authentication) - [Quick
-Start](#quick-start) - [Usage](#usage) - [# 01. Initialization](#-01-
-initialization) - [# 02. Generate content](#-02-generate-content) - [# 03. Send
-request](#-03-send-request) - [# 04. Text generation](#-04-text-generation) -
-[# 05. Image generation](#-05-image-generation) - [# 06. Retrieving Images from
-Gemini Responses](#-06-retrieving-images-from-gemini-responses) - [# 07.
-Generate content from images](#-07-generate-content-from-images) - [# 08.
-Generate content using Google Services](#-08-generate-content-using-google-
-services) - [# 09. Fix context setting rcid](#-09-fix-context-setting-rcid) -
-[# 10. Changing the Selected Response from 0 to *n*](#-10-changing-the-
-selected-response-from-0-to-n) - [# 11. Generate custom content](#-11-generate-
-custom-content) - [Further](#further) - [Open-source LLM, Gemma](#open-source-
-llm-gemma) - [How to use Gemma](#how-to-use-gemma) - [Utilize free open-source
-LLM API through Open Router](#utilize-free-open-source-llm-api-through-open-
-router)
+## Contents - [ Gemini API ](#-gemini-api---) - [What is Gemini? ð](#what-
+is-gemini) - [Installation â](#installation-) - [Authentication â]
+(#authentication) - [Quick Start â](#quick-start) - [Usage](#usage) - [# 01.
+Initialization â](#-01-initialization) - [# 02. Generate content](#-02-
+generate-content) - [# 03. Send request](#-03-send-request) - [# 04. Text
+generation](#-04-text-generation) - [# 05. Image generation](#-05-image-
+generation) - [# 06. Retrieving Images from Gemini Responses](#-06-retrieving-
+images-from-gemini-responses) - [# 07. Generate content from images](#-07-
+generate-content-from-images) - [# 08. Generate content using Google Services]
+(#-08-generate-content-using-google-services) - [# 09. Fix context setting
+RCID](#-09-fix-context-setting-rcid) - [# 10. Changing the Selected Response
+from 0 to *n*](#-10-changing-the-selected-response-from-0-to-n) - [# 11.
+Generate custom content](#-11-generate-custom-content) - [Further](#further) -
+[Google Open-source LLMs](#google-open-source-llms) - [Open-source LLM, Gemma
+ð¤](#open-source-llm-gemma) - [Open-source LLM, Code Gemma ð¤](#open-
+source-llm-code-gemma) - [Utilize free open-source LLM API through Open Router
+â](#utilize-free-open-source-llm-api-through-open-router)
 ## What is [Gemini](https://deepmind.google/technologies/gemini/#introduction)?
 | [Paper](https://arxiv.org/abs/2312.11805) | [Official Website](https://
 deepmind.google/technologies/gemini/#introduction) | [Official API](https://
 aistudio.google.com/) | [API Documents](https://cloud.google.com/vertex-ai/
 docs/generative-ai/model-reference/gemini) | Gemini is a family of generative
 AI models developed by Google DeepMind that is designed for multimodal use
 cases. The Gemini API gives you access to the Gemini Pro and Gemini Pro Vision
 models. In February 2024, Google's **Bard** service was changed to **Gemini**.
-## Installation ð¦ ``` pip install python-gemini-api ``` ``` pip install
-git+https://github.com/dsdanielpark/Gemini-API.git ``` For the updated version,
-use as follows: ``` pip install -q -U python-gemini-api ``` ## Authentication >
-[!NOTE] > Cookies can change quickly. Don't reopen the same session or repeat
-prompts too often; they'll expire faster. If the cookie value doesn't export
-correctly, refresh the Gemini page and export again. 1. Visit https://
+#### Overview of Google LLMs | Model | Type | Access | Details |:-------:|:----
+--:|:--------:|--------- [Gemini](https://huggingface.co/google/gemma-7b) |
+Proprietary | API [[13](https://ai.google.dev/tutorials/ai-studio_quickstart)]
+| A proprietary multimodal AI by Google DeepMind, including advanced models
+such as Gemini Pro and Gemini Pro Vision. Access is restricted to API usage;
+additional insights may be obtained through the paper and website. [[1](https:/
+/arxiv.org/abs/2312.11805)][[2](https://deepmind.google/technologies/gemini/
+#introduction)] [Gemma](https://huggingface.co/google/gemma-7b) | Open Source |
+[Downloadable](https://huggingface.co/google/gemma-7b)
+[Free API](https://github.com/dsdanielpark/Gemini-API?tab=readme-ov-
+file#utilize-free-open-source-llm-api-through-open-router) | An open-source
+text-to-text language model suitable for tasks like QA and summarization.
+Weights are downloadable for on-premises use, and detailed documentation is
+provided via the paper and website. [[3](https://arxiv.org/abs/2403.08295)][[4]
+(https://ai.google.dev/gemma/docs)] [Code Gemma](https://huggingface.co/google/
+codegemma-7b-it) | Open Source | [Downloadable](https://huggingface.co/google/
+codegemma-7b-it) | Designed specifically for programming tasks, this open-
+source model offers downloadable weights to assist developers with code
+generation and similar activities. Refer to the associated paper, blog post,
+and Hugging Face collection for more information. [[5](https://
+storage.googleapis.com/deepmind-media/gemma/
+codegemma_report.pdf?utm_source=substack&utm_medium=email)][[6](https://
+huggingface.co/blog/codegemma)][[7](https://huggingface.co/collections/google/
+codegemma-release-66152ac7b683e2667abdee11)]
+## What is [Python-Gemini-API](https://github.com/dsdanielpark/Gemini-API)?
+This is a Python wrapper derived from the [Bard API](https://github.com/
+dsdanielpark/Bard-API) project, designed to retrieve responses from Gemini Web
+in REST format. **Synchronous clients are preferred over asynchronous ones for
+Gemini because of rate limiting and blocking concerns.** ## Installation ð¦
+``` pip install python-gemini-api ``` ``` pip install git+https://github.com/
+dsdanielpark/Gemini-API.git ``` For the updated version, use as follows: ```
+pip install -q -U python-gemini-api ``` ## Authentication 1. Visit https://
 gemini.google.com/
 With browser open, try auto-collecting cookies first. ```python from gemini
 import Gemini GeminiClient = Gemini(auto_cookies=True) # Testing needed as
 cookies vary by region. # GeminiClient = Gemini(auto_cookies=True,
-target_cookies=["__Secure-1PSID", "__Secure-1PSIDTS"]) response =
-GeminiClient.generate_content("Hello, Gemini. What's the weather like in Seoul
-today?") print(response.payload) ``` 2. *(Manually)* `F12` for browser console
-â `Session: Application` â `Cookies` â Copy the value of some working
-cookie sets. If it doesn't work, go to step 3. Some working cookie sets Cookies
-may vary by account or region. First try `__Secure-1PSIDCC` alone. If it
-doesn't work, use `__Secure-1PSID` and `__Secure-1PSIDTS`. Still no success?
+target_cookies=["__Secure-1PSID", "__Secure-1PSIDTS"]) # GeminiClient = Gemini
+(auto_cookies=True, target_cookies="all") # You can pass whole cookies response
+= GeminiClient.generate_content("Hello, Gemini. What's the weather like in
+Seoul today?") print(response.payload) ``` 2. *(Manually)* `F12` for browser
+console â `Session: Application` â `Cookies` â Copy the value of some
+working cookie sets. If it doesn't work, go to step 3. Some working cookie sets
+Cookies may vary by account or region. First try `__Secure-1PSIDCC` alone. If
+it doesn't work, use `__Secure-1PSID` and `__Secure-1PSIDTS`. Still no success?
 Try these four cookies: `__Secure-1PSIDCC`, `__Secure-1PSID`, `__Secure-
 1PSIDTS`, `NID`. If none work, proceed to step 3 and consider sending the
 entire cookie file. 3. *(Recommended)* Export Gemini site cookies via a browser
 extension. For instance, use Chrome extension [ExportThisCookies](https://
 chromewebstore.google.com/detail/exportthiscookie/
 dannllckdimllhkiplchkcaoheibealk), open, and copy the txt file contents.
 Further: For manual collection or Required for a few users upon error 4. For
@@ -89,113 +117,104 @@
 few users upon error)* If errors persist after manually collecting cookies,
 refresh the Gemini website and collect cookies again. If errors continue, some
 users may need to manually set the nonce value. To do this: Press F12 â
 Network â Send any prompt to Gemini webui â Click the post address starting
 with "https://gemini.google.com/_/BardChatUi/data/
 assistant.lamda.BardFrontendService/StreamGenerate" â Payload â Form Data
 â Copy the "at" key value. See [this image](assets/nonce_value.pdf) for
-reference. > [!IMPORTANT] > Try different Google accounts until you find a
-working cookie. Use a fresh browser to ensure no remaining cookie values. Use
-secret browsing mode with independent cookies. Results may vary depending on
-factors like IP and account status. Providing the entire set of cookies seems
-to fix one cookie per account. Additionally, once successfully connected with
-that cookie, it seems to work flawlessly for over three weeks without any
-errors. *Try various methods until you succeed. Experiment in different
-environments.*
-## Quick Start *Simple usage* Setting Gemini response language (Optional):
-Check supported languages [here](https://developers.google.com/hotels/hotel-
-prices/dev-guide/country-codes). Default is English. ```python import os
-os.environ["GEMINI_LANGUAGE"] = "KR" ``` Generate content: returns parsed
-response. ```python from gemini import Gemini cookies = {} # Cookies may vary
-by account or region. Consider sending the entire cookie file. GeminiClient =
-Gemini(cookies=cookies) # You can use various args response =
-GeminiClient.generate_content("Hello, Gemini. What's the weather like in Seoul
-today?") response.payload ``` Generate content from image: you can use image as
-input. ```python from gemini import Gemini cookies = {} # Cookies may vary by
-account or region. Consider sending the entire cookie file. GeminiClient =
-Gemini(cookies=cookies) # You can use various args response =
-GeminiClient.generate_content("What does the text in this image say?",
-image='folder/image.jpg') response.payload ``` > [!NOTE] > If the
-generate_content method returns an empty payload, try executing it again
-without reinitializing the Gemini object.
-## Usage ### # 01. Initialization Please explicitly declare `cookies` in dict
-format. You can also enter the path to the file containing the cookie with
-`cookie_fp`(*.json, *.txt supported). Check this [sample cookie file](https://
-github.com/dsdanielpark/Gemini-API/blob/main/cookies.txt). ```python from
+reference. > [!IMPORTANT] > Experiment with different Google accounts and
+browser settings to find a working cookie. Success may vary by IP and account
+status. Once connected, a cookie typically remains effective over a month. Keep
+testing until successful.
+## Quick Start **Generate content:** returns parsed response. ```python from
+gemini import Gemini cookies = {} # Cookies may vary by account or region.
+Consider sending the entire cookie file. GeminiClient = Gemini(cookies=cookies)
+# You can use various args response = GeminiClient.generate_content("Hello,
+Gemini. What's the weather like in Seoul today?") response.payload ```
+**Generate content from image:** you can use image as input. ```python from
+gemini import Gemini cookies = {} # Cookies may vary by account or region.
+Consider sending the entire cookie file. GeminiClient = Gemini(cookies=cookies)
+# You can use various args response = GeminiClient.generate_content("What does
+the text in this image say?", image='folder/image.jpg') response.payload ``` >
+[!NOTE] > If the generate_content method returns an empty payload, try
+executing it again without reinitializing the Gemini object.
+
+## Usage *Setting language and Gemini version using environment variables:
+* Setting Gemini response language (Optional): Check supported languages [here]
+(https://developers.google.com/hotels/hotel-prices/dev-guide/country-codes).
+Default is English. ```python import os os.environ["GEMINI_LANGUAGE"] = "KR" #
+Setting Gemini response language (Optional) os.environ["GEMINI_ULTRA"] = "1" #
+Switch to Gemini-advanced response (Experimental, Optional) # In some accounts,
+access to Gemini Ultra may not be available. If that's the case, please revert
+it back to "0". ```
+### # 01. Initialization Please explicitly declare `cookies` in dict format.
+You can also enter the path to the file containing the cookie with `cookie_fp`
+(*.json, *.txt supported). Check sample cookie files in [assets](https://
+github.com/dsdanielpark/Gemini-API/tree/main/assets) folder. ```python from
 gemini import Gemini cookies = { "__Secure-1PSIDCC" : "value", "__Secure-1PSID"
 : "value", "__Secure-1PSIDTS" : "value", "NID" : "value", # Cookies may vary by
 account or region. Consider sending the entire cookie file. } GeminiClient =
 Gemini(cookies=cookies) # GeminiClient = Gemini(cookie_fp="folder/
 cookie_file.json") # (*.json, *.txt) are supported. # GeminiClient = Gemini
-(auto_cookies=True) # Or use auto_cookies paprameter ``` #### Auto Cookie
-Update For `auto_cookie` to be set to `True`, Gemini WebUI must be active in
-the browser. The [browser_cookie3](https://github.com/borisbabic/
-browser_cookie3) enables automatic cookie collection, though updates may not be
-complete yet. > [!IMPORTANT] > **If the session connects successfully and
-`generate_content` runs well, CLOSE Gemini website.** If Gemini web stays open
-in the browser, cookies may expire faster.
+(auto_cookies=True) # Or use auto_cookies paprameter ``` ##### Auto Cookie
+Update For `auto_cookie` to be set to `True`, and adjust `target_cookies`.
+Gemini WebUI must be active in the browser. The [browser_cookie3](https://
+github.com/borisbabic/browser_cookie3) enables automatic cookie collection,
+though updates may not be complete yet.
 ### # 02. Generate content Returns Gemini's response, but the first one might
-be empty. If generate_content yields an empty payload, rerun it without
-reinitializing Gemini. Regardless of model output type, access the
-response_dict property (renamed to payload after v2.3.0). https://github.com/
-dsdanielpark/Gemini-API/blob/fdf064c57bc1fb47fbbb4b93067618a200e77f62/gemini/
-core.py#L252 ```python prompt = "Hello, Gemini. What's the weather like in
-Seoul today?" response = GeminiClient.generate_content(prompt) print
-(response.payload) ``` > [!IMPORTANT] > Once connected and generating valid
-content, **Be sure to CLOSE the Gemini website or CLOSE your browser** for
-cookie stability.
+be empty. ```python prompt = "Hello, Gemini. What's the weather like in Seoul
+today?" response = GeminiClient.generate_content(prompt) print
+(response.payload) ``` > [!IMPORTANT] > DO NOT send same prompt repeatly. **If
+the session connects successfully and `generate_content` runs well, CLOSE
+Gemini website.** If Gemini web stays open in the browser, cookies may expire
+faster.
 The output of the generate_content function is `GeminiModelOutput`, with the
-following structure: **Properties of GeminiModelOutput:** - *rcid*: returns the
-response candidate id of the chosen candidate. - *text*: returns the text of
-the chosen candidate. - *code*: returns the codes of the chosen candidate. -
-*web_images*: returns a list of web images from the chosen candidate. -
-*generated_images*: returns a list of generated images from the chosen
-candidate. - *payload*: returns the response dictionary, if available. (same as
-*reponse_dict* under v2.3.0) https://github.com/dsdanielpark/Gemini-API/blob/
-fdf064c57bc1fb47fbbb4b93067618a200e77f62/gemini/src/model/output.py#L16 >
-[!NOTE] > If the session fails to connect, works improperly, or terminates,
-returning an error, it is recommended to manually renew the cookies. The error
-is likely due to incorrect cookie values. Refresh or log out of Gemini web to
-renew cookies and try again.
+following structure: - *rcid*: returns the response candidate id of the chosen
+candidate. - *text*: returns the text of the chosen candidate. - *code*:
+returns the codes of the chosen candidate. - *web_images*: returns a list of
+web images from the chosen candidate. - *generated_images*: returns a list of
+generated images from the chosen candidate. - *payload*: returns the response
+dictionary, if available. https://github.com/dsdanielpark/Gemini-API/blob/
+fdf064c57bc1fb47fbbb4b93067618a200e77f62/gemini/src/model/output.py#L16
 ### # 03. Send request Send request: returns the request's payload and
 status_code, making debugging easier. ```python from gemini import Gemini
 cookies = {} # Cookies may vary by account or region. Consider sending the
 entire cookie file. GeminiClient = Gemini(cookies=cookies) # You can use
 various args response_text, response_status = GeminiClient.send_request("Hello,
-Gemini. What's the weather like in Seoul today?") print(response_text) ```
+Gemini. What's the weather like in Seoul today?") print(response_text) ``` You
+can track the total number of requests made by accessing the `request_count`
+property within the `Gemini` class.
 ### # 04. Text generation Returns text generated by Gemini. ```python prompt =
 "Hello, Gemini. What's the weather like in Seoul today?" response =
 GeminiClient.generate_content(prompt) print(response.text) ```
-### # 05. Image generation Returns images generated by Gemini. https://
-github.com/dsdanielpark/Gemini-API/blob/
-fdf064c57bc1fb47fbbb4b93067618a200e77f62/gemini/src/model/image.py#L12 *Sync
-downloader* ```python from gemini import Gemini, GeminiImage response =
-GeminiClient.generate_content("Create illustrations of Seoul, South Korea.")
-generated_images = response.generated_images # Check generated images [Dict]
-GeminiImage.save_sync(generated_images, save_path="save_dir", cookies=cookies)
-# You can use byte type image dict for printing images as follow: #
-bytes_images_dict = GeminiImage.fetch_images_dict_sync(generated_images,
-cookies=cookies) # Get bytes images dict # GeminiImage.save_images_sync
-(bytes_images_dict, path="save_dir", cookies=cookies) # Save to path ```
-Display images in IPython You can display the image or transmit it to another
-application in byte format. ``` bytes_images_dict =
+### # 05. Image generation Returns images generated by Gemini. *Async
+downloader* ```python response = GeminiClient.generate_content("Create
+illustrations of Seoul, South Korea.") generated_images =
+response.generated_images # Check generated images [Dict] await
+GeminiImage.save(generated_images, "save_dir", cookies=cookies) #
+image_data_dict = await GeminiImage.fetch_images_dict(generated_images,
+cookies=cookies) # await GeminiImage.save_images(image_data_dict, "save_dir")
+``` Further *Display images in IPython* You can display the image or transmit
+it to another application in byte format. ```python bytes_images_dict =
 GeminiImage.fetch_images_dict_sync(generated_images, cookies) # Get bytes
 images dict from IPython.display import display, Image import io for
 image_name, image_bytes in bytes_images_dict.items(): print(image_name) image =
-Image(data=image_bytes) display(image) ``` *Async downloader* ```python
-response = GeminiClient.generate_content("Create illustrations of Seoul, South
-Korea.") generated_images = response.generated_images # Check generated images
-[Dict] await GeminiImage.save(generated_images, "save_dir", cookies=cookies) #
-image_data_dict = await GeminiImage.fetch_images_dict(generated_images,
-cookies=cookies) # await GeminiImage.save_images(image_data_dict, "save_dir")
-``` Async downloader wrapper ``` import asyncio from gemini import Gemini,
-GeminiImage async def save_generated_imagse(generated_imagse,
-save_path="save_dir", cookies=cookies): await GeminiImage.save
-(generated_imagse, save_path=save_path, cookies=cookies) # Run the async
-function if __name__ == "__main__": cookies = {"key" : "value"}
+Image(data=image_bytes) display(image) ``` *Sync downloader* ```python from
+gemini import Gemini, GeminiImage response = GeminiClient.generate_content
+("Create illustrations of Seoul, South Korea.") generated_images =
+response.generated_images # Check generated images [Dict] GeminiImage.save_sync
+(generated_images, save_path="save_dir", cookies=cookies) # You can use byte
+type image dict for printing images as follow: # bytes_images_dict =
+GeminiImage.fetch_images_dict_sync(generated_images, cookies=cookies) # Get
+bytes images dict # GeminiImage.save_images_sync(bytes_images_dict,
+path="save_dir", cookies=cookies) # Save to path ``` *Async downloader wrapper*
+```python import asyncio from gemini import Gemini, GeminiImage async def
+save_generated_imagse(generated_imagse, save_path="save_dir", cookies=cookies):
+await GeminiImage.save(generated_imagse, save_path=save_path, cookies=cookies)
+# Run the async function if __name__ == "__main__": cookies = {"key" : "value"}
 generated_imagse = response.generated_imagse asyncio.run(save_generated_imagse
 (generated_imagse, save_path="save_dir", cookies=cookies)) ```
 `GeminiImage.save` method logic ``` import asyncio from gemini import Gemini,
 GeminiImage async def save_generated_imagse(generated_imagse,
 save_path="save_dir", cookies=cookies): image_data_dict = await
 GeminiImage.fetch_images_dict(generated_imagse, cookies=cookies) # Get bytes
 images dict asynchronously await GeminiImage.save_images(image_data_dict,
@@ -204,38 +223,38 @@
 Check response images [Dict] asyncio.run(save_generated_imagse
 (generated_imagse, save_path="save_dir", cookies=cookies)) ``` > [!NOTE] > Use
 GeminiImage for image processing. `web_images` works without cookies, but for
 images like `generated_image` from Gemini, pass cookies. Cookies are needed to
 download images from Google's storage. Check the response or use existing
 cookies variable.
 ### # 06. Retrieving Images from Gemini Responses Returns images in response of
-Gemini. *Sync downloader* ```python from gemini import Gemini, GeminiImage
-response = GeminiClient.generate_content("Please recommend a travel itinerary
-for Seoul.") response_images = response.web_images # Check response images
-[Dict] GeminiImage.save_sync(response_images, save_path="save_dir") # You can
-use byte type image dict as follow: # bytes_images_dict =
-GeminiImage.fetch_bytes_sync(response_images, cookies) # Get bytes images dict
-# GeminiImage.save_images_sync(bytes_images_dict, path="save_dir") # Save to
-path ``` *Async downloader* ```python response = GeminiClient.generate_content
+Gemini. *Async downloader* ```python response = GeminiClient.generate_content
 ("Create illustrations of Seoul, South Korea.") response_images =
 response.web_images # Check generated images [Dict] await GeminiImage.save
 (response_images, "save_dir") # image_data_dict = await
 GeminiImage.fetch_images_dict(response_images) # await GeminiImage.save_images
-(image_data_dict, "save_dir") ``` Async downloader wrapper ``` import asyncio
-from gemini import Gemini, GeminiImage async def save_response_web_imagse
-(response_images, save_path="save_dir", cookies=cookies): await
-GeminiImage.save(response_images, save_path=save_path, cookies=cookies) # Run
-the async function if __name__ == "__main__": cookies = {"key" : "value"}
-response_images = response.web_images asyncio.run(save_response_web_imagse
-(response_images, save_path="save_dir", cookies=cookies)) ```
-`GeminiImage.save` method logic ``` import asyncio from gemini import Gemini,
-GeminiImage async def save_response_web_imagse(response_images,
-save_path="save_dir", cookies=cookies): image_data_dict = await
-GeminiImage.fetch_images_dict(response_images, cookies=cookies) # Get bytes
-images dict asynchronously await GeminiImage.save_images(image_data_dict,
+(image_data_dict, "save_dir") ``` Further *Sync downloader* ```python from
+gemini import Gemini, GeminiImage response = GeminiClient.generate_content
+("Please recommend a travel itinerary for Seoul.") response_images =
+response.web_images # Check response images [Dict] GeminiImage.save_sync
+(response_images, save_path="save_dir") # You can use byte type image dict as
+follow: # bytes_images_dict = GeminiImage.fetch_bytes_sync(response_images,
+cookies) # Get bytes images dict # GeminiImage.save_images_sync
+(bytes_images_dict, path="save_dir") # Save to path ``` *Async downloader
+wrapper* ```python import asyncio from gemini import Gemini, GeminiImage async
+def save_response_web_imagse(response_images, save_path="save_dir",
+cookies=cookies): await GeminiImage.save(response_images, save_path=save_path,
+cookies=cookies) # Run the async function if __name__ == "__main__": cookies =
+{"key" : "value"} response_images = response.web_images asyncio.run
+(save_response_web_imagse(response_images, save_path="save_dir",
+cookies=cookies)) ``` `GeminiImage.save` method logic ``` import asyncio from
+gemini import Gemini, GeminiImage async def save_response_web_imagse
+(response_images, save_path="save_dir", cookies=cookies): image_data_dict =
+await GeminiImage.fetch_images_dict(response_images, cookies=cookies) # Get
+bytes images dict asynchronously await GeminiImage.save_images(image_data_dict,
 save_path=save_path) # Run the async function if __name__ == "__main__":
 response_images = response.web_images # Check response images [Dict]
 asyncio.run(save_response_web_imagse(response_images, save_path="save_dir",
 cookies=cookies)) ```
 ### # 07. Generate content from images Takes an image as input and returns a
 response. ```python image = 'folder/image.jpg' # image = open('folder/
 image.jpg', 'rb').read() # (jpg, jpeg, png, webp) are supported. response =
@@ -261,93 +280,111 @@
 tailored travel itineraries. - Features: Holiday preparation, price comparison,
 trip planning - Google Hotels - Service: **@Google Hotels** - Description:
 Search for hotels considering what matters most to you, like having a
 conversation with a friend. - Features: Packing for travel, sightseeing,
 special relaxation - YouTube - Service: **@YouTube** - Description: Explore
 YouTube videos and ask questions about what interests you. - Features: Problem-
 solving, generating ideas, search, exploring topics
-### # 09. Fix context setting rcid You can specify a particular response by
-setting its response candidate id(rcid). ```python # Generate content for the
+### # 09. Fix context setting RCID You can specify a particular response by
+setting its Response Candidate ID(RCID). ```python # Generate content for the
 prompt "Give me some information about the USA." response1 =
 GeminiClient.generate_content("Give me some information about the USA.") #
 After reviewing the responses, choose the one you prefer and copy its RCID.
 GeminiClient.rcid = "rc_xxxx" # Now, generate content for the next prompt "How
 long does it take from LA to New York?" response2 =
-GeminiClient.generate_content("How long does it take from LA to New York?") ```
-
+GeminiClient.generate_content("How long does it take from LA to New York?") #
+However, RCID may not persist. If parsing fails, reset `GeminiClient.rcid` to
+None. # GeminiClient.rcid = None ```
 ### # 10. Changing the Selected Response from 0 to *n* In Gemini,
 generate_content returns the first response. This may vary depending on length
 or sorting. Therefore, you can specify the index of the chosen response from 0
 to *n* as follows. However, if there is only one response, revert it back to 0.
 ```python from gemini import GeminiModelOutput GeminiModelOutput.chosen = 1 #
-default is 0 response1 = GeminiClient.generate_content("Give me some
-information about the USA.") ```
+default is 0 response_choice_1 = GeminiClient.generate_content("Give me some
+information about the USA.") # If not all Gemini returns are necessarily
+plural, revert back to 0 in case of errors. # GeminiModelOutput.chosen = 0 ```
 ### # 11. Generate custom content Parse the response text to extract desired
-values. https://github.com/dsdanielpark/Gemini-API/blob/
-fdf064c57bc1fb47fbbb4b93067618a200e77f62/gemini/core.py#L317 Using
-`Gemini.generate_custom_content`, specify custom parsing to extract specific
-values. Utilize ParseMethod1 and ParseMethod2 by default, and you can pass
-custom parsing methods as arguments if desired. Refer to [custom_parser.py]
-(https://github.com/dsdanielpark/Gemini-API/blob/main/gemini/src/model/parser/
-custom_parser.py). ```python # You can create a parser method that takes
-response_text as the input for custom_parser. response_text, response_status =
-GeminiClient.send_request("Give me some information about the USA.") # Use
-custom_parser function or class inheriting from BaseParser response =
-GeminiClient.generate_custom_content("Give me some information about the USA.",
-*custom_parser) ```
-## Further ### Use rotating proxies If you want to **avoid blocked requests**
-and bans, then use [Smart Proxy by Crawlbase](https://crawlbase.com/docs/smart-
-proxy/?utm_source=github_ad&utm_medium=social&utm_campaign=bard_api). It
-forwards your connection requests to a **randomly rotating IP address** in a
-pool of proxies before reaching the target website. The combination of AI and
-ML make it more effective to avoid CAPTCHAs and blocks. ```python # Get your
-proxy url at crawlbase https://crawlbase.com/docs/smart-proxy/get/ proxy_url =
-"http://xxxxx:@smartproxy.crawlbase.com:8012" proxies = {"http": proxy_url,
-"https": proxy_url} GeminiClient = Gemini(cookies=cookies, proxies=proxies,
-timeout=30) GeminiClient.generate_content("Hello, Gemini. Give me a beautiful
-photo of Seoul's scenery.") ``` ### Reusable session object For standard cases,
-use Gemini class; for exceptions, use session objects. When creating a new bot
-Gemini server, adjust Headers.MAIN. ```python from gemini import Gemini,
-Headers import requests cookies = {} session = requests.Session()
+values. Using `Gemini.generate_custom_content`, specify custom parsing to
+extract specific values. Utilize ParseMethod1 and ParseMethod2 by default, and
+you can pass custom parsing methods as arguments if desired. Refer to
+[custom_parser.py](https://github.com/dsdanielpark/Gemini-API/blob/main/gemini/
+src/model/parser/custom_parser.py). ```python # You can create a parser method
+that takes response_text as the input for custom_parser. response_text,
+response_status = GeminiClient.send_request("Give me some information about the
+USA.") # Use custom_parser function or class inheriting from BaseParser
+response = GeminiClient.generate_custom_content("Give me some information about
+the USA.", *custom_parser) ``` https://github.com/dsdanielpark/Gemini-API/blob/
+31b842488bbc5429ad9c74b1d8b00e20d94e8cb1/gemini/client.py#L323
+## Further ### Use rotating proxies via [Smart Proxy by Crawlbase](https://
+crawlbase.com/docs/smart-proxy/
+?utm_source=github_ad&utm_medium=social&utm_campaign=bard_api) If you want to
+**avoid blocked requests** and bans, then use [Smart Proxy by Crawlbase](https:
+//crawlbase.com/docs/smart-proxy/
+?utm_source=github_ad&utm_medium=social&utm_campaign=bard_api). It forwards
+your connection requests to a **randomly rotating IP address** in a pool of
+proxies before reaching the target website. The combination of AI and ML make
+it more effective to avoid CAPTCHAs and blocks. ```python # Get your proxy url
+at crawlbase https://crawlbase.com/docs/smart-proxy/get/ proxy_url = "http://
+xxxxx:@smartproxy.crawlbase.com:8012" proxies = {"http": proxy_url, "https":
+proxy_url} GeminiClient = Gemini(cookies=cookies, proxies=proxies, timeout=30)
+GeminiClient.generate_content("Hello, Gemini. Give me a beautiful photo of
+Seoul's scenery.") ``` ### Reusable session object For standard cases, use
+Gemini class; for exceptions, use session objects. When creating a new bot
+Gemini server, adjust Headers.MAIN. ```python import requests from gemini
+import Gemini, Headers cookies = {} session = requests.Session()
 session.headers = Headers.MAIN for key, value in cookies.items():
 session.cookies.update({key: value}) GeminiClient = Gemini(session=session) #
 You can use various args response = GeminiClient.generate_content("Hello,
 Gemini. What's the weather like in Seoul today?") ```
 ## [More features](https://github.com/dsdanielpark/Gemini-API/blob/main/
 documents/README_DEV.md) Explore additional features in [this document](https:/
 /github.com/dsdanielpark/Gemini-API/blob/main/documents/README_DEV.md). If you
 want to develop your own simple code, you can start from [this simple code
 example](https://github.com/dsdanielpark/Gemini-API/blob/main/script/
 sample.ipynb).
-## Open-source LLM, [Gemma](https://huggingface.co/google/gemma-7b) If you have
-sufficient GPU resources, you can download weights directly instead of using
-the Gemini API to generate content. Consider Gemma, an open-source model
-**available for on-premises use**. [Gemma](https://huggingface.co/google/gemma-
-7b) models are Google's lightweight, advanced text-to-text, decoder-only
-language models, derived from Gemini research. Available in English, they offer
-open weights and variants, ideal for tasks like question answering and
-summarization. Their small size enables deployment in resource-limited
-settings, broadening access to cutting-edge AI. For more infomation, visit
-[Gemma-7b](https://huggingface.co/google/gemma-7b) model card. ### How to use
-Gemma ```python from transformers import AutoTokenizer, AutoModelForCausalLM
-tokenizer = AutoTokenizer.from_pretrained("google/gemma-7b") model =
+## Google Open-source LLMs If you have sufficient GPU resources, you can
+download weights directly instead of using the Gemini API to generate content.
+Consider Gemma and Code Gemma, an open-source models **available for on-
+premises use**. ### Open-source LLM, [Gemma](https://huggingface.co/google/
+gemma-7b) Gemma models are Google's lightweight, advanced text-to-text,
+decoder-only language models, derived from Gemini research. Available in
+English, they offer open weights and variants, ideal for tasks like question
+answering and summarization. For more infomation, visit [Gemma-7b](https://
+huggingface.co/google/gemma-7b) model card. #### How to use Gemma ```python
+from transformers import AutoTokenizer, AutoModelForCausalLM tokenizer =
+AutoTokenizer.from_pretrained("google/gemma-7b") model =
 AutoModelForCausalLM.from_pretrained("google/gemma-7b") input_text = "Write me
 a poem about Machine Learning." input_ids = tokenizer(input_text,
 return_tensors="pt") outputs = model.generate(**input_ids) print
+(tokenizer.decode(outputs[0])) ``` ### Open-source LLM, [Code Gemma](https://
+huggingface.co/collections/google/codegemma-release-66152ac7b683e2667abdee11)
+CodeGemma, which is an official release from Google for code LLMs, was released
+on April 9, 2024. It provides three models specifically designed for generating
+and interacting with code. You can explore the [Code Gemma models](https://
+huggingface.co/collections/google/codegemma-release-66152ac7b683e2667abdee11)
+and view the [model card](https://huggingface.co/google/codegemma-7b-it) for
+more details. #### How to use Code Gemma ```python from transformers import
+GemmaTokenizer, AutoModelForCausalLM tokenizer = GemmaTokenizer.from_pretrained
+("google/codegemma-7b-it") model = AutoModelForCausalLM.from_pretrained
+("google/codegemma-7b-it") input_text = "Write me a Python function to
+calculate the nth fibonacci number." input_ids = tokenizer(input_text,
+return_tensors="pt") outputs = model.generate(**input_ids) print
 (tokenizer.decode(outputs[0])) ```
 ## Utilize free open-source LLM API through [Open Router](https://
 openrouter.ai/) OpenRouter offers temporary free inference for select models.
 Obtain an API key from [Open Router API](https://openrouter.ai/keys) and check
 free models at [Open Router models](https://openrouter.ai/docs#models). Use
 models with a 0-dollar token cost primarily; other models may incur charges.
-See more [free open-source LLM API guide](https://github.com/dsdanielpark/
-Gemini-API/blob/main/documents/README_OPENROUTER.md) > [!NOTE] > You can easily
-receive responses from open LLMs without this package by following the
-instructions on [here](https://openrouter.ai/docs#models). ```python from
-gemini import OpenRouter OPENROUTER_API_KEY = "" GemmaClient = OpenRouter
+See more at [free open-source LLM API guide](https://github.com/dsdanielpark/
+Gemini-API/blob/main/documents/README_OPENROUTER.md). **Sync client is favored
+over async for Gemini due to rate limiting and blocking issues**, but
+OpenRouter offers reliable open-source LLMs for [async implementation](https://
+github.com/dsdanielpark/Gemini-API/blob/main/documents/
+README_OPENROUTER.md#openrouter-async-api-client). ```python from gemini import
+OpenRouter OPENROUTER_API_KEY = "" GemmaClient = OpenRouter
 (api_key=OPENROUTER_API_KEY, model="google/gemma-7b-it:free") prompt = "Do you
 know UCA academy in Korea? https://blog.naver.com/ulsancoding" response =
 GemmaClient.create_chat_completion(prompt) print(response) # payload =
 GemmaClient.generate_content(prompt) # print(payload.json()) ``` The free model
 list includes: - `google/gemma-7b-it:free` - [google/gemma-7b](https://
 huggingface.co/google/gemma-7b) from Google *** - `mistralai/mistral-7b-
 instruct:free` - [mistralai/Mistral-7B-Instruct-v0.1](https://huggingface.co/
@@ -358,38 +395,38 @@
 `openrouter/cinematika-7b:free` - [jondurbin/cinematika-7b-v0.1](https://
 huggingface.co/jondurbin/cinematika-7b-v0.1) - `undi95/toppy-m-7b:free` -
 [Undi95/Toppy-M-7B](https://huggingface.co/Undi95/Toppy-M-7B?not-for-all-
 audiences=true) - `gryphe/mythomist-7b:free` - [Gryphe/MythoMist-7b](https://
 huggingface.co/Gryphe/MythoMist-7b) - `nousresearch/nous-capybara-7b:free` -
 [NousResearch/Nous-Capybara-7B-V1](https://huggingface.co/NousResearch/Nous-
 Capybara-7B-V1) from Nous Research
+## Sponsor, [Crawlbase](https://crawlbase.com/) Use [Crawlbase](https://
+crawlbase.com/) API for efficient data scraping to train AI models, boasting a
+98% success rate and 99.9% uptime. It's quick to start, GDPR/CCPA compliant,
+supports massive data extraction, and is trusted by 70k+ developers.
 ## [FAQ](https://github.com/dsdanielpark/Gemini-API/blob/main/documents/
 README_FAQ.md) First review [HanaokaYuzu/Gemini-API](https://github.com/
 HanaokaYuzu/Gemini-API) and the [Official Google Gemini API](https://
 aistudio.google.com/) before using this package. You can find most help on the
 [FAQ](https://github.com/dsdanielpark/Gemini-API/blob/main/documents/
 README_FAQ.md) and [Issue](https://github.com/dsdanielpark/Gemini-API/issues)
 pages. ## [Issues](https://github.com/dsdanielpark/Gemini-API/issues) Sincerely
 grateful for any reports on new features or bugs. Your valuable feedback on the
 code is highly appreciated. Frequent errors may occur due to changes in
 Google's service API interface. Both [Issue reports](https://github.com/
 dsdanielpark/Gemini-API/issues) and [Pull requests](https://github.com/
 dsdanielpark/Gemini-API/pulls) contributing to improvements are always welcome.
-We strive to maintain an active and courteous open community. ## Sponsor Use
-[Crawlbase](https://crawlbase.com/) API for efficient data scraping to train AI
-models, boasting a 98% success rate and 99.9% uptime. It's quick to start,
-GDPR/CCPA compliant, supports massive data extraction, and is trusted by 70k+
-developers. ## Contributors We would like to express our sincere gratitude to
-all the contributors. This package aims to re-implement the functionality of
-the [Bard API](https://github.com/dsdanielpark/Bard-API/), which has been
-archived for the contributions of the beloved open-source community, despite
-Gemini's official API already being available. Contributors to the [Bard API]
-(https://github.com/dsdanielpark/Bard-API/) and [Gemini API](https://
-github.com/dsdanielpark/Gemini-API/). _[_h_t_t_p_s_:_/_/_c_o_n_t_r_i_b_._r_o_c_k_s_/
-_i_m_a_g_e_?_r_e_p_o_=_d_s_d_a_n_i_e_l_p_a_r_k_/_B_a_r_d___A_P_I_]
+We strive to maintain an active and courteous open community. ## Contributors
+We would like to express our sincere gratitude to all the contributors. This
+package aims to re-implement the functionality of the [Bard API](https://
+github.com/dsdanielpark/Bard-API/), which has been archived for the
+contributions of the beloved open-source community, despite Gemini's official
+API already being available. Contributors to the [Bard API](https://github.com/
+dsdanielpark/Bard-API/) and [Gemini API](https://github.com/dsdanielpark/
+Gemini-API/). _[_h_t_t_p_s_:_/_/_c_o_n_t_r_i_b_._r_o_c_k_s_/_i_m_a_g_e_?_r_e_p_o_=_d_s_d_a_n_i_e_l_p_a_r_k_/_B_a_r_d___A_P_I_]
 Further development potential Modifications to the async client using my logic
 are needed, along with automatic cookie collection via browser_cookie3, and
 implementation of other Bard API features (such as code extraction, export to
 Replit, graph drawing, etc.). Please note that while reviewing automatic cookie
 collection, it appears that cookies expire immediately upon sending a request
 for collection. Efforts to make it more user-friendly were unsuccessful. Also,
 the _sid value seems to work normally even when returned as None. Lastly, if
@@ -401,21 +438,38 @@
 Cheong](https://github.com/acheong08) / teapotv8@proton.me
 - [Daniel Park](https://github.com/DSDanielPark) / parkminwoo1991@gmail.com ##
 License Â©ï¸ [MIT](https://opensource.org/license/mit/) license, 2024. We
 hereby strongly disclaim any explicit or implicit legal liability related to
 our works. Users are required to use this package responsibly and at their own
 risk. This project is a personal initiative and is not affiliated with or
 endorsed by Google. It is recommended to use Google's official API. ##
-References [1] Github: [acheong08/Bard](https://github.com/acheong08/Bard)
-[2] GitHub: [HanaokaYuzu/Gemini-API](https://github.com/HanaokaYuzu/Gemini-API)
-
-[3] Github: [dsdanielpark/Bard-API](https://github.com/dsdanielpark/Bard-API)
-[4] Github: [GoogleCloudPlatform/generative-ai](https://github.com/
+References [1]: Paper - [Introducing GEMINI: Multimodal Generative Models]
+(https://arxiv.org/abs/2312.11805)
+[2]: Website - [Google DeepMind :: GEMINI Introduction](https://
+deepmind.google/technologies/gemini/#introduction)
+[3]: Paper - [GEMMA: A Unified Language Model for Text Generation,
+Understanding, Translation, Coding, and Math.]()
+[4]: Website - [AI at Google :: GEMS Documentation](https://ai.google.dev/
+gemma/docs)
+[5]: Report - [CodeGMMA: Large Language Models Can Write Realistic Programming
+Assignments](https://storage.googleapis.com/deepmind-media/gemma/
+codegemma_report.pdf?utm_source=substack&utm_medium=email)
+[6]: Blog Post - [Announcing CodeGen: Building Better Developersâ Tools Using
+LLMs](https://huggingface.co/blog/codegen)
+[7]: Collection - [Google :: CodeGen Release](https://huggingface.co/
+collections/google/codegen-release-5d0f4c4eaedbc5cefcfdcbdf)
+[8]: Github - [acheong08/Bard](https://github.com/acheong08/Bard)
+[9]: GitHub - [HanaokaYuzu/Gemini-API](https://github.com/HanaokaYuzu/Gemini-
+API)
+[10]: Github - [dsdanielpark/Bard-API](https://github.com/dsdanielpark/Bard-
+API)
+[11]: Github - [GoogleCloudPlatform/generative-ai](https://github.com/
 GoogleCloudPlatform/generative-ai)
-[5] Github: [OpenRouter](https://github.com/OpenRouterTeam/openrouter-runner)
-[6] WebSite: [Google AI Studio](https://ai.google.dev/tutorials/ai-
+[12]: Github - [OpenRouter](https://github.com/OpenRouterTeam/openrouter-
+runner)
+[13]: WebSite - [Google AI Studio](https://ai.google.dev/tutorials/ai-
 studio_quickstart)
 > *Warning* Users assume full legal responsibility for GeminiAPI. Not endorsed
 by Google. Excessive use may lead to account restrictions. Changes in policies
 or account status may affect functionality. Utilize issue and discussion pages.
 
 ## Requirements Python 3.7 or higher.
```

### Comparing `python-gemini-api-2.4.2/python_gemini_api.egg-info/SOURCES.txt` & `python_gemini_api-2.4.3/python_gemini_api.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -17,15 +17,17 @@
 gemini/src/model/output.py
 gemini/src/model/parser/__init__.py
 gemini/src/model/parser/base.py
 gemini/src/model/parser/custom_parser.py
 gemini/src/model/parser/response_parser.py
 gemini/src/modules/__init__.py
 gemini/src/modules/openrouter/__init__.py
+gemini/src/modules/openrouter/async_client.py
 gemini/src/modules/openrouter/client.py
+gemini/src/modules/openrouter/const.py
 gemini/src/modules/voice/__init__.py
 gemini/src/modules/voice/google.py
 gemini/src/modules/voice/openai.py
 python_gemini_api.egg-info/PKG-INFO
 python_gemini_api.egg-info/SOURCES.txt
 python_gemini_api.egg-info/dependency_links.txt
 python_gemini_api.egg-info/entry_points.txt
```

### Comparing `python-gemini-api-2.4.2/setup.py` & `python_gemini_api-2.4.3/setup.py`

 * *Files identical despite different names*


# Comparing `tmp/python_gemini_api-2.4.5.tar.gz` & `tmp/python_gemini_api-2.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_gemini_api-2.4.5.tar", last modified: Wed Apr 24 10:47:04 2024, max compression
+gzip compressed data, was "python_gemini_api-2.4.6.tar", last modified: Wed Apr 24 13:05:42 2024, max compression
```

## Comparing `python_gemini_api-2.4.5.tar` & `python_gemini_api-2.4.6.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxrwx   0        0        0        0 2024-04-24 10:47:04.652225 python_gemini_api-2.4.5/
--rw-rw-rw-   0        0        0     1097 2024-04-24 10:39:19.000000 python_gemini_api-2.4.5/LICENSE
--rw-rw-rw-   0        0        0    36565 2024-04-24 10:47:04.651224 python_gemini_api-2.4.5/PKG-INFO
--rw-rw-rw-   0        0        0    35262 2024-04-24 10:16:55.000000 python_gemini_api-2.4.5/README.md
-drwxrwxrwx   0        0        0        0 2024-04-24 10:47:04.591519 python_gemini_api-2.4.5/gemini/
--rw-rw-rw-   0        0        0     1445 2024-04-24 10:39:39.000000 python_gemini_api-2.4.5/gemini/__init__.py
--rw-rw-rw-   0        0        0    15192 2024-03-18 04:20:24.000000 python_gemini_api-2.4.5/gemini/async_client.py
--rw-rw-rw-   0        0        0    19096 2024-04-17 13:21:33.000000 python_gemini_api-2.4.5/gemini/client.py
-drwxrwxrwx   0        0        0        0 2024-04-24 10:47:04.592528 python_gemini_api-2.4.5/gemini/src/
--rw-rw-rw-   0        0        0        0 2024-03-05 10:25:37.000000 python_gemini_api-2.4.5/gemini/src/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 10:47:04.596472 python_gemini_api-2.4.5/gemini/src/extensions/
--rw-rw-rw-   0        0        0       40 2024-03-16 06:40:55.000000 python_gemini_api-2.4.5/gemini/src/extensions/__init__.py
--rw-rw-rw-   0        0        0      622 2024-03-18 04:30:10.000000 python_gemini_api-2.4.5/gemini/src/extensions/replit.py
-drwxrwxrwx   0        0        0        0 2024-04-24 10:47:04.605401 python_gemini_api-2.4.5/gemini/src/misc/
--rw-rw-rw-   0        0        0      265 2024-04-17 09:46:31.000000 python_gemini_api-2.4.5/gemini/src/misc/__init__.py
--rw-rw-rw-   0        0        0     9279 2024-04-05 10:13:11.000000 python_gemini_api-2.4.5/gemini/src/misc/constants.py
--rw-rw-rw-   0        0        0     3063 2024-03-18 04:29:01.000000 python_gemini_api-2.4.5/gemini/src/misc/decorator.py
--rw-rw-rw-   0        0        0     2421 2024-04-20 13:54:53.000000 python_gemini_api-2.4.5/gemini/src/misc/exceptions.py
--rw-rw-rw-   0        0        0     4487 2024-04-17 09:46:59.000000 python_gemini_api-2.4.5/gemini/src/misc/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-24 10:47:04.611045 python_gemini_api-2.4.5/gemini/src/model/
--rw-rw-rw-   0        0        0       88 2024-03-16 06:40:55.000000 python_gemini_api-2.4.5/gemini/src/model/__init__.py
--rw-rw-rw-   0        0        0     8611 2024-03-18 04:29:31.000000 python_gemini_api-2.4.5/gemini/src/model/image.py
--rw-rw-rw-   0        0        0     1858 2024-03-31 11:20:09.000000 python_gemini_api-2.4.5/gemini/src/model/output.py
-drwxrwxrwx   0        0        0        0 2024-04-24 10:47:04.618378 python_gemini_api-2.4.5/gemini/src/model/parser/
--rw-rw-rw-   0        0        0      130 2024-03-17 09:52:54.000000 python_gemini_api-2.4.5/gemini/src/model/parser/__init__.py
--rw-rw-rw-   0        0        0     1490 2024-03-05 10:15:40.000000 python_gemini_api-2.4.5/gemini/src/model/parser/base.py
--rw-rw-rw-   0        0        0     5433 2024-03-31 11:20:09.000000 python_gemini_api-2.4.5/gemini/src/model/parser/custom_parser.py
--rw-rw-rw-   0        0        0     7692 2024-03-31 11:20:09.000000 python_gemini_api-2.4.5/gemini/src/model/parser/response_parser.py
-drwxrwxrwx   0        0        0        0 2024-04-24 10:47:04.620388 python_gemini_api-2.4.5/gemini/src/modules/
--rw-rw-rw-   0        0        0        0 2024-03-29 00:25:32.000000 python_gemini_api-2.4.5/gemini/src/modules/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 10:47:04.627469 python_gemini_api-2.4.5/gemini/src/modules/openrouter/
--rw-rw-rw-   0        0        0      102 2024-04-21 13:59:49.000000 python_gemini_api-2.4.5/gemini/src/modules/openrouter/__init__.py
--rw-rw-rw-   0        0        0     3043 2024-04-21 13:58:36.000000 python_gemini_api-2.4.5/gemini/src/modules/openrouter/async_client.py
--rw-rw-rw-   0        0        0     4748 2024-04-21 13:58:36.000000 python_gemini_api-2.4.5/gemini/src/modules/openrouter/client.py
--rw-rw-rw-   0        0        0      447 2024-04-21 14:07:31.000000 python_gemini_api-2.4.5/gemini/src/modules/openrouter/const.py
-drwxrwxrwx   0        0        0        0 2024-04-24 10:47:04.633719 python_gemini_api-2.4.5/gemini/src/modules/voice/
--rw-rw-rw-   0        0        0       88 2024-03-18 04:18:39.000000 python_gemini_api-2.4.5/gemini/src/modules/voice/__init__.py
--rw-rw-rw-   0        0        0     2441 2024-03-18 04:18:26.000000 python_gemini_api-2.4.5/gemini/src/modules/voice/google.py
--rw-rw-rw-   0        0        0     3144 2024-03-17 14:01:32.000000 python_gemini_api-2.4.5/gemini/src/modules/voice/openai.py
-drwxrwxrwx   0        0        0        0 2024-04-24 10:47:04.647735 python_gemini_api-2.4.5/python_gemini_api.egg-info/
--rw-rw-rw-   0        0        0    36565 2024-04-24 10:47:04.000000 python_gemini_api-2.4.5/python_gemini_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1102 2024-04-24 10:47:04.000000 python_gemini_api-2.4.5/python_gemini_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-24 10:47:04.000000 python_gemini_api-2.4.5/python_gemini_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2024-04-24 10:47:04.000000 python_gemini_api-2.4.5/python_gemini_api.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      111 2024-04-24 10:47:04.000000 python_gemini_api-2.4.5/python_gemini_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-24 10:47:04.000000 python_gemini_api-2.4.5/python_gemini_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-24 10:47:04.653588 python_gemini_api-2.4.5/setup.cfg
--rw-rw-rw-   0        0        0     2184 2024-04-24 10:46:03.000000 python_gemini_api-2.4.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-24 13:05:42.695928 python_gemini_api-2.4.6/
+-rw-rw-rw-   0        0        0     1097 2024-04-24 10:59:38.000000 python_gemini_api-2.4.6/LICENSE
+-rw-rw-rw-   0        0        0    36565 2024-04-24 13:05:42.693663 python_gemini_api-2.4.6/PKG-INFO
+-rw-rw-rw-   0        0        0    35262 2024-04-24 10:16:55.000000 python_gemini_api-2.4.6/README.md
+drwxrwxrwx   0        0        0        0 2024-04-24 13:05:42.632745 python_gemini_api-2.4.6/gemini/
+-rw-rw-rw-   0        0        0     1511 2024-04-24 13:05:29.000000 python_gemini_api-2.4.6/gemini/__init__.py
+-rw-rw-rw-   0        0        0    15192 2024-03-18 04:20:24.000000 python_gemini_api-2.4.6/gemini/async_client.py
+-rw-rw-rw-   0        0        0    19096 2024-04-17 13:21:33.000000 python_gemini_api-2.4.6/gemini/client.py
+drwxrwxrwx   0        0        0        0 2024-04-24 13:05:42.634745 python_gemini_api-2.4.6/gemini/src/
+-rw-rw-rw-   0        0        0        0 2024-03-05 10:25:37.000000 python_gemini_api-2.4.6/gemini/src/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 13:05:42.638765 python_gemini_api-2.4.6/gemini/src/extensions/
+-rw-rw-rw-   0        0        0       40 2024-03-16 06:40:55.000000 python_gemini_api-2.4.6/gemini/src/extensions/__init__.py
+-rw-rw-rw-   0        0        0      622 2024-03-18 04:30:10.000000 python_gemini_api-2.4.6/gemini/src/extensions/replit.py
+drwxrwxrwx   0        0        0        0 2024-04-24 13:05:42.648091 python_gemini_api-2.4.6/gemini/src/misc/
+-rw-rw-rw-   0        0        0      265 2024-04-17 09:46:31.000000 python_gemini_api-2.4.6/gemini/src/misc/__init__.py
+-rw-rw-rw-   0        0        0     9279 2024-04-05 10:13:11.000000 python_gemini_api-2.4.6/gemini/src/misc/constants.py
+-rw-rw-rw-   0        0        0     3063 2024-03-18 04:29:01.000000 python_gemini_api-2.4.6/gemini/src/misc/decorator.py
+-rw-rw-rw-   0        0        0     2421 2024-04-20 13:54:53.000000 python_gemini_api-2.4.6/gemini/src/misc/exceptions.py
+-rw-rw-rw-   0        0        0     4487 2024-04-17 09:46:59.000000 python_gemini_api-2.4.6/gemini/src/misc/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-24 13:05:42.654773 python_gemini_api-2.4.6/gemini/src/model/
+-rw-rw-rw-   0        0        0       88 2024-03-16 06:40:55.000000 python_gemini_api-2.4.6/gemini/src/model/__init__.py
+-rw-rw-rw-   0        0        0     8611 2024-03-18 04:29:31.000000 python_gemini_api-2.4.6/gemini/src/model/image.py
+-rw-rw-rw-   0        0        0     1858 2024-03-31 11:20:09.000000 python_gemini_api-2.4.6/gemini/src/model/output.py
+drwxrwxrwx   0        0        0        0 2024-04-24 13:05:42.662227 python_gemini_api-2.4.6/gemini/src/model/parser/
+-rw-rw-rw-   0        0        0      130 2024-03-17 09:52:54.000000 python_gemini_api-2.4.6/gemini/src/model/parser/__init__.py
+-rw-rw-rw-   0        0        0     1490 2024-03-05 10:15:40.000000 python_gemini_api-2.4.6/gemini/src/model/parser/base.py
+-rw-rw-rw-   0        0        0     5433 2024-03-31 11:20:09.000000 python_gemini_api-2.4.6/gemini/src/model/parser/custom_parser.py
+-rw-rw-rw-   0        0        0     7692 2024-03-31 11:20:09.000000 python_gemini_api-2.4.6/gemini/src/model/parser/response_parser.py
+drwxrwxrwx   0        0        0        0 2024-04-24 13:05:42.664369 python_gemini_api-2.4.6/gemini/src/modules/
+-rw-rw-rw-   0        0        0        0 2024-03-29 00:25:32.000000 python_gemini_api-2.4.6/gemini/src/modules/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 13:05:42.672401 python_gemini_api-2.4.6/gemini/src/modules/openrouter/
+-rw-rw-rw-   0        0        0      102 2024-04-21 13:59:49.000000 python_gemini_api-2.4.6/gemini/src/modules/openrouter/__init__.py
+-rw-rw-rw-   0        0        0     3048 2024-04-24 12:55:46.000000 python_gemini_api-2.4.6/gemini/src/modules/openrouter/async_client.py
+-rw-rw-rw-   0        0        0     4753 2024-04-24 12:56:08.000000 python_gemini_api-2.4.6/gemini/src/modules/openrouter/client.py
+-rw-rw-rw-   0        0        0      501 2024-04-24 12:55:26.000000 python_gemini_api-2.4.6/gemini/src/modules/openrouter/const.py
+drwxrwxrwx   0        0        0        0 2024-04-24 13:05:42.677577 python_gemini_api-2.4.6/gemini/src/modules/voice/
+-rw-rw-rw-   0        0        0       88 2024-03-18 04:18:39.000000 python_gemini_api-2.4.6/gemini/src/modules/voice/__init__.py
+-rw-rw-rw-   0        0        0     2441 2024-03-18 04:18:26.000000 python_gemini_api-2.4.6/gemini/src/modules/voice/google.py
+-rw-rw-rw-   0        0        0     3144 2024-03-17 14:01:32.000000 python_gemini_api-2.4.6/gemini/src/modules/voice/openai.py
+drwxrwxrwx   0        0        0        0 2024-04-24 13:05:42.691491 python_gemini_api-2.4.6/python_gemini_api.egg-info/
+-rw-rw-rw-   0        0        0    36565 2024-04-24 13:05:42.000000 python_gemini_api-2.4.6/python_gemini_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1102 2024-04-24 13:05:42.000000 python_gemini_api-2.4.6/python_gemini_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 13:05:42.000000 python_gemini_api-2.4.6/python_gemini_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2024-04-24 13:05:42.000000 python_gemini_api-2.4.6/python_gemini_api.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      111 2024-04-24 13:05:42.000000 python_gemini_api-2.4.6/python_gemini_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-24 13:05:42.000000 python_gemini_api-2.4.6/python_gemini_api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-24 13:05:42.695928 python_gemini_api-2.4.6/setup.cfg
+-rw-rw-rw-   0        0        0     2184 2024-04-24 10:59:38.000000 python_gemini_api-2.4.6/setup.py
```

### Comparing `python_gemini_api-2.4.5/LICENSE` & `python_gemini_api-2.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `python_gemini_api-2.4.5/PKG-INFO` & `python_gemini_api-2.4.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-gemini-api
-Version: 2.4.5
+Version: 2.4.6
 Summary: The python package that returns Response of Google Gemini through API.
 Home-page: https://github.com/dsdanielpark/Gemini-API
 Author: Daniel Park
 Author-email: parkminwoo1991@gmail.com
 Keywords: Python,API,Gemini,Google Gemini,Large Language Model,Chatbot API,Google API,Chatbot
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: python-gemini-api Version: 2.4.5 Summary: The
+Metadata-Version: 2.1 Name: python-gemini-api Version: 2.4.6 Summary: The
 python package that returns Response of Google Gemini through API. Home-page:
 https://github.com/dsdanielpark/Gemini-API Author: Daniel Park Author-email:
 parkminwoo1991@gmail.com Keywords: Python,API,Gemini,Google Gemini,Large
 Language Model,Chatbot API,Google API,Chatbot Classifier: Development Status ::
 2 - Pre-Alpha Classifier: Intended Audience :: Science/Research Classifier:
 Natural Language :: English Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
```

### Comparing `python_gemini_api-2.4.5/README.md` & `python_gemini_api-2.4.6/README.md`

 * *Files identical despite different names*

### Comparing `python_gemini_api-2.4.5/gemini/__init__.py` & `python_gemini_api-2.4.6/gemini/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from os import environ
 
 from .client import Gemini
 from .async_client import GeminiClient
 from .src.modules.openrouter.client import OpenRouter
+from .src.modules.openrouter.async_client import AsyncOpenRouter
 
 from .src.model.image import GeminiImage
 from .src.model.output import GeminiCandidate, GeminiModelOutput
 from .src.model.parser.base import BaesParser
 from .src.model.parser.custom_parser import ParseMethod1, ParseMethod2
 from .src.model.parser.response_parser import ResponseParser
 
@@ -27,14 +28,14 @@
     from .src.modules.voice.google import google_tts, google_stt
     from .src.modules.voice.openai import openai_tts, openai_stt
 except ImportError as e:
     pass
 
 gemini_api_key = environ.get("GEMINI_COOKIES")
 
-__version__ = "2.4.5"
+__version__ = "2.4.6"
 __author__ = (
     "daniel park <parkminwoo1991@gmail.com>, antonio cheang <teapotv8@proton.me>, "
     "HanaokaYuzu, CBoYXD, veonua, thewh1teagle, jjkoh95, yihong0618, nishantchauhan949, MeemeeLab, kota113, "
     "sachnun, amit9021, zeelsheladiya, ayansengupta17, thecodekitchen, SalimLouDev, Qewertyy, "
     "senseibence, mirusu400, szv99, sudoAlireza"
 )
```

### Comparing `python_gemini_api-2.4.5/gemini/async_client.py` & `python_gemini_api-2.4.6/gemini/async_client.py`

 * *Files identical despite different names*

### Comparing `python_gemini_api-2.4.5/gemini/client.py` & `python_gemini_api-2.4.6/gemini/client.py`

 * *Files identical despite different names*

### Comparing `python_gemini_api-2.4.5/gemini/src/extensions/replit.py` & `python_gemini_api-2.4.6/gemini/src/extensions/replit.py`

 * *Files identical despite different names*

### Comparing `python_gemini_api-2.4.5/gemini/src/misc/constants.py` & `python_gemini_api-2.4.6/gemini/src/misc/constants.py`

 * *Files identical despite different names*

### Comparing `python_gemini_api-2.4.5/gemini/src/misc/decorator.py` & `python_gemini_api-2.4.6/gemini/src/misc/decorator.py`

 * *Files identical despite different names*

### Comparing `python_gemini_api-2.4.5/gemini/src/misc/exceptions.py` & `python_gemini_api-2.4.6/gemini/src/misc/exceptions.py`

 * *Files identical despite different names*

### Comparing `python_gemini_api-2.4.5/gemini/src/misc/utils.py` & `python_gemini_api-2.4.6/gemini/src/misc/utils.py`

 * *Files identical despite different names*

### Comparing `python_gemini_api-2.4.5/gemini/src/model/image.py` & `python_gemini_api-2.4.6/gemini/src/model/image.py`

 * *Files identical despite different names*

### Comparing `python_gemini_api-2.4.5/gemini/src/model/output.py` & `python_gemini_api-2.4.6/gemini/src/model/output.py`

 * *Files identical despite different names*

### Comparing `python_gemini_api-2.4.5/gemini/src/model/parser/base.py` & `python_gemini_api-2.4.6/gemini/src/model/parser/base.py`

 * *Files identical despite different names*

### Comparing `python_gemini_api-2.4.5/gemini/src/model/parser/custom_parser.py` & `python_gemini_api-2.4.6/gemini/src/model/parser/custom_parser.py`

 * *Files identical despite different names*

### Comparing `python_gemini_api-2.4.5/gemini/src/model/parser/response_parser.py` & `python_gemini_api-2.4.6/gemini/src/model/parser/response_parser.py`

 * *Files identical despite different names*

### Comparing `python_gemini_api-2.4.5/gemini/src/modules/openrouter/async_client.py` & `python_gemini_api-2.4.6/gemini/src/modules/openrouter/async_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import aiohttp
 import asyncio
-from const import FreeModel
+from .const import FREE_MODELS
 from typing import List, Optional
 
 
 class AsyncOpenRouter:
     """
     Manages API interactions with OpenRouter for creating chat completions using AI models asynchronously.
 
@@ -83,11 +83,11 @@
         if not isinstance(message, str):
             raise ValueError("Message must be a string")
 
     def _validate_model(self, model: str) -> None:
         """
         Checks if the specified model is in the list of free models.
         """
-        if model not in FreeModel:
+        if model not in FREE_MODELS:
             print(
                 "This model may not be free. Please check the following list for costs.\nUsers are responsible for API costs. Visit https://openrouter.ai/docs#models"
             )
```

### Comparing `python_gemini_api-2.4.5/gemini/src/modules/openrouter/client.py` & `python_gemini_api-2.4.6/gemini/src/modules/openrouter/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import requests
-from const import FreeModel
+from .const import FREE_MODELS
 from typing import List, Optional
 from requests.models import Response
 
 
 class OpenRouter:
     """
     Manages API interactions with OpenRouter for creating chat completions using AI models.
@@ -118,11 +118,11 @@
         if not isinstance(message, str):
             raise ValueError("Message must be a string")
 
     def _validate_model(self, model: str) -> None:
         """
         Checks if the specified model is in the list of free models.
         """
-        if model not in FreeModel:
+        if model not in FREE_MODELS:
             print(
                 "This model may not be free. Please check the following list for costs.\nUsers are responsible for API costs. Visit https://openrouter.ai/docs#models"
             )
```

### Comparing `python_gemini_api-2.4.5/gemini/src/modules/voice/google.py` & `python_gemini_api-2.4.6/gemini/src/modules/voice/google.py`

 * *Files identical despite different names*

### Comparing `python_gemini_api-2.4.5/gemini/src/modules/voice/openai.py` & `python_gemini_api-2.4.6/gemini/src/modules/voice/openai.py`

 * *Files identical despite different names*

### Comparing `python_gemini_api-2.4.5/python_gemini_api.egg-info/PKG-INFO` & `python_gemini_api-2.4.6/python_gemini_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-gemini-api
-Version: 2.4.5
+Version: 2.4.6
 Summary: The python package that returns Response of Google Gemini through API.
 Home-page: https://github.com/dsdanielpark/Gemini-API
 Author: Daniel Park
 Author-email: parkminwoo1991@gmail.com
 Keywords: Python,API,Gemini,Google Gemini,Large Language Model,Chatbot API,Google API,Chatbot
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: python-gemini-api Version: 2.4.5 Summary: The
+Metadata-Version: 2.1 Name: python-gemini-api Version: 2.4.6 Summary: The
 python package that returns Response of Google Gemini through API. Home-page:
 https://github.com/dsdanielpark/Gemini-API Author: Daniel Park Author-email:
 parkminwoo1991@gmail.com Keywords: Python,API,Gemini,Google Gemini,Large
 Language Model,Chatbot API,Google API,Chatbot Classifier: Development Status ::
 2 - Pre-Alpha Classifier: Intended Audience :: Science/Research Classifier:
 Natural Language :: English Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
```

### Comparing `python_gemini_api-2.4.5/python_gemini_api.egg-info/SOURCES.txt` & `python_gemini_api-2.4.6/python_gemini_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python_gemini_api-2.4.5/setup.py` & `python_gemini_api-2.4.6/setup.py`

 * *Files identical despite different names*


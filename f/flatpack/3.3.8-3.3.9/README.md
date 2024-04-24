# Comparing `tmp/flatpack-3.3.8.tar.gz` & `tmp/flatpack-3.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flatpack-3.3.8.tar", last modified: Sat Apr 20 00:40:07 2024, max compression
+gzip compressed data, was "flatpack-3.3.9.tar", last modified: Sat Apr 20 00:47:10 2024, max compression
```

## Comparing `flatpack-3.3.8.tar` & `flatpack-3.3.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-04-20 00:40:07.094478 flatpack-3.3.8/
--rw-r--r--   0 romlingroup   (501) staff       (20)    11357 2024-01-31 06:56:56.000000 flatpack-3.3.8/LICENSE
--rw-r--r--   0 romlingroup   (501) staff       (20)     6036 2024-04-20 00:40:07.094180 flatpack-3.3.8/PKG-INFO
--rw-r--r--   0 romlingroup   (501) staff       (20)     5347 2024-04-20 00:39:23.000000 flatpack-3.3.8/README.md
-drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-04-20 00:40:07.091514 flatpack-3.3.8/flatpack/
--rw-r--r--   0 romlingroup   (501) staff       (20)      132 2024-01-31 06:56:56.000000 flatpack-3.3.8/flatpack/__init__.py
--rw-r--r--   0 romlingroup   (501) staff       (20)      407 2024-01-31 06:56:56.000000 flatpack-3.3.8/flatpack/config.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     1029 2024-01-31 06:56:56.000000 flatpack-3.3.8/flatpack/datasets.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     1057 2024-01-31 06:56:56.000000 flatpack-3.3.8/flatpack/instructions.py
--rw-r--r--   0 romlingroup   (501) staff       (20)    26884 2024-04-19 23:45:08.000000 flatpack-3.3.8/flatpack/main.py
--rw-r--r--   0 romlingroup   (501) staff       (20)       59 2024-01-31 06:56:56.000000 flatpack-3.3.8/flatpack/models.py
-drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-04-20 00:40:07.093509 flatpack-3.3.8/flatpack/modules/
--rw-r--r--   0 romlingroup   (501) staff       (20)        0 2024-01-31 06:56:56.000000 flatpack-3.3.8/flatpack/modules/__init__.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     4297 2024-01-31 06:56:56.000000 flatpack-3.3.8/flatpack/modules/lstm.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     4292 2024-01-31 06:56:56.000000 flatpack-3.3.8/flatpack/modules/rnn.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     6972 2024-04-06 18:22:51.000000 flatpack-3.3.8/flatpack/parsers.py
--rw-r--r--   0 romlingroup   (501) staff       (20)      184 2024-01-31 06:56:56.000000 flatpack-3.3.8/flatpack/utils.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     6394 2024-04-19 23:44:50.000000 flatpack-3.3.8/flatpack/vector_manager.py
-drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-04-20 00:40:07.093855 flatpack-3.3.8/flatpack.egg-info/
--rw-r--r--   0 romlingroup   (501) staff       (20)     6036 2024-04-20 00:40:07.000000 flatpack-3.3.8/flatpack.egg-info/PKG-INFO
--rw-r--r--   0 romlingroup   (501) staff       (20)      485 2024-04-20 00:40:07.000000 flatpack-3.3.8/flatpack.egg-info/SOURCES.txt
--rw-r--r--   0 romlingroup   (501) staff       (20)        1 2024-04-20 00:40:07.000000 flatpack-3.3.8/flatpack.egg-info/dependency_links.txt
--rw-r--r--   0 romlingroup   (501) staff       (20)       48 2024-04-20 00:40:07.000000 flatpack-3.3.8/flatpack.egg-info/entry_points.txt
--rw-r--r--   0 romlingroup   (501) staff       (20)      232 2024-04-20 00:40:07.000000 flatpack-3.3.8/flatpack.egg-info/requires.txt
--rw-r--r--   0 romlingroup   (501) staff       (20)        9 2024-04-20 00:40:07.000000 flatpack-3.3.8/flatpack.egg-info/top_level.txt
--rw-r--r--   0 romlingroup   (501) staff       (20)       38 2024-04-20 00:40:07.094536 flatpack-3.3.8/setup.cfg
--rw-r--r--   0 romlingroup   (501) staff       (20)      964 2024-04-20 00:38:10.000000 flatpack-3.3.8/setup.py
+drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-04-20 00:47:10.898185 flatpack-3.3.9/
+-rw-r--r--   0 romlingroup   (501) staff       (20)    11357 2024-01-31 06:56:56.000000 flatpack-3.3.9/LICENSE
+-rw-r--r--   0 romlingroup   (501) staff       (20)     6336 2024-04-20 00:47:10.897865 flatpack-3.3.9/PKG-INFO
+-rw-r--r--   0 romlingroup   (501) staff       (20)     5647 2024-04-20 00:46:44.000000 flatpack-3.3.9/README.md
+drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-04-20 00:47:10.895350 flatpack-3.3.9/flatpack/
+-rw-r--r--   0 romlingroup   (501) staff       (20)      132 2024-01-31 06:56:56.000000 flatpack-3.3.9/flatpack/__init__.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)      407 2024-01-31 06:56:56.000000 flatpack-3.3.9/flatpack/config.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     1029 2024-01-31 06:56:56.000000 flatpack-3.3.9/flatpack/datasets.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     1057 2024-01-31 06:56:56.000000 flatpack-3.3.9/flatpack/instructions.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)    26884 2024-04-19 23:45:08.000000 flatpack-3.3.9/flatpack/main.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)       59 2024-01-31 06:56:56.000000 flatpack-3.3.9/flatpack/models.py
+drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-04-20 00:47:10.897190 flatpack-3.3.9/flatpack/modules/
+-rw-r--r--   0 romlingroup   (501) staff       (20)        0 2024-01-31 06:56:56.000000 flatpack-3.3.9/flatpack/modules/__init__.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     4297 2024-01-31 06:56:56.000000 flatpack-3.3.9/flatpack/modules/lstm.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     4292 2024-01-31 06:56:56.000000 flatpack-3.3.9/flatpack/modules/rnn.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     6972 2024-04-06 18:22:51.000000 flatpack-3.3.9/flatpack/parsers.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)      184 2024-01-31 06:56:56.000000 flatpack-3.3.9/flatpack/utils.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     6394 2024-04-19 23:44:50.000000 flatpack-3.3.9/flatpack/vector_manager.py
+drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-04-20 00:47:10.897511 flatpack-3.3.9/flatpack.egg-info/
+-rw-r--r--   0 romlingroup   (501) staff       (20)     6336 2024-04-20 00:47:10.000000 flatpack-3.3.9/flatpack.egg-info/PKG-INFO
+-rw-r--r--   0 romlingroup   (501) staff       (20)      485 2024-04-20 00:47:10.000000 flatpack-3.3.9/flatpack.egg-info/SOURCES.txt
+-rw-r--r--   0 romlingroup   (501) staff       (20)        1 2024-04-20 00:47:10.000000 flatpack-3.3.9/flatpack.egg-info/dependency_links.txt
+-rw-r--r--   0 romlingroup   (501) staff       (20)       48 2024-04-20 00:47:10.000000 flatpack-3.3.9/flatpack.egg-info/entry_points.txt
+-rw-r--r--   0 romlingroup   (501) staff       (20)      232 2024-04-20 00:47:10.000000 flatpack-3.3.9/flatpack.egg-info/requires.txt
+-rw-r--r--   0 romlingroup   (501) staff       (20)        9 2024-04-20 00:47:10.000000 flatpack-3.3.9/flatpack.egg-info/top_level.txt
+-rw-r--r--   0 romlingroup   (501) staff       (20)       38 2024-04-20 00:47:10.898251 flatpack-3.3.9/setup.cfg
+-rw-r--r--   0 romlingroup   (501) staff       (20)      964 2024-04-20 00:47:04.000000 flatpack-3.3.9/setup.py
```

### Comparing `flatpack-3.3.8/LICENSE` & `flatpack-3.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `flatpack-3.3.8/PKG-INFO` & `flatpack-3.3.9/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flatpack
-Version: 3.3.8
+Version: 3.3.9
 Summary: Ready-to-assemble AI
 Author: Romlin Group AB
 Author-email: hello@romlin.com
 License: Apache Software License (Apache-2.0)
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: beautifulsoup4==4.12.3
@@ -78,47 +78,49 @@
 BSD-3-Clause (INBOUND) is compatible with Apache-2.0 (OUTBOUND) for combined works but does not allow re-licensing of the original BSD-licensed component when distributed separately ([JLA 2023](https://joinup.ec.europa.eu/licence/compatibility-check/BSD-3-Clause/Apache-2.0)).
 
 MIT (INBOUND) is compatible with Apache-2.0 (OUTBOUND) for combined works but does not allow re-licensing of the original MIT-licensed component when distributed separately ([JLA 2023](https://joinup.ec.europa.eu/licence/compatibility-check/MIT/Apache-2.0)).
 
 *Check out the [JLA - Compatibility Checker](https://joinup.ec.europa.eu/collection/eupl/solution/joinup-licensing-assistant/jla-compatibility-checker) (European Commission 2023).*
 
 - **[beautifulsoup4](https://pypi.org/project/beautifulsoup4/)**\
-  MIT ([LICENSE](https://pypi.org/project/beautifulsoup4/))
+  MIT License (MIT License) ([LICENSE](https://pypi.org/project/beautifulsoup4/))
 
 - **[cryptography](https://pypi.org/project/cryptography/)**\
-  Apache-2.0 OR BSD-3-Clause ([LICENSE](https://github.com/pyca/cryptography/blob/main/LICENSE.APACHE))
+  Apache Software License, BSD License (Apache-2.0 OR BSD-3-Clause) ([LICENSE](https://github.com/pyca/cryptography/blob/main/LICENSE.APACHE))
 
 - **[faiss-cpu](https://pypi.org/project/faiss-cpu/)**\
-  MIT ([LICENSE](https://github.com/kyamagu/faiss-wheels/blob/main/LICENSE))
+  MIT License (MIT License) ([LICENSE](https://github.com/kyamagu/faiss-wheels/blob/main/LICENSE))
 
 - **[fastapi](https://pypi.org/project/fastapi/)**\
-  MIT ([LICENSE](https://github.com/tiangolo/fastapi/blob/master/LICENSE))
+  MIT License ([LICENSE](https://github.com/tiangolo/fastapi/blob/master/LICENSE))
 
 - **[httpx](https://pypi.org/project/httpx/)**\
-  BSD ([LICENSE](https://github.com/encode/httpx/blob/master/LICENSE.md))
+  BSD License ([LICENSE](https://github.com/encode/httpx/blob/master/LICENSE.md))
 
 - **[ngrok](https://pypi.org/project/ngrok/)**\
-  Apache-2.0 OR MIT ([LICENSE](https://github.com/ngrok/ngrok-python/blob/main/LICENSE-APACHE))
+  MIT License (MIT OR Apache-2.0) ([LICENSE](https://github.com/ngrok/ngrok-python/blob/main/LICENSE-APACHE))
 
 - **[nltk](https://pypi.org/project/nltk/)**\
-  Apache-2.0 ([LICENSE](https://github.com/nltk/nltk/blob/develop/LICENSE.txt))
+  Apache Software License (Apache License, Version 2.0) ([LICENSE](https://github.com/nltk/nltk/blob/develop/LICENSE.txt))
 
 - **[olefile](https://pypi.org/project/olefile/)**\
-  BSD ([LICENSE](https://github.com/decalage2/olefile/blob/master/LICENSE.txt))
+  BSD License (BSD) ([LICENSE](https://github.com/decalage2/olefile/blob/master/LICENSE.txt))
 
 - **[pypdf](https://pypi.org/project/pypdf/)**\
-  BSD ([LICENSE](https://github.com/py-pdf/pypdf/blob/main/LICENSE))
+  BSD License ([LICENSE](https://github.com/py-pdf/pypdf/blob/main/LICENSE))
 
 - **[requests](https://pypi.org/project/requests/)**\
-  Apache-2.0 ([LICENSE](https://github.com/psf/requests/blob/main/LICENSE))
+  Apache Software License (Apache 2.0) ([LICENSE](https://github.com/psf/requests/blob/main/LICENSE))
 
 - **[sentence-transformers](https://pypi.org/project/sentence-transformers/)**\
-  Apache-2.0 ([LICENSE](https://github.com/UKPLab/sentence-transformers/blob/master/LICENSE))
+  Apache Software License (Apache License 2.0) ([LICENSE](https://github.com/UKPLab/sentence-transformers/blob/master/LICENSE))
 
 - **[toml](https://pypi.org/project/toml/)**\
-  MIT ([LICENSE](https://github.com/uiri/toml/blob/master/LICENSE))
+  MIT License (MIT) ([LICENSE](https://github.com/uiri/toml/blob/master/LICENSE))
 
 - **[torch](https://pypi.org/project/torch/)**\
-  BSD-3 ([LICENSE](https://github.com/pytorch/pytorch/blob/main/LICENSE))
+  BSD License (BSD-3) ([LICENSE](https://github.com/pytorch/pytorch/blob/main/LICENSE))
 
 - **[uvicorn](https://pypi.org/project/uvicorn/)**\
-  BSD ([LICENSE](https://github.com/encode/uvicorn/blob/master/LICENSE.md))
+  BSD License ([LICENSE](https://github.com/encode/uvicorn/blob/master/LICENSE.md))
+
+Last updated: 2024-04-20
```

### Comparing `flatpack-3.3.8/README.md` & `flatpack-3.3.9/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -54,47 +54,49 @@
 BSD-3-Clause (INBOUND) is compatible with Apache-2.0 (OUTBOUND) for combined works but does not allow re-licensing of the original BSD-licensed component when distributed separately ([JLA 2023](https://joinup.ec.europa.eu/licence/compatibility-check/BSD-3-Clause/Apache-2.0)).
 
 MIT (INBOUND) is compatible with Apache-2.0 (OUTBOUND) for combined works but does not allow re-licensing of the original MIT-licensed component when distributed separately ([JLA 2023](https://joinup.ec.europa.eu/licence/compatibility-check/MIT/Apache-2.0)).
 
 *Check out the [JLA - Compatibility Checker](https://joinup.ec.europa.eu/collection/eupl/solution/joinup-licensing-assistant/jla-compatibility-checker) (European Commission 2023).*
 
 - **[beautifulsoup4](https://pypi.org/project/beautifulsoup4/)**\
-  MIT ([LICENSE](https://pypi.org/project/beautifulsoup4/))
+  MIT License (MIT License) ([LICENSE](https://pypi.org/project/beautifulsoup4/))
 
 - **[cryptography](https://pypi.org/project/cryptography/)**\
-  Apache-2.0 OR BSD-3-Clause ([LICENSE](https://github.com/pyca/cryptography/blob/main/LICENSE.APACHE))
+  Apache Software License, BSD License (Apache-2.0 OR BSD-3-Clause) ([LICENSE](https://github.com/pyca/cryptography/blob/main/LICENSE.APACHE))
 
 - **[faiss-cpu](https://pypi.org/project/faiss-cpu/)**\
-  MIT ([LICENSE](https://github.com/kyamagu/faiss-wheels/blob/main/LICENSE))
+  MIT License (MIT License) ([LICENSE](https://github.com/kyamagu/faiss-wheels/blob/main/LICENSE))
 
 - **[fastapi](https://pypi.org/project/fastapi/)**\
-  MIT ([LICENSE](https://github.com/tiangolo/fastapi/blob/master/LICENSE))
+  MIT License ([LICENSE](https://github.com/tiangolo/fastapi/blob/master/LICENSE))
 
 - **[httpx](https://pypi.org/project/httpx/)**\
-  BSD ([LICENSE](https://github.com/encode/httpx/blob/master/LICENSE.md))
+  BSD License ([LICENSE](https://github.com/encode/httpx/blob/master/LICENSE.md))
 
 - **[ngrok](https://pypi.org/project/ngrok/)**\
-  Apache-2.0 OR MIT ([LICENSE](https://github.com/ngrok/ngrok-python/blob/main/LICENSE-APACHE))
+  MIT License (MIT OR Apache-2.0) ([LICENSE](https://github.com/ngrok/ngrok-python/blob/main/LICENSE-APACHE))
 
 - **[nltk](https://pypi.org/project/nltk/)**\
-  Apache-2.0 ([LICENSE](https://github.com/nltk/nltk/blob/develop/LICENSE.txt))
+  Apache Software License (Apache License, Version 2.0) ([LICENSE](https://github.com/nltk/nltk/blob/develop/LICENSE.txt))
 
 - **[olefile](https://pypi.org/project/olefile/)**\
-  BSD ([LICENSE](https://github.com/decalage2/olefile/blob/master/LICENSE.txt))
+  BSD License (BSD) ([LICENSE](https://github.com/decalage2/olefile/blob/master/LICENSE.txt))
 
 - **[pypdf](https://pypi.org/project/pypdf/)**\
-  BSD ([LICENSE](https://github.com/py-pdf/pypdf/blob/main/LICENSE))
+  BSD License ([LICENSE](https://github.com/py-pdf/pypdf/blob/main/LICENSE))
 
 - **[requests](https://pypi.org/project/requests/)**\
-  Apache-2.0 ([LICENSE](https://github.com/psf/requests/blob/main/LICENSE))
+  Apache Software License (Apache 2.0) ([LICENSE](https://github.com/psf/requests/blob/main/LICENSE))
 
 - **[sentence-transformers](https://pypi.org/project/sentence-transformers/)**\
-  Apache-2.0 ([LICENSE](https://github.com/UKPLab/sentence-transformers/blob/master/LICENSE))
+  Apache Software License (Apache License 2.0) ([LICENSE](https://github.com/UKPLab/sentence-transformers/blob/master/LICENSE))
 
 - **[toml](https://pypi.org/project/toml/)**\
-  MIT ([LICENSE](https://github.com/uiri/toml/blob/master/LICENSE))
+  MIT License (MIT) ([LICENSE](https://github.com/uiri/toml/blob/master/LICENSE))
 
 - **[torch](https://pypi.org/project/torch/)**\
-  BSD-3 ([LICENSE](https://github.com/pytorch/pytorch/blob/main/LICENSE))
+  BSD License (BSD-3) ([LICENSE](https://github.com/pytorch/pytorch/blob/main/LICENSE))
 
 - **[uvicorn](https://pypi.org/project/uvicorn/)**\
-  BSD ([LICENSE](https://github.com/encode/uvicorn/blob/master/LICENSE.md))
+  BSD License ([LICENSE](https://github.com/encode/uvicorn/blob/master/LICENSE.md))
+
+Last updated: 2024-04-20
```

### Comparing `flatpack-3.3.8/flatpack/datasets.py` & `flatpack-3.3.9/flatpack/datasets.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.3.8/flatpack/instructions.py` & `flatpack-3.3.9/flatpack/instructions.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.3.8/flatpack/main.py` & `flatpack-3.3.9/flatpack/main.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.3.8/flatpack/modules/lstm.py` & `flatpack-3.3.9/flatpack/modules/lstm.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.3.8/flatpack/modules/rnn.py` & `flatpack-3.3.9/flatpack/modules/rnn.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.3.8/flatpack/parsers.py` & `flatpack-3.3.9/flatpack/parsers.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.3.8/flatpack/vector_manager.py` & `flatpack-3.3.9/flatpack/vector_manager.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.3.8/flatpack.egg-info/PKG-INFO` & `flatpack-3.3.9/flatpack.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flatpack
-Version: 3.3.8
+Version: 3.3.9
 Summary: Ready-to-assemble AI
 Author: Romlin Group AB
 Author-email: hello@romlin.com
 License: Apache Software License (Apache-2.0)
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: beautifulsoup4==4.12.3
@@ -78,47 +78,49 @@
 BSD-3-Clause (INBOUND) is compatible with Apache-2.0 (OUTBOUND) for combined works but does not allow re-licensing of the original BSD-licensed component when distributed separately ([JLA 2023](https://joinup.ec.europa.eu/licence/compatibility-check/BSD-3-Clause/Apache-2.0)).
 
 MIT (INBOUND) is compatible with Apache-2.0 (OUTBOUND) for combined works but does not allow re-licensing of the original MIT-licensed component when distributed separately ([JLA 2023](https://joinup.ec.europa.eu/licence/compatibility-check/MIT/Apache-2.0)).
 
 *Check out the [JLA - Compatibility Checker](https://joinup.ec.europa.eu/collection/eupl/solution/joinup-licensing-assistant/jla-compatibility-checker) (European Commission 2023).*
 
 - **[beautifulsoup4](https://pypi.org/project/beautifulsoup4/)**\
-  MIT ([LICENSE](https://pypi.org/project/beautifulsoup4/))
+  MIT License (MIT License) ([LICENSE](https://pypi.org/project/beautifulsoup4/))
 
 - **[cryptography](https://pypi.org/project/cryptography/)**\
-  Apache-2.0 OR BSD-3-Clause ([LICENSE](https://github.com/pyca/cryptography/blob/main/LICENSE.APACHE))
+  Apache Software License, BSD License (Apache-2.0 OR BSD-3-Clause) ([LICENSE](https://github.com/pyca/cryptography/blob/main/LICENSE.APACHE))
 
 - **[faiss-cpu](https://pypi.org/project/faiss-cpu/)**\
-  MIT ([LICENSE](https://github.com/kyamagu/faiss-wheels/blob/main/LICENSE))
+  MIT License (MIT License) ([LICENSE](https://github.com/kyamagu/faiss-wheels/blob/main/LICENSE))
 
 - **[fastapi](https://pypi.org/project/fastapi/)**\
-  MIT ([LICENSE](https://github.com/tiangolo/fastapi/blob/master/LICENSE))
+  MIT License ([LICENSE](https://github.com/tiangolo/fastapi/blob/master/LICENSE))
 
 - **[httpx](https://pypi.org/project/httpx/)**\
-  BSD ([LICENSE](https://github.com/encode/httpx/blob/master/LICENSE.md))
+  BSD License ([LICENSE](https://github.com/encode/httpx/blob/master/LICENSE.md))
 
 - **[ngrok](https://pypi.org/project/ngrok/)**\
-  Apache-2.0 OR MIT ([LICENSE](https://github.com/ngrok/ngrok-python/blob/main/LICENSE-APACHE))
+  MIT License (MIT OR Apache-2.0) ([LICENSE](https://github.com/ngrok/ngrok-python/blob/main/LICENSE-APACHE))
 
 - **[nltk](https://pypi.org/project/nltk/)**\
-  Apache-2.0 ([LICENSE](https://github.com/nltk/nltk/blob/develop/LICENSE.txt))
+  Apache Software License (Apache License, Version 2.0) ([LICENSE](https://github.com/nltk/nltk/blob/develop/LICENSE.txt))
 
 - **[olefile](https://pypi.org/project/olefile/)**\
-  BSD ([LICENSE](https://github.com/decalage2/olefile/blob/master/LICENSE.txt))
+  BSD License (BSD) ([LICENSE](https://github.com/decalage2/olefile/blob/master/LICENSE.txt))
 
 - **[pypdf](https://pypi.org/project/pypdf/)**\
-  BSD ([LICENSE](https://github.com/py-pdf/pypdf/blob/main/LICENSE))
+  BSD License ([LICENSE](https://github.com/py-pdf/pypdf/blob/main/LICENSE))
 
 - **[requests](https://pypi.org/project/requests/)**\
-  Apache-2.0 ([LICENSE](https://github.com/psf/requests/blob/main/LICENSE))
+  Apache Software License (Apache 2.0) ([LICENSE](https://github.com/psf/requests/blob/main/LICENSE))
 
 - **[sentence-transformers](https://pypi.org/project/sentence-transformers/)**\
-  Apache-2.0 ([LICENSE](https://github.com/UKPLab/sentence-transformers/blob/master/LICENSE))
+  Apache Software License (Apache License 2.0) ([LICENSE](https://github.com/UKPLab/sentence-transformers/blob/master/LICENSE))
 
 - **[toml](https://pypi.org/project/toml/)**\
-  MIT ([LICENSE](https://github.com/uiri/toml/blob/master/LICENSE))
+  MIT License (MIT) ([LICENSE](https://github.com/uiri/toml/blob/master/LICENSE))
 
 - **[torch](https://pypi.org/project/torch/)**\
-  BSD-3 ([LICENSE](https://github.com/pytorch/pytorch/blob/main/LICENSE))
+  BSD License (BSD-3) ([LICENSE](https://github.com/pytorch/pytorch/blob/main/LICENSE))
 
 - **[uvicorn](https://pypi.org/project/uvicorn/)**\
-  BSD ([LICENSE](https://github.com/encode/uvicorn/blob/master/LICENSE.md))
+  BSD License ([LICENSE](https://github.com/encode/uvicorn/blob/master/LICENSE.md))
+
+Last updated: 2024-04-20
```

### Comparing `flatpack-3.3.8/setup.py` & `flatpack-3.3.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="flatpack",
-    version="3.3.8",
+    version="3.3.9",
     license="Apache Software License (Apache-2.0)",
     packages=find_packages(),
     install_requires=[
         "beautifulsoup4==4.12.3",
         "cryptography==42.0.5",
         "faiss-cpu==1.8.0",
         "fastapi==0.110.1",
```


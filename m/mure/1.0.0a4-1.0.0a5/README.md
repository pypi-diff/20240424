# Comparing `tmp/mure-1.0.0a4.tar.gz` & `tmp/mure-1.0.0a5.tar.gz`

## Comparing `mure-1.0.0a4.tar` & `mure-1.0.0a5.tar`

### file list

```diff
@@ -1,16 +1,18 @@
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 mure-1.0.0a4/.pre-commit-config.yaml
--rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 mure-1.0.0a4/requirements-dev.lock
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 mure-1.0.0a4/requirements.lock
--rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 mure-1.0.0a4/.github/workflows/main.yml
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 mure-1.0.0a4/examples/example.py
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 mure-1.0.0a4/mure/__init__.py
--rw-r--r--   0        0        0     5850 2020-02-02 00:00:00.000000 mure-1.0.0a4/mure/core.py
--rw-r--r--   0        0        0     3853 2020-02-02 00:00:00.000000 mure-1.0.0a4/mure/dtos.py
--rw-r--r--   0        0        0     8833 2020-02-02 00:00:00.000000 mure-1.0.0a4/mure/iterator.py
--rw-r--r--   0        0        0     4272 2020-02-02 00:00:00.000000 mure-1.0.0a4/mure/logging.py
--rw-r--r--   0        0        0     1964 2020-02-02 00:00:00.000000 mure-1.0.0a4/tests/test_mure.py
--rw-r--r--   0        0        0     1808 2020-02-02 00:00:00.000000 mure-1.0.0a4/.gitignore
--rw-r--r--   0        0        0    11345 2020-02-02 00:00:00.000000 mure-1.0.0a4/LICENSE
--rw-r--r--   0        0        0     6526 2020-02-02 00:00:00.000000 mure-1.0.0a4/README.md
--rw-r--r--   0        0        0     2850 2020-02-02 00:00:00.000000 mure-1.0.0a4/pyproject.toml
--rw-r--r--   0        0        0     6909 2020-02-02 00:00:00.000000 mure-1.0.0a4/PKG-INFO
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 mure-1.0.0a5/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 mure-1.0.0a5/requirements-dev.lock
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 mure-1.0.0a5/requirements.lock
+-rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 mure-1.0.0a5/.github/workflows/main.yml
+-rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 mure-1.0.0a5/.vscode/settings.json
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 mure-1.0.0a5/examples/example.py
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 mure-1.0.0a5/mure/__init__.py
+-rw-r--r--   0        0        0     3705 2020-02-02 00:00:00.000000 mure-1.0.0a5/mure/cache.py
+-rw-r--r--   0        0        0     5829 2020-02-02 00:00:00.000000 mure-1.0.0a5/mure/core.py
+-rw-r--r--   0        0        0     3881 2020-02-02 00:00:00.000000 mure-1.0.0a5/mure/dtos.py
+-rw-r--r--   0        0        0     9208 2020-02-02 00:00:00.000000 mure-1.0.0a5/mure/iterator.py
+-rw-r--r--   0        0        0     4272 2020-02-02 00:00:00.000000 mure-1.0.0a5/mure/logging.py
+-rw-r--r--   0        0        0     2313 2020-02-02 00:00:00.000000 mure-1.0.0a5/tests/test_mure.py
+-rw-r--r--   0        0        0     1809 2020-02-02 00:00:00.000000 mure-1.0.0a5/.gitignore
+-rw-r--r--   0        0        0    11345 2020-02-02 00:00:00.000000 mure-1.0.0a5/LICENSE
+-rw-r--r--   0        0        0     6540 2020-02-02 00:00:00.000000 mure-1.0.0a5/README.md
+-rw-r--r--   0        0        0     2876 2020-02-02 00:00:00.000000 mure-1.0.0a5/pyproject.toml
+-rw-r--r--   0        0        0     6892 2020-02-02 00:00:00.000000 mure-1.0.0a5/PKG-INFO
```

### Comparing `mure-1.0.0a4/requirements-dev.lock` & `mure-1.0.0a5/requirements-dev.lock`

 * *Files 4% similar despite different names*

```diff
@@ -4,51 +4,51 @@
 # last locked with the following flags:
 #   pre: false
 #   features: []
 #   all-features: false
 #   with-sources: false
 
 -e file:.
-aiohttp==3.9.3
+aiohttp==3.9.5
     # via mure
 aiosignal==1.3.1
     # via aiohttp
 attrs==23.2.0
     # via aiohttp
 cfgv==3.4.0
     # via pre-commit
 chardet==5.2.0
     # via mure
 distlib==0.3.8
     # via virtualenv
-filelock==3.13.3
+filelock==3.13.4
     # via virtualenv
 frozenlist==1.4.1
     # via aiohttp
     # via aiosignal
-identify==2.5.35
+identify==2.5.36
     # via pre-commit
-idna==3.6
+idna==3.7
     # via yarl
 iniconfig==2.0.0
     # via pytest
 multidict==6.0.5
     # via aiohttp
     # via yarl
 nodeenv==1.8.0
     # via pre-commit
 packaging==24.0
     # via pytest
-platformdirs==4.2.0
+platformdirs==4.2.1
     # via virtualenv
-pluggy==1.4.0
+pluggy==1.5.0
     # via pytest
 pre-commit==3.7.0
 pytest==8.1.1
 pyyaml==6.0.1
     # via pre-commit
-virtualenv==20.25.1
+virtualenv==20.26.0
     # via pre-commit
 yarl==1.9.4
     # via aiohttp
-setuptools==69.2.0
+setuptools==69.5.1
     # via nodeenv
```

### Comparing `mure-1.0.0a4/examples/example.py` & `mure-1.0.0a5/examples/example.py`

 * *Files identical despite different names*

### Comparing `mure-1.0.0a4/mure/dtos.py` & `mure-1.0.0a5/mure/dtos.py`

 * *Files 8% similar despite different names*

```diff
@@ -60,50 +60,50 @@
 class HistoricResponse:
     """Historic HTTP response.
 
     Attributes
     ----------
     status : int
         HTTP status code of response, e.g. 200.
-    reason : str
+    reason : str | None
         HTTP status reason of response, e.g. "OK".
     ok : bool
         Boolean representation of HTTP status code. True if status is <400; otherwise, False.
     url : str
         Response URL.
     """
 
     status: int
-    reason: str
+    reason: str | None
     ok: bool
     url: str
 
 
 @dataclass
 class Response:
     """HTTP response.
 
     Attributes
     ----------
     status : int
         HTTP status code of response, e.g. 200.
-    reason : str
+    reason : str | None
         HTTP status reason of response, e.g. "OK".
     ok : bool
         Boolean representation of HTTP status code. True if status is <400; otherwise, False.
     text : str
         Response's body as decoded string.
     url : str
         Response URL.
     history : list[HistoricResponse]
         List of historic responses (in case requested URL redirected).
     """
 
     status: int
-    reason: str
+    reason: str | None
     ok: bool
     text: str
     url: str
     history: list[HistoricResponse]
 
     def json(self) -> Any:
         """Deserialize JSON to Python objects.
```

### Comparing `mure-1.0.0a4/mure/iterator.py` & `mure-1.0.0a5/mure/iterator.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,48 +1,51 @@
 import asyncio
+import os
 from asyncio import Event, PriorityQueue, Task
 from collections.abc import AsyncGenerator, Iterator
 from typing import Self
 
 import chardet
 from aiohttp import ClientSession
 
+from mure.cache import Cache
 from mure.dtos import HistoricResponse, HTTPResource, Response
 from mure.logging import Logger
 
 LOGGER = Logger(__name__)
 
 
 class ResponseIterator(Iterator[Response]):
     """Response iterator that fetches responses concurrently."""
 
     def __init__(
         self,
         resources: list[HTTPResource],
         *,
         batch_size: int = 5,
-        log_errors: bool = True,
+        cache: Cache | None = None,
     ):
         """Initialize a response iterator.
 
         Parameters
         ----------
         resources : list[HTTPResource]
             Resources to request.
         batch_size : int, optional
             Number of resources to request concurrently, by default 5.
-        log_errors : bool, optional
-            True if Python errors should be logged, by default True.
+        cache : Cache | None, optional
+            Cache to use for storing responses, by default None.
         """
         self.resources = resources
         self.num_resources = len(resources)
         self.pending = len(resources)
         self.batch_size = batch_size
+        self.cache = cache
 
-        self._log_errors = log_errors
+        self._log_errors = bool(os.environ.get("MURE_LOG_ERRORS"))
         self._loop = asyncio.new_event_loop()
         self._queue = PriorityQueue()
         self._events = [Event() for _ in resources]
         self._tasks: set[Task] = set()
         self._responses = self._fetch_responses()
         self._generator = None
 
@@ -168,16 +171,23 @@
         resource : HTTPResource
             Resource to request.
         event : Event
             Event to set when the response is ready.
         """
         LOGGER.debug(f"Started {priority}")
 
-        # fetch response
-        response = await self._afetch(session, resource)
+        # if cache is given and has the resource, use it
+        if self.cache and self.cache.has(resource):
+            response = self.cache.get(resource)
+        else:
+            response = await self._afetch(session, resource)
+
+            # save response to cache
+            if self.cache:
+                self.cache.save(resource, response)
 
         # put response in the queue
         await self._queue.put((priority, response))
 
         # set event to notify that the response is ready
         event.set()
 
@@ -266,15 +276,15 @@
                     text = content.decode(encoding, errors="replace")
                 except (LookupError, TypeError):
                     # LookupError is raised if the encoding was not found which could
                     # indicate a misspelling or similar mistake
                     #
                     # TypeError can be raised if encoding is None
                     encoding = chardet.detect(content)["encoding"]
-                    text = content.decode(encoding, errors="replace")
+                    text = content.decode(encoding or "utf-8", errors="replace")
 
                 return Response(
                     status=response.status,
                     reason=response.reason,
                     ok=response.ok,
                     text=text,
                     url=response.url.human_repr(),
```

### Comparing `mure-1.0.0a4/mure/logging.py` & `mure-1.0.0a5/mure/logging.py`

 * *Files identical despite different names*

### Comparing `mure-1.0.0a4/tests/test_mure.py` & `mure-1.0.0a5/tests/test_mure.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from json import JSONDecodeError
 
 import pytest
 
 import mure
+from mure.cache import InMemoryCache
 from mure.dtos import HTTPResource, Resource, Response
 
 
 def test_get():
     resources: list[Resource] = [
         {"url": "https://httpbin.org/get"},
         {"url": "https://httpbin.org/get", "params": {"foo": "bar"}},
@@ -65,7 +66,20 @@
 
     assert len(response.json()) == 4
 
 
 def test_invalid_json():
     with pytest.raises(JSONDecodeError):
         next(mure.get([{"url": "https://wikipedia.org"}])).json()
+
+
+def test_cache():
+    cache = InMemoryCache()
+    resource: HTTPResource = {"method": "GET", "url": "https://httpbin.org/get"}
+
+    # resource is not in the cache
+    assert not cache.has(resource)
+
+    next(mure.get([resource], cache=cache))
+
+    # resource is now in the cache
+    assert cache.has(resource)
```

### Comparing `mure-1.0.0a4/.gitignore` & `mure-1.0.0a5/.gitignore`

 * *Files 2% similar despite different names*

```diff
@@ -124,8 +124,8 @@
 .mypy_cache/
 .dmypy.json
 dmypy.json
 
 # Pyre type checker
 .pyre/
 
-.vscode
+*.shelve
```

### Comparing `mure-1.0.0a4/LICENSE` & `mure-1.0.0a5/LICENSE`

 * *Files identical despite different names*

### Comparing `mure-1.0.0a4/README.md` & `mure-1.0.0a5/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # mure
 
 [![downloads](https://static.pepy.tech/personalized-badge/mure?period=total&units=international_system&left_color=black&right_color=black&left_text=downloads)](https://pepy.tech/project/mure)
 [![downloads/month](https://static.pepy.tech/personalized-badge/mure?period=month&units=abbreviation&left_color=black&right_color=black&left_text=downloads/month)](https://pepy.tech/project/mure)
 [![downloads/week](https://static.pepy.tech/personalized-badge/mure?period=week&units=abbreviation&left_color=black&right_color=black&left_text=downloads/week)](https://pepy.tech/project/mure)
 
-This is a thin layer on top of [`aiohttp`](https://docs.aiohttp.org/en/stable/) to perform multiple HTTP requests in parallel – without writing boilerplate code or worrying about `async` functions.
+This is a thin layer on top of [`aiohttp`](https://docs.aiohttp.org/en/stable/) to perform multiple HTTP requests concurrently – without worrying about `async` functions.
 
 `mure` means **mu**ltiple **re**quests, but is also the German term for a form of mass wasting involving fast-moving flow of debris and dirt that has become liquified by the addition of water.
 
 ![Göscheneralp. Kolorierung des Dias durch Margrit Wehrli-Frey](https://upload.wikimedia.org/wikipedia/commons/thumb/6/6b/ETH-BIB-Muhrgang_zur_Kehlen-Reuss_vom_Rotfirn-Dia_247-13368.tif/lossy-page1-1280px-ETH-BIB-Muhrgang_zur_Kehlen-Reuss_vom_Rotfirn-Dia_247-13368.tif.jpg)
 
 (The photo was taken by [Leo Wehrli](https://de.wikipedia.org/wiki/Leo_Wehrli) and is licensed under CC BY-SA 4.0)
 
@@ -41,23 +41,23 @@
 {'url': 'https://httpbin.org/get'} status code: 200
 {'url': 'https://httpbin.org/get', 'params': {'foo': 'bar'}} status code: 200
 {'url': 'invalid'} status code: 0
 >>> responses
 <ResponseIterator: 0/3 pending>
 ```
 
-The keyword argument `batch_size` defines the number of requests to perform in parallel (don't be too greedy). The resources are requested batch-wise, i. e. only one batch of responses is kept in memory (depends of course also on how you use the `ResponseIterator`). Once you start accessing the first response of a batch, the next batch of resources is requested already in the background. So while you are doing something with a batch of responses (e.g. some CPU-heavy operation like parsing HTML), the next batch is already requested in the background.
+The keyword argument `batch_size` defines the number of requests to perform concurrently (don't be too greedy). The resources are requested batch-wise, i. e. only one batch of responses is kept in memory (depends of course also on how you use the `ResponseIterator`). Once you start accessing the first response of a batch, the next batch of resources is requested already in the background. So while you are doing something with a batch of responses (e.g. some CPU-heavy operation like parsing HTML), the next batch is already requested in the background.
 
 For example, if you have four resources, set `batch_size` to `2` and execute:
 
 ```python
 >>> next(responses)
 ```
 
-the first two resources are requested in parallel and blocks until both of the responses are available (i.e. if resource 1 takes 1 second and resource 2 takes 10 seconds, it blocks 10 seconds although resource 1 is already available after 1 second). Before the response of resource 1 is yielded, the next batch of resources (i.e. 3 and 4) is already requested in the background.
+the first two resources are requested concurrently and blocks until both of the responses are available (i.e. if resource 1 takes 1 second and resource 2 takes 10 seconds, it blocks 10 seconds although resource 1 is already available after 1 second). Before the response of resource 1 is yielded, the next batch of resources (i.e. 3 and 4) is already requested in the background.
 
 Executing `next()` a second time:
 
 ```python
 >>> next(responses)
 ```
 
@@ -93,19 +93,23 @@
 
 - Set timeouts (e.g. 10 seconds) to avoid waiting for too long.
 - It might be a good idea to order the URLs to be requested by domain names so that DNS resolution is done once per domain. Once a domain's IP has been resolved, subsequent requests to the same domain can benefit from cached DNS resolutions. Also when using protocols like HTTP/1.1, connections to the same domain can be reused. Batching requests by domain can allow for connection reuse.
 - Shuffling URLs randomly might be an alternative if you do not request the same domain multiple times. This helps in distributing potential slow URLs across different batches.
 
 ### Verbosity
 
-Control verbosity with the `log_errors` argument:
+Control verbosity with the `MURE_LOG_ERRORS` environment variable:
 
 ```python
+>>> import os
 >>> import mure
->>> next(mure.get([{"url": "invalid"}], log_errors=True))
+>>> next(mure.get([{"url": "invalid"}]))
+Response(status=0, reason='<InvalidURL invalid>', ok=False, text='')
+>>> os.environ["MURE_LOG_ERRORS"] = "true"
+>>> next(mure.get([{"url": "invalid"}]))
 invalid
 Traceback (most recent call last):
   File "/home/severin/git/mure/mure/iterator.py", line 131, in _process
     async with session.request(resource["method"], resource["url"], **kwargs) as response:
   File "/home/severin/git/mure/.env/lib/python3.11/site-packages/aiohttp/client.py", line 1141, in __aenter__
     self._resp = await self._coro
                  ^^^^^^^^^^^^^^^^
@@ -114,10 +118,8 @@
           ^^^^^^^^^^^^^^^^^^^^
   File "/home/severin/git/mure/.env/lib/python3.11/site-packages/aiohttp/client_reqrep.py", line 305, in __init__
     self.update_host(url)
   File "/home/severin/git/mure/.env/lib/python3.11/site-packages/aiohttp/client_reqrep.py", line 364, in update_host
     raise InvalidURL(url)
 aiohttp.client_exceptions.InvalidURL: invalid
 Response(status=0, reason='<InvalidURL invalid>', ok=False, text='')
->>> next(mure.get([{"url": "invalid"}], log_errors=False))
-Response(status=0, reason='<InvalidURL invalid>', ok=False, text='')
 ```
```

### Comparing `mure-1.0.0a4/pyproject.toml` & `mure-1.0.0a5/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
 name = "mure"
-version = "1.0.0a4"
-description = "Perform multiple HTTP requests in parallel – without writing boilerplate code or worrying about async functions."
+version = "1.0.0a5"
+description = "Perform multiple HTTP requests concurrently – without worrying about async functions."
 authors = [{ name = "Severin Simmler", email = "s.simmler@snapaddy.com" }]
 dependencies = ["aiohttp>=3.9.3", "chardet>=5.2.0"]
 readme = "README.md"
-requires-python = ">= 3.11, <= 3.12"
+requires-python = ">= 3.11, < 4"
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [tool.rye]
 managed = true
@@ -83,11 +83,12 @@
     "RUF001", # String contains ambiguous character
     "S608",   # Possible SQL injection vector through string-based query construction
     "S110",   # Consider logging the exception before pass
     "S112",   # Consider logging the exception before continue
     "S105",   # Possible hardcoded password
     "S320",   # Using lxml to parse untrusted data
     "S311",   # Standard pseudo-random generators are not suitable for cryptographic purposes
+    "S301",   # Use of `pickle` and modules that wrap it
 ]
 
 [tool.ruff.lint.pydocstyle]
 convention = "numpy"
```

### Comparing `mure-1.0.0a4/PKG-INFO` & `mure-1.0.0a5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.3
 Name: mure
-Version: 1.0.0a4
-Summary: Perform multiple HTTP requests in parallel – without writing boilerplate code or worrying about async functions.
+Version: 1.0.0a5
+Summary: Perform multiple HTTP requests concurrently – without worrying about async functions.
 Author-email: Severin Simmler <s.simmler@snapaddy.com>
 License-File: LICENSE
-Requires-Python: <=3.12,>=3.11
+Requires-Python: <4,>=3.11
 Requires-Dist: aiohttp>=3.9.3
 Requires-Dist: chardet>=5.2.0
 Description-Content-Type: text/markdown
 
 # mure
 
 [![downloads](https://static.pepy.tech/personalized-badge/mure?period=total&units=international_system&left_color=black&right_color=black&left_text=downloads)](https://pepy.tech/project/mure)
 [![downloads/month](https://static.pepy.tech/personalized-badge/mure?period=month&units=abbreviation&left_color=black&right_color=black&left_text=downloads/month)](https://pepy.tech/project/mure)
 [![downloads/week](https://static.pepy.tech/personalized-badge/mure?period=week&units=abbreviation&left_color=black&right_color=black&left_text=downloads/week)](https://pepy.tech/project/mure)
 
-This is a thin layer on top of [`aiohttp`](https://docs.aiohttp.org/en/stable/) to perform multiple HTTP requests in parallel – without writing boilerplate code or worrying about `async` functions.
+This is a thin layer on top of [`aiohttp`](https://docs.aiohttp.org/en/stable/) to perform multiple HTTP requests concurrently – without worrying about `async` functions.
 
 `mure` means **mu**ltiple **re**quests, but is also the German term for a form of mass wasting involving fast-moving flow of debris and dirt that has become liquified by the addition of water.
 
 ![Göscheneralp. Kolorierung des Dias durch Margrit Wehrli-Frey](https://upload.wikimedia.org/wikipedia/commons/thumb/6/6b/ETH-BIB-Muhrgang_zur_Kehlen-Reuss_vom_Rotfirn-Dia_247-13368.tif/lossy-page1-1280px-ETH-BIB-Muhrgang_zur_Kehlen-Reuss_vom_Rotfirn-Dia_247-13368.tif.jpg)
 
 (The photo was taken by [Leo Wehrli](https://de.wikipedia.org/wiki/Leo_Wehrli) and is licensed under CC BY-SA 4.0)
 
@@ -52,23 +52,23 @@
 {'url': 'https://httpbin.org/get'} status code: 200
 {'url': 'https://httpbin.org/get', 'params': {'foo': 'bar'}} status code: 200
 {'url': 'invalid'} status code: 0
 >>> responses
 <ResponseIterator: 0/3 pending>
 ```
 
-The keyword argument `batch_size` defines the number of requests to perform in parallel (don't be too greedy). The resources are requested batch-wise, i. e. only one batch of responses is kept in memory (depends of course also on how you use the `ResponseIterator`). Once you start accessing the first response of a batch, the next batch of resources is requested already in the background. So while you are doing something with a batch of responses (e.g. some CPU-heavy operation like parsing HTML), the next batch is already requested in the background.
+The keyword argument `batch_size` defines the number of requests to perform concurrently (don't be too greedy). The resources are requested batch-wise, i. e. only one batch of responses is kept in memory (depends of course also on how you use the `ResponseIterator`). Once you start accessing the first response of a batch, the next batch of resources is requested already in the background. So while you are doing something with a batch of responses (e.g. some CPU-heavy operation like parsing HTML), the next batch is already requested in the background.
 
 For example, if you have four resources, set `batch_size` to `2` and execute:
 
 ```python
 >>> next(responses)
 ```
 
-the first two resources are requested in parallel and blocks until both of the responses are available (i.e. if resource 1 takes 1 second and resource 2 takes 10 seconds, it blocks 10 seconds although resource 1 is already available after 1 second). Before the response of resource 1 is yielded, the next batch of resources (i.e. 3 and 4) is already requested in the background.
+the first two resources are requested concurrently and blocks until both of the responses are available (i.e. if resource 1 takes 1 second and resource 2 takes 10 seconds, it blocks 10 seconds although resource 1 is already available after 1 second). Before the response of resource 1 is yielded, the next batch of resources (i.e. 3 and 4) is already requested in the background.
 
 Executing `next()` a second time:
 
 ```python
 >>> next(responses)
 ```
 
@@ -104,19 +104,23 @@
 
 - Set timeouts (e.g. 10 seconds) to avoid waiting for too long.
 - It might be a good idea to order the URLs to be requested by domain names so that DNS resolution is done once per domain. Once a domain's IP has been resolved, subsequent requests to the same domain can benefit from cached DNS resolutions. Also when using protocols like HTTP/1.1, connections to the same domain can be reused. Batching requests by domain can allow for connection reuse.
 - Shuffling URLs randomly might be an alternative if you do not request the same domain multiple times. This helps in distributing potential slow URLs across different batches.
 
 ### Verbosity
 
-Control verbosity with the `log_errors` argument:
+Control verbosity with the `MURE_LOG_ERRORS` environment variable:
 
 ```python
+>>> import os
 >>> import mure
->>> next(mure.get([{"url": "invalid"}], log_errors=True))
+>>> next(mure.get([{"url": "invalid"}]))
+Response(status=0, reason='<InvalidURL invalid>', ok=False, text='')
+>>> os.environ["MURE_LOG_ERRORS"] = "true"
+>>> next(mure.get([{"url": "invalid"}]))
 invalid
 Traceback (most recent call last):
   File "/home/severin/git/mure/mure/iterator.py", line 131, in _process
     async with session.request(resource["method"], resource["url"], **kwargs) as response:
   File "/home/severin/git/mure/.env/lib/python3.11/site-packages/aiohttp/client.py", line 1141, in __aenter__
     self._resp = await self._coro
                  ^^^^^^^^^^^^^^^^
@@ -125,10 +129,8 @@
           ^^^^^^^^^^^^^^^^^^^^
   File "/home/severin/git/mure/.env/lib/python3.11/site-packages/aiohttp/client_reqrep.py", line 305, in __init__
     self.update_host(url)
   File "/home/severin/git/mure/.env/lib/python3.11/site-packages/aiohttp/client_reqrep.py", line 364, in update_host
     raise InvalidURL(url)
 aiohttp.client_exceptions.InvalidURL: invalid
 Response(status=0, reason='<InvalidURL invalid>', ok=False, text='')
->>> next(mure.get([{"url": "invalid"}], log_errors=False))
-Response(status=0, reason='<InvalidURL invalid>', ok=False, text='')
 ```
```


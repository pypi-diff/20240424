# Comparing `tmp/agency-1.6.2.tar.gz` & `tmp/agency-1.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agency-1.6.2.tar", max compression
+gzip compressed data, was "agency-1.6.3.tar", max compression
```

## Comparing `agency-1.6.2.tar` & `agency-1.6.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1073 2023-12-21 20:59:07.745504 agency-1.6.2/LICENSE
--rw-r--r--   0        0        0     5778 2023-12-21 20:59:07.745504 agency-1.6.2/README.md
--rw-r--r--   0        0        0       78 2023-12-21 20:59:07.745504 agency-1.6.2/agency/__init__.py
--rw-r--r--   0        0        0    22702 2023-12-21 20:59:07.745504 agency-1.6.2/agency/agent.py
--rw-r--r--   0        0        0     2606 2023-12-21 20:59:07.745504 agency-1.6.2/agency/logger.py
--rw-r--r--   0        0        0     5294 2023-12-21 20:59:07.745504 agency-1.6.2/agency/processor.py
--rw-r--r--   0        0        0     1154 2023-12-21 20:59:07.745504 agency-1.6.2/agency/queue.py
--rw-r--r--   0        0        0      684 2023-12-21 20:59:07.749504 agency-1.6.2/agency/resources.py
--rw-r--r--   0        0        0     1257 2023-12-21 20:59:07.749504 agency-1.6.2/agency/schema.py
--rwxr-xr-x   0        0        0     6966 2023-12-21 20:59:07.749504 agency-1.6.2/agency/space.py
--rw-r--r--   0        0        0        0 2023-12-21 20:59:07.749504 agency-1.6.2/agency/spaces/__init__.py
--rw-r--r--   0        0        0     7478 2023-12-21 20:59:07.749504 agency-1.6.2/agency/spaces/amqp_space.py
--rw-r--r--   0        0        0     3253 2023-12-21 20:59:07.749504 agency-1.6.2/agency/spaces/local_space.py
--rw-r--r--   0        0        0      604 2023-12-21 20:59:08.989504 agency-1.6.2/pyproject.toml
--rw-r--r--   0        0        0     6493 1970-01-01 00:00:00.000000 agency-1.6.2/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-04-24 20:50:59.674249 agency-1.6.3/LICENSE
+-rw-r--r--   0        0        0     4844 2024-04-24 20:50:59.674249 agency-1.6.3/README.md
+-rw-r--r--   0        0        0       78 2024-04-24 20:50:59.674249 agency-1.6.3/agency/__init__.py
+-rw-r--r--   0        0        0    22702 2024-04-24 20:50:59.674249 agency-1.6.3/agency/agent.py
+-rw-r--r--   0        0        0     2606 2024-04-24 20:50:59.674249 agency-1.6.3/agency/logger.py
+-rw-r--r--   0        0        0     5294 2024-04-24 20:50:59.674249 agency-1.6.3/agency/processor.py
+-rw-r--r--   0        0        0     1154 2024-04-24 20:50:59.674249 agency-1.6.3/agency/queue.py
+-rw-r--r--   0        0        0      797 2024-04-24 20:50:59.674249 agency-1.6.3/agency/resources.py
+-rw-r--r--   0        0        0     1257 2024-04-24 20:50:59.674249 agency-1.6.3/agency/schema.py
+-rwxr-xr-x   0        0        0     6966 2024-04-24 20:50:59.674249 agency-1.6.3/agency/space.py
+-rw-r--r--   0        0        0        0 2024-04-24 20:50:59.674249 agency-1.6.3/agency/spaces/__init__.py
+-rw-r--r--   0        0        0     7478 2024-04-24 20:50:59.674249 agency-1.6.3/agency/spaces/amqp_space.py
+-rw-r--r--   0        0        0     3282 2024-04-24 20:50:59.674249 agency-1.6.3/agency/spaces/local_space.py
+-rw-r--r--   0        0        0      604 2024-04-24 20:51:00.862250 agency-1.6.3/pyproject.toml
+-rw-r--r--   0        0        0     5559 1970-01-01 00:00:00.000000 agency-1.6.3/PKG-INFO
```

### Comparing `agency-1.6.2/LICENSE` & `agency-1.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `agency-1.6.2/README.md` & `agency-1.6.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,26 @@
+Metadata-Version: 2.1
+Name: agency
+Version: 1.6.3
+Summary: A fast and minimal framework for building agent-integrated systems
+License: GPL-3.0
+Author: Daniel Rodriguez
+Requires-Python: >=3.9,<4.0
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: colorlog (>=6.7.0,<7.0.0)
+Requires-Dist: docstring-parser (>=0.15,<0.16)
+Requires-Dist: kombu (>=5.3.1,<6.0.0)
+Requires-Dist: pydantic (>=1.8)
+Requires-Dist: pygments (>=2.16.1,<3.0.0)
+Description-Content-Type: text/markdown
+
 # Summary
 
 Agency is a python library that provides an [Actor
 model](https://en.wikipedia.org/wiki/Actor_model) framework for creating
 agent-integrated systems.
 
 The library provides an easy to use API that enables you to connect agents with
@@ -148,40 +167,22 @@
 
 <p align="center">
   <img src="https://i.ibb.co/h29m5S4/Screenshot-2023-07-26-at-4-53-05-PM.png"
       alt="Screenshot-2023-07-26-at-4-53-05-PM" border="0">
 </p>
 
 
-# FAQ
-
-## How does Agency compare to other agent frameworks?
-
-Though you could entirely create a simple agent using only the primitives in
-Agency (see [`examples/demo/agents/`](./examples/demo/agents/)), it is not
-intended to be an all-inclusive LLM-oriented toolset like other libraries. For
-example, it does not include support for constructing prompts or working with
-vector databases. Implementation of agent behavior is left entirely up to you,
-and you are free to use other libraries as needed for those purposes.
-
-Agency focuses on the concerns of communication, observation,
-and scalability. The library strives to provide the operating
-foundations of an agent system without imposing additional structure on you.
-
-The goal is to allow you to experiment and discover the right approaches and
-technologies that work for your application. And once you've found an
-implementation that works, you can scale it out to your needs.
-
 
 # Contributing
 
 Please do!
 
 If you're considering a contribution, please check out the [contributing
 guide](./CONTRIBUTING.md).
 
 # Planned Work
 
 [See the issues page.](https://github.com/operand/agency/issues)
 
 If you have any suggestions or otherwise, feel free to add an issue or open a
 [discussion](https://github.com/operand/agency/discussions).
+
```

### Comparing `agency-1.6.2/agency/agent.py` & `agency-1.6.3/agency/agent.py`

 * *Files identical despite different names*

### Comparing `agency-1.6.2/agency/logger.py` & `agency-1.6.3/agency/logger.py`

 * *Files identical despite different names*

### Comparing `agency-1.6.2/agency/processor.py` & `agency-1.6.3/agency/processor.py`

 * *Files identical despite different names*

### Comparing `agency-1.6.2/agency/queue.py` & `agency-1.6.3/agency/queue.py`

 * *Files identical despite different names*

### Comparing `agency-1.6.2/agency/resources.py` & `agency-1.6.3/agency/resources.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,18 +5,19 @@
 class ResourceManager:
     """
     Singleton for globally managing concurrency primitives
     """
     _instance = None
     _initialized = False
 
-    def __new__(cls):
+    def __new__(cls, *args, **kwargs):
         if cls._instance is None:
             cls._instance = super(ResourceManager, cls).__new__(cls)
         return cls._instance
 
-    def __init__(self):
+    def __init__(self, max_workers=None):
         if not self._initialized:
-            self.thread_pool_executor = ThreadPoolExecutor()
-            self.process_pool_executor = ProcessPoolExecutor()
+            self._max_workers = max_workers
+            self.thread_pool_executor = ThreadPoolExecutor(self._max_workers)
+            self.process_pool_executor = ProcessPoolExecutor(self._max_workers)
             self.multiprocessing_manager = multiprocessing.Manager()
             self._initialized = True
```

### Comparing `agency-1.6.2/agency/schema.py` & `agency-1.6.3/agency/schema.py`

 * *Files identical despite different names*

### Comparing `agency-1.6.2/agency/space.py` & `agency-1.6.3/agency/space.py`

 * *Files identical despite different names*

### Comparing `agency-1.6.2/agency/spaces/amqp_space.py` & `agency-1.6.3/agency/spaces/amqp_space.py`

 * *Files identical despite different names*

### Comparing `agency-1.6.2/agency/spaces/local_space.py` & `agency-1.6.3/agency/spaces/local_space.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,18 +27,18 @@
 
 
 class LocalSpace(Space):
     """
     A LocalSpace allows Agents to communicate within the python application
     """
 
-    def __init__(self):
+    def __init__(self, max_workers=None):
         super().__init__()
         self._stop_router_event: threading.Event = threading.Event()
-        self._outbound_message_event: multiprocessing.Event = ResourceManager(
+        self._outbound_message_event: multiprocessing.Event = ResourceManager(max_workers
         ).multiprocessing_manager.Event()
         self._router_future: Future = self._start_router_thread()
 
     def destroy(self):
         self._stop_router_thread()
         super().destroy()
```

### Comparing `agency-1.6.2/pyproject.toml` & `agency-1.6.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "agency"
-version = "1.6.2"
+version = "1.6.3"
 description = "A fast and minimal framework for building agent-integrated systems"
 authors = ["Daniel Rodriguez"]
 license = "GPL-3.0"
 readme = "README.md"
 include = ["agency/**/*"]
 exclude = ["*"]
```

### Comparing `agency-1.6.2/PKG-INFO` & `agency-1.6.3/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,26 +1,7 @@
-Metadata-Version: 2.1
-Name: agency
-Version: 1.6.2
-Summary: A fast and minimal framework for building agent-integrated systems
-License: GPL-3.0
-Author: Daniel Rodriguez
-Requires-Python: >=3.9,<4.0
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: colorlog (>=6.7.0,<7.0.0)
-Requires-Dist: docstring-parser (>=0.15,<0.16)
-Requires-Dist: kombu (>=5.3.1,<6.0.0)
-Requires-Dist: pydantic (>=1.8)
-Requires-Dist: pygments (>=2.16.1,<3.0.0)
-Description-Content-Type: text/markdown
-
 # Summary
 
 Agency is a python library that provides an [Actor
 model](https://en.wikipedia.org/wiki/Actor_model) framework for creating
 agent-integrated systems.
 
 The library provides an easy to use API that enables you to connect agents with
@@ -167,41 +148,21 @@
 
 <p align="center">
   <img src="https://i.ibb.co/h29m5S4/Screenshot-2023-07-26-at-4-53-05-PM.png"
       alt="Screenshot-2023-07-26-at-4-53-05-PM" border="0">
 </p>
 
 
-# FAQ
-
-## How does Agency compare to other agent frameworks?
-
-Though you could entirely create a simple agent using only the primitives in
-Agency (see [`examples/demo/agents/`](./examples/demo/agents/)), it is not
-intended to be an all-inclusive LLM-oriented toolset like other libraries. For
-example, it does not include support for constructing prompts or working with
-vector databases. Implementation of agent behavior is left entirely up to you,
-and you are free to use other libraries as needed for those purposes.
-
-Agency focuses on the concerns of communication, observation,
-and scalability. The library strives to provide the operating
-foundations of an agent system without imposing additional structure on you.
-
-The goal is to allow you to experiment and discover the right approaches and
-technologies that work for your application. And once you've found an
-implementation that works, you can scale it out to your needs.
-
 
 # Contributing
 
 Please do!
 
 If you're considering a contribution, please check out the [contributing
 guide](./CONTRIBUTING.md).
 
 # Planned Work
 
 [See the issues page.](https://github.com/operand/agency/issues)
 
 If you have any suggestions or otherwise, feel free to add an issue or open a
 [discussion](https://github.com/operand/agency/discussions).
-
```


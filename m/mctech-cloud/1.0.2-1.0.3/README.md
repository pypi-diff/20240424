# Comparing `tmp/mctech_cloud-1.0.2.tar.gz` & `tmp/mctech_cloud-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mctech_cloud-1.0.2.tar", last modified: Wed Jul 19 07:47:26 2023, max compression
+gzip compressed data, was "mctech_cloud-1.0.3.tar", last modified: Wed Apr 24 08:22:06 2024, max compression
```

## Comparing `mctech_cloud-1.0.2.tar` & `mctech_cloud-1.0.3.tar`

### file list

```diff
@@ -1,18 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-19 07:47:26.341568 mctech_cloud-1.0.2/
--rw-rw-rw-   0        0        0      147 2023-07-19 07:47:26.339576 mctech_cloud-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      497 2023-07-19 07:47:00.000000 mctech_cloud-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-19 07:47:26.283381 mctech_cloud-1.0.2/mctech_cloud/
--rw-rw-rw-   0        0        0       34 2022-10-08 03:15:48.000000 mctech_cloud-1.0.2/mctech_cloud/__init__.py
--rw-rw-rw-   0        0        0     1930 2022-10-18 06:23:52.000000 mctech_cloud-1.0.2/mctech_cloud/app_server.py
--rw-rw-rw-   0        0        0      927 2022-10-08 03:15:48.000000 mctech_cloud-1.0.2/mctech_cloud/header_filter.py
-drwxrwxrwx   0        0        0        0 2023-07-19 07:47:26.336569 mctech_cloud-1.0.2/mctech_cloud/middlewares/
--rw-rw-rw-   0        0        0      674 2022-10-08 03:15:48.000000 mctech_cloud-1.0.2/mctech_cloud/middlewares/__init__.py
--rw-rw-rw-   0        0        0     1385 2022-10-08 03:15:48.000000 mctech_cloud-1.0.2/mctech_cloud/middlewares/service_context_middleware.py
-drwxrwxrwx   0        0        0        0 2023-07-19 07:47:26.327566 mctech_cloud-1.0.2/mctech_cloud.egg-info/
--rw-rw-rw-   0        0        0      147 2023-07-19 07:47:26.000000 mctech_cloud-1.0.2/mctech_cloud.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      384 2023-07-19 07:47:26.000000 mctech_cloud-1.0.2/mctech_cloud.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-19 07:47:26.000000 mctech_cloud-1.0.2/mctech_cloud.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2023-07-19 07:47:26.000000 mctech_cloud-1.0.2/mctech_cloud.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-07-19 07:47:26.000000 mctech_cloud-1.0.2/mctech_cloud.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      355 2023-07-19 07:44:17.000000 mctech_cloud-1.0.2/mctech_cloud_setup.py
--rw-rw-rw-   0        0        0       42 2023-07-19 07:47:26.341568 mctech_cloud-1.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-24 08:22:06.125250 mctech_cloud-1.0.3/
+-rw-rw-rw-   0        0        0      147 2024-04-24 08:22:06.123369 mctech_cloud-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      555 2024-04-01 06:27:50.000000 mctech_cloud-1.0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-24 08:22:06.094247 mctech_cloud-1.0.3/mctech_cloud/
+-rw-rw-rw-   0        0        0       59 2024-04-24 04:22:58.000000 mctech_cloud-1.0.3/mctech_cloud/__init__.py
+-rw-rw-rw-   0        0        0     1663 2024-04-24 07:54:28.000000 mctech_cloud-1.0.3/mctech_cloud/app_server.py
+drwxrwxrwx   0        0        0        0 2024-04-24 08:22:06.119261 mctech_cloud-1.0.3/mctech_cloud/middlewares/
+-rw-rw-rw-   0        0        0      679 2024-04-24 07:52:22.000000 mctech_cloud-1.0.3/mctech_cloud/middlewares/__init__.py
+-rw-rw-rw-   0        0        0     1790 2024-04-24 07:59:34.000000 mctech_cloud-1.0.3/mctech_cloud/middlewares/service_context_middleware.py
+drwxrwxrwx   0        0        0        0 2024-04-24 08:22:06.112249 mctech_cloud-1.0.3/mctech_cloud.egg-info/
+-rw-rw-rw-   0        0        0      147 2024-04-24 08:22:06.000000 mctech_cloud-1.0.3/mctech_cloud.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      354 2024-04-24 08:22:06.000000 mctech_cloud-1.0.3/mctech_cloud.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 08:22:06.000000 mctech_cloud-1.0.3/mctech_cloud.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2024-04-24 08:22:06.000000 mctech_cloud-1.0.3/mctech_cloud.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-04-24 08:22:06.000000 mctech_cloud-1.0.3/mctech_cloud.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      314 2024-04-24 08:21:43.000000 mctech_cloud-1.0.3/mctech_cloud_setup.py
+-rw-rw-rw-   0        0        0       42 2024-04-24 08:22:06.126248 mctech_cloud-1.0.3/setup.cfg
```

### Comparing `mctech_cloud-1.0.2/mctech_cloud/app_server.py` & `mctech_cloud-1.0.3/mctech_cloud/app_server.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,50 +1,40 @@
 import uvicorn
-import math
 
 from log4py import logging
 from fastapi import FastAPI
 from mctech_discovery.discovery import discovery_client, configure
+from mctech_core import tracing
 from . import middlewares
 
 log = logging.getLogger('python.cloud.appServer')
 
 
-def try_convert_number(val: str):
-    ret = int(val)
-    return val if math.isnan(ret)else ret
-
-
 def init_app_manager():
     # log.info('开始初始化各部分组件......')
     # #  配置合并完成，开始触发执行延迟初始化事件
     # #  @ts-expect-error 未暴露方法
     # appManager.onIniting(configure)
     # log.info('组件初始化完成！')
     pass
 
 
 class AppServer:
     def __init__(self):
         self._app = FastAPI()
-        self._converters = {
-            'x-tenant-id': try_convert_number,
-            'x-user-id': try_convert_number,
-            'x-id': try_convert_number,
-            'x-org-id': try_convert_number
-        }
 
     @property
     def app(self):
         return self._app
 
     def _init(self):
         middlewares.create_actuator(configure, self._app)
         init_app_manager()
-        middlewares.create_extras(self._converters, self._app)
+        middlewares.create_extras(self._app)
+        tracing.create_tracing(self._app)
 
     def start(self):
         # 启动eureka(当前应用不会注册到注册中心)
         discovery_client.start()
         #  通过注册中心找到配置服务，加载远程配置
         discovery_client.load_config()
         configure.merge()
```

### Comparing `mctech_cloud-1.0.2/mctech_cloud/middlewares/__init__.py` & `mctech_cloud-1.0.3/mctech_cloud/middlewares/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from log4py import logging
 from fastapi import FastAPI
 from mctech_actuator import create_actuator_route
 
 log = logging.getLogger('python.cloud.middlewares')
 
 
-def create_extras(converters, app: FastAPI):
+def create_extras(app: FastAPI, converters=None):
     """创建构建extras的middleware
     """
     app.add_middleware(ServiceContextMiddleware, converters=converters)
     log.info('创建extras context middleware完成')
 
 
 def create_actuator(configure, app: FastAPI):
```

### Comparing `mctech_cloud-1.0.2/mctech_cloud/middlewares/service_context_middleware.py` & `mctech_cloud-1.0.3/mctech_cloud/middlewares/service_context_middleware.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,38 +1,53 @@
 import re
+import math
+
+from typing import Dict, Callable
 from starlette.datastructures import Headers
-from starlette.types import Receive, Scope, Send
-from .. import header_filter as filter
+from starlette.types import ASGIApp, Receive, Scope, Send
+from mctech_core.context import get_async_context, WebContext, \
+    header_filter as filter
 
 pattern = re.compile('-([a-z])', re.IGNORECASE)
 
 
+def try_convert_number(val: str):
+    ret = int(val)
+    return val if math.isnan(ret)else ret
+
+
+_converters: Dict[str, Callable[[str], any]] = {
+    'x-tenant-id': try_convert_number,
+    'x-user-id': try_convert_number,
+    'x-id': try_convert_number,
+    'x-org-id': try_convert_number
+}
+
+
 class ServiceContextMiddleware:
-    def __init__(self, app, converters):
+    def __init__(self,
+                 app: ASGIApp,
+                 converters: Dict[str, Callable[[str], any]]):
         self._app = app
-        self._converters = converters
+        self._converters = dict(_converters)
+        if converters:
+            self._converters.update(converters)
 
     async def __call__(self, scope: Scope, receive: Receive, send: Send):
         headers = Headers(scope=scope)
         headerNames = headers.keys()
-        processors = filter.process(headerNames)
-        tracingHeaders = processors['tracingHeaders']
-        extrasHeaders = processors['extrasHeaders']
-
-        tracing = {}
-        for header_name in tracingHeaders:
-            tracing[header_name] = headers[header_name]
-        scope['tracing'] = tracing
-
+        extrasHeaders = filter.process(headerNames, 'extras')
         extras = {}
         for header_name in extrasHeaders:
             self._resolve_extras_value(extras, headers, header_name)
 
         scope['extras'] = extras
-        await self._app(scope, receive, send)
+        ctx = get_async_context()
+        ctx.webContext = WebContext({}, extras)
+        return await ctx.run(self._app, scope, receive, send)
 
     def _resolve_extras_value(self, extras: dict, headers: Headers, name: str):
         key = pattern.sub(to_upper, name.replace('x-', ''))
         converter = self._converters.get(name)
         value = headers[name]
         if converter:
             value = converter(value)
```


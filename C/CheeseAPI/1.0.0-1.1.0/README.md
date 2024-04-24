# Comparing `tmp/cheeseapi-1.0.0.tar.gz` & `tmp/cheeseapi-1.1.0.tar.gz`

## Comparing `cheeseapi-1.0.0.tar` & `cheeseapi-1.1.0.tar`

### file list

```diff
@@ -1,20 +1,21 @@
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 cheeseapi-1.0.0/CheeseAPI/__init__.py
--rw-r--r--   0        0        0     2033 2020-02-02 00:00:00.000000 cheeseapi-1.0.0/CheeseAPI/app.py
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 cheeseapi-1.0.0/CheeseAPI/cors.py
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 cheeseapi-1.0.0/CheeseAPI/exception.py
--rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 cheeseapi-1.0.0/CheeseAPI/file.py
--rw-r--r--   0        0        0    30863 2020-02-02 00:00:00.000000 cheeseapi-1.0.0/CheeseAPI/handle.py
--rw-r--r--   0        0        0     4388 2020-02-02 00:00:00.000000 cheeseapi-1.0.0/CheeseAPI/protocol.py
--rw-r--r--   0        0        0     2803 2020-02-02 00:00:00.000000 cheeseapi-1.0.0/CheeseAPI/request.py
--rw-r--r--   0        0        0    15979 2020-02-02 00:00:00.000000 cheeseapi-1.0.0/CheeseAPI/response.py
--rw-r--r--   0        0        0     6814 2020-02-02 00:00:00.000000 cheeseapi-1.0.0/CheeseAPI/route.py
--rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 cheeseapi-1.0.0/CheeseAPI/server.py
--rw-r--r--   0        0        0     2362 2020-02-02 00:00:00.000000 cheeseapi-1.0.0/CheeseAPI/signal.py
--rw-r--r--   0        0        0     7664 2020-02-02 00:00:00.000000 cheeseapi-1.0.0/CheeseAPI/text.py
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 cheeseapi-1.0.0/CheeseAPI/websocket.py
--rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 cheeseapi-1.0.0/CheeseAPI/workspace.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 cheeseapi-1.0.0/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 cheeseapi-1.0.0/LICENSE
--rw-r--r--   0        0        0     4311 2020-02-02 00:00:00.000000 cheeseapi-1.0.0/README.md
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 cheeseapi-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     4776 2020-02-02 00:00:00.000000 cheeseapi-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 cheeseapi-1.1.0/CheeseAPI/__init__.py
+-rw-r--r--   0        0        0     7395 2020-02-02 00:00:00.000000 cheeseapi-1.1.0/CheeseAPI/app.py
+-rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 cheeseapi-1.1.0/CheeseAPI/cors.py
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 cheeseapi-1.1.0/CheeseAPI/exception.py
+-rw-r--r--   0        0        0     1312 2020-02-02 00:00:00.000000 cheeseapi-1.1.0/CheeseAPI/file.py
+-rw-r--r--   0        0        0    32439 2020-02-02 00:00:00.000000 cheeseapi-1.1.0/CheeseAPI/handle.py
+-rw-r--r--   0        0        0     4493 2020-02-02 00:00:00.000000 cheeseapi-1.1.0/CheeseAPI/protocol.py
+-rw-r--r--   0        0        0     4771 2020-02-02 00:00:00.000000 cheeseapi-1.1.0/CheeseAPI/request.py
+-rw-r--r--   0        0        0    17621 2020-02-02 00:00:00.000000 cheeseapi-1.1.0/CheeseAPI/response.py
+-rw-r--r--   0        0        0    11099 2020-02-02 00:00:00.000000 cheeseapi-1.1.0/CheeseAPI/route.py
+-rw-r--r--   0        0        0    10335 2020-02-02 00:00:00.000000 cheeseapi-1.1.0/CheeseAPI/schedule.py
+-rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 cheeseapi-1.1.0/CheeseAPI/server.py
+-rw-r--r--   0        0        0     2138 2020-02-02 00:00:00.000000 cheeseapi-1.1.0/CheeseAPI/signal.py
+-rw-r--r--   0        0        0     7664 2020-02-02 00:00:00.000000 cheeseapi-1.1.0/CheeseAPI/text.py
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 cheeseapi-1.1.0/CheeseAPI/websocket.py
+-rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 cheeseapi-1.1.0/CheeseAPI/workspace.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 cheeseapi-1.1.0/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 cheeseapi-1.1.0/LICENSE
+-rw-r--r--   0        0        0     4551 2020-02-02 00:00:00.000000 cheeseapi-1.1.0/README.md
+-rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 cheeseapi-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     5001 2020-02-02 00:00:00.000000 cheeseapi-1.1.0/PKG-INFO
```

### Comparing `cheeseapi-1.0.0/CheeseAPI/file.py` & `cheeseapi-1.1.0/CheeseAPI/file.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,34 @@
 import os
 from typing import overload
 
 class File:
     @overload
     def __init__(self, filePath: str):
-        ...
+        '''
+        通过文件路径进行读取；支持相对路径以及绝对路径。
+
+        ```python
+        from CheeseAPI import File
+
+        file = File('./media/a.py')
+        ```
+        '''
 
     @overload
     def __init__(self, name: str, data: bytes | str):
-        ...
+        '''
+        通过二进制数据或字符串创建文件。
+
+        ```python
+        from CheeseAPI import File
+
+        file = File('test.txt', '这里是CheeseAPI！')
+        ```
+        '''
 
     def __init__(self, arg0: str, arg1: bytes | None = None):
         from CheeseAPI.app import app
 
         self.name: str
         self.data: bytes
 
@@ -21,11 +37,15 @@
             self.data = arg1
         else:
             self.name = arg0.split('/')[-1]
             with open(arg0 if arg0[0] == '/' else os.path.join(app.workspace.base, arg0), 'rb') as f:
                 self.data = f.read()
 
     def save(self, filePath: str):
+        '''
+        保存文件；支持相对路径以及绝对路径。
+        '''
+
         from CheeseAPI.app import app
 
         with open(filePath if filePath[0] == '/' else os.path.join(app.workspace.base, filePath), 'w') as f:
             f.write(self.data)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cheeseapi-1.0.0/CheeseAPI/handle.py` & `cheeseapi-1.1.0/CheeseAPI/handle.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,26 @@
-import time, os, inspect, socket, multiprocessing, signal, http, ipaddress
+import time, os, inspect, socket, multiprocessing, signal, http, ipaddress, datetime
 from typing import TYPE_CHECKING, Dict, Tuple, List
 
 import asyncio, uvloop, setproctitle, websockets
 from CheeseLog import logger
 
 from CheeseAPI.response import BaseResponse, FileResponse, Response
+from CheeseAPI.exception import Route_404_Exception, Route_405_Exception
 
 if TYPE_CHECKING:
     from CheeseAPI.app import App
     from CheeseAPI.protocol import HttpProtocol, WebsocketProtocol
 
 class Handle:
     def __init__(self, app: 'App'):
         self._app: 'App' = app
 
+        self._timer: datetime.datetime | None = None
+
     def server_beforeStarting(self):
         self._app.g['startTime'] = time.time()
 
         for text in self._app._text.server_information():
             logger.starting(text[0], text[1])
 
         self.loadModules()
@@ -155,202 +158,233 @@
         self.worker_beforeStarting()
         if self._app.signal.worker_beforeStarting.receivers:
             self._app.signal.worker_beforeStarting.send()
 
         asyncio.set_event_loop_policy(uvloop.EventLoopPolicy())
         asyncio.run(self.worker_run(sock, master))
 
-        with self._app._managers['lock']:
-            self._app._managers['server.workers'].value -= 1
+        with self._app._managers_['lock']:
+            self._app._managers_['server.workers'].value -= 1
 
             for text in self._app._text.worker_stopping():
                 logger.debug(text[0], text[1])
 
             self.worker_afterStopping()
             if self._app.signal.worker_afterStopping.receivers:
                 self._app.signal.worker_afterStopping.send()
 
     async def worker_run(self, sock, master: bool):
         from CheeseAPI.app import app
         from CheeseAPI.protocol import HttpProtocol
 
-        app.g = self._app.g
-        app.managers = self._app.managers
-        app._managers = self._app._managers
+        app._g = self._app.g
+        app._managers = self._app.managers
+        app._managers_ = self._app._managers_
 
         loop = asyncio.get_running_loop()
         server = await loop.create_server(HttpProtocol, sock = sock)
         loop.add_signal_handler(signal.SIGINT, lambda server: server.close(), server)
         loop.add_signal_handler(signal.SIGTERM, lambda server: server.close(), server)
 
         await self.worker_afterStarting()
         if self._app.signal.worker_afterStarting.receivers:
-            await self._app.signal.worker_afterStarting.send_async()
+            await self._app.signal.worker_afterStarting.async_send()
 
-        with self._app._managers['lock']:
-            self._app._managers['server.workers'].value += 1
-            if self._app._managers['server.workers'].value == self._app.server.workers:
+        with self._app._managers_['lock']:
+            self._app._managers_['server.workers'].value += 1
+            if self._app._managers_['server.workers'].value == self._app.server.workers:
                 for text in self._app._text.server_starting():
                     logger.starting(text[0], text[1])
 
                 await self.server_afterStarting()
                 if self._app.signal.server_afterStarting.receivers:
-                    await self._app.signal.server_afterStarting.send_async()
+                    await self._app.signal.server_afterStarting.async_send()
 
         while server.is_serving():
             if master:
                 await self.server_running()
                 if self._app.signal.server_running.receivers:
-                    await self._app.signal.server_running.send_async()
+                    await self._app.signal.server_running.async_send()
 
             await self.worker_running()
             if self._app.signal.worker_running.receivers:
-                await self._app.signal.worker_running.send_async()
+                await self._app.signal.worker_running.async_send()
 
             await asyncio.sleep(self._app.server.intervalTime)
 
-        with self._app._managers['lock']:
-            if self._app._managers['server.workers'].value == self._app.server.workers:
+        with self._app._managers_['lock']:
+            if self._app._managers_['server.workers'].value == self._app.server.workers:
                 await self.server_beforeStopping()
                 if self._app.signal.server_beforeStopping.receivers:
-                    await self._app.signal.server_beforeStopping.send_async()
+                    await self._app.signal.server_beforeStopping.async_send()
 
             await self.worker_beforeStopping()
             if self._app.signal.worker_beforeStopping.receivers:
-                await self._app.signal.worker_beforeStopping.send_async()
+                await self._app.signal.worker_beforeStopping.async_send()
 
     async def worker_afterStarting(self):
         ...
 
     async def server_afterStarting(self):
         ...
 
     async def server_running(self):
-        ...
+        if not self._timer:
+            self._timer = datetime.datetime.now()
+            return
+
+        timer = datetime.datetime.now()
+
+        for task in self._app.scheduler.tasks.values():
+            triggeredTimer = task.startTimer + task.timer * task.total_repetition_num
+
+            if (self._timer < triggeredTimer < timer or self._timer > triggeredTimer + task.timer) and task.active and task.is_unexpired:
+                self._app._managers_['schedules'][task.key] = {
+                    **self._app._managers_['schedules'][task.key],
+                    'total_repetition_num': task.total_repetition_num + 1
+                }
+                await task.fn()
+                if task.is_expired and task.auto_remove:
+                    self._app.scheduler.remove(task.key)
+
+        self._timer = timer
 
     async def worker_running(self):
         ...
 
     async def http_beforeRequest(self, protocol: 'HttpProtocol'):
         ...
 
     async def http_afterRequest(self, protocol: 'HttpProtocol'):
         ...
 
     async def http(self, protocol: 'HttpProtocol'):
         try:
             await self._app._handle.http_beforeRequest(self)
             if self._app.signal.http_beforeRequest.receivers:
-                await self._app.signal.http_beforeRequest.send_async()
+                await self._app.signal.http_beforeRequest.async_send()
 
             await self.http_static(protocol)
             if isinstance(protocol.response, BaseResponse):
                 if self._app.signal.http_static.receivers:
-                    await self._app.signal.http_static.send_async(**{
+                    await self._app.signal.http_static.async_send(**{
                         'request': protocol.request,
                         'response': protocol.response,
                         **protocol.kwargs
                     })
                 await self.http_response(protocol)
                 return
 
             try:
                 func, protocol.kwargs = self._app.routeBus._match(protocol.request.path, protocol.request.method)
-            except KeyError as e:
+            except Route_404_Exception as e:
                 await self.http_afterRequest(protocol)
                 if self._app.signal.http_afterRequest.receivers:
-                    await self._app.signal.http_afterRequest.send_async(**{
+                    await self._app.signal.http_afterRequest.async_send(**{
                         'request': protocol.request,
                         **protocol.kwargs
                     })
 
-                if e.args[0] == 0:
-                    await self.http_404(protocol)
-                    if self._app.signal.http_404.receivers:
-                        await self._app.signal.http_404.send_async(**{
-                            'request': protocol.request,
-                            'response': protocol.response,
-                            **protocol.kwargs
-                        })
-                    await self.http_response(protocol)
-                    return
+                await self.http_404(protocol)
+                if self._app.signal.http_404.receivers:
+                    await self._app.signal.http_404.async_send(**{
+                        'request': protocol.request,
+                        'response': protocol.response,
+                        **protocol.kwargs
+                    })
+                await self.http_response(protocol)
+                return
+            except Route_405_Exception as e:
+                await self.http_afterRequest(protocol)
+                if self._app.signal.http_afterRequest.receivers:
+                    await self._app.signal.http_afterRequest.async_send(**{
+                        'request': protocol.request,
+                        **protocol.kwargs
+                    })
 
-                if e.args[0] == 1:
-                    if protocol.request.method == http.HTTPMethod.OPTIONS:
-                        protocol.response = Response(status = 200)
-
-                        if self._app.signal.http_options.receivers:
-                            await self._app.signal.http_options.send_async(**{
-                                'request': protocol.request,
-                                'response': protocol.response,
-                                **protocol.kwargs
-                            })
-                        await self.http_response(protocol)
-                        return
-
-                    await self.http_405(protocol)
-                    if self._app.signal.http_405.receivers:
-                        await self._app.signal.http_405.send_async(**{
+                if protocol.request.method == http.HTTPMethod.OPTIONS:
+                    protocol.response = Response(status = 200)
+
+                    if self._app.signal.http_options.receivers:
+                        await self._app.signal.http_options.async_send(**{
                             'request': protocol.request,
                             'response': protocol.response,
-                            'e': e,
                             **protocol.kwargs
                         })
                     await self.http_response(protocol)
                     return
 
-                raise e
+                await self.http_405(protocol)
+                if self._app.signal.http_405.receivers:
+                    await self._app.signal.http_405.async_send(**{
+                        'request': protocol.request,
+                        'response': protocol.response,
+                        'e': e,
+                        **protocol.kwargs
+                    })
+                await self.http_response(protocol)
+                return
 
             await self.http_afterRequest(protocol)
             if self._app.signal.http_afterRequest.receivers:
-                await self._app.signal.http_afterRequest.send_async(**{
+                await self._app.signal.http_afterRequest.async_send(**{
                     'request': protocol.request,
                     **protocol.kwargs
             })
 
             protocol.response = await func(**{
                 'request': protocol.request,
                 **protocol.kwargs
             })
 
+            if self._app.signal.http_custom.receivers:
+                await self._app.signal.http_custom.async_send(**{
+                    'request': protocol.request,
+                    'response': protocol.response,
+                    **protocol.kwargs
+                })
+
             await self.http_response(protocol)
         except BaseException as e:
             try:
                 await self.http_500(protocol, e)
                 if self._app.signal.http_500.receivers:
-                    await self._app.signal.http_500.send_async(**{
+                    await self._app.signal.http_500.async_send(**{
                         'request': protocol.request,
                         'response': protocol.response,
                         'e': e,
                         **protocol.kwargs
                     })
                 await self.http_response(protocol)
             except BaseException as e:
                 await self.http_500(protocol, e, True)
                 await self.http_response(protocol, True)
 
     async def http_static(self, protocol: 'HttpProtocol'):
         if self._app.server.static and self._app.workspace.static and protocol.request.path.startswith(self._app.server.static) and protocol.request.method == http.HTTPMethod.GET:
-            try:
-                protocol.response = FileResponse(os.path.join(self._app.workspace.static, protocol.request.path[1:]))
+            for key in [ '', '.html', 'index.html', '/index.html' ]:
+                try:
+                    protocol.response = FileResponse(os.path.join(self._app.workspace.static, protocol.request.path[1:] + key))
+
+                    await self.http_afterRequest(protocol)
+                    if self._app.signal.http_afterRequest.receivers:
+                        await self._app.signal.http_afterRequest.async_send(**{
+                            'request': protocol.request,
+                            **protocol.kwargs
+                        })
 
-                await self.http_afterRequest(protocol)
-                if self._app.signal.http_afterRequest.receivers:
-                    await self._app.signal.http_afterRequest.send_async(**{
-                        'request': protocol.request,
-                        **protocol.kwargs
-                    })
+                    if self._app.signal.http_static.receivers:
+                        await self._app.signal.http_static.async_send(**{
+                            'request': protocol.request,
+                            **protocol.kwargs
+                        })
 
-                if self._app.signal.http_static.receivers:
-                    await self._app.signal.http_static.send_async(**{
-                        'request': protocol.request,
-                        **protocol.kwargs
-                    })
-            except (FileNotFoundError, IsADirectoryError):
-                ...
+                    break
+                except (FileNotFoundError, NotADirectoryError, IsADirectoryError):
+                    ...
 
     async def http_options(self, protocol: 'HttpProtocol'):
         protocol.response = Response(status = http.HTTPStatus.OK)
 
     async def http_404(self, protocol: 'HttpProtocol'):
         protocol.response = Response(status = http.HTTPStatus.NOT_FOUND)
 
@@ -367,15 +401,15 @@
     async def http_response(self, protocol: 'HttpProtocol', recycled: bool = False):
         if not isinstance(protocol.response, BaseResponse):
             await self.noResponse(protocol)
 
         if not recycled:
             await self.http_beforeResponse(protocol)
             if self._app.signal.http_beforeResponse.receivers:
-                await self._app.signal.http_beforeResponse.send_async(**{
+                await self._app.signal.http_beforeResponse.async_send(**{
                     'request': protocol.request,
                     'response': protocol.response,
                     **protocol.kwargs
                 })
 
         if (
             (
@@ -411,15 +445,15 @@
                 protocol.transport.write(content)
         except RuntimeError:
             ...
 
         if not recycled:
             await self.http_afterResponse(protocol)
             if self._app.signal.http_afterResponse.receivers:
-                await self._app.signal.http_afterResponse.send_async(**{
+                await self._app.signal.http_afterResponse.async_send(**{
                     'request': protocol.request,
                     'response': protocol.response,
                     **protocol.kwargs
                 })
 
     async def noResponse(self, protocol: 'HttpProtocol') -> BaseResponse:
         protocol.response = Response(status = http.HTTPStatus.INTERNAL_SERVER_ERROR)
@@ -435,58 +469,58 @@
         try:
             try:
                 Server, kwargs = self._app.routeBus._match(protocol.request.path, 'WEBSOCKET')
                 protocol.kwargs.update(kwargs)
             except KeyError as e:
                 await self.websocket_afterRequest(protocol)
                 if self._app.signal.websocket_afterRequest.receivers:
-                    await self._app.signal.websocket_afterRequest.send_async(**{
+                    await self._app.signal.websocket_afterRequest.async_send(**{
                         'request': protocol.request,
                         **protocol.kwargs
                     })
 
                 if e.args[0] == 0:
                     await self.websocket_404(protocol)
                     if self._app.signal.websocket_404.receivers:
-                        await self._app.signal.websocket_404.send_async(**{
+                        await self._app.signal.websocket_404.async_send(**{
                             'request': protocol.request,
                             'response': protocol.response,
                             **protocol.kwargs
                         })
                     return await self.websocket_response(protocol)
 
                 elif e.args[0] == 1:
                     await self.websocket_405(protocol)
                     if self._app.signal.websocket_405.receivers:
-                        await self._app.signal.websocket_405.send_async(**{
+                        await self._app.signal.websocket_405.async_send(**{
                             'request': protocol.request,
                             'response': protocol.response,
                             **protocol.kwargs
                         })
                     return await self.websocket_response(protocol)
 
                 raise e
 
             protocol.server = Server()
 
             await self.websocket_afterRequest(protocol)
             if self._app.signal.websocket_afterRequest.receivers:
-                await self._app.signal.websocket_afterRequest.send_async(**{
+                await self._app.signal.websocket_afterRequest.async_send(**{
                     'request': protocol.request,
                     **protocol.kwargs
                 })
 
             await self.websocket_subprotocol(protocol)
 
             return await self.websocket_response(protocol)
         except BaseException as e:
             try:
                 await self.websocket_500(protocol, e)
                 if self._app.signal.websocket_500.receivers:
-                    await self._app.signal.websocket_500.send_async(**{
+                    await self._app.signal.websocket_500.async_send(**{
                         'request': protocol.request,
                         'response': protocol.response,
                         'e': e,
                         **protocol.kwargs
                     })
                 await self.websocket_response(protocol)
             except BaseException as e:
@@ -516,29 +550,29 @@
     async def websocket_response(self, protocol: 'WebsocketProtocol', recycled: bool = False) -> Tuple[int, Dict[str, str], bytes]:
         if not protocol.response or protocol.response.status == 200:
             return
 
         if not recycled:
             await self.websocket_beforeResponse(protocol)
             if self._app.signal.websocket_beforeResponse.receivers:
-                await self._app.signal.websocket_beforeResponse.send_async(**{
+                await self._app.signal.websocket_beforeResponse.async_send(**{
                     'request': protocol.request,
                     'response': protocol.response,
                     **protocol.kwargs
                 })
 
         results = int(protocol.response.status), protocol.response.headers, protocol.response.body.encode()
 
         if not recycled:
             for text in self._app._text.websocket_response(protocol):
                 logger.websocket(text[0], text[1])
 
             await self.websocket_afterResponse(protocol)
             if self._app.signal.websocket_afterResponse.receivers:
-                await self._app.signal.websocket_afterResponse.send_async(**{
+                await self._app.signal.websocket_afterResponse.async_send(**{
                     'request': protocol.request,
                     'response': protocol.response,
                     **protocol.kwargs
                 })
 
         return results
 
@@ -548,34 +582,34 @@
     async def websocket_afterResponse(self, protocol: 'WebsocketProtocol'):
         ...
 
     async def websocket_subprotocol(self, protocol: 'WebsocketProtocol') -> str:
         if not protocol.request.headers.get('Sec-Websocket-Protocol', None):
             return
 
-        protocol.request.subprotocols = protocol.request.headers['Sec-Websocket-Protocol'].split(', ')
+        protocol.request._subprotocols = protocol.request.headers['Sec-Websocket-Protocol'].split(', ')
 
         await self.websocket_beforeSubprotocol(protocol)
         if self._app.signal.websocket_beforeSubprotocol.receivers:
-            await self._app.signal.websocket_beforeSubprotocol.send_async(**{
+            await self._app.signal.websocket_beforeSubprotocol.async_send(**{
                 'request': protocol.request,
                 **protocol.kwargs
             })
 
-        protocol.request.subprotocol = await protocol.server.subprotocol(**{
+        protocol.request._subprotocol = await protocol.server.subprotocol(**{
             'request': protocol.request,
             **protocol.kwargs
         })
         if protocol.request.subprotocol not in protocol.request.subprotocols:
             protocol.response = Response(status = http.HTTPStatus.BAD_REQUEST)
             del protocol.response.headers['Transfer-Encoding']
 
         await self.websocket_afterSubprotocol(protocol)
         if self._app.signal.websocket_afterSubprotocol.receivers:
-            await self._app.signal.websocket_afterSubprotocol.send_async(**{
+            await self._app.signal.websocket_afterSubprotocol.async_send(**{
                 'request': protocol.request,
                 'response': protocol.response,
                 **protocol.kwargs
             })
 
     async def websocket_beforeSubprotocol(self, protocol: 'WebsocketProtocol'):
         ...
@@ -583,50 +617,50 @@
     async def websocket_afterSubprotocol(self, protocol: 'WebsocketProtocol'):
         ...
 
     async def websocket(self, protocol: 'WebsocketProtocol'):
         try:
             await self.websocket_beforeConnection(protocol)
             if self._app.signal.websocket_beforeConnection.receivers:
-                await self._app.signal.websocket_beforeConnection.send_async(**{
+                await self._app.signal.websocket_beforeConnection.async_send(**{
                     'request': protocol.request,
                     **protocol.kwargs
                 })
 
             await self.websocket_connection(protocol)
             await protocol.server.connection(**{
                 'request': protocol.request,
                 **protocol.kwargs
             })
 
             await self.websocket_afterConnection(protocol)
             if self._app.signal.websocket_afterConnection.receivers:
-                await self._app.signal.websocket_afterConnection.send_async(**{
+                await self._app.signal.websocket_afterConnection.async_send(**{
                     'request': protocol.request,
                     **protocol.kwargs
                 })
 
             try:
                 while not protocol.transport.is_closing():
                     await self._app._handle.websocket_message(protocol)
             except asyncio.CancelledError:
                 ...
 
             await self.websocket_disconnection(protocol)
             await self.websocket_afterDisconnection()
             if self._app.signal.websocket_afterDisconnection.receivers:
-                await self._app.signal.websocket_afterDisconnection.send_async(**{
+                await self._app.signal.websocket_afterDisconnection.async_send(**{
                     'request': protocol.request,
                     **protocol.kwargs
                 })
         except BaseException as e:
             try:
                 await self.websocket_500(protocol, e, False, True)
                 if self._app.signal.websocket_500.receivers:
-                    await self._app.signal.websocket_500.send_async(**{
+                    await self._app.signal.websocket_500.async_send(**{
                         'request': protocol.request,
                         'response': protocol.response,
                         'e': e,
                         **protocol.kwargs
                     })
             except BaseException as e:
                 await self.websocket_500(protocol, e, True, True)
@@ -646,29 +680,29 @@
 
     async def websocket_message(self, protocol: 'WebsocketProtocol'):
         try:
             message = await asyncio.wait_for(protocol.recv(), timeout = self._app.server.intervalTime)
 
             await self.websocket_beforeMessage(protocol, message)
             if self._app.signal.websocket_beforeMessage.receivers:
-                await self._app.signal.websocket_beforeMessage.send_async(**{
+                await self._app.signal.websocket_beforeMessage.async_send(**{
                     'request': protocol.request,
                     'message': message,
                     **protocol.kwargs
                 })
 
             await protocol.server.message(**{
                 'request': protocol.request,
                 'message': message,
                 **protocol.kwargs
             })
 
             await self.websocket_afterMessage(protocol, message)
             if self._app.signal.websocket_afterMessage.receivers:
-                await self._app.signal.websocket_afterMessage.send_async({
+                await self._app.signal.websocket_afterMessage.async_send({
                     'request': protocol.request,
                     'message': message,
                     **protocol.kwargs
                 })
         except (websockets.exceptions.ConnectionClosed, websockets.exceptions.ConnectionClosedError, websockets.exceptions.ConnectionClosedOK, asyncio.TimeoutError):
             ...
 
@@ -677,51 +711,51 @@
 
     async def websocket_afterMessage(self, protocol: 'WebsocketProtocol', message: str | bytes):
         ...
 
     async def websocket_send(self, protocol: 'WebsocketProtocol', message: str | bytes):
         await self.websocket_beforeSending(protocol, message)
         if self._app.signal.websocket_beforeSending.receivers:
-            await self._app.signal.websocket_beforeSending.send_async(**{
+            await self._app.signal.websocket_beforeSending.async_send(**{
                 'request': protocol.request,
                 'message': message,
                 **protocol.kwargs
             })
 
         await protocol.send(message)
 
         await self.websocket_afterSending(protocol, message)
         if self._app.signal.websocket_afterSending.receivers:
-            await self._app.signal.websocket_afterSending.send_async(**{
+            await self._app.signal.websocket_afterSending.async_send(**{
                 'request': protocol.request,
                 'message': message,
                 **protocol.kwargs
             })
 
     async def websocket_beforeSending(self, protocol: 'WebsocketProtocol', message: str | bytes):
         ...
 
     async def websocket_afterSending(self, protocol: 'WebsocketProtocol', message: str | bytes):
         ...
 
     async def websocket_close(self, protocol: 'WebsocketProtocol', code: int, reason: str):
         await self.websocket_beforeClosing(protocol, code, reason)
         if self._app.signal.websocket_beforeClosing.receivers:
-            await self._app.signal.websocket_beforeClosing.send_async(**{
+            await self._app.signal.websocket_beforeClosing.async_send(**{
                 'request': protocol.request,
                 'code': code,
                 'reason': reason,
                 **protocol.kwargs
             })
 
         await protocol.close(code, reason)
 
         await self.websocket_afterClosing(protocol, code, reason)
         if self._app.signal.websocket_afterSending.receivers:
-            await self._app.signal.websocket_afterSending.send_async(**{
+            await self._app.signal.websocket_afterSending.async_send(**{
                 'request': protocol.request,
                 'code': code,
                 'reason': reason,
                 **protocol.kwargs
             })
 
     async def websocket_beforeClosing(self, protocol: 'WebsocketProtocol', code: int, reason: str):
```

### Comparing `cheeseapi-1.0.0/CheeseAPI/protocol.py` & `cheeseapi-1.1.0/CheeseAPI/protocol.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,38 +30,41 @@
 
             websocketProtocol = WebsocketProtocol(self)
             websocketProtocol.connection_made(self.transport)
             websocketProtocol.data_received(data)
             self.transport.set_protocol(websocketProtocol)
 
     def on_url(self, url: bytes):
-        self.request = Request(http.HTTPMethod(self.parser.get_method().decode()), url.decode())
+        try:
+            self.request = Request(http.HTTPMethod(self.parser.get_method().decode()), url.decode())
+        except ValueError:
+            self.request = Request(None, url.decode())
         self.response = None
         self.kwargs = {}
 
     def on_header(self, key: bytes, value: bytes):
         self.request.headers['-'.join([t.capitalize() for t in key.decode().split('-')])] = value.decode()
 
     def on_headers_complete(self):
-        self.request.client = self.request.headers.get('X-Real-Ip', self.transport.get_extra_info('socket').getpeername()[0])
-        self.request.origin = self.request.headers.get('Origin', f'{self.transport.get_extra_info("socket").getsockname()[0]}:{self.transport.get_extra_info("socket").getsockname()[1]}')
-        self.request.scheme = self.request.headers.get('X-Forwarded-Proto', 'https' if self.transport.get_extra_info('sslcontext') else 'http')
+        self.request._client = self.request.headers.get('X-Real-Ip', self.transport.get_extra_info('socket').getpeername()[0])
+        self.request._origin = self.request.headers.get('Origin', f'{self.transport.get_extra_info("socket").getsockname()[0]}:{self.transport.get_extra_info("socket").getsockname()[1]}')
+        self.request._scheme = self.request.headers.get('X-Forwarded-Proto', 'https' if self.transport.get_extra_info('sslcontext') else 'http')
 
         if 'Cookie' in self.request.headers:
-            self.request.cookie = {
+            self.request._cookie = {
                 t.split('=')[0]: t.split('=')[1] for t in self.request.headers['Cookie'].split('; ')
             }
 
         if not self.parser.should_upgrade() and not int(self.request.headers.get('Content-Length', 0)):
             asyncio.get_event_loop().create_task(app._handle.http(self))
 
     def on_body(self, body: bytes):
         if self.request.body is None:
-            self.request.body = b''
-        self.request.body += body
+            self.request._body = b''
+        self.request._body += body
 
         if len(self.request.body) == int(self.request.headers.get('Content-Length', 0)):
             self.request._parseBody()
             asyncio.get_event_loop().create_task(app._handle.http(self))
 
     def connection_lost(self, exc: Exception | None):
         self.transport.close()
```

### Comparing `cheeseapi-1.0.0/CheeseAPI/response.py` & `cheeseapi-1.1.0/CheeseAPI/response.py`

 * *Files 17% similar despite different names*

```diff
@@ -333,14 +333,28 @@
     'x_t': 'application/x-x_t',
     'ipa': 'application/vnd.iphone',
     'apk': 'application/vnd.android.package-archive',
     'xap': 'application/x-silverlight-app',
 }
 
 class BaseResponse:
+    '''
+    其他Response的父类；平时使用它判断response是否是合法的，并不建议使用它创建response。
+
+    ```python
+    from CheeseAPI import app, BaseResponse
+
+    @app.route.get('/')
+    async def index(*args, **kwargs):
+        response = ...
+        if isinstance(response, BaseResponse):
+            ...
+    ```
+    '''
+
     def __init__(self, body: str | bytes | Callable | AsyncIterator | None = None, status: http.HTTPStatus | int = http.HTTPStatus.OK, headers: Dict[str, str] = {}):
         from CheeseAPI.app import app
 
         self.status: http.HTTPStatus = http.HTTPStatus(status)
         self.headers: Dict[str, str] = {
             'Server': app._text.response_server,
             'Transfer-Encoding': 'chunked',
@@ -413,35 +427,73 @@
             if isinstance(maxAge, int):
                 s += f' Max-Age={maxAge};'
             elif isinstance(maxAge, datetime.timedelta):
                 s += f' Max-Age={maxAge.total_seconds()};'
         self.headers['Set-Cookies'][key] = s
 
 class Response(BaseResponse):
+    '''
+    ```python
+    from CheeseAPI import app, Response
+
+    @app.route.get('/')
+    async def index(*args, **kwargs):
+        return Response('这里是CheeseAPI！')
+    ```
+    '''
+
     def __init__(self, body: str | bytes | Callable | AsyncIterator | None = None, status: http.HTTPStatus | int = http.HTTPStatus.OK, headers: Dict[str, str] = {}):
         super().__init__(body, status, {
             'Content-Type': 'text/plain',
             **headers
         })
 
 class JsonResponse(BaseResponse):
+    '''
+    可将`dict`或`list`自动转为可发送的格式。
+
+    ```python
+    from CheeseAPI import app, JsonResponse
+
+    @app.route.get('/')
+    async def index(*args, **kwargs):
+        return JsonResponse({
+            'welcome': '这里是CheeseAPI！'
+        })
+    ```
+    '''
+
     def __init__(self, body: dict | list = {}, status: http.HTTPStatus | int = http.HTTPStatus.OK, headers: Dict[str, str] = {}):
         super().__init__(json.dumps(body), status, {
             'Content-Type': 'application/json; charset=utf-8',
             **headers
         })
 
 class FileResponse(BaseResponse):
     @overload
     def __init__(self, path: str, headers: Dict[str, str] = {}, *, downloaded: bool = False, chunkSize: int = 1024 * 1024):
-        ...
+        '''
+        - Args
+
+            - path: 文件路径；支持相对路径与绝对路径。
+
+            - downloaded: 文件是否下载；为`False`时优先预览，若无法预览则仍然下载。
+
+            - chunkSize: 发送文件的chunk大小。
+        '''
 
     @overload
     def __init__(self, data: File, headers: Dict[str, str] = {}, *, downloaded: bool = False, chunkSize: int = 1024 * 1024):
-        ...
+        '''
+        - Args
+
+            - downloaded: 文件是否下载；为`False`时优先预览，若无法预览则仍然下载。
+
+            - chunkSize: 发送文件的chunk大小。
+        '''
 
     def __init__(self, arg: str | File, headers: Dict[str, str] = {}, *, downloaded: bool = False, chunkSize: int = 1024 * 1024):
         self.file: File = File(arg) if isinstance(arg, str) else arg
         self.downloaded: bool = downloaded
         self.chunkSize: int = chunkSize
 
         suffix = self.file.name.split('.')[-1]
@@ -456,7 +508,15 @@
         length = len(self.file.data)
         index = 0
 
         while index < length:
             endIndex = min(index + self.chunkSize, length)
             yield self.file.data[index:endIndex]
             index = endIndex
+
+class RedirectResponse(BaseResponse):
+    def __init__(self, location: str, status: http.HTTPStatus | int = http.HTTPStatus.FOUND, body: str | bytes | None = None, headers: Dict[str, str] = {}):
+        super().__init__(body, status, {
+            'Content-Type': 'text/plain',
+            'Location': location,
+            **headers
+        })
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cheeseapi-1.0.0/CheeseAPI/server.py` & `cheeseapi-1.1.0/CheeseAPI/server.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,19 +9,27 @@
         self._app: 'App' = app
 
         self.host: str = '0.0.0.0'
         self.port: int = 5214
         self._workers: int = 1
         self.backlog: int = 1024
         self.static: str = '/'
-        self.intervalTime: float = 0.016
+        self._intervalTime: float = 0.016
 
     @property
     def workers(self) -> int:
         return self._workers
 
     @workers.setter
     def workers(self, value: int):
         if value == 0:
             self._workers = os.cpu_count() * 2 + 1
         else:
             self._workers = value
+
+    @property
+    def intervalTime(self) -> float:
+        '''
+        服务器处理间隔时间，单位为秒；越小的处理间隔意味着服务器对于某些特定的响应会更快。
+        '''
+
+        return self._intervalTime
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cheeseapi-1.0.0/CheeseAPI/signal.py` & `cheeseapi-1.1.0/CheeseAPI/signal.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from typing import TYPE_CHECKING, Any, Callable
 
-import blinker
-from ordered_set import OrderedSet
+from CheeseSignal import Signal
 
 if TYPE_CHECKING:
     from CheeseAPI.app import App
 
 class _Signal:
     def __init__(self, app: 'App'):
         self.app: 'App' = app
@@ -46,13 +45,7 @@
         self.websocket_beforeMessage: Signal = Signal()
         self.websocket_afterMessage: Signal = Signal()
         self.websocket_beforeSending: Signal = Signal()
         self.websocket_afterSending: Signal = Signal()
         self.websocket_beforeClosing: Signal = Signal()
         self.websocket_afterClosing: Signal = Signal()
         self.websocket_afterDisconnection: Signal = Signal()
-
-class Signal(blinker.Signal):
-    def connect_via(self, sender: Any = blinker.ANY, weak: TYPE_CHECKING = False) -> Callable:
-        return super().connect_via(sender, weak)
-
-Signal.set_class = OrderedSet
```

### Comparing `cheeseapi-1.0.0/CheeseAPI/text.py` & `cheeseapi-1.1.0/CheeseAPI/text.py`

 * *Files identical despite different names*

### Comparing `cheeseapi-1.0.0/CheeseAPI/websocket.py` & `cheeseapi-1.1.0/CheeseAPI/websocket.py`

 * *Files identical despite different names*

### Comparing `cheeseapi-1.0.0/LICENSE` & `cheeseapi-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cheeseapi-1.0.0/README.md` & `cheeseapi-1.1.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 3. Websocket支持。
 
 ## **安装**
 
 系统要求：Linux。
 
-Python要求：目前仅保证支持3.11及以上版本的Python，新版本会优先支持Python的最新稳定版本。
+Python要求：目前仅保证支持3.12版本的Python，新版本会优先支持Python的最新稳定版本。
 
 ```
 pip install CheeseAPI
 ```
 
 ## **依赖**
 
@@ -118,24 +118,28 @@
 
 #### 1.3 [**Signal （信号插槽）**](https://github.com/CheeseUnknown/CheeseAPI/blob/master/document/App/Signal.md)
 
 #### 1.4 [**RouteBus （路由总线）**](https://github.com/CheeseUnknown/CheeseAPI/blob/master/document/App/RouteBus.md)
 
 #### 1.5 [**Cors （跨域管理）**](https://github.com/CheeseUnknown/CheeseAPI/blob/master/document/App/Cors.md)
 
+#### 1.6 [**Scheduler （任务调度者）**](https://github.com/CheeseUnknown/CheeseAPI/blob/master/document/App/Scheduler.md)
+
 ### 2. [**Request （请求体）**](https://github.com/CheeseUnknown/CheeseAPI/blob/master/document/Request.md)
 
 ### 3. [**Response （响应体）**](https://github.com/CheeseUnknown/CheeseAPI/blob/master/document/Response.md)
 
 ### 4. [**Route （路由）**](https://github.com/CheeseUnknown/CheeseAPI/blob/master/document/Route.md)
 
 ### 5. [**Websocket**](https://github.com/CheeseUnknown/CheeseAPI/blob/master/document/Websocket.md)
 
 ### 6. [**File （文件）**](https://github.com/CheeseUnknown/CheeseAPI/blob/master/document/File.md)
 
-### 7. [**For 开发者**](https://github.com/CheeseUnknown/CheeseAPI/blob/master/document/Developer.md)
+### 7. [**Schedule （任务调度）**](https://github.com/CheeseUnknown/CheeseAPI/blob/master/document/Schedule.md)
+
+### 8. [**For 开发者**](https://github.com/CheeseUnknown/CheeseAPI/blob/master/document/Developer.md)
 
 ## **可用的插件模块**
 
 ### 1. **[CheeseAPI_Websocket](https://github.com/CheeseUnknown/CheeseAPI_Websocket)**
 
 websocket的升级插件，支持了更多、更便捷的通讯方式。
```

### Comparing `cheeseapi-1.0.0/pyproject.toml` & `cheeseapi-1.1.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 [build-system]
 requires = [ "hatchling" ]
 build-backend = "hatchling.build"
 
 [project]
 name = "CheeseAPI"
-version = "1.0.0"
+version = "1.1.0"
 description = "一款web协程框架。"
 readme = "README.md"
 license-files = { paths = [ "LICENSE" ] }
 authors = [
     { name = "Cheese Unknown", email = "cheese@cheese.ren" }
 ]
 keywords = [ 'API', 'BackEnd' ]
 
 dependencies = [
     "CheeseLog==1.0.*",
     "xmltodict",
-    "blinker",
     "websockets",
     "uvloop",
     "httptools",
-    "ordered_set"
+    "CheeseSignal==1.1.*"
 ]
 
 [project.urls]
 Source = "https://github.com/CheeseUnknown/CheeseAPI"
 
 [tool.hatch.build.targets.sdist]
 include = [ "/CheeseAPI" ]
```

### Comparing `cheeseapi-1.0.0/PKG-INFO` & `cheeseapi-1.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.3
 Name: CheeseAPI
-Version: 1.0.0
+Version: 1.1.0
 Summary: 一款web协程框架。
 Project-URL: Source, https://github.com/CheeseUnknown/CheeseAPI
 Author-email: Cheese Unknown <cheese@cheese.ren>
 License-File: LICENSE
 Keywords: API,BackEnd
-Requires-Dist: blinker
 Requires-Dist: cheeselog==1.0.*
+Requires-Dist: cheesesignal==1.1.*
 Requires-Dist: httptools
-Requires-Dist: ordered-set
 Requires-Dist: uvloop
 Requires-Dist: websockets
 Requires-Dist: xmltodict
 Description-Content-Type: text/markdown
 
 # **CheeseAPI**
 
@@ -27,15 +26,15 @@
 
 3. Websocket支持。
 
 ## **安装**
 
 系统要求：Linux。
 
-Python要求：目前仅保证支持3.11及以上版本的Python，新版本会优先支持Python的最新稳定版本。
+Python要求：目前仅保证支持3.12版本的Python，新版本会优先支持Python的最新稳定版本。
 
 ```
 pip install CheeseAPI
 ```
 
 ## **依赖**
 
@@ -135,24 +134,28 @@
 
 #### 1.3 [**Signal （信号插槽）**](https://github.com/CheeseUnknown/CheeseAPI/blob/master/document/App/Signal.md)
 
 #### 1.4 [**RouteBus （路由总线）**](https://github.com/CheeseUnknown/CheeseAPI/blob/master/document/App/RouteBus.md)
 
 #### 1.5 [**Cors （跨域管理）**](https://github.com/CheeseUnknown/CheeseAPI/blob/master/document/App/Cors.md)
 
+#### 1.6 [**Scheduler （任务调度者）**](https://github.com/CheeseUnknown/CheeseAPI/blob/master/document/App/Scheduler.md)
+
 ### 2. [**Request （请求体）**](https://github.com/CheeseUnknown/CheeseAPI/blob/master/document/Request.md)
 
 ### 3. [**Response （响应体）**](https://github.com/CheeseUnknown/CheeseAPI/blob/master/document/Response.md)
 
 ### 4. [**Route （路由）**](https://github.com/CheeseUnknown/CheeseAPI/blob/master/document/Route.md)
 
 ### 5. [**Websocket**](https://github.com/CheeseUnknown/CheeseAPI/blob/master/document/Websocket.md)
 
 ### 6. [**File （文件）**](https://github.com/CheeseUnknown/CheeseAPI/blob/master/document/File.md)
 
-### 7. [**For 开发者**](https://github.com/CheeseUnknown/CheeseAPI/blob/master/document/Developer.md)
+### 7. [**Schedule （任务调度）**](https://github.com/CheeseUnknown/CheeseAPI/blob/master/document/Schedule.md)
+
+### 8. [**For 开发者**](https://github.com/CheeseUnknown/CheeseAPI/blob/master/document/Developer.md)
 
 ## **可用的插件模块**
 
 ### 1. **[CheeseAPI_Websocket](https://github.com/CheeseUnknown/CheeseAPI_Websocket)**
 
 websocket的升级插件，支持了更多、更便捷的通讯方式。
```


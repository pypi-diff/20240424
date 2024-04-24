# Comparing `tmp/pytest-girder-3.2.4.dev7.tar.gz` & `tmp/pytest_girder-5a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-girder-3.2.4.dev7.tar", last modified: Wed Apr 24 19:14:06 2024, max compression
+gzip compressed data, was "pytest_girder-5a2.tar", last modified: Fri Apr 12 16:33:32 2024, max compression
```

## Comparing `pytest-girder-3.2.4.dev7.tar` & `pytest_girder-5a2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 19:14:06.642418 pytest-girder-3.2.4.dev7/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11358 2024-04-24 19:11:47.000000 pytest-girder-3.2.4.dev7/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)       43 2024-04-24 19:11:47.000000 pytest-girder-3.2.4.dev7/MANIFEST.in
--rw-r--r--   0 circleci  (1001) circleci  (1002)      408 2024-04-24 19:14:06.642418 pytest-girder-3.2.4.dev7/PKG-INFO
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 19:14:06.638419 pytest-girder-3.2.4.dev7/pytest_girder/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-04-24 19:11:47.000000 pytest-girder-3.2.4.dev7/pytest_girder/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1022 2024-04-24 19:11:47.000000 pytest-girder-3.2.4.dev7/pytest_girder/assertions.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6446 2024-04-24 19:11:47.000000 pytest-girder-3.2.4.dev7/pytest_girder/fixtures.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1772 2024-04-24 19:11:47.000000 pytest-girder-3.2.4.dev7/pytest_girder/plugin.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2875 2024-04-24 19:11:47.000000 pytest-girder-3.2.4.dev7/pytest_girder/plugin_registry.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11468 2024-04-24 19:11:47.000000 pytest-girder-3.2.4.dev7/pytest_girder/utils.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5970 2024-04-24 19:11:47.000000 pytest-girder-3.2.4.dev7/pytest_girder/web_client.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 19:14:06.642418 pytest-girder-3.2.4.dev7/pytest_girder.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      408 2024-04-24 19:14:06.000000 pytest-girder-3.2.4.dev7/pytest_girder.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      440 2024-04-24 19:14:06.000000 pytest-girder-3.2.4.dev7/pytest_girder.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-24 19:14:06.000000 pytest-girder-3.2.4.dev7/pytest_girder.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       41 2024-04-24 19:14:06.000000 pytest-girder-3.2.4.dev7/pytest_girder.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       51 2024-04-24 19:14:06.000000 pytest-girder-3.2.4.dev7/pytest_girder.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       14 2024-04-24 19:14:06.000000 pytest-girder-3.2.4.dev7/pytest_girder.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-04-24 19:14:06.642418 pytest-girder-3.2.4.dev7/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1310 2024-04-24 19:11:47.000000 pytest-girder-3.2.4.dev7/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:33:32.149790 pytest_girder-5a2/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11358 2024-04-12 16:27:18.000000 pytest_girder-5a2/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       43 2024-04-12 16:27:18.000000 pytest_girder-5a2/MANIFEST.in
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      405 2024-04-12 16:33:32.149790 pytest_girder-5a2/PKG-INFO
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:33:32.149790 pytest_girder-5a2/pytest_girder/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:27:18.000000 pytest_girder-5a2/pytest_girder/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1022 2024-04-12 16:27:18.000000 pytest_girder-5a2/pytest_girder/assertions.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6136 2024-04-12 16:27:18.000000 pytest_girder-5a2/pytest_girder/fixtures.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1772 2024-04-12 16:27:18.000000 pytest_girder-5a2/pytest_girder/plugin.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2923 2024-04-12 16:27:18.000000 pytest_girder-5a2/pytest_girder/plugin_registry.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11332 2024-04-12 16:27:18.000000 pytest_girder-5a2/pytest_girder/utils.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5970 2024-04-12 16:27:18.000000 pytest_girder-5a2/pytest_girder/web_client.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:33:32.149790 pytest_girder-5a2/pytest_girder.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      405 2024-04-12 16:33:32.000000 pytest_girder-5a2/pytest_girder.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      440 2024-04-12 16:33:32.000000 pytest_girder-5a2/pytest_girder.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-12 16:33:32.000000 pytest_girder-5a2/pytest_girder.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       41 2024-04-12 16:33:32.000000 pytest_girder-5a2/pytest_girder.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       51 2024-04-12 16:33:32.000000 pytest_girder-5a2/pytest_girder.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       14 2024-04-12 16:33:32.000000 pytest_girder-5a2/pytest_girder.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-04-12 16:33:32.149790 pytest_girder-5a2/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1310 2024-04-12 16:27:18.000000 pytest_girder-5a2/setup.py
```

### Comparing `pytest-girder-3.2.4.dev7/LICENSE` & `pytest_girder-5a2/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-girder-3.2.4.dev7/pytest_girder/assertions.py` & `pytest_girder-5a2/pytest_girder/assertions.py`

 * *Files identical despite different names*

### Comparing `pytest-girder-3.2.4.dev7/pytest_girder/fixtures.py` & `pytest_girder-5a2/pytest_girder/fixtures.py`

 * *Files 10% similar despite different names*

```diff
@@ -133,18 +133,14 @@
 
 
 @pytest.fixture
 def smtp(db, server):
     """
     Provides a mock SMTP server for testing.
     """
-    # TODO strictly speaking, this does not depend on the server itself, but does
-    # depend on the events daemon, which is currently managed by the server fixture.
-    # We should sort this out so that the daemon is its own fixture rather than being
-    # started/stopped via the cherrypy server lifecycle.
     from girder.models.setting import Setting
     from girder.settings import SettingKey
 
     receiver = MockSmtpReceiver()
     receiver.start()
 
     host, port = receiver.address
```

### Comparing `pytest-girder-3.2.4.dev7/pytest_girder/plugin.py` & `pytest_girder-5a2/pytest_girder/plugin.py`

 * *Files identical despite different names*

### Comparing `pytest-girder-3.2.4.dev7/pytest_girder/plugin_registry.py` & `pytest_girder-5a2/pytest_girder/plugin_registry.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,7 +77,8 @@
         try:
             with unittest.mock.patch.object(
                     plugin, 'iter_entry_points', side_effect=self._iter_entry_points) as mock_:
                 yield mock_
         finally:
             plugin._pluginRegistry = None
             plugin._pluginLoadOrder = []
+            plugin._pluginStaticContent.clear()
```

### Comparing `pytest-girder-3.2.4.dev7/pytest_girder/utils.py` & `pytest_girder-5a2/pytest_girder/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 import base64
 import cherrypy
 import contextlib
+from dataclasses import dataclass
 import email
 import errno
 import io
 import json
 import os
 import queue
 import socket
 import threading
 import time
+from typing import Optional
 import urllib.parse
 
 _startPort = 31000
 _maxTries = 100
 
 
 class MockSmtpReceiver:
@@ -133,15 +135,15 @@
     return data
 
 
 def request(path='/', method='GET', params=None, user=None,
             prefix='/api/v1', isJson=True, basicAuth=None, body=None,
             type=None, exception=False, cookie=None, token=None,
             additionalHeaders=None, useHttps=False,
-            authHeader='Authorization', appPrefix=''):
+            authHeader='Authorization', appPrefix='/api'):
     """
     Make an HTTP request.
 
     :param path: The path part of the URI.
     :type path: str
     :param method: The HTTP method.
     :type method: str
@@ -290,51 +292,58 @@
 
 def _findFreePort():
     with contextlib.closing(socket.socket(socket.AF_INET, socket.SOCK_STREAM)) as sock:
         sock.bind(('', 0))
         return sock.getsockname()[1]
 
 
+@dataclass
+class ServerFixture:
+    request = staticmethod(request)
+    uploadFile = staticmethod(uploadFile)
+    serverRoot: cherrypy._cptree.Tree
+    boundPort: Optional[int] = None
+
+    def __getattr__(self, name):
+        return getattr(self.serverRoot, name)
+
+
 @contextlib.contextmanager
-def serverContext(plugins=None, bindPort=False):
-    # The event daemon cannot be restarted since it is a threading.Thread
-    # object, however all references to girder.events.daemon are a singular
-    # global daemon due to its side effect on import. We have to hack around
-    # this by creating a unique event daemon each time we startup the server
-    # and assigning it to the global.
-    import girder.events
+def serverContext(plugins=None, bindPort=False) -> ServerFixture:
+    from girder import plugin
     from girder.api import docs
-    from girder.utility.server import setup as setupServer
+    from girder.utility.server import create_app
     from girder.constants import ServerMode
 
-    girder.events.daemon = girder.events.AsyncEventsThread()
-
     if plugins is None:
         # By default, pass "[]" to "plugins", disabling any installed plugins
         plugins = []
-    server = setupServer(mode=ServerMode.TESTING, plugins=plugins)
-    server.request = request
-    server.uploadFile = uploadFile
+    app_info = create_app(mode=ServerMode.TESTING)
+    plugin._loadPlugins(app_info, plugins)
+
+    server_fixture = ServerFixture(serverRoot=app_info['serverRoot'])
+
+    cherrypy.tree = app_info['serverRoot']
     cherrypy.server.unsubscribe()
     if bindPort:
         cherrypy.server.subscribe()
         port = _findFreePort()
         cherrypy.config['server.socket_port'] = port
-        server.boundPort = port
+        server_fixture.boundPort = port
         # This is needed if cherrypy started once on another port
         cherrypy.server.socket_port = port
-    cherrypy.config.update({'environment': 'embedded',
-                            'log.screen': False,
-                            'request.throw_errors': True})
+    cherrypy.config.update({
+        'environment': 'embedded',
+        'log.screen': False,
+        'request.throw_errors': True
+    })
     cherrypy.engine.start()
 
     try:
-        yield server
+        yield server_fixture
     finally:
-        cherrypy.engine.unsubscribe('start', girder.events.daemon.start)
-        cherrypy.engine.unsubscribe('stop', girder.events.daemon.stop)
         cherrypy.engine.stop()
         cherrypy.engine.exit()
         cherrypy.tree.apps = {}
         # This is needed to allow cherrypy to restart on another port
         cherrypy.server.httpserver = None
         docs.routes.clear()
```

### Comparing `pytest-girder-3.2.4.dev7/pytest_girder/web_client.py` & `pytest_girder-5a2/pytest_girder/web_client.py`

 * *Files identical despite different names*

### Comparing `pytest-girder-3.2.4.dev7/setup.py` & `pytest_girder-5a2/setup.py`

 * *Files identical despite different names*


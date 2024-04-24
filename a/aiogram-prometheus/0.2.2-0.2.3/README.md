# Comparing `tmp/aiogram_prometheus-0.2.2.tar.gz` & `tmp/aiogram_prometheus-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiogram_prometheus-0.2.2.tar", max compression
+gzip compressed data, was "aiogram_prometheus-0.2.3.tar", max compression
```

## Comparing `aiogram_prometheus-0.2.2.tar` & `aiogram_prometheus-0.2.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1056 2024-04-06 12:49:37.028835 aiogram_prometheus-0.2.2/LICENSE
--rw-r--r--   0        0        0      432 2024-04-06 12:49:37.028835 aiogram_prometheus-0.2.2/aiogram_prometheus/__init__.py
--rw-r--r--   0        0        0      465 2024-04-06 12:49:37.028835 aiogram_prometheus-0.2.2/aiogram_prometheus/collectors/__init__.py
--rw-r--r--   0        0        0     1194 2024-04-06 12:49:37.028835 aiogram_prometheus-0.2.2/aiogram_prometheus/collectors/asyncio_loop.py
--rw-r--r--   0        0        0      512 2024-04-06 12:49:37.028835 aiogram_prometheus-0.2.2/aiogram_prometheus/collectors/base.py
--rw-r--r--   0        0        0     3393 2024-04-06 12:49:37.028835 aiogram_prometheus-0.2.2/aiogram_prometheus/collectors/bot.py
--rw-r--r--   0        0        0     5159 2024-04-06 12:49:37.028835 aiogram_prometheus-0.2.2/aiogram_prometheus/collectors/dispatcher.py
--rw-r--r--   0        0        0     1149 2024-04-06 12:49:37.032835 aiogram_prometheus-0.2.2/aiogram_prometheus/collectors/push_clients.py
--rw-r--r--   0        0        0     4475 2024-04-06 12:49:37.032835 aiogram_prometheus-0.2.2/aiogram_prometheus/collectors/storages.py
--rw-r--r--   0        0        0     3283 2024-04-06 12:49:37.032835 aiogram_prometheus-0.2.2/aiogram_prometheus/middlewares.py
--rw-r--r--   0        0        0      170 2024-04-06 12:49:37.032835 aiogram_prometheus-0.2.2/aiogram_prometheus/push_clients/__init__.py
--rw-r--r--   0        0        0     2212 2024-04-06 12:49:37.032835 aiogram_prometheus-0.2.2/aiogram_prometheus/push_clients/base.py
--rw-r--r--   0        0        0     2461 2024-04-06 12:49:37.032835 aiogram_prometheus-0.2.2/aiogram_prometheus/push_clients/pushgateway.py
--rw-r--r--   0        0        0      163 2024-04-06 12:49:37.032835 aiogram_prometheus-0.2.2/aiogram_prometheus/push_clients/statsd.py
--rw-r--r--   0        0        0     1442 2024-04-06 12:49:37.032835 aiogram_prometheus-0.2.2/aiogram_prometheus/storages.py
--rw-r--r--   0        0        0     2549 2024-04-06 12:49:37.032835 aiogram_prometheus-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     6308 2024-04-06 12:49:37.032835 aiogram_prometheus-0.2.2/readme.md
--rw-r--r--   0        0        0     7566 1970-01-01 00:00:00.000000 aiogram_prometheus-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1056 2024-04-24 14:51:29.584302 aiogram_prometheus-0.2.3/LICENSE
+-rw-r--r--   0        0        0      432 2024-04-24 14:51:29.584302 aiogram_prometheus-0.2.3/aiogram_prometheus/__init__.py
+-rw-r--r--   0        0        0      465 2024-04-24 14:51:29.584302 aiogram_prometheus-0.2.3/aiogram_prometheus/collectors/__init__.py
+-rw-r--r--   0        0        0     1194 2024-04-24 14:51:29.584302 aiogram_prometheus-0.2.3/aiogram_prometheus/collectors/asyncio_loop.py
+-rw-r--r--   0        0        0      512 2024-04-24 14:51:29.584302 aiogram_prometheus-0.2.3/aiogram_prometheus/collectors/base.py
+-rw-r--r--   0        0        0     3393 2024-04-24 14:51:29.584302 aiogram_prometheus-0.2.3/aiogram_prometheus/collectors/bot.py
+-rw-r--r--   0        0        0     5159 2024-04-24 14:51:29.584302 aiogram_prometheus-0.2.3/aiogram_prometheus/collectors/dispatcher.py
+-rw-r--r--   0        0        0     1149 2024-04-24 14:51:29.588302 aiogram_prometheus-0.2.3/aiogram_prometheus/collectors/push_clients.py
+-rw-r--r--   0        0        0     4475 2024-04-24 14:51:29.588302 aiogram_prometheus-0.2.3/aiogram_prometheus/collectors/storages.py
+-rw-r--r--   0        0        0     3283 2024-04-24 14:51:29.588302 aiogram_prometheus-0.2.3/aiogram_prometheus/middlewares.py
+-rw-r--r--   0        0        0      170 2024-04-24 14:51:29.588302 aiogram_prometheus-0.2.3/aiogram_prometheus/push_clients/__init__.py
+-rw-r--r--   0        0        0     2212 2024-04-24 14:51:29.588302 aiogram_prometheus-0.2.3/aiogram_prometheus/push_clients/base.py
+-rw-r--r--   0        0        0     2461 2024-04-24 14:51:29.588302 aiogram_prometheus-0.2.3/aiogram_prometheus/push_clients/pushgateway.py
+-rw-r--r--   0        0        0      163 2024-04-24 14:51:29.588302 aiogram_prometheus-0.2.3/aiogram_prometheus/push_clients/statsd.py
+-rw-r--r--   0        0        0     1442 2024-04-24 14:51:29.588302 aiogram_prometheus-0.2.3/aiogram_prometheus/storages.py
+-rw-r--r--   0        0        0     2549 2024-04-24 14:51:29.588302 aiogram_prometheus-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     6600 2024-04-24 14:51:29.588302 aiogram_prometheus-0.2.3/readme.md
+-rw-r--r--   0        0        0     7858 1970-01-01 00:00:00.000000 aiogram_prometheus-0.2.3/PKG-INFO
```

### Comparing `aiogram_prometheus-0.2.2/LICENSE` & `aiogram_prometheus-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `aiogram_prometheus-0.2.2/aiogram_prometheus/collectors/asyncio_loop.py` & `aiogram_prometheus-0.2.3/aiogram_prometheus/collectors/asyncio_loop.py`

 * *Files identical despite different names*

### Comparing `aiogram_prometheus-0.2.2/aiogram_prometheus/collectors/base.py` & `aiogram_prometheus-0.2.3/aiogram_prometheus/collectors/base.py`

 * *Files identical despite different names*

### Comparing `aiogram_prometheus-0.2.2/aiogram_prometheus/collectors/bot.py` & `aiogram_prometheus-0.2.3/aiogram_prometheus/collectors/bot.py`

 * *Files identical despite different names*

### Comparing `aiogram_prometheus-0.2.2/aiogram_prometheus/collectors/dispatcher.py` & `aiogram_prometheus-0.2.3/aiogram_prometheus/collectors/dispatcher.py`

 * *Files identical despite different names*

### Comparing `aiogram_prometheus-0.2.2/aiogram_prometheus/collectors/push_clients.py` & `aiogram_prometheus-0.2.3/aiogram_prometheus/collectors/push_clients.py`

 * *Files identical despite different names*

### Comparing `aiogram_prometheus-0.2.2/aiogram_prometheus/collectors/storages.py` & `aiogram_prometheus-0.2.3/aiogram_prometheus/collectors/storages.py`

 * *Files identical despite different names*

### Comparing `aiogram_prometheus-0.2.2/aiogram_prometheus/middlewares.py` & `aiogram_prometheus-0.2.3/aiogram_prometheus/middlewares.py`

 * *Files identical despite different names*

### Comparing `aiogram_prometheus-0.2.2/aiogram_prometheus/push_clients/base.py` & `aiogram_prometheus-0.2.3/aiogram_prometheus/push_clients/base.py`

 * *Files identical despite different names*

### Comparing `aiogram_prometheus-0.2.2/aiogram_prometheus/push_clients/pushgateway.py` & `aiogram_prometheus-0.2.3/aiogram_prometheus/push_clients/pushgateway.py`

 * *Files identical despite different names*

### Comparing `aiogram_prometheus-0.2.2/aiogram_prometheus/storages.py` & `aiogram_prometheus-0.2.3/aiogram_prometheus/storages.py`

 * *Files identical despite different names*

### Comparing `aiogram_prometheus-0.2.2/pyproject.toml` & `aiogram_prometheus-0.2.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aiogram_prometheus-0.2.2/readme.md` & `aiogram_prometheus-0.2.3/readme.md`

 * *Files 3% similar despite different names*

```diff
@@ -7,14 +7,22 @@
 [![GitLab last commit](https://img.shields.io/gitlab/last-commit/rocshers/python/aiogram-prometheus)](https://gitlab.com/rocshers/python/aiogram-prometheus)
 [![Docs](https://img.shields.io/badge/docs-exist-blue)](https://rocshers.gitlab.io/python/aiogram-prometheus/)
 
 [![Test coverage](https://codecov.io/gitlab/rocshers:python/aiogram-prometheus/graph/badge.svg?token=3C6SLDPHUC)](https://codecov.io/gitlab/rocshers:python/aiogram-prometheus)
 [![Downloads](https://static.pepy.tech/badge/aiogram-prometheus)](https://pepy.tech/project/aiogram-prometheus)
 [![GitLab stars](https://img.shields.io/gitlab/stars/rocshers/python/aiogram-prometheus)](https://gitlab.com/rocshers/python/aiogram-prometheus)
 
+## Functionality
+
+- Monitoring the `status` of bots and dispatchers
+- Middleware for monitoring the bot's `network activity`
+- Middleware for monitoring the `event handler performance`
+
+![example](https://gitlab.com/rocshers/python/aiogram-prometheus/-/raw/release/docs/grafana_example.png)
+
 ## Installation
 
 `pip install aiogram-prometheus`
 
 ## Quick start
 
 - **aiogram.BotAiogramCollector** - base `info` abut started bot
```

### Comparing `aiogram_prometheus-0.2.2/PKG-INFO` & `aiogram_prometheus-0.2.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiogram-prometheus
-Version: 0.2.2
+Version: 0.2.3
 Summary: Aiogram`s exporter for Prometheus
 Home-page: https://gitlab.com/rocshers/python/aiogram-prometheus
 License: MIT
 Author: aleksei.marusich
 Author-email: aleksei.marusich@rocshers.com
 Requires-Python: >=3.8,<4.0
 Classifier: Intended Audience :: Developers
@@ -36,14 +36,22 @@
 [![GitLab last commit](https://img.shields.io/gitlab/last-commit/rocshers/python/aiogram-prometheus)](https://gitlab.com/rocshers/python/aiogram-prometheus)
 [![Docs](https://img.shields.io/badge/docs-exist-blue)](https://rocshers.gitlab.io/python/aiogram-prometheus/)
 
 [![Test coverage](https://codecov.io/gitlab/rocshers:python/aiogram-prometheus/graph/badge.svg?token=3C6SLDPHUC)](https://codecov.io/gitlab/rocshers:python/aiogram-prometheus)
 [![Downloads](https://static.pepy.tech/badge/aiogram-prometheus)](https://pepy.tech/project/aiogram-prometheus)
 [![GitLab stars](https://img.shields.io/gitlab/stars/rocshers/python/aiogram-prometheus)](https://gitlab.com/rocshers/python/aiogram-prometheus)
 
+## Functionality
+
+- Monitoring the `status` of bots and dispatchers
+- Middleware for monitoring the bot's `network activity`
+- Middleware for monitoring the `event handler performance`
+
+![example](https://gitlab.com/rocshers/python/aiogram-prometheus/-/raw/release/docs/grafana_example.png)
+
 ## Installation
 
 `pip install aiogram-prometheus`
 
 ## Quick start
 
 - **aiogram.BotAiogramCollector** - base `info` abut started bot
```


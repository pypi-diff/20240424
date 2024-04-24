# Comparing `tmp/rabbitmqpubsub-1.0.0.tar.gz` & `tmp/rabbitmqpubsub-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rabbitmqpubsub-1.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "rabbitmqpubsub-1.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `rabbitmqpubsub-1.0.0.tar` & `rabbitmqpubsub-1.1.0.tar`

### file list

```diff
@@ -1,16 +1,17 @@
--rw-r--r--   0        0        0       91 2024-04-10 13:50:13.487352 rabbitmqpubsub-1.0.0/.flake8
--rw-r--r--   0        0        0     1788 2024-04-10 13:46:48.785995 rabbitmqpubsub-1.0.0/.gitignore
--rw-r--r--   0        0        0      366 2024-04-10 14:01:51.989415 rabbitmqpubsub-1.0.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0    11358 2024-04-10 13:46:48.785995 rabbitmqpubsub-1.0.0/LICENSE
--rw-r--r--   0        0        0     1120 2024-04-10 14:18:02.791439 rabbitmqpubsub-1.0.0/README.md
--rw-r--r--   0        0        0      305 2024-04-10 13:58:19.819388 rabbitmqpubsub-1.0.0/docker-compose.yml
--rw-r--r--   0        0        0      881 2024-04-10 13:59:16.827921 rabbitmqpubsub-1.0.0/pyproject.toml
--rw-r--r--   0        0        0       60 2024-04-10 13:57:24.170875 rabbitmqpubsub-1.0.0/rabbitmqpubsub/__init__.py
--rw-r--r--   0        0        0      154 2024-04-10 14:13:43.388697 rabbitmqpubsub-1.0.0/rabbitmqpubsub/rabbit_pubsub/__init__.py
--rw-r--r--   0        0        0     2320 2024-04-10 14:01:34.797247 rabbitmqpubsub-1.0.0/rabbitmqpubsub/rabbit_pubsub/publisher.py
--rw-r--r--   0        0        0     4515 2024-04-10 13:49:47.275172 rabbitmqpubsub-1.0.0/rabbitmqpubsub/rabbit_pubsub/rpcclient.py
--rw-r--r--   0        0        0    16256 2024-04-10 14:01:34.941248 rabbitmqpubsub-1.0.0/rabbitmqpubsub/rabbit_pubsub/subscriber.py
--rw-r--r--   0        0        0      532 2024-04-10 13:46:48.785995 rabbitmqpubsub-1.0.0/rabbitmqpubsub/rabbit_pubsub/utils.py
--rw-r--r--   0        0        0        0 2024-04-10 13:46:48.785995 rabbitmqpubsub-1.0.0/rabbitmqpubsub/tests/__init__.py
--rw-r--r--   0        0        0     2669 2024-04-10 14:01:34.813247 rabbitmqpubsub-1.0.0/rabbitmqpubsub/tests/test_subscriber.py
--rw-r--r--   0        0        0     1759 1970-01-01 00:00:00.000000 rabbitmqpubsub-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0       91 2024-04-10 13:50:13.487352 rabbitmqpubsub-1.1.0/.flake8
+-rw-r--r--   0        0        0     1788 2024-04-10 13:46:48.785995 rabbitmqpubsub-1.1.0/.gitignore
+-rw-r--r--   0        0        0      366 2024-04-10 14:01:51.989415 rabbitmqpubsub-1.1.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    11358 2024-04-10 13:46:48.785995 rabbitmqpubsub-1.1.0/LICENSE
+-rw-r--r--   0        0        0     1120 2024-04-10 14:18:02.791439 rabbitmqpubsub-1.1.0/README.md
+-rw-r--r--   0        0        0      305 2024-04-10 13:58:19.819388 rabbitmqpubsub-1.1.0/docker-compose.yml
+-rw-r--r--   0        0        0      855 2024-04-24 10:08:28.878612 rabbitmqpubsub-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0       60 2024-04-24 10:09:32.375147 rabbitmqpubsub-1.1.0/rabbitmqpubsub/__init__.py
+-rw-r--r--   0        0        0      211 2024-04-24 10:06:04.989480 rabbitmqpubsub-1.1.0/rabbitmqpubsub/rabbit_pubsub/__init__.py
+-rw-r--r--   0        0        0     3728 2024-04-24 10:09:16.483012 rabbitmqpubsub-1.1.0/rabbitmqpubsub/rabbit_pubsub/arpcclient.py
+-rw-r--r--   0        0        0     2320 2024-04-10 14:01:34.797247 rabbitmqpubsub-1.1.0/rabbitmqpubsub/rabbit_pubsub/publisher.py
+-rw-r--r--   0        0        0     4515 2024-04-10 13:49:47.275172 rabbitmqpubsub-1.1.0/rabbitmqpubsub/rabbit_pubsub/rpcclient.py
+-rw-r--r--   0        0        0    16256 2024-04-10 14:01:34.941248 rabbitmqpubsub-1.1.0/rabbitmqpubsub/rabbit_pubsub/subscriber.py
+-rw-r--r--   0        0        0      532 2024-04-10 13:46:48.785995 rabbitmqpubsub-1.1.0/rabbitmqpubsub/rabbit_pubsub/utils.py
+-rw-r--r--   0        0        0        0 2024-04-10 13:46:48.785995 rabbitmqpubsub-1.1.0/rabbitmqpubsub/tests/__init__.py
+-rw-r--r--   0        0        0     2669 2024-04-10 14:01:34.813247 rabbitmqpubsub-1.1.0/rabbitmqpubsub/tests/test_subscriber.py
+-rw-r--r--   0        0        0     1793 1970-01-01 00:00:00.000000 rabbitmqpubsub-1.1.0/PKG-INFO
```

### Comparing `rabbitmqpubsub-1.0.0/.gitignore` & `rabbitmqpubsub-1.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `rabbitmqpubsub-1.0.0/LICENSE` & `rabbitmqpubsub-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rabbitmqpubsub-1.0.0/README.md` & `rabbitmqpubsub-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `rabbitmqpubsub-1.0.0/pyproject.toml` & `rabbitmqpubsub-1.1.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "RabbitMQPubSub"
 authors = [{ name = "Nebojsa Mrkic", email = "mrkic.nebojsa@gmail.com" }]
 readme = "README.md"
 license = { file = "LICENSE" }
-classifiers = ["License :: OSI Approved :: MIT License"]
+classifiers = ['License :: OSI Approved :: Apache Software License']
 dynamic = ["version", "description"]
-dependencies = ["pika>=1.3.0", "dateutils"]
+dependencies = ["pika>=1.3.0", "dateutils", "aiormq"]
 
 [tool.flit.module]
 name = "rabbitmqpubsub"
 
 [project.urls]
 Home = "https://github.com/nmrkic/RabbitMQPubSub"
 
@@ -23,17 +23,14 @@
     "mock",
     "requests",
     "pytest-runner",
     "pre-commit",
     "pytest-mock",
 ]
 
-[tool.setuptools]
-packages = ["rabbit_pubsub"]
-
 [tool.coverage.run]
 source = ["./rabbit_pubsub"]
 
 [tool.coverage.report]
 fail_under = 80
 show_missing = true
 exclude_lines = ["pragma: no cover"]
```

### Comparing `rabbitmqpubsub-1.0.0/rabbitmqpubsub/rabbit_pubsub/publisher.py` & `rabbitmqpubsub-1.1.0/rabbitmqpubsub/rabbit_pubsub/publisher.py`

 * *Files identical despite different names*

### Comparing `rabbitmqpubsub-1.0.0/rabbitmqpubsub/rabbit_pubsub/rpcclient.py` & `rabbitmqpubsub-1.1.0/rabbitmqpubsub/rabbit_pubsub/rpcclient.py`

 * *Files identical despite different names*

### Comparing `rabbitmqpubsub-1.0.0/rabbitmqpubsub/rabbit_pubsub/subscriber.py` & `rabbitmqpubsub-1.1.0/rabbitmqpubsub/rabbit_pubsub/subscriber.py`

 * *Files identical despite different names*

### Comparing `rabbitmqpubsub-1.0.0/rabbitmqpubsub/rabbit_pubsub/utils.py` & `rabbitmqpubsub-1.1.0/rabbitmqpubsub/rabbit_pubsub/utils.py`

 * *Files identical despite different names*

### Comparing `rabbitmqpubsub-1.0.0/rabbitmqpubsub/tests/test_subscriber.py` & `rabbitmqpubsub-1.1.0/rabbitmqpubsub/tests/test_subscriber.py`

 * *Files identical despite different names*

### Comparing `rabbitmqpubsub-1.0.0/PKG-INFO` & `rabbitmqpubsub-1.1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: RabbitMQPubSub
-Version: 1.0.0
+Version: 1.1.0
 Summary: RabbitMQ helpers for pubsub.
 Author-email: Nebojsa Mrkic <mrkic.nebojsa@gmail.com>
 Description-Content-Type: text/markdown
-Classifier: License :: OSI Approved :: MIT License
+Classifier: License :: OSI Approved :: Apache Software License
 Requires-Dist: pika>=1.3.0
 Requires-Dist: dateutils
+Requires-Dist: aiormq
 Requires-Dist: pytest ; extra == "tests"
 Requires-Dist: mock ; extra == "tests"
 Requires-Dist: requests ; extra == "tests"
 Requires-Dist: pytest-runner ; extra == "tests"
 Requires-Dist: pre-commit ; extra == "tests"
 Requires-Dist: pytest-mock ; extra == "tests"
 Project-URL: Home, https://github.com/nmrkic/RabbitMQPubSub
```


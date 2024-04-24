# Comparing `tmp/dalpha-0.4.4rc4.tar.gz` & `tmp/dalpha-0.4.4rc5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dalpha-0.4.4rc4.tar", max compression
+gzip compressed data, was "dalpha-0.4.4rc5.tar", max compression
```

## Comparing `dalpha-0.4.4rc4.tar` & `dalpha-0.4.4rc5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      578 2023-12-18 04:10:26.318635 dalpha-0.4.4rc4/README.md
--rw-r--r--   0        0        0    30584 2024-04-22 06:41:31.414519 dalpha-0.4.4rc4/dalpha/__init__.py
--rw-r--r--   0        0        0      548 2024-04-19 16:22:01.493908 dalpha-0.4.4rc4/dalpha/cobra_cls.py
--rw-r--r--   0        0        0      573 2024-02-28 08:10:55.063883 dalpha-0.4.4rc4/dalpha/context.py
--rw-r--r--   0        0        0     1716 2024-02-28 08:10:55.063883 dalpha-0.4.4rc4/dalpha/dalpha_openai.py
--rw-r--r--   0        0        0      178 2024-04-22 06:41:31.414519 dalpha-0.4.4rc4/dalpha/error_code.py
--rw-r--r--   0        0        0      233 2024-03-25 02:37:47.094337 dalpha-0.4.4rc4/dalpha/kafka_cli.py
--rw-r--r--   0        0        0     1861 2024-03-11 02:52:37.986799 dalpha-0.4.4rc4/dalpha/logging/__init__.py
--rw-r--r--   0        0        0      229 2024-02-28 08:10:55.063883 dalpha-0.4.4rc4/dalpha/logging/events.py
--rw-r--r--   0        0        0     1116 2024-02-28 08:10:55.063883 dalpha-0.4.4rc4/dalpha/logging/log_formatter.py
--rw-r--r--   0        0        0     1817 2024-02-28 08:10:55.063883 dalpha-0.4.4rc4/dalpha/logging/utils.py
--rw-r--r--   0        0        0     5846 2024-03-06 10:11:38.540030 dalpha-0.4.4rc4/dalpha/redis.py
--rw-r--r--   0        0        0      497 2024-02-28 08:10:55.063883 dalpha-0.4.4rc4/dalpha/signal_handler.py
--rw-r--r--   0        0        0      881 2024-04-22 10:58:21.608774 dalpha-0.4.4rc4/pyproject.toml
--rw-r--r--   0        0        0     1321 1970-01-01 00:00:00.000000 dalpha-0.4.4rc4/PKG-INFO
+-rw-r--r--   0        0        0      578 2023-12-18 04:10:26.318635 dalpha-0.4.4rc5/README.md
+-rw-r--r--   0        0        0    30518 2024-04-22 12:19:21.276903 dalpha-0.4.4rc5/dalpha/__init__.py
+-rw-r--r--   0        0        0      548 2024-04-19 16:22:01.493908 dalpha-0.4.4rc5/dalpha/cobra_cls.py
+-rw-r--r--   0        0        0      573 2024-02-28 08:10:55.063883 dalpha-0.4.4rc5/dalpha/context.py
+-rw-r--r--   0        0        0     1716 2024-02-28 08:10:55.063883 dalpha-0.4.4rc5/dalpha/dalpha_openai.py
+-rw-r--r--   0        0        0      178 2024-04-22 06:41:31.414519 dalpha-0.4.4rc5/dalpha/error_code.py
+-rw-r--r--   0        0        0      233 2024-03-25 02:37:47.094337 dalpha-0.4.4rc5/dalpha/kafka_cli.py
+-rw-r--r--   0        0        0     1861 2024-03-11 02:52:37.986799 dalpha-0.4.4rc5/dalpha/logging/__init__.py
+-rw-r--r--   0        0        0      229 2024-02-28 08:10:55.063883 dalpha-0.4.4rc5/dalpha/logging/events.py
+-rw-r--r--   0        0        0     1116 2024-02-28 08:10:55.063883 dalpha-0.4.4rc5/dalpha/logging/log_formatter.py
+-rw-r--r--   0        0        0     1817 2024-02-28 08:10:55.063883 dalpha-0.4.4rc5/dalpha/logging/utils.py
+-rw-r--r--   0        0        0     5846 2024-03-06 10:11:38.540030 dalpha-0.4.4rc5/dalpha/redis.py
+-rw-r--r--   0        0        0      497 2024-02-28 08:10:55.063883 dalpha-0.4.4rc5/dalpha/signal_handler.py
+-rw-r--r--   0        0        0      881 2024-04-22 12:19:21.276903 dalpha-0.4.4rc5/pyproject.toml
+-rw-r--r--   0        0        0     1321 1970-01-01 00:00:00.000000 dalpha-0.4.4rc5/PKG-INFO
```

### Comparing `dalpha-0.4.4rc4/README.md` & `dalpha-0.4.4rc5/README.md`

 * *Files identical despite different names*

### Comparing `dalpha-0.4.4rc4/dalpha/__init__.py` & `dalpha-0.4.4rc5/dalpha/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -177,16 +177,14 @@
         self.mock = {}
         self.s3 = boto3.client('s3')
 
         # default
         self.use_kafka = False
         self.use_sqs = False
 
-        self.kafka_topic = None
-        self.update_record = None
         if use_kafka:  # 우선순위 1. kafka
             from dalpha.kafka_cli import get_consumer
 
             if self.queue_url is None:
                 logger.warning("kafka topic is not set")
                 raise ValueError("kafka topic is not set")
```

### Comparing `dalpha-0.4.4rc4/dalpha/cobra_cls.py` & `dalpha-0.4.4rc5/dalpha/cobra_cls.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.4.4rc4/dalpha/context.py` & `dalpha-0.4.4rc5/dalpha/context.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.4.4rc4/dalpha/dalpha_openai.py` & `dalpha-0.4.4rc5/dalpha/dalpha_openai.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.4.4rc4/dalpha/logging/__init__.py` & `dalpha-0.4.4rc5/dalpha/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.4.4rc4/dalpha/logging/log_formatter.py` & `dalpha-0.4.4rc5/dalpha/logging/log_formatter.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.4.4rc4/dalpha/logging/utils.py` & `dalpha-0.4.4rc5/dalpha/logging/utils.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.4.4rc4/dalpha/redis.py` & `dalpha-0.4.4rc5/dalpha/redis.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.4.4rc4/pyproject.toml` & `dalpha-0.4.4rc5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dalpha"
-version = "0.4.4rc4"
+version = "0.4.4rc5"
 description = ""
 authors = ["devops <devops@dalpha.so>"]
 readme = "README.md"
 packages = [{include = "dalpha"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
@@ -16,15 +16,15 @@
 kafka-python = "^2.0.2"
 
 [tool.poetry.group.dev.dependencies]
 twine = "^4.0.2"
 
 [project]
 name = "dalpha"
-version = "0.4.4rc4"
+version = "0.4.4rc5"
 authors = [
   { name="Beomseok", email="beomseok.lee@dalpha.so" },
 ]
 description = "Dalpha internal sdk"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `dalpha-0.4.4rc4/PKG-INFO` & `dalpha-0.4.4rc5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dalpha
-Version: 0.4.4rc4
+Version: 0.4.4rc5
 Summary: 
 Author: devops
 Author-email: devops@dalpha.so
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```


# Comparing `tmp/amqpstorm_flask-0.4.3.tar.gz` & `tmp/amqpstorm_flask-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amqpstorm_flask-0.4.3.tar", last modified: Tue Apr 23 14:45:53 2024, max compression
+gzip compressed data, was "amqpstorm_flask-0.4.4.tar", last modified: Wed Apr 24 13:51:49 2024, max compression
```

## Comparing `amqpstorm_flask-0.4.3.tar` & `amqpstorm_flask-0.4.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:45:53.780392 amqpstorm_flask-0.4.3/
--rw-r--r--   0 runner    (1001) docker     (127)    18092 2024-04-23 14:45:49.000000 amqpstorm_flask-0.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    22647 2024-04-23 14:45:53.780392 amqpstorm_flask-0.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-04-23 14:45:49.000000 amqpstorm_flask-0.4.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      741 2024-04-23 14:45:49.000000 amqpstorm_flask-0.4.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 14:45:53.780392 amqpstorm_flask-0.4.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:45:53.780392 amqpstorm_flask-0.4.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:45:53.780392 amqpstorm_flask-0.4.3/src/amqpstorm_flask/
--rw-r--r--   0 runner    (1001) docker     (127)     9638 2024-04-23 14:45:49.000000 amqpstorm_flask-0.4.3/src/amqpstorm_flask/RabbitMQ.py
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-23 14:45:49.000000 amqpstorm_flask-0.4.3/src/amqpstorm_flask/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-23 14:45:49.000000 amqpstorm_flask-0.4.3/src/amqpstorm_flask/exchange_params.py
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-23 14:45:49.000000 amqpstorm_flask-0.4.3/src/amqpstorm_flask/queue_params.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:45:53.780392 amqpstorm_flask-0.4.3/src/amqpstorm_flask.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    22647 2024-04-23 14:45:53.000000 amqpstorm_flask-0.4.3/src/amqpstorm_flask.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-23 14:45:53.000000 amqpstorm_flask-0.4.3/src/amqpstorm_flask.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 14:45:53.000000 amqpstorm_flask-0.4.3/src/amqpstorm_flask.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 14:45:53.000000 amqpstorm_flask-0.4.3/src/amqpstorm_flask.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-23 14:45:53.000000 amqpstorm_flask-0.4.3/src/amqpstorm_flask.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:51:49.722328 amqpstorm_flask-0.4.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    18092 2024-04-24 13:51:40.000000 amqpstorm_flask-0.4.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    22647 2024-04-24 13:51:49.722328 amqpstorm_flask-0.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-04-24 13:51:40.000000 amqpstorm_flask-0.4.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-04-24 13:51:40.000000 amqpstorm_flask-0.4.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 13:51:49.722328 amqpstorm_flask-0.4.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:51:49.718328 amqpstorm_flask-0.4.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:51:49.718328 amqpstorm_flask-0.4.4/src/amqpstorm_flask/
+-rw-r--r--   0 runner    (1001) docker     (127)     9461 2024-04-24 13:51:40.000000 amqpstorm_flask-0.4.4/src/amqpstorm_flask/RabbitMQ.py
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-24 13:51:40.000000 amqpstorm_flask-0.4.4/src/amqpstorm_flask/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-24 13:51:40.000000 amqpstorm_flask-0.4.4/src/amqpstorm_flask/exchange_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-24 13:51:40.000000 amqpstorm_flask-0.4.4/src/amqpstorm_flask/queue_params.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:51:49.722328 amqpstorm_flask-0.4.4/src/amqpstorm_flask.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    22647 2024-04-24 13:51:49.000000 amqpstorm_flask-0.4.4/src/amqpstorm_flask.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-24 13:51:49.000000 amqpstorm_flask-0.4.4/src/amqpstorm_flask.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 13:51:49.000000 amqpstorm_flask-0.4.4/src/amqpstorm_flask.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 13:51:49.000000 amqpstorm_flask-0.4.4/src/amqpstorm_flask.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-24 13:51:49.000000 amqpstorm_flask-0.4.4/src/amqpstorm_flask.egg-info/top_level.txt
```

### Comparing `amqpstorm_flask-0.4.3/LICENSE` & `amqpstorm_flask-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `amqpstorm_flask-0.4.3/PKG-INFO` & `amqpstorm_flask-0.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amqpstorm-flask
-Version: 0.4.3
+Version: 0.4.4
 Summary: amqpstorm library for Flask
 Author-email: Inuits <developers@inuits.eu>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 2, June 1991
         
          Copyright (C) 1989, 1991 Free Software Foundation, Inc.,
          51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA
```

### Comparing `amqpstorm_flask-0.4.3/README.md` & `amqpstorm_flask-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `amqpstorm_flask-0.4.3/pyproject.toml` & `amqpstorm_flask-0.4.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=59.6.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "amqpstorm-flask"
-version = "0.4.3"
+version = "0.4.4"
 description = "amqpstorm library for Flask"
 readme = "README.md"
 authors = [{ name = "Inuits", email = "developers@inuits.eu" }]
 license = { file = "LICENSE" }
 classifiers = [
   "License :: OSI Approved :: GNU General Public License v2 (GPLv2)",
   "Intended Audience :: Developers",
```

### Comparing `amqpstorm_flask-0.4.3/src/amqpstorm_flask/RabbitMQ.py` & `amqpstorm_flask-0.4.4/src/amqpstorm_flask/RabbitMQ.py`

 * *Files 5% similar despite different names*

```diff
@@ -65,18 +65,15 @@
         self.body_parser = body_parser
         self.msg_parser = msg_parser
         self.json_encoder = json_encoder
         self._validate_channel_connection()
 
     def check_health(self, check_consumers=True):
         if not self.get_connection().is_open:
-            # try to recover connection before failing the health check
-            self._validate_channel_connection(0.1)
-            if not self.get_connection().is_open:
-                return False, "Connection not open"
+            return False, "Connection not open"
         if check_consumers and len(self.channel.consumer_tags) < 1:
             return False, "No consumers available"
         return True, "Connection open"
 
     def get_connection(self):
         return self.connection
```

### Comparing `amqpstorm_flask-0.4.3/src/amqpstorm_flask.egg-info/PKG-INFO` & `amqpstorm_flask-0.4.4/src/amqpstorm_flask.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amqpstorm-flask
-Version: 0.4.3
+Version: 0.4.4
 Summary: amqpstorm library for Flask
 Author-email: Inuits <developers@inuits.eu>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 2, June 1991
         
          Copyright (C) 1989, 1991 Free Software Foundation, Inc.,
          51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA
```


# Comparing `tmp/aixblock_ml-0.0.7.tar.gz` & `tmp/aixblock_ml-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aixblock_ml-0.0.7.tar", max compression
+gzip compressed data, was "aixblock_ml-0.0.8.tar", max compression
```

## Comparing `aixblock_ml-0.0.7.tar` & `aixblock_ml-0.0.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      348 2024-04-15 02:52:58.946494 aixblock_ml-0.0.7/README.md
--rw-r--r--   0        0        0       84 2024-04-04 08:01:18.783734 aixblock_ml-0.0.7/aixblock_ml/__init__.py
--rw-r--r--   0        0        0    10484 2024-04-15 02:31:16.790340 aixblock_ml-0.0.7/aixblock_ml/api.py
--rw-r--r--   0        0        0      267 2024-04-01 06:20:49.118665 aixblock_ml-0.0.7/aixblock_ml/default_configs/Dockerfile
--rw-r--r--   0        0        0     2686 2024-04-15 02:26:57.535131 aixblock_ml-0.0.7/aixblock_ml/default_configs/README.md
--rw-r--r--   0        0        0     3854 2024-04-04 03:08:16.490661 aixblock_ml-0.0.7/aixblock_ml/default_configs/_wsgi.py
--rw-r--r--   0        0        0     3854 2024-04-04 03:08:16.489309 aixblock_ml-0.0.7/aixblock_ml/default_configs/_wsgi.py.tmpl
--rw-r--r--   0        0        0      559 2024-04-03 08:23:03.374688 aixblock_ml-0.0.7/aixblock_ml/default_configs/docker-compose.yml
--rw-r--r--   0        0        0     2129 2024-04-15 02:26:57.535807 aixblock_ml-0.0.7/aixblock_ml/default_configs/model.py
--rw-r--r--   0        0        0       90 2024-04-01 06:20:49.122796 aixblock_ml-0.0.7/aixblock_ml/default_configs/requirements.txt
--rw-r--r--   0        0        0     1899 2024-04-01 06:20:49.123299 aixblock_ml-0.0.7/aixblock_ml/exceptions.py
--rw-r--r--   0        0        0     2357 2024-04-01 06:43:06.660882 aixblock_ml-0.0.7/aixblock_ml/helpers.py
--rw-r--r--   0        0        0    35732 2024-04-15 02:32:53.891767 aixblock_ml-0.0.7/aixblock_ml/model.py
--rw-r--r--   0        0        0     7477 2024-04-15 02:26:57.534982 aixblock_ml-0.0.7/aixblock_ml/server.py
--rw-r--r--   0        0        0        6 2024-04-01 06:20:49.127187 aixblock_ml-0.0.7/aixblock_ml/templates/preview.html
--rw-r--r--   0        0        0     1987 2024-04-03 08:23:03.033057 aixblock_ml-0.0.7/aixblock_ml/utils.py
--rw-r--r--   0        0        0      325 2024-04-15 07:16:15.841753 aixblock_ml-0.0.7/pyproject.toml
--rw-r--r--   0        0        0      731 1970-01-01 00:00:00.000000 aixblock_ml-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0      341 2024-04-16 16:09:41.363976 aixblock_ml-0.0.8/README.md
+-rw-r--r--   0        0        0       84 2024-04-04 08:01:18.783734 aixblock_ml-0.0.8/aixblock_ml/__init__.py
+-rw-r--r--   0        0        0    10484 2024-04-15 02:31:16.790340 aixblock_ml-0.0.8/aixblock_ml/api.py
+-rw-r--r--   0        0        0      267 2024-04-01 06:20:49.118665 aixblock_ml-0.0.8/aixblock_ml/default_configs/Dockerfile
+-rw-r--r--   0        0        0     2686 2024-04-15 02:26:57.535131 aixblock_ml-0.0.8/aixblock_ml/default_configs/README.md
+-rw-r--r--   0        0        0     3854 2024-04-04 03:08:16.490661 aixblock_ml-0.0.8/aixblock_ml/default_configs/_wsgi.py
+-rw-r--r--   0        0        0     3854 2024-04-04 03:08:16.489309 aixblock_ml-0.0.8/aixblock_ml/default_configs/_wsgi.py.tmpl
+-rw-r--r--   0        0        0      559 2024-04-03 08:23:03.374688 aixblock_ml-0.0.8/aixblock_ml/default_configs/docker-compose.yml
+-rw-r--r--   0        0        0     2129 2024-04-15 02:26:57.535807 aixblock_ml-0.0.8/aixblock_ml/default_configs/model.py
+-rw-r--r--   0        0        0       90 2024-04-01 06:20:49.122796 aixblock_ml-0.0.8/aixblock_ml/default_configs/requirements.txt
+-rw-r--r--   0        0        0     1899 2024-04-01 06:20:49.123299 aixblock_ml-0.0.8/aixblock_ml/exceptions.py
+-rw-r--r--   0        0        0     2357 2024-04-01 06:43:06.660882 aixblock_ml-0.0.8/aixblock_ml/helpers.py
+-rw-r--r--   0        0        0    35738 2024-04-24 07:46:56.510948 aixblock_ml-0.0.8/aixblock_ml/model.py
+-rw-r--r--   0        0        0     7477 2024-04-15 02:26:57.534982 aixblock_ml-0.0.8/aixblock_ml/server.py
+-rw-r--r--   0        0        0        6 2024-04-01 06:20:49.127187 aixblock_ml-0.0.8/aixblock_ml/templates/preview.html
+-rw-r--r--   0        0        0     1987 2024-04-03 08:23:03.033057 aixblock_ml-0.0.8/aixblock_ml/utils.py
+-rw-r--r--   0        0        0      325 2024-04-16 16:09:32.277425 aixblock_ml-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0      724 1970-01-01 00:00:00.000000 aixblock_ml-0.0.8/PKG-INFO
```

### Comparing `aixblock_ml-0.0.7/aixblock_ml/api.py` & `aixblock_ml-0.0.8/aixblock_ml/api.py`

 * *Files identical despite different names*

### Comparing `aixblock_ml-0.0.7/aixblock_ml/default_configs/README.md` & `aixblock_ml-0.0.8/aixblock_ml/default_configs/README.md`

 * *Files identical despite different names*

### Comparing `aixblock_ml-0.0.7/aixblock_ml/default_configs/_wsgi.py` & `aixblock_ml-0.0.8/aixblock_ml/default_configs/_wsgi.py`

 * *Files identical despite different names*

### Comparing `aixblock_ml-0.0.7/aixblock_ml/default_configs/_wsgi.py.tmpl` & `aixblock_ml-0.0.8/aixblock_ml/default_configs/_wsgi.py.tmpl`

 * *Files identical despite different names*

### Comparing `aixblock_ml-0.0.7/aixblock_ml/default_configs/docker-compose.yml` & `aixblock_ml-0.0.8/aixblock_ml/default_configs/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `aixblock_ml-0.0.7/aixblock_ml/default_configs/model.py` & `aixblock_ml-0.0.8/aixblock_ml/default_configs/model.py`

 * *Files identical despite different names*

### Comparing `aixblock_ml-0.0.7/aixblock_ml/exceptions.py` & `aixblock_ml-0.0.8/aixblock_ml/exceptions.py`

 * *Files identical despite different names*

### Comparing `aixblock_ml-0.0.7/aixblock_ml/helpers.py` & `aixblock_ml-0.0.8/aixblock_ml/helpers.py`

 * *Files identical despite different names*

### Comparing `aixblock_ml-0.0.7/aixblock_ml/model.py` & `aixblock_ml-0.0.8/aixblock_ml/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -688,15 +688,15 @@
         if not os.getenv('AIXBLOCK_ML_BACKEND_V2', default=AIXBLOCK_ML_BACKEND_V2_DEFAULT):
             if try_fetch:
                 m = cls.fetch(project, label_config, force_reload)
             else:
                 m = cls.get(project)
                 if not m:
                     raise FileNotFoundError('No model loaded. Specify "try_fetch=True" option.')
-            predictions = m.model.model(project, **kwargs)
+            predictions = m.model.model_trial(project, **kwargs)
             return predictions, m
 
         if not cls._current_model:
             raise ValueError(f'Model is not loaded for {cls.__class__.__name__}: run setup() before using model()')
         predictions = m.model.model(project, **kwargs)
         return predictions, m
     # @classmethod
```

### Comparing `aixblock_ml-0.0.7/aixblock_ml/server.py` & `aixblock_ml-0.0.8/aixblock_ml/server.py`

 * *Files identical despite different names*

### Comparing `aixblock_ml-0.0.7/aixblock_ml/utils.py` & `aixblock_ml-0.0.8/aixblock_ml/utils.py`

 * *Files identical despite different names*

### Comparing `aixblock_ml-0.0.7/PKG-INFO` & `aixblock_ml-0.0.8/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aixblock_ml
-Version: 0.0.7
+Version: 0.0.8
 Summary: 
 Author: TonyShark
 Author-email: quoi@wow-ai.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -16,9 +16,9 @@
 aixblock-ml create my_ml_backend
 aixblock-ml start my_ml_backend
 aixblock-ml start my_ml_backend -p 9091
 
 aixblock-ml deploy gcp {ml-backend-local-dir} \
 --from={model-python-script} \
 --gcp-project-id {gcp-project-id} \
---label-studio-host {https://app.heartex.com} \
---label-studio-api-key {YOUR-LABEL-STUDIO-API-KEY}
+--label-studio-host {https://aixblock.org} \
+--label-studio-api-key {YOUR-AIXBLOCK-API-KEY}
```


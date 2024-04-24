# Comparing `tmp/wonder-diffusion-sdk-0.0.4.dev1.tar.gz` & `tmp/wonder-diffusion-sdk-0.0.4.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wonder-diffusion-sdk-0.0.4.dev1.tar", last modified: Fri Apr 19 07:13:35 2024, max compression
+gzip compressed data, was "wonder-diffusion-sdk-0.0.4.dev2.tar", last modified: Wed Apr 24 10:00:54 2024, max compression
```

## Comparing `wonder-diffusion-sdk-0.0.4.dev1.tar` & `wonder-diffusion-sdk-0.0.4.dev2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 basri      (501) staff       (20)        0 2024-04-19 07:13:35.760731 wonder-diffusion-sdk-0.0.4.dev1/
--rw-r--r--   0 basri      (501) staff       (20)     1080 2024-01-31 06:15:26.000000 wonder-diffusion-sdk-0.0.4.dev1/LICENCE
--rw-r--r--   0 basri      (501) staff       (20)      190 2024-04-19 07:13:35.760555 wonder-diffusion-sdk-0.0.4.dev1/PKG-INFO
--rw-r--r--   0 basri      (501) staff       (20)       38 2024-04-19 07:13:35.760889 wonder-diffusion-sdk-0.0.4.dev1/setup.cfg
--rw-r--r--   0 basri      (501) staff       (20)      319 2024-04-19 07:12:53.000000 wonder-diffusion-sdk-0.0.4.dev1/setup.py
-drwxr-xr-x   0 basri      (501) staff       (20)        0 2024-04-19 07:13:35.754094 wonder-diffusion-sdk-0.0.4.dev1/wonder_diffusion_sdk/
--rw-r--r--   0 basri      (501) staff       (20)    10595 2024-04-19 07:12:53.000000 wonder-diffusion-sdk-0.0.4.dev1/wonder_diffusion_sdk/__init__.py
-drwxr-xr-x   0 basri      (501) staff       (20)        0 2024-04-19 07:13:35.756757 wonder-diffusion-sdk-0.0.4.dev1/wonder_diffusion_sdk/components/
--rw-r--r--   0 basri      (501) staff       (20)      199 2024-03-22 14:04:45.000000 wonder-diffusion-sdk-0.0.4.dev1/wonder_diffusion_sdk/components/__init__.py
--rw-r--r--   0 basri      (501) staff       (20)      402 2024-03-22 14:04:23.000000 wonder-diffusion-sdk-0.0.4.dev1/wonder_diffusion_sdk/components/deepcache.py
--rw-r--r--   0 basri      (501) staff       (20)      117 2024-02-28 08:41:39.000000 wonder-diffusion-sdk-0.0.4.dev1/wonder_diffusion_sdk/components/dotdict.py
--rw-r--r--   0 basri      (501) staff       (20)      914 2024-04-17 08:38:18.000000 wonder-diffusion-sdk-0.0.4.dev1/wonder_diffusion_sdk/components/lightning.py
--rw-r--r--   0 basri      (501) staff       (20)     1137 2024-03-11 09:11:53.000000 wonder-diffusion-sdk-0.0.4.dev1/wonder_diffusion_sdk/components/logger.py
--rw-r--r--   0 basri      (501) staff       (20)     3207 2024-02-27 13:23:11.000000 wonder-diffusion-sdk-0.0.4.dev1/wonder_diffusion_sdk/components/safety_checker.py
-drwxr-xr-x   0 basri      (501) staff       (20)        0 2024-04-19 07:13:35.758331 wonder-diffusion-sdk-0.0.4.dev1/wonder_diffusion_sdk/config/
--rw-r--r--   0 basri      (501) staff       (20)      183 2024-04-17 12:15:34.000000 wonder-diffusion-sdk-0.0.4.dev1/wonder_diffusion_sdk/config/__init__.py
--rw-r--r--   0 basri      (501) staff       (20)       70 2024-03-20 09:12:50.000000 wonder-diffusion-sdk-0.0.4.dev1/wonder_diffusion_sdk/config/globals.py
--rw-r--r--   0 basri      (501) staff       (20)      996 2024-04-19 07:12:53.000000 wonder-diffusion-sdk-0.0.4.dev1/wonder_diffusion_sdk/config/lora_config.py
--rw-r--r--   0 basri      (501) staff       (20)     1503 2024-03-22 14:14:11.000000 wonder-diffusion-sdk-0.0.4.dev1/wonder_diffusion_sdk/config/model_config.py
--rw-r--r--   0 basri      (501) staff       (20)      197 2024-03-22 14:06:09.000000 wonder-diffusion-sdk-0.0.4.dev1/wonder_diffusion_sdk/config/sdk_config.py
-drwxr-xr-x   0 basri      (501) staff       (20)        0 2024-04-19 07:13:35.759969 wonder-diffusion-sdk-0.0.4.dev1/wonder_diffusion_sdk/types/
--rw-r--r--   0 basri      (501) staff       (20)      167 2024-03-11 10:04:17.000000 wonder-diffusion-sdk-0.0.4.dev1/wonder_diffusion_sdk/types/__init__.py
--rw-r--r--   0 basri      (501) staff       (20)      465 2024-04-17 12:15:34.000000 wonder-diffusion-sdk-0.0.4.dev1/wonder_diffusion_sdk/types/pipeline_type.py
--rw-r--r--   0 basri      (501) staff       (20)     2526 2024-04-03 11:08:09.000000 wonder-diffusion-sdk-0.0.4.dev1/wonder_diffusion_sdk/types/pipelines.py
--rw-r--r--   0 basri      (501) staff       (20)      815 2024-03-12 10:17:49.000000 wonder-diffusion-sdk-0.0.4.dev1/wonder_diffusion_sdk/types/scheduler_type.py
--rw-r--r--   0 basri      (501) staff       (20)     3174 2024-03-22 13:38:15.000000 wonder-diffusion-sdk-0.0.4.dev1/wonder_diffusion_sdk/types/schedulers.py
-drwxr-xr-x   0 basri      (501) staff       (20)        0 2024-04-19 07:13:35.754969 wonder-diffusion-sdk-0.0.4.dev1/wonder_diffusion_sdk.egg-info/
--rw-r--r--   0 basri      (501) staff       (20)      190 2024-04-19 07:13:35.000000 wonder-diffusion-sdk-0.0.4.dev1/wonder_diffusion_sdk.egg-info/PKG-INFO
--rw-r--r--   0 basri      (501) staff       (20)      954 2024-04-19 07:13:35.000000 wonder-diffusion-sdk-0.0.4.dev1/wonder_diffusion_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 basri      (501) staff       (20)        1 2024-04-19 07:13:35.000000 wonder-diffusion-sdk-0.0.4.dev1/wonder_diffusion_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 basri      (501) staff       (20)       18 2024-04-19 07:13:35.000000 wonder-diffusion-sdk-0.0.4.dev1/wonder_diffusion_sdk.egg-info/requires.txt
--rw-r--r--   0 basri      (501) staff       (20)       21 2024-04-19 07:13:35.000000 wonder-diffusion-sdk-0.0.4.dev1/wonder_diffusion_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 basri      (501) staff       (20)        0 2024-04-24 10:00:54.713578 wonder-diffusion-sdk-0.0.4.dev2/
+-rw-r--r--   0 basri      (501) staff       (20)     1080 2024-01-31 06:15:26.000000 wonder-diffusion-sdk-0.0.4.dev2/LICENCE
+-rw-r--r--   0 basri      (501) staff       (20)      190 2024-04-24 10:00:54.713422 wonder-diffusion-sdk-0.0.4.dev2/PKG-INFO
+-rw-r--r--   0 basri      (501) staff       (20)       38 2024-04-24 10:00:54.713637 wonder-diffusion-sdk-0.0.4.dev2/setup.cfg
+-rw-r--r--   0 basri      (501) staff       (20)      319 2024-04-24 10:00:26.000000 wonder-diffusion-sdk-0.0.4.dev2/setup.py
+drwxr-xr-x   0 basri      (501) staff       (20)        0 2024-04-24 10:00:54.710093 wonder-diffusion-sdk-0.0.4.dev2/wonder_diffusion_sdk/
+-rw-r--r--   0 basri      (501) staff       (20)    10651 2024-04-24 10:00:12.000000 wonder-diffusion-sdk-0.0.4.dev2/wonder_diffusion_sdk/__init__.py
+drwxr-xr-x   0 basri      (501) staff       (20)        0 2024-04-24 10:00:54.711698 wonder-diffusion-sdk-0.0.4.dev2/wonder_diffusion_sdk/components/
+-rw-r--r--   0 basri      (501) staff       (20)      199 2024-03-22 14:04:45.000000 wonder-diffusion-sdk-0.0.4.dev2/wonder_diffusion_sdk/components/__init__.py
+-rw-r--r--   0 basri      (501) staff       (20)      402 2024-03-22 14:04:23.000000 wonder-diffusion-sdk-0.0.4.dev2/wonder_diffusion_sdk/components/deepcache.py
+-rw-r--r--   0 basri      (501) staff       (20)      117 2024-02-28 08:41:39.000000 wonder-diffusion-sdk-0.0.4.dev2/wonder_diffusion_sdk/components/dotdict.py
+-rw-r--r--   0 basri      (501) staff       (20)      914 2024-04-17 08:38:18.000000 wonder-diffusion-sdk-0.0.4.dev2/wonder_diffusion_sdk/components/lightning.py
+-rw-r--r--   0 basri      (501) staff       (20)     1137 2024-03-11 09:11:53.000000 wonder-diffusion-sdk-0.0.4.dev2/wonder_diffusion_sdk/components/logger.py
+-rw-r--r--   0 basri      (501) staff       (20)     3207 2024-02-27 13:23:11.000000 wonder-diffusion-sdk-0.0.4.dev2/wonder_diffusion_sdk/components/safety_checker.py
+drwxr-xr-x   0 basri      (501) staff       (20)        0 2024-04-24 10:00:54.712304 wonder-diffusion-sdk-0.0.4.dev2/wonder_diffusion_sdk/config/
+-rw-r--r--   0 basri      (501) staff       (20)      183 2024-04-17 12:15:34.000000 wonder-diffusion-sdk-0.0.4.dev2/wonder_diffusion_sdk/config/__init__.py
+-rw-r--r--   0 basri      (501) staff       (20)       70 2024-03-20 09:12:50.000000 wonder-diffusion-sdk-0.0.4.dev2/wonder_diffusion_sdk/config/globals.py
+-rw-r--r--   0 basri      (501) staff       (20)     1182 2024-04-24 10:00:12.000000 wonder-diffusion-sdk-0.0.4.dev2/wonder_diffusion_sdk/config/lora_config.py
+-rw-r--r--   0 basri      (501) staff       (20)     1503 2024-03-22 14:14:11.000000 wonder-diffusion-sdk-0.0.4.dev2/wonder_diffusion_sdk/config/model_config.py
+-rw-r--r--   0 basri      (501) staff       (20)      197 2024-03-22 14:06:09.000000 wonder-diffusion-sdk-0.0.4.dev2/wonder_diffusion_sdk/config/sdk_config.py
+drwxr-xr-x   0 basri      (501) staff       (20)        0 2024-04-24 10:00:54.713186 wonder-diffusion-sdk-0.0.4.dev2/wonder_diffusion_sdk/types/
+-rw-r--r--   0 basri      (501) staff       (20)      167 2024-03-11 10:04:17.000000 wonder-diffusion-sdk-0.0.4.dev2/wonder_diffusion_sdk/types/__init__.py
+-rw-r--r--   0 basri      (501) staff       (20)      465 2024-04-17 12:15:34.000000 wonder-diffusion-sdk-0.0.4.dev2/wonder_diffusion_sdk/types/pipeline_type.py
+-rw-r--r--   0 basri      (501) staff       (20)     2526 2024-04-03 11:08:09.000000 wonder-diffusion-sdk-0.0.4.dev2/wonder_diffusion_sdk/types/pipelines.py
+-rw-r--r--   0 basri      (501) staff       (20)      815 2024-03-12 10:17:49.000000 wonder-diffusion-sdk-0.0.4.dev2/wonder_diffusion_sdk/types/scheduler_type.py
+-rw-r--r--   0 basri      (501) staff       (20)     3174 2024-03-22 13:38:15.000000 wonder-diffusion-sdk-0.0.4.dev2/wonder_diffusion_sdk/types/schedulers.py
+drwxr-xr-x   0 basri      (501) staff       (20)        0 2024-04-24 10:00:54.710977 wonder-diffusion-sdk-0.0.4.dev2/wonder_diffusion_sdk.egg-info/
+-rw-r--r--   0 basri      (501) staff       (20)      190 2024-04-24 10:00:54.000000 wonder-diffusion-sdk-0.0.4.dev2/wonder_diffusion_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 basri      (501) staff       (20)      954 2024-04-24 10:00:54.000000 wonder-diffusion-sdk-0.0.4.dev2/wonder_diffusion_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 basri      (501) staff       (20)        1 2024-04-24 10:00:54.000000 wonder-diffusion-sdk-0.0.4.dev2/wonder_diffusion_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 basri      (501) staff       (20)       18 2024-04-24 10:00:54.000000 wonder-diffusion-sdk-0.0.4.dev2/wonder_diffusion_sdk.egg-info/requires.txt
+-rw-r--r--   0 basri      (501) staff       (20)       21 2024-04-24 10:00:54.000000 wonder-diffusion-sdk-0.0.4.dev2/wonder_diffusion_sdk.egg-info/top_level.txt
```

### Comparing `wonder-diffusion-sdk-0.0.4.dev1/LICENCE` & `wonder-diffusion-sdk-0.0.4.dev2/LICENCE`

 * *Files identical despite different names*

### Comparing `wonder-diffusion-sdk-0.0.4.dev1/wonder_diffusion_sdk/__init__.py` & `wonder-diffusion-sdk-0.0.4.dev2/wonder_diffusion_sdk/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -276,13 +276,14 @@
         combined_adapter = adapters[0]
         for i in range(1, len(adapters)):
             combined_adapter += f'_{adapters[i]}'
 
         model.add_weighted_adapter(
             adapters=adapters,
             weights=adapter_weights,
-            combination_type="dare_linear",
-            adapter_name=combined_adapter
+            adapter_name=combined_adapter,
+            combination_type=config.peft_combination_type,
+            density=config.peft_density
         )
         model.set_adapters(combined_adapter)
 
         pipeline.unet = model
```

### Comparing `wonder-diffusion-sdk-0.0.4.dev1/wonder_diffusion_sdk/components/lightning.py` & `wonder-diffusion-sdk-0.0.4.dev2/wonder_diffusion_sdk/components/lightning.py`

 * *Files identical despite different names*

### Comparing `wonder-diffusion-sdk-0.0.4.dev1/wonder_diffusion_sdk/components/logger.py` & `wonder-diffusion-sdk-0.0.4.dev2/wonder_diffusion_sdk/components/logger.py`

 * *Files identical despite different names*

### Comparing `wonder-diffusion-sdk-0.0.4.dev1/wonder_diffusion_sdk/components/safety_checker.py` & `wonder-diffusion-sdk-0.0.4.dev2/wonder_diffusion_sdk/components/safety_checker.py`

 * *Files identical despite different names*

### Comparing `wonder-diffusion-sdk-0.0.4.dev1/wonder_diffusion_sdk/config/lora_config.py` & `wonder-diffusion-sdk-0.0.4.dev2/wonder_diffusion_sdk/config/lora_config.py`

 * *Files 12% similar despite different names*

```diff
@@ -30,10 +30,14 @@
     NOTES:
         - When using peft, both Loras must have the same `base_model_name_or_path`.
     """
     def __init__(
         self,
         loras: list[WonderLora] = [],
         use_peft: bool = False,
+        peft_combination_type: str = "dare_linear",
+        peft_density: float = 0.5
     ):
         self.loras = loras
         self.use_peft = use_peft
+        self.peft_combination_type = peft_combination_type
+        self.peft_density = peft_density
```

### Comparing `wonder-diffusion-sdk-0.0.4.dev1/wonder_diffusion_sdk/config/model_config.py` & `wonder-diffusion-sdk-0.0.4.dev2/wonder_diffusion_sdk/config/model_config.py`

 * *Files identical despite different names*

### Comparing `wonder-diffusion-sdk-0.0.4.dev1/wonder_diffusion_sdk/types/pipelines.py` & `wonder-diffusion-sdk-0.0.4.dev2/wonder_diffusion_sdk/types/pipelines.py`

 * *Files identical despite different names*

### Comparing `wonder-diffusion-sdk-0.0.4.dev1/wonder_diffusion_sdk/types/scheduler_type.py` & `wonder-diffusion-sdk-0.0.4.dev2/wonder_diffusion_sdk/types/scheduler_type.py`

 * *Files identical despite different names*

### Comparing `wonder-diffusion-sdk-0.0.4.dev1/wonder_diffusion_sdk/types/schedulers.py` & `wonder-diffusion-sdk-0.0.4.dev2/wonder_diffusion_sdk/types/schedulers.py`

 * *Files identical despite different names*

### Comparing `wonder-diffusion-sdk-0.0.4.dev1/wonder_diffusion_sdk.egg-info/SOURCES.txt` & `wonder-diffusion-sdk-0.0.4.dev2/wonder_diffusion_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*


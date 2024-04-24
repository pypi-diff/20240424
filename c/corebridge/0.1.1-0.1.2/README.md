# Comparing `tmp/corebridge-0.1.1.tar.gz` & `tmp/corebridge-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "corebridge-0.1.1.tar", last modified: Mon Apr 22 08:18:29 2024, max compression
+gzip compressed data, was "corebridge-0.1.2.tar", last modified: Wed Apr 24 15:21:05 2024, max compression
```

## Comparing `corebridge-0.1.1.tar` & `corebridge-0.1.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 fenke     (1000) users      (100)        0 2024-04-22 08:18:29.386892 corebridge-0.1.1/
--rw-r--r--   0 fenke     (1000) users      (100)    11337 2024-01-31 12:54:47.000000 corebridge-0.1.1/LICENSE
--rw-r--r--   0 fenke     (1000) users      (100)      111 2024-01-31 12:54:47.000000 corebridge-0.1.1/MANIFEST.in
--rw-r--r--   0 fenke     (1000) users      (100)     1203 2024-04-22 08:18:29.386892 corebridge-0.1.1/PKG-INFO
--rw-r--r--   0 fenke     (1000) users      (100)      435 2024-04-17 14:51:56.000000 corebridge-0.1.1/README.md
-drwxr-xr-x   0 fenke     (1000) users      (100)        0 2024-04-22 08:18:29.386892 corebridge-0.1.1/corebridge/
--rw-r--r--   0 fenke     (1000) users      (100)       22 2024-04-22 08:18:10.000000 corebridge-0.1.1/corebridge/__init__.py
--rw-r--r--   0 fenke     (1000) users      (100)     3300 2024-04-22 08:18:10.000000 corebridge-0.1.1/corebridge/_modidx.py
--rw-r--r--   0 fenke     (1000) users      (100)     8155 2024-04-22 08:18:10.000000 corebridge-0.1.1/corebridge/aicorebridge.py
--rw-r--r--   0 fenke     (1000) users      (100)     3766 2024-04-22 08:18:10.000000 corebridge-0.1.1/corebridge/core.py
-drwxr-xr-x   0 fenke     (1000) users      (100)        0 2024-04-22 08:18:29.386892 corebridge-0.1.1/corebridge.egg-info/
--rw-r--r--   0 fenke     (1000) users      (100)     1203 2024-04-22 08:18:29.000000 corebridge-0.1.1/corebridge.egg-info/PKG-INFO
--rw-r--r--   0 fenke     (1000) users      (100)      381 2024-04-22 08:18:29.000000 corebridge-0.1.1/corebridge.egg-info/SOURCES.txt
--rw-r--r--   0 fenke     (1000) users      (100)        1 2024-04-22 08:18:29.000000 corebridge-0.1.1/corebridge.egg-info/dependency_links.txt
--rw-r--r--   0 fenke     (1000) users      (100)       42 2024-04-22 08:18:29.000000 corebridge-0.1.1/corebridge.egg-info/entry_points.txt
--rw-r--r--   0 fenke     (1000) users      (100)        1 2024-01-31 15:42:47.000000 corebridge-0.1.1/corebridge.egg-info/not-zip-safe
--rw-r--r--   0 fenke     (1000) users      (100)      225 2024-04-22 08:18:29.000000 corebridge-0.1.1/corebridge.egg-info/requires.txt
--rw-r--r--   0 fenke     (1000) users      (100)       11 2024-04-22 08:18:29.000000 corebridge-0.1.1/corebridge.egg-info/top_level.txt
--rw-r--r--   0 fenke     (1000) users      (100)     1146 2024-04-22 08:17:53.000000 corebridge-0.1.1/settings.ini
--rw-r--r--   0 fenke     (1000) users      (100)       38 2024-04-22 08:18:29.386892 corebridge-0.1.1/setup.cfg
--rw-r--r--   0 fenke     (1000) users      (100)     2596 2024-01-31 12:54:47.000000 corebridge-0.1.1/setup.py
+drwxr-xr-x   0 fenke     (1000) users      (100)        0 2024-04-24 15:21:05.401792 corebridge-0.1.2/
+-rw-r--r--   0 fenke     (1000) users      (100)    11337 2024-01-31 12:54:47.000000 corebridge-0.1.2/LICENSE
+-rw-r--r--   0 fenke     (1000) users      (100)      111 2024-01-31 12:54:47.000000 corebridge-0.1.2/MANIFEST.in
+-rw-r--r--   0 fenke     (1000) users      (100)     1203 2024-04-24 15:21:05.401792 corebridge-0.1.2/PKG-INFO
+-rw-r--r--   0 fenke     (1000) users      (100)      435 2024-04-17 14:51:56.000000 corebridge-0.1.2/README.md
+drwxr-xr-x   0 fenke     (1000) users      (100)        0 2024-04-24 15:21:05.401792 corebridge-0.1.2/corebridge/
+-rw-r--r--   0 fenke     (1000) users      (100)       22 2024-04-24 15:20:58.000000 corebridge-0.1.2/corebridge/__init__.py
+-rw-r--r--   0 fenke     (1000) users      (100)     3300 2024-04-24 15:20:58.000000 corebridge-0.1.2/corebridge/_modidx.py
+-rw-r--r--   0 fenke     (1000) users      (100)     8419 2024-04-24 15:20:58.000000 corebridge-0.1.2/corebridge/aicorebridge.py
+-rw-r--r--   0 fenke     (1000) users      (100)     3766 2024-04-24 15:20:58.000000 corebridge-0.1.2/corebridge/core.py
+drwxr-xr-x   0 fenke     (1000) users      (100)        0 2024-04-24 15:21:05.401792 corebridge-0.1.2/corebridge.egg-info/
+-rw-r--r--   0 fenke     (1000) users      (100)     1203 2024-04-24 15:21:05.000000 corebridge-0.1.2/corebridge.egg-info/PKG-INFO
+-rw-r--r--   0 fenke     (1000) users      (100)      381 2024-04-24 15:21:05.000000 corebridge-0.1.2/corebridge.egg-info/SOURCES.txt
+-rw-r--r--   0 fenke     (1000) users      (100)        1 2024-04-24 15:21:05.000000 corebridge-0.1.2/corebridge.egg-info/dependency_links.txt
+-rw-r--r--   0 fenke     (1000) users      (100)       42 2024-04-24 15:21:05.000000 corebridge-0.1.2/corebridge.egg-info/entry_points.txt
+-rw-r--r--   0 fenke     (1000) users      (100)        1 2024-01-31 15:42:47.000000 corebridge-0.1.2/corebridge.egg-info/not-zip-safe
+-rw-r--r--   0 fenke     (1000) users      (100)      225 2024-04-24 15:21:05.000000 corebridge-0.1.2/corebridge.egg-info/requires.txt
+-rw-r--r--   0 fenke     (1000) users      (100)       11 2024-04-24 15:21:05.000000 corebridge-0.1.2/corebridge.egg-info/top_level.txt
+-rw-r--r--   0 fenke     (1000) users      (100)     1146 2024-04-24 15:14:23.000000 corebridge-0.1.2/settings.ini
+-rw-r--r--   0 fenke     (1000) users      (100)       38 2024-04-24 15:21:05.401792 corebridge-0.1.2/setup.cfg
+-rw-r--r--   0 fenke     (1000) users      (100)     2596 2024-01-31 12:54:47.000000 corebridge-0.1.2/setup.py
```

### Comparing `corebridge-0.1.1/LICENSE` & `corebridge-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `corebridge-0.1.1/PKG-INFO` & `corebridge-0.1.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: corebridge
-Version: 0.1.1
+Version: 0.1.2
 Summary: Bridge for Stactics AICore
 Home-page: https://github.com/fenke/corebridge
 Author: Fenke Meijer
 Author-email: fenkemeijer@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `corebridge-0.1.1/corebridge/_modidx.py` & `corebridge-0.1.2/corebridge/_modidx.py`

 * *Files identical despite different names*

### Comparing `corebridge-0.1.1/corebridge/aicorebridge.py` & `corebridge-0.1.2/corebridge/aicorebridge.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 # %% auto 0
 __all__ = ['syslog', 'AICoreModule']
 
 # %% ../nbs/01_aicorebridge.ipynb 2
 import typing
 import logging
 import inspect
+import traceback
 import datetime
 import json
 import pandas as pd
 import numpy as np
 
 from fastcore.basics import patch_to, patch
 
@@ -32,15 +33,15 @@
              *args, **kwargs):
     
     self.save_dir  = save_dir
     self.assets_dir  = assets_dir
     self._init_processor(processor)
 
     self.init_args = args
-    self.init_kwargs = kwargs
+    self.init_kwargs = {k:v for k,v in kwargs.items() if v is not None}
 
 
 
 # %% ../nbs/01_aicorebridge.ipynb 8
 @patch
 def _init_processor(
         self:AICoreModule, 
@@ -59,14 +60,15 @@
 def call_processor(self:AICoreModule, calldata, **callargs):
     return self.processor(calldata, **callargs)
 
 
 # %% ../nbs/01_aicorebridge.ipynb 10
 @patch
 def infer(self:AICoreModule, data:dict, *_, **kwargs):
+    msg=[]
     try:
 
         msg=[
             f"{self.processor.__name__}({self.processor_signature})",
             f"init_args: {self.init_args}, init_kwargs: {self.init_kwargs}",
         ]
 
@@ -96,17 +98,20 @@
             'msg':msg,
             'data': self.rewrite_data(
                 result if not lastSeen else result[-1:],
                 recordformat=recordformat,
                 timezone=timezone,
                 reversed=reversed)
         }
+
     except Exception as err:
+        msg.append(''.join(traceback.format_exception(None, err, err.__traceback__)))
+        syslog.exception(f"Exception {str(err)} in infer()")
         return {
-            'msg': f"Unexpected {err=}, {type(err)=}",
+            'msg': msg,
             'data': []
         }
 
 
 # %% ../nbs/01_aicorebridge.ipynb 11
 @patch
 def get_callargs(self:AICoreModule, **kwargs):
@@ -188,16 +193,15 @@
 
     if orient == 'split-index':
         orient = 'split'
 
     normalized_data = self.convert_to_dataframe(data, timezone=timezone)
     normalized_data.index = normalized_data.index.map(lambda x: x.isoformat())
     
-    if reversed:
-        normalized_data = normalized_data[::-1]
+    normalized_data.sort_index(ascending=not bool(reversed), inplace=True)
 
     if orient == 'records':
         records = normalized_data.reset_index().to_dict(orient='records')
     else:
         records =  normalized_data.to_dict(orient=orient)
     
 
@@ -248,14 +252,15 @@
                 data=adata[:, 1:],
                 index=pd.DatetimeIndex(adata[:,0]*1e9),
                 columns=columns
             )
         else:
             return pd.DataFrame()
 
-    df.index.name = 'time'
-    if not df.index.tz:
-        df.index = df.index.tz_localize('UTC').tz_convert(timezone)
-    elif str(df.index.tz) != timezone:
-        df.index = df.index.tz_convert(timezone)
+    if isinstance(df.index, pd.DatetimeIndex):
+        df.index.name = 'time'
+        if not df.index.tz:
+            df.index = df.index.tz_localize('UTC').tz_convert(timezone)
+        elif str(df.index.tz) != timezone:
+            df.index = df.index.tz_convert(timezone)
 
     return df
```

### Comparing `corebridge-0.1.1/corebridge/core.py` & `corebridge-0.1.2/corebridge/core.py`

 * *Files identical despite different names*

### Comparing `corebridge-0.1.1/corebridge.egg-info/PKG-INFO` & `corebridge-0.1.2/corebridge.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: corebridge
-Version: 0.1.1
+Version: 0.1.2
 Summary: Bridge for Stactics AICore
 Home-page: https://github.com/fenke/corebridge
 Author: Fenke Meijer
 Author-email: fenkemeijer@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `corebridge-0.1.1/settings.ini` & `corebridge-0.1.2/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = corebridge
 lib_name = %(repo)s
-version = 0.1.1
+version = 0.1.2
 min_python = 3.7
 license = apache2
 black_formatting = False
 
 ### nbdev ###
 doc_path = _docs
 lib_path = corebridge
```

### Comparing `corebridge-0.1.1/setup.py` & `corebridge-0.1.2/setup.py`

 * *Files identical despite different names*


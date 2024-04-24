# Comparing `tmp/klu-0.1.8.tar.gz` & `tmp/klu-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "klu-0.1.8.tar", max compression
+gzip compressed data, was "klu-0.1.9.tar", max compression
```

## Comparing `klu-0.1.8.tar` & `klu-0.1.9.tar`

### file list

```diff
@@ -1,59 +1,59 @@
--rw-r--r--   0        0        0     1070 2023-07-08 22:55:36.156770 klu-0.1.8/LICENSE
--rw-r--r--   0        0        0     2840 2023-07-08 22:55:36.156770 klu-0.1.8/README.md
--rw-r--r--   0        0        0      150 2023-07-08 22:55:36.156770 klu-0.1.8/klu/__init__.py
--rw-r--r--   0        0        0        0 2023-07-08 22:55:36.156770 klu-0.1.8/klu/action/__init__.py
--rw-r--r--   0        0        0    11398 2023-07-08 22:55:36.156770 klu-0.1.8/klu/action/client.py
--rw-r--r--   0        0        0      280 2023-07-08 22:55:36.156770 klu-0.1.8/klu/action/constants.py
--rw-r--r--   0        0        0      537 2023-07-08 22:55:36.156770 klu-0.1.8/klu/action/errors.py
--rw-r--r--   0        0        0     1936 2023-07-08 22:55:36.160770 klu-0.1.8/klu/action/models.py
--rw-r--r--   0        0        0        0 2023-07-08 22:55:36.160770 klu-0.1.8/klu/api/__init__.py
--rw-r--r--   0        0        0     2998 2023-07-08 22:55:36.160770 klu-0.1.8/klu/api/client.py
--rw-r--r--   0        0        0      199 2023-07-08 22:55:36.160770 klu-0.1.8/klu/api/config.py
--rw-r--r--   0        0        0      118 2023-07-08 22:55:36.160770 klu-0.1.8/klu/api/constants.py
--rw-r--r--   0        0        0     1406 2023-07-08 22:55:36.160770 klu-0.1.8/klu/api/sse_client.py
--rw-r--r--   0        0        0        0 2023-07-08 22:55:36.160770 klu-0.1.8/klu/application/__init__.py
--rw-r--r--   0        0        0     7753 2023-07-08 22:55:36.160770 klu-0.1.8/klu/application/client.py
--rw-r--r--   0        0        0      259 2023-07-08 22:55:36.160770 klu-0.1.8/klu/application/constants.py
--rw-r--r--   0        0        0      318 2023-07-08 22:55:36.160770 klu-0.1.8/klu/application/errors.py
--rw-r--r--   0        0        0     1421 2023-07-08 22:55:36.160770 klu-0.1.8/klu/application/models.py
--rw-r--r--   0        0        0        0 2023-07-08 22:55:36.160770 klu-0.1.8/klu/client/__init__.py
--rw-r--r--   0        0        0      898 2023-07-08 22:55:36.160770 klu-0.1.8/klu/client/klu.py
--rw-r--r--   0        0        0        0 2023-07-08 22:55:36.160770 klu-0.1.8/klu/common/__init__.py
--rw-r--r--   0        0        0     3086 2023-07-08 22:55:36.160770 klu-0.1.8/klu/common/client.py
--rw-r--r--   0        0        0     2975 2023-07-08 22:55:36.160770 klu-0.1.8/klu/common/errors.py
--rw-r--r--   0        0        0     2403 2023-07-08 22:55:36.160770 klu-0.1.8/klu/common/models.py
--rw-r--r--   0        0        0        0 2023-07-08 22:55:36.160770 klu-0.1.8/klu/data/__init__.py
--rw-r--r--   0        0        0     2534 2023-07-08 22:55:36.160770 klu-0.1.8/klu/data/client.py
--rw-r--r--   0        0        0       25 2023-07-08 22:55:36.160770 klu-0.1.8/klu/data/constants.py
--rw-r--r--   0        0        0      274 2023-07-08 22:55:36.160770 klu-0.1.8/klu/data/errors.py
--rw-r--r--   0        0        0     3381 2023-07-08 22:55:36.160770 klu-0.1.8/klu/data/models.py
--rw-r--r--   0        0        0        0 2023-07-08 22:55:36.160770 klu-0.1.8/klu/data_index/__init__.py
--rw-r--r--   0        0        0     8671 2023-07-08 22:55:36.160770 klu-0.1.8/klu/data_index/client.py
--rw-r--r--   0        0        0      287 2023-07-08 22:55:36.160770 klu-0.1.8/klu/data_index/constants.py
--rw-r--r--   0        0        0      309 2023-07-08 22:55:36.160770 klu-0.1.8/klu/data_index/errors.py
--rw-r--r--   0        0        0     3405 2023-07-08 22:55:36.160770 klu-0.1.8/klu/data_index/models.py
--rw-r--r--   0        0        0        0 2023-07-08 22:55:36.160770 klu-0.1.8/klu/experiment/__init__.py
--rw-r--r--   0        0        0     6137 2023-07-08 22:55:36.160770 klu-0.1.8/klu/experiment/client.py
--rw-r--r--   0        0        0      104 2023-07-08 22:55:36.160770 klu-0.1.8/klu/experiment/constants.py
--rw-r--r--   0        0        0      573 2023-07-08 22:55:36.160770 klu-0.1.8/klu/experiment/errors.py
--rw-r--r--   0        0        0     1083 2023-07-08 22:55:36.160770 klu-0.1.8/klu/experiment/models.py
--rw-r--r--   0        0        0       19 2023-07-08 22:55:36.160770 klu-0.1.8/klu/klu.py
--rw-r--r--   0        0        0        0 2023-07-08 22:55:36.160770 klu-0.1.8/klu/model/__init__.py
--rw-r--r--   0        0        0     3505 2023-07-08 22:55:36.160770 klu-0.1.8/klu/model/client.py
--rw-r--r--   0        0        0       28 2023-07-08 22:55:36.160770 klu-0.1.8/klu/model/constants.py
--rw-r--r--   0        0        0      447 2023-07-08 22:55:36.160770 klu-0.1.8/klu/model/errors.py
--rw-r--r--   0        0        0     1387 2023-07-08 22:55:36.160770 klu-0.1.8/klu/model/models.py
--rw-r--r--   0        0        0        0 2023-07-08 22:55:36.160770 klu-0.1.8/klu/session/__init__.py
--rw-r--r--   0        0        0     1483 2023-07-08 22:55:36.160770 klu-0.1.8/klu/session/client.py
--rw-r--r--   0        0        0       32 2023-07-08 22:55:36.160770 klu-0.1.8/klu/session/constants.py
--rw-r--r--   0        0        0     1255 2023-07-08 22:55:36.160770 klu-0.1.8/klu/session/models.py
--rw-r--r--   0        0        0      111 2023-07-08 22:55:36.160770 klu-0.1.8/klu/utils/dict_helpers.py
--rw-r--r--   0        0        0      752 2023-07-08 22:55:36.160770 klu-0.1.8/klu/utils/file_upload.py
--rw-r--r--   0        0        0     2407 2023-07-08 22:55:36.160770 klu-0.1.8/klu/utils/paginator.py
--rw-r--r--   0        0        0        0 2023-07-08 22:55:36.160770 klu-0.1.8/klu/workspace/__init__.py
--rw-r--r--   0        0        0     8052 2023-07-08 22:55:36.160770 klu-0.1.8/klu/workspace/client.py
--rw-r--r--   0        0        0      321 2023-07-08 22:55:36.160770 klu-0.1.8/klu/workspace/constants.py
--rw-r--r--   0        0        0      244 2023-07-08 22:55:36.160770 klu-0.1.8/klu/workspace/errors.py
--rw-r--r--   0        0        0      943 2023-07-08 22:55:36.160770 klu-0.1.8/klu/workspace/models.py
--rw-r--r--   0        0        0     1952 2023-07-08 22:55:36.160770 klu-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     3698 1970-01-01 00:00:00.000000 klu-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-07-10 00:18:13.045407 klu-0.1.9/LICENSE
+-rw-r--r--   0        0        0     2840 2023-07-10 00:18:13.045407 klu-0.1.9/README.md
+-rw-r--r--   0        0        0      150 2023-07-10 00:18:13.045407 klu-0.1.9/klu/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-10 00:18:13.045407 klu-0.1.9/klu/action/__init__.py
+-rw-r--r--   0        0        0    11398 2023-07-10 00:18:13.045407 klu-0.1.9/klu/action/client.py
+-rw-r--r--   0        0        0      280 2023-07-10 00:18:13.045407 klu-0.1.9/klu/action/constants.py
+-rw-r--r--   0        0        0      537 2023-07-10 00:18:13.045407 klu-0.1.9/klu/action/errors.py
+-rw-r--r--   0        0        0     2029 2023-07-10 00:18:13.045407 klu-0.1.9/klu/action/models.py
+-rw-r--r--   0        0        0        0 2023-07-10 00:18:13.045407 klu-0.1.9/klu/api/__init__.py
+-rw-r--r--   0        0        0     2998 2023-07-10 00:18:13.045407 klu-0.1.9/klu/api/client.py
+-rw-r--r--   0        0        0      199 2023-07-10 00:18:13.045407 klu-0.1.9/klu/api/config.py
+-rw-r--r--   0        0        0      118 2023-07-10 00:18:13.045407 klu-0.1.9/klu/api/constants.py
+-rw-r--r--   0        0        0     1406 2023-07-10 00:18:13.045407 klu-0.1.9/klu/api/sse_client.py
+-rw-r--r--   0        0        0        0 2023-07-10 00:18:13.045407 klu-0.1.9/klu/application/__init__.py
+-rw-r--r--   0        0        0     7753 2023-07-10 00:18:13.045407 klu-0.1.9/klu/application/client.py
+-rw-r--r--   0        0        0      259 2023-07-10 00:18:13.045407 klu-0.1.9/klu/application/constants.py
+-rw-r--r--   0        0        0      318 2023-07-10 00:18:13.045407 klu-0.1.9/klu/application/errors.py
+-rw-r--r--   0        0        0     1482 2023-07-10 00:18:13.045407 klu-0.1.9/klu/application/models.py
+-rw-r--r--   0        0        0        0 2023-07-10 00:18:13.045407 klu-0.1.9/klu/client/__init__.py
+-rw-r--r--   0        0        0      898 2023-07-10 00:18:13.045407 klu-0.1.9/klu/client/klu.py
+-rw-r--r--   0        0        0        0 2023-07-10 00:18:13.045407 klu-0.1.9/klu/common/__init__.py
+-rw-r--r--   0        0        0     3086 2023-07-10 00:18:13.045407 klu-0.1.9/klu/common/client.py
+-rw-r--r--   0        0        0     2975 2023-07-10 00:18:13.045407 klu-0.1.9/klu/common/errors.py
+-rw-r--r--   0        0        0     3402 2023-07-10 00:18:13.045407 klu-0.1.9/klu/common/models.py
+-rw-r--r--   0        0        0        0 2023-07-10 00:18:13.045407 klu-0.1.9/klu/data/__init__.py
+-rw-r--r--   0        0        0     2534 2023-07-10 00:18:13.045407 klu-0.1.9/klu/data/client.py
+-rw-r--r--   0        0        0       25 2023-07-10 00:18:13.045407 klu-0.1.9/klu/data/constants.py
+-rw-r--r--   0        0        0      274 2023-07-10 00:18:13.045407 klu-0.1.9/klu/data/errors.py
+-rw-r--r--   0        0        0     3564 2023-07-10 00:18:13.045407 klu-0.1.9/klu/data/models.py
+-rw-r--r--   0        0        0        0 2023-07-10 00:18:13.045407 klu-0.1.9/klu/data_index/__init__.py
+-rw-r--r--   0        0        0     8671 2023-07-10 00:18:13.045407 klu-0.1.9/klu/data_index/client.py
+-rw-r--r--   0        0        0      287 2023-07-10 00:18:13.045407 klu-0.1.9/klu/data_index/constants.py
+-rw-r--r--   0        0        0      309 2023-07-10 00:18:13.045407 klu-0.1.9/klu/data_index/errors.py
+-rw-r--r--   0        0        0     3588 2023-07-10 00:18:13.045407 klu-0.1.9/klu/data_index/models.py
+-rw-r--r--   0        0        0        0 2023-07-10 00:18:13.045407 klu-0.1.9/klu/experiment/__init__.py
+-rw-r--r--   0        0        0     6137 2023-07-10 00:18:13.045407 klu-0.1.9/klu/experiment/client.py
+-rw-r--r--   0        0        0      103 2023-07-10 00:18:13.045407 klu-0.1.9/klu/experiment/constants.py
+-rw-r--r--   0        0        0      573 2023-07-10 00:18:13.045407 klu-0.1.9/klu/experiment/errors.py
+-rw-r--r--   0        0        0     1144 2023-07-10 00:18:13.045407 klu-0.1.9/klu/experiment/models.py
+-rw-r--r--   0        0        0       19 2023-07-10 00:18:13.045407 klu-0.1.9/klu/klu.py
+-rw-r--r--   0        0        0        0 2023-07-10 00:18:13.045407 klu-0.1.9/klu/model/__init__.py
+-rw-r--r--   0        0        0     3486 2023-07-10 00:18:13.045407 klu-0.1.9/klu/model/client.py
+-rw-r--r--   0        0        0       90 2023-07-10 00:18:13.045407 klu-0.1.9/klu/model/constants.py
+-rw-r--r--   0        0        0      447 2023-07-10 00:18:13.045407 klu-0.1.9/klu/model/errors.py
+-rw-r--r--   0        0        0     1448 2023-07-10 00:18:13.045407 klu-0.1.9/klu/model/models.py
+-rw-r--r--   0        0        0        0 2023-07-10 00:18:13.045407 klu-0.1.9/klu/session/__init__.py
+-rw-r--r--   0        0        0     1483 2023-07-10 00:18:13.045407 klu-0.1.9/klu/session/client.py
+-rw-r--r--   0        0        0       32 2023-07-10 00:18:13.045407 klu-0.1.9/klu/session/constants.py
+-rw-r--r--   0        0        0     1316 2023-07-10 00:18:13.045407 klu-0.1.9/klu/session/models.py
+-rw-r--r--   0        0        0      111 2023-07-10 00:18:13.045407 klu-0.1.9/klu/utils/dict_helpers.py
+-rw-r--r--   0        0        0      752 2023-07-10 00:18:13.045407 klu-0.1.9/klu/utils/file_upload.py
+-rw-r--r--   0        0        0     2407 2023-07-10 00:18:13.045407 klu-0.1.9/klu/utils/paginator.py
+-rw-r--r--   0        0        0        0 2023-07-10 00:18:13.045407 klu-0.1.9/klu/workspace/__init__.py
+-rw-r--r--   0        0        0     8052 2023-07-10 00:18:13.045407 klu-0.1.9/klu/workspace/client.py
+-rw-r--r--   0        0        0      321 2023-07-10 00:18:13.045407 klu-0.1.9/klu/workspace/constants.py
+-rw-r--r--   0        0        0      244 2023-07-10 00:18:13.045407 klu-0.1.9/klu/workspace/errors.py
+-rw-r--r--   0        0        0     1004 2023-07-10 00:18:13.045407 klu-0.1.9/klu/workspace/models.py
+-rw-r--r--   0        0        0     1952 2023-07-10 00:18:13.049407 klu-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     3698 1970-01-01 00:00:00.000000 klu-0.1.9/PKG-INFO
```

### Comparing `klu-0.1.8/LICENSE` & `klu-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `klu-0.1.8/README.md` & `klu-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `klu-0.1.8/klu/action/client.py` & `klu-0.1.9/klu/action/client.py`

 * *Files identical despite different names*

### Comparing `klu-0.1.8/klu/action/errors.py` & `klu-0.1.9/klu/action/errors.py`

 * *Files identical despite different names*

### Comparing `klu-0.1.8/klu/action/models.py` & `klu-0.1.9/klu/model/models.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,66 +1,54 @@
 """
-This module provides data models for the Action.
+This module provides data models for the Model.
 """
+
 from dataclasses import asdict, dataclass
 from datetime import datetime
-from typing import Any, Dict, Optional
+from typing import Optional
 
-from klu.common.models import BaseDataClass, BaseEngineModel, PromptInput
+from klu.common.models import BaseEngineModel
 
 
 @dataclass
-class Action(BaseEngineModel):
+class Model(BaseEngineModel):
     """
-    This class represents the Action data model returned from the Klu engine
+    This class represents the Model data returned from the Klu engine
     """
 
+    id: int
+    llm: str
     guid: str
-    name: str
-    app_id: int
-    model_id: int
-    action_type: str
-    input: PromptInput
-    description: Optional[str]
-    model_config: Optional[dict]
+    model_name: str
+    created_by_id: str
+    workspace_model_provider_id: int
     updated_at: Optional[str] = None
     created_at: Optional[str] = None
-    meta_data: Optional[Dict[str, Any]] = None
+
+    def __repr__(self):
+        return self.generate_repr()
 
     @classmethod
-    def _from_engine_format(cls, data: dict) -> "Action":
+    def _from_engine_format(cls, data: dict) -> "Model":
         return cls._create_instance(
             **{
-                "app_id": data.pop("appId", None),
-                "model_id": data.pop("modelId", None),
                 "updated_at": data.pop("updatedAt", None),
                 "created_at": data.pop("createdAt", None),
-                "action_type": data.pop("agent_type", None),
+                "created_by_id": data.pop("createdById", None),
+                "workspace_model_provider_id": data.pop(
+                    "workspaceModelProviderId", None
+                ),
             },
             **data,
         )
 
     def _to_engine_format(self) -> dict:
-        base_dict = asdict(self)
-
-        return {
-            "appId": base_dict.pop("app_id", None),
-            "modelId": base_dict.pop("model_id", None),
-            "meta_data": base_dict.pop("meta_data", None),
-            "updatedAt": base_dict.pop("updated_at", None),
-            "createdAt": base_dict.pop("created_at", None),
-            "agent_type": base_dict.pop("action_type", None),
-            **base_dict,
-        }
-
+        base_dict = asdict(
+            self, dict_factory=lambda x: {k: v for (k, v) in x if v is not None}
+        )
 
-@dataclass
-class PromptResponse(BaseDataClass):
-    """
-    This class represents the Response data model returned from the Klu engine in response to action prompting.
-    """
+        base_dict.pop("updated_at", None)
+        base_dict.pop("created_at", None)
+        base_dict.pop("created_by_id", None)
+        base_dict.pop("workspace_model_provider_id", None)
 
-    msg: str
-    streaming: bool
-    result_url: Optional[str] = None
-    feedback_url: Optional[str] = None
-    streaming_url: Optional[str] = None
+        return base_dict
```

### Comparing `klu-0.1.8/klu/api/client.py` & `klu-0.1.9/klu/api/client.py`

 * *Files identical despite different names*

### Comparing `klu-0.1.8/klu/api/sse_client.py` & `klu-0.1.9/klu/api/sse_client.py`

 * *Files identical despite different names*

### Comparing `klu-0.1.8/klu/application/client.py` & `klu-0.1.9/klu/application/client.py`

 * *Files identical despite different names*

### Comparing `klu-0.1.8/klu/application/models.py` & `klu-0.1.9/klu/application/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,14 +24,17 @@
     created_by_id: str
 
     description: Optional[str]
     deleted: Optional[bool] = None
     updated_at: Optional[str] = None
     created_at: Optional[str] = None
 
+    def __repr__(self):
+        return self.generate_repr()
+
     @classmethod
     def _from_engine_format(cls, data: dict) -> "Application":
         return cls._create_instance(
             **{
                 "updated_at": data.pop("updatedAt", None),
                 "created_at": data.pop("createdAt", None),
                 "workspace_id": data.pop("workspaceId", None),
```

### Comparing `klu-0.1.8/klu/client/klu.py` & `klu-0.1.9/klu/client/klu.py`

 * *Files identical despite different names*

### Comparing `klu-0.1.8/klu/common/client.py` & `klu-0.1.9/klu/common/client.py`

 * *Files identical despite different names*

### Comparing `klu-0.1.8/klu/common/errors.py` & `klu-0.1.9/klu/common/errors.py`

 * *Files identical despite different names*

### Comparing `klu-0.1.8/klu/data/client.py` & `klu-0.1.9/klu/data/client.py`

 * *Files identical despite different names*

### Comparing `klu-0.1.8/klu/data/models.py` & `klu-0.1.9/klu/data/models.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,23 +14,29 @@
     """
     This class represents the base data with Id after it has been persisted into the Klu Database
     """
 
     id: int
     guid: str
 
+    def __repr__(self):
+        return self.generate_repr()
+
 
 @dataclass
 class DataWithFeedbackUrl(BaseEngineModel, ABC):
     """
     This class represents the data specific to the model returned from the Action prompting
     """
 
     feedback_url: int
 
+    def __repr__(self):
+        return self.generate_repr()
+
 
 @dataclass
 class DataBaseClass(BaseEngineModel):
     """
     This class represents the generic data information that is stored in the Klu database
     """
 
@@ -41,14 +47,17 @@
     rating: Optional[int] = None
     metadata: Optional[dict] = None
     correction: Optional[str] = None
     updated_at: Optional[str] = None
     created_at: Optional[str] = None
     full_prompt_sent: Optional[dict] = None
 
+    def __repr__(self):
+        return self.generate_repr()
+
     @classmethod
     def _from_engine_format(cls, data: dict) -> "DataBaseClass":
         return cls._create_instance(
             **{
                 "updated_at": data.pop("updatedAt", None),
                 "created_at": data.pop("createdAt", None),
             },
```

### Comparing `klu-0.1.8/klu/data_index/client.py` & `klu-0.1.9/klu/data_index/client.py`

 * *Files identical despite different names*

### Comparing `klu-0.1.8/klu/data_index/models.py` & `klu-0.1.9/klu/data_index/models.py`

 * *Files 10% similar despite different names*

```diff
@@ -42,14 +42,17 @@
     workspace_id: int
     created_by_id: str
 
     description: Optional[str]
     updated_at: Optional[str] = None
     created_at: Optional[str] = None
 
+    def __repr__(self):
+        return self.generate_repr()
+
     @classmethod
     def _from_engine_format(cls, data: dict) -> "DataIndex":
         return cls._create_instance(
             **{
                 "type_id": data.pop("typeId", None),
                 "task_id": data.pop("taskId", None),
                 "file_url": data.pop("fileUrl", None),
@@ -90,18 +93,24 @@
     This same object_url can be used during the data_index creation.
     """
 
     url: str
     fields: dict
     object_url: str
 
+    def __repr__(self):
+        return self.generate_repr()
+
 
 @dataclass
 class FileData(BaseDataClass):
     """
     file_name (str): The name of the file to be uploaded. Has to be unique among the files you uploaded before.
     file_path (str): The path to a file in your system.
     The file path can be an absolute path, a relative path, or a path that includes variables like ~ or $HOME
     """
 
     file_path: str
     file_name: str
+
+    def __repr__(self):
+        return self.generate_repr()
```

### Comparing `klu-0.1.8/klu/experiment/client.py` & `klu-0.1.9/klu/experiment/client.py`

 * *Files identical despite different names*

### Comparing `klu-0.1.8/klu/experiment/errors.py` & `klu-0.1.9/klu/experiment/errors.py`

 * *Files identical despite different names*

### Comparing `klu-0.1.8/klu/experiment/models.py` & `klu-0.1.9/klu/experiment/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,14 +19,17 @@
     status: str
     app_guid: str
     action_primary_guid: str
     action_secondary_guid: str
     created_at: Optional[str] = None
     updated_at: Optional[str] = None
 
+    def __repr__(self):
+        return self.generate_repr()
+
     @classmethod
     def _from_engine_format(cls, data: dict) -> "Experiment":
         return cls._create_instance(
             **{
                 "updated_at": data.pop("updatedAt", None),
                 "created_at": data.pop("createdAt", None),
             },
```

### Comparing `klu-0.1.8/klu/model/client.py` & `klu-0.1.9/klu/model/client.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from typing import Optional
 
 import aiohttp
 from aiohttp import ClientResponseError
 
 from klu.common.client import KluClientBase
 from klu.common.errors import InvalidUpdateParamsError, UnknownKluAPIError
-from klu.model.constants import MODEL_ENDPOINT
+from klu.model.constants import MODEL_ENDPOINT, VALIDATE_MODEL_API_KEY_ENDPOINT
 from klu.model.errors import UnknownModelProviderError
 from klu.model.models import Model
 from klu.utils.dict_helpers import dict_no_empty
 
 
 class ModelsClient(KluClientBase):
     def __init__(self, api_key: str):
@@ -73,30 +73,30 @@
             guid (str): ID of a model to delete.
 
         Returns:
             Deleted model object
         """
         return await super().delete(guid)
 
-    async def validate_provider_api_key(self, api_key: str, provider: str) -> bool:
+    async def validate_provider_api_key(self, api_key: str, provider: int) -> bool:
         """
         Validates API keys for provided api_key and provider values.
 
         Args:
             api_key (str): Model api_key
-            provider (str): Model provider. Required. Should be one of the following: [OpenAI, HuggingFace, NLPCloud, GooseAI, AI21 & Anthropic]
+            provider (int): Model provider id. Should be taken from the UI.
 
         Returns:
             A JSON response with a message about successful creation if model was created.
         """
         async with aiohttp.ClientSession() as session:
             client = self._get_api_client(session)
             try:
                 response = await client.post(
-                    MODEL_ENDPOINT,
+                    VALIDATE_MODEL_API_KEY_ENDPOINT,
                     {
                         "api_key": api_key,
                         "provider": provider,
                     },
                 )
                 return bool(response.get("validated"))
             except ClientResponseError as e:
```

### Comparing `klu-0.1.8/klu/session/client.py` & `klu-0.1.9/klu/session/client.py`

 * *Files identical despite different names*

### Comparing `klu-0.1.8/klu/session/models.py` & `klu-0.1.9/klu/session/models.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,14 +18,17 @@
     guid: str
     action_id: int
     created_by_id: str
     name: Optional[str] = None
     created_at: Optional[str] = None
     updated_at: Optional[str] = None
 
+    def __repr__(self):
+        return self.generate_repr()
+
     @classmethod
     def _from_engine_format(cls, data: dict) -> "Session":
         return cls._create_instance(
             **{
                 "action_id": data.pop("actionId", None),
                 "updated_at": data.pop("updatedAt", None),
                 "created_at": data.pop("createdAt", None),
```

### Comparing `klu-0.1.8/klu/utils/file_upload.py` & `klu-0.1.9/klu/utils/file_upload.py`

 * *Files identical despite different names*

### Comparing `klu-0.1.8/klu/utils/paginator.py` & `klu-0.1.9/klu/utils/paginator.py`

 * *Files identical despite different names*

### Comparing `klu-0.1.8/klu/workspace/client.py` & `klu-0.1.9/klu/workspace/client.py`

 * *Files identical despite different names*

### Comparing `klu-0.1.8/klu/workspace/models.py` & `klu-0.1.9/klu/workspace/models.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,14 +15,17 @@
     slug: str
     created_by_id: str
     """
         Workspace unique identifier. This is the id you can later use to query this object and create application.
     """
     project_guid: str
 
+    def __repr__(self):
+        return self.generate_repr()
+
     @classmethod
     def _from_engine_format(cls, data: dict) -> "Workspace":
         return cls._create_instance(
             **{
                 "created_by_id": data.pop("createdById", None),
             },
             **data,
```

### Comparing `klu-0.1.8/pyproject.toml` & `klu-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "klu"
-version = "0.1.8"
+version = "0.1.9"
 homepage = "https://github.com/ssabev/klu"
 description = "SDK for building AI Enabled apps."
 authors = ["Stefan Sabev <stefan@klu.ai>"]
 readme = "README.md"
 license =  "MIT"
 classifiers=[
     'Development Status :: 2 - Pre-Alpha',
```

### Comparing `klu-0.1.8/PKG-INFO` & `klu-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: klu
-Version: 0.1.8
+Version: 0.1.9
 Summary: SDK for building AI Enabled apps.
 Home-page: https://github.com/ssabev/klu
 License: MIT
 Author: Stefan Sabev
 Author-email: stefan@klu.ai
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
```


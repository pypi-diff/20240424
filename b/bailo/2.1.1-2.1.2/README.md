# Comparing `tmp/bailo-2.1.1.tar.gz` & `tmp/bailo-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bailo-2.1.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "bailo-2.1.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `bailo-2.1.1.tar` & `bailo-2.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     2241 2024-04-03 16:38:22.025113 bailo-2.1.1/README.md
--rw-r--r--   0        0        0     4869 2024-04-03 16:38:22.025113 bailo-2.1.1/pyproject.toml
--rw-r--r--   0        0        0      605 2024-04-03 16:38:22.025113 bailo-2.1.1/src/bailo/__init__.py
--rw-r--r--   0        0        0      153 2024-04-03 16:38:22.025113 bailo-2.1.1/src/bailo/core/__init__.py
--rw-r--r--   0        0        0     3458 2024-04-03 16:38:22.029113 bailo-2.1.1/src/bailo/core/agent.py
--rw-r--r--   0        0        0    19039 2024-04-03 16:38:22.029113 bailo-2.1.1/src/bailo/core/client.py
--rw-r--r--   0        0        0      564 2024-04-03 16:38:22.029113 bailo-2.1.1/src/bailo/core/enums.py
--rw-r--r--   0        0        0      221 2024-04-03 16:38:22.029113 bailo-2.1.1/src/bailo/core/exceptions.py
--rw-r--r--   0        0        0     1057 2024-04-03 16:38:22.029113 bailo-2.1.1/src/bailo/core/utils.py
--rw-r--r--   0        0        0      521 2024-04-03 16:38:22.029113 bailo-2.1.1/src/bailo/helper/__init__.py
--rw-r--r--   0        0        0     3923 2024-04-03 16:38:22.029113 bailo-2.1.1/src/bailo/helper/access_request.py
--rw-r--r--   0        0        0    15195 2024-04-03 16:38:22.029113 bailo-2.1.1/src/bailo/helper/model.py
--rw-r--r--   0        0        0     7043 2024-04-03 16:38:22.029113 bailo-2.1.1/src/bailo/helper/release.py
--rw-r--r--   0        0        0     2976 2024-04-03 16:38:22.029113 bailo-2.1.1/src/bailo/helper/schema.py
--rw-r--r--   0        0        0     3646 1970-01-01 00:00:00.000000 bailo-2.1.1/PKG-INFO
+-rw-r--r--   0        0        0     2241 2024-04-24 14:35:49.087870 bailo-2.1.2/README.md
+-rw-r--r--   0        0        0     4869 2024-04-24 14:35:49.087870 bailo-2.1.2/pyproject.toml
+-rw-r--r--   0        0        0      616 2024-04-24 14:35:49.087870 bailo-2.1.2/src/bailo/__init__.py
+-rw-r--r--   0        0        0      153 2024-04-24 14:35:49.087870 bailo-2.1.2/src/bailo/core/__init__.py
+-rw-r--r--   0        0        0     3458 2024-04-24 14:35:49.087870 bailo-2.1.2/src/bailo/core/agent.py
+-rw-r--r--   0        0        0    19238 2024-04-24 14:35:49.087870 bailo-2.1.2/src/bailo/core/client.py
+-rw-r--r--   0        0        0      672 2024-04-24 14:35:49.087870 bailo-2.1.2/src/bailo/core/enums.py
+-rw-r--r--   0        0        0      221 2024-04-24 14:35:49.087870 bailo-2.1.2/src/bailo/core/exceptions.py
+-rw-r--r--   0        0        0     1057 2024-04-24 14:35:49.087870 bailo-2.1.2/src/bailo/core/utils.py
+-rw-r--r--   0        0        0      521 2024-04-24 14:35:49.087870 bailo-2.1.2/src/bailo/helper/__init__.py
+-rw-r--r--   0        0        0     3923 2024-04-24 14:35:49.087870 bailo-2.1.2/src/bailo/helper/access_request.py
+-rw-r--r--   0        0        0    15468 2024-04-24 14:35:49.087870 bailo-2.1.2/src/bailo/helper/model.py
+-rw-r--r--   0        0        0     7043 2024-04-24 14:35:49.087870 bailo-2.1.2/src/bailo/helper/release.py
+-rw-r--r--   0        0        0     2976 2024-04-24 14:35:49.087870 bailo-2.1.2/src/bailo/helper/schema.py
+-rw-r--r--   0        0        0     3646 1970-01-01 00:00:00.000000 bailo-2.1.2/PKG-INFO
```

### Comparing `bailo-2.1.1/README.md` & `bailo-2.1.2/README.md`

 * *Files identical despite different names*

### Comparing `bailo-2.1.1/pyproject.toml` & `bailo-2.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bailo-2.1.1/src/bailo/__init__.py` & `bailo-2.1.2/src/bailo/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 Bailo Python Client
 ===================
 
 Bailo is a ecosystem for managing the lifecycle of managing machine learning models. This package provides support for interacting with models within Bailo.
 """
 from __future__ import annotations
 
-__version__ = "2.1.1"
+__version__ = "2.1.2"
 
 from bailo.core.agent import Agent, PkiAgent, TokenAgent
 from bailo.core.client import Client
-from bailo.core.enums import ModelVisibility, Role, SchemaKind
+from bailo.core.enums import EntryKind, ModelVisibility, Role, SchemaKind
 from bailo.helper.access_request import AccessRequest
-from bailo.helper.model import Model, Experiment
+from bailo.helper.model import Experiment, Model
 from bailo.helper.release import Release
 from bailo.helper.schema import Schema
```

### Comparing `bailo-2.1.1/src/bailo/core/agent.py` & `bailo-2.1.2/src/bailo/core/agent.py`

 * *Files identical despite different names*

### Comparing `bailo-2.1.1/src/bailo/core/client.py` & `bailo-2.1.2/src/bailo/core/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from __future__ import annotations
 
-import shutil
 from io import BytesIO
 from typing import Any
 
 from bailo.core.agent import Agent, TokenAgent
-from bailo.core.enums import ModelVisibility, SchemaKind
+from bailo.core.enums import EntryKind, ModelVisibility, SchemaKind
 from bailo.core.utils import filter_none
 
 
 class Client:
     """Create a Client object that can be used to talk to the website.
 
     :param url: Url of bailo website
@@ -19,31 +18,34 @@
     def __init__(self, url: str, agent: Agent = Agent()):
         self.url = url.rstrip("/") + "/api"
         self.agent = agent
 
     def post_model(
         self,
         name: str,
+        kind: EntryKind,
         description: str,
         team_id: str,
         visibility: ModelVisibility | None = None,
     ):
         """Create a model.
 
         :param name: Name of the model
+        :param kind: Either a Model or a Datacard
         :param description: Description of the model
         :param visibility: Enum to define model visibility (e.g public or private)
         :return: JSON response object
         """
         if visibility is not None:
             visibility = str(visibility)
 
         filtered_json = filter_none(
             {
                 "name": name,
+                "kind": kind,
                 "description": description,
                 "visibility": visibility,
                 "teamId": team_id,
             }
         )
 
         return self.agent.post(
@@ -95,26 +97,28 @@
             f"{self.url}/v2/model/{model_id}",
         ).json()
 
     def patch_model(
         self,
         model_id: str,
         name: str | None = None,
+        kind: str | None = None,
         description: str | None = None,
         visibility: str | None = None,
     ):
         """Update a specific model using its unique ID.
 
         :param model_id: Unique model ID
         :param name: Name of the model, defaults to None
+        :param kind: Either a Model or a Datacard
         :param description: Description of the model, defaults to None
         :param visibility: Enum to define model visibility (e.g. public or private), defaults to None
         :return: JSON response object
         """
-        filtered_json = filter_none({"name": name, "description": description, "visibility": visibility})
+        filtered_json = filter_none({"name": name, "kind": kind, "description": description, "visibility": visibility})
 
         return self.agent.patch(f"{self.url}/v2/model/{model_id}", json=filtered_json).json()
 
     def get_model_card(
         self,
         model_id: str,
         version: str,
```

### Comparing `bailo-2.1.1/src/bailo/core/utils.py` & `bailo-2.1.2/src/bailo/core/utils.py`

 * *Files identical despite different names*

### Comparing `bailo-2.1.1/src/bailo/helper/__init__.py` & `bailo-2.1.2/src/bailo/helper/__init__.py`

 * *Files identical despite different names*

### Comparing `bailo-2.1.1/src/bailo/helper/access_request.py` & `bailo-2.1.2/src/bailo/helper/access_request.py`

 * *Files identical despite different names*

### Comparing `bailo-2.1.1/src/bailo/helper/model.py` & `bailo-2.1.2/src/bailo/helper/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 from __future__ import annotations
 
+import os
+import shutil
+import tempfile
 from typing import Any
 
 from bailo.core.client import Client
-from bailo.core.enums import ModelVisibility
-from bailo.helper.release import Release
+from bailo.core.enums import EntryKind, ModelVisibility
 from bailo.core.exceptions import BailoException
 from bailo.core.utils import NestedDict
-
-import os
-import shutil
-import tempfile
+from bailo.helper.release import Release
 from semantic_version import Version
 
 try:
     import mlflow
 
     ml_flow = True
 except ImportError:
@@ -23,60 +22,66 @@
 
 class Model:
     """Represent a model within Bailo.
 
     :param client: A client object used to interact with Bailo
     :param model_id: A unique ID for the model
     :param name: Name of model
+    :param kind: Either a Model or a Datacard
     :param description: Description of model
     :param visibility: Visibility of model, using ModelVisibility enum (e.g Public or Private), defaults to None
     """
 
     def __init__(
         self,
         client: Client,
         model_id: str,
         name: str,
+        kind: EntryKind,
         description: str,
         visibility: ModelVisibility | None = None,
     ) -> None:
         self.client = client
 
         self.model_id = model_id
         self.name = name
+        self.kind = kind
         self.description = description
         self.visibility = visibility
 
         self.model_card = None
         self.model_card_version = None
         self.model_card_schema = None
 
     @classmethod
     def create(
         cls,
         client: Client,
         name: str,
+        kind: EntryKind,
         description: str,
         team_id: str,
         visibility: ModelVisibility | None = None,
     ) -> Model:
         """Build a model from Bailo and uploads it.
 
         :param client: A client object used to interact with Bailo
         :param name: Name of model
+        :param kind: Either a Model or a Datacard
         :param description: Description of model
         :param team_id: A unique team ID
         :param visibility: Visibility of model, using ModelVisibility enum (e.g Public or Private), defaults to None
         :return: Model object
         """
-        res = client.post_model(name=name, description=description, team_id=team_id, visibility=visibility)
+        res = client.post_model(name=name, kind=kind, description=description, team_id=team_id, visibility=visibility)
         model = cls(
             client=client,
             model_id=res["model"]["id"],
             name=name,
+            kind=kind,
             description=description,
             visibility=visibility,
         )
 
         model.__unpack(res["model"])
 
         return model
@@ -89,28 +94,30 @@
         :param model_id: A unique model ID
         :return: A model object
         """
         res = client.get_model(model_id=model_id)["model"]
         model = cls(
             client=client,
             model_id=model_id,
+            kind=res["kind"],
             name=res["name"],
             description=res["description"],
         )
         model.__unpack(res)
 
         model.get_card_latest()
 
         return model
 
     def update(self) -> None:
         """Upload and retrieves any changes to the model summary on Bailo."""
         res = self.client.patch_model(
             model_id=self.model_id,
             name=self.name,
+            kind=self.kind,
             description=self.description,
             visibility=self.visibility,
         )
         self.__unpack(res["model"])
 
     def update_model_card(self, model_card: dict[str, Any] | None = None) -> None:
         """Upload and retrieves any changes to the model card on Bailo.
```

### Comparing `bailo-2.1.1/src/bailo/helper/release.py` & `bailo-2.1.2/src/bailo/helper/release.py`

 * *Files identical despite different names*

### Comparing `bailo-2.1.1/src/bailo/helper/schema.py` & `bailo-2.1.2/src/bailo/helper/schema.py`

 * *Files identical despite different names*

### Comparing `bailo-2.1.1/PKG-INFO` & `bailo-2.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bailo
-Version: 2.1.1
+Version: 2.1.2
 Summary: Simplifies interacting with Bailo
 Requires-Python: >=3.8.1
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: bailo Version: 2.1.1 Summary: Simplifies
+Metadata-Version: 2.1 Name: bailo Version: 2.1.2 Summary: Simplifies
 interacting with Bailo Requires-Python: >=3.8.1 Description-Content-Type: text/
 markdown Classifier: Development Status :: 3 - Alpha Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: semantic-version==2.10.0 Requires-Dist: requests>=2.22 Requires-
 Dist: black==23.3.0 ; extra == "test" Requires-Dist: check-manifest==0.49 ;
```


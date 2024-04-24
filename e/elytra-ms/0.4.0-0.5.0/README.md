# Comparing `tmp/elytra_ms-0.4.0.tar.gz` & `tmp/elytra_ms-0.5.0.tar.gz`

## Comparing `elytra_ms-0.4.0.tar` & `elytra_ms-0.5.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 elytra_ms-0.4.0/elytra/__init__.py
--rw-r--r--   0        0        0     1328 2020-02-02 00:00:00.000000 elytra_ms-0.4.0/elytra/const.py
--rw-r--r--   0        0        0    17515 2020-02-02 00:00:00.000000 elytra_ms-0.4.0/elytra/core.py
--rw-r--r--   0        0        0     2631 2020-02-02 00:00:00.000000 elytra_ms-0.4.0/elytra/protocols.py
--rw-r--r--   0        0        0    14558 2020-02-02 00:00:00.000000 elytra_ms-0.4.0/elytra/retry_transport.py
--rw-r--r--   0        0        0     3546 2020-02-02 00:00:00.000000 elytra_ms-0.4.0/elytra/bedrock_realms/__init__.py
--rw-r--r--   0        0        0     3520 2020-02-02 00:00:00.000000 elytra_ms-0.4.0/elytra/bedrock_realms/models.py
--rw-r--r--   0        0        0     3606 2020-02-02 00:00:00.000000 elytra_ms-0.4.0/elytra/scripts/auth_device_code.py
--rw-r--r--   0        0        0     5507 2020-02-02 00:00:00.000000 elytra_ms-0.4.0/elytra/scripts/authenticate.py
--rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 elytra_ms-0.4.0/elytra/xbox/__init__.py
--rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 elytra_ms-0.4.0/elytra/xbox/core.py
--rw-r--r--   0        0        0     9968 2020-02-02 00:00:00.000000 elytra_ms-0.4.0/elytra/xbox/rta.py
--rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 elytra_ms-0.4.0/elytra/xbox/club/__init__.py
--rw-r--r--   0        0        0     5342 2020-02-02 00:00:00.000000 elytra_ms-0.4.0/elytra/xbox/club/models.py
--rw-r--r--   0        0        0     2439 2020-02-02 00:00:00.000000 elytra_ms-0.4.0/elytra/xbox/message/__init__.py
--rw-r--r--   0        0        0     3781 2020-02-02 00:00:00.000000 elytra_ms-0.4.0/elytra/xbox/message/models.py
--rw-r--r--   0        0        0     2209 2020-02-02 00:00:00.000000 elytra_ms-0.4.0/elytra/xbox/peoplehub/__init__.py
--rw-r--r--   0        0        0     7178 2020-02-02 00:00:00.000000 elytra_ms-0.4.0/elytra/xbox/peoplehub/models.py
--rw-r--r--   0        0        0     2642 2020-02-02 00:00:00.000000 elytra_ms-0.4.0/elytra/xbox/profile/__init__.py
--rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 elytra_ms-0.4.0/elytra/xbox/profile/models.py
--rw-r--r--   0        0        0     2941 2020-02-02 00:00:00.000000 elytra_ms-0.4.0/elytra/xbox/social/__init__.py
--rw-r--r--   0        0        0     3713 2020-02-02 00:00:00.000000 elytra_ms-0.4.0/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 elytra_ms-0.4.0/LICENSE
--rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 elytra_ms-0.4.0/README.md
--rw-r--r--   0        0        0     1976 2020-02-02 00:00:00.000000 elytra_ms-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     2631 2020-02-02 00:00:00.000000 elytra_ms-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 elytra_ms-0.5.0/elytra/__init__.py
+-rw-r--r--   0        0        0     1328 2020-02-02 00:00:00.000000 elytra_ms-0.5.0/elytra/const.py
+-rw-r--r--   0        0        0    17515 2020-02-02 00:00:00.000000 elytra_ms-0.5.0/elytra/core.py
+-rw-r--r--   0        0        0     2631 2020-02-02 00:00:00.000000 elytra_ms-0.5.0/elytra/protocols.py
+-rw-r--r--   0        0        0    14558 2020-02-02 00:00:00.000000 elytra_ms-0.5.0/elytra/retry_transport.py
+-rw-r--r--   0        0        0     3546 2020-02-02 00:00:00.000000 elytra_ms-0.5.0/elytra/bedrock_realms/__init__.py
+-rw-r--r--   0        0        0     3520 2020-02-02 00:00:00.000000 elytra_ms-0.5.0/elytra/bedrock_realms/models.py
+-rw-r--r--   0        0        0     3606 2020-02-02 00:00:00.000000 elytra_ms-0.5.0/elytra/scripts/auth_device_code.py
+-rw-r--r--   0        0        0     5507 2020-02-02 00:00:00.000000 elytra_ms-0.5.0/elytra/scripts/authenticate.py
+-rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 elytra_ms-0.5.0/elytra/xbox/__init__.py
+-rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 elytra_ms-0.5.0/elytra/xbox/core.py
+-rw-r--r--   0        0        0     9968 2020-02-02 00:00:00.000000 elytra_ms-0.5.0/elytra/xbox/rta.py
+-rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 elytra_ms-0.5.0/elytra/xbox/club/__init__.py
+-rw-r--r--   0        0        0     5342 2020-02-02 00:00:00.000000 elytra_ms-0.5.0/elytra/xbox/club/models.py
+-rw-r--r--   0        0        0     2929 2020-02-02 00:00:00.000000 elytra_ms-0.5.0/elytra/xbox/message/__init__.py
+-rw-r--r--   0        0        0     3798 2020-02-02 00:00:00.000000 elytra_ms-0.5.0/elytra/xbox/message/models.py
+-rw-r--r--   0        0        0     2209 2020-02-02 00:00:00.000000 elytra_ms-0.5.0/elytra/xbox/peoplehub/__init__.py
+-rw-r--r--   0        0        0     7178 2020-02-02 00:00:00.000000 elytra_ms-0.5.0/elytra/xbox/peoplehub/models.py
+-rw-r--r--   0        0        0     2642 2020-02-02 00:00:00.000000 elytra_ms-0.5.0/elytra/xbox/profile/__init__.py
+-rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 elytra_ms-0.5.0/elytra/xbox/profile/models.py
+-rw-r--r--   0        0        0     2941 2020-02-02 00:00:00.000000 elytra_ms-0.5.0/elytra/xbox/social/__init__.py
+-rw-r--r--   0        0        0     3713 2020-02-02 00:00:00.000000 elytra_ms-0.5.0/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 elytra_ms-0.5.0/LICENSE
+-rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 elytra_ms-0.5.0/README.md
+-rw-r--r--   0        0        0     1976 2020-02-02 00:00:00.000000 elytra_ms-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     2631 2020-02-02 00:00:00.000000 elytra_ms-0.5.0/PKG-INFO
```

### Comparing `elytra_ms-0.4.0/elytra/const.py` & `elytra_ms-0.5.0/elytra/const.py`

 * *Files identical despite different names*

### Comparing `elytra_ms-0.4.0/elytra/core.py` & `elytra_ms-0.5.0/elytra/core.py`

 * *Files identical despite different names*

### Comparing `elytra_ms-0.4.0/elytra/protocols.py` & `elytra_ms-0.5.0/elytra/protocols.py`

 * *Files identical despite different names*

### Comparing `elytra_ms-0.4.0/elytra/retry_transport.py` & `elytra_ms-0.5.0/elytra/retry_transport.py`

 * *Files identical despite different names*

### Comparing `elytra_ms-0.4.0/elytra/bedrock_realms/__init__.py` & `elytra_ms-0.5.0/elytra/bedrock_realms/__init__.py`

 * *Files identical despite different names*

### Comparing `elytra_ms-0.4.0/elytra/bedrock_realms/models.py` & `elytra_ms-0.5.0/elytra/bedrock_realms/models.py`

 * *Files identical despite different names*

### Comparing `elytra_ms-0.4.0/elytra/scripts/auth_device_code.py` & `elytra_ms-0.5.0/elytra/scripts/auth_device_code.py`

 * *Files identical despite different names*

### Comparing `elytra_ms-0.4.0/elytra/scripts/authenticate.py` & `elytra_ms-0.5.0/elytra/scripts/authenticate.py`

 * *Files identical despite different names*

### Comparing `elytra_ms-0.4.0/elytra/xbox/__init__.py` & `elytra_ms-0.5.0/elytra/xbox/__init__.py`

 * *Files identical despite different names*

### Comparing `elytra_ms-0.4.0/elytra/xbox/core.py` & `elytra_ms-0.5.0/elytra/xbox/core.py`

 * *Files identical despite different names*

### Comparing `elytra_ms-0.4.0/elytra/xbox/rta.py` & `elytra_ms-0.5.0/elytra/xbox/rta.py`

 * *Files identical despite different names*

### Comparing `elytra_ms-0.4.0/elytra/xbox/club/__init__.py` & `elytra_ms-0.5.0/elytra/xbox/club/__init__.py`

 * *Files identical despite different names*

### Comparing `elytra_ms-0.4.0/elytra/xbox/club/models.py` & `elytra_ms-0.5.0/elytra/xbox/club/models.py`

 * *Files identical despite different names*

### Comparing `elytra_ms-0.4.0/elytra/xbox/message/__init__.py` & `elytra_ms-0.5.0/elytra/xbox/message/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -54,14 +54,29 @@
                 URL,
                 headers=HEADERS,
                 params={"maxItems": max_items},
                 **kwargs,
             )
         )
 
+    async def fetch_folder(
+        self, folder: str = "Primary", max_items: int = 100, **kwargs: typing.Any
+    ) -> Folder:
+        URL = f"https://xblmessaging.xboxlive.com/network/Xbox/users/me/inbox/{folder}"
+        HEADERS = {"x-xbl-contract-version": "1"}
+
+        return await Folder.from_response(
+            await self.get(
+                URL,
+                headers=HEADERS,
+                params={"maxItems": max_items},
+                **kwargs,
+            )
+        )
+
     async def fetch_conversation(
         self, xuid: str | int, max_items: int = 100, **kwargs: typing.Any
     ) -> ConversationResponse:
         url = f"https://xblmessaging.xboxlive.com/network/Xbox/users/me/conversations/users/xuid({xuid})"
         HEADERS = {"x-xbl-contract-version": "1"}
 
         return await ConversationResponse.from_response(
```

### Comparing `elytra_ms-0.4.0/elytra/xbox/message/models.py` & `elytra_ms-0.5.0/elytra/xbox/message/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,15 +90,16 @@
     delete_horizon: str
     is_read: bool
     muted: bool
     folder: str
     last_message: Message
 
 
-class Folder(CamelBaseModel):
+@add_decoder
+class Folder(ParsableCamelModel):
     folder: str
     total_count: int
     unread_count: int
     conversations: typing.Optional[list[Conversation]] = None
 
 
 @add_decoder
```

### Comparing `elytra_ms-0.4.0/elytra/xbox/peoplehub/__init__.py` & `elytra_ms-0.5.0/elytra/xbox/peoplehub/__init__.py`

 * *Files identical despite different names*

### Comparing `elytra_ms-0.4.0/elytra/xbox/peoplehub/models.py` & `elytra_ms-0.5.0/elytra/xbox/peoplehub/models.py`

 * *Files identical despite different names*

### Comparing `elytra_ms-0.4.0/elytra/xbox/profile/__init__.py` & `elytra_ms-0.5.0/elytra/xbox/profile/__init__.py`

 * *Files identical despite different names*

### Comparing `elytra_ms-0.4.0/elytra/xbox/profile/models.py` & `elytra_ms-0.5.0/elytra/xbox/profile/models.py`

 * *Files identical despite different names*

### Comparing `elytra_ms-0.4.0/elytra/xbox/social/__init__.py` & `elytra_ms-0.5.0/elytra/xbox/social/__init__.py`

 * *Files identical despite different names*

### Comparing `elytra_ms-0.4.0/.gitignore` & `elytra_ms-0.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `elytra_ms-0.4.0/LICENSE` & `elytra_ms-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `elytra_ms-0.4.0/README.md` & `elytra_ms-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `elytra_ms-0.4.0/pyproject.toml` & `elytra_ms-0.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `elytra_ms-0.4.0/PKG-INFO` & `elytra_ms-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: elytra-ms
-Version: 0.4.0
+Version: 0.5.0
 Summary: A Python Library for various Microsoft APIs, including the Xbox and Bedrock Realms APIs.
 Project-URL: Homepage, https://github.com/Astrea-Stellarium-Labs/elytra-ms
 Author: AstreaTSS
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: AnyIO
```


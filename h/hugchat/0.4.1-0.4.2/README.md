# Comparing `tmp/hugchat-0.4.1.tar.gz` & `tmp/hugchat-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hugchat-0.4.1.tar", last modified: Fri Mar  8 08:33:14 2024, max compression
+gzip compressed data, was "hugchat-0.4.2.tar", last modified: Fri Apr 12 01:40:05 2024, max compression
```

## Comparing `hugchat-0.4.1.tar` & `hugchat-0.4.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 08:33:14.454427 hugchat-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-03-08 08:33:07.000000 hugchat-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6748 2024-03-08 08:33:14.454427 hugchat-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5673 2024-03-08 08:33:07.000000 hugchat-0.4.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-08 08:33:14.454427 hugchat-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-03-08 08:33:07.000000 hugchat-0.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 08:33:14.450427 hugchat-0.4.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 08:33:14.450427 hugchat-0.4.1/src/hugchat/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-08 08:33:07.000000 hugchat-0.4.1/src/hugchat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10354 2024-03-08 08:33:07.000000 hugchat-0.4.1/src/hugchat/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      853 2024-03-08 08:33:07.000000 hugchat-0.4.1/src/hugchat/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    31684 2024-03-08 08:33:07.000000 hugchat-0.4.1/src/hugchat/hugchat.py
--rw-r--r--   0 runner    (1001) docker     (127)     8561 2024-03-08 08:33:07.000000 hugchat-0.4.1/src/hugchat/login.py
--rw-r--r--   0 runner    (1001) docker     (127)     7184 2024-03-08 08:33:07.000000 hugchat-0.4.1/src/hugchat/message.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 08:33:14.450427 hugchat-0.4.1/src/hugchat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6748 2024-03-08 08:33:14.000000 hugchat-0.4.1/src/hugchat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-03-08 08:33:14.000000 hugchat-0.4.1/src/hugchat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-08 08:33:14.000000 hugchat-0.4.1/src/hugchat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-03-08 08:33:14.000000 hugchat-0.4.1/src/hugchat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-08 08:33:14.000000 hugchat-0.4.1/src/hugchat.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 01:40:05.327504 hugchat-0.4.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-04-12 01:40:01.000000 hugchat-0.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6804 2024-04-12 01:40:05.327504 hugchat-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5729 2024-04-12 01:40:01.000000 hugchat-0.4.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 01:40:05.327504 hugchat-0.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-04-12 01:40:01.000000 hugchat-0.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 01:40:05.323504 hugchat-0.4.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 01:40:05.323504 hugchat-0.4.2/src/hugchat/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 01:40:01.000000 hugchat-0.4.2/src/hugchat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10354 2024-04-12 01:40:01.000000 hugchat-0.4.2/src/hugchat/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-04-12 01:40:01.000000 hugchat-0.4.2/src/hugchat/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31684 2024-04-12 01:40:01.000000 hugchat-0.4.2/src/hugchat/hugchat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8561 2024-04-12 01:40:01.000000 hugchat-0.4.2/src/hugchat/login.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7567 2024-04-12 01:40:01.000000 hugchat-0.4.2/src/hugchat/message.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 01:40:05.327504 hugchat-0.4.2/src/hugchat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6804 2024-04-12 01:40:05.000000 hugchat-0.4.2/src/hugchat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-12 01:40:05.000000 hugchat-0.4.2/src/hugchat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 01:40:05.000000 hugchat-0.4.2/src/hugchat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-12 01:40:05.000000 hugchat-0.4.2/src/hugchat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-12 01:40:05.000000 hugchat-0.4.2/src/hugchat.egg-info/top_level.txt
```

### Comparing `hugchat-0.4.1/LICENSE` & `hugchat-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hugchat-0.4.1/PKG-INFO` & `hugchat-0.4.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hugchat
-Version: 0.4.1
+Version: 0.4.2
 Summary: A huggingchat python api.
 Home-page: https://github.com/Soulter/hugging-chat-api
 Author: Soulter
 Author-email: 905617992@qq.com
 License: GNU Affero General Public License v3.0
 Project-URL: Bug Report, https://github.com/Soulter/hugging-chat-api/issues
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -62,15 +62,15 @@
 ```py
 from hugchat import hugchat
 from hugchat.login import Login
 
 # Log in to huggingface and grant authorization to huggingchat
 EMAIL = "your email"
 PASSWD = "your password"
-cookie_path_dir = "./cookies"
+cookie_path_dir = "./cookies/" # NOTE: trailing slash (/) is required to avoid errors
 sign = Login(EMAIL, PASSWD)
 cookies = sign.login(cookie_dir_path=cookie_path_dir, save_cookies=True)
 
 # Create your ChatBot
 chatbot = hugchat.ChatBot(cookies=cookies.get_dict())  # or cookie_path="usercookies/<email>.json"
 
 # Non stream response
```

### Comparing `hugchat-0.4.1/README.md` & `hugchat-0.4.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 ```py
 from hugchat import hugchat
 from hugchat.login import Login
 
 # Log in to huggingface and grant authorization to huggingchat
 EMAIL = "your email"
 PASSWD = "your password"
-cookie_path_dir = "./cookies"
+cookie_path_dir = "./cookies/" # NOTE: trailing slash (/) is required to avoid errors
 sign = Login(EMAIL, PASSWD)
 cookies = sign.login(cookie_dir_path=cookie_path_dir, save_cookies=True)
 
 # Create your ChatBot
 chatbot = hugchat.ChatBot(cookies=cookies.get_dict())  # or cookie_path="usercookies/<email>.json"
 
 # Non stream response
```

### Comparing `hugchat-0.4.1/setup.py` & `hugchat-0.4.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import find_namespace_packages
 from setuptools import setup
 
 setup(
     name="hugchat",
-    version="0.4.1",
+    version="0.4.2",
     description="A huggingchat python api.",
     long_description=open("README.md", "rt", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/Soulter/hugging-chat-api",
     project_urls={
         "Bug Report": "https://github.com/Soulter/hugging-chat-api/issues"
     },
```

### Comparing `hugchat-0.4.1/src/hugchat/cli.py` & `hugchat-0.4.2/src/hugchat/cli.py`

 * *Files identical despite different names*

### Comparing `hugchat-0.4.1/src/hugchat/exceptions.py` & `hugchat-0.4.2/src/hugchat/exceptions.py`

 * *Files identical despite different names*

### Comparing `hugchat-0.4.1/src/hugchat/hugchat.py` & `hugchat-0.4.2/src/hugchat/hugchat.py`

 * *Files identical despite different names*

### Comparing `hugchat-0.4.1/src/hugchat/login.py` & `hugchat-0.4.2/src/hugchat/login.py`

 * *Files identical despite different names*

### Comparing `hugchat-0.4.1/src/hugchat/message.py` & `hugchat-0.4.2/src/hugchat/message.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,36 +1,34 @@
 from typing import Generator, Union
 
 from .exceptions import ChatError, ModelOverloadedError
 import json
 
-
-MSGTYPE_FINAL = "finalAnswer"
-MSGTYPE_STREAM = "stream"
-MSGTYPE_WEB = "webSearch"
-MSGTYPE_STATUS = "status"
+RESPONSE_TYPE_FINAL = "finalAnswer"
+RESPONSE_TYPE_STREAM = "stream"
+RESPONSE_TYPE_WEB = "webSearch"
+RESPONSE_TYPE_STATUS = "status"
+MSGTYPE_ERROR = "error"
 
 MSGSTATUS_PENDING = 0
 MSGSTATUS_RESOLVED = 1
 MSGSTATUS_REJECTED = 2
 
 
 class WebSearchSource:
     title: str
     link: str
     hostname: str
 
     def __str__(self):
-        return json.dumps(
-            {
-                "title": self.title,
-                "link": self.link,
-                "hostname": self.hostname,
-            }
-        )
+        return json.dumps({
+            "title": self.title,
+            "link": self.link,
+            "hostname": self.hostname,
+        })
 
 
 class Message(Generator):
     """
     :Args:
         * g: Generator
         * _stream_yield_all: bool = False
@@ -89,62 +87,68 @@
     def __next__(self) -> dict:
         if self.msg_status == MSGSTATUS_RESOLVED:
             raise StopIteration
         elif self.msg_status == MSGSTATUS_REJECTED:
             if self.error is not None:
                 raise self.error
             else:
-                raise Exception("Message stauts is `Rejected` but no error found")
+                raise Exception(
+                    "Message stauts is `Rejected` but no error found")
 
         try:
             a: dict = next(self.g)
             self._filterResponse(a)
             t: str = a["type"]
             message_type: str = ""
-            if "messageType" in a:
-                message_type: str = a["messageType"]
-            if message_type == "error":
-                self.error = ChatError(a["message"])
-                self.msg_status = MSGSTATUS_REJECTED
-            if t == MSGTYPE_STREAM:
-                self.web_search_done = True
-            elif t == MSGTYPE_STATUS:
-                pass
-            elif t == MSGTYPE_FINAL:
+            if t == RESPONSE_TYPE_FINAL:
                 self.text = a["text"]
                 self.msg_status = MSGSTATUS_RESOLVED
-            elif t == MSGTYPE_WEB:
-                if a.__contains__("sources"):
+            elif t == RESPONSE_TYPE_WEB:
+                # gracefully pass unparseable webpages
+                if message_type != MSGTYPE_ERROR and a.__contains__("sources"):
                     self.web_search_sources.clear()
                     sources = a["sources"]
                     for source in sources:
                         wss = WebSearchSource()
                         wss.title = source["title"]
                         wss.link = source["link"]
                         wss.hostname = source["hostname"]
                         self.web_search_sources.append(wss)
+            elif "messageType" in a:
+                message_type: str = a["messageType"]
+                if message_type == MSGTYPE_ERROR:
+                    self.error = ChatError(a["message"])
+                    self.msg_status = MSGSTATUS_REJECTED
+                if t == RESPONSE_TYPE_STREAM:
+                    self.web_search_done = True
+                elif t == RESPONSE_TYPE_STATUS:
+                    pass
             else:
                 if "Model is overloaded" in str(a):
                     self.error = ModelOverloadedError(
                         "Model is overloaded, please try again later or switch to another model."
                     )
                     self.msg_status = MSGSTATUS_REJECTED
-                elif a.__contains__("error"):
-                    self.error = ChatError(a["error"])
+                elif a.__contains__(MSGTYPE_ERROR):
+                    self.error = ChatError(a[MSGTYPE_ERROR])
                     self.msg_status = MSGSTATUS_REJECTED
                 else:
                     self.error = ChatError(f"Unknown json response: {a}")
 
             # If _stream_yield_all is True, yield all responses from the server.
-            if self._stream_yield_all or t == MSGTYPE_STREAM:
+            if self._stream_yield_all or t == RESPONSE_TYPE_STREAM:
                 return a
             else:
                 return self.__next__()
         except StopIteration:
-            # print("meet stop:", self.msg_status)
+            if self.msg_status == MSGSTATUS_PENDING:
+                self.error = ChatError(
+                    "Stream of responses has abruptly ended (final answer has not been received)."
+                )
+                raise self.error
             pass
         except Exception as e:
             # print("meet error: ", str(e))
             self.error = e
             self.msg_status = MSGSTATUS_REJECTED
             raise self.error
 
@@ -215,15 +219,15 @@
         """
         :Return:
             - self.web_search_done
 
         web search result will be set to `done` once the token is received
         """
         return self.web_search_done
-    
+
     def __str__(self):
         return self.wait_until_done()
 
     def __getitem__(self, key: str) -> str:
         print("_getitem_")
         self.wait_until_done()
         print("done")
```

### Comparing `hugchat-0.4.1/src/hugchat.egg-info/PKG-INFO` & `hugchat-0.4.2/src/hugchat.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hugchat
-Version: 0.4.1
+Version: 0.4.2
 Summary: A huggingchat python api.
 Home-page: https://github.com/Soulter/hugging-chat-api
 Author: Soulter
 Author-email: 905617992@qq.com
 License: GNU Affero General Public License v3.0
 Project-URL: Bug Report, https://github.com/Soulter/hugging-chat-api/issues
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -62,15 +62,15 @@
 ```py
 from hugchat import hugchat
 from hugchat.login import Login
 
 # Log in to huggingface and grant authorization to huggingchat
 EMAIL = "your email"
 PASSWD = "your password"
-cookie_path_dir = "./cookies"
+cookie_path_dir = "./cookies/" # NOTE: trailing slash (/) is required to avoid errors
 sign = Login(EMAIL, PASSWD)
 cookies = sign.login(cookie_dir_path=cookie_path_dir, save_cookies=True)
 
 # Create your ChatBot
 chatbot = hugchat.ChatBot(cookies=cookies.get_dict())  # or cookie_path="usercookies/<email>.json"
 
 # Non stream response
```


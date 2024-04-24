# Comparing `tmp/simple_rule34-0.1.5.5.tar.gz` & `tmp/simple_rule34-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\alexk\PycharmProjects\rule34-simple-api\SimpleRule34\dist\.tmp-yrw9xco7\simple_rule34-0.1.5.5.tar", last modified: Tue Apr 23 10:54:37 2024, max compression
+gzip compressed data, was "C:\Users\alexk\PycharmProjects\rule34-simple-api\SimpleRule34\dist\.tmp-sqz1x8v7\simple_rule34-0.1.6.tar", last modified: Wed Apr 24 16:06:02 2024, max compression
```

## Comparing `simple_rule34-0.1.5.5.tar` & `simple_rule34-0.1.6.tar`

### file list

```diff
@@ -1,26 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-04-23 10:54:37.480847 simple_rule34-0.1.5.5/
--rw-rw-rw-   0        0        0     1091 2023-07-16 23:21:11.000000 simple_rule34-0.1.5.5/LICENSE
--rw-rw-rw-   0        0        0     2083 2024-04-23 10:54:37.479850 simple_rule34-0.1.5.5/PKG-INFO
--rw-rw-rw-   0        0        0       92 2023-07-16 23:04:58.000000 simple_rule34-0.1.5.5/README.md
--rw-rw-rw-   0        0        0     1759 2024-04-23 10:54:19.000000 simple_rule34-0.1.5.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-23 10:54:37.480847 simple_rule34-0.1.5.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-23 10:54:37.425475 simple_rule34-0.1.5.5/src/
-drwxrwxrwx   0        0        0        0 2024-04-23 10:54:37.448416 simple_rule34-0.1.5.5/src/SimpleRule34/
--rw-rw-rw-   0        0        0     7136 2024-01-01 18:44:36.000000 simple_rule34-0.1.5.5/src/SimpleRule34/Rule34.py
--rw-rw-rw-   0        0        0       31 2023-07-16 22:47:21.000000 simple_rule34-0.1.5.5/src/SimpleRule34/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-23 10:54:37.452408 simple_rule34-0.1.5.5/src/SimpleRule34/aio/
--rw-rw-rw-   0        0        0     6858 2024-01-01 18:44:36.000000 simple_rule34-0.1.5.5/src/SimpleRule34/aio/ARule34.py
--rw-rw-rw-   0        0        0     3719 2024-04-23 10:53:50.000000 simple_rule34-0.1.5.5/src/SimpleRule34/aio/types.py
--rw-rw-rw-   0        0        0      616 2024-01-01 18:44:36.000000 simple_rule34-0.1.5.5/src/SimpleRule34/aio/utils.py
--rw-rw-rw-   0        0        0      354 2023-07-16 22:41:52.000000 simple_rule34-0.1.5.5/src/SimpleRule34/exceptions.py
--rw-rw-rw-   0        0        0      735 2023-07-16 23:11:26.000000 simple_rule34-0.1.5.5/src/SimpleRule34/setup.py
--rw-rw-rw-   0        0        0     3278 2024-01-01 18:44:36.000000 simple_rule34-0.1.5.5/src/SimpleRule34/types.py
--rw-rw-rw-   0        0        0      854 2024-01-01 18:44:36.000000 simple_rule34-0.1.5.5/src/SimpleRule34/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-23 10:54:37.477854 simple_rule34-0.1.5.5/src/simple_rule34.egg-info/
--rw-rw-rw-   0        0        0     2083 2024-04-23 10:54:37.000000 simple_rule34-0.1.5.5/src/simple_rule34.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      507 2024-04-23 10:54:37.000000 simple_rule34-0.1.5.5/src/simple_rule34.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-23 10:54:37.000000 simple_rule34-0.1.5.5/src/simple_rule34.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      764 2024-04-23 10:54:37.000000 simple_rule34-0.1.5.5/src/simple_rule34.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-04-23 10:54:37.000000 simple_rule34-0.1.5.5/src/simple_rule34.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-23 10:54:37.476857 simple_rule34-0.1.5.5/tests/
--rw-rw-rw-   0        0        0     1547 2024-01-01 18:44:36.000000 simple_rule34-0.1.5.5/tests/test.py
+drwxrwxrwx   0        0        0        0 2024-04-24 16:06:02.353770 simple_rule34-0.1.6/
+-rw-rw-rw-   0        0        0     1091 2023-07-16 23:21:11.000000 simple_rule34-0.1.6/LICENSE
+-rw-rw-rw-   0        0        0     2113 2024-04-24 16:06:02.353770 simple_rule34-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0       92 2023-07-16 23:04:58.000000 simple_rule34-0.1.6/README.md
+-rw-rw-rw-   0        0        0     1793 2024-04-24 16:05:04.000000 simple_rule34-0.1.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-24 16:06:02.354779 simple_rule34-0.1.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-24 16:06:02.330156 simple_rule34-0.1.6/src/
+drwxrwxrwx   0        0        0        0 2024-04-24 16:06:02.335727 simple_rule34-0.1.6/src/SimpleRule34/
+-rw-rw-rw-   0        0        0     5433 2024-04-24 16:05:49.000000 simple_rule34-0.1.6/src/SimpleRule34/Rule34.py
+-rw-rw-rw-   0        0        0       31 2023-07-16 22:47:21.000000 simple_rule34-0.1.6/src/SimpleRule34/__init__.py
+-rw-rw-rw-   0        0        0      491 2024-04-24 15:35:47.000000 simple_rule34-0.1.6/src/SimpleRule34/exceptions.py
+-rw-rw-rw-   0        0        0     1518 2024-04-24 16:03:47.000000 simple_rule34-0.1.6/src/SimpleRule34/types.py
+-rw-rw-rw-   0        0        0      616 2024-01-01 18:44:36.000000 simple_rule34-0.1.6/src/SimpleRule34/utils.py
+-rw-rw-rw-   0        0        0        0 2024-04-24 14:18:41.000000 simple_rule34-0.1.6/src/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 16:06:02.352264 simple_rule34-0.1.6/src/simple_rule34.egg-info/
+-rw-rw-rw-   0        0        0     2113 2024-04-24 16:06:02.000000 simple_rule34-0.1.6/src/simple_rule34.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      405 2024-04-24 16:06:02.000000 simple_rule34-0.1.6/src/simple_rule34.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 16:06:02.000000 simple_rule34-0.1.6/src/simple_rule34.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      780 2024-04-24 16:06:02.000000 simple_rule34-0.1.6/src/simple_rule34.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2024-04-24 16:06:02.000000 simple_rule34-0.1.6/src/simple_rule34.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-24 16:06:02.351276 simple_rule34-0.1.6/tests/
+-rw-rw-rw-   0        0        0      931 2024-04-24 16:01:38.000000 simple_rule34-0.1.6/tests/test.py
```

### Comparing `simple_rule34-0.1.5.5/LICENSE` & `simple_rule34-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `simple_rule34-0.1.5.5/PKG-INFO` & `simple_rule34-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple_rule34
-Version: 0.1.5.5
+Version: 0.1.6
 Summary: Simple api wrapper of rule34.xxx for python with asynchronous support
 Author-email: StarMan12 <author@example.com>
 Project-URL: Homepage, https://github.com/SyperAlexKomp/simple-rule34-api
 Project-URL: Bug Tracker, https://github.com/SyperAlexKomp/simple-rule34-api/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -47,10 +47,11 @@
 Requires-Dist: sphinxcontrib-serializinghtml==1.1.5
 Requires-Dist: tomli==2.0.1
 Requires-Dist: urllib3==2.0.3
 Requires-Dist: yarg==0.1.9
 Requires-Dist: yarl==1.9.2
 Requires-Dist: zipp==3.16.2
 Requires-Dist: aiofiles~=23.2.1
+Requires-Dist: pydantic~=2.7.1
 
 # rule34-simple-api
 Simple api wrapper of rule34.xxx for python with asynchronous support
```

### Comparing `simple_rule34-0.1.5.5/pyproject.toml` & `simple_rule34-0.1.6/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "simple_rule34"
-version = "0.1.5.5"
+version = "0.1.6"
 authors = [
   { name="StarMan12", email="author@example.com" },
 ]
 description = "Simple api wrapper of rule34.xxx for python with asynchronous support"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
-dependencies = ['aiohttp==3.8.4',
+dependencies = [
+    'aiohttp==3.8.4',
     'aiosignal==1.3.1',
     'alabaster==0.7.13',
     'async-timeout==4.0.2',
     'attrs==23.1.0',
     'Babel==2.9.1',
     'build==0.10.0',
     'certifi==2023.5.7',
@@ -51,12 +52,14 @@
     'sphinxcontrib-qthelp==1.0.3',
     'sphinxcontrib-serializinghtml==1.1.5',
     'tomli==2.0.1',
     'urllib3==2.0.3',
     'yarg==0.1.9',
     'yarl==1.9.2',
     'zipp==3.16.2',
-'aiofiles~=23.2.1']
+    'aiofiles~=23.2.1',
+    'pydantic~=2.7.1'
+]
 
 [project.urls]
 "Homepage" = "https://github.com/SyperAlexKomp/simple-rule34-api"
 "Bug Tracker" = "https://github.com/SyperAlexKomp/simple-rule34-api/issues"
```

### Comparing `simple_rule34-0.1.5.5/src/SimpleRule34/aio/ARule34.py` & `simple_rule34-0.1.6/src/SimpleRule34/Rule34.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,94 +2,57 @@
 import time
 
 import aiohttp
 import datetime
 import logging
 import xml.etree.ElementTree as ET
 
-from ..exceptions import *
+from .exceptions import *
 from .types import *
 
 
-async def parse_result(post_element):
-
-
-    id = int(post_element.get('id'))
-    height = int(post_element.get('height'))
-    width = int(post_element.get('width'))
-    url = post_element.get('file_url')
-
-    sample_height = int(post_element.get('sample_height'))
-    sample_width = int(post_element.get('sample_width'))
-    sample_url = post_element.get('sample_url')
-
-    sample_post = Rule34SamplePost(sample_height, sample_width, sample_url, id)
-
-    preview_height = int(post_element.get('preview_height'))
-    preview_width = int(post_element.get('preview_width'))
-    preview_url = post_element.get('preview_url')
-
-    preview_post = Rule34PreviewPost(preview_height, preview_width, preview_url, id)
-
-    score = int(post_element.get('score'))
-    rating = post_element.get('rating')
-    creator_id = int(post_element.get('creator_id'))
-    tags = post_element.get('tags')
-    has_children = post_element.get('has_children') == 'true'
-    created_date = datetime.datetime.strptime(post_element.get('created_at'), "%a %b %d %H:%M:%S %z %Y")
-    status = post_element.get('status')
-    source = post_element.get('source')
-    has_notes = post_element.get('has_notes') == 'true'
-    has_comments = post_element.get('has_comments') == 'true'
-
-    main_post = Rule34MainPost(score, rating, creator_id, tags, has_children, created_date, status,
-                               source, has_notes, has_comments, height, width, url, id)
-
-    return main_post, sample_post, preview_post
-
 class Rule34Api:
     def __init__(self):
-        self.header = {'User-Agent': 'rule34-simple-api 0.1.5.3 (Request)'}
+        self.header = {'User-Agent': 'rule34-simple-api 0.1.5.6 (Request)'}
     async def get_post_count(self, tags: str = '') -> int:
         async with aiohttp.ClientSession(headers=self.header) as session:
             async with session.get(f'https://api.rule34.xxx/index.php?'
                                    f'page=dapi&s=post&q=index&tags={tags}') as response:
                 xml_data = await response.text()
 
         xml_root = ET.fromstring(xml_data)
 
         return int(xml_root.get('count'))
 
-    async def get_post(self, id: int):
+    async def get_post(self, id: int) -> Post:
         st = time.time()
 
         async with aiohttp.ClientSession(headers=self.header) as session:
             async with session.get(f'https://api.rule34.xxx/index.php?'
-                                   f'page=dapi&s=post&q=index&id={id}') as response:
-                xml_data = await response.text()
-
-        try:
-            xml_root = ET.fromstring(xml_data)
-        except:
-            return None
-
-        post_element = xml_root.find('post')
+                                   f'json=1&page=dapi&s=post&q=index&id={id}') as response:
+                if response.status != 200:
+                    raise ApiException(f"Api returned status code {response.status} with message"
+                                       f" {await response.text()}")
+
+                j = await response.json()
+                data = j[0]
+
+        data["main"] = {
+            "url": data['file_url']
+        }
+        data["preview"] = {
+            "url": data['preview_url']
+        }
+        data["tags"] = data["tags"].split(" ")
 
-        parsed = await parse_result(post_element)
+        logging.debug(f"Post[{id}] where found in {time.time() - st}s")
 
-        if parsed is None:
-            return None
-        else:
-            main_post, sample_post, preview_post = parsed
-
-        logging.info(f"Post where found in {time.time() - st}s")
+        return Post(**data)
 
-        return Rule34PostData(id, main_post, sample_post, preview_post)
-
-    async def get_random_post(self, tags: str = '', forbidden_tags: list[str] = []):
+    async def get_random_post(self, tags: str = '', forbidden_tags: list[str] = []) -> Post:
         start_time = time.time()
 
         post_count = await self.get_post_count(tags)
 
         page_count = post_count // 1000
 
         if page_count > 0:
@@ -103,19 +66,19 @@
 
         for post in post_list:
             if any(tag in forbidden_tags for tag in post.main.tags):
                 pass
             else:
                 post_list_.append(post)
 
-        logging.info(f"Random post where found in {time.time() - start_time}s")
+        logging.debug(f"Random posts where found in {time.time() - start_time}s")
 
         return post_list_[random.randint(0, len(post_list_) - 1)] if len(post_list_) > 0 else None
 
-    async def get_random_posts(self, tags: str = '', count: int = 8, forbidden_tags: list[str] = []) -> list[Rule34PostData]:
+    async def get_random_posts(self, tags: str = '', count: int = 8, forbidden_tags: list[str] = []) -> list[Post]:
         st = time.time()
 
         request_count = 1
         true_count = count*20
 
         post_list = []
 
@@ -133,54 +96,54 @@
 
         for x in range(count):
             if len(post_list) > 0:
                 getted.append(post_list[random.randint(0, len(post_list) - 1)])
             else:
                 pass
 
-        logging.info(f"{count} random posts where found in {time.time() - st}s")
+        logging.debug(f"{count} random posts where found in {time.time() - st}s")
 
         return getted
 
     async def get_post_list(self, limit: int = 1000, page_id: int = 0, tags: str = '', forbidden_tags: list[str] = [])\
-            -> list[Rule34PostData]:
-        async with aiohttp.ClientSession(headers=self.header) as session:
-            if limit > 1000:
-                raise ToBigRequestException(f"The max size of request is 1000 when you tried to request {limit}")
+            -> list[Post]:
+        if limit > 1000:
+            raise ToBigRequestException(f"The max size of request is 1000 when you tried to request {limit}")
 
+        async with aiohttp.ClientSession(headers=self.header) as session:
             start_time = time.time()
 
             async with session.get(f'https://api.rule34.xxx/index.php?'
-                                   f'page=dapi&s=post&q=index&limit={limit}&pid={page_id}&tags={tags}') as response:
-                xml_data = await response.text()
+                                   f'json=1&page=dapi&s=post&q=index&limit={limit}&pid={page_id}&tags={tags}') as response:
+                if response.status != 200:
+                    raise ApiException(f"Api returned status code {response.status} with message"
+                                       f" {await response.text()}")
+
+                data = await response.json()
 
             logging.debug(f"Request with {limit} limit posts were done in {time.time() - start_time}s")
 
-            xml_root = ET.fromstring(xml_data)
-            posts = xml_root.findall('post')
             post_list = []
+            for post_data in data:
+                post_data["main"] = {
+                    "url": post_data['file_url']
+                }
+                post_data["preview"] = {
+                    "url": post_data['preview_url']
+                }
+                post_data["tags"] = post_data["tags"].split(" ")
 
-            start_time = time.time()
-
-            for post_element in posts:
-                parsed = await parse_result(post_element)
-
-                if parsed is None:
-                    return []
-                else:
-                    main_post, sample_post, preview_post = parsed
-
-                post_list.append(Rule34PostData(main_post.id, main_post, sample_post, preview_post))
+                post_list.append(Post(**post_data))
 
-            logging.debug(f"Creating {len(posts)} objects was done in {time.time() - start_time}s")
+            start_time = time.time()
 
             post_list_ = []
 
             for post in post_list:
-                if any(tag in forbidden_tags for tag in post.main.tags):
+                if any(tag in forbidden_tags for tag in post.tags):
                     pass
                 else:
                     post_list_.append(post)
 
-            logging.info(f"{len(post_list_)} posts where found in {time.time() - start_time}s")
+            logging.debug(f"{len(post_list_)} posts where found in {time.time() - start_time}s")
 
             return post_list_
```

### Comparing `simple_rule34-0.1.5.5/src/SimpleRule34/aio/utils.py` & `simple_rule34-0.1.6/src/SimpleRule34/utils.py`

 * *Files identical despite different names*

### Comparing `simple_rule34-0.1.5.5/src/simple_rule34.egg-info/PKG-INFO` & `simple_rule34-0.1.6/src/simple_rule34.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple_rule34
-Version: 0.1.5.5
+Version: 0.1.6
 Summary: Simple api wrapper of rule34.xxx for python with asynchronous support
 Author-email: StarMan12 <author@example.com>
 Project-URL: Homepage, https://github.com/SyperAlexKomp/simple-rule34-api
 Project-URL: Bug Tracker, https://github.com/SyperAlexKomp/simple-rule34-api/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -47,10 +47,11 @@
 Requires-Dist: sphinxcontrib-serializinghtml==1.1.5
 Requires-Dist: tomli==2.0.1
 Requires-Dist: urllib3==2.0.3
 Requires-Dist: yarg==0.1.9
 Requires-Dist: yarl==1.9.2
 Requires-Dist: zipp==3.16.2
 Requires-Dist: aiofiles~=23.2.1
+Requires-Dist: pydantic~=2.7.1
 
 # rule34-simple-api
 Simple api wrapper of rule34.xxx for python with asynchronous support
```

### Comparing `simple_rule34-0.1.5.5/src/simple_rule34.egg-info/requires.txt` & `simple_rule34-0.1.6/src/simple_rule34.egg-info/requires.txt`

 * *Files 16% similar despite different names*

```diff
@@ -34,7 +34,8 @@
 sphinxcontrib-serializinghtml==1.1.5
 tomli==2.0.1
 urllib3==2.0.3
 yarg==0.1.9
 yarl==1.9.2
 zipp==3.16.2
 aiofiles~=23.2.1
+pydantic~=2.7.1
```


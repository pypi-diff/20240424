# Comparing `tmp/chamco_ragbot-0.1.8.tar.gz` & `tmp/chamco_ragbot-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chamco_ragbot-0.1.8.tar", last modified: Fri Apr 19 07:45:52 2024, max compression
+gzip compressed data, was "chamco_ragbot-0.1.9.tar", last modified: Fri Apr 19 09:00:27 2024, max compression
```

## Comparing `chamco_ragbot-0.1.8.tar` & `chamco_ragbot-0.1.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 azureuser  (1000) azureuser  (1000)        0 2024-04-19 07:45:52.085364 chamco_ragbot-0.1.8/
--rw-r--r--   0 azureuser  (1000) azureuser  (1000)      108 2024-04-19 07:45:52.085364 chamco_ragbot-0.1.8/PKG-INFO
-drwxrwxr-x   0 azureuser  (1000) azureuser  (1000)        0 2024-04-19 07:45:52.081364 chamco_ragbot-0.1.8/chamco_ragbot/
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)        0 2024-04-18 14:27:21.000000 chamco_ragbot-0.1.8/chamco_ragbot/__init__.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     3284 2024-04-19 06:34:49.000000 chamco_ragbot-0.1.8/chamco_ragbot/acl.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     2075 2024-04-18 14:27:21.000000 chamco_ragbot-0.1.8/chamco_ragbot/chat.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     1933 2024-04-19 03:12:20.000000 chamco_ragbot-0.1.8/chamco_ragbot/datasource.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     1739 2024-04-19 03:45:28.000000 chamco_ragbot-0.1.8/chamco_ragbot/dept.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     2117 2024-04-18 14:27:21.000000 chamco_ragbot-0.1.8/chamco_ragbot/filetransfer.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     6212 2024-04-19 03:26:57.000000 chamco_ragbot-0.1.8/chamco_ragbot/index.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     2477 2024-04-18 14:27:21.000000 chamco_ragbot-0.1.8/chamco_ragbot/indexer.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     2320 2024-04-19 07:45:14.000000 chamco_ragbot-0.1.8/chamco_ragbot/main.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     4195 2024-04-18 14:27:21.000000 chamco_ragbot-0.1.8/chamco_ragbot/search.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     3663 2024-04-18 14:27:21.000000 chamco_ragbot-0.1.8/chamco_ragbot/skillset.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)      892 2024-04-19 03:28:31.000000 chamco_ragbot-0.1.8/chamco_ragbot/utils.py
-drwxrwxr-x   0 azureuser  (1000) azureuser  (1000)        0 2024-04-19 07:45:52.081364 chamco_ragbot-0.1.8/chamco_ragbot.egg-info/
--rw-r--r--   0 azureuser  (1000) azureuser  (1000)      108 2024-04-19 07:45:52.000000 chamco_ragbot-0.1.8/chamco_ragbot.egg-info/PKG-INFO
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)      448 2024-04-19 07:45:52.000000 chamco_ragbot-0.1.8/chamco_ragbot.egg-info/SOURCES.txt
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)        1 2024-04-19 07:45:52.000000 chamco_ragbot-0.1.8/chamco_ragbot.egg-info/dependency_links.txt
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)       14 2024-04-19 07:45:52.000000 chamco_ragbot-0.1.8/chamco_ragbot.egg-info/top_level.txt
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)       38 2024-04-19 07:45:52.085364 chamco_ragbot-0.1.8/setup.cfg
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)      268 2024-04-19 07:45:38.000000 chamco_ragbot-0.1.8/setup.py
+drwxrwxr-x   0 azureuser  (1000) azureuser  (1000)        0 2024-04-19 09:00:27.384796 chamco_ragbot-0.1.9/
+-rw-r--r--   0 azureuser  (1000) azureuser  (1000)      108 2024-04-19 09:00:27.384796 chamco_ragbot-0.1.9/PKG-INFO
+drwxrwxr-x   0 azureuser  (1000) azureuser  (1000)        0 2024-04-19 09:00:27.384796 chamco_ragbot-0.1.9/chamco_ragbot/
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)        0 2024-04-18 14:27:21.000000 chamco_ragbot-0.1.9/chamco_ragbot/__init__.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     3284 2024-04-19 06:34:49.000000 chamco_ragbot-0.1.9/chamco_ragbot/acl.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     2075 2024-04-18 14:27:21.000000 chamco_ragbot-0.1.9/chamco_ragbot/chat.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     1933 2024-04-19 03:12:20.000000 chamco_ragbot-0.1.9/chamco_ragbot/datasource.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     1739 2024-04-19 03:45:28.000000 chamco_ragbot-0.1.9/chamco_ragbot/dept.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     2117 2024-04-18 14:27:21.000000 chamco_ragbot-0.1.9/chamco_ragbot/filetransfer.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     6212 2024-04-19 03:26:57.000000 chamco_ragbot-0.1.9/chamco_ragbot/index.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     2477 2024-04-18 14:27:21.000000 chamco_ragbot-0.1.9/chamco_ragbot/indexer.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     2624 2024-04-19 09:00:10.000000 chamco_ragbot-0.1.9/chamco_ragbot/main.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     4195 2024-04-18 14:27:21.000000 chamco_ragbot-0.1.9/chamco_ragbot/search.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     3663 2024-04-18 14:27:21.000000 chamco_ragbot-0.1.9/chamco_ragbot/skillset.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)      892 2024-04-19 03:28:31.000000 chamco_ragbot-0.1.9/chamco_ragbot/utils.py
+drwxrwxr-x   0 azureuser  (1000) azureuser  (1000)        0 2024-04-19 09:00:27.384796 chamco_ragbot-0.1.9/chamco_ragbot.egg-info/
+-rw-r--r--   0 azureuser  (1000) azureuser  (1000)      108 2024-04-19 09:00:27.000000 chamco_ragbot-0.1.9/chamco_ragbot.egg-info/PKG-INFO
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)      448 2024-04-19 09:00:27.000000 chamco_ragbot-0.1.9/chamco_ragbot.egg-info/SOURCES.txt
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)        1 2024-04-19 09:00:27.000000 chamco_ragbot-0.1.9/chamco_ragbot.egg-info/dependency_links.txt
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)       14 2024-04-19 09:00:27.000000 chamco_ragbot-0.1.9/chamco_ragbot.egg-info/top_level.txt
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)       38 2024-04-19 09:00:27.384796 chamco_ragbot-0.1.9/setup.cfg
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)      268 2024-04-19 08:59:33.000000 chamco_ragbot-0.1.9/setup.py
```

### Comparing `chamco_ragbot-0.1.8/chamco_ragbot/acl.py` & `chamco_ragbot-0.1.9/chamco_ragbot/acl.py`

 * *Files identical despite different names*

### Comparing `chamco_ragbot-0.1.8/chamco_ragbot/chat.py` & `chamco_ragbot-0.1.9/chamco_ragbot/chat.py`

 * *Files identical despite different names*

### Comparing `chamco_ragbot-0.1.8/chamco_ragbot/datasource.py` & `chamco_ragbot-0.1.9/chamco_ragbot/datasource.py`

 * *Files identical despite different names*

### Comparing `chamco_ragbot-0.1.8/chamco_ragbot/dept.py` & `chamco_ragbot-0.1.9/chamco_ragbot/dept.py`

 * *Files identical despite different names*

### Comparing `chamco_ragbot-0.1.8/chamco_ragbot/filetransfer.py` & `chamco_ragbot-0.1.9/chamco_ragbot/filetransfer.py`

 * *Files identical despite different names*

### Comparing `chamco_ragbot-0.1.8/chamco_ragbot/index.py` & `chamco_ragbot-0.1.9/chamco_ragbot/index.py`

 * *Files identical despite different names*

### Comparing `chamco_ragbot-0.1.8/chamco_ragbot/indexer.py` & `chamco_ragbot-0.1.9/chamco_ragbot/indexer.py`

 * *Files identical despite different names*

### Comparing `chamco_ragbot-0.1.8/chamco_ragbot/main.py` & `chamco_ragbot-0.1.9/chamco_ragbot/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import os
 import asyncio
 
 from dotenv import load_dotenv
 load_dotenv()
 
-# import sys
-# sys.path.append('./chamco_ragbot')
+import sys
+sys.path.append('/home/azureuser/projects/rag_chatbot/src/chamco_ragbot')
+
 
 import logging
 
 # Configure logging
 logging.basicConfig(level=logging.INFO, format='%(asctime)s - %(levelname)s - %(message)s')
 
 
@@ -45,27 +46,29 @@
 
     try:
         loop = asyncio.get_running_loop()
     except RuntimeError:
         loop = None
 
     if loop and loop.is_running():
-        print('Async event loop already running. Adding coroutine to the event loop.')
+        logging.info("Async event loop already running. Adding coroutine to the event loop.'")
+        # print('Async event loop already running. Adding coroutine to the event loop.')
         tsk = loop.create_task(get_departments_group_ids())
         await tsk
         depts_dict = tsk.result()
-
+        logging.info(f'Task done with depts_dict={depts_dict}')
             # Move subsequent code here
         process_departments(depts_dict, dept_name, file_url, BLOB_CONTAINER_NAME)
 
     else:
-        print('Starting new event loop')
+        logging.info(f'Starting new event loop')
+        # print('Starting new event loop')
         depts_dict =  await get_departments_group_ids()  # Await the task completion
-        print(f'Task done with depts_dict={depts_dict}')
-        
+        # print(f'Task done with depts_dict={depts_dict}')
+        logging.info(f'Task done with depts_dict={depts_dict}')
         # Move subsequent code here
         process_departments(depts_dict, dept_name, file_url, BLOB_CONTAINER_NAME)
 
     
 
 # file_url = "/Shared Documents/GPTKB_HRTest/sample.txt"
 # asyncio.run(update_rag(file_url))
```

### Comparing `chamco_ragbot-0.1.8/chamco_ragbot/search.py` & `chamco_ragbot-0.1.9/chamco_ragbot/search.py`

 * *Files identical despite different names*

### Comparing `chamco_ragbot-0.1.8/chamco_ragbot/skillset.py` & `chamco_ragbot-0.1.9/chamco_ragbot/skillset.py`

 * *Files identical despite different names*

### Comparing `chamco_ragbot-0.1.8/chamco_ragbot/utils.py` & `chamco_ragbot-0.1.9/chamco_ragbot/utils.py`

 * *Files identical despite different names*


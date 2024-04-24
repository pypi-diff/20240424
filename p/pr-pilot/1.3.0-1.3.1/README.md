# Comparing `tmp/pr_pilot-1.3.0.tar.gz` & `tmp/pr_pilot-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pr_pilot-1.3.0.tar", last modified: Thu Apr 18 18:51:43 2024, max compression
+gzip compressed data, was "pr_pilot-1.3.1.tar", last modified: Wed Apr 24 20:23:24 2024, max compression
```

## Comparing `pr_pilot-1.3.0.tar` & `pr_pilot-1.3.1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:51:43.665241 pr_pilot-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-18 18:51:39.000000 pr_pilot-1.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-18 18:51:39.000000 pr_pilot-1.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-04-18 18:51:43.665241 pr_pilot-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-18 18:51:39.000000 pr_pilot-1.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:51:43.661241 pr_pilot-1.3.0/pr_pilot/
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-04-18 18:51:39.000000 pr_pilot-1.3.0/pr_pilot/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:51:43.665241 pr_pilot-1.3.0/pr_pilot/api/
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-18 18:51:39.000000 pr_pilot-1.3.0/pr_pilot/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11037 2024-04-18 18:51:39.000000 pr_pilot-1.3.0/pr_pilot/api/task_creation_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    10404 2024-04-18 18:51:39.000000 pr_pilot-1.3.0/pr_pilot/api/task_retrieval_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    26236 2024-04-18 18:51:39.000000 pr_pilot-1.3.0/pr_pilot/api_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-18 18:51:39.000000 pr_pilot-1.3.0/pr_pilot/api_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    15420 2024-04-18 18:51:39.000000 pr_pilot-1.3.0/pr_pilot/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     5902 2024-04-18 18:51:39.000000 pr_pilot-1.3.0/pr_pilot/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:51:43.665241 pr_pilot-1.3.0/pr_pilot/models/
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-04-18 18:51:39.000000 pr_pilot-1.3.0/pr_pilot/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2467 2024-04-18 18:51:39.000000 pr_pilot-1.3.0/pr_pilot/models/bad_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2382 2024-04-18 18:51:39.000000 pr_pilot-1.3.0/pr_pilot/models/not_found.py
--rw-r--r--   0 runner    (1001) docker     (127)     3032 2024-04-18 18:51:39.000000 pr_pilot-1.3.0/pr_pilot/models/prompt.py
--rw-r--r--   0 runner    (1001) docker     (127)     4144 2024-04-18 18:51:39.000000 pr_pilot-1.3.0/pr_pilot/models/task.py
--rw-r--r--   0 runner    (1001) docker     (127)     9332 2024-04-18 18:51:39.000000 pr_pilot-1.3.0/pr_pilot/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:51:43.665241 pr_pilot-1.3.0/pr_pilot/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 18:51:39.000000 pr_pilot-1.3.0/pr_pilot/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-04-18 18:51:39.000000 pr_pilot-1.3.0/pr_pilot/test/test_bad_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-04-18 18:51:39.000000 pr_pilot-1.3.0/pr_pilot/test/test_not_found.py
--rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-04-18 18:51:39.000000 pr_pilot-1.3.0/pr_pilot/test/test_prompt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-04-18 18:51:39.000000 pr_pilot-1.3.0/pr_pilot/test/test_task.py
--rw-r--r--   0 runner    (1001) docker     (127)      682 2024-04-18 18:51:39.000000 pr_pilot-1.3.0/pr_pilot/test/test_task_creation_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-18 18:51:39.000000 pr_pilot-1.3.0/pr_pilot/test/test_task_retrieval_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3442 2024-04-18 18:51:39.000000 pr_pilot-1.3.0/pr_pilot/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:51:43.665241 pr_pilot-1.3.0/pr_pilot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-04-18 18:51:43.000000 pr_pilot-1.3.0/pr_pilot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-04-18 18:51:43.000000 pr_pilot-1.3.0/pr_pilot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 18:51:43.000000 pr_pilot-1.3.0/pr_pilot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-18 18:51:43.000000 pr_pilot-1.3.0/pr_pilot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-18 18:51:43.000000 pr_pilot-1.3.0/pr_pilot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-18 18:51:39.000000 pr_pilot-1.3.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 18:51:43.665241 pr_pilot-1.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      961 2024-04-18 18:51:39.000000 pr_pilot-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:23:24.753994 pr_pilot-1.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-24 20:23:20.000000 pr_pilot-1.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-24 20:23:20.000000 pr_pilot-1.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-04-24 20:23:24.753994 pr_pilot-1.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-24 20:23:20.000000 pr_pilot-1.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:23:24.753994 pr_pilot-1.3.1/pr_pilot/
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-04-24 20:23:20.000000 pr_pilot-1.3.1/pr_pilot/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:23:24.753994 pr_pilot-1.3.1/pr_pilot/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-24 20:23:20.000000 pr_pilot-1.3.1/pr_pilot/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11037 2024-04-24 20:23:20.000000 pr_pilot-1.3.1/pr_pilot/api/task_creation_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10404 2024-04-24 20:23:20.000000 pr_pilot-1.3.1/pr_pilot/api/task_retrieval_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26236 2024-04-24 20:23:20.000000 pr_pilot-1.3.1/pr_pilot/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-24 20:23:20.000000 pr_pilot-1.3.1/pr_pilot/api_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15420 2024-04-24 20:23:20.000000 pr_pilot-1.3.1/pr_pilot/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5902 2024-04-24 20:23:20.000000 pr_pilot-1.3.1/pr_pilot/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:23:24.753994 pr_pilot-1.3.1/pr_pilot/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-04-24 20:23:20.000000 pr_pilot-1.3.1/pr_pilot/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2467 2024-04-24 20:23:20.000000 pr_pilot-1.3.1/pr_pilot/models/bad_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2382 2024-04-24 20:23:20.000000 pr_pilot-1.3.1/pr_pilot/models/not_found.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3032 2024-04-24 20:23:20.000000 pr_pilot-1.3.1/pr_pilot/models/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4144 2024-04-24 20:23:20.000000 pr_pilot-1.3.1/pr_pilot/models/task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9332 2024-04-24 20:23:20.000000 pr_pilot-1.3.1/pr_pilot/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:23:24.753994 pr_pilot-1.3.1/pr_pilot/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 20:23:20.000000 pr_pilot-1.3.1/pr_pilot/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-04-24 20:23:20.000000 pr_pilot-1.3.1/pr_pilot/test/test_bad_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-04-24 20:23:20.000000 pr_pilot-1.3.1/pr_pilot/test/test_not_found.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-04-24 20:23:20.000000 pr_pilot-1.3.1/pr_pilot/test/test_prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-04-24 20:23:20.000000 pr_pilot-1.3.1/pr_pilot/test/test_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-04-24 20:23:20.000000 pr_pilot-1.3.1/pr_pilot/test/test_task_creation_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-24 20:23:20.000000 pr_pilot-1.3.1/pr_pilot/test/test_task_retrieval_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3705 2024-04-24 20:23:20.000000 pr_pilot-1.3.1/pr_pilot/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:23:24.753994 pr_pilot-1.3.1/pr_pilot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-04-24 20:23:24.000000 pr_pilot-1.3.1/pr_pilot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-04-24 20:23:24.000000 pr_pilot-1.3.1/pr_pilot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 20:23:24.000000 pr_pilot-1.3.1/pr_pilot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-24 20:23:24.000000 pr_pilot-1.3.1/pr_pilot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-24 20:23:24.000000 pr_pilot-1.3.1/pr_pilot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-24 20:23:20.000000 pr_pilot-1.3.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 20:23:24.753994 pr_pilot-1.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-04-24 20:23:20.000000 pr_pilot-1.3.1/setup.py
```

### Comparing `pr_pilot-1.3.0/LICENSE` & `pr_pilot-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pr_pilot-1.3.0/PKG-INFO` & `pr_pilot-1.3.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pr_pilot
-Version: 1.3.0
+Version: 1.3.1
 Summary: Python SDK for PR Pilot, a text-to-task automation platform for Github.
 Home-page: https://github.com/PR-Pilot-AI/pr-pilot-python
 Author: Marco Lamina
 Author-email: marco@pr-pilot.ai
 License: GPL-3.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -19,24 +19,23 @@
 Requires-Dist: setuptools==69.1.1
 
 <div align="center">
 <img src="https://avatars.githubusercontent.com/ml/17635?s=140&v=" width="100" alt="PR Pilot Logo">
 </div>
 
 <p align="center">
-  <a href="https://github.com/marketplace/pr-pilot-ai"><b>Install</b></a> |
+  <a href="https://github.com/apps/pr-pilot-ai/installations/new"><b>Install</b></a> |
   <a href="https://docs.pr-pilot.ai">Documentation</a> | 
   <a href="https://www.pr-pilot.ai/blog">Blog</a> | 
   <a href="https://www.pr-pilot.ai">Website</a>
 </p>
 
+# PR Pilot - Python SDK
 
-# 🤖 PR Pilot - Python SDK
-
-PR Pilot is a **text-to-task** automation platform that enables GitHub developers to trigger AI-driven development tasks in their repositories from anywhere.
+**[PR Pilot](https://github.com/PR-Pilot-AI/pr-pilot)** is a platform that enables developers to create agentic workflows for Github Projects.
 
 This project contains the official Python SDK.
 
 ## Usage
 
 Install the Python SDK using pip:
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

#### html2text {}

```diff
@@ -1,20 +1,20 @@
-Metadata-Version: 2.1 Name: pr_pilot Version: 1.3.0 Summary: Python SDK for PR
+Metadata-Version: 2.1 Name: pr_pilot Version: 1.3.1 Summary: Python SDK for PR
 Pilot, a text-to-task automation platform for Github. Home-page: https://
 github.com/PR-Pilot-AI/pr-pilot-python Author: Marco Lamina Author-email:
 marco@pr-pilot.ai License: GPL-3.0 Classifier: Programming Language :: Python
 :: 3 Classifier: License :: OSI Approved :: MIT License Classifier: Operating
 System :: OS Independent Requires-Python: >=3.6 Description-Content-Type: text/
 markdown License-File: LICENSE Requires-Dist: pydantic==2.7.0 Requires-Dist:
 urllib3==2.2.1 Requires-Dist: python-dateutil==2.9.0 Requires-Dist:
 wheel==0.42.0 Requires-Dist: setuptools==69.1.1
                                 [PR Pilot Logo]
                    _II_nn_ss_tt_aa_ll_ll | _D_o_c_u_m_e_n_t_a_t_i_o_n | _B_l_o_g | _W_e_b_s_i_t_e
-# ð¤ PR Pilot - Python SDK PR Pilot is a **text-to-task** automation platform
-that enables GitHub developers to trigger AI-driven development tasks in their
-repositories from anywhere. This project contains the official Python SDK. ##
-Usage Install the Python SDK using pip: ```bash pip install pr-pilot ``` Use
-the `create_task`, `get_task` and `wait_for_result` functions to automate your
-Github project: ```python from pr_pilot.util import create_task,
-wait_for_result task = create_task("PR-Pilot-AI/pr-pilot", "Summarize the
-README file and create a Github issue with the result.") result =
-wait_for_result(task) print(f"Task completed. Result:\n\n{task.result}") ```
+# PR Pilot - Python SDK **[PR Pilot](https://github.com/PR-Pilot-AI/pr-pilot)**
+is a platform that enables developers to create agentic workflows for Github
+Projects. This project contains the official Python SDK. ## Usage Install the
+Python SDK using pip: ```bash pip install pr-pilot ``` Use the `create_task`,
+`get_task` and `wait_for_result` functions to automate your Github project:
+```python from pr_pilot.util import create_task, wait_for_result task =
+create_task("PR-Pilot-AI/pr-pilot", "Summarize the README file and create a
+Github issue with the result.") result = wait_for_result(task) print(f"Task
+completed. Result:\n\n{task.result}") ```
```

### Comparing `pr_pilot-1.3.0/README.md` & `pr_pilot-1.3.1/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 <div align="center">
 <img src="https://avatars.githubusercontent.com/ml/17635?s=140&v=" width="100" alt="PR Pilot Logo">
 </div>
 
 <p align="center">
-  <a href="https://github.com/marketplace/pr-pilot-ai"><b>Install</b></a> |
+  <a href="https://github.com/apps/pr-pilot-ai/installations/new"><b>Install</b></a> |
   <a href="https://docs.pr-pilot.ai">Documentation</a> | 
   <a href="https://www.pr-pilot.ai/blog">Blog</a> | 
   <a href="https://www.pr-pilot.ai">Website</a>
 </p>
 
+# PR Pilot - Python SDK
 
-# 🤖 PR Pilot - Python SDK
-
-PR Pilot is a **text-to-task** automation platform that enables GitHub developers to trigger AI-driven development tasks in their repositories from anywhere.
+**[PR Pilot](https://github.com/PR-Pilot-AI/pr-pilot)** is a platform that enables developers to create agentic workflows for Github Projects.
 
 This project contains the official Python SDK.
 
 ## Usage
 
 Install the Python SDK using pip:
 
@@ -28,8 +27,8 @@
 
 ```python
 from pr_pilot.util import create_task, wait_for_result
 
 task = create_task("PR-Pilot-AI/pr-pilot", "Summarize the README file and create a Github issue with the result.")
 result = wait_for_result(task)
 print(f"Task completed. Result:\n\n{task.result}")
-```
+```
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
                                 [PR Pilot Logo]
                    _II_nn_ss_tt_aa_ll_ll | _D_o_c_u_m_e_n_t_a_t_i_o_n | _B_l_o_g | _W_e_b_s_i_t_e
-# ð¤ PR Pilot - Python SDK PR Pilot is a **text-to-task** automation platform
-that enables GitHub developers to trigger AI-driven development tasks in their
-repositories from anywhere. This project contains the official Python SDK. ##
-Usage Install the Python SDK using pip: ```bash pip install pr-pilot ``` Use
-the `create_task`, `get_task` and `wait_for_result` functions to automate your
-Github project: ```python from pr_pilot.util import create_task,
-wait_for_result task = create_task("PR-Pilot-AI/pr-pilot", "Summarize the
-README file and create a Github issue with the result.") result =
-wait_for_result(task) print(f"Task completed. Result:\n\n{task.result}") ```
+# PR Pilot - Python SDK **[PR Pilot](https://github.com/PR-Pilot-AI/pr-pilot)**
+is a platform that enables developers to create agentic workflows for Github
+Projects. This project contains the official Python SDK. ## Usage Install the
+Python SDK using pip: ```bash pip install pr-pilot ``` Use the `create_task`,
+`get_task` and `wait_for_result` functions to automate your Github project:
+```python from pr_pilot.util import create_task, wait_for_result task =
+create_task("PR-Pilot-AI/pr-pilot", "Summarize the README file and create a
+Github issue with the result.") result = wait_for_result(task) print(f"Task
+completed. Result:\n\n{task.result}") ```
```

### Comparing `pr_pilot-1.3.0/pr_pilot/__init__.py` & `pr_pilot-1.3.1/pr_pilot/__init__.py`

 * *Files identical despite different names*

### Comparing `pr_pilot-1.3.0/pr_pilot/api/task_creation_api.py` & `pr_pilot-1.3.1/pr_pilot/api/task_creation_api.py`

 * *Files identical despite different names*

### Comparing `pr_pilot-1.3.0/pr_pilot/api/task_retrieval_api.py` & `pr_pilot-1.3.1/pr_pilot/api/task_retrieval_api.py`

 * *Files identical despite different names*

### Comparing `pr_pilot-1.3.0/pr_pilot/api_client.py` & `pr_pilot-1.3.1/pr_pilot/api_client.py`

 * *Files identical despite different names*

### Comparing `pr_pilot-1.3.0/pr_pilot/api_response.py` & `pr_pilot-1.3.1/pr_pilot/api_response.py`

 * *Files identical despite different names*

### Comparing `pr_pilot-1.3.0/pr_pilot/configuration.py` & `pr_pilot-1.3.1/pr_pilot/configuration.py`

 * *Files identical despite different names*

### Comparing `pr_pilot-1.3.0/pr_pilot/exceptions.py` & `pr_pilot-1.3.1/pr_pilot/exceptions.py`

 * *Files identical despite different names*

### Comparing `pr_pilot-1.3.0/pr_pilot/models/bad_request.py` & `pr_pilot-1.3.1/pr_pilot/models/bad_request.py`

 * *Files identical despite different names*

### Comparing `pr_pilot-1.3.0/pr_pilot/models/not_found.py` & `pr_pilot-1.3.1/pr_pilot/models/not_found.py`

 * *Files identical despite different names*

### Comparing `pr_pilot-1.3.0/pr_pilot/models/prompt.py` & `pr_pilot-1.3.1/pr_pilot/models/prompt.py`

 * *Files identical despite different names*

### Comparing `pr_pilot-1.3.0/pr_pilot/models/task.py` & `pr_pilot-1.3.1/pr_pilot/models/task.py`

 * *Files identical despite different names*

### Comparing `pr_pilot-1.3.0/pr_pilot/rest.py` & `pr_pilot-1.3.1/pr_pilot/rest.py`

 * *Files identical despite different names*

### Comparing `pr_pilot-1.3.0/pr_pilot/test/test_bad_request.py` & `pr_pilot-1.3.1/pr_pilot/test/test_bad_request.py`

 * *Files identical despite different names*

### Comparing `pr_pilot-1.3.0/pr_pilot/test/test_not_found.py` & `pr_pilot-1.3.1/pr_pilot/test/test_not_found.py`

 * *Files identical despite different names*

### Comparing `pr_pilot-1.3.0/pr_pilot/test/test_prompt.py` & `pr_pilot-1.3.1/pr_pilot/test/test_prompt.py`

 * *Files identical despite different names*

### Comparing `pr_pilot-1.3.0/pr_pilot/test/test_task.py` & `pr_pilot-1.3.1/pr_pilot/test/test_task.py`

 * *Files identical despite different names*

### Comparing `pr_pilot-1.3.0/pr_pilot/test/test_task_creation_api.py` & `pr_pilot-1.3.1/pr_pilot/test/test_task_creation_api.py`

 * *Files identical despite different names*

### Comparing `pr_pilot-1.3.0/pr_pilot/test/test_task_retrieval_api.py` & `pr_pilot-1.3.1/pr_pilot/test/test_task_retrieval_api.py`

 * *Files identical despite different names*

### Comparing `pr_pilot-1.3.0/pr_pilot/util.py` & `pr_pilot-1.3.1/pr_pilot/util.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,19 +26,25 @@
 
 def set_github_action_output(key: str, value: str):
     """Set an output parameter for GitHub Actions."""
     # Get the path to the environment file for outputs
     output_file = os.getenv('GITHUB_OUTPUT')
 
     # Ensure the output file path is available
-    if output_file is not None:
-        with open(output_file, "a") as file:
-            file.write(f"{key}={value}\n")
-    else:
+    if output_file is None:
         logger.debug("GITHUB_OUTPUT environment variable is not set.")
+        return
+
+    with open(output_file, "a") as file:
+        if "\n" in value:
+            # Handle multiline value
+            file.write(f"{key}<<EOF\n{value}\nEOF\n")
+        else:
+            # Write the key-value pair to the output file
+            file.write(f"{key}={value}\n")
 
 
 def set_github_step_summary(summary: str):
     """Set the step summary for GitHub Actions."""
     # Get the path to the environment file for outputs
     output_file = os.getenv('GITHUB_STEP_SUMMARY')
 
@@ -83,10 +89,11 @@
         if log:
             logger.info(f"Task status: {task.status}. Waiting for completion...")
         task = get_task(task.id)
 
         time.sleep(POLL_INTERVAL)
     if write_step_summary:
         dashboard_url = f"https://app.pr-pilot.ai/dashboard/tasks/{str(task.id)}/"
-        markdown_link = f"[Event Log]({dashboard_url})"
-        set_github_step_summary(f"{task.result}\n\n{markdown_link}")
+        markdown_link = f"📋 **[Log]({dashboard_url})**"
+        set_github_step_summary(f"---\n\n{task.result}\n\n---\n{markdown_link}")
+        set_github_action_output("task-result", task.result)
     return task.result
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pr_pilot-1.3.0/pr_pilot.egg-info/PKG-INFO` & `pr_pilot-1.3.1/pr_pilot.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pr_pilot
-Version: 1.3.0
+Version: 1.3.1
 Summary: Python SDK for PR Pilot, a text-to-task automation platform for Github.
 Home-page: https://github.com/PR-Pilot-AI/pr-pilot-python
 Author: Marco Lamina
 Author-email: marco@pr-pilot.ai
 License: GPL-3.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -19,24 +19,23 @@
 Requires-Dist: setuptools==69.1.1
 
 <div align="center">
 <img src="https://avatars.githubusercontent.com/ml/17635?s=140&v=" width="100" alt="PR Pilot Logo">
 </div>
 
 <p align="center">
-  <a href="https://github.com/marketplace/pr-pilot-ai"><b>Install</b></a> |
+  <a href="https://github.com/apps/pr-pilot-ai/installations/new"><b>Install</b></a> |
   <a href="https://docs.pr-pilot.ai">Documentation</a> | 
   <a href="https://www.pr-pilot.ai/blog">Blog</a> | 
   <a href="https://www.pr-pilot.ai">Website</a>
 </p>
 
+# PR Pilot - Python SDK
 
-# 🤖 PR Pilot - Python SDK
-
-PR Pilot is a **text-to-task** automation platform that enables GitHub developers to trigger AI-driven development tasks in their repositories from anywhere.
+**[PR Pilot](https://github.com/PR-Pilot-AI/pr-pilot)** is a platform that enables developers to create agentic workflows for Github Projects.
 
 This project contains the official Python SDK.
 
 ## Usage
 
 Install the Python SDK using pip:
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

#### html2text {}

```diff
@@ -1,20 +1,20 @@
-Metadata-Version: 2.1 Name: pr_pilot Version: 1.3.0 Summary: Python SDK for PR
+Metadata-Version: 2.1 Name: pr_pilot Version: 1.3.1 Summary: Python SDK for PR
 Pilot, a text-to-task automation platform for Github. Home-page: https://
 github.com/PR-Pilot-AI/pr-pilot-python Author: Marco Lamina Author-email:
 marco@pr-pilot.ai License: GPL-3.0 Classifier: Programming Language :: Python
 :: 3 Classifier: License :: OSI Approved :: MIT License Classifier: Operating
 System :: OS Independent Requires-Python: >=3.6 Description-Content-Type: text/
 markdown License-File: LICENSE Requires-Dist: pydantic==2.7.0 Requires-Dist:
 urllib3==2.2.1 Requires-Dist: python-dateutil==2.9.0 Requires-Dist:
 wheel==0.42.0 Requires-Dist: setuptools==69.1.1
                                 [PR Pilot Logo]
                    _II_nn_ss_tt_aa_ll_ll | _D_o_c_u_m_e_n_t_a_t_i_o_n | _B_l_o_g | _W_e_b_s_i_t_e
-# ð¤ PR Pilot - Python SDK PR Pilot is a **text-to-task** automation platform
-that enables GitHub developers to trigger AI-driven development tasks in their
-repositories from anywhere. This project contains the official Python SDK. ##
-Usage Install the Python SDK using pip: ```bash pip install pr-pilot ``` Use
-the `create_task`, `get_task` and `wait_for_result` functions to automate your
-Github project: ```python from pr_pilot.util import create_task,
-wait_for_result task = create_task("PR-Pilot-AI/pr-pilot", "Summarize the
-README file and create a Github issue with the result.") result =
-wait_for_result(task) print(f"Task completed. Result:\n\n{task.result}") ```
+# PR Pilot - Python SDK **[PR Pilot](https://github.com/PR-Pilot-AI/pr-pilot)**
+is a platform that enables developers to create agentic workflows for Github
+Projects. This project contains the official Python SDK. ## Usage Install the
+Python SDK using pip: ```bash pip install pr-pilot ``` Use the `create_task`,
+`get_task` and `wait_for_result` functions to automate your Github project:
+```python from pr_pilot.util import create_task, wait_for_result task =
+create_task("PR-Pilot-AI/pr-pilot", "Summarize the README file and create a
+Github issue with the result.") result = wait_for_result(task) print(f"Task
+completed. Result:\n\n{task.result}") ```
```

### Comparing `pr_pilot-1.3.0/pr_pilot.egg-info/SOURCES.txt` & `pr_pilot-1.3.1/pr_pilot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pr_pilot-1.3.0/setup.py` & `pr_pilot-1.3.1/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 this_dir = path.abspath(path.dirname(__file__))
 requirements_path = path.join(this_dir, 'requirements.txt')
 with open(requirements_path) as f:
     required = f.read().splitlines()
 
 setup(
     name='pr_pilot',
-    version='1.3.0',
+    version='1.3.1',
     packages=find_packages(),
     install_requires=required,
     python_requires='>=3.6',
     author='Marco Lamina',
     author_email='marco@pr-pilot.ai',
     description='Python SDK for PR Pilot, a text-to-task automation platform for Github.',
     long_description=open('README.md').read(),
```


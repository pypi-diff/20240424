# Comparing `tmp/leya-0.1.0.tar.gz` & `tmp/leya-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "leya-0.1.0.tar", last modified: Wed Apr 24 02:50:21 2024, max compression
+gzip compressed data, was "leya-0.1.1.tar", last modified: Wed Apr 24 03:22:04 2024, max compression
```

## Comparing `leya-0.1.0.tar` & `leya-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-24 02:50:21.342266 leya-0.1.0/
--rw-rw-rw-   0        0        0      184 2024-04-24 02:50:21.341253 leya-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     2495 2024-04-24 02:33:47.000000 leya-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-24 02:50:21.285590 leya-0.1.0/leya/
--rw-rw-rw-   0        0        0        0 2024-04-22 20:40:53.000000 leya-0.1.0/leya/__init__.py
--rw-rw-rw-   0        0        0     2434 2024-04-24 02:14:04.000000 leya-0.1.0/leya/cli.py
--rw-rw-rw-   0        0        0     2453 2024-04-24 02:14:04.000000 leya-0.1.0/leya/core.py
--rw-rw-rw-   0        0        0      638 2024-04-23 09:10:17.000000 leya-0.1.0/leya/repo_states.py
-drwxrwxrwx   0        0        0        0 2024-04-24 02:50:21.337046 leya-0.1.0/leya.egg-info/
--rw-rw-rw-   0        0        0      184 2024-04-24 02:50:21.000000 leya-0.1.0/leya.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      250 2024-04-24 02:50:21.000000 leya-0.1.0/leya.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-24 02:50:21.000000 leya-0.1.0/leya.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2024-04-24 02:50:21.000000 leya-0.1.0/leya.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      905 2024-04-24 02:50:21.000000 leya-0.1.0/leya.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-04-24 02:50:21.000000 leya-0.1.0/leya.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-24 02:50:21.343267 leya-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1851 2024-04-24 02:14:04.000000 leya-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:22:04.050874 leya-0.1.1/
+-rw-rw-rw-   0        0        0     1090 2024-04-24 03:18:12.000000 leya-0.1.1/License.txt
+-rw-rw-rw-   0        0        0      211 2024-04-24 03:22:04.049871 leya-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2495 2024-04-24 02:33:47.000000 leya-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-24 03:22:04.036872 leya-0.1.1/leya/
+-rw-rw-rw-   0        0        0        0 2024-04-22 20:40:53.000000 leya-0.1.1/leya/__init__.py
+-rw-rw-rw-   0        0        0     2422 2024-04-24 03:11:21.000000 leya-0.1.1/leya/cli.py
+-rw-rw-rw-   0        0        0     2433 2024-04-24 03:11:36.000000 leya-0.1.1/leya/core.py
+-rw-rw-rw-   0        0        0      638 2024-04-23 09:10:17.000000 leya-0.1.1/leya/repo_states.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:22:04.048918 leya-0.1.1/leya.egg-info/
+-rw-rw-rw-   0        0        0      211 2024-04-24 03:22:03.000000 leya-0.1.1/leya.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      262 2024-04-24 03:22:04.000000 leya-0.1.1/leya.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 03:22:03.000000 leya-0.1.1/leya.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2024-04-24 03:22:03.000000 leya-0.1.1/leya.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      905 2024-04-24 03:22:03.000000 leya-0.1.1/leya.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-04-24 03:22:03.000000 leya-0.1.1/leya.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-24 03:22:04.050874 leya-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1851 2024-04-24 03:20:58.000000 leya-0.1.1/setup.py
```

### Comparing `leya-0.1.0/README.md` & `leya-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `leya-0.1.0/leya/cli.py` & `leya-0.1.1/leya/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import argparse
 import os
 from dotenv import load_dotenv
-from leya.core import clone_repository, handle_query
-from leya.repo_states import save_selected_repo, load_selected_repo
-from leya.utils.set_enivronment_variables import set_environment_variables
+from .core import clone_repository, handle_query
+from .repo_states import save_selected_repo, load_selected_repo
+from .utils.set_enivronment_variables import set_environment_variables
 
 def list_repositories(repos_path):
     """ Lists directories in the given path """
     try:
         repos = [repo for repo in os.listdir(repos_path) if os.path.isdir(os.path.join(repos_path, repo))]
         return repos
     except FileNotFoundError:
```

### Comparing `leya-0.1.0/leya/core.py` & `leya-0.1.1/leya/core.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from git import Repo
 from git.exc import GitCommandError
 
-from leya.processors.repo_processor import process_repos
-from leya.services.pincecone import embed_chunks_and_upload_to_pinecone, setup_pinecone_index, get_most_similar_chunks_for_query
-from leya.utils.embedPrompt import build_prompt
-from leya.utils.format_text import format_answer
-from leya.services.openai import get_llm_answer
+from .processors.repo_processor import process_repos
+from .services.pincecone import embed_chunks_and_upload_to_pinecone, setup_pinecone_index, get_most_similar_chunks_for_query
+from .utils.embedPrompt import build_prompt
+from .utils.format_text import format_answer
+from .services.openai import get_llm_answer
 import os
 
 
 def clone_repository(repo_url):
     try:
         # Determine the name of the repository by splitting the URL
         repo_name = repo_url.split('/')[-1]
```

### Comparing `leya-0.1.0/leya/repo_states.py` & `leya-0.1.1/leya/repo_states.py`

 * *Files identical despite different names*

### Comparing `leya-0.1.0/leya.egg-info/requires.txt` & `leya-0.1.1/leya.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `leya-0.1.0/setup.py` & `leya-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,15 @@
     'Werkzeug==3.0.2',
     'wrapt==1.16.0',
     'zipp==3.18.1',
 ]
 
 setup(
     name='leya',
-    version='0.1.0',
+    version='0.1.1',
     packages=find_packages(),
     install_requires=install_requires,
     entry_points={
         'console_scripts': [
             'leya=leya.cli:main',
         ],
     },
```


# Comparing `tmp/leya-0.1.3.tar.gz` & `tmp/leya-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "leya-0.1.3.tar", last modified: Wed Apr 24 15:57:32 2024, max compression
+gzip compressed data, was "leya-0.1.4.tar", last modified: Wed Apr 24 16:28:52 2024, max compression
```

## Comparing `leya-0.1.3.tar` & `leya-0.1.4.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2024-04-24 15:57:32.003571 leya-0.1.3/
--rw-rw-rw-   0        0        0     1090 2024-04-24 03:18:12.000000 leya-0.1.3/License.txt
--rw-rw-rw-   0        0        0      211 2024-04-24 15:57:32.000573 leya-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     2495 2024-04-24 02:33:47.000000 leya-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2024-04-24 15:57:31.903939 leya-0.1.3/leya/
--rw-rw-rw-   0        0        0        0 2024-04-22 20:40:53.000000 leya-0.1.3/leya/__init__.py
--rw-rw-rw-   0        0        0     2422 2024-04-24 03:11:21.000000 leya-0.1.3/leya/cli.py
--rw-rw-rw-   0        0        0     2433 2024-04-24 03:11:36.000000 leya-0.1.3/leya/core.py
-drwxrwxrwx   0        0        0        0 2024-04-24 15:57:31.951932 leya-0.1.3/leya/processors/
--rw-rw-rw-   0        0        0        0 2024-04-24 03:40:04.000000 leya-0.1.3/leya/processors/__init__.py
--rw-rw-rw-   0        0        0     1131 2024-04-23 08:54:15.000000 leya-0.1.3/leya/processors/file_processor.py
--rw-rw-rw-   0        0        0     3193 2024-04-24 03:17:32.000000 leya-0.1.3/leya/processors/repo_processor.py
--rw-rw-rw-   0        0        0      638 2024-04-23 09:10:17.000000 leya-0.1.3/leya/repo_states.py
-drwxrwxrwx   0        0        0        0 2024-04-24 15:57:31.957932 leya-0.1.3/leya/services/
--rw-rw-rw-   0        0        0        0 2024-04-24 03:40:13.000000 leya-0.1.3/leya/services/__init__.py
--rw-rw-rw-   0        0        0     1487 2024-04-23 09:58:00.000000 leya-0.1.3/leya/services/openai.py
--rw-rw-rw-   0        0        0     3466 2024-04-24 03:15:39.000000 leya-0.1.3/leya/services/pincecone.py
-drwxrwxrwx   0        0        0        0 2024-04-24 15:57:31.998563 leya-0.1.3/leya/utils/
--rw-rw-rw-   0        0        0        0 2024-04-24 03:40:22.000000 leya-0.1.3/leya/utils/__init__.py
--rw-rw-rw-   0        0        0     1477 2024-04-23 11:11:23.000000 leya-0.1.3/leya/utils/condense_file.py
--rw-rw-rw-   0        0        0     1234 2024-04-23 18:48:04.000000 leya-0.1.3/leya/utils/embedPrompt.py
--rw-rw-rw-   0        0        0      873 2024-04-23 10:54:11.000000 leya-0.1.3/leya/utils/format_text.py
--rw-rw-rw-   0        0        0      800 2024-04-24 15:49:21.000000 leya-0.1.3/leya/utils/set_enivronment_variables.py
-drwxrwxrwx   0        0        0        0 2024-04-24 15:57:31.931925 leya-0.1.3/leya.egg-info/
--rw-rw-rw-   0        0        0      211 2024-04-24 15:57:31.000000 leya-0.1.3/leya.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      578 2024-04-24 15:57:31.000000 leya-0.1.3/leya.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-24 15:57:31.000000 leya-0.1.3/leya.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2024-04-24 15:57:31.000000 leya-0.1.3/leya.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      905 2024-04-24 15:57:31.000000 leya-0.1.3/leya.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-04-24 15:57:31.000000 leya-0.1.3/leya.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-24 15:57:32.003571 leya-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0     1851 2024-04-24 15:57:23.000000 leya-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-24 16:28:52.521577 leya-0.1.4/
+-rw-rw-rw-   0        0        0     1090 2024-04-24 03:18:12.000000 leya-0.1.4/License.txt
+-rw-rw-rw-   0        0        0      211 2024-04-24 16:28:52.518575 leya-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2495 2024-04-24 02:33:47.000000 leya-0.1.4/README.md
+drwxrwxrwx   0        0        0        0 2024-04-24 16:28:52.458872 leya-0.1.4/leya/
+-rw-rw-rw-   0        0        0        0 2024-04-22 20:40:53.000000 leya-0.1.4/leya/__init__.py
+-rw-rw-rw-   0        0        0     2422 2024-04-24 03:11:21.000000 leya-0.1.4/leya/cli.py
+-rw-rw-rw-   0        0        0     2433 2024-04-24 03:11:36.000000 leya-0.1.4/leya/core.py
+drwxrwxrwx   0        0        0        0 2024-04-24 16:28:52.493599 leya-0.1.4/leya/processors/
+-rw-rw-rw-   0        0        0        0 2024-04-24 03:40:04.000000 leya-0.1.4/leya/processors/__init__.py
+-rw-rw-rw-   0        0        0     1131 2024-04-23 08:54:15.000000 leya-0.1.4/leya/processors/file_processor.py
+-rw-rw-rw-   0        0        0     3193 2024-04-24 03:17:32.000000 leya-0.1.4/leya/processors/repo_processor.py
+-rw-rw-rw-   0        0        0      638 2024-04-23 09:10:17.000000 leya-0.1.4/leya/repo_states.py
+drwxrwxrwx   0        0        0        0 2024-04-24 16:28:52.500629 leya-0.1.4/leya/services/
+-rw-rw-rw-   0        0        0        0 2024-04-24 03:40:13.000000 leya-0.1.4/leya/services/__init__.py
+-rw-rw-rw-   0        0        0     1487 2024-04-23 09:58:00.000000 leya-0.1.4/leya/services/openai.py
+-rw-rw-rw-   0        0        0     3466 2024-04-24 03:15:39.000000 leya-0.1.4/leya/services/pincecone.py
+drwxrwxrwx   0        0        0        0 2024-04-24 16:28:52.512579 leya-0.1.4/leya/utils/
+-rw-rw-rw-   0        0        0        0 2024-04-24 03:40:22.000000 leya-0.1.4/leya/utils/__init__.py
+-rw-rw-rw-   0        0        0     1477 2024-04-23 11:11:23.000000 leya-0.1.4/leya/utils/condense_file.py
+-rw-rw-rw-   0        0        0     1234 2024-04-23 18:48:04.000000 leya-0.1.4/leya/utils/embedPrompt.py
+-rw-rw-rw-   0        0        0      873 2024-04-23 10:54:11.000000 leya-0.1.4/leya/utils/format_text.py
+-rw-rw-rw-   0        0        0      800 2024-04-24 15:49:21.000000 leya-0.1.4/leya/utils/set_enivronment_variables.py
+drwxrwxrwx   0        0        0        0 2024-04-24 16:28:52.484627 leya-0.1.4/leya.egg-info/
+-rw-rw-rw-   0        0        0      211 2024-04-24 16:28:52.000000 leya-0.1.4/leya.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      578 2024-04-24 16:28:52.000000 leya-0.1.4/leya.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 16:28:52.000000 leya-0.1.4/leya.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2024-04-24 16:28:52.000000 leya-0.1.4/leya.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      842 2024-04-24 16:28:52.000000 leya-0.1.4/leya.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-04-24 16:28:52.000000 leya-0.1.4/leya.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-24 16:28:52.522596 leya-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0     1756 2024-04-24 16:28:36.000000 leya-0.1.4/setup.py
```

### Comparing `leya-0.1.3/License.txt` & `leya-0.1.4/License.txt`

 * *Files identical despite different names*

### Comparing `leya-0.1.3/README.md` & `leya-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `leya-0.1.3/leya/cli.py` & `leya-0.1.4/leya/cli.py`

 * *Files identical despite different names*

### Comparing `leya-0.1.3/leya/core.py` & `leya-0.1.4/leya/core.py`

 * *Files identical despite different names*

### Comparing `leya-0.1.3/leya/processors/file_processor.py` & `leya-0.1.4/leya/processors/file_processor.py`

 * *Files identical despite different names*

### Comparing `leya-0.1.3/leya/processors/repo_processor.py` & `leya-0.1.4/leya/processors/repo_processor.py`

 * *Files identical despite different names*

### Comparing `leya-0.1.3/leya/repo_states.py` & `leya-0.1.4/leya/repo_states.py`

 * *Files identical despite different names*

### Comparing `leya-0.1.3/leya/services/openai.py` & `leya-0.1.4/leya/services/openai.py`

 * *Files identical despite different names*

### Comparing `leya-0.1.3/leya/services/pincecone.py` & `leya-0.1.4/leya/services/pincecone.py`

 * *Files identical despite different names*

### Comparing `leya-0.1.3/leya/utils/condense_file.py` & `leya-0.1.4/leya/utils/condense_file.py`

 * *Files identical despite different names*

### Comparing `leya-0.1.3/leya/utils/embedPrompt.py` & `leya-0.1.4/leya/utils/embedPrompt.py`

 * *Files identical despite different names*

### Comparing `leya-0.1.3/leya/utils/format_text.py` & `leya-0.1.4/leya/utils/format_text.py`

 * *Files identical despite different names*

### Comparing `leya-0.1.3/leya/utils/set_enivronment_variables.py` & `leya-0.1.4/leya/utils/set_enivronment_variables.py`

 * *Files identical despite different names*

### Comparing `leya-0.1.3/leya.egg-info/SOURCES.txt` & `leya-0.1.4/leya.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `leya-0.1.3/leya.egg-info/requires.txt` & `leya-0.1.4/leya.egg-info/requires.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,15 @@
 annotated-types==0.6.0
 anyio==4.3.0
 astunparse==1.6.3
 blinker==1.7.0
 cachelib==0.12.0
-certifi==2024.2.2
 charset-normalizer==3.3.2
 click==8.1.7
 colorama==0.4.6
-distro==1.9.0
-filelock==3.13.4
 fsspec==2024.3.1
 future==0.18.3
 gitdb==4.0.11
 GitPython==3.1.43
 h11==0.14.0
 httpcore==1.0.5
 httpx==0.27.0
@@ -20,15 +17,14 @@
 iniconfig==2.0.0
 itsdangerous==2.1.2
 markdown-it-py==3.0.0
 MarkupSafe==2.1.5
 mdurl==0.1.2
 mpmath==1.3.0
 msgspec==0.18.6
-networkx==3.3
 numpy==1.26.4
 packaging==24.0
 pinecone-client==3.2.2
 pluggy==1.5.0
 pydantic==2.6.4
 pydantic_core==2.16.3
 Pygments==2.17.2
```

### Comparing `leya-0.1.3/setup.py` & `leya-0.1.4/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,20 +3,17 @@
 # List of packages from requirements.txt
 install_requires = [
     'annotated-types==0.6.0',
     'anyio==4.3.0',
     'astunparse==1.6.3',
     'blinker==1.7.0',
     'cachelib==0.12.0',
-    'certifi==2024.2.2',
     'charset-normalizer==3.3.2',
     'click==8.1.7',
     'colorama==0.4.6',
-    'distro==1.9.0',
-    'filelock==3.13.4',
     'fsspec==2024.3.1',
     'future==0.18.3',
     'gitdb==4.0.11',
     'GitPython==3.1.43',
     'h11==0.14.0',
     'httpcore==1.0.5',
     'httpx==0.27.0',
@@ -24,15 +21,14 @@
     'iniconfig==2.0.0',
     'itsdangerous==2.1.2',
     'markdown-it-py==3.0.0',
     'MarkupSafe==2.1.5',
     'mdurl==0.1.2',
     'mpmath==1.3.0',
     'msgspec==0.18.6',
-    'networkx==3.3',
     'numpy==1.26.4',
     'packaging==24.0',
     'pinecone-client==3.2.2',
     'pluggy==1.5.0',
     'pydantic==2.6.4',
     'pydantic_core==2.16.3',
     'Pygments==2.17.2',
@@ -58,15 +54,15 @@
     'Werkzeug==3.0.2',
     'wrapt==1.16.0',
     'zipp==3.18.1',
 ]
 
 setup(
     name='leya',
-    version='0.1.3',
+    version='0.1.4',
     packages=find_packages(),
     install_requires=install_requires,
     entry_points={
         'console_scripts': [
             'leya=leya.cli:main',
         ],
     },
```


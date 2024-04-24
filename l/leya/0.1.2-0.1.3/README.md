# Comparing `tmp/leya-0.1.2.tar.gz` & `tmp/leya-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "leya-0.1.2.tar", last modified: Wed Apr 24 03:41:05 2024, max compression
+gzip compressed data, was "leya-0.1.3.tar", last modified: Wed Apr 24 15:57:32 2024, max compression
```

## Comparing `leya-0.1.2.tar` & `leya-0.1.3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2024-04-24 03:41:05.197351 leya-0.1.2/
--rw-rw-rw-   0        0        0     1090 2024-04-24 03:18:12.000000 leya-0.1.2/License.txt
--rw-rw-rw-   0        0        0      211 2024-04-24 03:41:05.195349 leya-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     2495 2024-04-24 02:33:47.000000 leya-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-24 03:41:05.153336 leya-0.1.2/leya/
--rw-rw-rw-   0        0        0        0 2024-04-22 20:40:53.000000 leya-0.1.2/leya/__init__.py
--rw-rw-rw-   0        0        0     2422 2024-04-24 03:11:21.000000 leya-0.1.2/leya/cli.py
--rw-rw-rw-   0        0        0     2433 2024-04-24 03:11:36.000000 leya-0.1.2/leya/core.py
-drwxrwxrwx   0        0        0        0 2024-04-24 03:41:05.181340 leya-0.1.2/leya/processors/
--rw-rw-rw-   0        0        0        0 2024-04-24 03:40:04.000000 leya-0.1.2/leya/processors/__init__.py
--rw-rw-rw-   0        0        0     1131 2024-04-23 08:54:15.000000 leya-0.1.2/leya/processors/file_processor.py
--rw-rw-rw-   0        0        0     3193 2024-04-24 03:17:32.000000 leya-0.1.2/leya/processors/repo_processor.py
--rw-rw-rw-   0        0        0      638 2024-04-23 09:10:17.000000 leya-0.1.2/leya/repo_states.py
-drwxrwxrwx   0        0        0        0 2024-04-24 03:41:05.185336 leya-0.1.2/leya/services/
--rw-rw-rw-   0        0        0        0 2024-04-24 03:40:13.000000 leya-0.1.2/leya/services/__init__.py
--rw-rw-rw-   0        0        0     1487 2024-04-23 09:58:00.000000 leya-0.1.2/leya/services/openai.py
--rw-rw-rw-   0        0        0     3466 2024-04-24 03:15:39.000000 leya-0.1.2/leya/services/pincecone.py
-drwxrwxrwx   0        0        0        0 2024-04-24 03:41:05.192358 leya-0.1.2/leya/utils/
--rw-rw-rw-   0        0        0        0 2024-04-24 03:40:22.000000 leya-0.1.2/leya/utils/__init__.py
--rw-rw-rw-   0        0        0     1477 2024-04-23 11:11:23.000000 leya-0.1.2/leya/utils/condense_file.py
--rw-rw-rw-   0        0        0     1234 2024-04-23 18:48:04.000000 leya-0.1.2/leya/utils/embedPrompt.py
--rw-rw-rw-   0        0        0      873 2024-04-23 10:54:11.000000 leya-0.1.2/leya/utils/format_text.py
--rw-rw-rw-   0        0        0      501 2024-04-24 02:28:37.000000 leya-0.1.2/leya/utils/set_enivronment_variables.py
-drwxrwxrwx   0        0        0        0 2024-04-24 03:41:05.175385 leya-0.1.2/leya.egg-info/
--rw-rw-rw-   0        0        0      211 2024-04-24 03:41:05.000000 leya-0.1.2/leya.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      578 2024-04-24 03:41:05.000000 leya-0.1.2/leya.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-24 03:41:05.000000 leya-0.1.2/leya.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2024-04-24 03:41:05.000000 leya-0.1.2/leya.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      905 2024-04-24 03:41:05.000000 leya-0.1.2/leya.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-04-24 03:41:05.000000 leya-0.1.2/leya.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-24 03:41:05.197351 leya-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1851 2024-04-24 03:41:01.000000 leya-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-24 15:57:32.003571 leya-0.1.3/
+-rw-rw-rw-   0        0        0     1090 2024-04-24 03:18:12.000000 leya-0.1.3/License.txt
+-rw-rw-rw-   0        0        0      211 2024-04-24 15:57:32.000573 leya-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2495 2024-04-24 02:33:47.000000 leya-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-24 15:57:31.903939 leya-0.1.3/leya/
+-rw-rw-rw-   0        0        0        0 2024-04-22 20:40:53.000000 leya-0.1.3/leya/__init__.py
+-rw-rw-rw-   0        0        0     2422 2024-04-24 03:11:21.000000 leya-0.1.3/leya/cli.py
+-rw-rw-rw-   0        0        0     2433 2024-04-24 03:11:36.000000 leya-0.1.3/leya/core.py
+drwxrwxrwx   0        0        0        0 2024-04-24 15:57:31.951932 leya-0.1.3/leya/processors/
+-rw-rw-rw-   0        0        0        0 2024-04-24 03:40:04.000000 leya-0.1.3/leya/processors/__init__.py
+-rw-rw-rw-   0        0        0     1131 2024-04-23 08:54:15.000000 leya-0.1.3/leya/processors/file_processor.py
+-rw-rw-rw-   0        0        0     3193 2024-04-24 03:17:32.000000 leya-0.1.3/leya/processors/repo_processor.py
+-rw-rw-rw-   0        0        0      638 2024-04-23 09:10:17.000000 leya-0.1.3/leya/repo_states.py
+drwxrwxrwx   0        0        0        0 2024-04-24 15:57:31.957932 leya-0.1.3/leya/services/
+-rw-rw-rw-   0        0        0        0 2024-04-24 03:40:13.000000 leya-0.1.3/leya/services/__init__.py
+-rw-rw-rw-   0        0        0     1487 2024-04-23 09:58:00.000000 leya-0.1.3/leya/services/openai.py
+-rw-rw-rw-   0        0        0     3466 2024-04-24 03:15:39.000000 leya-0.1.3/leya/services/pincecone.py
+drwxrwxrwx   0        0        0        0 2024-04-24 15:57:31.998563 leya-0.1.3/leya/utils/
+-rw-rw-rw-   0        0        0        0 2024-04-24 03:40:22.000000 leya-0.1.3/leya/utils/__init__.py
+-rw-rw-rw-   0        0        0     1477 2024-04-23 11:11:23.000000 leya-0.1.3/leya/utils/condense_file.py
+-rw-rw-rw-   0        0        0     1234 2024-04-23 18:48:04.000000 leya-0.1.3/leya/utils/embedPrompt.py
+-rw-rw-rw-   0        0        0      873 2024-04-23 10:54:11.000000 leya-0.1.3/leya/utils/format_text.py
+-rw-rw-rw-   0        0        0      800 2024-04-24 15:49:21.000000 leya-0.1.3/leya/utils/set_enivronment_variables.py
+drwxrwxrwx   0        0        0        0 2024-04-24 15:57:31.931925 leya-0.1.3/leya.egg-info/
+-rw-rw-rw-   0        0        0      211 2024-04-24 15:57:31.000000 leya-0.1.3/leya.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      578 2024-04-24 15:57:31.000000 leya-0.1.3/leya.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 15:57:31.000000 leya-0.1.3/leya.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2024-04-24 15:57:31.000000 leya-0.1.3/leya.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      905 2024-04-24 15:57:31.000000 leya-0.1.3/leya.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-04-24 15:57:31.000000 leya-0.1.3/leya.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-24 15:57:32.003571 leya-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1851 2024-04-24 15:57:23.000000 leya-0.1.3/setup.py
```

### Comparing `leya-0.1.2/License.txt` & `leya-0.1.3/License.txt`

 * *Files identical despite different names*

### Comparing `leya-0.1.2/README.md` & `leya-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `leya-0.1.2/leya/cli.py` & `leya-0.1.3/leya/cli.py`

 * *Files identical despite different names*

### Comparing `leya-0.1.2/leya/core.py` & `leya-0.1.3/leya/core.py`

 * *Files identical despite different names*

### Comparing `leya-0.1.2/leya/processors/file_processor.py` & `leya-0.1.3/leya/processors/file_processor.py`

 * *Files identical despite different names*

### Comparing `leya-0.1.2/leya/processors/repo_processor.py` & `leya-0.1.3/leya/processors/repo_processor.py`

 * *Files identical despite different names*

### Comparing `leya-0.1.2/leya/repo_states.py` & `leya-0.1.3/leya/repo_states.py`

 * *Files identical despite different names*

### Comparing `leya-0.1.2/leya/services/openai.py` & `leya-0.1.3/leya/services/openai.py`

 * *Files identical despite different names*

### Comparing `leya-0.1.2/leya/services/pincecone.py` & `leya-0.1.3/leya/services/pincecone.py`

 * *Files identical despite different names*

### Comparing `leya-0.1.2/leya/utils/condense_file.py` & `leya-0.1.3/leya/utils/condense_file.py`

 * *Files identical despite different names*

### Comparing `leya-0.1.2/leya/utils/embedPrompt.py` & `leya-0.1.3/leya/utils/embedPrompt.py`

 * *Files identical despite different names*

### Comparing `leya-0.1.2/leya/utils/format_text.py` & `leya-0.1.3/leya/utils/format_text.py`

 * *Files identical despite different names*

### Comparing `leya-0.1.2/leya.egg-info/SOURCES.txt` & `leya-0.1.3/leya.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `leya-0.1.2/leya.egg-info/requires.txt` & `leya-0.1.3/leya.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `leya-0.1.2/setup.py` & `leya-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,15 @@
     'Werkzeug==3.0.2',
     'wrapt==1.16.0',
     'zipp==3.18.1',
 ]
 
 setup(
     name='leya',
-    version='0.1.2',
+    version='0.1.3',
     packages=find_packages(),
     install_requires=install_requires,
     entry_points={
         'console_scripts': [
             'leya=leya.cli:main',
         ],
     },
```


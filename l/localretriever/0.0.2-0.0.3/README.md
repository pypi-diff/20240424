# Comparing `tmp/localretriever-0.0.2.tar.gz` & `tmp/localretriever-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "localretriever-0.0.2.tar", last modified: Wed Apr 24 14:22:03 2024, max compression
+gzip compressed data, was "localretriever-0.0.3.tar", last modified: Wed Apr 24 14:41:30 2024, max compression
```

## Comparing `localretriever-0.0.2.tar` & `localretriever-0.0.3.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxr-xr-x   0 sidharthkathpal   (501) staff       (20)        0 2024-04-24 14:22:03.915070 localretriever-0.0.2/
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)     1062 2024-04-23 05:51:14.000000 localretriever-0.0.2/LICENSE
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)      908 2024-04-24 14:22:03.914963 localretriever-0.0.2/PKG-INFO
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)      409 2024-04-24 08:54:46.000000 localretriever-0.0.2/README.md
-drwxr-xr-x   0 sidharthkathpal   (501) staff       (20)        0 2024-04-24 14:22:03.912414 localretriever-0.0.2/localretriever/
-drwxr-xr-x   0 sidharthkathpal   (501) staff       (20)        0 2024-04-24 14:22:03.914626 localretriever-0.0.2/localretriever/localretriever.egg-info/
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)      908 2024-04-24 14:22:03.000000 localretriever-0.0.2/localretriever/localretriever.egg-info/PKG-INFO
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)      254 2024-04-24 14:22:03.000000 localretriever-0.0.2/localretriever/localretriever.egg-info/SOURCES.txt
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)        1 2024-04-24 14:22:03.000000 localretriever-0.0.2/localretriever/localretriever.egg-info/dependency_links.txt
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)        1 2024-04-24 14:22:03.000000 localretriever-0.0.2/localretriever/localretriever.egg-info/top_level.txt
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)      397 2024-04-24 14:20:48.000000 localretriever-0.0.2/pyproject.toml
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)      658 2024-04-24 14:22:03.915456 localretriever-0.0.2/setup.cfg
+drwxr-xr-x   0 sidharthkathpal   (501) staff       (20)        0 2024-04-24 14:41:30.697359 localretriever-0.0.3/
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)     1062 2024-04-23 05:51:14.000000 localretriever-0.0.3/LICENSE
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)     1264 2024-04-24 14:41:30.697241 localretriever-0.0.3/PKG-INFO
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)      409 2024-04-24 08:54:46.000000 localretriever-0.0.3/README.md
+drwxr-xr-x   0 sidharthkathpal   (501) staff       (20)        0 2024-04-24 14:41:30.693408 localretriever-0.0.3/localretriever/
+drwxr-xr-x   0 sidharthkathpal   (501) staff       (20)        0 2024-04-24 14:41:30.696860 localretriever-0.0.3/localretriever/localretriever.egg-info/
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)     1264 2024-04-24 14:41:30.000000 localretriever-0.0.3/localretriever/localretriever.egg-info/PKG-INFO
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)      306 2024-04-24 14:41:30.000000 localretriever-0.0.3/localretriever/localretriever.egg-info/SOURCES.txt
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)        1 2024-04-24 14:41:30.000000 localretriever-0.0.3/localretriever/localretriever.egg-info/dependency_links.txt
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)      191 2024-04-24 14:41:30.000000 localretriever-0.0.3/localretriever/localretriever.egg-info/requires.txt
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)        1 2024-04-24 14:41:30.000000 localretriever-0.0.3/localretriever/localretriever.egg-info/top_level.txt
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)      397 2024-04-24 14:20:48.000000 localretriever-0.0.3/pyproject.toml
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)      880 2024-04-24 14:41:30.697775 localretriever-0.0.3/setup.cfg
```

### Comparing `localretriever-0.0.2/LICENSE` & `localretriever-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `localretriever-0.0.2/setup.cfg` & `localretriever-0.0.3/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = localretriever
-version = 0.0.2
+version = 0.0.3
 author = Sidharth Kathpal
 author_email = kathpal.sid@gmail.com
 description = A simple Python package
 long_description = file: README.md, LICENSE.txt
 long_description_content_type = text/markdown
 url = https://github.com/GovML/retriever.git
 project_urls = 
@@ -15,14 +15,26 @@
 	Operating System :: OS Independent
 
 [options]
 package_dir = 
 	= localretriever
 packages = find:
 python_requires = >=3.9
+install_requires = 
+	haystack-ai==2.0.0
+	pymupdf==1.22.5
+	sentence-transformers==2.5.1
+	umap==0.1.1
+	umap-learn==0.5.5
+	qdrant-haystack==3.0.0
+	Flask==3.0.2
+	pandas==2.2.1
+	torch==2.2.1
+	accelerate==0.27.2
+	gradio==4.21.0
 
 [options.packages.find]
 where = localretriever
 
 [egg_info]
 tag_build = 
 tag_date = 0
```


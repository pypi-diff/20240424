# Comparing `tmp/pdf4llm-0.0.5.tar.gz` & `tmp/pdf4llm-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdf4llm-0.0.5.tar", last modified: Tue Apr 23 14:36:22 2024, max compression
+gzip compressed data, was "pdf4llm-0.0.6.tar", last modified: Wed Apr 24 21:15:24 2024, max compression
```

## Comparing `pdf4llm-0.0.5.tar` & `pdf4llm-0.0.6.tar`

### file list

```diff
@@ -1,16 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-23 14:36:22.419515 pdf4llm-0.0.5/
--rw-rw-rw-   0        0        0    35184 2024-03-21 16:34:42.000000 pdf4llm-0.0.5/LICENSE
--rw-rw-rw-   0        0        0     2516 2024-04-23 14:36:22.418515 pdf4llm-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     1979 2024-04-23 08:21:48.000000 pdf4llm-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2024-04-23 14:36:22.404515 pdf4llm-0.0.5/pdf4llm/
--rw-rw-rw-   0        0        0       46 2024-04-22 23:14:44.000000 pdf4llm-0.0.5/pdf4llm/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-23 14:36:22.416515 pdf4llm-0.0.5/pdf4llm/helpers/
--rw-rw-rw-   0        0        0    13775 2024-04-23 08:06:26.000000 pdf4llm-0.0.5/pdf4llm/helpers/pymupdf_rag.py
-drwxrwxrwx   0        0        0        0 2024-04-23 14:36:22.417516 pdf4llm-0.0.5/pdf4llm.egg-info/
--rw-rw-rw-   0        0        0     2516 2024-04-23 14:36:22.000000 pdf4llm-0.0.5/pdf4llm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      231 2024-04-23 14:36:22.000000 pdf4llm-0.0.5/pdf4llm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-23 14:36:22.000000 pdf4llm-0.0.5/pdf4llm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-04-23 14:36:22.000000 pdf4llm-0.0.5/pdf4llm.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-23 14:36:22.000000 pdf4llm-0.0.5/pdf4llm.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-23 14:36:22.419515 pdf4llm-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      950 2024-04-23 14:35:55.000000 pdf4llm-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-24 21:15:24.194383 pdf4llm-0.0.6/
+-rw-rw-rw-   0        0        0     1740 2024-04-24 21:15:24.193386 pdf4llm-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1226 2024-04-24 14:40:20.000000 pdf4llm-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2024-04-24 21:15:24.174385 pdf4llm-0.0.6/pdf4llm/
+-rw-rw-rw-   0        0        0       46 2024-04-22 23:14:44.000000 pdf4llm-0.0.6/pdf4llm/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 21:15:24.190403 pdf4llm-0.0.6/pdf4llm/helpers/
+-rw-rw-rw-   0        0        0    13775 2024-04-23 08:06:26.000000 pdf4llm-0.0.6/pdf4llm/helpers/pymupdf_rag.py
+drwxrwxrwx   0        0        0        0 2024-04-24 21:15:24.191385 pdf4llm-0.0.6/pdf4llm.egg-info/
+-rw-rw-rw-   0        0        0     1740 2024-04-24 21:15:24.000000 pdf4llm-0.0.6/pdf4llm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      223 2024-04-24 21:15:24.000000 pdf4llm-0.0.6/pdf4llm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 21:15:24.000000 pdf4llm-0.0.6/pdf4llm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-04-24 21:15:24.000000 pdf4llm-0.0.6/pdf4llm.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-24 21:15:24.000000 pdf4llm-0.0.6/pdf4llm.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-24 21:15:24.194383 pdf4llm-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      967 2024-04-24 21:14:17.000000 pdf4llm-0.0.6/setup.py
```

### Comparing `pdf4llm-0.0.5/pdf4llm/helpers/pymupdf_rag.py` & `pdf4llm-0.0.6/pdf4llm/helpers/pymupdf_rag.py`

 * *Files identical despite different names*

### Comparing `pdf4llm-0.0.5/setup.py` & `pdf4llm-0.0.6/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -13,21 +13,23 @@
     "Programming Language :: Python :: 3",
     "Topic :: Utilities",
 ]
 requires = ["pymupdf>=1.24.2"]
 
 setuptools.setup(
     name="pdf4llm",
-    version="0.0.5",
+    version="0.0.6",
     author="Artifex",
     author_email="support@artifex.com",
     description="PyMuPDF Utilities for LLM/RAG",
     packages=setuptools.find_packages(),
     long_description=readme,
     long_description_content_type="text/markdown",
     install_requires=requires,
     license="GNU AFFERO GPL 3.0",
     url="https://github.com/pymupdf/RAG",
     classifiers=classifiers,
     project_urls={},
-    package_data={"pdf4llm": ["LICENSE", "helpers/*.py"]},
+    package_data={
+        "pdf4llm": ["LICENSE", "helpers/*.py"],
+    },
 )
```


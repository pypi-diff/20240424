# Comparing `tmp/mbp-1.5.93.tar.gz` & `tmp/mbp-1.5.94.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mbp-1.5.93.tar", last modified: Tue Apr 23 00:38:33 2024, max compression
+gzip compressed data, was "mbp-1.5.94.tar", last modified: Wed Apr 24 21:53:06 2024, max compression
```

## Comparing `mbp-1.5.93.tar` & `mbp-1.5.94.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-04-23 00:38:33.442085 mbp-1.5.93/
--rw-rw-rw-   0        0        0     1088 2024-04-22 04:13:20.000000 mbp-1.5.93/LICENSE
--rw-rw-rw-   0        0        0     1621 2024-04-23 00:38:33.441089 mbp-1.5.93/PKG-INFO
--rw-rw-rw-   0        0        0     1059 2024-04-23 00:38:07.000000 mbp-1.5.93/README.md
--rw-rw-rw-   0        0        0       42 2024-04-23 00:38:33.442085 mbp-1.5.93/setup.cfg
--rw-rw-rw-   0        0        0      810 2024-04-23 00:38:18.000000 mbp-1.5.93/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-23 00:38:33.416962 mbp-1.5.93/src/
-drwxrwxrwx   0        0        0        0 2024-04-23 00:38:33.426216 mbp-1.5.93/src/mbp/
--rw-rw-rw-   0        0        0       19 2024-04-22 04:13:20.000000 mbp-1.5.93/src/mbp/__init__.py
--rw-rw-rw-   0        0        0    37389 2024-04-23 00:37:38.000000 mbp-1.5.93/src/mbp/core.py
--rw-rw-rw-   0        0        0      374 2024-04-23 00:38:13.000000 mbp-1.5.93/src/mbp/info.py
--rw-rw-rw-   0        0        0     1774 2024-04-22 04:13:20.000000 mbp-1.5.93/src/mbp/llm.py
--rw-rw-rw-   0        0        0      149 2024-04-22 04:13:20.000000 mbp-1.5.93/src/mbp/sync.py
-drwxrwxrwx   0        0        0        0 2024-04-23 00:38:33.439703 mbp-1.5.93/src/mbp.egg-info/
--rw-rw-rw-   0        0        0     1621 2024-04-23 00:38:33.000000 mbp-1.5.93/src/mbp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      263 2024-04-23 00:38:33.000000 mbp-1.5.93/src/mbp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-23 00:38:33.000000 mbp-1.5.93/src/mbp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2024-04-23 00:38:33.000000 mbp-1.5.93/src/mbp.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2024-04-23 00:38:33.000000 mbp-1.5.93/src/mbp.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-24 21:53:06.286293 mbp-1.5.94/
+-rw-rw-rw-   0        0        0     1088 2024-04-22 04:13:20.000000 mbp-1.5.94/LICENSE
+-rw-rw-rw-   0        0        0     1621 2024-04-24 21:53:06.285291 mbp-1.5.94/PKG-INFO
+-rw-rw-rw-   0        0        0     1059 2024-04-24 21:51:16.000000 mbp-1.5.94/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-24 21:53:06.287300 mbp-1.5.94/setup.cfg
+-rw-rw-rw-   0        0        0      810 2024-04-24 21:51:05.000000 mbp-1.5.94/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-24 21:53:06.251293 mbp-1.5.94/src/
+drwxrwxrwx   0        0        0        0 2024-04-24 21:53:06.266294 mbp-1.5.94/src/mbp/
+-rw-rw-rw-   0        0        0       19 2024-04-22 04:13:20.000000 mbp-1.5.94/src/mbp/__init__.py
+-rw-rw-rw-   0        0        0    37389 2024-04-23 00:37:38.000000 mbp-1.5.94/src/mbp/core.py
+-rw-rw-rw-   0        0        0      374 2024-04-24 21:51:09.000000 mbp-1.5.94/src/mbp/info.py
+-rw-rw-rw-   0        0        0     1774 2024-04-22 04:13:20.000000 mbp-1.5.94/src/mbp/llm.py
+-rw-rw-rw-   0        0        0      149 2024-04-22 04:13:20.000000 mbp-1.5.94/src/mbp/sync.py
+drwxrwxrwx   0        0        0        0 2024-04-24 21:53:06.284291 mbp-1.5.94/src/mbp.egg-info/
+-rw-rw-rw-   0        0        0     1621 2024-04-24 21:53:06.000000 mbp-1.5.94/src/mbp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      263 2024-04-24 21:53:06.000000 mbp-1.5.94/src/mbp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 21:53:06.000000 mbp-1.5.94/src/mbp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2024-04-24 21:53:06.000000 mbp-1.5.94/src/mbp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2024-04-24 21:53:06.000000 mbp-1.5.94/src/mbp.egg-info/top_level.txt
```

### Comparing `mbp-1.5.93/LICENSE` & `mbp-1.5.94/LICENSE`

 * *Files identical despite different names*

### Comparing `mbp-1.5.93/PKG-INFO` & `mbp-1.5.94/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: mbp
-Version: 1.5.93
+Version: 1.5.94
 Summary: Make Python even more beautiful :) This package includes implementations that you wish were in the standard library.
 Home-page: https://github.com/sudongqi/MoreBeautifulPython.git
 Author: Dongqi Su
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.12.0
+Requires-Python: >=3.11.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: wcwidth>=0.2.5
 Requires-Dist: pyyaml>=5.1
 
 ## More Beautiful Python
 
@@ -22,15 +22,15 @@
     python -m pip install mbp
     python -m mbp.info
     =================================== More Beautiful Python ===================================
     examples              https://github.com/sudongqi/MoreBeautifulPython/blob/main/examples.py
     execution_directory   C:\Users\sudon\MoreBeautifulPython
     library_path          C:\Users\sudon\MoreBeautifulPython\src\mbp\core.py
     cpu_count             16
-    version               1.5.93
+    version               1.5.94
     =============================================================================================
 
 ### Examples
 
 https://github.com/sudongqi/MoreBeautifulPython/blob/main/examples.py
 
 -   replacement for logging
```

### Comparing `mbp-1.5.93/README.md` & `mbp-1.5.94/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     python -m pip install mbp
     python -m mbp.info
     =================================== More Beautiful Python ===================================
     examples              https://github.com/sudongqi/MoreBeautifulPython/blob/main/examples.py
     execution_directory   C:\Users\sudon\MoreBeautifulPython
     library_path          C:\Users\sudon\MoreBeautifulPython\src\mbp\core.py
     cpu_count             16
-    version               1.5.93
+    version               1.5.94
     =============================================================================================
 
 ### Examples
 
 https://github.com/sudongqi/MoreBeautifulPython/blob/main/examples.py
 
 -   replacement for logging
```

### Comparing `mbp-1.5.93/setup.py` & `mbp-1.5.94/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from setuptools import setup, find_packages
 
 setup(
     name="mbp",
-    version="1.5.93",
+    version="1.5.94",
     author="Dongqi Su",
     description="Make Python even more beautiful :) This package includes implementations that you wish were in the standard library.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/sudongqi/MoreBeautifulPython.git",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     py_modules=["mbp"],
     package_dir={"": "src"},
     packages=find_packages(where="src"),
-    python_requires=">=3.12.0",
+    python_requires=">=3.11.0",
     install_requires=[
         "wcwidth>=0.2.5",
         "pyyaml>=5.1",
     ],
 )
```

### Comparing `mbp-1.5.93/src/mbp/core.py` & `mbp-1.5.94/src/mbp/core.py`

 * *Files identical despite different names*

### Comparing `mbp-1.5.93/src/mbp/llm.py` & `mbp-1.5.94/src/mbp/llm.py`

 * *Files identical despite different names*

### Comparing `mbp-1.5.93/src/mbp.egg-info/PKG-INFO` & `mbp-1.5.94/src/mbp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: mbp
-Version: 1.5.93
+Version: 1.5.94
 Summary: Make Python even more beautiful :) This package includes implementations that you wish were in the standard library.
 Home-page: https://github.com/sudongqi/MoreBeautifulPython.git
 Author: Dongqi Su
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.12.0
+Requires-Python: >=3.11.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: wcwidth>=0.2.5
 Requires-Dist: pyyaml>=5.1
 
 ## More Beautiful Python
 
@@ -22,15 +22,15 @@
     python -m pip install mbp
     python -m mbp.info
     =================================== More Beautiful Python ===================================
     examples              https://github.com/sudongqi/MoreBeautifulPython/blob/main/examples.py
     execution_directory   C:\Users\sudon\MoreBeautifulPython
     library_path          C:\Users\sudon\MoreBeautifulPython\src\mbp\core.py
     cpu_count             16
-    version               1.5.93
+    version               1.5.94
     =============================================================================================
 
 ### Examples
 
 https://github.com/sudongqi/MoreBeautifulPython/blob/main/examples.py
 
 -   replacement for logging
```


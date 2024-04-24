# Comparing `tmp/lightningtoolkit-1.0.2.tar.gz` & `tmp/lightningtoolkit-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lightningtoolkit-1.0.2.tar", last modified: Wed Apr 24 12:34:53 2024, max compression
+gzip compressed data, was "lightningtoolkit-1.0.4.tar", last modified: Wed Apr 24 12:52:26 2024, max compression
```

## Comparing `lightningtoolkit-1.0.2.tar` & `lightningtoolkit-1.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 gqx       (1000) gqx       (1000)        0 2024-04-24 12:34:53.821962 lightningtoolkit-1.0.2/
--rw-rw-r--   0 gqx       (1000) gqx       (1000)     1070 2024-04-21 10:28:28.000000 lightningtoolkit-1.0.2/LICENSE
--rw-r--r--   0 gqx       (1000) gqx       (1000)     3462 2024-04-24 12:34:53.821962 lightningtoolkit-1.0.2/PKG-INFO
--rwx------   0 gqx       (1000) gqx       (1000)     2210 2024-04-24 12:07:15.000000 lightningtoolkit-1.0.2/README.md
-drwxrwxr-x   0 gqx       (1000) gqx       (1000)        0 2024-04-24 12:34:53.821962 lightningtoolkit-1.0.2/lightningtoolkit/
--rw-rw-r--   0 gqx       (1000) gqx       (1000)       32 2024-04-24 12:13:50.000000 lightningtoolkit-1.0.2/lightningtoolkit/__init__.py
--rwx------   0 gqx       (1000) gqx       (1000)     9067 2024-04-24 12:00:03.000000 lightningtoolkit-1.0.2/lightningtoolkit/run.py
-drwxrwxr-x   0 gqx       (1000) gqx       (1000)        0 2024-04-24 12:34:53.821962 lightningtoolkit-1.0.2/lightningtoolkit.egg-info/
--rw-r--r--   0 gqx       (1000) gqx       (1000)     3462 2024-04-24 12:34:53.000000 lightningtoolkit-1.0.2/lightningtoolkit.egg-info/PKG-INFO
--rw-rw-r--   0 gqx       (1000) gqx       (1000)      239 2024-04-24 12:34:53.000000 lightningtoolkit-1.0.2/lightningtoolkit.egg-info/SOURCES.txt
--rw-rw-r--   0 gqx       (1000) gqx       (1000)        1 2024-04-24 12:34:53.000000 lightningtoolkit-1.0.2/lightningtoolkit.egg-info/dependency_links.txt
--rw-rw-r--   0 gqx       (1000) gqx       (1000)       17 2024-04-24 12:34:53.000000 lightningtoolkit-1.0.2/lightningtoolkit.egg-info/top_level.txt
--rw-rw-r--   0 gqx       (1000) gqx       (1000)       38 2024-04-24 12:34:53.821962 lightningtoolkit-1.0.2/setup.cfg
--rw-rw-r--   0 gqx       (1000) gqx       (1000)     1353 2024-04-24 12:34:30.000000 lightningtoolkit-1.0.2/setup.py
+drwxrwxr-x   0 gqx       (1000) gqx       (1000)        0 2024-04-24 12:52:26.269863 lightningtoolkit-1.0.4/
+-rw-rw-r--   0 gqx       (1000) gqx       (1000)     1070 2024-04-21 10:28:28.000000 lightningtoolkit-1.0.4/LICENSE
+-rw-r--r--   0 gqx       (1000) gqx       (1000)     3462 2024-04-24 12:52:26.269863 lightningtoolkit-1.0.4/PKG-INFO
+-rwx------   0 gqx       (1000) gqx       (1000)     2210 2024-04-24 12:52:22.000000 lightningtoolkit-1.0.4/README.md
+drwxrwxr-x   0 gqx       (1000) gqx       (1000)        0 2024-04-24 12:52:26.269863 lightningtoolkit-1.0.4/lightningtoolkit/
+-rw-rw-r--   0 gqx       (1000) gqx       (1000)       32 2024-04-24 12:51:44.000000 lightningtoolkit-1.0.4/lightningtoolkit/__init__.py
+-rwx------   0 gqx       (1000) gqx       (1000)     9060 2024-04-24 12:38:37.000000 lightningtoolkit-1.0.4/lightningtoolkit/run.py
+drwxrwxr-x   0 gqx       (1000) gqx       (1000)        0 2024-04-24 12:52:26.269863 lightningtoolkit-1.0.4/lightningtoolkit.egg-info/
+-rw-r--r--   0 gqx       (1000) gqx       (1000)     3462 2024-04-24 12:52:26.000000 lightningtoolkit-1.0.4/lightningtoolkit.egg-info/PKG-INFO
+-rw-rw-r--   0 gqx       (1000) gqx       (1000)      239 2024-04-24 12:52:26.000000 lightningtoolkit-1.0.4/lightningtoolkit.egg-info/SOURCES.txt
+-rw-rw-r--   0 gqx       (1000) gqx       (1000)        1 2024-04-24 12:52:26.000000 lightningtoolkit-1.0.4/lightningtoolkit.egg-info/dependency_links.txt
+-rw-rw-r--   0 gqx       (1000) gqx       (1000)       17 2024-04-24 12:52:26.000000 lightningtoolkit-1.0.4/lightningtoolkit.egg-info/top_level.txt
+-rw-rw-r--   0 gqx       (1000) gqx       (1000)       38 2024-04-24 12:52:26.273863 lightningtoolkit-1.0.4/setup.cfg
+-rw-rw-r--   0 gqx       (1000) gqx       (1000)     1353 2024-04-24 12:51:49.000000 lightningtoolkit-1.0.4/setup.py
```

### Comparing `lightningtoolkit-1.0.2/LICENSE` & `lightningtoolkit-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `lightningtoolkit-1.0.2/PKG-INFO` & `lightningtoolkit-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightningtoolkit
-Version: 1.0.2
+Version: 1.0.4
 Summary: A toolkit that combines many functions
 Home-page: https://github.com/BinaryGuo/Lightning_Toolkit
 Author: GQX
 Author-email: kill114514251@outlook.com
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Natural Language :: English
@@ -35,15 +35,15 @@
 ### Project Description
 - This project is a toolkit
 - Github: https://github.com/BinaryGuo/Lightning_Toolkit/
 - Problem feedback: https://github.com/BinaryGuo/Lightning_Toolkit/issues
 - Contact email (GQX): kill114514251@outlook.com
 - TestPyPI: Same name
 ## Version
-- 1.0.0
+- 1.0.4
 ### Development environment
 - Ubuntu Linux 22.04
 - Python 3.10.12
 ### Change instructions
 #### 1.0 (this version)
 - This version is the first version
 - Add:
@@ -79,15 +79,15 @@
 - 此项目是一个工具包
 - github：https://github.com/BinaryGuo/Lightning_Toolkit/
 - 问题反馈：https://github.com/BinaryGuo/Lightning_Toolkit/issues
 - 联系邮箱（GQX）：kill114514251@outlook.com
 - testPyPI：同名
 
 ## 版本
-- 1.0.0
+- 1.0.4
 
 ### 开发环境
 - Ubuntu Linux 22.04
 - Python 3.10.12
 
 ### 改动说明
```

### Comparing `lightningtoolkit-1.0.2/README.md` & `lightningtoolkit-1.0.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ### Project Description
 - This project is a toolkit
 - Github: https://github.com/BinaryGuo/Lightning_Toolkit/
 - Problem feedback: https://github.com/BinaryGuo/Lightning_Toolkit/issues
 - Contact email (GQX): kill114514251@outlook.com
 - TestPyPI: Same name
 ## Version
-- 1.0.0
+- 1.0.4
 ### Development environment
 - Ubuntu Linux 22.04
 - Python 3.10.12
 ### Change instructions
 #### 1.0 (this version)
 - This version is the first version
 - Add:
@@ -49,15 +49,15 @@
 - 此项目是一个工具包
 - github：https://github.com/BinaryGuo/Lightning_Toolkit/
 - 问题反馈：https://github.com/BinaryGuo/Lightning_Toolkit/issues
 - 联系邮箱（GQX）：kill114514251@outlook.com
 - testPyPI：同名
 
 ## 版本
-- 1.0.0
+- 1.0.4
 
 ### 开发环境
 - Ubuntu Linux 22.04
 - Python 3.10.12
 
 ### 改动说明
```

### Comparing `lightningtoolkit-1.0.2/lightningtoolkit/run.py` & `lightningtoolkit-1.0.4/lightningtoolkit/run.py`

 * *Files 1% similar despite different names*

```diff
@@ -174,10 +174,8 @@
             print(eval(input('please enter formula: ')))
             break
         except:print("Enter Error")
     judge2(calculator)
 
 def run():
     logo()
-    while True:judge()
-
-run()
+    while True:judge()
```

### Comparing `lightningtoolkit-1.0.2/lightningtoolkit.egg-info/PKG-INFO` & `lightningtoolkit-1.0.4/lightningtoolkit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightningtoolkit
-Version: 1.0.2
+Version: 1.0.4
 Summary: A toolkit that combines many functions
 Home-page: https://github.com/BinaryGuo/Lightning_Toolkit
 Author: GQX
 Author-email: kill114514251@outlook.com
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Natural Language :: English
@@ -35,15 +35,15 @@
 ### Project Description
 - This project is a toolkit
 - Github: https://github.com/BinaryGuo/Lightning_Toolkit/
 - Problem feedback: https://github.com/BinaryGuo/Lightning_Toolkit/issues
 - Contact email (GQX): kill114514251@outlook.com
 - TestPyPI: Same name
 ## Version
-- 1.0.0
+- 1.0.4
 ### Development environment
 - Ubuntu Linux 22.04
 - Python 3.10.12
 ### Change instructions
 #### 1.0 (this version)
 - This version is the first version
 - Add:
@@ -79,15 +79,15 @@
 - 此项目是一个工具包
 - github：https://github.com/BinaryGuo/Lightning_Toolkit/
 - 问题反馈：https://github.com/BinaryGuo/Lightning_Toolkit/issues
 - 联系邮箱（GQX）：kill114514251@outlook.com
 - testPyPI：同名
 
 ## 版本
-- 1.0.0
+- 1.0.4
 
 ### 开发环境
 - Ubuntu Linux 22.04
 - Python 3.10.12
 
 ### 改动说明
```

### Comparing `lightningtoolkit-1.0.2/setup.py` & `lightningtoolkit-1.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup,find_packages
 with open("README.md", "r", encoding="utf-8") as fh:
     description = fh.read()
 setup(
 name = "lightningtoolkit",
-version = "1.0.2",
+version = "1.0.4",
 author = "GQX",
 author_email = "kill114514251@outlook.com",
 packages = find_packages(),
 description = "A toolkit that combines many functions",
 long_description_content_type = "text/markdown",
 long_description = description,
 url = "https://github.com/BinaryGuo/Lightning_Toolkit",
```


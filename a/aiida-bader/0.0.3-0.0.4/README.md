# Comparing `tmp/aiida_bader-0.0.3.tar.gz` & `tmp/aiida_bader-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiida_bader-0.0.3.tar", last modified: Wed Apr 24 13:00:54 2024, max compression
+gzip compressed data, was "aiida_bader-0.0.4.tar", last modified: Wed Apr 24 14:50:59 2024, max compression
```

## Comparing `aiida_bader-0.0.3.tar` & `aiida_bader-0.0.4.tar`

### file list

```diff
@@ -1,35 +1,36 @@
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2024-04-24 13:00:54.091826 aiida_bader-0.0.3/
--rw-rw-r--   0 xing      (1000) xing      (1000)     1066 2024-03-25 15:26:07.000000 aiida_bader-0.0.3/LICENSE
--rw-r--r--   0 xing      (1000) xing      (1000)     2136 2024-04-24 13:00:54.091826 aiida_bader-0.0.3/PKG-INFO
--rw-rw-r--   0 xing      (1000) xing      (1000)     1606 2024-03-25 15:26:07.000000 aiida_bader-0.0.3/README.md
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2024-04-24 13:00:54.091826 aiida_bader-0.0.3/aiida_bader/
--rw-rw-r--   0 xing      (1000) xing      (1000)        0 2024-03-25 15:26:07.000000 aiida_bader-0.0.3/aiida_bader/__init__.py
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2024-04-24 13:00:54.091826 aiida_bader-0.0.3/aiida_bader/calculations/
--rw-rw-r--   0 xing      (1000) xing      (1000)     3680 2024-03-25 15:26:07.000000 aiida_bader-0.0.3/aiida_bader/calculations/__init__.py
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2024-04-24 13:00:54.091826 aiida_bader-0.0.3/aiida_bader/parsers/
--rw-rw-r--   0 xing      (1000) xing      (1000)     2005 2024-03-25 15:26:07.000000 aiida_bader-0.0.3/aiida_bader/parsers/__init__.py
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2024-04-24 13:00:54.091826 aiida_bader-0.0.3/aiida_bader/qeapp/
--rw-rw-r--   0 xing      (1000) xing      (1000)      657 2024-03-25 15:26:07.000000 aiida_bader-0.0.3/aiida_bader/qeapp/__init__.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     3858 2024-04-10 19:56:14.000000 aiida_bader-0.0.3/aiida_bader/qeapp/result.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     2857 2024-04-10 19:56:14.000000 aiida_bader-0.0.3/aiida_bader/qeapp/widget.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     2758 2024-04-10 19:56:14.000000 aiida_bader-0.0.3/aiida_bader/qeapp/workchain.py
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2024-04-24 13:00:54.091826 aiida_bader-0.0.3/aiida_bader/workchains/
--rw-rw-r--   0 xing      (1000) xing      (1000)       93 2024-03-25 15:26:07.000000 aiida_bader-0.0.3/aiida_bader/workchains/__init__.py
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2024-04-24 13:00:54.091826 aiida_bader-0.0.3/aiida_bader/workchains/protocols/
--rw-rw-r--   0 xing      (1000) xing      (1000)        0 2024-03-25 15:26:07.000000 aiida_bader-0.0.3/aiida_bader/workchains/protocols/__init__.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     8003 2024-03-25 15:26:07.000000 aiida_bader-0.0.3/aiida_bader/workchains/qe_bader.py
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2024-04-24 13:00:54.091826 aiida_bader-0.0.3/aiida_bader/worktrees/
--rw-rw-r--   0 xing      (1000) xing      (1000)        0 2024-03-25 15:26:07.000000 aiida_bader-0.0.3/aiida_bader/worktrees/__init__.py
--rw-rw-r--   0 xing      (1000) xing      (1000)      635 2024-03-25 15:26:07.000000 aiida_bader-0.0.3/aiida_bader/worktrees/cp2k_bader.py
--rw-rw-r--   0 xing      (1000) xing      (1000)      903 2024-04-10 19:55:50.000000 aiida_bader-0.0.3/aiida_bader/worktrees/qe_bader.py
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2024-04-24 13:00:54.091826 aiida_bader-0.0.3/aiida_bader.egg-info/
--rw-r--r--   0 xing      (1000) xing      (1000)     2136 2024-04-24 13:00:54.000000 aiida_bader-0.0.3/aiida_bader.egg-info/PKG-INFO
--rw-rw-r--   0 xing      (1000) xing      (1000)      687 2024-04-24 13:00:54.000000 aiida_bader-0.0.3/aiida_bader.egg-info/SOURCES.txt
--rw-rw-r--   0 xing      (1000) xing      (1000)        1 2024-04-24 13:00:54.000000 aiida_bader-0.0.3/aiida_bader.egg-info/dependency_links.txt
--rw-rw-r--   0 xing      (1000) xing      (1000)      256 2024-04-24 13:00:54.000000 aiida_bader-0.0.3/aiida_bader.egg-info/entry_points.txt
--rw-rw-r--   0 xing      (1000) xing      (1000)      100 2024-04-24 13:00:54.000000 aiida_bader-0.0.3/aiida_bader.egg-info/requires.txt
--rw-rw-r--   0 xing      (1000) xing      (1000)       12 2024-04-24 13:00:54.000000 aiida_bader-0.0.3/aiida_bader.egg-info/top_level.txt
--rw-rw-r--   0 xing      (1000) xing      (1000)       38 2024-04-24 13:00:54.091826 aiida_bader-0.0.3/setup.cfg
--rw-rw-r--   0 xing      (1000) xing      (1000)     1491 2024-04-24 13:00:45.000000 aiida_bader-0.0.3/setup.py
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2024-04-24 13:00:54.091826 aiida_bader-0.0.3/tests/
--rw-rw-r--   0 xing      (1000) xing      (1000)      122 2024-03-25 15:26:07.000000 aiida_bader-0.0.3/tests/test_bader.py
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2024-04-24 14:50:59.706954 aiida_bader-0.0.4/
+-rw-rw-r--   0 xing      (1000) xing      (1000)     1066 2024-03-25 15:26:07.000000 aiida_bader-0.0.4/LICENSE
+-rw-r--r--   0 xing      (1000) xing      (1000)     2136 2024-04-24 14:50:59.706954 aiida_bader-0.0.4/PKG-INFO
+-rw-rw-r--   0 xing      (1000) xing      (1000)     1606 2024-03-25 15:26:07.000000 aiida_bader-0.0.4/README.md
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2024-04-24 14:50:59.706954 aiida_bader-0.0.4/aiida_bader/
+-rw-rw-r--   0 xing      (1000) xing      (1000)        0 2024-03-25 15:26:07.000000 aiida_bader-0.0.4/aiida_bader/__init__.py
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2024-04-24 14:50:59.706954 aiida_bader-0.0.4/aiida_bader/calculations/
+-rw-rw-r--   0 xing      (1000) xing      (1000)     3680 2024-03-25 15:26:07.000000 aiida_bader-0.0.4/aiida_bader/calculations/__init__.py
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2024-04-24 14:50:59.706954 aiida_bader-0.0.4/aiida_bader/parsers/
+-rw-rw-r--   0 xing      (1000) xing      (1000)     2005 2024-03-25 15:26:07.000000 aiida_bader-0.0.4/aiida_bader/parsers/__init__.py
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2024-04-24 14:50:59.706954 aiida_bader-0.0.4/aiida_bader/qeapp/
+-rw-rw-r--   0 xing      (1000) xing      (1000)      657 2024-03-25 15:26:07.000000 aiida_bader-0.0.4/aiida_bader/qeapp/__init__.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     3858 2024-04-10 19:56:14.000000 aiida_bader-0.0.4/aiida_bader/qeapp/result.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     2857 2024-04-10 19:56:14.000000 aiida_bader-0.0.4/aiida_bader/qeapp/widget.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     2758 2024-04-10 19:56:14.000000 aiida_bader-0.0.4/aiida_bader/qeapp/workchain.py
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2024-04-24 14:50:59.706954 aiida_bader-0.0.4/aiida_bader/workchains/
+-rw-rw-r--   0 xing      (1000) xing      (1000)       93 2024-03-25 15:26:07.000000 aiida_bader-0.0.4/aiida_bader/workchains/__init__.py
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2024-04-24 14:50:59.706954 aiida_bader-0.0.4/aiida_bader/workchains/protocols/
+-rw-rw-r--   0 xing      (1000) xing      (1000)        0 2024-03-25 15:26:07.000000 aiida_bader-0.0.4/aiida_bader/workchains/protocols/__init__.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     1196 2024-03-25 15:26:07.000000 aiida_bader-0.0.4/aiida_bader/workchains/protocols/bader.yaml
+-rw-rw-r--   0 xing      (1000) xing      (1000)     8003 2024-03-25 15:26:07.000000 aiida_bader-0.0.4/aiida_bader/workchains/qe_bader.py
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2024-04-24 14:50:59.706954 aiida_bader-0.0.4/aiida_bader/worktrees/
+-rw-rw-r--   0 xing      (1000) xing      (1000)        0 2024-03-25 15:26:07.000000 aiida_bader-0.0.4/aiida_bader/worktrees/__init__.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)      635 2024-03-25 15:26:07.000000 aiida_bader-0.0.4/aiida_bader/worktrees/cp2k_bader.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)      903 2024-04-10 19:55:50.000000 aiida_bader-0.0.4/aiida_bader/worktrees/qe_bader.py
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2024-04-24 14:50:59.706954 aiida_bader-0.0.4/aiida_bader.egg-info/
+-rw-r--r--   0 xing      (1000) xing      (1000)     2136 2024-04-24 14:50:59.000000 aiida_bader-0.0.4/aiida_bader.egg-info/PKG-INFO
+-rw-rw-r--   0 xing      (1000) xing      (1000)      731 2024-04-24 14:50:59.000000 aiida_bader-0.0.4/aiida_bader.egg-info/SOURCES.txt
+-rw-rw-r--   0 xing      (1000) xing      (1000)        1 2024-04-24 14:50:59.000000 aiida_bader-0.0.4/aiida_bader.egg-info/dependency_links.txt
+-rw-rw-r--   0 xing      (1000) xing      (1000)      256 2024-04-24 14:50:59.000000 aiida_bader-0.0.4/aiida_bader.egg-info/entry_points.txt
+-rw-rw-r--   0 xing      (1000) xing      (1000)      100 2024-04-24 14:50:59.000000 aiida_bader-0.0.4/aiida_bader.egg-info/requires.txt
+-rw-rw-r--   0 xing      (1000) xing      (1000)       12 2024-04-24 14:50:59.000000 aiida_bader-0.0.4/aiida_bader.egg-info/top_level.txt
+-rw-rw-r--   0 xing      (1000) xing      (1000)       38 2024-04-24 14:50:59.706954 aiida_bader-0.0.4/setup.cfg
+-rw-rw-r--   0 xing      (1000) xing      (1000)     1556 2024-04-24 14:50:48.000000 aiida_bader-0.0.4/setup.py
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2024-04-24 14:50:59.706954 aiida_bader-0.0.4/tests/
+-rw-rw-r--   0 xing      (1000) xing      (1000)      122 2024-03-25 15:26:07.000000 aiida_bader-0.0.4/tests/test_bader.py
```

### Comparing `aiida_bader-0.0.3/LICENSE` & `aiida_bader-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `aiida_bader-0.0.3/PKG-INFO` & `aiida_bader-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiida-bader
-Version: 0.0.3
+Version: 0.0.4
 Summary: AiiDA plugin for bader code.
 Home-page: https://github.com/superstart54/aiida-bader
 Author: Xing Wang
 Author-email: xingwang1991@gmail.com
 License: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `aiida_bader-0.0.3/README.md` & `aiida_bader-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `aiida_bader-0.0.3/aiida_bader/calculations/__init__.py` & `aiida_bader-0.0.4/aiida_bader/calculations/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida_bader-0.0.3/aiida_bader/parsers/__init__.py` & `aiida_bader-0.0.4/aiida_bader/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida_bader-0.0.3/aiida_bader/qeapp/__init__.py` & `aiida_bader-0.0.4/aiida_bader/qeapp/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida_bader-0.0.3/aiida_bader/qeapp/result.py` & `aiida_bader-0.0.4/aiida_bader/qeapp/result.py`

 * *Files identical despite different names*

### Comparing `aiida_bader-0.0.3/aiida_bader/qeapp/widget.py` & `aiida_bader-0.0.4/aiida_bader/qeapp/widget.py`

 * *Files identical despite different names*

### Comparing `aiida_bader-0.0.3/aiida_bader/qeapp/workchain.py` & `aiida_bader-0.0.4/aiida_bader/qeapp/workchain.py`

 * *Files identical despite different names*

### Comparing `aiida_bader-0.0.3/aiida_bader/workchains/qe_bader.py` & `aiida_bader-0.0.4/aiida_bader/workchains/qe_bader.py`

 * *Files identical despite different names*

### Comparing `aiida_bader-0.0.3/aiida_bader/worktrees/cp2k_bader.py` & `aiida_bader-0.0.4/aiida_bader/worktrees/cp2k_bader.py`

 * *Files identical despite different names*

### Comparing `aiida_bader-0.0.3/aiida_bader/worktrees/qe_bader.py` & `aiida_bader-0.0.4/aiida_bader/worktrees/qe_bader.py`

 * *Files identical despite different names*

### Comparing `aiida_bader-0.0.3/aiida_bader.egg-info/PKG-INFO` & `aiida_bader-0.0.4/aiida_bader.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiida-bader
-Version: 0.0.3
+Version: 0.0.4
 Summary: AiiDA plugin for bader code.
 Home-page: https://github.com/superstart54/aiida-bader
 Author: Xing Wang
 Author-email: xingwang1991@gmail.com
 License: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `aiida_bader-0.0.3/aiida_bader.egg-info/SOURCES.txt` & `aiida_bader-0.0.4/aiida_bader.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -13,11 +13,12 @@
 aiida_bader/qeapp/__init__.py
 aiida_bader/qeapp/result.py
 aiida_bader/qeapp/widget.py
 aiida_bader/qeapp/workchain.py
 aiida_bader/workchains/__init__.py
 aiida_bader/workchains/qe_bader.py
 aiida_bader/workchains/protocols/__init__.py
+aiida_bader/workchains/protocols/bader.yaml
 aiida_bader/worktrees/__init__.py
 aiida_bader/worktrees/cp2k_bader.py
 aiida_bader/worktrees/qe_bader.py
 tests/test_bader.py
```

### Comparing `aiida_bader-0.0.3/setup.py` & `aiida_bader-0.0.4/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 HERE = pathlib.Path(__file__).parent
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 setup(
     name="aiida-bader",
-    version="0.0.3",
+    version="0.0.4",
     description="AiiDA plugin for bader code.",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/superstart54/aiida-bader",
     author="Xing Wang",
     author_email="xingwang1991@gmail.com",
     license="MIT License",
@@ -48,11 +48,13 @@
         "aiida.workflows": [
             "bader.qe = aiida_bader.workchains:QeBaderWorkChain",
         ],
         "aiidalab_qe.properties": [
             "bader = aiida_bader.qeapp:bader",
         ],
     },
-    package_data={},
+    package_data={
+        "aiida_bader.workchains.protocols": ["bader.yaml"],
+    },
     python_requires=">=3.9",
     test_suite="setup.test_suite",
 )
```


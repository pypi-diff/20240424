# Comparing `tmp/aiida-bader-0.0.2.tar.gz` & `tmp/aiida_bader-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiida-bader-0.0.2.tar", last modified: Mon Mar 25 15:26:42 2024, max compression
+gzip compressed data, was "aiida_bader-0.0.3.tar", last modified: Wed Apr 24 13:00:54 2024, max compression
```

## Comparing `aiida-bader-0.0.2.tar` & `aiida_bader-0.0.3.tar`

### file list

```diff
@@ -1,34 +1,35 @@
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2024-03-25 15:26:42.438766 aiida-bader-0.0.2/
--rw-rw-r--   0 xing      (1000) xing      (1000)     1066 2024-03-25 15:26:07.000000 aiida-bader-0.0.2/LICENSE
--rw-r--r--   0 xing      (1000) xing      (1000)     2114 2024-03-25 15:26:42.438766 aiida-bader-0.0.2/PKG-INFO
--rw-rw-r--   0 xing      (1000) xing      (1000)     1606 2024-03-25 15:26:07.000000 aiida-bader-0.0.2/README.md
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2024-03-25 15:26:42.438766 aiida-bader-0.0.2/aiida_bader/
--rw-rw-r--   0 xing      (1000) xing      (1000)        0 2024-03-25 15:26:07.000000 aiida-bader-0.0.2/aiida_bader/__init__.py
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2024-03-25 15:26:42.438766 aiida-bader-0.0.2/aiida_bader/calculations/
--rw-rw-r--   0 xing      (1000) xing      (1000)     3680 2024-03-25 15:26:07.000000 aiida-bader-0.0.2/aiida_bader/calculations/__init__.py
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2024-03-25 15:26:42.438766 aiida-bader-0.0.2/aiida_bader/parsers/
--rw-rw-r--   0 xing      (1000) xing      (1000)     2005 2024-03-25 15:26:07.000000 aiida-bader-0.0.2/aiida_bader/parsers/__init__.py
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2024-03-25 15:26:42.438766 aiida-bader-0.0.2/aiida_bader/qeapp/
--rw-rw-r--   0 xing      (1000) xing      (1000)      657 2024-03-25 15:26:07.000000 aiida-bader-0.0.2/aiida_bader/qeapp/__init__.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     2538 2024-03-25 15:26:07.000000 aiida-bader-0.0.2/aiida_bader/qeapp/result.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     2600 2024-03-25 15:26:07.000000 aiida-bader-0.0.2/aiida_bader/qeapp/workchain.py
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2024-03-25 15:26:42.438766 aiida-bader-0.0.2/aiida_bader/workchains/
--rw-rw-r--   0 xing      (1000) xing      (1000)       93 2024-03-25 15:26:07.000000 aiida-bader-0.0.2/aiida_bader/workchains/__init__.py
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2024-03-25 15:26:42.438766 aiida-bader-0.0.2/aiida_bader/workchains/protocols/
--rw-rw-r--   0 xing      (1000) xing      (1000)        0 2024-03-25 15:26:07.000000 aiida-bader-0.0.2/aiida_bader/workchains/protocols/__init__.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     8003 2024-03-25 15:26:07.000000 aiida-bader-0.0.2/aiida_bader/workchains/qe_bader.py
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2024-03-25 15:26:42.438766 aiida-bader-0.0.2/aiida_bader/worktrees/
--rw-rw-r--   0 xing      (1000) xing      (1000)        0 2024-03-25 15:26:07.000000 aiida-bader-0.0.2/aiida_bader/worktrees/__init__.py
--rw-rw-r--   0 xing      (1000) xing      (1000)      635 2024-03-25 15:26:07.000000 aiida-bader-0.0.2/aiida_bader/worktrees/cp2k_bader.py
--rw-rw-r--   0 xing      (1000) xing      (1000)      903 2024-03-25 15:26:07.000000 aiida-bader-0.0.2/aiida_bader/worktrees/qe_bader.py
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2024-03-25 15:26:42.438766 aiida-bader-0.0.2/aiida_bader.egg-info/
--rw-r--r--   0 xing      (1000) xing      (1000)     2114 2024-03-25 15:26:42.000000 aiida-bader-0.0.2/aiida_bader.egg-info/PKG-INFO
--rw-rw-r--   0 xing      (1000) xing      (1000)      659 2024-03-25 15:26:42.000000 aiida-bader-0.0.2/aiida_bader.egg-info/SOURCES.txt
--rw-rw-r--   0 xing      (1000) xing      (1000)        1 2024-03-25 15:26:42.000000 aiida-bader-0.0.2/aiida_bader.egg-info/dependency_links.txt
--rw-rw-r--   0 xing      (1000) xing      (1000)      256 2024-03-25 15:26:42.000000 aiida-bader-0.0.2/aiida_bader.egg-info/entry_points.txt
--rw-rw-r--   0 xing      (1000) xing      (1000)       93 2024-03-25 15:26:42.000000 aiida-bader-0.0.2/aiida_bader.egg-info/requires.txt
--rw-rw-r--   0 xing      (1000) xing      (1000)       12 2024-03-25 15:26:42.000000 aiida-bader-0.0.2/aiida_bader.egg-info/top_level.txt
--rw-rw-r--   0 xing      (1000) xing      (1000)       38 2024-03-25 15:26:42.438766 aiida-bader-0.0.2/setup.cfg
--rw-rw-r--   0 xing      (1000) xing      (1000)     1473 2024-03-25 15:26:35.000000 aiida-bader-0.0.2/setup.py
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2024-03-25 15:26:42.438766 aiida-bader-0.0.2/tests/
--rw-rw-r--   0 xing      (1000) xing      (1000)      122 2024-03-25 15:26:07.000000 aiida-bader-0.0.2/tests/test_bader.py
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2024-04-24 13:00:54.091826 aiida_bader-0.0.3/
+-rw-rw-r--   0 xing      (1000) xing      (1000)     1066 2024-03-25 15:26:07.000000 aiida_bader-0.0.3/LICENSE
+-rw-r--r--   0 xing      (1000) xing      (1000)     2136 2024-04-24 13:00:54.091826 aiida_bader-0.0.3/PKG-INFO
+-rw-rw-r--   0 xing      (1000) xing      (1000)     1606 2024-03-25 15:26:07.000000 aiida_bader-0.0.3/README.md
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2024-04-24 13:00:54.091826 aiida_bader-0.0.3/aiida_bader/
+-rw-rw-r--   0 xing      (1000) xing      (1000)        0 2024-03-25 15:26:07.000000 aiida_bader-0.0.3/aiida_bader/__init__.py
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2024-04-24 13:00:54.091826 aiida_bader-0.0.3/aiida_bader/calculations/
+-rw-rw-r--   0 xing      (1000) xing      (1000)     3680 2024-03-25 15:26:07.000000 aiida_bader-0.0.3/aiida_bader/calculations/__init__.py
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2024-04-24 13:00:54.091826 aiida_bader-0.0.3/aiida_bader/parsers/
+-rw-rw-r--   0 xing      (1000) xing      (1000)     2005 2024-03-25 15:26:07.000000 aiida_bader-0.0.3/aiida_bader/parsers/__init__.py
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2024-04-24 13:00:54.091826 aiida_bader-0.0.3/aiida_bader/qeapp/
+-rw-rw-r--   0 xing      (1000) xing      (1000)      657 2024-03-25 15:26:07.000000 aiida_bader-0.0.3/aiida_bader/qeapp/__init__.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     3858 2024-04-10 19:56:14.000000 aiida_bader-0.0.3/aiida_bader/qeapp/result.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     2857 2024-04-10 19:56:14.000000 aiida_bader-0.0.3/aiida_bader/qeapp/widget.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     2758 2024-04-10 19:56:14.000000 aiida_bader-0.0.3/aiida_bader/qeapp/workchain.py
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2024-04-24 13:00:54.091826 aiida_bader-0.0.3/aiida_bader/workchains/
+-rw-rw-r--   0 xing      (1000) xing      (1000)       93 2024-03-25 15:26:07.000000 aiida_bader-0.0.3/aiida_bader/workchains/__init__.py
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2024-04-24 13:00:54.091826 aiida_bader-0.0.3/aiida_bader/workchains/protocols/
+-rw-rw-r--   0 xing      (1000) xing      (1000)        0 2024-03-25 15:26:07.000000 aiida_bader-0.0.3/aiida_bader/workchains/protocols/__init__.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     8003 2024-03-25 15:26:07.000000 aiida_bader-0.0.3/aiida_bader/workchains/qe_bader.py
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2024-04-24 13:00:54.091826 aiida_bader-0.0.3/aiida_bader/worktrees/
+-rw-rw-r--   0 xing      (1000) xing      (1000)        0 2024-03-25 15:26:07.000000 aiida_bader-0.0.3/aiida_bader/worktrees/__init__.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)      635 2024-03-25 15:26:07.000000 aiida_bader-0.0.3/aiida_bader/worktrees/cp2k_bader.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)      903 2024-04-10 19:55:50.000000 aiida_bader-0.0.3/aiida_bader/worktrees/qe_bader.py
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2024-04-24 13:00:54.091826 aiida_bader-0.0.3/aiida_bader.egg-info/
+-rw-r--r--   0 xing      (1000) xing      (1000)     2136 2024-04-24 13:00:54.000000 aiida_bader-0.0.3/aiida_bader.egg-info/PKG-INFO
+-rw-rw-r--   0 xing      (1000) xing      (1000)      687 2024-04-24 13:00:54.000000 aiida_bader-0.0.3/aiida_bader.egg-info/SOURCES.txt
+-rw-rw-r--   0 xing      (1000) xing      (1000)        1 2024-04-24 13:00:54.000000 aiida_bader-0.0.3/aiida_bader.egg-info/dependency_links.txt
+-rw-rw-r--   0 xing      (1000) xing      (1000)      256 2024-04-24 13:00:54.000000 aiida_bader-0.0.3/aiida_bader.egg-info/entry_points.txt
+-rw-rw-r--   0 xing      (1000) xing      (1000)      100 2024-04-24 13:00:54.000000 aiida_bader-0.0.3/aiida_bader.egg-info/requires.txt
+-rw-rw-r--   0 xing      (1000) xing      (1000)       12 2024-04-24 13:00:54.000000 aiida_bader-0.0.3/aiida_bader.egg-info/top_level.txt
+-rw-rw-r--   0 xing      (1000) xing      (1000)       38 2024-04-24 13:00:54.091826 aiida_bader-0.0.3/setup.cfg
+-rw-rw-r--   0 xing      (1000) xing      (1000)     1491 2024-04-24 13:00:45.000000 aiida_bader-0.0.3/setup.py
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2024-04-24 13:00:54.091826 aiida_bader-0.0.3/tests/
+-rw-rw-r--   0 xing      (1000) xing      (1000)      122 2024-03-25 15:26:07.000000 aiida_bader-0.0.3/tests/test_bader.py
```

### Comparing `aiida-bader-0.0.2/LICENSE` & `aiida_bader-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `aiida-bader-0.0.2/PKG-INFO` & `aiida_bader-0.0.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: aiida-bader
-Version: 0.0.2
+Version: 0.0.3
 Summary: AiiDA plugin for bader code.
 Home-page: https://github.com/superstart54/aiida-bader
 Author: Xing Wang
 Author-email: xingwang1991@gmail.com
 License: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: aiida-core
 Requires-Dist: aiida-worktree
-Requires-Dist: aiida-quantumespresso~=4.4
+Requires-Dist: aiida-quantumespresso
 Requires-Dist: aiida-cp2k
+Requires-Dist: weas-widget
 Requires-Dist: pytest
 Requires-Dist: pytest-cov
 Requires-Dist: pre-commit
 
 # AiiDA-Bader
 
 [![PyPI version](https://badge.fury.io/py/aiida-bader.svg)](https://badge.fury.io/py/aiida-bader)
```

### Comparing `aiida-bader-0.0.2/README.md` & `aiida_bader-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `aiida-bader-0.0.2/aiida_bader/calculations/__init__.py` & `aiida_bader-0.0.3/aiida_bader/calculations/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida-bader-0.0.2/aiida_bader/parsers/__init__.py` & `aiida_bader-0.0.3/aiida_bader/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida-bader-0.0.2/aiida_bader/qeapp/__init__.py` & `aiida_bader-0.0.3/aiida_bader/qeapp/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida-bader-0.0.2/aiida_bader/qeapp/workchain.py` & `aiida_bader-0.0.3/aiida_bader/qeapp/workchain.py`

 * *Files 8% similar despite different names*

```diff
@@ -76,12 +76,18 @@
             **kwargs,
         )
     else:
         raise ValueError("The pp_code and bader_code are required.")
     return builder
 
 
+def update_inputs(inputs, ctx):
+    """Update the inputs using context."""
+    inputs.structure = ctx.current_structure
+
+
 workchain_and_builder = {
     "workchain": QeBaderWorkChain,
     "exclude": ("clean_workdir", "structure", "relax"),
     "get_builder": get_builder,
+    "update_inputs": update_inputs,
 }
```

### Comparing `aiida-bader-0.0.2/aiida_bader/workchains/qe_bader.py` & `aiida_bader-0.0.3/aiida_bader/workchains/qe_bader.py`

 * *Files identical despite different names*

### Comparing `aiida-bader-0.0.2/aiida_bader/worktrees/cp2k_bader.py` & `aiida_bader-0.0.3/aiida_bader/worktrees/cp2k_bader.py`

 * *Files identical despite different names*

### Comparing `aiida-bader-0.0.2/aiida_bader/worktrees/qe_bader.py` & `aiida_bader-0.0.3/aiida_bader/worktrees/qe_bader.py`

 * *Files identical despite different names*

### Comparing `aiida-bader-0.0.2/aiida_bader.egg-info/PKG-INFO` & `aiida_bader-0.0.3/aiida_bader.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: aiida-bader
-Version: 0.0.2
+Version: 0.0.3
 Summary: AiiDA plugin for bader code.
 Home-page: https://github.com/superstart54/aiida-bader
 Author: Xing Wang
 Author-email: xingwang1991@gmail.com
 License: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: aiida-core
 Requires-Dist: aiida-worktree
-Requires-Dist: aiida-quantumespresso~=4.4
+Requires-Dist: aiida-quantumespresso
 Requires-Dist: aiida-cp2k
+Requires-Dist: weas-widget
 Requires-Dist: pytest
 Requires-Dist: pytest-cov
 Requires-Dist: pre-commit
 
 # AiiDA-Bader
 
 [![PyPI version](https://badge.fury.io/py/aiida-bader.svg)](https://badge.fury.io/py/aiida-bader)
```

### Comparing `aiida-bader-0.0.2/aiida_bader.egg-info/SOURCES.txt` & `aiida_bader-0.0.3/aiida_bader.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 aiida_bader.egg-info/entry_points.txt
 aiida_bader.egg-info/requires.txt
 aiida_bader.egg-info/top_level.txt
 aiida_bader/calculations/__init__.py
 aiida_bader/parsers/__init__.py
 aiida_bader/qeapp/__init__.py
 aiida_bader/qeapp/result.py
+aiida_bader/qeapp/widget.py
 aiida_bader/qeapp/workchain.py
 aiida_bader/workchains/__init__.py
 aiida_bader/workchains/qe_bader.py
 aiida_bader/workchains/protocols/__init__.py
 aiida_bader/worktrees/__init__.py
 aiida_bader/worktrees/cp2k_bader.py
 aiida_bader/worktrees/qe_bader.py
```

### Comparing `aiida-bader-0.0.2/setup.py` & `aiida_bader-0.0.3/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,29 +14,30 @@
 HERE = pathlib.Path(__file__).parent
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 setup(
     name="aiida-bader",
-    version="0.0.2",
+    version="0.0.3",
     description="AiiDA plugin for bader code.",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/superstart54/aiida-bader",
     author="Xing Wang",
     author_email="xingwang1991@gmail.com",
     license="MIT License",
     classifiers=[],
     packages=find_packages(),
     install_requires=[
         "aiida-core",
         "aiida-worktree",
-        "aiida-quantumespresso~=4.4",
+        "aiida-quantumespresso",
         "aiida-cp2k",
+        "weas-widget",
         "pytest",
         "pytest-cov",
         "pre-commit",
     ],
     entry_points={
         "aiida.calculations": [
             "bader = aiida_bader.calculations:BaderCalculation",
```


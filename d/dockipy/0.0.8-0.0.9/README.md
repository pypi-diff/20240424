# Comparing `tmp/dockipy-0.0.8.tar.gz` & `tmp/dockipy-0.0.9.tar.gz`

## Comparing `dockipy-0.0.8.tar` & `dockipy-0.0.9.tar`

### file list

```diff
@@ -1,15 +1,17 @@
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 dockipy-0.0.8/requirements.txt
--rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 dockipy-0.0.8/.github/workflows/publish.yml
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 dockipy-0.0.8/src/dockipy/__about__.py
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 dockipy-0.0.8/src/dockipy/__init__.py
--rw-r--r--   0        0        0     1217 2020-02-02 00:00:00.000000 dockipy-0.0.8/src/dockipy/dockinotebook.py
--rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 dockipy-0.0.8/src/dockipy/dockipy.py
--rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 dockipy-0.0.8/src/dockipy/dockishell.py
--rw-r--r--   0        0        0    10866 2020-02-02 00:00:00.000000 dockipy-0.0.8/src/dockipy/utils.py
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 dockipy-0.0.8/tests/__init__.py
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 dockipy-0.0.8/tests/init_test.py
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 dockipy-0.0.8/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 dockipy-0.0.8/LICENSE
--rw-r--r--   0        0        0     3720 2020-02-02 00:00:00.000000 dockipy-0.0.8/README.md
--rw-r--r--   0        0        0     2181 2020-02-02 00:00:00.000000 dockipy-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     4672 2020-02-02 00:00:00.000000 dockipy-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 dockipy-0.0.9/requirements.txt
+-rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 dockipy-0.0.9/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 dockipy-0.0.9/src/dockipy/__about__.py
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 dockipy-0.0.9/src/dockipy/__init__.py
+-rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 dockipy-0.0.9/src/dockipy/dockibook.py
+-rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 dockipy-0.0.9/src/dockipy/dockipy.py
+-rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 dockipy-0.0.9/src/dockipy/dockishell.py
+-rw-r--r--   0        0        0     2570 2020-02-02 00:00:00.000000 dockipy-0.0.9/src/dockipy/envibook.py
+-rw-r--r--   0        0        0     2034 2020-02-02 00:00:00.000000 dockipy-0.0.9/src/dockipy/envipy.py
+-rw-r--r--   0        0        0    10866 2020-02-02 00:00:00.000000 dockipy-0.0.9/src/dockipy/utils.py
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 dockipy-0.0.9/tests/__init__.py
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 dockipy-0.0.9/tests/init_test.py
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 dockipy-0.0.9/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 dockipy-0.0.9/LICENSE
+-rw-r--r--   0        0        0     4131 2020-02-02 00:00:00.000000 dockipy-0.0.9/README.md
+-rw-r--r--   0        0        0     2241 2020-02-02 00:00:00.000000 dockipy-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     5083 2020-02-02 00:00:00.000000 dockipy-0.0.9/PKG-INFO
```

### Comparing `dockipy-0.0.8/.github/workflows/publish.yml` & `dockipy-0.0.9/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `dockipy-0.0.8/src/dockipy/dockinotebook.py` & `dockipy-0.0.9/src/dockipy/dockibook.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
 import dockipy.utils as utils
 import sys
 
-def dockinotebook():
+def dockibook():
     work_dir, project_root, target_root = utils.find_project_root()
 
     command = sys.argv[1:]
 
     docki_config = utils.get_docki_config(project_root)
     
     token = docki_config.get("notebook_token", "docki")
```

### Comparing `dockipy-0.0.8/src/dockipy/dockipy.py` & `dockipy-0.0.9/src/dockipy/dockipy.py`

 * *Files identical despite different names*

### Comparing `dockipy-0.0.8/src/dockipy/dockishell.py` & `dockipy-0.0.9/src/dockipy/dockishell.py`

 * *Files identical despite different names*

### Comparing `dockipy-0.0.8/src/dockipy/utils.py` & `dockipy-0.0.9/src/dockipy/utils.py`

 * *Files identical despite different names*

### Comparing `dockipy-0.0.8/LICENSE` & `dockipy-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dockipy-0.0.8/README.md` & `dockipy-0.0.9/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -38,27 +38,39 @@
 
 Need to run an arbitrary command in a container? No problem! Just fire up dockishell and let the container magic begin.
 
 ```bash
 dockishell nvidia-smi
 ```
 
-#### How to Use dockinotebook
-Want to unleash the power of Jupyter Notebooks in a container? Say no more! Use dockinotebook and open the link in your browser, colab or visual studio code.
+#### How to Use dockibook
+Want to unleash the power of Jupyter Notebooks in a container? Say no more! Use dockibook and open the link in your browser, colab or visual studio code.
 
 ```bash
-dockinotebook
+dockibook
 ```
 
+#### Don't want to use Docker but still would like to use the configuration? No problem! Use envipy and envibook to run your code and notebooks in a virtual environment.
+Since Windows is such a messy work with rawdogging your environment is totally okay.
+```bash
+envipy my_script.py
+```
+    
+```bash
+envibook
+```
+
+
 ## Configure environment
 Tired of Docker feeling like a high-maintenance diva? Set up your environment like a pro with docki.yaml. No more Docker dramas, just smooth sailing.
 
 ```bash
 docki --init
 ```
+
 ### docki.yaml
 
 This file is used to specify the base image, system dependencies, and python dependencies for the Docker container.
 If the file does not exist, a template will be created in the project root using docki --init.
 
 base_image: The base image for the Docker container. You can find images on [Docker Hub](https://hub.docker.com/).
 
@@ -96,11 +108,12 @@
     file: ./requirements.txt
 notebook_token: docki
 notebook_password: docki
 ```
 ## TODO
 - [ ] Add support Windows Notebooks
 - [ ] Add support for Docker GPU driver installation on WLS2
+- [ ] Add support for Mac. I don't have a Mac! Pls send donations to my onlyfans so that i can afford one!
 
 ## License
 
 `dockipy` is like that cool friend who always lets you borrow their stuff without any fuss. It's distributed under the terms of the [apache-2.0](https://choosealicense.com/licenses/apache-2.0/) license. So go ahead, have some fun with it! 🎉
```

### Comparing `dockipy-0.0.8/pyproject.toml` & `dockipy-0.0.9/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -74,16 +74,18 @@
 [tool.coverage.paths]
 dockipy = ["src/dockipy", "*/dockipy/src/dockipy"]
 tests = ["tests", "*/dockipy/tests"]
 
 [project.scripts]
 dockipy = "dockipy.dockipy:dockipy"
 dockishell = "dockipy.dockishell:dockishell"
-dockinotebook = "dockipy.dockinotebook:dockinotebook"
+dockibook = "dockipy.dockibook:dockibook"
 docki = "dockipy.utils:docki"
+envipy = "dockipy.envipy:envipy"
+envibook = "dockipy.envibook:envibook"
 
 [tool.coverage.report]
 exclude_lines = [
   "no cov",
   "if __name__ == .__main__.:",
   "if TYPE_CHECKING:",
 ]
```

### Comparing `dockipy-0.0.8/PKG-INFO` & `dockipy-0.0.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: dockipy
-Version: 0.0.8
+Version: 0.0.9
 Project-URL: Documentation, https://github.com/Arty-Facts/dockipy#readme
 Project-URL: Issues, https://github.com/Arty-Facts/dockipy/issues
 Project-URL: Source, https://github.com/Arty-Facts/dockipy
 Author-email: Arturas Aleksandraus <arturas@aleksandraus.se>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha
@@ -61,27 +61,39 @@
 
 Need to run an arbitrary command in a container? No problem! Just fire up dockishell and let the container magic begin.
 
 ```bash
 dockishell nvidia-smi
 ```
 
-#### How to Use dockinotebook
-Want to unleash the power of Jupyter Notebooks in a container? Say no more! Use dockinotebook and open the link in your browser, colab or visual studio code.
+#### How to Use dockibook
+Want to unleash the power of Jupyter Notebooks in a container? Say no more! Use dockibook and open the link in your browser, colab or visual studio code.
 
 ```bash
-dockinotebook
+dockibook
 ```
 
+#### Don't want to use Docker but still would like to use the configuration? No problem! Use envipy and envibook to run your code and notebooks in a virtual environment.
+Since Windows is such a messy work with rawdogging your environment is totally okay.
+```bash
+envipy my_script.py
+```
+    
+```bash
+envibook
+```
+
+
 ## Configure environment
 Tired of Docker feeling like a high-maintenance diva? Set up your environment like a pro with docki.yaml. No more Docker dramas, just smooth sailing.
 
 ```bash
 docki --init
 ```
+
 ### docki.yaml
 
 This file is used to specify the base image, system dependencies, and python dependencies for the Docker container.
 If the file does not exist, a template will be created in the project root using docki --init.
 
 base_image: The base image for the Docker container. You can find images on [Docker Hub](https://hub.docker.com/).
 
@@ -119,11 +131,12 @@
     file: ./requirements.txt
 notebook_token: docki
 notebook_password: docki
 ```
 ## TODO
 - [ ] Add support Windows Notebooks
 - [ ] Add support for Docker GPU driver installation on WLS2
+- [ ] Add support for Mac. I don't have a Mac! Pls send donations to my onlyfans so that i can afford one!
 
 ## License
 
 `dockipy` is like that cool friend who always lets you borrow their stuff without any fuss. It's distributed under the terms of the [apache-2.0](https://choosealicense.com/licenses/apache-2.0/) license. So go ahead, have some fun with it! 🎉
```


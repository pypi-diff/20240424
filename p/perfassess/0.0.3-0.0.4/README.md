# Comparing `tmp/perfassess-0.0.3.tar.gz` & `tmp/perfassess-0.0.4.tar.gz`

## Comparing `perfassess-0.0.3.tar` & `perfassess-0.0.4.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 perfassess-0.0.3/.gitattributes
--rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 perfassess-0.0.3/mkdocs.yml
--rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 perfassess-0.0.3/.github/workflows/build_doc.yml
--rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 perfassess-0.0.3/.github/workflows/publish_pypi_package.yml
--rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 perfassess-0.0.3/.github/workflows/python_package.yml
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 perfassess-0.0.3/data/argument.yml
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 perfassess-0.0.3/data/existing_file.txt
--rw-r--r--   0        0        0  3627651 2020-02-02 00:00:00.000000 perfassess-0.0.3/data/memory_evaluation.html
--rw-r--r--   0        0        0  3865508 2020-02-02 00:00:00.000000 perfassess-0.0.3/data/time_evaluation.html
--rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 perfassess-0.0.3/docs/index.md
--rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 perfassess-0.0.3/docs/installation.md
--rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 perfassess-0.0.3/docs/style.css
--rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 perfassess-0.0.3/docs/code_documentation/class_performance_assessor.md
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 perfassess-0.0.3/docs/code_documentation/main.md
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 perfassess-0.0.3/docs/code_documentation/testor.md
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 perfassess-0.0.3/docs/code_documentation/parse_argument/check_argument.md
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 perfassess-0.0.3/docs/code_documentation/parse_argument/define_argument.md
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 perfassess-0.0.3/docs/code_documentation/parse_argument/parse_argument.md
--rw-r--r--   0        0        0  3627648 2020-02-02 00:00:00.000000 perfassess-0.0.3/docs/plot/memory_evaluation.html
--rw-r--r--   0        0        0  3865497 2020-02-02 00:00:00.000000 perfassess-0.0.3/docs/plot/time_evaluation.html
--rw-r--r--   0        0        0     7055 2020-02-02 00:00:00.000000 perfassess-0.0.3/docs/usage/command_line.md
--rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 perfassess-0.0.3/docs/usage/module.md
--rw-r--r--   0        0        0     2080 2020-02-02 00:00:00.000000 perfassess-0.0.3/env/README.md
--rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 perfassess-0.0.3/env/perfassess.yml
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 perfassess-0.0.3/env/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 perfassess-0.0.3/src/perfassess/__init__.py
--rw-r--r--   0        0        0    13951 2020-02-02 00:00:00.000000 perfassess-0.0.3/src/perfassess/class_performance_assessor.py
--rw-r--r--   0        0        0     1397 2020-02-02 00:00:00.000000 perfassess-0.0.3/src/perfassess/main.py
--rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 perfassess-0.0.3/src/perfassess/testor.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 perfassess-0.0.3/src/perfassess/parse_argument/__init__.py
--rw-r--r--   0        0        0     9204 2020-02-02 00:00:00.000000 perfassess-0.0.3/src/perfassess/parse_argument/check_argument.py
--rw-r--r--   0        0        0     6848 2020-02-02 00:00:00.000000 perfassess-0.0.3/src/perfassess/parse_argument/define_argument.py
--rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 perfassess-0.0.3/src/perfassess/parse_argument/parse_argument.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 perfassess-0.0.3/tests/__init__.py
--rw-r--r--   0        0        0     5503 2020-02-02 00:00:00.000000 perfassess-0.0.3/tests/test_check_argument.py
--rw-r--r--   0        0        0     2062 2020-02-02 00:00:00.000000 perfassess-0.0.3/tests/test_main.py
--rw-r--r--   0        0        0     3073 2020-02-02 00:00:00.000000 perfassess-0.0.3/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 perfassess-0.0.3/LICENSE
--rw-r--r--   0        0        0     6684 2020-02-02 00:00:00.000000 perfassess-0.0.3/README.md
--rw-r--r--   0        0        0     1381 2020-02-02 00:00:00.000000 perfassess-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     7486 2020-02-02 00:00:00.000000 perfassess-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 perfassess-0.0.4/.gitattributes
+-rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 perfassess-0.0.4/mkdocs.yml
+-rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 perfassess-0.0.4/.github/workflows/build_doc.yml
+-rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 perfassess-0.0.4/.github/workflows/publish_pypi_package.yml
+-rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 perfassess-0.0.4/.github/workflows/python_package.yml
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 perfassess-0.0.4/data/argument.yml
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 perfassess-0.0.4/data/existing_file.txt
+-rw-r--r--   0        0        0  3627651 2020-02-02 00:00:00.000000 perfassess-0.0.4/data/memory_evaluation.html
+-rw-r--r--   0        0        0  3865508 2020-02-02 00:00:00.000000 perfassess-0.0.4/data/time_evaluation.html
+-rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 perfassess-0.0.4/docs/index.md
+-rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 perfassess-0.0.4/docs/installation.md
+-rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 perfassess-0.0.4/docs/style.css
+-rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 perfassess-0.0.4/docs/code_documentation/class_performance_assessor.md
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 perfassess-0.0.4/docs/code_documentation/main.md
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 perfassess-0.0.4/docs/code_documentation/testor.md
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 perfassess-0.0.4/docs/code_documentation/parse_argument/check_argument.md
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 perfassess-0.0.4/docs/code_documentation/parse_argument/define_argument.md
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 perfassess-0.0.4/docs/code_documentation/parse_argument/parse_argument.md
+-rw-r--r--   0        0        0  3627648 2020-02-02 00:00:00.000000 perfassess-0.0.4/docs/plot/memory_evaluation.html
+-rw-r--r--   0        0        0  3865497 2020-02-02 00:00:00.000000 perfassess-0.0.4/docs/plot/time_evaluation.html
+-rw-r--r--   0        0        0     7055 2020-02-02 00:00:00.000000 perfassess-0.0.4/docs/usage/command_line.md
+-rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 perfassess-0.0.4/docs/usage/module.md
+-rw-r--r--   0        0        0     2080 2020-02-02 00:00:00.000000 perfassess-0.0.4/env/README.md
+-rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 perfassess-0.0.4/env/perfassess.yml
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 perfassess-0.0.4/env/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 perfassess-0.0.4/src/perfassess/__init__.py
+-rw-r--r--   0        0        0    13951 2020-02-02 00:00:00.000000 perfassess-0.0.4/src/perfassess/class_performance_assessor.py
+-rw-r--r--   0        0        0     1397 2020-02-02 00:00:00.000000 perfassess-0.0.4/src/perfassess/main.py
+-rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 perfassess-0.0.4/src/perfassess/testor.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 perfassess-0.0.4/src/perfassess/parse_argument/__init__.py
+-rw-r--r--   0        0        0     9204 2020-02-02 00:00:00.000000 perfassess-0.0.4/src/perfassess/parse_argument/check_argument.py
+-rw-r--r--   0        0        0     6848 2020-02-02 00:00:00.000000 perfassess-0.0.4/src/perfassess/parse_argument/define_argument.py
+-rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 perfassess-0.0.4/src/perfassess/parse_argument/parse_argument.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 perfassess-0.0.4/tests/__init__.py
+-rw-r--r--   0        0        0     5503 2020-02-02 00:00:00.000000 perfassess-0.0.4/tests/test_check_argument.py
+-rw-r--r--   0        0        0     2062 2020-02-02 00:00:00.000000 perfassess-0.0.4/tests/test_main.py
+-rw-r--r--   0        0        0     3073 2020-02-02 00:00:00.000000 perfassess-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 perfassess-0.0.4/LICENSE
+-rw-r--r--   0        0        0     7030 2020-02-02 00:00:00.000000 perfassess-0.0.4/README.md
+-rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 perfassess-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     8428 2020-02-02 00:00:00.000000 perfassess-0.0.4/PKG-INFO
```

### Comparing `perfassess-0.0.3/mkdocs.yml` & `perfassess-0.0.4/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `perfassess-0.0.3/.github/workflows/build_doc.yml` & `perfassess-0.0.4/.github/workflows/build_doc.yml`

 * *Files identical despite different names*

### Comparing `perfassess-0.0.3/.github/workflows/publish_pypi_package.yml` & `perfassess-0.0.4/.github/workflows/publish_pypi_package.yml`

 * *Files identical despite different names*

### Comparing `perfassess-0.0.3/.github/workflows/python_package.yml` & `perfassess-0.0.4/.github/workflows/python_package.yml`

 * *Files identical despite different names*

### Comparing `perfassess-0.0.3/data/memory_evaluation.html` & `perfassess-0.0.4/data/memory_evaluation.html`

 * *Files identical despite different names*

### Comparing `perfassess-0.0.3/data/time_evaluation.html` & `perfassess-0.0.4/data/time_evaluation.html`

 * *Files identical despite different names*

### Comparing `perfassess-0.0.3/docs/index.md` & `perfassess-0.0.4/docs/index.md`

 * *Files identical despite different names*

### Comparing `perfassess-0.0.3/docs/style.css` & `perfassess-0.0.4/docs/style.css`

 * *Files identical despite different names*

### Comparing `perfassess-0.0.3/docs/code_documentation/class_performance_assessor.md` & `perfassess-0.0.4/docs/code_documentation/class_performance_assessor.md`

 * *Files identical despite different names*

### Comparing `perfassess-0.0.3/docs/plot/memory_evaluation.html` & `perfassess-0.0.4/docs/plot/memory_evaluation.html`

 * *Files identical despite different names*

### Comparing `perfassess-0.0.3/docs/plot/time_evaluation.html` & `perfassess-0.0.4/docs/plot/time_evaluation.html`

 * *Files identical despite different names*

### Comparing `perfassess-0.0.3/docs/usage/command_line.md` & `perfassess-0.0.4/docs/usage/command_line.md`

 * *Files identical despite different names*

### Comparing `perfassess-0.0.3/docs/usage/module.md` & `perfassess-0.0.4/docs/usage/module.md`

 * *Files identical despite different names*

### Comparing `perfassess-0.0.3/env/README.md` & `perfassess-0.0.4/env/README.md`

 * *Files identical despite different names*

### Comparing `perfassess-0.0.3/env/perfassess.yml` & `perfassess-0.0.4/env/perfassess.yml`

 * *Files identical despite different names*

### Comparing `perfassess-0.0.3/src/perfassess/class_performance_assessor.py` & `perfassess-0.0.4/src/perfassess/class_performance_assessor.py`

 * *Files identical despite different names*

### Comparing `perfassess-0.0.3/src/perfassess/main.py` & `perfassess-0.0.4/src/perfassess/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 ```
 
 With "output_directory/" being the output directory of your choice
 """
 
 __authors__ = ["Lucas ROUAUD"]
 __contact__ = ["lucas.rouaud@gmail.com"]
-__version__ = "0.0.3"
+__version__ = "0.0.4"
 __date__ = "22/03/2024"
 __copyright__ = "MIT License"
 
 
 # [C]
 from .class_performance_assessor import PerformanceAssessor
 # [P]
```

### Comparing `perfassess-0.0.3/src/perfassess/parse_argument/check_argument.py` & `perfassess-0.0.4/src/perfassess/parse_argument/check_argument.py`

 * *Files identical despite different names*

### Comparing `perfassess-0.0.3/src/perfassess/parse_argument/define_argument.py` & `perfassess-0.0.4/src/perfassess/parse_argument/define_argument.py`

 * *Files identical despite different names*

### Comparing `perfassess-0.0.3/src/perfassess/parse_argument/parse_argument.py` & `perfassess-0.0.4/src/perfassess/parse_argument/parse_argument.py`

 * *Files identical despite different names*

### Comparing `perfassess-0.0.3/tests/test_check_argument.py` & `perfassess-0.0.4/tests/test_check_argument.py`

 * *Files identical despite different names*

### Comparing `perfassess-0.0.3/tests/test_main.py` & `perfassess-0.0.4/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `perfassess-0.0.3/.gitignore` & `perfassess-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `perfassess-0.0.3/LICENSE` & `perfassess-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `perfassess-0.0.3/README.md` & `perfassess-0.0.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,36 +1,43 @@
 <div align="center">
 
 # ⌛️ PERFASSESS 💾
 
-[![Python 3.10.8](https://img.shields.io/badge/python-%E2%89%A5_3.11.5-blue.svg)](https://www.python.org/downloads/release/python-397/)
-[![Conda 22.11.1](https://img.shields.io/badge/miniconda-%E2%89%A5_23.11.0-green.svg)](https://docs.conda.io/en/latest/miniconda.html)
+[![Python 3.11](https://img.shields.io/badge/python-%E2%89%A5_3.11-blue.svg)](https://www.python.org/downloads/release/python-3110/)
+[![pip 24.0](https://img.shields.io/badge/pip-%E2%89%A5_24.0-green.svg)](https://pip.pypa.io/en/latest/installation/)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
-
 ✍ Contributor: **Lucas ROUAUD**
 
 </div align="center">
 
 ## 📒 Description
 
-**This module permit to evaluate the performance of a given function and create Plotly bar plot.**
+**This module permit to evaluate the performance of a given function and create Plotly bar plot. Check the documentation at [https://filouplains.github.io/perfassess/](https://filouplains.github.io/perfassess/).**
 
 ## 🗄 Dependencies
 
-To run this software, you will need `python ≥ 3.10` and this next module:
+To run this software, you will need `python ≥ 3.11` and this next module:
 
 - `numpy ≥ 1.26.0`
 - `plotly ≥ 5.19.0`
 - `pyyaml ≥ 6.0.1`
 
 ## ⚙️ Installation
 
 ### 🥹 EZ way
 
+Recommended method:
+
+```bash
+$ pipx install perfassess
+```
+
+If you do not have pipx installed, check out the documentation at [https://pipx.pypa.io/stable/installation/](https://pipx.pypa.io/stable/installation/). Else, classical installation method:
+
 ```bash
 $ pip install perfassess
 ```
 
 ### 😩 From source
 #### 👬 Cloning the repository
```

### Comparing `perfassess-0.0.3/pyproject.toml` & `perfassess-0.0.4/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,14 +1,20 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "perfassess"
-version = "0.0.3"
+version = "0.0.4"
+requires-python = ">= 3.10"
+dependencies = [
+    "numpy",
+    "plotly",
+    "pyyaml"
+]
 description = "Access the performance of a given function and create plot."
 authors = [{ name = "Lucas ROUAUD", email = "lucas.rouaud@gmail.com" }]
 maintainers = [{ name = "Lucas ROUAUD", email = "lucas.rouaud@gmail.com" }]
 license = { text = "MIT License" }
 readme = "README.md"
 keywords = ["python", "performance", "assessor", "time", "memory", "plot"]
 classifiers = [
@@ -20,29 +26,27 @@
 ]
 
 [project.urls]
 Homepage = "https://github.com/FilouPlains/perfassess"
 Documentation = "https://filouplains.github.io/perfassess/"
 Repository = "https://github.com/FilouPlains/perfassess"
 
-[tool.poetry.dependencies]
-python = "^3.10"
-plotly = "^5.19.0"
-
-[tool.poetry.dev-dependencies]
-ipython = "^8.22.2"
-markdown = "^3.5.2"
-mkdocs = "^1.5.3"
-mkdocs-autorefs = "^1.0.1"
-mkdocs-callouts = "^1.13.2"
-mkdocs-material = "^9.5.14"
-mkdocs-material-extensions = "^1.3.1"
-mkdocstrings = "^0.24.1"
-mkdocstrings-python = "^1.9.0"
-pylint = "^2.16.2"
-pytest = "^7.0"
+[project.optional-dependencies]
+dev = [
+    "ipython",
+    "markdown",
+    "mkdocs",
+    "mkdocs-autorefs",
+    "mkdocs-callouts",
+    "mkdocs-material",
+    "mkdocs-material-extensions",
+    "mkdocstrings",
+    "mkdocstrings-python",
+    "pylint",
+    "pytest",
+]
 
 [project.entry-points."src.main"]
 perfassess = "perfassess.main:main"
 
 [project.scripts]
 perfassess = "perfassess.main:main"
```

### Comparing `perfassess-0.0.3/PKG-INFO` & `perfassess-0.0.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,55 +1,78 @@
 Metadata-Version: 2.3
 Name: perfassess
-Version: 0.0.3
+Version: 0.0.4
 Summary: Access the performance of a given function and create plot.
 Project-URL: Homepage, https://github.com/FilouPlains/perfassess
 Project-URL: Documentation, https://filouplains.github.io/perfassess/
 Project-URL: Repository, https://github.com/FilouPlains/perfassess
 Author-email: Lucas ROUAUD <lucas.rouaud@gmail.com>
 Maintainer-email: Lucas ROUAUD <lucas.rouaud@gmail.com>
 License: MIT License
 License-File: LICENSE
 Keywords: assessor,memory,performance,plot,python,time
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.10
+Requires-Python: >=3.10
+Requires-Dist: numpy
+Requires-Dist: plotly
+Requires-Dist: pyyaml
+Provides-Extra: dev
+Requires-Dist: ipython; extra == 'dev'
+Requires-Dist: markdown; extra == 'dev'
+Requires-Dist: mkdocs; extra == 'dev'
+Requires-Dist: mkdocs-autorefs; extra == 'dev'
+Requires-Dist: mkdocs-callouts; extra == 'dev'
+Requires-Dist: mkdocs-material; extra == 'dev'
+Requires-Dist: mkdocs-material-extensions; extra == 'dev'
+Requires-Dist: mkdocstrings; extra == 'dev'
+Requires-Dist: mkdocstrings-python; extra == 'dev'
+Requires-Dist: pylint; extra == 'dev'
+Requires-Dist: pytest; extra == 'dev'
 Description-Content-Type: text/markdown
 
 <div align="center">
 
 # ⌛️ PERFASSESS 💾
 
-[![Python 3.10.8](https://img.shields.io/badge/python-%E2%89%A5_3.11.5-blue.svg)](https://www.python.org/downloads/release/python-397/)
-[![Conda 22.11.1](https://img.shields.io/badge/miniconda-%E2%89%A5_23.11.0-green.svg)](https://docs.conda.io/en/latest/miniconda.html)
+[![Python 3.11](https://img.shields.io/badge/python-%E2%89%A5_3.11-blue.svg)](https://www.python.org/downloads/release/python-3110/)
+[![pip 24.0](https://img.shields.io/badge/pip-%E2%89%A5_24.0-green.svg)](https://pip.pypa.io/en/latest/installation/)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
-
 ✍ Contributor: **Lucas ROUAUD**
 
 </div align="center">
 
 ## 📒 Description
 
-**This module permit to evaluate the performance of a given function and create Plotly bar plot.**
+**This module permit to evaluate the performance of a given function and create Plotly bar plot. Check the documentation at [https://filouplains.github.io/perfassess/](https://filouplains.github.io/perfassess/).**
 
 ## 🗄 Dependencies
 
-To run this software, you will need `python ≥ 3.10` and this next module:
+To run this software, you will need `python ≥ 3.11` and this next module:
 
 - `numpy ≥ 1.26.0`
 - `plotly ≥ 5.19.0`
 - `pyyaml ≥ 6.0.1`
 
 ## ⚙️ Installation
 
 ### 🥹 EZ way
 
+Recommended method:
+
+```bash
+$ pipx install perfassess
+```
+
+If you do not have pipx installed, check out the documentation at [https://pipx.pypa.io/stable/installation/](https://pipx.pypa.io/stable/installation/). Else, classical installation method:
+
 ```bash
 $ pip install perfassess
 ```
 
 ### 😩 From source
 #### 👬 Cloning the repository
```


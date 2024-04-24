# Comparing `tmp/lambdapdk-0.1.8.tar.gz` & `tmp/lambdapdk-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lambdapdk-0.1.8.tar", last modified: Fri Feb 16 21:13:15 2024, max compression
+gzip compressed data, was "lambdapdk-0.1.9.tar", last modified: Tue Feb 20 16:47:15 2024, max compression
```

## Comparing `lambdapdk-0.1.8.tar` & `lambdapdk-0.1.9.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 21:13:15.974446 lambdapdk-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)    10766 2024-02-16 21:12:56.000000 lambdapdk-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-02-16 21:12:56.000000 lambdapdk-0.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    13744 2024-02-16 21:13:15.974446 lambdapdk-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      876 2024-02-16 21:12:56.000000 lambdapdk-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 21:13:15.970446 lambdapdk-0.1.8/lambdapdk/
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-02-16 21:12:56.000000 lambdapdk-0.1.8/lambdapdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 21:13:15.970446 lambdapdk-0.1.8/lambdapdk/asap7/
--rw-r--r--   0 runner    (1001) docker     (127)     4299 2024-02-16 21:12:56.000000 lambdapdk-0.1.8/lambdapdk/asap7/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 21:13:15.970446 lambdapdk-0.1.8/lambdapdk/asap7/libs/
--rw-r--r--   0 runner    (1001) docker     (127)     4991 2024-02-16 21:12:56.000000 lambdapdk-0.1.8/lambdapdk/asap7/libs/asap7sc7p5t.py
--rw-r--r--   0 runner    (1001) docker     (127)      864 2024-02-16 21:12:56.000000 lambdapdk-0.1.8/lambdapdk/asap7/libs/fakeram7.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 21:13:15.970446 lambdapdk-0.1.8/lambdapdk/freepdk45/
--rw-r--r--   0 runner    (1001) docker     (127)     3895 2024-02-16 21:12:56.000000 lambdapdk-0.1.8/lambdapdk/freepdk45/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 21:13:15.970446 lambdapdk-0.1.8/lambdapdk/freepdk45/libs/
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-02-16 21:12:56.000000 lambdapdk-0.1.8/lambdapdk/freepdk45/libs/fakeram45.py
--rw-r--r--   0 runner    (1001) docker     (127)     3680 2024-02-16 21:12:56.000000 lambdapdk-0.1.8/lambdapdk/freepdk45/libs/nangate45.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 21:13:15.970446 lambdapdk-0.1.8/lambdapdk/gf180/
--rw-r--r--   0 runner    (1001) docker     (127)     5434 2024-02-16 21:12:56.000000 lambdapdk-0.1.8/lambdapdk/gf180/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 21:13:15.970446 lambdapdk-0.1.8/lambdapdk/gf180/libs/
--rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-02-16 21:12:56.000000 lambdapdk-0.1.8/lambdapdk/gf180/libs/gf180io.py
--rw-r--r--   0 runner    (1001) docker     (127)     5638 2024-02-16 21:12:56.000000 lambdapdk-0.1.8/lambdapdk/gf180/libs/gf180mcu.py
--rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-02-16 21:12:56.000000 lambdapdk-0.1.8/lambdapdk/gf180/libs/gf180sram.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 21:13:15.970446 lambdapdk-0.1.8/lambdapdk/sky130/
--rw-r--r--   0 runner    (1001) docker     (127)     4215 2024-02-16 21:12:56.000000 lambdapdk-0.1.8/lambdapdk/sky130/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 21:13:15.970446 lambdapdk-0.1.8/lambdapdk/sky130/libs/
--rw-r--r--   0 runner    (1001) docker     (127)     6615 2024-02-16 21:12:56.000000 lambdapdk-0.1.8/lambdapdk/sky130/libs/sky130hd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-02-16 21:12:56.000000 lambdapdk-0.1.8/lambdapdk/sky130/libs/sky130io.py
--rw-r--r--   0 runner    (1001) docker     (127)      996 2024-02-16 21:12:57.000000 lambdapdk-0.1.8/lambdapdk/sky130/libs/sky130sram.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 21:13:15.974446 lambdapdk-0.1.8/lambdapdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13744 2024-02-16 21:13:15.000000 lambdapdk-0.1.8/lambdapdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      763 2024-02-16 21:13:15.000000 lambdapdk-0.1.8/lambdapdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-16 21:13:15.000000 lambdapdk-0.1.8/lambdapdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-02-16 21:13:15.000000 lambdapdk-0.1.8/lambdapdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-16 21:13:15.000000 lambdapdk-0.1.8/lambdapdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-02-16 21:12:57.000000 lambdapdk-0.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-16 21:13:15.974446 lambdapdk-0.1.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 21:13:15.974446 lambdapdk-0.1.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-02-16 21:12:57.000000 lambdapdk-0.1.8/tests/test_lambda.py
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-02-16 21:12:57.000000 lambdapdk-0.1.8/tests/test_local_detect.py
--rw-r--r--   0 runner    (1001) docker     (127)      821 2024-02-16 21:12:57.000000 lambdapdk-0.1.8/tests/test_paths.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 16:47:15.167188 lambdapdk-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    10766 2024-02-20 16:46:57.000000 lambdapdk-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-02-20 16:46:57.000000 lambdapdk-0.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    13744 2024-02-20 16:47:15.167188 lambdapdk-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      876 2024-02-20 16:46:57.000000 lambdapdk-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 16:47:15.163188 lambdapdk-0.1.9/lambdapdk/
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-02-20 16:46:57.000000 lambdapdk-0.1.9/lambdapdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 16:47:15.163188 lambdapdk-0.1.9/lambdapdk/asap7/
+-rw-r--r--   0 runner    (1001) docker     (127)     4299 2024-02-20 16:46:57.000000 lambdapdk-0.1.9/lambdapdk/asap7/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 16:47:15.163188 lambdapdk-0.1.9/lambdapdk/asap7/libs/
+-rw-r--r--   0 runner    (1001) docker     (127)     4991 2024-02-20 16:46:57.000000 lambdapdk-0.1.9/lambdapdk/asap7/libs/asap7sc7p5t.py
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-02-20 16:46:57.000000 lambdapdk-0.1.9/lambdapdk/asap7/libs/fakeram7.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 16:47:15.163188 lambdapdk-0.1.9/lambdapdk/freepdk45/
+-rw-r--r--   0 runner    (1001) docker     (127)     3895 2024-02-20 16:46:57.000000 lambdapdk-0.1.9/lambdapdk/freepdk45/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 16:47:15.167188 lambdapdk-0.1.9/lambdapdk/freepdk45/libs/
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-02-20 16:46:57.000000 lambdapdk-0.1.9/lambdapdk/freepdk45/libs/fakeram45.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3680 2024-02-20 16:46:57.000000 lambdapdk-0.1.9/lambdapdk/freepdk45/libs/nangate45.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 16:47:15.167188 lambdapdk-0.1.9/lambdapdk/gf180/
+-rw-r--r--   0 runner    (1001) docker     (127)     5434 2024-02-20 16:46:57.000000 lambdapdk-0.1.9/lambdapdk/gf180/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 16:47:15.167188 lambdapdk-0.1.9/lambdapdk/gf180/libs/
+-rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-02-20 16:46:57.000000 lambdapdk-0.1.9/lambdapdk/gf180/libs/gf180io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5638 2024-02-20 16:46:57.000000 lambdapdk-0.1.9/lambdapdk/gf180/libs/gf180mcu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-02-20 16:46:57.000000 lambdapdk-0.1.9/lambdapdk/gf180/libs/gf180sram.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 16:47:15.167188 lambdapdk-0.1.9/lambdapdk/sky130/
+-rw-r--r--   0 runner    (1001) docker     (127)     4215 2024-02-20 16:46:57.000000 lambdapdk-0.1.9/lambdapdk/sky130/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 16:47:15.167188 lambdapdk-0.1.9/lambdapdk/sky130/libs/
+-rw-r--r--   0 runner    (1001) docker     (127)     6615 2024-02-20 16:46:57.000000 lambdapdk-0.1.9/lambdapdk/sky130/libs/sky130hd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-02-20 16:46:57.000000 lambdapdk-0.1.9/lambdapdk/sky130/libs/sky130io.py
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-02-20 16:46:58.000000 lambdapdk-0.1.9/lambdapdk/sky130/libs/sky130sram.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 16:47:15.167188 lambdapdk-0.1.9/lambdapdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13744 2024-02-20 16:47:15.000000 lambdapdk-0.1.9/lambdapdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-02-20 16:47:15.000000 lambdapdk-0.1.9/lambdapdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-20 16:47:15.000000 lambdapdk-0.1.9/lambdapdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-02-20 16:47:15.000000 lambdapdk-0.1.9/lambdapdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-20 16:47:15.000000 lambdapdk-0.1.9/lambdapdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-02-20 16:46:58.000000 lambdapdk-0.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-20 16:47:15.167188 lambdapdk-0.1.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 16:47:15.167188 lambdapdk-0.1.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-02-20 16:46:58.000000 lambdapdk-0.1.9/tests/test_lambda.py
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-02-20 16:46:58.000000 lambdapdk-0.1.9/tests/test_local_detect.py
+-rw-r--r--   0 runner    (1001) docker     (127)      821 2024-02-20 16:46:58.000000 lambdapdk-0.1.9/tests/test_paths.py
```

### Comparing `lambdapdk-0.1.8/LICENSE` & `lambdapdk-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `lambdapdk-0.1.8/PKG-INFO` & `lambdapdk-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lambdapdk
-Version: 0.1.8
+Version: 0.1.9
 Summary: Library of open source Process Design Kits
 Author: Zero ASIC
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -194,21 +194,21 @@
            See the License for the specific language governing permissions and
            limitations under the License.
         
 Project-URL: Homepage, https://github.com/siliconcompiler/lambdapdk
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: siliconcompiler>=0.18.1
+Requires-Dist: siliconcompiler>=0.20.2
 Provides-Extra: dev
 Requires-Dist: flake8>=5.0.0; extra == "dev"
 Requires-Dist: pytest>=6.2.4; extra == "dev"
 Requires-Dist: pytest-timeout>=2.1.0; extra == "dev"
 Requires-Dist: tclint>=0.1.4; extra == "dev"
-Requires-Dist: lambdalib>=0.1.4; extra == "dev"
+Requires-Dist: lambdalib>=0.1.5; extra == "dev"
 
 # Lambdapdk Introduction
 
 The Lambdapdk project includes a number of open source Process Design Kits (PDKs). The original source of these PDKs is documented in the README file for each PDK. Cell level mapping is included to the generic technology independent [Lambdalib](https://github.com/siliconcompiler/lambdalib) library.
 
 Lambdapdk is supported by the [SiliconCompiler](https://github.com/siliconcompiler/siliconcompiler) project.
```

### Comparing `lambdapdk-0.1.8/README.md` & `lambdapdk-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `lambdapdk-0.1.8/lambdapdk/asap7/__init__.py` & `lambdapdk-0.1.9/lambdapdk/asap7/__init__.py`

 * *Files identical despite different names*

### Comparing `lambdapdk-0.1.8/lambdapdk/asap7/libs/asap7sc7p5t.py` & `lambdapdk-0.1.9/lambdapdk/asap7/libs/asap7sc7p5t.py`

 * *Files identical despite different names*

### Comparing `lambdapdk-0.1.8/lambdapdk/asap7/libs/fakeram7.py` & `lambdapdk-0.1.9/lambdapdk/asap7/libs/fakeram7.py`

 * *Files identical despite different names*

### Comparing `lambdapdk-0.1.8/lambdapdk/freepdk45/__init__.py` & `lambdapdk-0.1.9/lambdapdk/freepdk45/__init__.py`

 * *Files identical despite different names*

### Comparing `lambdapdk-0.1.8/lambdapdk/freepdk45/libs/fakeram45.py` & `lambdapdk-0.1.9/lambdapdk/freepdk45/libs/fakeram45.py`

 * *Files identical despite different names*

### Comparing `lambdapdk-0.1.8/lambdapdk/freepdk45/libs/nangate45.py` & `lambdapdk-0.1.9/lambdapdk/freepdk45/libs/nangate45.py`

 * *Files identical despite different names*

### Comparing `lambdapdk-0.1.8/lambdapdk/gf180/__init__.py` & `lambdapdk-0.1.9/lambdapdk/gf180/__init__.py`

 * *Files identical despite different names*

### Comparing `lambdapdk-0.1.8/lambdapdk/gf180/libs/gf180io.py` & `lambdapdk-0.1.9/lambdapdk/gf180/libs/gf180io.py`

 * *Files identical despite different names*

### Comparing `lambdapdk-0.1.8/lambdapdk/gf180/libs/gf180mcu.py` & `lambdapdk-0.1.9/lambdapdk/gf180/libs/gf180mcu.py`

 * *Files identical despite different names*

### Comparing `lambdapdk-0.1.8/lambdapdk/gf180/libs/gf180sram.py` & `lambdapdk-0.1.9/lambdapdk/gf180/libs/gf180sram.py`

 * *Files identical despite different names*

### Comparing `lambdapdk-0.1.8/lambdapdk/sky130/__init__.py` & `lambdapdk-0.1.9/lambdapdk/sky130/__init__.py`

 * *Files identical despite different names*

### Comparing `lambdapdk-0.1.8/lambdapdk/sky130/libs/sky130hd.py` & `lambdapdk-0.1.9/lambdapdk/sky130/libs/sky130hd.py`

 * *Files identical despite different names*

### Comparing `lambdapdk-0.1.8/lambdapdk/sky130/libs/sky130io.py` & `lambdapdk-0.1.9/lambdapdk/sky130/libs/sky130io.py`

 * *Files identical despite different names*

### Comparing `lambdapdk-0.1.8/lambdapdk/sky130/libs/sky130sram.py` & `lambdapdk-0.1.9/lambdapdk/sky130/libs/sky130sram.py`

 * *Files identical despite different names*

### Comparing `lambdapdk-0.1.8/lambdapdk.egg-info/PKG-INFO` & `lambdapdk-0.1.9/lambdapdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lambdapdk
-Version: 0.1.8
+Version: 0.1.9
 Summary: Library of open source Process Design Kits
 Author: Zero ASIC
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -194,21 +194,21 @@
            See the License for the specific language governing permissions and
            limitations under the License.
         
 Project-URL: Homepage, https://github.com/siliconcompiler/lambdapdk
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: siliconcompiler>=0.18.1
+Requires-Dist: siliconcompiler>=0.20.2
 Provides-Extra: dev
 Requires-Dist: flake8>=5.0.0; extra == "dev"
 Requires-Dist: pytest>=6.2.4; extra == "dev"
 Requires-Dist: pytest-timeout>=2.1.0; extra == "dev"
 Requires-Dist: tclint>=0.1.4; extra == "dev"
-Requires-Dist: lambdalib>=0.1.4; extra == "dev"
+Requires-Dist: lambdalib>=0.1.5; extra == "dev"
 
 # Lambdapdk Introduction
 
 The Lambdapdk project includes a number of open source Process Design Kits (PDKs). The original source of these PDKs is documented in the README file for each PDK. Cell level mapping is included to the generic technology independent [Lambdalib](https://github.com/siliconcompiler/lambdalib) library.
 
 Lambdapdk is supported by the [SiliconCompiler](https://github.com/siliconcompiler/siliconcompiler) project.
```

### Comparing `lambdapdk-0.1.8/lambdapdk.egg-info/SOURCES.txt` & `lambdapdk-0.1.9/lambdapdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lambdapdk-0.1.8/pyproject.toml` & `lambdapdk-0.1.9/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 authors = [{name = "Zero ASIC"}]
 description = "Library of open source Process Design Kits"
 readme = "README.md"
 urls = {Homepage = "https://github.com/siliconcompiler/lambdapdk"}
 requires-python = ">= 3.8"
 license = {file = "LICENSE"}
 dependencies = [
-    "siliconcompiler >= 0.18.1"
+    "siliconcompiler >= 0.20.2"
 ]
 dynamic = ['version']
 
 [tool.setuptools.dynamic]
 version = {attr = "lambdapdk.__version__"}
 
 [tool.pytest.ini_options]
@@ -27,15 +27,15 @@
 [project.optional-dependencies]
 # Dev dependencies.
 dev = [
     "flake8 >= 5.0.0",
     "pytest >= 6.2.4",
     "pytest-timeout >= 2.1.0",
     "tclint >= 0.1.4",
-    "lambdalib >= 0.1.4"
+    "lambdalib >= 0.1.5"
 ]
 
 [tool.tclint]
 exclude = [
     'build',
     'scripts/build',
     'dist',
```

### Comparing `lambdapdk-0.1.8/tests/test_lambda.py` & `lambdapdk-0.1.9/tests/test_lambda.py`

 * *Files identical despite different names*

### Comparing `lambdapdk-0.1.8/tests/test_paths.py` & `lambdapdk-0.1.9/tests/test_paths.py`

 * *Files identical despite different names*


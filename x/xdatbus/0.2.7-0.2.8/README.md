# Comparing `tmp/xdatbus-0.2.7.tar.gz` & `tmp/xdatbus-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xdatbus-0.2.7.tar", max compression
+gzip compressed data, was "xdatbus-0.2.8.tar", max compression
```

## Comparing `xdatbus-0.2.7.tar` & `xdatbus-0.2.8.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     1070 2024-03-17 23:39:00.304445 xdatbus-0.2.7/LICENSE
--rw-r--r--   0        0        0     3224 2024-03-17 23:39:00.304445 xdatbus-0.2.7/README.md
--rw-r--r--   0        0        0     1964 2024-03-17 23:39:00.316445 xdatbus-0.2.7/pyproject.toml
--rw-r--r--   0        0        0      585 2024-03-17 23:39:00.340445 xdatbus-0.2.7/xdatbus/__init__.py
--rw-r--r--   0        0        0     2074 2024-03-17 23:39:00.340445 xdatbus-0.2.7/xdatbus/bash01_bias.py
--rw-r--r--   0        0        0     4559 2024-03-17 23:39:00.340445 xdatbus-0.2.7/xdatbus/f01_xdc_aggregate.py
--rw-r--r--   0        0        0     4145 2024-03-17 23:39:00.340445 xdatbus-0.2.7/xdatbus/f02_xdc_unwrap.py
--rw-r--r--   0        0        0     2570 2024-03-17 23:39:00.340445 xdatbus-0.2.7/xdatbus/f03_xyz_unwarp.py
--rw-r--r--   0        0        0     1029 2024-03-17 23:39:00.340445 xdatbus-0.2.7/xdatbus/fcli.py
--rw-r--r--   0        0        0     1481 2024-03-17 23:39:00.340445 xdatbus-0.2.7/xdatbus/fcom01_drift.py
--rw-r--r--   0        0        0     1985 2024-03-17 23:39:00.340445 xdatbus-0.2.7/xdatbus/fcom02_contcar.py
--rw-r--r--   0        0        0     3306 2024-03-17 23:39:00.340445 xdatbus-0.2.7/xdatbus/fml01_xml2xyz.py
--rw-r--r--   0        0        0     1530 2024-03-17 23:39:00.340445 xdatbus-0.2.7/xdatbus/fmtd01_fes1d.py
--rw-r--r--   0        0        0     2052 2024-03-17 23:39:00.340445 xdatbus-0.2.7/xdatbus/fmtd02_fes2d.py
--rw-r--r--   0        0        0     2624 2024-03-17 23:39:00.340445 xdatbus-0.2.7/xdatbus/fmtd03_fes3d.py
--rw-r--r--   0        0        0     3036 2024-03-17 23:39:00.340445 xdatbus-0.2.7/xdatbus/fmtd04_hillspot2hills.py
--rw-r--r--   0        0        0     3998 2024-03-17 23:39:00.340445 xdatbus-0.2.7/xdatbus/fmtd05_report_loader.py
--rw-r--r--   0        0        0      667 2024-03-17 23:39:00.340445 xdatbus-0.2.7/xdatbus/fmtd06_xdc2xtc.py
--rw-r--r--   0        0        0     3172 2024-03-17 23:39:00.340445 xdatbus-0.2.7/xdatbus/fosz01_thermal_report.py
--rw-r--r--   0        0        0        0 2024-03-17 23:39:00.340445 xdatbus-0.2.7/xdatbus/resources/__init__.py
--rw-r--r--   0        0        0     2381 2024-03-17 23:39:00.340445 xdatbus-0.2.7/xdatbus/resources/color_data.yaml
--rw-r--r--   0        0        0 14415950 2024-03-17 23:39:00.376445 xdatbus-0.2.7/xdatbus/resources/node_data.blend
--rw-r--r--   0        0        0     1786 2024-03-17 23:39:00.376445 xdatbus-0.2.7/xdatbus/resources/sum_hills.sh
--rw-r--r--   0        0        0     4084 2024-03-17 23:39:00.376445 xdatbus-0.2.7/xdatbus/utils.py
--rw-r--r--   0        0        0    19248 2024-03-17 23:39:00.376445 xdatbus-0.2.7/xdatbus/utils_bpy.py
--rw-r--r--   0        0        0     4732 1970-01-01 00:00:00.000000 xdatbus-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-04-24 01:55:15.572847 xdatbus-0.2.8/LICENSE
+-rw-r--r--   0        0        0     3224 2024-04-24 01:55:15.572847 xdatbus-0.2.8/README.md
+-rw-r--r--   0        0        0     1965 2024-04-24 01:55:15.584847 xdatbus-0.2.8/pyproject.toml
+-rw-r--r--   0        0        0      585 2024-04-24 01:55:15.608847 xdatbus-0.2.8/xdatbus/__init__.py
+-rw-r--r--   0        0        0     2074 2024-04-24 01:55:15.608847 xdatbus-0.2.8/xdatbus/bash01_bias.py
+-rw-r--r--   0        0        0     4559 2024-04-24 01:55:15.608847 xdatbus-0.2.8/xdatbus/f01_xdc_aggregate.py
+-rw-r--r--   0        0        0     4145 2024-04-24 01:55:15.608847 xdatbus-0.2.8/xdatbus/f02_xdc_unwrap.py
+-rw-r--r--   0        0        0     2570 2024-04-24 01:55:15.608847 xdatbus-0.2.8/xdatbus/f03_xyz_unwarp.py
+-rw-r--r--   0        0        0     1029 2024-04-24 01:55:15.608847 xdatbus-0.2.8/xdatbus/fcli.py
+-rw-r--r--   0        0        0     1481 2024-04-24 01:55:15.608847 xdatbus-0.2.8/xdatbus/fcom01_drift.py
+-rw-r--r--   0        0        0     1985 2024-04-24 01:55:15.608847 xdatbus-0.2.8/xdatbus/fcom02_contcar.py
+-rw-r--r--   0        0        0     3306 2024-04-24 01:55:15.608847 xdatbus-0.2.8/xdatbus/fml01_xml2xyz.py
+-rw-r--r--   0        0        0     1530 2024-04-24 01:55:15.608847 xdatbus-0.2.8/xdatbus/fmtd01_fes1d.py
+-rw-r--r--   0        0        0     2052 2024-04-24 01:55:15.608847 xdatbus-0.2.8/xdatbus/fmtd02_fes2d.py
+-rw-r--r--   0        0        0     2624 2024-04-24 01:55:15.608847 xdatbus-0.2.8/xdatbus/fmtd03_fes3d.py
+-rw-r--r--   0        0        0     3036 2024-04-24 01:55:15.608847 xdatbus-0.2.8/xdatbus/fmtd04_hillspot2hills.py
+-rw-r--r--   0        0        0     3998 2024-04-24 01:55:15.608847 xdatbus-0.2.8/xdatbus/fmtd05_report_loader.py
+-rw-r--r--   0        0        0      899 2024-04-24 01:55:15.608847 xdatbus-0.2.8/xdatbus/fmtd06_xdc2xtc.py
+-rw-r--r--   0        0        0     3172 2024-04-24 01:55:15.608847 xdatbus-0.2.8/xdatbus/fosz01_thermal_report.py
+-rw-r--r--   0        0        0        0 2024-04-24 01:55:15.608847 xdatbus-0.2.8/xdatbus/resources/__init__.py
+-rw-r--r--   0        0        0     2381 2024-04-24 01:55:15.608847 xdatbus-0.2.8/xdatbus/resources/color_data.yaml
+-rw-r--r--   0        0        0 14415950 2024-04-24 01:55:15.644847 xdatbus-0.2.8/xdatbus/resources/node_data.blend
+-rw-r--r--   0        0        0     1786 2024-04-24 01:55:15.648847 xdatbus-0.2.8/xdatbus/resources/sum_hills.sh
+-rw-r--r--   0        0        0     4084 2024-04-24 01:55:15.648847 xdatbus-0.2.8/xdatbus/utils.py
+-rw-r--r--   0        0        0    19248 2024-04-24 01:55:15.648847 xdatbus-0.2.8/xdatbus/utils_bpy.py
+-rw-r--r--   0        0        0     4733 1970-01-01 00:00:00.000000 xdatbus-0.2.8/PKG-INFO
```

### Comparing `xdatbus-0.2.7/LICENSE` & `xdatbus-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `xdatbus-0.2.7/README.md` & `xdatbus-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `xdatbus-0.2.7/pyproject.toml` & `xdatbus-0.2.8/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "xdatbus"
-version = "0.2.7"
+version = "0.2.8"
 description = "A Python package for post-analysis of VASP AIMD data"
 authors = ["Jiacheng Wang <jiachengwang@umass.edu>"]
 maintainers = ["Jiacheng Wang"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://xdatbus.readthedocs.io/en/latest/"
 repository = "https://github.com/jcwang587/xdatbus/"
@@ -30,30 +30,30 @@
     "xdatbus-dev",
     "misc"
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.12"
 numpy = "1.26.4"
-pandas = "2.2.1"
-pyarrow = "15.0.1"
+pandas = "2.2.2"
+pyarrow = "16.0.0"
 ase = "3.22.1"
-pymatgen = "2024.3.1"
+pymatgen = "2024.4.13"
 mdanalysis = "2.7.0"
 rich = "13.7.1"
-plotly = { version = "5.20.0", optional = true }
+plotly = { version = "5.21.0", optional = true }
 dash = { version = "2.16.1", optional = true }
 rdkit = { version = "2023.9.5", optional = true }
 bpy = { version = "4.0.0", markers = "python_version == '3.10.*'", optional = true }
 pyyaml = { version = "6.0.1", optional = true }
-ovito = { version = "3.10.4", optional = true }
+ovito = { version = "3.10.5", optional = true }
 
 [tool.poetry.group.dev.dependencies]
 pytest = "8.1.1"
-pytest-cov = "4.1.0"
+pytest-cov = "5.0.0"
 
 [tool.poetry.extras]
 meta = ["rdkit", "bpy", "pyyaml", "ovito"]
 dash = ["plotly", "dash"]
 
 [tool.poetry.scripts]
 xdc_aggregate = "xdatbus.f01_xdc_aggregate:main"
```

### Comparing `xdatbus-0.2.7/xdatbus/__init__.py` & `xdatbus-0.2.8/xdatbus/__init__.py`

 * *Files identical despite different names*

### Comparing `xdatbus-0.2.7/xdatbus/bash01_bias.py` & `xdatbus-0.2.8/xdatbus/bash01_bias.py`

 * *Files identical despite different names*

### Comparing `xdatbus-0.2.7/xdatbus/f01_xdc_aggregate.py` & `xdatbus-0.2.8/xdatbus/f01_xdc_aggregate.py`

 * *Files identical despite different names*

### Comparing `xdatbus-0.2.7/xdatbus/f02_xdc_unwrap.py` & `xdatbus-0.2.8/xdatbus/f02_xdc_unwrap.py`

 * *Files identical despite different names*

### Comparing `xdatbus-0.2.7/xdatbus/f03_xyz_unwarp.py` & `xdatbus-0.2.8/xdatbus/f03_xyz_unwarp.py`

 * *Files identical despite different names*

### Comparing `xdatbus-0.2.7/xdatbus/fcli.py` & `xdatbus-0.2.8/xdatbus/fcli.py`

 * *Files identical despite different names*

### Comparing `xdatbus-0.2.7/xdatbus/fcom01_drift.py` & `xdatbus-0.2.8/xdatbus/fcom01_drift.py`

 * *Files identical despite different names*

### Comparing `xdatbus-0.2.7/xdatbus/fcom02_contcar.py` & `xdatbus-0.2.8/xdatbus/fcom02_contcar.py`

 * *Files identical despite different names*

### Comparing `xdatbus-0.2.7/xdatbus/fml01_xml2xyz.py` & `xdatbus-0.2.8/xdatbus/fml01_xml2xyz.py`

 * *Files identical despite different names*

### Comparing `xdatbus-0.2.7/xdatbus/fmtd01_fes1d.py` & `xdatbus-0.2.8/xdatbus/fmtd01_fes1d.py`

 * *Files identical despite different names*

### Comparing `xdatbus-0.2.7/xdatbus/fmtd02_fes2d.py` & `xdatbus-0.2.8/xdatbus/fmtd02_fes2d.py`

 * *Files identical despite different names*

### Comparing `xdatbus-0.2.7/xdatbus/fmtd03_fes3d.py` & `xdatbus-0.2.8/xdatbus/fmtd03_fes3d.py`

 * *Files identical despite different names*

### Comparing `xdatbus-0.2.7/xdatbus/fmtd04_hillspot2hills.py` & `xdatbus-0.2.8/xdatbus/fmtd04_hillspot2hills.py`

 * *Files identical despite different names*

### Comparing `xdatbus-0.2.7/xdatbus/fmtd05_report_loader.py` & `xdatbus-0.2.8/xdatbus/fmtd05_report_loader.py`

 * *Files identical despite different names*

### Comparing `xdatbus-0.2.7/xdatbus/fosz01_thermal_report.py` & `xdatbus-0.2.8/xdatbus/fosz01_thermal_report.py`

 * *Files identical despite different names*

### Comparing `xdatbus-0.2.7/xdatbus/resources/color_data.yaml` & `xdatbus-0.2.8/xdatbus/resources/color_data.yaml`

 * *Files identical despite different names*

### Comparing `xdatbus-0.2.7/xdatbus/resources/node_data.blend` & `xdatbus-0.2.8/xdatbus/resources/node_data.blend`

 * *Files identical despite different names*

### Comparing `xdatbus-0.2.7/xdatbus/resources/sum_hills.sh` & `xdatbus-0.2.8/xdatbus/resources/sum_hills.sh`

 * *Files identical despite different names*

### Comparing `xdatbus-0.2.7/xdatbus/utils.py` & `xdatbus-0.2.8/xdatbus/utils.py`

 * *Files identical despite different names*

### Comparing `xdatbus-0.2.7/xdatbus/utils_bpy.py` & `xdatbus-0.2.8/xdatbus/utils_bpy.py`

 * *Files identical despite different names*

### Comparing `xdatbus-0.2.7/PKG-INFO` & `xdatbus-0.2.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xdatbus
-Version: 0.2.7
+Version: 0.2.8
 Summary: A Python package for post-analysis of VASP AIMD data
 Home-page: https://xdatbus.readthedocs.io/en/latest/
 License: MIT
 Keywords: python,aimd,vasp,xdatcar
 Author: Jiacheng Wang
 Author-email: jiachengwang@umass.edu
 Maintainer: Jiacheng Wang
@@ -20,19 +20,19 @@
 Provides-Extra: dash
 Provides-Extra: meta
 Requires-Dist: ase (==3.22.1)
 Requires-Dist: bpy (==4.0.0) ; (python_version == "3.10.*") and (extra == "meta")
 Requires-Dist: dash (==2.16.1) ; extra == "dash"
 Requires-Dist: mdanalysis (==2.7.0)
 Requires-Dist: numpy (==1.26.4)
-Requires-Dist: ovito (==3.10.4) ; extra == "meta"
-Requires-Dist: pandas (==2.2.1)
-Requires-Dist: plotly (==5.20.0) ; extra == "dash"
-Requires-Dist: pyarrow (==15.0.1)
-Requires-Dist: pymatgen (==2024.3.1)
+Requires-Dist: ovito (==3.10.5) ; extra == "meta"
+Requires-Dist: pandas (==2.2.2)
+Requires-Dist: plotly (==5.21.0) ; extra == "dash"
+Requires-Dist: pyarrow (==16.0.0)
+Requires-Dist: pymatgen (==2024.4.13)
 Requires-Dist: pyyaml (==6.0.1) ; extra == "meta"
 Requires-Dist: rdkit (==2023.9.5) ; extra == "meta"
 Requires-Dist: rich (==13.7.1)
 Project-URL: Documentation, https://xdatbus.readthedocs.io/en/latest/
 Project-URL: Repository, https://github.com/jcwang587/xdatbus/
 Description-Content-Type: text/markdown
```


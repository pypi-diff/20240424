# Comparing `tmp/ICIW_Plots-1.0.6.tar.gz` & `tmp/ICIW_Plots-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ICIW_Plots-1.0.6.tar", last modified: Mon Jan  8 07:54:53 2024, max compression
+gzip compressed data, was "ICIW_Plots-1.0.7.tar", last modified: Mon Jan  8 08:07:53 2024, max compression
```

## Comparing `ICIW_Plots-1.0.6.tar` & `ICIW_Plots-1.0.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-01-08 07:54:53.341304 ICIW_Plots-1.0.6/
-drwxrwxrwx   0        0        0        0 2024-01-08 07:54:53.319300 ICIW_Plots-1.0.6/ICIW_Plots/
--rw-rw-rw-   0        0        0      114 2024-01-08 07:41:22.000000 ICIW_Plots-1.0.6/ICIW_Plots/__init__.py
--rw-rw-rw-   0        0        0     1896 2024-01-08 07:41:21.000000 ICIW_Plots-1.0.6/ICIW_Plots/cyclers.py
--rw-rw-rw-   0        0        0      795 2024-01-05 12:21:35.000000 ICIW_Plots-1.0.6/ICIW_Plots/layout.py
--rw-rw-rw-   0        0        0      112 2022-11-16 09:12:04.000000 ICIW_Plots-1.0.6/ICIW_Plots/util.py
-drwxrwxrwx   0        0        0        0 2024-01-08 07:54:53.332301 ICIW_Plots-1.0.6/ICIW_Plots.egg-info/
--rw-rw-rw-   0        0        0     1795 2024-01-08 07:54:53.000000 ICIW_Plots-1.0.6/ICIW_Plots.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      373 2024-01-08 07:54:53.000000 ICIW_Plots-1.0.6/ICIW_Plots.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-08 07:54:53.000000 ICIW_Plots-1.0.6/ICIW_Plots.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-01-08 07:54:53.000000 ICIW_Plots-1.0.6/ICIW_Plots.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-01-08 07:54:53.000000 ICIW_Plots-1.0.6/ICIW_Plots.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1091 2022-10-12 08:43:48.000000 ICIW_Plots-1.0.6/LICENSE.txt
--rw-rw-rw-   0        0        0       17 2022-10-12 13:26:13.000000 ICIW_Plots-1.0.6/MANIFEST.in
--rw-rw-rw-   0        0        0     1795 2024-01-08 07:54:53.340304 ICIW_Plots-1.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     1483 2022-10-13 07:24:32.000000 ICIW_Plots-1.0.6/README.md
--rw-rw-rw-   0        0        0       42 2024-01-08 07:54:53.341304 ICIW_Plots-1.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1673 2024-01-08 07:41:07.000000 ICIW_Plots-1.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2024-01-08 07:54:53.340304 ICIW_Plots-1.0.6/styles/
--rw-rw-rw-   0        0        0      893 2022-09-14 11:53:13.000000 ICIW_Plots-1.0.6/styles/ICIWlatex.mplstyle
--rw-rw-rw-   0        0        0       26 2022-09-14 12:00:32.000000 ICIW_Plots-1.0.6/styles/ICIWnobg.mplstyle
--rw-rw-rw-   0        0        0    41639 2022-11-14 10:34:34.000000 ICIW_Plots-1.0.6/styles/ICIWstyle.mplstyle
+drwxrwxrwx   0        0        0        0 2024-01-08 08:07:53.028862 ICIW_Plots-1.0.7/
+drwxrwxrwx   0        0        0        0 2024-01-08 08:07:53.014861 ICIW_Plots-1.0.7/ICIW_Plots/
+-rw-rw-rw-   0        0        0      116 2024-01-08 08:07:46.000000 ICIW_Plots-1.0.7/ICIW_Plots/__init__.py
+-rw-rw-rw-   0        0        0     1896 2024-01-08 07:41:21.000000 ICIW_Plots-1.0.7/ICIW_Plots/cyclers.py
+-rw-rw-rw-   0        0        0      795 2024-01-05 12:21:35.000000 ICIW_Plots-1.0.7/ICIW_Plots/layout.py
+-rw-rw-rw-   0        0        0      112 2022-11-16 09:12:04.000000 ICIW_Plots-1.0.7/ICIW_Plots/util.py
+drwxrwxrwx   0        0        0        0 2024-01-08 08:07:53.024863 ICIW_Plots-1.0.7/ICIW_Plots.egg-info/
+-rw-rw-rw-   0        0        0     1795 2024-01-08 08:07:52.000000 ICIW_Plots-1.0.7/ICIW_Plots.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      373 2024-01-08 08:07:52.000000 ICIW_Plots-1.0.7/ICIW_Plots.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-01-08 08:07:52.000000 ICIW_Plots-1.0.7/ICIW_Plots.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-01-08 08:07:52.000000 ICIW_Plots-1.0.7/ICIW_Plots.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-01-08 08:07:52.000000 ICIW_Plots-1.0.7/ICIW_Plots.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1091 2022-10-12 08:43:48.000000 ICIW_Plots-1.0.7/LICENSE.txt
+-rw-rw-rw-   0        0        0       17 2022-10-12 13:26:13.000000 ICIW_Plots-1.0.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     1795 2024-01-08 08:07:53.027862 ICIW_Plots-1.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1483 2022-10-13 07:24:32.000000 ICIW_Plots-1.0.7/README.md
+-rw-rw-rw-   0        0        0       42 2024-01-08 08:07:53.028862 ICIW_Plots-1.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1673 2024-01-08 08:07:43.000000 ICIW_Plots-1.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-01-08 08:07:53.026862 ICIW_Plots-1.0.7/styles/
+-rw-rw-rw-   0        0        0      893 2022-09-14 11:53:13.000000 ICIW_Plots-1.0.7/styles/ICIWlatex.mplstyle
+-rw-rw-rw-   0        0        0       26 2022-09-14 12:00:32.000000 ICIW_Plots-1.0.7/styles/ICIWnobg.mplstyle
+-rw-rw-rw-   0        0        0    41639 2022-11-14 10:34:34.000000 ICIW_Plots-1.0.7/styles/ICIWstyle.mplstyle
```

### Comparing `ICIW_Plots-1.0.6/ICIW_Plots/cyclers.py` & `ICIW_Plots-1.0.7/ICIW_Plots/cyclers.py`

 * *Files identical despite different names*

### Comparing `ICIW_Plots-1.0.6/ICIW_Plots/layout.py` & `ICIW_Plots-1.0.7/ICIW_Plots/layout.py`

 * *Files identical despite different names*

### Comparing `ICIW_Plots-1.0.6/ICIW_Plots.egg-info/PKG-INFO` & `ICIW_Plots-1.0.7/ICIW_Plots.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ICIW-Plots
-Version: 1.0.6
+Version: 1.0.7
 Summary: A collection of tools for use in the Institute of Chemical Engineering at Ulm University.
 Author: Hannes Stagge
 Author-email: hannes.stagge@uni-ulm.de
 License: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `ICIW_Plots-1.0.6/LICENSE.txt` & `ICIW_Plots-1.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ICIW_Plots-1.0.6/PKG-INFO` & `ICIW_Plots-1.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ICIW_Plots
-Version: 1.0.6
+Version: 1.0.7
 Summary: A collection of tools for use in the Institute of Chemical Engineering at Ulm University.
 Author: Hannes Stagge
 Author-email: hannes.stagge@uni-ulm.de
 License: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `ICIW_Plots-1.0.6/README.md` & `ICIW_Plots-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `ICIW_Plots-1.0.6/setup.py` & `ICIW_Plots-1.0.7/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 # Get description from README
 root = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(root, "README.md"), "r", encoding="utf-8") as f:
     long_description_str = f.read()
 
 setup(
     name="ICIW_Plots",
-    version="1.0.6",
+    version="1.0.7",
     description="A collection of tools for use in the Institute of Chemical Engineering at Ulm University.",
     long_description=long_description_str,
     long_description_content_type="text/markdown",
     author="Hannes Stagge",
     author_email="hannes.stagge@uni-ulm.de",
     license="MIT License",
     packages=["ICIW_Plots"],
```

### Comparing `ICIW_Plots-1.0.6/styles/ICIWlatex.mplstyle` & `ICIW_Plots-1.0.7/styles/ICIWlatex.mplstyle`

 * *Files identical despite different names*

### Comparing `ICIW_Plots-1.0.6/styles/ICIWstyle.mplstyle` & `ICIW_Plots-1.0.7/styles/ICIWstyle.mplstyle`

 * *Files identical despite different names*


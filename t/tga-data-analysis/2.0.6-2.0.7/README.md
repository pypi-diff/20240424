# Comparing `tmp/tga_data_analysis-2.0.6.tar.gz` & `tmp/tga_data_analysis-2.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tga_data_analysis-2.0.6.tar", last modified: Sun Apr 21 12:01:14 2024, max compression
+gzip compressed data, was "tga_data_analysis-2.0.7.tar", last modified: Tue Apr 23 03:26:38 2024, max compression
```

## Comparing `tga_data_analysis-2.0.6.tar` & `tga_data_analysis-2.0.7.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 12:01:14.031941 tga_data_analysis-2.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)     2047 2024-04-21 12:01:14.031941 tga_data_analysis-2.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-04-21 12:01:07.000000 tga_data_analysis-2.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-21 12:01:07.000000 tga_data_analysis-2.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 12:01:14.031941 tga_data_analysis-2.0.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 12:01:14.027941 tga_data_analysis-2.0.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 12:01:14.027941 tga_data_analysis-2.0.6/src/tga_data_analysis/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 12:01:07.000000 tga_data_analysis-2.0.6/src/tga_data_analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10365 2024-04-21 12:01:07.000000 tga_data_analysis-2.0.6/src/tga_data_analysis/kas_kinetics.py
--rw-r--r--   0 runner    (1001) docker     (127)     4229 2024-04-21 12:01:07.000000 tga_data_analysis-2.0.6/src/tga_data_analysis/measure.py
--rw-r--r--   0 runner    (1001) docker     (127)    27504 2024-04-21 12:01:07.000000 tga_data_analysis-2.0.6/src/tga_data_analysis/myfigure.py
--rw-r--r--   0 runner    (1001) docker     (127)    63386 2024-04-21 12:01:07.000000 tga_data_analysis-2.0.6/src/tga_data_analysis/tga.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 12:01:14.031941 tga_data_analysis-2.0.6/src/tga_data_analysis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2047 2024-04-21 12:01:14.000000 tga_data_analysis-2.0.6/src/tga_data_analysis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-21 12:01:14.000000 tga_data_analysis-2.0.6/src/tga_data_analysis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 12:01:14.000000 tga_data_analysis-2.0.6/src/tga_data_analysis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-21 12:01:14.000000 tga_data_analysis-2.0.6/src/tga_data_analysis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-21 12:01:14.000000 tga_data_analysis-2.0.6/src/tga_data_analysis.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 12:01:14.031941 tga_data_analysis-2.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-21 12:01:07.000000 tga_data_analysis-2.0.6/tests/test_deconvolution.py
--rw-r--r--   0 runner    (1001) docker     (127)     1979 2024-04-21 12:01:07.000000 tga_data_analysis-2.0.6/tests/test_kas_kinetics.py
--rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-04-21 12:01:07.000000 tga_data_analysis-2.0.6/tests/test_measure.py
--rw-r--r--   0 runner    (1001) docker     (127)     2933 2024-04-21 12:01:07.000000 tga_data_analysis-2.0.6/tests/test_my_figure.py
--rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-04-21 12:01:07.000000 tga_data_analysis-2.0.6/tests/test_oxidation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-04-21 12:01:07.000000 tga_data_analysis-2.0.6/tests/test_proximate.py
--rw-r--r--   0 runner    (1001) docker     (127)      959 2024-04-21 12:01:07.000000 tga_data_analysis-2.0.6/tests/test_soliddist.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 03:26:38.788982 tga_data_analysis-2.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     7854 2024-04-23 03:26:38.788982 tga_data_analysis-2.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7112 2024-04-23 03:26:32.000000 tga_data_analysis-2.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-23 03:26:33.000000 tga_data_analysis-2.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 03:26:38.788982 tga_data_analysis-2.0.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 03:26:38.784983 tga_data_analysis-2.0.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 03:26:38.788982 tga_data_analysis-2.0.7/src/tga_data_analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 03:26:33.000000 tga_data_analysis-2.0.7/src/tga_data_analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10365 2024-04-23 03:26:33.000000 tga_data_analysis-2.0.7/src/tga_data_analysis/kas_kinetics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4229 2024-04-23 03:26:33.000000 tga_data_analysis-2.0.7/src/tga_data_analysis/measure.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27504 2024-04-23 03:26:33.000000 tga_data_analysis-2.0.7/src/tga_data_analysis/myfigure.py
+-rw-r--r--   0 runner    (1001) docker     (127)    63511 2024-04-23 03:26:33.000000 tga_data_analysis-2.0.7/src/tga_data_analysis/tga.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 03:26:38.788982 tga_data_analysis-2.0.7/src/tga_data_analysis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7854 2024-04-23 03:26:38.000000 tga_data_analysis-2.0.7/src/tga_data_analysis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-23 03:26:38.000000 tga_data_analysis-2.0.7/src/tga_data_analysis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 03:26:38.000000 tga_data_analysis-2.0.7/src/tga_data_analysis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-23 03:26:38.000000 tga_data_analysis-2.0.7/src/tga_data_analysis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-23 03:26:38.000000 tga_data_analysis-2.0.7/src/tga_data_analysis.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 03:26:38.788982 tga_data_analysis-2.0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-23 03:26:33.000000 tga_data_analysis-2.0.7/tests/test_deconvolution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1979 2024-04-23 03:26:33.000000 tga_data_analysis-2.0.7/tests/test_kas_kinetics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-04-23 03:26:33.000000 tga_data_analysis-2.0.7/tests/test_measure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2933 2024-04-23 03:26:33.000000 tga_data_analysis-2.0.7/tests/test_my_figure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-04-23 03:26:33.000000 tga_data_analysis-2.0.7/tests/test_oxidation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-04-23 03:26:33.000000 tga_data_analysis-2.0.7/tests/test_proximate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-04-23 03:26:33.000000 tga_data_analysis-2.0.7/tests/test_soliddist.py
```

### Comparing `tga_data_analysis-2.0.6/pyproject.toml` & `tga_data_analysis-2.0.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "tga_data_analysis"
-version = "2.0.6"
+version = "2.0.7"
 authors = [
     { name = "Matteo Pecchi"}
 ]
 description = "Tool for automatic analysis of multiple TGA results"
 readme = "README.md"
 license = { text = "MIT" }
 classifiers = [
```

### Comparing `tga_data_analysis-2.0.6/src/tga_data_analysis/kas_kinetics.py` & `tga_data_analysis-2.0.7/src/tga_data_analysis/kas_kinetics.py`

 * *Files identical despite different names*

### Comparing `tga_data_analysis-2.0.6/src/tga_data_analysis/measure.py` & `tga_data_analysis-2.0.7/src/tga_data_analysis/measure.py`

 * *Files identical despite different names*

### Comparing `tga_data_analysis-2.0.6/src/tga_data_analysis/myfigure.py` & `tga_data_analysis-2.0.7/src/tga_data_analysis/myfigure.py`

 * *Files identical despite different names*

### Comparing `tga_data_analysis-2.0.6/src/tga_data_analysis/tga.py` & `tga_data_analysis-2.0.7/src/tga_data_analysis/tga.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,29 +14,29 @@
     Represents a project (identified by the folder where the data is stored)
     for TGA data analysis.
 
     """
 
     def __init__(
         self,
-        folder_path: plib.Path,
+        folder_path: plib.Path | str,
         name: str | None = None,
+        column_name_mapping: dict[str, str] | None = None,
+        load_skiprows: int = 0,
+        time_moist: float = 38.0,
+        time_vm: float = 147.0,
+        temp_initial_celsius: float = 40,
+        temp_lim_dtg_celsius: tuple[float] | None = None,
         temp_unit: Literal["C", "K"] = "C",
         plot_font: Literal["Dejavu Sans", "Times New Roman"] = "Dejavu Sans",
         dtg_basis: Literal["temperature", "time"] = "temperature",
         temp_i_temp_b_threshold: float = 0.01,  # % of the peak that is used for Ti and Tb
         resolution_sec_deg_dtg: int = 5,
         dtg_window_filter: int = 101,
         plot_grid: bool = False,
-        column_name_mapping: dict[str, str] | None = None,
-        load_skiprows: int = 0,
-        time_moist: float = 38.0,
-        time_vm: float = 147.0,
-        temp_initial_celsius: float = 40,
-        temp_lim_dtg_celsius: tuple[float] | None = None,
         auto_save_reports: bool = True,
     ):
         """
         Initialize a new Project instance with various parameters for analysis.
 
         :param folder_path: The path to the folder containing the project data.
         :type folder_path: plib.Path
@@ -67,16 +67,16 @@
         :param temp_initial_celsius: The initial temperature for certain calculations, in Celsius.
         :type temp_initial_celsius: float
         :param temp_lim_dtg_celsius: The temperature limits for DTG analysis, in Celsius.
         :type temp_lim_dtg_celsius: tuple[float], optional
         :param auto_save_reports: Whether to automatically save generated reports.
         :type auto_save_reports: bool
         """
-        self.folder_path = folder_path
-        self.out_path = plib.Path(folder_path, "output")
+        self.folder_path = plib.Path(folder_path)
+        self.out_path = plib.Path(self.folder_path, "output")
         if name is None:
             self.name = self.folder_path.parts[-1]
         else:
             self.name = name
         self.temp_unit = temp_unit
         self.plot_font = plot_font
         self.plot_grid = plot_grid
@@ -883,14 +883,16 @@
         :param correct_ash_mg: The correction value for ash in milligrams. If None, no correction is applied.
         :type correct_ash_mg: float, optional
         :param correct_ash_fr: The correction value for ash as a fraction. If None, no correction is applied.
         :type correct_ash_fr: float, optional
         :return: The corrected data as a pandas DataFrame.
         :rtype: pd.DataFrame
         """
+        if "m_mg" not in file.columns:
+            file["m_mg"] = file["m_p"]  # this avoids keyerrors
         if correct_ash_mg is not None:
             file["m_mg"] = file["m_mg"] - np.min(file["m_mg"]) + correct_ash_mg
         try:
             if file["m_mg"].iloc[-1] < 0:
                 print(
                     "neg. mass correction: Max [mg]",
                     np.round(np.max(file["m_mg"]), 3),
```

### Comparing `tga_data_analysis-2.0.6/src/tga_data_analysis.egg-info/SOURCES.txt` & `tga_data_analysis-2.0.7/src/tga_data_analysis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tga_data_analysis-2.0.6/tests/test_deconvolution.py` & `tga_data_analysis-2.0.7/tests/test_deconvolution.py`

 * *Files identical despite different names*

### Comparing `tga_data_analysis-2.0.6/tests/test_kas_kinetics.py` & `tga_data_analysis-2.0.7/tests/test_kas_kinetics.py`

 * *Files identical despite different names*

### Comparing `tga_data_analysis-2.0.6/tests/test_measure.py` & `tga_data_analysis-2.0.7/tests/test_measure.py`

 * *Files identical despite different names*

### Comparing `tga_data_analysis-2.0.6/tests/test_my_figure.py` & `tga_data_analysis-2.0.7/tests/test_my_figure.py`

 * *Files identical despite different names*

### Comparing `tga_data_analysis-2.0.6/tests/test_oxidation.py` & `tga_data_analysis-2.0.7/tests/test_oxidation.py`

 * *Files identical despite different names*

### Comparing `tga_data_analysis-2.0.6/tests/test_proximate.py` & `tga_data_analysis-2.0.7/tests/test_proximate.py`

 * *Files identical despite different names*

### Comparing `tga_data_analysis-2.0.6/tests/test_soliddist.py` & `tga_data_analysis-2.0.7/tests/test_soliddist.py`

 * *Files identical despite different names*


# Comparing `tmp/fm2prof-2.2.8.tar.gz` & `tmp/fm2prof-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fm2prof-2.2.8.tar", max compression
+gzip compressed data, was "fm2prof-2.3.1.tar", max compression
```

## Comparing `fm2prof-2.2.8.tar` & `fm2prof-2.3.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0       68 2024-03-04 13:54:30.256802 fm2prof-2.2.8/fm2prof/__init__.py
--rw-r--r--   0        0        0       70 2024-03-04 13:54:30.256802 fm2prof-2.2.8/fm2prof/__main__.py
--rw-r--r--   0        0        0     2560 2024-03-04 13:54:30.257804 fm2prof-2.2.8/fm2prof/cli.py
--rw-r--r--   0        0        0     9953 2024-03-04 13:54:30.258805 fm2prof-2.2.8/fm2prof/common.py
--rw-r--r--   0        0        0     4014 2024-03-04 13:54:30.258805 fm2prof-2.2.8/fm2prof/configurationfile_template.json
--rw-r--r--   0        0        0    61920 2024-03-15 14:38:36.609560 fm2prof-2.2.8/fm2prof/CrossSection.py
--rw-r--r--   0        0        0    17551 2024-03-04 13:54:30.241805 fm2prof-2.2.8/fm2prof/Export.py
--rw-r--r--   0        0        0    42662 2024-03-04 13:54:30.242804 fm2prof-2.2.8/fm2prof/Fm2ProfRunner.py
--rw-r--r--   0        0        0     8704 2024-03-04 13:54:30.243804 fm2prof-2.2.8/fm2prof/Functions.py
--rw-r--r--   0        0        0    12735 2024-03-04 13:54:30.244808 fm2prof-2.2.8/fm2prof/Import.py
--rw-r--r--   0        0        0    17323 2024-03-04 13:54:30.245804 fm2prof-2.2.8/fm2prof/IniFile.py
--rw-r--r--   0        0        0    17438 2024-03-04 13:54:30.262804 fm2prof-2.2.8/fm2prof/lib/polysimplify.py
--rw-r--r--   0        0        0     1526 2024-03-04 13:54:30.261804 fm2prof-2.2.8/fm2prof/lib/polysimplify.README.md
--rw-r--r--   0        0        0     1897 2024-03-15 19:24:08.964654 fm2prof-2.2.8/fm2prof/main.py
--rw-r--r--   0        0        0     3158 2024-03-04 13:54:30.254806 fm2prof-2.2.8/fm2prof/MaskOutputFile.py
--rw-r--r--   0        0        0    10321 2024-03-04 13:54:30.255803 fm2prof-2.2.8/fm2prof/RegionPolygonFile.py
--rw-r--r--   0        0        0   107273 2024-03-04 13:54:30.264804 fm2prof-2.2.8/fm2prof/utils.py
--rw-r--r--   0        0        0    35823 2024-03-04 13:54:29.969804 fm2prof-2.2.8/LICENSE.txt
--rw-r--r--   0        0        0      932 2024-03-04 13:54:29.970804 fm2prof-2.2.8/LICENSE_HEADER.txt
--rw-r--r--   0        0        0     1091 2024-03-15 19:52:34.715765 fm2prof-2.2.8/pyproject.toml
--rw-r--r--   0        0        0     2110 2024-03-04 13:54:29.972804 fm2prof-2.2.8/README.md
--rw-r--r--   0        0        0     2947 1970-01-01 00:00:00.000000 fm2prof-2.2.8/PKG-INFO
+-rw-r--r--   0        0        0       65 2024-04-24 18:51:55.859891 fm2prof-2.3.1/fm2prof/__init__.py
+-rw-r--r--   0        0        0       66 2024-04-24 18:51:55.861890 fm2prof-2.3.1/fm2prof/__main__.py
+-rw-r--r--   0        0        0     2457 2024-04-24 18:51:55.862889 fm2prof-2.3.1/fm2prof/cli.py
+-rw-r--r--   0        0        0    10183 2024-04-24 18:51:55.864889 fm2prof-2.3.1/fm2prof/common.py
+-rw-r--r--   0        0        0     4411 2024-04-24 18:51:55.867890 fm2prof-2.3.1/fm2prof/configurationfile_template.json
+-rw-r--r--   0        0        0    58333 2024-04-24 18:51:55.841887 fm2prof-2.3.1/fm2prof/CrossSection.py
+-rw-r--r--   0        0        0    17564 2024-04-24 18:51:55.844889 fm2prof-2.3.1/fm2prof/Export.py
+-rw-r--r--   0        0        0    42566 2024-04-24 18:51:55.847890 fm2prof-2.3.1/fm2prof/Fm2ProfRunner.py
+-rw-r--r--   0        0        0     8684 2024-04-24 18:51:55.849890 fm2prof-2.3.1/fm2prof/Functions.py
+-rw-r--r--   0        0        0    12579 2024-04-24 18:51:55.852894 fm2prof-2.3.1/fm2prof/Import.py
+-rw-r--r--   0        0        0    17768 2024-04-24 18:51:55.854890 fm2prof-2.3.1/fm2prof/IniFile.py
+-rw-r--r--   0        0        0    16955 2024-04-24 18:51:55.869892 fm2prof-2.3.1/fm2prof/lib/polysimplify.py
+-rw-r--r--   0        0        0     1484 2024-04-24 18:51:55.868896 fm2prof-2.3.1/fm2prof/lib/polysimplify.README.md
+-rw-r--r--   0        0        0     1897 2024-04-24 18:51:55.871890 fm2prof-2.3.1/fm2prof/main.py
+-rw-r--r--   0        0        0     3158 2024-04-24 18:51:55.856890 fm2prof-2.3.1/fm2prof/MaskOutputFile.py
+-rw-r--r--   0        0        0    10321 2024-04-24 18:51:55.857891 fm2prof-2.3.1/fm2prof/RegionPolygonFile.py
+-rw-r--r--   0        0        0   107724 2024-04-24 18:51:55.875890 fm2prof-2.3.1/fm2prof/utils.py
+-rw-r--r--   0        0        0    35823 2024-04-24 18:51:55.652889 fm2prof-2.3.1/LICENSE.txt
+-rw-r--r--   0        0        0      932 2024-04-24 18:51:55.653889 fm2prof-2.3.1/LICENSE_HEADER.txt
+-rw-r--r--   0        0        0     1295 2024-04-24 18:51:55.889892 fm2prof-2.3.1/pyproject.toml
+-rw-r--r--   0        0        0      794 2024-04-24 18:51:55.654907 fm2prof-2.3.1/README.md
+-rw-r--r--   0        0        0     1719 1970-01-01 00:00:00.000000 fm2prof-2.3.1/PKG-INFO
```

### Comparing `fm2prof-2.2.8/fm2prof/common.py` & `fm2prof-2.3.1/fm2prof/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,14 +58,17 @@
             "WARNING": [Back.YELLOW + Fore.BLACK, Fore.YELLOW],
             "ERROR": [Back.RED, Fore.RED],
             "CRITICAL": [Back.GREEN, Fore.GREEN],
         }
 
         colorama.init()
 
+        # saves amount of errors / warnings
+        self._loglibrary: dict = {"ERROR": 0, "WARNING": 0}
+
     @property
     def pbar(self):
         return self._pbar
 
     @pbar.setter
     def pbar(self, pbar):
         if isinstance(pbar, (tqdm.std.tqdm, type(None))):
@@ -103,14 +106,18 @@
     def __format_message(self, record: LogRecord):
         elapsed_seconds = record.created - self.start_time
         color = self._colors
 
         level = record.levelname
         message = record.getMessage()
 
+        # Counter of errors, warnings
+        if level in self._loglibrary:
+            self._loglibrary[level] += 1
+
         formatted_string = (
             f"║  {color[level][0]} {level:>7} "
             + f"{self._resetStyle}{color[level][1]}{self._resetStyle} T+ {elapsed_seconds:.2f}s {message}"
         )
 
         return formatted_string
```

### Comparing `fm2prof-2.2.8/fm2prof/configurationfile_template.json` & `fm2prof-2.3.1/fm2prof/configurationfile_template.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8648574561403508%*

 * *Differences: {"'sections'": "{'parameters': {'RelativeVelocityThreshold': {'hint': 'Relative velocity threshold "*

 * *               "(percentage). Used to determine storage'}, 'ConveyanceDetectionMethod': "*

 * *               "OrderedDict([('type', 'int'), ('hint', '[0] method based on mean flow velocity, "*

 * *               "[1] method based on maximum flow velocity (default)'), ('value', 1)]), delete: "*

 * *               "['ExportMapFiles', 'CssSelection']}, 'debug': OrderedDict([('ExportCSSData', "*

 * *               "OrderedDict([(' […]*

```diff
@@ -1,9 +1,26 @@
 {
     "sections": {
+        "debug": {
+            "CssSelection": {
+                "hint": "provide comma separated list of ints; e.g. 38, 39, 40. Leave empty to generate all cross-sections",
+                "type": "fm2prof.IniFile.ImportListType",
+                "value": ""
+            },
+            "ExportCSSData": {
+                "hint": "If True, exports pickled (1) input data for cross-section object, (2) flow mask for conveyance/storage.",
+                "type": "fm2prof.IniFile.ImportBoolType",
+                "value": false
+            },
+            "ExportMapFiles": {
+                "hint": "Export detailed map output. Only use for small models or limited number of cross-sections b/c output can be huge.",
+                "type": "fm2prof.IniFile.ImportBoolType",
+                "value": false
+            }
+        },
         "input": {
             "2DMapOutput": {
                 "hint": "Output file from FM2D model (.net file)",
                 "type": "str",
                 "value": ""
             },
             "CrossSectionLocationFile": {
@@ -46,23 +63,18 @@
                 "value": ""
             },
             "ClassificationMethod": {
                 "hint": "How to classify 2D output using Section and Region polygons. Options: [0] Do not classify regions or sections. [1] Use DeltaShell",
                 "type": "int",
                 "value": 0
             },
-            "CssSelection": {
-                "hint": "provide comma separated list of ints; e.g. 38, 39, 40. Leave empty to generate all cross-sections",
-                "type": "fm2prof.IniFile.ImportListType",
-                "value": ""
-            },
-            "ExportMapFiles": {
-                "hint": "Export detailed map output. Only use for small models or limited number of cross-sections b/c output can be huge.",
-                "type": "fm2prof.IniFile.ImportBoolType",
-                "value": false
+            "ConveyanceDetectionMethod": {
+                "hint": "[0] method based on mean flow velocity, [1] method based on maximum flow velocity (default)",
+                "type": "int",
+                "value": 1
             },
             "ExtrapolateStorage": {
                 "hint": "Add storage to water level independent cross-section section",
                 "type": "fm2prof.IniFile.ImportBoolType",
                 "value": true
             },
             "FrictionWeighingMethod": {
@@ -87,15 +99,15 @@
             },
             "MinimumTotalWidth": {
                 "hint": "Minimum width in meters. Zero width may lead to numerical instability in 1D solvers",
                 "type": "float",
                 "value": 0.5
             },
             "RelativeVelocityThreshold": {
-                "hint": "Relative velocity threshold (percent of mean flow velocity; 0-1). Used to determine storage",
+                "hint": "Relative velocity threshold (percentage). Used to determine storage",
                 "type": "float",
                 "value": 0.03
             },
             "SDCorrection": {
                 "hint": "Use summerdike volume correction",
                 "type": "fm2prof.IniFile.ImportBoolType",
                 "value": true
```

### Comparing `fm2prof-2.2.8/fm2prof/CrossSection.py` & `fm2prof-2.3.1/fm2prof/CrossSection.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,22 @@
-﻿"""
-Contains CrossSection class
-"""
 import math
+import pickle
 from logging import Logger
-from typing import List
+from typing import List, Dict
 import traceback
 from functools import reduce 
 
 from tqdm import tqdm
 import numpy as np
 import pandas as pd
 import scipy.optimize as so
 from scipy.integrate import cumtrapz
 
 from fm2prof import Functions as FE
 from fm2prof.common import FM2ProfBase, FrictionTable
-from fm2prof.Import import FmModelData
 from fm2prof.IniFile import IniFile
 from fm2prof.MaskOutputFile import MaskOutputFile
 
 from .lib import polysimplify as PS
 
 pd.options.mode.chained_assignment = None  # default='warn'
 
@@ -91,93 +88,95 @@
                 
                 pbar.update(1)
 
         return True
 
 
 class CrossSection(FM2ProfBase):
-    """
-    Use this class to derive cross-sections from fm_data (2D model results).
-    See docs how to acquire fm_data and how to prepare a proper 2D model.
-    """
-
-    __cs_parameter_css_points = "MaximumPointsInProfile"
     __cs_parameter_transitionheight_sd = "SDTransitionHeight"
+    __cs_parameter_conveyance_detection_method = "ConveyanceDetectionMethod"
     __cs_parameter_velocity_threshold = "AbsoluteVelocityThreshold"
     __cs_parameter_relative_threshold = "RelativeVelocityThreshold"
-    __cs_parameter_min_depth_storage = "MinimumDepthThreshold"
     __cs_parameter_plassen_timesteps = "LakeTimesteps"
-    __cs_parameter_storagemethod_wli = "ExtrapolateStorage"
-    __cs_parameter_bedlevelcriterium = "BedlevelCriterium"
-    __cs_parameter_SDstorage = "SDCorrection"
     __cs_parameter_Frictionweighing = "FrictionweighingMethod"
     __cs_parameter_sdoptimisationmethod = "sdoptimisationmethod"
     __cs_parameter_skip_maps = "SkipMaps"
-    __cs_parameter_floodplain_base_level = "SDFloodplainBase"
     __cs_parameter_minwidth = "MinimumTotalWidth"
-    __logger = None
 
     def __init__(
         self,
-        name: str,
-        length: float,
-        location: tuple,
-        branchid="not defined",
-        chainage=0,
-        fm_data: FmModelData = None,
-        logger: Logger = None,
-        inifile: IniFile = None,
+        data: Dict,
+        logger: Logger | None = None,
+        inifile: IniFile | None = None,
     ):
+        """   
+        Use this class to derive cross-sections from fm_data (2D model results).
+        See docs how to acquire fm_data and how to prepare a proper 2D model.
+        
+        Deprecated:
+            1.2: The `foo` attribute is deprecated.
+
+        >>> example co
+        hello!
+
+        Parameters:
+            data: contains stuff
+            logger: ala
+            inifile: woow
+
         """
-        Arguments:
-            InputParam_dict {Dictionary} -- [description]
-            name {str} -- [description]
-            length {float} -- [description]
-            location {tuple} -- [description]
-
-        Keyword Arguments:
-            branchid {str} -- [description] (default: {"not defined"})
-            chainage {int} -- [description] (default: {0})
-        """
+        # If inifile is not given, use default configuration
+        if inifile is None:
+            inifile = IniFile()
         super().__init__(logger=logger, inifile=inifile)
 
+        try:
+            assert all(key in data for key in ['id',
+                                               'length',
+                                               'xy',
+                                               'branchid',
+                                               'chainage',
+                                               'fm_data'])
+        except AssertionError:
+            raise KeyError("Input data does not have all required keys")
+            
         # Cross-section meta data
-        self.name = name  # cross-section id
-        self.length = length  # 'vaklengte'
-        self.location = location  # (x,y)
-        self.branch = branchid  # name of 1D branch for cross-section
-        self.chainage = chainage  # offset from beginning of branch
-        self.__output_mask_list = []  # initialize output mask list.
-        self._fm_data = fm_data  # dictionary with fmdata
+        self.name = data.get('id')  # cross-section id
+        self.length = data.get('length')  # 'vaklengte'
+        self.location = data.get('xy')  # (x,y)
+        self.branch = data.get('branchid')  # name of 1D branch for cross-section
+        self.chainage = data.get('chainage')  # offset from beginning of branch
+        self._fm_data: Dict = data.get('fm_data')  # dictionary with fmdata
+
 
         # Cross-section geometry
         self.z = []
         self.total_width = []
         self.flow_width = []
         self.section_widths = {"main": 0, "floodplain1": 0, "floodplain2": 0}
         self.friction_tables = dict()
         self.roughness_sections = np.array([])
 
         # delta h corrections ("summerdike option")
-        self.crest_level = 0
+        self.crest_level:float = 0
         # in cross-section def. WAQ2PROF did crest - some fixed value.
         #  how to do here?
         self.floodplain_base = 0.0
         # note" 'to avoid numerical oscillation'. might need minimal value.
         # fixed or variable? Test!
         self.transition_height = 0.5
         self.extra_flow_area = 0.0
         self.extra_total_volume = 0.0
         self.extra_area_percentage = list()
         self.extra_total_area = 0
         self.extra_flow_area = 0
 
         # These attributes are used for non-reduced sets
-        self._css_z = 0
-        self._css_total_volume = 0
+        self._css_z: np.ndarray = np.array([0])
+        self._css_total_volume: np.ndarray = np.array([0])
         self._css_total_volume_corrected = None
         self._css_flow_volume = 0
         self._css_flow_volume_corrected = None
         self._css_total_width = 0
         self._css_flow_width = 0
         self._css_volume_legacy = 0
         self._css_index_of_first_nonzero = 0
@@ -232,22 +231,32 @@
             return self.face_points_list
         elif pointtype == "edge":
             return self.edge_points_list
         else:
             raise ValueError('pointtype must be "face" or "edge"')
 
     # Public functions
-    def build_geometry(self):
+    def build_geometry(self) -> None:
         """
-        Build 1D geometrical cross-section from FM data.
+        This methods builds 1D geometrical cross-section from 2D data.
+        The 2D data is set on initalisation of the `CrossSection` object. 
+        The methods modifies the following attributes 
+        
+        Attributes:
+           _fm_wet_area
+           _fm_flow_area
+           _fm_total_volume
+           _fm_total_volume
+           _css_z_roughness
+           _css_z
+           _css_total_width
+           _css_flow_width
 
-        :param fm_data: dict
-        :return:
         """
-        fm_data = self._fm_data
+        fm_data: Dict = self._fm_data
 
         # Unpack FM data
         waterlevel = fm_data["waterlevel"].iloc[
             :, self.get_parameter(self.__cs_parameter_skip_maps) :
         ]
         waterdepth = fm_data["waterdepth"].iloc[
             :, self.get_parameter(self.__cs_parameter_skip_maps) :
@@ -271,53 +280,51 @@
         # Retrieve the water-depth
         # & water level nearest to the cross-section location
         self.set_logger_message("Retrieving centre point values")
         (centre_depth, centre_level) = FE.get_centre_values(
             self.location, fm_data["x"], fm_data["y"], waterdepth, waterlevel
         )
 
-        # apply rolling average over the velocities
-        # to smooth out extreme values
-        velocity = velocity.rolling(
-            window=10, min_periods=1, center=True, axis=1
-        ).mean()
-
         # Identify river lakes (plassen)
         self.set_logger_message("Identifying lakes")
         (
             plassen_mask,
             wet_not_plas_mask,
             plassen_depth_correction,
         ) = self._identify_lakes(
             waterdepth
         )  # plassen_mask needed for arrays in output
 
         # Masks for wet and flow cells (stroomvoeringscriteria)
-        self.set_logger_message("Seperating flow from storage")
-        flow_mask = self._distinguish_flow_from_storage(waterdepth, velocity)
+        self.set_logger_message("Separating conveyance from storage")
+        flow_mask = self._distinguish_conveyance_from_storage(waterdepth, velocity)
+
+        if self.get_inifile().get_parameter("ExportCSSData"): # pickle css data
+            output_dir = self.get_inifile().get_output_directory()
+            self.set_logger_message(f'pickling to {output_dir}')
+            with open(output_dir.joinpath(f"{self.name}_flowmask.pickle"), 'wb') as f:
+                pickle.dump(flow_mask, f)
 
         # Calculate area and volume as function of waterlevel & waterdepth
         self._fm_wet_area = np.nansum(area_matrix[wet_not_plas_mask], axis=0)
         self._fm_flow_area = np.nansum(area_matrix[flow_mask], axis=0)
 
         # Correct waterdepth for lakes
         waterdepth = waterdepth + plassen_depth_correction
         waterdepth = waterdepth[waterdepth >= 0]
 
         # Correct waterdepth for deep pools (volume below deepest point in centre
-        # should not be considered to be conveyance)
+        # should not be considered)
         pools_id = [
             i[0] for i in np.argwhere(waterdepth.to_numpy()[:, 0] > centre_depth[0])
         ]
         for pool in pools_id:
             amount_deeper = waterdepth.iloc[pool, 0] - centre_depth[0]
             waterdepth.iloc[pool] -= amount_deeper
 
-        # waterdepth[waterdepth > centre_depth[0]] = centre_depth[0]
-
         # Compute 2D volume as sum of area times depth
         self._fm_total_volume = np.array(
             np.nansum(
                 area_matrix[wet_not_plas_mask] * waterdepth[wet_not_plas_mask], axis=0
             )
         )
         self._fm_flow_volume = np.array(
@@ -342,16 +349,14 @@
 
         # Compute geometry below z0 - Water level independent calculation
         self.set_logger_message("Computing cross-section from bed levels")
         self._extend_css_below_z0(
             centre_level,
             centre_depth,
             waterlevel,
-            bedlevel_matrix,
-            area_matrix,
             wet_not_plas_mask.iloc[:, 0].values,
         )
 
         # Compute 1D volume as integral of width with respect to z times length
         self._css_total_volume = np.append(
             [0], cumtrapz(self._css_total_width, self._css_z) * self.length
         )
@@ -363,18 +368,14 @@
         self._css_total_volume_corrected = self._css_total_volume
         self._css_flow_volume_corrected = self._css_flow_volume
 
         # convert to float64 array for uniformity
         # (apparently entries can be float32)
         self._css_z = np.array(self._css_z, dtype=np.dtype("float64"))
 
-        fm_data["islake"] = plassen_mask
-
-        # generate all mask points for the given cross_section
-        # self.set_mask_output_list(fm_data, plassen_mask)
 
     def check_requirements(self):
         """
         Performs check on cross-section such that it
         hold up to requirements.
         """
         # Remove multiple zeroes in the bottom of the cross-section
@@ -485,15 +486,15 @@
             level="debug",
         )
         self.set_logger_message(
             "Final flow area: {:.4f} m2".format(extra_flow_volume / self.length),
             level="debug",
         )
 
-        extra_area_percentage = self.__get_extra_total_area(
+        extra_area_percentage = self._get_extra_total_area(
             self._css_z, crest_level, transition_height
         )
 
         # Write to attributes
         self._css_total_volume_corrected = (
             self._css_total_volume + extra_area_percentage * extra_total_volume
         )
@@ -532,43 +533,37 @@
         """use this method to return the number of 2D faces within control volume"""
         return len(self._fm_data.get("x"))
 
     def get_number_of_vertices(self) -> int:
         """Use this method to return the current number of geometry vertices"""
         return len(self._css_total_width)
 
-    def reduce_points(
-        self,
-        count_after: int = 20,
-        method: str = "visvalingam_whyatt",
-        verbose: bool = True,
-    ) -> None:
+    def reduce_points(self, count_after: int = 20) -> None:
         """
-        The cross-section geometry generated by |project| contains one point per output
+        The cross-section geometry generated by `fm2prof` contains one point per output
         timestep in the 2D map file. This resolution is often too high given the
         complexity of the cross-sections, and results in very large input files for the
-        1D model. Therefore |project| includes a simplification algorithm that reduces
+        1D model. Therefore `fm2prof` includes a simplification algorithm that reduces
         the number of points while preservering the shape of the geometry. This algorithm
         reduces as many points until the number specified in
-        :ref:`MaximumPointsInProfile<parameter_maximumpointsinprofile>` is reached.
-        We use the Visvalingam-Whyatt method of poly-line vertex reduction [VW]_.
-        The :term:`Total width` is leading for the simplification of the geometry meaning
+        `MaximumPointsInProfile` is reached.
+
+        We use the Visvalingam-Whyatt method of poly-line vertex reduction[^1].
+        The [total width](glossary.md#total-width) is leading for the simplification of the geometry meaning
         that the choice for which points to remove to simplify the geometry is based on
-        the total width. Subsequently, the corresponding point are removed from the :term:`Flow width`.
+        the total width. Subsequently, the corresponding point are removed from the [flow width](glossary.md#flow-width).
 
-        .. [VW] Visvalingam, M and Whyatt J D (1993) "Line Generalisation by Repeated Elimination of Points", Cartographic J., 30 (1), 46 - 51 URL: http://web.archive.org/web/20100428020453/http://www2.dcs.hull.ac.uk/CISRG/publications/DPs/DP10/DP10.html
+        [^1]:
+            Visvalingam, M and Whyatt J D (1993) "Line Generalisation by Repeated Elimination of Points", Cartographic J., 30 (1), 46 - 51 URL: http://web.archive.org/web/20100428020453/http://www2.dcs.hull.ac.uk/CISRG/publications/DPs/DP10/DP10.html
                 Implemented vertex reduction methods:
+            
 
-        Args:
-            n (int): asdf
-            method (str): asdf
-            verbose (bool): asdf
+        Parameters:
+            count_after: number of points in cross-section after application of this function
 
-        Returns:
-            None: This method directly works on the object attributes
         """
 
         n_before_reduction = self.get_number_of_vertices()
 
         points = np.array(
             [
                 [self._css_z[i], self._css_total_width[i]]
@@ -576,25 +571,23 @@
             ]
         )
 
         # The number of points is equal to n, it cannot be further reduced
         reduced_index = np.array([True] * n_before_reduction)
 
         if n_before_reduction > count_after:
-            # default is the same value as it came
-            if method.lower() == "visvalingam_whyatt":
-                try:
-                    simplifier = PS.VWSimplifier(points)
-                    reduced_index = simplifier.from_number_index(count_after)
-                except Exception as e:
-                    self.set_logger_message(
-                        "Exception thrown while using polysimplify: "
-                        + "{}".format(str(e)),
-                        "error",
-                    )
+            try:
+                simplifier = PS.VWSimplifier(points)
+                reduced_index = simplifier.from_number_index(count_after)
+            except Exception as e:
+                self.set_logger_message(
+                    "Exception thrown while using polysimplify: "
+                    + "{}".format(str(e)),
+                    "error",
+                )
 
         # Write to attributes
         self.z = self._css_z[reduced_index]
         self.total_width = self._css_total_width[reduced_index]
         self.flow_width = self._css_flow_width[reduced_index]
 
         self.set_logger_message(
@@ -616,19 +609,19 @@
             fm_data {dict} -- Dictionary containing x,y values.
             mask_array {NP.array} -- Array of values.
         """
         fm_data = self._fm_data
 
         # Properties keys
         cross_section_id_key = "cross_section_id"
-        cross_section_region_key = "region"
         is_lake_key = "is_lake"
         bedlevel_key = "bedlevel"
         section_key = "section"
         region_key = "region"
+        
 
         try:
             # Normalize np arrays to list for correct access
             x_coords = fm_data.get("x").tolist()
             y_coords = fm_data.get("y").tolist()
             region_list = fm_data.get("region").tolist()
             section_list = fm_data.get("section").tolist()
@@ -636,15 +629,14 @@
             is_lake_mask_list = fm_data.get("islake").tolist()
 
             # Assume same length for x and y coords.
             for i in range(len(x_coords)):
                 mask_properties = {
                     cross_section_id_key: self.name,
                     is_lake_key: is_lake_mask_list[i],
-                    cross_section_region_key: region_list[i],
                     bedlevel_key: bedlevel_list[i],
                     region_key: region_list[i],
                     section_key: section_list[i],
                 }
                 mask_coords = (x_coords[i], y_coords[i])
                 # Create the actual geojson element.
                 output_mask = MaskOutputFile.create_mask_point(
@@ -720,41 +712,24 @@
             self.set_logger_message(
                 "Error setting output masks "
                 + "for Cross Section {}. ".format(self.name)
                 + "Reason: {}".format(str(e_error)),
                 level="error",
             )
 
-    def interpolate_roughness_table(self, tablename, z_values):
-        """
-        Interpolates the roughness table to z values
-        """
-        table_name_list = ["main", "floodplain1"]
-
-        if tablename not in table_name_list:
-            raise KeyError("tablename not in list {}".format(table_name_list))
-
-        pass
-
     def _check_remove_duplicate_zeroes(self):
         """
         Removes duplicate zeroes in the total width
         """
-        mask = np.array([True] * len(self._css_z))
 
         # Remove multiple 0s in the total width
         index_of_first_nonzero = max(1, np.argwhere(self._css_total_width != 0)[0][0])
 
         return index_of_first_nonzero
 
-        # self._css_z = self._return_first_item_and_after_index(self._css_z, index_of_first_nonzero)
-        # self._css_flow_width = self._return_first_item_and_after_index(self._css_flow_width, index_of_first_nonzero)
-        # self._css_total_width = self._return_first_item_and_after_index(self._css_total_width, index_of_first_nonzero)
-        # self.set_logger_message(f'Removed {index_of_first_nonzero-1} duplicate zero widths', 'debug')
-
     @staticmethod
     def _return_first_item_and_after_index(listin, after_index):
         return np.append(listin[0], listin[after_index:].tolist())
 
     def _check_remove_zero_widths(self, width_array):
         """
         A zero width may lead to numerical instability
@@ -770,25 +745,25 @@
         Cost function, combines total volume error and flow volume error
         """
         (crest_level, extra_total_volume, extra_flow_volume) = opt_in
         transition_height = self.get_parameter(self.__cs_parameter_transitionheight_sd)
 
         predicted_total_volume = (
             self._css_total_volume
-            + self.__get_extra_total_area(self._css_z, crest_level, transition_height)
+            + self._get_extra_total_area(self._css_z, crest_level, transition_height)
             * extra_total_volume
         )
 
         predicted_flow_volume = (
             self._css_flow_volume
-            + self.__get_extra_total_area(self._css_z, crest_level, transition_height)
+            + self._get_extra_total_area(self._css_z, crest_level, transition_height)
             * extra_flow_volume
         )
 
-        return self.__return_volume_error(
+        return self._return_volume_error(
             predicted_total_volume + predicted_flow_volume,
             self._fm_total_volume + self._fm_flow_volume,
         )
 
     def _optimisation_func(self, opt_in, *args):
         """
         Objective function used in optimising a delta-h correction
@@ -809,18 +784,18 @@
             crest_level = args[0][2]
 
         volume = args[0][1]
         transition_height = self.get_parameter(self.__cs_parameter_transitionheight_sd)
 
         predicted_volume = (
             volume
-            + self.__get_extra_total_area(self._css_z, crest_level, transition_height)
+            + self._get_extra_total_area(self._css_z, crest_level, transition_height)
             * extra_volume
         )
-        return self.__return_volume_error(predicted_volume, self._fm_total_volume)
+        return self._return_volume_error(predicted_volume, self._fm_total_volume)
 
     def _optimize_sd_storage(
         self, initial_crest, initial_total_volume, initial_flow_volume
     ) -> dict:
         """
         Optimised the crest level and volumes
 
@@ -928,29 +903,29 @@
         ]
 
         sections = np.unique(self._fm_data.get("edge_section"))
 
         for section in sections:
             chezy_section = chezy_fm[self._fm_data["edge_section"] == section]
             if self.get_parameter(self.__cs_parameter_Frictionweighing) == 0:
-                friction = self._friction_weighing_simple(chezy_section, section)
+                friction = self._friction_weighing_simple(chezy_section)
             elif self.get_parameter(self.__cs_parameter_Frictionweighing) == 1:
                 friction = self._friction_weighing_area(chezy_section, section)
             else:
                 raise ValueError(
                     "unknown option for roughness weighing: {}".format(
                         self.get_parameter(self.__cs_parameter_Frictionweighing)
                     )
                 )
 
             self.friction_tables[self._section_map[str(section)]] = FrictionTable(
                 level=self._css_z_roughness, friction=friction
             )
 
-    def _friction_weighing_simple(self, link_chezy, section):
+    def _friction_weighing_simple(self, link_chezy):
         """Simple mean, no weight"""
         # Remove chezy where zero
         link_chezy = link_chezy.replace(0, np.NaN)
         output = link_chezy.mean(axis=0).replace(np.NaN, 0)
 
         return output.values
 
@@ -983,15 +958,15 @@
         """
         Computes sections widths by dividing the area assigned to a section
         by the length of the cross-section.
 
         If the sum of the section widths is smaller than the flow width, the
         width is increase proportionally
         """
-        total_area = sum(self._fm_data["area"])
+        
         unassigned_area = sum(self._fm_data["area"][self._fm_data["section"] == -999])
         if unassigned_area > 0:
             self.set_logger_message(
                 f"{unassigned_area} m2 was not assigned to any section in input files, and is added to the main section",
                 "warning",
             )
 
@@ -1048,36 +1023,36 @@
             self.set_logger_message(
                 f"No Floodplain found, floodplain defaults to {self.crest_level - tolerance}"
             )
 
     def _calc_chezy(self, depth, manning):
         return depth ** (1 / float(6)) / manning
 
-    def _identify_lakes(self, waterdepth):
+    def _identify_lakes(self, waterdepth:pd.DataFrame) -> np.ndarray:
         """
-        This algorithms determines whether a :ref:`2D cell <section_parsing_2d_data>` should
-        be marked as a :term:`Lake<Lakes>`.
+        This algorithms determines whether a 2D cell should
+        be marked as [Lake](glossary.md#Lakes).
 
         Cells are marked as lake if the following conditions are both met:
-            - the waterdepth on timestep :ref:`LakeTimeSteps <parameter_laketimesteps>` is positive
-            - the waterdepth on timestep :ref:`LakeTimeSteps <parameter_laketimesteps>` is at least 1 cm higher than the waterlevel on timestep 0.
+        - the waterdepth on timestep [LakeTimeSteps](configuration.md#exec-1--laketimesteps) is positive
+        - the waterdepth on timestep [LakeTimeSteps](configuration.md#exec-1--laketimesteps) is at least 1 cm higher than the waterlevel on timestep 0.
 
         Next, the following steps are taken
 
         - It is determined at what timestep the waterlevel in the lake starts rising. From that point on the lake counts as regular geometry and counts toward the total volume. A cell is considered active if its waterlevel has risen by 1 mm.
         - A correction matrix is built that contains the 'lake water level' for each lake cell. This matrix is subtracted from the waterdepth to compute volumes.
 
 
-        Args:
-            waterdepth (pandas dataframe):
+        Parameters:
+            waterdepth: a DataFrame containing all waterdepth output in the [control volume](glossary.md#control-volume)
 
         Returns:
-            lake_mask (ndarray): mask of all cells that are a 'lake'
-            wet_not_lake_mask (ndarray): mask of all cells that are wet, but not a lake
-            lake_depth_correction (ndarray): the depth of a lake at the start of the 2D computation
+            lake_mask: mask of all cells that are a 'lake'
+            wet_not_lake_mask: mask of all cells that are wet, but not a lake
+            lake_depth_correction: the depth of a lake at the start of the 2D computation
 
         """
         # preallocate arrays
         plassen_depth_correction = np.zeros(waterdepth.shape, dtype=float)
 
         # check for non-rising waterlevels
         waterdepth_diff = np.diff(waterdepth, n=1, axis=-1)
@@ -1157,97 +1132,108 @@
 
         # Flow width must increase at each z
         for i in range(2, len(self._css_flow_width) + 1):
             self._css_flow_width[-i] = np.min(
                 [self._css_flow_width[-i], self._css_flow_width[-i + 1]]
             )
 
-    def _distinguish_flow_from_storage_2(self, waterdepth, velocity):
+    def _distinguish_conveyance_from_storage(self, waterdepth: pd.DataFrame, velocity: pd.DataFrame) -> pd.DataFrame:
         """
-        This method determines which cells should be considered 'flowing'. A cell is considered flowing if all following conditions are met:
+        In 1D hydrodynamic models, flow through a cross-section is resolved assuming a 
+        cross-sectionally average velocity. This assumed that the entire cross-section
+        is available to for conveyance. However in reality some parts of the cross-section
+        do not contribute to flow. For example, sections of a river behind a levee where
+        water is stagnant contribute to storage (volume), but not flow. 
+
+        SOBEK enables distinction between 'flow area' and 'storage area'. `fm2prof` implements
+        methods to resolve from 2D model output which cells add to the 'flow volume' within a
+        [control volume](glossary.md#control-volume) and which to the storage volume. 
+
+        `fm2prof` implements two methods. The configuration parameter [`ConveyanceDetectionMethod`](configuration.md#exec-1--conveyancedetectionmethod) is used
+        to determine which method is used.
+
+        **`max_method`**
+        A cell is considered flowing if the velocity magnitude is more than the average
+        of the three higher flow velocities per outputmap multiplied by the 
+        [`relative velocity threshold`](configuration.md#exec-1--relativevelocitythreshold) OR
+        if the flow velocity meets the absolute threshold [`absolute velocity threshold`](configuration.md#exec-1--absolutevelocitythreshold)
 
-        - the waterdepth greater than 0
-        - the velocity is greater than :ref:`AbsoluteVelocityThreshold<parameter_absolutevelocitythreshold>`
-        - the velocity is greater than the product of the mean velocity (of all cells within the control volume) and the :ref:`RelativeVelocityThreshold<parameter_relativevelocitythreshold>`
+        **`mean_method`**
+        Not recommended. Legacy method.
 
-        Args:
-            waterdepth (pandas Dataframe) with cell id
-                for index and time in columns
-            velocity (pandas Dataframe() with cell id
-                for index and time in columns
+        Parameters:
+            waterdepth: dataframe of a control volume with waterdepths per cel per output map
+            velocity:  dataframe of a control volume with velocity magnitude per cel per output map
 
         Returns:
-            flow_mask (pandas Dataframe) with cell id for index and time in columns. True for flow, False for storage
+            flow_mask: dataframe of a control volume with the flow condition per cel per output map. `True` means flowing, `False` storage. 
         """
-        flow_mask = (
-            (waterdepth > 0)
-            & (velocity > self.get_parameter(self.__cs_parameter_velocity_threshold))
-            & (
-                velocity
-                > self.get_parameter(self.__cs_parameter_relative_threshold)
-                * np.mean(velocity)
-            )
-        )
-
-        # shallow flows should not be used for identifying storage
-        # (cells with small velocities are uncorrectly seen as storage)
-        waterdepth_correction = (waterdepth > 0) & (
-            waterdepth < self.get_parameter(self.__cs_parameter_min_depth_storage)
-        )
-
-        # combine flow and depth mask to avoid assigning shallow flows
-        flow_mask = flow_mask | waterdepth_correction
-
-        return flow_mask
-
-    def _distinguish_flow_from_storage(self, waterdepth, velocity):
-        """
-        This method determines which cells should be considered 'flowing'. A cell is considered flowing if all following conditions are met:
-
-        - the waterdepth greater than 0
-        - the velocity is greater than :ref:`AbsoluteVelocityThreshold<parameter_absolutevelocitythreshold>`
-        - the velocity is greater than the product of the mean velocity (of all cells within the control volume) and the :ref:`RelativeVelocityThreshold<parameter_relativevelocitythreshold>`
-
-        Args:
-            waterdepth (pandas Dataframe) with cell id
-                for index and time in columns
-            velocity (pandas Dataframe() with cell id
-                for index and time in columns
+        @staticmethod
+        def max_velocity_method(waterdepth: pd.DataFrame, velocity: pd.DataFrame) -> pd.DataFrame:
+            """
+            This method was added in version 2.3 because the mean_velocity_method
+            led to unreasonably high conveyance if the river was connected to 
+            an inland harbour. 
+            """
+            # This condition may be redundant
+            waterdepth_condition = waterdepth > 0
+            
+            # Determine maximum as the average of the top 3 flow velocities
+            maxv = velocity.max()
+            for i in velocity:
+                maxv[i] = velocity[i].sort_values().iloc[-3:].mean()
+            
+            # Relative to max condition
+            relative_velocity_condition = velocity > maxv*self.get_parameter(self.__cs_parameter_relative_threshold)
+            
+            # Absolute flow condition
+            absolute_velocity_condition =  velocity > self.get_parameter(self.__cs_parameter_velocity_threshold)
 
-        Returns:
-            flow_mask (pandas Dataframe) with cell id for index and time in columns. True for flow, False for storage
-        """
-        flow_mask = (
-            (waterdepth > 0)
-            & (velocity > self.get_parameter(self.__cs_parameter_velocity_threshold))
-            & (
-                velocity
-                > self.get_parameter(self.__cs_parameter_relative_threshold)
-                * np.mean(velocity)
+            # Flow mask determines which cells are conveyance (TRUE)
+            flow_mask = waterdepth_condition & (relative_velocity_condition | absolute_velocity_condition)
+            
+            return flow_mask
+            
+        @staticmethod
+        def mean_velocity_method(waterdepth, velocity):
+            """
+            This was the default method < 2.3. This method leads to unreasonably 
+            high conveyance if the river was connected to an inland harbour. 
+            """
+            # apply rolling average over the velocities
+            # to smooth out extreme values
+            velocity = velocity.rolling(
+                window=10, min_periods=1, center=True).mean()
+                
+            flow_mask = (
+                (waterdepth > 0)
+                & (velocity > self.get_parameter(self.__cs_parameter_velocity_threshold))
+                & (
+                    velocity
+                    > self.get_parameter(self.__cs_parameter_relative_threshold)
+                    * np.mean(velocity)
+                )
             )
-        )
-
-        # shallow flows should not be used for identifying storage
-        # (cells with small velocities are uncorrectly seen as storage)
-        waterdepth_correction = (waterdepth > 0) & (
-            waterdepth < self.get_parameter(self.__cs_parameter_min_depth_storage)
-        )
 
-        # combine flow and depth mask to avoid assigning shallow flows
-        # flow_mask = flow_mask | waterdepth_correction
+            return flow_mask
 
-        return flow_mask
+        match self.get_inifile().get_parameter(self.__cs_parameter_conveyance_detection_method):
+            case 0:
+                return mean_velocity_method(waterdepth, velocity)    
+            case 1:
+                return max_velocity_method(waterdepth, velocity)
+            case _:
+                self.set_logger_message('Invalid conveyance method. Defaulting to [1]', 'warning')
+                return max_velocity_method(waterdepth, velocity)
 
     def _extend_css_below_z0(
         self,
         centre_level,
         centre_depth,
         waterlevel,
-        bedlevel_matrix,
-        area_matrix,
         wet_not_plas_mask,
     ) -> None:
         """
         This methods computeS for level (z) below the water level at the first 2D output (z0) the corresponding
         :term:`Total width` and :term:`Flow width`. This is done in the following way:
 
         1. Take a number of steps (see note below) from z at t0 do the bed level at the :term:`Cross-section location`
@@ -1260,23 +1246,22 @@
             - if :ref:`ExtrapolateStorage <parameter_extrapolatestorage>` is False, the flow area is equal to the total area
 
         .. note::
             - the number of steps between z at t0 to bed level is hard-coded at 10.
             - the tolerance for deciding which cell is wet is hardcoded at -1e-3
 
 
-        Returns:
-            None: This method extends the following attributes:
-                    _css_z
-                    _css_total_width
-                    _css_flow_width
-                    _fm_wet_area
-                    _fm_flow_area
-                    _fm_flow_volume
-                    _fm_total_volume
+        Attributes:
+            _css_z
+            _css_total_width
+            _css_flow_width
+            _fm_wet_area
+            _fm_flow_area
+            _fm_flow_volume
+            _fm_total_volume
         """
 
         bedlevel = self._fm_data.get("bedlevel").values
         cell_area = self._fm_data.get("area").values
         flow_area_at_z0 = self._fm_flow_area[0]
         lowest_level_of_css = (
             centre_level[0] - centre_depth[0]
@@ -1296,137 +1281,55 @@
 
             # Extension of flow/storage below z0
             if not self.get_parameter("extrapolatestorage"):
                 total_flow_area = total_wet_area
             elif self.get_parameter("extrapolatestorage"):
                 total_flow_area = np.min([total_wet_area, flow_area_at_z0])
 
-            self._css_z = CrossSection.__append_to_start(
+            self._css_z = self._append_to_start(
                 self._css_z, centre_level_at_dz
             )
-            self._css_total_width = CrossSection.__append_to_start(
+            self._css_total_width = self._append_to_start(
                 self._css_total_width, total_wet_area / self.length
             )
-            self._css_flow_width = CrossSection.__append_to_start(
+            self._css_flow_width = self._append_to_start(
                 self._css_flow_width, total_flow_area / self.length
             )
-            self._fm_wet_area = CrossSection.__append_to_start(
+            self._fm_wet_area = self._append_to_start(
                 self._fm_wet_area, total_wet_area
             )
-            self._fm_flow_area = CrossSection.__append_to_start(
+            self._fm_flow_area = self._append_to_start(
                 self._fm_flow_area, total_flow_area
             )
             self._fm_flow_volume = np.insert(self._fm_flow_volume, 0, np.nan)
             self._fm_total_volume = np.insert(self._fm_total_volume, 0, np.nan)
 
-    @staticmethod
-    def __get_extra_total_area(
-        waterlevel, crest_level, transition_height: float, hysteresis=False
-    ):
+    def _get_extra_total_area(self,
+        waterlevel, crest_level, transition_height: float):
         """
         releases extra area dependent on waterlevel using a logistic (sigmoid) function
         """
         delta = 0.00001  # accuracy parameter
         return 1 / (
             1
             + np.e
             ** (
                 np.log(delta)
                 / (transition_height)
                 * (waterlevel - (crest_level + 0.5 * transition_height))
             )
         )
 
-    @staticmethod
-    def __append_to_start(array, to_add):
+    def _append_to_start(self, array, to_add):
         """
         adds ``to add`` to beginning of array
         """
         return np.insert(array, 0, to_add)
 
-    def __extend_css_with_constant_waterdepth(
-        self, centre_level, centre_depth, bedlevel_matrix, area_matrix, plassen_mask
-    ):
-        """
-        Extends the cross-sectional information below the water level
-        at the first timestep,
-        under assumption that the polygon formed by the water level
-        and the bed level is convex.
-        It works by walking down to the bed level at the center point
-        in 'virtual water level steps'.
-        At each step, we sum the area of cells width bedlevels which
-        would be submerged at that virtual water level.
-        """
-        filter_by_depth_percentage = (
-            self.get_parameter(self.__cs_parameter_bedlevelcriterium) * 100
-        )
-        filter_value = FE.empirical_ppf(
-            [filter_by_depth_percentage], bedlevel_matrix.values.T[0]
-        )[0]
-        self.set_logger_message(
-            "Lowest {}% of bed levels are filtered (z<{:.4f}m)".format(
-                filter_by_depth_percentage, filter_value
-            ),
-            level="debug",
-        )
-        level_z0 = centre_level[0]
-        bdata = bedlevel_matrix[~plassen_mask]
-        bmask = (bdata < level_z0) & (bdata >= filter_value)
-
-        self.set_logger_message(
-            "Number of points below z0 after applying filter: {}".format(
-                np.sum(bmask.values.T[0])
-            ),
-            level="debug",
-        )
-
-        # Compute values at z0
-        bedlevels_below_z0 = bdata[bmask]
-        lowest_level_below_z0 = centre_level[0] - centre_depth[0]
-        flow_area_at_z0 = self._fm_flow_area[0]
-        total_area_at_z0 = self._fm_wet_area[0]
-
-        for unique_level_below_z0 in reversed(
-            np.linspace(lowest_level_below_z0, level_z0, 10)
-        ):
-
-            # count area
-            areas = area_matrix[bedlevels_below_z0 <= unique_level_below_z0]
-
-            # Set area, such that the width computed from this area is equal or lower
-            # than the minimum width from the flow-dependent level
-            area_at_unique_level = np.min(
-                [np.nansum(areas.values.T[-1]), total_area_at_z0]
-            )
-
-            # Extension of flow/storage below z0
-            if self.get_parameter(self.__cs_parameter_storagemethod_wli) == 0:
-                flow_area_at_unique_level = area_at_unique_level
-            elif self.get_parameter(self.__cs_parameter_storagemethod_wli) == 1:
-                flow_area_at_unique_level = np.min(
-                    [area_at_unique_level, flow_area_at_z0]
-                )
-
-            # Insert values in existing arrays
-            self._css_z = np.insert(self._css_z, 0, unique_level_below_z0)
-            self._css_flow_width = np.insert(
-                self._css_flow_width, 0, flow_area_at_unique_level / self.length
-            )
-            self._css_total_width = np.insert(
-                self._css_total_width, 0, area_at_unique_level / self.length
-            )
-            self._fm_wet_area = np.insert(self._fm_wet_area, 0, area_at_unique_level)
-            self._fm_flow_area = np.insert(
-                self._fm_flow_area, 0, flow_area_at_unique_level
-            )
-            self._fm_flow_volume = np.insert(self._fm_flow_volume, 0, np.nan)
-            self._fm_total_volume = np.insert(self._fm_total_volume, 0, np.nan)
-
-    @staticmethod
-    def __return_volume_error(predicted, measured, gof="rmse"):
+    def _return_volume_error(self, predicted, measured):
         """
         Returns the squared relative error
         """
         non_nan_mask = ~np.isnan(predicted) & ~np.isnan(measured)
         predicted = predicted[non_nan_mask]
         measured = measured[non_nan_mask]
         error = np.array(predicted - measured) / np.maximum(
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `fm2prof-2.2.8/fm2prof/Export.py` & `fm2prof-2.3.1/fm2prof/Export.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,18 @@
 ﻿""" Input/output """
 
 # import from standar library
-import collections
-import locale
-import sys
 from dataclasses import astuple, dataclass
-from logging import Logger
-
+from typing import List
 import numpy as np
 
 # import from package
 from fm2prof import Functions as FE
 from fm2prof.common import FM2ProfBase
-
+from fm2prof.CrossSection import CrossSection
 
 @dataclass
 class OutputFiles:
     dimr_css_locations: str = "CrossSectionLocations.ini"
     dimr_css_definitions: str = "CrossSectionDefinitions.ini"
     dimr_roughness_main: str = "roughness-Main.ini"
     dimr_roughness_floodplain1: str = "roughness-FloodPlain1.ini"
@@ -36,15 +32,15 @@
 
 class Export1DModelData(FM2ProfBase):
     """
     This class contains all functions related to exporting to various output export.
     In the future, split in different classes for SOBEK, D-Hydro etc formats
     """
 
-    def export_geometry(self, cross_sections, file_path, fmt="sobek3"):
+    def export_geometry(self, cross_sections: List[CrossSection], file_path, fmt="sobek3"):
         with open(file_path, "w") as f:
             if fmt == "sobek3":
                 """SOBEK 3 style csv"""
                 self._write_geometry_sobek3(f, cross_sections)
             elif fmt == "dflow1d":
                 """DFM 1D style"""
                 self._write_geometry_fm1d(f, cross_sections)
```

### Comparing `fm2prof-2.2.8/fm2prof/Fm2ProfRunner.py` & `fm2prof-2.3.1/fm2prof/Fm2ProfRunner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import datetime
 import os
 import sys
 import time
+import pickle
 import traceback
 from pathlib import Path
 from typing import Dict, Generator, List, Mapping, NoReturn, Union
 
 import geojson
 import numpy as np
 import tqdm
@@ -129,15 +130,15 @@
             f"{self.__copyright__:>6}",
             "=" * 80,
             "",
         ]
         for line in header_text:
             self.set_logger_message(line, header=True)
 
-    def _run_inifile(self) -> None:
+    def _run_inifile(self) -> bool:
         """
         Executes main program from the configuration file. 
 
         The main steps in the program are:
         
         1. Initialize fm2prof
         2. Generate cross-sections
@@ -708,15 +709,15 @@
 
         if fm_model_data is None:
             raise Exception(
                 "No FM data given for new cross section {}".format(css_name)
             )
         
         # Create cross section
-        created_css = self._get_new_cross_section(css_data=css_data)
+        created_css = self._create_new_cross_section(css_data=css_data)
 
         if created_css is None:
             self.set_logger_message(
                 f"No Cross-section could be generated for {css_name}", "error"
             )
             return None
         if created_css.get_number_of_faces() < 10:
@@ -746,15 +747,15 @@
 
         Parameters:
             cross_section {CrossSection}
                 -- Given Cross Section.
         """
 
         if cross_section is None:
-            return
+            raise Exception
 
         # Build cross-section
         self.set_logger_message("Start building geometry", "debug")
         cross_section.build_geometry()
 
         # 2D Volume Correction (SummerDike option)
         if self.get_inifile().get_parameter("SDCorrection"):
@@ -782,15 +783,15 @@
         # Assign roughness
         self.set_logger_message("Starting computing roughness tables", "debug")
         cross_section.assign_roughness()
         self.set_logger_message("Computed roughness", "info")
 
         return cross_section
 
-    def _get_new_cross_section(self, css_data: Mapping[str, str]):
+    def _create_new_cross_section(self, css_data: Mapping[str, str]):
         """Creates a cross section with the given input param dictionary.
 
         Arguments:
             css_data {Mapping[str, str]}
                 -- FM Model data for cross section.
             input_param_dict {Mapping[str, str]}
                 -- Dictionary with parameters for Cross Section.
@@ -798,42 +799,37 @@
         Returns:
             {CrossSection} -- New cross section object.
         """
         # Get id data and id index
         if not css_data:
             return None
 
-        css_data_id = css_data.get("id")
-        if not css_data_id:
+        if not css_data.get("id"):
             return None
 
-        # Get remainig data
-        css_data_length = css_data.get("length")
-        css_data_location = css_data.get("xy")
-        css_data_branch_id = css_data.get("branchid")
-        css_data_chainage = css_data.get("chainage")
-
         if (
-            css_data_length is None
-            or css_data_location is None
-            or css_data_branch_id is None
-            or css_data_chainage is None
+            css_data.get("length") is None
+            or css_data.get("xy") is None
+            or css_data.get("branchid") is None
+            or css_data.get("chainage") is None
         ):
             return None
 
+        # Get remainig data
+        css_data['fm_data'] = self.fm_model_data.get_selection(css_data.get("id"))
+
+        if self.get_inifile().get_parameter("ExportCSSData"):
+            output_dir = self.get_inifile().get_output_directory()
+            with open(output_dir.joinpath(f"{css_data.get('id')}.pickle"), 'wb') as f:
+                pickle.dump(css_data, f)
         try:
             css = CrossSection(
                 logger=self.get_logger(),
                 inifile=self.get_inifile(),
-                name=css_data_id,
-                length=css_data_length,
-                location=css_data_location,
-                branchid=css_data_branch_id,
-                chainage=css_data_chainage,
-                fm_data=self.fm_model_data.get_selection(css_data_id),
+                data = css_data,
             )
 
         except Exception as e_info:
             self.set_logger_message(
                 "Exception thrown while creating cross-section "
                 + "{}, message: {}".format(css_data_id, str(e_info)),
                 "error",
```

### Comparing `fm2prof-2.2.8/fm2prof/Functions.py` & `fm2prof-2.3.1/fm2prof/Functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,17 +103,15 @@
 
         # Do Nearest Neighour
         neigh = _get_class_tree(css_xy, css_id)
         css_2d_nodes = neigh.predict(np.array([x_2d_node, y_2d_node]).T)
         css_2d_edges = neigh.predict(np.array([x_2d_edge, y_2d_edge]).T)
 
         # Update data in main structures
-        time_independent_data["sclass"][
-            node_mask
-        ] = css_2d_nodes  # sclass = cross-section id
+        time_independent_data.loc[node_mask, "sclass"] = css_2d_nodes  # sclass = cross-section id
 
         edge_data["sclass"][edge_mask] = css_2d_edges
 
     return time_independent_data, edge_data
 
 
 def classify_without_regions(cssdata, time_independent_data, edge_data):
```

### Comparing `fm2prof-2.2.8/fm2prof/Import.py` & `fm2prof-2.3.1/fm2prof/Import.py`

 * *Files 2% similar despite different names*

```diff
@@ -239,39 +239,35 @@
         edge_section = edge_data["section"][
             edge_data["sclass"] == css_name
         ]  # roughness section number
 
         # retrieve the full set for face_nodes and area, needed for the roughness calculation
         # face_nodes = edge_data['face_nodes'][dti['sclass'] == css_name]
         # face_nodes_full = edge_data['face_nodes']
-        area_full = dti["area"]
-        bedlevel_full = dti["bedlevel"]
         bedlevel = dti["bedlevel"][dti["sclass"] == css_name]
 
         velocity = (vx**2 + vy**2) ** 0.5
         waterlevel[waterdepth == 0] = np.nan
 
         return_dict = {
             "x": x,
             "y": y,
             "area": area,
             "bedlevel": bedlevel,
-            "bedlevel_full": bedlevel_full,
             "waterdepth": waterdepth,
             "waterlevel": waterlevel,
             "velocity": velocity,
             "section": face_section,
             "chezy": chezy,
             "region": region,
             "islake": islake,
             "edge_faces": edge_faces,
             "edge_x": edge_x,
             "edge_y": edge_y,
             "edge_section": edge_section,
-            "area_full": area_full,
         }
 
         return return_dict
 
 
 class ImportInputFiles(FM2ProfBase):
     """
```

### Comparing `fm2prof-2.2.8/fm2prof/IniFile.py` & `fm2prof-2.3.1/fm2prof/IniFile.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,14 +50,15 @@
         file_path (str): path to filestring
 
     """
 
     _file: Path = None
     __input_files_key = "input"
     __input_parameters_key = "parameters"
+    __input_debug_key = "debug"
     __output_key = "output"
     __output_directory_key = "OutputDirectory"
     __ini_keys = dict(
         map_file="2dmapoutput",
         css_file="crosssectionlocationfile",
         region_file="regionpolygonfile",
         section_file="sectionpolygonfile",
@@ -198,23 +199,31 @@
         """
         return self._get_from_configuration("input", key)
 
     def get_parameter(self, key: str) -> Union[str, bool, int, float]:
         """
         Use this method to return a parameter value
         """
-        return self._get_from_configuration("parameters", key)
+        try:
+            return self._get_from_configuration("parameters", key)
+        except KeyError:
+            pass
+        try:
+            return self._get_from_configuration("debug", key)
+        except KeyError:
+            pass
+        self.set_logger_message(f"unknown key {key}", "error")
 
-    def set_input_file(self, key: str, value=None) -> bool:
+    def set_input_file(self, key: str, value=None) -> None:
         """Use this method to set a input files the configuration"""
         self._set_config_value("input", key, value)
 
-    def set_parameter(self, key, value) -> None:
+    def set_parameter(self, key:str, value, section="parameters") -> None:
         """Use this method to set a key/value pair to the configuration"""
-        self._set_config_value("parameters", key, value)
+        self._set_config_value(section, key, value)
 
     def _set_config_value(self, section, key, value) -> None:
         """Use this method to set a input files the configuration"""
         ckey = self._get_key_from_case_insensitive_input(section=section, key_in=key)
         if ckey:
             self._configuration["sections"][section][ckey]["value"] = value
             return True
@@ -265,14 +274,15 @@
 
     def _get_from_configuration(
         self, section: str, key: str
     ) -> Union[str, bool, int, float]:
         for parameter, content in self._configuration["sections"].get(section).items():
             if parameter.lower() == key.lower():
                 return content.get("value")
+        raise KeyError(f"key {key} not found")
 
     def _get_template_ini(self) -> Dict:
         # Open config file
         path, _ = os.path.split(inspect.getabsfile(IniFile))
         with open(os.path.join(path, "configurationfile_template.json"), "r") as f:
             default_ini = json.load(f)
 
@@ -311,47 +321,48 @@
         try:
             self._extract_input_files(supplied_ini)
         except Exception as e_info:
             self.set_logger_message(
                 "Unexpected error reading input files. Check config file", "error"
             )
         try:
-            self._extract_parameters(supplied_ini)
+            self._extract_parameters(supplied_ini, self.__input_parameters_key)
+            self._extract_parameters(supplied_ini, self.__input_debug_key)
         except Exception:
             self.set_logger_message(
-                "Unexpected error reading parameters. Check config file", "error"
+                "Unexpected error reading (debug) parameters. Check config file", "error"
             )
         try:
             self._extract_output_dir(supplied_ini)
         except Exception:
             self.set_logger_message(
                 "Unexpected error output parameters. Check config file", "error"
             )
 
-    def _extract_parameters(self, supplied_ini: Mapping[str, list]):
+    def _extract_parameters(self, supplied_ini: Mapping[str, list], section: str):
         """Extract InputParameters and convert values either integer or float from string
 
         Arguments:
             inifile_parameters {Mapping[str, list} -- Collection of parameters as read in the original file
 
         Returns:
             {Mapping[str, number]} -- Dictionary of mapped parameters to a either integer or float
         """
         try:
-            inputsection = supplied_ini.get(self.__input_parameters_key)
+            inputsection = supplied_ini.get(section)
         except KeyError:
             raise InvalidConfigurationFileError
 
         for key, value in inputsection.items():
             key_default, key_type = self._get_key_from_template(
-                self.__input_parameters_key, key
+                section, key
             )
             try:
                 parsed_value = key_type(value)
-                self.set_parameter(key_default, parsed_value)
+                self.set_parameter(key_default, parsed_value, section)
             except ValueError:
                 self.set_logger_message(
                     f"{key} could not be cast as {key_type}", "debug"
                 )
             except KeyError:
                 pass
```

### Comparing `fm2prof-2.2.8/fm2prof/lib/polysimplify.README.md` & `fm2prof-2.3.1/fm2prof/lib/polysimplify.README.md`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-Visvalingam-Whyatt polyline simplification
-=====================
-
-Efficient Pure Python implementation of Visvalingam and Whyatt's 
-algorithm for reducing the complexity of poly-lines.  Also 
-includes precision decimation to reduce file sizes if desired. 
-
-Works with GDAL OGRGeometry LINESTRING, POLYGON and MULTIPOLYGON
-objects as well as lists of vertices.
-
-This method ranks the verticies by their importance to the 
-shape (how much removing the affects the area) in a 
-non-destructive manner.  Once the ranking has been done, 
-filtering of points is ultra fast (just one numpy mask 
-operation).
-
-However, even for just one filtering operation, this
-method seems to be faster than Ramer-Douglas-Peucker.
-
-    from polysimplify import VWSimplifier
-    import numpy as np
-    from time import time
-
-    n = 5000
-    thetas = np.linspace(0,2*np.pi,n)
-    pts = np.array([[np.sin(x),np.cos(x)] for x in thetas])
-    
-    start=time()
-    simplifier = VWSimplifier(pts)
-    VWpts = simplifier.from_number(n/100)
-    end = time() 
-    print "Visvalingam: reduced to %s points in %03f seconds" %(len(VWpts),end-start)
-    #50 points in .131 seconds on my computer
-
-
-    from rdp import rdp
-    start=time()
-    RDPpts = rdp(pts,epsilon=.00485) #found by trail and error
-    end = time()
-    print "Ramer-Douglas-Peucker: to %s points in %023 seconds" %(len(RDPpts),end-start)
-    #40 points in 1.35 seconds on my computer
-	
+Visvalingam-Whyatt polyline simplification
+=====================
+
+Efficient Pure Python implementation of Visvalingam and Whyatt's 
+algorithm for reducing the complexity of poly-lines.  Also 
+includes precision decimation to reduce file sizes if desired. 
+
+Works with GDAL OGRGeometry LINESTRING, POLYGON and MULTIPOLYGON
+objects as well as lists of vertices.
+
+This method ranks the verticies by their importance to the 
+shape (how much removing the affects the area) in a 
+non-destructive manner.  Once the ranking has been done, 
+filtering of points is ultra fast (just one numpy mask 
+operation).
+
+However, even for just one filtering operation, this
+method seems to be faster than Ramer-Douglas-Peucker.
+
+    from polysimplify import VWSimplifier
+    import numpy as np
+    from time import time
+
+    n = 5000
+    thetas = np.linspace(0,2*np.pi,n)
+    pts = np.array([[np.sin(x),np.cos(x)] for x in thetas])
+    
+    start=time()
+    simplifier = VWSimplifier(pts)
+    VWpts = simplifier.from_number(n/100)
+    end = time() 
+    print "Visvalingam: reduced to %s points in %03f seconds" %(len(VWpts),end-start)
+    #50 points in .131 seconds on my computer
+
+
+    from rdp import rdp
+    start=time()
+    RDPpts = rdp(pts,epsilon=.00485) #found by trail and error
+    end = time()
+    print "Ramer-Douglas-Peucker: to %s points in %023 seconds" %(len(RDPpts),end-start)
+    #40 points in 1.35 seconds on my computer
+	
 retrieved from https://github.com/Permafacture on 23-march-2016
```

### Comparing `fm2prof-2.2.8/fm2prof/main.py` & `fm2prof-2.3.1/fm2prof/main.py`

 * *Files identical despite different names*

### Comparing `fm2prof-2.2.8/fm2prof/MaskOutputFile.py` & `fm2prof-2.3.1/fm2prof/MaskOutputFile.py`

 * *Files identical despite different names*

### Comparing `fm2prof-2.2.8/fm2prof/RegionPolygonFile.py` & `fm2prof-2.3.1/fm2prof/RegionPolygonFile.py`

 * *Files identical despite different names*

### Comparing `fm2prof-2.2.8/fm2prof/utils.py` & `fm2prof-2.3.1/fm2prof/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -606,16 +606,15 @@
                     bbox_inches="tight",
                 )
             else:
                 return fig
 
         except Exception as e:
             self.set_logger_message(
-                f"error processing: {css['id']} {str(e)}", "error", pbar=pbar
-            )
+                f"error processing: {css['id']} {str(e)}", "error")
             return None
 
         finally:
             plt.close()
 
     def plot_cross_sections(self):
         """Makes figures for all cross-sections in project,
@@ -999,16 +998,16 @@
             # Set styles for each axis
             legend_title = r"toelichting"
             handles = list()
             labels = list()
 
             for ax in fig.axes:
 
-                ax.grid(b=True, which="major", linestyle="-", linewidth=1, color="k")
-                ax.grid(b=True, which="minor", linestyle="-", linewidth=0.5, color="k")
+                ax.grid(visible=True, which="major", linestyle="-", linewidth=1, color="k")
+                ax.grid(visible=True, which="minor", linestyle="-", linewidth=0.5, color="k")
 
                 for _, spine in ax.spines.items():
                     spine.set_linewidth(2)
 
                 if cls._is_timeaxis(ax.xaxis):
                     ax.xaxis.set_major_formatter(cls.myFmt)
                     ax.xaxis.set_major_locator(cls.monthlocator)
@@ -1235,27 +1234,27 @@
     _key_2D_H = "waterlevel"
     __fileOutName_1D2DMap = "map_1d_2d.csv"
 
     _time_fmt = "%Y-%m-%d %H:%M:%S"
 
     def __init__(self, 
                  logger=None, 
-                 start_time: datetime = None,
-                 stop_time: datetime = None):
+                 start_time: datetime | None = None,
+                 stop_time: datetime | None = None):
         super().__init__(logger=logger)
 
         self._path_out: Path = Path(".")
         self._path_flow1d: Path = Path(".")
         self._path_flow2d: Path = Path(".")
 
         self._data_1D_Q: pd.DataFrame = None
         self._time_offset_1d: int = 0
 
-        self._start_time: Union[datetime, type(None)] = start_time
-        self._stop_time: Union[datetime, type(None)] = stop_time
+        self._start_time: datetime | None = start_time
+        self._stop_time: datetime | None = stop_time
 
     @property
     def start_time(self) -> Union[datetime, None]:
         """if defined, used to mask data"""
         return self._start_time
 
     @start_time.setter
@@ -1304,21 +1303,21 @@
             >>> ModelOutputReader.path_flow1d = path_to_dir_that_contains_dimr_xml
         """
         if self.file_1D_Q.is_file() & self.file_1D_H.is_file():
             self._data_1D_Q = pd.read_csv(
                 self.file_1D_Q,
                 index_col=0,
                 parse_dates=True,
-                date_parser=self._dateparser,
+                date_format=self._time_fmt,
             )
             self._data_1D_H = pd.read_csv(
                 self.file_1D_H,
                 index_col=0,
                 parse_dates=True,
-                date_parser=self._dateparser,
+                date_format=self._time_fmt,
             )
             self.set_logger_message("Using existing flow1d csv files")
         else:
             self.set_logger_message("Importing from NetCDF")
             self._data_1D_H, self._data_1D_Q = self._import_1Dobservations()
             self.set_logger_message("Writing to CSV (waterlevels)")
             self._data_1D_H.to_csv(self.file_1D_H)
@@ -1335,39 +1334,39 @@
             >>> ModelOutputReader.path_flow2d = path_to_netcdf_file
         """
         if self.file_2D_Q.is_file() & self.file_2D_H.is_file():
             self._data_2D_Q = pd.read_csv(
                 self.file_2D_Q,
                 index_col=0,
                 parse_dates=True,
-                date_parser=self._dateparser,
+                date_format=self._time_fmt,
             )
             self._data_2D_H = pd.read_csv(
                 self.file_2D_H,
                 index_col=0,
                 parse_dates=True,
-                date_parser=self._dateparser,
+                date_format=self._time_fmt,
             )
             self.set_logger_message("Using existing flow2d csv files")
         else:
             # write to file
             self._import_2Dobservations()
 
             # then load
             self._data_2D_Q = pd.read_csv(
                 self.file_2D_Q,
                 index_col=0,
                 parse_dates=True,
-                date_parser=self._dateparser,
+                date_format=self._time_fmt,
             )
             self._data_2D_H = pd.read_csv(
                 self.file_2D_H,
                 index_col=0,
                 parse_dates=True,
-                date_parser=self._dateparser,
+                date_format=self._time_fmt,
             )
 
     def get_1d2d_map(self):
         """Writes a map between stations in 1D and stations in 2D. Matches based on identical characters in first nine slots"""
         if self.file_1D2D_map.is_file():
             self.set_logger_message("using existing 1d-2d map")
             return
@@ -1377,14 +1376,15 @@
     def read_all_data(self) -> None:
         """ """
         self.load_flow1d_data()
         self.get_1d2d_map()
         self.load_flow2d_data()
 
     def _dateparser(self, t):
+        #DEPRECATED
         return datetime.strptime(t, self._time_fmt)
 
     @property
     def output_path(self) -> Path:
         return self._path_out
 
     @output_path.setter
@@ -1436,15 +1436,22 @@
         return self._time_offset_1d
 
     @time_offset_1d.setter
     def time_offset_1d(self, seconds: int = 0):
         self._time_offset_1d = seconds
 
     def _apply_startstop_time(self, data: pd.DataFrame) -> pd.DataFrame:
-        """ Applies stop/start time to data """
+        """ 
+        Applies stop/start time to data 
+        """
+        if self.stop_time is None:
+            self.stop_time = data.index[-1]
+        if self.start_time is None:
+            self.start_time = data.index[0]
+
         if self.start_time >= self.stop_time:
             self.set_logger_message("Stop time ({self.stop_time}) should be later than start time ({self.start_time})", "error")
             raise ValueError
         if bool(self.start_time) and (self.start_time >= data.index[-1]):
             self.set_logger_message(f'Provided start time {self.start_time} is later than last record in data ({data.index[-1]})', 'error')
             raise ValueError
         if bool(self.stop_time) and (self.stop_time <= data.index[0]):
@@ -1601,31 +1608,31 @@
     """
 
     _routes: List[List[str]] = None
 
     def __init__(
         self,
         project: Project,
-        path_1d: Union[Path, str],
-        path_2d: Union[Path, str],
+        path_1d: Union[Path, str] | None,
+        path_2d: Union[Path, str] | None,
         routes: List[List[str]],
         start_time: Union[None, datetime] = None,
         stop_time: Union[None, datetime] = None,
     ):
         if project:
             super().__init__(logger=project.get_logger(), start_time=start_time, stop_time=stop_time)
             self.output_path = project.get_output_directory()
         else:
             super().__init__()
 
-        if isinstance(path_1d, (Path, str)) & Path(path_1d).is_file():
+        if isinstance(path_1d, (Path, str)) and Path(path_1d).is_file():
             self.path_flow1d = path_1d
         else:
             self.set_logger_message(f'1D netCDF file does not exist or is not provided. Input provided: {path_1d}.', 'debug')
-        if isinstance(path_1d, (Path, str)) & Path(path_2d).is_file():
+        if isinstance(path_1d, (Path, str)) and Path(path_2d).is_file():
             self.path_flow2d = path_2d
         else:
             self.set_logger_message(f'2D netCDF file does not exist or is not provided. Input provided: {path_2d}.', 'debug')
 
         self.routes = routes
         self.statistics = None
         self._data_1D_H: pd.DataFrame = None
@@ -1908,15 +1915,24 @@
 
     def _style_error_axes(self, ax, ylim: List[float] = [-0.5, 0.5]):
         ax.set_ylim(ylim)
         ax.spines["right"].set_edgecolor(self._color_error)
         ax.tick_params(axis="y", colors=self._color_error)
         ax.grid(False)
 
-    def _compute_statistics(self):
+    def _compute_statistics(self) -> pd.DataFrame:
+        """
+        Computes statistics for the difference between 1D and 2D water levels
+
+        Returns DataFrame with 
+            columns: rkm, branch, is_lmw, bias, std, mae
+            rows: observation stations
+    
+        """
+
         diff = self.data_1D_H - self.data_2D_H
         station_names = diff.columns
         rkms = self._names_to_rkms(station_names)
         branches = self._names_to_branches(station_names)
 
         stats = pd.DataFrame(data=diff.mean(), columns=["bias"])
         stats["rkm"] = rkms
```

### Comparing `fm2prof-2.2.8/LICENSE.txt` & `fm2prof-2.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fm2prof-2.2.8/LICENSE_HEADER.txt` & `fm2prof-2.3.1/LICENSE_HEADER.txt`

 * *Files identical despite different names*


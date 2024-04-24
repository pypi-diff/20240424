# Comparing `tmp/audian-1.6.tar.gz` & `tmp/audian-1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audian-1.6.tar", last modified: Sat Apr 20 09:37:03 2024, max compression
+gzip compressed data, was "audian-1.7.tar", last modified: Wed Apr 24 10:10:47 2024, max compression
```

## Comparing `audian-1.6.tar` & `audian-1.7.tar`

### file list

```diff
@@ -1,31 +1,30 @@
-drwxrwxr-x   0 benda     (1001) benda     (1001)        0 2024-04-20 09:37:03.470482 audian-1.6/
--rw-rw-r--   0 benda     (1001) benda     (1001)    35141 2022-09-12 08:36:43.000000 audian-1.6/LICENSE
--rw-r--r--   0 benda     (1001) benda     (1001)    46971 2024-04-20 09:37:03.470482 audian-1.6/PKG-INFO
--rw-rw-r--   0 benda     (1001) benda     (1001)     5200 2024-03-13 09:56:03.000000 audian-1.6/README.md
--rw-rw-r--   0 benda     (1001) benda     (1001)     1460 2024-04-20 09:33:52.000000 audian-1.6/pyproject.toml
--rw-rw-r--   0 benda     (1001) benda     (1001)       38 2024-04-20 09:37:03.470482 audian-1.6/setup.cfg
--rw-rw-r--   0 benda     (1001) benda     (1001)       38 2024-04-20 09:33:52.000000 audian-1.6/setup.py
-drwxrwxr-x   0 benda     (1001) benda     (1001)        0 2024-04-20 09:37:03.466482 audian-1.6/src/
-drwxrwxr-x   0 benda     (1001) benda     (1001)        0 2024-04-20 09:37:03.470482 audian-1.6/src/audian/
--rw-rw-r--   0 benda     (1001) benda     (1001)       96 2024-04-20 09:33:52.000000 audian-1.6/src/audian/__init__.py
--rw-rw-r--   0 benda     (1001) benda     (1001)    52259 2024-04-20 09:33:52.000000 audian-1.6/src/audian/audian.py
--rw-rw-r--   0 benda     (1001) benda     (1001)    51241 2024-04-20 09:33:52.000000 audian-1.6/src/audian/audiangui.py
--rw-rw-r--   0 benda     (1001) benda     (1001)    13425 2024-04-20 09:33:52.000000 audian-1.6/src/audian/configfile.py
--rw-rw-r--   0 benda     (1001) benda     (1001)    72633 2024-04-20 09:33:52.000000 audian-1.6/src/audian/databrowser.py
--rw-rw-r--   0 benda     (1001) benda     (1001)     7428 2024-04-20 09:33:52.000000 audian-1.6/src/audian/fulltraceplot.py
--rw-rw-r--   0 benda     (1001) benda     (1001)    17684 2024-04-20 09:33:52.000000 audian-1.6/src/audian/markerdata.py
--rw-rw-r--   0 benda     (1001) benda     (1001)     3470 2024-04-20 09:33:52.000000 audian-1.6/src/audian/oscillogramplot.py
--rw-rw-r--   0 benda     (1001) benda     (1001)     4279 2024-04-20 09:33:52.000000 audian-1.6/src/audian/selectviewbox.py
--rw-rw-r--   0 benda     (1001) benda     (1001)     6835 2024-04-20 09:33:52.000000 audian-1.6/src/audian/specitem.py
--rw-rw-r--   0 benda     (1001) benda     (1001)     5566 2024-04-20 09:33:52.000000 audian-1.6/src/audian/spectrumplot.py
--rw-rw-r--   0 benda     (1001) benda     (1001)     4036 2024-04-20 09:33:52.000000 audian-1.6/src/audian/timeaxisitem.py
--rw-rw-r--   0 benda     (1001) benda     (1001)     6993 2024-04-20 09:33:52.000000 audian-1.6/src/audian/traceitem.py
--rw-rw-r--   0 benda     (1001) benda     (1001)      199 2024-04-20 09:33:52.000000 audian-1.6/src/audian/version.py
--rw-rw-r--   0 benda     (1001) benda     (1001)     1209 2024-04-20 09:33:52.000000 audian-1.6/src/audian/yaxisitem.py
-drwxrwxr-x   0 benda     (1001) benda     (1001)        0 2024-04-20 09:37:03.470482 audian-1.6/src/audian.egg-info/
--rw-r--r--   0 benda     (1001) benda     (1001)    46971 2024-04-20 09:37:03.000000 audian-1.6/src/audian.egg-info/PKG-INFO
--rw-rw-r--   0 benda     (1001) benda     (1001)      624 2024-04-20 09:37:03.000000 audian-1.6/src/audian.egg-info/SOURCES.txt
--rw-rw-r--   0 benda     (1001) benda     (1001)        1 2024-04-20 09:37:03.000000 audian-1.6/src/audian.egg-info/dependency_links.txt
--rw-rw-r--   0 benda     (1001) benda     (1001)       78 2024-04-20 09:37:03.000000 audian-1.6/src/audian.egg-info/entry_points.txt
--rw-rw-r--   0 benda     (1001) benda     (1001)       65 2024-04-20 09:37:03.000000 audian-1.6/src/audian.egg-info/requires.txt
--rw-rw-r--   0 benda     (1001) benda     (1001)        7 2024-04-20 09:37:03.000000 audian-1.6/src/audian.egg-info/top_level.txt
+drwxrwxr-x   0 benda     (1001) benda     (1001)        0 2024-04-24 10:10:47.390179 audian-1.7/
+-rw-rw-r--   0 benda     (1001) benda     (1001)    35141 2022-09-12 08:36:43.000000 audian-1.7/LICENSE
+-rw-r--r--   0 benda     (1001) benda     (1001)    47100 2024-04-24 10:10:47.390179 audian-1.7/PKG-INFO
+-rw-rw-r--   0 benda     (1001) benda     (1001)     5331 2024-04-24 10:09:05.000000 audian-1.7/README.md
+-rw-rw-r--   0 benda     (1001) benda     (1001)     1458 2024-04-24 10:08:09.000000 audian-1.7/pyproject.toml
+-rw-rw-r--   0 benda     (1001) benda     (1001)       38 2024-04-24 10:10:47.390179 audian-1.7/setup.cfg
+drwxrwxr-x   0 benda     (1001) benda     (1001)        0 2024-04-24 10:10:47.386179 audian-1.7/src/
+drwxrwxr-x   0 benda     (1001) benda     (1001)        0 2024-04-24 10:10:47.386179 audian-1.7/src/audian/
+-rw-rw-r--   0 benda     (1001) benda     (1001)       96 2024-04-20 09:33:52.000000 audian-1.7/src/audian/__init__.py
+-rw-rw-r--   0 benda     (1001) benda     (1001)    52221 2024-04-24 10:08:09.000000 audian-1.7/src/audian/audian.py
+-rw-rw-r--   0 benda     (1001) benda     (1001)    51241 2024-04-20 09:33:52.000000 audian-1.7/src/audian/audiangui.py
+-rw-rw-r--   0 benda     (1001) benda     (1001)    13425 2024-04-20 09:33:52.000000 audian-1.7/src/audian/configfile.py
+-rw-rw-r--   0 benda     (1001) benda     (1001)    72631 2024-04-24 10:08:09.000000 audian-1.7/src/audian/databrowser.py
+-rw-rw-r--   0 benda     (1001) benda     (1001)     7428 2024-04-20 09:33:52.000000 audian-1.7/src/audian/fulltraceplot.py
+-rw-rw-r--   0 benda     (1001) benda     (1001)    17684 2024-04-20 09:33:52.000000 audian-1.7/src/audian/markerdata.py
+-rw-rw-r--   0 benda     (1001) benda     (1001)     3470 2024-04-20 09:33:52.000000 audian-1.7/src/audian/oscillogramplot.py
+-rw-rw-r--   0 benda     (1001) benda     (1001)     4279 2024-04-20 09:33:52.000000 audian-1.7/src/audian/selectviewbox.py
+-rw-rw-r--   0 benda     (1001) benda     (1001)     6835 2024-04-20 09:33:52.000000 audian-1.7/src/audian/specitem.py
+-rw-rw-r--   0 benda     (1001) benda     (1001)     5566 2024-04-20 09:33:52.000000 audian-1.7/src/audian/spectrumplot.py
+-rw-rw-r--   0 benda     (1001) benda     (1001)     4036 2024-04-20 09:33:52.000000 audian-1.7/src/audian/timeaxisitem.py
+-rw-rw-r--   0 benda     (1001) benda     (1001)     6993 2024-04-20 09:33:52.000000 audian-1.7/src/audian/traceitem.py
+-rw-rw-r--   0 benda     (1001) benda     (1001)      199 2024-04-24 10:09:59.000000 audian-1.7/src/audian/version.py
+-rw-rw-r--   0 benda     (1001) benda     (1001)     1209 2024-04-20 09:33:52.000000 audian-1.7/src/audian/yaxisitem.py
+drwxrwxr-x   0 benda     (1001) benda     (1001)        0 2024-04-24 10:10:47.386179 audian-1.7/src/audian.egg-info/
+-rw-r--r--   0 benda     (1001) benda     (1001)    47100 2024-04-24 10:10:47.000000 audian-1.7/src/audian.egg-info/PKG-INFO
+-rw-rw-r--   0 benda     (1001) benda     (1001)      615 2024-04-24 10:10:47.000000 audian-1.7/src/audian.egg-info/SOURCES.txt
+-rw-rw-r--   0 benda     (1001) benda     (1001)        1 2024-04-24 10:10:47.000000 audian-1.7/src/audian.egg-info/dependency_links.txt
+-rw-rw-r--   0 benda     (1001) benda     (1001)       78 2024-04-24 10:10:47.000000 audian-1.7/src/audian.egg-info/entry_points.txt
+-rw-rw-r--   0 benda     (1001) benda     (1001)       63 2024-04-24 10:10:47.000000 audian-1.7/src/audian.egg-info/requires.txt
+-rw-rw-r--   0 benda     (1001) benda     (1001)        7 2024-04-24 10:10:47.000000 audian-1.7/src/audian.egg-info/top_level.txt
```

### Comparing `audian-1.6/LICENSE` & `audian-1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `audian-1.6/PKG-INFO` & `audian-1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audian
-Version: 1.6
+Version: 1.7
 Summary: GUI for viewing and analyzing recordings of animal vocalizations.
 Author-email: Jan Benda <jan.benda@uni-tuebingen.de>
 Maintainer-email: Jan Benda <jan.benda@uni-tuebingen.de>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
@@ -699,15 +699,15 @@
 Requires-Dist: scipy
 Requires-Dist: numpy
 Requires-Dist: numba
 Requires-Dist: pandas
 Requires-Dist: matplotlib
 Requires-Dist: PyQt5
 Requires-Dist: pyqtgraph
-Requires-Dist: audioio>=2.1
+Requires-Dist: thunderlab
 
 [![PyPI license](https://img.shields.io/pypi/l/audian.svg)](https://pypi.python.org/pypi/audian/)
 [![PyPI version](https://badge.fury.io/py/audian.svg)](https://badge.fury.io/py/audian)
 
 # audian - AUDIoANalyzer
 
 Python-based GUI for viewing and analyzing recordings of animal
@@ -839,14 +839,18 @@
 ## Installation
 
 Simply run (as superuser):
 ```
 pip install audian
 ```
 
+This should also install:
+- [ThunderLab](https://github.com/bendalab/thunderlab)
+- [AudioIO](https://github.com/bendalab/audioio)
+
 
 ## Options
 
 Output of `audian --help`:
 
 ``` txt
 usage: audian [-h] [--version] [-v] [-c [cfgfile]] [-f FREQ] [-l FREQ] [file] [channel]
```

### Comparing `audian-1.6/README.md` & `audian-1.7/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -132,14 +132,18 @@
 ## Installation
 
 Simply run (as superuser):
 ```
 pip install audian
 ```
 
+This should also install:
+- [ThunderLab](https://github.com/bendalab/thunderlab)
+- [AudioIO](https://github.com/bendalab/audioio)
+
 
 ## Options
 
 Output of `audian --help`:
 
 ``` txt
 usage: audian [-h] [--version] [-v] [-c [cfgfile]] [-f FREQ] [-l FREQ] [file] [channel]
```

### Comparing `audian-1.6/pyproject.toml` & `audian-1.7/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -9,15 +9,15 @@
   "scipy",
   "numpy",
   "numba",
   "pandas",
   "matplotlib",
   "PyQt5",
   "pyqtgraph",
-  "audioio>=2.1"
+  "thunderlab"
 ]
 requires-python = ">=3.4"
 authors = [
   {name = "Jan Benda", email = "jan.benda@uni-tuebingen.de"},
 ]
 maintainers = [
   {name = "Jan Benda", email = "jan.benda@uni-tuebingen.de"},
```

### Comparing `audian-1.6/src/audian/audian.py` & `audian-1.7/src/audian/audian.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 import argparse
 import numpy as np
 import matplotlib.pyplot as plt
 import matplotlib.mlab as ml
 import matplotlib.colors as mc
 import matplotlib.widgets as widgets
 import scipy.signal as sig
-from collections import OrderedDict
 from audioio import load_audio, write_audio, PlayAudio, fade
 from .version import __version__, __year__
 from .configfile import ConfigFile
 
     
 cfg = ConfigFile()
 
@@ -68,15 +67,15 @@
 
 ###############################################################################
 ## peak detection:
 
 def detect_peaks_fixed(data, threshold):
     """Detect peaks and troughs using a fixed, relative threshold.
 
-    From https://github.com/bendalab/thunderfish/blob/master/thunderfish/eventdetection.py
+    From https://github.com/bendalab/thunderlab/blob/master/thunderlab/eventdetection.py
 
     Parameters
     ----------
     data: array
         An 1-D array of input data where peaks are detected.
     threshold: float
         A positive number setting the detection threshold,
```

### Comparing `audian-1.6/src/audian/audiangui.py` & `audian-1.7/src/audian/audiangui.py`

 * *Files identical despite different names*

### Comparing `audian-1.6/src/audian/configfile.py` & `audian-1.7/src/audian/configfile.py`

 * *Files identical despite different names*

### Comparing `audian-1.6/src/audian/databrowser.py` & `audian-1.7/src/audian/databrowser.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,16 +17,16 @@
 from PyQt5.QtWidgets import QLabel, QSizePolicy, QTableView
 from PyQt5.QtWidgets import QDialog, QDialogButtonBox, QFileDialog
 from PyQt5.QtWidgets import QAbstractItemView, QGraphicsRectItem
 import pyqtgraph as pg
 from audioio import fade
 from audioio import get_datetime, update_starttime
 from audioio import bext_history_str, add_history
-from thunderfish.dataloader import DataLoader
-from thunderfish.datawriter import available_formats, write_data
+from thunderlab.dataloader import DataLoader
+from thunderlab.datawriter import available_formats, write_data
 from .version import __version__, __year__
 from .fulltraceplot import FullTracePlot, secs_to_str
 from .oscillogramplot import OscillogramPlot
 from .spectrumplot import SpectrumPlot
 from .traceitem import TraceItem
 from .specitem import SpecItem
 from .markerdata import colors, MarkerLabel, MarkerLabelsModel
```

### Comparing `audian-1.6/src/audian/fulltraceplot.py` & `audian-1.7/src/audian/fulltraceplot.py`

 * *Files identical despite different names*

### Comparing `audian-1.6/src/audian/markerdata.py` & `audian-1.7/src/audian/markerdata.py`

 * *Files identical despite different names*

### Comparing `audian-1.6/src/audian/oscillogramplot.py` & `audian-1.7/src/audian/oscillogramplot.py`

 * *Files identical despite different names*

### Comparing `audian-1.6/src/audian/selectviewbox.py` & `audian-1.7/src/audian/selectviewbox.py`

 * *Files identical despite different names*

### Comparing `audian-1.6/src/audian/specitem.py` & `audian-1.7/src/audian/specitem.py`

 * *Files identical despite different names*

### Comparing `audian-1.6/src/audian/spectrumplot.py` & `audian-1.7/src/audian/spectrumplot.py`

 * *Files identical despite different names*

### Comparing `audian-1.6/src/audian/timeaxisitem.py` & `audian-1.7/src/audian/timeaxisitem.py`

 * *Files identical despite different names*

### Comparing `audian-1.6/src/audian/traceitem.py` & `audian-1.7/src/audian/traceitem.py`

 * *Files identical despite different names*

### Comparing `audian-1.6/src/audian/yaxisitem.py` & `audian-1.7/src/audian/yaxisitem.py`

 * *Files identical despite different names*

### Comparing `audian-1.6/src/audian.egg-info/PKG-INFO` & `audian-1.7/src/audian.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audian
-Version: 1.6
+Version: 1.7
 Summary: GUI for viewing and analyzing recordings of animal vocalizations.
 Author-email: Jan Benda <jan.benda@uni-tuebingen.de>
 Maintainer-email: Jan Benda <jan.benda@uni-tuebingen.de>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
@@ -699,15 +699,15 @@
 Requires-Dist: scipy
 Requires-Dist: numpy
 Requires-Dist: numba
 Requires-Dist: pandas
 Requires-Dist: matplotlib
 Requires-Dist: PyQt5
 Requires-Dist: pyqtgraph
-Requires-Dist: audioio>=2.1
+Requires-Dist: thunderlab
 
 [![PyPI license](https://img.shields.io/pypi/l/audian.svg)](https://pypi.python.org/pypi/audian/)
 [![PyPI version](https://badge.fury.io/py/audian.svg)](https://badge.fury.io/py/audian)
 
 # audian - AUDIoANalyzer
 
 Python-based GUI for viewing and analyzing recordings of animal
@@ -839,14 +839,18 @@
 ## Installation
 
 Simply run (as superuser):
 ```
 pip install audian
 ```
 
+This should also install:
+- [ThunderLab](https://github.com/bendalab/thunderlab)
+- [AudioIO](https://github.com/bendalab/audioio)
+
 
 ## Options
 
 Output of `audian --help`:
 
 ``` txt
 usage: audian [-h] [--version] [-v] [-c [cfgfile]] [-f FREQ] [-l FREQ] [file] [channel]
```

### Comparing `audian-1.6/src/audian.egg-info/SOURCES.txt` & `audian-1.7/src/audian.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 LICENSE
 README.md
 pyproject.toml
-setup.py
 src/audian/__init__.py
 src/audian/audian.py
 src/audian/audiangui.py
 src/audian/configfile.py
 src/audian/databrowser.py
 src/audian/fulltraceplot.py
 src/audian/markerdata.py
```


# Comparing `tmp/imaging-research-0.0.9.tar.gz` & `tmp/imaging_research-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imaging-research-0.0.9.tar", last modified: Wed Mar 13 23:06:09 2024, max compression
+gzip compressed data, was "imaging_research-0.1.0.tar", last modified: Wed Apr 24 15:43:18 2024, max compression
```

## Comparing `imaging-research-0.0.9.tar` & `imaging_research-0.1.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 fraser    (1000) fraser    (1000)        0 2024-03-13 23:06:09.012356 imaging-research-0.0.9/
--rw-rw-r--   0 fraser    (1000) fraser    (1000)    35149 2023-07-21 12:13:15.000000 imaging-research-0.0.9/LICENSE
--rw-r--r--   0 fraser    (1000) fraser    (1000)     3705 2024-03-13 23:06:09.008356 imaging-research-0.0.9/PKG-INFO
--rw-rw-r--   0 fraser    (1000) fraser    (1000)     2900 2024-03-13 14:30:47.000000 imaging-research-0.0.9/README.md
-drwxrwxr-x   0 fraser    (1000) fraser    (1000)        0 2024-03-13 23:06:09.008356 imaging-research-0.0.9/imaging_research.egg-info/
--rw-r--r--   0 fraser    (1000) fraser    (1000)     3705 2024-03-13 23:06:09.000000 imaging-research-0.0.9/imaging_research.egg-info/PKG-INFO
--rw-rw-r--   0 fraser    (1000) fraser    (1000)      454 2024-03-13 23:06:09.000000 imaging-research-0.0.9/imaging_research.egg-info/SOURCES.txt
--rw-rw-r--   0 fraser    (1000) fraser    (1000)        1 2024-03-13 23:06:09.000000 imaging-research-0.0.9/imaging_research.egg-info/dependency_links.txt
--rw-rw-r--   0 fraser    (1000) fraser    (1000)       63 2024-03-13 23:06:09.000000 imaging-research-0.0.9/imaging_research.egg-info/entry_points.txt
--rw-rw-r--   0 fraser    (1000) fraser    (1000)       31 2024-03-13 23:06:09.000000 imaging-research-0.0.9/imaging_research.egg-info/requires.txt
--rw-rw-r--   0 fraser    (1000) fraser    (1000)       11 2024-03-13 23:06:09.000000 imaging-research-0.0.9/imaging_research.egg-info/top_level.txt
-drwxrwxr-x   0 fraser    (1000) fraser    (1000)        0 2024-03-13 23:06:09.008356 imaging-research-0.0.9/miresearch/
--rw-rw-r--   0 fraser    (1000) fraser    (1000)        0 2023-07-21 12:13:15.000000 imaging-research-0.0.9/miresearch/__init__.py
--rw-rw-r--   0 fraser    (1000) fraser    (1000)     3745 2024-03-13 14:30:47.000000 imaging-research-0.0.9/miresearch/mi_config.py
--rw-rw-r--   0 fraser    (1000) fraser    (1000)    41468 2024-03-13 22:58:21.000000 imaging-research-0.0.9/miresearch/mi_subject.py
--rw-rw-r--   0 fraser    (1000) fraser    (1000)    11245 2024-03-13 14:30:47.000000 imaging-research-0.0.9/miresearch/mi_utils.py
--rw-rw-r--   0 fraser    (1000) fraser    (1000)      408 2024-03-13 14:30:47.000000 imaging-research-0.0.9/miresearch/miresearch.conf
--rw-rw-r--   0 fraser    (1000) fraser    (1000)     4312 2024-03-13 14:30:47.000000 imaging-research-0.0.9/miresearch/miresearch_main.py
--rw-rw-r--   0 fraser    (1000) fraser    (1000)     6298 2024-02-27 11:00:41.000000 imaging-research-0.0.9/miresearch/miresearch_watchdog.py
--rw-rw-r--   0 fraser    (1000) fraser    (1000)       38 2024-03-13 23:06:09.012356 imaging-research-0.0.9/setup.cfg
--rw-rw-r--   0 fraser    (1000) fraser    (1000)     3555 2024-03-13 23:04:56.000000 imaging-research-0.0.9/setup.py
+drwxrwxr-x   0 fraser    (1000) fraser    (1000)        0 2024-04-24 15:43:18.269956 imaging_research-0.1.0/
+-rw-rw-r--   0 fraser    (1000) fraser    (1000)    35149 2023-07-21 12:13:15.000000 imaging_research-0.1.0/LICENSE
+-rw-r--r--   0 fraser    (1000) fraser    (1000)     5363 2024-04-24 15:43:18.269956 imaging_research-0.1.0/PKG-INFO
+-rw-rw-r--   0 fraser    (1000) fraser    (1000)     4558 2024-04-24 15:41:49.000000 imaging_research-0.1.0/README.md
+drwxrwxr-x   0 fraser    (1000) fraser    (1000)        0 2024-04-24 15:43:18.269956 imaging_research-0.1.0/imaging_research.egg-info/
+-rw-r--r--   0 fraser    (1000) fraser    (1000)     5363 2024-04-24 15:43:18.000000 imaging_research-0.1.0/imaging_research.egg-info/PKG-INFO
+-rw-rw-r--   0 fraser    (1000) fraser    (1000)      454 2024-04-24 15:43:18.000000 imaging_research-0.1.0/imaging_research.egg-info/SOURCES.txt
+-rw-rw-r--   0 fraser    (1000) fraser    (1000)        1 2024-04-24 15:43:18.000000 imaging_research-0.1.0/imaging_research.egg-info/dependency_links.txt
+-rw-rw-r--   0 fraser    (1000) fraser    (1000)       63 2024-04-24 15:43:18.000000 imaging_research-0.1.0/imaging_research.egg-info/entry_points.txt
+-rw-rw-r--   0 fraser    (1000) fraser    (1000)       31 2024-04-24 15:43:18.000000 imaging_research-0.1.0/imaging_research.egg-info/requires.txt
+-rw-rw-r--   0 fraser    (1000) fraser    (1000)       11 2024-04-24 15:43:18.000000 imaging_research-0.1.0/imaging_research.egg-info/top_level.txt
+drwxrwxr-x   0 fraser    (1000) fraser    (1000)        0 2024-04-24 15:43:18.269956 imaging_research-0.1.0/miresearch/
+-rw-rw-r--   0 fraser    (1000) fraser    (1000)        0 2023-07-21 12:13:15.000000 imaging_research-0.1.0/miresearch/__init__.py
+-rw-rw-r--   0 fraser    (1000) fraser    (1000)     4002 2024-04-24 15:29:19.000000 imaging_research-0.1.0/miresearch/mi_config.py
+-rw-rw-r--   0 fraser    (1000) fraser    (1000)    45869 2024-04-24 15:29:19.000000 imaging_research-0.1.0/miresearch/mi_subject.py
+-rw-rw-r--   0 fraser    (1000) fraser    (1000)     7311 2024-03-24 21:22:35.000000 imaging_research-0.1.0/miresearch/mi_utils.py
+-rw-rw-r--   0 fraser    (1000) fraser    (1000)      428 2024-04-24 15:29:19.000000 imaging_research-0.1.0/miresearch/miresearch.conf
+-rw-rw-r--   0 fraser    (1000) fraser    (1000)     8504 2024-03-25 08:57:05.000000 imaging_research-0.1.0/miresearch/miresearch_main.py
+-rw-rw-r--   0 fraser    (1000) fraser    (1000)    10833 2024-04-24 15:33:57.000000 imaging_research-0.1.0/miresearch/miresearch_watchdog.py
+-rw-rw-r--   0 fraser    (1000) fraser    (1000)       38 2024-04-24 15:43:18.269956 imaging_research-0.1.0/setup.cfg
+-rw-rw-r--   0 fraser    (1000) fraser    (1000)     3555 2024-04-24 15:36:09.000000 imaging_research-0.1.0/setup.py
```

### Comparing `imaging-research-0.0.9/LICENSE` & `imaging_research-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `imaging-research-0.0.9/PKG-INFO` & `imaging_research-0.1.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,76 +1,81 @@
-Metadata-Version: 2.1
-Name: imaging-research
-Version: 0.0.9
-Summary: Medical Imaginging Research structuring and automation
-Home-page: https://github.com/fraser29/miresearch
-Author: Fraser M. Callaghan
-Author-email: callaghan.fm@gmail.com
-License: MIT
-Keywords: medical,imaging,mri,ct,dicom
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.9.0
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: spydcmtk
-Requires-Dist: pandas
-Requires-Dist: numpy
-Requires-Dist: watchdog
-
-
 # miresearch
 Organisation and automation tools for medical imaging research data
 
 ## Installation: 
 
 ```bash
 pip install imaging-research
 ```
 Note: pypi reported naming conflicts for miresearch
 
+> [!IMPORTANT]  
+> This package is currently undergoing frequent development and testing. Please check back regularly for version updates.
+
 ## About
 
 This is a collection of classes for following OOP principles for organisation of research data for medical imaging research studies. 
 
 It takes advantage of the dicom standard and the package [spydcmtk](https://github.com/fraser29/spydcmtk) for automating and generalising many typical steps with the intention of making the researcher's life easier. 
 
 This package may be easily adapted and expanded upon for a high level control over your research data. Or, it may be used as is for basic structure and organisation of data and automation of common tasks. 
 
+> [!NOTE]  
+> Version 0.1.0 release: Greater flexibility in subject ID naming and stability improvements to miresearch_watchdog.
+
+
 ## Class structure
 
 **AbstractSubject**  class is top level class taking inputs:
 - *subjectNumber* : an integer
 - *dataRoot* : the root directory where subjects to be stored             
 - *subjectPrefix* : a prefix to be combined with *subjectNumber* for naming each subject
     - Optional: will be guessed from subjects already present in *dataRoot* if not given. 
 - *DIRECTORY_STRUCTURE_TREE* : DirectoryStructureTree class to define directory structure for each subject directory (see wiki for construction shortcuts)
     - Optional: Defaults to **RAW** and **META** directories. 
 
-This is the basic parent class containing fundamental methods for organisation and management. See [wiki](https://github.com/fraser29/miresearch/wiki) for advanced usage, epsecially via inheritance and polymorphism. 
+This is the basic parent class containing fundamental methods for organisation and management. See  [miresearch docs](https://fraser29.github.io/miresearch/) for advanced usage, epsecially via inheritance and polymorphism. 
 
 # Exposed commandline tool: miresearch
 
 ```bash
 
 miresearch -h
-usage:  ... 
+usage: miresearch [-h] [-config CONFIGFILE] [-FORCE] [-QUIET] [-INFO] [-DEBUG] [-s [SUBJNLIST ...]] [-sf SUBJNLISTFILE] [-sR SUBJRANGE SUBJRANGE] [-y DATAROOT] [-sPrefix SUBJPREFIX] [-anonName ANONNAME]CODE
+                  [-Load LOADPATH] [-LOAD_MULTI] [-LOAD_MULTI_FORCE] [-RunPost] [-SubjInfo] [-SummaryCSV SUMMARYCSV] [-WatchDirectory WATCHDIRECTORY]
+
+options:
+  -h, --help            show this help message and exit
+
+Management Parameters:
+  -config CONFIGFILE    Path to configuration file to use.
+  -FORCE                force action - use with caution
+  -QUIET                Suppress progress bars and logging to terminal
+  -INFO                 Provide setup (configuration) info and exit.
+  -DEBUG                Run in DEBUG mode (save intermediate steps, increase log output)
+
+Subject Definition:
+  -s [SUBJNLIST ...]    Subject number
+  -sf SUBJNLISTFILE     Subject numbers in file
+  -sR SUBJRANGE SUBJRANGE
+                        Subject range
+  -y DATAROOT           Path of root data directory (where subjects are stored) [default None -> may be set in config file]
+  -sPrefix SUBJPREFIX   Subject prefix [default None -> will get from config file OR dataRoot]
+  -anonName ANONNAME    Set to anonymise newly loaded subject. Set to true to use for WatchDirectory. [default None]
 
 Actions:
   -Load LOADPATH        Path to load dicoms from (file / directory / tar / tar.gz / zip)
   -LOAD_MULTI           Combine with "Load": Load new subject for each subdirectory under loadPath
   -LOAD_MULTI_FORCE     Combine with "Load": Force to ignore studyUIDs and load new ID per subdirectory
-  -WatchDirectory WATCHDIRECTORY
-                        Will watch given directory for new data and load as new study
+  -RunPost              Run post load pipeline
+  -SubjInfo             Print info for each subject
   -SummaryCSV SUMMARYCSV
                         Write summary CSV file (give output file name)
+  -WatchDirectory WATCHDIRECTORY
+                        Will watch given directory for new data and load as new study
 
 ```
 
 # Configuration
 
 miresearch uses a miresearch.conf file for configuration. 
 
@@ -86,8 +91,8 @@
 Files are read in the above order with each subsequent variable present overwritting any previously defined. 
 For information on files found and variables used run:
 
 `miresearch -INFO` 
 
 # Documentation
 
-For full documentation see [read-the-docs](https://miresearch.readthedocs.io/en/latest/#)
+For full documentation see [miresearch docs](https://fraser29.github.io/miresearch/)
```

### Comparing `imaging-research-0.0.9/miresearch/mi_config.py` & `imaging_research-0.1.0/miresearch/mi_config.py`

 * *Files 9% similar despite different names*

```diff
@@ -33,21 +33,25 @@
         self.config.read(self.all_config_files)
 
         self.DEBUG = self.config.getboolean("app", "debug", fallback=False)
         self._anon_level = self.config.get("app", "anon_level", fallback='NONE')
         self._data_root_dir = self.config.get("app", "data_root_dir", fallback="")
         self._subject_prefix = self.config.get("app", "subject_prefix", fallback="")
         self.stable_directory_age_sec = self.config.getint("app", "stable_directory_age_sec", fallback=60)
+        self.default_pad_zeros = self.config.getint("app", "default_pad_zeros", fallback=6)
         self.directory_structure = json.loads(self.config.get("app", "directories"))
 
         self.class_obj = None
         class_path = self.config.get("app", "class_path", fallback=None)
         if class_path:
             module_name, class_name = class_path.rsplit('.', 1)
-            module = importlib.import_module(module_name)
+            try:
+                module = importlib.import_module(module_name)
+            except ModuleNotFoundError as e:
+                raise ModuleNotFoundError(f"*** is {module_name} found in PYTHONPATH? ***") from e
             self.class_obj = getattr(module, class_name)
 
         ## All parameters: 
         self.params = {}
         for section in self.config.sections():
             if section.lower() == 'parameters':
                 self.params[section] = {}
```

### Comparing `imaging-research-0.0.9/miresearch/mi_subject.py` & `imaging_research-0.1.0/miresearch/mi_subject.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,62 +9,77 @@
 Adapted for general use from KMR project. 
 
 
 """
 
 
 import os
+import re
 from zipfile import ZipFile
 import numpy as np
 import datetime
 import pandas as pd
+import shutil
 import logging
 ##
 from spydcmtk import spydcm
 from miresearch import mi_utils
 
 # ====================================================================================================
 # ====================================================================================================
 
-
 # ====================================================================================================
 #       ABSTRACT SUBJECT CLASS
 # ====================================================================================================
 class AbstractSubject(object):
     """
     An abstract subject controlling most basic structure
     """
     def __init__(self, subjectNumber, 
                         dataRoot, 
                         subjectPrefix=None,
-                        DIRECTORY_STRUCTURE_TREE=mi_utils.buildDirectoryStructureTree()) -> None:
-        if (subjectNumber is None) and (subjectPrefix is None):
-            raise ValueError(f"Give subjectNumber (as int) or subjectPrefix as subjID")
-        try:
-            self.subjN = int(subjectNumber)
-        except ValueError:
-            tSubjPrefix, self.subjN = splitSubjID(subjectNumber)
-            if subjectPrefix is not None:
-                if subjectPrefix != tSubjPrefix:
-                    raise mi_utils.SubjPrefixError("Subject prefix passed does not match subjectID passed")
-            else:
-                subjectPrefix = tSubjPrefix
-        except TypeError: # subjectNumber passed as None - so use subjectPrefix as subjID (already check subjectPrefix not None)
-            self.subjN = None
+                        DIRECTORY_STRUCTURE_TREE=mi_utils.buildDirectoryStructureTree(),
+                        padZeros=mi_utils.MIResearch_config.default_pad_zeros,
+                        suffix="") -> None:
+        # -- CHECK REQUIRED INPUT --
+        if subjectNumber is None:
+            raise ValueError(f"Give subjectNumber (as int) or as subjID")
         self.dataRoot = dataRoot
-        if subjectPrefix is None:
-            self.subjectPrefix = guessSubjectPrefix(self.dataRoot)
-        else:
+        self._subjID = None
+        if not os.path.isdir(self.dataRoot):
+            raise ValueError(f"'dataRoot' must be a directory and must exist: Not found: {self.dataRoot}")
+        # -- PROCESS INPUT ##
+        # A) subjectNumber is an int
+        try:
+            self._subjN = int(subjectNumber)
+            if subjectPrefix is None:
+                # not given - guess from others in dataRoot
+                subjectPrefix = guessSubjectPrefix(self.dataRoot) # will raise mi_utils.SubjPrefixError if not obvious
             self.subjectPrefix = subjectPrefix
+        except ValueError: # fail on int 
+            # B) subjectNumber not an int - then treat as subjectID
+            #       first check if can split to prefix, N, suffix
+            try:
+                prefix_N_suffix = splitSubjID(subjectNumber)
+                self.subjectPrefix = prefix_N_suffix[0]
+                self._subjN = prefix_N_suffix[1]
+                if len(prefix_N_suffix) == 3:
+                    suffix = prefix_N_suffix[2]
+            except IndexError: 
+                self._subjID = subjectNumber
+
+        self.suffix = suffix
+        self.padZeros = padZeros
         self.DIRECTORY_STRUCTURE_TREE = DIRECTORY_STRUCTURE_TREE
         self.BUILD_DIR_IF_NEED = True
         self.dicomMetaTagList = mi_utils.DEFAULT_DICOM_META_TAG_LIST
         self.QUIET = False
         #
         self._logger = None
+        self._loggerFH = None
 
 
     ### ----------------------------------------------------------------------------------------------------------------
     ### Class Methods
     ### ----------------------------------------------------------------------------------------------------------------
 
     ### ----------------------------------------------------------------------------------------------------------------
@@ -90,32 +105,50 @@
         return f"{self.subjID} at {self.dataRoot}"
 
     ### ----------------------------------------------------------------------------------------------------------------
     ### Properties
     ### ----------------------------------------------------------------------------------------------------------------
     @property
     def subjID(self):
-        return buildSubjectID(self.subjN, self.subjectPrefix)
+        if self._subjID is not None:
+            return self._subjID
+        return buildSubjectID(self._subjN, self.subjectPrefix, padZeros=self.padZeros, suffix=self.suffix)
 
+    @property
+    def subjN(self):
+        return splitSubjID(self.subjID)[1]
     ### ----------------------------------------------------------------------------------------------------------------
     ### Logging
     ### ----------------------------------------------------------------------------------------------------------------
     @property
     def logger(self):
         if self._logger is None:
             rr = os.path.split(self.dataRoot)[1]
             self._logger = logging.getLogger(f"{rr}/{self.subjID}")
             self._logger.setLevel(logging.INFO)
-            fh = logging.FileHandler(os.path.join(self.getMetaDir(), f'{self.subjID}.log'))
-            fh.setFormatter(logging.Formatter('%(asctime)s | %(levelname)-7s | %(name)s | %(message)s', datefmt='%d-%b-%y %H:%M:%S'))
-            self._logger.addHandler(fh)
+            self._loggerFH = logging.FileHandler(self.logfileName)
+            self._loggerFH.setFormatter(logging.Formatter('%(asctime)s | %(levelname)-7s | %(name)s | %(message)s', datefmt='%d-%b-%y %H:%M:%S'))
+            self._logger.addHandler(self._loggerFH)
             if not self.QUIET:
                 self._logger.addHandler(logging.StreamHandler())
         return self._logger
 
+    @property
+    def logfileName(self):
+        return os.path.join(self.getMetaDir(), f'{self.subjID}.log')
+
+    def _renameLogger(self):
+        """Rename the logger - is run from method renameSubjID
+        """
+        self._loggerFH.close()
+        self.logger.removeHandler(self._loggerFH)
+        self._loggerFH = None
+        self._loggerFH = logging.FileHandler(self.logfileName, mode='a')
+        self._loggerFH.setFormatter(logging.Formatter('%(asctime)s | %(levelname)-7s | %(name)s | %(message)s', datefmt='%d-%b-%y %H:%M:%S'))
+        self._logger.addHandler(self._loggerFH)
 
     ### ----------------------------------------------------------------------------------------------------------------
     ### Methods
     ### ----------------------------------------------------------------------------------------------------------------
     def initDirectoryStructure(self):
         if os.path.isdir(self.getTopDir()):
             self.logger.info(f"Study participant {self.subjID} exists at {self.getTopDir()}. Updating directory structure")
@@ -195,22 +228,30 @@
     
     def getDicomsDir(self):
         dirName = self._getDir([mi_utils.RAW, mi_utils.DICOM])
         return dirName
     
     def renameSubjID(self, newSubjID):
         oldID = self.subjID
+        if newSubjID == oldID:
+            self.logger.error(f"Can not rename from {oldID} to {newSubjID}")
+            return
         self.logger.warning(f"Changing subjID from {oldID} to {newSubjID}")
         self.logger.warning(" *** THIS WILL LIKELY HAVE BREAKING CONSEQUENCES ***")
-        os.rename(self.getTopDir(), os.path.join(self.dataRoot, newSubjID))
+        newName = os.path.join(self.dataRoot, newSubjID)
+        if os.path.isdir(newName):
+            shutil.rmtree(newName)
+        os.rename(self.getTopDir(), newName)
         self.subjectPrefix = newSubjID
-        self.subjN = None
-        self._logger = None
+        self._subjN = None
+        self._renameLogger()
         self.logger.warning(f"New logger after subjID changed from {oldID} to {self.subjID}")
-        self.logger.warning(" *** THIS WILL LIKELY HAVE BREAKING CONSEQUENCES ***")
+        self.logger.warning(" *** THIS WILL LIKELY HAVE BREAKING CONSEQUENCES ***")        
+        self.buildDicomMeta()
+        self.buildSeriesDataMetaCSV(FORCE=True)
 
     ### META STUFF -----------------------------------------------------------------------------------------------------
     def getSeriesMetaCSV(self):
         return os.path.join(self.getMetaDir(), 'ScanSeriesInfo.csv')
 
     def getSeriesMetaAsDataFrame(self):
         return pd.read_csv(self.getSeriesMetaCSV(),  encoding="ISO-8859-1")
@@ -246,22 +287,22 @@
     def askUserForDicomSeriesNumber(self):
         self.printDicomsInfo()
         seNum = input("Enter the dicom series number: ")
         return int(seNum)
 
     def findDicomSeries(self, descriptionStr, excludeStr=None):
         return self.getSeriesNumbersMatchingDescriptionStr(descriptionStr, excludeStr=excludeStr)
-    
+
     def getStartTime_EndTimeOfExam(self):
         NN = self.getListOfSeNums()
         Ns = min(NN)
         Ne = max([i for i in NN if i < 99])
         df = self.getSeriesMetaAsDataFrame()
         t2 = self.getStartTimeForSeriesN_HHMMSS(Ne, df=df)
-        t2 = datetime.datetime.strptime(str(t2), '%H%M%S.%f')
+        t2 = mi_utils.timeToDatetime(str(t2))
         endT = t2 + datetime.timedelta(0, self.getTimeTakenForSeriesN_s(Ne, df=df))
         endT_HHMMSS = datetime.datetime.strftime(endT, '%H%M%S')
         return self.getStartTimeForSeriesN_HHMMSS(Ns), endT_HHMMSS
 
     def getTimeTakenForSeriesN_s(self, N, df=None):
         if df is None:
             df = self.getSeriesMetaAsDataFrame()
@@ -277,16 +318,16 @@
             df = self.getSeriesMetaAsDataFrame()
         return list(df.loc[df['SeriesNumber']==N,'AcquisitionTime'])[0]
 
     def getDifferenceBetweenStartTimesOfTwoScans_s(self, seN1, seN2):
         df = self.getSeriesMetaAsDataFrame()
         t1 = self.getStartTimeForSeriesN_HHMMSS(seN1, df)
         t2 = self.getStartTimeForSeriesN_HHMMSS(seN2, df)
-        t1 = datetime.datetime.strptime(str(t1), '%H%M%S.%f')
-        t2 = datetime.datetime.strptime(str(t2), '%H%M%S.%f')
+        t1 = mi_utils.timeToDatetime(str(t1))
+        t2 = mi_utils.timeToDatetime(str(t2))
         return (t2-t1).seconds
 
     def getTotalScanTime_s(self):
         se = self.getListOfSeNums()
         se = [i for i in se if i < 1000]
         s1 = self.getDifferenceBetweenStartTimesOfTwoScans_s(min(se), max(se))
         s2 = self.getTimeTakenForSeriesN_s(max(se))
@@ -300,64 +341,95 @@
         dOut = {}
         for iSeries in dcmStudy:
             if descriptionStr.lower() in iSeries.getTag('SeriesDescription').lower():
                 dOut[iSeries.getTag('SeriesNumber', ifNotFound='#')] = iSeries.getSeriesOutDirName()
         return dOut
 
     def getSeriesMetaValue(self, seNum, varName):
-        """
-        :param seNum:
-        :param varName: from : EchoTime FlipAngle HeartRate
-                                InPlanePhaseEncodingDirection InternalPulseSequenceName PulseSequenceName
-                                 RepetitionTime ScanDuration SeriesDescription
-                                 SeriesNumber SpacingBetweenSlices AcquisitionTime
-                                 dCol dRow dSlice dTime
-                                 nCols nRow nSlice nTime
-        :return:
+        """Get meta value for given series naumber
+
+        Args:
+            seNum (int): series number
+            varName (str): tag name, from: EchoTime FlipAngle HeartRate
+                InPlanePhaseEncodingDirection InternalPulseSequenceName PulseSequenceName
+                RepetitionTime ScanDuration SeriesDescription
+                SeriesNumber SpacingBetweenSlices StartTime
+                dCol dRow dSlice dTime
+                nCols nRow nSlice nTime
+
+        Returns:
+            ANY: tag value
         """
         df = self.getSeriesMetaAsDataFrame()
         return list(df.loc[df['SeriesNumber'] == seNum, varName])[0]
 
     def getMetaTagsFile(self, suffix=""):
         return os.path.join(self.getMetaDir(), f"{self.subjID}Tags{suffix}.json")
 
     def setTagValue(self, tag, value, suffix=""):
         self.updateMetaFile({tag:value}, suffix)
 
     def getTagValue(self, tagName, ifNotFound='Unknown'): # FIXME is this done correctly
         return self.getMetaDict().get(tagName, ifNotFound)
 
     def getMetaDict(self, suffix=""):
+        """Get meta json file as dictionary
+
+        Args:
+            suffix (str, optional): Suffix of json file. Defaults to "".
+
+        Returns:
+            dict: Meta json file 
+        """
         ff = self.getMetaTagsFile(suffix)
         dd = {}
         if os.path.isfile(ff):
             dd = spydcm.dcmTools.parseJsonToDictionary(ff)
         return dd
 
     def getMetaTagValue(self, tag, NOT_FOUND=None, metaSuffix=""):
+        """Get specific tag from meta json file
+
+        Args:
+            tag (str): Name of tag to return
+            NOT_FOUND (ANY, optional): A default value to return if "tag" not found. Defaults to None.
+            metaSuffix (str, optional): Suffix of json file. Defaults to "".
+
+        Raises:
+            e: OSError if meta json file not found
+
+        Returns:
+            ANY: tag value from json file
+        """
         try:
             return self.getMetaDict(metaSuffix).get(tag, NOT_FOUND)
         except OSError as e:
             if NOT_FOUND is not None:
                 return NOT_FOUND
             else:
                 raise e
 
     def updateMetaFile(self, metaDict, metasuffix=""):
+        """Update the meta json file
+
+        Args:
+            metaDict (dict): dictionary with key value pairs to update
+            metasuffix (str, optional): Suffix of json file. Defaults to "".
+        """
         dd = self.getMetaDict(metasuffix)
         dd.update(metaDict)
         spydcm.dcmTools.writeDictionaryToJSON(self.getMetaTagsFile(metasuffix), dd)
         self.logger.info('updateMetaFile')
 
     def buildDicomMeta(self):
         # this uses pydicom - so tag names are different.
         dcmStudies = spydcm.dcmTK.ListOfDicomStudies.setFromDirectory(self.getDicomsDir(), HIDE_PROGRESSBAR=True)
         ddFull = dcmStudies[0].getStudySummaryDict()
         ddFull['SubjectID'] = self.subjID
-        ddFull['SubjN'] = self.subjN
+        ddFull['SubjN'] = self._subjN
         for k1 in range(1, len(dcmStudies)):
             ddFull['Series'] += dcmStudies[k1].getStudySummaryDict()['Series']
         self.updateMetaFile(ddFull)
 
     def countNumberOfDicoms(self):
         return mi_utils.countFilesInDir(self.getDicomsDir())
     
@@ -453,42 +525,62 @@
         #   header keys
         infoKeys = ['SubjectID', 'SubjN', 'PatientBirthDate', 'PatientID', 'PatientName', 'PatientSex',
                     'StudyDate', 'StudyDescription', 'StudyInstanceUID', 'StudyID'] + extraKeys
         mm = self.getMetaDict()
         aa = '%5.2f'%(self.getAge())
         return [mm.get(i, "Unknown") for i in infoKeys]+[aa], infoKeys + ['Age']
 
+    # ------------------------------------------------------------------------------------------
     def anonymise(self, anonName=None):
         if type(anonName) == str:
             if len(anonName) == 0:  
                 anonName = None # Still anonymise, but let program choose the new anonName
         self.logger.info('Anonymise in place')
         spydcm.anonymiseInPlace(self.getDicomsDir(), anonName=anonName)
+        self.setIsAnonymised()
         self.buildDicomMeta()
 
+    def setIsAnonymised(self):
+        self.updateMetaFile({"ANONYMISED": True})
+    
+    def isAnonymised(self):
+        return self.getTagValue("ANONYMISED", False)
+
     def setEncodedName(self, NAME, FIRST_NAMES=""):
         """
         funct to add name after (will encode)
         :param NAME:
         :param FIRST_NAMES:
         :return:
         """
         dd = {'NAME': mi_utils.encodeString(NAME, self.subjID),
               'FIRST_NAMES': mi_utils.encodeString(FIRST_NAMES, self.subjID)}
         self.updateMetaFile(dd)
 
     def getName(self):
-        try:
-            return mi_utils.decodeString(self.getTagValue("NAME", "UNKNOWN"), self.subjID)
-        except:
-            return self.getMetaDict().get('PatientName', 'Name-Unknown')
+        if self.isAnonymised():
+            try:
+                return mi_utils.decodeString(self.getTagValue("NAME", "UNKNOWN"), self.subjID)
+            except:
+                return self.getTagValue('PatientName', 'Name-Unknown')
+        else:
+            return self.getTagValue('PatientName', 'Name-Unknown')
 
     def getName_FirstNames(self):
-        return mi_utils.decodeString(self.getTagValue("NAME", "UNKNOWN"), self.subjID), \
-               mi_utils.decodeString(self.getTagValue("FIRST_NAMES", "UNKNOWN"), self.subjID)
+        if self.isAnonymised():
+            return mi_utils.decodeString(self.getTagValue("NAME", "UNKNOWN"), self.subjID), \
+                mi_utils.decodeString(self.getTagValue("FIRST_NAMES", "UNKNOWN"), self.subjID)
+        else:
+            name = self.getName()
+            name = name.replace(" ","_")
+            name = name.replace("^","_")
+            while "__" in name:
+                name = name.replace("__","_")
+            return name
+
 
     # ------------------------------------------------------------------------------------------
     def getSummary_list(self):
         hh = ["SubjectID","PatientID","Gender","StudyDate","NumberOfSeries","SERIES_DECRIPTIONS"]
         parts = [self.subjID, self.getMetaTagValue('PatientID'), 
                 self.getMetaTagValue('PatientSex'), self.getMetaTagValue('StudyDate'), 
                 len(self.getMetaTagValue('Series')), self.getSeriesDescriptionsStr()]
@@ -499,19 +591,31 @@
         """
         This returns a float, and is slightly wrong in account of leap years.
         This is intentional.
         :return: years - float
         """
         dd = self.getMetaDict()
         try:
-            birth = dd["PatientBirthDate"]
-            study = dd["StudyDate"]
-            return (spydcm.dcmTools.dbDateToDateTime(study) - spydcm.dcmTools.dbDateToDateTime(birth)).days / 365.0
-        except (KeyError, ValueError):
-            return np.nan
+            ageStr = dd['PatientAge']
+        except KeyError:
+            try:
+                birth = dd["PatientBirthDate"]
+                study = dd["StudyDate"]
+                return (spydcm.dcmTools.dbDateToDateTime(study) - spydcm.dcmTools.dbDateToDateTime(birth)).days / 365.0
+            except (KeyError, ValueError):
+                return np.nan
+        age = np.nan
+        try:
+            age = int(ageStr)
+        except ValueError:
+            try:
+                age = int(ageStr.lower().replace('y', ''))
+            except ValueError:
+                pass
+        return age
 
     def getGender(self):
         return self.getMetaDict()['PatientSex']
     
     def isMale(self):
         sex = self.getGender()
         return sex.strip().lower() == 'm'
@@ -718,21 +822,39 @@
         return None
     SubjList = SubjectList.setByDirectory(dataRoot=dataRoot, subjectPrefix=subjPrefix)
     return SubjList.findSubjMatchingStudyUID(queryUID)
 
 
 ### ====================================================================================================================
 def splitSubjID(s):
-    prefix = s.rstrip('0123456789')
-    number = int(s[len(prefix):])
-    return prefix, number
+    """Strip a subject ID to prefix and number
+
+    Args:
+        s (str): subject ID
+
+    Returns:
+        tuple: prefix: str, number: int (if len 3 - then also suffix: str)
+    """
+    parts = re.split(r'(\d+)', s)  # Split the string on one or more digits
+    parts = [part for part in parts if part]  # Filter out empty parts
+    if len(parts) >= 3:
+        return parts[0], int(parts[1]), ''.join(parts[2:])
+    return parts[0], int(parts[1])
 
 def getNumberFromSubjID(subjID):
     return splitSubjID(subjID)[1]
 
+def findZeroPadding(subjID):
+    match = re.search(r'\d+', subjID) # first seq of numbers
+    if match:
+        number = match.group()  # group numbers
+        return len(number)# 
+    else:
+        return 0  # If no number found, return 0
+
 def guessSubjectPrefix(dataRootDir):
     """Guess the subject prefix by looking for common names in the dataRootDir
 
     Args:
         dataRootDir (str): path to root directory of subject filesystem database
 
     Returns:
@@ -741,48 +863,50 @@
     Exception:
         mi_utils.SubjPrefixError: is ambiguous
     """
     allDir = [i for i in os.listdir(dataRootDir) if os.path.isdir(os.path.join(dataRootDir, i))]
     allDir_subj = {}
     for i in allDir:
         try:
-            prefix, N = splitSubjID(i)
+            prefix_N_suffix = splitSubjID(i)
+            prefix = prefix_N_suffix[0]
+            N = prefix_N_suffix[1]
         except ValueError: 
             continue # directory not correct format - could not split to integer
         allDir_subj.setdefault(prefix, []).append(N)
     options = list(allDir_subj.keys())
     if len(options) == 0:
-        raise mi_utils.SubjPrefixError("Error guessing subject prefix - ambiguous")
+        raise mi_utils.SubjPrefixError("Error guessing subject prefix - ambiguous - please provide")
     counts = [len(allDir_subj[i]) for i in options]
     maxCount = np.argmax(counts)
     if options.count(options[maxCount]) != 1:
-        raise mi_utils.SubjPrefixError("Error guessing subject prefix - ambiguous")
+        raise mi_utils.SubjPrefixError("Error guessing subject prefix - ambiguous - please provide")
     return options[maxCount]
 
 ### ====================================================================================================================
 ###  Helper functions for building new or adding to subjects
 ### ====================================================================================================================
-def buildSubjectID(subjN, subjectPrefix):
+def buildSubjectID(subjN, subjectPrefix, padZeros=mi_utils.MIResearch_config.default_pad_zeros, suffix=''):
     if subjN is None:
         return subjectPrefix
-    return f"{subjectPrefix}{subjN:06d}"
+    return f"{subjectPrefix}{subjN:0{padZeros}d}{suffix}"
 
 def getNextSubjN(dataRootDir, subjectPrefix=None):
     if subjectPrefix is None:
         subjectPrefix = guessSubjectPrefix(dataRootDir)
-    allNums = [int(i[len(subjectPrefix):]) for i in os.listdir(dataRootDir) if (os.path.isdir(os.path.join(dataRootDir, i)) and  i.startswith(subjectPrefix))]
+    allNums = [getNumberFromSubjID(i) for i in os.listdir(dataRootDir) if (os.path.isdir(os.path.join(dataRootDir, i)) and  i.startswith(subjectPrefix))]
     try:
         return max(allNums)+1
     except ValueError:
         return 1
 
-def doesSubjectExist(subjN, dataRootDir, subjectPrefix=None):
+def doesSubjectExist(subjN, dataRootDir, subjectPrefix=None, padZeros=mi_utils.MIResearch_config.default_pad_zeros, suffix=""):
     if subjectPrefix is None:
         subjectPrefix = guessSubjectPrefix(dataRootDir)
-    return os.path.isdir(os.path.join(dataRootDir, buildSubjectID(subjN, subjectPrefix)))
+    return os.path.isdir(os.path.join(dataRootDir, buildSubjectID(subjN, subjectPrefix, padZeros=padZeros, suffix=suffix)))
 
 def getNextSubjID(dataRootDir, subjectPrefix=None):
     if subjectPrefix is None:
         subjectPrefix = guessSubjectPrefix(dataRootDir)
     return buildSubjectID(getNextSubjN(dataRootDir, subjectPrefix), subjectPrefix)
 
 def _createSubjectHelper(dicomDir_orData, SubjClass, subjNumber, dataRoot, subjPrefix, anonName, QUIET, FORCE_NEW_SUBJ=False):
```

### Comparing `imaging-research-0.0.9/setup.py` & `imaging_research-0.1.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'imaging-research'
 DESCRIPTION = 'Medical Imaginging Research structuring and automation'
 URL = 'https://github.com/fraser29/miresearch'
 EMAIL = 'callaghan.fm@gmail.com'
 AUTHOR = 'Fraser M. Callaghan'
 REQUIRES_PYTHON = '>=3.9.0'
-VERSION = '0.0.9'
+VERSION = '0.1.0'
 KEYWORDS="medical, imaging, mri, ct, dicom"
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     "spydcmtk", "pandas", "numpy", "watchdog"
 ]
```


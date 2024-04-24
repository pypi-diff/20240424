# Comparing `tmp/rcsb.utils.struct-0.45.tar.gz` & `tmp/rcsb_utils_struct-0.46.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rcsb.utils.struct-0.45.tar", last modified: Mon Aug  7 22:26:08 2023, max compression
+gzip compressed data, was "rcsb_utils_struct-0.46.tar", last modified: Wed Apr 24 17:47:00 2024, max compression
```

## Comparing `rcsb.utils.struct-0.45.tar` & `rcsb_utils_struct-0.46.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-08-07 22:26:08.313214 rcsb.utils.struct-0.45/
--rw-r--r--   0 vsts      (1001) docker     (122)     2594 2023-08-07 22:24:24.000000 rcsb.utils.struct-0.45/HISTORY.txt
--rw-r--r--   0 vsts      (1001) docker     (122)    11357 2023-08-07 22:24:24.000000 rcsb.utils.struct-0.45/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (122)      111 2023-08-07 22:24:24.000000 rcsb.utils.struct-0.45/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (122)     1804 2023-08-07 22:26:08.313214 rcsb.utils.struct-0.45/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)     1006 2023-08-07 22:24:24.000000 rcsb.utils.struct-0.45/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-08-07 22:26:08.309214 rcsb.utils.struct-0.45/rcsb/
--rw-r--r--   0 vsts      (1001) docker     (122)       65 2023-08-07 22:24:24.000000 rcsb.utils.struct-0.45/rcsb/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-08-07 22:26:08.309214 rcsb.utils.struct-0.45/rcsb/utils/
--rw-r--r--   0 vsts      (1001) docker     (122)       65 2023-08-07 22:24:24.000000 rcsb.utils.struct-0.45/rcsb/utils/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-08-07 22:26:08.313214 rcsb.utils.struct-0.45/rcsb/utils/struct/
--rw-r--r--   0 vsts      (1001) docker     (122)    13214 2023-08-07 22:24:24.000000 rcsb.utils.struct-0.45/rcsb/utils/struct/CathClassificationProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)    15694 2023-08-07 22:24:24.000000 rcsb.utils.struct-0.45/rcsb/utils/struct/EcodClassificationProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3191 2023-08-07 22:24:24.000000 rcsb.utils.struct-0.45/rcsb/utils/struct/EntryInfoProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)    21008 2023-08-07 22:24:24.000000 rcsb.utils.struct-0.45/rcsb/utils/struct/Scop2ClassificationProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)    16717 2023-08-07 22:24:24.000000 rcsb.utils.struct-0.45/rcsb/utils/struct/ScopClassificationProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)      154 2023-08-07 22:24:24.000000 rcsb.utils.struct-0.45/rcsb/utils/struct/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-08-07 22:26:08.309214 rcsb.utils.struct-0.45/rcsb.utils.struct.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (122)     1804 2023-08-07 22:26:08.000000 rcsb.utils.struct-0.45/rcsb.utils.struct.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)      623 2023-08-07 22:26:08.000000 rcsb.utils.struct-0.45/rcsb.utils.struct.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-08-07 22:26:08.000000 rcsb.utils.struct-0.45/rcsb.utils.struct.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-08-07 22:25:00.000000 rcsb.utils.struct-0.45/rcsb.utils.struct.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (122)       59 2023-08-07 22:26:08.000000 rcsb.utils.struct-0.45/rcsb.utils.struct.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        5 2023-08-07 22:26:08.000000 rcsb.utils.struct-0.45/rcsb.utils.struct.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (122)       21 2023-08-07 22:24:24.000000 rcsb.utils.struct-0.45/requirements.txt
--rwxr-xr-x   0 vsts      (1001) docker     (122)      108 2023-08-07 22:26:08.313214 rcsb.utils.struct-0.45/setup.cfg
--rwxr-xr-x   0 vsts      (1001) docker     (122)     2325 2023-08-07 22:24:24.000000 rcsb.utils.struct-0.45/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-24 17:47:00.872362 rcsb_utils_struct-0.46/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2730 2024-04-24 17:44:41.000000 rcsb_utils_struct-0.46/HISTORY.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)    11357 2024-04-24 17:44:41.000000 rcsb_utils_struct-0.46/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (127)      111 2024-04-24 17:44:41.000000 rcsb_utils_struct-0.46/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (127)     1926 2024-04-24 17:47:00.872362 rcsb_utils_struct-0.46/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     1006 2024-04-24 17:44:41.000000 rcsb_utils_struct-0.46/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-24 17:47:00.868362 rcsb_utils_struct-0.46/rcsb/
+-rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-04-24 17:44:41.000000 rcsb_utils_struct-0.46/rcsb/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-24 17:47:00.868362 rcsb_utils_struct-0.46/rcsb/utils/
+-rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-04-24 17:44:41.000000 rcsb_utils_struct-0.46/rcsb/utils/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-24 17:47:00.872362 rcsb_utils_struct-0.46/rcsb/utils/struct/
+-rw-r--r--   0 vsts      (1001) docker     (127)    13214 2024-04-24 17:44:41.000000 rcsb_utils_struct-0.46/rcsb/utils/struct/CathClassificationProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    15694 2024-04-24 17:44:41.000000 rcsb_utils_struct-0.46/rcsb/utils/struct/EcodClassificationProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3191 2024-04-24 17:44:41.000000 rcsb_utils_struct-0.46/rcsb/utils/struct/EntryInfoProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    21605 2024-04-24 17:44:41.000000 rcsb_utils_struct-0.46/rcsb/utils/struct/Scop2ClassificationProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    16717 2024-04-24 17:44:41.000000 rcsb_utils_struct-0.46/rcsb/utils/struct/ScopClassificationProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      154 2024-04-24 17:44:41.000000 rcsb_utils_struct-0.46/rcsb/utils/struct/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-24 17:47:00.872362 rcsb_utils_struct-0.46/rcsb.utils.struct.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1926 2024-04-24 17:47:00.000000 rcsb_utils_struct-0.46/rcsb.utils.struct.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)      623 2024-04-24 17:47:00.000000 rcsb_utils_struct-0.46/rcsb.utils.struct.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-24 17:47:00.000000 rcsb_utils_struct-0.46/rcsb.utils.struct.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-24 17:45:33.000000 rcsb_utils_struct-0.46/rcsb.utils.struct.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (127)       59 2024-04-24 17:47:00.000000 rcsb_utils_struct-0.46/rcsb.utils.struct.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        5 2024-04-24 17:47:00.000000 rcsb_utils_struct-0.46/rcsb.utils.struct.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       21 2024-04-24 17:44:41.000000 rcsb_utils_struct-0.46/requirements.txt
+-rwxr-xr-x   0 vsts      (1001) docker     (127)      108 2024-04-24 17:47:00.872362 rcsb_utils_struct-0.46/setup.cfg
+-rwxr-xr-x   0 vsts      (1001) docker     (127)     2325 2024-04-24 17:44:41.000000 rcsb_utils_struct-0.46/setup.py
```

### Comparing `rcsb.utils.struct-0.45/HISTORY.txt` & `rcsb_utils_struct-0.46/HISTORY.txt`

 * *Files 4% similar despite different names*

```diff
@@ -31,8 +31,9 @@
  22-Sep-2021    V0.38 Add module EntryInfoProvider and associated tests (accessor methods only)
  23-Sep-2021    V0.39 Update SCOP version and path details
  16-Nov-2021    V0.40 Append additional ECOD annotations for given entryId and chainId instead of overwriting
  24-Feb-2022    V0.41 Resolve duplication issues with Scop2 tree node list, and fix parent ID lists for nodes with multiple parents
   9-Mar-2022    V0.42 Fix issue related to V0.41 update to Scop2 provider
   6-Jan-2023    V0.43 Configuration changes to support tox 4
  18-Apr-2023    V0.44 Fix Ecod and Scop2 provider fall-back file import
- 18-Jul-2023    V0.45 Resolve duplication issues with Scop2 families and CATH residue range lists
+ 18-Jul-2023    V0.45 Resolve duplication issues with Scop2 families and CATH residue range lists
+ 24-Apr-2024    V0.46 Turn off fetching of source SCOP2/SCOP2B data following shutdown of host website; rely on latest fallback instead
```

### Comparing `rcsb.utils.struct-0.45/LICENSE` & `rcsb_utils_struct-0.46/LICENSE`

 * *Files identical despite different names*

### Comparing `rcsb.utils.struct-0.45/PKG-INFO` & `rcsb_utils_struct-0.46/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 Metadata-Version: 2.1
 Name: rcsb.utils.struct
-Version: 0.45
+Version: 0.46
 Summary: RCSB Python utility classes for accessing PDB primary structure data and features associated with these data
 Home-page: https://github.com/rcsb/py-rcsb_utils_seq
 Author: John Westbrook
 Author-email: john.westbrook@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: rcsb.utils.io>=1.28
 Provides-Extra: dev
+Requires-Dist: check-manifest; extra == "dev"
 Provides-Extra: test
-License-File: LICENSE
+Requires-Dist: coverage; extra == "test"
 
 # RCSB Python Primary Structure Data Utilities
 
 [![Build Status](https://dev.azure.com/rcsb/RCSB%20PDB%20Python%20Projects/_apis/build/status/rcsb.py-rcsb_utils_struct?branchName=master)](https://dev.azure.com/rcsb/RCSB%20PDB%20Python%20Projects/_build/latest?definitionId=2&branchName=master)
 
 ## Introduction
```

### Comparing `rcsb.utils.struct-0.45/README.md` & `rcsb_utils_struct-0.46/README.md`

 * *Files identical despite different names*

### Comparing `rcsb.utils.struct-0.45/rcsb/utils/struct/CathClassificationProvider.py` & `rcsb_utils_struct-0.46/rcsb/utils/struct/CathClassificationProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.struct-0.45/rcsb/utils/struct/EcodClassificationProvider.py` & `rcsb_utils_struct-0.46/rcsb/utils/struct/EcodClassificationProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.struct-0.45/rcsb/utils/struct/EntryInfoProvider.py` & `rcsb_utils_struct-0.46/rcsb/utils/struct/EntryInfoProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.struct-0.45/rcsb/utils/struct/Scop2ClassificationProvider.py` & `rcsb_utils_struct-0.46/rcsb/utils/struct/Scop2ClassificationProvider.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 #  Date:  29-Jun-2021 jdw
 #
 #  Updates:
 #   10-Sep-2021 jdw split tree with type and class roots
 #   24-Feb-2022 dwp Resolve duplication issues with Scop2 tree node list, and fix parent ID lists for nodes with multiple parents
 #   18-Apr-2023 aae Use "pickle" as default file format
 #   18-Jul-2023 dwp Resolve duplication issues with Scop2 families list
+#   23-Apr-2024 dwp SCOP2/SCOP2B website was shut down--turn off fetching of source data until/if new site is made available again
 ##
 """
   Extract SCOP2 domain assignments, term descriptions and SCOP2 classification hierarchy
   from SCOP2 and SCOP2B flat files.
 
 """
 
@@ -40,21 +41,22 @@
         self.__dirPath = os.path.join(self.__cachePath, dirName)
         self.__useCache = useCache
         super(Scop2ClassificationProvider, self).__init__(self.__cachePath, [dirName])
         #
         self.__version = "latest"
         self.__fmt = "pickle"
         self.__mU = MarshalUtil(workPath=self.__dirPath)
-        self.__nD, self.__ntD, self.__pAD, self.__pBD, self.__pBRootD, self.__fD, self.__sfD, self.__sf2bD = self.__reload(useCache=self.__useCache, fmt=self.__fmt)
-        #
-        if not useCache and not self.testCache():
-            ok = self.__fetchFromBackup(fmt=self.__fmt)
-            if ok:
-                self.__nD, self.__ntD, self.__pAD, self.__pBD, self.__pBRootD, self.__fD, self.__sfD, self.__sf2bD = self.__reload(useCache=True, fmt=self.__fmt)
         #
+        # Temporarily turn off fetching of source data until new site is made available again
+        # self.__nD, self.__ntD, self.__pAD, self.__pBD, self.__pBRootD, self.__fD, self.__sfD, self.__sf2bD = self.__reload(useCache=self.__useCache, fmt=self.__fmt)
+        # if not useCache and not self.testCache():
+        self.__fetchFromBackup(fmt=self.__fmt)
+        self.__nD, self.__ntD, self.__pAD, self.__pBD, self.__pBRootD, self.__fD, self.__sfD, self.__sf2bD = self.__reload(useCache=True, fmt=self.__fmt)
+        if not self.testCache():
+            logger.error("Failed to build SCOP2 CACHE")
 
     def testCache(self):
         logger.info(
             "SCOP2 lengths nD %d pAD %d pBD %d pBRootD %d fD %d sfD %d sf2bD %d",
             len(self.__nD), len(self.__pAD), len(self.__pBD), len(self.__pBRootD), len(self.__fD), len(self.__sfD), len(self.__sf2bD)
         )
         if (len(self.__nD) > 9000) and (len(self.__pAD) > 70000):
@@ -240,19 +242,21 @@
 
     def __fetchFromBackup(self, fmt="pickle"):
         urlTarget = "https://raw.githubusercontent.com/rcsb/py-rcsb_exdb_assets/master/fall_back/SCOP2"
         #
         fn = self.__getAssignmentFileName(fmt=fmt)
         assignmentPath = os.path.join(self.__dirPath, fn)
         urlPath = os.path.join(urlTarget, fn)
-        self.__mU.mkdir(assignmentPath)
         #
-        logger.info("Using backup URL %r", urlPath)
+        logger.info("Creating directory %r", self.__dirPath)
+        self.__mU.mkdir(self.__dirPath)
+        logger.info("Fetching backup URL %r to local path %r", urlPath, assignmentPath)
         fU = FileUtil()
         ok = fU.get(urlPath, assignmentPath)
+        logger.info("Fetch status %r", ok)
         return ok
 
     def __fetchFromSource(self):
         """Fetch the classification names and domain assignments from SCOP2 and SCOP2B resources.
 
         SCOP2 domain names:
             https://scop.mrc-lmb.cam.ac.uk/files/scop-des-latest.txt
@@ -440,14 +444,17 @@
 
         # 2021/06/12 - 05:52 | PDB: 23.21 | UniProt: 2021.03
           PDB     CHAIN   SF_DOMID        SP_PRIMARY      RES_BEG RES_END PDB_BEG PDB_END SP_BEG  SP_END
           5id7    B       8033045 P02768  197     388     197     388     221     412
           1o9x    A       8033045 P02768  197     388     197     388     221     412
         """
         sfD = {}
+        if len(scop2bL) == 0 or len(domToSfD) == 0:
+            logger.error("Empty list or dict (scop2bL len %r, domToSfD len %r)", len(scop2bL), len(domToSfD))
+            return sfD
         try:
             for rowD in scop2bL:
                 if rowD["SF_DOMID"] in domToSfD:
                     sfD.setdefault((rowD["PDB"].upper(), rowD["CHAIN"]), []).append((rowD["SF_DOMID"], domToSfD[rowD["SF_DOMID"]], rowD["CHAIN"], rowD["PDB_BEG"], rowD["PDB_END"]))
                 else:
                     logger.warning("Missing SCOP2B SF ID mapping for %r", rowD["SF_DOMID"])
         except Exception as e:
```

### Comparing `rcsb.utils.struct-0.45/rcsb/utils/struct/ScopClassificationProvider.py` & `rcsb_utils_struct-0.46/rcsb/utils/struct/ScopClassificationProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.struct-0.45/rcsb.utils.struct.egg-info/PKG-INFO` & `rcsb_utils_struct-0.46/rcsb.utils.struct.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 Metadata-Version: 2.1
 Name: rcsb.utils.struct
-Version: 0.45
+Version: 0.46
 Summary: RCSB Python utility classes for accessing PDB primary structure data and features associated with these data
 Home-page: https://github.com/rcsb/py-rcsb_utils_seq
 Author: John Westbrook
 Author-email: john.westbrook@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: rcsb.utils.io>=1.28
 Provides-Extra: dev
+Requires-Dist: check-manifest; extra == "dev"
 Provides-Extra: test
-License-File: LICENSE
+Requires-Dist: coverage; extra == "test"
 
 # RCSB Python Primary Structure Data Utilities
 
 [![Build Status](https://dev.azure.com/rcsb/RCSB%20PDB%20Python%20Projects/_apis/build/status/rcsb.py-rcsb_utils_struct?branchName=master)](https://dev.azure.com/rcsb/RCSB%20PDB%20Python%20Projects/_build/latest?definitionId=2&branchName=master)
 
 ## Introduction
```

### Comparing `rcsb.utils.struct-0.45/rcsb.utils.struct.egg-info/SOURCES.txt` & `rcsb_utils_struct-0.46/rcsb.utils.struct.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rcsb.utils.struct-0.45/setup.py` & `rcsb_utils_struct-0.46/setup.py`

 * *Files identical despite different names*


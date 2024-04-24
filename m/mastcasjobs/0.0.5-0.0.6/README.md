# Comparing `tmp/mastcasjobs-0.0.5.tar.gz` & `tmp/mastcasjobs-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mastcasjobs-0.0.5.tar", last modified: Thu Jul 28 18:29:08 2022, max compression
+gzip compressed data, was "mastcasjobs-0.0.6.tar", last modified: Wed Apr 24 18:47:54 2024, max compression
```

## Comparing `mastcasjobs-0.0.5.tar` & `mastcasjobs-0.0.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 rlw       (4809) STSCI\science  (1031)        0 2022-07-28 18:29:08.840096 mastcasjobs-0.0.5/
--rw-r--r--   0 rlw       (4809) STSCI\science  (1031)     1060 2017-02-24 22:38:55.000000 mastcasjobs-0.0.5/LICENSE.rst
--rw-r--r--   0 rlw       (4809) STSCI\science  (1031)       48 2017-02-24 22:38:55.000000 mastcasjobs-0.0.5/MANIFEST.in
--rw-r--r--   0 rlw       (4809) STSCI\science  (1031)     3555 2022-07-28 18:29:08.840175 mastcasjobs-0.0.5/PKG-INFO
--rw-r--r--   0 rlw       (4809) STSCI\science  (1031)     2951 2022-07-28 18:20:39.000000 mastcasjobs-0.0.5/README.rst
-drwxr-xr-x   0 rlw       (4809) STSCI\science  (1031)        0 2022-07-28 18:29:08.838660 mastcasjobs-0.0.5/mastcasjobs/
--rw-r--r--   0 rlw       (4809) STSCI\science  (1031)    15073 2022-07-28 18:06:26.000000 mastcasjobs-0.0.5/mastcasjobs/__init__.py
-drwxr-xr-x   0 rlw       (4809) STSCI\science  (1031)        0 2022-07-28 18:29:08.839930 mastcasjobs-0.0.5/mastcasjobs.egg-info/
--rw-r--r--   0 rlw       (4809) STSCI\science  (1031)     3555 2022-07-28 18:29:08.000000 mastcasjobs-0.0.5/mastcasjobs.egg-info/PKG-INFO
--rw-r--r--   0 rlw       (4809) STSCI\science  (1031)      302 2022-07-28 18:29:08.000000 mastcasjobs-0.0.5/mastcasjobs.egg-info/SOURCES.txt
--rw-r--r--   0 rlw       (4809) STSCI\science  (1031)        1 2022-07-28 18:29:08.000000 mastcasjobs-0.0.5/mastcasjobs.egg-info/dependency_links.txt
--rw-r--r--   0 rlw       (4809) STSCI\science  (1031)        1 2022-05-17 22:31:49.000000 mastcasjobs-0.0.5/mastcasjobs.egg-info/not-zip-safe
--rw-r--r--   0 rlw       (4809) STSCI\science  (1031)       32 2022-07-28 18:29:08.000000 mastcasjobs-0.0.5/mastcasjobs.egg-info/requires.txt
--rw-r--r--   0 rlw       (4809) STSCI\science  (1031)       12 2022-07-28 18:29:08.000000 mastcasjobs-0.0.5/mastcasjobs.egg-info/top_level.txt
--rw-r--r--   0 rlw       (4809) STSCI\science  (1031)       24 2022-07-28 18:07:43.000000 mastcasjobs-0.0.5/requirements.txt
--rw-r--r--   0 rlw       (4809) STSCI\science  (1031)      707 2022-07-28 18:29:08.840569 mastcasjobs-0.0.5/setup.cfg
--rw-r--r--   0 rlw       (4809) STSCI\science  (1031)       38 2021-08-18 14:36:39.000000 mastcasjobs-0.0.5/setup.py
+drwxr-xr-x   0 rlw       (4809) STSCI\science  (1031)        0 2024-04-24 18:47:54.698469 mastcasjobs-0.0.6/
+-rw-r--r--   0 rlw       (4809) STSCI\science  (1031)     1060 2017-02-24 22:38:55.000000 mastcasjobs-0.0.6/LICENSE.rst
+-rw-r--r--   0 rlw       (4809) STSCI\science  (1031)       48 2017-02-24 22:38:55.000000 mastcasjobs-0.0.6/MANIFEST.in
+-rw-r--r--   0 rlw       (4809) STSCI\science  (1031)     3555 2024-04-24 18:47:54.698599 mastcasjobs-0.0.6/PKG-INFO
+-rw-r--r--   0 rlw       (4809) STSCI\science  (1031)     2951 2022-07-28 18:20:39.000000 mastcasjobs-0.0.6/README.rst
+drwxr-xr-x   0 rlw       (4809) STSCI\science  (1031)        0 2024-04-24 18:47:54.695421 mastcasjobs-0.0.6/mastcasjobs/
+-rw-r--r--   0 rlw       (4809) STSCI\science  (1031)    17843 2024-04-24 18:30:10.000000 mastcasjobs-0.0.6/mastcasjobs/__init__.py
+drwxr-xr-x   0 rlw       (4809) STSCI\science  (1031)        0 2024-04-24 18:47:54.698085 mastcasjobs-0.0.6/mastcasjobs.egg-info/
+-rw-r--r--   0 rlw       (4809) STSCI\science  (1031)     3555 2024-04-24 18:47:54.000000 mastcasjobs-0.0.6/mastcasjobs.egg-info/PKG-INFO
+-rw-r--r--   0 rlw       (4809) STSCI\science  (1031)      302 2024-04-24 18:47:54.000000 mastcasjobs-0.0.6/mastcasjobs.egg-info/SOURCES.txt
+-rw-r--r--   0 rlw       (4809) STSCI\science  (1031)        1 2024-04-24 18:47:54.000000 mastcasjobs-0.0.6/mastcasjobs.egg-info/dependency_links.txt
+-rw-r--r--   0 rlw       (4809) STSCI\science  (1031)        1 2022-05-17 22:31:49.000000 mastcasjobs-0.0.6/mastcasjobs.egg-info/not-zip-safe
+-rw-r--r--   0 rlw       (4809) STSCI\science  (1031)       32 2024-04-24 18:47:54.000000 mastcasjobs-0.0.6/mastcasjobs.egg-info/requires.txt
+-rw-r--r--   0 rlw       (4809) STSCI\science  (1031)       12 2024-04-24 18:47:54.000000 mastcasjobs-0.0.6/mastcasjobs.egg-info/top_level.txt
+-rw-r--r--   0 rlw       (4809) STSCI\science  (1031)       24 2022-07-28 18:07:43.000000 mastcasjobs-0.0.6/requirements.txt
+-rw-r--r--   0 rlw       (4809) STSCI\science  (1031)      707 2024-04-24 18:47:54.699267 mastcasjobs-0.0.6/setup.cfg
+-rw-r--r--   0 rlw       (4809) STSCI\science  (1031)       38 2021-08-18 14:36:39.000000 mastcasjobs-0.0.6/setup.py
```

### Comparing `mastcasjobs-0.0.5/LICENSE.rst` & `mastcasjobs-0.0.6/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `mastcasjobs-0.0.5/PKG-INFO` & `mastcasjobs-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mastcasjobs
-Version: 0.0.5
+Version: 0.0.6
 Summary: An interface to MAST CasJobs.
 Home-page: https://github.com/rlwastro/mastcasjobs
 Author: Richard L. White
 Author-email: rlw@stsci.edu
 License: MIT
 Platform: OS Independent
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `mastcasjobs-0.0.5/README.rst` & `mastcasjobs-0.0.6/README.rst`

 * *Files identical despite different names*

### Comparing `mastcasjobs-0.0.5/mastcasjobs/__init__.py` & `mastcasjobs-0.0.6/mastcasjobs/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 
 from casjobs import CasJobs
 import astropy, numpy, time, sys, os, re, requests
 from astropy.table import Table
 from astropy.io import fits, ascii
 from collections import defaultdict
 import xml.etree.ElementTree as ET
+from io import StringIO
 
 __all__ = ["MastCasJobs", "contexts"]
 
 # some common MAST database contexts
 contexts = [
             "GAIA_DR1",
             "GALEX_Catalogs",
@@ -286,37 +287,84 @@
             r = requests.get(url)
             r.raise_for_status()
             tab = ascii.read(MastCasJobs.replacenull(r.text),format='csv')
         if verbose:
             print("{:.1f} s: Retrieved {} row {} table".format(time.time()-t0,len(tab),format))
         return tab
 
-    def upload_table(self, tablename, data, exists=False):
-        """Upload ascii CSV data into a table in MyDB
+    def upload_table(self, tablename, data, exists=False, verbose=False, sizelimit=200000000):
+        """Upload astropy.Table or ascii CSV data into a table in MyDB
         
         Note there are limits to the volume of data that can be loaded in
-        a single call.  Break the data up into chunks and use the exists 
-        parameter to add each additional chunk for a large table.
+        a single call.  If an astropy table is passed, this function automatically
+        breaks the table up into chunks to allow uploading large tables.
+
+        If the data is specified as a long CSV string, you should break the data up
+        into chunks manually, and use the exists parameter to add each additional
+        chunk.
+
+        Embedded blanks in astropy table columns are converted to underscores
+        to work around a bug in the upload interface. If data is a CSV string,
+        embedded blanks should also be removed or replaced to avoid errors.
+        (This function does not do that for you.)
 
         ## Arguments
 
         * `tablename` (str): Name of table in MyDB.
-        * `data` (str): String containing the CSV data to upload
+        * `data` (astropy.Table or str): astropy.Table or CSV string containing the data to upload
 
         ## Keyword Arguments
 
         * `exists` (bool): If True, expects `tablename` to exist and tries to
             load additional data into that table.  If False, creates a new table.
             If False and table exists, an exception is raised.
+        * `verbose` (bool): If True, prints additional info on upload.
+        * `sizelimit` (int): Maximum size for upload (in bytes).  If data is an
+            astropy.table, the upload is broken into chunks for large tables.
 
         ## Returns
 
         * Nothing.
 
         """
+        if isinstance(data, Table):
+            c = StringIO()
+            tab = data
+            tab.write(c, format="ascii.csv")
+            bdata = c.getvalue()
+            if len(bdata) > sizelimit:
+                # Data is close to limit on maximum upload size
+                # Break data up into chunks that are about 1/2 of size limit to allow
+                # for some variation in row length.  After initial call, set exists to
+                # True so additional rows are added to table.
+                block = len(tab)*(sizelimit//2)//len(bdata)
+                if block == 0:
+                    # uh-oh, this is probably trouble
+                    print("Warning: very long rows in data, upload failure may occur", file=sys.stderr)
+                    block = 1
+                # Recursively call the upload_table function.  If any very long rows are encountered,
+                # the blocks can be broken up further as needed in the recursive calls.
+                for iblock, i in enumerate(range(0, len(tab), block), start=1):
+                    self.upload_table(tablename, tab[i:i+block], exists=exists,
+                                      sizelimit=sizelimit, verbose=verbose)
+                    exists = True
+                    if verbose:
+                        print(f"Copied block {iblock} rows [{i}:{i+block}]")
+                return
+            # embedded blanks break upload interface, so replace them
+            data = bdata.replace(' ','_')
+            if verbose and data != bdata:
+                print("Blanks in table were replaced with underscores")
+            del c, bdata
+        if verbose:
+            print(f"Uploading {len(data):,}-byte data to {tablename}")
+        if len(data) > sizelimit:
+            # uh-oh, this is probably trouble
+            print(f"Warning: data length is greater than size limit ({sizelimit:,} bytes), upload failure may occur",
+                  file=sys.stderr)
         params = dict(tableName=tablename, data=data, tableExists=exists)
         self._send_request("UploadData", params=params)
 
     @staticmethod
     def convert_quick_table(result):
         """Convert the CSV format returned from a quick query to an astropy Table
         ## Arguments
```

### Comparing `mastcasjobs-0.0.5/mastcasjobs.egg-info/PKG-INFO` & `mastcasjobs-0.0.6/mastcasjobs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mastcasjobs
-Version: 0.0.5
+Version: 0.0.6
 Summary: An interface to MAST CasJobs.
 Home-page: https://github.com/rlwastro/mastcasjobs
 Author: Richard L. White
 Author-email: rlw@stsci.edu
 License: MIT
 Platform: OS Independent
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `mastcasjobs-0.0.5/setup.cfg` & `mastcasjobs-0.0.6/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = mastcasjobs
-version = 0.0.5
+version = 0.0.6
 description = An interface to MAST CasJobs.
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 author = Richard L. White
 author_email = rlw@stsci.edu
 url = https://github.com/rlwastro/mastcasjobs
 license = MIT
```


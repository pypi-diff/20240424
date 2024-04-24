# Comparing `tmp/grass_gis_helpers-1.0.0.tar.gz` & `tmp/grass_gis_helpers-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grass_gis_helpers-1.0.0.tar", last modified: Tue Apr  2 10:25:40 2024, max compression
+gzip compressed data, was "grass_gis_helpers-1.1.0.tar", last modified: Wed Apr 24 13:39:11 2024, max compression
```

## Comparing `grass_gis_helpers-1.0.0.tar` & `grass_gis_helpers-1.1.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 10:25:40.456539 grass_gis_helpers-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-04-02 10:25:15.000000 grass_gis_helpers-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-04-02 10:25:40.452539 grass_gis_helpers-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-02 10:25:15.000000 grass_gis_helpers-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      820 2024-04-02 10:25:35.000000 grass_gis_helpers-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 10:25:40.456539 grass_gis_helpers-1.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 10:25:40.448539 grass_gis_helpers-1.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 10:25:40.452539 grass_gis_helpers-1.0.0/src/grass_gis_helpers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 10:25:15.000000 grass_gis_helpers-1.0.0/src/grass_gis_helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4817 2024-04-02 10:25:15.000000 grass_gis_helpers-1.0.0/src/grass_gis_helpers/cleanup.py
--rw-r--r--   0 runner    (1001) docker     (127)    14469 2024-04-02 10:25:15.000000 grass_gis_helpers-1.0.0/src/grass_gis_helpers/data_import.py
--rw-r--r--   0 runner    (1001) docker     (127)     4403 2024-04-02 10:25:15.000000 grass_gis_helpers-1.0.0/src/grass_gis_helpers/general.py
--rw-r--r--   0 runner    (1001) docker     (127)     3349 2024-04-02 10:25:15.000000 grass_gis_helpers-1.0.0/src/grass_gis_helpers/location.py
--rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-04-02 10:25:15.000000 grass_gis_helpers-1.0.0/src/grass_gis_helpers/mapset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 10:25:40.452539 grass_gis_helpers-1.0.0/src/grass_gis_helpers/open_geodata_germany/
--rw-r--r--   0 runner    (1001) docker     (127)     5430 2024-04-02 10:25:15.000000 grass_gis_helpers-1.0.0/src/grass_gis_helpers/open_geodata_germany/download_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     5030 2024-04-02 10:25:15.000000 grass_gis_helpers-1.0.0/src/grass_gis_helpers/open_geodata_germany/federal_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     4021 2024-04-02 10:25:15.000000 grass_gis_helpers-1.0.0/src/grass_gis_helpers/parallel.py
--rw-r--r--   0 runner    (1001) docker     (127)     3625 2024-04-02 10:25:15.000000 grass_gis_helpers-1.0.0/src/grass_gis_helpers/raster.py
--rw-r--r--   0 runner    (1001) docker     (127)     3438 2024-04-02 10:25:15.000000 grass_gis_helpers-1.0.0/src/grass_gis_helpers/tiling.py
--rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-04-02 10:25:15.000000 grass_gis_helpers-1.0.0/src/grass_gis_helpers/validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-04-02 10:25:15.000000 grass_gis_helpers-1.0.0/src/grass_gis_helpers/vector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 10:25:40.452539 grass_gis_helpers-1.0.0/src/grass_gis_helpers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-04-02 10:25:40.000000 grass_gis_helpers-1.0.0/src/grass_gis_helpers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-04-02 10:25:40.000000 grass_gis_helpers-1.0.0/src/grass_gis_helpers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 10:25:40.000000 grass_gis_helpers-1.0.0/src/grass_gis_helpers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-02 10:25:40.000000 grass_gis_helpers-1.0.0/src/grass_gis_helpers.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-02 10:25:40.000000 grass_gis_helpers-1.0.0/src/grass_gis_helpers.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:39:11.945000 grass_gis_helpers-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-04-24 13:38:40.000000 grass_gis_helpers-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-04-24 13:39:11.945000 grass_gis_helpers-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-24 13:38:40.000000 grass_gis_helpers-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      820 2024-04-24 13:39:06.000000 grass_gis_helpers-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 13:39:11.945000 grass_gis_helpers-1.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:39:11.941000 grass_gis_helpers-1.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:39:11.945000 grass_gis_helpers-1.1.0/src/grass_gis_helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 13:38:40.000000 grass_gis_helpers-1.1.0/src/grass_gis_helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4817 2024-04-24 13:38:40.000000 grass_gis_helpers-1.1.0/src/grass_gis_helpers/cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14469 2024-04-24 13:38:40.000000 grass_gis_helpers-1.1.0/src/grass_gis_helpers/data_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4840 2024-04-24 13:38:40.000000 grass_gis_helpers-1.1.0/src/grass_gis_helpers/general.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3349 2024-04-24 13:38:40.000000 grass_gis_helpers-1.1.0/src/grass_gis_helpers/location.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-04-24 13:38:40.000000 grass_gis_helpers-1.1.0/src/grass_gis_helpers/mapset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:39:11.945000 grass_gis_helpers-1.1.0/src/grass_gis_helpers/open_geodata_germany/
+-rw-r--r--   0 runner    (1001) docker     (127)     5707 2024-04-24 13:38:40.000000 grass_gis_helpers-1.1.0/src/grass_gis_helpers/open_geodata_germany/download_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5189 2024-04-24 13:38:40.000000 grass_gis_helpers-1.1.0/src/grass_gis_helpers/open_geodata_germany/federal_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4021 2024-04-24 13:38:40.000000 grass_gis_helpers-1.1.0/src/grass_gis_helpers/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3625 2024-04-24 13:38:40.000000 grass_gis_helpers-1.1.0/src/grass_gis_helpers/raster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3438 2024-04-24 13:38:40.000000 grass_gis_helpers-1.1.0/src/grass_gis_helpers/tiling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-04-24 13:38:40.000000 grass_gis_helpers-1.1.0/src/grass_gis_helpers/validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-04-24 13:38:40.000000 grass_gis_helpers-1.1.0/src/grass_gis_helpers/vector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:39:11.945000 grass_gis_helpers-1.1.0/src/grass_gis_helpers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-04-24 13:39:11.000000 grass_gis_helpers-1.1.0/src/grass_gis_helpers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-04-24 13:39:11.000000 grass_gis_helpers-1.1.0/src/grass_gis_helpers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 13:39:11.000000 grass_gis_helpers-1.1.0/src/grass_gis_helpers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-24 13:39:11.000000 grass_gis_helpers-1.1.0/src/grass_gis_helpers.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-24 13:39:11.000000 grass_gis_helpers-1.1.0/src/grass_gis_helpers.egg-info/top_level.txt
```

### Comparing `grass_gis_helpers-1.0.0/LICENSE` & `grass_gis_helpers-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `grass_gis_helpers-1.0.0/PKG-INFO` & `grass_gis_helpers-1.1.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grass_gis_helpers
-Version: 1.0.0
+Version: 1.1.0
 Summary: This library provides functions which can be used for developing GRASS GIS addons.
 Author-email: Anika Weinmann <weinmann@mundialis.de>
 Maintainer-email: "mundialis GmbH & Co. KG" <info@mundialis.de>
 Project-URL: Homepage, https://github.com/mundialis/grass-gis-helpers
 Project-URL: Bug Tracker, https://github.com/mundialis/grass-gis-helpers/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `grass_gis_helpers-1.0.0/README.md` & `grass_gis_helpers-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `grass_gis_helpers-1.0.0/pyproject.toml` & `grass_gis_helpers-1.1.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "grass_gis_helpers"
-version = "1.0.0"
+version = "1.1.0"
 authors = [
   { name="Anika Weinmann", email="weinmann@mundialis.de" },
 ]
 maintainers = [{name="mundialis GmbH & Co. KG", email="info@mundialis.de"}]
 description = "This library provides functions which can be used for developing GRASS GIS addons."
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `grass_gis_helpers-1.0.0/src/grass_gis_helpers/cleanup.py` & `grass_gis_helpers-1.1.0/src/grass_gis_helpers/cleanup.py`

 * *Files identical despite different names*

### Comparing `grass_gis_helpers-1.0.0/src/grass_gis_helpers/data_import.py` & `grass_gis_helpers-1.1.0/src/grass_gis_helpers/data_import.py`

 * *Files identical despite different names*

### Comparing `grass_gis_helpers-1.0.0/src/grass_gis_helpers/general.py` & `grass_gis_helpers-1.1.0/src/grass_gis_helpers/general.py`

 * *Files 10% similar despite different names*

```diff
@@ -129,7 +129,21 @@
         grass.warning(
             _(f"Using {memory} MB but only {free_ram} MB RAM available.")
         )
         grass.warning(_(f"Set used memory to {free_ram} MB."))
         return free_ram
     else:
         return memory
+
+
+def check_installed_addon(addon, url):
+    """Check if addon is already installed and raise error if not.
+    Args:
+        addon(string): Addon to check if it is installed
+        url(string): Path to addon
+    """
+    if not grass.find_program(addon, "--help"):
+        msg = (
+            f"The '{addon}' module was not found, install  it first:\n"
+            f"g.extension {addon} url={url}"
+        )
+        grass.fatal(_(msg))
```

### Comparing `grass_gis_helpers-1.0.0/src/grass_gis_helpers/location.py` & `grass_gis_helpers-1.1.0/src/grass_gis_helpers/location.py`

 * *Files identical despite different names*

### Comparing `grass_gis_helpers-1.0.0/src/grass_gis_helpers/mapset.py` & `grass_gis_helpers-1.1.0/src/grass_gis_helpers/mapset.py`

 * *Files identical despite different names*

### Comparing `grass_gis_helpers-1.0.0/src/grass_gis_helpers/open_geodata_germany/download_data.py` & `grass_gis_helpers-1.1.0/src/grass_gis_helpers/open_geodata_germany/download_data.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,42 +28,49 @@
 import zipfile_deflate64
 from zipfile import ZipFile
 
 import grass.script as grass
 
 
 def check_download_dir(download_dir):
-    """Checks if download directory is set. If yes, checks if folder exists or
-    creates it. If not set, a temporary directory will be used.
+    """Check if download directory is set. If yes, check if folder exists or
+    create it. If not set, a temporary directory will be used.
 
     Args:
-        download_dir (str): download directory module parameter
+        download_dir (str): Download directory module parameter
     Returns:
         (str): Path to download directory
     """
     if not download_dir:
         download_dir = grass.tempdir()
     else:
         if not os.path.isdir(download_dir):
             grass.message(
                 _(
                     f"Download folder {download_dir} does not exist and will "
                     "be created."
                 )
             )
             os.makedirs(download_dir)
+        elif os.path.exists(download_dir) and os.listdir(download_dir):
+            grass.warning(
+                _(
+                    f"Download folder {download_dir} exists and is not empty. "
+                    "Folder will NOT be deleted."
+                )
+            )
     grass.message(f"Download directory: {download_dir}")
     return download_dir
 
 
 def url_response(url):
     """URL response function which is used by download_data_using_threadpool
 
     Args:
-        url (str): data download url
+        url (str): Data download url
     Return:
         url (str): Return the url for printing
     """
     filename = os.path.basename(url)
     response = requests.get(url, stream=True)
     with open(str(filename), "wb") as f:
         for chunk in response:
```

### Comparing `grass_gis_helpers-1.0.0/src/grass_gis_helpers/open_geodata_germany/federal_state.py` & `grass_gis_helpers-1.1.0/src/grass_gis_helpers/open_geodata_germany/federal_state.py`

 * *Files 3% similar despite different names*

```diff
@@ -122,30 +122,34 @@
 
 
 def get_federal_states(federal_state, federal_state_file):
     """Get federal state and federal state file module parameters and return
     list with federal state abbreviations
 
     Args:
-        federal_state (str): federal state module parameter
-        federal_state_file (str): federal state file module parameter
+        federal_state (str): Federal state module parameter
+        federal_state_file (str): Federal state file module parameter
     Returns:
-        (list): list with federale state abbreviations
+        (list): List with federal state abbreviations
 
     """
     if federal_state_file:
         if not os.path.isfile(federal_state_file):
             grass.fatal(
                 _(
                     "Federal state file is given, but file "
-                    f"<{federal_state_file}> does not exists."
+                    f"<{federal_state_file}> does not exist."
                 )
             )
         with open(federal_state_file) as fs_file:
             fs_list_str = fs_file.read().strip()
+            if fs_list_str == "":
+                grass.fatal(
+                    _("Federal state in <federal_state_file> is empty string!")
+                )
     elif federal_state:
         fs_list_str = federal_state.strip()
     else:
         grass.fatal(
             _(
                 "Neither <federal_state> nor <federal_state_file> are given. "
                 "Please set one of the two."
```

### Comparing `grass_gis_helpers-1.0.0/src/grass_gis_helpers/parallel.py` & `grass_gis_helpers-1.1.0/src/grass_gis_helpers/parallel.py`

 * *Files identical despite different names*

### Comparing `grass_gis_helpers-1.0.0/src/grass_gis_helpers/raster.py` & `grass_gis_helpers-1.1.0/src/grass_gis_helpers/raster.py`

 * *Files identical despite different names*

### Comparing `grass_gis_helpers-1.0.0/src/grass_gis_helpers/tiling.py` & `grass_gis_helpers-1.1.0/src/grass_gis_helpers/tiling.py`

 * *Files identical despite different names*

### Comparing `grass_gis_helpers-1.0.0/src/grass_gis_helpers/validation.py` & `grass_gis_helpers-1.1.0/src/grass_gis_helpers/validation.py`

 * *Files identical despite different names*

### Comparing `grass_gis_helpers-1.0.0/src/grass_gis_helpers/vector.py` & `grass_gis_helpers-1.1.0/src/grass_gis_helpers/vector.py`

 * *Files identical despite different names*

### Comparing `grass_gis_helpers-1.0.0/src/grass_gis_helpers.egg-info/PKG-INFO` & `grass_gis_helpers-1.1.0/src/grass_gis_helpers.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grass_gis_helpers
-Version: 1.0.0
+Version: 1.1.0
 Summary: This library provides functions which can be used for developing GRASS GIS addons.
 Author-email: Anika Weinmann <weinmann@mundialis.de>
 Maintainer-email: "mundialis GmbH & Co. KG" <info@mundialis.de>
 Project-URL: Homepage, https://github.com/mundialis/grass-gis-helpers
 Project-URL: Bug Tracker, https://github.com/mundialis/grass-gis-helpers/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `grass_gis_helpers-1.0.0/src/grass_gis_helpers.egg-info/SOURCES.txt` & `grass_gis_helpers-1.1.0/src/grass_gis_helpers.egg-info/SOURCES.txt`

 * *Files identical despite different names*


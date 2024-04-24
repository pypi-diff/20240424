# Comparing `tmp/pollination-annual-daylight.viz-0.10.8.tar.gz` & `tmp/pollination-annual-daylight.viz-0.10.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pollination-annual-daylight.viz-0.10.8.tar", last modified: Mon Jul 17 12:06:35 2023, max compression
+gzip compressed data, was "pollination-annual-daylight.viz-0.10.9.tar", last modified: Tue Jul 18 11:59:15 2023, max compression
```

## Comparing `pollination-annual-daylight.viz-0.10.8.tar` & `pollination-annual-daylight.viz-0.10.9.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:06:35.798164 pollination-annual-daylight.viz-0.10.8/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:06:35.798164 pollination-annual-daylight.viz-0.10.8/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-07-17 12:05:53.000000 pollination-annual-daylight.viz-0.10.8/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:06:35.798164 pollination-annual-daylight.viz-0.10.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     6691 2023-07-17 12:05:53.000000 pollination-annual-daylight.viz-0.10.8/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-17 12:05:53.000000 pollination-annual-daylight.viz-0.10.8/.github/workflows/tests.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-07-17 12:05:53.000000 pollination-annual-daylight.viz-0.10.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-17 12:05:53.000000 pollination-annual-daylight.viz-0.10.8/.releaserc.json
--rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-07-17 12:05:53.000000 pollination-annual-daylight.viz-0.10.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-07-17 12:06:35.798164 pollination-annual-daylight.viz-0.10.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-07-17 12:05:53.000000 pollination-annual-daylight.viz-0.10.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-17 12:05:53.000000 pollination-annual-daylight.viz-0.10.8/deploy.sh
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-17 12:05:53.000000 pollination-annual-daylight.viz-0.10.8/dev-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-17 12:05:53.000000 pollination-annual-daylight.viz-0.10.8/extras-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:06:35.794164 pollination-annual-daylight.viz-0.10.8/pollination/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:06:35.798164 pollination-annual-daylight.viz-0.10.8/pollination/annual_daylight/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-17 12:05:53.000000 pollination-annual-daylight.viz-0.10.8/pollination/annual_daylight/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-07-17 12:05:53.000000 pollination-annual-daylight.viz-0.10.8/pollination/annual_daylight/_post_process.py
--rw-r--r--   0 runner    (1001) docker     (123)     6308 2023-07-17 12:05:53.000000 pollination-annual-daylight.viz-0.10.8/pollination/annual_daylight/_prepare_folder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3630 2023-07-17 12:05:53.000000 pollination-annual-daylight.viz-0.10.8/pollination/annual_daylight/_raytracing.py
--rw-r--r--   0 runner    (1001) docker     (123)     8578 2023-07-17 12:05:53.000000 pollination-annual-daylight.viz-0.10.8/pollination/annual_daylight/entry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:06:35.798164 pollination-annual-daylight.viz-0.10.8/pollination_annual_daylight.viz.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-07-17 12:06:35.000000 pollination-annual-daylight.viz-0.10.8/pollination_annual_daylight.viz.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-07-17 12:06:35.000000 pollination-annual-daylight.viz-0.10.8/pollination_annual_daylight.viz.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 12:06:35.000000 pollination-annual-daylight.viz-0.10.8/pollination_annual_daylight.viz.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 12:06:35.000000 pollination-annual-daylight.viz-0.10.8/pollination_annual_daylight.viz.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-17 12:06:35.000000 pollination-annual-daylight.viz-0.10.8/pollination_annual_daylight.viz.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-17 12:06:35.000000 pollination-annual-daylight.viz-0.10.8/pollination_annual_daylight.viz.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-17 12:05:53.000000 pollination-annual-daylight.viz-0.10.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-17 12:06:35.798164 pollination-annual-daylight.viz-0.10.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-07-17 12:05:53.000000 pollination-annual-daylight.viz-0.10.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:06:35.798164 pollination-annual-daylight.viz-0.10.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 12:05:53.000000 pollination-annual-daylight.viz-0.10.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-07-17 12:05:53.000000 pollination-annual-daylight.viz-0.10.8/tests/validation_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:59:15.985600 pollination-annual-daylight.viz-0.10.9/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:59:15.981600 pollination-annual-daylight.viz-0.10.9/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-07-18 11:58:27.000000 pollination-annual-daylight.viz-0.10.9/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:59:15.981600 pollination-annual-daylight.viz-0.10.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     6691 2023-07-18 11:58:27.000000 pollination-annual-daylight.viz-0.10.9/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-18 11:58:27.000000 pollination-annual-daylight.viz-0.10.9/.github/workflows/tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-07-18 11:58:27.000000 pollination-annual-daylight.viz-0.10.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-18 11:58:27.000000 pollination-annual-daylight.viz-0.10.9/.releaserc.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-07-18 11:58:27.000000 pollination-annual-daylight.viz-0.10.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-07-18 11:59:15.985600 pollination-annual-daylight.viz-0.10.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-07-18 11:58:27.000000 pollination-annual-daylight.viz-0.10.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-18 11:58:27.000000 pollination-annual-daylight.viz-0.10.9/deploy.sh
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-18 11:58:27.000000 pollination-annual-daylight.viz-0.10.9/dev-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-18 11:58:27.000000 pollination-annual-daylight.viz-0.10.9/extras-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:59:15.973600 pollination-annual-daylight.viz-0.10.9/pollination/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:59:15.981600 pollination-annual-daylight.viz-0.10.9/pollination/annual_daylight/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-18 11:58:27.000000 pollination-annual-daylight.viz-0.10.9/pollination/annual_daylight/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-07-18 11:58:27.000000 pollination-annual-daylight.viz-0.10.9/pollination/annual_daylight/_post_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6345 2023-07-18 11:58:27.000000 pollination-annual-daylight.viz-0.10.9/pollination/annual_daylight/_prepare_folder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3630 2023-07-18 11:58:27.000000 pollination-annual-daylight.viz-0.10.9/pollination/annual_daylight/_raytracing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8578 2023-07-18 11:58:27.000000 pollination-annual-daylight.viz-0.10.9/pollination/annual_daylight/entry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:59:15.985600 pollination-annual-daylight.viz-0.10.9/pollination_annual_daylight.viz.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-07-18 11:59:15.000000 pollination-annual-daylight.viz-0.10.9/pollination_annual_daylight.viz.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-07-18 11:59:15.000000 pollination-annual-daylight.viz-0.10.9/pollination_annual_daylight.viz.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 11:59:15.000000 pollination-annual-daylight.viz-0.10.9/pollination_annual_daylight.viz.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 11:59:15.000000 pollination-annual-daylight.viz-0.10.9/pollination_annual_daylight.viz.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-18 11:59:15.000000 pollination-annual-daylight.viz-0.10.9/pollination_annual_daylight.viz.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-18 11:59:15.000000 pollination-annual-daylight.viz-0.10.9/pollination_annual_daylight.viz.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-18 11:58:27.000000 pollination-annual-daylight.viz-0.10.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-18 11:59:15.985600 pollination-annual-daylight.viz-0.10.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-07-18 11:58:27.000000 pollination-annual-daylight.viz-0.10.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:59:15.985600 pollination-annual-daylight.viz-0.10.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 11:58:27.000000 pollination-annual-daylight.viz-0.10.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-07-18 11:58:27.000000 pollination-annual-daylight.viz-0.10.9/tests/validation_test.py
```

### Comparing `pollination-annual-daylight.viz-0.10.8/.github/workflows/ci.yaml` & `pollination-annual-daylight.viz-0.10.9/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `pollination-annual-daylight.viz-0.10.8/.github/workflows/tests.yaml` & `pollination-annual-daylight.viz-0.10.9/.github/workflows/tests.yaml`

 * *Files identical despite different names*

### Comparing `pollination-annual-daylight.viz-0.10.8/LICENSE` & `pollination-annual-daylight.viz-0.10.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pollination-annual-daylight.viz-0.10.8/PKG-INFO` & `pollination-annual-daylight.viz-0.10.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pollination-annual-daylight.viz
-Version: 0.10.8
+Version: 0.10.9
 Summary: Annual daylight recipe for Pollination.
 Home-page: https://github.com/pollination/annual-daylight
 Author: ladybug-tools
 Author-email: info@ladybug.tools
 Maintainer: mostapha, ladybug-tools
 Maintainer-email: mostapha@ladybug.tools, info@ladybug.tools
 License: PolyForm Shield License 1.0.0, https://polyformproject.org/wp-content/uploads/2020/06/PolyForm-Shield-1.0.0.txt
```

### Comparing `pollination-annual-daylight.viz-0.10.8/README.md` & `pollination-annual-daylight.viz-0.10.9/README.md`

 * *Files identical despite different names*

### Comparing `pollination-annual-daylight.viz-0.10.8/pollination/annual_daylight/_post_process.py` & `pollination-annual-daylight.viz-0.10.9/pollination/annual_daylight/_post_process.py`

 * *Files identical despite different names*

### Comparing `pollination-annual-daylight.viz-0.10.8/pollination/annual_daylight/_prepare_folder.py` & `pollination-annual-daylight.viz-0.10.9/pollination/annual_daylight/_prepare_folder.py`

 * *Files 2% similar despite different names*

```diff
@@ -165,9 +165,9 @@
     )
 
     results = Outputs.folder(
         source='results', description='results folder.'
     )
 
     sensor_grids = Outputs.list(
-        source='resources/grid/_info.json'
+        source='resources/grid/_info.json', description='list of sensor grids.'
     )
```

### Comparing `pollination-annual-daylight.viz-0.10.8/pollination/annual_daylight/_raytracing.py` & `pollination-annual-daylight.viz-0.10.9/pollination/annual_daylight/_raytracing.py`

 * *Files identical despite different names*

### Comparing `pollination-annual-daylight.viz-0.10.8/pollination/annual_daylight/entry.py` & `pollination-annual-daylight.viz-0.10.9/pollination/annual_daylight/entry.py`

 * *Files identical despite different names*

### Comparing `pollination-annual-daylight.viz-0.10.8/pollination_annual_daylight.viz.egg-info/PKG-INFO` & `pollination-annual-daylight.viz-0.10.9/pollination_annual_daylight.viz.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pollination-annual-daylight.viz
-Version: 0.10.8
+Version: 0.10.9
 Summary: Annual daylight recipe for Pollination.
 Home-page: https://github.com/pollination/annual-daylight
 Author: ladybug-tools
 Author-email: info@ladybug.tools
 Maintainer: mostapha, ladybug-tools
 Maintainer-email: mostapha@ladybug.tools, info@ladybug.tools
 License: PolyForm Shield License 1.0.0, https://polyformproject.org/wp-content/uploads/2020/06/PolyForm-Shield-1.0.0.txt
```

### Comparing `pollination-annual-daylight.viz-0.10.8/pollination_annual_daylight.viz.egg-info/SOURCES.txt` & `pollination-annual-daylight.viz-0.10.9/pollination_annual_daylight.viz.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pollination-annual-daylight.viz-0.10.8/setup.py` & `pollination-annual-daylight.viz-0.10.9/setup.py`

 * *Files identical despite different names*


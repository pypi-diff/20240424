# Comparing `tmp/gardener_cicd_dso-1.2382.0.tar.gz` & `tmp/gardener_cicd_dso-1.2383.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gardener_cicd_dso-1.2382.0.tar", last modified: Fri Apr 19 14:51:34 2024, max compression
+gzip compressed data, was "gardener_cicd_dso-1.2383.0.tar", last modified: Wed Apr 24 11:09:18 2024, max compression
```

## Comparing `gardener_cicd_dso-1.2382.0.tar` & `gardener_cicd_dso-1.2383.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 14:51:34.780177 gardener_cicd_dso-1.2382.0/
--rw-r--r--   0 root         (0) root         (0)    11357 2024-04-19 13:05:37.000000 gardener_cicd_dso-1.2382.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      211 2024-04-19 14:51:34.780177 gardener_cicd_dso-1.2382.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2093 2024-04-19 13:05:37.000000 gardener_cicd_dso-1.2382.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 14:51:34.776177 gardener_cicd_dso-1.2382.0/checkmarx/
--rw-r--r--   0 root         (0) root         (0)      132 2024-04-19 13:05:37.000000 gardener_cicd_dso-1.2382.0/checkmarx/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7945 2024-04-19 13:05:37.000000 gardener_cicd_dso-1.2382.0/checkmarx/client.py
--rw-r--r--   0 root         (0) root         (0)     3746 2024-04-19 13:05:37.000000 gardener_cicd_dso-1.2382.0/checkmarx/model.py
--rw-r--r--   0 root         (0) root         (0)     7033 2024-04-19 13:05:37.000000 gardener_cicd_dso-1.2382.0/checkmarx/project.py
--rw-r--r--   0 root         (0) root         (0)     5790 2024-04-19 13:05:37.000000 gardener_cicd_dso-1.2382.0/checkmarx/tablefmt.py
--rw-r--r--   0 root         (0) root         (0)    19358 2024-04-19 13:05:37.000000 gardener_cicd_dso-1.2382.0/checkmarx/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 14:51:34.776177 gardener_cicd_dso-1.2382.0/clamav/
--rw-r--r--   0 root         (0) root         (0)      132 2024-04-19 13:05:37.000000 gardener_cicd_dso-1.2382.0/clamav/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4680 2024-04-19 13:05:37.000000 gardener_cicd_dso-1.2382.0/clamav/client.py
--rw-r--r--   0 root         (0) root         (0)     8345 2024-04-19 13:05:37.000000 gardener_cicd_dso-1.2382.0/clamav/cnudie.py
--rw-r--r--   0 root         (0) root         (0)     2252 2024-04-19 13:05:37.000000 gardener_cicd_dso-1.2382.0/clamav/model.py
--rw-r--r--   0 root         (0) root         (0)     1902 2024-04-19 13:05:37.000000 gardener_cicd_dso-1.2382.0/clamav/report.py
--rw-r--r--   0 root         (0) root         (0)     1083 2024-04-19 13:05:37.000000 gardener_cicd_dso-1.2382.0/clamav/routes.py
--rw-r--r--   0 root         (0) root         (0)     7469 2024-04-19 13:05:37.000000 gardener_cicd_dso-1.2382.0/clamav/scan.py
--rw-r--r--   0 root         (0) root         (0)     5564 2024-04-19 13:05:37.000000 gardener_cicd_dso-1.2382.0/clamav/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 14:51:34.780177 gardener_cicd_dso-1.2382.0/gardener_cicd_dso.egg-info/
--rw-r--r--   0 root         (0) root         (0)      211 2024-04-19 14:51:34.000000 gardener_cicd_dso-1.2382.0/gardener_cicd_dso.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      670 2024-04-19 14:51:34.000000 gardener_cicd_dso-1.2382.0/gardener_cicd_dso.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-19 14:51:34.000000 gardener_cicd_dso-1.2382.0/gardener_cicd_dso.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       37 2024-04-19 14:51:34.000000 gardener_cicd_dso-1.2382.0/gardener_cicd_dso.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       27 2024-04-19 14:51:34.000000 gardener_cicd_dso-1.2382.0/gardener_cicd_dso.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 14:51:34.780177 gardener_cicd_dso-1.2382.0/protecode/
--rw-r--r--   0 root         (0) root         (0)      132 2024-04-19 13:05:37.000000 gardener_cicd_dso-1.2382.0/protecode/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7653 2024-04-19 13:05:37.000000 gardener_cicd_dso-1.2382.0/protecode/assessments.py
--rw-r--r--   0 root         (0) root         (0)    17319 2024-04-19 13:05:37.000000 gardener_cicd_dso-1.2382.0/protecode/client.py
--rw-r--r--   0 root         (0) root         (0)    10709 2024-04-19 13:05:37.000000 gardener_cicd_dso-1.2382.0/protecode/model.py
--rw-r--r--   0 root         (0) root         (0)     3636 2024-04-19 13:05:37.000000 gardener_cicd_dso-1.2382.0/protecode/rescore.py
--rw-r--r--   0 root         (0) root         (0)    29221 2024-04-19 13:05:37.000000 gardener_cicd_dso-1.2382.0/protecode/scanning.py
--rw-r--r--   0 root         (0) root         (0)     9178 2024-04-19 13:05:37.000000 gardener_cicd_dso-1.2382.0/protecode/util.py
--rw-r--r--   0 root         (0) root         (0)      359 2024-04-19 13:05:37.000000 gardener_cicd_dso-1.2382.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)      174 2024-04-19 14:51:34.780177 gardener_cicd_dso-1.2382.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      673 2024-04-19 13:05:37.000000 gardener_cicd_dso-1.2382.0/setup.dso.py
--rw-r--r--   0 root         (0) root         (0)     2174 2024-04-19 13:05:37.000000 gardener_cicd_dso-1.2382.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 11:09:18.489871 gardener_cicd_dso-1.2383.0/
+-rw-r--r--   0 root         (0) root         (0)    11357 2024-04-24 11:08:33.000000 gardener_cicd_dso-1.2383.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      211 2024-04-24 11:09:18.489871 gardener_cicd_dso-1.2383.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2093 2024-04-24 11:08:33.000000 gardener_cicd_dso-1.2383.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 11:09:18.485871 gardener_cicd_dso-1.2383.0/checkmarx/
+-rw-r--r--   0 root         (0) root         (0)      132 2024-04-24 11:08:33.000000 gardener_cicd_dso-1.2383.0/checkmarx/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7945 2024-04-24 11:08:33.000000 gardener_cicd_dso-1.2383.0/checkmarx/client.py
+-rw-r--r--   0 root         (0) root         (0)     3746 2024-04-24 11:08:33.000000 gardener_cicd_dso-1.2383.0/checkmarx/model.py
+-rw-r--r--   0 root         (0) root         (0)     7033 2024-04-24 11:08:33.000000 gardener_cicd_dso-1.2383.0/checkmarx/project.py
+-rw-r--r--   0 root         (0) root         (0)     5790 2024-04-24 11:08:33.000000 gardener_cicd_dso-1.2383.0/checkmarx/tablefmt.py
+-rw-r--r--   0 root         (0) root         (0)    19358 2024-04-24 11:08:33.000000 gardener_cicd_dso-1.2383.0/checkmarx/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 11:09:18.489871 gardener_cicd_dso-1.2383.0/clamav/
+-rw-r--r--   0 root         (0) root         (0)      132 2024-04-24 11:08:33.000000 gardener_cicd_dso-1.2383.0/clamav/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4680 2024-04-24 11:08:33.000000 gardener_cicd_dso-1.2383.0/clamav/client.py
+-rw-r--r--   0 root         (0) root         (0)     8427 2024-04-24 11:08:33.000000 gardener_cicd_dso-1.2383.0/clamav/cnudie.py
+-rw-r--r--   0 root         (0) root         (0)     2252 2024-04-24 11:08:33.000000 gardener_cicd_dso-1.2383.0/clamav/model.py
+-rw-r--r--   0 root         (0) root         (0)     1902 2024-04-24 11:08:33.000000 gardener_cicd_dso-1.2383.0/clamav/report.py
+-rw-r--r--   0 root         (0) root         (0)     1083 2024-04-24 11:08:33.000000 gardener_cicd_dso-1.2383.0/clamav/routes.py
+-rw-r--r--   0 root         (0) root         (0)     7469 2024-04-24 11:08:33.000000 gardener_cicd_dso-1.2383.0/clamav/scan.py
+-rw-r--r--   0 root         (0) root         (0)     5564 2024-04-24 11:08:33.000000 gardener_cicd_dso-1.2383.0/clamav/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 11:09:18.489871 gardener_cicd_dso-1.2383.0/gardener_cicd_dso.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      211 2024-04-24 11:09:18.000000 gardener_cicd_dso-1.2383.0/gardener_cicd_dso.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      670 2024-04-24 11:09:18.000000 gardener_cicd_dso-1.2383.0/gardener_cicd_dso.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-24 11:09:18.000000 gardener_cicd_dso-1.2383.0/gardener_cicd_dso.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       37 2024-04-24 11:09:18.000000 gardener_cicd_dso-1.2383.0/gardener_cicd_dso.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       27 2024-04-24 11:09:18.000000 gardener_cicd_dso-1.2383.0/gardener_cicd_dso.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 11:09:18.489871 gardener_cicd_dso-1.2383.0/protecode/
+-rw-r--r--   0 root         (0) root         (0)      132 2024-04-24 11:08:33.000000 gardener_cicd_dso-1.2383.0/protecode/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7653 2024-04-24 11:08:33.000000 gardener_cicd_dso-1.2383.0/protecode/assessments.py
+-rw-r--r--   0 root         (0) root         (0)    17319 2024-04-24 11:08:33.000000 gardener_cicd_dso-1.2383.0/protecode/client.py
+-rw-r--r--   0 root         (0) root         (0)    10709 2024-04-24 11:08:33.000000 gardener_cicd_dso-1.2383.0/protecode/model.py
+-rw-r--r--   0 root         (0) root         (0)     3636 2024-04-24 11:08:33.000000 gardener_cicd_dso-1.2383.0/protecode/rescore.py
+-rw-r--r--   0 root         (0) root         (0)    29221 2024-04-24 11:08:33.000000 gardener_cicd_dso-1.2383.0/protecode/scanning.py
+-rw-r--r--   0 root         (0) root         (0)     9178 2024-04-24 11:08:33.000000 gardener_cicd_dso-1.2383.0/protecode/util.py
+-rw-r--r--   0 root         (0) root         (0)      359 2024-04-24 11:08:33.000000 gardener_cicd_dso-1.2383.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)      174 2024-04-24 11:09:18.489871 gardener_cicd_dso-1.2383.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      673 2024-04-24 11:08:33.000000 gardener_cicd_dso-1.2383.0/setup.dso.py
+-rw-r--r--   0 root         (0) root         (0)     2174 2024-04-24 11:08:33.000000 gardener_cicd_dso-1.2383.0/setup.py
```

### Comparing `gardener_cicd_dso-1.2382.0/LICENSE` & `gardener_cicd_dso-1.2383.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gardener_cicd_dso-1.2382.0/README.md` & `gardener_cicd_dso-1.2383.0/README.md`

 * *Files identical despite different names*

### Comparing `gardener_cicd_dso-1.2382.0/checkmarx/client.py` & `gardener_cicd_dso-1.2383.0/checkmarx/client.py`

 * *Files identical despite different names*

### Comparing `gardener_cicd_dso-1.2382.0/checkmarx/model.py` & `gardener_cicd_dso-1.2383.0/checkmarx/model.py`

 * *Files identical despite different names*

### Comparing `gardener_cicd_dso-1.2382.0/checkmarx/project.py` & `gardener_cicd_dso-1.2383.0/checkmarx/project.py`

 * *Files identical despite different names*

### Comparing `gardener_cicd_dso-1.2382.0/checkmarx/tablefmt.py` & `gardener_cicd_dso-1.2383.0/checkmarx/tablefmt.py`

 * *Files identical despite different names*

### Comparing `gardener_cicd_dso-1.2382.0/checkmarx/util.py` & `gardener_cicd_dso-1.2383.0/checkmarx/util.py`

 * *Files identical despite different names*

### Comparing `gardener_cicd_dso-1.2382.0/clamav/client.py` & `gardener_cicd_dso-1.2383.0/clamav/client.py`

 * *Files identical despite different names*

### Comparing `gardener_cicd_dso-1.2382.0/clamav/cnudie.py` & `gardener_cicd_dso-1.2383.0/clamav/cnudie.py`

 * *Files 1% similar despite different names*

```diff
@@ -206,14 +206,15 @@
 
 def resource_scan_result_to_artefact_metadata(
     resource_scan_result: clamav.model.ClamAVResourceScanResult,
     datasource: str = dso.model.Datasource.CLAMAV,
     datatype: str = dso.model.Datatype.MALWARE,
     creation_date: datetime.datetime = datetime.datetime.now(),
 ) -> dso.model.ArtefactMetadata:
+    discovery_date = datetime.date.today()
 
     artefact = github.compliance.model.artifact_from_node(resource_scan_result.scanned_element)
     artefact_ref = dso.model.component_artefact_id_from_ocm(
         component=resource_scan_result.scanned_element.component,
         artefact=artefact,
     )
 
@@ -240,8 +241,9 @@
         )
     )
 
     return dso.model.ArtefactMetadata(
         artefact=artefact_ref,
         meta=meta,
         data=finding,
+        discovery_date=discovery_date,
     )
```

### Comparing `gardener_cicd_dso-1.2382.0/clamav/model.py` & `gardener_cicd_dso-1.2383.0/clamav/model.py`

 * *Files identical despite different names*

### Comparing `gardener_cicd_dso-1.2382.0/clamav/report.py` & `gardener_cicd_dso-1.2383.0/clamav/report.py`

 * *Files identical despite different names*

### Comparing `gardener_cicd_dso-1.2382.0/clamav/routes.py` & `gardener_cicd_dso-1.2383.0/clamav/routes.py`

 * *Files identical despite different names*

### Comparing `gardener_cicd_dso-1.2382.0/clamav/scan.py` & `gardener_cicd_dso-1.2383.0/clamav/scan.py`

 * *Files identical despite different names*

### Comparing `gardener_cicd_dso-1.2382.0/clamav/util.py` & `gardener_cicd_dso-1.2383.0/clamav/util.py`

 * *Files identical despite different names*

### Comparing `gardener_cicd_dso-1.2382.0/gardener_cicd_dso.egg-info/SOURCES.txt` & `gardener_cicd_dso-1.2383.0/gardener_cicd_dso.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gardener_cicd_dso-1.2382.0/protecode/assessments.py` & `gardener_cicd_dso-1.2383.0/protecode/assessments.py`

 * *Files identical despite different names*

### Comparing `gardener_cicd_dso-1.2382.0/protecode/client.py` & `gardener_cicd_dso-1.2383.0/protecode/client.py`

 * *Files identical despite different names*

### Comparing `gardener_cicd_dso-1.2382.0/protecode/model.py` & `gardener_cicd_dso-1.2383.0/protecode/model.py`

 * *Files identical despite different names*

### Comparing `gardener_cicd_dso-1.2382.0/protecode/rescore.py` & `gardener_cicd_dso-1.2383.0/protecode/rescore.py`

 * *Files identical despite different names*

### Comparing `gardener_cicd_dso-1.2382.0/protecode/scanning.py` & `gardener_cicd_dso-1.2383.0/protecode/scanning.py`

 * *Files identical despite different names*

### Comparing `gardener_cicd_dso-1.2382.0/protecode/util.py` & `gardener_cicd_dso-1.2383.0/protecode/util.py`

 * *Files identical despite different names*

### Comparing `gardener_cicd_dso-1.2382.0/setup.dso.py` & `gardener_cicd_dso-1.2383.0/setup.dso.py`

 * *Files identical despite different names*

### Comparing `gardener_cicd_dso-1.2382.0/setup.py` & `gardener_cicd_dso-1.2383.0/setup.py`

 * *Files identical despite different names*


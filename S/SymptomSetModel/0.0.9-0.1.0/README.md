# Comparing `tmp/SymptomSetModel-0.0.9.tar.gz` & `tmp/SymptomSetModel-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SymptomSetModel-0.0.9.tar", last modified: Sun Apr 21 20:23:08 2024, max compression
+gzip compressed data, was "SymptomSetModel-0.1.0.tar", last modified: Wed Apr 24 01:12:07 2024, max compression
```

## Comparing `SymptomSetModel-0.0.9.tar` & `SymptomSetModel-0.1.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 davidblair   (501) staff       (20)        0 2024-04-21 20:23:08.032580 SymptomSetModel-0.0.9/
--rw-r--r--   0 davidblair   (501) staff       (20)      474 2024-04-21 20:23:08.032431 SymptomSetModel-0.0.9/PKG-INFO
--rw-r--r--   0 davidblair   (501) staff       (20)      164 2023-11-26 23:59:41.000000 SymptomSetModel-0.0.9/README.md
-drwxr-xr-x   0 davidblair   (501) staff       (20)        0 2024-04-21 20:23:08.031435 SymptomSetModel-0.0.9/SymptomSetModel/
--rw-r--r--   0 davidblair   (501) staff       (20)    10396 2024-04-02 21:43:22.000000 SymptomSetModel-0.0.9/SymptomSetModel/AffectedModel.py
--rw-r--r--   0 davidblair   (501) staff       (20)    21383 2024-04-02 20:50:29.000000 SymptomSetModel-0.0.9/SymptomSetModel/BackgroundModels.py
--rw-r--r--   0 davidblair   (501) staff       (20)     4603 2024-03-28 05:37:03.000000 SymptomSetModel-0.0.9/SymptomSetModel/InferenceDataStruct.py
--rw-r--r--   0 davidblair   (501) staff       (20)    32741 2024-04-21 20:20:53.000000 SymptomSetModel-0.0.9/SymptomSetModel/SymptomSetModel.py
--rw-r--r--   0 davidblair   (501) staff       (20)       73 2023-11-28 05:25:06.000000 SymptomSetModel-0.0.9/SymptomSetModel/__init__.py
-drwxr-xr-x   0 davidblair   (501) staff       (20)        0 2024-04-21 20:23:08.032210 SymptomSetModel-0.0.9/SymptomSetModel.egg-info/
--rw-r--r--   0 davidblair   (501) staff       (20)      474 2024-04-21 20:23:07.000000 SymptomSetModel-0.0.9/SymptomSetModel.egg-info/PKG-INFO
--rw-r--r--   0 davidblair   (501) staff       (20)      383 2024-04-21 20:23:08.000000 SymptomSetModel-0.0.9/SymptomSetModel.egg-info/SOURCES.txt
--rw-r--r--   0 davidblair   (501) staff       (20)        1 2024-04-21 20:23:07.000000 SymptomSetModel-0.0.9/SymptomSetModel.egg-info/dependency_links.txt
--rw-r--r--   0 davidblair   (501) staff       (20)       85 2024-04-21 20:23:07.000000 SymptomSetModel-0.0.9/SymptomSetModel.egg-info/requires.txt
--rw-r--r--   0 davidblair   (501) staff       (20)       16 2024-04-21 20:23:07.000000 SymptomSetModel-0.0.9/SymptomSetModel.egg-info/top_level.txt
--rw-r--r--   0 davidblair   (501) staff       (20)       38 2024-04-21 20:23:08.032618 SymptomSetModel-0.0.9/setup.cfg
--rw-r--r--   0 davidblair   (501) staff       (20)     1036 2024-04-21 20:22:19.000000 SymptomSetModel-0.0.9/setup.py
+drwxr-xr-x   0 davidblair   (501) staff       (20)        0 2024-04-24 01:12:07.603472 SymptomSetModel-0.1.0/
+-rw-r--r--   0 davidblair   (501) staff       (20)      474 2024-04-24 01:12:07.603340 SymptomSetModel-0.1.0/PKG-INFO
+-rw-r--r--   0 davidblair   (501) staff       (20)      164 2023-11-26 23:59:41.000000 SymptomSetModel-0.1.0/README.md
+drwxr-xr-x   0 davidblair   (501) staff       (20)        0 2024-04-24 01:12:07.602329 SymptomSetModel-0.1.0/SymptomSetModel/
+-rw-r--r--   0 davidblair   (501) staff       (20)    10396 2024-04-02 21:43:22.000000 SymptomSetModel-0.1.0/SymptomSetModel/AffectedModel.py
+-rw-r--r--   0 davidblair   (501) staff       (20)    21398 2024-04-24 01:05:42.000000 SymptomSetModel-0.1.0/SymptomSetModel/BackgroundModels.py
+-rw-r--r--   0 davidblair   (501) staff       (20)     4603 2024-03-28 05:37:03.000000 SymptomSetModel-0.1.0/SymptomSetModel/InferenceDataStruct.py
+-rw-r--r--   0 davidblair   (501) staff       (20)    32741 2024-04-24 01:07:09.000000 SymptomSetModel-0.1.0/SymptomSetModel/SymptomSetModel.py
+-rw-r--r--   0 davidblair   (501) staff       (20)       73 2023-11-28 05:25:06.000000 SymptomSetModel-0.1.0/SymptomSetModel/__init__.py
+drwxr-xr-x   0 davidblair   (501) staff       (20)        0 2024-04-24 01:12:07.603145 SymptomSetModel-0.1.0/SymptomSetModel.egg-info/
+-rw-r--r--   0 davidblair   (501) staff       (20)      474 2024-04-24 01:12:07.000000 SymptomSetModel-0.1.0/SymptomSetModel.egg-info/PKG-INFO
+-rw-r--r--   0 davidblair   (501) staff       (20)      383 2024-04-24 01:12:07.000000 SymptomSetModel-0.1.0/SymptomSetModel.egg-info/SOURCES.txt
+-rw-r--r--   0 davidblair   (501) staff       (20)        1 2024-04-24 01:12:07.000000 SymptomSetModel-0.1.0/SymptomSetModel.egg-info/dependency_links.txt
+-rw-r--r--   0 davidblair   (501) staff       (20)       85 2024-04-24 01:12:07.000000 SymptomSetModel-0.1.0/SymptomSetModel.egg-info/requires.txt
+-rw-r--r--   0 davidblair   (501) staff       (20)       16 2024-04-24 01:12:07.000000 SymptomSetModel-0.1.0/SymptomSetModel.egg-info/top_level.txt
+-rw-r--r--   0 davidblair   (501) staff       (20)       38 2024-04-24 01:12:07.603510 SymptomSetModel-0.1.0/setup.cfg
+-rw-r--r--   0 davidblair   (501) staff       (20)     1036 2024-04-21 20:22:19.000000 SymptomSetModel-0.1.0/setup.py
```

### Comparing `SymptomSetModel-0.0.9/SymptomSetModel/AffectedModel.py` & `SymptomSetModel-0.1.0/SymptomSetModel/AffectedModel.py`

 * *Files identical despite different names*

### Comparing `SymptomSetModel-0.0.9/SymptomSetModel/BackgroundModels.py` & `SymptomSetModel-0.1.0/SymptomSetModel/BackgroundModels.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,16 +57,16 @@
 			DxArray=DxArray.reshape(1,-1)
 
 		assert len(set(SymptomColumns).intersection(self.SymptomPresentWeights.index))>0,"DxArray must contain some symptom overlap with IndependentBackground model."
 		SymptomColumns=list(SymptomColumns)
 		new_symptom_columns = list(set(SymptomColumns).intersection(self.SymptomPresentWeights.index))
 		new_dx_array = DxArray[:,[SymptomColumns.index(s) for s in new_symptom_columns]]
 
-		if isinstance(DxArray,sparse.csr_matrix):
-			DxArray=DxArray.toarray()
+		if isinstance(new_dx_array,sparse.csr_matrix):
+			new_dx_array=new_dx_array.toarray()
 
 		pos_weight_vec = np.array([self.SymptomPresentWeights[s] for s in new_symptom_columns])
 		neg_weight_vec = np.array([self.SymptomAbsentWeights[s] for s in new_symptom_columns])
 
 		pos_component = (pos_weight_vec*new_dx_array).sum(axis=1)
 		neg_component = (neg_weight_vec*(1-new_dx_array)).sum(axis=1)
 		return pos_component+neg_component
```

### Comparing `SymptomSetModel-0.0.9/SymptomSetModel/InferenceDataStruct.py` & `SymptomSetModel-0.1.0/SymptomSetModel/InferenceDataStruct.py`

 * *Files identical despite different names*

### Comparing `SymptomSetModel-0.0.9/SymptomSetModel/SymptomSetModel.py` & `SymptomSetModel-0.1.0/SymptomSetModel/SymptomSetModel.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 
 
 
 SMALL_FLOAT=np.finfo(np.float64).eps
 MINLOG = -300.0
 
-__version__ = "0.0.9"
+__version__ = "0.1.0"
 
 
 
 class SymptomaticDiseaseModel:
 
 	def _convert_bounds_to_beta_prior(self,lower_bound,upper_bound,CI=0.99,tol=1e-8):
 		mean=lower_bound+(upper_bound-lower_bound)/2.0
```

### Comparing `SymptomSetModel-0.0.9/setup.py` & `SymptomSetModel-0.1.0/setup.py`

 * *Files identical despite different names*


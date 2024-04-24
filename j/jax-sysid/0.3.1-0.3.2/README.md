# Comparing `tmp/jax-sysid-0.3.1.tar.gz` & `tmp/jax_sysid-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jax-sysid-0.3.1.tar", last modified: Mon Apr  8 20:24:26 2024, max compression
+gzip compressed data, was "jax_sysid-0.3.2.tar", last modified: Wed Apr 24 13:49:30 2024, max compression
```

## Comparing `jax-sysid-0.3.1.tar` & `jax_sysid-0.3.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 bemporad   (501) staff       (20)        0 2024-04-08 20:24:26.389467 jax-sysid-0.3.1/
--rw-r--r--   0 bemporad   (501) staff       (20)    11345 2024-03-01 16:55:21.000000 jax-sysid-0.3.1/LICENSE.txt
--rw-r--r--   0 bemporad   (501) staff       (20)    12952 2024-04-08 20:24:26.389233 jax-sysid-0.3.1/PKG-INFO
--rw-r--r--   0 bemporad   (501) staff       (20)    12152 2024-03-07 06:02:39.000000 jax-sysid-0.3.1/README.md
--rw-r--r--   0 bemporad   (501) staff       (20)      801 2024-04-08 20:18:23.000000 jax-sysid-0.3.1/pyproject.toml
--rw-r--r--   0 bemporad   (501) staff       (20)       38 2024-04-08 20:24:26.389503 jax-sysid-0.3.1/setup.cfg
-drwxr-xr-x   0 bemporad   (501) staff       (20)        0 2024-04-08 20:24:26.387355 jax-sysid-0.3.1/src/
-drwxr-xr-x   0 bemporad   (501) staff       (20)        0 2024-04-08 20:24:26.388149 jax-sysid-0.3.1/src/jax_sysid/
--rw-r--r--   0 bemporad   (501) staff       (20)        0 2023-01-10 11:29:35.000000 jax-sysid-0.3.1/src/jax_sysid/__init__.py
--rw-r--r--   0 bemporad   (501) staff       (20)    65267 2024-04-08 20:22:55.000000 jax-sysid-0.3.1/src/jax_sysid/models.py
--rw-r--r--   0 bemporad   (501) staff       (20)    11265 2024-04-08 20:22:40.000000 jax-sysid-0.3.1/src/jax_sysid/utils.py
-drwxr-xr-x   0 bemporad   (501) staff       (20)        0 2024-04-08 20:24:26.389020 jax-sysid-0.3.1/src/jax_sysid.egg-info/
--rw-r--r--   0 bemporad   (501) staff       (20)    12952 2024-04-08 20:24:26.000000 jax-sysid-0.3.1/src/jax_sysid.egg-info/PKG-INFO
--rw-r--r--   0 bemporad   (501) staff       (20)      314 2024-04-08 20:24:26.000000 jax-sysid-0.3.1/src/jax_sysid.egg-info/SOURCES.txt
--rw-r--r--   0 bemporad   (501) staff       (20)        1 2024-04-08 20:24:26.000000 jax-sysid-0.3.1/src/jax_sysid.egg-info/dependency_links.txt
--rw-r--r--   0 bemporad   (501) staff       (20)       49 2024-04-08 20:24:26.000000 jax-sysid-0.3.1/src/jax_sysid.egg-info/requires.txt
--rw-r--r--   0 bemporad   (501) staff       (20)       10 2024-04-08 20:24:26.000000 jax-sysid-0.3.1/src/jax_sysid.egg-info/top_level.txt
-drwxr-xr-x   0 bemporad   (501) staff       (20)        0 2024-04-08 20:24:26.388857 jax-sysid-0.3.1/tests/
--rw-r--r--   0 bemporad   (501) staff       (20)     5280 2024-03-06 15:24:05.000000 jax-sysid-0.3.1/tests/test_models.py
+drwxr-xr-x   0 bemporad   (501) staff       (20)        0 2024-04-24 13:49:30.540259 jax_sysid-0.3.2/
+-rw-r--r--   0 bemporad   (501) staff       (20)    11345 2024-03-01 16:55:21.000000 jax_sysid-0.3.2/LICENSE.txt
+-rw-r--r--   0 bemporad   (501) staff       (20)    12952 2024-04-24 13:49:30.540044 jax_sysid-0.3.2/PKG-INFO
+-rw-r--r--   0 bemporad   (501) staff       (20)    12152 2024-03-07 06:02:39.000000 jax_sysid-0.3.2/README.md
+-rw-r--r--   0 bemporad   (501) staff       (20)      801 2024-04-24 13:41:31.000000 jax_sysid-0.3.2/pyproject.toml
+-rw-r--r--   0 bemporad   (501) staff       (20)       38 2024-04-24 13:49:30.540294 jax_sysid-0.3.2/setup.cfg
+drwxr-xr-x   0 bemporad   (501) staff       (20)        0 2024-04-24 13:49:30.538075 jax_sysid-0.3.2/src/
+drwxr-xr-x   0 bemporad   (501) staff       (20)        0 2024-04-24 13:49:30.538905 jax_sysid-0.3.2/src/jax_sysid/
+-rw-r--r--   0 bemporad   (501) staff       (20)        0 2023-01-10 11:29:35.000000 jax_sysid-0.3.2/src/jax_sysid/__init__.py
+-rw-r--r--   0 bemporad   (501) staff       (20)    65287 2024-04-09 15:02:27.000000 jax_sysid-0.3.2/src/jax_sysid/models.py
+-rw-r--r--   0 bemporad   (501) staff       (20)    11300 2024-04-24 13:40:59.000000 jax_sysid-0.3.2/src/jax_sysid/utils.py
+drwxr-xr-x   0 bemporad   (501) staff       (20)        0 2024-04-24 13:49:30.539816 jax_sysid-0.3.2/src/jax_sysid.egg-info/
+-rw-r--r--   0 bemporad   (501) staff       (20)    12952 2024-04-24 13:49:30.000000 jax_sysid-0.3.2/src/jax_sysid.egg-info/PKG-INFO
+-rw-r--r--   0 bemporad   (501) staff       (20)      314 2024-04-24 13:49:30.000000 jax_sysid-0.3.2/src/jax_sysid.egg-info/SOURCES.txt
+-rw-r--r--   0 bemporad   (501) staff       (20)        1 2024-04-24 13:49:30.000000 jax_sysid-0.3.2/src/jax_sysid.egg-info/dependency_links.txt
+-rw-r--r--   0 bemporad   (501) staff       (20)       49 2024-04-24 13:49:30.000000 jax_sysid-0.3.2/src/jax_sysid.egg-info/requires.txt
+-rw-r--r--   0 bemporad   (501) staff       (20)       10 2024-04-24 13:49:30.000000 jax_sysid-0.3.2/src/jax_sysid.egg-info/top_level.txt
+drwxr-xr-x   0 bemporad   (501) staff       (20)        0 2024-04-24 13:49:30.539634 jax_sysid-0.3.2/tests/
+-rw-r--r--   0 bemporad   (501) staff       (20)     5280 2024-03-06 15:24:05.000000 jax_sysid-0.3.2/tests/test_models.py
```

### Comparing `jax-sysid-0.3.1/LICENSE.txt` & `jax_sysid-0.3.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jax-sysid-0.3.1/PKG-INFO` & `jax_sysid-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jax-sysid
-Version: 0.3.1
+Version: 0.3.2
 Summary: jax-sysid - A Python package for linear and nonlinear system identification and nonlinear regression using Jax.
 Author-email: Alberto Bemporad <alberto.bemporad@imtlucca.it>
 Project-URL: Homepage, http://cse.lab.imtlucca.it/~bemporad/jax-sysid
 Keywords: system identification,subspace identification,nonlinear regression
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `jax-sysid-0.3.1/README.md` & `jax_sysid-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `jax-sysid-0.3.1/pyproject.toml` & `jax_sysid-0.3.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "jax-sysid"
-version = "0.3.1"
+version = "0.3.2"
 authors = [
   { name="Alberto Bemporad", email="alberto.bemporad@imtlucca.it" },
 ]
 description = "jax-sysid - A Python package for linear and nonlinear system identification and nonlinear regression using Jax."
 readme = "README.md"
 requires-python = ">=3.9"
 dependencies = ["numpy","scipy","jax","jaxopt","flax","tqdm","matplotlib","pmlb"]
```

### Comparing `jax-sysid-0.3.1/src/jax_sysid/models.py` & `jax_sysid-0.3.2/src/jax_sysid/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -348,15 +348,15 @@
         rho_th : float
             L2-regularization on model parameters
         tau_th : float
             L1-regularization on model parameters
         tau_g : float
             group-Lasso regularization penalty
         group_lasso_fcn : function
-            function defining the group-Lasso penalty on the model parameters "params" and initial state "x0", minimized as tau_g*sum(||[params;x]_i||_2). For linear models, you can use the "group_lasso_x" or "group_lasso_u" methods.
+            function f(params,x0) defining the group-Lasso penalty on the model parameters "params" and initial state "x0", minimized as tau_g*sum(||[params;x0]_i||_2). For linear models, you can use the "group_lasso_x" or "group_lasso_u" methods.
         zero_coeff : _type_
             Entries smaller than zero_coeff are set to zero. Useful when tau_th>0 or tau_g>0.
         xsat : float
             Saturation value for state variables, forced during training to avoid numerical issues.
         train_x0 : bool
             If True, also train the initial state x0, otherwise set x0=0 and ignore rho_x0.
         custom_regularization : function
@@ -1363,15 +1363,15 @@
         rho_th : float
             L2-regularization on model parameters
         tau_th : float
             L1-regularization on model parameters
         tau_g : float
             group-Lasso regularization penalty
         group_lasso_fcn : function
-            function defining the group-Lasso penalty on the model parameters "params", minimized as tau_g*sum(||[params;x]_i||_2).
+            function f(params) defining the group-Lasso penalty on the model parameters "params", minimized as tau_g*sum(||params_i||_2).
         zero_coeff : _type_
             Entries smaller than zero_coeff are set to zero. Useful when tau_th>0 or tau_g>0.
         custom_regularization : function
             Custom regularization term, a function of the model parameters 
             custom_regularization(params, x0).            
         """
         if output_loss is None:
```

### Comparing `jax-sysid-0.3.1/src/jax_sysid/utils.py` & `jax_sysid-0.3.2/src/jax_sysid/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -169,15 +169,15 @@
     if isAcc:
         unit = "%"
     else:
         unit = ""
 
     if ny > 1:
         for i in range(ny):
-            if isR2 or isBFR or isRMSE:
+            if isR2 or isBFR:
                 if use_training:
                     nY_train2 = np.sum(
                         (Y_train[:, i] - np.mean(Y_train[:, i]))**2)
                 if use_test:
                     nY_test2 = np.sum(
                         (Y_test[:, i] - np.mean(Y_test[:, i]))**2)
             text = f"y{i+1}: "
@@ -193,15 +193,15 @@
             elif isBFR:
                 if use_training:
                     score_train[i] = 100. * (1. - np.linalg.norm(
                         Yhat_train[:, i] - Y_train[:, i]) / np.sqrt(nY_train2))
                 if use_test:
                     score_test[i] = 100. * (1. - np.linalg.norm(
                         Yhat_test[:, i] - Y_test[:, i]) / np.sqrt(nY_test2))
-            if isRMSE:
+            elif isRMSE:
                 if use_training:
                     score_train[i] = np.sqrt((np.sum((Yhat_train[:, i] -
                                                       Y_train[:, i]) ** 2))/Y_train.shape[0])
                 if use_test:
                     score_test[i] = np.sqrt(np.sum((Yhat_test[:, i] -
                                                     Y_test[:, i]) ** 2)/Y_test.shape[0])
             elif isAcc:
@@ -217,18 +217,19 @@
                 score_test[i] = np.nan
 
             text += f"{fit.capitalize()} score: training = {score_train[i]: 5.4f}{unit}, test = {score_test[i]: 5.4f}{unit}"
             msg += '\n' + text
             # print(text)
         msg += "\n-----\nAverage "
     else:
-        if use_training:
-            nY_train2 = np.sum((Y_train-np.mean(Y_train))**2)
-        if use_test:
-            nY_test2 = np.sum((Y_test - np.mean(Y_test))**2)
+        if isR2 or isBFR:
+            if use_training:
+                nY_train2 = np.sum((Y_train-np.mean(Y_train))**2)
+            if use_test:
+                nY_test2 = np.sum((Y_test - np.mean(Y_test))**2)
         if isR2:
             if use_training:
                 score_train = 100. * \
                     (1. - np.sum((Yhat_train - Y_train) ** 2) / nY_train2)
             if use_test:
                 score_test = 100. * \
                     (1. - np.sum((Yhat_test - Y_test) ** 2) / nY_test2)
```

### Comparing `jax-sysid-0.3.1/src/jax_sysid.egg-info/PKG-INFO` & `jax_sysid-0.3.2/src/jax_sysid.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jax-sysid
-Version: 0.3.1
+Version: 0.3.2
 Summary: jax-sysid - A Python package for linear and nonlinear system identification and nonlinear regression using Jax.
 Author-email: Alberto Bemporad <alberto.bemporad@imtlucca.it>
 Project-URL: Homepage, http://cse.lab.imtlucca.it/~bemporad/jax-sysid
 Keywords: system identification,subspace identification,nonlinear regression
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `jax-sysid-0.3.1/tests/test_models.py` & `jax_sysid-0.3.2/tests/test_models.py`

 * *Files identical despite different names*


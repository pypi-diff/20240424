# Comparing `tmp/miracle_imputation-0.1.5-py3-none-macosx_10_14_x86_64.whl.zip` & `tmp/miracle_imputation-0.1.6-py3-none-macosx_10_14_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 14968 bytes, number of entries: 15
--rw-r--r--  2.0 unx    15745 b- defN 22-Dec-27 16:10 miracle/MIRACLE.py
--rw-r--r--  2.0 unx       97 b- defN 22-Dec-27 16:10 miracle/__init__.py
--rw-r--r--  2.0 unx     2770 b- defN 22-Dec-27 16:10 miracle/logger.py
--rw-r--r--  2.0 unx       22 b- defN 22-Dec-27 16:10 miracle/version.py
--rw-r--r--  2.0 unx      769 b- defN 22-Dec-27 16:10 miracle/third_party/__init__.py
--rw-r--r--  2.0 unx     8764 b- defN 22-Dec-27 16:10 miracle/third_party/imputation_gain.py
--rw-r--r--  2.0 unx      609 b- defN 22-Dec-27 16:10 miracle/third_party/imputation_knn.py
--rw-r--r--  2.0 unx      846 b- defN 22-Dec-27 16:10 miracle/third_party/imputation_mean.py
--rw-r--r--  2.0 unx     2718 b- defN 22-Dec-27 16:10 miracle/third_party/imputation_mice.py
--rw-r--r--  2.0 unx     1889 b- defN 22-Dec-27 16:10 miracle/third_party/imputation_missforest.py
--rw-r--r--  2.0 unx     1519 b- defN 22-Dec-27 16:10 miracle_imputation-0.1.5.dist-info/LICENSE
--rw-r--r--  2.0 unx     3120 b- defN 22-Dec-27 16:10 miracle_imputation-0.1.5.dist-info/METADATA
--rw-r--r--  2.0 unx      108 b- defN 22-Dec-27 16:10 miracle_imputation-0.1.5.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 22-Dec-27 16:10 miracle_imputation-0.1.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1303 b- defN 22-Dec-27 16:10 miracle_imputation-0.1.5.dist-info/RECORD
-15 files, 40287 bytes uncompressed, 12782 bytes compressed:  68.3%
+Zip file size: 15119 bytes, number of entries: 15
+-rw-r--r--  2.0 unx    15745 b- defN 24-Apr-24 19:10 miracle/MIRACLE.py
+-rw-r--r--  2.0 unx       97 b- defN 24-Apr-24 19:10 miracle/__init__.py
+-rw-r--r--  2.0 unx     2770 b- defN 24-Apr-24 19:10 miracle/logger.py
+-rw-r--r--  2.0 unx       22 b- defN 24-Apr-24 19:10 miracle/version.py
+-rw-r--r--  2.0 unx      769 b- defN 24-Apr-24 19:10 miracle/third_party/__init__.py
+-rw-r--r--  2.0 unx     8764 b- defN 24-Apr-24 19:10 miracle/third_party/imputation_gain.py
+-rw-r--r--  2.0 unx      609 b- defN 24-Apr-24 19:10 miracle/third_party/imputation_knn.py
+-rw-r--r--  2.0 unx      846 b- defN 24-Apr-24 19:10 miracle/third_party/imputation_mean.py
+-rw-r--r--  2.0 unx     2780 b- defN 24-Apr-24 19:10 miracle/third_party/imputation_mice.py
+-rw-r--r--  2.0 unx     1909 b- defN 24-Apr-24 19:10 miracle/third_party/imputation_missforest.py
+-rw-r--r--  2.0 unx     1519 b- defN 24-Apr-24 19:10 miracle_imputation-0.1.6.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3433 b- defN 24-Apr-24 19:10 miracle_imputation-0.1.6.dist-info/METADATA
+-rw-r--r--  2.0 unx      108 b- defN 24-Apr-24 19:10 miracle_imputation-0.1.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 24-Apr-24 19:10 miracle_imputation-0.1.6.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1303 b- defN 24-Apr-24 19:10 miracle_imputation-0.1.6.dist-info/RECORD
+15 files, 40682 bytes uncompressed, 12933 bytes compressed:  68.2%
```

## zipnote {}

```diff
@@ -24,23 +24,23 @@
 
 Filename: miracle/third_party/imputation_mice.py
 Comment: 
 
 Filename: miracle/third_party/imputation_missforest.py
 Comment: 
 
-Filename: miracle_imputation-0.1.5.dist-info/LICENSE
+Filename: miracle_imputation-0.1.6.dist-info/LICENSE
 Comment: 
 
-Filename: miracle_imputation-0.1.5.dist-info/METADATA
+Filename: miracle_imputation-0.1.6.dist-info/METADATA
 Comment: 
 
-Filename: miracle_imputation-0.1.5.dist-info/WHEEL
+Filename: miracle_imputation-0.1.6.dist-info/WHEEL
 Comment: 
 
-Filename: miracle_imputation-0.1.5.dist-info/top_level.txt
+Filename: miracle_imputation-0.1.6.dist-info/top_level.txt
 Comment: 
 
-Filename: miracle_imputation-0.1.5.dist-info/RECORD
+Filename: miracle_imputation-0.1.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## miracle/version.py

```diff
@@ -1 +1 @@
-__version__ = "0.1.5"
+__version__ = "0.1.6"
```

## miracle/third_party/imputation_mice.py

```diff
@@ -5,21 +5,27 @@
 # third party
 import numpy as np
 from sklearn.experimental import enable_iterative_imputer  # noqa: F401,E402
 from sklearn.impute import IterativeImputer
 
 
 class MiceImputation:
-    """Imputation plugin for completing missing values using the Multivariate Iterative chained equations and multiple imputations.
+    """Imputation plugin for completing missing values using the Multivariate Iterative chained equations and multiple \
+    imputations.
 
     Method:
-        Multivariate Iterative chained equations(MICE) methods model each feature with missing values as a function of other features in a round-robin fashion. For each step of the round-robin imputation, we use a BayesianRidge estimator, which does a regularized linear regression.
-        The class `sklearn.impute.IterativeImputer` is able to generate multiple imputations of the same incomplete dataset. We can then learn a regression or classification model on different imputations of the same dataset.
-        Setting `sample_posterior=True` for the IterativeImputer will randomly draw values to fill each missing value from the Gaussian posterior of the predictions. If each `IterativeImputer` uses a different `random_state`, this results in multiple imputations, each of which can be used to train a predictive model.
-        The final result is the average of all the `n_imputation` estimates.
+        Multivariate Iterative chained equations(MICE) methods model each feature with missing values as a function of \
+        other features in a round-robin fashion. For each step of the round-robin imputation, we use a BayesianRidge \
+        estimator, which does a regularized linear regression. The class `sklearn.impute.IterativeImputer` is able to \
+        generate multiple imputations of the same incomplete dataset. We can then learn a regression or classification \
+        model on different imputations of the same dataset. Setting `sample_posterior=True` for the IterativeImputer \
+        will randomly draw values to fill each missing value from the Gaussian posterior of the predictions. \
+        If each `IterativeImputer` uses a different `random_state`, this results in multiple imputations, each of \
+        which can be used to train a predictive model. The final result is the average of all the `n_imputation` \
+        estimates.
 
     Args:
         n_imputations: int, default=5i
             number of multiple imputations to perform.
         max_iter: int, default=500
             maximum number of imputation rounds to perform.
         random_state: int, default set to the current time.
```

## miracle/third_party/imputation_missforest.py

```diff
@@ -9,15 +9,17 @@
 from sklearn.impute import IterativeImputer
 
 
 class MissForestImputation:
     """Imputation plugin for completing missing values using the MissForest strategy.
 
     Method:
-        Iterative chained equations(ICE) methods model each feature with missing values as a function of other features in a round-robin fashion. For each step of the round-robin imputation, we use a ExtraTreesRegressor, which fits a number of randomized extra-trees and averages the results.
+        Iterative chained equations(ICE) methods model each feature with missing values as a function of other \
+        features in a round-robin fashion. For each step of the round-robin imputation, we use a ExtraTreesRegressor, \
+        which fits a number of randomized extra-trees and averages the results.
 
     Args:
         n_estimators: int, default=10
             The number of trees in the forest.
         max_iter: int, default=500
             maximum number of imputation rounds to perform.
         random_state: int, default set to the current time.
```

## Comparing `miracle_imputation-0.1.5.dist-info/LICENSE` & `miracle_imputation-0.1.6.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `miracle_imputation-0.1.5.dist-info/METADATA` & `miracle_imputation-0.1.6.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: miracle-imputation
-Version: 0.1.5
+Version: 0.1.6
 Summary: Missing data Imputation Refinement And Causal LEarning
 Home-page: https://github.com/trentkyono/MIRACLE
 Author: Trent Kyono
 Author-email: 
 License: BSD-3-Clause
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
@@ -13,15 +13,15 @@
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: loguru
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: scikit-learn
-Requires-Dist: tensorflow (>=2.0)
+Requires-Dist: tensorflow >=2.0
 
 # MIRACLE (Missing data Imputation Refinement And Causal LEarning)
 
 [![Tests](https://github.com/vanderschaarlab/MIRACLE/actions/workflows/test_miracle.yml/badge.svg)](https://github.com/vanderschaarlab/MIRACLE/actions/workflows/test_miracle.yml)
 [![License](https://img.shields.io/badge/License-BSD%203--Clause-blue.svg)](https://github.com/vanderschaarlab/MIRACLE/blob/main/LICENSE)
 
 Code Author: Trent Kyono
@@ -31,14 +31,19 @@
 ## Installation
 
 ```bash
 pip install -r requirements.txt
 pip install .
 ```
 
+### CUDA support (optional)
+For CUDA support, you should make sure [TensorFlow 2 CUDA requirements](https://www.tensorflow.org/install/pip) are met.
+
+Install the library as above, then install the CUDA enabled version of TensorFlow by following the [official instructions](https://www.tensorflow.org/install/pip).
+
 ## Tests
 You can run the tests using
 ```bash
 pip install -r requirements_dev.txt
 pip install .
 pytest -vsx
 ```
```

## Comparing `miracle_imputation-0.1.5.dist-info/RECORD` & `miracle_imputation-0.1.6.dist-info/RECORD`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 miracle/MIRACLE.py,sha256=amNEKx-XNOew7L2mXJyKcw-5MaLuGkKMd92sM0r2XxE,15745
 miracle/__init__.py,sha256=OYQCcSmjJEOz8arHBSbbfsnsx3d70yVzj-pj1b4pUPs,97
 miracle/logger.py,sha256=IhmTkOUrQmFOpRZ3qCS1eZCwtp50ipKAoEl97uqlFyU,2770
-miracle/version.py,sha256=rPSfWgIeq2YWVPyESOAwCBt8vftsTpIkuLAGDEzyRQc,22
+miracle/version.py,sha256=n3oM6B_EMz93NsTI18NNZd-jKFcUPzUkbIKj5VFK5ok,22
 miracle/third_party/__init__.py,sha256=NtDkvTKHHDchjKJya1LcdJBEmCWtpShPZEB6Q5AzIsg,769
 miracle/third_party/imputation_gain.py,sha256=Hd0eBENC8byfPodysyFiH5fN7YVNzVvyWyeJYenqP-Y,8764
 miracle/third_party/imputation_knn.py,sha256=aYH2wNp8tG4jynfZ4e9gKs9fVhSQ9r7aas1vNxFoT7c,609
 miracle/third_party/imputation_mean.py,sha256=CB_yowgF9HNri9oje5ltf7-eZvtQMOBzyGq7HdLe3-Y,846
-miracle/third_party/imputation_mice.py,sha256=dsTGLj1L2D_0IrVmlTuqJfBjnr2JrP_XKHWvC_MeQYM,2718
-miracle/third_party/imputation_missforest.py,sha256=W4C7j82InQ-Lt99OfkulBxrhpYKfbDmCdS0qCXfuDfg,1889
-miracle_imputation-0.1.5.dist-info/LICENSE,sha256=IqNZq6018gGT6U3hgHKp6w2drRVAx7rVPQxeX8nrMfc,1519
-miracle_imputation-0.1.5.dist-info/METADATA,sha256=YpFt_iTOkR_jJhpbuwII91fqGZXiW3nxifEhw4rzxO4,3120
-miracle_imputation-0.1.5.dist-info/WHEEL,sha256=eB2aNjTYg-Xs2sC-30SiF6Qy3QhFjN9gbOG6r08MITc,108
-miracle_imputation-0.1.5.dist-info/top_level.txt,sha256=vpatNurm8q8Gz53DpoixkNixhjI2DAHYGuWwoULNO8A,8
-miracle_imputation-0.1.5.dist-info/RECORD,,
+miracle/third_party/imputation_mice.py,sha256=K6101Z0q0Suh7DB2BSRMUGSSSPaCISTCJal8qccfMbA,2780
+miracle/third_party/imputation_missforest.py,sha256=y6628SwI8vvIeE7aKO_g7LLnWotIepVHwvQcSde5xaE,1909
+miracle_imputation-0.1.6.dist-info/LICENSE,sha256=IqNZq6018gGT6U3hgHKp6w2drRVAx7rVPQxeX8nrMfc,1519
+miracle_imputation-0.1.6.dist-info/METADATA,sha256=ynjsg8LKvw-Apjk7nj308k0r6_L3QPSECaZcwd8fA6Y,3433
+miracle_imputation-0.1.6.dist-info/WHEEL,sha256=s-jf7gmrBrV_U-pwIXd5OG1p5njLlhrnaNl0sF75gq4,108
+miracle_imputation-0.1.6.dist-info/top_level.txt,sha256=vpatNurm8q8Gz53DpoixkNixhjI2DAHYGuWwoULNO8A,8
+miracle_imputation-0.1.6.dist-info/RECORD,,
```


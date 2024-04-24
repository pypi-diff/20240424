# Comparing `tmp/ikpls-1.2.0.post1.tar.gz` & `tmp/ikpls-1.2.0.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ikpls-1.2.0.post1.tar", max compression
+gzip compressed data, was "ikpls-1.2.0.post2.tar", max compression
```

## Comparing `ikpls-1.2.0.post1.tar` & `ikpls-1.2.0.post2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    11433 2024-04-22 14:18:40.603925 ikpls-1.2.0.post1/LICENSE
--rw-r--r--   0        0        0     8767 2024-04-22 14:18:40.603925 ikpls-1.2.0.post1/README.rst
--rw-r--r--   0        0        0       28 2024-04-22 14:18:40.603925 ikpls-1.2.0.post1/ikpls/__init__.py
--rw-r--r--   0        0        0        0 2024-04-22 14:18:40.607925 ikpls-1.2.0.post1/ikpls/fast_cross_validation/__init__.py
--rw-r--r--   0        0        0    23705 2024-04-22 14:18:40.607925 ikpls-1.2.0.post1/ikpls/fast_cross_validation/numpy_ikpls.py
--rw-r--r--   0        0        0    15583 2024-04-22 14:18:40.607925 ikpls-1.2.0.post1/ikpls/jax_ikpls_alg_1.py
--rw-r--r--   0        0        0    13495 2024-04-22 14:18:40.607925 ikpls-1.2.0.post1/ikpls/jax_ikpls_alg_2.py
--rw-r--r--   0        0        0    41664 2024-04-22 14:18:40.607925 ikpls-1.2.0.post1/ikpls/jax_ikpls_base.py
--rw-r--r--   0        0        0    10170 2024-04-22 14:18:40.607925 ikpls-1.2.0.post1/ikpls/numpy_ikpls.py
--rw-r--r--   0        0        0      559 2024-04-22 14:18:40.611925 ikpls-1.2.0.post1/pyproject.toml
--rw-r--r--   0        0        0     9692 1970-01-01 00:00:00.000000 ikpls-1.2.0.post1/PKG-INFO
+-rw-r--r--   0        0        0    11433 2024-04-24 00:21:01.861739 ikpls-1.2.0.post2/LICENSE
+-rw-r--r--   0        0        0     7674 2024-04-24 00:21:01.861739 ikpls-1.2.0.post2/README.md
+-rw-r--r--   0        0        0       28 2024-04-24 00:21:01.865739 ikpls-1.2.0.post2/ikpls/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-24 00:21:01.865739 ikpls-1.2.0.post2/ikpls/fast_cross_validation/__init__.py
+-rw-r--r--   0        0        0    23705 2024-04-24 00:21:01.865739 ikpls-1.2.0.post2/ikpls/fast_cross_validation/numpy_ikpls.py
+-rw-r--r--   0        0        0    15583 2024-04-24 00:21:01.865739 ikpls-1.2.0.post2/ikpls/jax_ikpls_alg_1.py
+-rw-r--r--   0        0        0    13495 2024-04-24 00:21:01.865739 ikpls-1.2.0.post2/ikpls/jax_ikpls_alg_2.py
+-rw-r--r--   0        0        0    41664 2024-04-24 00:21:01.865739 ikpls-1.2.0.post2/ikpls/jax_ikpls_base.py
+-rw-r--r--   0        0        0    10170 2024-04-24 00:21:01.865739 ikpls-1.2.0.post2/ikpls/numpy_ikpls.py
+-rw-r--r--   0        0        0      558 2024-04-24 00:21:01.869739 ikpls-1.2.0.post2/pyproject.toml
+-rw-r--r--   0        0        0     8602 1970-01-01 00:00:00.000000 ikpls-1.2.0.post2/PKG-INFO
```

### Comparing `ikpls-1.2.0.post1/LICENSE` & `ikpls-1.2.0.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `ikpls-1.2.0.post1/README.rst` & `ikpls-1.2.0.post2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,157 +1,170 @@
-Improved Kernel Partial Least Squares (IKPLS) and Fast Cross-Validation
-=======================================================================
+# Improved Kernel Partial Least Squares (IKPLS) and Fast Cross-Validation
 
-.. image:: https://img.shields.io/pypi/v/ikpls.svg
-   :target: https://pypi.python.org/pypi/ikpls/
-   :alt: PyPI Version
-.. image:: https://img.shields.io/pypi/dm/ikpls
-   :target: https://pypi.python.org/pypi/ikpls/
-   :alt: PyPI - Downloads
-.. image:: https://img.shields.io/pypi/pyversions/ikpls.svg
-   :target: https://pypi.python.org/pypi/ikpls/
-   :alt: Python Versions
-.. image:: https://img.shields.io/pypi/l/ikpls.svg
-   :target: https://pypi.python.org/pypi/ikpls/
-   :alt: License
-.. image:: https://readthedocs.org/projects/ikpls/badge/?version=latest
-   :target: https://ikpls.readthedocs.io/en/latest/?badge=latest
-   :alt: Documentation Status
-.. image:: https://github.com/Sm00thix/IKPLS/actions/workflows/workflow.yml/badge.svg
-   :target: https://github.com/Sm00thix/IKPLS/actions/workflows/workflow.yml
-   :alt: Build Status
-.. image:: https://joss.theoj.org/papers/ac559cbcdc6e6551f58bb3e573a73afc/status.svg
-   :target: https://joss.theoj.org/papers/ac559cbcdc6e6551f58bb3e573a73afc
-   :alt: JOSS Status
+[![PyPI Version](https://img.shields.io/pypi/v/ikpls.svg)](https://pypi.python.org/pypi/ikpls/)
 
-Fast CPU, GPU, and TPU Python implementations of Improved Kernel PLS Algorithm #1 and Algorithm #2 by Dayal and MacGregor [1]_. Improved Kernel PLS is both fast [2]_ and numerically stable [3]_.
-The CPU implementations use NumPy [4]_ and subclass BaseEstimator from scikit-learn [5]_, allowing integration into scikit-learn's ecosystem of machine learning algorithms and pipelines. For example, the CPU implementations can be used with scikit-learn's `cross_validate <https://scikit-learn.org/stable/modules/generated/sklearn.model_selection.cross_validate.html>`_.
-The GPU and TPU implementations use Google's JAX [6]_. JAX supports automatic differentiation while allowing CPU, GPU, and TPU execution. This implies that the JAX implementations can be combined with deep learning approaches, as the PLS fit is differentiable.
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/ikpls)](https://pypi.python.org/pypi/ikpls/)
 
-The documentation is available at https://ikpls.readthedocs.io/en/latest/; examples can be found at https://github.com/Sm00thix/IKPLS/tree/main/examples.
+[![Python Versions](https://img.shields.io/pypi/pyversions/ikpls.svg)](https://pypi.python.org/pypi/ikpls/)
 
-.. [1] `Dayal, B. S., & MacGregor, J. F. (1997). Improved PLS algorithms. Journal of Chemometrics: A Journal of the Chemometrics Society, 11(1), 73-85`_.
-.. [2] `Alin, A. (2009). Comparison of PLS algorithms when the number of objects is much larger than the number of variables. Statistical papers, 50, 711-720`_.
-.. [3] `Andersson, M. (2009). A comparison of nine PLS1 algorithms. Journal of Chemometrics: A Journal of the Chemometrics Society, 23(10), 518-529`_.
-.. [4] `NumPy`_.
-.. [5] `scikit-learn`_.
-.. [6] `JAX`_.
-
-.. _Dayal, B. S., & MacGregor, J. F. (1997). Improved PLS algorithms. Journal of Chemometrics\: A Journal of the Chemometrics Society, 11(1), 73-85: https://doi.org/10.1002/(SICI)1099-128X(199701)11:1%3C73::AID-CEM435%3E3.0.CO;2-%23?
-.. _Alin, A. (2009). Comparison of PLS algorithms when the number of objects is much larger than the number of variables. Statistical papers, 50, 711-720: https://doi.org/10.1007/s00362-009-0251-7
-.. _Andersson, M. (2009). A comparison of nine PLS1 algorithms. Journal of Chemometrics\: A Journal of the Chemometrics Society, 23(10), 518-529: https://doi.org/10.1002/cem.1248
-.. _NumPy: https://numpy.org/
-.. _scikit-learn: https://scikit-learn.org/stable/
-.. _JAX: https://jax.readthedocs.io/en/latest/
-
-Fast Cross-Validation
--------------------------------
-In addition to the implementations mentioned above, this package contains the novel, fast cross-validation algorithms mentioned in [7]_ using both IKPLS algorithms.
-The fast cross-validation algorithms benefit both IKPLS Algorithms and especially Algorithm #2.
-The fast cross-validation algorithms are mathematically equivalent to the classical cross-validation algorithm. Still, they are much quicker if cross-validation splits exceed 3.
-The fast cross-validation algorithms correctly handle (column-wise) centering and scaling of the X and Y input matrices using training set means and standard deviations to avoid data leakage from the validation set.
-This centering and scaling can be enabled by setting the center parameter to True and the scale parameter to True, respectively.
-The fast cross-validation algorithms correctly handle row-wise preprocessing such as (row-wise) centering and scaling of the X and Y input matrices, convolution, or other preprocessing.
-Row-wise preprocessing can safely be applied before passing the data to the fast cross-validation algorithms.
-
-.. [7] `Engstrøm, O.-C. G. (2024). Shortcutting Cross-Validation: Efficiently Deriving Column-Wise Centered and Scaled Training Set $\\mathbf{X}^\\mathbf{T}\\mathbf{X}$ and $\\mathbf{X}^\\mathbf{T}\\mathbf{Y}$ Without Full Recomputation of Matrix Products or Statistical Moments`_.
-
-.. _Engstrøm, O.-C. G. (2024). Shortcutting Cross-Validation\: Efficiently Deriving Column-Wise Centered and Scaled Training Set $\\mathbf{X}^\\mathbf{T}\\mathbf{X}$ and $\\mathbf{X}^\\mathbf{T}\\mathbf{Y}$ Without Full Recomputation of Matrix Products or Statistical Moments: https://arxiv.org/abs/2401.13185
-
-Pre-requisites
---------------
-
-The JAX implementations support running on both CPU, GPU, and TPU. To use the GPU or TPU, follow the instructions from the `JAX Installation Guide
-<https://jax.readthedocs.io/en/latest/installation.html>`_.
-
-To ensure that JAX implementations use Float64, set the environment variable JAX_ENABLE_X64=True as per the `Current Gotchas
-<https://github.com/google/jax#current-gotchas>`_.
-
-Installation
-------------
-
--  | Install the package for Python3 using the following command:
-   | ``$ pip3 install ikpls``
--  | Now you can import the NumPy and JAX implementations with:
-   | ``from ikpls.numpy_ikpls import PLS as NpPLS``
-   | ``from ikpls.jax_ikpls_alg_1 import PLS as JAXPLS_Alg_1``
-   | ``from ikpls.jax_ikpls_alg_2 import PLS as JAXPLS_Alg_2``
-   | ``from ikpls.fast_cross_validation.numpy_ikpls import PLS as NpPLS_FastCV``
-
-
-Quick Start
------------
-Use the ikpls package for PLS modeling
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~   
-
-  .. code:: python
-
-   import numpy as np
-
-   from ikpls.numpy_ikpls import PLS
-
-
-    N = 100  # Number of samples.
-    K = 50  # Number of features.
-    M = 10  # Number of targets.
-    A = 20  # Number of latent variables (PLS components).
-
-    # Using float64 is important for numerical stability.
-    X = np.random.uniform(size=(N, K)).astype(np.float64)
-    Y = np.random.uniform(size=(N, M)).astype(np.float64)
-
-    # The other PLS algorithms and implementations have the same interface for fit()
-    # and predict(). The fast cross-validation implementation with IKPLS has a
-    # different interface.
-    np_ikpls_alg_1 = PLS(algorithm=1)
-    np_ikpls_alg_1.fit(X, Y, A)
-
-    # Has shape (A, N, M) = (20, 100, 10). Contains a prediction for all possible
-    # numbers of components up to and including A.
-    y_pred = np_ikpls_alg_1.predict(X)
-
-    # Has shape (N, M) = (100, 10).
-    y_pred_20_components = np_ikpls_alg_1.predict(X, n_components=20)
-    (y_pred_20_components == y_pred[19]).all()  # True
-
-    # The internal model parameters can be accessed as follows:
-
-    # Regression coefficients tensor of shape (A, K, M) = (20, 50, 10).
-    np_ikpls_alg_1.B
-
-    # X weights matrix of shape (K, A) = (50, 20).
-    np_ikpls_alg_1.W
-
-    # X loadings matrix of shape (K, A) = (50, 20).
-    np_ikpls_alg_1.P
-
-    # Y loadings matrix of shape (M, A) = (10, 20).
-    np_ikpls_alg_1.Q
-
-    # X rotations matrix of shape (K, A) = (50, 20).
-    np_ikpls_alg_1.R
-
-    # X scores matrix of shape (N, A) = (100, 20).
-    # This is only computed for IKPLS Algorithm #1.
-    np_ikpls_alg_1.T
-
-Examples
-~~~~~~~~
-
-In `examples <https://github.com/Sm00thix/IKPLS/tree/main/examples>`_ you will find:
-
-- `Fit and Predict with NumPy. <https://github.com/Sm00thix/IKPLS/tree/main/examples/fit_predict_numpy.py>`_
-
-- `Fit and Predict with JAX. <https://github.com/Sm00thix/IKPLS/tree/main/examples/fit_predict_jax.py>`_
-
-- `Cross-validate with NumPy. <https://github.com/Sm00thix/IKPLS/tree/main/examples/cross_val_numpy.py>`_
-
-- `Cross-validate with NumPy and fast cross-validation. <https://github.com/Sm00thix/IKPLS/tree/main/examples/fast_cross_val_numpy.py>`_
-
-- `Cross-validate with JAX. <https://github.com/Sm00thix/IKPLS/tree/main/examples/cross_val_jax.py>`_
-
-- `Compute the gradient of a preprocessing convolution filter with respect to the RMSE between the target value and the value predicted by PLS after fitting with JAX. <https://github.com/Sm00thix/IKPLS/tree/main/examples/gradient_jax.py>`_
-
-Contribute
-----------
-
-To contribute, please read the `Contribution Guidelines <https://github.com/Sm00thix/IKPLS/blob/main/CONTRIBUTING.rst>`_.
+[![License](https://img.shields.io/pypi/l/ikpls.svg)](https://pypi.python.org/pypi/ikpls/)
+
+[![Documentation Status](https://readthedocs.org/projects/ikpls/badge/?version=latest)](https://ikpls.readthedocs.io/en/latest/?badge=latest)
+
+[![Build Status](https://github.com/Sm00thix/IKPLS/actions/workflows/workflow.yml/badge.svg)](https://github.com/Sm00thix/IKPLS/actions/workflows/workflow.yml)
+
+[![JOSS Status](https://joss.theoj.org/papers/ac559cbcdc6e6551f58bb3e573a73afc/status.svg)](https://joss.theoj.org/papers/ac559cbcdc6e6551f58bb3e573a73afc)
+
+Fast CPU, GPU, and TPU Python implementations of Improved Kernel PLS
+Algorithm #1 and Algorithm #2 [[1]](#references). Improved
+Kernel PLS is both fast [[2]](#references) and numerically stable [[3]](#references). The CPU
+implementations use [[4]](#references) and subclass BaseEstimator from scikit-learn [[5]](#references),
+allowing integration into scikit-learn\'s ecosystem of
+machine learning algorithms and pipelines. For example, the CPU
+implementations can be used with scikit-learn\'s
+[cross_validate](https://scikit-learn.org/stable/modules/generated/sklearn.model_selection.cross_validate.html).
+The GPU and TPU implementations use Google\'s JAX [[6]](#references). JAX supports
+automatic differentiation while allowing CPU, GPU, and TPU execution.
+This implies that the JAX implementations can be combined with deep
+learning approaches, as the PLS fit is differentiable.
+
+The documentation is available at
+<https://ikpls.readthedocs.io/en/latest/>; examples can be found at
+<https://github.com/Sm00thix/IKPLS/tree/main/examples>.
+
+## Fast Cross-Validation
+
+In addition to the implementations mentioned above, this package
+contains the novel, fast cross-validation algorithms by Engstrøm [[7]](#references)
+using both IKPLS algorithms. The fast cross-validation algorithms
+benefit both IKPLS Algorithms and especially Algorithm #2. The fast
+cross-validation algorithms are mathematically equivalent to the
+classical cross-validation algorithm. Still, they are much quicker if
+cross-validation splits exceed 3. The fast cross-validation algorithms
+correctly handle (column-wise) centering and scaling of the X and Y
+input matrices using training set means and standard deviations to avoid
+data leakage from the validation set. This centering and scaling can be
+enabled by setting the center parameter to True and the scale parameter
+to True, respectively. The fast cross-validation algorithms correctly
+handle row-wise preprocessing such as (row-wise) centering and scaling
+of the X and Y input matrices, convolution, or other preprocessing.
+Row-wise preprocessing can safely be applied before passing the data to
+the fast cross-validation algorithms.
+
+## Pre-requisites
+
+The JAX implementations support running on both CPU, GPU, and TPU. To
+use the GPU or TPU, follow the instructions from the [JAX Installation
+Guide](https://jax.readthedocs.io/en/latest/installation.html).
+
+To ensure that JAX implementations use Float64, set the environment
+variable JAX_ENABLE_X64=True as per the [Current
+Gotchas](https://github.com/google/jax#current-gotchas).
+
+## Installation
+
+- Install the package for Python3 using the following command:
+    ```shell
+    pip3 install ikpls
+    ```
+
+- Now you can import the NumPy and JAX implementations with:
+    ```python
+    from ikpls.numpy_ikpls import PLS as NpPLS
+    from ikpls.jax_ikpls_alg_1 import PLS as JAXPLS_Alg_1
+    from ikpls.jax_ikpls_alg_2 import PLS as JAXPLS_Alg_2
+    from ikpls.fast_cross_validation.numpy_ikpls import PLS as NpPLS_FastCV
+    ```
+
+## Quick Start
+
+### Use the ikpls package for PLS modeling
+
+> ```python
+> import numpy as np
+>
+> from ikpls.numpy_ikpls import PLS
+>
+>
+>  N = 100  # Number of samples.
+>  K = 50  # Number of features.
+>  M = 10  # Number of targets.
+>  A = 20  # Number of latent variables (PLS components).
+>
+>  # Using float64 is important for numerical stability.
+>  X = np.random.uniform(size=(N, K)).astype(np.float64)
+>  Y = np.random.uniform(size=(N, M)).astype(np.float64)
+>
+>  # The other PLS algorithms and implementations have the same interface for fit()
+>  # and predict(). The fast cross-validation implementation with IKPLS has a
+>  # different interface.
+>  np_ikpls_alg_1 = PLS(algorithm=1)
+>  np_ikpls_alg_1.fit(X, Y, A)
+>
+>  # Has shape (A, N, M) = (20, 100, 10). Contains a prediction for all possible
+>  # numbers of components up to and including A.
+>  y_pred = np_ikpls_alg_1.predict(X)
+>
+>  # Has shape (N, M) = (100, 10).
+>  y_pred_20_components = np_ikpls_alg_1.predict(X, n_components=20)
+>  (y_pred_20_components == y_pred[19]).all()  # True
+>
+>  # The internal model parameters can be accessed as follows:
+>
+>  # Regression coefficients tensor of shape (A, K, M) = (20, 50, 10).
+>  np_ikpls_alg_1.B
+>
+>  # X weights matrix of shape (K, A) = (50, 20).
+>  np_ikpls_alg_1.W
+>
+>  # X loadings matrix of shape (K, A) = (50, 20).
+>  np_ikpls_alg_1.P
+>
+>  # Y loadings matrix of shape (M, A) = (10, 20).
+>  np_ikpls_alg_1.Q
+>
+>  # X rotations matrix of shape (K, A) = (50, 20).
+>  np_ikpls_alg_1.R
+>
+>  # X scores matrix of shape (N, A) = (100, 20).
+>  # This is only computed for IKPLS Algorithm #1.
+>  np_ikpls_alg_1.T
+> ```
+
+### Examples
+
+In [examples](https://github.com/Sm00thix/IKPLS/tree/main/examples) you
+will find:
+
+-   [Fit and Predict with
+    NumPy.](https://github.com/Sm00thix/IKPLS/tree/main/examples/fit_predict_numpy.py)
+-   [Fit and Predict with
+    JAX.](https://github.com/Sm00thix/IKPLS/tree/main/examples/fit_predict_jax.py)
+-   [Cross-validate with
+    NumPy.](https://github.com/Sm00thix/IKPLS/tree/main/examples/cross_val_numpy.py)
+-   [Cross-validate with NumPy and fast
+    cross-validation.](https://github.com/Sm00thix/IKPLS/tree/main/examples/fast_cross_val_numpy.py)
+-   [Cross-validate with
+    JAX.](https://github.com/Sm00thix/IKPLS/tree/main/examples/cross_val_jax.py)
+-   [Compute the gradient of a preprocessing convolution filter with
+    respect to the RMSE between the target value and the value predicted
+    by PLS after fitting with
+    JAX.](https://github.com/Sm00thix/IKPLS/tree/main/examples/gradient_jax.py)
+
+## Contribute
+
+To contribute, please read the [Contribution
+Guidelines](https://github.com/Sm00thix/IKPLS/blob/main/CONTRIBUTING.md).
+
+## References
+
+1. [Dayal, B. S., & MacGregor, J. F. (1997). Improved PLS algorithms. *Journal of Chemometrics*, 11(1), 73-85.](https://doi.org/10.1002/(SICI)1099-128X(199701)11:1%3C73::AID-CEM435%3E3.0.CO;2-%23?)
+2. [Alin, A. (2009). Comparison of PLS algorithms when the number of objects is much larger than the number of variables. *Statistical Papers*, 50, 711-720.](https://doi.org/10.1007/s00362-009-0251-7)
+3. [Andersson, M. (2009). A comparison of nine PLS1 algorithms. *Journal of Chemometrics*, 23(10), 518-529.](https://doi.org/10.1002/cem.1248)
+4. [NumPy](https://numpy.org/)
+5. [scikit-learn](https://scikit-learn.org/stable/)
+6. [JAX](https://jax.readthedocs.io/en/latest/)
+7. [Engstrøm, O.-C. G. (2024). Shortcutting Cross-Validation:
+    Efficiently Deriving Column-Wise Centered and Scaled Training Set
+    \$\\\\mathbf{X}\^\\\\mathbf{T}\\\\mathbf{X}\$ and
+    \$\\\\mathbf{X}\^\\\\mathbf{T}\\\\mathbf{Y}\$ Without Full
+    Recomputation of Matrix Products or Statistical Moments](https://arxiv.org/abs/2401.13185)
```

### Comparing `ikpls-1.2.0.post1/ikpls/fast_cross_validation/numpy_ikpls.py` & `ikpls-1.2.0.post2/ikpls/fast_cross_validation/numpy_ikpls.py`

 * *Files identical despite different names*

### Comparing `ikpls-1.2.0.post1/ikpls/jax_ikpls_alg_1.py` & `ikpls-1.2.0.post2/ikpls/jax_ikpls_alg_1.py`

 * *Files identical despite different names*

### Comparing `ikpls-1.2.0.post1/ikpls/jax_ikpls_alg_2.py` & `ikpls-1.2.0.post2/ikpls/jax_ikpls_alg_2.py`

 * *Files identical despite different names*

### Comparing `ikpls-1.2.0.post1/ikpls/jax_ikpls_base.py` & `ikpls-1.2.0.post2/ikpls/jax_ikpls_base.py`

 * *Files identical despite different names*

### Comparing `ikpls-1.2.0.post1/ikpls/numpy_ikpls.py` & `ikpls-1.2.0.post2/ikpls/numpy_ikpls.py`

 * *Files identical despite different names*

### Comparing `ikpls-1.2.0.post1/pyproject.toml` & `ikpls-1.2.0.post2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [tool.poetry]
 name = "ikpls"
-version = "1.2.0.post1"
+version = "1.2.0.post2"
 description = ""
 authors = ["Sm00thix <oleemail@icloud.com>"]
 maintainers = ["Sm00thix <oleemail@icloud.com>"]
 license = "Apache-2.0"
-readme = "README.rst"
+readme = "README.md"
 homepage = "https://ikpls.readthedocs.io/en/latest/"
 repository = "https://github.com/Sm00thix/IKPLS"
 
 [tool.poetry.dependencies]
 python = ">=3.9, <3.13"
 numpy = "^1.26.3"
 jax = "^0.4.20"
```

### Comparing `ikpls-1.2.0.post1/PKG-INFO` & `ikpls-1.2.0.post2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ikpls
-Version: 1.2.0.post1
+Version: 1.2.0.post2
 Summary: 
 Home-page: https://ikpls.readthedocs.io/en/latest/
 License: Apache-2.0
 Author: Sm00thix
 Author-email: oleemail@icloud.com
 Maintainer: Sm00thix
 Maintainer-email: oleemail@icloud.com
@@ -18,166 +18,179 @@
 Requires-Dist: jax (>=0.4.20,<0.5.0)
 Requires-Dist: jaxlib (>=0.4.20,<0.5.0)
 Requires-Dist: joblib (>=1.3.2,<2.0.0)
 Requires-Dist: numpy (>=1.26.3,<2.0.0)
 Requires-Dist: scikit-learn (>=1.4.1,<2.0.0)
 Requires-Dist: tqdm (>=4.66.1,<5.0.0)
 Project-URL: Repository, https://github.com/Sm00thix/IKPLS
-Description-Content-Type: text/x-rst
+Description-Content-Type: text/markdown
 
-Improved Kernel Partial Least Squares (IKPLS) and Fast Cross-Validation
-=======================================================================
+# Improved Kernel Partial Least Squares (IKPLS) and Fast Cross-Validation
 
-.. image:: https://img.shields.io/pypi/v/ikpls.svg
-   :target: https://pypi.python.org/pypi/ikpls/
-   :alt: PyPI Version
-.. image:: https://img.shields.io/pypi/dm/ikpls
-   :target: https://pypi.python.org/pypi/ikpls/
-   :alt: PyPI - Downloads
-.. image:: https://img.shields.io/pypi/pyversions/ikpls.svg
-   :target: https://pypi.python.org/pypi/ikpls/
-   :alt: Python Versions
-.. image:: https://img.shields.io/pypi/l/ikpls.svg
-   :target: https://pypi.python.org/pypi/ikpls/
-   :alt: License
-.. image:: https://readthedocs.org/projects/ikpls/badge/?version=latest
-   :target: https://ikpls.readthedocs.io/en/latest/?badge=latest
-   :alt: Documentation Status
-.. image:: https://github.com/Sm00thix/IKPLS/actions/workflows/workflow.yml/badge.svg
-   :target: https://github.com/Sm00thix/IKPLS/actions/workflows/workflow.yml
-   :alt: Build Status
-.. image:: https://joss.theoj.org/papers/ac559cbcdc6e6551f58bb3e573a73afc/status.svg
-   :target: https://joss.theoj.org/papers/ac559cbcdc6e6551f58bb3e573a73afc
-   :alt: JOSS Status
+[![PyPI Version](https://img.shields.io/pypi/v/ikpls.svg)](https://pypi.python.org/pypi/ikpls/)
 
-Fast CPU, GPU, and TPU Python implementations of Improved Kernel PLS Algorithm #1 and Algorithm #2 by Dayal and MacGregor [1]_. Improved Kernel PLS is both fast [2]_ and numerically stable [3]_.
-The CPU implementations use NumPy [4]_ and subclass BaseEstimator from scikit-learn [5]_, allowing integration into scikit-learn's ecosystem of machine learning algorithms and pipelines. For example, the CPU implementations can be used with scikit-learn's `cross_validate <https://scikit-learn.org/stable/modules/generated/sklearn.model_selection.cross_validate.html>`_.
-The GPU and TPU implementations use Google's JAX [6]_. JAX supports automatic differentiation while allowing CPU, GPU, and TPU execution. This implies that the JAX implementations can be combined with deep learning approaches, as the PLS fit is differentiable.
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/ikpls)](https://pypi.python.org/pypi/ikpls/)
 
-The documentation is available at https://ikpls.readthedocs.io/en/latest/; examples can be found at https://github.com/Sm00thix/IKPLS/tree/main/examples.
-
-.. [1] `Dayal, B. S., & MacGregor, J. F. (1997). Improved PLS algorithms. Journal of Chemometrics: A Journal of the Chemometrics Society, 11(1), 73-85`_.
-.. [2] `Alin, A. (2009). Comparison of PLS algorithms when the number of objects is much larger than the number of variables. Statistical papers, 50, 711-720`_.
-.. [3] `Andersson, M. (2009). A comparison of nine PLS1 algorithms. Journal of Chemometrics: A Journal of the Chemometrics Society, 23(10), 518-529`_.
-.. [4] `NumPy`_.
-.. [5] `scikit-learn`_.
-.. [6] `JAX`_.
-
-.. _Dayal, B. S., & MacGregor, J. F. (1997). Improved PLS algorithms. Journal of Chemometrics\: A Journal of the Chemometrics Society, 11(1), 73-85: https://doi.org/10.1002/(SICI)1099-128X(199701)11:1%3C73::AID-CEM435%3E3.0.CO;2-%23?
-.. _Alin, A. (2009). Comparison of PLS algorithms when the number of objects is much larger than the number of variables. Statistical papers, 50, 711-720: https://doi.org/10.1007/s00362-009-0251-7
-.. _Andersson, M. (2009). A comparison of nine PLS1 algorithms. Journal of Chemometrics\: A Journal of the Chemometrics Society, 23(10), 518-529: https://doi.org/10.1002/cem.1248
-.. _NumPy: https://numpy.org/
-.. _scikit-learn: https://scikit-learn.org/stable/
-.. _JAX: https://jax.readthedocs.io/en/latest/
-
-Fast Cross-Validation
--------------------------------
-In addition to the implementations mentioned above, this package contains the novel, fast cross-validation algorithms mentioned in [7]_ using both IKPLS algorithms.
-The fast cross-validation algorithms benefit both IKPLS Algorithms and especially Algorithm #2.
-The fast cross-validation algorithms are mathematically equivalent to the classical cross-validation algorithm. Still, they are much quicker if cross-validation splits exceed 3.
-The fast cross-validation algorithms correctly handle (column-wise) centering and scaling of the X and Y input matrices using training set means and standard deviations to avoid data leakage from the validation set.
-This centering and scaling can be enabled by setting the center parameter to True and the scale parameter to True, respectively.
-The fast cross-validation algorithms correctly handle row-wise preprocessing such as (row-wise) centering and scaling of the X and Y input matrices, convolution, or other preprocessing.
-Row-wise preprocessing can safely be applied before passing the data to the fast cross-validation algorithms.
-
-.. [7] `Engstrøm, O.-C. G. (2024). Shortcutting Cross-Validation: Efficiently Deriving Column-Wise Centered and Scaled Training Set $\\mathbf{X}^\\mathbf{T}\\mathbf{X}$ and $\\mathbf{X}^\\mathbf{T}\\mathbf{Y}$ Without Full Recomputation of Matrix Products or Statistical Moments`_.
-
-.. _Engstrøm, O.-C. G. (2024). Shortcutting Cross-Validation\: Efficiently Deriving Column-Wise Centered and Scaled Training Set $\\mathbf{X}^\\mathbf{T}\\mathbf{X}$ and $\\mathbf{X}^\\mathbf{T}\\mathbf{Y}$ Without Full Recomputation of Matrix Products or Statistical Moments: https://arxiv.org/abs/2401.13185
-
-Pre-requisites
---------------
-
-The JAX implementations support running on both CPU, GPU, and TPU. To use the GPU or TPU, follow the instructions from the `JAX Installation Guide
-<https://jax.readthedocs.io/en/latest/installation.html>`_.
-
-To ensure that JAX implementations use Float64, set the environment variable JAX_ENABLE_X64=True as per the `Current Gotchas
-<https://github.com/google/jax#current-gotchas>`_.
-
-Installation
-------------
-
--  | Install the package for Python3 using the following command:
-   | ``$ pip3 install ikpls``
--  | Now you can import the NumPy and JAX implementations with:
-   | ``from ikpls.numpy_ikpls import PLS as NpPLS``
-   | ``from ikpls.jax_ikpls_alg_1 import PLS as JAXPLS_Alg_1``
-   | ``from ikpls.jax_ikpls_alg_2 import PLS as JAXPLS_Alg_2``
-   | ``from ikpls.fast_cross_validation.numpy_ikpls import PLS as NpPLS_FastCV``
-
-
-Quick Start
------------
-Use the ikpls package for PLS modeling
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~   
-
-  .. code:: python
-
-   import numpy as np
-
-   from ikpls.numpy_ikpls import PLS
-
-
-    N = 100  # Number of samples.
-    K = 50  # Number of features.
-    M = 10  # Number of targets.
-    A = 20  # Number of latent variables (PLS components).
-
-    # Using float64 is important for numerical stability.
-    X = np.random.uniform(size=(N, K)).astype(np.float64)
-    Y = np.random.uniform(size=(N, M)).astype(np.float64)
-
-    # The other PLS algorithms and implementations have the same interface for fit()
-    # and predict(). The fast cross-validation implementation with IKPLS has a
-    # different interface.
-    np_ikpls_alg_1 = PLS(algorithm=1)
-    np_ikpls_alg_1.fit(X, Y, A)
-
-    # Has shape (A, N, M) = (20, 100, 10). Contains a prediction for all possible
-    # numbers of components up to and including A.
-    y_pred = np_ikpls_alg_1.predict(X)
-
-    # Has shape (N, M) = (100, 10).
-    y_pred_20_components = np_ikpls_alg_1.predict(X, n_components=20)
-    (y_pred_20_components == y_pred[19]).all()  # True
-
-    # The internal model parameters can be accessed as follows:
-
-    # Regression coefficients tensor of shape (A, K, M) = (20, 50, 10).
-    np_ikpls_alg_1.B
-
-    # X weights matrix of shape (K, A) = (50, 20).
-    np_ikpls_alg_1.W
-
-    # X loadings matrix of shape (K, A) = (50, 20).
-    np_ikpls_alg_1.P
-
-    # Y loadings matrix of shape (M, A) = (10, 20).
-    np_ikpls_alg_1.Q
-
-    # X rotations matrix of shape (K, A) = (50, 20).
-    np_ikpls_alg_1.R
-
-    # X scores matrix of shape (N, A) = (100, 20).
-    # This is only computed for IKPLS Algorithm #1.
-    np_ikpls_alg_1.T
-
-Examples
-~~~~~~~~
-
-In `examples <https://github.com/Sm00thix/IKPLS/tree/main/examples>`_ you will find:
-
-- `Fit and Predict with NumPy. <https://github.com/Sm00thix/IKPLS/tree/main/examples/fit_predict_numpy.py>`_
-
-- `Fit and Predict with JAX. <https://github.com/Sm00thix/IKPLS/tree/main/examples/fit_predict_jax.py>`_
-
-- `Cross-validate with NumPy. <https://github.com/Sm00thix/IKPLS/tree/main/examples/cross_val_numpy.py>`_
-
-- `Cross-validate with NumPy and fast cross-validation. <https://github.com/Sm00thix/IKPLS/tree/main/examples/fast_cross_val_numpy.py>`_
-
-- `Cross-validate with JAX. <https://github.com/Sm00thix/IKPLS/tree/main/examples/cross_val_jax.py>`_
-
-- `Compute the gradient of a preprocessing convolution filter with respect to the RMSE between the target value and the value predicted by PLS after fitting with JAX. <https://github.com/Sm00thix/IKPLS/tree/main/examples/gradient_jax.py>`_
-
-Contribute
-----------
-
-To contribute, please read the `Contribution Guidelines <https://github.com/Sm00thix/IKPLS/blob/main/CONTRIBUTING.rst>`_.
+[![Python Versions](https://img.shields.io/pypi/pyversions/ikpls.svg)](https://pypi.python.org/pypi/ikpls/)
+
+[![License](https://img.shields.io/pypi/l/ikpls.svg)](https://pypi.python.org/pypi/ikpls/)
+
+[![Documentation Status](https://readthedocs.org/projects/ikpls/badge/?version=latest)](https://ikpls.readthedocs.io/en/latest/?badge=latest)
+
+[![Build Status](https://github.com/Sm00thix/IKPLS/actions/workflows/workflow.yml/badge.svg)](https://github.com/Sm00thix/IKPLS/actions/workflows/workflow.yml)
+
+[![JOSS Status](https://joss.theoj.org/papers/ac559cbcdc6e6551f58bb3e573a73afc/status.svg)](https://joss.theoj.org/papers/ac559cbcdc6e6551f58bb3e573a73afc)
+
+Fast CPU, GPU, and TPU Python implementations of Improved Kernel PLS
+Algorithm #1 and Algorithm #2 [[1]](#references). Improved
+Kernel PLS is both fast [[2]](#references) and numerically stable [[3]](#references). The CPU
+implementations use [[4]](#references) and subclass BaseEstimator from scikit-learn [[5]](#references),
+allowing integration into scikit-learn\'s ecosystem of
+machine learning algorithms and pipelines. For example, the CPU
+implementations can be used with scikit-learn\'s
+[cross_validate](https://scikit-learn.org/stable/modules/generated/sklearn.model_selection.cross_validate.html).
+The GPU and TPU implementations use Google\'s JAX [[6]](#references). JAX supports
+automatic differentiation while allowing CPU, GPU, and TPU execution.
+This implies that the JAX implementations can be combined with deep
+learning approaches, as the PLS fit is differentiable.
+
+The documentation is available at
+<https://ikpls.readthedocs.io/en/latest/>; examples can be found at
+<https://github.com/Sm00thix/IKPLS/tree/main/examples>.
+
+## Fast Cross-Validation
+
+In addition to the implementations mentioned above, this package
+contains the novel, fast cross-validation algorithms by Engstrøm [[7]](#references)
+using both IKPLS algorithms. The fast cross-validation algorithms
+benefit both IKPLS Algorithms and especially Algorithm #2. The fast
+cross-validation algorithms are mathematically equivalent to the
+classical cross-validation algorithm. Still, they are much quicker if
+cross-validation splits exceed 3. The fast cross-validation algorithms
+correctly handle (column-wise) centering and scaling of the X and Y
+input matrices using training set means and standard deviations to avoid
+data leakage from the validation set. This centering and scaling can be
+enabled by setting the center parameter to True and the scale parameter
+to True, respectively. The fast cross-validation algorithms correctly
+handle row-wise preprocessing such as (row-wise) centering and scaling
+of the X and Y input matrices, convolution, or other preprocessing.
+Row-wise preprocessing can safely be applied before passing the data to
+the fast cross-validation algorithms.
+
+## Pre-requisites
+
+The JAX implementations support running on both CPU, GPU, and TPU. To
+use the GPU or TPU, follow the instructions from the [JAX Installation
+Guide](https://jax.readthedocs.io/en/latest/installation.html).
+
+To ensure that JAX implementations use Float64, set the environment
+variable JAX_ENABLE_X64=True as per the [Current
+Gotchas](https://github.com/google/jax#current-gotchas).
+
+## Installation
+
+- Install the package for Python3 using the following command:
+    ```shell
+    pip3 install ikpls
+    ```
+
+- Now you can import the NumPy and JAX implementations with:
+    ```python
+    from ikpls.numpy_ikpls import PLS as NpPLS
+    from ikpls.jax_ikpls_alg_1 import PLS as JAXPLS_Alg_1
+    from ikpls.jax_ikpls_alg_2 import PLS as JAXPLS_Alg_2
+    from ikpls.fast_cross_validation.numpy_ikpls import PLS as NpPLS_FastCV
+    ```
+
+## Quick Start
+
+### Use the ikpls package for PLS modeling
+
+> ```python
+> import numpy as np
+>
+> from ikpls.numpy_ikpls import PLS
+>
+>
+>  N = 100  # Number of samples.
+>  K = 50  # Number of features.
+>  M = 10  # Number of targets.
+>  A = 20  # Number of latent variables (PLS components).
+>
+>  # Using float64 is important for numerical stability.
+>  X = np.random.uniform(size=(N, K)).astype(np.float64)
+>  Y = np.random.uniform(size=(N, M)).astype(np.float64)
+>
+>  # The other PLS algorithms and implementations have the same interface for fit()
+>  # and predict(). The fast cross-validation implementation with IKPLS has a
+>  # different interface.
+>  np_ikpls_alg_1 = PLS(algorithm=1)
+>  np_ikpls_alg_1.fit(X, Y, A)
+>
+>  # Has shape (A, N, M) = (20, 100, 10). Contains a prediction for all possible
+>  # numbers of components up to and including A.
+>  y_pred = np_ikpls_alg_1.predict(X)
+>
+>  # Has shape (N, M) = (100, 10).
+>  y_pred_20_components = np_ikpls_alg_1.predict(X, n_components=20)
+>  (y_pred_20_components == y_pred[19]).all()  # True
+>
+>  # The internal model parameters can be accessed as follows:
+>
+>  # Regression coefficients tensor of shape (A, K, M) = (20, 50, 10).
+>  np_ikpls_alg_1.B
+>
+>  # X weights matrix of shape (K, A) = (50, 20).
+>  np_ikpls_alg_1.W
+>
+>  # X loadings matrix of shape (K, A) = (50, 20).
+>  np_ikpls_alg_1.P
+>
+>  # Y loadings matrix of shape (M, A) = (10, 20).
+>  np_ikpls_alg_1.Q
+>
+>  # X rotations matrix of shape (K, A) = (50, 20).
+>  np_ikpls_alg_1.R
+>
+>  # X scores matrix of shape (N, A) = (100, 20).
+>  # This is only computed for IKPLS Algorithm #1.
+>  np_ikpls_alg_1.T
+> ```
+
+### Examples
+
+In [examples](https://github.com/Sm00thix/IKPLS/tree/main/examples) you
+will find:
+
+-   [Fit and Predict with
+    NumPy.](https://github.com/Sm00thix/IKPLS/tree/main/examples/fit_predict_numpy.py)
+-   [Fit and Predict with
+    JAX.](https://github.com/Sm00thix/IKPLS/tree/main/examples/fit_predict_jax.py)
+-   [Cross-validate with
+    NumPy.](https://github.com/Sm00thix/IKPLS/tree/main/examples/cross_val_numpy.py)
+-   [Cross-validate with NumPy and fast
+    cross-validation.](https://github.com/Sm00thix/IKPLS/tree/main/examples/fast_cross_val_numpy.py)
+-   [Cross-validate with
+    JAX.](https://github.com/Sm00thix/IKPLS/tree/main/examples/cross_val_jax.py)
+-   [Compute the gradient of a preprocessing convolution filter with
+    respect to the RMSE between the target value and the value predicted
+    by PLS after fitting with
+    JAX.](https://github.com/Sm00thix/IKPLS/tree/main/examples/gradient_jax.py)
+
+## Contribute
+
+To contribute, please read the [Contribution
+Guidelines](https://github.com/Sm00thix/IKPLS/blob/main/CONTRIBUTING.md).
+
+## References
+
+1. [Dayal, B. S., & MacGregor, J. F. (1997). Improved PLS algorithms. *Journal of Chemometrics*, 11(1), 73-85.](https://doi.org/10.1002/(SICI)1099-128X(199701)11:1%3C73::AID-CEM435%3E3.0.CO;2-%23?)
+2. [Alin, A. (2009). Comparison of PLS algorithms when the number of objects is much larger than the number of variables. *Statistical Papers*, 50, 711-720.](https://doi.org/10.1007/s00362-009-0251-7)
+3. [Andersson, M. (2009). A comparison of nine PLS1 algorithms. *Journal of Chemometrics*, 23(10), 518-529.](https://doi.org/10.1002/cem.1248)
+4. [NumPy](https://numpy.org/)
+5. [scikit-learn](https://scikit-learn.org/stable/)
+6. [JAX](https://jax.readthedocs.io/en/latest/)
+7. [Engstrøm, O.-C. G. (2024). Shortcutting Cross-Validation:
+    Efficiently Deriving Column-Wise Centered and Scaled Training Set
+    \$\\\\mathbf{X}\^\\\\mathbf{T}\\\\mathbf{X}\$ and
+    \$\\\\mathbf{X}\^\\\\mathbf{T}\\\\mathbf{Y}\$ Without Full
+    Recomputation of Matrix Products or Statistical Moments](https://arxiv.org/abs/2401.13185)
```


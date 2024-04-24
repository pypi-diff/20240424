# Comparing `tmp/torchvinecopulib-2024.3.3.tar.gz` & `tmp/torchvinecopulib-2024.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchvinecopulib-2024.3.3.tar", max compression
+gzip compressed data, was "torchvinecopulib-2024.4.0.tar", max compression
```

## Comparing `torchvinecopulib-2024.3.3.tar` & `torchvinecopulib-2024.4.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0    35593 2024-03-17 13:26:15.252816 torchvinecopulib-2024.3.3/LICENSE
--rw-r--r--   0        0        0     1447 2024-03-19 08:01:03.246809 torchvinecopulib-2024.3.3/pyproject.toml
--rw-r--r--   0        0        0     5509 2024-03-19 08:03:21.873332 torchvinecopulib-2024.3.3/README.md
--rw-r--r--   0        0        0       97 2024-03-17 13:26:14.680422 torchvinecopulib-2024.3.3/torchvinecopulib/__init__.py
--rw-r--r--   0        0        0      379 2024-03-17 13:26:14.910123 torchvinecopulib-2024.3.3/torchvinecopulib/bicop/__init__.py
--rw-r--r--   0        0        0     9267 2024-03-19 01:36:47.658289 torchvinecopulib-2024.3.3/torchvinecopulib/bicop/_abc.py
--rw-r--r--   0        0        0     1357 2024-03-19 04:27:40.081281 torchvinecopulib-2024.3.3/torchvinecopulib/bicop/_archimedean.py
--rw-r--r--   0        0        0     1949 2024-03-19 04:27:40.113282 torchvinecopulib-2024.3.3/torchvinecopulib/bicop/_clayton.py
--rw-r--r--   0        0        0     8300 2024-03-19 04:27:40.176281 torchvinecopulib-2024.3.3/torchvinecopulib/bicop/_data_bcp.py
--rw-r--r--   0        0        0      414 2024-03-17 13:26:14.695424 torchvinecopulib-2024.3.3/torchvinecopulib/bicop/_elliptical.py
--rw-r--r--   0        0        0     4558 2024-03-19 05:17:03.239408 torchvinecopulib-2024.3.3/torchvinecopulib/bicop/_factory_bcp.py
--rw-r--r--   0        0        0     2837 2024-03-19 04:27:40.155282 torchvinecopulib-2024.3.3/torchvinecopulib/bicop/_frank.py
--rw-r--r--   0        0        0     1676 2024-03-19 04:27:40.154283 torchvinecopulib-2024.3.3/torchvinecopulib/bicop/_gaussian.py
--rw-r--r--   0        0        0     2438 2024-03-19 04:19:29.014984 torchvinecopulib-2024.3.3/torchvinecopulib/bicop/_gumbel.py
--rw-r--r--   0        0        0     1353 2024-03-17 13:26:14.706423 torchvinecopulib-2024.3.3/torchvinecopulib/bicop/_independent.py
--rw-r--r--   0        0        0     3045 2024-03-19 04:27:40.178281 torchvinecopulib-2024.3.3/torchvinecopulib/bicop/_joe.py
--rw-r--r--   0        0        0     3386 2024-03-19 04:27:40.195280 torchvinecopulib-2024.3.3/torchvinecopulib/bicop/_studentt.py
--rw-r--r--   0        0        0    27951 2024-03-19 05:17:03.457410 torchvinecopulib-2024.3.3/torchvinecopulib/util/__init__.py
--rw-r--r--   0        0        0      207 2024-03-17 13:26:14.717422 torchvinecopulib-2024.3.3/torchvinecopulib/vinecop/__init__.py
--rw-r--r--   0        0        0    28581 2024-03-19 05:17:03.439410 torchvinecopulib-2024.3.3/torchvinecopulib/vinecop/_data_vcp.py
--rw-r--r--   0        0        0    21360 2024-03-19 05:17:03.389409 torchvinecopulib-2024.3.3/torchvinecopulib/vinecop/_factory_vcp.py
--rw-r--r--   0        0        0     6653 1970-01-01 00:00:00.000000 torchvinecopulib-2024.3.3/PKG-INFO
+-rw-r--r--   0        0        0    35593 2024-03-24 13:40:35.000000 torchvinecopulib-2024.4.0/LICENSE
+-rw-r--r--   0        0        0     1481 2024-04-23 09:41:23.523981 torchvinecopulib-2024.4.0/pyproject.toml
+-rw-r--r--   0        0        0     5690 2024-04-23 09:41:23.320364 torchvinecopulib-2024.4.0/README.md
+-rw-r--r--   0        0        0       97 2024-03-24 13:54:38.000000 torchvinecopulib-2024.4.0/torchvinecopulib/__init__.py
+-rw-r--r--   0        0        0      379 2024-03-24 13:54:38.000000 torchvinecopulib-2024.4.0/torchvinecopulib/bicop/__init__.py
+-rw-r--r--   0        0        0     9267 2024-03-24 13:54:38.000000 torchvinecopulib-2024.4.0/torchvinecopulib/bicop/_abc.py
+-rw-r--r--   0        0        0     1357 2024-03-24 13:54:38.000000 torchvinecopulib-2024.4.0/torchvinecopulib/bicop/_archimedean.py
+-rw-r--r--   0        0        0     1949 2024-03-24 13:54:38.000000 torchvinecopulib-2024.4.0/torchvinecopulib/bicop/_clayton.py
+-rw-r--r--   0        0        0     8300 2024-03-24 13:54:38.000000 torchvinecopulib-2024.4.0/torchvinecopulib/bicop/_data_bcp.py
+-rw-r--r--   0        0        0      414 2024-03-24 13:54:38.000000 torchvinecopulib-2024.4.0/torchvinecopulib/bicop/_elliptical.py
+-rw-r--r--   0        0        0     4901 2024-04-22 06:08:15.918924 torchvinecopulib-2024.4.0/torchvinecopulib/bicop/_factory_bcp.py
+-rw-r--r--   0        0        0     2837 2024-03-24 13:54:38.000000 torchvinecopulib-2024.4.0/torchvinecopulib/bicop/_frank.py
+-rw-r--r--   0        0        0     1676 2024-03-24 13:54:38.000000 torchvinecopulib-2024.4.0/torchvinecopulib/bicop/_gaussian.py
+-rw-r--r--   0        0        0     2438 2024-03-24 13:54:38.000000 torchvinecopulib-2024.4.0/torchvinecopulib/bicop/_gumbel.py
+-rw-r--r--   0        0        0     1353 2024-03-24 13:54:38.000000 torchvinecopulib-2024.4.0/torchvinecopulib/bicop/_independent.py
+-rw-r--r--   0        0        0     3133 2024-04-02 13:53:35.188111 torchvinecopulib-2024.4.0/torchvinecopulib/bicop/_joe.py
+-rw-r--r--   0        0        0     3389 2024-04-21 12:47:06.000000 torchvinecopulib-2024.4.0/torchvinecopulib/bicop/_studentt.py
+-rw-r--r--   0        0        0    29166 2024-04-22 06:04:15.787345 torchvinecopulib-2024.4.0/torchvinecopulib/util/__init__.py
+-rw-r--r--   0        0        0      207 2024-03-24 13:54:42.000000 torchvinecopulib-2024.4.0/torchvinecopulib/vinecop/__init__.py
+-rw-r--r--   0        0        0    33223 2024-04-23 08:23:14.413176 torchvinecopulib-2024.4.0/torchvinecopulib/vinecop/_data_vcp.py
+-rw-r--r--   0        0        0    25352 2024-04-23 06:54:37.752451 torchvinecopulib-2024.4.0/torchvinecopulib/vinecop/_factory_vcp.py
+-rw-r--r--   0        0        0     6831 1970-01-01 00:00:00.000000 torchvinecopulib-2024.4.0/PKG-INFO
```

### Comparing `torchvinecopulib-2024.3.3/LICENSE` & `torchvinecopulib-2024.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `torchvinecopulib-2024.3.3/pyproject.toml` & `torchvinecopulib-2024.4.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.poetry]
 package-mode = true
 license = "GNU GPLv3"
 name = "torchvinecopulib"
-version = "2024.3.3"
+version = "2024.4.0"
 description = "yet another vine copula library for PyTorch."
 authors = ["Tuoyuan Cheng <cty120120@gmail.com>"]
 maintainers = ["Xiaosheng You <e1204754@u.nus.edu>"]
 readme = "README.md"
 # homepage = ""
 repository = "https://github.com/TY-Cheng/torchvinecopulib"
 documentation = "https://ty-cheng.github.io/torchvinecopulib/"
@@ -28,14 +28,15 @@
 torch = "^2"
 
 
 [tool.poetry.group.all.dependencies]
 matplotlib = "*"
 pot = "*"
 scikit-learn = "*"
+fastkde = "*"
 
 
 [tool.poetry.group.dev.dependencies]
 black = "*"
 coverage = "*"
 flake8 = "*"
 furo = "*"
@@ -43,14 +44,15 @@
 matplotlib = "*"
 pandas = "*"
 pot = "*"
 pytest = "*"
 pyvinecopulib = "0.6.4"
 scikit-learn = "*"
 sphinx = "*"
+tokenize-rt = "*"
 
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/TY-Cheng/torchvinecopulib/issues/new"
 
 
 [build-system]
```

### Comparing `torchvinecopulib-2024.3.3/README.md` & `torchvinecopulib-2024.4.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 # TorchVineCopuLib
 
 [![Python package](https://github.com/TY-Cheng/torchvinecopulib/actions/workflows/python-package.yml/badge.svg?branch=main)](https://github.com/TY-Cheng/torchvinecopulib/actions/workflows/python-package.yml)
-[![Deploy Docs](https://github.com/TY-Cheng/torchvinecopulib/actions/workflows/static.yml/badge.svg?branch=main)](https://github.com/TY-Cheng/torchvinecopulib/actions/workflows/static.yml)
-[![Codacy Badge](https://app.codacy.com/project/badge/Coverage/e8a7a7448b2043d9bbefafc5a3ec14f7)](https://app.codacy.com?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_coverage)
 ![Static Badge](https://img.shields.io/badge/Python-%203.10%7C3.11%7C3.12-blue)
+[![Codacy Badge](https://app.codacy.com/project/badge/Coverage/e8a7a7448b2043d9bbefafc5a3ec14f7)](https://app.codacy.com?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_coverage)
+[![Deploy Docs](https://github.com/TY-Cheng/torchvinecopulib/actions/workflows/static.yml/badge.svg?branch=main)](https://github.com/TY-Cheng/torchvinecopulib/actions/workflows/static.yml)
 [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
 ![PyPI - Version](https://img.shields.io/pypi/v/torchvinecopulib?style=flat)
+[![DOI](https://zenodo.org/badge/768037665.svg)](https://zenodo.org/doi/10.5281/zenodo.10836953)
+
 
 Yet another vine copula package, using [PyTorch](https://pytorch.org/get-started/locally/).
 
+- C/D/R-Vine full simulation/ quantile-regression/ conditoinal-simulation, all in one package
+  - Flexible simulation workflow for experienced users
 - Vectorized tensor computation with GPU (`device='cuda'`) support
 - Shorter runtimes for higher dimension simulations
 - Decoupled dataclasses and factory methods
-- Pure `Python` library, tested against [pyvinecopulib](https://github.com/vinecopulib/pyvinecopulib/) on Windows, Linux, MacOS
+- Pure `Python` library, inspired by and tested against [pyvinecopulib](https://github.com/vinecopulib/pyvinecopulib/) on Windows, Linux, MacOS
 - IO and visualization support
 
 ## Dependencies
 
 ```toml
 # inside the `./pyproject.toml` file
 python = "^3.10"
@@ -48,17 +52,17 @@
 ```
 
 By `pip` from `./dist/*.whl` or `./dist/*.tar.gz` in this repo.
 Need to use proper file name.
 
 ```bash
 # inside project root folder
-pip install ./dist/torchvinecopulib-2024.3.3-py3-none-any.whl
+pip install ./dist/torchvinecopulib-2024.4.0-py3-none-any.whl
 # or
-pip install ./dist/torchvinecopulib-2024.3.3.tar.gz
+pip install ./dist/torchvinecopulib-2024.4.0.tar.gz
 ```
 
 ## Examples
 
 Visit the `./examples/` folder for `.ipynb` Jupyter notebooks.
 
 ## Documentation
@@ -104,18 +108,17 @@
 - Include a clear and descriptive title and description for your pull request.
 - Make sure all tests pass before submitting the pull request.
 - If your pull request addresses an open issue, reference the issue number in the description using the syntax `#issue_number`.
 - [in-place ops can be slower](https://discuss.pytorch.org/t/are-inplace-operations-faster/61209/4)
 - [torch.jit.script can be slower](https://discuss.pytorch.org/t/why-is-torch-jit-script-slower/120131/6)
 
 ### TODO
-
-1. more `bicop` class in `torch`
-2. potentially deprecating `'mle'` from `mtd_fit`
-3. bivariate dependence funcs in `util.ENUM_FUNC_BIDEP`, resolve non-`torch` pkg dependencies (`scikit-learn`, `pot`)
+1. non-par bicop
+2. more (non-parametric) `bicop` class in `torch`
+3. potentially deprecating `'mle'` from `mtd_fit`
 
 ## License
 
 > Copyright (C) 2024 Tuoyuan Cheng, Xiaosheng You, Kan Chen
 >
 > This file is part of torchvinecopulib.
 > torchvinecopulib is free software: you can redistribute it and/or modify
```

### Comparing `torchvinecopulib-2024.3.3/torchvinecopulib/bicop/_abc.py` & `torchvinecopulib-2024.4.0/torchvinecopulib/bicop/_abc.py`

 * *Files identical despite different names*

### Comparing `torchvinecopulib-2024.3.3/torchvinecopulib/bicop/_archimedean.py` & `torchvinecopulib-2024.4.0/torchvinecopulib/bicop/_archimedean.py`

 * *Files identical despite different names*

### Comparing `torchvinecopulib-2024.3.3/torchvinecopulib/bicop/_clayton.py` & `torchvinecopulib-2024.4.0/torchvinecopulib/bicop/_clayton.py`

 * *Files identical despite different names*

### Comparing `torchvinecopulib-2024.3.3/torchvinecopulib/bicop/_data_bcp.py` & `torchvinecopulib-2024.4.0/torchvinecopulib/bicop/_data_bcp.py`

 * *Files identical despite different names*

### Comparing `torchvinecopulib-2024.3.3/torchvinecopulib/bicop/_factory_bcp.py` & `torchvinecopulib-2024.4.0/torchvinecopulib/bicop/_factory_bcp.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from ..util import kendall_tau
 from ._data_bcp import ENUM_FAM_BICOP, DataBiCop, SET_FAMnROT
 
 
 def bcp_from_obs(
     obs_bcp: torch.Tensor,
     tau: float | None = None,
+    thresh_trunc: float = 0.1,
     mtd_fit: str = "itau",
     mtd_mle: str = "COBYLA",
     mtd_sel: str = "aic",
     tpl_fam: tuple[str, ...] = (
         "Clayton",
         "Frank",
         "Gaussian",
@@ -24,14 +25,16 @@
 ) -> DataBiCop:
     """factory method to make a bivariate copula dataclass object, fitted from observations
 
     :param obs_bcp: bivariate copula obs, of shape (num_obs, 2) with values in [0, 1]
     :type obs_bcp: torch.Tensor
     :param tau: Kendall's tau of the observations, defaults to None for the function to estimate
     :type tau: float, optional
+    :param thresh_trunc: threshold of Kendall's tau independence test, below which we reject independent bicop, defaults to 0.1
+    :type thresh_trunc: float, optional
     :param mtd_fit: parameter estimation method, either 'itau' (inverse of tau) or 'mle' (maximum likelihood estimation); defaults to "itau"
     :type mtd_fit: str, optional
     :param mtd_mle: optimization method for mle as used by scipy.optimize.minimize, defaults to "COBYLA"
     :type mtd_mle: str, optional
     :param mtd_sel: model selection criterion, either 'aic' or 'bic'; defaults to "aic"
     :type mtd_sel: str, optional
     :param tpl_fam: tuple of str as candidate family names to fit, could be a subset of ('Clayton', 'Frank', 'Gaussian', 'Gumbel', 'Independent', 'Joe', 'StudentT')
@@ -42,15 +45,17 @@
     :return: fitted bivariate copula dataclass object
     :rtype: DataBiCop
     """
     # things known before fitting
     num_obs = obs_bcp.shape[0]
     # * tau from data, for inv-tau/tau2par, whose par is taken as init value for mle
     if tau is None:
-        tau = kendall_tau(x=obs_bcp[:, [0]], y=obs_bcp[:, [1]])
+        tau, pval = kendall_tau(x=obs_bcp[:, [0]], y=obs_bcp[:, [1]])
+        if pval >= thresh_trunc:
+            return DataBiCop(fam="Independent", negloglik=0.0, num_obs=num_obs, par=tuple(), rot=0)
 
     def _fit_itau(i_fam: str, i_rot: int) -> DataBiCop:
         # fetch the class
         i_cls = ENUM_FAM_BICOP[i_fam].value
         # tau to par
         i_par = i_cls.tau2par(tau=tau, obs=obs_bcp)
         return DataBiCop(
```

### Comparing `torchvinecopulib-2024.3.3/torchvinecopulib/bicop/_frank.py` & `torchvinecopulib-2024.4.0/torchvinecopulib/bicop/_frank.py`

 * *Files identical despite different names*

### Comparing `torchvinecopulib-2024.3.3/torchvinecopulib/bicop/_gaussian.py` & `torchvinecopulib-2024.4.0/torchvinecopulib/bicop/_gaussian.py`

 * *Files identical despite different names*

### Comparing `torchvinecopulib-2024.3.3/torchvinecopulib/bicop/_gumbel.py` & `torchvinecopulib-2024.4.0/torchvinecopulib/bicop/_gumbel.py`

 * *Files identical despite different names*

### Comparing `torchvinecopulib-2024.3.3/torchvinecopulib/bicop/_independent.py` & `torchvinecopulib-2024.4.0/torchvinecopulib/bicop/_independent.py`

 * *Files identical despite different names*

### Comparing `torchvinecopulib-2024.3.3/torchvinecopulib/bicop/_joe.py` & `torchvinecopulib-2024.4.0/torchvinecopulib/bicop/_joe.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import torch
-from scipy.special import digamma
 
-from ..util import solve_ITP, _CDF_MAX, _CDF_MIN
+from ..util import _CDF_MAX, _CDF_MIN, solve_ITP
 from ._archimedean import BiCopArchimedean
 
 
 class Joe(BiCopArchimedean):
     # Joe 2014 page 170
     # * suggest torch.float64 for |par|<88, torch.float32 for |par|<7
     _PAR_MIN, _PAR_MAX = (1.000001,), (88.0,)
@@ -53,15 +52,20 @@
     @staticmethod
     def par2tau_0(par: tuple) -> float:
         delta = par[0]
         if delta == 2:
             # 1- PolyGamma[1, 2] = 2 - pi**2 / 6
             return 0.3550659331517736
         else:
-            return 1.0 + 2.0 / (2.0 - delta) * (0.42278433509846713 - digamma(2.0 / delta + 1.0))
+            return (
+                1.0
+                + 2.0
+                / (2.0 - delta)
+                * (0.42278433509846713 - torch.special.digamma(torch.as_tensor(2.0 / delta + 1.0)))
+            ).item()
 
     @staticmethod
     def pdf_0(obs: torch.Tensor, par: tuple[float]) -> torch.Tensor:
         delta = par[0]
         x = obs[:, [0]].neg().log1p()
         y = obs[:, [1]].neg().log1p()
         x_y = x + y
```

### Comparing `torchvinecopulib-2024.3.3/torchvinecopulib/bicop/_studentt.py` & `torchvinecopulib-2024.4.0/torchvinecopulib/bicop/_studentt.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,15 +80,15 @@
         return cls.rho2tau_0(rho=par[0])
 
     @classmethod
     def tau2par(
         cls, tau: float = None, obs: torch.Tensor = None, mtd_opt: str = "COBYLA", **kwargs
     ) -> tuple:
         if tau is None:
-            tau = kendall_tau(x=obs[:, [0]], y=obs[:, [1]])
+            tau, _ = kendall_tau(x=obs[:, [0]], y=obs[:, [1]])
 
         rho = cls.tau2rho_0(tau=tau)
 
         # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
         # TODO: change estimator for nu
         # * scipy minimize, Powell, Nelder-Mead, COBYLA
         def fun_nll(vec):
```

### Comparing `torchvinecopulib-2024.3.3/torchvinecopulib/util/__init__.py` & `torchvinecopulib-2024.4.0/torchvinecopulib/util/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import math
 from enum import Enum
 from functools import partial
 
 import torch
-from scipy.stats import t
+from scipy.stats import t, kendalltau
 
 __all__ = [
     "ENUM_FUNC_BIDEP",
     "kendall_tau",
     "mutual_info",
     "ferreira_tail_dep_coeff",
     "chatterjee_xi",
@@ -19,46 +19,76 @@
 
 _CDF_MIN, _CDF_MAX = 0.0, 1.0
 _NU_MIN, _NU_MAX = 1.001, 49.999
 _RHO_MIN, _RHO_MAX = -0.99, 0.99
 _TAU_MIN, _TAU_MAX = -0.999, 0.999
 
 
+# def kendall_tau(
+#     x: torch.Tensor,
+#     y: torch.Tensor,
+#     tau_min: float = _TAU_MIN,
+#     tau_max: float = _TAU_MAX,
+# ) -> float:
+#     """https://gist.github.com/ili3p/f2b38b898f6eab0d87ec248ea39fde94
+#     x,y are both of shape (n, 1)
+#     """
+#     n = x.shape[0]
+#     n *= n - 1
+#     return (
+#         ((x.T - x).sign() * (y.T - y).sign()).sum().div(n).clamp(min=tau_min, max=tau_max).item()
+#     )
+
+
 def kendall_tau(
     x: torch.Tensor,
     y: torch.Tensor,
     tau_min: float = _TAU_MIN,
     tau_max: float = _TAU_MAX,
 ) -> float:
     """https://gist.github.com/ili3p/f2b38b898f6eab0d87ec248ea39fde94
     x,y are both of shape (n, 1)
     """
-    n = x.shape[0]
-    n *= n - 1
-    return (
-        ((x.T - x).sign() * (y.T - y).sign()).sum().div(n).clamp(min=tau_min, max=tau_max).item()
-    )
+    res = kendalltau(x.cpu().ravel(), y.cpu().ravel())
+    return (max(min(res[0], tau_max), tau_min), res[1])
 
 
-def mutual_info(x: torch.Tensor, y: torch.Tensor) -> float:
+def mutual_info(x: torch.Tensor, y: torch.Tensor, is_sklearn: bool = True) -> float:
     """https://scikit-learn.org/stable/modules/generated/sklearn.feature_selection.mutual_info_regression.html
     x,y are both of shape (n, 1)
+
+    Purkayastha, S., & Song, P. X. K. (2024).
+    fastMI: A fast and consistent copula-based nonparametric estimator of mutual information.
+    Journal of Multivariate Analysis, 201, 105270.
     """
-    # TODO: remove sklearn dependency
-    from sklearn.feature_selection import mutual_info_regression
+    if is_sklearn:
+        from sklearn.feature_selection import mutual_info_regression
 
-    return mutual_info_regression(
-        X=x.cpu(),
-        # ! notice the shape of y
-        y=y.cpu().ravel(),
-        discrete_features=False,
-        n_neighbors=3,
-        copy=True,
-        random_state=None,
-    )[0]
+        return mutual_info_regression(
+            X=x.cpu(),
+            # ! notice the shape of y
+            y=y.cpu().ravel(),
+            discrete_features=False,
+            n_neighbors=3,
+            copy=True,
+            random_state=None,
+        )[0]
+    else:
+        # Purkayastha, S., & Song, P. X. K. (2024).
+        from fastkde.fastKDE import pdf_at_points
+        from numpy import log
+
+        x_, y_ = x.ravel(), y.ravel()
+        joint = pdf_at_points(var1=x_, var2=y_)
+        joint = joint[joint > 0]
+        margin_x = pdf_at_points(var1=x_)
+        margin_x = margin_x[margin_x > 0]
+        margin_y = pdf_at_points(var1=y_)
+        margin_y = margin_y[margin_y > 0]
+        return (log(joint).mean() - log(margin_x).mean() - log(margin_y).mean()).item()
 
 
 def ferreira_tail_dep_coeff(x: torch.Tensor, y: torch.Tensor) -> float:
     """pairwise tail dependence coefficient (λ) estimator, max of rotation 0, 90, 180, 270
     x and y are both of shape (n, 1) inside (0, 1)
     symmetric for (x,y), (y,1-x), (1-x,1-y), (1-y,x), (y,x), (1-x,y), (1-y,1-x), (x,1-y)
     Ferreira, M.S., 2013. Nonparametric estimation of the tail-dependence coefficient;
@@ -122,56 +152,57 @@
         torch.as_tensor([xy_sum(m) for m in range(1, M + 1)]).sum(dim=0).max().item()
     ) / (M * (1.0 + n) * (1.0 + M + 4.0 * n))
 
 
 def wasserstein_dist_ind(
     x: torch.Tensor,
     y: torch.Tensor,
-    reg: float = 1e-2,
-    metric: str = "sqeuclidean",
+    reg: float = 0.1,
+    p: int = 2,
     seed: int = 0,
+    num_sim: int = 2,
 ) -> float:
-    """Wasserstein distance from bicop obs to indep bicop simulations, by ot.bregman.empirical_sinkhorn2 (averaged for each observation).
-
-    if num_row <= 1000, use all obs; otherwise, use 1000 random obs
-
-    https://pythonot.github.io/gen_modules/ot.bregman.html#ot.bregman.empirical_sinkhorn2
+    """Wasserstein distance from bicop obs to indep bicop simulations, by ot.sinkhorn2 (averaged for each observation).
 
     :param x: copula obs of shape (n,1)
     :type x: torch.Tensor
     :param y: copula obs of shape (n,1)
     :type y: torch.Tensor
-    :param reg: regularization strength, defaults to 1e-2
+    :param reg: regularization strength, defaults to 0.1
     :type reg: float, optional
-    :param metric: ground metric for the Wasserstein problem, defaults to 'sqeuclidean'
-    :type metric: str, optional
+    :param p: p-norm distance to calculate between each vector pair, defaults to 2
+    :type p: int, optional
     :param seed: random seed for torch.manual_seed() in indep bicop simulations, defaults to 0
     :type seed: int, optional
     :return: Wasserstein distance from bicop obs to indep bicop simulations
     :rtype: float
     """
-    # * remove ot dependency
-    from ot.bregman import empirical_sinkhorn2
+    from ot import sinkhorn2
 
     torch.manual_seed(seed=seed)
-    num_row = x.shape[0]
-    if num_row <= 1000:
-        return empirical_sinkhorn2(
-            X_s=torch.hstack([x, y]),
-            X_t=torch.rand(size=(num_row, 2), device=x.device, dtype=x.dtype),
-            reg=reg,
-            metric=metric,
-        ).item()
-    else:
-        return empirical_sinkhorn2(
-            X_s=torch.hstack([x, y])[torch.randperm(n=num_row, device=x.device)[:1000], :],
-            X_t=torch.rand(size=(1000, 2), device=x.device, dtype=x.dtype),
-            reg=reg,
-            metric=metric,
-        ).item()
+    X_s = torch.hstack([x, y])
+    num_obs = x.shape[0]
+    a, b = (
+        torch.ones(size=(num_obs, 1), device=x.device, dtype=x.dtype) / num_obs,
+        torch.ones(size=(num_obs, 1), device=x.device, dtype=x.dtype) / num_obs,
+    )
+    return (
+        sum(
+            (
+                sinkhorn2(
+                    a=a,
+                    b=b,
+                    M=torch.cdist(X_s, torch.rand_like(X_s), p=p),
+                    reg=reg,
+                ).item()
+                for _ in range(num_sim)
+            )
+        )
+        / num_sim
+    )
 
 
 class ENUM_FUNC_BIDEP(Enum):
     """an enum class for bivariate dependence measures"""
 
     chatterjee_xi = partial(chatterjee_xi)
     ferreira_tail_dep_coeff = partial(ferreira_tail_dep_coeff)
@@ -315,145 +346,145 @@
             + (pnorm(h) * pnorm(k))
         )
         .nan_to_num()
         .clamp(min=_CDF_MIN, max=_CDF_MAX)
     )
 
 
-# * Student's t distribution CDF (p), PPF (q), density (d)
-def inc_beta_reg(vec: torch.Tensor, a: float, b: float) -> torch.Tensor:
-    # * regularized incomplete beta integral, with a = 0.5, b = nu / 2, vec in [0,1]
-    # https://stats.stackexchange.com/questions/615961/students-t-cdf-ppf-or-hypergeometric-2f1-or-betainc-using-pytorch
-    # https://stats.stackexchange.com/questions/52341/formula-to-generate-critical-t-values-for-t-test-instead-of-using-a-look-up-arr
-    res = torch.empty_like(vec)
-    if (idx := vec > ((a + 1.0) / (2.0 + a + b))).any():
-        res[idx] = 1.0 - inc_beta_reg(vec=1.0 - vec[idx], a=b, b=a)
-    idx = ~idx
-    x = vec[idx]
-    qab = a + b
-    qap = a + 1.0
-    qam = a - 1.0
-    c = torch.ones_like(x)
-    d = 1.0 / (1.0 - qab * x / qap)
-    f = d.clone()
-    front = (
-        -math.lgamma(a)
-        - math.lgamma(b)
-        + math.lgamma(a + b)
-        - math.log(a)
-        + x.log() * a
-        + x.neg().log1p() * b
-    ).exp()
-    for i in range(1, 200):
-        i2 = i * 2.0
-        ai2 = a + i2
-        nmrt = (i * (b - i) / ((qam + i2) * ai2)) * x
-        d = (d * nmrt + 1.0).reciprocal()
-        c = nmrt / c + 1.0
-        f *= c * d
-        nmrt = (-(a + i) * (qab + i) / ((qap + i2) * ai2)) * x
-        d = (d * nmrt + 1.0).reciprocal()
-        c = nmrt / c + 1.0
-        cd = c * d
-        f *= cd
-        if ((1.0 - cd).abs() < 1e-6).all():
-            break
-    res[idx] = front * f
-    return res.nan_to_num().clamp(min=_CDF_MIN, max=_CDF_MAX)
-
-
-def inc_beta_reg_inv(vec: torch.Tensor, a: float, b: float) -> torch.Tensor:
-    a1, b1 = a - 1.0, b - 1.0
-    if a > 1.0 and b > 1.0:
-        tmp = vec.clone()
-        idx = vec >= 0.5
-        tmp[idx] = 1.0 - tmp[idx]
-        t = (-2.0 * tmp.log()).sqrt()
-        x = (2.30753 + t * 0.27061) / (1.0 + t * (0.99229 + t * 0.04481)) - t
-        idx = ~idx
-        x[idx] = -x[idx]
-        al = (x.square() - 3.0) / 6.0
-        h = 2.0 / (1.0 / (2.0 * a - 1.0) + 1.0 / (2.0 * b - 1.0))
-        w = (x * math.sqrt(al + h) / h) - (1.0 / (2.0 * b - 1.0) - 1.0 / (2.0 * a - 1.0)) * (
-            al + 5.0 / 6.0 - 2.0 / (3.0 * h)
-        )
-        x = a / (a + b * (2.0 * w).exp())
-    else:
-        x = vec.clone()
-        t = math.exp(a * math.log(a / (a + b))) / a
-        w = t + math.exp(b * math.log(b / (a + b))) / b
-        idx = vec < t / w
-        x[idx] = (a * w * x[idx]).pow(1.0 / a)
-        idx = ~idx
-        x[idx] = 1.0 - (b * w * (1.0 - x[idx])).pow(1.0 / b)
-    afac = math.lgamma(a + b) - math.lgamma(a) - math.lgamma(b)
-    for _ in range(10):
-        t = (a1 * x.log() + b1 * x.neg().log1p() + afac).exp()
-        u = (inc_beta_reg(vec=x, a=a, b=b) - vec) / t
-        t = u / (1.0 - 0.5 * (u * (a1 / x - b1 / (1.0 - x))).clamp_max(max=1.0))
-        idx = (x > 0.0) & (x < 1.0)
-        x[idx] -= t[idx]
-        idx = x < 0.0
-        x[idx] = 0.5 * (x[idx] + t[idx])
-        idx = x > 1.0
-        x[idx] = 0.5 * (x[idx] + t[idx] + 1.0)
-        x = x.nan_to_num().clamp(min=_CDF_MIN, max=_CDF_MAX)
-    return x
-
-
-def pt(vec: torch.Tensor, nu: float) -> torch.Tensor:
-    if nu == 1:
-        res = vec.atan() / 3.141592653589793 + 0.5
-    elif nu == 2:
-        res = (vec / (vec.square() + 2.0).sqrt() + 1.0) / 2.0
-    elif nu == 3:
-        res = (
-            (vec / 1.7320508075688772).atan() / 3.141592653589793
-            + 0.5
-            + 0.5513288954217921 * vec / (vec.square() + 3.0)
-        )
-    elif nu == 4:
-        _ = vec.square()
-        res = (vec * (_ + 6.0) / (_ + 4.0).pow(1.5) + 1.0) / 2.0
-    elif nu == 5:
-        res = (
-            (vec / 2.23606797749979).atan() / 3.141592653589793
-            + (
-                (vec.square() * 3.0 + 25.0)
-                * 0.23725418113905902
-                * vec
-                / (vec.square() + 5.0).square()
-            )
-            + 0.5
-        )
-
-    elif nu == 6:
-        res = vec.square()
-        res = ((res.square() * 2.0 + res * 30.0 + 135.0) * vec / (res + 6.0).pow(2.5)) / 4.0 + 0.5
-
-    else:
-        nu = max(min(_NU_MAX, nu), _NU_MIN)
-        res = inc_beta_reg(vec=nu / (vec.square() + nu), a=nu / 2.0, b=0.5)
-        idx = vec > 0.0
-        res[idx] = 2.0 - res[idx]
-        res *= 0.5
-    return res.nan_to_num().clamp(min=_CDF_MIN, max=_CDF_MAX)
-
-
-def qt(vec: torch.Tensor, nu: float) -> torch.Tensor:
-    vec2 = vec * 2.0
-    nu2 = nu / 2.0
-    res = torch.empty_like(input=vec, device=vec.device)
-    idx = vec < 0.5
-    res[idx] = (inc_beta_reg_inv(vec=vec2[idx], a=nu2, b=0.5).reciprocal() - 1.0).sqrt().neg()
-    idx = ~idx
-    res[idx] = (inc_beta_reg_inv(vec=2.0 - vec2[idx], a=nu2, b=0.5).reciprocal() - 1.0).sqrt()
-    res[vec == 0.5] = 0.0
-    res *= math.sqrt(nu)
-    return res.nan_to_num()
+# # * Student's t distribution CDF (p), PPF (q), density (d)
+# def inc_beta_reg(vec: torch.Tensor, a: float, b: float) -> torch.Tensor:
+#     # * regularized incomplete beta integral, with a = 0.5, b = nu / 2, vec in [0,1]
+#     # https://stats.stackexchange.com/questions/615961/students-t-cdf-ppf-or-hypergeometric-2f1-or-betainc-using-pytorch
+#     # https://stats.stackexchange.com/questions/52341/formula-to-generate-critical-t-values-for-t-test-instead-of-using-a-look-up-arr
+#     res = torch.empty_like(vec)
+#     if (idx := vec > ((a + 1.0) / (2.0 + a + b))).any():
+#         res[idx] = 1.0 - inc_beta_reg(vec=1.0 - vec[idx], a=b, b=a)
+#     idx = ~idx
+#     x = vec[idx]
+#     qab = a + b
+#     qap = a + 1.0
+#     qam = a - 1.0
+#     c = torch.ones_like(x)
+#     d = 1.0 / (1.0 - qab * x / qap)
+#     f = d.clone()
+#     front = (
+#         -math.lgamma(a)
+#         - math.lgamma(b)
+#         + math.lgamma(a + b)
+#         - math.log(a)
+#         + x.log() * a
+#         + x.neg().log1p() * b
+#     ).exp()
+#     for i in range(1, 200):
+#         i2 = i * 2.0
+#         ai2 = a + i2
+#         nmrt = (i * (b - i) / ((qam + i2) * ai2)) * x
+#         d = (d * nmrt + 1.0).reciprocal()
+#         c = nmrt / c + 1.0
+#         f *= c * d
+#         nmrt = (-(a + i) * (qab + i) / ((qap + i2) * ai2)) * x
+#         d = (d * nmrt + 1.0).reciprocal()
+#         c = nmrt / c + 1.0
+#         cd = c * d
+#         f *= cd
+#         if ((1.0 - cd).abs() < 1e-6).all():
+#             break
+#     res[idx] = front * f
+#     return res.nan_to_num().clamp(min=_CDF_MIN, max=_CDF_MAX)
+
+
+# def inc_beta_reg_inv(vec: torch.Tensor, a: float, b: float) -> torch.Tensor:
+#     a1, b1 = a - 1.0, b - 1.0
+#     if a > 1.0 and b > 1.0:
+#         tmp = vec.clone()
+#         idx = vec >= 0.5
+#         tmp[idx] = 1.0 - tmp[idx]
+#         t = (-2.0 * tmp.log()).sqrt()
+#         x = (2.30753 + t * 0.27061) / (1.0 + t * (0.99229 + t * 0.04481)) - t
+#         idx = ~idx
+#         x[idx] = -x[idx]
+#         al = (x.square() - 3.0) / 6.0
+#         h = 2.0 / (1.0 / (2.0 * a - 1.0) + 1.0 / (2.0 * b - 1.0))
+#         w = (x * math.sqrt(al + h) / h) - (1.0 / (2.0 * b - 1.0) - 1.0 / (2.0 * a - 1.0)) * (
+#             al + 5.0 / 6.0 - 2.0 / (3.0 * h)
+#         )
+#         x = a / (a + b * (2.0 * w).exp())
+#     else:
+#         x = vec.clone()
+#         t = math.exp(a * math.log(a / (a + b))) / a
+#         w = t + math.exp(b * math.log(b / (a + b))) / b
+#         idx = vec < t / w
+#         x[idx] = (a * w * x[idx]).pow(1.0 / a)
+#         idx = ~idx
+#         x[idx] = 1.0 - (b * w * (1.0 - x[idx])).pow(1.0 / b)
+#     afac = math.lgamma(a + b) - math.lgamma(a) - math.lgamma(b)
+#     for _ in range(10):
+#         t = (a1 * x.log() + b1 * x.neg().log1p() + afac).exp()
+#         u = (inc_beta_reg(vec=x, a=a, b=b) - vec) / t
+#         t = u / (1.0 - 0.5 * (u * (a1 / x - b1 / (1.0 - x))).clamp_max(max=1.0))
+#         idx = (x > 0.0) & (x < 1.0)
+#         x[idx] -= t[idx]
+#         idx = x < 0.0
+#         x[idx] = 0.5 * (x[idx] + t[idx])
+#         idx = x > 1.0
+#         x[idx] = 0.5 * (x[idx] + t[idx] + 1.0)
+#         x = x.nan_to_num().clamp(min=_CDF_MIN, max=_CDF_MAX)
+#     return x
+
+
+# def pt(vec: torch.Tensor, nu: float) -> torch.Tensor:
+#     if nu == 1:
+#         res = vec.atan() / 3.141592653589793 + 0.5
+#     elif nu == 2:
+#         res = (vec / (vec.square() + 2.0).sqrt() + 1.0) / 2.0
+#     elif nu == 3:
+#         res = (
+#             (vec / 1.7320508075688772).atan() / 3.141592653589793
+#             + 0.5
+#             + 0.5513288954217921 * vec / (vec.square() + 3.0)
+#         )
+#     elif nu == 4:
+#         _ = vec.square()
+#         res = (vec * (_ + 6.0) / (_ + 4.0).pow(1.5) + 1.0) / 2.0
+#     elif nu == 5:
+#         res = (
+#             (vec / 2.23606797749979).atan() / 3.141592653589793
+#             + (
+#                 (vec.square() * 3.0 + 25.0)
+#                 * 0.23725418113905902
+#                 * vec
+#                 / (vec.square() + 5.0).square()
+#             )
+#             + 0.5
+#         )
+
+#     elif nu == 6:
+#         res = vec.square()
+#         res = ((res.square() * 2.0 + res * 30.0 + 135.0) * vec / (res + 6.0).pow(2.5)) / 4.0 + 0.5
+
+#     else:
+#         nu = max(min(_NU_MAX, nu), _NU_MIN)
+#         res = inc_beta_reg(vec=nu / (vec.square() + nu), a=nu / 2.0, b=0.5)
+#         idx = vec > 0.0
+#         res[idx] = 2.0 - res[idx]
+#         res *= 0.5
+#     return res.nan_to_num().clamp(min=_CDF_MIN, max=_CDF_MAX)
+
+
+# def qt(vec: torch.Tensor, nu: float) -> torch.Tensor:
+#     vec2 = vec * 2.0
+#     nu2 = nu / 2.0
+#     res = torch.empty_like(input=vec, device=vec.device)
+#     idx = vec < 0.5
+#     res[idx] = (inc_beta_reg_inv(vec=vec2[idx], a=nu2, b=0.5).reciprocal() - 1.0).sqrt().neg()
+#     idx = ~idx
+#     res[idx] = (inc_beta_reg_inv(vec=2.0 - vec2[idx], a=nu2, b=0.5).reciprocal() - 1.0).sqrt()
+#     res[vec == 0.5] = 0.0
+#     res *= math.sqrt(nu)
+#     return res.nan_to_num()
 
 
 def pt_scipy(vec: torch.Tensor, nu: float) -> torch.Tensor:
     if vec.device.type == "cpu":
         return torch.from_numpy(t.cdf(x=vec, df=nu))
     else:
         return torch.from_numpy(t.cdf(x=vec.cpu(), df=nu)).cuda()
```

### Comparing `torchvinecopulib-2024.3.3/torchvinecopulib/vinecop/_data_vcp.py` & `torchvinecopulib-2024.4.0/torchvinecopulib/vinecop/_data_vcp.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 class DataVineCop(ABC):
     """Dataclass for a vine copula model"""
 
     dct_bcp: dict
     """bivariate copulas, stored as {level: {(vertex_left, vertex_right, frozenset_cond): DataBiCop}}"""
     dct_tree: dict
     """bivariate dependency measures of edges in trees, stored as {level: {(vertex_left, vertex_right, frozenset_cond): bidep}}"""
-    lst_sim: list
+    tpl_sim: tuple
     """the source vertices (pseudo-obs) of simulation paths, read from right to left; some vertices can be given as simulated at the beginning of each simulation workflow"""
     mtd_bidep: str
     """method to calculate bivariate dependence"""
 
     @property
     def aic(self) -> float:
         """
@@ -41,29 +41,29 @@
         :return: Bayesian information criterion (BIC)
         :rtype: float
         """
         return 2.0 * self.negloglik + self.num_par * math.log(self.num_obs)
 
     @property
     def matrix(self) -> np.array:
-        """structure matrix: upper triangular, in row-major order (each row has a bicop as: vertex_left,...,vertex_right;set_and)
+        """structure matrix: upper triangular, in row-major order (each row has a bicop as: vertex_left,...,vertex_right;set_cond)
 
         :return: structure matrix
         :rtype: np.array
         """
         # NumPy arrays, like arrays in C, are stored in row-major order by default.
         # In a 2D array, the data is stored row by row: elements in the same row are stored in adjacent memory locations.
         mat = []
         lst_diag = []
         # * levels in reverse order
         for idx, lv in enumerate(sorted(self.dct_tree, reverse=True)):
             v_diag = None
             lst_nebr = [-1 for _ in range(idx)]
             for i_lv in range(lv, -1, -1):
-                for v_l, v_r, s_and in self.dct_tree[i_lv]:
+                for v_l, v_r, _ in self.dct_tree[i_lv]:
                     if (v_l not in lst_diag) and (v_r not in lst_diag):
                         if v_diag is None:
                             # ! pick the node with smaller index (v_l < v_r), then mat <-> structure is bijection
                             v_diag = v_l
                             lst_nebr.append(v_diag)
                         if v_diag in (v_l, v_r):
                             lst_nebr.append(v_l if v_diag == v_r else v_r)
@@ -108,31 +108,38 @@
         :rtype: tuple
         """
         lv_up = len(s_down) - 1
         for (v_l, v_r, s_up), bcp in self.dct_bcp[lv_up].items():
             if ({v_l, v_r} | s_up) == ({v_down} | s_down):
                 return v_l, v_r, s_up, bcp
 
-    def _ref_count(self, lst_first: list[int] = []) -> tuple[dict, list[int]]:
-        """reference counting for each vertex during simulation workflow, for garbage collection (memory release)
-
-        :param lst_first: list of vertices that are taken as already simulated at the beginning of a simulation workflow, defaults to []
-        :type lst_first: list[int], optional
-        :return: reference counting for each vertex
+    def _ref_count(
+        self,
+        tpl_first_vs: tuple[tuple[int, frozenset]] = tuple(),
+        tpl_sim: tuple[int] = tuple(),
+    ) -> tuple[dict, list[int]]:
+        """reference counting for each vertex during simulation (quant-reg/cond-sim) workflow, for garbage collection (memory release)
+
+        :param tpl_first_vs: tuple of vertices (explicitly arranged in conditioned - conditioning set) that are taken as known at the beginning of a simulation workflow, defaults to tuple()
+        :type tpl_first_vs: tuple[tuple[int, frozenset]], optional
+        :param tpl_sim: tuple of vertices in a full simulation workflow, gives flexibility to experienced users, defaults to tuple()
+        :type tpl_sim: tuple[int], optional
+        :return: reference counting for each vertex; list of source vertices in this simulation workflow from shallow to deep
         :rtype: tuple[dict, list[int]]
         """
         # * v for vertex, s for condition (frozen)set, read from right to left
-        lst_source = self.lst_sim
+        dct_first_vs = {v[0]: v for v in tpl_first_vs}
+        lst_source = tpl_sim if tpl_sim else self.tpl_sim
         lst_source = [
-            ((v, frozenset()) if v in lst_first else (v, frozenset(lst_source[(idx + 1) :])))
+            (dct_first_vs[v] if v in dct_first_vs else (v, frozenset(lst_source[(idx + 1) :])))
             for idx, v in enumerate(lst_source)
         ][::-1]
 
         # ! count in initial sim (pseudo obs that are given at the beginning of each sim path)
-        dct_ref_count = {v_s: 1 for v_s in lst_source}
+        dct_ref_count = {v_s_cond: 1 for v_s_cond in lst_source}
 
         def visit_hfunc(v_down: int, s_down: frozenset):
             v_l, v_r, s_up, _ = self._loc_bcp(v_down=v_down, s_down=s_down)
             # vertex left on upper level
             if dct_ref_count.get((v_l, s_up), 0) < 1:
                 visit_hfunc(v_down=v_l, s_down=s_up)
             dct_ref_count[v_l, s_up] += 1
@@ -173,15 +180,15 @@
         return dct_ref_count, lst_source
 
     def __repr__(self) -> str:
         return pformat(
             {
                 "dct_bcp": self.dct_bcp,
                 "dct_tree": self.dct_tree,
-                "lst_sim": self.lst_sim,
+                "tpl_sim": self.tpl_sim,
                 "mtd_bidep": self.mtd_bidep,
             },
             indent=2,
             compact=True,
             sort_dicts=True,
             underscore_numbers=True,
         )
@@ -193,15 +200,15 @@
                 "num_dim": self.num_dim,
                 "num_obs": self.num_obs,
                 "num_par": self.num_par,
                 "negloglik": round(self.negloglik, 4),
                 "aic": round(self.aic, 4),
                 "bic": round(self.bic, 4),
                 "matrix": self.matrix.__str__(),
-                "lst_sim": self.lst_sim,
+                "tpl_sim": self.tpl_sim,
             },
             compact=True,
             sort_dicts=False,
             underscore_numbers=True,
         ).replace("\\n", "")
 
     def draw_lv(
@@ -239,25 +246,24 @@
         fig, ax = plt.subplots(nrows=1, ncols=1, figsize=fig_size)
         ax.set_title(
             label=f"Vine Copula, Level {lv}, BiDep Metric {self.mtd_bidep}",
             fontsize=font_size_vertex + 1,
         )
         if lv == 0:
             tpl_uvw = tuple(
-                (u, v, round(w, ndigits=num_digit))
-                for (u, v, s_and), w in self.dct_tree[lv].items()
+                (u, v, round(w, ndigits=num_digit)) for (u, v, _), w in self.dct_tree[lv].items()
             )
         elif is_bcp:
             tpl_uvw = tuple(
                 (
-                    self._loc_bcp(v_down=u, s_down=s_and),
-                    self._loc_bcp(v_down=v, s_down=s_and),
+                    self._loc_bcp(v_down=u, s_down=s_cond),
+                    self._loc_bcp(v_down=v, s_down=s_cond),
                     round(w, ndigits=num_digit),
                 )
-                for (u, v, s_and), w in self.dct_tree[lv].items()
+                for (u, v, s_cond), w in self.dct_tree[lv].items()
             )
             tpl_uvw = tuple(
                 (
                     f"{tpl_l[0]},{tpl_l[1]};"
                     + ("" if lv == 1 else "\n")
                     + f"{','.join([str(_) for _ in sorted(tpl_l[2])])}",
                     f"{tpl_r[0]},{tpl_r[1]};"
@@ -266,19 +272,19 @@
                     w,
                 )
                 for (tpl_l, tpl_r, w) in tpl_uvw
             )
         else:
             tpl_uvw = tuple(
                 (
-                    f"{u}|{','.join([f'{_}' for _ in sorted(s_and)])}",
-                    f"{v}|{','.join([f'{_}' for _ in sorted(s_and)])}",
+                    f"{u}|{','.join([f'{_}' for _ in sorted(s_cond)])}",
+                    f"{v}|{','.join([f'{_}' for _ in sorted(s_cond)])}",
                     round(w, ndigits=num_digit),
                 )
-                for (u, v, s_and), w in self.dct_tree[lv].items()
+                for (u, v, s_cond), w in self.dct_tree[lv].items()
             )
         G = nx.Graph()
         G.add_weighted_edges_from(tpl_uvw)
         pos = nx.planar_layout(G)
         nx.draw_networkx_nodes(
             G=G,
             pos=pos,
@@ -312,38 +318,41 @@
             fig.savefig(fname=f_path, bbox_inches="tight")
             return fig, ax, G, f_path
         else:
             return fig, ax, G
 
     def draw_dag(
         self,
-        lst_first: list[int] = [],
+        tpl_first_vs: tuple = tuple(),
+        tpl_sim: tuple = tuple(),
         font_size_vertex: int = 8,
         f_path: Path = None,
         fig_size: tuple = None,
     ) -> tuple:
         """draw the directed acyclic graph (DAG) of the vine copula, with pseudo observations and bicops as nodes. The source nodes in simulation workflow are highlighted in yellow.
 
-        :param lst_first: list of vertices that are taken as already simulated at the beginning of a simulation workflow, affecting the color of nodes, defaults to []
-        :type lst_first: list[int], optional
+        :param tpl_first_vs: tuple of vertices (explicitly arranged in conditioned - conditioning set) that are taken as already simulated at the beginning of a simulation workflow, affecting the color of nodes, defaults to tuple()
+        :type tpl_first_vs: tuple, optional
+        :param tpl_sim: tuple of vertices in a full simulation workflow, gives flexibility to experienced users, defaults to tuple()
+        :type tpl_sim: tuple, optional
         :param font_size_vertex: font size for vertex labels, defaults to 8
         :type font_size_vertex: int, optional
         :param f_path: file path to save the figure, defaults to None for no saving
         :type f_path: Path, optional
         :param fig_size: figure size, defaults to None
         :type fig_size: tuple, optional
-        :return: fig, ax, (and file path if the figure is saved)
+        :return: _description_
         :rtype: tuple
         """
         import matplotlib.pyplot as plt
         import networkx as nx
 
         fig, ax = plt.subplots(nrows=1, ncols=1, figsize=fig_size)
         ax.set_title(
-            label=f"Vine Copula, Obs and BiCop",
+            label="Vine Copula, Obs and BiCop",
             fontsize=font_size_vertex + 1,
         )
         G = nx.DiGraph()
         pos_obs = {}
         pos_bcp = {}
         dct_label = {}
         for lv in self.dct_tree:
@@ -356,25 +365,25 @@
                 lst_node_up = [(_, frozenset()) for _ in range(self.num_dim)]
                 for _ in lst_node_up:
                     dct_label[_] = _[0]
                 num_node = len(lst_node_up)
                 loc_x = np.linspace(-num_node / 2, num_node / 2, num=num_node)
                 for _ in range(num_node):
                     pos_obs[lst_node_up[_]] = loc_x[_], 1
-            for (v_l, v_r, s_and), _ in self.dct_tree[lv].items():
+            for (v_l, v_r, s_cond), _ in self.dct_tree[lv].items():
                 # node bcp
-                lst_node_bcp.append((v_l, v_r, s_and))
+                lst_node_bcp.append((v_l, v_r, s_cond))
                 # node down
-                lst_node_down.append((v_l, s_and | {v_r}))
-                lst_node_down.append((v_r, s_and | {v_l}))
+                lst_node_down.append((v_l, s_cond | {v_r}))
+                lst_node_down.append((v_r, s_cond | {v_l}))
                 # edge
-                lst_edge.append(((v_l, s_and), (v_l, v_r, s_and)))
-                lst_edge.append(((v_r, s_and), (v_l, v_r, s_and)))
-                lst_edge.append(((v_l, v_r, s_and), (v_l, s_and | {v_r})))
-                lst_edge.append(((v_l, v_r, s_and), (v_r, s_and | {v_l})))
+                lst_edge.append(((v_l, s_cond), (v_l, v_r, s_cond)))
+                lst_edge.append(((v_r, s_cond), (v_l, v_r, s_cond)))
+                lst_edge.append(((v_l, v_r, s_cond), (v_l, s_cond | {v_r})))
+                lst_edge.append(((v_l, v_r, s_cond), (v_r, s_cond | {v_l})))
             # locate lower nodes
             num_node = len(lst_node_down)
             loc_x = np.linspace(-num_node / 2, num_node / 2, num=num_node)
             for _ in range(num_node):
                 pos_obs[lst_node_down[_]] = loc_x[_], -lv
             for _ in lst_node_down:
                 dct_label[_] = f"{_[0]}|{','.join([f'{__}' for __ in sorted(_[1])])}"
@@ -383,65 +392,66 @@
             loc_x = np.linspace(-num_node / 2, num_node / 2, num=num_node)
             for _ in range(num_node):
                 pos_bcp[lst_node_bcp[_]] = loc_x[_], -lv + 0.5
             for _ in lst_node_bcp:
                 __ = "\n" * min(lv, 1)
                 dct_label[_] = f"{_[0]},{_[1]};{__}{','.join([f'{__}' for __ in sorted(_[2])])}"
             G.add_edges_from(lst_edge)
-        # highlight source nodes, given lst_first
-        lst_source = self._ref_count(lst_first=lst_first)[1]
+        pos = pos_obs | pos_bcp
+        # highlight source nodes, given tpl_first
+        lst_source = self._ref_count(tpl_first_vs=tpl_first_vs, tpl_sim=tpl_sim)[1]
         # pseudo obs nodes
         lst_node = [_ for _ in G.nodes if len(_) == 2 and _ not in lst_source]
         nx.draw_networkx_nodes(
             G=G,
-            pos=pos_obs | pos_bcp,
+            pos=pos,
             ax=ax,
             nodelist=lst_node,
             node_color="white",
             node_shape="o",
             alpha=0.8,
             linewidths=0.5,
             edgecolors="gray",
         )
         nx.draw_networkx_nodes(
             G=G,
-            pos=pos_obs | pos_bcp,
+            pos=pos,
             ax=ax,
             nodelist=lst_source,
             node_color="yellow",
             node_shape="o",
             alpha=0.8,
             linewidths=0.5,
             edgecolors="gray",
         )
 
         # bicop nodes
         lst_node = [_ for _ in G.nodes if len(_) == 3]
         nx.draw_networkx_nodes(
             G=G,
-            pos=pos_obs | pos_bcp,
+            pos=pos,
             ax=ax,
             nodelist=lst_node,
             node_color="white",
             node_shape="s",
             alpha=0.8,
             linewidths=0.5,
             edgecolors="gray",
         )
         nx.draw_networkx_labels(
             G=G,
-            pos=pos_obs | pos_bcp,
+            pos=pos,
             ax=ax,
             labels=dct_label,
             font_size=font_size_vertex,
             font_color="black",
         )
         nx.draw_networkx_edges(
             G=G,
-            pos=pos_obs | pos_bcp,
+            pos=pos,
             ax=ax,
             edge_color="gray",
             width=0.5,
             style="--",
             alpha=0.8,
         )
         fig.tight_layout()
@@ -499,79 +509,163 @@
             size=(obs_mvcp.shape[0], 1),
             device=obs_mvcp.device,
             dtype=obs_mvcp.dtype,
         )
 
         def update_obs(v: int, s_cond: frozenset):
             # * calc hfunc for pseudo obs when necessary
+            # the lv of bcp
             lv = len(s_cond) - 1
-            for (v_l, v_r, s_and), bcp in self.dct_bcp[lv].items():
+            for (v_l, v_r, s_cond_bcp), bcp in self.dct_bcp[lv].items():
                 # ! notice hfunc1 or hfunc2
-                if v == v_l and s_cond == frozenset({v_r} | s_and):
-                    dct_obs[lv + 1][(v_l, s_cond)] = bcp.hfunc2(
+                if v == v_l and s_cond == frozenset({v_r} | s_cond_bcp):
+                    dct_obs[lv + 1][(v, s_cond)] = bcp.hfunc2(
                         obs=torch.hstack(
                             [
-                                dct_obs[lv][v_l, s_and],
-                                dct_obs[lv][v_r, s_and],
+                                dct_obs[lv][v_l, s_cond_bcp],
+                                dct_obs[lv][v_r, s_cond_bcp],
                             ]
                         )
                     )
-                elif v == v_r and s_cond == frozenset({v_l} | s_and):
-                    dct_obs[lv + 1][(v_r, s_cond)] = bcp.hfunc1(
+                elif v == v_r and s_cond == frozenset({v_l} | s_cond_bcp):
+                    dct_obs[lv + 1][(v, s_cond)] = bcp.hfunc1(
                         obs=torch.hstack(
                             [
-                                dct_obs[lv][v_l, s_and],
-                                dct_obs[lv][v_r, s_and],
+                                dct_obs[lv][v_l, s_cond_bcp],
+                                dct_obs[lv][v_r, s_cond_bcp],
                             ]
                         )
                     )
                 else:
                     pass
 
         for lv in self.dct_tree:
-            for (v_l, v_r, s_and), bcp in self.dct_bcp[lv].items():
+            for (v_l, v_r, s_cond), bcp in self.dct_bcp[lv].items():
                 # * update the pseudo observations
                 for idx in (v_l, v_r):
-                    if dct_obs[lv].get((idx, s_and)) is None:
-                        update_obs(v=idx, s_cond=s_and)
-                obs_l = dct_obs[lv][(v_l, s_and)]
-                obs_r = dct_obs[lv][(v_r, s_and)]
-                res += bcp.l_pdf(obs=torch.hstack([obs_l, obs_r]))
+                    if dct_obs[lv].get((idx, s_cond)) is None:
+                        update_obs(v=idx, s_cond=s_cond)
+                res += bcp.l_pdf(
+                    obs=torch.hstack(
+                        [
+                            dct_obs[lv][(v_l, s_cond)],
+                            dct_obs[lv][(v_r, s_cond)],
+                        ]
+                    )
+                )
             if lv > 0:
                 # ! garbage collection
                 del dct_obs[lv - 1]
 
         return res
 
+    def rosenblatt_transform(
+        self,
+        obs_mvcp: torch.Tensor,
+        tpl_sim: tuple = tuple(),
+    ) -> torch.Tensor:
+        """Rosenblatt transformation, from the multivariate copula (with dependence) to the uniform multivariate copula (independent), using constructed vine copula
+
+        :param obs_mvcp: observation of the multivariate copula, of shape (num_obs, num_dim)
+        :type obs_mvcp: torch.Tensor
+        :param tpl_sim: tuple of vertices (read from right to left) in a full simulation workflow, gives flexibility to experienced users, defaults to tuple()
+        :type tpl_sim: tuple, optional
+        :return: ideally independent uniform multivariate copula, of shape (num_obs, num_dim)
+        :rtype: torch.Tensor
+        """
+        num_dim = self.num_dim
+        if not tpl_sim:
+            tpl_sim = self.tpl_sim
+        tpl_sim_v_s_cond = tuple(
+            (v, frozenset(tpl_sim[idx + 1 :])) for idx, v in enumerate(tpl_sim)
+        )
+        dct_obs = {_: {} for _ in range(num_dim)}
+        dct_obs[0] = {(idx, frozenset()): obs_mvcp[:, [idx]] for idx in range(num_dim)}
+
+        def update_obs(v: int, s_cond: frozenset):
+            # * calc hfunc for pseudo obs when necessary
+            # the lv of bcp
+            lv = len(s_cond) - 1
+            for (v_l, v_r, s_cond_bcp), bcp in self.dct_bcp[lv].items():
+                # ! notice hfunc1 or hfunc2
+                if v == v_l and s_cond == frozenset({v_r} | s_cond_bcp):
+                    dct_obs[lv + 1][(v, s_cond)] = bcp.hfunc2(
+                        obs=torch.hstack(
+                            [
+                                dct_obs[lv][v_l, s_cond_bcp],
+                                dct_obs[lv][v_r, s_cond_bcp],
+                            ]
+                        )
+                    )
+                elif v == v_r and s_cond == frozenset({v_l} | s_cond_bcp):
+                    dct_obs[lv + 1][(v, s_cond)] = bcp.hfunc1(
+                        obs=torch.hstack(
+                            [
+                                dct_obs[lv][v_l, s_cond_bcp],
+                                dct_obs[lv][v_r, s_cond_bcp],
+                            ]
+                        )
+                    )
+                else:
+                    pass
+
+        for lv in self.dct_tree:
+            for (v_l, v_r, s_cond), _ in self.dct_bcp[lv].items():
+                # * update the pseudo observations
+                for idx in (v_l, v_r):
+                    if dct_obs[lv].get((idx, s_cond)) is None:
+                        update_obs(v=idx, s_cond=s_cond)
+                if (v_l, s_cond | {v_r}) in tpl_sim_v_s_cond:
+                    update_obs(v=v_l, s_cond=s_cond | {v_r})
+                if (v_r, s_cond | {v_l}) in tpl_sim_v_s_cond:
+                    update_obs(v=v_r, s_cond=s_cond | {v_l})
+            if lv > 0:
+                # ! garbage collection
+                for v_s_cond in dict(dct_obs[lv - 1]):
+                    if v_s_cond not in tpl_sim_v_s_cond:
+                        del dct_obs[lv - 1][v_s_cond]
+        dct_obs = {
+            k: v
+            for dct_lv in dct_obs.values()
+            for k, v in dct_lv.items()
+            if (k in tpl_sim_v_s_cond)
+        }
+        return dct_obs
+
     def sim(
         self,
-        num_sim: int,
-        dct_first: dict = {},
+        num_sim: int = 1,
+        dct_first_vs: dict = {},
+        tpl_sim: tuple = tuple(),
         seed: int = 0,
         device: str = "cpu",
         dtype: torch.dtype = torch.float64,
     ) -> torch.Tensor:
-        """simulate from the vine copula, as scheduled task with reference counting for garbage collection. Sequentially (from right to left) for each beginning vertex in the lst_sim, move upward by calling hinv until the top vertex (whose cond set is empty) is reached. (Recursively) call hfunc for the other upper vertex if necessary.
+        """full simulation/ quantile-regression/ conditional-simulation using the vine copula. Sequentially for each beginning vertex in the tpl_sim (from right to left, as from shallower lv to deeper lv in the DAG), walk upward by calling hinv until the top vertex (whose cond set is empty) is reached. (Recursively) call hfunc for the other upper vertex if necessary.
 
-        :param num_sim: number of simulations
+        :param num_sim: number of simulations; ignored when dct_first_vs is not empty
         :type num_sim: int
-        :param dct_first: dict of {idx: torch.Tensor(size=(n,1))} in cond sim, where vertices are taken as already simulated at the beginning of a simulation workflow; intentionally asking for explicit user input, defaults to {}
-        :type dct_first: dict, optional
+        :param dct_first_vs: dict of {(vertex,cond_set): torch.Tensor(size=(n,1))} in quantile regression/ conditional simulation, where vertices are taken as given already; defaults to {}
+        :type dct_first_vs: dict, optional
+        :param tpl_sim: tuple of vertices (read from right to left) in a full simulation workflow, gives flexibility to experienced users, defaults to tuple()
+        :type tpl_sim: tuple, optional
         :param seed: random seed for torch.manual_seed(), defaults to 0
         :type seed: int, optional
         :param device: device for torch.rand(), defaults to 'cpu'
         :type device: str, optional
         :param dtype: dtype for torch.rand(), defaults to torch.float64
         :type dtype: torch.dtype, optional
         :return: simulated observations of the vine copula, of shape (num_sim, num_dim)
         :rtype: torch.Tensor
         """
-        dct_obs = {}
+        dct_obs = dct_first_vs.copy()
         # * source vertices in each path; reference counting for whole DAG
-        dct_ref_count, lst_source = self._ref_count(lst_first=list(dct_first))
+        dct_ref_count, lst_source = self._ref_count(
+            tpl_first_vs=tuple(dct_first_vs), tpl_sim=tpl_sim
+        )
 
         def _update_ref_count(v: int, s: frozenset) -> None:
             # * countdown and release memory if necessary
             dct_ref_count[v, s] -= 1
             if dct_ref_count[v, s] < 1:
                 del dct_obs[v, s]
 
@@ -630,30 +724,32 @@
                 (v_down, s_up),
             ):
                 _update_ref_count(v=v, s=s)
             # * return the next vertex
             return v_down, s_up
 
         torch.manual_seed(seed=seed)
-        num_dim = self.num_dim
         # * init sim of U_mvcp (multivariate independent copula)
-        U_mvcp = torch.rand(size=(num_sim, num_dim - len(dct_first)), device=device, dtype=dtype)
+        dim_sim = self.num_dim - len(dct_first_vs)
+        if dim_sim > 0:
+            # ! skip for quant-reg
+            U_mvcp = torch.rand(size=(num_sim, dim_sim), device=device, dtype=dtype)
         # * update dct_obs and dct_ref_count
         idx = 0
         for v, s in lst_source:
-            if v in dct_first:
-                dct_obs[v, s] = dct_first[v]
-            else:
+            if (v, s) not in dct_obs:
                 dct_obs[v, s] = U_mvcp[:, [idx]]
                 idx += 1
             # ! let the top level obs (target vertices) escape garbage collection
             dct_ref_count[v, frozenset()] += 1
             # update ref count
             dct_ref_count[v, s] -= 1
-        del seed, num_dim, U_mvcp, dct_first, idx
+        del seed, dct_first_vs, idx
+        if dim_sim > 0:
+            del U_mvcp
         for v, s in lst_source:
             # walk the path if cond set is not empty
             if len(s):
                 # call hinv and update vertex/cond-set iteratively to walk towards target vertex (top lv)
                 v_next, s_next = visit_hinv(v_down=v, s_down=s)
                 while len(s_next):
                     v_next, s_next = visit_hinv(v_down=v_next, s_down=s_next)
```

### Comparing `torchvinecopulib-2024.3.3/torchvinecopulib/vinecop/_factory_vcp.py` & `torchvinecopulib-2024.4.0/torchvinecopulib/vinecop/_factory_vcp.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,36 +1,38 @@
-import math
 import pickle
 from collections import deque
-from itertools import combinations, product
+from itertools import combinations
 from operator import itemgetter
 from pathlib import Path
 from typing import Deque
 
 import numpy as np
 import torch
 
 from ..bicop import bcp_from_obs
 from ..util import ENUM_FUNC_BIDEP
 from ._data_vcp import DataVineCop
 
 
-def _mst_from_edge_rvine(lst_key_obs: list, dct_edge_lv: dict) -> list:
-    """Construct Kruskal's MAXIMUM spanning tree (MST) from bivariate copula edges, using modified disjoint set/ union find.
+def _mst_from_edge_rvine(tpl_key_obs: tuple, dct_edge_lv: dict, s_rest: set) -> list:
+    """Construct Kruskal's MAXIMUM spanning tree (MST) from bivariate copula edges, restricted to rvine, using modified disjoint set/ union find.
 
-    :param lst_key_obs: list of keys of (pseudo) observations, each key is a tuple of (vertex, cond set)
-    :type lst_key_obs: list
-    :param dct_edge_lv: dictionary of edges (vertex_l, vertex_r, cond set) and corresponding bivariate dependence metric value
+    :param tpl_key_obs: tuple of keys of (pseudo) observations, each key is a tuple of (vertex, cond set)
+    :type tpl_key_obs: tuple
+    :param dct_edge_lv: dictionary of edges (vertex_left, vertex_right, cond_set) and corresponding bivariate dependence metric value
     :type dct_edge_lv: dict
+    :param s_rest: vertices to be kept deeper in the simulation workflow (static, wont update at each level)
+    :type s_rest: set
     :return: list of edges (vertex_l, vertex_r, cond set) in the MST
-    :rtype: _type_
+    :rtype: list
     """
     # * edge2tree, rvine (Kruskal's MST, disjoint set/ union find)
-    # ! modify 'parent' to let pseudo obs linked to previous bicop edge
-    parent = {k_obs: frozenset((k_obs[0], *k_obs[1])) for k_obs in lst_key_obs}
+    # ! modify 'parent' to let a pseudo obs vertex linked to its previous bicop vertex
+    parent = {v_s_cond: frozenset((v_s_cond[0], *v_s_cond[1])) for v_s_cond in tpl_key_obs}
+    # * and bicop vertices are linked to themselves
     parent = {**parent, **{v: v for _, v in parent.items()}}
     rank = {k_obs: 0 for k_obs in parent}
     mst = []
 
     def find(v):
         if parent[v] != v:
             parent[v] = find(parent[v])
@@ -41,389 +43,456 @@
         if rank[root_a] < rank[root_b]:
             parent[root_a] = root_b
         else:
             parent[root_b] = root_a
             if rank[root_b] == rank[root_a]:
                 rank[root_a] += 1
 
+    # ! filter for edges that DONT touch rest set vertices
+    dct_edge = {
+        (v_l, v_r, s_cond): bidep
+        for (v_l, v_r, s_cond), bidep in dct_edge_lv.items()
+        if ((v_l not in s_rest) and (v_r not in s_rest))
+    }
     # * notice we sort edges by ABS(bidep) in DESCENDING order
-    for (v_l, v_r, s_and), bidep_abs in sorted(
-        dct_edge_lv.items(), key=lambda x: abs(x[1]), reverse=True
-    ):
-        if find((v_l, s_and)) != find((v_r, s_and)):
-            mst.append((v_l, v_r, s_and))
-            union((v_l, s_and), (v_r, s_and))
+    for (v_l, v_r, s_cond), _ in sorted(dct_edge.items(), key=lambda x: abs(x[1]), reverse=True):
+        if find((v_l, s_cond)) != find((v_r, s_cond)):
+            mst.append((v_l, v_r, s_cond))
+            union((v_l, s_cond), (v_r, s_cond))
+    # ! filter for edges that touch rest set vertices
+    dct_edge = set(dct_edge_lv) - set(dct_edge)
+    if dct_edge:
+        dct_edge = {k: v for k, v in dct_edge_lv.items() if k in dct_edge}
+        for (v_l, v_r, s_cond), _ in sorted(
+            dct_edge.items(), key=lambda x: abs(x[1]), reverse=True
+        ):
+            if find((v_l, s_cond)) != find((v_r, s_cond)):
+                mst.append((v_l, v_r, s_cond))
+                union((v_l, s_cond), (v_r, s_cond))
     return mst
 
 
 def _mst_from_edge_cvine(
-    lst_key_obs: list, dct_edge_lv: dict, s_first: set, deq_sim: Deque
+    tpl_key_obs: tuple, dct_edge_lv: dict, s_first: set, deq_sim: Deque
 ) -> tuple:
     """Construct Kruskal's MAXIMUM spanning tree (MST) from bivariate copula edges, restricted to cvine
 
-    :param lst_key_obs: list of keys of (pseudo) observations, each key is a tuple of (vertex, cond set)
-    :type lst_key_obs: list
-    :param dct_edge_lv: dictionary of edges (vertex_l, vertex_r, cond set) and corresponding bivariate dependence metric value
+    :param tpl_key_obs: tuple of keys of (pseudo) observations, each key is a tuple of (vertex, cond set)
+    :type tpl_key_obs: tuple
+    :param dct_edge_lv: dictionary of edges (vertex_left, vertex_right, cond set) and corresponding bivariate dependence metric value
     :type dct_edge_lv: dict
-    :param s_first: set of vertices that are prioritized to be first in the simulation workflow
-    :type s_first: set
-    :param deq_sim: deque of vertices, to record the order of simulation (read from right to left, as simulated pseudo-obs vertices from shallowest to deepest level)
+    :param deq_sim: deque of vertices, as simulation workflow (read from right to left, as simulated pseudo-obs vertices from shallowest to deepest level) (dynamically updated at each level)
     :type deq_sim: Deque
-    :return: list of edges (vertex_l, vertex_r, cond set) in the MST; updated deq_sim; updated s_first
+    :param s_first: set of vertices that are kept shallower in the simulation workflow (dynamically updated at each level)
+    :type s_first: set
+    :return: list of edges (vertex_left, vertex_right, cond set) in the MST; updated deq_sim; updated s_first
     :rtype: tuple
     """
     # * edge2tree, cvine (MST, restricted to cvine)
     # init dict, the sum of abs bidep for each vertex
     if s_first:
-        # prioritize this set; only consider edges from/to vertices in this set
-        dct_bidep_abs_sum = {v_s: 0 for v_s in lst_key_obs if v_s[0] in s_first}
-        dct_edge_lv = {
-            (v_l, v_r, s_and): bidep
-            for ((v_l, v_r, s_and), bidep) in dct_edge_lv.items()
-            if ((v_l in s_first) or (v_r in s_first))
-        }
+        # ! filter for edges that touch first set vertices
+        dct_bidep_abs_sum = {v_s_cond: 0 for v_s_cond in tpl_key_obs if v_s_cond[0] in s_first}
     else:
-        dct_bidep_abs_sum = {v_s: 0 for v_s in lst_key_obs}
-    for (v_l, v_r, s_and), bidep in dct_edge_lv.items():
+        dct_bidep_abs_sum = {v_s_cond: 0 for v_s_cond in tpl_key_obs}
+    for (v_l, v_r, s_cond), bidep in dct_edge_lv.items():
         # cum sum of abs bidep for each vertex
-        if (v_l, s_and) in dct_bidep_abs_sum:
-            dct_bidep_abs_sum[(v_l, s_and)] += abs(bidep)
-        if (v_r, s_and) in dct_bidep_abs_sum:
-            dct_bidep_abs_sum[(v_r, s_and)] += abs(bidep)
+        if (v_l, s_cond) in dct_bidep_abs_sum:
+            dct_bidep_abs_sum[(v_l, s_cond)] += abs(bidep)
+        if (v_r, s_cond) in dct_bidep_abs_sum:
+            dct_bidep_abs_sum[(v_r, s_cond)] += abs(bidep)
     # center vertex (and its cond set) for cvine at this level
-    v_c, s_c = sorted(dct_bidep_abs_sum.items(), key=itemgetter(1))[-1][0]
-    # record edges from/to the center vertex
+    for (v_c, s_cond_c), _ in sorted(dct_bidep_abs_sum.items(), key=itemgetter(1), reverse=True):
+        # ! exclude those already in deq_sim
+        if v_c not in deq_sim:
+            break
+    # record edges that touch the center vertex
     mst = [
-        (v_l, v_r, s_and)
-        for (v_l, v_r, s_and) in dct_edge_lv
-        if ((s_and == s_c) and ((v_c == v_l) or (v_c == v_r)))
+        (v_l, v_r, s_cond)
+        for (v_l, v_r, s_cond) in dct_edge_lv
+        if ((s_cond == s_cond_c) and ((v_c == v_l) or (v_c == v_r)))
     ]
     # update the deq_sim, let those sim first be last in the deq_sim
     deq_sim.appendleft(v_c)
     if len(mst) == 1:
         # for the last lv, only one edge left, appendleft the other vertex into deq_sim
         deq_sim.appendleft(v_l if v_l != v_c else v_r)
-    # update the priority set
+    # update the first set
     s_first -= {v_c}
     # * mst(cvine), deq_sim, s_first
     return mst, deq_sim, s_first
 
 
-def _mst_from_edge_dvine(lst_key_obs: list, dct_edge_lv: dict, s_first: set) -> tuple:
-    """Construct Kruskal's MAXIMUM spanning tree (MST) from bivariate copula edges, restricted to dvine
+def _mst_from_edge_dvine(tpl_key_obs: tuple, dct_edge_lv: dict, s_first: set) -> tuple:
+    """Construct Kruskal's MAXIMUM spanning tree (MST) from bivariate copula edges, restricted to dvine. For dvine the whole struct (and sim flow) is known after lv0, and this func is only called at lv0.
 
-    :param lst_key_obs: list of keys of (pseudo) observations, each key is a tuple of (vertex, cond set)
-    :type lst_key_obs: list
+    :param tpl_key_obs: tuple of keys of (pseudo) observations, each key is a tuple of (vertex, cond set)
+    :type tpl_key_obs: tuple
     :param dct_edge_lv: dictionary of edges (vertex_l, vertex_r, cond set) and corresponding bivariate dependence metric value
     :type dct_edge_lv: dict
-    :param s_first: set of vertices that are prioritized to be first in the simulation workflow
+    :param s_first: set of vertices that are kept shallower in the simulation workflow
     :type s_first: set
     :return: list of edges (vertex_l, vertex_r, cond set) in the MST (lv0); updated deq_sim; emptied s_first
     :rtype: tuple
     """
     # * edge2tree, dvine (MST, restricted to dvine)
-    # for dvine the whole struct (and sim flow) is known after lv0, and this func is only called at lv0.
-    # ! at lv0, s_and is known to be empty
-    from networkx import Graph
-    from networkx.algorithms.approximation import threshold_accepting_tsp
-
-    # revert bidep into cost per edge for TSP
-    dct_cost = {
-        (v_l, v_r): math.log1p(1 / max(abs(bidep), 1e-10))
-        for (v_l, v_r, s_and), bidep in dct_edge_lv.items()
-    }
-    G = Graph()
-    G.add_weighted_edges_from([(*k, v) for k, v in dct_cost.items()])
-    s_rest = set(G.nodes) - s_first
-    # rest set: build tsp
-    tsp_rest = threshold_accepting_tsp(G.subgraph(nodes=s_rest), init_cycle="greedy")
-    len_first = len(s_first)
-    if len_first == 0:
-        # just drop the top cost edge in s_rest, when s_first is empty
-        rest_drop_cost = -math.inf
-        mst_lv0 = []
-        for idx, v_rest in enumerate(tsp_rest):
-            if idx < 1:
-                continue
-            edge = (*sorted((v_rest, tsp_rest[idx - 1])),)
-            mst_lv0.append(edge)
-            edge_cost = dct_cost[edge]
-            if edge_cost > rest_drop_cost:
-                rest_drop = edge
-                rest_drop_cost = edge_cost
-        mst_lv0 = [(*sorted(_), frozenset()) for _ in mst_lv0 if _ != edge]
-
+    # * at lv0, s_cond is known to be empty
+    if len(tpl_key_obs) < 3:
+        # ! only two vertices
+        v_head, v_tail = tpl_key_obs
+        v_head, v_tail = v_head[0], v_tail[0]
+        mst = [(v_head, v_tail, frozenset())]
     else:
-        # ! drop one edge from tsp_first and one from tsp_rest, then add an edge connecting two sets
-        # ! iter all combinations, decide drop fwd/bwd, then calculate cost difference for each (drop,drop,add) modification
-        # * drop: pick the edge to drop (from the hamiltonian circle), either fwd or bwd that has higher cost
-        # rest set: record forward/backward links
-        num_dim = len(s_rest)
-        dct_rest_fwd = {v: tsp_rest[idx + 1] for idx, v in enumerate(tsp_rest) if idx < num_dim}
-        dct_rest_bwd = {v: tsp_rest[idx - 1] for idx, v in enumerate(tsp_rest) if idx > 0}
-        # ! when s_first has only one element, nothing to drop.
-        first_drop, first_drop_cost = (None, None), 0
-        if len_first > 1:
-            # cond set: build tsp, record forward/backward links
-            tsp_first = threshold_accepting_tsp(
-                G=G.subgraph(nodes=s_first),
-                init_cycle="greedy",
+        # ! more than two vertices
+        import math
+        from networkx import Graph
+        from networkx.algorithms.approximation import threshold_accepting_tsp
+
+        dct_cost = {
+            (v_l, v_r): math.log1p(1 / max(abs(bidep), 1e-10))
+            for (v_l, v_r, s_cond), bidep in dct_edge_lv.items()
+        }
+        G = Graph()
+        G.add_weighted_edges_from([(*k, v) for k, v in dct_cost.items()])
+        s_rest = set(G.nodes) - s_first
+        if (not s_first) or (not s_rest):
+            # ! one set is empty: global TSP
+            tsp = threshold_accepting_tsp(G, init_cycle="greedy")
+            # * fetch the edges in the TSP, drop the one with max cost
+            mst = [
+                tuple(sorted((v, tsp[idx - 1]))) for idx, v in enumerate(tsp, start=0) if idx > 0
+            ]
+            s_l_r_cost = sorted(
+                [(v_l, v_r, dct_cost[(v_l, v_r)]) for v_l, v_r in mst],
+                key=lambda x: x[-1],
+                reverse=True,
             )
-            dct_first_fwd = {
-                v: tsp_first[idx + 1] for idx, v in enumerate(tsp_first) if idx < len_first
-            }
-            dct_first_bwd = {v: tsp_first[idx - 1] for idx, v in enumerate(tsp_first) if idx > 0}
-        cost_diff = math.inf
-        for v_first, v_rest in product(s_first, s_rest):
-            if len_first > 2:
-                # ! drop an edge from cond set, only when s_first has more than 2 elements
-                first_drop = (*sorted((v_first, dct_first_fwd[v_first])),)
-                first_drop_cost = dct_cost[first_drop]
-                edge = (*sorted((v_first, dct_first_bwd[v_first])),)
-                edge_cost = dct_cost[edge]
-                if edge_cost > first_drop_cost:
-                    first_drop, first_drop_cost = edge, edge_cost
-            # drop an edge from rest set
-            rest_drop = (*sorted((v_rest, dct_rest_fwd[v_rest])),)
-            rest_drop_cost = dct_cost[rest_drop]
-            edge = (*sorted((v_rest, dct_rest_bwd[v_rest])),)
-            edge_cost = dct_cost[edge]
-            if edge_cost > rest_drop_cost:
-                rest_drop, rest_drop_cost = edge, edge_cost
-            # add an edge to connect two sets
-            edge = (*sorted((v_first, v_rest)),)
-            # record total cost diff (as forming a hamiltonian path from two hamiltonian circles)
-            tmp_cost_diff = dct_cost[edge] - first_drop_cost - rest_drop_cost
-            if tmp_cost_diff < cost_diff:
-                drop_drop_add = (first_drop, rest_drop, edge)
-                cost_diff = tmp_cost_diff
-        # mst: add, drop, drop
-        mst_lv0 = [] if len_first < 2 else [(*sorted((k, v)),) for k, v in dct_first_fwd.items()]
-        mst_lv0 += [(*sorted((k, v)),) for k, v in dct_rest_fwd.items()]
-        mst_lv0 += [drop_drop_add[2]]
-        mst_lv0 = list({(*_, frozenset()) for _ in mst_lv0 if _ not in drop_drop_add[:-1]})
-    # ! for dvine, deq_sim is known and s_first is empty now
-    s_edge = {(v_l, v_r) for v_l, v_r, s_and in mst_lv0}
-    deq_sim = deque()
-    num_dim = len(lst_key_obs)
-    while len(deq_sim) < num_dim:
-        for v_l, v_r in set(s_edge):
-            if len(deq_sim) < 1:
-                deq_sim.append(v_l)
-                deq_sim.append(v_r)
-                s_edge.remove((v_l, v_r))
-            elif v_l == deq_sim[0]:
-                deq_sim.appendleft(v_r)
-                s_edge.remove((v_l, v_r))
-            elif v_l == deq_sim[-1]:
+            mst = s_l_r_cost[1:]
+            mst = [(v_l, v_r, frozenset()) for (v_l, v_r, _) in mst]
+            v_head, v_tail, _ = s_l_r_cost[0]
+        elif len(s_first) in (1, len(tpl_key_obs) - 1):
+            # ! one set is a singleton (head-neck-...-tail: add head-neck, drop neck-tail)
+            tsp, v_head = (
+                (s_first, list(s_rest)[0]) if len(s_rest) == 1 else (s_rest, list(s_first)[0])
+            )
+            # * TSP on the subgraph without the singleton
+            tsp = threshold_accepting_tsp(G.subgraph(tsp), init_cycle="greedy")
+            # * loop over the TSP and pick the combination with min cost
+            tsp.append(tsp[1])
+            cost = math.inf
+            for idx, v in enumerate(tsp[1:-1], start=1):
+                v_prev, v_next = tsp[idx - 1], tsp[idx + 1]
+                # tail given neck
+                if (cost_next := dct_cost[tuple(sorted((v, v_next)))]) > (
+                    cost_prev := dct_cost[tuple(sorted((v, v_prev)))]
+                ):
+                    v_nebr, cost_nebr = v_next, cost_next
+                else:
+                    v_nebr, cost_nebr = v_prev, cost_prev
+                # neck
+                if (i_cost := dct_cost[tuple(sorted((v_head, v)))] - cost_nebr) < cost:
+                    v_tail, v_neck, cost = v_nebr, v, i_cost
+            mst = [(*sorted((v_head, v_neck)), frozenset())]
+            for idx, v in enumerate(tsp[1:-1], start=1):
+                v_l, v_r = sorted((v, tsp[idx + 1]))
+                if {v_l, v_r} != {v_neck, v_tail}:
+                    mst.append((v_l, v_r, frozenset()))
+        else:
+            # ! both sets have more than one vertex (head-...-neck-body-...-tail, drop head-neck, add neck-body, drop body-tail)
+            tsp_first = threshold_accepting_tsp(G.subgraph(s_first), init_cycle="greedy")
+            tsp_first.append(tsp_first[1])
+            tsp_rest = threshold_accepting_tsp(G.subgraph(s_rest), init_cycle="greedy")
+            tsp_rest.append(tsp_rest[1])
+            cost = math.inf
+            # * loop over two TSPs and pick the combination with min cost
+            for idx_neck, _v_neck in enumerate(tsp_first[1:-1], start=1):
+                # * for the first TSP, drop head-neck
+                v_prev, v_next = tsp_first[idx_neck - 1], tsp_first[idx_neck + 1]
+                if (cost_next := dct_cost[tuple(sorted((_v_neck, v_next)))]) > (
+                    cost_prev := dct_cost[tuple(sorted((_v_neck, v_prev)))]
+                ):
+                    v_nebr_neck, cost_nebr_neck = v_next, cost_next
+                else:
+                    v_nebr_neck, cost_nebr_neck = v_prev, cost_prev
+                for idx_body, _v_body in enumerate(tsp_rest[1:-1], start=1):
+                    # * for the second TSP, drop body-tail
+                    v_prev, v_next = tsp_rest[idx_body - 1], tsp_rest[idx_body + 1]
+                    if (cost_next := dct_cost[tuple(sorted((_v_body, v_next)))]) > (
+                        cost_prev := dct_cost[tuple(sorted((_v_body, v_prev)))]
+                    ):
+                        v_nebr_body, cost_nebr_body = v_next, cost_next
+                    else:
+                        v_nebr_body, cost_nebr_body = v_prev, cost_prev
+                    if (
+                        i_cost := dct_cost[tuple(sorted((_v_neck, _v_body)))]
+                        - cost_nebr_neck
+                        - cost_nebr_body
+                    ) < cost:
+                        # ! cost, drop head-neck, drop body-tail, add neck-body
+                        v_head, v_neck, v_body, v_tail, cost = (
+                            v_nebr_neck,
+                            _v_neck,
+                            _v_body,
+                            v_nebr_body,
+                            i_cost,
+                        )
+            mst = [(*sorted((v_neck, v_body)), frozenset())]
+            if len(tsp_first) == 4:
+                mst.append((*sorted((v_head, v_neck)), frozenset()))
+            else:
+                for idx, v in enumerate(tsp_first[1:-1], start=1):
+                    v_l, v_r = sorted((v, tsp_first[idx + 1]))
+                    if {v_l, v_r} != {v_head, v_neck}:
+                        mst.append((v_l, v_r, frozenset()))
+            if len(tsp_rest) == 4:
+                mst.append((*sorted((v_body, v_tail)), frozenset()))
+            else:
+                for idx, v in enumerate(tsp_rest[1:-1], start=1):
+                    v_l, v_r = sorted((v, tsp_rest[idx + 1]))
+                    if {v_l, v_r} != {v_body, v_tail}:
+                        mst.append((v_l, v_r, frozenset()))
+    # * sim workflow, chain the vertices in deq_sim
+    deq_sim = deque([v_head])
+    s_edge = set(mst)
+    while deq_sim[-1] != v_tail:
+        for v_l, v_r, s_cond in set(s_edge):
+            if v_l == deq_sim[-1]:
                 deq_sim.append(v_r)
-                s_edge.remove((v_l, v_r))
-            elif v_r == deq_sim[0]:
-                deq_sim.appendleft(v_l)
-                s_edge.remove((v_l, v_r))
+                s_edge.remove((v_l, v_r, s_cond))
             elif v_r == deq_sim[-1]:
                 deq_sim.append(v_l)
-                s_edge.remove((v_l, v_r))
-    # let those sim first be last in the lst_sim
-    if s_first and (deq_sim[0] in s_first):
+                s_edge.remove((v_l, v_r, s_cond))
+    # ! let those sim first (s_first) be last in the tpl_sim
+    if deq_sim[0] in s_first:
         deq_sim.reverse()
     # * mst(dvine), deq_sim, s_first
-    return mst_lv0, deq_sim, {}
+    return mst, deq_sim, {}
 
 
 def vcp_from_obs(
     obs_mvcp: torch.Tensor,
     is_Dissmann: bool = True,
-    cdrvine: str = "rvine",
-    lst_first: list[int] = [],
     matrix: np.ndarray | None = None,
+    tpl_first: tuple[int] = tuple(),
+    mtd_vine: str = "rvine",
     mtd_bidep: str = "chatterjee_xi",
+    thresh_trunc: float = 0.1,
     mtd_fit: str = "itau",
     mtd_mle: str = "COBYLA",
     mtd_sel: str = "aic",
     tpl_fam: tuple[str, ...] = (
         "Clayton",
         "Frank",
         "Gaussian",
         "Gumbel",
         "Independent",
         "Joe",
     ),
     topk: int = 2,
 ) -> DataVineCop:
-    """Construct a vine copula model from multivariate observations, with structure prescribed by either Dissmann's (MST per level) method or a given matrix. May prioritize some vertices to be first in the cond simulation workflow.
+    """Construct a vine copula model from multivariate observations, with structure prescribed by either Dissmann's (MST per level) method or a given matrix. May prioritize some vertices to be first (shallower) in the quantile-regression/conditional-simulation workflow.
 
     :param obs_mvcp: multivariate observations, of shape (num_obs, num_dim)
     :type obs_mvcp: torch.Tensor
     :param is_Dissmann: whether to use Dissmann's method or follow a given matrix, defaults to True; Dissmann, J., Brechmann, E. C., Czado, C., & Kurowicka, D. (2013). Selecting and estimating regular vine copulae and application to financial returns. Computational Statistics & Data Analysis, 59, 52-69.
     :type is_Dissmann: bool, optional
-    :param cdrvine: one of 'cvine', 'dvine', 'rvine', defaults to "rvine"
-    :type cdrvine: str, optional
-    :param lst_first: list of vertices to be prioritized in the cond sim workflow, only used when cdrvine is "cvine" or "dvine". if empty then no priority is set, defaults to []
-    :type lst_first: list[int], optional
-    :param matrix: matrix of vine copula structure, of shape (num_dim, num_dim), used when is_Dissmann is False, defaults to None
+    :param mtd_vine: one of 'cvine', 'dvine', 'rvine', defaults to "rvine"
+    :type mtd_vine: str, optional
+    :param tpl_first: tuple of vertices to be prioritized (kept shallower) in the cond sim workflow. if empty then no priority is set, defaults to tuple()
+    :type tpl_first: tuple[int], optional
+    :param matrix: a matrix of vine copula structure, of shape (num_dim, num_dim), used when is_Dissmann is False, defaults to None
     :type matrix: np.ndarray | None, optional
     :param mtd_bidep: method to calculate bivariate dependence, one of "kendall_tau", "mutual_info", "ferreira_tail_dep_coeff", "chatterjee_xi", "wasserstein_dist_ind", defaults to "chatterjee_xi"
     :type mtd_bidep: str, optional
+    :param thresh_trunc: threshold of Kendall's tau independence test, below which we reject independent bicop, defaults to 0.1
+    :type thresh_trunc: float, optional
     :param mtd_fit: method to fit bivariate copula, either 'itau' (inverse of tau) or 'mle' (maximum likelihood estimation); defaults to "itau"
     :type mtd_fit: str, optional
     :param mtd_mle: optimization method for mle as used by scipy.optimize.minimize, defaults to "COBYLA"
     :type mtd_mle: str, optional
     :param mtd_sel: bivariate copula model selection criterion, either 'aic' or 'bic'; defaults to "aic"
     :type mtd_sel: str, optional
-    :param tpl_fam: tuple of str as candidate family names to fit bicop, could be a subset of ('Clayton', 'Frank', 'Gaussian', 'Gumbel', 'Independent', 'Joe', 'StudentT')
+    :param tpl_fam: tuple of str as candidate family names to fit bicop, could be a subset of ('Clayton', 'Frank', 'Gaussian', 'Gumbel', 'Independent', 'Joe', 'StudentT'), defaults to ( "Clayton", "Frank", "Gaussian", "Gumbel", "Independent", "Joe")
     :type tpl_fam: tuple[str, ...], optional
-    :param topk: number of best itau fit taken into further mle, used when mtd_fit is 'mle'; defaults to 2
+    :param topk: number of best "itau" fit taken into further "mle", used when mtd_fit is "mle"; defaults to 2
     :type topk: int, optional
-    :raises ValueError: when cdrvine is not one of 'cvine', 'dvine', 'rvine'
-    :return: a fitted DataVineCop object
+    :raises ValueError: when mtd_vine is not one of 'cvine', 'dvine', 'rvine'
+    :return: a constructed DataVineCop object
     :rtype: DataVineCop
     """
+    is_kendall_tau = mtd_bidep == "kendall_tau"
     f_bidep = ENUM_FUNC_BIDEP[mtd_bidep]._value_
     num_dim = obs_mvcp.shape[1]
-    s_first = set(lst_first) if lst_first else set()
-    # * a list to record the order of sim (read from right to left, as simulated pseudo-obs vertices from shallowest to deepest level)
+    s_first = set(tpl_first)
+    s_rest = set(range(num_dim)) - s_first
+    # ! an object to record the order of sim (read from right to left, as simulated pseudo-obs vertices from shallowest to deepest level)
     deq_sim = deque()
     r_D1 = range(num_dim - 1)
     dct_obs = {_: {} for _ in r_D1}
     # * tree is either from Dissmann (MST on edges, needs to record edges) or from matrix
     if is_Dissmann:
         dct_edge = {_: {} for _ in r_D1}
     dct_tree = {_: {} for _ in r_D1}
     dct_bcp = {_: {} for _ in r_D1}
 
     def _update_obs(v: int, s_cond: frozenset) -> torch.Tensor:
         """calc hfunc for pseudo obs and update dct_obs, only when necessary (lazy hfunc)"""
+        # * v and s_cond are from the pseudo obs
         lv = len(s_cond)
-        lv_1 = lv - 1
-        for (v_l, v_r, s_and), bcp in dct_bcp[lv_1].items():
+        # * lv_bcp and s_cond_bcp mark the prev lv and bcp cond set
+        lv_bcp = lv - 1
+        for (v_l, v_r, s_cond_bcp), bcp in dct_bcp[lv_bcp].items():
             # ! notice hfunc1 or hfunc2
-            if (v == v_l) and (s_cond == frozenset({v_r} | s_and)):
+            if (v == v_l) and (s_cond == frozenset({v_r} | s_cond_bcp)):
                 dct_obs[lv][(v_l, s_cond)] = bcp.hfunc2(
                     obs=torch.hstack(
                         [
-                            dct_obs[lv_1][v_l, s_and],
-                            dct_obs[lv_1][v_r, s_and],
+                            dct_obs[lv_bcp][v_l, s_cond_bcp],
+                            dct_obs[lv_bcp][v_r, s_cond_bcp],
                         ]
                     )
                 )
-            elif (v == v_r) and (s_cond == frozenset({v_l} | s_and)):
+            elif (v == v_r) and (s_cond == frozenset({v_l} | s_cond_bcp)):
                 dct_obs[lv][(v_r, s_cond)] = bcp.hfunc1(
                     obs=torch.hstack(
                         [
-                            dct_obs[lv_1][v_l, s_and],
-                            dct_obs[lv_1][v_r, s_and],
+                            dct_obs[lv_bcp][v_l, s_cond_bcp],
+                            dct_obs[lv_bcp][v_r, s_cond_bcp],
                         ]
                     )
                 )
 
     for lv in r_D1:
-        # ! lv_0 obs, preprocess to append a cond frozenset (s_and)
+        # * lv_0 obs, preprocess to append an empty frozenset (s_cond)
         if lv == 0:
             dct_obs[0] = {(idx, frozenset()): obs_mvcp[:, [idx]] for idx in range(num_dim)}
         if is_Dissmann:
             # * obs2edge, list possible edges that connect two pseudo obs, calc f_bidep
-            lst_key_obs = dct_obs[lv].keys()
-            for tpl_l, tpl_r in combinations(lst_key_obs, 2):
-                # ! only those obs with same 'cond set' (the frozen set) can have edges (proximity condition)
-                if tpl_l[1] == tpl_r[1]:
+            tpl_key_obs = dct_obs[lv].keys()
+            for (v_l, s_cond_l), (v_r, s_cond_r) in combinations(tpl_key_obs, 2):
+                # ! proximity condition: only those obs with same 'cond set' (the frozen set) can have edges
+                if s_cond_l == s_cond_r:
                     # ! sorted !
-                    v_l, v_r = sorted((tpl_l[0], tpl_r[0]))
-                    s_and = tpl_l[1]
-                    if dct_obs[lv][v_l, s_and] is None:
-                        _update_obs(v_l, s_and)
-                    if dct_obs[lv][v_r, s_and] is None:
-                        _update_obs(v_r, s_and)
-                    dct_edge[lv][(v_l, v_r, s_and)] = f_bidep(
-                        x=dct_obs[lv][v_l, s_and],
-                        y=dct_obs[lv][v_r, s_and],
-                    )
-            if cdrvine == "dvine":
+                    v_l, v_r = sorted((v_l, v_r))
+                    if dct_obs[lv][v_l, s_cond_l] is None:
+                        _update_obs(v_l, s_cond_l)
+                    if dct_obs[lv][v_r, s_cond_l] is None:
+                        _update_obs(v_r, s_cond_l)
+                    if is_kendall_tau:
+                        dct_edge[lv][(v_l, v_r, s_cond_l)] = f_bidep(
+                            x=dct_obs[lv][v_l, s_cond_l],
+                            y=dct_obs[lv][v_r, s_cond_l],
+                        )[0]
+                    else:
+                        dct_edge[lv][(v_l, v_r, s_cond_l)] = f_bidep(
+                            x=dct_obs[lv][v_l, s_cond_l],
+                            y=dct_obs[lv][v_r, s_cond_l],
+                        )
+            if mtd_vine == "dvine":
                 # * edge2tree, dvine
+                # ! for dvine, the whole struct (and deq_sim) is known after lv0
                 if lv == 0:
-                    # ! for dvine the whole struct (and deq_sim) is known after lv0
                     mst, deq_sim, s_first = _mst_from_edge_dvine(
-                        lst_key_obs=lst_key_obs,
+                        tpl_key_obs=tpl_key_obs,
                         dct_edge_lv=dct_edge[lv],
                         s_first=s_first,
                     )
                     dct_tree[lv] = {key_edge: dct_edge[lv][key_edge] for key_edge in mst}
                 else:
                     dct_tree[lv] = dct_edge[lv]
-            elif cdrvine == "cvine":
+            elif mtd_vine == "cvine":
                 # * edge2tree, cvine
-                # ! for cvine, at each lv the center vertex is chosen to be the one with the largest sum of abs bidep
+                # ! for cvine, at each lv the center vertex is the one with the largest sum of abs bidep
                 mst, deq_sim, s_first = _mst_from_edge_cvine(
-                    lst_key_obs=lst_key_obs,
+                    tpl_key_obs=tpl_key_obs,
                     dct_edge_lv=dct_edge[lv],
                     s_first=s_first,
                     deq_sim=deq_sim,
                 )
                 dct_tree[lv] = {key_edge: dct_edge[lv][key_edge] for key_edge in mst}
-            elif cdrvine == "rvine":
+            elif mtd_vine == "rvine":
                 # * edge2tree, rvine
-                mst = _mst_from_edge_rvine(lst_key_obs=lst_key_obs, dct_edge_lv=dct_edge[lv])
+                mst = _mst_from_edge_rvine(
+                    tpl_key_obs=tpl_key_obs,
+                    dct_edge_lv=dct_edge[lv],
+                    s_rest=s_rest,
+                )
                 dct_tree[lv] = {key_edge: dct_edge[lv][key_edge] for key_edge in mst}
             else:
-                raise ValueError("cdrvine must be one of 'cvine', 'dvine', 'rvine'")
+                raise ValueError("mtd_vine must be one of 'cvine', 'dvine', 'rvine'")
         else:
             # * tree structure is inferred from matrix, if not Dissmann
             for idx in range(num_dim - lv - 1):
                 # ! sorted !
                 v_l, v_r = sorted((matrix[idx, idx], matrix[idx, num_dim - lv - 1]))
-                s_and = frozenset(matrix[idx, (num_dim - lv) :])
-                if dct_obs[lv][v_l, s_and] is None:
-                    _update_obs(v=v_l, s_cond=s_and)
-                if dct_obs[lv][v_r, s_and] is None:
-                    _update_obs(v=v_r, s_cond=s_and)
-                dct_tree[lv][(v_l, v_r, s_and)] = f_bidep(
-                    x=dct_obs[lv][v_l, s_and],
-                    y=dct_obs[lv][v_r, s_and],
-                )
+                s_cond = frozenset(matrix[idx, (num_dim - lv) :])
+                if dct_obs[lv][v_l, s_cond] is None:
+                    _update_obs(v=v_l, s_cond=s_cond)
+                if dct_obs[lv][v_r, s_cond] is None:
+                    _update_obs(v=v_r, s_cond=s_cond)
+                if is_kendall_tau:
+                    dct_tree[lv][(v_l, v_r, s_cond)] = f_bidep(
+                        x=dct_obs[lv][(v_l, s_cond)],
+                        y=dct_obs[lv][(v_r, s_cond)],
+                    )[0]
+                else:
+                    dct_tree[lv][(v_l, v_r, s_cond)] = f_bidep(
+                        x=dct_obs[lv][(v_l, s_cond)],
+                        y=dct_obs[lv][(v_r, s_cond)],
+                    )
         # * tree2bicop, fit bicop & record key of potential pseudo obs for next lv (lazy hfunc later)
-        for (v_l, v_r, s_and), bidep in dct_tree[lv].items():
-            dct_bcp[lv][(v_l, v_r, s_and)] = bcp_from_obs(
+        for (v_l, v_r, s_cond), bidep in dct_tree[lv].items():
+            dct_bcp[lv][(v_l, v_r, s_cond)] = bcp_from_obs(
                 obs_bcp=torch.hstack(
-                    [dct_obs[lv][v_l, s_and], dct_obs[lv][v_r, s_and]],
+                    [dct_obs[lv][v_l, s_cond], dct_obs[lv][v_r, s_cond]],
                 ),
                 tau=bidep if mtd_bidep == "kendall_tau" else None,
+                thresh_trunc=thresh_trunc,
                 mtd_fit=mtd_fit,
                 mtd_mle=mtd_mle,
                 mtd_sel=mtd_sel,
                 tpl_fam=tpl_fam,
                 topk=topk,
             )
             i_lv_next = lv + 1
             if i_lv_next < num_dim - 1:
-                dct_obs[i_lv_next][v_r, s_and | {v_l}] = None
-                dct_obs[i_lv_next][v_l, s_and | {v_r}] = None
+                dct_obs[i_lv_next][v_r, s_cond | {v_l}] = None
+                dct_obs[i_lv_next][v_l, s_cond | {v_r}] = None
         # ! garbage collection
         if is_Dissmann:
             del dct_edge[lv]
         if lv > 0:
             del dct_obs[lv - 1]
     # * for cvine/dvine, deq_sim is known and s_first is empty now
-    # * for rvine, deq_sim is empty and to be filled by diag of matrix
+    # * for rvine, deq_sim is empty and to be arranged
     if not deq_sim:
         for lv in sorted(dct_tree, reverse=True):
-            v_diag = None
-            for i_lv in range(lv, -1, -1):
-                for v_l, v_r, s_and in dct_tree[i_lv]:
-                    if (v_diag is None) and (v_l not in deq_sim) and (v_r not in deq_sim):
-                        # ! pick the node with smaller index (v_l < v_r), then mat <-> structure is bijection
-                        v_diag = v_l
-                        deq_sim.append(v_diag)
-                        if lv == 0:
+            for v_l, v_r, s_cond in dct_tree[lv]:
+                # ! if this bcp vertex is not yet in the paths of existing deq_sim elements
+                if (v_l not in deq_sim) and (v_r not in deq_sim):
+                    # ! obs in set_rest but not yet arranged in deq_sim
+                    if s_tmp := s_rest - set(deq_sim):
+                        if v_l in s_tmp:
+                            deq_sim.append(v_l)
+                        else:
+                            deq_sim.append(v_r)
+                    else:
+                        # ! pick the node with smaller index (v_l < v_r), then sim paths <-> structure is bijection
+                        deq_sim.append(v_l)
+                    if lv == 0:
+                        if v_l in deq_sim:
                             deq_sim.append(v_r)
-                        break
+                        else:
+                            deq_sim.append(v_l)
+                    break
 
     return DataVineCop(
         dct_bcp=dct_bcp,
         dct_tree=dct_tree,
-        lst_sim=list(deq_sim),
+        tpl_sim=tuple(deq_sim),
         mtd_bidep=mtd_bidep,
     )
 
 
 def vcp_from_json(f_path: Path = Path("./vcp.json")) -> DataVineCop:
     """load a DataVineCop from a json file
 
@@ -435,15 +504,15 @@
     from ..bicop import DataBiCop
 
     with open(f_path, "r") as file:
         obj = eval(file.read())
     return DataVineCop(
         dct_bcp=obj["dct_bcp"],
         dct_tree=obj["dct_tree"],
-        lst_sim=obj["lst_sim"],
+        tpl_sim=obj["tpl_sim"],
         mtd_bidep=obj["mtd_bidep"],
     )
 
 
 def vcp_from_pkl(f_path: Path = Path("./vcp.pkl")) -> DataVineCop:
     """load a DataVineCop from a pickle file
```

### Comparing `torchvinecopulib-2024.3.3/PKG-INFO` & `torchvinecopulib-2024.4.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchvinecopulib
-Version: 2024.3.3
+Version: 2024.4.0
 Summary: yet another vine copula library for PyTorch.
 Home-page: https://github.com/TY-Cheng/torchvinecopulib
 License: GNU GPLv3
 Keywords: vine copula,copula,torch
 Author: Tuoyuan Cheng
 Author-email: cty120120@gmail.com
 Maintainer: Xiaosheng You
@@ -27,26 +27,30 @@
 Project-URL: Documentation, https://ty-cheng.github.io/torchvinecopulib/
 Project-URL: Repository, https://github.com/TY-Cheng/torchvinecopulib
 Description-Content-Type: text/markdown
 
 # TorchVineCopuLib
 
 [![Python package](https://github.com/TY-Cheng/torchvinecopulib/actions/workflows/python-package.yml/badge.svg?branch=main)](https://github.com/TY-Cheng/torchvinecopulib/actions/workflows/python-package.yml)
-[![Deploy Docs](https://github.com/TY-Cheng/torchvinecopulib/actions/workflows/static.yml/badge.svg?branch=main)](https://github.com/TY-Cheng/torchvinecopulib/actions/workflows/static.yml)
-[![Codacy Badge](https://app.codacy.com/project/badge/Coverage/e8a7a7448b2043d9bbefafc5a3ec14f7)](https://app.codacy.com?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_coverage)
 ![Static Badge](https://img.shields.io/badge/Python-%203.10%7C3.11%7C3.12-blue)
+[![Codacy Badge](https://app.codacy.com/project/badge/Coverage/e8a7a7448b2043d9bbefafc5a3ec14f7)](https://app.codacy.com?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_coverage)
+[![Deploy Docs](https://github.com/TY-Cheng/torchvinecopulib/actions/workflows/static.yml/badge.svg?branch=main)](https://github.com/TY-Cheng/torchvinecopulib/actions/workflows/static.yml)
 [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
 ![PyPI - Version](https://img.shields.io/pypi/v/torchvinecopulib?style=flat)
+[![DOI](https://zenodo.org/badge/768037665.svg)](https://zenodo.org/doi/10.5281/zenodo.10836953)
+
 
 Yet another vine copula package, using [PyTorch](https://pytorch.org/get-started/locally/).
 
+- C/D/R-Vine full simulation/ quantile-regression/ conditoinal-simulation, all in one package
+  - Flexible simulation workflow for experienced users
 - Vectorized tensor computation with GPU (`device='cuda'`) support
 - Shorter runtimes for higher dimension simulations
 - Decoupled dataclasses and factory methods
-- Pure `Python` library, tested against [pyvinecopulib](https://github.com/vinecopulib/pyvinecopulib/) on Windows, Linux, MacOS
+- Pure `Python` library, inspired by and tested against [pyvinecopulib](https://github.com/vinecopulib/pyvinecopulib/) on Windows, Linux, MacOS
 - IO and visualization support
 
 ## Dependencies
 
 ```toml
 # inside the `./pyproject.toml` file
 python = "^3.10"
@@ -78,17 +82,17 @@
 ```
 
 By `pip` from `./dist/*.whl` or `./dist/*.tar.gz` in this repo.
 Need to use proper file name.
 
 ```bash
 # inside project root folder
-pip install ./dist/torchvinecopulib-2024.3.3-py3-none-any.whl
+pip install ./dist/torchvinecopulib-2024.4.0-py3-none-any.whl
 # or
-pip install ./dist/torchvinecopulib-2024.3.3.tar.gz
+pip install ./dist/torchvinecopulib-2024.4.0.tar.gz
 ```
 
 ## Examples
 
 Visit the `./examples/` folder for `.ipynb` Jupyter notebooks.
 
 ## Documentation
@@ -134,18 +138,17 @@
 - Include a clear and descriptive title and description for your pull request.
 - Make sure all tests pass before submitting the pull request.
 - If your pull request addresses an open issue, reference the issue number in the description using the syntax `#issue_number`.
 - [in-place ops can be slower](https://discuss.pytorch.org/t/are-inplace-operations-faster/61209/4)
 - [torch.jit.script can be slower](https://discuss.pytorch.org/t/why-is-torch-jit-script-slower/120131/6)
 
 ### TODO
-
-1. more `bicop` class in `torch`
-2. potentially deprecating `'mle'` from `mtd_fit`
-3. bivariate dependence funcs in `util.ENUM_FUNC_BIDEP`, resolve non-`torch` pkg dependencies (`scikit-learn`, `pot`)
+1. non-par bicop
+2. more (non-parametric) `bicop` class in `torch`
+3. potentially deprecating `'mle'` from `mtd_fit`
 
 ## License
 
 > Copyright (C) 2024 Tuoyuan Cheng, Xiaosheng You, Kan Chen
 >
 > This file is part of torchvinecopulib.
 > torchvinecopulib is free software: you can redistribute it and/or modify
```


# Comparing `tmp/smefit-0.0.1.tar.gz` & `tmp/smefit-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smefit-0.0.1.tar", max compression
+gzip compressed data, was "smefit-3.0.0.tar", max compression
```

## Comparing `smefit-0.0.1.tar` & `smefit-3.0.0.tar`

### file list

```diff
@@ -1,36 +1,39 @@
--rw-r--r--   0        0        0    35149 2022-10-06 13:01:10.427621 smefit-0.0.1/LICENSE
--rw-r--r--   0        0        0     3279 2023-11-23 08:31:42.774123 smefit-0.0.1/README.md
--rw-r--r--   0        0        0     2047 2023-12-01 09:04:35.977391 smefit-0.0.1/pyproject.toml
--rw-r--r--   0        0        0       64 2022-10-06 13:01:10.484631 smefit-0.0.1/src/smefit/__init__.py
--rw-r--r--   0        0        0     2419 2022-12-05 16:17:19.754782 smefit-0.0.1/src/smefit/analyze/__init__.py
--rw-r--r--   0        0        0    68429 2022-10-27 09:11:48.505803 smefit-0.0.1/src/smefit/analyze/assets/index.css
--rw-r--r--   0        0        0      854 2022-10-27 09:11:48.507792 smefit-0.0.1/src/smefit/analyze/assets/index.html
--rw-r--r--   0        0        0     4204 2022-10-27 09:11:48.509790 smefit-0.0.1/src/smefit/analyze/assets/style.css
--rw-r--r--   0        0        0    13591 2023-11-23 14:37:58.089613 smefit-0.0.1/src/smefit/analyze/chi2_utils.py
--rw-r--r--   0        0        0    19738 2023-11-23 14:37:58.091616 smefit-0.0.1/src/smefit/analyze/coefficients_utils.py
--rw-r--r--   0        0        0     4793 2023-11-23 14:37:58.093618 smefit-0.0.1/src/smefit/analyze/contours_2d.py
--rw-r--r--   0        0        0     3018 2023-03-24 15:18:56.140026 smefit-0.0.1/src/smefit/analyze/correlations.py
--rw-r--r--   0        0        0    14578 2023-11-23 14:37:58.096638 smefit-0.0.1/src/smefit/analyze/fisher.py
--rw-r--r--   0        0        0     3653 2023-11-23 14:37:58.098606 smefit-0.0.1/src/smefit/analyze/html_utils.py
--rw-r--r--   0        0        0     2595 2023-11-23 14:37:58.100619 smefit-0.0.1/src/smefit/analyze/latex_tools.py
--rw-r--r--   0        0        0    26415 2022-10-06 13:01:10.528621 smefit-0.0.1/src/smefit/analyze/logo.png
--rw-r--r--   0        0        0    13046 2023-11-23 14:37:58.102620 smefit-0.0.1/src/smefit/analyze/pca.py
--rw-r--r--   0        0        0    16505 2023-12-01 08:20:54.602559 smefit-0.0.1/src/smefit/analyze/report.py
--rw-r--r--   0        0        0     6614 2023-11-23 14:37:58.106610 smefit-0.0.1/src/smefit/analyze/summary.py
--rw-r--r--   0        0        0     3239 2023-03-24 15:18:56.190023 smefit-0.0.1/src/smefit/basis_rotation.py
--rw-r--r--   0        0        0     8146 2023-11-23 14:37:58.108620 smefit-0.0.1/src/smefit/chi2.py
--rw-r--r--   0        0        0     4159 2023-12-01 08:20:54.604560 smefit-0.0.1/src/smefit/cli/__init__.py
--rw-r--r--   0        0        0      277 2022-10-06 13:01:10.587634 smefit-0.0.1/src/smefit/cli/base.py
--rw-r--r--   0        0        0     8462 2023-11-23 14:37:58.113606 smefit-0.0.1/src/smefit/coefficients.py
--rw-r--r--   0        0        0     1884 2022-11-01 07:24:53.158469 smefit-0.0.1/src/smefit/compute_theory.py
--rw-r--r--   0        0        0     3757 2023-11-23 14:37:58.115609 smefit-0.0.1/src/smefit/covmat.py
--rw-r--r--   0        0        0     4922 2023-11-23 14:37:58.116622 smefit-0.0.1/src/smefit/fit_manager.py
--rw-r--r--   0        0        0    18597 2023-11-23 08:31:38.099131 smefit-0.0.1/src/smefit/loader.py
--rw-r--r--   0        0        0     1135 2022-10-06 13:01:10.600622 smefit-0.0.1/src/smefit/log.py
--rw-r--r--   0        0        0     3861 2023-11-23 14:37:58.118615 smefit-0.0.1/src/smefit/optimize/__init__.py
--rw-r--r--   0        0        0    10089 2023-11-23 14:37:58.120607 smefit-0.0.1/src/smefit/optimize/mc.py
--rw-r--r--   0        0        0     9879 2023-11-23 14:37:58.122614 smefit-0.0.1/src/smefit/optimize/ultranest.py
--rw-r--r--   0        0        0     3348 2023-11-23 14:37:58.123626 smefit-0.0.1/src/smefit/postfit/__init__.py
--rw-r--r--   0        0        0     1566 2023-12-01 08:20:54.606562 smefit-0.0.1/src/smefit/prefit/__init__.py
--rw-r--r--   0        0        0     7287 2023-11-23 14:37:58.125623 smefit-0.0.1/src/smefit/runner.py
--rw-r--r--   0        0        0     4582 1970-01-01 00:00:00.000000 smefit-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-04-24 12:58:04.270236 smefit-3.0.0/LICENSE
+-rw-r--r--   0        0        0     3053 2024-04-24 12:58:04.270236 smefit-3.0.0/README.md
+-rw-r--r--   0        0        0     2091 2024-04-24 12:58:04.390237 smefit-3.0.0/pyproject.toml
+-rw-r--r--   0        0        0       64 2024-04-24 12:58:04.410237 smefit-3.0.0/src/smefit/__init__.py
+-rw-r--r--   0        0        0     2419 2024-04-24 12:58:04.410237 smefit-3.0.0/src/smefit/analyze/__init__.py
+-rw-r--r--   0        0        0    68429 2024-04-24 12:58:04.410237 smefit-3.0.0/src/smefit/analyze/assets/index.css
+-rw-r--r--   0        0        0      854 2024-04-24 12:58:04.410237 smefit-3.0.0/src/smefit/analyze/assets/index.html
+-rw-r--r--   0        0        0     4204 2024-04-24 12:58:04.410237 smefit-3.0.0/src/smefit/analyze/assets/style.css
+-rw-r--r--   0        0        0    13593 2024-04-24 12:58:04.410237 smefit-3.0.0/src/smefit/analyze/chi2_utils.py
+-rw-r--r--   0        0        0    32688 2024-04-24 12:58:04.410237 smefit-3.0.0/src/smefit/analyze/coefficients_utils.py
+-rw-r--r--   0        0        0     6093 2024-04-24 12:58:04.410237 smefit-3.0.0/src/smefit/analyze/contours_2d.py
+-rw-r--r--   0        0        0     3139 2024-04-24 12:58:04.410237 smefit-3.0.0/src/smefit/analyze/correlations.py
+-rw-r--r--   0        0        0    14556 2024-04-24 12:58:04.410237 smefit-3.0.0/src/smefit/analyze/fisher.py
+-rw-r--r--   0        0        0     3653 2024-04-24 12:58:04.410237 smefit-3.0.0/src/smefit/analyze/html_utils.py
+-rw-r--r--   0        0        0     2630 2024-04-24 12:58:04.410237 smefit-3.0.0/src/smefit/analyze/latex_tools.py
+-rw-r--r--   0        0        0    26415 2024-04-24 12:58:04.410237 smefit-3.0.0/src/smefit/analyze/logo.png
+-rw-r--r--   0        0        0    13045 2024-04-24 12:58:04.410237 smefit-3.0.0/src/smefit/analyze/pca.py
+-rw-r--r--   0        0        0    19282 2024-04-24 12:58:04.410237 smefit-3.0.0/src/smefit/analyze/report.py
+-rw-r--r--   0        0        0     3897 2024-04-24 12:58:04.410237 smefit-3.0.0/src/smefit/analyze/spider.py
+-rw-r--r--   0        0        0     6534 2024-04-24 12:58:04.410237 smefit-3.0.0/src/smefit/analyze/summary.py
+-rw-r--r--   0        0        0     3239 2024-04-24 12:58:04.410237 smefit-3.0.0/src/smefit/basis_rotation.py
+-rw-r--r--   0        0        0     8194 2024-04-24 12:58:04.410237 smefit-3.0.0/src/smefit/chi2.py
+-rw-r--r--   0        0        0     5627 2024-04-24 12:58:04.410237 smefit-3.0.0/src/smefit/cli/__init__.py
+-rw-r--r--   0        0        0      277 2024-04-24 12:58:04.410237 smefit-3.0.0/src/smefit/cli/base.py
+-rw-r--r--   0        0        0     8462 2024-04-24 12:58:04.410237 smefit-3.0.0/src/smefit/coefficients.py
+-rw-r--r--   0        0        0     1884 2024-04-24 12:58:04.410237 smefit-3.0.0/src/smefit/compute_theory.py
+-rw-r--r--   0        0        0     3757 2024-04-24 12:58:04.410237 smefit-3.0.0/src/smefit/covmat.py
+-rw-r--r--   0        0        0     4975 2024-04-24 12:58:04.410237 smefit-3.0.0/src/smefit/fit_manager.py
+-rw-r--r--   0        0        0    19474 2024-04-24 12:58:04.410237 smefit-3.0.0/src/smefit/loader.py
+-rw-r--r--   0        0        0     1135 2024-04-24 12:58:04.410237 smefit-3.0.0/src/smefit/log.py
+-rw-r--r--   0        0        0     5890 2024-04-24 12:58:04.410237 smefit-3.0.0/src/smefit/optimize/__init__.py
+-rw-r--r--   0        0        0     6242 2024-04-24 12:58:04.410237 smefit-3.0.0/src/smefit/optimize/analytic.py
+-rw-r--r--   0        0        0    10462 2024-04-24 12:58:04.410237 smefit-3.0.0/src/smefit/optimize/mc.py
+-rw-r--r--   0        0        0    10426 2024-04-24 12:58:04.410237 smefit-3.0.0/src/smefit/optimize/ultranest.py
+-rw-r--r--   0        0        0     3348 2024-04-24 12:58:04.410237 smefit-3.0.0/src/smefit/postfit/__init__.py
+-rw-r--r--   0        0        0     1519 2024-04-24 12:58:04.410237 smefit-3.0.0/src/smefit/prefit/__init__.py
+-rw-r--r--   0        0        0    12000 2024-04-24 12:58:04.410237 smefit-3.0.0/src/smefit/projections/__init__.py
+-rw-r--r--   0        0        0    10013 2024-04-24 12:58:04.410237 smefit-3.0.0/src/smefit/runner.py
+-rw-r--r--   0        0        0     4335 1970-01-01 00:00:00.000000 smefit-3.0.0/PKG-INFO
```

### Comparing `smefit-0.0.1/LICENSE` & `smefit-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `smefit-0.0.1/README.md` & `smefit-3.0.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -15,21 +15,14 @@
 
 To install smefit you can do:
 
 ```bash
 pip install smefit
 ```
 
-Note this installation does not allow you to run in parallel mode.
-To do that you can install from source using the provided conda environment
-or if you have an MPI compiler available just add:
-
-```bash
-pip install mpi4py
-```
 
 ## Installation from source using conda
 You can install smefit from source using a conda environnement.
 To install it you need a [conda](https://docs.conda.io/en/latest/) installation and run:
 
 ```bash
 ./install.sh -n <env_name='smefit_installation'>
```

#### html2text {}

```diff
@@ -1,17 +1,14 @@
                                    _[_S_M_E_F_i_T_]
  _[_T_e_s_t_s_]_[_h_t_t_p_s_:_/_/_c_o_d_e_c_o_v_._i_o_/_g_h_/_L_H_C_f_i_t_N_i_k_h_e_f_/_s_m_e_f_i_t___r_e_l_e_a_s_e_/_b_r_a_n_c_h_/_m_a_i_n_/_g_r_a_p_h_/
                     _b_a_d_g_e_._s_v_g_?_t_o_k_e_n_=_M_R_T_E_X_U_P_8_X_U_]_[_C_o_d_e_F_a_c_t_o_r_]
 [SMEFiT](https://lhcfitnikhef.github.io/smefit_release/index.html) is a python
 program for Standard Model Effective Field Theory fits ## Installation To
-install smefit you can do: ```bash pip install smefit ``` Note this
-installation does not allow you to run in parallel mode. To do that you can
-install from source using the provided conda environment or if you have an MPI
-compiler available just add: ```bash pip install mpi4py ``` ## Installation
-from source using conda You can install smefit from source using a conda
+install smefit you can do: ```bash pip install smefit ``` ## Installation from
+source using conda You can install smefit from source using a conda
 environnement. To install it you need a [conda](https://docs.conda.io/en/
 latest/) installation and run: ```bash ./install.sh -n
 'smefit_installation'> ``` The installed package will be available in an
 environnement called `smefit_installation`, to activate it you can do: ```bash
 conda activate
 'smefit_installation'> smefit -h ``` ## Running The fitting code provide two
 equivalent fitting strategies. To run the code with `Nested Sampling` you can
```

### Comparing `smefit-0.0.1/pyproject.toml` & `smefit-3.0.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "smefit"
-version = "0.0.1"
+version = "3.0.0"
 description = "Standard Model Effective Field Theory Fitter"
 authors = [
     "Tommaso Giani <tgiani@nikhef.nl>",
     "Giacomo Magni <gmagni@nikhef.nl>",
-    "Jaco Ter Hoeve <i.j.ter.hoeve@vu.nl>",
+    "Jaco ter Hoeve <i.j.ter.hoeve@vu.nl>",
 ]
 license = "LICENSE"
 readme = "README.md"
 keywords = ["packaging", "dependency", "infer", "pyproject.toml"]
 homepage = "https://lhcfitnikhef.github.io/smefit_release/"
 repository = "https://github.com/LHCfitNikhef/smefit_release"
 classifiers=[
@@ -22,25 +22,27 @@
   "Programming Language :: Python :: 3",
   "Topic :: Scientific/Engineering",
   "Topic :: Scientific/Engineering :: Physics",
 ]
 
 # Requirements
 [tool.poetry.dependencies]
-python = ">=3.8,<=3.11.6"
+python = ">=3.10,<=3.11.8"
 rich="^11.2.0"
 matplotlib="^3.7.4"
 pyyaml="^6.0.1"
 numpy="^1.21.5"
 pandas="^1.4.1"
-ultranest="^3.6.4"
+ultranest="3.6.4"
 scipy="^1.8.0"
 click="^8.1.3"
 cma="^3.2.2"
 seaborn="^0.11.2"
+mpi4py-mpich="^3.1.5"
+arviz="^0.18.0"
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
 Sphinx = "^4.3.2"
 sphinx-rtd-theme = "^1.0.0"
@@ -78,16 +80,16 @@
 
 
 [tool.pytest.ini_options]
 testpaths = ['tests/']
 python_files = ['test_*.py', 'benchmark_*.py']
 python_classes = ['Test*', 'Benchmark*']
 python_functions = ['test_*', 'benchmark_*']
-addopts = [
-  '--cov=smefit',
-  '--cov-report=html',
-  '--cov-report=xml',
-  '--strict-markers',
-]
+#addopts = [
+#  '--cov=smefit',
+#  '--cov-report=html',
+#  '--cov-report=xml',
+#  '--strict-markers',
+#]
 
 [tool.poetry.scripts]
 smefit = "smefit.cli:base_command"
```

### Comparing `smefit-0.0.1/src/smefit/analyze/__init__.py` & `smefit-3.0.0/src/smefit/analyze/__init__.py`

 * *Files identical despite different names*

### Comparing `smefit-0.0.1/src/smefit/analyze/assets/index.css` & `smefit-3.0.0/src/smefit/analyze/assets/index.css`

 * *Files identical despite different names*

### Comparing `smefit-0.0.1/src/smefit/analyze/assets/index.html` & `smefit-3.0.0/src/smefit/analyze/assets/index.html`

 * *Files identical despite different names*

### Comparing `smefit-0.0.1/src/smefit/analyze/assets/style.css` & `smefit-3.0.0/src/smefit/analyze/assets/style.css`

 * *Files identical despite different names*

### Comparing `smefit-0.0.1/src/smefit/analyze/chi2_utils.py` & `smefit-3.0.0/src/smefit/analyze/chi2_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -353,15 +353,15 @@
             chi2_bar.shape[0] * 10,
             ls="dashed",
             color="grey",
             lw=0.5,
         )
         plt.tick_params(axis="x", direction="in", labelsize=15)
         plt.xlabel(r"$\chi^2$", fontsize=20)
-        plt.xlim(0, chi2_bar.max().max() + 0.01)
+        plt.xlim(-0.1, chi2_bar.max().max() + 0.2)
         plt.legend(loc="upper right", frameon=False, prop={"size": 11})
         plt.tight_layout()
         plt.savefig(f"{fig_name}.pdf")
         plt.savefig(f"{fig_name}.png")
 
     def plot_dist(self, chi2_hist, fig_name, figsize=(7, 5)):
         r"""Plots the :math:`\chi^2` distribution."""
```

### Comparing `smefit-0.0.1/src/smefit/analyze/coefficients_utils.py` & `smefit-3.0.0/src/smefit/analyze/coefficients_utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,19 +1,25 @@
 # -*- coding: utf-8 -*-
 import itertools
 import pathlib
 from collections.abc import Iterable
 
+import arviz
+import matplotlib.lines as mlines
+import matplotlib.markers as markers
+import matplotlib.patches as patches
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
+import seaborn as sns
 from matplotlib import cm
 
-from .contours_2d import plot_contours
+from .contours_2d import confidence_ellipse, plot_contours, split_solution
 from .latex_tools import latex_packages, multicolum_table_header
+from .spider import radar_factory
 
 
 def get_confidence_values(dist, has_posterior=True):
     """
     Get confidence level bounds given the distribution
     """
     cl_vals = {}
@@ -32,31 +38,23 @@
         cl_vals["mid"] = dist["bestfit"]
 
     for cl in [68, 95]:
         cl_vals[f"mean_err{cl}"] = (cl_vals[f"high{cl}"] - cl_vals[f"low{cl}"]) / 2.0
         cl_vals[f"err{cl}_low"] = cl_vals["mid"] - cl_vals[f"low{cl}"]
         cl_vals[f"err{cl}_high"] = cl_vals[f"high{cl}"] - cl_vals["mid"]
 
-    return cl_vals
-
-
-def split_solution(full_solution):
-    """Split the posterior solution"""
+        # highest density intervals
+        hdi_widths = np.diff(
+            arviz.hdi(dist.values, hdi=cl * 1e-2, multimodal=True), axis=1
+        )
+        cl_vals[f"hdi_{cl}"] = np.sum(hdi_widths.flatten())
 
-    min_val = min(full_solution)
-    max_val = max(full_solution)
-    mid = np.mean([max_val, min_val])
-
-    # solution 1 should be closer to 0
-    solution1 = full_solution[full_solution < mid]
-    solution2 = full_solution[full_solution > mid]
-    if min(abs(solution2)) < min(abs(solution1)):
-        solution1, solution2 = solution2, solution1
+    cl_vals["pull"] = cl_vals["mid"] / cl_vals["mean_err68"]
 
-    return solution1, solution2
+    return cl_vals
 
 
 def compute_confidence_level(
     posterior, coeff_info, has_posterior, disjointed_list=None
 ):
     """
     Compute central value, 95 % and 68 % confidence levels and store the result in a dictionary
@@ -87,15 +85,14 @@
             if name in disjointed_list:
                 solution1, solution2 = split_solution(posterior[name])
                 bounds[(group, latex_name)] = pd.DataFrame(
                     [get_confidence_values(solution1), get_confidence_values(solution2)]
                 ).stack()
             # single solution
             else:
-
                 bounds[(group, latex_name)] = pd.DataFrame(
                     [get_confidence_values(posterior[name], has_posterior)]
                 ).stack()
     return pd.DataFrame(bounds)
 
 
 class CoefficientsPlotter:
@@ -124,35 +121,34 @@
         coefficients latex names by gropup type
     logo : bool
         if True dispaly the logo on scatter and bar plots
 
     """
 
     def __init__(self, report_path, coeff_config, logo=False):
-
         self.report_folder = report_path
         self.coeff_info = coeff_config
 
         # SMEFiT logo
         if logo:
             self.logo = plt.imread(
                 f"{pathlib.Path(__file__).absolute().parent}/logo.png"
             )
         else:
             self.logo = None
 
         self.npar = self.coeff_info.shape[0]
 
-    def _plot_logo(self, ax):
+    def _plot_logo(self, ax, extent=[0.8, 0.999, 0.001, 0.30]):
         if self.logo is not None:
             ax.imshow(
                 self.logo,
                 aspect="auto",
                 transform=ax.transAxes,
-                extent=[0.8, 0.999, 0.001, 0.30],
+                extent=extent,
                 zorder=-1,
             )
 
     def _get_suplblots(self, figsize):
         groups = self.coeff_info.groupby(level=0).count()
         _, axs = plt.subplots(
             groups.size,
@@ -270,14 +266,27 @@
         """
         Plot error bars at given confidence level
 
         Parameters
         ----------
             error: dict
                confidence level bounds per fit and coefficient
+            figsize: list, optional
+                Figure size, (10, 15) by default
+            plot_cutoff: float
+                Only show bounds up to here
+            x_log: bool, optional
+                Use a log scale on the x-axis, true by default
+            x_min: float, optional
+                Minimum x-value, 1e-2 by default
+            x_max: float, optional
+                Maximum x-value, 500 by default
+            legend_loc: string, optional
+                Legend location, "best" by default
+
         """
         df = pd.DataFrame(error)
         groups, axs = self._get_suplblots(figsize)
 
         for ax, (g, bars) in zip(axs, df.groupby(level=0)):
             bars.droplevel(0).plot(
                 kind="barh",
@@ -307,33 +316,338 @@
             r"$95\%\ {\rm Confidence\ Level\ Bounds}\ (1/{\rm TeV}^2)$", fontsize=20
         )
         axs[0].legend(loc=legend_loc, frameon=False, prop={"size": 13})
         plt.tight_layout()
         plt.savefig(f"{self.report_folder}/coefficient_bar.pdf", dpi=500)
         plt.savefig(f"{self.report_folder}/coefficient_bar.png")
 
+    def plot_pull(
+        self,
+        pull,
+        x_min=-3,
+        x_max=3,
+        figsize=(10, 15),
+        legend_loc="best",
+    ):
+        """
+        Plot error bars at given confidence level
+
+        Parameters
+        ----------
+            pull: dict
+                Fit residuals per fit and coefficient
+            x_min: float, optional
+                Minimum sigma to display, -3 by default
+            x_max: float, optional
+                Maximum sigma to display, +3 by default
+            figsize: list, optional
+                Figure size, (10, 15) by default
+            legend_loc: string, optional
+                Legend location, "best" by default
+        """
+
+        df = pd.DataFrame(pull)
+        groups, axs = self._get_suplblots(figsize)
+
+        for ax, (g, bars) in zip(axs, df.groupby(level=0)):
+            bars.droplevel(0).plot(
+                kind="barh",
+                width=0.6,
+                ax=ax,
+                legend=None,
+                xlim=(x_min, x_max),
+                fontsize=13,
+            )
+            ax.set_title(f"\\rm {g}", x=0.95, y=1.0)
+            ax.grid(True, which="both", ls="dashed", axis="x", lw=0.5)
+
+        self._plot_logo(axs[-1])
+        axs[-1].set_xlabel(r"${\rm Fit\:Residual\:}(\sigma)$", fontsize=20)
+        axs[0].legend(loc=legend_loc, frameon=False, prop={"size": 13})
+        plt.tight_layout()
+        plt.savefig(f"{self.report_folder}/coefficient_pull.pdf", dpi=500)
+        plt.savefig(f"{self.report_folder}/coefficient_pull.png")
+
+    def plot_spider(
+        self,
+        error,
+        labels,
+        title,
+        marker_styles,
+        ncol,
+        ymax=100,
+        log_scale=True,
+        fontsize=12,
+        figsize=(9, 9),
+        legend_loc="best",
+        radial_lines=None,
+        class_order=None,
+    ):
+        """
+        Creates a spider plot that displays the ratio of uncertainties to a baseline fit,
+         which is taken as the first fit specified in the report runcard
+
+        Parameters
+        ----------
+            error: dict
+               confidence level bounds per fit and coefficient
+            labels: list
+                Fit labels, taken from the report runcard
+            title: string
+                Plot title
+            marker_styles: list, optional
+                Marker styles per fit
+            ncol: int, optional
+                Number of columns in the legend. Uses a single row by default.
+            ymax: float, optional
+                Radius in percentage
+            log_scale: bool, optional
+                Use a logarithmic radial scale, true by default
+            fontsize: int, optional
+                Font size
+            figsize: list, optional
+                Figure size, (9, 9) by default
+            legend_loc: string, optional
+                Location of the legend, "best" by default
+            radial_lines: list, optional
+                Location of radial lines in percentage
+            class_order: list, optional
+                Order of operator classes, starting at 12'o clock anticlockwise
+
+        """
+
+        def log_transform(x, delta_shift):
+            """
+            Log transform plus possible shift to map to semi-positive value
+
+            Parameters
+            ----------
+            x: array_like
+            delta_shift: float
+
+            Returns
+            -------
+            Log transformed data
+            """
+            return np.log10(x) + delta_shift
+
+        df = pd.DataFrame(error)
+
+        if radial_lines is None:
+            radial_lines = [1, 5, 10, 20, 40, 60, 80]
+        if class_order is None:
+            class_order = df.index.get_level_values(0).unique()
+
+        # check if more than one fit is loaded
+        if df.shape[1] < 2:
+            print("At least two fits are required for the spider plot")
+            return
+
+        theta = radar_factory(len(df), frame="circle")
+
+        # normalise to first fit
+        ratio = df.iloc[:, 1:].values / df.iloc[:, 0].values.reshape(-1, 1) * 100
+        delta = np.abs(np.log10(min(ratio.flatten())))
+
+        if log_scale:
+            # in case the ratio < 1 %, its log transform is negative, so we add the absolute minimum
+            data = log_transform(ratio, delta)
+        else:
+            data = ratio
+
+        spoke_labels = df.index.get_level_values(1)
+
+        fig = plt.figure(figsize=figsize)
+
+        # margin settings
+        outer_ax_width = 0.8
+        left_outer_ax = (1 - outer_ax_width) / 2
+        rect = [left_outer_ax, left_outer_ax, outer_ax_width, outer_ax_width]
+
+        n_axis = 3  # number of spines with radial labels
+        axes = [fig.add_axes(rect, projection="radar") for i in range(n_axis)]
+
+        perc_labels = [rf"$\mathbf{{{(perc / 100):.3g}}}$" for perc in radial_lines]
+        if log_scale:
+            radial_lines = log_transform(radial_lines, delta)
+
+        # take first axis as main, the rest only serve to show the remaining percentage axes
+        ax = axes[0]
+
+        # zero degrees is 12 o'clock
+        start_angle = (
+            theta[np.argwhere(theta > 2 * np.pi - np.pi / 3).flatten()[0]] * 180 / np.pi
+        )
+
+        angles = np.arange(start_angle, start_angle + 360, 360.0 / n_axis)
+
+        prop_cycle = plt.rcParams["axes.prop_cycle"]
+        colors = prop_cycle.by_key()["color"]
+
+        if marker_styles is None:
+            marker_styles = list(markers.MarkerStyle.markers.keys())
+        marker_styles = itertools.cycle(marker_styles)
+
+        # add the ratios to the spider plot
+        for i, data_fit_i in enumerate(data.T):
+            ax.plot(theta, data_fit_i, color=colors[i], zorder=1)
+            ax.scatter(
+                theta,
+                data_fit_i,
+                marker=next(marker_styles),
+                s=50,
+                color=colors[i],
+                zorder=1,
+            )
+            ax.fill(
+                theta,
+                data_fit_i,
+                alpha=0.25,
+                label="_nolegend_",
+                color=colors[i],
+                zorder=1,
+            )
+
+        for i, axis in enumerate(axes):
+            if i > 0:
+                axis.patch.set_visible(False)
+                axis.xaxis.set_visible(False)
+
+            angle = angles[i]
+            text_alignment = "right" if angle % 360 > 180 else "left"
+
+            axis.yaxis.set_tick_params(labelsize=11, zorder=100)
+
+            if i == 0:
+                axis.set_rgrids(
+                    radial_lines,
+                    angle=angle,
+                    labels=perc_labels,
+                    horizontalalignment=text_alignment,
+                    zorder=0,
+                )
+            else:
+                axis.set_rgrids(
+                    radial_lines[1:],
+                    angle=angle,
+                    labels=perc_labels[1:],
+                    horizontalalignment=text_alignment,
+                    zorder=0,
+                )
+
+            if log_scale:
+                axis.set_ylim(0, log_transform(ymax, delta))
+            else:
+                axis.set_ylim(0, ymax)
+
+        ax.set_varlabels(spoke_labels, fontsize=fontsize)
+        ax.tick_params(axis="x", pad=17)
+
+        ax2 = fig.add_axes(rect=[0, 0, 1, 1])
+        width_disk = 0.055
+        ax2.patch.set_visible(False)
+        ax2.grid("off")
+        ax2.xaxis.set_visible(False)
+        ax2.yaxis.set_visible(False)
+        delta_disk = 0.3
+        radius = outer_ax_width / 2 + (1 + delta_disk) * width_disk
+
+        if title is not None:
+            ax2.set_title(title, fontsize=18)
+
+        # add coloured arcs along circle
+        angle_sweep = [
+            sum(op_type in index for index in self.coeff_info.index)
+            / len(self.coeff_info)
+            for op_type in class_order
+        ]
+
+        # determine angles of the colored arcs
+        prop_cycle = plt.rcParams["axes.prop_cycle"]
+        colors = prop_cycle.by_key()["color"]
+
+        filled_start_angle = 90 - 180 / len(self.coeff_info)
+
+        for i, op_type in enumerate(class_order):
+
+            filled_end_angle = (
+                angle_sweep[i] * 360 + filled_start_angle
+            )  # End angle in degrees
+            center = (0.5, 0.5)  # Coordinates relative to the figure
+
+            alpha = 0.3
+
+            ax2.axis("off")
+
+            # Create the filled portion of the circular patch
+            filled_wedge = patches.Wedge(
+                center,
+                radius,
+                filled_start_angle,
+                filled_end_angle,
+                facecolor=colors[i],
+                alpha=alpha,
+                ec=None,
+                width=width_disk,
+                transform=ax2.transAxes,
+            )
+            ax2.add_patch(filled_wedge)
+
+            filled_start_angle += angle_sweep[i] * 360
+
+        handles = [
+            plt.Line2D(
+                [0],
+                [0],
+                color=colors[i],
+                linewidth=3,
+                marker=next(marker_styles),
+                markersize=10,
+            )
+            for i in range(len(labels[1:]))
+        ]
+
+        ax2.legend(
+            handles,
+            labels[1:],
+            frameon=False,
+            fontsize=15,
+            loc=legend_loc,
+            ncol=ncol,
+            bbox_to_anchor=(0.0, -0.05, 1.0, 0.05),
+            bbox_transform=fig.transFigure,
+        )
+
+        self._plot_logo(ax2, [0.75, 0.95, 0.001, 0.07])
+
+        plt.savefig(
+            f"{self.report_folder}/spider_plot.pdf", dpi=500, bbox_inches="tight"
+        )
+        plt.savefig(f"{self.report_folder}/spider_plot.png", bbox_inches="tight")
+
     def plot_posteriors(self, posteriors, labels, disjointed_lists=None):
         """Plot posteriors histograms.
 
         Parameters
         ----------
             posteriors : list
                 posterior distributions per fit and coefficient
             labels : list
                 list of fit names
             disjointed_list: list, optional
                 list of coefficients with double solutions per fit
         """
         colors = plt.rcParams["axes.prop_cycle"].by_key()["color"]
         grid_size = int(np.sqrt(self.npar)) + 1
-        fig = plt.figure(figsize=(grid_size * 4, grid_size * 3))
+        fig = plt.figure(figsize=(grid_size * 4, grid_size * 4))
         # loop on coefficients
+        cnt = 0
         for idx, ((_, l), latex_name) in enumerate(self.coeff_info.items()):
             try:
-                ax = plt.subplot(grid_size - 1, grid_size, idx + 1)
+                ax = plt.subplot(grid_size, grid_size, idx + 1)
             except ValueError:
                 ax = plt.subplot(grid_size, grid_size, idx + 1)
             # loop on fits
             for clr_idx, posterior in enumerate(posteriors):
                 if l not in posterior:
                     continue
                 solution = posterior[l]
@@ -364,91 +678,159 @@
                     0.85,
                     latex_name,
                     transform=ax.transAxes,
                     fontsize=25,
                 )
                 ax.tick_params(which="both", direction="in", labelsize=22.5)
                 ax.tick_params(labelleft=False)
+            cnt += 1
 
         lines, labels = fig.axes[0].get_legend_handles_labels()
         for axes in fig.axes:
             if len(axes.get_legend_handles_labels()[0]) > len(lines):
                 lines, labels = axes.get_legend_handles_labels()
+
         fig.legend(
-            lines, labels, loc="lower center", prop={"size": 35}, ncol=len(posteriors)
+            lines,
+            labels,
+            ncol=len(posteriors),
+            prop={"size": 25 * (grid_size * 4) / 20},
+            bbox_to_anchor=(0.5, 1.0),
+            loc="upper center",
+            frameon=False,
         )
-        plt.tight_layout()
+
+        ax_logo_nr = int(np.ceil(cnt / grid_size)) * grid_size
+        ax_logo = plt.subplot(grid_size, grid_size, ax_logo_nr)
+
+        plt.axis("off")
+        self._plot_logo(ax_logo, [0, 1, 0.001, 0.4])
+
+        fig.tight_layout(
+            rect=[0, 0.05 * (5.0 / grid_size), 1, 1 - 0.08 * (5.0 / grid_size)]
+        )
+
         plt.savefig(f"{self.report_folder}/coefficient_histo.pdf")
         plt.savefig(f"{self.report_folder}/coefficient_histo.png")
 
-    def plot_contours_2d(self, posteriors, labels, confidence_level=95, dofs_show=None):
+    def plot_contours_2d(
+        self,
+        posteriors,
+        labels,
+        confidence_level=95,
+        dofs_show=None,
+        double_solution=None,
+    ):
         """Plots 2D marginalised projections confidence level contours
 
         Parameters
         ----------
         posteriors : list
             posterior distributions per fit and coefficient
         labels : list
             list of fit names
         dofs_show: list, optional
             List of coefficients to include in the cornerplot, set to ``None`` by default, i.e. all fitted coefficients
             are included.
+        double_solution: dict, optional
+            Dictionary of operators with double (disjoint) solution per fit
         """
 
+        if double_solution is None:
+            double_solution = {"fit1": [], "fit2": []}
+
         if dofs_show is not None:
             posteriors = [
                 (posterior[0][dofs_show], posterior[1]) for posterior in posteriors
             ]
             coeff = dofs_show
             n_par = len(dofs_show)
         else:
             coeff = self.coeff_info.index.levels[1]
             n_par = self.npar
 
-        n_cols = n_par - 1 if n_par != 2 else 2
+        n_cols = n_par - 1
         n_rows = n_cols
-
-        fig = plt.figure(figsize=(n_cols * 4, n_rows * 4))
-        grid = plt.GridSpec(n_rows, n_cols, hspace=0.1, wspace=0.1)
+        if n_par > 2:
+            fig = plt.figure(figsize=(n_cols * 4, n_rows * 4))
+            grid = plt.GridSpec(n_rows, n_cols, hspace=0.1, wspace=0.1)
+        else:
+            fig = plt.figure(figsize=(8, 8))
+            grid = plt.GridSpec(1, 1, hspace=0.1, wspace=0.1)
 
         c1_old = coeff[0]
 
         row_idx = -1
         col_idx = -1
         j = 1
 
         # loop over coefficient pairs
-        for (c1, c2) in itertools.combinations(coeff, 2):
-
+        for c1, c2 in itertools.combinations(coeff, 2):
             if c1 != c1_old:
                 row_idx += -1
                 col_idx = -1 - j
                 j += 1
                 c1_old = c1
-
-            ax = fig.add_subplot(grid[row_idx, col_idx])
+            if n_par > 2:
+                ax = fig.add_subplot(grid[row_idx, col_idx])
+            else:
+                ax = fig.add_subplot(grid[0, 0])
 
             # loop over fits
             hndls_all = []
+            fit_number = -1
             for clr_idx, (posterior, kde) in enumerate(posteriors):
+                fit_number = fit_number + 1
+
+                # case when confidence levels = [cl1, cl2]
+                if isinstance(confidence_level, list):
+                    colors = plt.rcParams["axes.prop_cycle"].by_key()["color"]
+                    # plot the first one dashed
+                    if kde:
+                        sns.kdeplot(
+                            x=posterior[c2].values,
+                            y=posterior[c1].values,
+                            levels=[1 - confidence_level[0] / 100.0, 1.0],
+                            bw_adjust=1.2,
+                            ax=ax,
+                            linestyles="dashed",
+                            linewidths=2,
+                            color=colors[clr_idx],
+                            label=None,
+                        )
+                    else:
+                        confidence_ellipse(
+                            posterior[c2].values,
+                            posterior[c1].values,
+                            ax,
+                            edgecolor=colors[clr_idx],
+                            confidence_level=confidence_level[0],
+                            linestyle="dashed",
+                            linewidth=2,
+                        )
+                    cl = confidence_level[1]
+                else:
+                    cl = confidence_level
 
                 hndls_contours = plot_contours(
                     ax,
                     posterior,
                     coeff1=c1,
                     coeff2=c2,
                     ax_labels=[
                         self.coeff_info[:, c1].values[0],
                         self.coeff_info[:, c2].values[0],
                     ],
                     kde=kde,
                     clr_idx=clr_idx,
-                    confidence_level=confidence_level,
+                    confidence_level=cl,
+                    double_solution=list(double_solution.values())[clr_idx]
+                    if kde
+                    else None,
                 )
-
                 hndls_all.append(hndls_contours)
 
                 if row_idx != -1:
                     ax.set(xlabel=None)
                     ax.tick_params(
                         axis="x",  # changes apply to the x-axis
                         which="both",  # both major and minor ticks are affected
@@ -462,32 +844,39 @@
                         labelleft=False,
                     )
 
             hndls_sm_point = ax.scatter(0, 0, c="k", marker="+", s=50, zorder=10)
             hndls_all.append(hndls_sm_point)
 
             col_idx -= 1
-
-        ax = fig.add_subplot(grid[0, -1])
-        ax.axis("off")
+            ax.locator_params(axis="x", nbins=5)
+            ax.locator_params(axis="y", nbins=6)
+            ax.minorticks_on()
+            ax.grid(linestyle="dotted", linewidth=0.5)
+
+        # in case n_par > 2, put legend outside subplot
+        if n_par > 2:
+            ax = fig.add_subplot(grid[0, -1])
+            ax.axis("off")
 
         ax.legend(
             labels=labels + [r"$\mathrm{SM}$"],
             handles=hndls_all,
-            loc="upper left",
+            loc="lower left",
             frameon=False,
-            fontsize=24,
+            fontsize=20,
             handlelength=1,
             borderpad=0.5,
             handletextpad=1,
             title_fontsize=24,
         )
 
-        fig.suptitle(
-            r"$\mathrm{Marginalised}\:95\:\%\:\mathrm{C.L.\:intervals}$", fontsize=18
+        ax.set_title(
+            rf"$\mathrm{{Marginalised}}\:{cl}\:\%\:\mathrm{{C.L.\:intervals}}$",
+            fontsize=18,
         )
         grid.tight_layout(fig)
         fig.savefig(f"{self.report_folder}/contours_2d.pdf")
         fig.savefig(f"{self.report_folder}/contours_2d.png")
 
     def write_cl_table(self, bounds, round_val=3):
         """Coefficients latex table"""
```

### Comparing `smefit-0.0.1/src/smefit/analyze/contours_2d.py` & `smefit-3.0.0/src/smefit/analyze/contours_2d.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,14 +3,30 @@
 import numpy as np
 import scipy.stats
 import seaborn as sns
 from matplotlib import patches, transforms
 from matplotlib.patches import Ellipse
 
 
+def split_solution(full_solution):
+    """Split the posterior solution"""
+
+    min_val = min(full_solution)
+    max_val = max(full_solution)
+    mid = np.mean([max_val, min_val])
+
+    # solution 1 should be closer to 0
+    solution1 = full_solution[full_solution < mid]
+    solution2 = full_solution[full_solution > mid]
+    if min(abs(solution2)) < min(abs(solution1)):
+        solution1, solution2 = solution2, solution1
+
+    return solution1, solution2
+
+
 def confidence_ellipse(
     coeff1, coeff2, ax, facecolor="none", confidence_level=95, **kwargs
 ):
     """
     Draws 95% C.L. ellipse for data points `x` and `y`
 
     Parameters
@@ -77,15 +93,23 @@
 
     ellipse.set_transform(transf + ax.transData)
 
     return ax.add_patch(ellipse)
 
 
 def plot_contours(
-    ax, posterior, ax_labels, coeff1, coeff2, kde, clr_idx, confidence_level=95
+    ax,
+    posterior,
+    ax_labels,
+    coeff1,
+    coeff2,
+    kde,
+    clr_idx,
+    confidence_level=95,
+    double_solution=None,
 ):
     """
 
     Parameters
     ----------
     ax: matplotlib.axes
         Axes object to plot on
@@ -99,28 +123,38 @@
         Name of second coefficient
     kde: bool
         Performs kernel density estimate (kde) when quadratics are turned on
     clr_idx: int
         Color index that makes sure each fit gets associated a different color
     confidence_level: int, optional
         Confidence level interval, set to 95% by default
+    double_solution: dict, optional
+        Dictionary of operators with double (disjoint) solution per fit
 
     Returns
     -------
     hndls: list
         List of Patch objects
     """
 
     colors = plt.rcParams["axes.prop_cycle"].by_key()["color"]
 
     x_values = posterior[coeff2].values
     y_values = posterior[coeff1].values
 
     # perform kde for quadratic EFT fit
     if kde:
+        solution1x = solution2x = x_values
+        if coeff2 in double_solution:
+            solution1x, solution2x = split_solution(posterior[coeff2])
+
+        solution1y = solution2y = y_values
+        if coeff1 in double_solution:
+            solution1y, solution2y = split_solution(posterior[coeff1])
+
         sns.kdeplot(
             x=x_values,
             y=y_values,
             levels=[1 - confidence_level / 100.0, 1.0],
             bw_adjust=1.2,
             ax=ax,
             fill=True,
@@ -131,25 +165,39 @@
             x=x_values,
             y=y_values,
             levels=[1 - confidence_level / 100.0],
             bw_adjust=1.2,
             ax=ax,
             alpha=1,
             color=colors[clr_idx],
+            label=confidence_level,
+        )
+        ax.scatter(
+            np.mean(solution1x),
+            np.mean(solution1y),
+            c=colors[clr_idx],
+            s=50,
+            marker="o",
+        )
+        ax.scatter(
+            np.mean(solution2x),
+            np.mean(solution2y),
+            c=colors[clr_idx],
+            s=50,
+            marker="o",
         )
 
         hndls = (
             patches.Patch(ec=colors[clr_idx], fc=colors[clr_idx], fill=True, alpha=0.3),
             patches.Patch(
                 ec=colors[clr_idx], fc=colors[clr_idx], fill=False, alpha=1.0
             ),
         )
 
     else:  # draw ellipses for linear EFT fit
-
         p1 = confidence_ellipse(
             x_values,
             y_values,
             ax,
             alpha=1,
             edgecolor=colors[clr_idx],
             confidence_level=confidence_level,
```

### Comparing `smefit-0.0.1/src/smefit/analyze/correlations.py` & `smefit-3.0.0/src/smefit/analyze/correlations.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 def plot_correlations(
     posterior_df,
     latex_names,
     fig_name,
     thr_show=None,
     hide_dofs=None,
     title=None,
+    figsize=(10, 10),
 ):
     """
     Computes and displays the correlation coefficients
     between parameters in a heat map
 
     Parameters
     ----------
@@ -28,15 +29,16 @@
         path to save the plot
     thr_show: float, None
         if given shows only off diagonal entries higher than the threshold
     hide_dofs: list, None
         coefficients to hide
     title: str, None
         plot title
-
+    figsize: tuple, (10, 10)
+        Figure size
     """
     if hide_dofs is not None:
         posterior_df = posterior_df.drop(hide_dofs, axis=1)
 
     # get correlation of free parameters
     correlations = posterior_df.corr()
 
@@ -51,36 +53,38 @@
         correlations = correlations[correlations.sum() != 0]
         coeff_to_keep = correlations.index
         correlations = correlations.loc[:, coeff_to_keep]
         correlations = correlations.replace(np.nan, 0) + np.eye(correlations.shape[0])
     else:
         coeff_to_keep = correlations.index
 
-    fig = plt.figure(figsize=(10, 10))
+    fig = plt.figure(figsize=figsize)
     ax = fig.add_subplot(111)
 
     cmap = cm.get_cmap("coolwarm")
     norm = colors.BoundaryNorm(np.arange(-1, 1.1, step=0.1), cmap.N)
 
     divider = make_axes_locatable(ax)
     cax = ax.matshow(correlations.values, cmap=cmap, norm=norm)
     fig.colorbar(cax, cax=divider.append_axes("right", size="5%", pad=0.1))
 
     for i, row in enumerate(correlations.values):
         for j, cij in enumerate(row):
-            if thr_show is None or np.abs(cij) < thr_show:
+            if thr_show is None or np.abs(cij) >= thr_show:
+                ax.text(
+                    i,
+                    j,
+                    f"{cij:.1f}",
+                    va="center",
+                    ha="center",
+                    fontsize=10,
+                )
+            else:
                 continue
-            ax.text(
-                i,
-                j,
-                f"{cij:.1f}",
-                va="center",
-                ha="center",
-                fontsize=10,
-            )
+
     labels = latex_names[coeff_to_keep].values
     ticks = np.arange(labels.shape[0])
     ax.set_yticks(ticks, labels=labels, fontsize=15)
     ax.set_xticks(ticks, labels=labels, rotation=90, fontsize=15)
     ax.tick_params(which="major", top=False, bottom=False, left=False)
 
     # minor grid
```

### Comparing `smefit-0.0.1/src/smefit/analyze/fisher.py` & `smefit-3.0.0/src/smefit/analyze/fisher.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 
     def compute_linear(self):
         """Compute linear Fisher information."""
         fisher_tab = []
         cnt = 0
         for ndat in self.datasets.NdataExp:
             fisher_row = np.zeros(self.free_parameters.size)
-            idxs = slice(cnt, cnt + ndat + 1)
+            idxs = slice(cnt, cnt + ndat)
             sigma = self.new_LinearCorrections[:, idxs]
             fisher_row = np.diag(sigma @ self.datasets.InvCovMat[idxs, idxs] @ sigma.T)
             fisher_tab.append(fisher_row)
             cnt += ndat
         self.lin_fisher = pd.DataFrame(
             fisher_tab, index=self.datasets.ExpNames, columns=self.free_parameters
         )
@@ -97,15 +97,15 @@
 
         cnt = 0
         for ndat in track(
             self.datasets.NdataExp,
             description="[green]Computing quadratic Fisher information per dataset...",
         ):
             # slice the big matrices
-            idxs = slice(cnt, cnt + ndat + 1)
+            idxs = slice(cnt, cnt + ndat)
             quad_corr = diag_corr[idxs, :].T
             lin_corr = self.new_LinearCorrections[:, idxs]
             inv_corr = self.datasets.InvCovMat[idxs, idxs]
             delta = delta_th[idxs]
             A = A_all[:, idxs]
             B = B_all[:, idxs]
             D = D_all[:, idxs, idxs]
@@ -170,14 +170,15 @@
     def groupby_data(self, table, data_groups, norm, log):
         """Merge fisher per data group."""
         summary_table = pd.merge(
             data_groups.reset_index(), table, left_on="level_1", right_index=True
         )
         summary_table = summary_table.groupby("level_0").sum(numeric_only=True)
         summary_table.index.name = "data_group"
+
         return self.normalize(summary_table, norm, log)
 
     def write_grouped(self, coeff_config, data_groups, summary_only):
         """Write Fisher information tables in latex, both for grouped data and for summary.
 
         Parameters
         ----------
@@ -349,23 +350,23 @@
 
         fig = plt.figure(figsize=figsize)
         if quad_fisher_df is not None:
             ax = fig.add_subplot(121)
         else:
             ax = plt.gca()
 
-        # clolor map
+        # colour map
         cmap_full = cm.get_cmap("Blues")
         cmap = colors.LinearSegmentedColormap.from_list(
             f"trunc({{{cmap_full.name}}},{{0}},{{0.8}})",
             cmap_full(np.linspace(0, 0.8, 100)),
         )
         norm = colors.BoundaryNorm(np.arange(110, step=10), cmap.N)
 
-        # thicks
+        # ticks
         yticks = np.arange(fisher_df.shape[1])
         xticks = np.arange(fisher_df.shape[0])
         x_labels = [f"\\rm{{{name}}}".replace("_", "\\_") for name in fisher_df.index]
 
         def set_ticks(ax):
             ax.set_yticks(yticks, labels=latex_names, fontsize=15)
             ax.set_xticks(
@@ -380,44 +381,46 @@
             ax.set_yticks(yticks - 0.5, minor=True)
             ax.tick_params(which="minor", bottom=False)
             ax.grid(visible=True, which="minor", alpha=0.2)
 
         def plot_values(ax, df):
             for i, row in enumerate(df.values.T):
                 for j, elem in enumerate(row):
-                    if elem > 10:
+                    if elem > 0:
                         ax.text(
                             j,
                             i,
                             f"{elem:.1f}",
                             va="center",
                             ha="center",
                             fontsize=8,
                         )
 
         cax = ax.matshow(fisher_df.values.T, cmap=cmap, norm=norm)
         plot_values(ax, fisher_df)
         set_ticks(ax)
         ax.set_title(r"\rm Linear", fontsize=20, y=-0.08)
-        cax1 = make_axes_locatable(ax).append_axes("right", size="10%", pad=0.1)
+        cax1 = make_axes_locatable(ax).append_axes("right", size="5%", pad=0.5)
         colour_bar = fig.colorbar(cax, cax=cax1)
 
         if quad_fisher_df is not None:
             ax = fig.add_subplot(122)
             cax = ax.matshow(quad_fisher_df.values.T, cmap=cmap, norm=norm)
             plot_values(ax, quad_fisher_df)
             set_ticks(ax)
             ax.set_title(r"\rm Quadratic", fontsize=20, y=-0.08)
             cax1 = make_axes_locatable(ax).append_axes("right", size="10%", pad=0.1)
             colour_bar = fig.colorbar(cax, cax=cax1)
 
+        fig.subplots_adjust(top=0.85)
+
         colour_bar.set_label(
             r"${\rm Normalized\ Value}$",
             fontsize=25,
             labelpad=30,
             rotation=270,
         )
-        if title is not None:
-            plt.suptitle(f"\\rm Fisher\\ information:\\ {title}", fontsize=25)
-        plt.tight_layout()
+
+        plt.suptitle(f"\\rm Fisher\\ information:\\ {title}", fontsize=25, y=0.98)
+
         plt.savefig(f"{fig_name}.pdf")
         plt.savefig(f"{fig_name}.png")
```

### Comparing `smefit-0.0.1/src/smefit/analyze/html_utils.py` & `smefit-3.0.0/src/smefit/analyze/html_utils.py`

 * *Files identical despite different names*

### Comparing `smefit-0.0.1/src/smefit/analyze/latex_tools.py` & `smefit-3.0.0/src/smefit/analyze/latex_tools.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,14 +15,15 @@
         r"\usepackage{booktabs}",
         r"\usepackage[a4paper]{geometry}",
         r"\usepackage{array}",
         r"\usepackage{hyperref}",
         r"\usepackage{xcolor}",
         r"\usepackage{multirow}",
         r"\usepackage{pdflscape}",
+        r"\usepackage{longtable}",
         r"\allowdisplaybreaks",
         r"\newcolumntype{C}[1]{>{\centering\let\newline\\\arraybackslash\hspace{0pt}}m{#1}}",
         r"\usepackage{graphicx}",
         r"\usepackage{tabularx}",
         r"\geometry{verbose, tmargin = 1.5cm, bmargin = 1.5cm, lmargin = 1cm, rmargin = 1cm}",
     ]
     return L
```

### Comparing `smefit-0.0.1/src/smefit/analyze/logo.png` & `smefit-3.0.0/src/smefit/analyze/logo.png`

 * *Files identical despite different names*

### Comparing `smefit-0.0.1/src/smefit/analyze/pca.py` & `smefit-3.0.0/src/smefit/analyze/pca.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,14 +53,15 @@
             config["use_quad"],
             config["use_theory_covmat"],
             config["use_t0"],
             config.get("use_multiplicative_prescription", False),
             config.get("theory_path", None),
             config.get("rot_to_fit_basis", None),
             config.get("uv_couplings", False),
+            config.get("external_chi2", False),
         )
 
         coefficients = CoefficientManager.from_dict(config["coefficients"])
 
         return cls(loaded_datasets, coefficients, config)
 
     def compute(self):
@@ -248,16 +249,15 @@
     def compute(self):
         """Compute PCA."""
         free_parameters = self.coefficients.free_parameters.index
 
         new_LinearCorrections = impose_constrain(self.datasets, self.coefficients)
         X = new_LinearCorrections @ self.datasets.InvCovMat @ new_LinearCorrections.T
         # Decompose matrix with SVD and identify PCs
-        X_centered = X - X.mean(axis=0)
-        _, W, Vt = np.linalg.svd(X_centered)
+        _, W, Vt = np.linalg.svd(X)
 
         pca_labels = [f"PC{i:02d}" for i in range(W.size)]
         self.pc_matrix = pd.DataFrame(Vt.T, index=free_parameters, columns=pca_labels)
         self.SVs = pd.Series(W, index=pca_labels)
 
     def write(self, fit_label, thr_show=1e-2):
         """Write PCA latex table.
```

### Comparing `smefit-0.0.1/src/smefit/analyze/report.py` & `smefit-3.0.0/src/smefit/analyze/report.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
-import pathlib
 import copy
+import pathlib
 
 import numpy as np
 import pandas as pd
 
 from ..fit_manager import FitManager
 from ..log import logging
 from .chi2_utils import Chi2tableCalculator
@@ -45,15 +45,14 @@
     report_config: dict
         dictionary with report configuration, see `/run_cards/analyze/report_runcard.yaml`
         for an example
 
     """
 
     def __init__(self, report_path, result_path, report_config):
-
         self.report = pathlib.Path(f"{report_path}/{report_config['name']}").absolute()
         self.fits = []
         # build the fits labels if needed
         if "fit_labels" not in report_config:
             fit_labels = [
                 f"${{\\rm {fit}}}$".replace("_", r"\ ")
                 for fit in report_config["result_IDs"]
@@ -151,15 +150,16 @@
 
         # here we store the info for each fit
         chi2_dict = {}
         chi2_dict_group = {}
         chi2_replica = {}
         for fit in self.fits:
             chi2_df, chi2_total_rep = chi2_cal.compute(
-                fit.datasets, fit.smeft_predictions,
+                fit.datasets,
+                fit.smeft_predictions,
             )
             chi2_replica[fit.label] = chi2_total_rep
             chi2_dict[fit.label] = chi2_cal.add_normalized_chi2(chi2_df)
             chi2_dict_group[fit.label] = chi2_cal.group_chi2_df(chi2_df)
 
         if table:
             lines = chi2_cal.write(chi2_dict, chi2_dict_group)
@@ -180,14 +180,16 @@
 
         self._append_section("Chi2", links=links_list, figs=figs_list)
 
     def coefficients(
         self,
         scatter_plot=None,
         confidence_level_bar=None,
+        pull_bar=None,
+        spider_plot=None,
         posterior_histograms=True,
         contours_2d=None,
         hide_dofs=None,
         show_only=None,
         logo=True,
         table=None,
         double_solution=None,
@@ -218,15 +220,19 @@
         figs_list = []
         coeff_config = self.coeff_info
         if show_only is not None:
             coeff_config = coeff_config.loc[:, show_only]
         if hide_dofs is not None:
             coeff_config = coeff_config.drop(hide_dofs, level=1)
 
-        coeff_plt = CoefficientsPlotter(self.report, coeff_config, logo=logo,)
+        coeff_plt = CoefficientsPlotter(
+            self.report,
+            coeff_config,
+            logo=logo,
+        )
 
         # compute confidence level bounds
         bounds_dict = {}
         for fit in self.fits:
             bounds_dict[fit.label] = compute_confidence_level(
                 fit.results,
                 coeff_plt.coeff_info,
@@ -237,15 +243,15 @@
             )
 
         if scatter_plot is not None:
             _logger.info("Plotting : Central values and Confidence Level bounds")
             coeff_plt.plot_coeffs(bounds_dict, **scatter_plot)
             figs_list.append("coefficient_central")
 
-        # when we plot the 95% CL we show 95% CL for null solutions.
+        # when we plot the 95% CL we show the 95% CL for null solutions.
         # the error coming from a degenerate solution is not taken into account.
         if confidence_level_bar is not None:
             _logger.info("Plotting : Confidence Level error bars")
             bar_cl = confidence_level_bar["confidence_level"]
             confidence_level_bar.pop("confidence_level")
             zero_sol = 0
             coeff_plt.plot_coeffs_bar(
@@ -254,14 +260,69 @@
                     + bound_df.loc[zero_sol, f"high{bar_cl}"]
                     for name, bound_df in bounds_dict.items()
                 },
                 **confidence_level_bar,
             )
             figs_list.append("coefficient_bar")
 
+        # when we plot the 95% CL we show the 95% CL for null solutions.
+        # the error coming from a degenerate solution is not taken into account.
+        if pull_bar is not None:
+            _logger.info("Plotting : Pull ")
+            zero_sol = 0
+            coeff_plt.plot_pull(
+                {
+                    name: bound_df.loc[zero_sol, "pull"]
+                    for name, bound_df in bounds_dict.items()
+                },
+                **pull_bar,
+            )
+            figs_list.append("pull_bar")
+
+        if spider_plot is not None:
+            _logger.info("Plotting : spider plot")
+
+            spider_cl = spider_plot["confidence_level"]
+            spider_plot.pop("confidence_level")
+
+            spider_bounds = {}
+            for name, bound_df in bounds_dict.items():
+                dbl_solution = bound_df.index.get_level_values(0)
+                # if dbl solution requested, add the confidence intervals, otherwise just
+                # use the sum of the hdi intervals
+                if 1 in dbl_solution:
+
+                    dbl_op = double_solution.get(fit.name, None)
+                    idx = [
+                        np.argwhere(
+                            self.coeff_info.index.get_level_values(1) == op
+                        ).flatten()[0]
+                        for op in dbl_op
+                    ]
+                    bound_df_dbl = bound_df.iloc[:, idx]
+
+                    width_0 = bound_df_dbl.loc[0, f"hdi_{spider_cl}"]
+                    width_1 = bound_df_dbl.loc[1, f"hdi_{spider_cl}"]
+                    width_tot = width_0 + width_1
+
+                    # update bound df
+                    bound_df.loc[0, f"hdi_{spider_cl}"].iloc[idx] = width_tot
+
+                    spider_bounds[name] = bound_df.loc[0, f"hdi_{spider_cl}"]
+
+                else:
+                    spider_bounds[name] = bound_df.loc[0, f"hdi_{spider_cl}"]
+
+            coeff_plt.plot_spider(
+                spider_bounds,
+                labels=[fit.label for fit in self.fits],
+                **spider_plot,
+            )
+            figs_list.append("spider_plot")
+
         if posterior_histograms:
             _logger.info("Plotting : Posterior histograms")
             disjointed_lists = [
                 double_solution.get(fit.name, None)
                 if double_solution is not None
                 else None
                 for fit in self.fits
@@ -288,51 +349,67 @@
                         fit.config["use_quad"],
                     )
                     for fit in self.fits
                 ],
                 labels=[fit.label for fit in self.fits],
                 confidence_level=contours_2d["confidence_level"],
                 dofs_show=contours_2d["dofs_show"],
+                double_solution=double_solution,
             )
             figs_list.append("contours_2d")
 
         self._append_section("Coefficients", links=links_list, figs=figs_list)
 
-    def correlations(self, hide_dofs=None, thr_show=0.1, title=True):
+    def correlations(
+        self, hide_dofs=None, thr_show=0.1, title=True, fit_list=None, figsize=(10, 10)
+    ):
         """Plot coefficients correlation matrix.
 
         Parameters
         ----------
         hide_dofs: list
             list of operator not to display.
         thr_show: float, None
             minimum threshold value to show.
             If None the full correlation matrix is displayed.
         title: bool
             if True display fit label name as title
-
+        fit_list: list, optional
+            list of fit names for which the correlation is computed.
+            By default all the fits included in the report
         """
         figs_list = []
-        for fit in self.fits:
+
+        if fit_list is not None:
+            fit_list = [fit for fit in self.fits if fit in fit_list]
+        else:
+            fit_list = self.fits
+
+        for fit in fit_list:
             _logger.info(f"Plotting correlations for: {fit.name}")
             coeff_to_keep = fit.coefficients.free_parameters.index
             plot_correlations(
                 fit.results[coeff_to_keep],
                 latex_names=self.coeff_info.droplevel(0),
                 fig_name=f"{self.report}/correlations_{fit.name}",
                 title=fit.label if title else None,
                 hide_dofs=hide_dofs,
                 thr_show=thr_show,
+                figsize=figsize,
             )
             figs_list.append(f"correlations_{fit.name}")
 
         self._append_section("Correlations", figs=figs_list)
 
     def pca(
-        self, table=True, plot=None, thr_show=1e-2, fit_list=None,
+        self,
+        table=True,
+        plot=None,
+        thr_show=1e-2,
+        fit_list=None,
     ):
         """Principal Components Analysis runner.
 
         Parameters
         ----------
         table: bool, optional
             if True writes the PC directions in a latex list
@@ -342,42 +419,50 @@
             minimum threshold value to show
         fit_list: list, optional
             list of fit names for which the PCA is computed.
             By default all the fits included in the report
         """
         figs_list, links_list = [], []
         if fit_list is not None:
-            fit_list = self.fits[self.fits == fit_list]
+            fit_list = [fit for fit in self.fits if fit in fit_list]
         else:
             fit_list = self.fits
         for fit in fit_list:
             _logger.info(f"Computing PCA for fit {fit.name}")
             pca_cal = PcaCalculator(
-                fit.datasets, fit.coefficients, self.coeff_info.droplevel(0),
+                fit.datasets,
+                fit.coefficients,
+                self.coeff_info.droplevel(0),
             )
             pca_cal.compute()
 
             if table:
                 compile_tex(
                     self.report,
                     pca_cal.write(fit.label, thr_show),
                     f"pca_table_{fit.name}",
                 )
                 links_list.append((f"pca_table_{fit.name}", f"Table {fit.label}"))
             if plot is not None:
-                fit_plot = copy.deepcopy(plot)
-                title = fit.label if fit_plot.pop("title") else None
+                title = fit.name
+
+                # TODO: check why **fit_plot got removed (see PR)
                 pca_cal.plot_heatmap(
-                    f"{self.report}/pca_heatmap_{fit.name}", title=title, **fit_plot
+                    f"{self.report}/pca_heatmap_{fit.name}", title=title
                 )
                 figs_list.append(f"pca_heatmap_{fit.name}")
         self._append_section("PCA", figs=figs_list, links=links_list)
 
     def fisher(
-        self, norm="coeff", summary_only=True, plot=None, fit_list=None, log=False,
+        self,
+        norm="coeff",
+        summary_only=True,
+        plot=None,
+        fit_list=None,
+        log=False,
     ):
         """Fisher information table and plots runner.
 
         Summary table and plots are the default
 
         Parameters
         ----------
@@ -393,15 +478,15 @@
             By default all the fits included in the report
         log: bool, optional
             if True shows the log of the Fisher informaltion
 
         """
         figs_list, links_list = [], []
         if fit_list is not None:
-            fit_list = self.fits[self.fits == fit_list]
+            fit_list = [fit for fit in self.fits if fit in fit_list]
         else:
             fit_list = self.fits
 
         for fit in fit_list:
             compute_quad = fit.config["use_quad"]
             fisher_cal = FisherCalculator(fit.coefficients, fit.datasets, compute_quad)
             fisher_cal.compute_linear()
```

### Comparing `smefit-0.0.1/src/smefit/analyze/summary.py` & `smefit-3.0.0/src/smefit/analyze/summary.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,19 +85,17 @@
                 list of the latex commands
         """
         L = latex_packages()
         L.extend(
             [
                 r"\usepackage{underscore}",
                 r"\begin{document}",
-                r"\begin{table}[H]",
-                r"\footnotesize",
-                r"\centering",
-                r"\begin{tabular}{|c|l|" + "c|" * self.nfits + "}",
+                r"\begin{longtable}{|c|l|" + "c|" * self.nfits + "}",
                 r"\hline",
+                r"\footnotesize",
             ]
         )
         temp = " Type & Datasets "
         for fit in self.fits:
             temp += f" & {fit.label}"
         temp += r" \\ \hline"
         L.append(temp)
@@ -120,15 +118,15 @@
         # temp = r"\hline & Total number of data points"
         # for fit in self.fits:
         #     temp += f" & {np.sum(fit.datasets.NdataExp)}"
         # temp += r" \\ \hline"
         # L.extend(
         #     [temp, r"\end{tabular}", r"\caption{Dataset comparison}", r"\end{table}"]
         # )
-        L.extend([r"\end{tabular}", r"\caption{Dataset comparison}", r"\end{table}"])
+        L.extend([r"\caption{Dataset comparison}", r"\end{longtable}"])
         return L
 
     def write_coefficients_table(self):
         """Write the coefficients tables
 
         Returns
         -------
```

### Comparing `smefit-0.0.1/src/smefit/basis_rotation.py` & `smefit-3.0.0/src/smefit/basis_rotation.py`

 * *Files identical despite different names*

### Comparing `smefit-0.0.1/src/smefit/chi2.py` & `smefit-3.0.0/src/smefit/chi2.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,29 +70,30 @@
     """
 
     def __init__(self, run_card, n_replica):
 
         self.n_replica = n_replica
         self.use_quad = run_card["use_quad"]
         self.result_path = f"{run_card['result_path']}/{run_card['result_ID']}"
-        self.use_multiplicative_prescription = (
-            run_card.get("use_multiplicative_prescription", False)
+        self.use_multiplicative_prescription = run_card.get(
+            "use_multiplicative_prescription", False
         )
         self.datasets = load_datasets(
             run_card["data_path"],
             run_card["datasets"],
             run_card["coefficients"],
             run_card["order"],
             run_card["use_quad"],
             run_card["use_theory_covmat"],
             False,
             self.use_multiplicative_prescription,
             run_card.get("theory_path", None),
             run_card.get("rot_to_fit_basis", None),
             run_card.get("uv_couplings", False),
+            run_card.get("external_chi2", False),
         )
 
         # set all the coefficients to 0
         self.coefficients = CoefficientManager.from_dict(run_card["coefficients"])
         self.coefficients.set_free_parameters(
             np.full(self.coefficients.free_parameters.shape[0], 0)
         )
```

### Comparing `smefit-0.0.1/src/smefit/coefficients.py` & `smefit-3.0.0/src/smefit/coefficients.py`

 * *Files identical despite different names*

### Comparing `smefit-0.0.1/src/smefit/compute_theory.py` & `smefit-3.0.0/src/smefit/compute_theory.py`

 * *Files identical despite different names*

### Comparing `smefit-0.0.1/src/smefit/covmat.py` & `smefit-3.0.0/src/smefit/covmat.py`

 * *Files identical despite different names*

### Comparing `smefit-0.0.1/src/smefit/fit_manager.py` & `smefit-3.0.0/src/smefit/fit_manager.py`

 * *Files 3% similar despite different names*

```diff
@@ -118,14 +118,15 @@
             self.config["use_quad"],
             self.config["use_theory_covmat"],
             False,  # t0 is not used here because in the report we look at the experimental chi2
             self.config.get("use_multiplicative_prescription", False),
             self.config.get("theory_path", None),
             self.config.get("rot_to_fit_basis", None),
             self.config.get("uv_couplings", False),
+            self.config.get("external_chi2", False),
         )
 
     @property
     def smeft_predictions(self):
         """Compute |SMEFT| predictions for each replica.
 
         Returns
```

### Comparing `smefit-0.0.1/src/smefit/loader.py` & `smefit-3.0.0/src/smefit/loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,16 @@
         "SMTheory",
         "OperatorsNames",
         "LinearCorrections",
         "QuadraticCorrections",
         "ExpNames",
         "NdataExp",
         "InvCovMat",
+        "ThCovMat",
+        "Luminosity",
         "Replica",
     ),
 )
 
 
 def check_file(path):
     """Check if path exists."""
@@ -104,14 +106,15 @@
         )
 
         (
             self.dataspec["central_values"],
             self.dataspec["sys_error"],
             self.dataspec["sys_error_t0"],
             self.dataspec["stat_error"],
+            self.dataspec["luminosity"],
         ) = self.load_experimental_data()
 
         if len(self.dataspec["central_values"]) != len(self.dataspec["SM_predictions"]):
             raise ValueError(
                 f"Number of experimental data points and theory predictions does not match in dataset {self.setname}."
             )
 
@@ -131,14 +134,15 @@
 
         _logger.info(f"Loading dataset : {self.setname}")
         with open(data_file, encoding="utf-8") as f:
             data_dict = yaml.safe_load(f)
 
         central_values = np.array(data_dict["data_central"])
         stat_error = np.array(data_dict["statistical_error"])
+        luminosity = data_dict.get("luminosity", None)
 
         num_sys = data_dict["num_sys"]
         num_data = data_dict["num_data"]
 
         # Load systematics from commondata file.
         # Read values of sys first
 
@@ -181,15 +185,15 @@
         df = pd.DataFrame(data=sys.T, columns=name_sys)
         df_t0 = pd.DataFrame(data=sys_t0.T, columns=name_sys)
         # limit case 1 data
         if num_data == 1:
             central_values = np.asarray([central_values])
 
         # here return both exp sys and t0 modified sys
-        return central_values, df, df_t0, stat_error
+        return central_values, df, df_t0, stat_error, luminosity
 
     def load_theory(
         self,
         operators_to_keep,
         order,
         use_quad,
         use_theory_covmat,
@@ -289,14 +293,27 @@
         -------
             n_data: int
                 number of experimental data
         """
         return self.dataspec["central_values"].size
 
     @property
+    def lumi(self):
+        """
+        Integrated luminosity of the dataset in fb^-1
+
+        Returns
+        -------
+            lumi: float
+                Integrated luminosity of the dataset in fb^-1
+
+        """
+        return self.dataspec["luminosity"]
+
+    @property
     def central_values(self):
         """
         Central values
 
         Returns
         -------
             central_values: numpy.ndarray
@@ -457,14 +474,15 @@
     use_quad,
     use_theory_covmat,
     use_t0,
     use_multiplicative_prescription,
     theory_path=None,
     rot_to_fit_basis=None,
     has_uv_couplings=False,
+    has_external_chi2=False,
 ):
     """
     Loads experimental data, theory and |SMEFT| corrections into a namedtuple
 
     Parameters
     ----------
         commondata_path : str, pathlib.Path
@@ -480,24 +498,29 @@
         use_theory_covmat: bool
             if True add the theory covariance matrix to the experimental one
         theory_path : str, pathlib.Path, optional
             path to theory folder, theory excluded.
             Default it assumes to be the same as commondata_path
         rot_to_fit_basis: dict, optional
             matrix rotation to fit basis or None
+        has_uv_couplings: bool, optional
+            True for UV fits
+        has_external_chi2: bool, optional
+            True in the presence of external chi2 modules
     """
 
     exp_data = []
     sm_theory = []
     sys_error_t0 = []
     sys_error = []
     stat_error = []
     lin_corr_list = []
     quad_corr_list = []
     n_data_exp = []
+    lumi_exp = []
     exp_name = []
     th_cov = []
 
     Loader.commondata_path = pathlib.Path(commondata_path)
     if theory_path is not None:
         Loader.theory_path = pathlib.Path(theory_path)
     else:
@@ -511,14 +534,15 @@
             use_quad,
             use_theory_covmat,
             use_multiplicative_prescription,
             rot_to_fit_basis,
         )
         exp_name.append(sset)
         n_data_exp.append(dataset.n_data)
+        lumi_exp.append(dataset.lumi)
         exp_data.extend(dataset.central_values)
         sm_theory.extend(dataset.sm_prediction)
         lin_corr_list.append([dataset.n_data, dataset.lin_corrections])
         quad_corr_list.append([dataset.n_data, dataset.quad_corrections])
         sys_error_t0.append(dataset.sys_error_t0)
         sys_error.append(dataset.sys_error)
         stat_error.append(dataset.stat_error)
@@ -526,15 +550,15 @@
 
     exp_data = np.array(exp_data)
     n_data_tot = exp_data.size
 
     sorted_keys = None
     # if uv couplings are present allow for op which are not in the
     # theory files
-    if has_uv_couplings:
+    if has_uv_couplings or has_external_chi2:
         sorted_keys = np.unique((*operators_to_keep,))
     operators_names, lin_corr_values = construct_corrections_matrix(
         lin_corr_list, n_data_tot, sorted_keys
     )
     check_missing_oparators(operators_names, operators_to_keep)
 
     if use_quad:
@@ -553,14 +577,15 @@
         quad_corr_values = None
 
     # Construct unique large cov matrix accounting for correlations between different datasets
     # The theory covariance matrix, when used, will be different from zero.
     # At the moment it does not account for correlation between different datasets
     theory_covariance = la.block_diag(*th_cov)
     exp_covmat = covmat_from_systematics(stat_error, sys_error) + theory_covariance
+
     # replicas always generated using the experimental covmat, no t0
     replica = np.random.multivariate_normal(exp_data, exp_covmat)
     if use_t0:
         fit_covmat = (
             covmat_from_systematics(stat_error, sys_error_t0) + theory_covariance
         )
     else:
@@ -572,30 +597,35 @@
         np.array(sm_theory),
         operators_names,
         lin_corr_values,
         quad_corr_values,
         np.array(exp_name),
         np.array(n_data_exp),
         np.linalg.inv(fit_covmat),
+        theory_covariance,
+        np.array(lumi_exp),
         replica,
     )
 
 
 def get_dataset(datasets, data_name):
     idx = np.where(datasets.ExpNames == data_name)[0][0]
     ndata = datasets.NdataExp[idx]
+    lumi = datasets.Luminosity[idx]
     posix_in = datasets.NdataExp[:idx].sum()
     posix_out = posix_in + ndata
 
     return DataTuple(
         datasets.Commondata[posix_in:posix_out],
         datasets.SMTheory[posix_in:posix_out],
         datasets.OperatorsNames,
         datasets.LinearCorrections[posix_in:posix_out],
         datasets.QuadraticCorrections[posix_in:posix_out]
         if datasets.QuadraticCorrections is not None
         else None,
         data_name,
         ndata,
         datasets.InvCovMat[posix_in:posix_out].T[posix_in:posix_out],
+        datasets.ThCovMat[posix_in:posix_out].T[posix_in:posix_out],
+        lumi,
         datasets.Replica[posix_in:posix_out],
     )
```

### Comparing `smefit-0.0.1/src/smefit/log.py` & `smefit-3.0.0/src/smefit/log.py`

 * *Files identical despite different names*

### Comparing `smefit-0.0.1/src/smefit/optimize/mc.py` & `smefit-3.0.0/src/smefit/optimize/mc.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 # -*- coding: utf-8 -*-
-
 """Fitting the Wilson coefficients with |MC|."""
 import time
 
 import cma
 import numpy as np
 import scipy.optimize as opt
 from rich.style import Style
@@ -23,22 +22,26 @@
 
     Parameters
     ----------
     loaded_datasets : `smefit.loader.DataTuple`
         dataset tuple
     coefficients : `smefit.coefficients.CoefficientManager`
         instance of `CoefficientManager` with all the relevant coefficients to fit
+    result_path: pathlib.Path
+        path to result folder
     use_quad : bool
         If True use also |HO| corrections
     result_ID : str
-        result ID
-    replica : int
-        replica number
+        result name
     single_parameter_fits : bool
         True for individual scan fits
+    use_multiplicative_prescription : bool
+        if True uses the multiplicative prescription for the |EFT| corrections
+    replica : int
+        replica number
     use_bounds : bool
         If true start the minimization with the specified values of min and max for each coeffient
     minimizer_specs : dict
         minimizer options. The allowed optrions are:
 
         Args:
 
@@ -66,22 +69,24 @@
         use_quad,
         result_ID,
         replica,
         single_parameter_fits,
         use_bounds,
         minimizer_specs,
         use_multiplicative_prescription,
+        external_chi2=None,
     ):
         super().__init__(
             f"{result_path}/{result_ID}",
             loaded_datasets,
             coefficients,
             use_quad,
             single_parameter_fits,
             use_multiplicative_prescription,
+            external_chi2,
         )
         self.chi2_values = []
         self.coeff_steps = []
         self.replica = replica
         self.epoch = 0
         self.use_bounds = use_bounds
         self.minimizer_specs = minimizer_specs
@@ -121,14 +126,15 @@
             config["use_quad"],
             config["use_theory_covmat"],
             config["use_t0"],
             config.get("use_multiplicative_prescription", False),
             config.get("theory_path", None),
             config.get("rot_to_fit_basis", None),
             config.get("uv_couplings", False),
+            config.get("external_chi2", False),
         )
 
         coefficients = CoefficientManager.from_dict(config["coefficients"])
 
         use_bounds = config.get("use_bounds", True)
         if not use_bounds:
             log.console.log("Running minimization without initial bounds")
@@ -156,25 +162,29 @@
         if "maxiter" not in config:
             _logger.warning("Setting maximum number of iterations (maxiter) to 1e4")
 
         single_parameter_fits = config.get("single_parameter_fits", False)
         use_multiplicative_prescription = config.get(
             "use_multiplicative_prescription", False
         )
+
+        external_chi2 = config.get("external_chi2", None)
+
         return cls(
             loaded_datasets,
             coefficients,
             config["result_path"],
             config["use_quad"],
             config["result_ID"],
             config["replica"],
             single_parameter_fits,
             use_bounds,
             minimizer_specs,
             use_multiplicative_prescription,
+            external_chi2,
         )
 
     def get_status(self, chi2):
 
         if len(self.chi2_values) == 0:
             self.chi2_values.append(chi2)
```

### Comparing `smefit-0.0.1/src/smefit/optimize/ultranest.py` & `smefit-3.0.0/src/smefit/optimize/ultranest.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,9 @@
 # -*- coding: utf-8 -*-
-
-"""
-Fitting the Wilson coefficients with |NS|
-"""
+"""Fitting the Wilson coefficients with |NS|"""
 import time
 
 import ultranest
 from rich.style import Style
 from rich.table import Table
 from ultranest import stepsampler
 
@@ -22,39 +19,49 @@
 except ModuleNotFoundError:
     run_parallel = False
 
 _logger = log.logging.getLogger(__name__)
 
 
 class USOptimizer(Optimizer):
-    """
-    Optimizer specification for Ultra nest
+    """Optimizer specification for Ultra nest.
 
     Parameters
     ----------
-        loaded_datasets : `smefit.loader.DataTuple`,
-            dataset tuple
-        coefficients : `smefit.coefficients.CoefficientManager`
-            instance of `CoefficientManager` with all the relevant coefficients to fit
-        use_quad : bool
-            If True use also |HO| corrections
-        live_points : int
-            number of |NS| live points
-        lepsilon : float
-            sampling tollerance. Terminate when live point likelihoods are all the same, within Lepsilon tolerance.
-            Increase this when your likelihood function is inaccurate,
-        target_evidence_unc: float
-            target evidence uncertainty.
-        target_post_unc: float
-            target posterior uncertainty.
-        frac_remain: float
-            integrate until this fraction of the integral is left in the remainder.
-            Set to a higher number (0.5) if you know the posterior is simple.
-        store_raw: bool
-            if True store the result to eventually resume the job
+    loaded_datasets : `smefit.loader.DataTuple`,
+        dataset tuple
+    coefficients : `smefit.coefficients.CoefficientManager`
+        instance of `CoefficientManager` with all the relevant coefficients to fit
+    result_path: pathlib.Path
+        path to result folder
+    use_quad : bool
+        If True use also |HO| corrections
+    result_ID : str
+        result name
+    single_parameter_fits : bool
+        True for single parameter fits
+    pairwise_fits : bool
+        True for pairwise parameter fits
+    use_multiplicative_prescription : bool
+        if True uses the multiplicative prescription for the |EFT| corrections
+    live_points : int
+        number of |NS| live points
+    lepsilon : float
+        sampling tollerance. Terminate when live point likelihoods are all the same, within Lepsilon tolerance.
+        Increase this when your likelihood function is inaccurate,
+    target_evidence_unc: float
+        target evidence uncertainty.
+    target_post_unc: float
+        target posterior uncertainty.
+    frac_remain: float
+        integrate until this fraction of the integral is left in the remainder.
+        Set to a higher number (0.5) if you know the posterior is simple.
+    store_raw: bool
+        if True store the result to eventually resume the job
+
     """
 
     print_rate = 5000
 
     def __init__(
         self,
         loaded_datasets,
@@ -67,62 +74,67 @@
         use_multiplicative_prescription,
         live_points=500,
         lepsilon=0.001,
         target_evidence_unc=0.5,
         target_post_unc=0.5,
         frac_remain=0.01,
         store_raw=False,
+        external_chi2=None,
     ):
         super().__init__(
             f"{result_path}/{result_ID}",
             loaded_datasets,
             coefficients,
             use_quad,
             single_parameter_fits,
             use_multiplicative_prescription,
+            external_chi2,
         )
         self.live_points = live_points
         self.lepsilon = lepsilon
         self.target_evidence_unc = target_evidence_unc
         self.target_post_unc = target_post_unc
         self.frac_remain = frac_remain
         self.npar = self.free_parameters.shape[0]
         self.result_ID = result_ID
         self.pairwise_fits = pairwise_fits
         self.store_raw = store_raw
 
     @classmethod
     def from_dict(cls, config):
-        """
-        Create object from theory dictionary.
+        """Create object from theory dictionary.
 
         Parameters
         ----------
-            config : dict
-                configuration dictionary
+        config : dict
+            configuration dictionary
 
         Returns
         -------
-            cls : Optimizer
-                created object
+        cls : Optimizer
+            created object
         """
 
-        loaded_datasets = load_datasets(
-            config["data_path"],
-            config["datasets"],
-            config["coefficients"],
-            config["order"],
-            config["use_quad"],
-            config["use_theory_covmat"],
-            config["use_t0"],
-            config.get("use_multiplicative_prescription", False),
-            config.get("theory_path", None),
-            config.get("rot_to_fit_basis", None),
-            config.get("uv_couplings", False),
-        )
+        if config.get("datasets") is not None:
+            loaded_datasets = load_datasets(
+                config["data_path"],
+                config["datasets"],
+                config["coefficients"],
+                config["order"],
+                config["use_quad"],
+                config["use_theory_covmat"],
+                config["use_t0"],
+                config.get("use_multiplicative_prescription", False),
+                config.get("theory_path", None),
+                config.get("rot_to_fit_basis", None),
+                config.get("uv_couplings", False),
+                config.get("external_chi2", False),
+            )
+        elif config.get("external_chi2") is not None:
+            loaded_datasets = None
 
         coefficients = CoefficientManager.from_dict(config["coefficients"])
 
         single_parameter_fits = config.get("single_parameter_fits", False)
         pairwise_fits = config.get("pairwise_fits", False)
         nlive = config.get("nlive", 500)
 
@@ -156,14 +168,17 @@
             )
 
         store_raw = config.get("store_raw", False)
 
         use_multiplicative_prescription = config.get(
             "use_multiplicative_prescription", False
         )
+
+        external_chi2 = config.get("external_chi2", None)
+
         return cls(
             loaded_datasets,
             coefficients,
             config["result_path"],
             config["use_quad"],
             config["result_ID"],
             single_parameter_fits,
@@ -171,66 +186,64 @@
             use_multiplicative_prescription,
             live_points=nlive,
             lepsilon=lepsilon,
             target_evidence_unc=target_evidence_unc,
             target_post_unc=target_post_unc,
             frac_remain=frac_remain,
             store_raw=store_raw,
+            external_chi2=external_chi2,
         )
 
     def chi2_func_ns(self, params):
-        """
-        Wrap the chi2 in a function for the optimizer. Pass noise and
+        """Wrap the chi2 in a function for the optimizer. Pass noise and
         data info as args. Log the chi2 value and values of the coefficients.
 
         Parameters
         ----------
-            params : np.ndarray
-                noise and data info
+        params : np.ndarray
+            noise and data info
+
         Returns
         -------
-            current_chi2 : np.ndarray
-                chi2 function
-
+        current_chi2 : np.ndarray
+            chi2 function
         """
         self.coefficients.set_free_parameters(params)
         self.coefficients.set_constraints()
 
         return self.chi2_func()
 
     def gaussian_loglikelihood(self, hypercube):
-        """
-        Multi gaussian log likelihood function
+        """Multi gaussian log likelihood function.
 
         Parameters
         ----------
-            hypercube :  np.ndarray
-                hypercube prior
+        hypercube :  np.ndarray
+            hypercube prior
 
         Returns
         -------
-            -0.5 * chi2 : np.ndarray
-                multi gaussian log likelihood
+        -0.5 * chi2 : np.ndarray
+            multi gaussian log likelihood
         """
 
         return -0.5 * self.chi2_func_ns(hypercube)
 
     def flat_prior(self, hypercube):
-        """
-        Update the prior function
+        """Update the prior function.
 
         Parameters
         ----------
-            hypercube : np.ndarray
-                hypercube prior
+        hypercube : np.ndarray
+            hypercube prior
 
         Returns
         -------
-            flat_prior : np.ndarray
-                updated hypercube prior
+        flat_prior : np.ndarray
+            updated hypercube prior
         """
         min_val = self.free_parameters.minimum.values
         max_val = self.free_parameters.maximum.values
         return hypercube * (max_val - min_val) + min_val
 
     def run_sampling(self):
         """Run the minimization with Ultra nest."""
@@ -282,30 +295,27 @@
             for par, col in zip(self.free_parameters.index, result["samples"].T):
                 table.add_row(f"{par}", f"{col.mean():.3f}", f"{col.std():.3f}")
             log.console.print(table)
 
             self.save(result)
 
     def save(self, result):
-        """
-        Save |NS| replicas to json inside a dictionary:
-        {coff: [replicas values]}
+        """Save |NS| replicas to json inside a dictionary: {coff: [replicas values]}.
 
         Parameters
         ----------
-            result : dict
-                result dictionary
+        result : dict
+            result dictionary
 
         """
         values = {}
         for c in self.coefficients.name:
             values[c] = []
 
         for sample in result["samples"]:
-
             self.coefficients.set_free_parameters(sample)
             self.coefficients.set_constraints()
 
             for c in self.coefficients.name:
                 values[c].append(self.coefficients[c].value)
 
         if self.pairwise_fits:
```

### Comparing `smefit-0.0.1/src/smefit/postfit/__init__.py` & `smefit-3.0.0/src/smefit/postfit/__init__.py`

 * *Files identical despite different names*

### Comparing `smefit-0.0.1/src/smefit/prefit/__init__.py` & `smefit-3.0.0/src/smefit/prefit/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
             config["data_path"],
             config["datasets"],
             config["coefficients"],
             config["order"],
             config["use_quad"],
             config["use_theory_covmat"],
             config["use_t0"],
-            config.get("use_multiplicative_prescription", False),
+            False,
             config.get("theory_path", None),
             config.get("rot_to_fit_basis", None),
             config.get("uv_couplings", False),
         )
 
     def chi2_sm(self):
         """Prints the SM chi2 per datapoint per dataset."""
```

### Comparing `smefit-0.0.1/PKG-INFO` & `smefit-3.0.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 Metadata-Version: 2.1
 Name: smefit
-Version: 0.0.1
+Version: 3.0.0
 Summary: Standard Model Effective Field Theory Fitter
 Home-page: https://lhcfitnikhef.github.io/smefit_release/
 License: LICENSE
 Keywords: packaging,dependency,infer,pyproject.toml
 Author: Tommaso Giani
 Author-email: tgiani@nikhef.nl
-Requires-Python: >=3.8,<=3.11.6
+Requires-Python: >=3.10,<=3.11.8
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Physics
+Requires-Dist: arviz (>=0.18.0,<0.19.0)
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: cma (>=3.2.2,<4.0.0)
 Requires-Dist: matplotlib (>=3.7.4,<4.0.0)
+Requires-Dist: mpi4py-mpich (>=3.1.5,<4.0.0)
 Requires-Dist: numpy (>=1.21.5,<2.0.0)
 Requires-Dist: pandas (>=1.4.1,<2.0.0)
 Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
 Requires-Dist: rich (>=11.2.0,<12.0.0)
 Requires-Dist: scipy (>=1.8.0,<2.0.0)
 Requires-Dist: seaborn (>=0.11.2,<0.12.0)
-Requires-Dist: ultranest (>=3.6.4,<4.0.0)
+Requires-Dist: ultranest (==3.6.4)
 Project-URL: Repository, https://github.com/LHCfitNikhef/smefit_release
 Description-Content-Type: text/markdown
 
 
 <p align="center">
   <a href="https://lhcfitnikhef.github.io/smefit_release/"><img alt="SMEFiT" src=https://github.com/LHCfitNikhef/SMEFT/blob/master/docs/sphinx/_assets/logo.png/>
 </a>
@@ -48,21 +48,14 @@
 
 To install smefit you can do:
 
 ```bash
 pip install smefit
 ```
 
-Note this installation does not allow you to run in parallel mode.
-To do that you can install from source using the provided conda environment
-or if you have an MPI compiler available just add:
-
-```bash
-pip install mpi4py
-```
 
 ## Installation from source using conda
 You can install smefit from source using a conda environnement.
 To install it you need a [conda](https://docs.conda.io/en/latest/) installation and run:
 
 ```bash
 ./install.sh -n <env_name='smefit_installation'>
```

#### html2text {}

```diff
@@ -1,35 +1,32 @@
-Metadata-Version: 2.1 Name: smefit Version: 0.0.1 Summary: Standard Model
+Metadata-Version: 2.1 Name: smefit Version: 3.0.0 Summary: Standard Model
 Effective Field Theory Fitter Home-page: https://lhcfitnikhef.github.io/
 smefit_release/ License: LICENSE Keywords:
 packaging,dependency,infer,pyproject.toml Author: Tommaso Giani Author-email:
-tgiani@nikhef.nl Requires-Python: >=3.8,<=3.11.6 Classifier: License :: Other/
+tgiani@nikhef.nl Requires-Python: >=3.10,<=3.11.8 Classifier: License :: Other/
 Proprietary License Classifier: Operating System :: Unix Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
-Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11 Classifier: Topic ::
-Scientific/Engineering Classifier: Topic :: Scientific/Engineering :: Physics
-Requires-Dist: click (>=8.1.3,<9.0.0) Requires-Dist: cma (>=3.2.2,<4.0.0)
-Requires-Dist: matplotlib (>=3.7.4,<4.0.0) Requires-Dist: numpy
-(>=1.21.5,<2.0.0) Requires-Dist: pandas (>=1.4.1,<2.0.0) Requires-Dist: pyyaml
-(>=6.0.1,<7.0.0) Requires-Dist: rich (>=11.2.0,<12.0.0) Requires-Dist: scipy
-(>=1.8.0,<2.0.0) Requires-Dist: seaborn (>=0.11.2,<0.12.0) Requires-Dist:
-ultranest (>=3.6.4,<4.0.0) Project-URL: Repository, https://github.com/
-LHCfitNikhef/smefit_release Description-Content-Type: text/markdown
+Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Language :: Python :: 3.11 Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: Scientific/Engineering :: Physics Requires-Dist: arviz
+(>=0.18.0,<0.19.0) Requires-Dist: click (>=8.1.3,<9.0.0) Requires-Dist: cma
+(>=3.2.2,<4.0.0) Requires-Dist: matplotlib (>=3.7.4,<4.0.0) Requires-Dist:
+mpi4py-mpich (>=3.1.5,<4.0.0) Requires-Dist: numpy (>=1.21.5,<2.0.0) Requires-
+Dist: pandas (>=1.4.1,<2.0.0) Requires-Dist: pyyaml (>=6.0.1,<7.0.0) Requires-
+Dist: rich (>=11.2.0,<12.0.0) Requires-Dist: scipy (>=1.8.0,<2.0.0) Requires-
+Dist: seaborn (>=0.11.2,<0.12.0) Requires-Dist: ultranest (==3.6.4) Project-
+URL: Repository, https://github.com/LHCfitNikhef/smefit_release Description-
+Content-Type: text/markdown
                                    _[_S_M_E_F_i_T_]
  _[_T_e_s_t_s_]_[_h_t_t_p_s_:_/_/_c_o_d_e_c_o_v_._i_o_/_g_h_/_L_H_C_f_i_t_N_i_k_h_e_f_/_s_m_e_f_i_t___r_e_l_e_a_s_e_/_b_r_a_n_c_h_/_m_a_i_n_/_g_r_a_p_h_/
                     _b_a_d_g_e_._s_v_g_?_t_o_k_e_n_=_M_R_T_E_X_U_P_8_X_U_]_[_C_o_d_e_F_a_c_t_o_r_]
 [SMEFiT](https://lhcfitnikhef.github.io/smefit_release/index.html) is a python
 program for Standard Model Effective Field Theory fits ## Installation To
-install smefit you can do: ```bash pip install smefit ``` Note this
-installation does not allow you to run in parallel mode. To do that you can
-install from source using the provided conda environment or if you have an MPI
-compiler available just add: ```bash pip install mpi4py ``` ## Installation
-from source using conda You can install smefit from source using a conda
+install smefit you can do: ```bash pip install smefit ``` ## Installation from
+source using conda You can install smefit from source using a conda
 environnement. To install it you need a [conda](https://docs.conda.io/en/
 latest/) installation and run: ```bash ./install.sh -n
 'smefit_installation'> ``` The installed package will be available in an
 environnement called `smefit_installation`, to activate it you can do: ```bash
 conda activate
 'smefit_installation'> smefit -h ``` ## Running The fitting code provide two
 equivalent fitting strategies. To run the code with `Nested Sampling` you can
```


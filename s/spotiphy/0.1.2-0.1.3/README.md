# Comparing `tmp/spotiphy-0.1.2.tar.gz` & `tmp/spotiphy-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spotiphy-0.1.2.tar", last modified: Mon Dec  4 01:29:11 2023, max compression
+gzip compressed data, was "spotiphy-0.1.3.tar", last modified: Wed Apr 24 02:07:39 2024, max compression
```

## Comparing `spotiphy-0.1.2.tar` & `spotiphy-0.1.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-12-04 01:29:11.410245 spotiphy-0.1.2/
--rw-rw-rw-   0        0        0    11558 2023-11-24 15:44:08.000000 spotiphy-0.1.2/LICENSE
--rw-rw-rw-   0        0        0    16359 2023-12-04 01:29:11.408245 spotiphy-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     2064 2023-12-04 01:20:25.000000 spotiphy-0.1.2/README.md
--rw-rw-rw-   0        0        0     1055 2023-12-04 01:20:25.000000 spotiphy-0.1.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-12-04 01:29:11.410245 spotiphy-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      887 2023-12-04 01:20:25.000000 spotiphy-0.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-12-04 01:29:11.373244 spotiphy-0.1.2/spotiphy/
--rw-rw-rw-   0        0        0      348 2023-09-13 02:41:57.000000 spotiphy-0.1.2/spotiphy/__init__.py
--rw-rw-rw-   0        0        0    42214 2023-12-04 01:02:32.000000 spotiphy-0.1.2/spotiphy/deconvolution.py
--rw-rw-rw-   0        0        0     9951 2023-12-04 01:18:25.000000 spotiphy-0.1.2/spotiphy/plot.py
--rw-rw-rw-   0        0        0    17873 2023-10-10 02:53:40.000000 spotiphy-0.1.2/spotiphy/sc_reference.py
--rw-rw-rw-   0        0        0    13501 2023-12-03 22:43:03.000000 spotiphy-0.1.2/spotiphy/segmentation.py
-drwxrwxrwx   0        0        0        0 2023-12-04 01:29:11.406244 spotiphy-0.1.2/spotiphy.egg-info/
--rw-rw-rw-   0        0        0    16359 2023-12-04 01:29:11.000000 spotiphy-0.1.2/spotiphy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      314 2023-12-04 01:29:11.000000 spotiphy-0.1.2/spotiphy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-12-04 01:29:11.000000 spotiphy-0.1.2/spotiphy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      224 2023-12-04 01:29:11.000000 spotiphy-0.1.2/spotiphy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-12-04 01:29:11.000000 spotiphy-0.1.2/spotiphy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-24 02:07:39.651826 spotiphy-0.1.3/
+-rw-rw-rw-   0        0        0    11558 2023-11-24 15:44:08.000000 spotiphy-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0    18496 2024-04-24 02:07:39.650826 spotiphy-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4203 2024-01-23 21:52:26.000000 spotiphy-0.1.3/README.md
+-rw-rw-rw-   0        0        0     1055 2024-04-24 02:01:21.000000 spotiphy-0.1.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-24 02:07:39.652826 spotiphy-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      887 2023-12-04 01:20:25.000000 spotiphy-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-24 02:07:39.616827 spotiphy-0.1.3/spotiphy/
+-rw-rw-rw-   0        0        0      348 2023-09-13 02:41:57.000000 spotiphy-0.1.3/spotiphy/__init__.py
+-rw-rw-rw-   0        0        0    42162 2024-01-11 00:41:37.000000 spotiphy-0.1.3/spotiphy/deconvolution.py
+-rw-rw-rw-   0        0        0    10730 2024-01-13 04:43:14.000000 spotiphy-0.1.3/spotiphy/plot.py
+-rw-rw-rw-   0        0        0    10221 2024-03-28 20:43:32.000000 spotiphy-0.1.3/spotiphy/sc_reference.py
+-rw-rw-rw-   0        0        0    13725 2024-04-24 01:59:40.000000 spotiphy-0.1.3/spotiphy/segmentation.py
+drwxrwxrwx   0        0        0        0 2024-04-24 02:07:39.648826 spotiphy-0.1.3/spotiphy.egg-info/
+-rw-rw-rw-   0        0        0    18496 2024-04-24 02:07:39.000000 spotiphy-0.1.3/spotiphy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      314 2024-04-24 02:07:39.000000 spotiphy-0.1.3/spotiphy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 02:07:39.000000 spotiphy-0.1.3/spotiphy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      224 2024-04-24 02:07:39.000000 spotiphy-0.1.3/spotiphy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-24 02:07:39.000000 spotiphy-0.1.3/spotiphy.egg-info/top_level.txt
```

### Comparing `spotiphy-0.1.2/LICENSE` & `spotiphy-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `spotiphy-0.1.2/PKG-INFO` & `spotiphy-0.1.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spotiphy
-Version: 0.1.2
+Version: 0.1.3
 Summary: An integrated pipeline designed to deconvolute and decompose spatial transcriptomics data, and produce pseudo single-cell resolution images.
 Home-page: https://github.com/jyyulab/Spotiphy
 Author: Ziqian Zheng
 Author-email: Ziqian Zheng <zzheng92@wisc.edu>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
@@ -227,22 +227,42 @@
 Requires-Dist: tensorflow==2.12.0
 Requires-Dist: stardist==0.8.3
 Requires-Dist: torch
 Requires-Dist: pyro-ppl==1.8.4
 Requires-Dist: opencv-python>=4.7
 Requires-Dist: jupyter
 
-# Spotiphy reveals location-specific cell subtypes through transcriptome profile at single-cell resolution
+# Spotiphy: generative modeling in single-cell spatial whole transcriptomics
 
 [![Pypi version](https://img.shields.io/pypi/v/spotiphy)](https://pypi.org/project/spotiphy/)
+[![Downloads](https://static.pepy.tech/badge/spotiphy)](https://pepy.tech/project/spotiphy)
 [![Github star](https://img.shields.io/github/stars/jyyulab/Spotiphy)](https://github.com/jyyulab/Spotiphy/stargazers)
+[![Static Badge](https://img.shields.io/badge/Document-Latest-green)](https://jyyulab.github.io/Spotiphy)
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/jyyulab/Spotiphy/blob/main/tutorials/Spotiphy_tutorial_1.ipynb)
+[![Zenodo](https://img.shields.io/badge/data_download-Zenodo?logo=Zenodo&labelColor=ffcc6d&color=b28e4c)](https://zenodo.org/records/10520022)
 
+![Spotiphy_cover](https://github.com/jyyulab/Spotiphy/blob/9a16882511aef6e0e7db9154f0d9f59a2c567c6f/figures/cover.png)
 
-## Usage and Tutorials
-Tutorials of spotiphy can be found in folder [Tutorials](https://github.com/jyyulab/Spotiphy/tree/main/tutorials).
+Spotiphy is a Python-based pipeline designed to enhance our understanding of biological tissues by integrating sequencing-based spatial transcriptomics data, scRNA-seq data, and high-resolution histological images. Employing a probabilistic model, Bayesian inference, and advanced image processing techniques, Spotiphy primarily executes three key tasks:
+- **Deconvolution**: Spotiphy estimates the abundance of each cell type in each capture area of spatial tissue.
+- **Decomposition**: Spotiphy decomposes spatial transcriptomics data to the single-cell level.
+- **Pseudo single-cell resolution image**: Spotiphy generates a pseudo single-cell resolution image to reconstruct cell neighbors.
+
+With these outputs, Spotiphy facilitates numerous downstream analyses. For more detailed information, please refer to the associated research paper.
+
+![Spotiphy_overview](https://github.com/jyyulab/Spotiphy/blob/d62e05cb677ef6177acbda660b029ee0de1e82b3/figures/Spotiphy_overview.png)
+
+## Tutorials and documents
+
+The following tutorial are available:
+
++ Deconvolution and decomposition of mouse cortex with Spotiphy [[document](https://colab.research.google.com/github/jyyulab/Spotiphy/blob/main/tutorials/Spotiphy_tutorial_1.ipynb)][[Google Colab](https://colab.research.google.com/github/jyyulab/Spotiphy/blob/main/tutorials/Spotiphy_tutorial_1.ipynb)]
+
+
+For more details, please refer to the [documents](https://jyyulab.github.io/Spotiphy).
 
 ## Installation
 
 [//]: # (### Requirements)
 [//]: # (+ Linux/UNIX/Windows system)
 [//]: # (+ Python >= 3.9)
 [//]: # (+ pytorch == 1.7.1)
@@ -259,29 +279,30 @@
 more flexibility, particularly for those who wish to utilize CUDA capabilities.
 We offer two methods for installing the Spotiphy package:
 + **Install from GitHub**: This method allows you to install the latest version directly from the source code hosted on 
 GitHub.
 ```bash
 pip install git+https://github.com/jyyulab/Spotiphy.git
 ```
-+ **Install from PyPI using `pip`**: This approach is for installing the Spotiphy package from the Python Package Index 
++ **Install from PyPI**: This approach is for installing the Spotiphy package from the Python Package Index 
 (PyPI), which is more streamlined for users who prefer standard package installations.
 ```bash
-pip install spotiphy==0.1.2
+pip install spotiphy
 ```
 
 To test the Installation, try to import Spotiphy in Python.
 ```Python
 import spotiphy
 ```
-## Documentation and API details
 
 
-## FAQ
-See https://github.com/jyyulab/Spotiphy/discussions
+## Frequently asked questions
+Answers to frequently asked questions can be found [here](https://jyyulab.github.io/Spotiphy/questions.html).
+
+Should you have any further questions, feel free to start a [discussion](https://github.com/jyyulab/Spotiphy/discussions) or reach out directly to the package authors:
++ Ziqian Zheng - [zzheng92@wisc.edu](mailto:zzheng92@wisc.edu)
++ Jiyuan Yang - [jiyuan.yang@stjude.org](mailto:jiyuan.yang@stjude.org)
 
 
 ## Cite Spotiphy:
 
-If you have questions, please contact the authors of the method:
-+ Ziqian Zheng - zzheng92@wic.edu
-+ Jiyuan Yang - jiyuan.yang@stjude.org
+Pending
```

### Comparing `spotiphy-0.1.2/README.md` & `spotiphy-0.1.3/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,35 @@
-# Spotiphy reveals location-specific cell subtypes through transcriptome profile at single-cell resolution
+# Spotiphy: generative modeling in single-cell spatial whole transcriptomics
 
 [![Pypi version](https://img.shields.io/pypi/v/spotiphy)](https://pypi.org/project/spotiphy/)
+[![Downloads](https://static.pepy.tech/badge/spotiphy)](https://pepy.tech/project/spotiphy)
 [![Github star](https://img.shields.io/github/stars/jyyulab/Spotiphy)](https://github.com/jyyulab/Spotiphy/stargazers)
+[![Static Badge](https://img.shields.io/badge/Document-Latest-green)](https://jyyulab.github.io/Spotiphy)
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/jyyulab/Spotiphy/blob/main/tutorials/Spotiphy_tutorial_1.ipynb)
+[![Zenodo](https://img.shields.io/badge/data_download-Zenodo?logo=Zenodo&labelColor=ffcc6d&color=b28e4c)](https://zenodo.org/records/10520022)
 
+![Spotiphy_cover](https://github.com/jyyulab/Spotiphy/blob/9a16882511aef6e0e7db9154f0d9f59a2c567c6f/figures/cover.png)
 
-## Usage and Tutorials
-Tutorials of spotiphy can be found in folder [Tutorials](https://github.com/jyyulab/Spotiphy/tree/main/tutorials).
+Spotiphy is a Python-based pipeline designed to enhance our understanding of biological tissues by integrating sequencing-based spatial transcriptomics data, scRNA-seq data, and high-resolution histological images. Employing a probabilistic model, Bayesian inference, and advanced image processing techniques, Spotiphy primarily executes three key tasks:
+- **Deconvolution**: Spotiphy estimates the abundance of each cell type in each capture area of spatial tissue.
+- **Decomposition**: Spotiphy decomposes spatial transcriptomics data to the single-cell level.
+- **Pseudo single-cell resolution image**: Spotiphy generates a pseudo single-cell resolution image to reconstruct cell neighbors.
+
+With these outputs, Spotiphy facilitates numerous downstream analyses. For more detailed information, please refer to the associated research paper.
+
+![Spotiphy_overview](https://github.com/jyyulab/Spotiphy/blob/d62e05cb677ef6177acbda660b029ee0de1e82b3/figures/Spotiphy_overview.png)
+
+## Tutorials and documents
+
+The following tutorial are available:
+
++ Deconvolution and decomposition of mouse cortex with Spotiphy [[document](https://colab.research.google.com/github/jyyulab/Spotiphy/blob/main/tutorials/Spotiphy_tutorial_1.ipynb)][[Google Colab](https://colab.research.google.com/github/jyyulab/Spotiphy/blob/main/tutorials/Spotiphy_tutorial_1.ipynb)]
+
+
+For more details, please refer to the [documents](https://jyyulab.github.io/Spotiphy).
 
 ## Installation
 
 [//]: # (### Requirements)
 [//]: # (+ Linux/UNIX/Windows system)
 [//]: # (+ Python >= 3.9)
 [//]: # (+ pytorch == 1.7.1)
@@ -26,29 +46,30 @@
 more flexibility, particularly for those who wish to utilize CUDA capabilities.
 We offer two methods for installing the Spotiphy package:
 + **Install from GitHub**: This method allows you to install the latest version directly from the source code hosted on 
 GitHub.
 ```bash
 pip install git+https://github.com/jyyulab/Spotiphy.git
 ```
-+ **Install from PyPI using `pip`**: This approach is for installing the Spotiphy package from the Python Package Index 
++ **Install from PyPI**: This approach is for installing the Spotiphy package from the Python Package Index 
 (PyPI), which is more streamlined for users who prefer standard package installations.
 ```bash
-pip install spotiphy==0.1.2
+pip install spotiphy
 ```
 
 To test the Installation, try to import Spotiphy in Python.
 ```Python
 import spotiphy
 ```
-## Documentation and API details
 
 
-## FAQ
-See https://github.com/jyyulab/Spotiphy/discussions
+## Frequently asked questions
+Answers to frequently asked questions can be found [here](https://jyyulab.github.io/Spotiphy/questions.html).
+
+Should you have any further questions, feel free to start a [discussion](https://github.com/jyyulab/Spotiphy/discussions) or reach out directly to the package authors:
++ Ziqian Zheng - [zzheng92@wisc.edu](mailto:zzheng92@wisc.edu)
++ Jiyuan Yang - [jiyuan.yang@stjude.org](mailto:jiyuan.yang@stjude.org)
 
 
 ## Cite Spotiphy:
 
-If you have questions, please contact the authors of the method:
-+ Ziqian Zheng - zzheng92@wic.edu
-+ Jiyuan Yang - jiyuan.yang@stjude.org
+Pending
```

### Comparing `spotiphy-0.1.2/pyproject.toml` & `spotiphy-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "spotiphy"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
     { name="Ziqian Zheng", email="zzheng92@wisc.edu" },
 ]
 description = "An integrated pipeline designed to deconvolute and decompose spatial transcriptomics data, and produce pseudo single-cell resolution images."
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.9"
```

### Comparing `spotiphy-0.1.2/setup.py` & `spotiphy-0.1.3/setup.py`

 * *Files identical despite different names*

### Comparing `spotiphy-0.1.2/spotiphy/deconvolution.py` & `spotiphy-0.1.3/spotiphy/deconvolution.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import anndata
 import os
-# import matplotlib as mpl
 import cv2 as cv
 import matplotlib.pyplot as plt
 from matplotlib.ticker import MaxNLocator
 import pandas as pd
 import seaborn as sns
 import numpy as np
 import torch
@@ -14,30 +13,29 @@
 import pyro.distributions.constraints as constraints
 from pyro.optim import Adam
 from pyro.infer import SVI, Trace_ELBO
 from scipy.spatial.distance import jensenshannon
 import time
 from sklearn.gaussian_process import GaussianProcessRegressor
 from sklearn.gaussian_process.kernels import RBF, ConstantKernel as C
-from . import sc_reference
+from spotiphy import sc_reference
 
 
 def deconvolute(X, sc_ref, device='cuda', n_epoch=8000, adam_params=None, batch_prior=2,
                 plot=False, fig_size=(4.8, 3.6), dpi=200):
-    """
-    Deconvolution of the proportion of genes contributed by each cell type.
+    """Deconvolution of the proportion of genes contributed by each cell type.
 
     Args:
         X: Spatial transcriptomics data. n_spot*n_gene.
         sc_ref: Single cell reference. n_type*n_gene.
         device: The device used for the deconvolution.
         plot: Whether to plot the ELBO loss.
         n_epoch: Number of training epochs.
         adam_params: Parameters for the adam optimizer.
-        batch_prior: Parameter of the prior Dirichlet distribution of the batch effect: 2^(Uniform(0, batch_prior))
+        batch_prior: Parameter of the prior distribution of the batch effect: 2^(Uniform(0, batch_prior))
         fig_size: Size of the figure.
         dpi: Dots per inch (DPI) of the figure.
 
     Returns:
         Parameters in the generative model.
     """
     if adam_params is None:
@@ -110,15 +108,15 @@
 def estimation_proportion(X, adata_sc, sc_ref, type_list, key_type, device='cuda', n_epoch=8000, adam_params=None,
                           batch_prior=2, plot=False, fig_size=(4.8, 3.6), dpi=200):
     """
     Estimate the proportion of each cell type in each spot.
 
     Args:
         X: Spatial transcriptomics data. n_spot*n_gene.
-        adata_sc: scRNA data (Anndata).
+        adata_sc (anndata.Anndata): scRNA data.
         sc_ref: Single cell reference. n_type*n_gene.
         type_list: List of the cell types.
         key_type: Column name of the cell types in adata_sc.
         device: The device used for the deconvolution.
         plot: Whether to plot the ELBO loss.
         n_epoch: Number of training epochs.
         adam_params: Parameters for the adam optimizer.
@@ -137,28 +135,30 @@
                          for i in range(len(type_list))])
     cell_proportion = sigma/mean_exp
     cell_proportion = cell_proportion/np.sum(cell_proportion, axis=1)[:, np.newaxis]
     return cell_proportion
 
 
 def plot_proportion(img, proportion, spot_location, radius, cmap_name='viridis', alpha=0.4, save_path='proportion.png',
-                    vmax=0.98, spot_scale=1.3, show_figure=False):
+                    vmax=0.98, spot_scale=1.3, show_figure=False, int_ticks=False, bar_location=(5800, 8100)):
     """
     Plot the proportion of a cell type.
 
     Args:
         img: 3 channel img with integer values in [0, 255]
         proportion: Proportion of a cell type.
         spot_location: Location of the spots.
         radius: Radius of the spot
         cmap_name: Name of the camp.
         alpha: Level of transparency of the background img.
         save_path: If not none, save the img to the path.
         vmax: Quantile of the maximum value in the color bar.
         spot_scale: Scale of the spot in the figure.
+        show_figure: Whether plot the figure.
+        int_ticks: Whether the ticks must be integers.
     """
     def render_to_array(fig):
         fig.canvas.draw()
         buf = fig.canvas.tostring_rgb()
         ncols, nrows = fig.canvas.get_width_height()
         return np.frombuffer(buf, dtype=np.uint8).reshape(nrows, ncols, 3)
 
@@ -177,23 +177,25 @@
 
     fig = plt.figure(figsize=(1, 2.5), dpi=1200)
     cbar_ax = fig.add_axes([0, 0.1, 0.25, 0.85])
     if vmax >= 0.2:
         a = int(vmax*10)/20
     else:
         a = int(vmax*100)/200
+    if int_ticks:
+        a = int(a)
     ticks=[0, a, a*2]
     cb1 = plt.colorbar(plt.cm.ScalarMappable(norm=plt.Normalize(vmin, vmax), cmap=cmap), cax=cbar_ax, ticks=ticks)
     cb1.outline.set_edgecolor("none")
     for label in cb1.ax.get_yticklabels():
         label.set_size(13)
     cbar_array = render_to_array(fig)
     plt.close(fig)
 
-    c = [5800, 8100]
+    c = [bar_location[0], bar_location[1]]
     img[c[0]:c[0]+cbar_array.shape[0], c[1]:c[1]+cbar_array.shape[1]][np.sum(cbar_array, axis=2) < 252*3] \
         = cbar_array[np.sum(cbar_array, axis=2) < 252*3]
 
     if save_path is not None:
         print('Saving the image.')
         img1 = img[:, :, [2, 1, 0]]
         cv.imwrite(save_path, img1)
@@ -227,34 +229,29 @@
         if np.sum(count) == n:
             return count
         idx = np.argsort(r)[-int(np.round(n - np.sum(count))):]
         count[idx] += 1
     return count
 
 
-def estimation_N(proportion, mean_exp_type, adata_st):
-    sum_exp_spot = np.sum(np.array(adata_st.X))
-
-
-
 def simulation(adata_st: anndata.AnnData, adata_sc: anndata.AnnData, key_type: str, cell_proportion: np.ndarray,
                n_cell=10, batch_effect_sigma=0.1, zero_proportion=0.3, additive_noise_sigma=0.05, save=True,
                out_dir='', filename="ST_Simulated.h5ad", verbose=0):
     """
     Simulation of the spatial transcriptomics data based on a real spatial sample and deconvolution results of Spotiphy.
 
     Args:
         adata_st: Original spatial transcriptomics data.
         adata_sc: Original single-cell data.
         key_type: The key that is used to extract cell type information from adata_sc.obs.
         cell_proportion: Proportion of each cell type obtained by the deconvolution.
         n_cell: Number of cells in each spot, either a key of adata_st.obs or a positive integer.
         batch_effect_sigma: Sigma of the log-normal distribution when generate batch effect.
         zero_proportion: Proportion of gene expression set to 0. Note that since some gene expression in the original
-                         X is already 0, the final proportion of 0 gene read is larger than zero_proportion.
+            X is already 0, the final proportion of 0 gene read is larger than zero_proportion.
         additive_noise_sigma: Sigma of the log-normal distribution when generate additive noise.
         save: If True, save the generated adata_st as a file.
         out_dir: Output directory.
         filename: Name of the saved file.
         verbose: Whether print the time spend.
     Returns:
         Simulated ST Anndata.
@@ -468,19 +465,20 @@
             return jensenshannon(proportion_truth, proportion_estimated, axis=0)
         else:
             raise ValueError(f"Invalid metric type {metric_type}")
 
     def evaluate_metric(self, metric='Cosine similarity', metric_type='Spot', region=None):
         """
         Evaluate the proportions based on the metric.
+
         Args:
             metric: Name of the metric.
             metric_type: How the metric is calculated. 'Spot': metric is calculated for each spot; 'Cell type',
-                         metric is calculated for each cell type; 'Individual': metric is calculated for each individual
-                         proportion estimation.
+                metric is calculated for each cell type; 'Individual': metric is calculated for each individual
+                proportion estimation.
             region: The region that is being evaluated.
         """
         assert metric in self.metric_type_dict[metric_type]
         metric_values = []
         func = self.function_map.get(metric)
         if region is None:
             select = np.array([True]*len(self.proportion_truth))
@@ -497,26 +495,27 @@
             metric_values.append(func(self.proportion_truth[select], self.proportion_estimated_list[i][select],
                                       metric_type))
         self.metric_dict[metric+' '+metric_type] = metric_values
         return metric_values
 
     def plot_metric(self, save=False, region=None, metric='Cosine similarity', metric_type='Spot', cell_types=None,
                     suffix='', show=True):
-        """
-        Plot the box plot of each method based on the metric.
+        """Plot the box plot of each method based on the metric.
+
         Box number equals to the number of methods.
+
         Args:
             save: If true, save the figure.
             region: Regions of the tissue.
             metric: Name of the metric.
             metric_type: How the metric is calculated. 'Spot': metric is calculated for each spot; 'Cell type',
-                         metric is calculated for each cell type; 'Individual': metric is calculated for each individual
-                         proportion estimation.
+                metric is calculated for each cell type; 'Individual': metric is calculated for each individual
+                proportion estimation.
             cell_types: If metric_type is 'Cell type' and cell_types is not None, then only plot the results
-                        corresponding to the cell_types.
+                corresponding to the cell_types.
             suffix: suffix of the save file.
             show: Whether to show the figure
         """
         assert metric_type == 'Spot' or metric_type == 'Cell type'
         assert metric in self.metric_type_dict[metric_type]
         if metric+' '+metric_type not in self.metric_dict.keys():
             self.evaluate_metric(metric=metric, metric_type=metric_type, region=region)
@@ -640,16 +639,15 @@
             plt.savefig(f'{self.out_dir}figures/{metric}{region_name}.tiff', dpi=800, bbox_inches='tight')
         plt.show()
 
 
 def decomposition(adata_st: anndata.AnnData, adata_sc: anndata.AnnData, key_type: str, cell_proportion: np.ndarray,
                   save=True, out_dir='', threshold=0.1, n_cell=None, spot_location: np.ndarray = None,
                   filtering_gene=False, filename="ST_decomposition.h5ad", verbose=0, use_original_proportion=False):
-    """
-    Decompose ST.
+    """Decompose ST.
 
     Args:
         adata_st: Original spatial transcriptomics data.
         adata_sc: Original single-cell data.
         key_type: The key that is used to extract cell type information from adata_sc.obs.
         cell_proportion: Proportion of each cell type obtained by the deconvolution.
         save: If True, save the generated adata_st as a file.
@@ -657,15 +655,15 @@
         threshold: If n_cell is none, discard cell types with proportion less than threshold.
         n_cell: Number of cells in each spot.
         spot_location: Coordinates of the spots.
         filtering_gene: Whether filter the genes in sc_reference.initialization.
         filename: Name of the saved file.
         verbose: Whether print the time spend.
         use_original_proportion: If the original proportion is used to estimate the iscRNA. Note that even when the
-                                 original proportion is used, we still filter some cells in iscRNA.
+            original proportion is used, we still filter some cells in iscRNA.
     Returns:
         adata_st_decomposed: Anndata similar to scRNA, but obtained by decomposing ST.
     """
     time_start = time.time()
     type_list = sorted(list(adata_sc.obs[key_type].unique()))  # list of the cell type.
     assert len(type_list) == cell_proportion.shape[1]
     assert len(cell_proportion) == len(adata_st)
@@ -761,22 +759,22 @@
         if verbose:
             print('Saved file to output folder. Time use {:.2f}'.format(time.time() - time_start))
 
     return adata_st_decomposed
 
 
 def assign_type_spot(nucleus_df, n_cell_df, cell_number, type_list):
-    """
-    Assign the cell type to the cells inside the spot.
+    """Assign the cell type to the cells inside the spot.
 
     Args:
         nucleus_df: Dataframe of the nucleus. Part of spotiphy.segmentation.Segmentation.
         n_cell_df: Dataframe of the number of cells in each spot. Part of spotiphy.segmentation.Segmentation.
         cell_number: Number of each cell type in each spot.
         type_list: List of the cell types.
+
     Returns:
         nucleus_df with assigned spot
     """
     assert len(type_list) == cell_number.shape[1]
     assert len(n_cell_df) == len(cell_number)
     cell_number = cell_number.astype(np.int32)
     if 'cell_type' not in nucleus_df.columns:
@@ -790,25 +788,25 @@
                 if n > 0:
                     nucleus_df.loc[index[j1:j1+n], 'cell_type'] = type_list[j2]
                     j1 += n
     return nucleus_df
 
 
 def assign_type_out(nucleus_df, cell_proportion, spot_centers, type_list, max_distance=100, band_width=100):
-    """
-    Assign the cell type to the cells outside the spot.
+    """Assign the cell type to the cells outside the spot.
 
     Args:
         nucleus_df: Dataframe of the nucleus. Part of spotiphy.segmentation.Segmentation.
         spot_centers: Centers of the spots.
         cell_proportion: Proportion of each cell type in each spot.
         type_list: List of the cell types.
         max_distance: If the distance between a nucleus and the closest spot is larger than max_distance, the cell type
-                      will not be assigned to this nucleus.
+            will not be assigned to this nucleus.
         band_width: Band width of the kernel.
+
     Returns:
         nucleus_df with assigned spot
     """
     assert len(type_list) == cell_proportion.shape[1]
     assert len(cell_proportion) == len(spot_centers)
     if 'cell_type' not in nucleus_df.columns:
         nucleus_df['cell_type'] = 'unknown'
@@ -828,25 +826,25 @@
             t_temp -= smooth[i, j]
             j += 1
         nucleus_df.loc[i, 'cell_type'] = type_list[j]
     return nucleus_df, smooth
 
 
 def archive_assign_type_out_gp(nucleus_df, cell_proportion, spot_centers, type_list, max_distance=100, return_gp=False):
-    """
-    Assign the cell type to the cells outside the spot.
+    """Assign the cell type to the cells outside the spot.
 
     Args:
         nucleus_df: Dataframe of the nucleus. Part of spotiphy.segmentation.Segmentation.
         spot_centers: Centers of the spots.
         cell_proportion: Proportion of each cell type in each spot.
         type_list: List of the cell types.
         max_distance: If the distance between a nucleus and the closest spot is larger than max_distance, the cell type
-                      will not be assigned to this nucleus.
+            will not be assigned to this nucleus.
         return_gp: If return the fitted GP models.
+
     Returns:
         nucleus_df with assigned spot
     """
     assert len(type_list) == cell_proportion.shape[1]
     assert len(cell_proportion) == len(spot_centers)
     if 'cell_type' not in nucleus_df.columns:
         nucleus_df['cell_type'] = 'unknown'
```

### Comparing `spotiphy-0.1.2/spotiphy/plot.py` & `spotiphy-0.1.3/spotiphy/plot.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,20 +3,21 @@
 import os
 from tqdm import tqdm
 import cv2 as cv
 import matplotlib.patches as patches
 
 
 class Plot_Visium:
-    def __init__(self, segmentation, boundary_dict, type_list):
+    def __init__(self, segmentation, boundary_dict, type_list, colors=None):
         """
         Args:
             segmentation: Object of spotiphy.segmentation.Segmentation.
             boundary_dict: Output of function spotiphy.segmentation.cell_boundary.
             type_list: List of the cell types.
+            colors: Colors of each cell type.
         """
         self.img = segmentation.img  # Original image.
         if np.max(self.img) <= 1:
             self.img = (self.img*255).astype(np.int32)
         self.img_seg = segmentation.label  # Segmented image.
         self.n_cell_df = segmentation.n_cell_df  # Dataframe shown the cells in each spot.
         self.nucleus_boundary = segmentation.nucleus_boundary.astype(np.int32)  # Segmented nucleus boundaries.
@@ -28,16 +29,19 @@
         self.img_cell = boundary_dict['img_cell'].astype(np.int32)   # Inferred cell location.
         self.type_mask = None
         self.img_boundary = boundary_dict['cell_boundary']
         self.individual_boundary = boundary_dict['individual_boundary']
         self.img_size = self.img_seg.shape[:2]
         self.type_list = type_list
 
-        self.colors = np.array(list(plt.get_cmap("tab20b").colors) + list(plt.get_cmap("tab20c").colors))
-        self.colors = (self.colors*255).astype(np.int32)
+        if colors is None:
+            self.colors = np.array(list(plt.get_cmap("tab20b").colors) + list(plt.get_cmap("tab20c").colors))
+            self.colors = (self.colors*255).astype(np.int32)
+        else:
+            self.colors = colors
         self.color_dict = {type_: list(self.colors[i]) for i, type_ in enumerate(type_list)}
 
     def plot(self, background=False, cell='both', shape='cell', circle_size=10, boundary=None,
              save='Visium_plot.png', background_alpha=0.5, spot=True, spot_width=2, spot_color=(0, 0, 255),
              cell_boundary_color=(100, 100, 100), dpi=300):
         """
         Args:
@@ -64,15 +68,16 @@
         print('Adding cells.')
         if shape == 'cell':
             d = {t: i for i, t in enumerate(self.type_list)}
             type_mask = np.zeros((img.shape[0], img.shape[1], len(self.type_list)), dtype=bool)
             for i in tqdm(range(len(self.img_cell))):
                 for j in range(len(self.img_cell[0])):
                     k = self.img_cell[i, j]
-                    if k > 0 and type_annotation[k-1] in d.keys() and in_spot[k-1] in group_dict[cell]:
+                    if (0 < k <= len(type_annotation) and type_annotation[k-1] in d.keys()
+                            and in_spot[k-1] in group_dict[cell]):
                         type_mask[i, j, d[type_annotation[k-1]]] = True
             for i, type_ in tqdm(enumerate(self.type_list)):
                 color = np.array(self.color_dict[type_]).astype(np.int32)
                 img[type_mask[:, :, i]] = color
             # img.astype(np.int32)
 
         for i, type_ in tqdm(enumerate(type_annotation)):
@@ -99,27 +104,38 @@
         if save is not None:
             print('Saving the image.')
             img1 = img[:, :, [2, 1, 0]]
             cv.imwrite(save, img1)
         plt.figure(dpi=dpi)
         plt.imshow(img)
 
-    def plot_legend(self, save=None, dpi=300):
-        img = np.zeros((len(self.type_list)*60+40, 400, 3))
+    def plot_legend(self, save=None, dpi=300, background=(0, 0, 0), ncol=1, word_color=(255, 255, 255), fontsize=6,
+                    horizontal_distance=380):
+        nrow = len(self.type_list)//ncol
+        if nrow*ncol < len(self.type_list):
+            nrow += 1
+        img = np.ones((nrow*60+40, ncol*horizontal_distance-30, 3)) * np.array(background)
+        img = img.astype(np.int32)
+
         fig, ax = plt.subplots(dpi=dpi)
         plt.imshow(img)
-        i = 0
+        i = 0  # col index
+        j = 0  # row index
+        word_color = (word_color[0]/255, word_color[1]/255, word_color[2]/255)
         for k, v in self.color_dict.items():
-            ax.add_patch(patches.Rectangle((240, i*60+20), 150, 45, facecolor=np.array(v)/255,
-                                           edgecolor='none'))
-            ax.text(20, i*60+40, k, va="center", ha="left", fontsize=5, color='white')
-            i += 1
+            ax.add_patch(patches.Rectangle((i*horizontal_distance+20, j*60+20), 100, 45,
+                                           facecolor=np.array(v)/255, edgecolor='none'))
+            ax.text(i*horizontal_distance+145, j*60+43, k, va="center", ha="left", fontsize=fontsize, color=word_color)
+            j += 1
+            if j == nrow:
+                j = 0
+                i += 1
         ax.axis('off')
         if save is not None:
-            plt.savefig(save)
+            plt.savefig(save, bbox_inches='tight', pad_inches=0)
         plt.show()
 
 
 class Plot_Xenium:
     def __init__(self, Xenium_img, cell_boundaries, nucleus_boundaries, type_list, cell_type, nucleus_centers):
         """
         Args:
```

### Comparing `spotiphy-0.1.2/spotiphy/segmentation.py` & `spotiphy-0.1.3/spotiphy/segmentation.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import pandas as pd
 import numpy as np
 import matplotlib.pyplot as plt
-from numba import cuda
 from stardist.models import StarDist2D
 from csbdeep.utils import normalize
 import tensorflow as tf
 from packaging import version
 import os
 from scipy.signal import convolve2d
 from tqdm import tqdm
@@ -13,21 +12,24 @@
 
 
 class Segmentation:
     def __init__(self, img, spot_center: np.ndarray, out_dir: str = '', prob_thresh: float = 0.2,
                  nms_thresh: float = 0.5, spot_radius: float = 36.5, n_tiles=(8, 8, 1)):
         """
         Args:
-            img: Array(_*_*3). Three channel stained image. In default, it should be hematoxylin and eosin (H&E) stained
-                 image.
+            img (numpy.ndarray):. Three channel stained image. In default, it should be hematoxylin and eosin (H&E) stained
+                image.
             spot_center: Coordinates of the center of the spots.
             out_dir: Output directory.
             Prob_thresh, nms_thresh: Two thresholds used in Stardist. User should adjust these two threshold based on
-                                    the segmentation results.
+                the segmentation results.
             spot_radius: Radius of the spots. In 10X Visium, it should be 36.5.
+            n_tiles: Out of memory (OOM) errors can occur if the input image is too large. To avoid this problem, the
+                input image is broken up into (overlapping) tiles that are processed independently and re-assembled.
+                (Copied from stardist document). In default, we break the image into 8*8 tiles.
 
         """
         self.img = img
         if spot_center is not None:
             assert spot_center.shape[1] == 2, "spot_center must have exact two columns."
         self.spot_center = np.array(spot_center)
         self.prob_thresh = prob_thresh
@@ -45,56 +47,58 @@
         if version.parse(tf.__version__) >= version.parse("2.9.0"):
             tf.keras.Model.predict = change_predict_defaults(tf.keras.Model.predict)
             print(f"Suppress the output of tensorflow prediction for tensorflow version {tf.version.VERSION}>=2.9.0.")
 
     @staticmethod
     def stardist_2D_versatile_he(img, prob_thresh: float = 0.2, nms_thresh: float = 0.5, n_tiles=(8, 8, 1),
                                  verbose: bool = True):
-        """
-        Segmentation function provided by Stardist.
+        """Segmentation function provided by Stardist.
+
         Args:
             img: Three channel image.
             nms_thresh: Parameter of non-maximum suppression.
             prob_thresh: The probability threshold that determines the retention of a nucleus.
-            n_tiles: Out of memory (OOM) errors can occur if the input image is too large.
-                     To avoid this problem, the input image is broken up into (overlapping) tiles that are processed
-                     independently and re-assembled. (Copied from stardist document).
-                     In default, we break the image into 8*8 tiles.
+            n_tiles: Out of memory (OOM) errors can occur if the input image is too large. To avoid this problem, the
+                input image is broken up into (overlapping) tiles that are processed independently and re-assembled.
+                (Copied from stardist document). In default, we break the image into 8*8 tiles.
             verbose: Whether to print segmentation progress.
+
         Returns:
-            label: 2D np.ndarray represents the segmented image. Background pixels has value 0 and nucleus pixels has
-                    the positive integer value as the index of the nucleus.
-            details: Details[0]: np.ndarray(n_nucleus*2*32). Boundaries of each nucleus.
-                     Details[1]: np.ndarray(n_nucleus*2). Center of each nucleus.
-                     Details[2]: np.ndarray(n_nucleus). Probability that a segmented nucleus is indeed a nucleus.
+            There are two returns.
+
+            np.ndarray: The segmented image. Background pixels has value 0 and nucleus pixels has
+            the positive integer value as the index of the nucleus.
+
+            list: Nucleus details. Details[0]: np.ndarray(n_nucleus*2*32). Boundaries of each nucleus. Details[1]:
+            np.ndarray(n_nucleus*2). Center of each nucleus. Details[2]: np.ndarray(n_nucleus). Probability that a
+            segmented nucleus is indeed a nucleus.
         """
         axis_norm = (0, 1, 2)  # normalize channels jointly
         img = normalize(img, 1, 99.8, axis=axis_norm)
         model = StarDist2D.from_pretrained('2D_versatile_he')
         label, details = model.predict_instances(img, nms_thresh=nms_thresh, prob_thresh=prob_thresh, n_tiles=n_tiles,
                                                  show_tile_progress=verbose)
-        device = cuda.get_current_device()
-        device.reset()
         return label, details
 
     @staticmethod
     def n_cell_in_spot(nucleus_center: np.ndarray, spot_center: np.ndarray, spot_radius: float,
                        nucleus_df: pd.DataFrame = None) -> pd.DataFrame:
-        """
-        Find the number of cells in each spot. If the center of a nucleus is inside the spot, we assume that the cell is
-        in the spot.
+        """Find the number of cells in each spot.
+
+        If the center of a nucleus is inside the spot, we assume that the cell is in the spot.
+
         Args:
             nucleus_center: np.ndarray(n_nucleus*2). Coordinates of the nucleus centers.
             spot_center: np.ndarray(n_spot*2). Coordinates of the spot centers.
             spot_radius: Radius of the spots.
             nucleus_df: Optional, dataframe of the nucleus.
+
         Returns:
-            n_cell_df: Pandas data frame with two columns.
-                       Column 'cell_count' represents the number of cells in a spot.
-                       Column 'centers' represents the coordinates of the nucleus centers.
+            Pandas data frame with two columns. Column 'cell_count' represents the number of cells in a spot.
+            Column 'centers' represents the coordinates of the nucleus centers.
         """
         n_spot = len(spot_center)
         n_cell_df = pd.DataFrame({'cell_count': [0] * n_spot, 'Nucleus centers': None, 'Nucleus indices':None})
         distance = np.sum((spot_center[:, :, np.newaxis] - nucleus_center.T) ** 2, axis=1)
         if nucleus_df is not None:
             nucleus_df['in_spot'] = False
         for i in range(n_spot):
@@ -103,16 +107,16 @@
             n_cell_df.at[i, 'Nucleus centers'] = nucleus_center[nucleus_index] if len(nucleus_index) else np.array([])
             n_cell_df.at[i, 'Nucleus indices'] = nucleus_index
             if nucleus_df is not None:
                 nucleus_df.loc[nucleus_index, 'in_spot'] = True
         return n_cell_df
 
     def segment_nucleus(self, save=True):
-        """
-        Conduct the segmentation using StarDist pretrained model.
+        """Conduct the segmentation using StarDist pretrained model.
+
         Args:
             save: Whether to save the segmentation results.
         """
         self.label, details = self.stardist_2D_versatile_he(self.img, nms_thresh=self.nms_thresh,
                                                             prob_thresh=self.prob_thresh, n_tiles=self.n_tiles)
         nucleus_boundary, nucleus_center, self.probability = details['coord'], details['points'], details['prob']
         nucleus_boundary = np.transpose(nucleus_boundary, [0, 2, 1])
@@ -121,33 +125,32 @@
         self.n_cell_df = self.n_cell_in_spot(self.nucleus_df[['x', 'y']].values, self.spot_center, self.spot_radius,
                                              self.nucleus_df)
         self.is_segmented = True
         if save:
             self.save_results()
 
     def save_results(self):
-        """
-        Save segmentation results.
+        """Save segmentation results.
         """
         assert self.is_segmented, "Please conduct segmentation first."
         np.save(f'{self.out_dir}segmentation_label.npy', self.label)
         np.save(f'{self.out_dir}segmentation_boundary.npy', self.nucleus_boundary)
         np.save(f'{self.out_dir}nucleus_df.csv', self.nucleus_df)
         np.save(f'{self.out_dir}segmentation_probability.npy', self.probability)
         self.n_cell_df.to_csv(f'{self.out_dir}n_cell_df.csv')
 
     def plot(self, fig_size=(10, 4.5), dpi=300, crop=None, cmap_segmented='hot', save=False, path=None):
-        """
-        Plot the segmentation results.
+        """Plot the segmentation results.
+
         It is recommended to adjust the stardist parameters nms_thresh and prob_thresh based on this plot.
+
         Args:
             fig_size: Size of the figure.
             dpi: Dots per inch (DPI) of the figure.
-            crop: If None, show the full image.
-                  Otherwise, crop should be
+            crop: If None, show the full image. Otherwise, crop should be
             cmap_segmented: Color map of the segmented image.
             save: If true, save the figure.
             path: Path to the save figure.
         """
         assert self.is_segmented, "Please conduct segmentation first."
         fig, ax = plt.subplots(1, 2, figsize=fig_size, dpi=dpi)
         if crop is None:
@@ -164,18 +167,20 @@
         ax[1].axis('off')
         if save:
             plt.savefig(path, bbox_inches='tight')
         plt.show()
 
 
 def change_predict_defaults(predict_function):
-    """
+    """Wrap prediction function for tensorflow>=2.9.0 to reduce outputs.
+
     Start from tensorflow 2.9.0, the default verbose value in function tensorflow.keras.Model.predict is set to 'auto',
-    which takes value 1 for the most of the time. Thus, this function is a decorator to wrap the predict function and
-    set the default verbose to 0.
+    which takes value 1 for the most of the time. Thus, this function is a decorator to wrap the predict function
+    and set the default verbose to 0.
+
     Args:
         predict_function: tensorflow.keras.Model.predict
     """
     def wrapper(instance, x, verbose=0, **kwargs):
         return predict_function(instance, x, verbose=verbose, **kwargs)
     return wrapper
 
@@ -188,16 +193,17 @@
         nucleus_location: Coordinates of the nucleus centers.
         img_size: The size of the image.
         max_dist: The largest distance from the cell boundary to the nucleus center.
         max_area: Largest area of a cell. Segmented nuclei with size larger than this value are discarded.
         search_direction: The search direction when determine the cell boundary.
         verbose: Whether to print progress.
         delta: Increment of the radius in each round.
-    Returns:
 
+    Returns:
+        Dictionary of the cell boundary information.
     """
     img_cell = np.zeros(img_size)
     n_nuclei = len(nucleus_location)
     n_pixel = [0] * n_nuclei
     nuclei_left = set(range(1, n_nuclei+1))
 
     radius = 0
```

### Comparing `spotiphy-0.1.2/spotiphy.egg-info/PKG-INFO` & `spotiphy-0.1.3/spotiphy.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spotiphy
-Version: 0.1.2
+Version: 0.1.3
 Summary: An integrated pipeline designed to deconvolute and decompose spatial transcriptomics data, and produce pseudo single-cell resolution images.
 Home-page: https://github.com/jyyulab/Spotiphy
 Author: Ziqian Zheng
 Author-email: Ziqian Zheng <zzheng92@wisc.edu>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
@@ -227,22 +227,42 @@
 Requires-Dist: tensorflow==2.12.0
 Requires-Dist: stardist==0.8.3
 Requires-Dist: torch
 Requires-Dist: pyro-ppl==1.8.4
 Requires-Dist: opencv-python>=4.7
 Requires-Dist: jupyter
 
-# Spotiphy reveals location-specific cell subtypes through transcriptome profile at single-cell resolution
+# Spotiphy: generative modeling in single-cell spatial whole transcriptomics
 
 [![Pypi version](https://img.shields.io/pypi/v/spotiphy)](https://pypi.org/project/spotiphy/)
+[![Downloads](https://static.pepy.tech/badge/spotiphy)](https://pepy.tech/project/spotiphy)
 [![Github star](https://img.shields.io/github/stars/jyyulab/Spotiphy)](https://github.com/jyyulab/Spotiphy/stargazers)
+[![Static Badge](https://img.shields.io/badge/Document-Latest-green)](https://jyyulab.github.io/Spotiphy)
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/jyyulab/Spotiphy/blob/main/tutorials/Spotiphy_tutorial_1.ipynb)
+[![Zenodo](https://img.shields.io/badge/data_download-Zenodo?logo=Zenodo&labelColor=ffcc6d&color=b28e4c)](https://zenodo.org/records/10520022)
 
+![Spotiphy_cover](https://github.com/jyyulab/Spotiphy/blob/9a16882511aef6e0e7db9154f0d9f59a2c567c6f/figures/cover.png)
 
-## Usage and Tutorials
-Tutorials of spotiphy can be found in folder [Tutorials](https://github.com/jyyulab/Spotiphy/tree/main/tutorials).
+Spotiphy is a Python-based pipeline designed to enhance our understanding of biological tissues by integrating sequencing-based spatial transcriptomics data, scRNA-seq data, and high-resolution histological images. Employing a probabilistic model, Bayesian inference, and advanced image processing techniques, Spotiphy primarily executes three key tasks:
+- **Deconvolution**: Spotiphy estimates the abundance of each cell type in each capture area of spatial tissue.
+- **Decomposition**: Spotiphy decomposes spatial transcriptomics data to the single-cell level.
+- **Pseudo single-cell resolution image**: Spotiphy generates a pseudo single-cell resolution image to reconstruct cell neighbors.
+
+With these outputs, Spotiphy facilitates numerous downstream analyses. For more detailed information, please refer to the associated research paper.
+
+![Spotiphy_overview](https://github.com/jyyulab/Spotiphy/blob/d62e05cb677ef6177acbda660b029ee0de1e82b3/figures/Spotiphy_overview.png)
+
+## Tutorials and documents
+
+The following tutorial are available:
+
++ Deconvolution and decomposition of mouse cortex with Spotiphy [[document](https://colab.research.google.com/github/jyyulab/Spotiphy/blob/main/tutorials/Spotiphy_tutorial_1.ipynb)][[Google Colab](https://colab.research.google.com/github/jyyulab/Spotiphy/blob/main/tutorials/Spotiphy_tutorial_1.ipynb)]
+
+
+For more details, please refer to the [documents](https://jyyulab.github.io/Spotiphy).
 
 ## Installation
 
 [//]: # (### Requirements)
 [//]: # (+ Linux/UNIX/Windows system)
 [//]: # (+ Python >= 3.9)
 [//]: # (+ pytorch == 1.7.1)
@@ -259,29 +279,30 @@
 more flexibility, particularly for those who wish to utilize CUDA capabilities.
 We offer two methods for installing the Spotiphy package:
 + **Install from GitHub**: This method allows you to install the latest version directly from the source code hosted on 
 GitHub.
 ```bash
 pip install git+https://github.com/jyyulab/Spotiphy.git
 ```
-+ **Install from PyPI using `pip`**: This approach is for installing the Spotiphy package from the Python Package Index 
++ **Install from PyPI**: This approach is for installing the Spotiphy package from the Python Package Index 
 (PyPI), which is more streamlined for users who prefer standard package installations.
 ```bash
-pip install spotiphy==0.1.2
+pip install spotiphy
 ```
 
 To test the Installation, try to import Spotiphy in Python.
 ```Python
 import spotiphy
 ```
-## Documentation and API details
 
 
-## FAQ
-See https://github.com/jyyulab/Spotiphy/discussions
+## Frequently asked questions
+Answers to frequently asked questions can be found [here](https://jyyulab.github.io/Spotiphy/questions.html).
+
+Should you have any further questions, feel free to start a [discussion](https://github.com/jyyulab/Spotiphy/discussions) or reach out directly to the package authors:
++ Ziqian Zheng - [zzheng92@wisc.edu](mailto:zzheng92@wisc.edu)
++ Jiyuan Yang - [jiyuan.yang@stjude.org](mailto:jiyuan.yang@stjude.org)
 
 
 ## Cite Spotiphy:
 
-If you have questions, please contact the authors of the method:
-+ Ziqian Zheng - zzheng92@wic.edu
-+ Jiyuan Yang - jiyuan.yang@stjude.org
+Pending
```


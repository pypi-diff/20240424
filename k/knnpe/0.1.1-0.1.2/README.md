# Comparing `tmp/knnpe-0.1.1.tar.gz` & `tmp/knnpe-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "knnpe-0.1.1.tar", last modified: Tue Mar 19 18:28:54 2024, max compression
+gzip compressed data, was "knnpe-0.1.2.tar", last modified: Wed Apr 24 20:51:12 2024, max compression
```

## Comparing `knnpe-0.1.1.tar` & `knnpe-0.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 18:28:54.711377 knnpe-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-03-19 18:28:39.000000 knnpe-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     9042 2024-03-19 18:28:54.711377 knnpe-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8315 2024-03-19 18:28:39.000000 knnpe-0.1.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 18:28:54.707377 knnpe-0.1.1/knnpe/
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-03-19 18:28:39.000000 knnpe-0.1.1/knnpe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13578 2024-03-19 18:28:39.000000 knnpe-0.1.1/knnpe/knnpe.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 18:28:54.707377 knnpe-0.1.1/knnpe/rwalk/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-19 18:28:39.000000 knnpe-0.1.1/knnpe/rwalk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7989 2024-03-19 18:28:39.000000 knnpe-0.1.1/knnpe/rwalk/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 18:28:54.711377 knnpe-0.1.1/knnpe.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9042 2024-03-19 18:28:54.000000 knnpe-0.1.1/knnpe.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-03-19 18:28:54.000000 knnpe-0.1.1/knnpe.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-19 18:28:54.000000 knnpe-0.1.1/knnpe.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-19 18:28:54.000000 knnpe-0.1.1/knnpe.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-03-19 18:28:39.000000 knnpe-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-03-19 18:28:54.711377 knnpe-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      777 2024-03-19 18:28:39.000000 knnpe-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:51:12.469764 knnpe-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-04-24 20:51:04.000000 knnpe-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8489 2024-04-24 20:51:12.469764 knnpe-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7762 2024-04-24 20:51:04.000000 knnpe-0.1.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:51:12.469764 knnpe-0.1.2/knnpe/
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-24 20:51:04.000000 knnpe-0.1.2/knnpe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14964 2024-04-24 20:51:04.000000 knnpe-0.1.2/knnpe/knnpe.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:51:12.469764 knnpe-0.1.2/knnpe/rwalk/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-24 20:51:04.000000 knnpe-0.1.2/knnpe/rwalk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7989 2024-04-24 20:51:04.000000 knnpe-0.1.2/knnpe/rwalk/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:51:12.469764 knnpe-0.1.2/knnpe.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8489 2024-04-24 20:51:12.000000 knnpe-0.1.2/knnpe.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-24 20:51:12.000000 knnpe-0.1.2/knnpe.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 20:51:12.000000 knnpe-0.1.2/knnpe.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-24 20:51:12.000000 knnpe-0.1.2/knnpe.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-24 20:51:04.000000 knnpe-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-24 20:51:12.473764 knnpe-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-04-24 20:51:04.000000 knnpe-0.1.2/setup.py
```

### Comparing `knnpe-0.1.1/LICENSE` & `knnpe-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `knnpe-0.1.1/PKG-INFO` & `knnpe-0.1.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,64 +1,50 @@
 Metadata-Version: 2.1
 Name: knnpe
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Python package for characterizing unstructured data with the nearest neighbor permutation entropy
 Author: L. G. J. M. Voltarelli, A. A. B. Pessa, L. Zunino, R. S. Zola, E. K. Lenzi, M. Perc, H. V. Ribeiro
 Author-email: "Haroldo V. Ribeiro" <hvr@dfi.uem.br>
 Project-URL: Homepage, https://github.com/hvribeiro/knnpe
 Project-URL: Repository, https://github.com/hvribeiro/knnpe
 Project-URL: Issues, https://github.com/hvribeiro/knnpe/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
-.. |logo1| image:: https://img.shields.io/pypi/v/knnpe?style=plastic   :alt: PyPI 
-   :target: https://pypi.org/project/knnpe/
-   :scale: 100%
-.. |logo2| image:: https://img.shields.io/github/license/hvribeiro/knnpe?style=plastic   :alt: GitHub 
-   :target: https://github.com/hvribeiro/knnpe/blob/main/LICENSE
-   :scale: 100%
-.. |logo3| image:: https://img.shields.io/pypi/dm/knnpe?style=plastic   :alt: PyPI - Downloads
-   :target: https://pypi.org/project/knnpe/
-   :scale: 100%
-.. |logo4| image:: https://readthedocs.org/projects/knnpe/badge/?version=latest
-   :target: https://knnpe.readthedocs.io/?badge=latest
-   :alt: Documentation Status
-   :scale: 100%
-
-|logo1| |logo2| |logo3| |logo4|
-
 knnpe: A Python package implementing the *k*-nearest neighbor permutation entropy
 =================================================================================
 
 The *k*-nearest neighbor permutation entropy [#voltarelli2024]_ extends the fundamental premise of investigating 
 the relative ordering of time series elements [#bandtpompe2002]_ or image pixels [#ribeiro2012]_ inaugurated by 
 permutation entropy to unstructured datasets. This method builds upon nearest neighbor graphs to establish neighborhood
 relations among data points and uses random walks over these graphs to extract ordinal patterns and their distribution, 
 thereby defining the $k$-nearest neighbor permutation entropy.
-
-If you have used ``knnpe`` in a scientific publication, we would appreciate citations to the following reference [#voltarelli2024]_:
+ 
+If you have used ``knnpe`` in a scientific publication, we would appreciate citations to the following reference:
 
 - L. G. J. M. Voltarelli, A. A. B. Pessa, L. Zunino, R. S. Zola, E. K. Lenzi, M. Perc, H. V. Ribeiro, 
-  `Characterizing unstructured data with the nearest neighbor permutation entropy <https://doi.org/?>`_, 
-  ?, ? (2024).  `arXiv:? <https://arxiv.org/abs/?>`_
+  `Characterizing unstructured data with the nearest neighbor permutation entropy <https://arxiv.org/abs/2403.13122>`_, 
+  ?, ? (2024).  `arXiv:2403.13122 <https://arxiv.org/abs/2403.13122>`_
 
 .. code-block:: bibtex
     
    @article{voltarelli2024characterizing,
     title         = {Characterizing unstructured data with the nearest neighbor permutation entropy}, 
     author        = {L. G. J. M. Voltarelli, A. A. B. Pessa, L. Zunino, R. S. Zola, E. K. Lenzi, M. Perc, H. V. Ribeiro},
     journal       = {},
     volume        = {},
     number        = {},
     pages         = {},
     year          = {2024},
+    eprint        = {2403.13122},
+    archivePrefix = {arXiv},
     doi           = {},
    }
 
 Installing
 ==========
 
 ``knnpe`` uses `OpenMP <https://www.openmp.org/>`_ and `GNU Scientific Library (GSL) <https://www.gnu.org/software/gsl/>`_ 
@@ -69,15 +55,15 @@
 
 .. code-block:: console
 
    sudo apt install build-essential
    sudo apt install libgsl-dev
    sudo apt install libomp-dev
 
-If these dependencies are not available, ``knnpe`` will use a native Python function for doing the random walks. This function is also parallelized and may work nicely for most applications; still, it is significantly slower than its C counterpart. For large datasets, we strongly recommend using the C version.
+If these dependencies are not available, ``knnpe`` will use a native Python function to do the random walks. This function is also parallelized and may work nicely for most applications; still, it is significantly slower than its C counterpart. For large datasets, we strongly recommend using the C version.
 
 If all dependencies are available, ``knnpe`` can be installed via:
 
 .. code-block:: console
 
    pip install git+https://github.com/hvribeiro/knnpe
 
@@ -85,39 +71,38 @@
 
 .. code-block:: console
 
    git clone https://github.com/hvribeiro/knnpe.git
    cd knnpe
    pip install -e .
 
-If all dependencies are **not** available, you can the PyPI version via:
+If all dependencies are **not** available, you can use the PyPI version via:
 
 .. code-block:: console
 
    pip install knnpe
 
 Basic usage
 ===========
 Implementation of the $k$-nearest neighbor permutation entropy. (A) Illustration of a dataset with irregularly distributed data points $\\{z_i\\}_{i=1,\\dots,N}$ in the $xy$-plane where each coordinate pair $(x_i,y_i)$ is associated with a value $z_i$. (B) Initially, we construct a $k$-nearest neighbor graph using the data coordinates to define neighborhood relationships. In this graph, each data point $z_i$ represents a node, with undirected edges connecting pairs $i\\leftrightarrow j$ when $j$ is among the $k$-nearest neighbors of $i$ ($k=3$ in this example). (C) Subsequently, we execute $n$ biased random walks of length $w$ starting from each node, sampling the data points to generate time series ($n=2$ and $w=6$ in this example). We then apply the Bandt-Pompe approach to each of these time series. This involves creating overlapping partitions of length $d$ (embedding dimension) and arranging the partition indices in ascending order of their values to determine the sorting permutations for each partition ($d=3$ in this example). (D) Finally, we evaluate the probability of each of the $d!$ possible permutations (ordinal distribution) and calculate its Shannon entropy, thereby defining the $k$-nearest neighbor permutation entropy.
 
 .. figure:: https://raw.githubusercontent.com/hvribeiro/knnpe/main/examples/figs/figmethod.png
-   :scale: 80 %
    :align: center
 
 The function `knn_permutation_entropy` of ``knnpe`` calculates $k$-nearest neighbor permutation entropy as illustrated below for a random dataset with three columns.
 
 .. code-block:: python
 
    import numpy as np
    from knnpe import knn_permutation_entropy
    
    data = np.random.normal(size=(100,3))
    knn_permutation_entropy(data)
 
-The last column in `data` corresponds to $\\{z_i\\}_{i=1,\\dots,N}$ values, while the first two columns are used as the data coordinates $\\vec{r}_i = (x_i,y_i)$. If the dataset has more dimensions in data coordinates, they must be passed as the first columns of the dataset, and the last column is always assumed to be corresponding $z_i$ values. The code below illustrates the case of data with three dimensions in data coordinates:
+The last column in `data` corresponds to $\\{z_i\\}_{i=1,\\dots,N}$ values, while the first two columns are used as the data coordinates $\\vec{r}_i = (x_i,y_i)$. If the dataset has more dimensions in data coordinates, they must be passed as the first columns of the dataset, and the last column is always assumed to correspond to $z_i$ values. The code below illustrates the case of data with three dimensions in data coordinates:
 
 .. code-block:: python
 
    import numpy as np
    from knnpe import knn_permutation_entropy
    
    data = np.random.normal(size=(100,4))
@@ -145,27 +130,32 @@
      The number of neighbors for constructing the k-nearest neighbor graph (default is 25).
  nthreads : int, optional
      The number of parallel threads for the computation (default is -1, which uses all available cores).
  hide_bar : bool, optional
      If True, the progress bar is not displayed (default is False).
  metrics : bool, optional
      If True, calculates graph density and largest component fraction (default is False).
+ complexity : bool, optional
+     If True, also calculates the knn permutation complexity.
 
 We provide a `notebook <https://github.com/hvribeiro/knnpe/blob/main/examples/knnpe.ipynb>`_
-illustrating how to use ``knnpe`` and further information we refer to the knnpe's `documentation <https://readthedocs.org/projects/knnpe/badge/?version=latest>`_
+illustrating how to use ``knnpe`` and further information we refer to the knnpe's `documentation <https://hvribeiro.github.io/knnpe/>`_
 
 Contributing
 ============
 
 Pull requests addressing errors or adding new functionalities are always welcome.
 
 References
 ==========
 
-.. [#voltarelli2024] L. G. J. M. Voltarelli, A. A. B. Pessa, L. Zunino, 
-   R. S. Zola, E. K. Lenzi, M. Perc, H. V. Ribeiro. Characterizing unstructured 
-   data with the nearest neighbor permutation entropy. ?, ? (2024).
-.. [#bandtpompe2002] C. Bandt, B. Pompe. Permutation entropy: A Natural 
-   Complexity Measure for Time Series. Physical Review Letters 88, 174102 (2002).
-.. [#ribeiro2012] H. V. Ribeiro, L. Zunino, E. K. Lenzi, P. A. Santoro, R. S.
-   Mendes. Complexity-Entropy Causality Plane as a Complexity
-   Measure for Two-Dimensional Patterns. PLOS ONE 7, e40689 (2012).
+.. [#voltarelli2024] L. G. J. M. Voltarelli, A. A. B. Pessa, L. Zunino, R. S. Zola, E. K. Lenzi, M. Perc, H. V. Ribeiro. 
+   Characterizing unstructured data with the nearest neighbor permutation entropy. 
+   arXiv, 2403.13122 (2024).
+
+.. [#bandtpompe2002] C. Bandt, B. Pompe. 
+   Permutation entropy: A Natural Complexity Measure for Time Series. 
+   Physical Review Letters 88, 174102 (2002).
+
+.. [#ribeiro2012] H. V. Ribeiro, L. Zunino, E. K. Lenzi, P. A. Santoro, R. S. Mendes.
+   Complexity-Entropy Causality Plane as a Complexity Measure for Two-Dimensional Patterns. 
+   PLOS ONE 7, e40689 (2012).
```

### Comparing `knnpe-0.1.1/README.rst` & `knnpe-0.1.2/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,48 +1,34 @@
-.. |logo1| image:: https://img.shields.io/pypi/v/knnpe?style=plastic   :alt: PyPI 
-   :target: https://pypi.org/project/knnpe/
-   :scale: 100%
-.. |logo2| image:: https://img.shields.io/github/license/hvribeiro/knnpe?style=plastic   :alt: GitHub 
-   :target: https://github.com/hvribeiro/knnpe/blob/main/LICENSE
-   :scale: 100%
-.. |logo3| image:: https://img.shields.io/pypi/dm/knnpe?style=plastic   :alt: PyPI - Downloads
-   :target: https://pypi.org/project/knnpe/
-   :scale: 100%
-.. |logo4| image:: https://readthedocs.org/projects/knnpe/badge/?version=latest
-   :target: https://knnpe.readthedocs.io/?badge=latest
-   :alt: Documentation Status
-   :scale: 100%
-
-|logo1| |logo2| |logo3| |logo4|
-
 knnpe: A Python package implementing the *k*-nearest neighbor permutation entropy
 =================================================================================
 
 The *k*-nearest neighbor permutation entropy [#voltarelli2024]_ extends the fundamental premise of investigating 
 the relative ordering of time series elements [#bandtpompe2002]_ or image pixels [#ribeiro2012]_ inaugurated by 
 permutation entropy to unstructured datasets. This method builds upon nearest neighbor graphs to establish neighborhood
 relations among data points and uses random walks over these graphs to extract ordinal patterns and their distribution, 
 thereby defining the $k$-nearest neighbor permutation entropy.
-
-If you have used ``knnpe`` in a scientific publication, we would appreciate citations to the following reference [#voltarelli2024]_:
+ 
+If you have used ``knnpe`` in a scientific publication, we would appreciate citations to the following reference:
 
 - L. G. J. M. Voltarelli, A. A. B. Pessa, L. Zunino, R. S. Zola, E. K. Lenzi, M. Perc, H. V. Ribeiro, 
-  `Characterizing unstructured data with the nearest neighbor permutation entropy <https://doi.org/?>`_, 
-  ?, ? (2024).  `arXiv:? <https://arxiv.org/abs/?>`_
+  `Characterizing unstructured data with the nearest neighbor permutation entropy <https://arxiv.org/abs/2403.13122>`_, 
+  ?, ? (2024).  `arXiv:2403.13122 <https://arxiv.org/abs/2403.13122>`_
 
 .. code-block:: bibtex
     
    @article{voltarelli2024characterizing,
     title         = {Characterizing unstructured data with the nearest neighbor permutation entropy}, 
     author        = {L. G. J. M. Voltarelli, A. A. B. Pessa, L. Zunino, R. S. Zola, E. K. Lenzi, M. Perc, H. V. Ribeiro},
     journal       = {},
     volume        = {},
     number        = {},
     pages         = {},
     year          = {2024},
+    eprint        = {2403.13122},
+    archivePrefix = {arXiv},
     doi           = {},
    }
 
 Installing
 ==========
 
 ``knnpe`` uses `OpenMP <https://www.openmp.org/>`_ and `GNU Scientific Library (GSL) <https://www.gnu.org/software/gsl/>`_ 
@@ -53,15 +39,15 @@
 
 .. code-block:: console
 
    sudo apt install build-essential
    sudo apt install libgsl-dev
    sudo apt install libomp-dev
 
-If these dependencies are not available, ``knnpe`` will use a native Python function for doing the random walks. This function is also parallelized and may work nicely for most applications; still, it is significantly slower than its C counterpart. For large datasets, we strongly recommend using the C version.
+If these dependencies are not available, ``knnpe`` will use a native Python function to do the random walks. This function is also parallelized and may work nicely for most applications; still, it is significantly slower than its C counterpart. For large datasets, we strongly recommend using the C version.
 
 If all dependencies are available, ``knnpe`` can be installed via:
 
 .. code-block:: console
 
    pip install git+https://github.com/hvribeiro/knnpe
 
@@ -69,39 +55,38 @@
 
 .. code-block:: console
 
    git clone https://github.com/hvribeiro/knnpe.git
    cd knnpe
    pip install -e .
 
-If all dependencies are **not** available, you can the PyPI version via:
+If all dependencies are **not** available, you can use the PyPI version via:
 
 .. code-block:: console
 
    pip install knnpe
 
 Basic usage
 ===========
 Implementation of the $k$-nearest neighbor permutation entropy. (A) Illustration of a dataset with irregularly distributed data points $\\{z_i\\}_{i=1,\\dots,N}$ in the $xy$-plane where each coordinate pair $(x_i,y_i)$ is associated with a value $z_i$. (B) Initially, we construct a $k$-nearest neighbor graph using the data coordinates to define neighborhood relationships. In this graph, each data point $z_i$ represents a node, with undirected edges connecting pairs $i\\leftrightarrow j$ when $j$ is among the $k$-nearest neighbors of $i$ ($k=3$ in this example). (C) Subsequently, we execute $n$ biased random walks of length $w$ starting from each node, sampling the data points to generate time series ($n=2$ and $w=6$ in this example). We then apply the Bandt-Pompe approach to each of these time series. This involves creating overlapping partitions of length $d$ (embedding dimension) and arranging the partition indices in ascending order of their values to determine the sorting permutations for each partition ($d=3$ in this example). (D) Finally, we evaluate the probability of each of the $d!$ possible permutations (ordinal distribution) and calculate its Shannon entropy, thereby defining the $k$-nearest neighbor permutation entropy.
 
 .. figure:: https://raw.githubusercontent.com/hvribeiro/knnpe/main/examples/figs/figmethod.png
-   :scale: 80 %
    :align: center
 
 The function `knn_permutation_entropy` of ``knnpe`` calculates $k$-nearest neighbor permutation entropy as illustrated below for a random dataset with three columns.
 
 .. code-block:: python
 
    import numpy as np
    from knnpe import knn_permutation_entropy
    
    data = np.random.normal(size=(100,3))
    knn_permutation_entropy(data)
 
-The last column in `data` corresponds to $\\{z_i\\}_{i=1,\\dots,N}$ values, while the first two columns are used as the data coordinates $\\vec{r}_i = (x_i,y_i)$. If the dataset has more dimensions in data coordinates, they must be passed as the first columns of the dataset, and the last column is always assumed to be corresponding $z_i$ values. The code below illustrates the case of data with three dimensions in data coordinates:
+The last column in `data` corresponds to $\\{z_i\\}_{i=1,\\dots,N}$ values, while the first two columns are used as the data coordinates $\\vec{r}_i = (x_i,y_i)$. If the dataset has more dimensions in data coordinates, they must be passed as the first columns of the dataset, and the last column is always assumed to correspond to $z_i$ values. The code below illustrates the case of data with three dimensions in data coordinates:
 
 .. code-block:: python
 
    import numpy as np
    from knnpe import knn_permutation_entropy
    
    data = np.random.normal(size=(100,4))
@@ -129,27 +114,32 @@
      The number of neighbors for constructing the k-nearest neighbor graph (default is 25).
  nthreads : int, optional
      The number of parallel threads for the computation (default is -1, which uses all available cores).
  hide_bar : bool, optional
      If True, the progress bar is not displayed (default is False).
  metrics : bool, optional
      If True, calculates graph density and largest component fraction (default is False).
+ complexity : bool, optional
+     If True, also calculates the knn permutation complexity.
 
 We provide a `notebook <https://github.com/hvribeiro/knnpe/blob/main/examples/knnpe.ipynb>`_
-illustrating how to use ``knnpe`` and further information we refer to the knnpe's `documentation <https://readthedocs.org/projects/knnpe/badge/?version=latest>`_
+illustrating how to use ``knnpe`` and further information we refer to the knnpe's `documentation <https://hvribeiro.github.io/knnpe/>`_
 
 Contributing
 ============
 
 Pull requests addressing errors or adding new functionalities are always welcome.
 
 References
 ==========
 
-.. [#voltarelli2024] L. G. J. M. Voltarelli, A. A. B. Pessa, L. Zunino, 
-   R. S. Zola, E. K. Lenzi, M. Perc, H. V. Ribeiro. Characterizing unstructured 
-   data with the nearest neighbor permutation entropy. ?, ? (2024).
-.. [#bandtpompe2002] C. Bandt, B. Pompe. Permutation entropy: A Natural 
-   Complexity Measure for Time Series. Physical Review Letters 88, 174102 (2002).
-.. [#ribeiro2012] H. V. Ribeiro, L. Zunino, E. K. Lenzi, P. A. Santoro, R. S.
-   Mendes. Complexity-Entropy Causality Plane as a Complexity
-   Measure for Two-Dimensional Patterns. PLOS ONE 7, e40689 (2012).
+.. [#voltarelli2024] L. G. J. M. Voltarelli, A. A. B. Pessa, L. Zunino, R. S. Zola, E. K. Lenzi, M. Perc, H. V. Ribeiro. 
+   Characterizing unstructured data with the nearest neighbor permutation entropy. 
+   arXiv, 2403.13122 (2024).
+
+.. [#bandtpompe2002] C. Bandt, B. Pompe. 
+   Permutation entropy: A Natural Complexity Measure for Time Series. 
+   Physical Review Letters 88, 174102 (2002).
+
+.. [#ribeiro2012] H. V. Ribeiro, L. Zunino, E. K. Lenzi, P. A. Santoro, R. S. Mendes.
+   Complexity-Entropy Causality Plane as a Complexity Measure for Two-Dimensional Patterns. 
+   PLOS ONE 7, e40689 (2012).
```

### Comparing `knnpe-0.1.1/knnpe/knnpe.py` & `knnpe-0.1.2/knnpe/knnpe.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,34 +2,38 @@
 knnpe: A Python package implementing the *k*-nearest neighbor permutation entropy
 =================================================================================
 
 The *k*-nearest neighbor permutation entropy [#voltarelli2024]_ extends the fundamental premise of investigating 
 the relative ordering of time series elements [#bandtpompe2002]_ or image pixels [#ribeiro2012]_ inaugurated by 
 permutation entropy to unstructured datasets. This method builds upon nearest neighbor graphs to establish neighborhood
 relations among data points and uses random walks over these graphs to extract ordinal patterns and their distribution, 
-thereby defining the :math:`k`-nearest neighbor permutation entropy.
+thereby defining the $k$-nearest neighbor permutation entropy.
 
-If you have used ``knnpe`` in a scientific publication, we would appreciate citations to the following reference [#voltarelli2024]_:
-
-- L. G. J. M. Voltarelli, A. A. B. Pessa, L. Zunino, R. S. Zola, E. K. Lenzi, M. Perc, H. V. Ribeiro, 
-  `Characterizing unstructured data with the nearest neighbor permutation entropy <https://doi.org/?>`_, 
-  ?, ? (2024).  `arXiv:? <https://arxiv.org/abs/?>`_
-
-.. code-block:: bibtex
-    
-   @article{voltarelli2024characterizing,
-    title         = {Characterizing unstructured data with the nearest neighbor permutation entropy}, 
-    author        = {L. G. J. M. Voltarelli, A. A. B. Pessa, L. Zunino, R. S. Zola, E. K. Lenzi, M. Perc, H. V. Ribeiro},
-    journal       = {},
-    volume        = {},
-    number        = {},
-    pages         = {},
-    year          = {2024},
-    doi           = {},
-   }
+.. note::
+  
+   If you have used ``knnpe`` in a scientific publication, we would appreciate citations to the following reference:
+
+   - L. G. J. M. Voltarelli, A. A. B. Pessa, L. Zunino, R. S. Zola, E. K. Lenzi, M. Perc, H. V. Ribeiro, 
+     `Characterizing unstructured data with the nearest neighbor permutation entropy <https://arxiv.org/abs/2403.13122>`_, 
+     ?, ? (2024). `arXiv:2403.13122 <https://arxiv.org/abs/2403.13122>`_
+
+   .. code-block:: bibtex
+       
+      @article{voltarelli2024characterizing,
+       title         = {Characterizing unstructured data with the nearest neighbor permutation entropy}, 
+       author        = {L. G. J. M. Voltarelli, A. A. B. Pessa, L. Zunino, R. S. Zola, E. K. Lenzi, M. Perc, H. V. Ribeiro},
+       journal       = {},
+       volume        = {},
+       number        = {},
+       pages         = {},
+       year          = {2024},
+       eprint        = {2403.13122},
+       archivePrefix = {arXiv},
+       doi           = {},
+      }
 
 Installing
 ==========
 
 ``knnpe`` uses `OpenMP <https://www.openmp.org/>`_ and `GNU Scientific Library (GSL) <https://www.gnu.org/software/gsl/>`_ 
 to implement a parallelized numerically efficient random walk function. This function is written in C and it is integrated with our 
 Python module via the `ctypes <https://docs.python.org/3/library/ctypes.html>`_ library. To use this function, you must have OpenMP and GSL installed before installing ``knnpe``. 
@@ -38,51 +42,55 @@
 
 .. code-block:: console
 
    sudo apt install build-essential
    sudo apt install libgsl-dev
    sudo apt install libomp-dev
 
-If these dependencies are not available, ``knnpe`` will use a native Python function for doing the random walks. This function is also parallelized and may work nicely for most applications; still, it is significantly slower than its C counterpart. For large datasets, we strongly recommend using the C version.
+If these dependencies are not available, ``knnpe`` will use a native Python function to do the random walks. This function is also parallelized and may work nicely for most applications; still, it is significantly slower than its C counterpart. For large datasets, we strongly recommend using the C version.
 
-Whether the dependencies are available or not, ``knnpe`` can be installed via:
+If all dependencies are available, ``knnpe`` can be installed via:
 
 .. code-block:: console
 
-   pip install knnpe
+   pip install git+https://github.com/hvribeiro/knnpe
 
-or you can directly clone its git repository:
+or
 
 .. code-block:: console
 
    git clone https://github.com/hvribeiro/knnpe.git
    cd knnpe
    pip install -e .
 
+If all dependencies are **not** available, you can use the PyPI version via:
+
+.. code-block:: console
+
+   pip install knnpe
 
 Basic usage
 ===========
-Implementation of the :math:`k`-nearest neighbor permutation entropy. (A) Illustration of a dataset with irregularly distributed data points :math:`\\{z_i\\}_{i=1,\\dots,N}` in the :math:`xy`-plane where each coordinate pair :math:`(x_i,y_i)` is associated with a value :math:`z_i`. (B) Initially, we construct a :math:`k`-nearest neighbor graph using the data coordinates to define neighborhood relationships. In this graph, each data point :math:`z_i` represents a node, with undirected edges connecting pairs :math:`i\\leftrightarrow j` when :math:`j` is among the :math:`k`-nearest neighbors of :math:`i` (:math:`k=3` in this example). (C) Subsequently, we execute :math:`n` biased random walks of length :math:`w` starting from each node, sampling the data points to generate time series (`n=2` and :math:`w=6` in this example). We then apply the Bandt-Pompe approach to each of these time series. This involves creating overlapping partitions of length :math:`d` (embedding dimension) and arranging the partition indices in ascending order of their values to determine the sorting permutations for each partition (`d=3` in this example). (D) Finally, we evaluate the probability of each of the :math:`d!` possible permutations (ordinal distribution) and calculate its Shannon entropy, thereby defining the :math:`k`-nearest neighbor permutation entropy.
+Implementation of the $k$-nearest neighbor permutation entropy. (A) Illustration of a dataset with irregularly distributed data points $\\{z_i\\}_{i=1,\\dots,N}$ in the $xy$-plane where each coordinate pair $(x_i,y_i)$ is associated with a value $z_i$. (B) Initially, we construct a $k$-nearest neighbor graph using the data coordinates to define neighborhood relationships. In this graph, each data point $z_i$ represents a node, with undirected edges connecting pairs $i\\leftrightarrow j$ when $j$ is among the $k$-nearest neighbors of $i$ ($k=3$ in this example). (C) Subsequently, we execute $n$ biased random walks of length $w$ starting from each node, sampling the data points to generate time series ($n=2$ and $w=6$ in this example). We then apply the Bandt-Pompe approach to each of these time series. This involves creating overlapping partitions of length $d$ (embedding dimension) and arranging the partition indices in ascending order of their values to determine the sorting permutations for each partition ($d=3$ in this example). (D) Finally, we evaluate the probability of each of the $d!$ possible permutations (ordinal distribution) and calculate its Shannon entropy, thereby defining the $k$-nearest neighbor permutation entropy.
 
 .. figure:: https://raw.githubusercontent.com/hvribeiro/knnpe/main/examples/figs/figmethod.png
+   :scale: 80 %
    :align: center
 
-|
-
-The function `knn_permutation_entropy` of ``knnpe`` calculates :math:`k`-nearest neighbor permutation entropy as illustrated below for a random dataset with three columns.
+The function `knn_permutation_entropy` of ``knnpe`` calculates $k$-nearest neighbor permutation entropy as illustrated below for a random dataset with three columns.
 
 .. code-block:: python
 
    import numpy as np
    from knnpe import knn_permutation_entropy
    
    data = np.random.normal(size=(100,3))
    knn_permutation_entropy(data)
 
-The last column in `data` corresponds to :math:`\\{z_i\\}_{i=1,\\dots,N}` values, while the first two columns are used as the data coordinates :math:`\\vec{r}_i = (x_i,y_i)`. If the dataset has more dimensions in data coordinates, they must be passed as the first columns of the dataset, and the last column is always assumed to be corresponding :math:`z_i` values. The code below illustrates the case of data with three dimensions in data coordinates:
+The last column in `data` corresponds to $\\{z_i\\}_{i=1,\\dots,N}$ values, while the first two columns are used as the data coordinates $\\vec{r}_i = (x_i,y_i)$. If the dataset has more dimensions in data coordinates, they must be passed as the first columns of the dataset, and the last column is always assumed to correspond to $z_i$ values. The code below illustrates the case of data with three dimensions in data coordinates:
 
 .. code-block:: python
 
    import numpy as np
    from knnpe import knn_permutation_entropy
    
    data = np.random.normal(size=(100,4))
@@ -110,49 +118,55 @@
      The number of neighbors for constructing the k-nearest neighbor graph (default is 25).
  nthreads : int, optional
      The number of parallel threads for the computation (default is -1, which uses all available cores).
  hide_bar : bool, optional
      If True, the progress bar is not displayed (default is False).
  metrics : bool, optional
      If True, calculates graph density and largest component fraction (default is False).
+ complexity : bool, optional
+     If True, also calculates the knn permutation complexity.
 
-We provide a `notebook <https://github.com/hvribeiro/knnpe/blob/master/examples/knnpe.ipynb>`_
-illustrating how to use ``knnpe`` and further information we refer to the knnpe's `documentation <https://readthedocs.org/projects/knnpe/badge/?version=latest>`_
+We provide a `notebook <https://github.com/hvribeiro/knnpe/blob/main/examples/knnpe.ipynb>`_
+illustrating how to use ``knnpe`` and further information we refer to the knnpe's `documentation <https://hvribeiro.github.io/knnpe/>`_
 
 Contributing
 ============
 
 Pull requests addressing errors or adding new functionalities are always welcome.
 
 References
 ==========
 
-.. [#voltarelli2024] L. G. J. M. Voltarelli, A. A. B. Pessa, L. Zunino, 
-   R. S. Zola, E. K. Lenzi, M. Perc, H. V. Ribeiro. Characterizing unstructured 
-   data with the nearest neighbor permutation entropy. ?, ? (2024).
-.. [#bandtpompe2002] C. Bandt, B. Pompe. Permutation entropy: A Natural 
-   Complexity Measure for Time Series. Physical Review Letters 88, 174102 (2002).
-.. [#ribeiro2012] H. V. Ribeiro, L. Zunino, E. K. Lenzi, P. A. Santoro, R. S.
-   Mendes. Complexity-Entropy Causality Plane as a Complexity
-   Measure for Two-Dimensional Patterns. PLOS ONE 7, e40689 (2012).
+.. [#voltarelli2024] L. G. J. M. Voltarelli, A. A. B. Pessa, L. Zunino, R. S. Zola, E. K. Lenzi, M. Perc, H. V. Ribeiro. 
+   Characterizing unstructured data with the nearest neighbor permutation entropy. 
+   arXiv, 2403.13122 (2024).
+
+.. [#bandtpompe2002] C. Bandt, B. Pompe. 
+   Permutation entropy: A Natural Complexity Measure for Time Series. 
+   Physical Review Letters 88, 174102 (2002).
+
+.. [#ribeiro2012] H. V. Ribeiro, L. Zunino, E. K. Lenzi, P. A. Santoro, R. S. Mendes.
+   Complexity-Entropy Causality Plane as a Complexity Measure for Two-Dimensional Patterns. 
+   PLOS ONE 7, e40689 (2012).
 
 """
 
 import numpy as np
 
 from math                 import factorial
 from scipy.sparse.csgraph import connected_components
 from sklearn.neighbors    import kneighbors_graph
 from tqdm                 import tqdm
 
 from .rwalk import *
 
 
 def knn_permutation_entropy(data, d=3, tau=1, p=10, q=0.001, random_walk_steps=10, 
-                            num_walks=10, n_neighbors=25, nthreads=-1, hide_bar=True, metrics=False):
+                            num_walks=10, n_neighbors=25, nthreads=-1, hide_bar=True, metrics=False,
+                            complexity=False):
     """
     Estimates the k-nearest neighbor permutation entropy of unstructured data
     
     Parameters
     ----------
     data : ndarray
         Input array containing unstructured data points, where each row is in the form [x, y, value].
@@ -174,25 +188,29 @@
         The number of neighbors for constructing the k-nearest neighbor graph (default is 25).
     nthreads : int, optional
         The number of parallel threads for the computation (default is -1, which uses all available cores).
     hide_bar : bool, optional
         If True, the progress bar is not displayed (default is False).
     metrics : bool, optional
         If True, calculates graph density and largest component fraction (default is False).
+    complexity : bool, optional
+        If True, also calculates the knn permutation complexity.
+
     Returns
     -------
     float or np.ndarray
        The knn permutation entropy by default or an array of values for n_neighbors.
            If metrics is True, for each value in n_neighbors, it returns: 
                [n_neighbors, graph largest component fraction, graph density, knn entropy]
+        If complexity=True, knn entropy is replace by a list: [knn entropy, knn permutation complexity].
     """
 
 
     # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
-    def estimate_entropy_from_walks(time_series, all_walks, d, tau):
+    def estimate_entropy_from_walks(time_series, all_walks, d, tau, complexity=False):
         """
         Estimates the permutation entropy of a time series based on a set of random walks.
 
 
         Parameters
         ----------
         time_series : ndarray
@@ -200,23 +218,28 @@
         all_walks : list of ndarrays
             A list where each element is a numpy array representing a random walk. Each array
             contains indices corresponding to the time points in the time series.
         d : int
             The embedding dimension for the entropy calculation.
         tau : int
             The embedding delay for the entropy calculation.
+        complexity : bool, optional
+            If True, also calculates the permutation complexity.
 
         Returns
         -------
         float
             The knn permutation entropy of the time series based on the provided random walks.
+            If complexity=True, knn entropy is replace by list: [knn entropy, knn permutation complexity].
         """
-    
+
         ordinal_sequence = []
 
+        Smax  = np.log(factorial(d))
+
         for walk in all_walks:
             ts = np.expand_dims(time_series[walk],axis=0)
 
             partitions = np.apply_along_axis(func1d       = np.lib.stride_tricks.sliding_window_view, 
                                              axis         = 1, 
                                              arr          = ts, 
                                              window_shape = (d+(d-1)*(tau-1),)
@@ -224,15 +247,31 @@
 
             ordinal_sequence += [np.apply_along_axis(np.argsort, 1, partitions)]
 
         ordinal_sequence = np.vstack(ordinal_sequence)
         _, symbols_count = np.unique(ordinal_sequence, return_counts=True, axis=0)
         probabilities    = symbols_count/symbols_count.sum()
 
-        S = -np.sum(probabilities*np.log(probabilities))
+        S = -np.sum(probabilities*np.log(probabilities))/Smax
+
+        if complexity:
+            n = float(factorial(d))
+            n_states_not_occuring = n-len(probabilities)
+            uniform_dist          = 1/n
+
+            p_plus_u_over_2      = (uniform_dist + probabilities)/2  
+            s_of_p_plus_u_over_2 = -np.sum(p_plus_u_over_2*np.log(p_plus_u_over_2)) - (0.5*uniform_dist)*np.log(0.5*uniform_dist)*n_states_not_occuring
+
+            s_of_p_over_2 = -np.sum(probabilities*np.log(probabilities))/2
+            s_of_u_over_2 = np.log(n)/2.
+
+            js_div_max = -0.5*(((n+1)/n)*np.log(n+1) + np.log(n) - 2*np.log(2*n))    
+            js_div     = s_of_p_plus_u_over_2 - s_of_p_over_2 - s_of_u_over_2
+
+            return [S, S*js_div/js_div_max]
         
         return S
     # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
 
 
 
     data = np.asarray(data)
@@ -241,16 +280,14 @@
     time_series = data[:,-1]
 
     if not isinstance(n_neighbors, (list,np.ndarray)):
         n_neighbors = [n_neighbors]
 
     number_of_vertex = len(time_series)
     max_number_of_egdes = number_of_vertex*(number_of_vertex-1)/2.
-    
-    Smax  = np.log(factorial(d))
 
     property_list = []
     
     for n_neighbor in tqdm(n_neighbors, position=0, leave=True, disable=hide_bar):
         
         adj_matrix = kneighbors_graph(data_to_graph, n_neighbors=n_neighbor, n_jobs=-1)
         adj_matrix = ((adj_matrix+adj_matrix.T)>0).astype(int)
@@ -258,15 +295,15 @@
         
         ptr, neighs = adj_matrix_csr.indptr, adj_matrix_csr.indices
 
         all_walks = biased_random_walk(ptr, neighs, num_steps=random_walk_steps, 
                                        num_walks=num_walks, p=p, q=q, 
                                        nthreads=nthreads, seed=np.random.randint(1,1e6))
 
-        S = estimate_entropy_from_walks(time_series, all_walks, d, tau)/Smax
+        S = estimate_entropy_from_walks(time_series, all_walks, d, tau, complexity)
         
         if metrics:
             ncomonents, labels = connected_components(adj_matrix)
             component_ids, nvertex_component = np.unique(labels,return_counts=True)
             frac_largest_component = max(nvertex_component)/number_of_vertex
             number_of_egdes = int(np.sum(adj_matrix)/2)
             graph_density = number_of_egdes/max_number_of_egdes
```

### Comparing `knnpe-0.1.1/knnpe/rwalk/config.py` & `knnpe-0.1.2/knnpe/rwalk/config.py`

 * *Files identical despite different names*

### Comparing `knnpe-0.1.1/knnpe.egg-info/PKG-INFO` & `knnpe-0.1.2/knnpe.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,64 +1,50 @@
 Metadata-Version: 2.1
 Name: knnpe
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Python package for characterizing unstructured data with the nearest neighbor permutation entropy
 Author: L. G. J. M. Voltarelli, A. A. B. Pessa, L. Zunino, R. S. Zola, E. K. Lenzi, M. Perc, H. V. Ribeiro
 Author-email: "Haroldo V. Ribeiro" <hvr@dfi.uem.br>
 Project-URL: Homepage, https://github.com/hvribeiro/knnpe
 Project-URL: Repository, https://github.com/hvribeiro/knnpe
 Project-URL: Issues, https://github.com/hvribeiro/knnpe/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
-.. |logo1| image:: https://img.shields.io/pypi/v/knnpe?style=plastic   :alt: PyPI 
-   :target: https://pypi.org/project/knnpe/
-   :scale: 100%
-.. |logo2| image:: https://img.shields.io/github/license/hvribeiro/knnpe?style=plastic   :alt: GitHub 
-   :target: https://github.com/hvribeiro/knnpe/blob/main/LICENSE
-   :scale: 100%
-.. |logo3| image:: https://img.shields.io/pypi/dm/knnpe?style=plastic   :alt: PyPI - Downloads
-   :target: https://pypi.org/project/knnpe/
-   :scale: 100%
-.. |logo4| image:: https://readthedocs.org/projects/knnpe/badge/?version=latest
-   :target: https://knnpe.readthedocs.io/?badge=latest
-   :alt: Documentation Status
-   :scale: 100%
-
-|logo1| |logo2| |logo3| |logo4|
-
 knnpe: A Python package implementing the *k*-nearest neighbor permutation entropy
 =================================================================================
 
 The *k*-nearest neighbor permutation entropy [#voltarelli2024]_ extends the fundamental premise of investigating 
 the relative ordering of time series elements [#bandtpompe2002]_ or image pixels [#ribeiro2012]_ inaugurated by 
 permutation entropy to unstructured datasets. This method builds upon nearest neighbor graphs to establish neighborhood
 relations among data points and uses random walks over these graphs to extract ordinal patterns and their distribution, 
 thereby defining the $k$-nearest neighbor permutation entropy.
-
-If you have used ``knnpe`` in a scientific publication, we would appreciate citations to the following reference [#voltarelli2024]_:
+ 
+If you have used ``knnpe`` in a scientific publication, we would appreciate citations to the following reference:
 
 - L. G. J. M. Voltarelli, A. A. B. Pessa, L. Zunino, R. S. Zola, E. K. Lenzi, M. Perc, H. V. Ribeiro, 
-  `Characterizing unstructured data with the nearest neighbor permutation entropy <https://doi.org/?>`_, 
-  ?, ? (2024).  `arXiv:? <https://arxiv.org/abs/?>`_
+  `Characterizing unstructured data with the nearest neighbor permutation entropy <https://arxiv.org/abs/2403.13122>`_, 
+  ?, ? (2024).  `arXiv:2403.13122 <https://arxiv.org/abs/2403.13122>`_
 
 .. code-block:: bibtex
     
    @article{voltarelli2024characterizing,
     title         = {Characterizing unstructured data with the nearest neighbor permutation entropy}, 
     author        = {L. G. J. M. Voltarelli, A. A. B. Pessa, L. Zunino, R. S. Zola, E. K. Lenzi, M. Perc, H. V. Ribeiro},
     journal       = {},
     volume        = {},
     number        = {},
     pages         = {},
     year          = {2024},
+    eprint        = {2403.13122},
+    archivePrefix = {arXiv},
     doi           = {},
    }
 
 Installing
 ==========
 
 ``knnpe`` uses `OpenMP <https://www.openmp.org/>`_ and `GNU Scientific Library (GSL) <https://www.gnu.org/software/gsl/>`_ 
@@ -69,15 +55,15 @@
 
 .. code-block:: console
 
    sudo apt install build-essential
    sudo apt install libgsl-dev
    sudo apt install libomp-dev
 
-If these dependencies are not available, ``knnpe`` will use a native Python function for doing the random walks. This function is also parallelized and may work nicely for most applications; still, it is significantly slower than its C counterpart. For large datasets, we strongly recommend using the C version.
+If these dependencies are not available, ``knnpe`` will use a native Python function to do the random walks. This function is also parallelized and may work nicely for most applications; still, it is significantly slower than its C counterpart. For large datasets, we strongly recommend using the C version.
 
 If all dependencies are available, ``knnpe`` can be installed via:
 
 .. code-block:: console
 
    pip install git+https://github.com/hvribeiro/knnpe
 
@@ -85,39 +71,38 @@
 
 .. code-block:: console
 
    git clone https://github.com/hvribeiro/knnpe.git
    cd knnpe
    pip install -e .
 
-If all dependencies are **not** available, you can the PyPI version via:
+If all dependencies are **not** available, you can use the PyPI version via:
 
 .. code-block:: console
 
    pip install knnpe
 
 Basic usage
 ===========
 Implementation of the $k$-nearest neighbor permutation entropy. (A) Illustration of a dataset with irregularly distributed data points $\\{z_i\\}_{i=1,\\dots,N}$ in the $xy$-plane where each coordinate pair $(x_i,y_i)$ is associated with a value $z_i$. (B) Initially, we construct a $k$-nearest neighbor graph using the data coordinates to define neighborhood relationships. In this graph, each data point $z_i$ represents a node, with undirected edges connecting pairs $i\\leftrightarrow j$ when $j$ is among the $k$-nearest neighbors of $i$ ($k=3$ in this example). (C) Subsequently, we execute $n$ biased random walks of length $w$ starting from each node, sampling the data points to generate time series ($n=2$ and $w=6$ in this example). We then apply the Bandt-Pompe approach to each of these time series. This involves creating overlapping partitions of length $d$ (embedding dimension) and arranging the partition indices in ascending order of their values to determine the sorting permutations for each partition ($d=3$ in this example). (D) Finally, we evaluate the probability of each of the $d!$ possible permutations (ordinal distribution) and calculate its Shannon entropy, thereby defining the $k$-nearest neighbor permutation entropy.
 
 .. figure:: https://raw.githubusercontent.com/hvribeiro/knnpe/main/examples/figs/figmethod.png
-   :scale: 80 %
    :align: center
 
 The function `knn_permutation_entropy` of ``knnpe`` calculates $k$-nearest neighbor permutation entropy as illustrated below for a random dataset with three columns.
 
 .. code-block:: python
 
    import numpy as np
    from knnpe import knn_permutation_entropy
    
    data = np.random.normal(size=(100,3))
    knn_permutation_entropy(data)
 
-The last column in `data` corresponds to $\\{z_i\\}_{i=1,\\dots,N}$ values, while the first two columns are used as the data coordinates $\\vec{r}_i = (x_i,y_i)$. If the dataset has more dimensions in data coordinates, they must be passed as the first columns of the dataset, and the last column is always assumed to be corresponding $z_i$ values. The code below illustrates the case of data with three dimensions in data coordinates:
+The last column in `data` corresponds to $\\{z_i\\}_{i=1,\\dots,N}$ values, while the first two columns are used as the data coordinates $\\vec{r}_i = (x_i,y_i)$. If the dataset has more dimensions in data coordinates, they must be passed as the first columns of the dataset, and the last column is always assumed to correspond to $z_i$ values. The code below illustrates the case of data with three dimensions in data coordinates:
 
 .. code-block:: python
 
    import numpy as np
    from knnpe import knn_permutation_entropy
    
    data = np.random.normal(size=(100,4))
@@ -145,27 +130,32 @@
      The number of neighbors for constructing the k-nearest neighbor graph (default is 25).
  nthreads : int, optional
      The number of parallel threads for the computation (default is -1, which uses all available cores).
  hide_bar : bool, optional
      If True, the progress bar is not displayed (default is False).
  metrics : bool, optional
      If True, calculates graph density and largest component fraction (default is False).
+ complexity : bool, optional
+     If True, also calculates the knn permutation complexity.
 
 We provide a `notebook <https://github.com/hvribeiro/knnpe/blob/main/examples/knnpe.ipynb>`_
-illustrating how to use ``knnpe`` and further information we refer to the knnpe's `documentation <https://readthedocs.org/projects/knnpe/badge/?version=latest>`_
+illustrating how to use ``knnpe`` and further information we refer to the knnpe's `documentation <https://hvribeiro.github.io/knnpe/>`_
 
 Contributing
 ============
 
 Pull requests addressing errors or adding new functionalities are always welcome.
 
 References
 ==========
 
-.. [#voltarelli2024] L. G. J. M. Voltarelli, A. A. B. Pessa, L. Zunino, 
-   R. S. Zola, E. K. Lenzi, M. Perc, H. V. Ribeiro. Characterizing unstructured 
-   data with the nearest neighbor permutation entropy. ?, ? (2024).
-.. [#bandtpompe2002] C. Bandt, B. Pompe. Permutation entropy: A Natural 
-   Complexity Measure for Time Series. Physical Review Letters 88, 174102 (2002).
-.. [#ribeiro2012] H. V. Ribeiro, L. Zunino, E. K. Lenzi, P. A. Santoro, R. S.
-   Mendes. Complexity-Entropy Causality Plane as a Complexity
-   Measure for Two-Dimensional Patterns. PLOS ONE 7, e40689 (2012).
+.. [#voltarelli2024] L. G. J. M. Voltarelli, A. A. B. Pessa, L. Zunino, R. S. Zola, E. K. Lenzi, M. Perc, H. V. Ribeiro. 
+   Characterizing unstructured data with the nearest neighbor permutation entropy. 
+   arXiv, 2403.13122 (2024).
+
+.. [#bandtpompe2002] C. Bandt, B. Pompe. 
+   Permutation entropy: A Natural Complexity Measure for Time Series. 
+   Physical Review Letters 88, 174102 (2002).
+
+.. [#ribeiro2012] H. V. Ribeiro, L. Zunino, E. K. Lenzi, P. A. Santoro, R. S. Mendes.
+   Complexity-Entropy Causality Plane as a Complexity Measure for Two-Dimensional Patterns. 
+   PLOS ONE 7, e40689 (2012).
```

### Comparing `knnpe-0.1.1/pyproject.toml` & `knnpe-0.1.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "knnpe"
-version = "0.1.1"
+version = "0.1.2"
 authors = [{ name="Haroldo V. Ribeiro", email="hvr@dfi.uem.br" },]
 description = "A Python package for characterizing unstructured data with the nearest neighbor permutation entropy"
 readme = "README.rst"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
@@ -21,8 +21,8 @@
     "setuptools>=42",
     "numpy>=1.20",
     "scipy",
     "scikit-learn",
     "tqdm",
     "wheel"
 ]
-build-backend = "setuptools.build_meta"
+build-backend = "setuptools.build_meta"
```

### Comparing `knnpe-0.1.1/setup.cfg` & `knnpe-0.1.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = knnpe
-version = 0.1.1
+version = 0.1.2
 author = L. G. J. M. Voltarelli, A. A. B. Pessa, L. Zunino, R. S. Zola, E. K. Lenzi, M. Perc, H. V. Ribeiro
 author_email = hvr@uem.dfi.br
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 description = A Python package for characterizing unstructured data with the nearest neighbor permutation entropy
```

### Comparing `knnpe-0.1.1/setup.py` & `knnpe-0.1.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.rst", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="knnpe",
-    version="0.1.1",
+    version="0.1.2",
     author="L. G. J. M. Voltarelli, A. A. B. Pessa, L. Zunino, R. S. Zola, E. K. Lenzi, M. Perc, H. V. Ribeiro",
     author_email="hvr@dfi.uem.br",
     description="A Python package for characterizing unstructured data with the nearest neighbor permutation entropy",
     long_description=long_description,
     long_description_content_type="text/x-rst; charset=UTF-8",
     packages=find_packages(),
     classifiers=[
```


# Comparing `tmp/radtract-0.2.1.tar.gz` & `tmp/radtract-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "radtract-0.2.1.tar", last modified: Fri Jan  5 17:54:27 2024, max compression
+gzip compressed data, was "radtract-0.2.2.tar", last modified: Wed Apr 24 07:36:53 2024, max compression
```

## Comparing `radtract-0.2.1.tar` & `radtract-0.2.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxr-x   0 neher     (1000) neher     (1000)        0 2024-01-05 17:54:27.260432 radtract-0.2.1/
-drwxrwxr-x   0 neher     (1000) neher     (1000)        0 2024-01-05 17:54:27.220434 radtract-0.2.1/LICENSES/
--rw-rw-r--   0 neher     (1000) neher     (1000)    10280 2024-01-05 10:50:20.000000 radtract-0.2.1/LICENSES/Apache-2.0.txt
--rw-rw-r--   0 neher     (1000) neher     (1000)      154 2024-01-05 10:50:20.000000 radtract-0.2.1/MANIFEST.in
--rw-r--r--   0 neher     (1000) neher     (1000)    16385 2024-01-05 17:54:27.260432 radtract-0.2.1/PKG-INFO
--rw-rw-r--   0 neher     (1000) neher     (1000)     4581 2024-01-05 17:52:25.000000 radtract-0.2.1/README.md
--rw-rw-r--   0 neher     (1000) neher     (1000)     2039 2024-01-05 17:53:25.000000 radtract-0.2.1/pyproject.toml
-drwxrwxr-x   0 neher     (1000) neher     (1000)        0 2024-01-05 17:54:27.260432 radtract-0.2.1/radtract/
--rw-rw-r--   0 neher     (1000) neher     (1000)      357 2024-01-05 17:53:21.000000 radtract-0.2.1/radtract/__init__.py
--rw-rw-r--   0 neher     (1000) neher     (1000)    20307 2024-01-05 12:57:55.000000 radtract-0.2.1/radtract/features.py
--rw-rw-r--   0 neher     (1000) neher     (1000)    37601 2024-01-05 10:50:20.000000 radtract-0.2.1/radtract/parcellation.py
--rw-rw-r--   0 neher     (1000) neher     (1000)     7498 2024-01-05 13:15:53.000000 radtract-0.2.1/radtract/prediction.py
--rw-rw-r--   0 neher     (1000) neher     (1000)     3626 2024-01-05 10:50:20.000000 radtract-0.2.1/radtract/pyrad.yaml
--rw-rw-r--   0 neher     (1000) neher     (1000)     3634 2024-01-05 10:50:20.000000 radtract-0.2.1/radtract/pyrad_D.yaml
--rw-rw-r--   0 neher     (1000) neher     (1000)     3570 2024-01-05 10:50:20.000000 radtract-0.2.1/radtract/pyrad_nofilter.yaml
--rw-rw-r--   0 neher     (1000) neher     (1000)     3578 2024-01-05 10:50:20.000000 radtract-0.2.1/radtract/pyrad_nofilter_D.yaml
--rw-rw-r--   0 neher     (1000) neher     (1000)     8999 2024-01-05 10:50:20.000000 radtract-0.2.1/radtract/tractdensity.py
--rw-rw-r--   0 neher     (1000) neher     (1000)    19552 2024-01-05 10:50:20.000000 radtract-0.2.1/radtract/tractfiltering.py
--rw-rw-r--   0 neher     (1000) neher     (1000)    13528 2024-01-05 10:50:20.000000 radtract-0.2.1/radtract/utils.py
-drwxrwxr-x   0 neher     (1000) neher     (1000)        0 2024-01-05 17:54:27.260432 radtract-0.2.1/radtract.egg-info/
--rw-r--r--   0 neher     (1000) neher     (1000)    16385 2024-01-05 17:54:27.000000 radtract-0.2.1/radtract.egg-info/PKG-INFO
--rw-rw-r--   0 neher     (1000) neher     (1000)      539 2024-01-05 17:54:27.000000 radtract-0.2.1/radtract.egg-info/SOURCES.txt
--rw-rw-r--   0 neher     (1000) neher     (1000)        1 2024-01-05 17:54:27.000000 radtract-0.2.1/radtract.egg-info/dependency_links.txt
--rw-rw-r--   0 neher     (1000) neher     (1000)      701 2024-01-05 17:54:27.000000 radtract-0.2.1/radtract.egg-info/entry_points.txt
--rw-rw-r--   0 neher     (1000) neher     (1000)      131 2024-01-05 17:54:27.000000 radtract-0.2.1/radtract.egg-info/requires.txt
--rw-rw-r--   0 neher     (1000) neher     (1000)        9 2024-01-05 17:54:27.000000 radtract-0.2.1/radtract.egg-info/top_level.txt
--rw-rw-r--   0 neher     (1000) neher     (1000)       38 2024-01-05 17:54:27.260432 radtract-0.2.1/setup.cfg
-drwxrwxr-x   0 neher     (1000) neher     (1000)        0 2024-01-05 17:54:27.260432 radtract-0.2.1/tests/
--rw-rw-r--   0 neher     (1000) neher     (1000)     5914 2024-01-05 15:10:26.000000 radtract-0.2.1/tests/test_radtract.py
+drwxrwxr-x   0 neher     (1000) neher     (1000)        0 2024-04-24 07:36:53.721283 radtract-0.2.2/
+drwxrwxr-x   0 neher     (1000) neher     (1000)        0 2024-04-24 07:36:53.721283 radtract-0.2.2/LICENSES/
+-rw-rw-r--   0 neher     (1000) neher     (1000)    10280 2024-04-24 07:27:54.000000 radtract-0.2.2/LICENSES/Apache-2.0.txt
+-rw-rw-r--   0 neher     (1000) neher     (1000)      154 2024-04-24 07:27:54.000000 radtract-0.2.2/MANIFEST.in
+-rw-r--r--   0 neher     (1000) neher     (1000)    17045 2024-04-24 07:36:53.721283 radtract-0.2.2/PKG-INFO
+-rw-rw-r--   0 neher     (1000) neher     (1000)     5241 2024-04-24 07:27:54.000000 radtract-0.2.2/README.md
+-rw-rw-r--   0 neher     (1000) neher     (1000)     2039 2024-04-24 07:31:42.000000 radtract-0.2.2/pyproject.toml
+drwxrwxr-x   0 neher     (1000) neher     (1000)        0 2024-04-24 07:36:53.721283 radtract-0.2.2/radtract/
+-rw-rw-r--   0 neher     (1000) neher     (1000)      357 2024-04-24 07:31:27.000000 radtract-0.2.2/radtract/__init__.py
+-rw-rw-r--   0 neher     (1000) neher     (1000)    20501 2024-04-24 07:34:04.000000 radtract-0.2.2/radtract/features.py
+-rw-rw-r--   0 neher     (1000) neher     (1000)    38105 2024-04-24 07:29:36.000000 radtract-0.2.2/radtract/parcellation.py
+-rw-rw-r--   0 neher     (1000) neher     (1000)     7498 2024-04-24 07:27:54.000000 radtract-0.2.2/radtract/prediction.py
+-rw-rw-r--   0 neher     (1000) neher     (1000)     3626 2024-04-24 07:27:54.000000 radtract-0.2.2/radtract/pyrad.yaml
+-rw-rw-r--   0 neher     (1000) neher     (1000)     3634 2024-04-24 07:27:54.000000 radtract-0.2.2/radtract/pyrad_D.yaml
+-rw-rw-r--   0 neher     (1000) neher     (1000)     3570 2024-04-24 07:27:54.000000 radtract-0.2.2/radtract/pyrad_nofilter.yaml
+-rw-rw-r--   0 neher     (1000) neher     (1000)     3578 2024-04-24 07:27:54.000000 radtract-0.2.2/radtract/pyrad_nofilter_D.yaml
+-rw-rw-r--   0 neher     (1000) neher     (1000)     8999 2024-04-24 07:27:54.000000 radtract-0.2.2/radtract/tractdensity.py
+-rw-rw-r--   0 neher     (1000) neher     (1000)    19552 2024-04-24 07:27:54.000000 radtract-0.2.2/radtract/tractfiltering.py
+-rw-rw-r--   0 neher     (1000) neher     (1000)    13565 2024-04-24 07:28:26.000000 radtract-0.2.2/radtract/utils.py
+drwxrwxr-x   0 neher     (1000) neher     (1000)        0 2024-04-24 07:36:53.721283 radtract-0.2.2/radtract.egg-info/
+-rw-r--r--   0 neher     (1000) neher     (1000)    17045 2024-04-24 07:36:53.000000 radtract-0.2.2/radtract.egg-info/PKG-INFO
+-rw-rw-r--   0 neher     (1000) neher     (1000)      539 2024-04-24 07:36:53.000000 radtract-0.2.2/radtract.egg-info/SOURCES.txt
+-rw-rw-r--   0 neher     (1000) neher     (1000)        1 2024-04-24 07:36:53.000000 radtract-0.2.2/radtract.egg-info/dependency_links.txt
+-rw-rw-r--   0 neher     (1000) neher     (1000)      701 2024-04-24 07:36:53.000000 radtract-0.2.2/radtract.egg-info/entry_points.txt
+-rw-rw-r--   0 neher     (1000) neher     (1000)      131 2024-04-24 07:36:53.000000 radtract-0.2.2/radtract.egg-info/requires.txt
+-rw-rw-r--   0 neher     (1000) neher     (1000)        9 2024-04-24 07:36:53.000000 radtract-0.2.2/radtract.egg-info/top_level.txt
+-rw-rw-r--   0 neher     (1000) neher     (1000)       38 2024-04-24 07:36:53.721283 radtract-0.2.2/setup.cfg
+drwxrwxr-x   0 neher     (1000) neher     (1000)        0 2024-04-24 07:36:53.721283 radtract-0.2.2/tests/
+-rw-rw-r--   0 neher     (1000) neher     (1000)     6216 2024-04-24 07:27:54.000000 radtract-0.2.2/tests/test_radtract.py
```

### Comparing `radtract-0.2.1/LICENSES/Apache-2.0.txt` & `radtract-0.2.2/LICENSES/Apache-2.0.txt`

 * *Files identical despite different names*

### Comparing `radtract-0.2.1/PKG-INFO` & `radtract-0.2.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: radtract
-Version: 0.2.1
+Version: 0.2.2
 Summary: Radiomic Tractometry for advanced along-tract analysis of diffusion-weighted MRI
 Author-email: Peter Neher <p.neher@dkfz-heidelberg.de>
 Maintainer-email: Peter Neher <p.neher@dkfz-heidelberg.de>
 License: Apache License
         Version 2.0, January 2004
         http://www.apache.org/licenses/
         
@@ -110,32 +110,31 @@
 Copyright © German Cancer Research Center (DKFZ), [Division of Medical Image Computing (MIC)](https://www.dkfz.de/en/mic/index.php). Please make sure that your usage of this code is in compliance with the code [license](https://github.com/MIC-DKFZ/radtract/blob/master/LICENSE).
 
 If you use RadTract, please cite our [paper](https://www.nature.com/articles/s41467-023-44591-3): `Neher, P., Hirjak, D. & Maier-Hein, K. Radiomic tractometry reveals tract-specific imaging biomarkers in white matter. Nat Commun 15, 303 (2024). https://doi.org/10.1038/s41467-023-44591-3`
 
 
 ## Overview
 
-Python package for radiomic tractometry (RadTract). RadTract is a tool designed for tract-specific microstructural analysis of the brain’s white matter using diffusion MRI. It enhances traditional tractometry, which often misses valuable information due to its reliance on summary statistics and scalar values.
-
-RadTract incorporates radiomics, a method that analyzes a multitude of quantitative image features beyond visual perception, into tractometry. This integration allows for improved predictive modeling while maintaining the localization capability of tractometry.
+RadTract is a python implementation of radiomic tractometry or "Tractomics". It is designed for tract-specific microstructural analysis of the brain’s white matter using diffusion MRI. It enhances traditional tractometry, which often misses valuable information due to its reliance on bare summary statistics and scalar values. RadTract incorporates radiomics, a method that analyzes a multitude of quantitative image features beyond visual perception, into tractometry. This integration allows for improved predictive modeling while maintaining the localization capability of tractometry.
 
 RadTract has demonstrated its effectiveness in diagnosing disease subgroups across various datasets and estimating demographic and clinical parameters in multiple clinical populations. It holds the potential to pioneer a new generation of tract-specific imaging biomarkers, benefiting a wide range of applications from basic neuroscience to medical research.
 
 For details about the approach, please refer to our [paper](https://www.nature.com/articles/s41467-023-44591-3): `Neher, P., Hirjak, D. & Maier-Hein, K. Radiomic tractometry reveals tract-specific imaging biomarkers in white matter. Nat Commun 15, 303 (2024). https://doi.org/10.1038/s41467-023-44591-3`. An overview of the method is shown in Figure 1.
 
-a multitude![](resources/radtract_overview.png)_Figure 1: Illustration of the complete RadTract process. The points of a statically resampled tract (a) can be seen as samples of partly overlapping classes that are not linearly separable. We are aiming at finding the hyperplanes, superimposed as white lines on the tract in (a), that optimally separate the classes with the smallest amount of errors. This task can be solved using large-margin classifiers such as SVMs. This enables us to create parcellations directly in voxel-space (b) that do not suffer from projection-induced misassignments, as is the case in the centerline-based approach (d). For visualization purposes, the tract parcellation in voxel-space is projected back on the original streamlines (e). The proposed tract parcellation in voxel-space (b) is used to calculate a multitude of radiomics features per parcel, visualized in (c). Exemplary feature classes and image filters available when using [pyradiomics](https://pyradiomics.readthedocs.io/en/latest/) as calculation engine are listed in (f). RadTract currently supports [MIRP](https://github.com/oncoray/mirp) as an alternative engine for calculating radiomics features.
+![](resources/radtract_overview.png)_Figure 1: Illustration of the complete RadTract process. The points of a statically resampled tract (a) can be seen as samples of partly overlapping classes that are not linearly separable. We are aiming at finding the hyperplanes, superimposed as white lines on the tract in (a), that optimally separate the classes with the smallest amount of errors. This task can be solved using large-margin classifiers such as SVMs. This enables us to create parcellations directly in voxel-space (b) that do not suffer from projection-induced misassignments, as is the case in the centerline-based approach (d). For visualization purposes, the tract parcellation in voxel-space is projected back on the original streamlines (e). The proposed tract parcellation in voxel-space (b) is used to calculate a multitude of radiomics features per parcel, visualized in (c). Exemplary feature classes and image filters available when using [pyradiomics](https://pyradiomics.readthedocs.io/en/latest/) as calculation engine are listed in (f). RadTract currently supports [MIRP](https://github.com/oncoray/mirp) as an alternative engine for calculating radiomics features.
 
 ## Installation
 
 ### Requirements
 
 - No specific hardware requirements. A state-of-the-art desktop computer should be sufficient.
 - Tested on Ubuntu 22.04 but should run on other systems as well.
 - Tested with Python 3.8 and higher
-- Numpy should be installed prior to the RadTract setup, all other dependencies will be installed automatically. 
+- Numpy should be installed prior to the RadTract setup (pyradiomics requirement), all other dependencies will be installed automatically. 
+- Should the pyradiomics setup fail with a missing numpy error despite installed numpy, see section "Pyradiomics installation issues" below.
 - It is recommended to use a virtual environment for the installation. 
 
 See `.gitlab-ci.yml` for the currently tested configurations.
 
 ### Installation
 
 Installation via anaconda is not supported currently!
@@ -145,14 +144,23 @@
    - Activate the virtual environment: `source myvenv/bin/activate`
 2. Installation
    - Install from source: navigate to the root directory of RadTract and run `pip install .`
    - Install from PyPI: run `pip install radtract`
 
 Installation should complete within a few seconds.
 
+### Pyradiomics installation issues
+
+If the pyradiomics installation fails with a missing numpy error despite numpy being installed, a workaround is to install pyradimics directly from source:
+
+1. Checkout the pyradiomics repo: `git clone git://github.com/Radiomics/pyradiomics`
+2. Activate your virtual environment (if you use one): `source myvenv/bin/activate`
+3. Navigate to the pyradiomics source and install from there: `pip install .`
+4. Then run pip `pip install radtract` again.
+
 ## Examples
 
 A complete pipeline example can be found in [example.ipynb](https://github.com/MIC-DKFZ/radtract/blob/main/example.ipynb). 
 
 Further examples can be found in the RadTract test script `tests\test_radtract.py`. Test data is included in `tests\test_data`.
```

### Comparing `radtract-0.2.1/README.md` & `radtract-0.2.2/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -9,32 +9,31 @@
 Copyright © German Cancer Research Center (DKFZ), [Division of Medical Image Computing (MIC)](https://www.dkfz.de/en/mic/index.php). Please make sure that your usage of this code is in compliance with the code [license](https://github.com/MIC-DKFZ/radtract/blob/master/LICENSE).
 
 If you use RadTract, please cite our [paper](https://www.nature.com/articles/s41467-023-44591-3): `Neher, P., Hirjak, D. & Maier-Hein, K. Radiomic tractometry reveals tract-specific imaging biomarkers in white matter. Nat Commun 15, 303 (2024). https://doi.org/10.1038/s41467-023-44591-3`
 
 
 ## Overview
 
-Python package for radiomic tractometry (RadTract). RadTract is a tool designed for tract-specific microstructural analysis of the brain’s white matter using diffusion MRI. It enhances traditional tractometry, which often misses valuable information due to its reliance on summary statistics and scalar values.
-
-RadTract incorporates radiomics, a method that analyzes a multitude of quantitative image features beyond visual perception, into tractometry. This integration allows for improved predictive modeling while maintaining the localization capability of tractometry.
+RadTract is a python implementation of radiomic tractometry or "Tractomics". It is designed for tract-specific microstructural analysis of the brain’s white matter using diffusion MRI. It enhances traditional tractometry, which often misses valuable information due to its reliance on bare summary statistics and scalar values. RadTract incorporates radiomics, a method that analyzes a multitude of quantitative image features beyond visual perception, into tractometry. This integration allows for improved predictive modeling while maintaining the localization capability of tractometry.
 
 RadTract has demonstrated its effectiveness in diagnosing disease subgroups across various datasets and estimating demographic and clinical parameters in multiple clinical populations. It holds the potential to pioneer a new generation of tract-specific imaging biomarkers, benefiting a wide range of applications from basic neuroscience to medical research.
 
 For details about the approach, please refer to our [paper](https://www.nature.com/articles/s41467-023-44591-3): `Neher, P., Hirjak, D. & Maier-Hein, K. Radiomic tractometry reveals tract-specific imaging biomarkers in white matter. Nat Commun 15, 303 (2024). https://doi.org/10.1038/s41467-023-44591-3`. An overview of the method is shown in Figure 1.
 
-a multitude![](resources/radtract_overview.png)_Figure 1: Illustration of the complete RadTract process. The points of a statically resampled tract (a) can be seen as samples of partly overlapping classes that are not linearly separable. We are aiming at finding the hyperplanes, superimposed as white lines on the tract in (a), that optimally separate the classes with the smallest amount of errors. This task can be solved using large-margin classifiers such as SVMs. This enables us to create parcellations directly in voxel-space (b) that do not suffer from projection-induced misassignments, as is the case in the centerline-based approach (d). For visualization purposes, the tract parcellation in voxel-space is projected back on the original streamlines (e). The proposed tract parcellation in voxel-space (b) is used to calculate a multitude of radiomics features per parcel, visualized in (c). Exemplary feature classes and image filters available when using [pyradiomics](https://pyradiomics.readthedocs.io/en/latest/) as calculation engine are listed in (f). RadTract currently supports [MIRP](https://github.com/oncoray/mirp) as an alternative engine for calculating radiomics features.
+![](resources/radtract_overview.png)_Figure 1: Illustration of the complete RadTract process. The points of a statically resampled tract (a) can be seen as samples of partly overlapping classes that are not linearly separable. We are aiming at finding the hyperplanes, superimposed as white lines on the tract in (a), that optimally separate the classes with the smallest amount of errors. This task can be solved using large-margin classifiers such as SVMs. This enables us to create parcellations directly in voxel-space (b) that do not suffer from projection-induced misassignments, as is the case in the centerline-based approach (d). For visualization purposes, the tract parcellation in voxel-space is projected back on the original streamlines (e). The proposed tract parcellation in voxel-space (b) is used to calculate a multitude of radiomics features per parcel, visualized in (c). Exemplary feature classes and image filters available when using [pyradiomics](https://pyradiomics.readthedocs.io/en/latest/) as calculation engine are listed in (f). RadTract currently supports [MIRP](https://github.com/oncoray/mirp) as an alternative engine for calculating radiomics features.
 
 ## Installation
 
 ### Requirements
 
 - No specific hardware requirements. A state-of-the-art desktop computer should be sufficient.
 - Tested on Ubuntu 22.04 but should run on other systems as well.
 - Tested with Python 3.8 and higher
-- Numpy should be installed prior to the RadTract setup, all other dependencies will be installed automatically. 
+- Numpy should be installed prior to the RadTract setup (pyradiomics requirement), all other dependencies will be installed automatically. 
+- Should the pyradiomics setup fail with a missing numpy error despite installed numpy, see section "Pyradiomics installation issues" below.
 - It is recommended to use a virtual environment for the installation. 
 
 See `.gitlab-ci.yml` for the currently tested configurations.
 
 ### Installation
 
 Installation via anaconda is not supported currently!
@@ -44,14 +43,23 @@
    - Activate the virtual environment: `source myvenv/bin/activate`
 2. Installation
    - Install from source: navigate to the root directory of RadTract and run `pip install .`
    - Install from PyPI: run `pip install radtract`
 
 Installation should complete within a few seconds.
 
+### Pyradiomics installation issues
+
+If the pyradiomics installation fails with a missing numpy error despite numpy being installed, a workaround is to install pyradimics directly from source:
+
+1. Checkout the pyradiomics repo: `git clone git://github.com/Radiomics/pyradiomics`
+2. Activate your virtual environment (if you use one): `source myvenv/bin/activate`
+3. Navigate to the pyradiomics source and install from there: `pip install .`
+4. Then run pip `pip install radtract` again.
+
 ## Examples
 
 A complete pipeline example can be found in [example.ipynb](https://github.com/MIC-DKFZ/radtract/blob/main/example.ipynb). 
 
 Further examples can be found in the RadTract test script `tests\test_radtract.py`. Test data is included in `tests\test_data`.
```

### Comparing `radtract-0.2.1/pyproject.toml` & `radtract-0.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "radtract"
-version = "0.2.1"
+version = "0.2.2"
 authors = [
   { name="Peter Neher", email="p.neher@dkfz-heidelberg.de" },
 ]
 maintainers = [
   { name="Peter Neher", email="p.neher@dkfz-heidelberg.de" },
 ]
```

### Comparing `radtract-0.2.1/radtract/features.py` & `radtract-0.2.2/radtract/features.py`

 * *Files 1% similar despite different names*

```diff
@@ -266,20 +266,23 @@
             if self.num_parcels is not None:
                 assert self.num_parcels == len(labels) - 1, 'Number of parcels does not match number of labels in ' + parcellation_file_name
 
             # to-do: get global features
                 
 
             # get features for each label
+            np.random.seed(0)
+            print('RANDOM SEED SET TO 0 FOR MIRP')
+            print('\033[91mWARNING: MIRP is automatically normalizing inside the mask. This is aknown issue and has to be fixed.\033[0m')
             mirp_output = mirp.extract_features(image=parameter_map_file_name, 
                                             mask=parcellation_file_name, 
                                             base_discretisation_method="fixed_bin_number", 
                                             base_discretisation_n_bins=32, 
-                                            export_features=True, 
-                                            num_cpus=16)
+                                            export_features=True)
+            np.random.seed(None)
             mirp_output = mirp_output[0]
 
             # drop column 'sample_name'
             mirp_output = mirp_output.drop(columns=['sample_name'])
 
             # drop all columns where column name starts with 'image_'
             mirp_output = mirp_output.loc[:, ~mirp_output.columns.str.startswith('image_')]
```

### Comparing `radtract-0.2.1/radtract/parcellation.py` & `radtract-0.2.2/radtract/parcellation.py`

 * *Files 1% similar despite different names*

```diff
@@ -319,14 +319,16 @@
             print('Creating binary envelope from start region')
             binary_envelope = tract_envelope(streamlines, start_region)
             auto_envelope = True
         elif type(reference_image) is nib.Nifti1Image:
             print('Creating binary envelope from reference image')
             binary_envelope = tract_envelope(streamlines, reference_image)
             auto_envelope = True
+        else:
+            raise Exception('No binary envelope provided and no start region or reference image set for automatic envelope calculation.')
     else:
         print('Using provided binary envelope')
 
     if type(streamlines) is not nib.streamlines.array_sequence.ArraySequence:
         raise Exception('Streamlines must be in dipy format!')
     if type(binary_envelope) is not nib.Nifti1Image:
         raise Exception('Binary envelope must be Nifti1Image!')
@@ -379,14 +381,15 @@
     if max(envelope_data.shape)//2 <= num_parcels and not streamline_space:
         print('\033[91mWARNING: num_parcels is high in comparison to the image size. Consider a lower number of parcels for a voxel-space tract parcellation.\033[0m')
 
     # define outputs
     reduced_streamlines = None
     svc = None
     streamline_point_parcels = None
+    train_data_point_parcels = None
     colors = None
 
     if num_parcels > 1 and parcellation_type == 'hyperplane':
         print('Reducing input bundle')
         threshold = 20
         num_centroids = 0
         reduced_streamlines = None
@@ -402,14 +405,18 @@
 
         samples = []
         classes = []
         for s in reduced_streamlines:
             samples += s.tolist()
             classes += np.arange(1, len(s) + 1, 1).tolist()
 
+        train_data_point_parcels = dict()
+        train_data_point_parcels['points'] = samples
+        train_data_point_parcels['parcels'] = classes
+
         samples = np.array(samples)
         classes = np.array(classes)
 
         print('Fitting parcellation model to ' + str(len(classes)) + ' points')
         svc = SVC(C=1, kernel='rbf')
         svc.fit(X=samples, y=classes)
 
@@ -651,14 +658,17 @@
                 color = lut_cmap[p-1]*255.0
                 color = np.append(color, 255.0)
                 colors.append(color)
 
 
     if save_intermediate_files:
 
+        if train_data_point_parcels is not None:
+            joblib.dump(train_data_point_parcels, out_parcellation_filename.replace('.nii.gz', '_train_data.pkl'))
+
         if envelope_data is not None:
             new_envelope_data = np.zeros(envelope_data.shape, dtype='uint8')
             new_envelope_data[np.where(envelope_data > 0)] = 1
             new_envelope = nib.Nifti1Image(new_envelope_data, affine=binary_envelope.affine)
             nib.save(new_envelope, out_parcellation_filename.replace('.nii.gz', '_envelope.nii.gz'))
 
         if reference_streamline is not None:
@@ -759,7 +769,8 @@
                      fast_mode=args.fast_mode,
                      resample=args.resample,
                      out_parcellation_filename=args.output)
 
 
 if __name__ == '__main__':
     main()
+
```

### Comparing `radtract-0.2.1/radtract/prediction.py` & `radtract-0.2.2/radtract/prediction.py`

 * *Files identical despite different names*

### Comparing `radtract-0.2.1/radtract/pyrad.yaml` & `radtract-0.2.2/radtract/pyrad.yaml`

 * *Files identical despite different names*

### Comparing `radtract-0.2.1/radtract/pyrad_D.yaml` & `radtract-0.2.2/radtract/pyrad_D.yaml`

 * *Files identical despite different names*

### Comparing `radtract-0.2.1/radtract/pyrad_nofilter.yaml` & `radtract-0.2.2/radtract/pyrad_nofilter.yaml`

 * *Files identical despite different names*

### Comparing `radtract-0.2.1/radtract/pyrad_nofilter_D.yaml` & `radtract-0.2.2/radtract/pyrad_nofilter_D.yaml`

 * *Files identical despite different names*

### Comparing `radtract-0.2.1/radtract/tractdensity.py` & `radtract-0.2.2/radtract/tractdensity.py`

 * *Files identical despite different names*

### Comparing `radtract-0.2.1/radtract/tractfiltering.py` & `radtract-0.2.2/radtract/tractfiltering.py`

 * *Files identical despite different names*

### Comparing `radtract-0.2.1/radtract/utils.py` & `radtract-0.2.2/radtract/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -197,15 +197,15 @@
     """
     for i in range(3):
         if index[i] < 0 or index[i] > image.shape[i] - 1:
             return False
     return True
 
 
-def point_label_file_to_mitkpointset(point_label_file, out_path, streamline_files = []):
+def point_label_file_to_mitkpointset(point_label_file, out_path, streamline_files = [], point_size=1.0):
     """
     Converts a point label file to a scene file of mitk pointsets. This is useful to visualize the streamline points with labels as point clouds in MITK Diffusion (https://github.com/MIC-DKFZ/MITK-Diffusion/).
     :param point_label_file: path to point label file
     :param out_path: output path
     :param streamline_files: list of streamline files to include in the mitk scene file
     :return:
     """
@@ -301,15 +301,15 @@
 
         color = lut_cmap[parcel-1]
 
         # write props2
         text = '<?xml version="1.0" encoding="UTF-8"?>'
         text += '<Version Writer="/home/neher/coding/mitk/mitk/Modules/SceneSerializationBase/src/mitkPropertyListSerializer.cpp" Revision="$Revision: 17055 $" FileVersion="1"/>'
         text += '<property key="pointsize" type="FloatProperty">'
-        text += '<float value="0.5"/>'
+        text += '<float value="' + str(point_size) + '"/>'
         text += '</property>'
         text += '<property key="color" type="ColorProperty">'
         text += '<color r="' + str(color[0]) + '" g="' + str(color[1]) + '" b="' + str(color[2]) + '"/>'
         text += '</property>'
         text += '<property key="name" type="StringProperty">'
         text += '<string value="P' + str(parcel) + '"/>'
         text += '</property>'
@@ -353,7 +353,8 @@
 
 def main():
     pass
 
 
 if __name__ == '__main__':
     main()
+
```

### Comparing `radtract-0.2.1/radtract.egg-info/PKG-INFO` & `radtract-0.2.2/radtract.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: radtract
-Version: 0.2.1
+Version: 0.2.2
 Summary: Radiomic Tractometry for advanced along-tract analysis of diffusion-weighted MRI
 Author-email: Peter Neher <p.neher@dkfz-heidelberg.de>
 Maintainer-email: Peter Neher <p.neher@dkfz-heidelberg.de>
 License: Apache License
         Version 2.0, January 2004
         http://www.apache.org/licenses/
         
@@ -110,32 +110,31 @@
 Copyright © German Cancer Research Center (DKFZ), [Division of Medical Image Computing (MIC)](https://www.dkfz.de/en/mic/index.php). Please make sure that your usage of this code is in compliance with the code [license](https://github.com/MIC-DKFZ/radtract/blob/master/LICENSE).
 
 If you use RadTract, please cite our [paper](https://www.nature.com/articles/s41467-023-44591-3): `Neher, P., Hirjak, D. & Maier-Hein, K. Radiomic tractometry reveals tract-specific imaging biomarkers in white matter. Nat Commun 15, 303 (2024). https://doi.org/10.1038/s41467-023-44591-3`
 
 
 ## Overview
 
-Python package for radiomic tractometry (RadTract). RadTract is a tool designed for tract-specific microstructural analysis of the brain’s white matter using diffusion MRI. It enhances traditional tractometry, which often misses valuable information due to its reliance on summary statistics and scalar values.
-
-RadTract incorporates radiomics, a method that analyzes a multitude of quantitative image features beyond visual perception, into tractometry. This integration allows for improved predictive modeling while maintaining the localization capability of tractometry.
+RadTract is a python implementation of radiomic tractometry or "Tractomics". It is designed for tract-specific microstructural analysis of the brain’s white matter using diffusion MRI. It enhances traditional tractometry, which often misses valuable information due to its reliance on bare summary statistics and scalar values. RadTract incorporates radiomics, a method that analyzes a multitude of quantitative image features beyond visual perception, into tractometry. This integration allows for improved predictive modeling while maintaining the localization capability of tractometry.
 
 RadTract has demonstrated its effectiveness in diagnosing disease subgroups across various datasets and estimating demographic and clinical parameters in multiple clinical populations. It holds the potential to pioneer a new generation of tract-specific imaging biomarkers, benefiting a wide range of applications from basic neuroscience to medical research.
 
 For details about the approach, please refer to our [paper](https://www.nature.com/articles/s41467-023-44591-3): `Neher, P., Hirjak, D. & Maier-Hein, K. Radiomic tractometry reveals tract-specific imaging biomarkers in white matter. Nat Commun 15, 303 (2024). https://doi.org/10.1038/s41467-023-44591-3`. An overview of the method is shown in Figure 1.
 
-a multitude![](resources/radtract_overview.png)_Figure 1: Illustration of the complete RadTract process. The points of a statically resampled tract (a) can be seen as samples of partly overlapping classes that are not linearly separable. We are aiming at finding the hyperplanes, superimposed as white lines on the tract in (a), that optimally separate the classes with the smallest amount of errors. This task can be solved using large-margin classifiers such as SVMs. This enables us to create parcellations directly in voxel-space (b) that do not suffer from projection-induced misassignments, as is the case in the centerline-based approach (d). For visualization purposes, the tract parcellation in voxel-space is projected back on the original streamlines (e). The proposed tract parcellation in voxel-space (b) is used to calculate a multitude of radiomics features per parcel, visualized in (c). Exemplary feature classes and image filters available when using [pyradiomics](https://pyradiomics.readthedocs.io/en/latest/) as calculation engine are listed in (f). RadTract currently supports [MIRP](https://github.com/oncoray/mirp) as an alternative engine for calculating radiomics features.
+![](resources/radtract_overview.png)_Figure 1: Illustration of the complete RadTract process. The points of a statically resampled tract (a) can be seen as samples of partly overlapping classes that are not linearly separable. We are aiming at finding the hyperplanes, superimposed as white lines on the tract in (a), that optimally separate the classes with the smallest amount of errors. This task can be solved using large-margin classifiers such as SVMs. This enables us to create parcellations directly in voxel-space (b) that do not suffer from projection-induced misassignments, as is the case in the centerline-based approach (d). For visualization purposes, the tract parcellation in voxel-space is projected back on the original streamlines (e). The proposed tract parcellation in voxel-space (b) is used to calculate a multitude of radiomics features per parcel, visualized in (c). Exemplary feature classes and image filters available when using [pyradiomics](https://pyradiomics.readthedocs.io/en/latest/) as calculation engine are listed in (f). RadTract currently supports [MIRP](https://github.com/oncoray/mirp) as an alternative engine for calculating radiomics features.
 
 ## Installation
 
 ### Requirements
 
 - No specific hardware requirements. A state-of-the-art desktop computer should be sufficient.
 - Tested on Ubuntu 22.04 but should run on other systems as well.
 - Tested with Python 3.8 and higher
-- Numpy should be installed prior to the RadTract setup, all other dependencies will be installed automatically. 
+- Numpy should be installed prior to the RadTract setup (pyradiomics requirement), all other dependencies will be installed automatically. 
+- Should the pyradiomics setup fail with a missing numpy error despite installed numpy, see section "Pyradiomics installation issues" below.
 - It is recommended to use a virtual environment for the installation. 
 
 See `.gitlab-ci.yml` for the currently tested configurations.
 
 ### Installation
 
 Installation via anaconda is not supported currently!
@@ -145,14 +144,23 @@
    - Activate the virtual environment: `source myvenv/bin/activate`
 2. Installation
    - Install from source: navigate to the root directory of RadTract and run `pip install .`
    - Install from PyPI: run `pip install radtract`
 
 Installation should complete within a few seconds.
 
+### Pyradiomics installation issues
+
+If the pyradiomics installation fails with a missing numpy error despite numpy being installed, a workaround is to install pyradimics directly from source:
+
+1. Checkout the pyradiomics repo: `git clone git://github.com/Radiomics/pyradiomics`
+2. Activate your virtual environment (if you use one): `source myvenv/bin/activate`
+3. Navigate to the pyradiomics source and install from there: `pip install .`
+4. Then run pip `pip install radtract` again.
+
 ## Examples
 
 A complete pipeline example can be found in [example.ipynb](https://github.com/MIC-DKFZ/radtract/blob/main/example.ipynb). 
 
 Further examples can be found in the RadTract test script `tests\test_radtract.py`. Test data is included in `tests\test_data`.
```

### Comparing `radtract-0.2.1/radtract.egg-info/SOURCES.txt` & `radtract-0.2.2/radtract.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `radtract-0.2.1/radtract.egg-info/entry_points.txt` & `radtract-0.2.2/radtract.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `radtract-0.2.1/tests/test_radtract.py` & `radtract-0.2.2/tests/test_radtract.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 # SPDX-License-Identifier: Apache-2.0
 
 import numpy as np
 import pandas as pd
 from radtract import parcellation, features, tractdensity
 import nibabel as nib
 import os
+import sys
 
 
 def load_data():
     data_folder = os.path.dirname(__file__) + '/test_data/'
     beginnings = nib.load(data_folder + 'test_tract_b.nii.gz')
     envelope = nib.load(data_folder + 'test_tract_envelope.nii.gz')
     centerline_parcellation = nib.load(data_folder + 'centerline_parcellation.nii.gz')
@@ -62,51 +63,56 @@
                                             reference_image=beginnings,
                                             num_voxels=5)
     assert num == 18, 'num parcel estimation test 1 failed'
 
 
 def test_pyradiomics_features():
     data_folder = os.path.dirname(__file__) + '/test_data/'
-    features_df = pd.read_pickle(data_folder + 'hyperplane_features.pkl')
+    features_df = pd.read_pickle(data_folder + 'pyrad_features.pkl')
     pyrad_extractor = features.PyradiomicsExtractor(num_parcels=17)
     new_features = pyrad_extractor.calc_features(parcellation_file_name=data_folder + 'hyperplane_parcellation.nii.gz',
                                                  parameter_map_file_name=data_folder + 'test_map.nii.gz'
                                                 )
     # remove path from 'map' and 'parcellation' columns
     new_features['map'] = new_features['map'].str.split('/').str[-1]
     new_features['parcellation'] = new_features['parcellation'].str.split('/').str[-1]
-    new_features.to_pickle(get_results_path() + 'hyperplane_features.pkl')
+    new_features.to_pickle(get_results_path() + 'pyrad_features.pkl')
 
     # drop 'extractor_version' and 'radtract_version' columns
     new_features = new_features.drop(columns=['extractor_version', 'radtract_version'])
     features_df = features_df.drop(columns=['extractor_version', 'radtract_version'])
 
-    # print pandas version
-    print('pandas version', pd.__version__)
-    print(new_features.equals(features_df))
-
-    # print first three rows of both dataframes, only values
-    print(new_features.head(3))
-    print(features_df.head(3))
-
     tmp1 = new_features.drop(columns=['value'])
     tmp2 = features_df.drop(columns=['value'])
     pd.testing.assert_frame_equal(tmp1, tmp2, check_dtype=False)
     
     i = 0
     for el1, el2 in zip(new_features['value'], features_df['value']):
         dpercent = abs(1.0 - el1 / el2)
-        assert dpercent < 1.0e-5, 'value ' + str(i) + ', ' + str(i) + ' differs by ' + str(dpercent) + ' from reference'
+        assert dpercent < 1.0e-5, 'value ' + str(i) + ' differs by ' + str(dpercent) + ' from reference'
         i += 1
 
+
 def test_mirp_features():
-    data_folder = os.path.dirname(__file__) + '/test_data/'
-    features_df = pd.read_pickle(data_folder + 'mirp_features.pkl')
-    pyrad_extractor = features.MirpExtractor(num_parcels=1)
-    new_features = pyrad_extractor.calc_features(parcellation_file_name=data_folder + 'test_tract_envelope.nii.gz',
-                                                 parameter_map_file_name=data_folder + 'test_map.nii.gz'
-                                                )
-    # remove path from 'map' and 'parcellation' columns
-    new_features['map'] = new_features['map'].str.split('/').str[-1]
-    new_features['parcellation'] = new_features['parcellation'].str.split('/').str[-1]
-    new_features.to_pickle(get_results_path() + 'mirp_features.pkl')
-    pd.testing.assert_frame_equal(new_features, features_df, check_dtype=False)
+
+    if sys.version_info >= (3, 11): # mirp only works with python >= 3.11
+        data_folder = os.path.dirname(__file__) + '/test_data/'
+        features_df = pd.read_pickle(data_folder + 'mirp_features.pkl')
+        pyrad_extractor = features.MirpExtractor(num_parcels=1)
+        new_features = pyrad_extractor.calc_features(parcellation_file_name=data_folder + 'test_tract_envelope.nii.gz',
+                                                    parameter_map_file_name=data_folder + 'test_map.nii.gz'
+                                                    )
+        # remove path from 'map' and 'parcellation' columns
+        new_features['map'] = new_features['map'].str.split('/').str[-1]
+        new_features['parcellation'] = new_features['parcellation'].str.split('/').str[-1]
+        new_features.to_pickle(get_results_path() + 'mirp_features.pkl')
+
+        new_features = new_features.drop(columns=['extractor_version', 'radtract_version'])
+        features_df = features_df.drop(columns=['extractor_version', 'radtract_version'])
+
+        i = 0
+        for el1, el2 in zip(new_features['value'], features_df['value']):
+            dpercent = abs(1.0 - el1 / el2)
+            assert dpercent < 0.025, 'value ' + str(i) + ' differs by ' + str(dpercent) + ' from reference'
+            i += 1
+    else:
+        print('Skipping MIRP tests because python version is < 3.11')
```


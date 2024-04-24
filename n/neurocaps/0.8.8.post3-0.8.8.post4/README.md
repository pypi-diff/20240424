# Comparing `tmp/neurocaps-0.8.8.post3.tar.gz` & `tmp/neurocaps-0.8.8.post4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neurocaps-0.8.8.post3.tar", last modified: Mon Mar 25 16:14:19 2024, max compression
+gzip compressed data, was "neurocaps-0.8.8.post4.tar", last modified: Wed Apr 24 02:00:18 2024, max compression
```

## Comparing `neurocaps-0.8.8.post3.tar` & `neurocaps-0.8.8.post4.tar`

### file list

```diff
@@ -1,36 +1,37 @@
-drwxr-xr-x   0 dsmit216 (351141) hpc_nbc    (147)        0 2024-03-25 16:14:19.000000 neurocaps-0.8.8.post3/
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     1077 2024-03-25 16:14:04.000000 neurocaps-0.8.8.post3/LICENSE.md
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)    10826 2024-03-25 16:14:19.000000 neurocaps-0.8.8.post3/PKG-INFO
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     9899 2024-03-25 16:14:04.000000 neurocaps-0.8.8.post3/README.md
-drwxr-xr-x   0 dsmit216 (351141) hpc_nbc    (147)        0 2024-03-25 16:14:19.000000 neurocaps-0.8.8.post3/neurocaps/
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)       78 2024-03-25 16:14:04.000000 neurocaps-0.8.8.post3/neurocaps/__init__.py
-drwxr-xr-x   0 dsmit216 (351141) hpc_nbc    (147)        0 2024-03-25 16:14:19.000000 neurocaps-0.8.8.post3/neurocaps/_utils/
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)      352 2024-03-25 16:14:04.000000 neurocaps-0.8.8.post3/neurocaps/_utils/__init__.py
-drwxr-xr-x   0 dsmit216 (351141) hpc_nbc    (147)        0 2024-03-25 16:14:19.000000 neurocaps-0.8.8.post3/neurocaps/_utils/_cap_internals/
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)       87 2024-03-25 16:14:04.000000 neurocaps-0.8.8.post3/neurocaps/_utils/_cap_internals/__init__.py
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     2227 2024-03-25 16:14:04.000000 neurocaps-0.8.8.post3/neurocaps/_utils/_cap_internals/_capgetter.py
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)      179 2024-03-25 16:14:04.000000 neurocaps-0.8.8.post3/neurocaps/_utils/_cap_internals/_pickle_to_dict.py
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     2813 2024-03-25 16:14:04.000000 neurocaps-0.8.8.post3/neurocaps/_utils/_check_confound_names.py
-drwxr-xr-x   0 dsmit216 (351141) hpc_nbc    (147)        0 2024-03-25 16:14:19.000000 neurocaps-0.8.8.post3/neurocaps/_utils/_timeseriesextractor_internals/
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)      178 2024-03-25 16:14:04.000000 neurocaps-0.8.8.post3/neurocaps/_utils/_timeseriesextractor_internals/__init__.py
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     2901 2024-03-25 16:14:04.000000 neurocaps-0.8.8.post3/neurocaps/_utils/_timeseriesextractor_internals/_check_parcel_approach.py
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     5994 2024-03-25 16:14:04.000000 neurocaps-0.8.8.post3/neurocaps/_utils/_timeseriesextractor_internals/_extract_timeseries.py
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     2405 2024-03-25 16:14:04.000000 neurocaps-0.8.8.post3/neurocaps/_utils/_timeseriesextractor_internals/_timeseriesextractorgetter.py
-drwxr-xr-x   0 dsmit216 (351141) hpc_nbc    (147)        0 2024-03-25 16:14:19.000000 neurocaps-0.8.8.post3/neurocaps/analysis/
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)       85 2024-03-25 16:14:04.000000 neurocaps-0.8.8.post3/neurocaps/analysis/__init__.py
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)    44374 2024-03-25 16:14:04.000000 neurocaps-0.8.8.post3/neurocaps/analysis/cap.py
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     4697 2024-03-25 16:14:04.000000 neurocaps-0.8.8.post3/neurocaps/analysis/merge.py
-drwxr-xr-x   0 dsmit216 (351141) hpc_nbc    (147)        0 2024-03-25 16:14:19.000000 neurocaps-0.8.8.post3/neurocaps/extraction/
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)       86 2024-03-25 16:14:04.000000 neurocaps-0.8.8.post3/neurocaps/extraction/__init__.py
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)    19484 2024-03-25 16:14:04.000000 neurocaps-0.8.8.post3/neurocaps/extraction/timeseriesextractor.py
-drwxr-xr-x   0 dsmit216 (351141) hpc_nbc    (147)        0 2024-03-25 16:14:19.000000 neurocaps-0.8.8.post3/neurocaps.egg-info/
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)    10826 2024-03-25 16:14:19.000000 neurocaps-0.8.8.post3/neurocaps.egg-info/PKG-INFO
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)      922 2024-03-25 16:14:19.000000 neurocaps-0.8.8.post3/neurocaps.egg-info/SOURCES.txt
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)        1 2024-03-25 16:14:19.000000 neurocaps-0.8.8.post3/neurocaps.egg-info/dependency_links.txt
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)       94 2024-03-25 16:14:19.000000 neurocaps-0.8.8.post3/neurocaps.egg-info/requires.txt
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)       10 2024-03-25 16:14:19.000000 neurocaps-0.8.8.post3/neurocaps.egg-info/top_level.txt
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     1240 2024-03-25 16:14:04.000000 neurocaps-0.8.8.post3/pyproject.toml
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)       38 2024-03-25 16:14:19.000000 neurocaps-0.8.8.post3/setup.cfg
-drwxr-xr-x   0 dsmit216 (351141) hpc_nbc    (147)        0 2024-03-25 16:14:19.000000 neurocaps-0.8.8.post3/tests/
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     6365 2024-03-25 16:14:04.000000 neurocaps-0.8.8.post3/tests/test_CAP.py
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     1906 2024-03-25 16:14:04.000000 neurocaps-0.8.8.post3/tests/test_merge_dicts.py
+drwxr-xr-x   0 dsmit216 (351141) hpc_nbc    (147)        0 2024-04-24 02:00:18.000000 neurocaps-0.8.8.post4/
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     1077 2024-04-24 01:37:40.000000 neurocaps-0.8.8.post4/LICENSE.md
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)    12235 2024-04-24 02:00:18.000000 neurocaps-0.8.8.post4/PKG-INFO
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)    11310 2024-04-24 01:37:40.000000 neurocaps-0.8.8.post4/README.md
+drwxr-xr-x   0 dsmit216 (351141) hpc_nbc    (147)        0 2024-04-24 02:00:17.000000 neurocaps-0.8.8.post4/neurocaps/
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)       78 2024-04-24 01:37:40.000000 neurocaps-0.8.8.post4/neurocaps/__init__.py
+drwxr-xr-x   0 dsmit216 (351141) hpc_nbc    (147)        0 2024-04-24 02:00:17.000000 neurocaps-0.8.8.post4/neurocaps/_utils/
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)      352 2024-04-24 01:37:40.000000 neurocaps-0.8.8.post4/neurocaps/_utils/__init__.py
+drwxr-xr-x   0 dsmit216 (351141) hpc_nbc    (147)        0 2024-04-24 02:00:17.000000 neurocaps-0.8.8.post4/neurocaps/_utils/_cap_internals/
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)       87 2024-04-24 01:37:40.000000 neurocaps-0.8.8.post4/neurocaps/_utils/_cap_internals/__init__.py
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     2227 2024-04-24 01:37:40.000000 neurocaps-0.8.8.post4/neurocaps/_utils/_cap_internals/_capgetter.py
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)      179 2024-04-24 01:37:40.000000 neurocaps-0.8.8.post4/neurocaps/_utils/_cap_internals/_pickle_to_dict.py
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     2825 2024-04-24 01:37:40.000000 neurocaps-0.8.8.post4/neurocaps/_utils/_check_confound_names.py
+drwxr-xr-x   0 dsmit216 (351141) hpc_nbc    (147)        0 2024-04-24 02:00:18.000000 neurocaps-0.8.8.post4/neurocaps/_utils/_timeseriesextractor_internals/
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)      178 2024-04-24 01:37:40.000000 neurocaps-0.8.8.post4/neurocaps/_utils/_timeseriesextractor_internals/__init__.py
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     2901 2024-04-24 01:37:40.000000 neurocaps-0.8.8.post4/neurocaps/_utils/_timeseriesextractor_internals/_check_parcel_approach.py
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     6126 2024-04-24 01:37:40.000000 neurocaps-0.8.8.post4/neurocaps/_utils/_timeseriesextractor_internals/_extract_timeseries.py
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     2405 2024-04-24 01:37:40.000000 neurocaps-0.8.8.post4/neurocaps/_utils/_timeseriesextractor_internals/_timeseriesextractorgetter.py
+drwxr-xr-x   0 dsmit216 (351141) hpc_nbc    (147)        0 2024-04-24 02:00:18.000000 neurocaps-0.8.8.post4/neurocaps/analysis/
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)       85 2024-04-24 01:37:40.000000 neurocaps-0.8.8.post4/neurocaps/analysis/__init__.py
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)    44374 2024-04-24 01:37:40.000000 neurocaps-0.8.8.post4/neurocaps/analysis/cap.py
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     4697 2024-04-24 01:37:40.000000 neurocaps-0.8.8.post4/neurocaps/analysis/merge.py
+drwxr-xr-x   0 dsmit216 (351141) hpc_nbc    (147)        0 2024-04-24 02:00:18.000000 neurocaps-0.8.8.post4/neurocaps/extraction/
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)       86 2024-04-24 01:37:40.000000 neurocaps-0.8.8.post4/neurocaps/extraction/__init__.py
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)    20113 2024-04-24 01:37:40.000000 neurocaps-0.8.8.post4/neurocaps/extraction/timeseriesextractor.py
+drwxr-xr-x   0 dsmit216 (351141) hpc_nbc    (147)        0 2024-04-24 02:00:17.000000 neurocaps-0.8.8.post4/neurocaps.egg-info/
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)    12235 2024-04-24 02:00:17.000000 neurocaps-0.8.8.post4/neurocaps.egg-info/PKG-INFO
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)      956 2024-04-24 02:00:17.000000 neurocaps-0.8.8.post4/neurocaps.egg-info/SOURCES.txt
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)        1 2024-04-24 02:00:17.000000 neurocaps-0.8.8.post4/neurocaps.egg-info/dependency_links.txt
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)       94 2024-04-24 02:00:17.000000 neurocaps-0.8.8.post4/neurocaps.egg-info/requires.txt
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)       10 2024-04-24 02:00:17.000000 neurocaps-0.8.8.post4/neurocaps.egg-info/top_level.txt
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     1240 2024-04-24 01:37:40.000000 neurocaps-0.8.8.post4/pyproject.toml
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)       38 2024-04-24 02:00:18.000000 neurocaps-0.8.8.post4/setup.cfg
+drwxr-xr-x   0 dsmit216 (351141) hpc_nbc    (147)        0 2024-04-24 02:00:18.000000 neurocaps-0.8.8.post4/tests/
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     6365 2024-04-24 01:37:41.000000 neurocaps-0.8.8.post4/tests/test_CAP.py
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     1005 2024-04-24 01:37:41.000000 neurocaps-0.8.8.post4/tests/test_TimeseriesExtractor.py
+-rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     1906 2024-04-24 01:37:41.000000 neurocaps-0.8.8.post4/tests/test_merge_dicts.py
```

### Comparing `neurocaps-0.8.8.post3/LICENSE.md` & `neurocaps-0.8.8.post4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neurocaps-0.8.8.post3/PKG-INFO` & `neurocaps-0.8.8.post4/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,174 +1,151 @@
-Metadata-Version: 2.1
-Name: neurocaps
-Version: 0.8.8.post3
-Summary: Co-activation patterns Python package
-Author-email: Donisha Smith <donishasmith@outlook.com>
-Project-URL: Homepage, https://github.com/donishadsmith/neurocaps
-Keywords: python,Co-Activation Patterns,CAPs,neuroimaging,fmri,dfc,dynamic functional connectivity,fMRIPrep
-Classifier: Intended Audience :: Education
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Operating System :: Microsoft :: Windows :: Windows 11
-Classifier: Development Status :: 4 - Beta
-Requires-Python: >=3.9.0
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
-Requires-Dist: numpy
-Requires-Dist: pandas
-Requires-Dist: matplotlib
-Requires-Dist: seaborn
-Requires-Dist: kneed
-Requires-Dist: nilearn==0.10.2
-Requires-Dist: pybids; platform_system != "Windows"
-
-# neurocaps
-This is a Python package to perform Co-activation Patterns (CAPs) analyses, which involves using kmeans clustering to group timepoints (TR's) into brain states, on both resting-state or task data. It is compatible with data preprocessed with **fMRIPrep** and assumes your directory is BIDS-compliant and contains a derivatives folder with a pipeline folder, such as fMRIPrep, containing preprocessed BOLD data.
-
-**Still in beta but stable.**
-
-# Installation
-
-**Note**: The `.get_bold()` method in the `TimeseriesExtractor` class in this package uses pybids, which is only functional on POSIX operating system and Mac OS. Assuming you have a pickled timeseries dictionary in the proper nested form, this package can be used on windows to visualize the bold timeseries, use the `CAP` class, and the `merge_dicts()` fuction. 
-
-To install, using your preferred terminal:
-
-**Installation with pip:**
-
-```bash
-
-pip install neurocaps
-
-```
-
-**From source (Development version):**
-
-```bash
-pip install git+https://github.com/donishadsmith/neurocaps.git
-```
-
-or
-
-```bash
-
-git clone https://github.com/donishadsmith/neurocaps/
-cd neurocaps
-pip install -e .
-
-```
-
-# Usage
- **This package contains two main classes - `TimeseriesExtractor`, for extracting the timeseries, and `CAP`, for performing the CAPs analysis.**
-
-**Note**: When extracting the timeseries, **this package uses the Schaefer atlas or the Automated Anatomical Labeling (AAL) atlas**. The number of ROIs and networks for the Schaefer atlas can be modified with the `parcel_approach` parameter when initializing the main `TimeseriesExtractor` class. To modify it, you must use a nested dictionary, where the primary key is "Schaefer" and the sub-keys are "n_rois" and "yeo_networks". Example: `parcel_approach = {"Schaefer": {"n_rois": 100, "yeo_networks": 7}}`. Similary the version of the AAL atlas can be modified using `parcel_approach = {"AAL": {"version": "SPM12"}}`.
-
-**Main features for `TimeseriesExtractor` includes:**
-
-- Timeseries extraction for resting state or task data and creating a nested dictionary containing the subject ID, run number, and associated timeseries. This is used as input for the `get_caps()` method in the `CAP` class.
-- Saving the nested dictionary containing timeseries as a pickle file.
-- Visualizing the timeseries of a Schaefer or AAL node or network subject's run. Also includes the ability to save plots.
-- Ability to use parallel processing by specifiying the number of CPU cores to use in the `n_cores` parameter in the `get_bold()` method. Testing on an HPC using a loop with `TimeseriesExtractor.get_bold()` to extract the session 1 and 2 bold timeries from 105 subjects from resting-state data (single-run containing 360 volumes) and two task datasets (three-runs containing 200 volumes each and two-runs containing 200 volumes) reduced processing time from 5 hrs 48 mins to 1 hr 26 mins (using 10 cores).
-
-**Main features for `CAP` includes:**
-
-- Performing the silhouette or elbow method to identify the optimal cluster size. When the optimal cluster size is identified, the optimal model is saved as an attribute.
-- Visualizing the CAPs identified as an outer product or regular heatmap. For outer products, you also have the ability to use subplots to reduce the number of individual plots. You can also save the plots and use them. Please refer to the docstring for the `visualize_caps()` method in the `CAP` class to see the list of available kwargs arguments to modify plots.
-- Grouping feature to perform CAPs independently on groups of subject IDs. When grouping is specified, k-means clustering, silhouette and elbow methods, as well as plotting, are done for each independent group.
-- Calculating CAP metrics as described in [Liu et al., 2018](https://doi.org/10.1016/j.neuroimage.2018.01.041)[^1] and [Yang et al., 2021](https://doi.org/10.1016/j.neuroimage.2021.118193)[^2], where *temporal fraction* is the proportion of total volumes spent in a single CAP over all volumes in a run, *persistence* is the average time spent in a single CAP before transitioning to another CAP (average consecutive/uninterrupted time), and *counts* is the frequency of each CAP observed in a run, and *transition frequency* is the number of switches between
-different CAPs across the entire run.
-
-**Additionally, the `neurocaps.analysis` submodule contains the `merge_dicts` function, which allows you to merge the subject_timeseries dictionaries (merged dictionary will be returned and can be saved as a pickle file) for overlapping subjects across tasks in order to identify similar CAPs across different tasks[^3].**
-
-Please refer to [demo.ipynb](https://github.com/donishadsmith/neurocaps/blob/main/demo.ipynb) to see a more extensive demonstration of the features included in this package. 
-
-Quick code example:
-
-```python
-
-from neurocaps.extraction import TimeseriesExtractor
-from neurocaps.analysis import CAP
-
-"""If an asterisk '*' is after a name, all confounds starting with the 
-term preceding the parameter will be used. in this case, all parameters 
-starting with cosine will be used."""
-confounds = ["cosine*", "non_steady_state*", "trans_x", "trans_x_derivative1", "trans_y", 
-             "trans_y_derivative1", "trans_z","trans_z_derivative1", 
-             "rot_x", "rot_x_derivative1", "rot_y", "rot_y_derivative1", 
-             "rot_z","rot_z_derivative1"]
-
-"""If use_confounds is True but no confound_names provided, there are hardcoded 
-confound names that will extract the data from the confound files outputted by fMRIPrep
-`n_acompcor_separate` will use the first 'n' components derived from the separate 
-white-matter (WM) and cerebrospinal fluid (CSF). To use the acompcor components from the 
-combined mask, list them in the `confound_names` parameter"""
-parcel_approach = {"Schaefer": {"n_rois": 100, "yeo_networks": 7}}
-
-extractor = TimeseriesExtractor(parcel_approach=parcel_approach, standardize="zscore_sample",
-                                 use_confounds=True, detrend=True, low_pass=0.15, high_pass=0.01, 
-                                 confound_names=confounds, n_acompcor_separate=6)
-
-bids_dir = "/path/to/bids/dir"
-
-# If there are multiple pipelines in the derivatives folder, you can specify a specific pipeline
-pipeline_name = "fmriprep-1.4.0"
-
-# Resting State
-# extractor.get_bold(bids_dir=bids_dir, task="rest", pipeline_name=pipeline_name)
-
-# Task; use parallel processing with `n_cores`
-extractor.get_bold(bids_dir=bids_dir, task="emo", condition="positive", 
-                   pipeline_name=pipeline_name, n_cores=10)
-
-cap_analysis = CAP(parcel_approach=extractor.parcel_approach,
-                    n_clusters=6)
-
-cap_analysis.get_caps(subject_timeseries=extractor.subject_timeseries, 
-                      standardize = True)
-
-# Visualize CAPs
-cap_analysis.visualize_caps(visual_scope="networks", plot_options="outer product", 
-                            task_title="- Positive Valence", ncol=3, sharey=True, 
-                            subplots=True)
-
-cap_analysis.visualize_caps(visual_scope="nodes", plot_options="outer product", 
-                            task_title="- Positive Valence", ncol=3,sharey=True, 
-                            subplots=True, xlabel_rotation=90, tight_layout=False, 
-                            hspace = 0.4)
-
-# Get CAP metrics
-outputs = cap_analysis.calculate_metrics(subject_timeseries=extractor.subject_timeseries, tr=2.0, 
-                                         return_df=True, output_dir=output_dir,
-                                         metrics=["temporal fraction", "persistence"],
-                                         continuous_runs=True, file_name="All_Subjects_CAPs_metrics")
-
-print(outputs["temporal fraction"])
-
-```
-**Graph Outputs:**
-![image](https://github.com/donishadsmith/neurocaps/assets/112973674/4699bbd9-1f55-462b-9d9e-4ef17da79ad4)
-![image](https://github.com/donishadsmith/neurocaps/assets/112973674/506c5be5-540d-43a9-8a61-c02062f5c6f9)
-
-**DataFrame Output:**
-| Subject_ID | Group | Run | CAP-1 | CAP-2 | CAP-3 | CAP-4 | CAP-5 | CAP-6 |
-| --- | --- | --- | --- | --- | --- | --- | --- | --- |
-| 1 | All Subjects | Continuous Runs | 0.14 | 0.17 | 0.14 | 0.2 | 0.15 | 0.19 |
-| 2 | All Subjects | Continuous Runs | 0.17 | 0.17 | 0.16 | 0.16 | 0.15 | 0.19 |
-| 3 | All Subjects | Continuous Runs | 0.15 | 0.2 | 0.14 | 0.18 | 0.17 | 0.17 |
-| 4 | All Subjects | Continuous Runs | 0.17 | 0.21 | 0.18 | 0.17 | 0.1 | 0.16 |
-| 5 | All Subjects | Continuous Runs | 0.14 | 0.19 | 0.14 | 0.16 | 0.2 | 0.18 |
-| 6 | All Subjects | Continuous Runs | 0.16 | 0.21 | 0.16 | 0.18 | 0.16 | 0.13 |
-| 7 | All Subjects | Continuous Runs | 0.16 | 0.16 | 0.17 | 0.15 | 0.19 | 0.17 |
-| 8 | All Subjects | Continuous Runs | 0.17 | 0.21 | 0.13 | 0.14 | 0.17 | 0.18 |
-| 9 | All Subjects | Continuous Runs | 0.18 | 0.1 | 0.17 | 0.18 | 0.16 | 0.2 |
-| 10 | All Subjects | Continuous Runs | 0.14 | 0.19 | 0.14 | 0.17 | 0.19 | 0.16 |
-
-# References
-[^1]: Liu, X., Zhang, N., Chang, C., & Duyn, J. H. (2018). Co-activation patterns in resting-state fMRI signals. NeuroImage, 180, 485–494. https://doi.org/10.1016/j.neuroimage.2018.01.041
-
-[^2]: Yang, H., Zhang, H., Di, X., Wang, S., Meng, C., Tian, L., & Biswal, B. (2021). Reproducible coactivation patterns of functional brain networks reveal the aberrant dynamic state transition in schizophrenia. NeuroImage, 237, 118193. https://doi.org/10.1016/j.neuroimage.2021.118193
-
-[^3]: Kupis, L., Romero, C., Dirks, B., Hoang, S., Parladé, M. V., Beaumont, A. L., Cardona, S. M., Alessandri, M., Chang, C., Nomi, J. S., & Uddin, L. Q. (2020). Evoked and intrinsic brain network dynamics in children with autism spectrum disorder. NeuroImage: Clinical, 28, 102396. https://doi.org/10.1016/j.nicl.2020.102396
-
+# neurocaps
+This is a Python package to perform Co-activation Patterns (CAPs) analyses, which involves using kmeans clustering to group timepoints (TR's) into brain states, on both resting-state or task data. It is compatible with data preprocessed with **fMRIPrep** and assumes your directory is BIDS-compliant and contains a derivatives folder with a pipeline folder, such as fMRIPrep, containing preprocessed BOLD data.
+
+**Still in beta but stable.**
+
+# Installation
+
+**Note**: The `.get_bold()` method in the `TimeseriesExtractor` class in this package uses pybids, which is only functional on POSIX operating system and Mac OS. Assuming you have a pickled timeseries dictionary in the proper nested form, this package can be used on windows to visualize the bold timeseries, use the `CAP` class, and the `merge_dicts()` fuction. 
+
+To install, using your preferred terminal:
+
+**Installation with pip:**
+
+```bash
+
+pip install neurocaps
+
+```
+
+**From source (Development version):**
+
+```bash
+pip install git+https://github.com/donishadsmith/neurocaps.git
+```
+
+or
+
+```bash
+
+git clone https://github.com/donishadsmith/neurocaps/
+cd neurocaps
+pip install -e .
+
+```
+
+# Usage
+ **This package contains two main classes - `TimeseriesExtractor`, for extracting the timeseries, and `CAP`, for performing the CAPs analysis.**
+
+**Note**: When extracting the timeseries, **this package uses the Schaefer atlas or the Automated Anatomical Labeling (AAL) atlas**. The number of ROIs and networks for the Schaefer atlas can be modified with the `parcel_approach` parameter when initializing the main `TimeseriesExtractor` class. To modify it, you must use a nested dictionary, where the primary key is "Schaefer" and the sub-keys are "n_rois" and "yeo_networks". Example: `parcel_approach = {"Schaefer": {"n_rois": 100, "yeo_networks": 7}}`. Similary the version of the AAL atlas can be modified using `parcel_approach = {"AAL": {"version": "SPM12"}}`.
+
+**Main features for `TimeseriesExtractor` includes:**
+
+- Timeseries extraction for resting state or task data and creating a nested dictionary containing the subject ID, run number, and associated timeseries. This is used as input for the `get_caps()` method in the `CAP` class.
+- Saving the nested dictionary containing timeseries as a pickle file.
+- Visualizing the timeseries of a Schaefer or AAL node or network subject's run. Also includes the ability to save plots.
+- Ability to use parallel processing by specifiying the number of CPU cores to use in the `n_cores` parameter in the `get_bold()` method. Testing on an HPC using a loop with `TimeseriesExtractor.get_bold()` to extract the session 1 and 2 bold timeries from 105 subjects from resting-state data (single-run containing 360 volumes) and two task datasets (three-runs containing 200 volumes each and two-runs containing 200 volumes) reduced processing time from 5 hrs 48 mins to 1 hr 26 mins (using 10 cores).
+
+**Main features for `CAP` includes:**
+
+- Performing the silhouette or elbow method to identify the optimal cluster size. When the optimal cluster size is identified, the optimal model is saved as an attribute.
+- Visualizing the CAPs identified as an outer product or regular heatmap. For outer products, you also have the ability to use subplots to reduce the number of individual plots. You can also save the plots and use them. Please refer to the docstring for the `visualize_caps()` method in the `CAP` class to see the list of available kwargs arguments to modify plots.
+- Grouping feature to perform CAPs independently on groups of subject IDs. When grouping is specified, k-means clustering, silhouette and elbow methods, as well as plotting, are done for each independent group.
+- Calculating CAP metrics as described in [Liu et al., 2018](https://doi.org/10.1016/j.neuroimage.2018.01.041)[^1] and [Yang et al., 2021](https://doi.org/10.1016/j.neuroimage.2021.118193)[^2], where *temporal fraction* is the proportion of total volumes spent in a single CAP over all volumes in a run, *persistence* is the average time spent in a single CAP before transitioning to another CAP (average consecutive/uninterrupted time), and *counts* is the frequency of each CAP observed in a run, and *transition frequency* is the number of switches between
+different CAPs across the entire run.
+
+**Additionally, the `neurocaps.analysis` submodule contains the `merge_dicts` function, which allows you to merge the subject_timeseries dictionaries (merged dictionary will be returned and can be saved as a pickle file) for overlapping subjects across tasks in order to identify similar CAPs across different tasks[^3].**
+
+Please refer to [demo.ipynb](https://github.com/donishadsmith/neurocaps/blob/main/demo.ipynb) to see a more extensive demonstration of the features included in this package. 
+
+Quick code example:
+
+```python
+
+from neurocaps.extraction import TimeseriesExtractor
+from neurocaps.analysis import CAP
+
+"""If an asterisk '*' is after a name, all confounds starting with the 
+term preceding the parameter will be used. in this case, all parameters 
+starting with cosine will be used."""
+confounds = ["cosine*", "trans_x", "trans_x_derivative1", "trans_y", 
+             "trans_y_derivative1", "trans_z","trans_z_derivative1", 
+             "rot_x", "rot_x_derivative1", "rot_y", "rot_y_derivative1", 
+             "rot_z","rot_z_derivative1"]
+
+"""If use_confounds is True but no confound_names provided, there are hardcoded 
+confound names that will extract the data from the confound files outputted by fMRIPrep
+`n_acompcor_separate` will use the first 'n' components derived from the separate 
+white-matter (WM) and cerebrospinal fluid (CSF). To use the acompcor components from the 
+combined mask, list them in the `confound_names` parameter"""
+parcel_approach = {"Schaefer": {"n_rois": 100, "yeo_networks": 7}}
+
+extractor = TimeseriesExtractor(parcel_approach=parcel_approach, standardize="zscore_sample",
+                                 use_confounds=True, detrend=True, low_pass=0.15, high_pass=0.01, 
+                                 confound_names=confounds, n_acompcor_separate=6)
+
+bids_dir = "/path/to/bids/dir"
+
+# If there are multiple pipelines in the derivatives folder, you can specify a specific pipeline
+pipeline_name = "fmriprep-1.4.0"
+
+# Resting State
+# extractor.get_bold(bids_dir=bids_dir, task="rest", pipeline_name=pipeline_name)
+
+# Task; use parallel processing with `n_cores`
+extractor.get_bold(bids_dir=bids_dir, task="emo", condition="positive", 
+                   pipeline_name=pipeline_name, n_cores=10)
+
+cap_analysis = CAP(parcel_approach=extractor.parcel_approach,
+                    n_clusters=6)
+
+cap_analysis.get_caps(subject_timeseries=extractor.subject_timeseries, 
+                      standardize = True)
+
+# Visualize CAPs
+cap_analysis.visualize_caps(visual_scope="networks", plot_options="outer product", 
+                            task_title="- Positive Valence", ncol=3, sharey=True, 
+                            subplots=True)
+
+cap_analysis.visualize_caps(visual_scope="nodes", plot_options="outer product", 
+                            task_title="- Positive Valence", ncol=3,sharey=True, 
+                            subplots=True, xlabel_rotation=90, tight_layout=False, 
+                            hspace = 0.4)
+
+# Get CAP metrics
+outputs = cap_analysis.calculate_metrics(subject_timeseries=extractor.subject_timeseries, tr=2.0, 
+                                         return_df=True, output_dir=output_dir,
+                                         metrics=["temporal fraction", "persistence"],
+                                         continuous_runs=True, file_name="All_Subjects_CAPs_metrics")
+
+print(outputs["temporal fraction"])
+
+```
+**Graph Outputs:**
+![image](https://github.com/donishadsmith/neurocaps/assets/112973674/4699bbd9-1f55-462b-9d9e-4ef17da79ad4)
+![image](https://github.com/donishadsmith/neurocaps/assets/112973674/506c5be5-540d-43a9-8a61-c02062f5c6f9)
+
+**DataFrame Output:**
+| Subject_ID | Group | Run | CAP-1 | CAP-2 | CAP-3 | CAP-4 | CAP-5 | CAP-6 |
+| --- | --- | --- | --- | --- | --- | --- | --- | --- |
+| 1 | All Subjects | Continuous Runs | 0.14 | 0.17 | 0.14 | 0.2 | 0.15 | 0.19 |
+| 2 | All Subjects | Continuous Runs | 0.17 | 0.17 | 0.16 | 0.16 | 0.15 | 0.19 |
+| 3 | All Subjects | Continuous Runs | 0.15 | 0.2 | 0.14 | 0.18 | 0.17 | 0.17 |
+| 4 | All Subjects | Continuous Runs | 0.17 | 0.21 | 0.18 | 0.17 | 0.1 | 0.16 |
+| 5 | All Subjects | Continuous Runs | 0.14 | 0.19 | 0.14 | 0.16 | 0.2 | 0.18 |
+| 6 | All Subjects | Continuous Runs | 0.16 | 0.21 | 0.16 | 0.18 | 0.16 | 0.13 |
+| 7 | All Subjects | Continuous Runs | 0.16 | 0.16 | 0.17 | 0.15 | 0.19 | 0.17 |
+| 8 | All Subjects | Continuous Runs | 0.17 | 0.21 | 0.13 | 0.14 | 0.17 | 0.18 |
+| 9 | All Subjects | Continuous Runs | 0.18 | 0.1 | 0.17 | 0.18 | 0.16 | 0.2 |
+| 10 | All Subjects | Continuous Runs | 0.14 | 0.19 | 0.14 | 0.17 | 0.19 | 0.16 |
+
+# Testing 
+This package was tested using a closed dataset as well as a modified version of a single subject open dataset to test the TimeseriesExtractor function on Github Actions. Furthermore, the open dataset provided by [Laumann & Poldrack](https://openfmri.org/dataset/ds000031/) and used in [Laumann et al., 2015](https://doi.org/10.1016/j.neuron.2015.06.037)[^4]. Additionally, this data was obtained from the OpenfMRI database. Its accession number is ds000031. Modifications to the data consist of truncating the preprocessed bold data and confounds form 448 timepoints to 34 timepoints, only including session 002 data, adding a dataset_description.json file to the fmriprep folder, excluding the nii.gz file in the root bids folder, only retaining the mask, truncated preprocessed bold file, and truncated confounds file in the fmriprep folder, and slighly changing the naming style of the mask, preprocessed bold file, and confounds file in the fmriprep folder ot conform with the naming conventions of modern fmriprep outputs.
+
+# References
+[^1]: Liu, X., Zhang, N., Chang, C., & Duyn, J. H. (2018). Co-activation patterns in resting-state fMRI signals. NeuroImage, 180, 485–494. https://doi.org/10.1016/j.neuroimage.2018.01.041
+
+[^2]: Yang, H., Zhang, H., Di, X., Wang, S., Meng, C., Tian, L., & Biswal, B. (2021). Reproducible coactivation patterns of functional brain networks reveal the aberrant dynamic state transition in schizophrenia. NeuroImage, 237, 118193. https://doi.org/10.1016/j.neuroimage.2021.118193
+
+[^3]: Kupis, L., Romero, C., Dirks, B., Hoang, S., Parladé, M. V., Beaumont, A. L., Cardona, S. M., Alessandri, M., Chang, C., Nomi, J. S., & Uddin, L. Q. (2020). Evoked and intrinsic brain network dynamics in children with autism spectrum disorder. NeuroImage: Clinical, 28, 102396. https://doi.org/10.1016/j.nicl.2020.102396
+
+[^4]: Laumann, T. O., Gordon, E. M., Adeyemo, B., Snyder, A. Z., Joo, S. J., Chen, M. Y., Gilmore, A. W., McDermott, K. B., Nelson, S. M., Dosenbach, N. U., Schlaggar, B. L., Mumford, J. A., Poldrack, R. A., & Petersen, S. E. (2015). Functional system and areal organization of a highly sampled individual human brain. Neuron, 87(3), 657–670. https://doi.org/10.1016/j.neuron.2015.06.037
```

### Comparing `neurocaps-0.8.8.post3/README.md` & `neurocaps-0.8.8.post4/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,147 +1,178 @@
-# neurocaps
-This is a Python package to perform Co-activation Patterns (CAPs) analyses, which involves using kmeans clustering to group timepoints (TR's) into brain states, on both resting-state or task data. It is compatible with data preprocessed with **fMRIPrep** and assumes your directory is BIDS-compliant and contains a derivatives folder with a pipeline folder, such as fMRIPrep, containing preprocessed BOLD data.
-
-**Still in beta but stable.**
-
-# Installation
-
-**Note**: The `.get_bold()` method in the `TimeseriesExtractor` class in this package uses pybids, which is only functional on POSIX operating system and Mac OS. Assuming you have a pickled timeseries dictionary in the proper nested form, this package can be used on windows to visualize the bold timeseries, use the `CAP` class, and the `merge_dicts()` fuction. 
-
-To install, using your preferred terminal:
-
-**Installation with pip:**
-
-```bash
-
-pip install neurocaps
-
-```
-
-**From source (Development version):**
-
-```bash
-pip install git+https://github.com/donishadsmith/neurocaps.git
-```
-
-or
-
-```bash
-
-git clone https://github.com/donishadsmith/neurocaps/
-cd neurocaps
-pip install -e .
-
-```
-
-# Usage
- **This package contains two main classes - `TimeseriesExtractor`, for extracting the timeseries, and `CAP`, for performing the CAPs analysis.**
-
-**Note**: When extracting the timeseries, **this package uses the Schaefer atlas or the Automated Anatomical Labeling (AAL) atlas**. The number of ROIs and networks for the Schaefer atlas can be modified with the `parcel_approach` parameter when initializing the main `TimeseriesExtractor` class. To modify it, you must use a nested dictionary, where the primary key is "Schaefer" and the sub-keys are "n_rois" and "yeo_networks". Example: `parcel_approach = {"Schaefer": {"n_rois": 100, "yeo_networks": 7}}`. Similary the version of the AAL atlas can be modified using `parcel_approach = {"AAL": {"version": "SPM12"}}`.
-
-**Main features for `TimeseriesExtractor` includes:**
-
-- Timeseries extraction for resting state or task data and creating a nested dictionary containing the subject ID, run number, and associated timeseries. This is used as input for the `get_caps()` method in the `CAP` class.
-- Saving the nested dictionary containing timeseries as a pickle file.
-- Visualizing the timeseries of a Schaefer or AAL node or network subject's run. Also includes the ability to save plots.
-- Ability to use parallel processing by specifiying the number of CPU cores to use in the `n_cores` parameter in the `get_bold()` method. Testing on an HPC using a loop with `TimeseriesExtractor.get_bold()` to extract the session 1 and 2 bold timeries from 105 subjects from resting-state data (single-run containing 360 volumes) and two task datasets (three-runs containing 200 volumes each and two-runs containing 200 volumes) reduced processing time from 5 hrs 48 mins to 1 hr 26 mins (using 10 cores).
-
-**Main features for `CAP` includes:**
-
-- Performing the silhouette or elbow method to identify the optimal cluster size. When the optimal cluster size is identified, the optimal model is saved as an attribute.
-- Visualizing the CAPs identified as an outer product or regular heatmap. For outer products, you also have the ability to use subplots to reduce the number of individual plots. You can also save the plots and use them. Please refer to the docstring for the `visualize_caps()` method in the `CAP` class to see the list of available kwargs arguments to modify plots.
-- Grouping feature to perform CAPs independently on groups of subject IDs. When grouping is specified, k-means clustering, silhouette and elbow methods, as well as plotting, are done for each independent group.
-- Calculating CAP metrics as described in [Liu et al., 2018](https://doi.org/10.1016/j.neuroimage.2018.01.041)[^1] and [Yang et al., 2021](https://doi.org/10.1016/j.neuroimage.2021.118193)[^2], where *temporal fraction* is the proportion of total volumes spent in a single CAP over all volumes in a run, *persistence* is the average time spent in a single CAP before transitioning to another CAP (average consecutive/uninterrupted time), and *counts* is the frequency of each CAP observed in a run, and *transition frequency* is the number of switches between
-different CAPs across the entire run.
-
-**Additionally, the `neurocaps.analysis` submodule contains the `merge_dicts` function, which allows you to merge the subject_timeseries dictionaries (merged dictionary will be returned and can be saved as a pickle file) for overlapping subjects across tasks in order to identify similar CAPs across different tasks[^3].**
-
-Please refer to [demo.ipynb](https://github.com/donishadsmith/neurocaps/blob/main/demo.ipynb) to see a more extensive demonstration of the features included in this package. 
-
-Quick code example:
-
-```python
-
-from neurocaps.extraction import TimeseriesExtractor
-from neurocaps.analysis import CAP
-
-"""If an asterisk '*' is after a name, all confounds starting with the 
-term preceding the parameter will be used. in this case, all parameters 
-starting with cosine will be used."""
-confounds = ["cosine*", "non_steady_state*", "trans_x", "trans_x_derivative1", "trans_y", 
-             "trans_y_derivative1", "trans_z","trans_z_derivative1", 
-             "rot_x", "rot_x_derivative1", "rot_y", "rot_y_derivative1", 
-             "rot_z","rot_z_derivative1"]
-
-"""If use_confounds is True but no confound_names provided, there are hardcoded 
-confound names that will extract the data from the confound files outputted by fMRIPrep
-`n_acompcor_separate` will use the first 'n' components derived from the separate 
-white-matter (WM) and cerebrospinal fluid (CSF). To use the acompcor components from the 
-combined mask, list them in the `confound_names` parameter"""
-parcel_approach = {"Schaefer": {"n_rois": 100, "yeo_networks": 7}}
-
-extractor = TimeseriesExtractor(parcel_approach=parcel_approach, standardize="zscore_sample",
-                                 use_confounds=True, detrend=True, low_pass=0.15, high_pass=0.01, 
-                                 confound_names=confounds, n_acompcor_separate=6)
-
-bids_dir = "/path/to/bids/dir"
-
-# If there are multiple pipelines in the derivatives folder, you can specify a specific pipeline
-pipeline_name = "fmriprep-1.4.0"
-
-# Resting State
-# extractor.get_bold(bids_dir=bids_dir, task="rest", pipeline_name=pipeline_name)
-
-# Task; use parallel processing with `n_cores`
-extractor.get_bold(bids_dir=bids_dir, task="emo", condition="positive", 
-                   pipeline_name=pipeline_name, n_cores=10)
-
-cap_analysis = CAP(parcel_approach=extractor.parcel_approach,
-                    n_clusters=6)
-
-cap_analysis.get_caps(subject_timeseries=extractor.subject_timeseries, 
-                      standardize = True)
-
-# Visualize CAPs
-cap_analysis.visualize_caps(visual_scope="networks", plot_options="outer product", 
-                            task_title="- Positive Valence", ncol=3, sharey=True, 
-                            subplots=True)
-
-cap_analysis.visualize_caps(visual_scope="nodes", plot_options="outer product", 
-                            task_title="- Positive Valence", ncol=3,sharey=True, 
-                            subplots=True, xlabel_rotation=90, tight_layout=False, 
-                            hspace = 0.4)
-
-# Get CAP metrics
-outputs = cap_analysis.calculate_metrics(subject_timeseries=extractor.subject_timeseries, tr=2.0, 
-                                         return_df=True, output_dir=output_dir,
-                                         metrics=["temporal fraction", "persistence"],
-                                         continuous_runs=True, file_name="All_Subjects_CAPs_metrics")
-
-print(outputs["temporal fraction"])
-
-```
-**Graph Outputs:**
-![image](https://github.com/donishadsmith/neurocaps/assets/112973674/4699bbd9-1f55-462b-9d9e-4ef17da79ad4)
-![image](https://github.com/donishadsmith/neurocaps/assets/112973674/506c5be5-540d-43a9-8a61-c02062f5c6f9)
-
-**DataFrame Output:**
-| Subject_ID | Group | Run | CAP-1 | CAP-2 | CAP-3 | CAP-4 | CAP-5 | CAP-6 |
-| --- | --- | --- | --- | --- | --- | --- | --- | --- |
-| 1 | All Subjects | Continuous Runs | 0.14 | 0.17 | 0.14 | 0.2 | 0.15 | 0.19 |
-| 2 | All Subjects | Continuous Runs | 0.17 | 0.17 | 0.16 | 0.16 | 0.15 | 0.19 |
-| 3 | All Subjects | Continuous Runs | 0.15 | 0.2 | 0.14 | 0.18 | 0.17 | 0.17 |
-| 4 | All Subjects | Continuous Runs | 0.17 | 0.21 | 0.18 | 0.17 | 0.1 | 0.16 |
-| 5 | All Subjects | Continuous Runs | 0.14 | 0.19 | 0.14 | 0.16 | 0.2 | 0.18 |
-| 6 | All Subjects | Continuous Runs | 0.16 | 0.21 | 0.16 | 0.18 | 0.16 | 0.13 |
-| 7 | All Subjects | Continuous Runs | 0.16 | 0.16 | 0.17 | 0.15 | 0.19 | 0.17 |
-| 8 | All Subjects | Continuous Runs | 0.17 | 0.21 | 0.13 | 0.14 | 0.17 | 0.18 |
-| 9 | All Subjects | Continuous Runs | 0.18 | 0.1 | 0.17 | 0.18 | 0.16 | 0.2 |
-| 10 | All Subjects | Continuous Runs | 0.14 | 0.19 | 0.14 | 0.17 | 0.19 | 0.16 |
-
-# References
-[^1]: Liu, X., Zhang, N., Chang, C., & Duyn, J. H. (2018). Co-activation patterns in resting-state fMRI signals. NeuroImage, 180, 485–494. https://doi.org/10.1016/j.neuroimage.2018.01.041
-
-[^2]: Yang, H., Zhang, H., Di, X., Wang, S., Meng, C., Tian, L., & Biswal, B. (2021). Reproducible coactivation patterns of functional brain networks reveal the aberrant dynamic state transition in schizophrenia. NeuroImage, 237, 118193. https://doi.org/10.1016/j.neuroimage.2021.118193
-
-[^3]: Kupis, L., Romero, C., Dirks, B., Hoang, S., Parladé, M. V., Beaumont, A. L., Cardona, S. M., Alessandri, M., Chang, C., Nomi, J. S., & Uddin, L. Q. (2020). Evoked and intrinsic brain network dynamics in children with autism spectrum disorder. NeuroImage: Clinical, 28, 102396. https://doi.org/10.1016/j.nicl.2020.102396
-
+Metadata-Version: 2.1
+Name: neurocaps
+Version: 0.8.8.post4
+Summary: Co-activation patterns Python package
+Author-email: Donisha Smith <donishasmith@outlook.com>
+Project-URL: Homepage, https://github.com/donishadsmith/neurocaps
+Keywords: python,Co-Activation Patterns,CAPs,neuroimaging,fmri,dfc,dynamic functional connectivity,fMRIPrep
+Classifier: Intended Audience :: Education
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Operating System :: Microsoft :: Windows :: Windows 11
+Classifier: Development Status :: 4 - Beta
+Requires-Python: >=3.9.0
+Description-Content-Type: text/markdown
+License-File: LICENSE.md
+Requires-Dist: numpy
+Requires-Dist: pandas
+Requires-Dist: matplotlib
+Requires-Dist: seaborn
+Requires-Dist: kneed
+Requires-Dist: nilearn==0.10.2
+Requires-Dist: pybids; platform_system != "Windows"
+
+# neurocaps
+This is a Python package to perform Co-activation Patterns (CAPs) analyses, which involves using kmeans clustering to group timepoints (TR's) into brain states, on both resting-state or task data. It is compatible with data preprocessed with **fMRIPrep** and assumes your directory is BIDS-compliant and contains a derivatives folder with a pipeline folder, such as fMRIPrep, containing preprocessed BOLD data.
+
+**Still in beta but stable.**
+
+# Installation
+
+**Note**: The `.get_bold()` method in the `TimeseriesExtractor` class in this package uses pybids, which is only functional on POSIX operating system and Mac OS. Assuming you have a pickled timeseries dictionary in the proper nested form, this package can be used on windows to visualize the bold timeseries, use the `CAP` class, and the `merge_dicts()` fuction. 
+
+To install, using your preferred terminal:
+
+**Installation with pip:**
+
+```bash
+
+pip install neurocaps
+
+```
+
+**From source (Development version):**
+
+```bash
+pip install git+https://github.com/donishadsmith/neurocaps.git
+```
+
+or
+
+```bash
+
+git clone https://github.com/donishadsmith/neurocaps/
+cd neurocaps
+pip install -e .
+
+```
+
+# Usage
+ **This package contains two main classes - `TimeseriesExtractor`, for extracting the timeseries, and `CAP`, for performing the CAPs analysis.**
+
+**Note**: When extracting the timeseries, **this package uses the Schaefer atlas or the Automated Anatomical Labeling (AAL) atlas**. The number of ROIs and networks for the Schaefer atlas can be modified with the `parcel_approach` parameter when initializing the main `TimeseriesExtractor` class. To modify it, you must use a nested dictionary, where the primary key is "Schaefer" and the sub-keys are "n_rois" and "yeo_networks". Example: `parcel_approach = {"Schaefer": {"n_rois": 100, "yeo_networks": 7}}`. Similary the version of the AAL atlas can be modified using `parcel_approach = {"AAL": {"version": "SPM12"}}`.
+
+**Main features for `TimeseriesExtractor` includes:**
+
+- Timeseries extraction for resting state or task data and creating a nested dictionary containing the subject ID, run number, and associated timeseries. This is used as input for the `get_caps()` method in the `CAP` class.
+- Saving the nested dictionary containing timeseries as a pickle file.
+- Visualizing the timeseries of a Schaefer or AAL node or network subject's run. Also includes the ability to save plots.
+- Ability to use parallel processing by specifiying the number of CPU cores to use in the `n_cores` parameter in the `get_bold()` method. Testing on an HPC using a loop with `TimeseriesExtractor.get_bold()` to extract the session 1 and 2 bold timeries from 105 subjects from resting-state data (single-run containing 360 volumes) and two task datasets (three-runs containing 200 volumes each and two-runs containing 200 volumes) reduced processing time from 5 hrs 48 mins to 1 hr 26 mins (using 10 cores).
+
+**Main features for `CAP` includes:**
+
+- Performing the silhouette or elbow method to identify the optimal cluster size. When the optimal cluster size is identified, the optimal model is saved as an attribute.
+- Visualizing the CAPs identified as an outer product or regular heatmap. For outer products, you also have the ability to use subplots to reduce the number of individual plots. You can also save the plots and use them. Please refer to the docstring for the `visualize_caps()` method in the `CAP` class to see the list of available kwargs arguments to modify plots.
+- Grouping feature to perform CAPs independently on groups of subject IDs. When grouping is specified, k-means clustering, silhouette and elbow methods, as well as plotting, are done for each independent group.
+- Calculating CAP metrics as described in [Liu et al., 2018](https://doi.org/10.1016/j.neuroimage.2018.01.041)[^1] and [Yang et al., 2021](https://doi.org/10.1016/j.neuroimage.2021.118193)[^2], where *temporal fraction* is the proportion of total volumes spent in a single CAP over all volumes in a run, *persistence* is the average time spent in a single CAP before transitioning to another CAP (average consecutive/uninterrupted time), and *counts* is the frequency of each CAP observed in a run, and *transition frequency* is the number of switches between
+different CAPs across the entire run.
+
+**Additionally, the `neurocaps.analysis` submodule contains the `merge_dicts` function, which allows you to merge the subject_timeseries dictionaries (merged dictionary will be returned and can be saved as a pickle file) for overlapping subjects across tasks in order to identify similar CAPs across different tasks[^3].**
+
+Please refer to [demo.ipynb](https://github.com/donishadsmith/neurocaps/blob/main/demo.ipynb) to see a more extensive demonstration of the features included in this package. 
+
+Quick code example:
+
+```python
+
+from neurocaps.extraction import TimeseriesExtractor
+from neurocaps.analysis import CAP
+
+"""If an asterisk '*' is after a name, all confounds starting with the 
+term preceding the parameter will be used. in this case, all parameters 
+starting with cosine will be used."""
+confounds = ["cosine*", "trans_x", "trans_x_derivative1", "trans_y", 
+             "trans_y_derivative1", "trans_z","trans_z_derivative1", 
+             "rot_x", "rot_x_derivative1", "rot_y", "rot_y_derivative1", 
+             "rot_z","rot_z_derivative1"]
+
+"""If use_confounds is True but no confound_names provided, there are hardcoded 
+confound names that will extract the data from the confound files outputted by fMRIPrep
+`n_acompcor_separate` will use the first 'n' components derived from the separate 
+white-matter (WM) and cerebrospinal fluid (CSF). To use the acompcor components from the 
+combined mask, list them in the `confound_names` parameter"""
+parcel_approach = {"Schaefer": {"n_rois": 100, "yeo_networks": 7}}
+
+extractor = TimeseriesExtractor(parcel_approach=parcel_approach, standardize="zscore_sample",
+                                 use_confounds=True, detrend=True, low_pass=0.15, high_pass=0.01, 
+                                 confound_names=confounds, n_acompcor_separate=6)
+
+bids_dir = "/path/to/bids/dir"
+
+# If there are multiple pipelines in the derivatives folder, you can specify a specific pipeline
+pipeline_name = "fmriprep-1.4.0"
+
+# Resting State
+# extractor.get_bold(bids_dir=bids_dir, task="rest", pipeline_name=pipeline_name)
+
+# Task; use parallel processing with `n_cores`
+extractor.get_bold(bids_dir=bids_dir, task="emo", condition="positive", 
+                   pipeline_name=pipeline_name, n_cores=10)
+
+cap_analysis = CAP(parcel_approach=extractor.parcel_approach,
+                    n_clusters=6)
+
+cap_analysis.get_caps(subject_timeseries=extractor.subject_timeseries, 
+                      standardize = True)
+
+# Visualize CAPs
+cap_analysis.visualize_caps(visual_scope="networks", plot_options="outer product", 
+                            task_title="- Positive Valence", ncol=3, sharey=True, 
+                            subplots=True)
+
+cap_analysis.visualize_caps(visual_scope="nodes", plot_options="outer product", 
+                            task_title="- Positive Valence", ncol=3,sharey=True, 
+                            subplots=True, xlabel_rotation=90, tight_layout=False, 
+                            hspace = 0.4)
+
+# Get CAP metrics
+outputs = cap_analysis.calculate_metrics(subject_timeseries=extractor.subject_timeseries, tr=2.0, 
+                                         return_df=True, output_dir=output_dir,
+                                         metrics=["temporal fraction", "persistence"],
+                                         continuous_runs=True, file_name="All_Subjects_CAPs_metrics")
+
+print(outputs["temporal fraction"])
+
+```
+**Graph Outputs:**
+![image](https://github.com/donishadsmith/neurocaps/assets/112973674/4699bbd9-1f55-462b-9d9e-4ef17da79ad4)
+![image](https://github.com/donishadsmith/neurocaps/assets/112973674/506c5be5-540d-43a9-8a61-c02062f5c6f9)
+
+**DataFrame Output:**
+| Subject_ID | Group | Run | CAP-1 | CAP-2 | CAP-3 | CAP-4 | CAP-5 | CAP-6 |
+| --- | --- | --- | --- | --- | --- | --- | --- | --- |
+| 1 | All Subjects | Continuous Runs | 0.14 | 0.17 | 0.14 | 0.2 | 0.15 | 0.19 |
+| 2 | All Subjects | Continuous Runs | 0.17 | 0.17 | 0.16 | 0.16 | 0.15 | 0.19 |
+| 3 | All Subjects | Continuous Runs | 0.15 | 0.2 | 0.14 | 0.18 | 0.17 | 0.17 |
+| 4 | All Subjects | Continuous Runs | 0.17 | 0.21 | 0.18 | 0.17 | 0.1 | 0.16 |
+| 5 | All Subjects | Continuous Runs | 0.14 | 0.19 | 0.14 | 0.16 | 0.2 | 0.18 |
+| 6 | All Subjects | Continuous Runs | 0.16 | 0.21 | 0.16 | 0.18 | 0.16 | 0.13 |
+| 7 | All Subjects | Continuous Runs | 0.16 | 0.16 | 0.17 | 0.15 | 0.19 | 0.17 |
+| 8 | All Subjects | Continuous Runs | 0.17 | 0.21 | 0.13 | 0.14 | 0.17 | 0.18 |
+| 9 | All Subjects | Continuous Runs | 0.18 | 0.1 | 0.17 | 0.18 | 0.16 | 0.2 |
+| 10 | All Subjects | Continuous Runs | 0.14 | 0.19 | 0.14 | 0.17 | 0.19 | 0.16 |
+
+# Testing 
+This package was tested using a closed dataset as well as a modified version of a single subject open dataset to test the TimeseriesExtractor function on Github Actions. Furthermore, the open dataset provided by [Laumann & Poldrack](https://openfmri.org/dataset/ds000031/) and used in [Laumann et al., 2015](https://doi.org/10.1016/j.neuron.2015.06.037)[^4]. Additionally, this data was obtained from the OpenfMRI database. Its accession number is ds000031. Modifications to the data consist of truncating the preprocessed bold data and confounds form 448 timepoints to 34 timepoints, only including session 002 data, adding a dataset_description.json file to the fmriprep folder, excluding the nii.gz file in the root bids folder, only retaining the mask, truncated preprocessed bold file, and truncated confounds file in the fmriprep folder, and slighly changing the naming style of the mask, preprocessed bold file, and confounds file in the fmriprep folder ot conform with the naming conventions of modern fmriprep outputs.
+
+# References
+[^1]: Liu, X., Zhang, N., Chang, C., & Duyn, J. H. (2018). Co-activation patterns in resting-state fMRI signals. NeuroImage, 180, 485–494. https://doi.org/10.1016/j.neuroimage.2018.01.041
+
+[^2]: Yang, H., Zhang, H., Di, X., Wang, S., Meng, C., Tian, L., & Biswal, B. (2021). Reproducible coactivation patterns of functional brain networks reveal the aberrant dynamic state transition in schizophrenia. NeuroImage, 237, 118193. https://doi.org/10.1016/j.neuroimage.2021.118193
+
+[^3]: Kupis, L., Romero, C., Dirks, B., Hoang, S., Parladé, M. V., Beaumont, A. L., Cardona, S. M., Alessandri, M., Chang, C., Nomi, J. S., & Uddin, L. Q. (2020). Evoked and intrinsic brain network dynamics in children with autism spectrum disorder. NeuroImage: Clinical, 28, 102396. https://doi.org/10.1016/j.nicl.2020.102396
+
+[^4]: Laumann, T. O., Gordon, E. M., Adeyemo, B., Snyder, A. Z., Joo, S. J., Chen, M. Y., Gilmore, A. W., McDermott, K. B., Nelson, S. M., Dosenbach, N. U., Schlaggar, B. L., Mumford, J. A., Poldrack, R. A., & Petersen, S. E. (2015). Functional system and areal organization of a highly sampled individual human brain. Neuron, 87(3), 657–670. https://doi.org/10.1016/j.neuron.2015.06.037
```

### Comparing `neurocaps-0.8.8.post3/neurocaps/_utils/_cap_internals/_capgetter.py` & `neurocaps-0.8.8.post4/neurocaps/_utils/_cap_internals/_capgetter.py`

 * *Files identical despite different names*

### Comparing `neurocaps-0.8.8.post3/neurocaps/_utils/_check_confound_names.py` & `neurocaps-0.8.8.post4/neurocaps/_utils/_check_confound_names.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,10 +30,10 @@
     if n_acompcor_separate:
         check_confounds = [confound for confound in confound_names if "a_comp_cor" not in confound]
         if len(confound_names) > len(check_confounds):
             removed_confounds = [element for element in confound_names if element not in check_confounds]
             if specified_confound_names: warnings.warn(f"Since `n_acompcor_separate` has been specified, specified acompcor components in `confound_names` will be disregarded and replaced with the first {n_acompcor_separate} components of the white matter and cerebrospinal fluid masks for each participant. The following components will not be used {removed_confounds}")
             confound_names = check_confounds 
     
-    print(f"List of confound regressors that will be used during timeseries extraction if available in confound dataframe: {confound_names}")
+    print(f"List of confound regressors that will be used during timeseries extraction if available in confound dataframe: {confound_names}", flush=True)
     
     return confound_names
```

### Comparing `neurocaps-0.8.8.post3/neurocaps/_utils/_timeseriesextractor_internals/_check_parcel_approach.py` & `neurocaps-0.8.8.post4/neurocaps/_utils/_timeseriesextractor_internals/_check_parcel_approach.py`

 * *Files identical despite different names*

### Comparing `neurocaps-0.8.8.post3/neurocaps/_utils/_timeseriesextractor_internals/_extract_timeseries.py` & `neurocaps-0.8.8.post4/neurocaps/_utils/_timeseriesextractor_internals/_extract_timeseries.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-def _extract_timeseries(subj_id, nifti_files, mask_files, event_files, confound_files, confound_metadata_files, run_list, tr, condition, parcel_approach, signal_clean_info):
+def _extract_timeseries(subj_id, nifti_files, mask_files, event_files, confound_files, confound_metadata_files, run_list, tr, condition, parcel_approach, signal_clean_info, verbose, flush_print):
 
     from nilearn.maskers import NiftiLabelsMasker
     from nilearn.image import index_img, load_img
     import pandas as pd, json, math, copy, warnings
 
     # Intitialize subject dictionary
     subject_timeseries = {subj_id: {}}
@@ -11,15 +11,15 @@
 
         # Get files from specific run
         nifti_file = [nifti_file for nifti_file in nifti_files if run in nifti_file]
         mask_file = [mask_file for mask_file in mask_files if run in mask_file]
         confound_file = [confound_file for confound_file in confound_files if run in confound_file] if signal_clean_info["use_confounds"] else None
         confound_metadata_file = [confound_metadata_file for confound_metadata_file in confound_metadata_files if run in confound_metadata_file] if signal_clean_info["use_confounds"] and signal_clean_info["n_acompcor_separate"] else None
 
-        print(f"Running subject: {subj_id}; {run}; \n {nifti_file}")
+        if verbose: print(f"Running subject: {subj_id}; {run}; \n {nifti_file}", flush=flush_print)
 
         confound_df = pd.read_csv(confound_file[0], sep="\t") if signal_clean_info["use_confounds"] else None
 
         event_file = None if len(event_files) == 0 else [event_file for event_file in event_files if run in event_file]
 
         # Extract confound information of interest and ensure confound file does not contain NAs
         if signal_clean_info["use_confounds"]:
@@ -44,19 +44,20 @@
                     confounds_list = [col for col in confound_df.columns if col.startswith(prefix)]
                 else:
                     confounds_list = [col for col in confound_df.columns if col == confound_name] 
             
                 if len(confounds_list) > 0: valid_confounds.extend(confounds_list)
                 else: invalid_confounds.extend([confound_name])
 
-            if len(invalid_confounds) > 0: print(f"Subject {subj_id} did not have the following confounds: {invalid_confounds}")
+            if len(invalid_confounds) > 0: 
+                if verbose: print(f"Subject {subj_id} did not have the following confounds: {invalid_confounds}", flush=flush_print)
 
             confounds = confound_df[valid_confounds]
             confounds = confounds.fillna(0)
-            print(f"Confounds used for subject: {subj_id}; {run} - {confounds.columns}")
+            if verbose: print(f"Confounds used for subject: {subj_id}; {run} - {confounds.columns}", flush=flush_print)
 
         # Create the masker for extracting time series
         masker = NiftiLabelsMasker(
             mask_img=mask_file[0],
             labels_img=parcel_approach[list(parcel_approach.keys())[0]]["maps"], 
             labels=parcel_approach[list(parcel_approach.keys())[0]]["labels"], 
             resampling_target='data',
```

### Comparing `neurocaps-0.8.8.post3/neurocaps/_utils/_timeseriesextractor_internals/_timeseriesextractorgetter.py` & `neurocaps-0.8.8.post4/neurocaps/_utils/_timeseriesextractor_internals/_timeseriesextractorgetter.py`

 * *Files identical despite different names*

### Comparing `neurocaps-0.8.8.post3/neurocaps/analysis/cap.py` & `neurocaps-0.8.8.post4/neurocaps/analysis/cap.py`

 * *Files identical despite different names*

### Comparing `neurocaps-0.8.8.post3/neurocaps/analysis/merge.py` & `neurocaps-0.8.8.post4/neurocaps/analysis/merge.py`

 * *Files identical despite different names*

### Comparing `neurocaps-0.8.8.post3/neurocaps/extraction/timeseriesextractor.py` & `neurocaps-0.8.8.post4/neurocaps/extraction/timeseriesextractor.py`

 * *Files 5% similar despite different names*

```diff
@@ -51,26 +51,27 @@
 
         # Check parcel_apprach
         self._parcel_approach = _check_parcel_approach(parcel_approach=parcel_approach)
 
         if self._signal_clean_info["use_confounds"]:
             self._signal_clean_info["confound_names"] = _check_confound_names(high_pass=high_pass, specified_confound_names=confound_names, n_acompcor_separate=n_acompcor_separate)
             
-    def get_bold(self, bids_dir: str, session: int, runs: list[int]=None, task: str="rest", condition: str=None, tr: Union[int, float]=None, run_subjects: list[str]=None, exclude_subjects: list[str]= None, pipeline_name: str=None, n_cores: Union[bool, int]=None) -> None: 
+    def get_bold(self, bids_dir: str, session: Union[int,str]=None, runs: list[int]=None, task: str="rest", condition: str=None, tr: Union[int, float]=None, 
+                 run_subjects: list[str]=None, exclude_subjects: list[str]= None, pipeline_name: str=None, n_cores: Union[bool, int]=None, verbose: bool=True, flush_print: bool=False) -> None: 
         """Get Bold Data
 
         Collects files needed to extract timeseries data from NIfTI files for BIDS-compliant datasets.
 
         Parameters
         ----------
         bids_dir : str
             Path to a BIDS compliant directory. 
-        session : int
+        session : int, default=None
             Session to extract timeseries from. Only a single session can be extracted at a time. 
-        runs : list[int]
+        runs : list[int], default=None
             Run number to extract timeseries data from. Extracts all runs if unspecified.
         task : str, default="rest"
             Task name.
         condition : str, default=None
             Specific condition in the task to extract from. Only a single condition can be extracted at a time.
         tr : int or float, default=None
             Repetition time.
@@ -79,14 +80,18 @@
         exclude_subjects : List[str], default=None
             List of subject IDs to exclude.  
         pipeline_name: str, default=None
             The name of the pipeline folder in the derivatives folder containing the preprocessed data. If None, BIDSLayout will use the name of dset_dir with derivatives=True. This parameter
             should be used if their are multiple pipelines in the derivatives folder.
         n_cores: bool or int, default=None
             The number of CPU cores to use for multiprocessing. If true, all available cores will be used.
+        verbose: bool, default=True
+            Print subject specific information such as confounds being extracted and id and run of subject being processed during timeseries extraction.
+        flush_print: bool, default=False
+            Flush the printed subject specific infomation produced during the timeseries extraction process.
         """
         import bids, multiprocessing
 
         if sys.platform == "win32":
             raise SystemError("Cannot use this method on Windows devices since it relies on the `pybids` module which is only compatable with POSIX systems.")
 
         # Update attributes
@@ -98,16 +103,16 @@
         self._subject_info = {}
 
         if pipeline_name:
             layout = bids.BIDSLayout(bids_dir, derivatives=os.path.join(bids_dir, "derivatives", pipeline_name))
         else:
             layout = bids.BIDSLayout(bids_dir, derivatives=True)
 
-        print(f"Bids layout collected.")
-
+        print(f"Bids layout collected.", flush=True)
+        print(layout, flush=True)
         subj_id_list = sorted(layout.get(return_type="id", target="subject", task=task, space=self._space, suffix="bold")) 
 
         if exclude_subjects: 
             exclude_subjects = [str(subj_id) if not isinstance(subj_id,str) else subj_id for subj_id in exclude_subjects]
             subj_id_list = sorted([subj_id for subj_id in subj_id_list if subj_id not in exclude_subjects])
 
         if run_subjects: 
@@ -125,15 +130,15 @@
                     raise ValueError(f"More cores specified than available - Number of cores specified: {n_cores}; Max cores available: {multiprocessing.cpu_count()}")
                 else:
                     self._n_cores = n_cores
             
             # Generate list of tuples for each subject
             args_list = [(subj_id, self._subject_info[subj_id]["nifti_files"],self._subject_info[subj_id]["mask_files"],self._subject_info[subj_id]["event_files"],
                           self._subject_info[subj_id]["confound_files"], self._subject_info[subj_id]["confound_metadata_files"], self._subject_info[subj_id]["run_list"],
-                          self._subject_info[subj_id]["tr"], condition, self._parcel_approach, self._signal_clean_info
+                          self._subject_info[subj_id]["tr"], condition, self._parcel_approach, self._signal_clean_info, verbose, flush_print
                           ) for subj_id in self._subject_ids]
 
             with multiprocessing.Pool(processes=self._n_cores) as pool:
                 outputs = pool.starmap(_extract_timeseries, args_list)
             
             for output in outputs:
                 if isinstance(output, dict):
@@ -146,15 +151,16 @@
             pool.close()
         else:
             for subj_id in self._subject_ids:
 
                 subject_timeseries=_extract_timeseries(subj_id=subj_id, nifti_files=self._subject_info[subj_id]["nifti_files"], mask_files=self._subject_info[subj_id]["mask_files"], 
                                                        event_files=self._subject_info[subj_id]["event_files"], confound_files=self._subject_info[subj_id]["confound_files"],
                                                        confound_metadata_files=self._subject_info[subj_id]["confound_metadata_files"], run_list=self._subject_info[subj_id]["run_list"], 
-                                                       tr=self._subject_info[subj_id]["tr"], condition=condition, parcel_approach=self._parcel_approach, signal_clean_info=self._signal_clean_info)
+                                                       tr=self._subject_info[subj_id]["tr"], condition=condition, parcel_approach=self._parcel_approach, signal_clean_info=self._signal_clean_info,
+                                                       verbose=verbose, flush_print=flush_print)
             
                 # Aggregate new timeseries
                 if isinstance(subject_timeseries, dict): self._subject_timeseries.update(subject_timeseries)
         
     # Get valid subjects to iterate through
     def _setup_extraction(self, layout, subj_id_list):
        for subj_id in subj_id_list:
@@ -205,15 +211,15 @@
                     continue
                 else: warnings.warn(f"Subject: {subj_id} only has the following runs available: {', '.join(run_list)}")
 
             # Add subject list to subject attribute. These are subjects that will be ran
             self._subject_ids.append(subj_id)
 
             # Get repetition time for the subject
-            tr = tr if self._task_info["tr"] else json.load(open(bold_metadata_files[0]))["RepetitionTime"]
+            tr = self._task_info["tr"] if self._task_info["tr"] else json.load(open(bold_metadata_files[0]))["RepetitionTime"]
 
             # Store subject specific information
             self._subject_info[subj_id] = {"nifti_files": nifti_files, "event_files": event_files, "confound_files": confound_files, "confound_metadata_files": confound_metadata_files, "mask_files": mask_files,
                                            "tr": tr, "run_list": run_list}
 
     def timeseries_to_pickle(self, output_dir: str, file_name: str):
         """Save Bold Data
```

### Comparing `neurocaps-0.8.8.post3/neurocaps.egg-info/PKG-INFO` & `neurocaps-0.8.8.post4/neurocaps.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neurocaps
-Version: 0.8.8.post3
+Version: 0.8.8.post4
 Summary: Co-activation patterns Python package
 Author-email: Donisha Smith <donishasmith@outlook.com>
 Project-URL: Homepage, https://github.com/donishadsmith/neurocaps
 Keywords: python,Co-Activation Patterns,CAPs,neuroimaging,fmri,dfc,dynamic functional connectivity,fMRIPrep
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -90,15 +90,15 @@
 
 from neurocaps.extraction import TimeseriesExtractor
 from neurocaps.analysis import CAP
 
 """If an asterisk '*' is after a name, all confounds starting with the 
 term preceding the parameter will be used. in this case, all parameters 
 starting with cosine will be used."""
-confounds = ["cosine*", "non_steady_state*", "trans_x", "trans_x_derivative1", "trans_y", 
+confounds = ["cosine*", "trans_x", "trans_x_derivative1", "trans_y", 
              "trans_y_derivative1", "trans_z","trans_z_derivative1", 
              "rot_x", "rot_x_derivative1", "rot_y", "rot_y_derivative1", 
              "rot_z","rot_z_derivative1"]
 
 """If use_confounds is True but no confound_names provided, there are hardcoded 
 confound names that will extract the data from the confound files outputted by fMRIPrep
 `n_acompcor_separate` will use the first 'n' components derived from the separate 
@@ -161,14 +161,18 @@
 | 5 | All Subjects | Continuous Runs | 0.14 | 0.19 | 0.14 | 0.16 | 0.2 | 0.18 |
 | 6 | All Subjects | Continuous Runs | 0.16 | 0.21 | 0.16 | 0.18 | 0.16 | 0.13 |
 | 7 | All Subjects | Continuous Runs | 0.16 | 0.16 | 0.17 | 0.15 | 0.19 | 0.17 |
 | 8 | All Subjects | Continuous Runs | 0.17 | 0.21 | 0.13 | 0.14 | 0.17 | 0.18 |
 | 9 | All Subjects | Continuous Runs | 0.18 | 0.1 | 0.17 | 0.18 | 0.16 | 0.2 |
 | 10 | All Subjects | Continuous Runs | 0.14 | 0.19 | 0.14 | 0.17 | 0.19 | 0.16 |
 
+# Testing 
+This package was tested using a closed dataset as well as a modified version of a single subject open dataset to test the TimeseriesExtractor function on Github Actions. Furthermore, the open dataset provided by [Laumann & Poldrack](https://openfmri.org/dataset/ds000031/) and used in [Laumann et al., 2015](https://doi.org/10.1016/j.neuron.2015.06.037)[^4]. Additionally, this data was obtained from the OpenfMRI database. Its accession number is ds000031. Modifications to the data consist of truncating the preprocessed bold data and confounds form 448 timepoints to 34 timepoints, only including session 002 data, adding a dataset_description.json file to the fmriprep folder, excluding the nii.gz file in the root bids folder, only retaining the mask, truncated preprocessed bold file, and truncated confounds file in the fmriprep folder, and slighly changing the naming style of the mask, preprocessed bold file, and confounds file in the fmriprep folder ot conform with the naming conventions of modern fmriprep outputs.
+
 # References
 [^1]: Liu, X., Zhang, N., Chang, C., & Duyn, J. H. (2018). Co-activation patterns in resting-state fMRI signals. NeuroImage, 180, 485–494. https://doi.org/10.1016/j.neuroimage.2018.01.041
 
 [^2]: Yang, H., Zhang, H., Di, X., Wang, S., Meng, C., Tian, L., & Biswal, B. (2021). Reproducible coactivation patterns of functional brain networks reveal the aberrant dynamic state transition in schizophrenia. NeuroImage, 237, 118193. https://doi.org/10.1016/j.neuroimage.2021.118193
 
 [^3]: Kupis, L., Romero, C., Dirks, B., Hoang, S., Parladé, M. V., Beaumont, A. L., Cardona, S. M., Alessandri, M., Chang, C., Nomi, J. S., & Uddin, L. Q. (2020). Evoked and intrinsic brain network dynamics in children with autism spectrum disorder. NeuroImage: Clinical, 28, 102396. https://doi.org/10.1016/j.nicl.2020.102396
 
+[^4]: Laumann, T. O., Gordon, E. M., Adeyemo, B., Snyder, A. Z., Joo, S. J., Chen, M. Y., Gilmore, A. W., McDermott, K. B., Nelson, S. M., Dosenbach, N. U., Schlaggar, B. L., Mumford, J. A., Poldrack, R. A., & Petersen, S. E. (2015). Functional system and areal organization of a highly sampled individual human brain. Neuron, 87(3), 657–670. https://doi.org/10.1016/j.neuron.2015.06.037
```

### Comparing `neurocaps-0.8.8.post3/neurocaps.egg-info/SOURCES.txt` & `neurocaps-0.8.8.post4/neurocaps.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -18,8 +18,9 @@
 neurocaps/_utils/_timeseriesextractor_internals/_timeseriesextractorgetter.py
 neurocaps/analysis/__init__.py
 neurocaps/analysis/cap.py
 neurocaps/analysis/merge.py
 neurocaps/extraction/__init__.py
 neurocaps/extraction/timeseriesextractor.py
 tests/test_CAP.py
+tests/test_TimeseriesExtractor.py
 tests/test_merge_dicts.py
```

### Comparing `neurocaps-0.8.8.post3/pyproject.toml` & `neurocaps-0.8.8.post4/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "neurocaps"
-version = "0.8.8post3"
+version = "0.8.8post4"
 authors = [{name = "Donisha Smith", email = "donishasmith@outlook.com"}]
 description = "Co-activation patterns Python package"
 readme = "README.md"
 requires-python = ">=3.9.0"
 keywords = ["python", "Co-Activation Patterns", "CAPs", "neuroimaging", "fmri", "dfc", "dynamic functional connectivity", "fMRIPrep"]
 classifiers = [
     "Intended Audience :: Education",
```

### Comparing `neurocaps-0.8.8.post3/tests/test_CAP.py` & `neurocaps-0.8.8.post4/tests/test_CAP.py`

 * *Files identical despite different names*

### Comparing `neurocaps-0.8.8.post3/tests/test_merge_dicts.py` & `neurocaps-0.8.8.post4/tests/test_merge_dicts.py`

 * *Files identical despite different names*


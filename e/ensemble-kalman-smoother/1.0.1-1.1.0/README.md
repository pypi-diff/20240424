# Comparing `tmp/ensemble-kalman-smoother-1.0.1.tar.gz` & `tmp/ensemble-kalman-smoother-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ensemble-kalman-smoother-1.0.1.tar", last modified: Tue Apr  9 16:03:12 2024, max compression
+gzip compressed data, was "ensemble-kalman-smoother-1.1.0.tar", last modified: Wed Apr 24 13:47:19 2024, max compression
```

## Comparing `ensemble-kalman-smoother-1.0.1.tar` & `ensemble-kalman-smoother-1.1.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 mattw     (1000) mattw     (1000)        0 2024-04-09 16:03:12.963881 ensemble-kalman-smoother-1.0.1/
--rw-r--r--   0 mattw     (1000) mattw     (1000)     1069 2023-03-23 13:30:16.000000 ensemble-kalman-smoother-1.0.1/LICENSE
--rw-rw-r--   0 mattw     (1000) mattw     (1000)     4261 2024-04-09 16:03:12.963881 ensemble-kalman-smoother-1.0.1/PKG-INFO
--rw-r--r--   0 mattw     (1000) mattw     (1000)     3927 2024-04-09 15:43:27.000000 ensemble-kalman-smoother-1.0.1/README.md
-drwxrwxr-x   0 mattw     (1000) mattw     (1000)        0 2024-04-09 16:03:12.963881 ensemble-kalman-smoother-1.0.1/eks/
--rw-r--r--   0 mattw     (1000) mattw     (1000)       41 2024-04-09 15:36:45.000000 ensemble-kalman-smoother-1.0.1/eks/__init__.py
--rw-rw-r--   0 mattw     (1000) mattw     (1000)     8375 2024-04-09 13:14:04.000000 ensemble-kalman-smoother-1.0.1/eks/ensemble_kalman.py
--rw-rw-r--   0 mattw     (1000) mattw     (1000)    26528 2024-04-09 13:14:04.000000 ensemble-kalman-smoother-1.0.1/eks/multiview_pca_smoother.py
--rw-rw-r--   0 mattw     (1000) mattw     (1000)     9911 2024-04-09 13:14:04.000000 ensemble-kalman-smoother-1.0.1/eks/pupil_smoother.py
--rw-rw-r--   0 mattw     (1000) mattw     (1000)     4444 2024-04-09 13:14:04.000000 ensemble-kalman-smoother-1.0.1/eks/singleview_smoother.py
--rw-rw-r--   0 mattw     (1000) mattw     (1000)      719 2024-04-09 13:14:04.000000 ensemble-kalman-smoother-1.0.1/eks/utils.py
-drwxrwxr-x   0 mattw     (1000) mattw     (1000)        0 2024-04-09 16:03:12.963881 ensemble-kalman-smoother-1.0.1/ensemble_kalman_smoother.egg-info/
--rw-rw-r--   0 mattw     (1000) mattw     (1000)     4261 2024-04-09 16:03:12.000000 ensemble-kalman-smoother-1.0.1/ensemble_kalman_smoother.egg-info/PKG-INFO
--rw-rw-r--   0 mattw     (1000) mattw     (1000)      396 2024-04-09 16:03:12.000000 ensemble-kalman-smoother-1.0.1/ensemble_kalman_smoother.egg-info/SOURCES.txt
--rw-rw-r--   0 mattw     (1000) mattw     (1000)        1 2024-04-09 16:03:12.000000 ensemble-kalman-smoother-1.0.1/ensemble_kalman_smoother.egg-info/dependency_links.txt
--rw-rw-r--   0 mattw     (1000) mattw     (1000)      201 2024-04-09 16:03:12.000000 ensemble-kalman-smoother-1.0.1/ensemble_kalman_smoother.egg-info/requires.txt
--rw-rw-r--   0 mattw     (1000) mattw     (1000)        4 2024-04-09 16:03:12.000000 ensemble-kalman-smoother-1.0.1/ensemble_kalman_smoother.egg-info/top_level.txt
--rw-rw-r--   0 mattw     (1000) mattw     (1000)       38 2024-04-09 16:03:12.963881 ensemble-kalman-smoother-1.0.1/setup.cfg
--rw-r--r--   0 mattw     (1000) mattw     (1000)     1514 2024-04-09 16:02:54.000000 ensemble-kalman-smoother-1.0.1/setup.py
+drwxrwxr-x   0 mattw     (1000) mattw     (1000)        0 2024-04-24 13:47:19.644703 ensemble-kalman-smoother-1.1.0/
+-rw-rw-r--   0 mattw     (1000) mattw     (1000)     1069 2023-03-23 13:30:16.000000 ensemble-kalman-smoother-1.1.0/LICENSE
+-rw-rw-r--   0 mattw     (1000) mattw     (1000)     4353 2024-04-24 13:47:19.644703 ensemble-kalman-smoother-1.1.0/PKG-INFO
+-rw-rw-r--   0 mattw     (1000) mattw     (1000)     4055 2024-04-24 13:44:17.000000 ensemble-kalman-smoother-1.1.0/README.md
+drwxrwxr-x   0 mattw     (1000) mattw     (1000)        0 2024-04-24 13:47:19.644703 ensemble-kalman-smoother-1.1.0/eks/
+-rw-rw-r--   0 mattw     (1000) mattw     (1000)       41 2024-04-24 13:44:31.000000 ensemble-kalman-smoother-1.1.0/eks/__init__.py
+-rw-rw-r--   0 mattw     (1000) mattw     (1000)    13880 2024-04-24 13:44:17.000000 ensemble-kalman-smoother-1.1.0/eks/core.py
+-rw-rw-r--   0 mattw     (1000) mattw     (1000)    27285 2024-04-24 13:44:17.000000 ensemble-kalman-smoother-1.1.0/eks/multiview_pca_smoother.py
+-rw-rw-r--   0 mattw     (1000) mattw     (1000)     9911 2024-04-24 13:44:17.000000 ensemble-kalman-smoother-1.1.0/eks/pupil_smoother.py
+-rw-rw-r--   0 mattw     (1000) mattw     (1000)     5558 2024-04-24 13:44:17.000000 ensemble-kalman-smoother-1.1.0/eks/singleview_smoother.py
+-rw-rw-r--   0 mattw     (1000) mattw     (1000)     2805 2024-04-24 13:44:17.000000 ensemble-kalman-smoother-1.1.0/eks/utils.py
+drwxrwxr-x   0 mattw     (1000) mattw     (1000)        0 2024-04-24 13:47:19.644703 ensemble-kalman-smoother-1.1.0/ensemble_kalman_smoother.egg-info/
+-rw-r--r--   0 mattw     (1000) mattw     (1000)     4353 2024-04-24 13:47:19.000000 ensemble-kalman-smoother-1.1.0/ensemble_kalman_smoother.egg-info/PKG-INFO
+-rw-r--r--   0 mattw     (1000) mattw     (1000)      395 2024-04-24 13:47:19.000000 ensemble-kalman-smoother-1.1.0/ensemble_kalman_smoother.egg-info/SOURCES.txt
+-rw-r--r--   0 mattw     (1000) mattw     (1000)        1 2024-04-24 13:47:19.000000 ensemble-kalman-smoother-1.1.0/ensemble_kalman_smoother.egg-info/dependency_links.txt
+-rw-r--r--   0 mattw     (1000) mattw     (1000)      201 2024-04-24 13:47:19.000000 ensemble-kalman-smoother-1.1.0/ensemble_kalman_smoother.egg-info/requires.txt
+-rw-r--r--   0 mattw     (1000) mattw     (1000)        4 2024-04-24 13:47:19.000000 ensemble-kalman-smoother-1.1.0/ensemble_kalman_smoother.egg-info/top_level.txt
+-rw-rw-r--   0 mattw     (1000) mattw     (1000)      220 2024-04-24 13:47:19.644703 ensemble-kalman-smoother-1.1.0/setup.cfg
+-rw-rw-r--   0 mattw     (1000) mattw     (1000)     1514 2024-04-24 13:44:14.000000 ensemble-kalman-smoother-1.1.0/setup.py
```

### Comparing `ensemble-kalman-smoother-1.0.1/LICENSE` & `ensemble-kalman-smoother-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ensemble-kalman-smoother-1.0.1/PKG-INFO` & `ensemble-kalman-smoother-1.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: ensemble-kalman-smoother
-Version: 1.0.1
+Version: 1.1.0
 Summary: Ensembling and kalman smoothing for pose estimation
 Home-page: http://www.github.com/colehurwitz/eks
 Author: Cole Hurwitz
 Author-email: 
-License: UNKNOWN
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # EKS
 This repo contains code to run an Ensemble Kalman Smoother (EKS) for improving pose estimation outputs. 
 
@@ -59,22 +57,23 @@
 pip install -e ".[dev]"
 ```
 
 ### Method 2: pip
 
 You can also install the `eks` package using the Python Package Index (PyPI):
 ```
-python3 -m pip install eks
+python3 -m pip install ensemble-kalman-smoother
 ```
 Note that you will not have access to the example data or example scripts with the pip install 
 option.
 
 ## Example scripts
 
-We provide several example datasets and fitting scripts to illustrate use of the package.
+We provide several example datasets and fitting scripts to illustrate use of the package. See
+[Command-Line Arguments](docs/command-line_arguments.md) for more information on arguments.
 
 ### Single-camera datasets
 The `singlecam_example.py` script demonstrates how to run the EKS code for standard single-camera
 setups. 
 Any of the provided datasets are compatible with this script; below we'll use `data/ibl-pupil` as
 our example. 
 To run the EKS on the example data, execute the following command from inside this repo:
@@ -117,8 +116,8 @@
 ```
 
 ### Authors 
 Cole Hurwitz
 
 Matt Whiteway
 
-
+Keemin Lee
```

### Comparing `ensemble-kalman-smoother-1.0.1/README.md` & `ensemble-kalman-smoother-1.1.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -46,22 +46,23 @@
 pip install -e ".[dev]"
 ```
 
 ### Method 2: pip
 
 You can also install the `eks` package using the Python Package Index (PyPI):
 ```
-python3 -m pip install eks
+python3 -m pip install ensemble-kalman-smoother
 ```
 Note that you will not have access to the example data or example scripts with the pip install 
 option.
 
 ## Example scripts
 
-We provide several example datasets and fitting scripts to illustrate use of the package.
+We provide several example datasets and fitting scripts to illustrate use of the package. See
+[Command-Line Arguments](docs/command-line_arguments.md) for more information on arguments.
 
 ### Single-camera datasets
 The `singlecam_example.py` script demonstrates how to run the EKS code for standard single-camera
 setups. 
 Any of the provided datasets are compatible with this script; below we'll use `data/ibl-pupil` as
 our example. 
 To run the EKS on the example data, execute the following command from inside this repo:
@@ -103,7 +104,9 @@
 python scripts/multiview_paw_example.py --csv-dir ./data/ibl-paw
 ```
 
 ### Authors 
 Cole Hurwitz
 
 Matt Whiteway
+
+Keemin Lee
```

### Comparing `ensemble-kalman-smoother-1.0.1/eks/multiview_pca_smoother.py` & `ensemble-kalman-smoother-1.1.0/eks/multiview_pca_smoother.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,43 +1,51 @@
 import numpy as np
 import pandas as pd
 from scipy.interpolate import interp1d
 from sklearn.decomposition import PCA
 from eks.utils import make_dlc_pandas_index
-from eks.ensemble_kalman import ensemble, filtering_pass, kalman_dot, smooth_backward, eks_zscore
+from eks.core import ensemble, forward_pass, \
+    backward_pass, eks_zscore, optimize_smoothing_param, filter_smooth_nll
 
 
 # -----------------------
 # funcs for kalman paw
 # -----------------------
 def remove_camera_means(ensemble_stacks, camera_means):
     scaled_ensemble_stacks = ensemble_stacks.copy()
     for k in range(len(ensemble_stacks)):
         for camera_id, camera_mean in enumerate(camera_means):
-            scaled_ensemble_stacks[k][:,camera_id] = ensemble_stacks[k][:,camera_id] - camera_mean
+            scaled_ensemble_stacks[k][:, camera_id] = \
+                ensemble_stacks[k][:, camera_id] - camera_mean
     return scaled_ensemble_stacks
 
 
 def add_camera_means(ensemble_stacks, camera_means):
     scaled_ensemble_stacks = ensemble_stacks.copy()
     for k in range(len(ensemble_stacks)):
         for camera_id, camera_mean in enumerate(camera_means):
-            scaled_ensemble_stacks[k][:,camera_id] = ensemble_stacks[k][:,camera_id] + camera_mean
+            scaled_ensemble_stacks[k][:, camera_id] = \
+                ensemble_stacks[k][:, camera_id] + camera_mean
     return scaled_ensemble_stacks
 
 
 def pca(S, n_comps):
     pca_ = PCA(n_components=n_comps)
     return pca_.fit(S), pca_.explained_variance_ratio_
 
 
 def ensemble_kalman_smoother_paw_asynchronous(
         markers_list_left_cam, markers_list_right_cam, timestamps_left_cam,
-        timestamps_right_cam, keypoint_names, smooth_param, quantile_keep_pca, ensembling_mode='median', zscore_threshold=2, img_width=128):
-    """--(IBL-specific)- -Use multi-view constraints to fit a 3d latent subspace for each body part with 2 ansynchronous cameras.
+        timestamps_right_cam, keypoint_names, smooth_param, quantile_keep_pca,
+        ensembling_mode='median',
+        zscore_threshold=2, img_width=128):
+    """
+    --(IBL-specific)-
+    -Use multi-view constraints to fit a 3d latent subspace for each body part with 2
+    asynchronous cameras.
 
     Parameters
     ----------
     markers_list_left_cam : list of pd.DataFrames
         each list element is a dataframe of predictions from one ensemble member (left view)
     markers_list_right_cam : list of pd.DataFrames
         each list element is a dataframe of predictions from one ensemble member (right view)
@@ -50,15 +58,16 @@
     smooth_param : float
         ranges from .01-2 (smaller values = more smoothing)
     quantile_keep_pca
         percentage of the points are kept for multi-view PCA (lowest ensemble variance)
     ensembling_mode:
         the function used for ensembling ('mean', 'median', or 'confidence_weighted_mean')
     zscore_threshold:
-        Minimum std threshold to reduce the effect of low ensemble std on a zscore metric (default 2).
+        Minimum std threshold to reduce the effect of low ensemble std on a zscore metric
+        (default 2).
     img_width
         The width of the image being smoothed (128 default, IBL-specific).
     Returns
     -------
 
     Returns
     -------
@@ -111,18 +120,24 @@
 
     markers_list_right_cam = []
     for k in range(len(markers_list_interp[1])):
         markers_right_cam = pd.DataFrame(markers_list_interp[1][k], columns=keys)
         markers_list_right_cam.append(markers_right_cam)
 
     # compute ensemble median left camera
-    left_cam_ensemble_preds, left_cam_ensemble_vars, left_cam_ensemble_stacks, left_cam_keypoints_mean_dict, left_cam_keypoints_var_dict, left_cam_keypoints_stack_dict =  ensemble(markers_list_left_cam, keys, mode=ensembling_mode)
+    left_cam_ensemble_preds, left_cam_ensemble_vars, left_cam_ensemble_stacks, \
+        left_cam_keypoints_mean_dict, left_cam_keypoints_var_dict, \
+        left_cam_keypoints_stack_dict = \
+        ensemble(markers_list_left_cam, keys, mode=ensembling_mode)
 
     # compute ensemble median right camera
-    right_cam_ensemble_preds, right_cam_ensemble_vars, right_cam_ensemble_stacks, right_cam_keypoints_mean_dict, right_cam_keypoints_var_dict, right_cam_keypoints_stack_dict = ensemble(markers_list_right_cam, keys, mode=ensembling_mode)
+    right_cam_ensemble_preds, right_cam_ensemble_vars, right_cam_ensemble_stacks, \
+        right_cam_keypoints_mean_dict, right_cam_keypoints_var_dict, \
+        right_cam_keypoints_stack_dict = \
+        ensemble(markers_list_right_cam, keys, mode=ensembling_mode)
 
     # ensemble_stacked = np.median(markers_list_stacked_interp, 0)
     # ensemble_stacked_vars = np.var(markers_list_stacked_interp, 0)
 
     # keep percentage of the points for multi-view PCA based lowest ensemble variance
     hstacked_vars = np.hstack((left_cam_ensemble_vars, right_cam_ensemble_vars))
     max_vars = np.max(hstacked_vars, 1)
@@ -177,31 +192,31 @@
     mean_camera_l_y = good_stacked_ensemble_preds[:, 1].mean()
     mean_camera_r_x = good_stacked_ensemble_preds[:, 2].mean()
     mean_camera_r_y = good_stacked_ensemble_preds[:, 3].mean()
     means_camera = [mean_camera_l_x, mean_camera_l_y, mean_camera_r_x, mean_camera_r_y]
 
     left_paw_ensemble_stacks = np.concatenate(
         (left_cam_ensemble_stacks[:, :, :2], right_cam_ensemble_stacks[:, :, :2]), 2)
-    scaled_left_paw_ensemble_stacks = remove_camera_means(
-        left_paw_ensemble_stacks, means_camera)
+
+    remove_camera_means(left_paw_ensemble_stacks, means_camera)
 
     right_paw_ensemble_stacks = np.concatenate(
         (right_cam_ensemble_stacks[:, :, :2], right_cam_ensemble_stacks[:, :, :2]), 2)
-    scaled_right_paw_ensemble_stacks = remove_camera_means(
-        right_paw_ensemble_stacks, means_camera)
+
+    remove_camera_means(right_paw_ensemble_stacks, means_camera)
 
     good_scaled_stacked_ensemble_preds = \
         remove_camera_means(good_stacked_ensemble_preds[None, :, :], means_camera)[0]
     ensemble_pca, ensemble_ex_var = pca(good_scaled_stacked_ensemble_preds, 3)
 
     scaled_left_paw_ensemble_preds = \
         remove_camera_means(left_paw_ensemble_preds[None, :, :], means_camera)[0]
     ensemble_pcs_left_paw = ensemble_pca.transform(scaled_left_paw_ensemble_preds)
     good_ensemble_pcs_left_paw = ensemble_pcs_left_paw[good_frames]
-    
+
     scaled_right_paw_ensemble_preds = \
         remove_camera_means(right_paw_ensemble_preds[None, :, :], means_camera)[0]
     ensemble_pcs_right_paw = ensemble_pca.transform(scaled_right_paw_ensemble_preds)
     good_ensemble_pcs_right_paw = ensemble_pcs_right_paw[good_frames]
 
     # --------------------------------------------------------------
     # kalman filtering + smoothing
@@ -217,21 +232,21 @@
         # Set values for kalman filter
         # --------------------------------------
         if paw == 'left':
             save_keypoint_name = keypoint_names[0]
             good_ensemble_pcs = good_ensemble_pcs_left_paw
             ensemble_vars = left_paw_ensemble_vars
             y = scaled_left_paw_ensemble_preds
-            ensemble_stacks = scaled_left_paw_ensemble_stacks
+            # ensemble_stacks = scaled_left_paw_ensemble_stacks
         else:
             save_keypoint_name = keypoint_names[1]
             good_ensemble_pcs = good_ensemble_pcs_right_paw
             ensemble_vars = right_paw_ensemble_vars
             y = scaled_right_paw_ensemble_preds
-            ensemble_stacks = scaled_right_paw_ensemble_stacks
+            # ensemble_stacks = scaled_right_paw_ensemble_stacks
 
         # compute center of mass
         # latent variables (observed)
         good_z_t_obs = good_ensemble_pcs  # latent variables - true 3D pca
 
         # Set values for kalman filter #
         # initial state: mean
@@ -258,33 +273,36 @@
         R = np.eye(ensemble_pca.components_.shape[1])
 
         # --------------------------------------
         # perform filtering
         # --------------------------------------
         # do filtering pass with time-varying ensemble variances
         print(f"filtering {paw} paw...")
-        mf, Vf, S = filtering_pass(y, m0, S0, C, R, A, Q, ensemble_vars)
+        mf, Vf, S, _, _ = forward_pass(y, m0, S0, C, R, A, Q, ensemble_vars)
         print("done filtering")
 
         # --------------------------------------
         # perform smoothing
         # --------------------------------------
         # Do the smoothing step
         print(f"smoothing {paw} paw...")
-        ms, Vs, _ = smooth_backward(y, mf, Vf, S, A, Q, C)
+        ms, Vs, _ = backward_pass(y, mf, Vf, S, A, Q, C)
         print("done smoothing")
         # Smoothed posterior over y
         y_m_smooth = np.dot(C, ms.T).T
         y_v_smooth = np.swapaxes(np.dot(C, np.dot(Vs, C.T)), 0, 1)
 
         # --------------------------------------
         # cleanup for this paw
         # --------------------------------------
         save_keypoint_names = ['l_cam_' + save_keypoint_name, 'r_cam_' + save_keypoint_name]
-        pdindex = make_dlc_pandas_index(save_keypoint_names, labels=["x", "y", "likelihood", "x_var", "y_var", "zscore"])
+        pdindex = make_dlc_pandas_index(
+            save_keypoint_names,
+            labels=["x", "y", "likelihood", "x_var", "y_var", "zscore"]
+        )
 
         scaled_y_m_smooth = add_camera_means(y_m_smooth[None, :, :], means_camera)[0]
         scaled_y = add_camera_means(y[None, :, :], means_camera)[0]
         pred_arr = []
         for i in range(len(save_keypoint_names)):
             pred_arr.append(scaled_y_m_smooth.T[0 + 2 * i])
             pred_arr.append(scaled_y_m_smooth.T[1 + 2 * i])
@@ -292,99 +310,128 @@
             var[:] = np.nan
             pred_arr.append(var)
             x_var = y_v_smooth[:, 0 + 2 * i, 0 + 2 * i]
             y_var = y_v_smooth[:, 1 + 2 * i, 1 + 2 * i]
             pred_arr.append(x_var)
             pred_arr.append(y_var)
             ###
-            eks_predictions = np.asarray([scaled_y_m_smooth.T[0 + 2 * i], scaled_y_m_smooth.T[1 + 2 * i]]).T
-            ensemble_preds = scaled_y[:,2*i:2*(i+1)]
-            ensemble_vars_curr = ensemble_vars[:,2*i:2*(i+1)]
-            zscore = eks_zscore(eks_predictions, ensemble_preds, ensemble_vars_curr, min_ensemble_std=4)
+            eks_predictions = np.asarray([scaled_y_m_smooth.T[0 + 2 * i],
+                                          scaled_y_m_smooth.T[1 + 2 * i]]).T
+            ensemble_preds = scaled_y[:, 2 * i:2 * (i + 1)]
+            ensemble_vars_curr = ensemble_vars[:, 2 * i:2 * (i + 1)]
+            zscore = eks_zscore(eks_predictions, ensemble_preds, ensemble_vars_curr,
+                                min_ensemble_std=4)
             pred_arr.append(zscore)
             ###
         pred_arr = np.asarray(pred_arr)
         dfs[paw] = pd.DataFrame(pred_arr.T, columns=pdindex)
 
     # --------------------------------------
     # final cleanup
     # --------------------------------------
-    pdindex = make_dlc_pandas_index(keypoint_names, labels=["x", "y", "likelihood", "x_var", "y_var", "zscore"])
-
+    pdindex = make_dlc_pandas_index(keypoint_names,
+                                    labels=["x", "y", "likelihood", "x_var", "y_var", "zscore"])
 
     # make left cam dataframe
     pred_arr = np.hstack([
-        dfs['left'].loc[:, ('ensemble-kalman_tracker', 'l_cam_paw_l', 'x')].to_numpy()[:, None],
-        dfs['left'].loc[:, ('ensemble-kalman_tracker', 'l_cam_paw_l', 'y')].to_numpy()[:, None],
-        dfs['left'].loc[:, ('ensemble-kalman_tracker', 'l_cam_paw_l', 'likelihood')].to_numpy()[:, None],
-        dfs['left'].loc[:, ('ensemble-kalman_tracker', 'l_cam_paw_l', 'x_var')].to_numpy()[:, None],
-        dfs['left'].loc[:, ('ensemble-kalman_tracker', 'l_cam_paw_l', 'y_var')].to_numpy()[:, None],
-        dfs['left'].loc[:, ('ensemble-kalman_tracker', 'l_cam_paw_l', 'zscore')].to_numpy()[:, None],
+        dfs['left'].loc[:, ('ensemble-kalman_tracker', 'l_cam_paw_l', 'x')].to_numpy()
+        [:, None],
+        dfs['left'].loc[:, ('ensemble-kalman_tracker', 'l_cam_paw_l', 'y')].to_numpy()
+        [:, None],
+        dfs['left'].loc[:, ('ensemble-kalman_tracker', 'l_cam_paw_l', 'likelihood')].to_numpy()
+        [:, None],
+        dfs['left'].loc[:, ('ensemble-kalman_tracker', 'l_cam_paw_l', 'x_var')].to_numpy()
+        [:, None],
+        dfs['left'].loc[:, ('ensemble-kalman_tracker', 'l_cam_paw_l', 'y_var')].to_numpy()
+        [:, None],
+        dfs['left'].loc[:, ('ensemble-kalman_tracker', 'l_cam_paw_l', 'zscore')].to_numpy()
+        [:, None],
         dfs['right'].loc[:, ('ensemble-kalman_tracker', 'l_cam_paw_r', 'x')].to_numpy()[:, None],
         dfs['right'].loc[:, ('ensemble-kalman_tracker', 'l_cam_paw_r', 'y')].to_numpy()[:, None],
-        dfs['right'].loc[:, ('ensemble-kalman_tracker', 'l_cam_paw_r', 'likelihood')].to_numpy()[:, None],
-        dfs['right'].loc[:, ('ensemble-kalman_tracker', 'l_cam_paw_r', 'x_var')].to_numpy()[:, None],
-        dfs['right'].loc[:, ('ensemble-kalman_tracker', 'l_cam_paw_r', 'y_var')].to_numpy()[:, None],
-        dfs['right'].loc[:, ('ensemble-kalman_tracker', 'l_cam_paw_r', 'zscore')].to_numpy()[:, None],
+        dfs['right'].loc[:, ('ensemble-kalman_tracker', 'l_cam_paw_r', 'likelihood')].to_numpy()
+        [:, None],
+        dfs['right'].loc[:, ('ensemble-kalman_tracker', 'l_cam_paw_r', 'x_var')].to_numpy()
+        [:, None],
+        dfs['right'].loc[:, ('ensemble-kalman_tracker', 'l_cam_paw_r', 'y_var')].to_numpy()
+        [:, None],
+        dfs['right'].loc[:, ('ensemble-kalman_tracker', 'l_cam_paw_r', 'zscore')].to_numpy()
+        [:, None],
     ])
     df_left = pd.DataFrame(pred_arr, columns=pdindex)
 
     # make right cam dataframe
     # note we swap left and right paws to match dlc/lp convention
     # note we flip the paws horizontally to match lp convention
     pred_arr = np.hstack([
-        img_width - dfs['right'].loc[:, ('ensemble-kalman_tracker', 'r_cam_paw_r', 'x')].to_numpy()[:, None],
-        dfs['right'].loc[:, ('ensemble-kalman_tracker', 'r_cam_paw_r', 'y')].to_numpy()[:, None],
-        dfs['right'].loc[:, ('ensemble-kalman_tracker', 'r_cam_paw_r', 'likelihood')].to_numpy()[:, None],
-        dfs['right'].loc[:, ('ensemble-kalman_tracker', 'r_cam_paw_r', 'x_var')].to_numpy()[:, None],
-        dfs['right'].loc[:, ('ensemble-kalman_tracker', 'r_cam_paw_r', 'y_var')].to_numpy()[:, None],
-        dfs['right'].loc[:, ('ensemble-kalman_tracker', 'r_cam_paw_r', 'zscore')].to_numpy()[:, None],
-        img_width - dfs['left'].loc[:, ('ensemble-kalman_tracker', 'r_cam_paw_l', 'x')].to_numpy()[:, None],
-        dfs['left'].loc[:, ('ensemble-kalman_tracker', 'r_cam_paw_l', 'y')].to_numpy()[:, None],
-        dfs['left'].loc[:, ('ensemble-kalman_tracker', 'r_cam_paw_l', 'likelihood')].to_numpy()[:, None],
-        dfs['left'].loc[:, ('ensemble-kalman_tracker', 'r_cam_paw_l', 'x_var')].to_numpy()[:, None],
-        dfs['left'].loc[:, ('ensemble-kalman_tracker', 'r_cam_paw_l', 'y_var')].to_numpy()[:, None],
-        dfs['left'].loc[:, ('ensemble-kalman_tracker', 'r_cam_paw_l', 'zscore')].to_numpy()[:, None],
+        img_width - dfs['right'].loc[:, ('ensemble-kalman_tracker', 'r_cam_paw_r', 'x')].to_numpy()
+        [:, None],
+        dfs['right'].loc[:, ('ensemble-kalman_tracker', 'r_cam_paw_r', 'y')].to_numpy()
+        [:, None],
+        dfs['right'].loc[:, ('ensemble-kalman_tracker', 'r_cam_paw_r', 'likelihood')].to_numpy()
+        [:, None],
+        dfs['right'].loc[:, ('ensemble-kalman_tracker', 'r_cam_paw_r', 'x_var')].to_numpy()
+        [:, None],
+        dfs['right'].loc[:, ('ensemble-kalman_tracker', 'r_cam_paw_r', 'y_var')].to_numpy()
+        [:, None],
+        dfs['right'].loc[:, ('ensemble-kalman_tracker', 'r_cam_paw_r', 'zscore')].to_numpy()
+        [:, None],
+        img_width - dfs['left'].loc[:, ('ensemble-kalman_tracker', 'r_cam_paw_l', 'x')].to_numpy()
+        [:, None],
+        dfs['left'].loc[:, ('ensemble-kalman_tracker', 'r_cam_paw_l', 'y')].to_numpy()
+        [:, None],
+        dfs['left'].loc[:, ('ensemble-kalman_tracker', 'r_cam_paw_l', 'likelihood')].to_numpy()
+        [:, None],
+        dfs['left'].loc[:, ('ensemble-kalman_tracker', 'r_cam_paw_l', 'x_var')].to_numpy()
+        [:, None],
+        dfs['left'].loc[:, ('ensemble-kalman_tracker', 'r_cam_paw_l', 'y_var')].to_numpy()
+        [:, None],
+        dfs['left'].loc[:, ('ensemble-kalman_tracker', 'r_cam_paw_l', 'zscore')].to_numpy()
+        [:, None],
     ])
     df_right = pd.DataFrame(pred_arr, columns=pdindex)
 
-    return {'left_df': df_left, 'right_df': df_right}, markers_list_left_cam, markers_list_right_cam
+    return {'left_df': df_left, 'right_df': df_right}, \
+        markers_list_left_cam, markers_list_right_cam
 
 
 # -----------------------
 # funcs for mirror-mouse
 # -----------------------
 def ensemble_kalman_smoother_multi_cam(
-        markers_list_cameras, keypoint_ensemble, smooth_param, quantile_keep_pca, camera_names, ensembling_mode='median', zscore_threshold=2):
+    markers_list_cameras, keypoint_ensemble, smooth_param, quantile_keep_pca, camera_names,
+        ensembling_mode='median', zscore_threshold=2):
     """Use multi-view constraints to fit a 3d latent subspace for each body part.
 
     Parameters
     ----------
     markers_list_cameras : list of list of pd.DataFrames
-        each list element is a list of dataframe predictions from one ensemble member for each camera.
+        each list element is a list of dataframe predictions from one ensemble member for each
+        camera.
     keypoint_ensemble : str
         the name of the keypoint to be ensembled and smoothed
     smooth_param : float
         ranges from .01-2 (smaller values = more smoothing)
     quantile_keep_pca
         percentage of the points are kept for multi-view PCA (lowest ensemble variance)
     camera_names: list
         the camera names (should be the same length as markers_list_cameras).
     ensembling_mode:
         the function used for ensembling ('mean', 'median', or 'confidence_weighted_mean')
     zscore_threshold:
-        Minimum std threshold to reduce the effect of low ensemble std on a zscore metric (default 2).
+        Minimum std threshold to reduce the effect of low ensemble std on a zscore metric
+        (default 2).
 
     Returns
     -------
 
     Returns
     -------
     dict
-        camera_dfs: dataframe containing smoothed markers for each camera; same format as input dataframes
+        camera_dfs: dataframe containing smoothed markers for each camera; same format as input
+        dataframes
     """
 
     # --------------------------------------------------------------
     # interpolate right cam markers to left cam timestamps
     # --------------------------------------------------------------
     num_cameras = len(camera_names)
     markers_list_stacked_interp = []
@@ -398,132 +445,143 @@
             curr_markers = []
             for camera in range(num_cameras):
                 markers = np.array(markers_list_cameras[camera][model_id].to_numpy()[i, [0, 1]])
                 likelihood = np.array(markers_list_cameras[camera][model_id].to_numpy()[i, [2]])[0]
                 camera_markers_curr[camera].append(markers)
                 curr_markers.append(markers)
                 camera_likelihoods[camera].append(likelihood)
-            bl_markers_curr.append(np.concatenate(curr_markers)) #combine predictions for all cameras
+            # combine predictions for all cameras
+            bl_markers_curr.append(np.concatenate(curr_markers))
         markers_list_stacked_interp.append(bl_markers_curr)
         camera_likelihoods_stacked.append(camera_likelihoods)
         camera_likelihoods = np.asarray(camera_likelihoods)
         for camera in range(num_cameras):
             markers_list_interp[camera].append(camera_markers_curr[camera])
             camera_likelihoods[camera] = np.asarray(camera_likelihoods[camera])
     markers_list_stacked_interp = np.asarray(markers_list_stacked_interp)
     markers_list_interp = np.asarray(markers_list_interp)
     camera_likelihoods_stacked = np.asarray(camera_likelihoods_stacked)
-    
-    keys = [keypoint_ensemble+'_x', keypoint_ensemble+'_y']
+
+    keys = [keypoint_ensemble + '_x', keypoint_ensemble + '_y']
     markers_list_cams = [[] for i in range(num_cameras)]
     for k in range(len(markers_list_interp[0])):
         for camera in range(num_cameras):
             markers_cam = pd.DataFrame(markers_list_interp[camera][k], columns=keys)
             markers_cam[f'{keypoint_ensemble}_likelihood'] = camera_likelihoods_stacked[k][camera]
             markers_list_cams[camera].append(markers_cam)
-    #compute ensemble median for each camera
+    # compute ensemble median for each camera
     cam_ensemble_preds = []
     cam_ensemble_vars = []
     cam_ensemble_stacks = []
     cam_keypoints_mean_dict = []
     cam_keypoints_var_dict = []
     cam_keypoints_stack_dict = []
     for camera in range(num_cameras):
-        cam_ensemble_preds_curr, cam_ensemble_vars_curr, cam_ensemble_stacks_curr, cam_keypoints_mean_dict_curr, cam_keypoints_var_dict_curr, cam_keypoints_stack_dict_curr = ensemble(markers_list_cams[camera], keys, mode=ensembling_mode)
+        cam_ensemble_preds_curr, cam_ensemble_vars_curr, cam_ensemble_stacks_curr, \
+            cam_keypoints_mean_dict_curr, cam_keypoints_var_dict_curr, \
+            cam_keypoints_stack_dict_curr = \
+            ensemble(markers_list_cams[camera], keys, mode=ensembling_mode)
         cam_ensemble_preds.append(cam_ensemble_preds_curr)
         cam_ensemble_vars.append(cam_ensemble_vars_curr)
         cam_ensemble_stacks.append(cam_ensemble_stacks_curr)
         cam_keypoints_mean_dict.append(cam_keypoints_mean_dict_curr)
         cam_keypoints_var_dict.append(cam_keypoints_var_dict_curr)
         cam_keypoints_stack_dict.append(cam_keypoints_stack_dict_curr)
-        
-    #filter by low ensemble variances
+
+    # filter by low ensemble variances
     hstacked_vars = np.hstack(cam_ensemble_vars)
-    max_vars = np.max(hstacked_vars,1)
+    max_vars = np.max(hstacked_vars, 1)
     quantile_keep = quantile_keep_pca
     good_frames = np.where(max_vars <= np.percentile(max_vars, quantile_keep))[0]
 
     good_cam_ensemble_preds = []
     good_cam_ensemble_vars = []
     for camera in range(num_cameras):
         good_cam_ensemble_preds.append(cam_ensemble_preds[camera][good_frames])
         good_cam_ensemble_vars.append(cam_ensemble_vars[camera][good_frames])
 
     good_ensemble_preds = np.hstack(good_cam_ensemble_preds)
-    good_ensemble_vars = np.hstack(good_cam_ensemble_vars)
+    # good_ensemble_vars = np.hstack(good_cam_ensemble_vars)
     means_camera = []
     for i in range(good_ensemble_preds.shape[1]):
-        means_camera.append(good_ensemble_preds[:,i].mean())
+        means_camera.append(good_ensemble_preds[:, i].mean())
 
     ensemble_preds = np.hstack(cam_ensemble_preds)
     ensemble_vars = np.hstack(cam_ensemble_vars)
-    ensemble_stacks = np.concatenate(cam_ensemble_stacks,2)
-    scaled_ensemble_stacks = remove_camera_means(ensemble_stacks, means_camera)
+    ensemble_stacks = np.concatenate(cam_ensemble_stacks, 2)
+    remove_camera_means(ensemble_stacks, means_camera)
 
-    good_scaled_ensemble_preds = remove_camera_means(good_ensemble_preds[None,:,:], means_camera)[0]
-    ensemble_pca, ensemble_ex_var = pca(good_scaled_ensemble_preds, 3)
+    good_scaled_ensemble_preds = remove_camera_means(
+        good_ensemble_preds[None, :, :], means_camera)[0]
+    ensemble_pca, ensemble_ex_var = pca(
+        good_scaled_ensemble_preds, 3)
 
-    scaled_ensemble_preds = remove_camera_means(ensemble_preds[None,:,:], means_camera)[0]
+    scaled_ensemble_preds = remove_camera_means(ensemble_preds[None, :, :], means_camera)[0]
     ensemble_pcs = ensemble_pca.transform(scaled_ensemble_preds)
     good_ensemble_pcs = ensemble_pcs[good_frames]
 
     y_obs = scaled_ensemble_preds
-    
-    #compute center of mass
-    #latent variables (observed)
-    good_z_t_obs = good_ensemble_pcs #latent variables - true 3D pca
-
-    ##### Set values for kalman filter #####
-    m0 = np.asarray([0.0, 0.0, 0.0]) # initial state: mean
-    S0 =  np.asarray([[np.var(good_z_t_obs[:,0]), 0.0, 0.0], [0.0, np.var(good_z_t_obs[:,1]), 0.0], [0.0, 0.0, np.var(good_z_t_obs[:,2])]]) # diagonal: var
 
-    A = np.asarray([[1.0, 0.0, 0.0], [0.0, 1.0, 0.0], [0.0, 0.0, 1.0]]) #state-transition matrix,
-    # Q = np.asarray([[10.0, 0.0, 0.0], [0.0, 10.0, 0.0], [0.0, 0.0, 10.0]]) #state covariance matrix?????
+    # compute center of mass
+    # latent variables (observed)
+    good_z_t_obs = good_ensemble_pcs  # latent variables - true 3D pca
+
+    # ------ Set values for kalman filter ------
+    m0 = np.asarray([0.0, 0.0, 0.0])  # initial state: mean
+    S0 = np.asarray([[np.var(good_z_t_obs[:, 0]), 0.0, 0.0],
+                     [0.0, np.var(good_z_t_obs[:, 1]), 0.0],
+                     [0.0, 0.0, np.var(good_z_t_obs[:, 2])]])  # diagonal: var
+
+    A = np.asarray([[1.0, 0.0, 0.0], [0.0, 1.0, 0.0], [0.0, 0.0, 1.0]])  # state-transition matrix,
+
+    # Q = np.asarray([[10.0, 0.0, 0.0], [0.0, 10.0, 0.0], [0.0, 0.0, 10.0]]) <-- state-cov matrix?
+
     d_t = good_z_t_obs[1:] - good_z_t_obs[:-1]
 
-    Q = smooth_param*np.cov(d_t.T)
+    C = ensemble_pca.components_.T  # Measurement function is inverse transform of PCA
+    R = np.eye(ensemble_pca.components_.shape[1])  # placeholder diagonal matrix for ensemble var
 
-    C = ensemble_pca.components_.T # Measurement function is inverse transform of PCA
-    R = np.eye(ensemble_pca.components_.shape[1]) # placeholder diagonal matrix for ensemble variance
+    cov_matrix = np.cov(d_t.T)
 
-    print(f"filtering {keypoint_ensemble}...")
-    mf, Vf, S = filtering_pass(y_obs, m0, S0, C, R, A, Q, ensemble_vars)
-    print("done filtering")
-    y_m_filt = np.dot(C, mf.T).T
-    y_v_filt = np.swapaxes(np.dot(C, np.dot(Vf, C.T)), 0, 1)
-
-    # Do the smoothing step
-    print(f"smoothing {keypoint_ensemble}...")
-    ms, Vs, _ = smooth_backward(y_obs, mf, Vf, S, A, Q, C)
-    print("done smoothing")
+    # Call functions from ensemble_kalman to optimize smooth_param before filtering and smoothing
+    if smooth_param is None:
+        smooth_param = optimize_smoothing_param(cov_matrix, y_obs, m0, S0, C, A, R, ensemble_vars)
+    ms, Vs, nll, nll_values = filter_smooth_nll(
+        cov_matrix, smooth_param, y_obs, m0, S0, C, A, R, ensemble_vars)
+    print(f"NLL is {nll} for {keypoint_ensemble}, smooth_param={smooth_param}")
+    smooth_param_final = smooth_param
 
     # Smoothed posterior over y
     y_m_smooth = np.dot(C, ms.T).T
     y_v_smooth = np.swapaxes(np.dot(C, np.dot(Vs, C.T)), 0, 1)
 
     # --------------------------------------
     # final cleanup
     # --------------------------------------
-    pdindex = make_dlc_pandas_index([keypoint_ensemble], labels=["x", "y", "likelihood", "x_var", "y_var", "zscore"])
+    pdindex = make_dlc_pandas_index([keypoint_ensemble],
+                                    labels=["x", "y", "likelihood", "x_var", "y_var", "zscore"])
     camera_indices = []
     for camera in range(num_cameras):
-        camera_indices.append([camera*2, camera*2+1])
+        camera_indices.append([camera * 2, camera * 2 + 1])
     camera_dfs = {}
     for camera, camera_name in enumerate(camera_names):
         var = np.empty(y_m_smooth.T[camera_indices[camera][0]].shape)
         var[:] = np.nan
-        eks_pred_x = y_m_smooth.T[camera_indices[camera][0]] + means_camera[camera_indices[camera][0]]
-        eks_pred_y = y_m_smooth.T[camera_indices[camera][1]] + means_camera[camera_indices[camera][1]]
-        #compute zscore for EKS to see how it deviates from the ensemble
+        eks_pred_x = \
+            y_m_smooth.T[camera_indices[camera][0]] + means_camera[camera_indices[camera][0]]
+        eks_pred_y = \
+            y_m_smooth.T[camera_indices[camera][1]] + means_camera[camera_indices[camera][1]]
+        # compute zscore for EKS to see how it deviates from the ensemble
         eks_predictions = np.asarray([eks_pred_x, eks_pred_y]).T
-        zscore = eks_zscore(eks_predictions, cam_ensemble_preds[camera], cam_ensemble_vars[camera], min_ensemble_std=zscore_threshold)
+        zscore = eks_zscore(eks_predictions, cam_ensemble_preds[camera], cam_ensemble_vars[camera],
+                            min_ensemble_std=zscore_threshold)
         pred_arr = np.vstack([
             eks_pred_x,
             eks_pred_y,
             var,
-            y_v_smooth[:,camera_indices[camera][0],camera_indices[camera][0]],
-            y_v_smooth[:,camera_indices[camera][1],camera_indices[camera][1]],
+            y_v_smooth[:, camera_indices[camera][0], camera_indices[camera][0]],
+            y_v_smooth[:, camera_indices[camera][1], camera_indices[camera][1]],
             zscore,
         ]).T
         camera_dfs[camera_name + '_df'] = pd.DataFrame(pred_arr, columns=pdindex)
-    return camera_dfs
-    #return camera_dfs, cam_keypoints_mean_dict, cam_keypoints_var_dict
+    return camera_dfs, smooth_param_final, nll_values
+    # return camera_dfs, cam_keypoints_mean_dict, cam_keypoints_var_dict
```

### Comparing `ensemble-kalman-smoother-1.0.1/eks/pupil_smoother.py` & `ensemble-kalman-smoother-1.1.0/eks/pupil_smoother.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 import numpy as np
 import pandas as pd
-from scipy.interpolate import interp1d
-from sklearn.decomposition import PCA
 from eks.utils import make_dlc_pandas_index
-from eks.ensemble_kalman import ensemble, filtering_pass, kalman_dot, smooth_backward, eks_zscore
+from eks.core import ensemble, forward_pass, backward_pass, eks_zscore
 import warnings
 
 
 # -----------------------
 # funcs for kalman pupil
 # -----------------------
 def get_pupil_location(dlc):
@@ -16,28 +14,28 @@
     and in addition assume it's a circle and
     estimate diameter from other pairs of points
     Author: Michael Schartner
     """
     s = 1
     t = np.vstack((dlc['pupil_top_r_x'], dlc['pupil_top_r_y'])).T / s
     b = np.vstack((dlc['pupil_bottom_r_x'], dlc['pupil_bottom_r_y'])).T / s
-    l = np.vstack((dlc['pupil_left_r_x'], dlc['pupil_left_r_y'])).T / s
+    le = np.vstack((dlc['pupil_left_r_x'], dlc['pupil_left_r_y'])).T / s
     r = np.vstack((dlc['pupil_right_r_x'], dlc['pupil_right_r_y'])).T / s
     center = np.zeros(t.shape)
 
     # ok if either top or bottom is nan in x-dir
     tmp_x1 = np.nanmedian(np.hstack([t[:, 0, None], b[:, 0, None]]), axis=1)
     # both left and right must be present in x-dir
-    tmp_x2 = np.median(np.hstack([r[:, 0, None], l[:, 0, None]]), axis=1)
+    tmp_x2 = np.median(np.hstack([r[:, 0, None], le[:, 0, None]]), axis=1)
     center[:, 0] = np.nanmedian(np.hstack([tmp_x1[:, None], tmp_x2[:, None]]), axis=1)
 
     # both top and bottom must be present in y-dir
     tmp_y1 = np.median(np.hstack([t[:, 1, None], b[:, 1, None]]), axis=1)
     # ok if either left or right is nan in y-dir
-    tmp_y2 = np.nanmedian(np.hstack([r[:, 1, None], l[:, 1, None]]), axis=1)
+    tmp_y2 = np.nanmedian(np.hstack([r[:, 1, None], le[:, 1, None]]), axis=1)
     center[:, 1] = np.nanmedian(np.hstack([tmp_y1[:, None], tmp_y2[:, None]]), axis=1)
     return center
 
 
 def get_pupil_diameter(dlc):
     """
     from: https://int-brain-lab.github.io/iblenv/_modules/brainbox/behavior/dlc.html
@@ -95,29 +93,30 @@
     keypoint_names: list
     tracker_name : str
         tracker name for constructing final dataframe
     state_transition_matrix : np.ndarray
     likelihood_default
         value to store in likelihood column; should be np.nan or int in [0, 1]
     zscore_threshold:
-        Minimum std threshold to reduce the effect of low ensemble std on a zscore metric (default 2).
+        Minimum std threshold to reduce the effect of low ensemble std on a zscore metric
+        (default 2).
 
     Returns
     -------
     dict
         markers_df: dataframe containing smoothed markers; same format as input dataframes
         latents_df: dataframe containing 3d latents: pupil diameter and pupil center of mass
 
     """
 
     # compute ensemble median
     keys = ['pupil_top_r_x', 'pupil_top_r_y', 'pupil_bottom_r_x', 'pupil_bottom_r_y',
             'pupil_right_r_x', 'pupil_right_r_y', 'pupil_left_r_x', 'pupil_left_r_y']
-    ensemble_preds, ensemble_vars, ensemble_stacks, keypoints_mean_dict, keypoints_var_dict, keypoints_stack_dict = ensemble(
-        markers_list, keys)
+    ensemble_preds, ensemble_vars, ensemble_stacks, keypoints_mean_dict, keypoints_var_dict, \
+        keypoints_stack_dict = ensemble(markers_list, keys)
     # ## Set parameters
     # compute center of mass
     pupil_locations = get_pupil_location(keypoints_mean_dict)
     pupil_diameters = get_pupil_diameter(keypoints_mean_dict)
     diameters = []
     for i in range(len(markers_list)):
         keypoints_dict = keypoints_stack_dict[i]
@@ -181,60 +180,62 @@
     y = scaled_ensemble_preds
 
     # --------------------------------------
     # perform filtering
     # --------------------------------------
     # do filtering pass with time-varying ensemble variances
     print("filtering...")
-    mf, Vf, S = filtering_pass(y, m0, S0, C, R, A, Q, ensemble_vars)
+    mf, Vf, S, _, _ = forward_pass(y, m0, S0, C, R, A, Q, ensemble_vars)
     print("done filtering")
 
     # --------------------------------------
     # perform smoothing
     # --------------------------------------
     # Do the smoothing step
     print("smoothing...")
-    ms, Vs, _ = smooth_backward(y, mf, Vf, S, A, Q, C)
+    ms, Vs, _ = backward_pass(y, mf, Vf, S, A, Q, C)
     print("done smoothing")
     # Smoothed posterior over y
     y_m_smooth = np.dot(C, ms.T).T
     y_v_smooth = np.swapaxes(np.dot(C, np.dot(Vs, C.T)), 0, 1)
 
     # --------------------------------------
     # cleanup
     # --------------------------------------
     # save out marker info
-    pdindex = make_dlc_pandas_index(keypoint_names, labels=["x", "y", "likelihood", "x_var", "y_var", "zscore"])
+    pdindex = make_dlc_pandas_index(keypoint_names,
+                                    labels=["x", "y", "likelihood", "x_var", "y_var", "zscore"])
     processed_arr_dict = add_mean_to_array(y_m_smooth, keys, mean_x_obs, mean_y_obs)
     key_pair_list = [['pupil_top_r_x', 'pupil_top_r_y'],
                      ['pupil_right_r_x', 'pupil_right_r_y'],
                      ['pupil_bottom_r_x', 'pupil_bottom_r_y'],
                      ['pupil_left_r_x', 'pupil_left_r_y']]
-    ensemble_indices = [(0,1), (4,5), (2,3), (6,7)]
+    ensemble_indices = [(0, 1), (4, 5), (2, 3), (6, 7)]
     pred_arr = []
     for i, key_pair in enumerate(key_pair_list):
         pred_arr.append(processed_arr_dict[key_pair[0]])
         pred_arr.append(processed_arr_dict[key_pair[1]])
         var = np.empty(processed_arr_dict[key_pair[0]].shape)
         var[:] = likelihood_default
         pred_arr.append(var)
-        x_var = y_v_smooth[:,i, i]
-        y_var = y_v_smooth[:,i+1, i+1]
+        x_var = y_v_smooth[:, i, i]
+        y_var = y_v_smooth[:, i + 1, i + 1]
         pred_arr.append(x_var)
         pred_arr.append(y_var)
-        #compute zscore for EKS to see how it deviates from the ensemble
-        eks_predictions = np.asarray([processed_arr_dict[key_pair[0]], processed_arr_dict[key_pair[1]]]).T
-        ensemble_preds_curr = ensemble_preds[:,ensemble_indices[i][0]: ensemble_indices[i][1]+1]
-        ensemble_vars_curr = ensemble_vars[:,ensemble_indices[i][0]: ensemble_indices[i][1]+1]
-        zscore = eks_zscore(eks_predictions, ensemble_preds_curr, ensemble_vars_curr, min_ensemble_std=zscore_threshold)
+        # compute zscore for EKS to see how it deviates from the ensemble
+        eks_predictions = \
+            np.asarray([processed_arr_dict[key_pair[0]], processed_arr_dict[key_pair[1]]]).T
+        ensemble_preds_curr = ensemble_preds[:, ensemble_indices[i][0]: ensemble_indices[i][1] + 1]
+        ensemble_vars_curr = ensemble_vars[:, ensemble_indices[i][0]: ensemble_indices[i][1] + 1]
+        zscore = eks_zscore(eks_predictions, ensemble_preds_curr, ensemble_vars_curr,
+                            min_ensemble_std=zscore_threshold)
         pred_arr.append(zscore)
-    
+
     pred_arr = np.asarray(pred_arr)
     markers_df = pd.DataFrame(pred_arr.T, columns=pdindex)
-
     # save out latents info: pupil diam, center of mass
     pred_arr2 = []
     pred_arr2.append(ms[:, 0])
     pred_arr2.append(ms[:, 1] + mean_x_obs)  # add back x mean of pupil location
     pred_arr2.append(ms[:, 2] + mean_y_obs)  # add back y mean of pupil location
     pred_arr2 = np.asarray(pred_arr2)
     arrays = [[tracker_name, tracker_name, tracker_name], ['diameter', 'com_x', 'com_y']]
```

### Comparing `ensemble-kalman-smoother-1.0.1/eks/singleview_smoother.py` & `ensemble-kalman-smoother-1.1.0/eks/singleview_smoother.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,106 +1,148 @@
 import numpy as np
 import pandas as pd
-from scipy.interpolate import interp1d
-from sklearn.decomposition import PCA
 from eks.utils import make_dlc_pandas_index
-from eks.ensemble_kalman import ensemble, filtering_pass, kalman_dot, smooth_backward, eks_zscore
+from eks.core import ensemble, eks_zscore, optimize_smoothing_param, \
+    filter_smooth_nll
+
 
 # -----------------------
 # funcs for single-view
 # -----------------------
 def ensemble_kalman_smoother_single_view(
-        markers_list, keypoint_ensemble, smooth_param, ensembling_mode='median', zscore_threshold=2, verbose=False):
-    """Use an identity observation matrix and smoothes by adjusting the smoothing parameter in the state-covariance matrix.
+        markers_list, keypoint_ensemble, smooth_param, ensembling_mode='median',
+        zscore_threshold=2, verbose=False):
+    """ Use an identity observation matrix and smoothes by adjusting the smoothing parameter in the
+    state-covariance matrix.
 
     Parameters
     ----------
     markers_list : list of list of pd.DataFrames
         each list element is a list of dataframe predictions from one ensemble member.
     keypoint_ensemble : str
         the name of the keypoint to be ensembled and smoothed
     smooth_param : float
         ranges from .01-20 (smaller values = more smoothing)
     ensembling_mode:
         the function used for ensembling ('mean', 'median', or 'confidence_weighted_mean')
     zscore_threshold:
-        Minimum std threshold to reduce the effect of low ensemble std on a zscore metric (default 2).
+        Minimum std threshold to reduce the effect of low ensemble std on a zscore metric
+        (default 2).
     verbose: bool
         If True, progress will be printed for the user.
     Returns
     -------
 
     Returns
     -------
     dict
-        keypoint_df: dataframe containing smoothed markers for one keypoint; same format as input dataframes
+        keypoint_df: dataframe containing smoothed markers for one keypoint; same format as input
+        dataframes
     """
 
     # --------------------------------------------------------------
     # interpolate right cam markers to left cam timestamps
     # --------------------------------------------------------------
-    keys = [keypoint_ensemble+'_x', keypoint_ensemble+'_y']
+    keys = [keypoint_ensemble + '_x', keypoint_ensemble + '_y']
     x_key = keys[0]
     y_key = keys[1]
 
-    #compute ensemble median
-    ensemble_preds, ensemble_vars, ensemble_stacks, keypoints_mean_dict, keypoints_var_dict, keypoints_stack_dict = ensemble(markers_list, keys, mode=ensembling_mode)
+    # compute ensemble median
+    ensemble_preds, ensemble_vars, ensemble_stacks, keypoints_mean_dict, keypoints_var_dict, \
+        keypoints_stack_dict = ensemble(markers_list, keys, mode=ensembling_mode)
 
     mean_x_obs = np.mean(keypoints_mean_dict[x_key])
     mean_y_obs = np.mean(keypoints_mean_dict[y_key])
-    x_t_obs, y_t_obs = keypoints_mean_dict[x_key] - mean_x_obs, keypoints_mean_dict[y_key] - mean_y_obs 
-    z_t_obs = np.vstack((x_t_obs, y_t_obs)) #latent variables - true x and y
-    
-     ##### Set values for kalman filter #####
-    m0 = np.asarray([0.0, 0.0]) # initial state: mean
-    S0 =  np.asarray([[np.var(x_t_obs), 0.0], [0.0 , np.var(y_t_obs)]]) # diagonal: var
-
-    A = np.asarray([[1.0, 0], [0, 1.0]]) #state-transition matrix,
-    Q = np.asarray([[smooth_param, 0], [0, smooth_param]]) #state covariance matrix -> smaller = more smoothing
-    C = np.asarray([[1, 0], [0, 1]]) # Measurement function
-    R = np.eye(2) # placeholder diagonal matrix for ensemble variance
-    
+    x_t_obs, y_t_obs = \
+        keypoints_mean_dict[x_key] - mean_x_obs, keypoints_mean_dict[y_key] - mean_y_obs
+    # z_t_obs = np.vstack((x_t_obs, y_t_obs))  # latent variables - true x and y
+
+    # ------ Set values for kalman filter ------
+    m0 = np.asarray([0.0, 0.0])  # initial state: mean
+    S0 = np.asarray([[np.var(x_t_obs), 0.0], [0.0 , np.var(y_t_obs)]])  # diagonal: var
+
+    A = np.asarray([[1.0, 0], [0, 1.0]])  # state-transition matrix,
+    cov_matrix = np.asarray([[1, 0], [0, 1]])  # state covariance matrix; smaller = more smoothing
+    C = np.asarray([[1, 0], [0, 1]])  # Measurement function
+    R = np.eye(2)  # placeholder diagonal matrix for ensemble variance
+
     scaled_ensemble_preds = ensemble_preds.copy()
     scaled_ensemble_preds[:, 0] -= mean_x_obs
     scaled_ensemble_preds[:, 1] -= mean_y_obs
-    
+
     y_obs = scaled_ensemble_preds
-    
+
+    '''
     if verbose:
         print(f"filtering {keypoint_ensemble}...")
     mf, Vf, S = filtering_pass(y_obs, m0, S0, C, R, A, Q, ensemble_vars)
     if verbose:
         print("done filtering")
     y_m_filt = np.dot(C, mf.T).T
     y_v_filt = np.swapaxes(np.dot(C, np.dot(Vf, C.T)), 0, 1)
 
     # Do the smoothing step
     if verbose:
         print(f"smoothing {keypoint_ensemble}...")
     ms, Vs, _ = smooth_backward(y_obs, mf, Vf, S, A, Q, C)
     if verbose:
         print("done smoothing")
+    # compute NLL
+    nll = compute_nll_2(y_obs, mf, S, C)
+    nll_values = compute_nll_2_steps(y_obs, mf, S, C)
+    '''
+
+    # Call functions from ensemble_kalman to optimize smooth_param before filtering and smoothing
+    if smooth_param is None:
+        smooth_param_final = \
+            optimize_smoothing_param(cov_matrix, y_obs, m0, S0, C, A, R, ensemble_vars)
+    else:
+        smooth_param_final = smooth_param
+    ms, Vs, nll, nll_values = \
+        filter_smooth_nll(cov_matrix, smooth_param_final, y_obs, m0, S0, C, A, R, ensemble_vars)
+    print(f"NLL is {nll} for {keypoint_ensemble}, smooth_param={smooth_param_final}")
 
     # Smoothed posterior over y
     y_m_smooth = np.dot(C, ms.T).T
     y_v_smooth = np.swapaxes(np.dot(C, np.dot(Vs, C.T)), 0, 1)
-    
-    #compute zscore for EKS to see how it deviates from the ensemble
+
+    # compute zscore for EKS to see how it deviates from the ensemble
     eks_predictions = y_m_smooth.copy()
-    eks_predictions = np.asarray([eks_predictions.T[0] + mean_x_obs, eks_predictions.T[1] + mean_y_obs]).T
-    zscore = eks_zscore(eks_predictions, ensemble_preds, ensemble_vars, min_ensemble_std=zscore_threshold)
+    eks_predictions = \
+        np.asarray([eks_predictions.T[0] + mean_x_obs, eks_predictions.T[1] + mean_y_obs]).T
+    zscore = \
+        eks_zscore(eks_predictions, ensemble_preds, ensemble_vars,
+                   min_ensemble_std=zscore_threshold)
+
     # --------------------------------------
     # final cleanup
     # --------------------------------------
-    pdindex = make_dlc_pandas_index([keypoint_ensemble], labels=["x", "y", "likelihood", "x_var", "y_var", "zscore"])
+    pdindex = make_dlc_pandas_index([keypoint_ensemble],
+                                    labels=["x", "y", "likelihood", "x_var", "y_var", "zscore"])
     var = np.empty(y_m_smooth.T[0].shape)
     var[:] = np.nan
     pred_arr = np.vstack([
         y_m_smooth.T[0] + mean_x_obs,
         y_m_smooth.T[1] + mean_y_obs,
         var,
-        y_v_smooth[:,0,0],
-        y_v_smooth[:,1,1],
+        y_v_smooth[:, 0, 0],
+        y_v_smooth[:, 1, 1],
         zscore,
     ]).T
     df = pd.DataFrame(pred_arr, columns=pdindex)
-    return {keypoint_ensemble+'_df': df}
+    return {keypoint_ensemble + '_df': df}, smooth_param_final, nll_values
+
+
+'''
+Plotting NLL traces (paste in before final cleanup)
+    # Plot nll values against time
+    plt.plot(range(len(nll_values)), nll_values)
+    plt.xlabel('Time Step')
+    plt.ylabel('Negative Log Likelihood (nll)')
+    plt.title(f'Negative Log Likelihood vs Time for IBL Pupil s={smooth_param}')
+    plt.grid(True)
+
+    # Save the plot as a PDF file
+    plt.savefig('nll_plot.pdf')
+
+    plt.show()
+'''
```

### Comparing `ensemble-kalman-smoother-1.0.1/ensemble_kalman_smoother.egg-info/PKG-INFO` & `ensemble-kalman-smoother-1.1.0/ensemble_kalman_smoother.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: ensemble-kalman-smoother
-Version: 1.0.1
+Version: 1.1.0
 Summary: Ensembling and kalman smoothing for pose estimation
 Home-page: http://www.github.com/colehurwitz/eks
 Author: Cole Hurwitz
 Author-email: 
-License: UNKNOWN
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # EKS
 This repo contains code to run an Ensemble Kalman Smoother (EKS) for improving pose estimation outputs. 
 
@@ -59,22 +57,23 @@
 pip install -e ".[dev]"
 ```
 
 ### Method 2: pip
 
 You can also install the `eks` package using the Python Package Index (PyPI):
 ```
-python3 -m pip install eks
+python3 -m pip install ensemble-kalman-smoother
 ```
 Note that you will not have access to the example data or example scripts with the pip install 
 option.
 
 ## Example scripts
 
-We provide several example datasets and fitting scripts to illustrate use of the package.
+We provide several example datasets and fitting scripts to illustrate use of the package. See
+[Command-Line Arguments](docs/command-line_arguments.md) for more information on arguments.
 
 ### Single-camera datasets
 The `singlecam_example.py` script demonstrates how to run the EKS code for standard single-camera
 setups. 
 Any of the provided datasets are compatible with this script; below we'll use `data/ibl-pupil` as
 our example. 
 To run the EKS on the example data, execute the following command from inside this repo:
@@ -117,8 +116,8 @@
 ```
 
 ### Authors 
 Cole Hurwitz
 
 Matt Whiteway
 
-
+Keemin Lee
```

### Comparing `ensemble-kalman-smoother-1.0.1/setup.py` & `ensemble-kalman-smoother-1.1.0/setup.py`

 * *Files identical despite different names*


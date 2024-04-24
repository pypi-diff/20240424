# Comparing `tmp/cnspy_trajectory_evaluation-0.1.1.tar.gz` & `tmp/cnspy_trajectory_evaluation-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/jungr/workspace/CNS/VIO_Evaluation_Framework/py3_pkgs/cnspy_eco_system_test/pkgs/f_trajectory_evaluation/dist/tmptmxxv1zj", last modified: Sat Mar 20 14:24:22 2021, max compression
+gzip compressed data, was "cnspy_trajectory_evaluation-0.2.0.tar", last modified: Wed Apr 24 12:17:54 2024, max compression
```

## Comparing `cnspy_trajectory_evaluation-0.1.1.tar` & `cnspy_trajectory_evaluation-0.2.0.tar`

### file list

```diff
@@ -1,29 +1,37 @@
-drwxrwxr-x   0 jungr     (1000) jungr     (1000)        0 2021-03-20 14:24:22.495911 cnspy_trajectory_evaluation-0.1.1/
--rw-rw-r--   0 jungr     (1000) jungr     (1000)     7103 2021-03-20 14:24:22.495911 cnspy_trajectory_evaluation-0.1.1/PKG-INFO
--rw-rw-r--   0 jungr     (1000) jungr     (1000)     5792 2021-03-20 14:21:45.000000 cnspy_trajectory_evaluation-0.1.1/README.md
-drwxrwxr-x   0 jungr     (1000) jungr     (1000)        0 2021-03-20 14:24:22.495911 cnspy_trajectory_evaluation-0.1.1/cnspy_trajectory_evaluation/
--rwxrwxr-x   0 jungr     (1000) jungr     (1000)     6998 2021-03-20 12:20:48.000000 cnspy_trajectory_evaluation-0.1.1/cnspy_trajectory_evaluation/AbsoluteTrajectoryError.py
--rwxrwxr-x   0 jungr     (1000) jungr     (1000)     2297 2021-03-20 12:20:48.000000 cnspy_trajectory_evaluation-0.1.1/cnspy_trajectory_evaluation/AlignedTrajectories.py
--rwxrwxr-x   0 jungr     (1000) jungr     (1000)     4020 2021-03-20 12:20:48.000000 cnspy_trajectory_evaluation-0.1.1/cnspy_trajectory_evaluation/AssociatedTrajectories.py
--rwxrwxr-x   0 jungr     (1000) jungr     (1000)     2875 2021-03-20 12:20:48.000000 cnspy_trajectory_evaluation-0.1.1/cnspy_trajectory_evaluation/EvaluationReport.py
--rwxrwxr-x   0 jungr     (1000) jungr     (1000)    10480 2021-03-20 12:20:48.000000 cnspy_trajectory_evaluation-0.1.1/cnspy_trajectory_evaluation/SpatialAlignment.py
--rwxrwxr-x   0 jungr     (1000) jungr     (1000)     3147 2021-03-20 12:20:48.000000 cnspy_trajectory_evaluation-0.1.1/cnspy_trajectory_evaluation/TrajectoryAlignmentTypes.py
--rwxrwxr-x   0 jungr     (1000) jungr     (1000)     4713 2021-03-20 12:20:48.000000 cnspy_trajectory_evaluation-0.1.1/cnspy_trajectory_evaluation/TrajectoryEvaluation.py
--rwxrwxr-x   0 jungr     (1000) jungr     (1000)     7849 2021-03-20 12:20:48.000000 cnspy_trajectory_evaluation-0.1.1/cnspy_trajectory_evaluation/TrajectoryNEES.py
--rwxrwxr-x   0 jungr     (1000) jungr     (1000)        0 2021-03-20 12:20:48.000000 cnspy_trajectory_evaluation-0.1.1/cnspy_trajectory_evaluation/__init__.py
-drwxrwxr-x   0 jungr     (1000) jungr     (1000)        0 2021-03-20 14:24:22.495911 cnspy_trajectory_evaluation-0.1.1/cnspy_trajectory_evaluation.egg-info/
--rw-rw-r--   0 jungr     (1000) jungr     (1000)     7103 2021-03-20 14:24:22.000000 cnspy_trajectory_evaluation-0.1.1/cnspy_trajectory_evaluation.egg-info/PKG-INFO
--rw-rw-r--   0 jungr     (1000) jungr     (1000)      921 2021-03-20 14:24:22.000000 cnspy_trajectory_evaluation-0.1.1/cnspy_trajectory_evaluation.egg-info/SOURCES.txt
--rw-rw-r--   0 jungr     (1000) jungr     (1000)        1 2021-03-20 14:24:22.000000 cnspy_trajectory_evaluation-0.1.1/cnspy_trajectory_evaluation.egg-info/dependency_links.txt
--rw-rw-r--   0 jungr     (1000) jungr     (1000)      171 2021-03-20 14:24:22.000000 cnspy_trajectory_evaluation-0.1.1/cnspy_trajectory_evaluation.egg-info/requires.txt
--rw-rw-r--   0 jungr     (1000) jungr     (1000)       33 2021-03-20 14:24:22.000000 cnspy_trajectory_evaluation-0.1.1/cnspy_trajectory_evaluation.egg-info/top_level.txt
--rw-rw-r--   0 jungr     (1000) jungr     (1000)       38 2021-03-20 14:24:22.495911 cnspy_trajectory_evaluation-0.1.1/setup.cfg
--rw-rw-r--   0 jungr     (1000) jungr     (1000)     1456 2021-03-20 14:21:27.000000 cnspy_trajectory_evaluation-0.1.1/setup.py
-drwxrwxr-x   0 jungr     (1000) jungr     (1000)        0 2021-03-20 14:24:22.495911 cnspy_trajectory_evaluation-0.1.1/test/
--rwxrwxr-x   0 jungr     (1000) jungr     (1000)        0 2021-03-20 12:20:48.000000 cnspy_trajectory_evaluation-0.1.1/test/__init__.py
--rwxrwxr-x   0 jungr     (1000) jungr     (1000)     2991 2021-03-20 12:20:48.000000 cnspy_trajectory_evaluation-0.1.1/test/pandas_test.py
--rw-rw-r--   0 jungr     (1000) jungr     (1000)     5774 2021-03-20 12:20:48.000000 cnspy_trajectory_evaluation-0.1.1/test/test_AbsoluteTrajectoryError.py
--rw-rw-r--   0 jungr     (1000) jungr     (1000)     2683 2021-03-20 12:20:48.000000 cnspy_trajectory_evaluation-0.1.1/test/test_AlignedTrajectories.py
--rw-rw-r--   0 jungr     (1000) jungr     (1000)     2186 2021-03-20 12:20:48.000000 cnspy_trajectory_evaluation-0.1.1/test/test_EvaluationReport.py
--rw-rw-r--   0 jungr     (1000) jungr     (1000)     2011 2021-03-20 12:20:48.000000 cnspy_trajectory_evaluation-0.1.1/test/test_TrajectoryEvaluation.py
--rw-rw-r--   0 jungr     (1000) jungr     (1000)     2857 2021-03-20 12:20:48.000000 cnspy_trajectory_evaluation-0.1.1/test/test_TrajectoryNEES.py
+drwxrwxr-x   0 jungr     (1000) jungr     (1000)        0 2024-04-24 12:17:54.133337 cnspy_trajectory_evaluation-0.2.0/
+-rw-rw-r--   0 jungr     (1000) jungr     (1000)    35149 2022-05-30 14:10:29.000000 cnspy_trajectory_evaluation-0.2.0/LICENCE
+-rw-r--r--   0 jungr     (1000) jungr     (1000)     6954 2024-04-24 12:17:54.129337 cnspy_trajectory_evaluation-0.2.0/PKG-INFO
+-rw-rw-r--   0 jungr     (1000) jungr     (1000)     5935 2022-05-30 14:10:29.000000 cnspy_trajectory_evaluation-0.2.0/README.md
+drwxrwxr-x   0 jungr     (1000) jungr     (1000)        0 2024-04-24 12:17:54.129337 cnspy_trajectory_evaluation-0.2.0/cnspy_trajectory_evaluation/
+-rwxrwxr-x   0 jungr     (1000) jungr     (1000)    14401 2024-04-24 11:58:51.000000 cnspy_trajectory_evaluation-0.2.0/cnspy_trajectory_evaluation/AbsoluteTrajectoryError.py
+-rwxrwxr-x   0 jungr     (1000) jungr     (1000)     2812 2024-04-24 11:58:51.000000 cnspy_trajectory_evaluation-0.2.0/cnspy_trajectory_evaluation/AlignedTrajectories.py
+-rwxrwxr-x   0 jungr     (1000) jungr     (1000)     8867 2024-04-24 11:58:51.000000 cnspy_trajectory_evaluation-0.2.0/cnspy_trajectory_evaluation/AssociatedTrajectories.py
+-rw-rw-r--   0 jungr     (1000) jungr     (1000)     4593 2024-04-24 11:58:51.000000 cnspy_trajectory_evaluation-0.2.0/cnspy_trajectory_evaluation/DifferentialTrajectoryError.py
+-rw-rw-r--   0 jungr     (1000) jungr     (1000)     3442 2024-04-24 11:58:51.000000 cnspy_trajectory_evaluation-0.2.0/cnspy_trajectory_evaluation/EstimationTrajectoryError.py
+-rwxrwxr-x   0 jungr     (1000) jungr     (1000)     3171 2024-04-24 11:58:51.000000 cnspy_trajectory_evaluation-0.2.0/cnspy_trajectory_evaluation/EvaluationReport.py
+-rw-rw-r--   0 jungr     (1000) jungr     (1000)     9682 2022-10-03 12:25:07.000000 cnspy_trajectory_evaluation-0.2.0/cnspy_trajectory_evaluation/ICP.py
+-rwxrwxr-x   0 jungr     (1000) jungr     (1000)    15426 2024-04-24 11:58:51.000000 cnspy_trajectory_evaluation-0.2.0/cnspy_trajectory_evaluation/SpatialAlignment.py
+-rw-rw-r--   0 jungr     (1000) jungr     (1000)    12533 2024-04-24 11:58:51.000000 cnspy_trajectory_evaluation-0.2.0/cnspy_trajectory_evaluation/TrajectoryANEES.py
+-rwxrwxr-x   0 jungr     (1000) jungr     (1000)     3890 2024-04-24 11:58:51.000000 cnspy_trajectory_evaluation-0.2.0/cnspy_trajectory_evaluation/TrajectoryAlignmentTypes.py
+-rwxrwxr-x   0 jungr     (1000) jungr     (1000)    10241 2024-04-24 11:58:51.000000 cnspy_trajectory_evaluation-0.2.0/cnspy_trajectory_evaluation/TrajectoryEvaluation.py
+-rwxrwxr-x   0 jungr     (1000) jungr     (1000)    11227 2024-04-24 11:58:51.000000 cnspy_trajectory_evaluation-0.2.0/cnspy_trajectory_evaluation/TrajectoryPosOrientNEES.py
+-rwxrwxr-x   0 jungr     (1000) jungr     (1000)        0 2022-05-30 14:10:29.000000 cnspy_trajectory_evaluation-0.2.0/cnspy_trajectory_evaluation/__init__.py
+drwxrwxr-x   0 jungr     (1000) jungr     (1000)        0 2024-04-24 12:17:54.129337 cnspy_trajectory_evaluation-0.2.0/cnspy_trajectory_evaluation.egg-info/
+-rw-r--r--   0 jungr     (1000) jungr     (1000)     6954 2024-04-24 12:17:54.000000 cnspy_trajectory_evaluation-0.2.0/cnspy_trajectory_evaluation.egg-info/PKG-INFO
+-rw-rw-r--   0 jungr     (1000) jungr     (1000)     1252 2024-04-24 12:17:54.000000 cnspy_trajectory_evaluation-0.2.0/cnspy_trajectory_evaluation.egg-info/SOURCES.txt
+-rw-rw-r--   0 jungr     (1000) jungr     (1000)        1 2024-04-24 12:17:54.000000 cnspy_trajectory_evaluation-0.2.0/cnspy_trajectory_evaluation.egg-info/dependency_links.txt
+-rw-rw-r--   0 jungr     (1000) jungr     (1000)      178 2024-04-24 12:17:54.000000 cnspy_trajectory_evaluation-0.2.0/cnspy_trajectory_evaluation.egg-info/requires.txt
+-rw-rw-r--   0 jungr     (1000) jungr     (1000)       33 2024-04-24 12:17:54.000000 cnspy_trajectory_evaluation-0.2.0/cnspy_trajectory_evaluation.egg-info/top_level.txt
+-rw-rw-r--   0 jungr     (1000) jungr     (1000)       38 2024-04-24 12:17:54.133337 cnspy_trajectory_evaluation-0.2.0/setup.cfg
+-rw-rw-r--   0 jungr     (1000) jungr     (1000)     1466 2024-04-24 11:58:51.000000 cnspy_trajectory_evaluation-0.2.0/setup.py
+drwxrwxr-x   0 jungr     (1000) jungr     (1000)        0 2024-04-24 12:17:54.129337 cnspy_trajectory_evaluation-0.2.0/test/
+-rwxrwxr-x   0 jungr     (1000) jungr     (1000)        0 2022-05-30 14:10:29.000000 cnspy_trajectory_evaluation-0.2.0/test/__init__.py
+-rwxrwxr-x   0 jungr     (1000) jungr     (1000)     2991 2022-05-30 14:10:29.000000 cnspy_trajectory_evaluation-0.2.0/test/pandas_test.py
+-rw-rw-r--   0 jungr     (1000) jungr     (1000)    10923 2024-04-24 11:58:51.000000 cnspy_trajectory_evaluation-0.2.0/test/test_AbsoluteTrajectoryError.py
+-rw-rw-r--   0 jungr     (1000) jungr     (1000)     8030 2024-04-24 11:58:51.000000 cnspy_trajectory_evaluation-0.2.0/test/test_AlignedTrajectories.py
+-rw-rw-r--   0 jungr     (1000) jungr     (1000)     3566 2024-04-24 11:58:51.000000 cnspy_trajectory_evaluation-0.2.0/test/test_DifferentialTrajectoryError.py
+-rw-rw-r--   0 jungr     (1000) jungr     (1000)     2206 2024-04-24 11:58:51.000000 cnspy_trajectory_evaluation-0.2.0/test/test_EvaluationReport.py
+-rw-rw-r--   0 jungr     (1000) jungr     (1000)     3164 2024-04-24 11:58:51.000000 cnspy_trajectory_evaluation-0.2.0/test/test_OV_TrajectoryEvaluation.py
+-rw-rw-r--   0 jungr     (1000) jungr     (1000)     3332 2024-04-24 11:58:51.000000 cnspy_trajectory_evaluation-0.2.0/test/test_TrajectoryANEES.py
+-rw-rw-r--   0 jungr     (1000) jungr     (1000)     2031 2024-04-24 11:58:51.000000 cnspy_trajectory_evaluation-0.2.0/test/test_TrajectoryEvaluation.py
+-rw-rw-r--   0 jungr     (1000) jungr     (1000)     3886 2024-04-24 11:58:51.000000 cnspy_trajectory_evaluation-0.2.0/test/test_TrajectoryPosOrientNEES.py
```

### Comparing `cnspy_trajectory_evaluation-0.1.1/PKG-INFO` & `cnspy_trajectory_evaluation-0.2.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,96 +1,110 @@
 Metadata-Version: 2.1
 Name: cnspy_trajectory_evaluation
-Version: 0.1.1
+Version: 0.2.0
 Summary: Evaluation of trajectories.
 Home-page: https://github.com/aau-cns/cnspy_trajectory_evaluation/
 Author: Roland Jung
 Author-email: roland.jung@aau.at
-License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/aau-cns/cnspy_trajectory_evaluation/issues
-Description: # cnspy_trajectory_evaluation
-        
-        The class [TrajectoryEvaluation](./cnspy_trajectory_evaluation/TrajectoryEvaluation.py) evaluates two trajectories given by a CSV-file (estimated and ground-truth), associates their timestamps, aligns them according to a specified scheme, and computes the absolute trajectory error (ATE) and the normalized estimation error square (NEES). The NEES is based on the uncertainty of the estimated trajectory and the ATE. 
-        The results can be plotted and will be saved as [EvaluationReport](./cnspy_trajectory_evaluation/EvaluationReport.py).
-        
-        The CSV-file of the estimated trajectory must contain the pose uncertainty (`CSVFormatPose.PoseWithCov`). For the file format please refer to the [cnspy_spatial_csv_formats](https://github.com/aau-cns/cnspy_spatial_csv_formats) package and the `CSVFormatPose.py` file. 
-        
-        ## Installation
-        
-        Install the current code base from GitHub and pip install a link to that cloned copy
-        ```
-        git clone https://github.com/aau-cns/cnspy_trajectory_evaluation.git
-        cd cnspy_trajectory_evaluation
-        pip install -e .
-        ```
-        
-        
-        ## Dependencies
-        
-        It is part of the [cnspy eco-system](https://github.com/aau-cns/cnspy_eco_system_test) of the [cns-github](https://github.com/aau-cns) group.  
-        Main dependencies are:
-        * [numpy]()
-        * [matplotlib]()
-        * [pandas]()
-        * [scipy]()
-        * [cnspy_timestamp_association](https://github.com/aau-cns/cnspy_timestamp_association)
-        * [cnspy_csv2dataframe](https://github.com/aau-cns/cnspy_csv2dataframe)
-        * [cnspy_spatial_csv_formats](https://github.com/aau-cns/cnspy_spatial_csv_formats)
-        * [cnspy_trajectory](https://github.com/aau-cns/cnspy_trajectory)  
-        
-        ## Definitions and Metrics
-        
-        As mentioned in the introduction, the aim to evaluate an estimated trajectory of a body reference frame with respect to a global/world reference frame against the true/actual trajectory (the so called groundtruth). Compared to [1], we removed the relative trajectory error (RTE) evaluation, as we agree with the authors that it is less straightforward to compare/judge estimation accuracy. In addition to [1], we added the normalized estimation error square (NEES) evaluation as measure for the estimator's credibility as defined in [2]. The NEES, also known as the Mahalonobis distance squared, is a unit-less metric that relates the absolute estimation error to the estimated uncertainty.  
-        
-        The estimated quantities can be modeled in various ways, which directly influences the definition of the uncertainty. E.g. assuming we have two coordinate reference frames `G` (GLOBAL) and `B` (BODY). The estimated states are the position and orientation of `B` with respect to `G`. Now regarding the error definition for the position and velocity, one has two options: (i) the position error with respect to the global frame (common case) or (ii) with respect to the body frame. 
-        As we compute the ATE and the NEES with respect to the global/world reference frame `G`, the uncertainty the position must be expressed in this frame as well. If the uncertainty of the estimator is defined in the body reference frame, it has to be transformed in advance back to the global frame, before the trajectory evaluation is performed. 
-        In case of the orientation, again various possibilities to define the uncertainty exists. 
-        First, different representations of orientations exists: rotation matrices in SO(3), unit quaternions in H, or euler angles in radians or degrees. For indirect (error-state) EKF formulations, the use of quaternions has become a gold standard (OpenVINS, LARVIO, VinsMono), while the trend goes towards representing the error in the tangent space of the corresponding manifold (ROVIO).  
-        Currently, the evaluation tool assumes the orientation uncertainty to refer to the small angle approximations of quaternions `theta`.
-        Thus, the rotational error for quaternions is defined as `q_err = [1; 0.5 * theta]` or as `R_err = eye(3) + skew(theta)` for SO(3) matrices.
-        The rotational error is defined as `R_G_B_err = R_G_B_true^T * R_G_B_est`, leading to local perturbations (EQ. 190 in [3]). Note that rotation matrices and unit-quaternions can be mapped directly `R_A_B = R(q_A_B)`, reading as the orientation of `B` with respect to `A`. This means that the uncertainty of the orientation/attitude has to be defined in the local/body reference frame `B`.
-        
-        ## Examples
-        
-        Please refer to the unit-test sections in the directory `test`.
-        
-        ### position error plot
-        
-        ![p_ARMSE](./doc/p_ARMSE.png "p_ARMSE")
-        
-        ### Pose error plot
-        
-        ![pose-err-plot](./doc/pose-err-plot.png "pose-err-plot")
-        
-        ### Pose NEES plot
-        
-        ![pose-nees](./doc/pose-nees.png "pose-nees")
-        
-        ## Credits
-        
-        The classes `AbsoluteTrajectoryError` and `SpatialAlignment` of the  package `trajectory_evaluation` are based on the preliminary work of the  [Robotics and Perception Group, ETH Zurich](http://rpg.ifi.uzh.ch/index.html).
-        
-        
-        1) From ETH Zurich: [rpg_trajectory_evaluation](https://github.com/uzh-rpg/rpg_trajectory_evaluation) released by Zichao Zhang and Davide Scaramuzza with [1]. 
-        
-        ## References
-        
-        [1] Z. Zhang and D. Scaramuzza, "A Tutorial on Quantitative Trajectory Evaluation for Visual(-Inertial) Odometry," 2018 IEEE/RSJ International Conference on Intelligent Robots and Systems (IROS), Madrid, Spain, 2018, pp. 7244-7251, doi: 10.1109/IROS.2018.8593941.
-        
-        [2] X. R. Li, Z. Zhao and X. Li, "Evaluation of Estimation Algorithms: Credibility Tests," in IEEE Transactions on Systems, Man, and Cybernetics - Part A: Systems and Humans, vol. 42, no. 1, pp. 147-163, Jan. 2012, doi: 10.1109/TSMCA.2011.2158095.
-        
-        [3] Joan Solà, "Quaternion kinematics for the error-state Kalman filter", 2017 arXiv, eprint: 1711.02508.
-        
-        ## License
-        
-        Software License Agreement (GNU GPLv3  License), refer to the LICENSE file.
-        
-        *Sharing is caring!* - [Roland Jung](https://github.com/jungr-ait)  
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENCE
+Requires-Dist: numpy
+Requires-Dist: pandas
+Requires-Dist: spatialmath-python
+Requires-Dist: scipy
+Requires-Dist: matplotlib
+Requires-Dist: joblib
+Requires-Dist: configparser
+Requires-Dist: cnspy_numpy_utils
+Requires-Dist: cnspy_trajectory
+Requires-Dist: cnspy_timestamp_association
+Requires-Dist: cnspy_spatial_csv_formats
+Requires-Dist: cnspy_csv2dataframe
+
+# cnspy_trajectory_evaluation
+
+The class [TrajectoryEvaluation](./cnspy_trajectory_evaluation/TrajectoryEvaluation.py) evaluates two trajectories given by a CSV-file (estimated and ground-truth), associates their timestamps, aligns them according to a specified scheme, and computes the absolute trajectory error (ATE) and the normalized estimation error square (NEES). The NEES is based on the uncertainty of the estimated trajectory and the ATE. 
+The results can be plotted and will be saved as [EvaluationReport](./cnspy_trajectory_evaluation/EvaluationReport.py).
+
+The CSV-file of the estimated trajectory must contain the pose uncertainty (`CSVFormatPose.PoseWithCov`). For the file format please refer to the [cnspy_spatial_csv_formats](https://github.com/aau-cns/cnspy_spatial_csv_formats) package and the `CSVFormatPose.py` file. 
+
+## Installation
+
+Install the current code base from GitHub and pip install a link to that cloned copy
+```
+git clone https://github.com/aau-cns/cnspy_trajectory_evaluation.git
+cd cnspy_trajectory_evaluation
+pip install -e .
+```
+or the [official package](https://pypi.org/project/cnspy-trajectory-evaluation/) via
+```commandline
+pip install cnspy-trajectory-evaluation
+```
+
+## Dependencies
+
+It is part of the [cnspy eco-system](https://github.com/aau-cns/cnspy_eco_system_test) of the [cns-github](https://github.com/aau-cns) group.  
+Main dependencies are:
+* [numpy]()
+* [matplotlib]()
+* [pandas]()
+* [scipy]()
+* [cnspy_timestamp_association](https://github.com/aau-cns/cnspy_timestamp_association)
+* [cnspy_csv2dataframe](https://github.com/aau-cns/cnspy_csv2dataframe)
+* [cnspy_spatial_csv_formats](https://github.com/aau-cns/cnspy_spatial_csv_formats)
+* [cnspy_trajectory](https://github.com/aau-cns/cnspy_trajectory)  
+
+## Definitions and Metrics
+
+As mentioned in the introduction, the aim to evaluate an estimated trajectory of a body reference frame with respect to a global/world reference frame against the true/actual trajectory (the so called groundtruth). Compared to [1], we removed the relative trajectory error (RTE) evaluation, as we agree with the authors that it is less straightforward to compare/judge estimation accuracy. In addition to [1], we added the normalized estimation error square (NEES) evaluation as measure for the estimator's credibility as defined in [2]. The NEES, also known as the Mahalonobis distance squared, is a unit-less metric that relates the absolute estimation error to the estimated uncertainty.  
+
+The estimated quantities can be modeled in various ways, which directly influences the definition of the uncertainty. E.g. assuming we have two coordinate reference frames `G` (GLOBAL) and `B` (BODY). The estimated states are the position and orientation of `B` with respect to `G`. Now regarding the error definition for the position and velocity, one has two options: (i) the position error with respect to the global frame (common case) or (ii) with respect to the body frame. 
+As we compute the ATE and the NEES with respect to the global/world reference frame `G`, the uncertainty the position must be expressed in this frame as well. If the uncertainty of the estimator is defined in the body reference frame, it has to be transformed in advance back to the global frame, before the trajectory evaluation is performed. 
+In case of the orientation, again various possibilities to define the uncertainty exists. 
+First, different representations of orientations exists: rotation matrices in SO(3), unit quaternions in H, or euler angles in radians or degrees. For indirect (error-state) EKF formulations, the use of quaternions has become a gold standard (OpenVINS, LARVIO, VinsMono), while the trend goes towards representing the error in the tangent space of the corresponding manifold (ROVIO).  
+Currently, the evaluation tool assumes the orientation uncertainty to refer to the small angle approximations of quaternions `theta`.
+Thus, the rotational error for quaternions is defined as `q_err = [1; 0.5 * theta]` or as `R_err = eye(3) + skew(theta)` for SO(3) matrices.
+The rotational error is defined as `R_G_B_err = R_G_B_true^T * R_G_B_est`, leading to local perturbations (EQ. 190 in [3]). Note that rotation matrices and unit-quaternions can be mapped directly `R_A_B = R(q_A_B)`, reading as the orientation of `B` with respect to `A`. This means that the uncertainty of the orientation/attitude has to be defined in the local/body reference frame `B`.
+
+## Examples
+
+Please refer to the unit-test sections in the directory `test`.
+
+### position error plot
+
+![p_ARMSE](./doc/p_ARMSE.png "p_ARMSE")
+
+### Pose error plot
+
+![pose-err-plot](./doc/pose-err-plot.png "pose-err-plot")
+
+### Pose NEES plot
+
+![pose-nees](./doc/pose-nees.png "pose-nees")
+
+## Credits
+
+The classes `AbsoluteTrajectoryError` and `SpatialAlignment` of the  package `trajectory_evaluation` are based on the preliminary work of the  [Robotics and Perception Group, ETH Zurich](http://rpg.ifi.uzh.ch/index.html).
+
+
+1) From ETH Zurich: [rpg_trajectory_evaluation](https://github.com/uzh-rpg/rpg_trajectory_evaluation) released by Zichao Zhang and Davide Scaramuzza with [1]. 
+
+## References
+
+[1] Z. Zhang and D. Scaramuzza, "A Tutorial on Quantitative Trajectory Evaluation for Visual(-Inertial) Odometry," 2018 IEEE/RSJ International Conference on Intelligent Robots and Systems (IROS), Madrid, Spain, 2018, pp. 7244-7251, doi: 10.1109/IROS.2018.8593941.
+
+[2] X. R. Li, Z. Zhao and X. Li, "Evaluation of Estimation Algorithms: Credibility Tests," in IEEE Transactions on Systems, Man, and Cybernetics - Part A: Systems and Humans, vol. 42, no. 1, pp. 147-163, Jan. 2012, doi: 10.1109/TSMCA.2011.2158095.
+
+[3] Joan Solà, "Quaternion kinematics for the error-state Kalman filter", 2017 arXiv, eprint: 1711.02508.
+
+## License
+
+Software License Agreement (GNU GPLv3  License), refer to the LICENSE file.
+
+*Sharing is caring!* - [Roland Jung](https://github.com/jungr-ait)
```

### Comparing `cnspy_trajectory_evaluation-0.1.1/README.md` & `cnspy_trajectory_evaluation-0.2.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,18 @@
 
 Install the current code base from GitHub and pip install a link to that cloned copy
 ```
 git clone https://github.com/aau-cns/cnspy_trajectory_evaluation.git
 cd cnspy_trajectory_evaluation
 pip install -e .
 ```
-
+or the [official package](https://pypi.org/project/cnspy-trajectory-evaluation/) via
+```commandline
+pip install cnspy-trajectory-evaluation
+```
 
 ## Dependencies
 
 It is part of the [cnspy eco-system](https://github.com/aau-cns/cnspy_eco_system_test) of the [cns-github](https://github.com/aau-cns) group.  
 Main dependencies are:
 * [numpy]()
 * [matplotlib]()
```

### Comparing `cnspy_trajectory_evaluation-0.1.1/cnspy_trajectory_evaluation/AlignedTrajectories.py` & `cnspy_trajectory_evaluation-0.2.0/cnspy_trajectory_evaluation/AlignedTrajectories.py`

 * *Files 11% similar despite different names*

```diff
@@ -21,34 +21,43 @@
 ########################################################################################################################
 import os
 
 from cnspy_trajectory_evaluation.AssociatedTrajectories import AssociatedTrajectories
 from cnspy_trajectory_evaluation.TrajectoryAlignmentTypes import TrajectoryAlignmentTypes
 
 
+# TODO: align the gt trajectory to the estimated one, as the estimated global covariance
+#  would need to be transformed as well!
 class AlignedTrajectories:
     traj_est_matched_aligned = None
     traj_gt_matched = None
+    alignment_type = TrajectoryAlignmentTypes.none
 
-    def __init__(self, associated, alignment_type=TrajectoryAlignmentTypes.sim3, num_frames=-1):
+    def __init__(self, associated=None, traj_gt_matched=None, traj_est_matched=None,
+                 alignment_type=TrajectoryAlignmentTypes.sim3, num_frames=-1):
+        self.alignment_type = alignment_type
 
-        #        assert (isinstance(associated, AssociatedTrajectories))
+        if associated is not None:
+            assert (isinstance(associated, AssociatedTrajectories))
+            traj_est_matched, self.traj_gt_matched = associated.get_trajectories()
+        else:
+            self.traj_gt_matched = traj_gt_matched
 
-        self.traj_est_matched_aligned, self.traj_gt_matched = associated.get_trajectories()
 
-        s, R, t = TrajectoryAlignmentTypes.trajectory_aligment(self.traj_est_matched_aligned, self.traj_gt_matched,
+        s, R_gt_est, t_gt_est_in_gt = TrajectoryAlignmentTypes.trajectory_aligment(traj_est_matched, self.traj_gt_matched,
                                                                method=alignment_type,
                                                                num_frames=num_frames)
 
-        self.traj_est_matched_aligned.transform(scale=s, t=t, R=R)
+        self.traj_est_matched_aligned = traj_est_matched.clone()
+        self.traj_est_matched_aligned.transform(scale=s, p_GN_in_G=t_gt_est_in_gt, R_GN=R_gt_est)
 
     def save(self, result_dir='.', prefix=None):
         if not prefix:
             prefix = ""
 
         if not os.path.exists(result_dir):
             os.makedirs(os.path.abspath(result_dir))
         self.traj_est_matched_aligned.save_to_CSV(
-            os.path.join(result_dir, str(prefix) + 'est_matched_aligned.csv'))
+            os.path.join(result_dir, str(prefix) + 'est_matched_aligned_' + str(self.alignment_type) + '.csv'))
         self.traj_gt_matched.save_to_CSV(
             os.path.join(result_dir, str(prefix) + 'gt_matched_aligned.csv'))
```

### Comparing `cnspy_trajectory_evaluation-0.1.1/cnspy_trajectory_evaluation/EvaluationReport.py` & `cnspy_trajectory_evaluation-0.2.0/cnspy_trajectory_evaluation/EvaluationReport.py`

 * *Files 16% similar despite different names*

```diff
@@ -17,39 +17,42 @@
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 #
 # Requirements:
 # configparser
 ########################################################################################################################
 import configparser
 
+# TODO: to compute the ANEES of multiple runs, the NEES-vectors and timestamps need to be stored! As they need to be associated later again.
+# TODO: the EvaluationReport does not reflect a real ANEES, only the average NEES over a single run!
 
 class EvaluationReport:
     def __init__(self, directory='', fn_gt='', fn_est='', alignment='none',
-                 num_aligned_samples=0, ANEES_p=0.0, ANEES_q=0.0, RMSE_p=0.0, RMSE_q=0.0):
+                 num_aligned_samples=0, num_runs=0, ANEES_p=0.0, ANEES_R=0.0, ARMSE_p=0.0, ARMSE_R=0.0):
         self.directory = directory
         self.fn_gt = fn_gt
         self.fn_est = fn_est
         self.alignment = str(alignment)
         self.num_aligned_samples = int(num_aligned_samples)
+        self.num_runs = int(num_runs)
         self.ANEES_p = ANEES_p
-        self.ANEES_q = ANEES_q
-        self.ARMSE_p = RMSE_p
-        self.ARMSE_q = RMSE_q
+        self.ANEES_R = ANEES_R
+        self.ARMSE_p = ARMSE_p
+        self.ARMSE_R = ARMSE_R
 
     def save(self, fn):
         config = configparser.ConfigParser()
         config['EvaluationReport'] = {'directory': self.directory,
                                       'fn_gt': self.fn_gt,
                                       'fn_est': self.fn_est,
                                       'alignment': self.alignment,
                                       'num_aligned_samples': self.num_aligned_samples,
                                       'ANEES_p': self.ANEES_p,
-                                      'ANEES_q': self.ANEES_q,
+                                      'ANEES_R': self.ANEES_R,
                                       'ARMSE_p': self.ARMSE_p,
-                                      'ARMSE_q': self.ARMSE_q}
+                                      'ARMSE_R': self.ARMSE_R}
         # print('Save config file....')
         with open(fn, 'w') as configfile:
             config.write(configfile)
             configfile.close()
 
     def load(self, fn):
         config = configparser.ConfigParser()
@@ -57,11 +60,11 @@
         config.read(fn)
         # print('load from section')
         section = config['EvaluationReport']
         self.directory = section.get('directory', 'default')
         self.fn_gt = section.get('fn_gt', 'default')
         self.fn_est = section.get('fn_est', 'default')
         self.ANEES_p = section.get('ANEES_p', 'default')
-        self.ANEES_q = section.get('ANEES_q', 'default')
+        self.ANEES_R = section.get('ANEES_R', 'default')
         self.ARMSE_p = section.get('ARMSE_p', 'default')
-        self.ARMSE_q = section.get('ARMSE_q', 'default')
+        self.ARMSE_R = section.get('ARMSE_R', 'default')
```

### Comparing `cnspy_trajectory_evaluation-0.1.1/cnspy_trajectory_evaluation.egg-info/PKG-INFO` & `cnspy_trajectory_evaluation-0.2.0/cnspy_trajectory_evaluation.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,96 +1,110 @@
 Metadata-Version: 2.1
-Name: cnspy-trajectory-evaluation
-Version: 0.1.1
+Name: cnspy_trajectory_evaluation
+Version: 0.2.0
 Summary: Evaluation of trajectories.
 Home-page: https://github.com/aau-cns/cnspy_trajectory_evaluation/
 Author: Roland Jung
 Author-email: roland.jung@aau.at
-License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/aau-cns/cnspy_trajectory_evaluation/issues
-Description: # cnspy_trajectory_evaluation
-        
-        The class [TrajectoryEvaluation](./cnspy_trajectory_evaluation/TrajectoryEvaluation.py) evaluates two trajectories given by a CSV-file (estimated and ground-truth), associates their timestamps, aligns them according to a specified scheme, and computes the absolute trajectory error (ATE) and the normalized estimation error square (NEES). The NEES is based on the uncertainty of the estimated trajectory and the ATE. 
-        The results can be plotted and will be saved as [EvaluationReport](./cnspy_trajectory_evaluation/EvaluationReport.py).
-        
-        The CSV-file of the estimated trajectory must contain the pose uncertainty (`CSVFormatPose.PoseWithCov`). For the file format please refer to the [cnspy_spatial_csv_formats](https://github.com/aau-cns/cnspy_spatial_csv_formats) package and the `CSVFormatPose.py` file. 
-        
-        ## Installation
-        
-        Install the current code base from GitHub and pip install a link to that cloned copy
-        ```
-        git clone https://github.com/aau-cns/cnspy_trajectory_evaluation.git
-        cd cnspy_trajectory_evaluation
-        pip install -e .
-        ```
-        
-        
-        ## Dependencies
-        
-        It is part of the [cnspy eco-system](https://github.com/aau-cns/cnspy_eco_system_test) of the [cns-github](https://github.com/aau-cns) group.  
-        Main dependencies are:
-        * [numpy]()
-        * [matplotlib]()
-        * [pandas]()
-        * [scipy]()
-        * [cnspy_timestamp_association](https://github.com/aau-cns/cnspy_timestamp_association)
-        * [cnspy_csv2dataframe](https://github.com/aau-cns/cnspy_csv2dataframe)
-        * [cnspy_spatial_csv_formats](https://github.com/aau-cns/cnspy_spatial_csv_formats)
-        * [cnspy_trajectory](https://github.com/aau-cns/cnspy_trajectory)  
-        
-        ## Definitions and Metrics
-        
-        As mentioned in the introduction, the aim to evaluate an estimated trajectory of a body reference frame with respect to a global/world reference frame against the true/actual trajectory (the so called groundtruth). Compared to [1], we removed the relative trajectory error (RTE) evaluation, as we agree with the authors that it is less straightforward to compare/judge estimation accuracy. In addition to [1], we added the normalized estimation error square (NEES) evaluation as measure for the estimator's credibility as defined in [2]. The NEES, also known as the Mahalonobis distance squared, is a unit-less metric that relates the absolute estimation error to the estimated uncertainty.  
-        
-        The estimated quantities can be modeled in various ways, which directly influences the definition of the uncertainty. E.g. assuming we have two coordinate reference frames `G` (GLOBAL) and `B` (BODY). The estimated states are the position and orientation of `B` with respect to `G`. Now regarding the error definition for the position and velocity, one has two options: (i) the position error with respect to the global frame (common case) or (ii) with respect to the body frame. 
-        As we compute the ATE and the NEES with respect to the global/world reference frame `G`, the uncertainty the position must be expressed in this frame as well. If the uncertainty of the estimator is defined in the body reference frame, it has to be transformed in advance back to the global frame, before the trajectory evaluation is performed. 
-        In case of the orientation, again various possibilities to define the uncertainty exists. 
-        First, different representations of orientations exists: rotation matrices in SO(3), unit quaternions in H, or euler angles in radians or degrees. For indirect (error-state) EKF formulations, the use of quaternions has become a gold standard (OpenVINS, LARVIO, VinsMono), while the trend goes towards representing the error in the tangent space of the corresponding manifold (ROVIO).  
-        Currently, the evaluation tool assumes the orientation uncertainty to refer to the small angle approximations of quaternions `theta`.
-        Thus, the rotational error for quaternions is defined as `q_err = [1; 0.5 * theta]` or as `R_err = eye(3) + skew(theta)` for SO(3) matrices.
-        The rotational error is defined as `R_G_B_err = R_G_B_true^T * R_G_B_est`, leading to local perturbations (EQ. 190 in [3]). Note that rotation matrices and unit-quaternions can be mapped directly `R_A_B = R(q_A_B)`, reading as the orientation of `B` with respect to `A`. This means that the uncertainty of the orientation/attitude has to be defined in the local/body reference frame `B`.
-        
-        ## Examples
-        
-        Please refer to the unit-test sections in the directory `test`.
-        
-        ### position error plot
-        
-        ![p_ARMSE](./doc/p_ARMSE.png "p_ARMSE")
-        
-        ### Pose error plot
-        
-        ![pose-err-plot](./doc/pose-err-plot.png "pose-err-plot")
-        
-        ### Pose NEES plot
-        
-        ![pose-nees](./doc/pose-nees.png "pose-nees")
-        
-        ## Credits
-        
-        The classes `AbsoluteTrajectoryError` and `SpatialAlignment` of the  package `trajectory_evaluation` are based on the preliminary work of the  [Robotics and Perception Group, ETH Zurich](http://rpg.ifi.uzh.ch/index.html).
-        
-        
-        1) From ETH Zurich: [rpg_trajectory_evaluation](https://github.com/uzh-rpg/rpg_trajectory_evaluation) released by Zichao Zhang and Davide Scaramuzza with [1]. 
-        
-        ## References
-        
-        [1] Z. Zhang and D. Scaramuzza, "A Tutorial on Quantitative Trajectory Evaluation for Visual(-Inertial) Odometry," 2018 IEEE/RSJ International Conference on Intelligent Robots and Systems (IROS), Madrid, Spain, 2018, pp. 7244-7251, doi: 10.1109/IROS.2018.8593941.
-        
-        [2] X. R. Li, Z. Zhao and X. Li, "Evaluation of Estimation Algorithms: Credibility Tests," in IEEE Transactions on Systems, Man, and Cybernetics - Part A: Systems and Humans, vol. 42, no. 1, pp. 147-163, Jan. 2012, doi: 10.1109/TSMCA.2011.2158095.
-        
-        [3] Joan Solà, "Quaternion kinematics for the error-state Kalman filter", 2017 arXiv, eprint: 1711.02508.
-        
-        ## License
-        
-        Software License Agreement (GNU GPLv3  License), refer to the LICENSE file.
-        
-        *Sharing is caring!* - [Roland Jung](https://github.com/jungr-ait)  
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENCE
+Requires-Dist: numpy
+Requires-Dist: pandas
+Requires-Dist: spatialmath-python
+Requires-Dist: scipy
+Requires-Dist: matplotlib
+Requires-Dist: joblib
+Requires-Dist: configparser
+Requires-Dist: cnspy_numpy_utils
+Requires-Dist: cnspy_trajectory
+Requires-Dist: cnspy_timestamp_association
+Requires-Dist: cnspy_spatial_csv_formats
+Requires-Dist: cnspy_csv2dataframe
+
+# cnspy_trajectory_evaluation
+
+The class [TrajectoryEvaluation](./cnspy_trajectory_evaluation/TrajectoryEvaluation.py) evaluates two trajectories given by a CSV-file (estimated and ground-truth), associates their timestamps, aligns them according to a specified scheme, and computes the absolute trajectory error (ATE) and the normalized estimation error square (NEES). The NEES is based on the uncertainty of the estimated trajectory and the ATE. 
+The results can be plotted and will be saved as [EvaluationReport](./cnspy_trajectory_evaluation/EvaluationReport.py).
+
+The CSV-file of the estimated trajectory must contain the pose uncertainty (`CSVFormatPose.PoseWithCov`). For the file format please refer to the [cnspy_spatial_csv_formats](https://github.com/aau-cns/cnspy_spatial_csv_formats) package and the `CSVFormatPose.py` file. 
+
+## Installation
+
+Install the current code base from GitHub and pip install a link to that cloned copy
+```
+git clone https://github.com/aau-cns/cnspy_trajectory_evaluation.git
+cd cnspy_trajectory_evaluation
+pip install -e .
+```
+or the [official package](https://pypi.org/project/cnspy-trajectory-evaluation/) via
+```commandline
+pip install cnspy-trajectory-evaluation
+```
+
+## Dependencies
+
+It is part of the [cnspy eco-system](https://github.com/aau-cns/cnspy_eco_system_test) of the [cns-github](https://github.com/aau-cns) group.  
+Main dependencies are:
+* [numpy]()
+* [matplotlib]()
+* [pandas]()
+* [scipy]()
+* [cnspy_timestamp_association](https://github.com/aau-cns/cnspy_timestamp_association)
+* [cnspy_csv2dataframe](https://github.com/aau-cns/cnspy_csv2dataframe)
+* [cnspy_spatial_csv_formats](https://github.com/aau-cns/cnspy_spatial_csv_formats)
+* [cnspy_trajectory](https://github.com/aau-cns/cnspy_trajectory)  
+
+## Definitions and Metrics
+
+As mentioned in the introduction, the aim to evaluate an estimated trajectory of a body reference frame with respect to a global/world reference frame against the true/actual trajectory (the so called groundtruth). Compared to [1], we removed the relative trajectory error (RTE) evaluation, as we agree with the authors that it is less straightforward to compare/judge estimation accuracy. In addition to [1], we added the normalized estimation error square (NEES) evaluation as measure for the estimator's credibility as defined in [2]. The NEES, also known as the Mahalonobis distance squared, is a unit-less metric that relates the absolute estimation error to the estimated uncertainty.  
+
+The estimated quantities can be modeled in various ways, which directly influences the definition of the uncertainty. E.g. assuming we have two coordinate reference frames `G` (GLOBAL) and `B` (BODY). The estimated states are the position and orientation of `B` with respect to `G`. Now regarding the error definition for the position and velocity, one has two options: (i) the position error with respect to the global frame (common case) or (ii) with respect to the body frame. 
+As we compute the ATE and the NEES with respect to the global/world reference frame `G`, the uncertainty the position must be expressed in this frame as well. If the uncertainty of the estimator is defined in the body reference frame, it has to be transformed in advance back to the global frame, before the trajectory evaluation is performed. 
+In case of the orientation, again various possibilities to define the uncertainty exists. 
+First, different representations of orientations exists: rotation matrices in SO(3), unit quaternions in H, or euler angles in radians or degrees. For indirect (error-state) EKF formulations, the use of quaternions has become a gold standard (OpenVINS, LARVIO, VinsMono), while the trend goes towards representing the error in the tangent space of the corresponding manifold (ROVIO).  
+Currently, the evaluation tool assumes the orientation uncertainty to refer to the small angle approximations of quaternions `theta`.
+Thus, the rotational error for quaternions is defined as `q_err = [1; 0.5 * theta]` or as `R_err = eye(3) + skew(theta)` for SO(3) matrices.
+The rotational error is defined as `R_G_B_err = R_G_B_true^T * R_G_B_est`, leading to local perturbations (EQ. 190 in [3]). Note that rotation matrices and unit-quaternions can be mapped directly `R_A_B = R(q_A_B)`, reading as the orientation of `B` with respect to `A`. This means that the uncertainty of the orientation/attitude has to be defined in the local/body reference frame `B`.
+
+## Examples
+
+Please refer to the unit-test sections in the directory `test`.
+
+### position error plot
+
+![p_ARMSE](./doc/p_ARMSE.png "p_ARMSE")
+
+### Pose error plot
+
+![pose-err-plot](./doc/pose-err-plot.png "pose-err-plot")
+
+### Pose NEES plot
+
+![pose-nees](./doc/pose-nees.png "pose-nees")
+
+## Credits
+
+The classes `AbsoluteTrajectoryError` and `SpatialAlignment` of the  package `trajectory_evaluation` are based on the preliminary work of the  [Robotics and Perception Group, ETH Zurich](http://rpg.ifi.uzh.ch/index.html).
+
+
+1) From ETH Zurich: [rpg_trajectory_evaluation](https://github.com/uzh-rpg/rpg_trajectory_evaluation) released by Zichao Zhang and Davide Scaramuzza with [1]. 
+
+## References
+
+[1] Z. Zhang and D. Scaramuzza, "A Tutorial on Quantitative Trajectory Evaluation for Visual(-Inertial) Odometry," 2018 IEEE/RSJ International Conference on Intelligent Robots and Systems (IROS), Madrid, Spain, 2018, pp. 7244-7251, doi: 10.1109/IROS.2018.8593941.
+
+[2] X. R. Li, Z. Zhao and X. Li, "Evaluation of Estimation Algorithms: Credibility Tests," in IEEE Transactions on Systems, Man, and Cybernetics - Part A: Systems and Humans, vol. 42, no. 1, pp. 147-163, Jan. 2012, doi: 10.1109/TSMCA.2011.2158095.
+
+[3] Joan Solà, "Quaternion kinematics for the error-state Kalman filter", 2017 arXiv, eprint: 1711.02508.
+
+## License
+
+Software License Agreement (GNU GPLv3  License), refer to the LICENSE file.
+
+*Sharing is caring!* - [Roland Jung](https://github.com/jungr-ait)
```

### Comparing `cnspy_trajectory_evaluation-0.1.1/cnspy_trajectory_evaluation.egg-info/SOURCES.txt` & `cnspy_trajectory_evaluation-0.2.0/cnspy_trajectory_evaluation.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,31 @@
+LICENCE
 README.md
 setup.py
 cnspy_trajectory_evaluation/AbsoluteTrajectoryError.py
 cnspy_trajectory_evaluation/AlignedTrajectories.py
 cnspy_trajectory_evaluation/AssociatedTrajectories.py
+cnspy_trajectory_evaluation/DifferentialTrajectoryError.py
+cnspy_trajectory_evaluation/EstimationTrajectoryError.py
 cnspy_trajectory_evaluation/EvaluationReport.py
+cnspy_trajectory_evaluation/ICP.py
 cnspy_trajectory_evaluation/SpatialAlignment.py
+cnspy_trajectory_evaluation/TrajectoryANEES.py
 cnspy_trajectory_evaluation/TrajectoryAlignmentTypes.py
 cnspy_trajectory_evaluation/TrajectoryEvaluation.py
-cnspy_trajectory_evaluation/TrajectoryNEES.py
+cnspy_trajectory_evaluation/TrajectoryPosOrientNEES.py
 cnspy_trajectory_evaluation/__init__.py
 cnspy_trajectory_evaluation.egg-info/PKG-INFO
 cnspy_trajectory_evaluation.egg-info/SOURCES.txt
 cnspy_trajectory_evaluation.egg-info/dependency_links.txt
 cnspy_trajectory_evaluation.egg-info/requires.txt
 cnspy_trajectory_evaluation.egg-info/top_level.txt
 test/__init__.py
 test/pandas_test.py
 test/test_AbsoluteTrajectoryError.py
 test/test_AlignedTrajectories.py
+test/test_DifferentialTrajectoryError.py
 test/test_EvaluationReport.py
+test/test_OV_TrajectoryEvaluation.py
+test/test_TrajectoryANEES.py
 test/test_TrajectoryEvaluation.py
-test/test_TrajectoryNEES.py
+test/test_TrajectoryPosOrientNEES.py
```

### Comparing `cnspy_trajectory_evaluation-0.1.1/setup.py` & `cnspy_trajectory_evaluation-0.2.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,9 +31,9 @@
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Operating System :: OS Independent",
     ],
     
     packages=find_packages(exclude=["test_*", "TODO*"]),
     python_requires='>=3.6',
-    install_requires=['numpy', 'pandas', 'spatialmath-python', 'scipy', 'matplotlib', 'configparser', 'cnspy_numpy_utils', 'cnspy_trajectory', 'cnspy_timestamp_association', 'cnspy_spatial_csv_formats', 'cnspy_csv2dataframe' ],
+    install_requires=['numpy', 'pandas', 'spatialmath-python', 'scipy', 'matplotlib', 'joblib', 'configparser', 'cnspy_numpy_utils', 'cnspy_trajectory', 'cnspy_timestamp_association', 'cnspy_spatial_csv_formats', 'cnspy_csv2dataframe' ],
 )
```

### Comparing `cnspy_trajectory_evaluation-0.1.1/test/pandas_test.py` & `cnspy_trajectory_evaluation-0.2.0/test/pandas_test.py`

 * *Files identical despite different names*

### Comparing `cnspy_trajectory_evaluation-0.1.1/test/test_AlignedTrajectories.py` & `cnspy_trajectory_evaluation-0.2.0/test/test_TrajectoryANEES.py`

 * *Files 15% similar despite different names*

```diff
@@ -16,49 +16,69 @@
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 #
 ########################################################################################################################
 import os
 import unittest
 import time
-from cnspy_trajectory.Trajectory import Trajectory
-from cnspy_trajectory.TrajectoryPlotter import TrajectoryPlotter
-from cnspy_trajectory.TrajectoryPlotConfig import TrajectoryPlotConfig
-from cnspy_trajectory_evaluation.AlignedTrajectories import *
+
+from cnspy_trajectory.TrajectoryEstimated import TrajectoryEstimated
+from cnspy_trajectory_evaluation.TrajectoryANEES import TrajectoryANEES
+from cnspy_trajectory_evaluation.TrajectoryEvaluation import *
 
 SAMPLE_DATA_DIR = os.path.join(os.path.dirname(os.path.abspath(__file__)), 'sample_data')
 
-class AlignedTrajectories_Test(unittest.TestCase):
+
+class TrajectoryANNES_Test(unittest.TestCase):
     start_time = None
 
     def start(self):
         self.start_time = time.time()
 
-    def stop(self):
-        print("Process time: " + str((time.time() - self.start_time)))
+    def stop(self, info="Process time"):
+        print(str(info) + " took : " + str((time.time() - self.start_time)) + " [sec]")
 
-    def get_associated(self):
-        fn_gt_csv = str(SAMPLE_DATA_DIR + '/ID1-pose-gt.csv')
-        fn_est_csv = str(SAMPLE_DATA_DIR + '/ID1-pose-est-cov.csv')
-        return AssociatedTrajectories(fn_est=fn_est_csv, fn_gt=fn_gt_csv)
+    def get_trajectories(self):
+        fn_gt_csv = str(SAMPLE_DATA_DIR + '/MC/ID1-pose-gt.csv')
+        traj_gt = Trajectory(fn=fn_gt_csv)
+        traj_est_arr = []
+        for i in range(11):
+            fn_est_csv = str(SAMPLE_DATA_DIR + '/MC/ID1-pose-est-posorient-cov-run{}.csv'.format(i+1))
+            traj_est_i = TrajectoryEstimated(fn=fn_est_csv)
+            traj_est_arr.append(traj_est_i)
+        return traj_gt, traj_est_arr
 
     def test_init(self):
         self.start()
-        associated = self.get_associated()
-        self.stop()
+        traj_gt, traj_est_arr = self.get_trajectories()
+        self.stop(info="Loading trajectories")
+
+        self.start()
+        NEES_arr, ETE_arr, EST_aligned_arr, traj_gt_matched = \
+            TrajectoryANEES.evaluate(traj_gt,
+                                     traj_est_arr,
+                                     max_difference=0.01,
+                                     round_decimals=4,
+                                     unique_timestamps=True,
+                                     alignment_type=TrajectoryAlignmentTypes.none,
+                                     num_aligned_samples=1)
+        self.stop(info="Evaluating trajectories")
+
+        self.start()
+        ANEES = TrajectoryANEES(NEES_arr=NEES_arr)
+        self.stop(info="ANEES ")
+
+        self.start()
+        result_dir = str(SAMPLE_DATA_DIR + '/results/MC')
+        for i in range(len(NEES_arr)):
+            NEES_arr[i].plot(cfg=TrajectoryPlotConfig(show=False, close_figure=True,
+                                            result_dir=result_dir, save_fn='NEES_{}.jpg'.format(i)))
+
 
-    def test_align_trajectories(self):
-        associated = self.get_associated()
-        aligned = AlignedTrajectories(associated=associated)
-        aligned.save(result_dir=str(SAMPLE_DATA_DIR + '/results/'))
-        traj_est_matched = Trajectory(df=associated.data_frame_est_matched)
-        plot_gt = TrajectoryPlotter(traj_obj=aligned.traj_gt_matched)
-        plot_est = TrajectoryPlotter(traj_obj=traj_est_matched)
-        plot_est_aligned = TrajectoryPlotter(traj_obj=aligned.traj_est_matched_aligned)
-
-        TrajectoryPlotter.multi_plot_3D(traj_plotter_list=[plot_gt, plot_est, plot_est_aligned],
-                                        cfg=TrajectoryPlotConfig(),
-                                        name_list=['gt_matched', 'est_matched', 'est_matched_aligned'])
 
+        fn_ANEES = 'ANEES.jpg'
+        ANEES.plot(cfg=TrajectoryPlotConfig(show=True, close_figure=False,
+                                            result_dir=result_dir, save_fn=fn_ANEES))
+        self.stop(info="ANEES plots ")
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `cnspy_trajectory_evaluation-0.1.1/test/test_EvaluationReport.py` & `cnspy_trajectory_evaluation-0.2.0/test/test_EvaluationReport.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,27 +31,27 @@
         self.start_time = time.time()
 
     def stop(self, info="Process time"):
         print(str(info) + " took : " + str((time.time() - self.start_time)) + " [sec]")
 
     def get_fn(self):
         fn_gt_csv = str(SAMPLE_DATA_DIR + '/ID1-pose-gt.csv')
-        fn_est_csv = str(SAMPLE_DATA_DIR + '/ID1-pose-est-cov.csv')
+        fn_est_csv = str(SAMPLE_DATA_DIR + '/ID1-pose-est-posorient-cov.csv')
         return fn_gt_csv, fn_est_csv
 
     def test_init(self):
         self.start()
         report = EvaluationReport()
         report.directory = ''
         report.fn_gt = str(SAMPLE_DATA_DIR + '/ID1-pose-gt.csv')
-        report.fn_est = str(SAMPLE_DATA_DIR + '/ID1-pose-est-cov.csv')
+        report.fn_est = str(SAMPLE_DATA_DIR + '/ID1-pose-est-posorient-cov.csv')
         report.ANEES_p = 0.1
-        report.ANEES_q = 0.2
+        report.ANEES_R = 0.2
         report.ARMSE_p = 0.3
-        report.ARMSE_q = 0.4
+        report.ARMSE_R = 0.4
 
         fn = str(SAMPLE_DATA_DIR + '/results/eval-report.ini')
         report.save(fn)
 
         report_ = EvaluationReport()
         report_.load(fn)
```

### Comparing `cnspy_trajectory_evaluation-0.1.1/test/test_TrajectoryEvaluation.py` & `cnspy_trajectory_evaluation-0.2.0/test/test_TrajectoryEvaluation.py`

 * *Files 9% similar despite different names*

```diff
@@ -31,21 +31,21 @@
         self.start_time = time.time()
 
     def stop(self, info="Process time"):
         print(str(info) + " took : " + str((time.time() - self.start_time)) + " [sec]")
 
     def get_fn(self):
         fn_gt_csv = str(SAMPLE_DATA_DIR + '/ID1-pose-gt.csv')
-        fn_est_csv = str(SAMPLE_DATA_DIR + '/ID1-pose-est-cov.csv')
+        fn_est_csv = str(SAMPLE_DATA_DIR + '/ID1-pose-est-posorient-cov.csv')
         return fn_gt_csv, fn_est_csv
 
     def test_init(self):
         self.start()
         fn_gt_csv = str(SAMPLE_DATA_DIR + '/ID1-pose-gt.csv')
-        fn_est_csv = str(SAMPLE_DATA_DIR + '/ID1-pose-est-cov.csv')
+        fn_est_csv = str(SAMPLE_DATA_DIR + '/ID1-pose-est-posorient-cov.csv')
         eval = TrajectoryEvaluation(fn_gt_csv, fn_est_csv, result_dir=str(SAMPLE_DATA_DIR + '/results/eval'), prefix='eval-ID1-',
                                     alignment_type=TrajectoryAlignmentTypes.none)
 
         self.stop()
 
 
 if __name__ == "__main__":
```

### Comparing `cnspy_trajectory_evaluation-0.1.1/test/test_TrajectoryNEES.py` & `cnspy_trajectory_evaluation-0.2.0/test/test_DifferentialTrajectoryError.py`

 * *Files 24% similar despite different names*

```diff
@@ -15,52 +15,60 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 #
 ########################################################################################################################
 import os
 import unittest
-import time
-from cnspy_trajectory_evaluation.AbsoluteTrajectoryError import AbsoluteTrajectoryError
-from cnspy_trajectory.TrajectoryPlotter import TrajectoryPlotter, TrajectoryPlotConfig
-from cnspy_trajectory.TrajectoryPlotTypes import TrajectoryPlotTypes
-from cnspy_trajectory_evaluation.TrajectoryNEES import *
+from cnspy_spatial_csv_formats.CSVSpatialFormat import CSVSpatialFormat, EstimationErrorType, ErrorRepresentationType, CSVSpatialFormatType
+from cnspy_trajectory.TrajectoryEstimated import TrajectoryEstimated
+from cnspy_trajectory_evaluation.AbsoluteTrajectoryError import *
+from cnspy_trajectory.TrajectoryPlotter import TrajectoryPlotter, TrajectoryPlotConfig, TrajectoryPlotTypes
+from cnspy_trajectory.TrajectoryErrorType import TrajectoryErrorType
+from cnspy_trajectory.SpatialConverter import SpatialConverter
+from spatialmath import SO3
+
+from cnspy_trajectory_evaluation.AssociatedTrajectories import AssociatedTrajectories
+from cnspy_trajectory_evaluation.DifferentialTrajectoryError import DifferentialTrajectoryError
 
 SAMPLE_DATA_DIR = os.path.join(os.path.dirname(os.path.abspath(__file__)), 'sample_data')
 
-class TrajectoryNEES_Test(unittest.TestCase):
-    start_time = None
+class DifferentialTrajectoryError_Test(unittest.TestCase):
 
-    def start(self):
-        self.start_time = time.time()
+    def get_trajectories(self):
+        fn_gt  = str(SAMPLE_DATA_DIR + '/ID1-pose-est-posorient-cov.csv')
+        fn_est = str(SAMPLE_DATA_DIR + '/ID1-pose-gt.csv')
 
-    def stop(self, info="Process time"):
-        print(str(info) + " took : " + str((time.time() - self.start_time)) + " [sec]")
+        assoc = AssociatedTrajectories(fn_gt=fn_gt, fn_est=fn_est)
+        assoc.plot_timestamps(cfg=TrajectoryPlotConfig(show=False))
+        return assoc.get_trajectories()  # est, gt
 
-    def get_trajectories(self):
-        traj_est = TrajectoryEstimated()
-        self.assertTrue(traj_est.load_from_CSV(str(SAMPLE_DATA_DIR + '/ID1-pose-est-cov.csv')))
-        traj_gt = Trajectory()
-        self.assertTrue(traj_gt.load_from_CSV(str(SAMPLE_DATA_DIR + '/ID1-pose-gt.csv')))
-        return traj_est, traj_gt
 
-    def test_nees(self):
-        self.start()
+    def test_DTE(self):
         traj_est, traj_gt = self.get_trajectories()
-        ATE = AbsoluteTrajectoryError(traj_est, traj_gt)
-        print('ARMSE p={:.2f}, q={:.2f}'.format(ATE.ARMSE_p, ATE.ARMSE_q_deg))
-        self.stop('Loading + ATE')
-        self.start()
-        NEES = TrajectoryNEES(ATE.traj_est, ATE.traj_err)
-        self.stop('NEES computation')
-        print('ANEES_p: ' + str(NEES.ANEES_p))
-        print('ANEES_q: ' + str(NEES.ANEES_q))
-
-        NEES.plot(cfg=TrajectoryPlotConfig(show=True, save_fn=str(SAMPLE_DATA_DIR + '/../../doc/pose-nees.png')))
-        NEES.save_to_CSV(str(SAMPLE_DATA_DIR + '/results/nees.csv'))
-        ATE.plot_pose_err(
-            cfg=TrajectoryPlotConfig(show=True, radians=False, plot_type=TrajectoryPlotTypes.plot_2D_over_t, save_fn=str(SAMPLE_DATA_DIR + '/../../doc/pose-err-plot.png')),
-            angles=True)
+        traj_est.subsample(step=10)
+        traj_gt.subsample(step=10)
+
+        R_GN = SO3.Rz(135, unit='deg')
+        R_GN = np.array(R_GN.R)
+        p_GN_in_G = np.array([1, 2, 4])
+        traj_gt.transform(scale=1.0, p_GN_in_G=p_GN_in_G, R_GN=R_GN)
+
+        TrajectoryPlotter.multi_plot_3D(traj_list=[traj_gt, traj_est],
+                                        cfg=TrajectoryPlotConfig(show=False),
+                                        name_list=['gt_matched', 'est_matched'])
+        DTE = DifferentialTrajectoryError(traj_est=traj_est, traj_gt=traj_gt)
+        DTE.plot_p_err(cfg=TrajectoryPlotConfig(show=False, plot_type=TrajectoryPlotTypes.plot_2D_over_t))
+        DTE.plot_rpy_err(cfg=TrajectoryPlotConfig(show=False, plot_type=TrajectoryPlotTypes.plot_2D_over_t))
+        DTE.plot_pose(cfg=TrajectoryPlotConfig(show=False, plot_type=TrajectoryPlotTypes.plot_2D_over_t),
+                      plot_angle_distance=True, plot_eucl_distance=True)
+        DTE.plot_pose(
+            cfg=TrajectoryPlotConfig(show=True, radians=False, plot_type=TrajectoryPlotTypes.plot_2D_over_t),
+            plot_angle_distance=True, plot_eucl_distance=True)
+
+        ARMSE_p, ARMSE_q = DTE.get_ARMSE()
+        print('test_DTE done:ARMSE p={:.2f}, q={:.2f}'.format(ARMSE_p, ARMSE_q))
+
 
 
 if __name__ == "__main__":
     unittest.main()
```


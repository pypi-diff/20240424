# Comparing `tmp/cnspy_trajectory-0.1.1.tar.gz` & `tmp/cnspy_trajectory-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/jungr/workspace/CNS/VIO_Evaluation_Framework/py3_pkgs/cnspy_eco_system_test/pkgs/f_trajectory/dist/tmp5b4d4gtd/cnspy_traj", last modified: Sat Mar 20 14:24:10 2021, max compression
+gzip compressed data, was "cnspy_trajectory-0.2.0.tar", last modified: Wed Apr 24 12:17:41 2024, max compression
```

## Comparing `cnspy_trajectory-0.1.1.tar` & `cnspy_trajectory-0.2.0.tar`

### file list

```diff
@@ -1,27 +1,36 @@
-drwxrwxr-x   0 jungr     (1000) jungr     (1000)        0 2021-03-20 14:24:10.963424 cnspy_trajectory-0.1.1/
--rw-rw-r--   0 jungr     (1000) jungr     (1000)     3247 2021-03-20 14:24:10.963424 cnspy_trajectory-0.1.1/PKG-INFO
--rw-rw-r--   0 jungr     (1000) jungr     (1000)     2107 2021-03-20 14:21:27.000000 cnspy_trajectory-0.1.1/README.md
-drwxrwxr-x   0 jungr     (1000) jungr     (1000)        0 2021-03-20 14:24:10.959424 cnspy_trajectory-0.1.1/cnspy_trajectory/
--rwxrwxr-x   0 jungr     (1000) jungr     (1000)     1575 2021-03-20 12:20:48.000000 cnspy_trajectory-0.1.1/cnspy_trajectory/PlotLineStyle.py
--rw-rw-r--   0 jungr     (1000) jungr     (1000)     4441 2021-03-20 12:20:48.000000 cnspy_trajectory-0.1.1/cnspy_trajectory/SpatialConverter.py
--rwxrwxr-x   0 jungr     (1000) jungr     (1000)     5157 2021-03-20 12:20:48.000000 cnspy_trajectory-0.1.1/cnspy_trajectory/Trajectory.py
--rwxrwxr-x   0 jungr     (1000) jungr     (1000)     2886 2021-03-20 12:20:48.000000 cnspy_trajectory-0.1.1/cnspy_trajectory/TrajectoryEstimated.py
--rwxrwxr-x   0 jungr     (1000) jungr     (1000)     2909 2021-03-20 12:20:48.000000 cnspy_trajectory-0.1.1/cnspy_trajectory/TrajectoryPlotConfig.py
--rwxrwxr-x   0 jungr     (1000) jungr     (1000)     1171 2021-03-20 12:20:48.000000 cnspy_trajectory-0.1.1/cnspy_trajectory/TrajectoryPlotTypes.py
--rwxrwxr-x   0 jungr     (1000) jungr     (1000)    13973 2021-03-20 12:20:48.000000 cnspy_trajectory-0.1.1/cnspy_trajectory/TrajectoryPlotter.py
--rwxrwxr-x   0 jungr     (1000) jungr     (1000)        0 2021-03-20 12:20:48.000000 cnspy_trajectory-0.1.1/cnspy_trajectory/__init__.py
--rwxrwxr-x   0 jungr     (1000) jungr     (1000)     2017 2021-03-20 12:20:48.000000 cnspy_trajectory-0.1.1/cnspy_trajectory/pyplot_utils.py
-drwxrwxr-x   0 jungr     (1000) jungr     (1000)        0 2021-03-20 14:24:10.963424 cnspy_trajectory-0.1.1/cnspy_trajectory.egg-info/
--rw-rw-r--   0 jungr     (1000) jungr     (1000)     3247 2021-03-20 14:24:10.000000 cnspy_trajectory-0.1.1/cnspy_trajectory.egg-info/PKG-INFO
--rw-rw-r--   0 jungr     (1000) jungr     (1000)      675 2021-03-20 14:24:10.000000 cnspy_trajectory-0.1.1/cnspy_trajectory.egg-info/SOURCES.txt
--rw-rw-r--   0 jungr     (1000) jungr     (1000)        1 2021-03-20 14:24:10.000000 cnspy_trajectory-0.1.1/cnspy_trajectory.egg-info/dependency_links.txt
--rw-rw-r--   0 jungr     (1000) jungr     (1000)       82 2021-03-20 14:24:10.000000 cnspy_trajectory-0.1.1/cnspy_trajectory.egg-info/requires.txt
--rw-rw-r--   0 jungr     (1000) jungr     (1000)       22 2021-03-20 14:24:10.000000 cnspy_trajectory-0.1.1/cnspy_trajectory.egg-info/top_level.txt
--rw-rw-r--   0 jungr     (1000) jungr     (1000)       38 2021-03-20 14:24:10.963424 cnspy_trajectory-0.1.1/setup.cfg
--rw-rw-r--   0 jungr     (1000) jungr     (1000)     1329 2021-03-20 14:21:27.000000 cnspy_trajectory-0.1.1/setup.py
-drwxrwxr-x   0 jungr     (1000) jungr     (1000)        0 2021-03-20 14:24:10.963424 cnspy_trajectory-0.1.1/test/
--rwxrwxr-x   0 jungr     (1000) jungr     (1000)        0 2021-03-20 12:20:48.000000 cnspy_trajectory-0.1.1/test/__init__.py
--rw-rw-r--   0 jungr     (1000) jungr     (1000)     2859 2021-03-20 12:20:48.000000 cnspy_trajectory-0.1.1/test/test_SpatialConverter.py
--rw-rw-r--   0 jungr     (1000) jungr     (1000)     3832 2021-03-20 12:20:48.000000 cnspy_trajectory-0.1.1/test/test_Trajectory.py
--rw-rw-r--   0 jungr     (1000) jungr     (1000)     2023 2021-03-20 12:20:48.000000 cnspy_trajectory-0.1.1/test/test_TrajectoryEstimated.py
--rw-rw-r--   0 jungr     (1000) jungr     (1000)     3930 2021-03-20 12:20:48.000000 cnspy_trajectory-0.1.1/test/test_TrajectoryPlotter.py
+drwxrwxr-x   0 jungr     (1000) jungr     (1000)        0 2024-04-24 12:17:41.325316 cnspy_trajectory-0.2.0/
+-rw-rw-r--   0 jungr     (1000) jungr     (1000)    35149 2022-05-30 14:10:29.000000 cnspy_trajectory-0.2.0/LICENCE
+-rw-r--r--   0 jungr     (1000) jungr     (1000)     3604 2024-04-24 12:17:41.325316 cnspy_trajectory-0.2.0/PKG-INFO
+-rw-rw-r--   0 jungr     (1000) jungr     (1000)     2805 2024-04-24 11:56:52.000000 cnspy_trajectory-0.2.0/README.md
+drwxrwxr-x   0 jungr     (1000) jungr     (1000)        0 2024-04-24 12:17:41.325316 cnspy_trajectory-0.2.0/cnspy_trajectory/
+-rwxrwxr-x   0 jungr     (1000) jungr     (1000)     1575 2022-05-30 14:10:29.000000 cnspy_trajectory-0.2.0/cnspy_trajectory/PlotLineStyle.py
+-rwxrwxr-x   0 jungr     (1000) jungr     (1000)     5951 2024-04-24 11:56:52.000000 cnspy_trajectory-0.2.0/cnspy_trajectory/PlotTrajectory.py
+-rw-rw-r--   0 jungr     (1000) jungr     (1000)     8595 2024-04-24 11:56:52.000000 cnspy_trajectory-0.2.0/cnspy_trajectory/SpatialConverter.py
+-rwxrwxr-x   0 jungr     (1000) jungr     (1000)    19584 2024-04-24 11:56:52.000000 cnspy_trajectory-0.2.0/cnspy_trajectory/Trajectory.py
+-rw-rw-r--   0 jungr     (1000) jungr     (1000)     4553 2024-04-24 11:56:52.000000 cnspy_trajectory-0.2.0/cnspy_trajectory/TrajectoryBase.py
+-rw-rw-r--   0 jungr     (1000) jungr     (1000)     9329 2024-04-24 11:56:52.000000 cnspy_trajectory-0.2.0/cnspy_trajectory/TrajectoryError.py
+-rw-rw-r--   0 jungr     (1000) jungr     (1000)     3645 2024-04-24 11:56:52.000000 cnspy_trajectory-0.2.0/cnspy_trajectory/TrajectoryErrorType.py
+-rwxrwxr-x   0 jungr     (1000) jungr     (1000)    24424 2024-04-24 11:56:52.000000 cnspy_trajectory-0.2.0/cnspy_trajectory/TrajectoryEstimated.py
+-rw-rw-r--   0 jungr     (1000) jungr     (1000)     5420 2024-04-24 11:56:52.000000 cnspy_trajectory-0.2.0/cnspy_trajectory/TrajectoryEstimationError.py
+-rwxrwxr-x   0 jungr     (1000) jungr     (1000)     3116 2024-04-24 11:56:52.000000 cnspy_trajectory-0.2.0/cnspy_trajectory/TrajectoryPlotConfig.py
+-rwxrwxr-x   0 jungr     (1000) jungr     (1000)     1171 2022-05-30 14:10:29.000000 cnspy_trajectory-0.2.0/cnspy_trajectory/TrajectoryPlotTypes.py
+-rw-rw-r--   0 jungr     (1000) jungr     (1000)     7100 2024-04-24 11:56:52.000000 cnspy_trajectory-0.2.0/cnspy_trajectory/TrajectoryPlotUtils.py
+-rwxrwxr-x   0 jungr     (1000) jungr     (1000)     4640 2024-04-24 11:56:52.000000 cnspy_trajectory-0.2.0/cnspy_trajectory/TrajectoryPlotter.py
+-rwxrwxr-x   0 jungr     (1000) jungr     (1000)        0 2022-05-30 14:10:29.000000 cnspy_trajectory-0.2.0/cnspy_trajectory/__init__.py
+-rwxrwxr-x   0 jungr     (1000) jungr     (1000)     2017 2022-07-12 09:08:34.000000 cnspy_trajectory-0.2.0/cnspy_trajectory/pyplot_utils.py
+drwxrwxr-x   0 jungr     (1000) jungr     (1000)        0 2024-04-24 12:17:41.325316 cnspy_trajectory-0.2.0/cnspy_trajectory.egg-info/
+-rw-r--r--   0 jungr     (1000) jungr     (1000)     3604 2024-04-24 12:17:41.000000 cnspy_trajectory-0.2.0/cnspy_trajectory.egg-info/PKG-INFO
+-rw-rw-r--   0 jungr     (1000) jungr     (1000)      977 2024-04-24 12:17:41.000000 cnspy_trajectory-0.2.0/cnspy_trajectory.egg-info/SOURCES.txt
+-rw-rw-r--   0 jungr     (1000) jungr     (1000)        1 2024-04-24 12:17:41.000000 cnspy_trajectory-0.2.0/cnspy_trajectory.egg-info/dependency_links.txt
+-rw-rw-r--   0 jungr     (1000) jungr     (1000)       82 2024-04-24 12:17:41.000000 cnspy_trajectory-0.2.0/cnspy_trajectory.egg-info/requires.txt
+-rw-rw-r--   0 jungr     (1000) jungr     (1000)       22 2024-04-24 12:17:41.000000 cnspy_trajectory-0.2.0/cnspy_trajectory.egg-info/top_level.txt
+-rw-rw-r--   0 jungr     (1000) jungr     (1000)       38 2024-04-24 12:17:41.325316 cnspy_trajectory-0.2.0/setup.cfg
+-rw-rw-r--   0 jungr     (1000) jungr     (1000)     1329 2022-05-30 14:10:29.000000 cnspy_trajectory-0.2.0/setup.py
+drwxrwxr-x   0 jungr     (1000) jungr     (1000)        0 2024-04-24 12:17:41.325316 cnspy_trajectory-0.2.0/test/
+-rwxrwxr-x   0 jungr     (1000) jungr     (1000)        0 2022-05-30 14:10:29.000000 cnspy_trajectory-0.2.0/test/__init__.py
+-rw-rw-r--   0 jungr     (1000) jungr     (1000)     5296 2024-04-24 11:56:52.000000 cnspy_trajectory-0.2.0/test/test_SpatialConverter.py
+-rw-rw-r--   0 jungr     (1000) jungr     (1000)     8383 2024-04-24 11:56:52.000000 cnspy_trajectory-0.2.0/test/test_Trajectory.py
+-rw-rw-r--   0 jungr     (1000) jungr     (1000)     2630 2024-04-24 11:56:52.000000 cnspy_trajectory-0.2.0/test/test_TrajectoryError.py
+-rw-rw-r--   0 jungr     (1000) jungr     (1000)     1572 2024-04-24 11:56:52.000000 cnspy_trajectory-0.2.0/test/test_TrajectoryErrorType.py
+-rw-rw-r--   0 jungr     (1000) jungr     (1000)     4130 2024-04-24 11:56:52.000000 cnspy_trajectory-0.2.0/test/test_TrajectoryEstimated.py
+-rw-rw-r--   0 jungr     (1000) jungr     (1000)     3826 2024-04-24 11:56:52.000000 cnspy_trajectory-0.2.0/test/test_TrajectoryPlotter.py
```

### Comparing `cnspy_trajectory-0.1.1/cnspy_trajectory/PlotLineStyle.py` & `cnspy_trajectory-0.2.0/cnspy_trajectory/PlotLineStyle.py`

 * *Files identical despite different names*

### Comparing `cnspy_trajectory-0.1.1/cnspy_trajectory/TrajectoryEstimated.py` & `cnspy_trajectory-0.2.0/test/test_TrajectoryError.py`

 * *Files 24% similar despite different names*

```diff
@@ -12,57 +12,54 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 #
+# Requirements:
+# enum
 ########################################################################################################################
 import os
+
+from cnspy_spatial_csv_formats.ErrorRepresentationType import ErrorRepresentationType
+from cnspy_spatial_csv_formats.EstimationErrorType import EstimationErrorType
 from cnspy_trajectory.Trajectory import Trajectory
-from cnspy_csv2dataframe.PoseWithCov2DataFrame import PoseWithCov2DataFrame
-from cnspy_csv2dataframe.CSV2DataFrame import CSV2DataFrame
-from cnspy_spatial_csv_formats.CSVFormatPose import CSVFormatPose
-
-
-class TrajectoryEstimated(Trajectory):
-    # position uncertainty: 3x3 covariance matrix.
-    # The with upper triangular elements are vectorized: 'pxx', 'pxy', 'pxz', 'pyy', 'pyz', 'pzz'
-    Sigma_p_vec = None
-
-    # small angle `theta` uncertainty: R = ( eye(3) + slew(theta)), a 3x3 covariance matrix.
-    # The with upper triangular elements are vectorized: 'qrr', 'qrp', 'qry', 'qpp', 'qpy', 'qyy'
-    Sigma_q_vec = None
-
-    def __init__(self, t_vec=None, p_vec=None, q_vec=None, Sigma_p_vec=None, Sigma_q_vec=None, df=None):
-        Trajectory.__init__(self, t_vec=t_vec, p_vec=p_vec, q_vec=q_vec)
-        self.Sigma_p_vec = Sigma_p_vec
-        self.Sigma_q_vec = Sigma_q_vec
-
-        if df is not None:
-            self.load_from_DataFrame(df)
-
-    def load_from_CSV(self, filename):
-        if not os.path.isfile(filename):
-            print("Trajectory: could not find file %s" % os.path.abspath(filename))
-            return False
-
-        loader = CSV2DataFrame(filename=filename)
-        self.load_from_DataFrame(loader.data_frame)
-        return loader.data_loaded
-
-    def load_from_DataFrame(self, df):
-        self.t_vec, self.p_vec, self.q_vec, self.Sigma_p_vec, self.Sigma_q_vec = PoseWithCov2DataFrame.DataFrame_to_TPQCov(
-            data_frame=df)
-
-    def to_DataFrame(self):
-        return PoseWithCov2DataFrame.TPQCov_to_DataFrame(self.t_vec, self.p_vec, self.q_vec, self.Sigma_p_vec,
-                                                         self.Sigma_q_vec)
-
-    def save_to_CSV(self, filename):
-        if self.is_empty():
-            return False
-        df = self.to_DataFrame()
-        CSV2DataFrame.save_CSV(df, filename=filename, fmt=CSVFormatPose.PoseWithCov)
-        return True
+from cnspy_trajectory.TrajectoryError import TrajectoryError
+from cnspy_trajectory.TrajectoryErrorType import TrajectoryErrorType
+from cnspy_trajectory.TrajectoryEstimated import TrajectoryEstimated
+import unittest
+import time
+
+from cnspy_trajectory.TrajectoryPlotConfig import TrajectoryPlotConfig
+from cnspy_trajectory.TrajectoryPlotTypes import TrajectoryPlotTypes
+
+SAMPLE_DATA_DIR = os.path.join(os.path.dirname(os.path.abspath(__file__)), 'sample_data')
+
+class TrajectoryError_Test(unittest.TestCase):
+    start_time = None
+
+    def start(self):
+        self.start_time = time.time()
+
+    def stop(self):
+        print("Process time: " + str((time.time() - self.start_time)))
+
+    def load_(self):
+        print('loading...')
+        fn = str(SAMPLE_DATA_DIR + '/ID1-pose-err.csv')
+        obj = TrajectoryError(fn=fn)
+        obj.traj_err_type = TrajectoryErrorType(err_type=EstimationErrorType.type1)
+        return obj
+
+
+    def test_plot(self):
+        traj_err = self.load_()
+        traj_err.save_to_CSV(str(SAMPLE_DATA_DIR + '/results/ID1-pose-err.COPY.csv'))
+        cfg = TrajectoryPlotConfig(show=True, close_figure=False,
+                                   save_fn=str(SAMPLE_DATA_DIR + '/../../doc/traj_err_pos.png'))
+        traj_err.plot_p_err(cfg=cfg)
+        cfg = TrajectoryPlotConfig(show=True, close_figure=False,
+                                   save_fn=str(SAMPLE_DATA_DIR + '/../../doc/traj_err_rpy.png'))
 
+        traj_err.plot_rpy_err(cfg=cfg)
```

### Comparing `cnspy_trajectory-0.1.1/cnspy_trajectory/TrajectoryPlotConfig.py` & `cnspy_trajectory-0.2.0/cnspy_trajectory/TrajectoryPlotConfig.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,31 +33,33 @@
     title = ""
     scale = 1.0
     save_fn = ""
     result_dir = "."
     show = True
     close_figure = False
     radians = True
+    relative_time = True
     view_angle = (45, 45)  # viewing angle of 3D plots tuple (azimuth, elevation)
 
     def __init__(self, white_list=[], num_points=0,
                  plot_type=TrajectoryPlotTypes.plot_3D, dpi=200, title="",
-                 scale=1.0, save_fn="", result_dir=".", show=True, close_figure=False, radians=True,
+                 scale=1.0, save_fn="", result_dir=".", show=True, close_figure=False, radians=True, relative_time=True,
                  view_angle=(45, 45)):
         self.white_list = white_list
         self.num_points = num_points
         self.plot_type = plot_type
         self.dpi = dpi
         self.title = title
         self.scale = scale
         self.save_fn = save_fn
         self.result_dir = result_dir
         self.show = show
         self.close_figure = close_figure
         self.radians = radians
+        self.relative_time = relative_time
         self.view_angle = view_angle
 
     @staticmethod
     def set_view_angle(cfg, ax):
         """
         set the view angle of a 3D plot
 
@@ -68,17 +70,21 @@
         assert (isinstance(cfg, TrajectoryPlotConfig))
         ax.view_init(azim=cfg.view_angle[0], elev=cfg.view_angle[1])
 
     @staticmethod
     def show_save_figure(cfg, fig):
         assert (isinstance(cfg, TrajectoryPlotConfig))
         assert(isinstance(fig, plt.Figure))
+        plt.pause(0.01)
         plt.draw()
-        plt.pause(0.001)
+        plt.pause(0.01)
         if cfg.save_fn:
+            if not os.path.exists(cfg.result_dir):
+                os.makedirs(cfg.result_dir)
+
             filename = os.path.join(cfg.result_dir, cfg.save_fn)
             print("save to file: " + filename)
             plt.savefig(filename, dpi=int(cfg.dpi))
         if cfg.show:
             plt.show()
         if cfg.close_figure:
             plt.close(fig)
```

### Comparing `cnspy_trajectory-0.1.1/cnspy_trajectory/TrajectoryPlotTypes.py` & `cnspy_trajectory-0.2.0/cnspy_trajectory/TrajectoryPlotTypes.py`

 * *Files identical despite different names*

### Comparing `cnspy_trajectory-0.1.1/cnspy_trajectory/pyplot_utils.py` & `cnspy_trajectory-0.2.0/cnspy_trajectory/pyplot_utils.py`

 * *Files identical despite different names*

### Comparing `cnspy_trajectory-0.1.1/cnspy_trajectory.egg-info/SOURCES.txt` & `cnspy_trajectory-0.2.0/cnspy_trajectory.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,30 @@
+LICENCE
 README.md
 setup.py
 cnspy_trajectory/PlotLineStyle.py
+cnspy_trajectory/PlotTrajectory.py
 cnspy_trajectory/SpatialConverter.py
 cnspy_trajectory/Trajectory.py
+cnspy_trajectory/TrajectoryBase.py
+cnspy_trajectory/TrajectoryError.py
+cnspy_trajectory/TrajectoryErrorType.py
 cnspy_trajectory/TrajectoryEstimated.py
+cnspy_trajectory/TrajectoryEstimationError.py
 cnspy_trajectory/TrajectoryPlotConfig.py
 cnspy_trajectory/TrajectoryPlotTypes.py
+cnspy_trajectory/TrajectoryPlotUtils.py
 cnspy_trajectory/TrajectoryPlotter.py
 cnspy_trajectory/__init__.py
 cnspy_trajectory/pyplot_utils.py
 cnspy_trajectory.egg-info/PKG-INFO
 cnspy_trajectory.egg-info/SOURCES.txt
 cnspy_trajectory.egg-info/dependency_links.txt
 cnspy_trajectory.egg-info/requires.txt
 cnspy_trajectory.egg-info/top_level.txt
 test/__init__.py
 test/test_SpatialConverter.py
 test/test_Trajectory.py
+test/test_TrajectoryError.py
+test/test_TrajectoryErrorType.py
 test/test_TrajectoryEstimated.py
 test/test_TrajectoryPlotter.py
```

### Comparing `cnspy_trajectory-0.1.1/setup.py` & `cnspy_trajectory-0.2.0/setup.py`

 * *Files identical despite different names*


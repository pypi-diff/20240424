# Comparing `tmp/cnspy_rosbag2csv-0.1.2.tar.gz` & `tmp/cnspy_rosbag2csv-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/jungr/workspace/CNS/VIO_Evaluation_Framework/py3_pkgs/cnspy_eco_system_test/pkgs/e_rosbag2csv/dist/tmpcpmsoibd/cnspy_rosb", last modified: Mon Mar 29 13:56:08 2021, max compression
+gzip compressed data, was "cnspy_rosbag2csv-0.2.0.tar", last modified: Wed Apr 24 12:17:06 2024, max compression
```

## Comparing `cnspy_rosbag2csv-0.1.2.tar` & `cnspy_rosbag2csv-0.2.0.tar`

### file list

```diff
@@ -1,25 +1,28 @@
-drwxrwxr-x   0 jungr     (1000) jungr     (1000)        0 2021-03-29 13:56:08.976990 cnspy_rosbag2csv-0.1.2/
--rw-rw-r--   0 jungr     (1000) jungr     (1000)     7737 2021-03-29 13:56:08.976990 cnspy_rosbag2csv-0.1.2/PKG-INFO
--rw-rw-r--   0 jungr     (1000) jungr     (1000)     6125 2021-03-29 13:44:18.000000 cnspy_rosbag2csv-0.1.2/README.md
-drwxrwxr-x   0 jungr     (1000) jungr     (1000)        0 2021-03-29 13:56:08.976990 cnspy_rosbag2csv-0.1.2/cnspy_rosbag2csv/
--rwxrwxr-x   0 jungr     (1000) jungr     (1000)     6634 2021-03-20 12:20:48.000000 cnspy_rosbag2csv-0.1.2/cnspy_rosbag2csv/CSV2ROSbag.py
--rwxrwxr-x   0 jungr     (1000) jungr     (1000)     5585 2021-03-20 12:20:48.000000 cnspy_rosbag2csv-0.1.2/cnspy_rosbag2csv/CSVLine2ROSMsg.py
--rw-rw-r--   0 jungr     (1000) jungr     (1000)     2115 2021-03-20 12:20:48.000000 cnspy_rosbag2csv-0.1.2/cnspy_rosbag2csv/CSVParser.py
--rwxrwxr-x   0 jungr     (1000) jungr     (1000)     4369 2021-03-20 12:20:48.000000 cnspy_rosbag2csv-0.1.2/cnspy_rosbag2csv/ROSMessageTypes.py
--rwxrwxr-x   0 jungr     (1000) jungr     (1000)     9904 2021-03-20 12:20:48.000000 cnspy_rosbag2csv-0.1.2/cnspy_rosbag2csv/ROSMsg2CSVLine.py
--rwxrwxr-x   0 jungr     (1000) jungr     (1000)     9296 2021-03-20 12:20:48.000000 cnspy_rosbag2csv-0.1.2/cnspy_rosbag2csv/ROSbag2CSV.py
--rwxrwxr-x   0 jungr     (1000) jungr     (1000)        0 2021-03-20 12:20:48.000000 cnspy_rosbag2csv-0.1.2/cnspy_rosbag2csv/__init__.py
-drwxrwxr-x   0 jungr     (1000) jungr     (1000)        0 2021-03-29 13:56:08.976990 cnspy_rosbag2csv-0.1.2/cnspy_rosbag2csv.egg-info/
--rw-rw-r--   0 jungr     (1000) jungr     (1000)     7737 2021-03-29 13:56:08.000000 cnspy_rosbag2csv-0.1.2/cnspy_rosbag2csv.egg-info/PKG-INFO
--rw-rw-r--   0 jungr     (1000) jungr     (1000)      565 2021-03-29 13:56:08.000000 cnspy_rosbag2csv-0.1.2/cnspy_rosbag2csv.egg-info/SOURCES.txt
--rw-rw-r--   0 jungr     (1000) jungr     (1000)        1 2021-03-29 13:56:08.000000 cnspy_rosbag2csv-0.1.2/cnspy_rosbag2csv.egg-info/dependency_links.txt
--rw-rw-r--   0 jungr     (1000) jungr     (1000)      135 2021-03-29 13:56:08.000000 cnspy_rosbag2csv-0.1.2/cnspy_rosbag2csv.egg-info/requires.txt
--rw-rw-r--   0 jungr     (1000) jungr     (1000)       22 2021-03-29 13:56:08.000000 cnspy_rosbag2csv-0.1.2/cnspy_rosbag2csv.egg-info/top_level.txt
--rw-rw-r--   0 jungr     (1000) jungr     (1000)       38 2021-03-29 13:56:08.976990 cnspy_rosbag2csv-0.1.2/setup.cfg
--rw-rw-r--   0 jungr     (1000) jungr     (1000)     1411 2021-03-29 13:44:18.000000 cnspy_rosbag2csv-0.1.2/setup.py
-drwxrwxr-x   0 jungr     (1000) jungr     (1000)        0 2021-03-29 13:56:08.976990 cnspy_rosbag2csv-0.1.2/test/
--rwxrwxr-x   0 jungr     (1000) jungr     (1000)        0 2021-03-20 12:20:48.000000 cnspy_rosbag2csv-0.1.2/test/__init__.py
--rw-rw-r--   0 jungr     (1000) jungr     (1000)     1589 2021-03-20 12:20:48.000000 cnspy_rosbag2csv-0.1.2/test/test_CSV2ROSbag.py
--rw-rw-r--   0 jungr     (1000) jungr     (1000)     3034 2021-03-20 12:20:48.000000 cnspy_rosbag2csv-0.1.2/test/test_CSVLine2ROSMsg.py
--rw-rw-r--   0 jungr     (1000) jungr     (1000)     7469 2021-03-20 12:20:48.000000 cnspy_rosbag2csv-0.1.2/test/test_ROSMsg2CSVLine.py
--rw-rw-r--   0 jungr     (1000) jungr     (1000)     1614 2021-03-20 12:20:48.000000 cnspy_rosbag2csv-0.1.2/test/test_ROSbag2CSV.py
+drwxrwxr-x   0 jungr     (1000) jungr     (1000)        0 2024-04-24 12:17:06.585258 cnspy_rosbag2csv-0.2.0/
+-rw-rw-r--   0 jungr     (1000) jungr     (1000)    35149 2022-05-30 14:10:28.000000 cnspy_rosbag2csv-0.2.0/LICENCE
+-rw-r--r--   0 jungr     (1000) jungr     (1000)     9266 2024-04-24 12:17:06.585258 cnspy_rosbag2csv-0.2.0/PKG-INFO
+-rw-rw-r--   0 jungr     (1000) jungr     (1000)     8313 2024-04-24 11:47:54.000000 cnspy_rosbag2csv-0.2.0/README.md
+drwxrwxr-x   0 jungr     (1000) jungr     (1000)        0 2024-04-24 12:17:06.585258 cnspy_rosbag2csv-0.2.0/cnspy_rosbag2csv/
+-rwxrwxr-x   0 jungr     (1000) jungr     (1000)     6610 2024-04-24 11:47:54.000000 cnspy_rosbag2csv-0.2.0/cnspy_rosbag2csv/CSV2ROSbag.py
+-rwxrwxr-x   0 jungr     (1000) jungr     (1000)     7471 2024-04-24 11:47:54.000000 cnspy_rosbag2csv-0.2.0/cnspy_rosbag2csv/CSVLine2ROSMsg.py
+-rw-rw-r--   0 jungr     (1000) jungr     (1000)     2180 2024-04-24 11:47:54.000000 cnspy_rosbag2csv-0.2.0/cnspy_rosbag2csv/CSVParser.py
+-rwxrwxr-x   0 jungr     (1000) jungr     (1000)     4369 2024-04-24 11:29:19.000000 cnspy_rosbag2csv-0.2.0/cnspy_rosbag2csv/ROSMessageTypes.py
+-rwxrwxr-x   0 jungr     (1000) jungr     (1000)    14124 2024-04-24 11:47:54.000000 cnspy_rosbag2csv-0.2.0/cnspy_rosbag2csv/ROSMsg2CSVLine.py
+-rwxrwxr-x   0 jungr     (1000) jungr     (1000)    10249 2024-04-24 11:47:54.000000 cnspy_rosbag2csv-0.2.0/cnspy_rosbag2csv/ROSbag2CSV.py
+-rw-rw-r--   0 jungr     (1000) jungr     (1000)     7623 2024-04-24 11:47:54.000000 cnspy_rosbag2csv-0.2.0/cnspy_rosbag2csv/ROSbagMerge.py
+-rw-rw-r--   0 jungr     (1000) jungr     (1000)     4465 2024-04-24 11:47:54.000000 cnspy_rosbag2csv-0.2.0/cnspy_rosbag2csv/ROSbag_ReTimestamp.py
+-rwxrwxr-x   0 jungr     (1000) jungr     (1000)        0 2022-05-30 14:10:28.000000 cnspy_rosbag2csv-0.2.0/cnspy_rosbag2csv/__init__.py
+drwxrwxr-x   0 jungr     (1000) jungr     (1000)        0 2024-04-24 12:17:06.585258 cnspy_rosbag2csv-0.2.0/cnspy_rosbag2csv.egg-info/
+-rw-r--r--   0 jungr     (1000) jungr     (1000)     9266 2024-04-24 12:17:06.000000 cnspy_rosbag2csv-0.2.0/cnspy_rosbag2csv.egg-info/PKG-INFO
+-rw-rw-r--   0 jungr     (1000) jungr     (1000)      644 2024-04-24 12:17:06.000000 cnspy_rosbag2csv-0.2.0/cnspy_rosbag2csv.egg-info/SOURCES.txt
+-rw-rw-r--   0 jungr     (1000) jungr     (1000)        1 2024-04-24 12:17:06.000000 cnspy_rosbag2csv-0.2.0/cnspy_rosbag2csv.egg-info/dependency_links.txt
+-rw-rw-r--   0 jungr     (1000) jungr     (1000)      123 2024-04-24 12:17:06.000000 cnspy_rosbag2csv-0.2.0/cnspy_rosbag2csv.egg-info/requires.txt
+-rw-rw-r--   0 jungr     (1000) jungr     (1000)       22 2024-04-24 12:17:06.000000 cnspy_rosbag2csv-0.2.0/cnspy_rosbag2csv.egg-info/top_level.txt
+-rw-rw-r--   0 jungr     (1000) jungr     (1000)       38 2024-04-24 12:17:06.585258 cnspy_rosbag2csv-0.2.0/setup.cfg
+-rw-rw-r--   0 jungr     (1000) jungr     (1000)     1399 2024-04-24 11:47:54.000000 cnspy_rosbag2csv-0.2.0/setup.py
+drwxrwxr-x   0 jungr     (1000) jungr     (1000)        0 2024-04-24 12:17:06.585258 cnspy_rosbag2csv-0.2.0/test/
+-rwxrwxr-x   0 jungr     (1000) jungr     (1000)        0 2022-05-30 14:10:28.000000 cnspy_rosbag2csv-0.2.0/test/__init__.py
+-rw-rw-r--   0 jungr     (1000) jungr     (1000)     2115 2024-04-24 11:47:54.000000 cnspy_rosbag2csv-0.2.0/test/test_CSV2ROSbag.py
+-rw-rw-r--   0 jungr     (1000) jungr     (1000)     3532 2024-04-24 11:47:54.000000 cnspy_rosbag2csv-0.2.0/test/test_CSVLine2ROSMsg.py
+-rw-rw-r--   0 jungr     (1000) jungr     (1000)     8427 2024-04-24 11:47:54.000000 cnspy_rosbag2csv-0.2.0/test/test_ROSMsg2CSVLine.py
+-rw-rw-r--   0 jungr     (1000) jungr     (1000)     2184 2024-04-24 11:47:54.000000 cnspy_rosbag2csv-0.2.0/test/test_ROSbag2CSV.py
```

### Comparing `cnspy_rosbag2csv-0.1.2/cnspy_rosbag2csv/CSV2ROSbag.py` & `cnspy_rosbag2csv-0.2.0/cnspy_rosbag2csv/CSV2ROSbag.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,16 +22,15 @@
 import os
 import argparse
 import yaml
 import csv
 from tqdm import tqdm
 
 from cnspy_rosbag2csv.CSVLine2ROSMsg import CSVLine2ROSMsg
-from cnspy_spatial_csv_formats.CSVFormatPose import CSVFormatPose
-import cnspy_script_utils.utils as script_utils
+from cnspy_spatial_csv_formats.CSVSpatialFormatType import CSVSpatialFormatType
 
 from cnspy_rosbag2csv.ROSMessageTypes import ROSMessageTypes
 from cnspy_rosbag2csv.CSVParser import CSVParser
 
 
 class CSV2ROSbag:
     def __init__(self):
@@ -118,15 +117,15 @@
             print(info_dict)
         bag.close()
         return True
 
 
 
 if __name__ == "__main__":
-    # --bagfile_name dummy.bag --topics /pose_est /pose_gt --filenames ./sample_data/ID1-pose-est-cov.csv ./sample_data/ID1-pose-gt.csv --fmt_list GEOMETRY_MSGS_POSEWITHCOVARIANCESTAMPED GEOMETRY_MSGS_POSESTAMPED --verbose
+    # --bagfile_name dummy.bag --topics /pose_est /pose_gt --filenames ./sample_data/ID1-pose-est-posorient-cov.csv ./sample_data/ID1-pose-gt.csv --fmt_list GEOMETRY_MSGS_POSEWITHCOVARIANCESTAMPED GEOMETRY_MSGS_POSESTAMPED --verbose
 
     parser = argparse.ArgumentParser(
         description='CSV2ROSbag: read CSV files and convert lines to specified ROS msg and store them into a rosbag')
     parser.add_argument('--bagfile_name', help='name of bag file (no path!)', default="not specified")
     parser.add_argument('--topics', nargs='*', help='topics to create', default=[])
     parser.add_argument('--filenames', nargs='*', help='csv filename of corresponding topic', default=[])
     parser.add_argument('--fmt_list', nargs='*', type=ROSMessageTypes, help='CSV format', choices=list(ROSMessageTypes),
@@ -139,10 +138,9 @@
     args = parser.parse_args()
 
     if CSV2ROSbag.extract(bagfile_name=args.bagfile_name, topic_list=args.topics,
                           fn_list=args.filenames, fmt_list=args.fmt_list, result_dir=args.result_dir,
                           verbose=args.verbose):
         print(" ")
         print("finished after [%s sec]\n" % str(time.time() - tp_start))
-        script_utils.exit_success()
     else:
-        script_utils.exit_failure()
+        print("failed! after [%s sec]\n" % str(time.time() - tp_start))
```

### Comparing `cnspy_rosbag2csv-0.1.2/cnspy_rosbag2csv/CSVParser.py` & `cnspy_rosbag2csv-0.2.0/cnspy_rosbag2csv/CSVParser.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,36 +17,37 @@
 #
 ########################################################################################################################
 import time
 import os
 import csv
 
 from cnspy_rosbag2csv.CSVLine2ROSMsg import CSVLine2ROSMsg
-from cnspy_spatial_csv_formats.CSVFormatPose import CSVFormatPose
+from cnspy_spatial_csv_formats.CSVSpatialFormat import CSVSpatialFormat
 from cnspy_rosbag2csv.ROSMessageTypes import ROSMessageTypes
 
 class CSVParser:
     curr_msg = None
     done = False
     t = None
-    fmt = None
+    fmt = None  # CSVSpatialFormat
     file = None
     line_number = 0
     msg_type = None
     fn = None
+    header = None
 
     def __init__(self, fn, msg_type=ROSMessageTypes.GEOMETRY_MSGS_POSEWITHCOVARIANCESTAMPED):
-        self.fmt = CSVFormatPose.identify_format(fn)
-        assert (self.fmt is not CSVFormatPose.none)
+        self.fmt = CSVSpatialFormat.identify_format(fn)
+        assert (self.fmt is not CSVSpatialFormat.type.none)
         self.fn = fn
         self.msg_type = msg_type
 
         self.file = open(fn, "r")
         line = self.file.readline()
-        header = str(line).rstrip("\n\r")
+        self.header = str(line).rstrip("\n\r")
         self.next_line()
 
     def __del__(self):
         # Closing files
         self.file.close()
 
     def next_line(self):
@@ -54,10 +55,10 @@
             return False
 
         line = self.file.readline()
         if not line:
             self.done = True
             return False
         line = str(line).rstrip("\n\r")
-        self.curr_msg, self.t = CSVLine2ROSMsg.to(self.fmt, line, self.line_number, self.msg_type)
+        self.curr_msg, self.t = CSVLine2ROSMsg.to(self.fmt.type, line, self.line_number, self.msg_type)
         self.line_number += 1
         return True
```

### Comparing `cnspy_rosbag2csv-0.1.2/cnspy_rosbag2csv/ROSMessageTypes.py` & `cnspy_rosbag2csv-0.2.0/cnspy_rosbag2csv/ROSMessageTypes.py`

 * *Files identical despite different names*

### Comparing `cnspy_rosbag2csv-0.1.2/cnspy_rosbag2csv/ROSMsg2CSVLine.py` & `cnspy_rosbag2csv-0.2.0/cnspy_rosbag2csv/ROSMsg2CSVLine.py`

 * *Files 15% similar despite different names*

```diff
@@ -14,33 +14,45 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 #
 ########################################################################################################################
 from cnspy_rosbag2csv.ROSMessageTypes import ROSMessageTypes
-from cnspy_spatial_csv_formats.CSVFormatPose import CSVFormatPose
-
+from cnspy_spatial_csv_formats.CSVSpatialFormatType import CSVSpatialFormatType
+from cnspy_spatial_csv_formats.EstimationErrorType import EstimationErrorType
+from cnspy_spatial_csv_formats.ErrorRepresentationType import ErrorRepresentationType
 
 class ROSMsg2CSVLine:
     def __init__(self):
         pass
 
     @staticmethod
-    def to(fmt, msg, t, msg_type):
-        if fmt == CSVFormatPose.TUM:
+    def to(fmt, msg, t, msg_type, est_err_type=EstimationErrorType.none, err_rep=ErrorRepresentationType.none):
+        if fmt == CSVSpatialFormatType.TUM or fmt == CSVSpatialFormatType.PoseStamped:
             return ROSMsg2CSVLine.to_TUM(msg, t, msg_type)
-        elif fmt == CSVFormatPose.PositionStamped:
+        elif fmt == CSVSpatialFormatType.PositionStamped:
             return ROSMsg2CSVLine.to_TUM(msg, t, msg_type)
-        elif fmt == CSVFormatPose.PoseCov:
+        elif fmt == CSVSpatialFormatType.PosOrientCov:
+            return ROSMsg2CSVLine.to_PosOrientCov(msg, t, msg_type)
+        elif fmt == CSVSpatialFormatType.PoseCov:
             return ROSMsg2CSVLine.to_PoseCov(msg, t, msg_type)
-        elif fmt == CSVFormatPose.PoseWithCov:
+        elif fmt == CSVSpatialFormatType.PosOrientWithCov:
+            return ROSMsg2CSVLine.to_PosOrientWithCov(msg, t, msg_type)
+        elif fmt == CSVSpatialFormatType.PoseWithCov:
             return ROSMsg2CSVLine.to_PoseWithCov(msg, t, msg_type)
+        elif fmt == CSVSpatialFormatType.PosOrientWithCovTyped:
+            return ROSMsg2CSVLine.to_PosOrientWithCovTyped(msg, t, msg_type, est_err_type, err_rep)
+        elif fmt == CSVSpatialFormatType.PoseWithCovTyped:
+            return ROSMsg2CSVLine.to_PoseWithCov(msg, t, msg_type, est_err_type, err_rep)
         else:
-            return None
+            print("ROSMsg2CSVLine.to(...): type {0} not supported".format(str(fmt)))
+            assert False
+
+        return None
 
     @staticmethod
     def to_TUM(msg_, t_, msg_type=ROSMessageTypes.NOT_SUPPORTED):
         """
 
         :rtype: list of floats
         """
@@ -157,15 +169,15 @@
             return ["%f" % msg_.header.stamp.to_sec(), str(msg_.transform.translation.x),
                     str(msg_.transform.translation.y),
                     str(msg_.transform.translation.z)]
         # else:
         return None
 
     @staticmethod
-    def to_PoseCov(msg_, t_, msg_type=ROSMessageTypes.NOT_SUPPORTED):
+    def to_PosOrientCov(msg_, t_, msg_type=ROSMessageTypes.NOT_SUPPORTED):
 
         if msg_type == ROSMessageTypes.GEOMETRY_MSGS_POSEWITHCOVARIANCESTAMPED or msg_type == ROSMessageTypes.GEOMETRY_MSGS_POSEWITHCOVARIANCE:
             if msg_type == ROSMessageTypes.GEOMETRY_MSGS_POSEWITHCOVARIANCESTAMPED:
                 P = msg_.pose.covariance
                 t = msg_.header.stamp.to_sec()
             else:
                 P = msg_.covariance
@@ -175,15 +187,38 @@
         elif msg_type != ROSMessageTypes.NOT_SUPPORTED:
             t = float(t_.secs) + float(t_.nsecs) * 1e-9
             return [str(t), '0', '0', '0', '0', '0', '0', '0', '0', '0', '0', '0', '0']
         # else:
         return None
 
     @staticmethod
-    def to_PoseWithCov(msg_, t_, msg_type=ROSMessageTypes.NOT_SUPPORTED):
+    def to_PoseCov(msg_, t_, msg_type=ROSMessageTypes.NOT_SUPPORTED):
+
+        if msg_type == ROSMessageTypes.GEOMETRY_MSGS_POSEWITHCOVARIANCESTAMPED or msg_type == ROSMessageTypes.GEOMETRY_MSGS_POSEWITHCOVARIANCE:
+            if msg_type == ROSMessageTypes.GEOMETRY_MSGS_POSEWITHCOVARIANCESTAMPED:
+                P = msg_.pose.covariance
+                t = msg_.header.stamp.to_sec()
+            else:
+                P = msg_.covariance
+                t = float(t_.secs) + float(t_.nsecs) * 1e-9
+
+            return ["%f" % (t), P[0], P[1], P[2], P[3], P[4], P[5],
+                    P[7], P[8], P[9], P[10], P[11],
+                    P[14], P[15], P[16], P[17],
+                    P[21], P[22], P[23],
+                    P[28], P[29],
+                    P[35]]
+        elif msg_type != ROSMessageTypes.NOT_SUPPORTED:
+            t = float(t_.secs) + float(t_.nsecs) * 1e-9
+            return [str(t), '0', '0', '0', '0', '0', '0', '0', '0', '0', '0', '0', '0', '0', '0', '0', '0', '0', '0', '0', '0', '0']
+        # else:
+        return None
+
+    @staticmethod
+    def to_PosOrientWithCov(msg_, t_, msg_type=ROSMessageTypes.NOT_SUPPORTED):
 
         if msg_type == ROSMessageTypes.GEOMETRY_MSGS_POSEWITHCOVARIANCESTAMPED or msg_type == ROSMessageTypes.GEOMETRY_MSGS_POSEWITHCOVARIANCE:
             if msg_type == ROSMessageTypes.GEOMETRY_MSGS_POSEWITHCOVARIANCESTAMPED:
                 P = msg_.pose.covariance
                 p = msg_.pose.pose.position
                 q = msg_.pose.pose.orientation
                 t = msg_.header.stamp.to_sec()
@@ -198,7 +233,53 @@
         elif msg_type != ROSMessageTypes.NOT_SUPPORTED:
             line = ROSMsg2CSVLine.to_TUM(msg_, t_, msg_type)
             line = line + ['0', '0', '0', '0', '0', '0', '0', '0', '0', '0', '0', '0']
             return line
         # else:
         return None
 
+
+    @staticmethod
+    def to_PoseWithCov(msg_, t_, msg_type=ROSMessageTypes.NOT_SUPPORTED):
+
+        if msg_type == ROSMessageTypes.GEOMETRY_MSGS_POSEWITHCOVARIANCESTAMPED or msg_type == ROSMessageTypes.GEOMETRY_MSGS_POSEWITHCOVARIANCE:
+            if msg_type == ROSMessageTypes.GEOMETRY_MSGS_POSEWITHCOVARIANCESTAMPED:
+                P = msg_.pose.covariance
+                p = msg_.pose.pose.position
+                q = msg_.pose.pose.orientation
+                t = msg_.header.stamp.to_sec()
+            else:
+                P = msg_.covariance
+                p = msg_.pose.position
+                q = msg_.pose.orientation
+                t = float(t_.secs) + float(t_.nsecs) * 1e-9
+
+            return ["%f" % (t), str(p.x), str(p.y), str(p.z), str(q.x), str(q.y), str(q.z), str(q.w),
+                    P[0], P[1], P[2], P[3], P[4], P[5],
+                    P[7], P[8], P[9], P[10], P[11],
+                    P[14], P[15], P[16], P[17],
+                    P[21], P[22], P[23],
+                    P[28], P[29],
+                    P[35]]
+        elif msg_type != ROSMessageTypes.NOT_SUPPORTED:
+            line = ROSMsg2CSVLine.to_TUM(msg_, t_, msg_type)
+            line = line + ['0', '0', '0', '0', '0', '0', '0', '0', '0', '0', '0', '0', '0', '0', '0', '0', '0', '0', '0', '0', '0']
+            return line
+        # else:
+        return None
+
+    @staticmethod
+    def to_PosOrientWithCovTyped(msg_, t_, msg_type=ROSMessageTypes.NOT_SUPPORTED,
+                                 est_err_type=EstimationErrorType.none, err_rep=ErrorRepresentationType.none):
+
+        line = ROSMsg2CSVLine.to_PosOrientWithCov(msg_, t_, msg_type)
+        if line is not None:
+            return line + [str(est_err_type), str(err_rep)]
+        return line
+
+    @staticmethod
+    def to_PoseWithCovTyped(msg_, t_, msg_type=ROSMessageTypes.NOT_SUPPORTED,
+                            est_err_type=EstimationErrorType.none, err_rep=ErrorRepresentationType.none):
+        line = ROSMsg2CSVLine.to_PoseWithCovCov(msg_, t_, msg_type)
+        if line is not None:
+            return line + [str(est_err_type), str(err_rep)]
+        return line
```

### Comparing `cnspy_rosbag2csv-0.1.2/cnspy_rosbag2csv/ROSbag2CSV.py` & `cnspy_rosbag2csv-0.2.0/cnspy_rosbag2csv/ROSbag2CSV.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,41 +21,44 @@
 import time
 import os
 import argparse
 import yaml
 import csv
 from tqdm import tqdm
 
-from cnspy_spatial_csv_formats.CSVFormatPose import CSVFormatPose
+from cnspy_spatial_csv_formats.CSVSpatialFormatType import CSVSpatialFormatType
+from cnspy_spatial_csv_formats.EstimationErrorType import EstimationErrorType
+from cnspy_spatial_csv_formats.ErrorRepresentationType import ErrorRepresentationType
 from cnspy_rosbag2csv.ROSMsg2CSVLine import ROSMsg2CSVLine
 from cnspy_rosbag2csv.ROSMessageTypes import ROSMessageTypes
 
-import cnspy_script_utils.utils as script_utils
-
 
 class ROSbag2CSV:
     def __init__(self):
         pass
 
     @staticmethod
-    def extract(bagfile_name, topic_list, result_dir="", fn_list=[], verbose=False, fmt=CSVFormatPose.TUM):
+    def extract(bagfile_name, topic_list, result_dir="", fn_list=[], verbose=False, fmt=CSVSpatialFormatType.TUM,
+                est_err_type=EstimationErrorType.none,
+                err_rep=ErrorRepresentationType.none,
+                ):
         """"
         Extracts a list of topic from a rosbag file and stores each topic in a file specified in "fn_list"
 
 
         Example:
         >> args.bagfile  = "example.bag"
         >> args.topics =  ["/CS_200_MAV1/estimated_poseWithCov",  "/pose_sensor/pose"]
         >> args.verbose = True
         >> args.result_dir = "./results"
         >> args.filenames = ["mav_PoseWithCov.csv", "sensor_PoseWithCov"]
-        >> args.format = CSVFormatPose.PoseWithCov
+        >> args.format = CSVSpatialFormatType.PoseWithCov
         >> ROSbag2CSV.extract(bagfile_name=args.bagfile, topic_list=args.topics,
                       fn_list=args.filenames, result_dir=args.result_dir,
-                      verbose=args.verbose, fmt=CSVFormatPose(args.format)):
+                      verbose=args.verbose, fmt=CSVSpatialFormatType(args.format)):
 
 
         Input:
         bagfile_name -- file name of the rosbag
         topic_list -- list of topic names, these must start with a "/" (absolute topic name)
         result_dir  -- root directory the files to be created (defined in fn_list)
         fn_list -- list of file names;  (not the entire path!) just name with or without extension
@@ -100,15 +103,15 @@
             if verbose:
                 print("ROSbag2CSV: Unexpected error, bag file might be empty!")
             bag.close()
             return False
 
         ## create result dir:
         if result_dir == "":
-            folder = str.rstrip(bagfile_name, ".bag")
+            folder = str(bagfile_name).replace(".bag", "")
         else:
             folder = result_dir
 
         folder = os.path.abspath(folder)
         try:  # else already exists
             os.makedirs(folder)
         except:
@@ -169,19 +172,20 @@
         for topic, msg, t in tqdm(bag.read_messages(), total=num_messages, unit="msgs"):
             if topic in topic_list:
                 message_type = ROSMessageTypes.get_message_type(msg)
                 if message_type != ROSMessageTypes.NOT_SUPPORTED:
                     file_writer = dict_file_writers[topic]
 
                     if not dict_header_written[topic]:
-                        file_writer.writerow(CSVFormatPose.get_header(fmt))
+                        file_writer.writerow(CSVSpatialFormatType.get_header(fmt))
                         dict_header_written[topic] = True
 
                     # HINT: all conversions are done in ROSMsg2CSVLine
-                    content = ROSMsg2CSVLine.to(fmt, msg, t, message_type)
+                    content = ROSMsg2CSVLine.to(fmt, msg, t, message_type,
+                                                est_err_type=est_err_type, err_rep=err_rep)
 
                     if content is not None:
                         file_writer.writerow(content)
 
         ## CLEANUP:
         # close all csv files
         for topicName in topic_list:
@@ -212,21 +216,26 @@
         description='ROSbag2CSV: extract and store given topics of a rosbag into a CSV file')
     parser.add_argument('--bagfile', help='input bag file', default="not specified")
     parser.add_argument('--topics', nargs='*', help='desired topics', default=[])
     parser.add_argument('--filenames', nargs='*', help='csv filename of corresponding topic', default=[])
     parser.add_argument('--result_dir', help='directory to store results [otherwise bagfile name will be a directory]',
                         default='')
     parser.add_argument('--verbose', action='store_true', default=False)
-    parser.add_argument('--format', help='CSV format', choices=CSVFormatPose.list(),
-                        default=str(CSVFormatPose.TUM))
-
+    parser.add_argument('--format', help='CSV format', choices=CSVSpatialFormatType.list(),
+                        default=str(CSVSpatialFormatType.TUM))
+    parser.add_argument('--est_err_type', help='Estimation error type (e.g. global/local pose)', choices=EstimationErrorType.list(),
+                        default=str(EstimationErrorType.none))
+    parser.add_argument('--err_rep', help='Error representation type', choices=ErrorRepresentationType.list(),
+                        default=str(ErrorRepresentationType.none))
     tp_start = time.time()
     args = parser.parse_args()
 
     if ROSbag2CSV.extract(bagfile_name=args.bagfile, topic_list=args.topics,
                           fn_list=args.filenames, result_dir=args.result_dir,
-                          verbose=args.verbose, fmt=CSVFormatPose(args.format)):
+                          verbose=args.verbose, fmt=CSVSpatialFormatType(args.format),
+                          est_err_type=EstimationErrorType(args.est_err_type),
+                          err_rep=ErrorRepresentationType(args.err_rep)
+                          ):
         print(" ")
         print("finished after [%s sec]\n" % str(time.time() - tp_start))
-        script_utils.exit_success()
     else:
-        script_utils.exit_failure()
+        print("failed! after [%s sec]\n" % str(time.time() - tp_start))
```

### Comparing `cnspy_rosbag2csv-0.1.2/cnspy_rosbag2csv.egg-info/SOURCES.txt` & `cnspy_rosbag2csv-0.2.0/cnspy_rosbag2csv.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,18 @@
+LICENCE
 README.md
 setup.py
 cnspy_rosbag2csv/CSV2ROSbag.py
 cnspy_rosbag2csv/CSVLine2ROSMsg.py
 cnspy_rosbag2csv/CSVParser.py
 cnspy_rosbag2csv/ROSMessageTypes.py
 cnspy_rosbag2csv/ROSMsg2CSVLine.py
 cnspy_rosbag2csv/ROSbag2CSV.py
+cnspy_rosbag2csv/ROSbagMerge.py
+cnspy_rosbag2csv/ROSbag_ReTimestamp.py
 cnspy_rosbag2csv/__init__.py
 cnspy_rosbag2csv.egg-info/PKG-INFO
 cnspy_rosbag2csv.egg-info/SOURCES.txt
 cnspy_rosbag2csv.egg-info/dependency_links.txt
 cnspy_rosbag2csv.egg-info/requires.txt
 cnspy_rosbag2csv.egg-info/top_level.txt
 test/__init__.py
```

### Comparing `cnspy_rosbag2csv-0.1.2/setup.py` & `cnspy_rosbag2csv-0.2.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -31,9 +31,9 @@
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Operating System :: OS Independent",
     ],
     
     packages=find_packages(exclude=["test_*", "TODO*"]),
     python_requires='>=3.6',
-    install_requires=['numpy', 'tqdm', 'pandas', 'argparse', 'PyYAML', 'spatialmath-python', 'pycryptodomex', 'pycryptodome', 'gnupg', 'lz4', 'cnspy_script_utils', 'cnspy_spatial_csv_formats'],
+    install_requires=['numpy', 'tqdm', 'pandas', 'argparse', 'PyYAML', 'rospkg', 'spatialmath-python', 'pycryptodomex', 'pycryptodome', 'gnupg', 'lz4', 'cnspy_spatial_csv_formats'],
 )
```

### Comparing `cnspy_rosbag2csv-0.1.2/test/test_CSV2ROSbag.py` & `cnspy_rosbag2csv-0.2.0/test/test_ROSbag2CSV.py`

 * *Files 20% similar despite different names*

```diff
@@ -15,21 +15,32 @@
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 #
 ########################################################################################################################
 
 import os
 import unittest
-from cnspy_rosbag2csv.CSV2ROSbag import *
+from cnspy_rosbag2csv.ROSbag2CSV import *
 
 SAMPLE_DATA_DIR = os.path.join(os.path.dirname(os.path.abspath(__file__)), 'sample_data')
 
-class CSV2ROSbag_Test(unittest.TestCase):
-    def test_identify(self):
-        fn_list = [str(SAMPLE_DATA_DIR + '/ID1-pose-est-cov.csv'), str(SAMPLE_DATA_DIR + '/ID1-pose-gt.csv')]
+class ROSbag2CSV_Test(unittest.TestCase):
+    def test_convert2PosOrientCov(self):
+        fn_list = ['/mav_PosOrientWithCov.csv', '/sensor_PosOrientWithCov.csv']
         topic_list = ['/pose_est', '/pose_gt']
-        fmt_list = [ROSMessageTypes.GEOMETRY_MSGS_POSEWITHCOVARIANCESTAMPED, ROSMessageTypes.GEOMETRY_MSGS_POSESTAMPED]
-        CSV2ROSbag.extract('my.bag', topic_list, fn_list, fmt_list, result_dir=str(SAMPLE_DATA_DIR + '/results'), verbose=True)
 
+        bagfile = str(SAMPLE_DATA_DIR + '/example.bag')    
+        self.assertTrue(ROSbag2CSV.extract(bagfile_name=bagfile, topic_list=topic_list,
+                                           fn_list=fn_list, result_dir=str(SAMPLE_DATA_DIR + '/results'),
+                                           verbose=True, fmt=CSVSpatialFormatType('PosOrientWithCov')))
+
+    def test_convert2PosCov(self):
+        fn_list = ['/mav_PoseWithCov.csv', '/sensor_PoseWithCov.csv']
+        topic_list = ['/pose_est', '/pose_gt']
+
+        bagfile = str(SAMPLE_DATA_DIR + '/example.bag')
+        self.assertTrue(ROSbag2CSV.extract(bagfile_name=bagfile, topic_list=topic_list,
+                                           fn_list=fn_list, result_dir=str(SAMPLE_DATA_DIR + '/results'),
+                                           verbose=True, fmt=CSVSpatialFormatType('PoseWithCov')))
 
 if __name__ == "__main__":
      unittest.main()
```

### Comparing `cnspy_rosbag2csv-0.1.2/test/test_CSVLine2ROSMsg.py` & `cnspy_rosbag2csv-0.2.0/test/test_CSVLine2ROSMsg.py`

 * *Files 12% similar despite different names*

```diff
@@ -45,16 +45,24 @@
         print(msg)
         msg = CSVLine2ROSMsg.from_TUM(line, 1, msg_type=ROSMessageTypes.GEOMETRY_MSGS_TRANSFORM)
         print(msg)
         msg = CSVLine2ROSMsg.from_TUM(line, 1, msg_type=ROSMessageTypes.GEOMETRY_MSGS_TRANSFORMSTAMPED)
         print(msg)
         print('done')
 
-    def test_from_PoseWithCov(self):
+    def test_from_PosOrientWithCov(self):
         line = str('0.1, 1.0, 2.0,3.0, 0,0,0,1.0, 8.0,8.1,8.2,8.7,8.8,8.14, 9.21,9.22,9.23,9.28,9.29,9.35')
+        msg = CSVLine2ROSMsg.from_PosOrientWithCov(line, 1, msg_type=ROSMessageTypes.GEOMETRY_MSGS_POSEWITHCOVARIANCESTAMPED)
+        print(msg)
+        msg = CSVLine2ROSMsg.from_PosOrientWithCov(line, 1, msg_type=ROSMessageTypes.GEOMETRY_MSGS_POSEWITHCOVARIANCE)
+        print(msg)
+        print('done')
+
+    def test_from_PoseWithCov(self):
+        line = str('0.1, 1.0, 2.0,3.0, 0,0,0,1.0, 8.0,8.1,8.2,8.7,8.8,8.14, 9.21,9.22,9.23,9.28,9.29,9.35, 7.3,7.4,7.5,7.9,7.10,7.11,7.15,7.16,7.17')
         msg = CSVLine2ROSMsg.from_PoseWithCov(line, 1, msg_type=ROSMessageTypes.GEOMETRY_MSGS_POSEWITHCOVARIANCESTAMPED)
         print(msg)
         msg = CSVLine2ROSMsg.from_PoseWithCov(line, 1, msg_type=ROSMessageTypes.GEOMETRY_MSGS_POSEWITHCOVARIANCE)
         print(msg)
         print('done')
```

### Comparing `cnspy_rosbag2csv-0.1.2/test/test_ROSMsg2CSVLine.py` & `cnspy_rosbag2csv-0.2.0/test/test_ROSMsg2CSVLine.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #
 # Requirements:
 # enum
 ########################################################################################################################
 import unittest
 from cnspy_rosbag2csv.ROSMsg2CSVLine import *
 from cnspy_rosbag2csv.ROSMessageTypes import ROSMessageTypes
-from cnspy_spatial_csv_formats.CSVFormatPose import CSVFormatPose
+from cnspy_spatial_csv_formats.CSVSpatialFormatType import CSVSpatialFormatType
 
 from geometry_msgs.msg import Point, PointStamped, Vector3, Vector3Stamped
 from geometry_msgs.msg import Pose, PoseStamped, PoseWithCovariance, PoseWithCovarianceStamped
 from geometry_msgs.msg import Quaternion, QuaternionStamped, Transform, TransformStamped
 
 
 class Time:
@@ -104,34 +104,56 @@
         line = ROSMsg2CSVLine.to(fmt, Quaternion(), t, ROSMessageTypes.GEOMETRY_MSGS_QUATERNION)
         line = ROSMsg2CSVLine.to(fmt, QuaternionStamped(), t, ROSMessageTypes.GEOMETRY_MSGS_QUATERNIONSTAMPED)
         line = ROSMsg2CSVLine.to(fmt, Transform(), t, ROSMessageTypes.GEOMETRY_MSGS_TRANSFORM)
         line = ROSMsg2CSVLine.to(fmt, TransformStamped(), t, ROSMessageTypes.GEOMETRY_MSGS_TRANSFORMSTAMPED)
         return line
 
     def test_MESSAGE_TO_TUM_SHORT(self):
-        line = self.get_lines(CSVFormatPose.PositionStamped)
+        line = self.get_lines(CSVSpatialFormatType.PositionStamped)
+
+    def test_MESSAGE_TO_PosOrientCov(self):
+        t = Time()
+        t.secs = 0
+        pose_cov = PoseWithCovarianceStamped()
+        pose_cov.pose.covariance = range(0, 36, 1)
+        line = ROSMsg2CSVLine.to_PosOrientCov(pose_cov, t, ROSMessageTypes.GEOMETRY_MSGS_POSEWITHCOVARIANCESTAMPED)
+        print('\nline1:' + str(line))
+
+        pose_cov = PoseWithCovariance()
+        pose_cov.covariance = range(0, 36, 1)
+        line = ROSMsg2CSVLine.to_PosOrientCov(pose_cov, t, ROSMessageTypes.GEOMETRY_MSGS_POSEWITHCOVARIANCE)
+        print('\nline2:' + str(line))
+        self.assertTrue(len(line) == 13)
+        line = self.get_lines(CSVSpatialFormatType.PosOrientCov)
+        self.assertTrue(len(line) == 13)
 
     def test_MESSAGE_TO_PoseCov(self):
         t = Time()
         t.secs = 0
         pose_cov = PoseWithCovarianceStamped()
         pose_cov.pose.covariance = range(0, 36, 1)
         line = ROSMsg2CSVLine.to_PoseCov(pose_cov, t, ROSMessageTypes.GEOMETRY_MSGS_POSEWITHCOVARIANCESTAMPED)
-        print('line1:' + str(line))
+        print('\nline1:' + str(line))
 
         pose_cov = PoseWithCovariance()
         pose_cov.covariance = range(0, 36, 1)
         line = ROSMsg2CSVLine.to_PoseCov(pose_cov, t, ROSMessageTypes.GEOMETRY_MSGS_POSEWITHCOVARIANCE)
-        print('line2:' + str(line))
-        self.assertTrue(len(line) == 13)
-        line = self.get_lines(CSVFormatPose.PoseCov)
-        self.assertTrue(len(line) == 13)
+        print('\nline2:' + str(line))
+        self.assertTrue(len(line) == 13+9)
+        line = self.get_lines(CSVSpatialFormatType.PoseCov)
+        self.assertTrue(len(line) == 13+9)
 
-    def test_MESSAGE_TO_PoseWithCov(self):
-        line = self.get_lines(CSVFormatPose.PoseWithCov)
-        print('line:' + str(line))
+
+    def test_MESSAGE_TO_PosOrientWithCov(self):
+        line = self.get_lines(CSVSpatialFormatType.PosOrientWithCov)
+        print('\nline:' + str(line))
         self.assertTrue(len(line) == 20)
 
+    def test_MESSAGE_TO_PoseWithCov(self):
+        line = self.get_lines(CSVSpatialFormatType.PoseWithCov)
+        print('\nline:' + str(line))
+        self.assertTrue(len(line) == 29)
+
 
 if __name__ == "__main__":
     unittest.main()
     print("testing supported ROS msgs types")
```


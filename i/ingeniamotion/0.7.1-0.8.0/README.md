# Comparing `tmp/ingeniamotion-0.7.1.tar.gz` & `tmp/ingeniamotion-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ingeniamotion-0.7.1.tar", last modified: Fri Mar 15 08:54:43 2024, max compression
+gzip compressed data, was "ingeniamotion-0.8.0.tar", last modified: Tue Apr 23 13:21:54 2024, max compression
```

## Comparing `ingeniamotion-0.7.1.tar` & `ingeniamotion-0.8.0.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxrwxrwx   0        0        0        0 2024-03-15 08:54:40.216308 ingeniamotion-0.7.1/
--rw-rw-rw-   0        0        0    17630 2024-03-15 08:49:30.000000 ingeniamotion-0.7.1/LICENSE.md
--rw-rw-rw-   0        0        0       38 2024-03-15 08:49:30.000000 ingeniamotion-0.7.1/MANIFEST.in
--rw-rw-rw-   0        0        0     3977 2024-03-15 08:54:43.141409 ingeniamotion-0.7.1/PKG-INFO
--rw-rw-rw-   0        0        0     1259 2024-03-15 08:49:30.000000 ingeniamotion-0.7.1/README.md
-drwxrwxrwx   0        0        0        0 2024-03-15 08:54:40.196310 ingeniamotion-0.7.1/docs/
--rw-rw-rw-   0        0        0     3314 2024-03-15 08:49:30.000000 ingeniamotion-0.7.1/docs/what_is_ingeniamotion.rst
-drwxrwxrwx   0        0        0        0 2024-03-15 08:54:40.238307 ingeniamotion-0.7.1/ingeniamotion/
--rw-rw-rw-   0        0        0      167 2024-03-15 08:49:30.000000 ingeniamotion-0.7.1/ingeniamotion/__init__.py
--rw-rw-rw-   0        0        0    27436 2024-03-15 08:49:30.000000 ingeniamotion-0.7.1/ingeniamotion/capture.py
--rw-rw-rw-   0        0        0     6355 2024-03-15 08:49:30.000000 ingeniamotion-0.7.1/ingeniamotion/comkit.py
--rw-rw-rw-   0        0        0    42177 2024-03-15 08:49:30.000000 ingeniamotion-0.7.1/ingeniamotion/communication.py
--rw-rw-rw-   0        0        0    47052 2024-03-15 08:49:30.000000 ingeniamotion-0.7.1/ingeniamotion/configuration.py
--rw-rw-rw-   0        0        0    12648 2024-03-15 08:49:30.000000 ingeniamotion-0.7.1/ingeniamotion/disturbance.py
--rw-rw-rw-   0        0        0    18276 2024-03-15 08:49:30.000000 ingeniamotion-0.7.1/ingeniamotion/drive_tests.py
-drwxrwxrwx   0        0        0        0 2024-03-15 08:54:40.227309 ingeniamotion-0.7.1/ingeniamotion/enums/
--rw-rw-rw-   0        0        0     4606 2024-03-15 08:49:30.000000 ingeniamotion-0.7.1/ingeniamotion/enums/__init__.py
--rw-rw-rw-   0        0        0    11615 2024-03-15 08:49:30.000000 ingeniamotion-0.7.1/ingeniamotion/errors.py
--rw-rw-rw-   0        0        0      803 2024-03-15 08:49:30.000000 ingeniamotion-0.7.1/ingeniamotion/exceptions.py
--rw-rw-rw-   0        0        0    24696 2024-03-15 08:49:30.000000 ingeniamotion-0.7.1/ingeniamotion/feedbacks.py
--rw-rw-rw-   0        0        0    10453 2024-03-15 08:49:30.000000 ingeniamotion-0.7.1/ingeniamotion/homing.py
--rw-rw-rw-   0        0        0    10990 2024-03-15 08:49:30.000000 ingeniamotion-0.7.1/ingeniamotion/information.py
--rw-rw-rw-   0        0        0     3117 2024-03-15 08:49:30.000000 ingeniamotion-0.7.1/ingeniamotion/metaclass.py
-drwxrwxrwx   0        0        0        0 2024-03-15 08:54:40.237307 ingeniamotion-0.7.1/ingeniamotion/monitoring/
--rw-rw-rw-   0        0        0        0 2024-03-15 08:49:30.000000 ingeniamotion-0.7.1/ingeniamotion/monitoring/__init__.py
--rw-rw-rw-   0        0        0    19787 2024-03-15 08:49:30.000000 ingeniamotion-0.7.1/ingeniamotion/monitoring/base_monitoring.py
--rw-rw-rw-   0        0        0     7031 2024-03-15 08:49:30.000000 ingeniamotion-0.7.1/ingeniamotion/monitoring/monitoring_v1.py
--rw-rw-rw-   0        0        0     6004 2024-03-15 08:49:30.000000 ingeniamotion-0.7.1/ingeniamotion/monitoring/monitoring_v3.py
--rw-rw-rw-   0        0        0    30525 2024-03-15 08:49:30.000000 ingeniamotion-0.7.1/ingeniamotion/motion.py
--rw-rw-rw-   0        0        0     4451 2024-03-15 08:49:30.000000 ingeniamotion-0.7.1/ingeniamotion/motion_controller.py
--rw-rw-rw-   0        0        0        0 2024-03-15 08:49:30.000000 ingeniamotion-0.7.1/ingeniamotion/py.typed
-drwxrwxrwx   0        0        0        0 2024-03-15 08:54:40.249304 ingeniamotion-0.7.1/ingeniamotion/wizard_tests/
--rw-rw-rw-   0        0        0        0 2024-03-15 08:49:30.000000 ingeniamotion-0.7.1/ingeniamotion/wizard_tests/__init__.py
--rw-rw-rw-   0        0        0     4247 2024-03-15 08:49:30.000000 ingeniamotion-0.7.1/ingeniamotion/wizard_tests/base_test.py
--rw-rw-rw-   0        0        0     2816 2024-03-15 08:49:30.000000 ingeniamotion-0.7.1/ingeniamotion/wizard_tests/brake.py
--rw-rw-rw-   0        0        0     5988 2024-03-15 08:49:30.000000 ingeniamotion-0.7.1/ingeniamotion/wizard_tests/brake_tune.py
-drwxrwxrwx   0        0        0        0 2024-03-15 08:54:40.260307 ingeniamotion-0.7.1/ingeniamotion/wizard_tests/feedbacks_tests/
--rw-rw-rw-   0        0        0        0 2024-03-15 08:49:30.000000 ingeniamotion-0.7.1/ingeniamotion/wizard_tests/feedbacks_tests/__init__.py
--rw-rw-rw-   0        0        0      665 2024-03-15 08:49:30.000000 ingeniamotion-0.7.1/ingeniamotion/wizard_tests/feedbacks_tests/absolute_encoder1_test.py
--rw-rw-rw-   0        0        0      944 2024-03-15 08:49:30.000000 ingeniamotion-0.7.1/ingeniamotion/wizard_tests/feedbacks_tests/absolute_encoder2_test.py
--rw-rw-rw-   0        0        0     6591 2024-03-15 08:49:30.000000 ingeniamotion-0.7.1/ingeniamotion/wizard_tests/feedbacks_tests/dc_feedback_polarity_test.py
--rw-rw-rw-   0        0        0     6404 2024-03-15 08:49:30.000000 ingeniamotion-0.7.1/ingeniamotion/wizard_tests/feedbacks_tests/dc_feedback_resolution_test.py
--rw-rw-rw-   0        0        0     2933 2024-03-15 08:49:30.000000 ingeniamotion-0.7.1/ingeniamotion/wizard_tests/feedbacks_tests/digital_hall_test.py
--rw-rw-rw-   0        0        0      651 2024-03-15 08:49:30.000000 ingeniamotion-0.7.1/ingeniamotion/wizard_tests/feedbacks_tests/digital_incremental1_test.py
--rw-rw-rw-   0        0        0      654 2024-03-15 08:49:30.000000 ingeniamotion-0.7.1/ingeniamotion/wizard_tests/feedbacks_tests/digital_incremental2_test.py
--rw-rw-rw-   0        0        0    20411 2024-03-15 08:49:30.000000 ingeniamotion-0.7.1/ingeniamotion/wizard_tests/feedbacks_tests/feedback_test.py
--rw-rw-rw-   0        0        0      618 2024-03-15 08:49:30.000000 ingeniamotion-0.7.1/ingeniamotion/wizard_tests/feedbacks_tests/secondary_ssi_test.py
--rw-rw-rw-   0        0        0    13814 2024-03-15 08:49:30.000000 ingeniamotion-0.7.1/ingeniamotion/wizard_tests/phase_calibration.py
--rw-rw-rw-   0        0        0     8635 2024-03-15 08:49:30.000000 ingeniamotion-0.7.1/ingeniamotion/wizard_tests/phasing_check.py
--rw-rw-rw-   0        0        0     4349 2024-03-15 08:49:30.000000 ingeniamotion-0.7.1/ingeniamotion/wizard_tests/sto.py
--rw-rw-rw-   0        0        0      915 2024-03-15 08:49:30.000000 ingeniamotion-0.7.1/ingeniamotion/wizard_tests/stoppable.py
-drwxrwxrwx   0        0        0        0 2024-03-15 08:54:40.216308 ingeniamotion-0.7.1/ingeniamotion.egg-info/
--rw-rw-rw-   0        0        0     3977 2024-03-15 08:54:39.000000 ingeniamotion-0.7.1/ingeniamotion.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2313 2024-03-15 08:54:40.000000 ingeniamotion-0.7.1/ingeniamotion.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-15 08:54:39.000000 ingeniamotion-0.7.1/ingeniamotion.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2024-03-15 08:54:39.000000 ingeniamotion-0.7.1/ingeniamotion.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2024-03-15 08:54:39.000000 ingeniamotion-0.7.1/ingeniamotion.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-15 08:54:43.159459 ingeniamotion-0.7.1/setup.cfg
--rw-rw-rw-   0        0        0     1264 2024-03-15 08:49:30.000000 ingeniamotion-0.7.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-15 08:54:40.273306 ingeniamotion-0.7.1/tests/
--rw-rw-rw-   0        0        0        0 2024-03-15 08:49:30.000000 ingeniamotion-0.7.1/tests/__init__.py
--rw-rw-rw-   0        0        0     7768 2024-03-15 08:49:30.000000 ingeniamotion-0.7.1/tests/conftest.py
--rw-rw-rw-   0        0        0     7358 2024-03-15 08:49:30.000000 ingeniamotion-0.7.1/tests/load_FWs.py
--rw-rw-rw-   0        0        0    11447 2024-03-15 08:49:30.000000 ingeniamotion-0.7.1/tests/test_all_drive_tests.py
--rw-rw-rw-   0        0        0    17659 2024-03-15 08:49:30.000000 ingeniamotion-0.7.1/tests/test_capture.py
--rw-rw-rw-   0        0        0     3136 2024-03-15 08:49:30.000000 ingeniamotion-0.7.1/tests/test_comkit.py
--rw-rw-rw-   0        0        0    11142 2024-03-15 08:49:30.000000 ingeniamotion-0.7.1/tests/test_communication.py
--rw-rw-rw-   0        0        0    30620 2024-03-15 08:49:30.000000 ingeniamotion-0.7.1/tests/test_configuration.py
--rw-rw-rw-   0        0        0     5513 2024-03-15 08:49:30.000000 ingeniamotion-0.7.1/tests/test_disturbance.py
--rw-rw-rw-   0        0        0     6446 2024-03-15 08:49:30.000000 ingeniamotion-0.7.1/tests/test_errors.py
--rw-rw-rw-   0        0        0     6986 2024-03-15 08:49:30.000000 ingeniamotion-0.7.1/tests/test_examples.py
--rw-rw-rw-   0        0        0     3210 2024-03-15 08:49:30.000000 ingeniamotion-0.7.1/tests/test_feedback_test.py
--rw-rw-rw-   0        0        0    17939 2024-03-15 08:49:30.000000 ingeniamotion-0.7.1/tests/test_feedbacks.py
--rw-rw-rw-   0        0        0    10468 2024-03-15 08:49:30.000000 ingeniamotion-0.7.1/tests/test_homing.py
--rw-rw-rw-   0        0        0     7354 2024-03-15 08:49:30.000000 ingeniamotion-0.7.1/tests/test_information.py
--rw-rw-rw-   0        0        0    15648 2024-03-15 08:49:30.000000 ingeniamotion-0.7.1/tests/test_monitoring.py
--rw-rw-rw-   0        0        0    17833 2024-03-15 08:49:30.000000 ingeniamotion-0.7.1/tests/test_motion.py
--rw-rw-rw-   0        0        0     3785 2024-03-15 08:49:30.000000 ingeniamotion-0.7.1/tests/test_motion_controller.py
+drwxrwxrwx   0        0        0        0 2024-04-23 13:21:52.132677 ingeniamotion-0.8.0/
+-rw-rw-rw-   0        0        0    17630 2024-04-23 13:18:25.000000 ingeniamotion-0.8.0/LICENSE.md
+-rw-rw-rw-   0        0        0       38 2024-04-23 13:18:25.000000 ingeniamotion-0.8.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     3977 2024-04-23 13:21:54.506051 ingeniamotion-0.8.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1259 2024-04-23 13:18:25.000000 ingeniamotion-0.8.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-23 13:21:52.113482 ingeniamotion-0.8.0/docs/
+-rw-rw-rw-   0        0        0     3314 2024-04-23 13:18:25.000000 ingeniamotion-0.8.0/docs/what_is_ingeniamotion.rst
+drwxrwxrwx   0        0        0        0 2024-04-23 13:21:52.151679 ingeniamotion-0.8.0/ingeniamotion/
+-rw-rw-rw-   0        0        0      167 2024-04-23 13:18:25.000000 ingeniamotion-0.8.0/ingeniamotion/__init__.py
+-rw-rw-rw-   0        0        0    27703 2024-04-23 13:18:25.000000 ingeniamotion-0.8.0/ingeniamotion/capture.py
+-rw-rw-rw-   0        0        0    51658 2024-04-23 13:18:25.000000 ingeniamotion-0.8.0/ingeniamotion/communication.py
+-rw-rw-rw-   0        0        0    47052 2024-04-23 13:18:25.000000 ingeniamotion-0.8.0/ingeniamotion/configuration.py
+-rw-rw-rw-   0        0        0    12634 2024-04-23 13:18:25.000000 ingeniamotion-0.8.0/ingeniamotion/disturbance.py
+-rw-rw-rw-   0        0        0    18276 2024-04-23 13:18:25.000000 ingeniamotion-0.8.0/ingeniamotion/drive_tests.py
+drwxrwxrwx   0        0        0        0 2024-04-23 13:21:52.142680 ingeniamotion-0.8.0/ingeniamotion/enums/
+-rw-rw-rw-   0        0        0     4606 2024-04-23 13:18:25.000000 ingeniamotion-0.8.0/ingeniamotion/enums/__init__.py
+-rw-rw-rw-   0        0        0    11615 2024-04-23 13:18:25.000000 ingeniamotion-0.8.0/ingeniamotion/errors.py
+-rw-rw-rw-   0        0        0      803 2024-04-23 13:18:25.000000 ingeniamotion-0.8.0/ingeniamotion/exceptions.py
+-rw-rw-rw-   0        0        0    24696 2024-04-23 13:18:25.000000 ingeniamotion-0.8.0/ingeniamotion/feedbacks.py
+-rw-rw-rw-   0        0        0    10453 2024-04-23 13:18:25.000000 ingeniamotion-0.8.0/ingeniamotion/homing.py
+-rw-rw-rw-   0        0        0    10513 2024-04-23 13:18:25.000000 ingeniamotion-0.8.0/ingeniamotion/information.py
+-rw-rw-rw-   0        0        0     3117 2024-04-23 13:18:25.000000 ingeniamotion-0.8.0/ingeniamotion/metaclass.py
+drwxrwxrwx   0        0        0        0 2024-04-23 13:21:52.151679 ingeniamotion-0.8.0/ingeniamotion/monitoring/
+-rw-rw-rw-   0        0        0        0 2024-04-23 13:18:25.000000 ingeniamotion-0.8.0/ingeniamotion/monitoring/__init__.py
+-rw-rw-rw-   0        0        0    19787 2024-04-23 13:18:25.000000 ingeniamotion-0.8.0/ingeniamotion/monitoring/base_monitoring.py
+-rw-rw-rw-   0        0        0     7031 2024-04-23 13:18:25.000000 ingeniamotion-0.8.0/ingeniamotion/monitoring/monitoring_v1.py
+-rw-rw-rw-   0        0        0     6004 2024-04-23 13:18:25.000000 ingeniamotion-0.8.0/ingeniamotion/monitoring/monitoring_v3.py
+-rw-rw-rw-   0        0        0    30525 2024-04-23 13:18:25.000000 ingeniamotion-0.8.0/ingeniamotion/motion.py
+-rw-rw-rw-   0        0        0     4451 2024-04-23 13:18:25.000000 ingeniamotion-0.8.0/ingeniamotion/motion_controller.py
+-rw-rw-rw-   0        0        0    29773 2024-04-23 13:18:25.000000 ingeniamotion-0.8.0/ingeniamotion/pdo.py
+-rw-rw-rw-   0        0        0        0 2024-04-23 13:18:25.000000 ingeniamotion-0.8.0/ingeniamotion/py.typed
+drwxrwxrwx   0        0        0        0 2024-04-23 13:21:52.161680 ingeniamotion-0.8.0/ingeniamotion/wizard_tests/
+-rw-rw-rw-   0        0        0        0 2024-04-23 13:18:25.000000 ingeniamotion-0.8.0/ingeniamotion/wizard_tests/__init__.py
+-rw-rw-rw-   0        0        0     4247 2024-04-23 13:18:25.000000 ingeniamotion-0.8.0/ingeniamotion/wizard_tests/base_test.py
+-rw-rw-rw-   0        0        0     2816 2024-04-23 13:18:25.000000 ingeniamotion-0.8.0/ingeniamotion/wizard_tests/brake.py
+-rw-rw-rw-   0        0        0     5988 2024-04-23 13:18:25.000000 ingeniamotion-0.8.0/ingeniamotion/wizard_tests/brake_tune.py
+drwxrwxrwx   0        0        0        0 2024-04-23 13:21:52.172681 ingeniamotion-0.8.0/ingeniamotion/wizard_tests/feedbacks_tests/
+-rw-rw-rw-   0        0        0        0 2024-04-23 13:18:25.000000 ingeniamotion-0.8.0/ingeniamotion/wizard_tests/feedbacks_tests/__init__.py
+-rw-rw-rw-   0        0        0      665 2024-04-23 13:18:25.000000 ingeniamotion-0.8.0/ingeniamotion/wizard_tests/feedbacks_tests/absolute_encoder1_test.py
+-rw-rw-rw-   0        0        0      944 2024-04-23 13:18:25.000000 ingeniamotion-0.8.0/ingeniamotion/wizard_tests/feedbacks_tests/absolute_encoder2_test.py
+-rw-rw-rw-   0        0        0     6591 2024-04-23 13:18:25.000000 ingeniamotion-0.8.0/ingeniamotion/wizard_tests/feedbacks_tests/dc_feedback_polarity_test.py
+-rw-rw-rw-   0        0        0     6404 2024-04-23 13:18:25.000000 ingeniamotion-0.8.0/ingeniamotion/wizard_tests/feedbacks_tests/dc_feedback_resolution_test.py
+-rw-rw-rw-   0        0        0     2933 2024-04-23 13:18:25.000000 ingeniamotion-0.8.0/ingeniamotion/wizard_tests/feedbacks_tests/digital_hall_test.py
+-rw-rw-rw-   0        0        0      651 2024-04-23 13:18:25.000000 ingeniamotion-0.8.0/ingeniamotion/wizard_tests/feedbacks_tests/digital_incremental1_test.py
+-rw-rw-rw-   0        0        0      654 2024-04-23 13:18:25.000000 ingeniamotion-0.8.0/ingeniamotion/wizard_tests/feedbacks_tests/digital_incremental2_test.py
+-rw-rw-rw-   0        0        0    20411 2024-04-23 13:18:25.000000 ingeniamotion-0.8.0/ingeniamotion/wizard_tests/feedbacks_tests/feedback_test.py
+-rw-rw-rw-   0        0        0      618 2024-04-23 13:18:25.000000 ingeniamotion-0.8.0/ingeniamotion/wizard_tests/feedbacks_tests/secondary_ssi_test.py
+-rw-rw-rw-   0        0        0    13814 2024-04-23 13:18:25.000000 ingeniamotion-0.8.0/ingeniamotion/wizard_tests/phase_calibration.py
+-rw-rw-rw-   0        0        0     8635 2024-04-23 13:18:25.000000 ingeniamotion-0.8.0/ingeniamotion/wizard_tests/phasing_check.py
+-rw-rw-rw-   0        0        0     4349 2024-04-23 13:18:25.000000 ingeniamotion-0.8.0/ingeniamotion/wizard_tests/sto.py
+-rw-rw-rw-   0        0        0      915 2024-04-23 13:18:25.000000 ingeniamotion-0.8.0/ingeniamotion/wizard_tests/stoppable.py
+drwxrwxrwx   0        0        0        0 2024-04-23 13:21:52.132677 ingeniamotion-0.8.0/ingeniamotion.egg-info/
+-rw-rw-rw-   0        0        0     3977 2024-04-23 13:21:51.000000 ingeniamotion-0.8.0/ingeniamotion.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2307 2024-04-23 13:21:51.000000 ingeniamotion-0.8.0/ingeniamotion.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-23 13:21:51.000000 ingeniamotion-0.8.0/ingeniamotion.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2024-04-23 13:21:51.000000 ingeniamotion-0.8.0/ingeniamotion.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2024-04-23 13:21:51.000000 ingeniamotion-0.8.0/ingeniamotion.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-23 13:21:54.521703 ingeniamotion-0.8.0/setup.cfg
+-rw-rw-rw-   0        0        0     1264 2024-04-23 13:18:25.000000 ingeniamotion-0.8.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-23 13:21:52.182676 ingeniamotion-0.8.0/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-23 13:18:25.000000 ingeniamotion-0.8.0/tests/__init__.py
+-rw-rw-rw-   0        0        0     7829 2024-04-23 13:18:25.000000 ingeniamotion-0.8.0/tests/conftest.py
+-rw-rw-rw-   0        0        0     7358 2024-04-23 13:18:25.000000 ingeniamotion-0.8.0/tests/load_FWs.py
+-rw-rw-rw-   0        0        0    11447 2024-04-23 13:18:25.000000 ingeniamotion-0.8.0/tests/test_all_drive_tests.py
+-rw-rw-rw-   0        0        0    17659 2024-04-23 13:18:25.000000 ingeniamotion-0.8.0/tests/test_capture.py
+-rw-rw-rw-   0        0        0    19463 2024-04-23 13:18:25.000000 ingeniamotion-0.8.0/tests/test_communication.py
+-rw-rw-rw-   0        0        0    30620 2024-04-23 13:18:25.000000 ingeniamotion-0.8.0/tests/test_configuration.py
+-rw-rw-rw-   0        0        0     5513 2024-04-23 13:18:25.000000 ingeniamotion-0.8.0/tests/test_disturbance.py
+-rw-rw-rw-   0        0        0     6446 2024-04-23 13:18:25.000000 ingeniamotion-0.8.0/tests/test_errors.py
+-rw-rw-rw-   0        0        0    31377 2024-04-23 13:18:25.000000 ingeniamotion-0.8.0/tests/test_examples.py
+-rw-rw-rw-   0        0        0     3210 2024-04-23 13:18:25.000000 ingeniamotion-0.8.0/tests/test_feedback_test.py
+-rw-rw-rw-   0        0        0    17939 2024-04-23 13:18:25.000000 ingeniamotion-0.8.0/tests/test_feedbacks.py
+-rw-rw-rw-   0        0        0    10468 2024-04-23 13:18:25.000000 ingeniamotion-0.8.0/tests/test_homing.py
+-rw-rw-rw-   0        0        0     8404 2024-04-23 13:18:25.000000 ingeniamotion-0.8.0/tests/test_information.py
+-rw-rw-rw-   0        0        0    15648 2024-04-23 13:18:25.000000 ingeniamotion-0.8.0/tests/test_monitoring.py
+-rw-rw-rw-   0        0        0    17833 2024-04-23 13:18:25.000000 ingeniamotion-0.8.0/tests/test_motion.py
+-rw-rw-rw-   0        0        0     3785 2024-04-23 13:18:25.000000 ingeniamotion-0.8.0/tests/test_motion_controller.py
+-rw-rw-rw-   0        0        0    12713 2024-04-23 13:18:25.000000 ingeniamotion-0.8.0/tests/test_pdo.py
```

### Comparing `ingeniamotion-0.7.1/LICENSE.md` & `ingeniamotion-0.8.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ingeniamotion-0.7.1/PKG-INFO` & `ingeniamotion-0.8.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: ingeniamotion
-Version: 0.7.1
+Version: 0.8.0
 Summary: Motion library for Ingenia servo drives
 Home-page: https://www.ingeniamc.com
 Author: Ingenia Motion Control
 Author-email: support@ingeniamc.com
-Project-URL: Documentation, https://distext.ingeniamc.com/doc/ingeniamotion/0.7.1
+Project-URL: Documentation, https://distext.ingeniamc.com/doc/ingeniamotion/0.8.0
 Project-URL: Source, https://github.com/ingeniamc/ingeniamotion
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.md
-Requires-Dist: ingenialink<8.0.0,>=7.2.0
+Requires-Dist: ingenialink<8.0.0,>=7.3.0
 Requires-Dist: ingenialogger>=0.2.1
 Requires-Dist: ifaddr==0.1.7
 
 What is Ingeniamotion?
 ======================
 
 Ingeniamotion is a library that works over ingenialink and aims to simplify the interaction with Ingenia's drives.
```

### Comparing `ingeniamotion-0.7.1/README.md` & `ingeniamotion-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `ingeniamotion-0.7.1/docs/what_is_ingeniamotion.rst` & `ingeniamotion-0.8.0/docs/what_is_ingeniamotion.rst`

 * *Files identical despite different names*

### Comparing `ingeniamotion-0.7.1/ingeniamotion/capture.py` & `ingeniamotion-0.8.0/ingeniamotion/capture.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,32 @@
 from typing import TYPE_CHECKING, Dict, List, Optional, Union
 
 import numpy as np
+from numpy.typing import NDArray
 from ingenialink.exceptions import ILIOError
 from ingenialink.poller import Poller
-from numpy.typing import NDArray
+from ingenialink.dictionary import SubnodeType
 
 from ingeniamotion.disturbance import Disturbance
 from ingeniamotion.enums import (
     MonitoringProcessStage,
     MonitoringSoCConfig,
     MonitoringSoCType,
     MonitoringVersion,
 )
-from ingeniamotion.exceptions import IMMonitoringError, IMRegisterNotExist, IMStatusWordError
+from ingeniamotion.exceptions import (
+    IMMonitoringError,
+    IMRegisterNotExist,
+    IMStatusWordError,
+)
 from ingeniamotion.metaclass import DEFAULT_AXIS, DEFAULT_SERVO, MCMetaClass
 from ingeniamotion.monitoring.base_monitoring import Monitoring
 from ingeniamotion.monitoring.monitoring_v1 import MonitoringV1
 from ingeniamotion.monitoring.monitoring_v3 import MonitoringV3
+from ingeniamotion.pdo import PDONetworkManager
 
 if TYPE_CHECKING:
     from ingeniamotion.motion_controller import MotionController
 
 
 class Capture(metaclass=MCMetaClass):
     """Capture."""
@@ -48,14 +54,15 @@
         MonitoringVersion.MONITORING_V1: 0x800,
         MonitoringVersion.MONITORING_V2: 0x800,
         MonitoringVersion.MONITORING_V3: 0x10,
     }
 
     def __init__(self, motion_controller: "MotionController") -> None:
         self.mc = motion_controller
+        self.pdo = PDONetworkManager(self.mc)
 
     def create_poller(
         self,
         registers: List[Dict[str, Union[int, str]]],
         servo: str = DEFAULT_SERVO,
         sampling_time: float = 0.125,
         buffer_size: int = 100,
@@ -625,17 +632,20 @@
         Args:
             servo : servo alias to reference it. ``default`` by default.
 
         Raises:
             IMStatusWordError: If motor is enabled.
 
         """
-        subnodes = self.mc.info.get_subnodes(servo)
-        for axis in range(1, subnodes):
-            if self.mc.configuration.is_motor_enabled(servo=servo, axis=axis):
+        for subnode in [
+            subnode
+            for subnode, subnode_type in self.mc.info.get_subnodes(servo).items()
+            if subnode_type == SubnodeType.MOTION
+        ]:
+            if self.mc.configuration.is_motor_enabled(servo=servo, axis=subnode):
                 raise IMStatusWordError("Motor is enabled")
         self.enable_monitoring(servo=servo)
         self.disable_monitoring(servo=servo)
 
     def disturbance_max_sample_size(self, servo: str = DEFAULT_SERVO) -> int:
         """Return disturbance max size, in bytes.
```

### Comparing `ingeniamotion-0.7.1/ingeniamotion/configuration.py` & `ingeniamotion-0.8.0/ingeniamotion/configuration.py`

 * *Files identical despite different names*

### Comparing `ingeniamotion-0.7.1/ingeniamotion/disturbance.py` & `ingeniamotion-0.8.0/ingeniamotion/disturbance.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from functools import wraps
 from typing import TYPE_CHECKING, Callable, Dict, List, Optional, Union
 
 import ingenialogger
 import numpy as np
-from ingenialink.enums.register import REG_DTYPE
+from ingenialink.enums.register import REG_DTYPE, RegCyclicType
 from ingenialink.exceptions import ILValueError
 from numpy import ndarray
 from numpy.typing import ArrayLike, NDArray
 
 from ingeniamotion.enums import MonitoringVersion
 from ingeniamotion.exceptions import IMDisturbanceError, IMStatusWordError
 from ingeniamotion.metaclass import DEFAULT_AXIS, DEFAULT_SERVO
@@ -46,16 +46,14 @@
         servo : servo alias to reference it. ``default`` by default.
     """
 
     DISTURBANCE_FREQUENCY_DIVIDER_REGISTER = "DIST_FREQ_DIV"
     DISTURBANCE_MAXIMUM_SAMPLE_SIZE_REGISTER = "DIST_MAX_SIZE"
     MONITORING_DISTURBANCE_STATUS_REGISTER = "MON_DIST_STATUS"
 
-    CYCLIC_RX = "CYCLIC_RX"
-
     DISTURBANCE_STATUS_ENABLED_BIT = 0x1000  # TODO: Not implemented yet
     MONITORING_STATUS_ENABLED_BIT = 0x1
     REGISTER_MAP_OFFSET = 0x800
 
     __data_type_size = {
         REG_DTYPE.U8: 1,
         REG_DTYPE.S8: 1,
@@ -153,15 +151,15 @@
                 raise TypeError("Subnode value has to be an integer")
             register = channel["name"]
             if not isinstance(register, str):
                 raise TypeError("Register key has to be a string")
             register_obj = self.mc.info.register_info(register, subnode, servo=self.servo)
             dtype = register_obj.dtype
             cyclic = register_obj.cyclic
-            if cyclic != self.CYCLIC_RX:
+            if cyclic != RegCyclicType.RX:
                 drive.disturbance_remove_all_mapped_registers()
                 raise IMDisturbanceError(
                     "{} can not be mapped as a disturbance register".format(register)
                 )
             channel["dtype"] = dtype
             drive.disturbance_set_mapped_register(
                 ch_idx,
```

### Comparing `ingeniamotion-0.7.1/ingeniamotion/drive_tests.py` & `ingeniamotion-0.8.0/ingeniamotion/drive_tests.py`

 * *Files identical despite different names*

### Comparing `ingeniamotion-0.7.1/ingeniamotion/enums/__init__.py` & `ingeniamotion-0.8.0/ingeniamotion/enums/__init__.py`

 * *Files identical despite different names*

### Comparing `ingeniamotion-0.7.1/ingeniamotion/errors.py` & `ingeniamotion-0.8.0/ingeniamotion/errors.py`

 * *Files identical despite different names*

### Comparing `ingeniamotion-0.7.1/ingeniamotion/exceptions.py` & `ingeniamotion-0.8.0/ingeniamotion/exceptions.py`

 * *Files identical despite different names*

### Comparing `ingeniamotion-0.7.1/ingeniamotion/feedbacks.py` & `ingeniamotion-0.8.0/ingeniamotion/feedbacks.py`

 * *Files identical despite different names*

### Comparing `ingeniamotion-0.7.1/ingeniamotion/homing.py` & `ingeniamotion-0.8.0/ingeniamotion/homing.py`

 * *Files identical despite different names*

### Comparing `ingeniamotion-0.7.1/ingeniamotion/information.py` & `ingeniamotion-0.8.0/ingeniamotion/information.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 import os
 from typing import TYPE_CHECKING, Dict, Optional, Tuple, Union
 
+from ingenialink import CAN_BAUDRATE
 from ingenialink.eoe.network import EoENetwork
 from ingenialink.ethernet.network import EthernetNetwork
 from ingenialink.canopen.network import CanopenNetwork
 from ingenialink.ethercat.network import EthercatNetwork
 from ingenialink.register import Register
 from ingenialink.enums.register import REG_ACCESS, REG_DTYPE
+from ingenialink.dictionary import SubnodeType
 import ingenialogger
 
 from ingeniamotion.exceptions import IMRegisterNotExist, IMException
 from ingeniamotion.metaclass import MCMetaClass, DEFAULT_AXIS, DEFAULT_SERVO
 from ingeniamotion.enums import COMMUNICATION_TYPE
-from ingeniamotion.comkit import create_comkit_dictionary
 
 
 if TYPE_CHECKING:
     from ingeniamotion.motion_controller import MotionController
 
 logger = ingenialogger.get_logger(__name__)
 
@@ -140,35 +141,14 @@
         Returns:
             ``True`` if register exists, else ``False``.
 
         """
         drive = self.mc.servos[servo]
         return register in drive.dictionary.registers(axis)
 
-    @staticmethod
-    def create_comkit_dictionary(
-        coco_dict_path: str, moco_dict_path: str, dest_file: Optional[str] = None
-    ) -> str:
-        """Create a dictionary for COMKIT by merging a COCO dictionary and a MOCO dictionary.
-
-        Args:
-            coco_dict_path : COCO dictionary path.
-            moco_dict_path : MOCO dictionary path.
-            dest_file: Path to store the COMKIT dictionary. If it's not provided the
-                merged dictionary is stored in the temporary system's folder.
-
-        Returns:
-            Path to the COMKIT dictionary.
-
-        Raises:
-            ValueError: If destination file has a wrong extension.
-
-        """
-        return create_comkit_dictionary(coco_dict_path, moco_dict_path, dest_file)
-
     def get_product_name(self, alias: str = DEFAULT_SERVO) -> Optional[str]:
         """Get the product name of the drive.
 
         Args:
             alias: alias of the servo.
 
         Returns:
@@ -192,14 +172,28 @@
         net = self.mc._get_network(alias)
         drive = self.mc.servos[alias]
         if isinstance(net, CanopenNetwork):
             return int(drive.target)
         else:
             raise IMException("You need a CANopen communication to use this function")
 
+    def get_baudrate(self, alias: str = DEFAULT_SERVO) -> CAN_BAUDRATE:
+        """Get the baudrate of target servo
+
+        Args:
+            alias: alias of the servo.
+
+        Returns:
+            Baudrate of the drive.
+        """
+        net = self.mc._get_network(alias)
+        if isinstance(net, CanopenNetwork):
+            return CAN_BAUDRATE(net.baudrate)
+        raise IMException(f"The servo {alias} is not a CANopen device.")
+
     def get_ip(self, alias: str = DEFAULT_SERVO) -> str:
         """Get the IP for Ethernet communications.
 
         Args:
             alias: alias of the servo.
 
         Returns:
@@ -273,25 +267,25 @@
         full_name = f"{prod_name} - {name}"
         net = self.mc._get_network(alias)
         if isinstance(net, EthernetNetwork):
             ip = self.get_ip(alias)
             full_name = f"{full_name} ({ip})"
         return full_name
 
-    def get_subnodes(self, alias: str = DEFAULT_SERVO) -> int:
-        """Return the number of subnodes.
+    def get_subnodes(self, alias: str = DEFAULT_SERVO) -> Dict[int, SubnodeType]:
+        """Return a dictionary with the subnodes IDs as keys and their type as values.
 
         Args:
             alias: Drive alias.
 
         Returns:
-            Number of subnodes.
+            Dictionary of subnode ids and their type.
         """
         drive = self.mc.servos[alias]
-        return int(drive.subnodes)
+        return drive.subnodes
 
     def get_categories(self, alias: str) -> Dict[str, str]:
         """Return dictionary categories instance.
 
         Args:
             alias: Drive alias.
 
@@ -316,24 +310,18 @@
 
         Returns:
             Dictionary file name.
         """
         drive = self.mc.servos[alias]
         return str(os.path.basename(drive.dictionary.path))
 
-    def get_encoded_image_from_dictionary(self, alias: str, axis: int = 0) -> Optional[str]:
+    def get_encoded_image_from_dictionary(self, alias: str) -> Optional[str]:
         """Get the encoded product image from a drive dictionary.
         This function reads a dictionary of a drive, and it parses whether the dictionary file has a
         DriveImage tag and its content.
         Args:
             alias: Alias of the drive.
-            axis: Drive axis. Used when using  COM-KIT.
         Returns:
             The encoded image or NoneType object.
         """
         drive = self.mc.servos[alias]
-        encoded_image: Optional[str] = None
-        if axis == 1:
-            encoded_image = drive.dictionary.moco_image
-        else:
-            encoded_image = drive.dictionary.image
-        return encoded_image
+        return drive.dictionary.image
```

### Comparing `ingeniamotion-0.7.1/ingeniamotion/metaclass.py` & `ingeniamotion-0.8.0/ingeniamotion/metaclass.py`

 * *Files identical despite different names*

### Comparing `ingeniamotion-0.7.1/ingeniamotion/monitoring/base_monitoring.py` & `ingeniamotion-0.8.0/ingeniamotion/monitoring/base_monitoring.py`

 * *Files identical despite different names*

### Comparing `ingeniamotion-0.7.1/ingeniamotion/monitoring/monitoring_v1.py` & `ingeniamotion-0.8.0/ingeniamotion/monitoring/monitoring_v1.py`

 * *Files identical despite different names*

### Comparing `ingeniamotion-0.7.1/ingeniamotion/monitoring/monitoring_v3.py` & `ingeniamotion-0.8.0/ingeniamotion/monitoring/monitoring_v3.py`

 * *Files identical despite different names*

### Comparing `ingeniamotion-0.7.1/ingeniamotion/motion.py` & `ingeniamotion-0.8.0/ingeniamotion/motion.py`

 * *Files identical despite different names*

### Comparing `ingeniamotion-0.7.1/ingeniamotion/motion_controller.py` & `ingeniamotion-0.8.0/ingeniamotion/motion_controller.py`

 * *Files identical despite different names*

### Comparing `ingeniamotion-0.7.1/ingeniamotion/wizard_tests/base_test.py` & `ingeniamotion-0.8.0/ingeniamotion/wizard_tests/base_test.py`

 * *Files identical despite different names*

### Comparing `ingeniamotion-0.7.1/ingeniamotion/wizard_tests/brake.py` & `ingeniamotion-0.8.0/ingeniamotion/wizard_tests/brake.py`

 * *Files identical despite different names*

### Comparing `ingeniamotion-0.7.1/ingeniamotion/wizard_tests/brake_tune.py` & `ingeniamotion-0.8.0/ingeniamotion/wizard_tests/brake_tune.py`

 * *Files identical despite different names*

### Comparing `ingeniamotion-0.7.1/ingeniamotion/wizard_tests/feedbacks_tests/absolute_encoder1_test.py` & `ingeniamotion-0.8.0/ingeniamotion/wizard_tests/feedbacks_tests/absolute_encoder1_test.py`

 * *Files identical despite different names*

### Comparing `ingeniamotion-0.7.1/ingeniamotion/wizard_tests/feedbacks_tests/absolute_encoder2_test.py` & `ingeniamotion-0.8.0/ingeniamotion/wizard_tests/feedbacks_tests/absolute_encoder2_test.py`

 * *Files identical despite different names*

### Comparing `ingeniamotion-0.7.1/ingeniamotion/wizard_tests/feedbacks_tests/dc_feedback_polarity_test.py` & `ingeniamotion-0.8.0/ingeniamotion/wizard_tests/feedbacks_tests/dc_feedback_polarity_test.py`

 * *Files identical despite different names*

### Comparing `ingeniamotion-0.7.1/ingeniamotion/wizard_tests/feedbacks_tests/dc_feedback_resolution_test.py` & `ingeniamotion-0.8.0/ingeniamotion/wizard_tests/feedbacks_tests/dc_feedback_resolution_test.py`

 * *Files identical despite different names*

### Comparing `ingeniamotion-0.7.1/ingeniamotion/wizard_tests/feedbacks_tests/digital_hall_test.py` & `ingeniamotion-0.8.0/ingeniamotion/wizard_tests/feedbacks_tests/digital_hall_test.py`

 * *Files identical despite different names*

### Comparing `ingeniamotion-0.7.1/ingeniamotion/wizard_tests/feedbacks_tests/digital_incremental1_test.py` & `ingeniamotion-0.8.0/ingeniamotion/wizard_tests/feedbacks_tests/digital_incremental1_test.py`

 * *Files identical despite different names*

### Comparing `ingeniamotion-0.7.1/ingeniamotion/wizard_tests/feedbacks_tests/digital_incremental2_test.py` & `ingeniamotion-0.8.0/ingeniamotion/wizard_tests/feedbacks_tests/digital_incremental2_test.py`

 * *Files identical despite different names*

### Comparing `ingeniamotion-0.7.1/ingeniamotion/wizard_tests/feedbacks_tests/feedback_test.py` & `ingeniamotion-0.8.0/ingeniamotion/wizard_tests/feedbacks_tests/feedback_test.py`

 * *Files identical despite different names*

### Comparing `ingeniamotion-0.7.1/ingeniamotion/wizard_tests/feedbacks_tests/secondary_ssi_test.py` & `ingeniamotion-0.8.0/ingeniamotion/wizard_tests/feedbacks_tests/secondary_ssi_test.py`

 * *Files identical despite different names*

### Comparing `ingeniamotion-0.7.1/ingeniamotion/wizard_tests/phase_calibration.py` & `ingeniamotion-0.8.0/ingeniamotion/wizard_tests/phase_calibration.py`

 * *Files identical despite different names*

### Comparing `ingeniamotion-0.7.1/ingeniamotion/wizard_tests/phasing_check.py` & `ingeniamotion-0.8.0/ingeniamotion/wizard_tests/phasing_check.py`

 * *Files identical despite different names*

### Comparing `ingeniamotion-0.7.1/ingeniamotion/wizard_tests/sto.py` & `ingeniamotion-0.8.0/ingeniamotion/wizard_tests/sto.py`

 * *Files identical despite different names*

### Comparing `ingeniamotion-0.7.1/ingeniamotion/wizard_tests/stoppable.py` & `ingeniamotion-0.8.0/ingeniamotion/wizard_tests/stoppable.py`

 * *Files identical despite different names*

### Comparing `ingeniamotion-0.7.1/ingeniamotion.egg-info/PKG-INFO` & `ingeniamotion-0.8.0/ingeniamotion.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: ingeniamotion
-Version: 0.7.1
+Version: 0.8.0
 Summary: Motion library for Ingenia servo drives
 Home-page: https://www.ingeniamc.com
 Author: Ingenia Motion Control
 Author-email: support@ingeniamc.com
-Project-URL: Documentation, https://distext.ingeniamc.com/doc/ingeniamotion/0.7.1
+Project-URL: Documentation, https://distext.ingeniamc.com/doc/ingeniamotion/0.8.0
 Project-URL: Source, https://github.com/ingeniamc/ingeniamotion
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.md
-Requires-Dist: ingenialink<8.0.0,>=7.2.0
+Requires-Dist: ingenialink<8.0.0,>=7.3.0
 Requires-Dist: ingenialogger>=0.2.1
 Requires-Dist: ifaddr==0.1.7
 
 What is Ingeniamotion?
 ======================
 
 Ingeniamotion is a library that works over ingenialink and aims to simplify the interaction with Ingenia's drives.
```

### Comparing `ingeniamotion-0.7.1/ingeniamotion.egg-info/SOURCES.txt` & `ingeniamotion-0.8.0/ingeniamotion.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 LICENSE.md
 MANIFEST.in
 README.md
 setup.py
 docs/what_is_ingeniamotion.rst
 ingeniamotion/__init__.py
 ingeniamotion/capture.py
-ingeniamotion/comkit.py
 ingeniamotion/communication.py
 ingeniamotion/configuration.py
 ingeniamotion/disturbance.py
 ingeniamotion/drive_tests.py
 ingeniamotion/errors.py
 ingeniamotion/exceptions.py
 ingeniamotion/feedbacks.py
 ingeniamotion/homing.py
 ingeniamotion/information.py
 ingeniamotion/metaclass.py
 ingeniamotion/motion.py
 ingeniamotion/motion_controller.py
+ingeniamotion/pdo.py
 ingeniamotion/py.typed
 ingeniamotion.egg-info/PKG-INFO
 ingeniamotion.egg-info/SOURCES.txt
 ingeniamotion.egg-info/dependency_links.txt
 ingeniamotion.egg-info/requires.txt
 ingeniamotion.egg-info/top_level.txt
 ingeniamotion/enums/__init__.py
@@ -48,20 +48,20 @@
 ingeniamotion/wizard_tests/feedbacks_tests/feedback_test.py
 ingeniamotion/wizard_tests/feedbacks_tests/secondary_ssi_test.py
 tests/__init__.py
 tests/conftest.py
 tests/load_FWs.py
 tests/test_all_drive_tests.py
 tests/test_capture.py
-tests/test_comkit.py
 tests/test_communication.py
 tests/test_configuration.py
 tests/test_disturbance.py
 tests/test_errors.py
 tests/test_examples.py
 tests/test_feedback_test.py
 tests/test_feedbacks.py
 tests/test_homing.py
 tests/test_information.py
 tests/test_monitoring.py
 tests/test_motion.py
-tests/test_motion_controller.py
+tests/test_motion_controller.py
+tests/test_pdo.py
```

### Comparing `ingeniamotion-0.7.1/setup.py` & `ingeniamotion-0.8.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,13 +30,13 @@
         "Source": "https://github.com/ingeniamc/ingeniamotion",
     },
     classifiers=[
         "Programming Language :: Python :: 3",
         "Operating System :: OS Independent",
     ],
     install_requires=[
-        "ingenialink>=7.2.0, < 8.0.0",
+        "ingenialink>=7.3.0, < 8.0.0",
         "ingenialogger>=0.2.1",
         "ifaddr==0.1.7",
     ],
     python_requires=">=3.9",
 )
```

### Comparing `ingeniamotion-0.7.1/tests/conftest.py` & `ingeniamotion-0.8.0/tests/conftest.py`

 * *Files 0% similar despite different names*

```diff
@@ -86,14 +86,15 @@
         virtual_drive = VirtualDrive(read_config["port"], read_config["dictionary"])
         virtual_drive.start()
         connect_eoe(mc, read_config, alias)
     else:
         connect_eoe(mc, read_config, alias)
 
     if protocol != "virtual":
+        mc.configuration.restore_configuration(servo=alias)
         mc.configuration.load_configuration(read_config["config_file"], servo=alias)
         yield mc, alias
         mc.communication.disconnect(alias)
     else:
         yield mc, alias
         virtual_drive.stop()
```

### Comparing `ingeniamotion-0.7.1/tests/load_FWs.py` & `ingeniamotion-0.8.0/tests/load_FWs.py`

 * *Files identical despite different names*

### Comparing `ingeniamotion-0.7.1/tests/test_all_drive_tests.py` & `ingeniamotion-0.8.0/tests/test_all_drive_tests.py`

 * *Files identical despite different names*

### Comparing `ingeniamotion-0.7.1/tests/test_capture.py` & `ingeniamotion-0.8.0/tests/test_capture.py`

 * *Files identical despite different names*

### Comparing `ingeniamotion-0.7.1/tests/test_configuration.py` & `ingeniamotion-0.8.0/tests/test_configuration.py`

 * *Files identical despite different names*

### Comparing `ingeniamotion-0.7.1/tests/test_disturbance.py` & `ingeniamotion-0.8.0/tests/test_disturbance.py`

 * *Files identical despite different names*

### Comparing `ingeniamotion-0.7.1/tests/test_errors.py` & `ingeniamotion-0.8.0/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `ingeniamotion-0.7.1/tests/test_feedback_test.py` & `ingeniamotion-0.8.0/tests/test_feedback_test.py`

 * *Files identical despite different names*

### Comparing `ingeniamotion-0.7.1/tests/test_feedbacks.py` & `ingeniamotion-0.8.0/tests/test_feedbacks.py`

 * *Files identical despite different names*

### Comparing `ingeniamotion-0.7.1/tests/test_homing.py` & `ingeniamotion-0.8.0/tests/test_homing.py`

 * *Files identical despite different names*

### Comparing `ingeniamotion-0.7.1/tests/test_information.py` & `ingeniamotion-0.8.0/tests/test_information.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pytest
 
 from ingenialink.ethercat.network import EthercatNetwork
 from ingenialink.ethernet.network import EthernetNetwork
-from ingenialink.canopen.network import CanopenNetwork
-from ingenialink.canopen import CAN_DEVICE
+from ingenialink.canopen.network import CanopenNetwork, CAN_DEVICE, CAN_BAUDRATE
+from ingenialink.dictionary import SubnodeType
 
 from ingeniamotion.enums import REG_DTYPE, REG_ACCESS
 from ingeniamotion.information import COMMUNICATION_TYPE
 from ingeniamotion.exceptions import IMRegisterNotExist, IMException
 
 
 @pytest.mark.virtual
@@ -164,15 +164,17 @@
 @pytest.mark.virtual
 def test_get_subnodes(motion_controller):
     expected_subnodes = 2
 
     mc, alias = motion_controller
     subnodes = mc.info.get_subnodes(alias)
 
-    assert subnodes == expected_subnodes
+    assert len(subnodes) == expected_subnodes
+    assert subnodes[0] == SubnodeType.COMMUNICATION
+    assert subnodes[1] == SubnodeType.MOTION
 
 
 @pytest.mark.virtual
 def test_get_categories(motion_controller):
     expected_number_categories = 19
 
     mc, alias = motion_controller
@@ -233,7 +235,34 @@
 
 
 @pytest.mark.virtual
 def test_get_slave_id_exception(motion_controller):
     mc, alias = motion_controller
     with pytest.raises(IMException):
         mc.info.get_slave_id(alias)
+
+
+@pytest.mark.virtual
+def test_get_baudrate_success(motion_controller, mocker):
+    mc, _ = motion_controller
+
+    fake_device = CAN_DEVICE.PCAN
+    fake_channel = 0
+    fake_baudrate = CAN_BAUDRATE.Baudrate_1M
+    fake_network = CanopenNetwork(fake_device, fake_channel, fake_baudrate)
+    mocker.patch.object(mc, "_get_network", return_value=fake_network)
+
+    test_baudrate = mc.info.get_baudrate()
+
+    assert fake_baudrate == test_baudrate
+
+
+@pytest.mark.virtual
+def test_get_baudrate_failed(motion_controller, mocker):
+    mc, _ = motion_controller
+
+    mocker.patch.object(mc, "_get_network", return_value=EthercatNetwork("fake_interface_name"))
+    with pytest.raises(IMException) as imexpeption_info:
+        _ = mc.info.get_baudrate()
+
+    expected_message_error = "The servo default is not a CANopen device."
+    assert expected_message_error == imexpeption_info.value.args[0]
```

### Comparing `ingeniamotion-0.7.1/tests/test_monitoring.py` & `ingeniamotion-0.8.0/tests/test_monitoring.py`

 * *Files identical despite different names*

### Comparing `ingeniamotion-0.7.1/tests/test_motion.py` & `ingeniamotion-0.8.0/tests/test_motion.py`

 * *Files identical despite different names*

### Comparing `ingeniamotion-0.7.1/tests/test_motion_controller.py` & `ingeniamotion-0.8.0/tests/test_motion_controller.py`

 * *Files identical despite different names*


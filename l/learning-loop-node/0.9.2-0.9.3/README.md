# Comparing `tmp/learning_loop_node-0.9.2.tar.gz` & `tmp/learning_loop_node-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "learning_loop_node-0.9.2.tar", max compression
+gzip compressed data, was "learning_loop_node-0.9.3.tar", max compression
```

## Comparing `learning_loop_node-0.9.2.tar` & `learning_loop_node-0.9.3.tar`

### file list

```diff
@@ -1,87 +1,88 @@
--rw-r--r--   0        0        0     7501 2024-02-02 16:38:43.916515 learning_loop_node-0.9.2/README.md
--rw-r--r--   0        0        0      366 2024-02-02 16:38:43.916515 learning_loop_node-0.9.2/learning_loop_node/__init__.py
--rw-r--r--   0        0        0        0 2024-02-02 16:38:43.916515 learning_loop_node-0.9.2/learning_loop_node/annotation/__init__.py
--rw-r--r--   0        0        0      984 2024-02-02 16:38:43.916515 learning_loop_node-0.9.2/learning_loop_node/annotation/annotator_logic.py
--rw-r--r--   0        0        0     4055 2024-02-02 16:38:43.916515 learning_loop_node-0.9.2/learning_loop_node/annotation/annotator_node.py
--rw-r--r--   0        0        0     2065 2024-02-02 16:38:43.916515 learning_loop_node-0.9.2/learning_loop_node/annotation/tests/test_annotator_node.py
--rw-r--r--   0        0        0     3492 2024-02-02 16:38:43.916515 learning_loop_node-0.9.2/learning_loop_node/conftest.py
--rw-r--r--   0        0        0        0 2024-02-02 16:38:43.916515 learning_loop_node-0.9.2/learning_loop_node/converter/__init__.py
--rw-r--r--   0        0        0     2534 2024-02-02 16:38:43.916515 learning_loop_node-0.9.2/learning_loop_node/converter/converter_logic.py
--rw-r--r--   0        0        0     4932 2024-02-02 16:38:43.916515 learning_loop_node-0.9.2/learning_loop_node/converter/converter_node.py
--rw-r--r--   0        0        0     2207 2024-02-02 16:38:43.916515 learning_loop_node-0.9.2/learning_loop_node/converter/tests/test_converter.py
--rw-r--r--   0        0        0      783 2024-02-02 16:38:43.916515 learning_loop_node-0.9.2/learning_loop_node/data_classes/__init__.py
--rw-r--r--   0        0        0     1211 2024-02-02 16:38:43.916515 learning_loop_node-0.9.2/learning_loop_node/data_classes/annotations.py
--rw-r--r--   0        0        0     4115 2024-02-02 16:38:43.916515 learning_loop_node-0.9.2/learning_loop_node/data_classes/detections.py
--rw-r--r--   0        0        0     4635 2024-02-02 16:38:43.916515 learning_loop_node-0.9.2/learning_loop_node/data_classes/general.py
--rw-r--r--   0        0        0      655 2024-02-02 16:38:43.916515 learning_loop_node-0.9.2/learning_loop_node/data_classes/socket_response.py
--rw-r--r--   0        0        0     4870 2024-02-02 16:38:43.916515 learning_loop_node-0.9.2/learning_loop_node/data_classes/training.py
--rw-r--r--   0        0        0    10346 2024-02-02 16:38:43.916515 learning_loop_node-0.9.2/learning_loop_node/data_exchanger.py
--rw-r--r--   0        0        0        1 2024-02-02 16:38:43.916515 learning_loop_node-0.9.2/learning_loop_node/detector/__init__.py
--rw-r--r--   0        0        0     1741 2024-02-02 16:38:43.916515 learning_loop_node-0.9.2/learning_loop_node/detector/detector_logic.py
--rw-r--r--   0        0        0    16559 2024-02-02 16:38:43.916515 learning_loop_node-0.9.2/learning_loop_node/detector/detector_node.py
--rw-r--r--   0        0        0        0 2024-02-02 16:38:43.916515 learning_loop_node-0.9.2/learning_loop_node/detector/inbox_filter/__init__.py
--rw-r--r--   0        0        0     3437 2024-02-02 16:38:43.916515 learning_loop_node-0.9.2/learning_loop_node/detector/inbox_filter/cam_observation_history.py
--rw-r--r--   0        0        0     1011 2024-02-02 16:38:43.916515 learning_loop_node-0.9.2/learning_loop_node/detector/inbox_filter/relevance_filter.py
--rw-r--r--   0        0        0     1385 2024-02-02 16:38:43.916515 learning_loop_node-0.9.2/learning_loop_node/detector/inbox_filter/tests/test_observation.py
--rw-r--r--   0        0        0     7865 2024-02-02 16:38:43.916515 learning_loop_node-0.9.2/learning_loop_node/detector/inbox_filter/tests/test_relevance_group.py
--rw-r--r--   0        0        0     1804 2024-02-02 16:38:43.916515 learning_loop_node-0.9.2/learning_loop_node/detector/inbox_filter/tests/test_unexpected_observations_count.py
--rw-r--r--   0        0        0     4296 2024-02-02 16:38:43.916515 learning_loop_node-0.9.2/learning_loop_node/detector/outbox.py
--rw-r--r--   0        0        0        0 2024-02-02 16:38:43.916515 learning_loop_node-0.9.2/learning_loop_node/detector/rest/__init__.py
--rw-r--r--   0        0        0     1725 2024-02-02 16:38:43.916515 learning_loop_node-0.9.2/learning_loop_node/detector/rest/backdoor_controls.py
--rw-r--r--   0        0        0     1873 2024-02-02 16:38:43.916515 learning_loop_node-0.9.2/learning_loop_node/detector/rest/detect.py
--rw-r--r--   0        0        0     1664 2024-02-02 16:38:43.916515 learning_loop_node-0.9.2/learning_loop_node/detector/rest/operation_mode.py
--rw-r--r--   0        0        0      435 2024-02-02 16:38:43.916515 learning_loop_node-0.9.2/learning_loop_node/detector/rest/upload.py
--rw-r--r--   0        0        0        0 2024-02-02 16:38:43.916515 learning_loop_node-0.9.2/learning_loop_node/detector/tests/__init__.py
--rw-r--r--   0        0        0     3132 2024-02-02 16:38:43.916515 learning_loop_node-0.9.2/learning_loop_node/detector/tests/conftest.py
--rw-r--r--   0        0        0   161390 2024-02-02 16:38:43.916515 learning_loop_node-0.9.2/learning_loop_node/detector/tests/test.jpg
--rw-r--r--   0        0        0     3871 2024-02-02 16:38:43.916515 learning_loop_node-0.9.2/learning_loop_node/detector/tests/test_client_communication.py
--rw-r--r--   0        0        0     2011 2024-02-02 16:38:43.916515 learning_loop_node-0.9.2/learning_loop_node/detector/tests/test_outbox.py
--rw-r--r--   0        0        0     1981 2024-02-02 16:38:43.916515 learning_loop_node-0.9.2/learning_loop_node/detector/tests/test_relevance_filter.py
--rw-r--r--   0        0        0     1032 2024-02-02 16:38:43.916515 learning_loop_node-0.9.2/learning_loop_node/detector/tests/testing_detector.py
--rw-r--r--   0        0        0     2038 2024-02-02 16:38:43.916515 learning_loop_node-0.9.2/learning_loop_node/examples/novelty_score_updater.py
--rw-r--r--   0        0        0      165 2024-02-02 16:38:43.916515 learning_loop_node-0.9.2/learning_loop_node/globals.py
--rw-r--r--   0        0        0        0 2024-02-02 16:38:43.916515 learning_loop_node-0.9.2/learning_loop_node/helpers/__init__.py
--rw-r--r--   0        0        0     1543 2024-02-02 16:38:43.916515 learning_loop_node-0.9.2/learning_loop_node/helpers/environment_reader.py
--rwxr-xr-x   0        0        0     1129 2024-02-02 16:38:43.916515 learning_loop_node-0.9.2/learning_loop_node/helpers/gdrive_downloader.py
--rw-r--r--   0        0        0      824 2024-02-02 16:38:43.916515 learning_loop_node-0.9.2/learning_loop_node/helpers/log_conf.py
--rw-r--r--   0        0        0     4153 2024-02-02 16:38:43.920515 learning_loop_node-0.9.2/learning_loop_node/helpers/misc.py
--rw-r--r--   0        0        0     4730 2024-02-02 16:38:43.920515 learning_loop_node-0.9.2/learning_loop_node/loop_communication.py
--rw-r--r--   0        0        0     9793 2024-02-02 16:38:43.920515 learning_loop_node-0.9.2/learning_loop_node/node.py
--rw-r--r--   0        0        0      262 2024-02-02 16:38:43.920515 learning_loop_node-0.9.2/learning_loop_node/pytest.ini
--rw-r--r--   0        0        0        0 2024-02-02 16:38:43.920515 learning_loop_node-0.9.2/learning_loop_node/tests/__init__.py
--rw-r--r--   0        0        0      920 2024-02-02 16:38:43.920515 learning_loop_node-0.9.2/learning_loop_node/tests/conftest.py
--rw-r--r--   0        0        0       19 2024-02-02 16:38:43.920515 learning_loop_node-0.9.2/learning_loop_node/tests/test_data/file_1.txt
--rw-r--r--   0        0        0       19 2024-02-02 16:38:43.920515 learning_loop_node-0.9.2/learning_loop_node/tests/test_data/file_2.txt
--rw-r--r--   0        0        0      516 2024-02-02 16:38:43.920515 learning_loop_node-0.9.2/learning_loop_node/tests/test_data/model.json
--rw-r--r--   0        0        0      788 2024-02-02 16:38:43.920515 learning_loop_node-0.9.2/learning_loop_node/tests/test_data_classes.py
--rw-r--r--   0        0        0     2755 2024-02-02 16:38:43.920515 learning_loop_node-0.9.2/learning_loop_node/tests/test_downloader.py
--rw-r--r--   0        0        0     1948 2024-02-02 16:38:43.920515 learning_loop_node-0.9.2/learning_loop_node/tests/test_executor.py
--rw-r--r--   0        0        0     2412 2024-02-02 16:38:43.920515 learning_loop_node-0.9.2/learning_loop_node/tests/test_helper.py
--rw-r--r--   0        0        0      701 2024-02-02 16:38:43.920515 learning_loop_node-0.9.2/learning_loop_node/tests/test_learning_loop_node.py
--rw-r--r--   0        0        0        0 2024-02-02 16:38:43.920515 learning_loop_node-0.9.2/learning_loop_node/trainer/__init__.py
--rw-r--r--   0        0        0     1467 2024-02-02 16:38:43.920515 learning_loop_node-0.9.2/learning_loop_node/trainer/downloader.py
--rw-r--r--   0        0        0     3118 2024-02-02 16:38:43.920515 learning_loop_node-0.9.2/learning_loop_node/trainer/executor.py
--rw-r--r--   0        0        0     4419 2024-02-02 16:38:43.920515 learning_loop_node-0.9.2/learning_loop_node/trainer/io_helpers.py
--rw-r--r--   0        0        0        0 2024-02-02 16:38:43.920515 learning_loop_node-0.9.2/learning_loop_node/trainer/rest/__init__.py
--rw-r--r--   0        0        0     5635 2024-02-02 16:38:43.920515 learning_loop_node-0.9.2/learning_loop_node/trainer/rest/backdoor_controls.py
--rw-r--r--   0        0        0      897 2024-02-02 16:38:43.920515 learning_loop_node-0.9.2/learning_loop_node/trainer/rest/controls.py
--rw-r--r--   0        0        0        0 2024-02-02 16:38:43.920515 learning_loop_node-0.9.2/learning_loop_node/trainer/tests/__init__.py
--rw-r--r--   0        0        0     2829 2024-02-02 16:38:43.920515 learning_loop_node-0.9.2/learning_loop_node/trainer/tests/conftest.py
--rw-r--r--   0        0        0      934 2024-02-02 16:38:43.920515 learning_loop_node-0.9.2/learning_loop_node/trainer/tests/state_helper.py
--rw-r--r--   0        0        0        0 2024-02-02 16:38:43.920515 learning_loop_node-0.9.2/learning_loop_node/trainer/tests/states/__init__.py
--rw-r--r--   0        0        0     1310 2024-02-02 16:38:43.920515 learning_loop_node-0.9.2/learning_loop_node/trainer/tests/states/test_state_cleanup.py
--rw-r--r--   0        0        0     3608 2024-02-02 16:38:43.920515 learning_loop_node-0.9.2/learning_loop_node/trainer/tests/states/test_state_detecting.py
--rw-r--r--   0        0        0     2604 2024-02-02 16:38:43.920515 learning_loop_node-0.9.2/learning_loop_node/trainer/tests/states/test_state_download_train_model.py
--rw-r--r--   0        0        0     2233 2024-02-02 16:38:43.920515 learning_loop_node-0.9.2/learning_loop_node/trainer/tests/states/test_state_prepare.py
--rw-r--r--   0        0        0     4558 2024-02-02 16:38:43.920515 learning_loop_node-0.9.2/learning_loop_node/trainer/tests/states/test_state_sync_confusion_matrix.py
--rw-r--r--   0        0        0     3309 2024-02-02 16:38:43.920515 learning_loop_node-0.9.2/learning_loop_node/trainer/tests/states/test_state_train.py
--rw-r--r--   0        0        0     7202 2024-02-02 16:38:43.920515 learning_loop_node-0.9.2/learning_loop_node/trainer/tests/states/test_state_upload_detections.py
--rw-r--r--   0        0        0     3558 2024-02-02 16:38:43.920515 learning_loop_node-0.9.2/learning_loop_node/trainer/tests/states/test_state_upload_model.py
--rw-r--r--   0        0        0     1915 2024-02-02 16:38:43.920515 learning_loop_node-0.9.2/learning_loop_node/trainer/tests/test_errors.py
--rw-r--r--   0        0        0     1144 2024-02-02 16:38:43.920515 learning_loop_node-0.9.2/learning_loop_node/trainer/tests/test_trainer_states.py
--rw-r--r--   0        0        0     3957 2024-02-02 16:38:43.920515 learning_loop_node-0.9.2/learning_loop_node/trainer/tests/testing_trainer_logic.py
--rw-r--r--   0        0        0    33057 2024-02-02 16:38:43.920515 learning_loop_node-0.9.2/learning_loop_node/trainer/trainer_logic.py
--rw-r--r--   0        0        0     8018 2024-02-02 16:38:43.920515 learning_loop_node-0.9.2/learning_loop_node/trainer/trainer_node.py
--rw-r--r--   0        0        0     1884 2024-02-02 16:38:43.920515 learning_loop_node-0.9.2/learning_loop_node/trainer/training_syncronizer.py
--rw-r--r--   0        0        0     1148 2024-02-02 16:38:53.712512 learning_loop_node-0.9.2/pyproject.toml
--rw-r--r--   0        0        0     9157 1970-01-01 00:00:00.000000 learning_loop_node-0.9.2/PKG-INFO
+-rw-r--r--   0        0        0     7501 2024-02-12 10:34:30.589011 learning_loop_node-0.9.3/README.md
+-rw-r--r--   0        0        0      366 2024-02-12 10:34:30.589011 learning_loop_node-0.9.3/learning_loop_node/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-12 10:34:30.589011 learning_loop_node-0.9.3/learning_loop_node/annotation/__init__.py
+-rw-r--r--   0        0        0      984 2024-02-12 10:34:30.589011 learning_loop_node-0.9.3/learning_loop_node/annotation/annotator_logic.py
+-rw-r--r--   0        0        0     4055 2024-02-12 10:34:30.593011 learning_loop_node-0.9.3/learning_loop_node/annotation/annotator_node.py
+-rw-r--r--   0        0        0     2065 2024-02-12 10:34:30.593011 learning_loop_node-0.9.3/learning_loop_node/annotation/tests/test_annotator_node.py
+-rw-r--r--   0        0        0     3492 2024-02-12 10:34:30.593011 learning_loop_node-0.9.3/learning_loop_node/conftest.py
+-rw-r--r--   0        0        0        0 2024-02-12 10:34:30.593011 learning_loop_node-0.9.3/learning_loop_node/converter/__init__.py
+-rw-r--r--   0        0        0     2534 2024-02-12 10:34:30.593011 learning_loop_node-0.9.3/learning_loop_node/converter/converter_logic.py
+-rw-r--r--   0        0        0     4932 2024-02-12 10:34:30.593011 learning_loop_node-0.9.3/learning_loop_node/converter/converter_node.py
+-rw-r--r--   0        0        0     2207 2024-02-12 10:34:30.593011 learning_loop_node-0.9.3/learning_loop_node/converter/tests/test_converter.py
+-rw-r--r--   0        0        0      783 2024-02-12 10:34:30.593011 learning_loop_node-0.9.3/learning_loop_node/data_classes/__init__.py
+-rw-r--r--   0        0        0     1211 2024-02-12 10:34:30.593011 learning_loop_node-0.9.3/learning_loop_node/data_classes/annotations.py
+-rw-r--r--   0        0        0     4115 2024-02-12 10:34:30.593011 learning_loop_node-0.9.3/learning_loop_node/data_classes/detections.py
+-rw-r--r--   0        0        0     4761 2024-02-12 10:34:30.593011 learning_loop_node-0.9.3/learning_loop_node/data_classes/general.py
+-rw-r--r--   0        0        0      655 2024-02-12 10:34:30.593011 learning_loop_node-0.9.3/learning_loop_node/data_classes/socket_response.py
+-rw-r--r--   0        0        0     4870 2024-02-12 10:34:30.593011 learning_loop_node-0.9.3/learning_loop_node/data_classes/training.py
+-rw-r--r--   0        0        0    10346 2024-02-12 10:34:30.593011 learning_loop_node-0.9.3/learning_loop_node/data_exchanger.py
+-rw-r--r--   0        0        0        1 2024-02-12 10:34:30.593011 learning_loop_node-0.9.3/learning_loop_node/detector/__init__.py
+-rw-r--r--   0        0        0     1660 2024-02-12 10:34:30.593011 learning_loop_node-0.9.3/learning_loop_node/detector/detector_logic.py
+-rw-r--r--   0        0        0    16646 2024-02-12 10:34:30.593011 learning_loop_node-0.9.3/learning_loop_node/detector/detector_node.py
+-rw-r--r--   0        0        0        0 2024-02-12 10:34:30.593011 learning_loop_node-0.9.3/learning_loop_node/detector/inbox_filter/__init__.py
+-rw-r--r--   0        0        0     3437 2024-02-12 10:34:30.593011 learning_loop_node-0.9.3/learning_loop_node/detector/inbox_filter/cam_observation_history.py
+-rw-r--r--   0        0        0     1011 2024-02-12 10:34:30.593011 learning_loop_node-0.9.3/learning_loop_node/detector/inbox_filter/relevance_filter.py
+-rw-r--r--   0        0        0     1385 2024-02-12 10:34:30.593011 learning_loop_node-0.9.3/learning_loop_node/detector/inbox_filter/tests/test_observation.py
+-rw-r--r--   0        0        0     7865 2024-02-12 10:34:30.593011 learning_loop_node-0.9.3/learning_loop_node/detector/inbox_filter/tests/test_relevance_group.py
+-rw-r--r--   0        0        0     1804 2024-02-12 10:34:30.593011 learning_loop_node-0.9.3/learning_loop_node/detector/inbox_filter/tests/test_unexpected_observations_count.py
+-rw-r--r--   0        0        0     4296 2024-02-12 10:34:30.593011 learning_loop_node-0.9.3/learning_loop_node/detector/outbox.py
+-rw-r--r--   0        0        0        0 2024-02-12 10:34:30.593011 learning_loop_node-0.9.3/learning_loop_node/detector/rest/__init__.py
+-rw-r--r--   0        0        0      606 2024-02-12 10:34:30.593011 learning_loop_node-0.9.3/learning_loop_node/detector/rest/about.py
+-rw-r--r--   0        0        0     1725 2024-02-12 10:34:30.593011 learning_loop_node-0.9.3/learning_loop_node/detector/rest/backdoor_controls.py
+-rw-r--r--   0        0        0     1873 2024-02-12 10:34:30.593011 learning_loop_node-0.9.3/learning_loop_node/detector/rest/detect.py
+-rw-r--r--   0        0        0     1664 2024-02-12 10:34:30.593011 learning_loop_node-0.9.3/learning_loop_node/detector/rest/operation_mode.py
+-rw-r--r--   0        0        0      435 2024-02-12 10:34:30.593011 learning_loop_node-0.9.3/learning_loop_node/detector/rest/upload.py
+-rw-r--r--   0        0        0        0 2024-02-12 10:34:30.593011 learning_loop_node-0.9.3/learning_loop_node/detector/tests/__init__.py
+-rw-r--r--   0        0        0     3333 2024-02-12 10:34:30.593011 learning_loop_node-0.9.3/learning_loop_node/detector/tests/conftest.py
+-rw-r--r--   0        0        0   161390 2024-02-12 10:34:30.593011 learning_loop_node-0.9.3/learning_loop_node/detector/tests/test.jpg
+-rw-r--r--   0        0        0     4539 2024-02-12 10:34:30.593011 learning_loop_node-0.9.3/learning_loop_node/detector/tests/test_client_communication.py
+-rw-r--r--   0        0        0     2011 2024-02-12 10:34:30.593011 learning_loop_node-0.9.3/learning_loop_node/detector/tests/test_outbox.py
+-rw-r--r--   0        0        0     1981 2024-02-12 10:34:30.593011 learning_loop_node-0.9.3/learning_loop_node/detector/tests/test_relevance_filter.py
+-rw-r--r--   0        0        0     1060 2024-02-12 10:34:30.593011 learning_loop_node-0.9.3/learning_loop_node/detector/tests/testing_detector.py
+-rw-r--r--   0        0        0     2038 2024-02-12 10:34:30.593011 learning_loop_node-0.9.3/learning_loop_node/examples/novelty_score_updater.py
+-rw-r--r--   0        0        0      165 2024-02-12 10:34:30.593011 learning_loop_node-0.9.3/learning_loop_node/globals.py
+-rw-r--r--   0        0        0        0 2024-02-12 10:34:30.593011 learning_loop_node-0.9.3/learning_loop_node/helpers/__init__.py
+-rw-r--r--   0        0        0     1543 2024-02-12 10:34:30.593011 learning_loop_node-0.9.3/learning_loop_node/helpers/environment_reader.py
+-rwxr-xr-x   0        0        0     1129 2024-02-12 10:34:30.593011 learning_loop_node-0.9.3/learning_loop_node/helpers/gdrive_downloader.py
+-rw-r--r--   0        0        0      824 2024-02-12 10:34:30.593011 learning_loop_node-0.9.3/learning_loop_node/helpers/log_conf.py
+-rw-r--r--   0        0        0     4153 2024-02-12 10:34:30.593011 learning_loop_node-0.9.3/learning_loop_node/helpers/misc.py
+-rw-r--r--   0        0        0     4730 2024-02-12 10:34:30.593011 learning_loop_node-0.9.3/learning_loop_node/loop_communication.py
+-rw-r--r--   0        0        0     9793 2024-02-12 10:34:30.593011 learning_loop_node-0.9.3/learning_loop_node/node.py
+-rw-r--r--   0        0        0      262 2024-02-12 10:34:30.593011 learning_loop_node-0.9.3/learning_loop_node/pytest.ini
+-rw-r--r--   0        0        0        0 2024-02-12 10:34:30.593011 learning_loop_node-0.9.3/learning_loop_node/tests/__init__.py
+-rw-r--r--   0        0        0      920 2024-02-12 10:34:30.593011 learning_loop_node-0.9.3/learning_loop_node/tests/conftest.py
+-rw-r--r--   0        0        0       19 2024-02-12 10:34:30.593011 learning_loop_node-0.9.3/learning_loop_node/tests/test_data/file_1.txt
+-rw-r--r--   0        0        0       19 2024-02-12 10:34:30.593011 learning_loop_node-0.9.3/learning_loop_node/tests/test_data/file_2.txt
+-rw-r--r--   0        0        0      516 2024-02-12 10:34:30.593011 learning_loop_node-0.9.3/learning_loop_node/tests/test_data/model.json
+-rw-r--r--   0        0        0      788 2024-02-12 10:34:30.593011 learning_loop_node-0.9.3/learning_loop_node/tests/test_data_classes.py
+-rw-r--r--   0        0        0     2755 2024-02-12 10:34:30.593011 learning_loop_node-0.9.3/learning_loop_node/tests/test_downloader.py
+-rw-r--r--   0        0        0     1948 2024-02-12 10:34:30.593011 learning_loop_node-0.9.3/learning_loop_node/tests/test_executor.py
+-rw-r--r--   0        0        0     2412 2024-02-12 10:34:30.593011 learning_loop_node-0.9.3/learning_loop_node/tests/test_helper.py
+-rw-r--r--   0        0        0      701 2024-02-12 10:34:30.593011 learning_loop_node-0.9.3/learning_loop_node/tests/test_learning_loop_node.py
+-rw-r--r--   0        0        0        0 2024-02-12 10:34:30.593011 learning_loop_node-0.9.3/learning_loop_node/trainer/__init__.py
+-rw-r--r--   0        0        0     1467 2024-02-12 10:34:30.593011 learning_loop_node-0.9.3/learning_loop_node/trainer/downloader.py
+-rw-r--r--   0        0        0     3118 2024-02-12 10:34:30.593011 learning_loop_node-0.9.3/learning_loop_node/trainer/executor.py
+-rw-r--r--   0        0        0     4419 2024-02-12 10:34:30.593011 learning_loop_node-0.9.3/learning_loop_node/trainer/io_helpers.py
+-rw-r--r--   0        0        0        0 2024-02-12 10:34:30.593011 learning_loop_node-0.9.3/learning_loop_node/trainer/rest/__init__.py
+-rw-r--r--   0        0        0     5635 2024-02-12 10:34:30.593011 learning_loop_node-0.9.3/learning_loop_node/trainer/rest/backdoor_controls.py
+-rw-r--r--   0        0        0      897 2024-02-12 10:34:30.593011 learning_loop_node-0.9.3/learning_loop_node/trainer/rest/controls.py
+-rw-r--r--   0        0        0        0 2024-02-12 10:34:30.593011 learning_loop_node-0.9.3/learning_loop_node/trainer/tests/__init__.py
+-rw-r--r--   0        0        0     2829 2024-02-12 10:34:30.593011 learning_loop_node-0.9.3/learning_loop_node/trainer/tests/conftest.py
+-rw-r--r--   0        0        0      934 2024-02-12 10:34:30.593011 learning_loop_node-0.9.3/learning_loop_node/trainer/tests/state_helper.py
+-rw-r--r--   0        0        0        0 2024-02-12 10:34:30.593011 learning_loop_node-0.9.3/learning_loop_node/trainer/tests/states/__init__.py
+-rw-r--r--   0        0        0     1310 2024-02-12 10:34:30.597011 learning_loop_node-0.9.3/learning_loop_node/trainer/tests/states/test_state_cleanup.py
+-rw-r--r--   0        0        0     3608 2024-02-12 10:34:30.597011 learning_loop_node-0.9.3/learning_loop_node/trainer/tests/states/test_state_detecting.py
+-rw-r--r--   0        0        0     2604 2024-02-12 10:34:30.597011 learning_loop_node-0.9.3/learning_loop_node/trainer/tests/states/test_state_download_train_model.py
+-rw-r--r--   0        0        0     2233 2024-02-12 10:34:30.597011 learning_loop_node-0.9.3/learning_loop_node/trainer/tests/states/test_state_prepare.py
+-rw-r--r--   0        0        0     4558 2024-02-12 10:34:30.597011 learning_loop_node-0.9.3/learning_loop_node/trainer/tests/states/test_state_sync_confusion_matrix.py
+-rw-r--r--   0        0        0     3309 2024-02-12 10:34:30.597011 learning_loop_node-0.9.3/learning_loop_node/trainer/tests/states/test_state_train.py
+-rw-r--r--   0        0        0     7202 2024-02-12 10:34:30.597011 learning_loop_node-0.9.3/learning_loop_node/trainer/tests/states/test_state_upload_detections.py
+-rw-r--r--   0        0        0     3558 2024-02-12 10:34:30.597011 learning_loop_node-0.9.3/learning_loop_node/trainer/tests/states/test_state_upload_model.py
+-rw-r--r--   0        0        0     1915 2024-02-12 10:34:30.597011 learning_loop_node-0.9.3/learning_loop_node/trainer/tests/test_errors.py
+-rw-r--r--   0        0        0     1144 2024-02-12 10:34:30.597011 learning_loop_node-0.9.3/learning_loop_node/trainer/tests/test_trainer_states.py
+-rw-r--r--   0        0        0     3957 2024-02-12 10:34:30.597011 learning_loop_node-0.9.3/learning_loop_node/trainer/tests/testing_trainer_logic.py
+-rw-r--r--   0        0        0    33057 2024-02-12 10:34:30.597011 learning_loop_node-0.9.3/learning_loop_node/trainer/trainer_logic.py
+-rw-r--r--   0        0        0     8018 2024-02-12 10:34:30.597011 learning_loop_node-0.9.3/learning_loop_node/trainer/trainer_node.py
+-rw-r--r--   0        0        0     1884 2024-02-12 10:34:30.597011 learning_loop_node-0.9.3/learning_loop_node/trainer/training_syncronizer.py
+-rw-r--r--   0        0        0     1148 2024-02-12 10:34:43.637126 learning_loop_node-0.9.3/pyproject.toml
+-rw-r--r--   0        0        0     9157 1970-01-01 00:00:00.000000 learning_loop_node-0.9.3/PKG-INFO
```

### Comparing `learning_loop_node-0.9.2/README.md` & `learning_loop_node-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `learning_loop_node-0.9.2/learning_loop_node/annotation/annotator_logic.py` & `learning_loop_node-0.9.3/learning_loop_node/annotation/annotator_logic.py`

 * *Files identical despite different names*

### Comparing `learning_loop_node-0.9.2/learning_loop_node/annotation/annotator_node.py` & `learning_loop_node-0.9.3/learning_loop_node/annotation/annotator_node.py`

 * *Files identical despite different names*

### Comparing `learning_loop_node-0.9.2/learning_loop_node/annotation/tests/test_annotator_node.py` & `learning_loop_node-0.9.3/learning_loop_node/annotation/tests/test_annotator_node.py`

 * *Files identical despite different names*

### Comparing `learning_loop_node-0.9.2/learning_loop_node/conftest.py` & `learning_loop_node-0.9.3/learning_loop_node/conftest.py`

 * *Files identical despite different names*

### Comparing `learning_loop_node-0.9.2/learning_loop_node/converter/converter_logic.py` & `learning_loop_node-0.9.3/learning_loop_node/converter/converter_logic.py`

 * *Files identical despite different names*

### Comparing `learning_loop_node-0.9.2/learning_loop_node/converter/converter_node.py` & `learning_loop_node-0.9.3/learning_loop_node/converter/converter_node.py`

 * *Files identical despite different names*

### Comparing `learning_loop_node-0.9.2/learning_loop_node/converter/tests/test_converter.py` & `learning_loop_node-0.9.3/learning_loop_node/converter/tests/test_converter.py`

 * *Files identical despite different names*

### Comparing `learning_loop_node-0.9.2/learning_loop_node/data_classes/__init__.py` & `learning_loop_node-0.9.3/learning_loop_node/data_classes/__init__.py`

 * *Files identical despite different names*

### Comparing `learning_loop_node-0.9.2/learning_loop_node/data_classes/annotations.py` & `learning_loop_node-0.9.3/learning_loop_node/data_classes/annotations.py`

 * *Files identical despite different names*

### Comparing `learning_loop_node-0.9.2/learning_loop_node/data_classes/detections.py` & `learning_loop_node-0.9.3/learning_loop_node/data_classes/detections.py`

 * *Files identical despite different names*

### Comparing `learning_loop_node-0.9.2/learning_loop_node/data_classes/general.py` & `learning_loop_node-0.9.3/learning_loop_node/data_classes/general.py`

 * *Files 3% similar despite different names*

```diff
@@ -86,14 +86,18 @@
         if not self.model_root_path:
             raise Exception("model_root_path is not set")
         with open(self.model_root_path + '/model.json', 'w') as f:
             self_as_dict = asdict(self)
             del self_as_dict['model_root_path']
             f.write(json.dumps(self_as_dict))
 
+    @staticmethod
+    def from_dict(data: Dict) -> 'ModelInformation':
+        return from_dict(ModelInformation, data=data)
+
 
 @dataclass(**KWONLY_SLOTS)
 class ErrorConfiguration():
     begin_training: Optional[bool] = False
     save_model: Optional[bool] = False
     get_new_model: Optional[bool] = False
     crash_training: Optional[bool] = False
```

### Comparing `learning_loop_node-0.9.2/learning_loop_node/data_classes/socket_response.py` & `learning_loop_node-0.9.3/learning_loop_node/data_classes/socket_response.py`

 * *Files identical despite different names*

### Comparing `learning_loop_node-0.9.2/learning_loop_node/data_classes/training.py` & `learning_loop_node-0.9.3/learning_loop_node/data_classes/training.py`

 * *Files identical despite different names*

### Comparing `learning_loop_node-0.9.2/learning_loop_node/data_exchanger.py` & `learning_loop_node-0.9.3/learning_loop_node/data_exchanger.py`

 * *Files identical despite different names*

### Comparing `learning_loop_node-0.9.2/learning_loop_node/detector/detector_logic.py` & `learning_loop_node-0.9.3/learning_loop_node/detector/detector_logic.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,19 +9,17 @@
 
 
 class DetectorLogic():
 
     def __init__(self, model_format: str) -> None:
         self.model_format: str = model_format
         self._model_info: Optional[ModelInformation] = None
-        self.target_model: Optional[str] = None
 
     async def soft_reload(self):
         self._model_info = None
-        self.target_model = None
 
     @property
     def model_info(self) -> ModelInformation:
         if self._model_info is None:
             raise Exception('Model not loaded')
         return self._model_info
```

### Comparing `learning_loop_node-0.9.2/learning_loop_node/detector/detector_node.py` & `learning_loop_node-0.9.3/learning_loop_node/detector/detector_node.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,24 +10,24 @@
 
 import numpy as np
 from dacite import from_dict
 from fastapi.encoders import jsonable_encoder
 from fastapi_socketio import SocketManager
 from socketio import AsyncClient
 
-from ..data_classes import (Category, Context, Detections, DetectionStatus,
-                            ModelInformation, NodeState, Shape)
+from ..data_classes import Category, Context, Detections, DetectionStatus, ModelInformation, NodeState, Shape
 from ..data_classes.socket_response import SocketResponse
 from ..data_exchanger import DataExchanger, DownloadError
 from ..globals import GLOBALS
 from ..helpers import environment_reader
 from ..node import Node
 from .detector_logic import DetectorLogic
 from .inbox_filter.relevance_filter import RelevanceFilter
 from .outbox import Outbox
+from .rest import about as rest_about
 from .rest import backdoor_controls
 from .rest import detect as rest_detect
 from .rest import operation_mode as rest_mode
 from .rest import upload as rest_upload
 from .rest.operation_mode import OperationMode
 
 
@@ -46,19 +46,21 @@
 
         self.outbox: Outbox = Outbox()
         self.data_exchanger = DataExchanger(
             Context(organization=self.organization, project=self.project),
             self.loop_communicator)
 
         self.relevance_filter: RelevanceFilter = RelevanceFilter(self.outbox)
-        self.target_model = None
+        self.target_model: Optional[str] = None
 
         self.include_router(rest_detect.router, tags=["detect"])
         self.include_router(rest_upload.router, prefix="")
         self.include_router(rest_mode.router, tags=["operation_mode"])
+        self.include_router(rest_about.router, tags=["about"])
+
         if use_backdoor_controls:
             self.include_router(backdoor_controls.router)
 
         self.setup_sio_server()
 
     async def soft_reload(self) -> None:
         # simulate init
```

### Comparing `learning_loop_node-0.9.2/learning_loop_node/detector/inbox_filter/cam_observation_history.py` & `learning_loop_node-0.9.3/learning_loop_node/detector/inbox_filter/cam_observation_history.py`

 * *Files identical despite different names*

### Comparing `learning_loop_node-0.9.2/learning_loop_node/detector/inbox_filter/relevance_filter.py` & `learning_loop_node-0.9.3/learning_loop_node/detector/inbox_filter/relevance_filter.py`

 * *Files identical despite different names*

### Comparing `learning_loop_node-0.9.2/learning_loop_node/detector/inbox_filter/tests/test_observation.py` & `learning_loop_node-0.9.3/learning_loop_node/detector/inbox_filter/tests/test_observation.py`

 * *Files identical despite different names*

### Comparing `learning_loop_node-0.9.2/learning_loop_node/detector/inbox_filter/tests/test_relevance_group.py` & `learning_loop_node-0.9.3/learning_loop_node/detector/inbox_filter/tests/test_relevance_group.py`

 * *Files identical despite different names*

### Comparing `learning_loop_node-0.9.2/learning_loop_node/detector/inbox_filter/tests/test_unexpected_observations_count.py` & `learning_loop_node-0.9.3/learning_loop_node/detector/inbox_filter/tests/test_unexpected_observations_count.py`

 * *Files identical despite different names*

### Comparing `learning_loop_node-0.9.2/learning_loop_node/detector/outbox.py` & `learning_loop_node-0.9.3/learning_loop_node/detector/outbox.py`

 * *Files identical despite different names*

### Comparing `learning_loop_node-0.9.2/learning_loop_node/detector/rest/backdoor_controls.py` & `learning_loop_node-0.9.3/learning_loop_node/detector/rest/backdoor_controls.py`

 * *Files identical despite different names*

### Comparing `learning_loop_node-0.9.2/learning_loop_node/detector/rest/detect.py` & `learning_loop_node-0.9.3/learning_loop_node/detector/rest/detect.py`

 * *Files identical despite different names*

### Comparing `learning_loop_node-0.9.2/learning_loop_node/detector/rest/operation_mode.py` & `learning_loop_node-0.9.3/learning_loop_node/detector/rest/operation_mode.py`

 * *Files identical despite different names*

### Comparing `learning_loop_node-0.9.2/learning_loop_node/detector/tests/conftest.py` & `learning_loop_node-0.9.3/learning_loop_node/detector/tests/conftest.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,23 +33,27 @@
     except Exception:
         pass
     return should_have_seg
 
 
 @pytest.fixture()
 async def test_detector_node():
+    """Initializes and runs a detector testnode. Note that the running instance and the one the function returns are not the same instances!"""
+
     os.environ['ORGANIZATION'] = 'zauberzeug'
     os.environ['PROJECT'] = 'demo'
 
     detector = TestingDetectorLogic()
     node = DetectorNode(name='test', detector=detector)
     await port_is(free=True)
 
     multiprocessing.set_start_method('fork', force=True)
     assert multiprocessing.get_start_method() == 'fork'
+    # print('\n\n',multiprocessing.get_start_method())
+
     proc = Process(target=uvicorn.run,
                    args=(node,),
                    kwargs={
                        "host": "127.0.0.1",
                        "port": detector_port,
                    }, daemon=True)
     proc.start()
```

### Comparing `learning_loop_node-0.9.2/learning_loop_node/detector/tests/test.jpg` & `learning_loop_node-0.9.3/learning_loop_node/detector/tests/test.jpg`

 * *Files identical despite different names*

### Comparing `learning_loop_node-0.9.2/learning_loop_node/detector/tests/test_client_communication.py` & `learning_loop_node-0.9.3/learning_loop_node/detector/tests/test_client_communication.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import asyncio
+import json
 
 import pytest
 import requests
 
 from learning_loop_node import DetectorNode
+from learning_loop_node.data_classes import Category, ModelInformation
 from learning_loop_node.detector.tests.conftest import get_outbox_files
 from learning_loop_node.globals import GLOBALS
 
 from .testing_detector import TestingDetectorLogic
 
 
 @pytest.mark.asyncio
@@ -80,7 +82,21 @@
     assert len(get_outbox_files(test_detector_node.outbox)) == 0
 
     with open('detector/tests/test.jpg', 'rb') as f:
         image_bytes = f.read()
     result = await sio_client.call('upload', {'image': image_bytes})
     assert result is None
     assert len(get_outbox_files(test_detector_node.outbox)) == 2, 'There should be one image and one .json file.'
+
+
+async def test_about_endpoint(test_detector_node: DetectorNode):
+    await asyncio.sleep(1)
+    response = requests.get(f'http://localhost:{GLOBALS.detector_port}/about', timeout=30)
+
+    assert response.status_code == 200
+    response_dict = json.loads(response.content)
+    model_information = ModelInformation.from_dict(response_dict['model_info'])
+
+    assert response_dict['operation_mode'] == 'idle'
+    assert response_dict['state'] == 'online'
+    assert response_dict['target_model'] == '1.1'
+    assert any([c.name == 'purple point' for c in model_information.categories])
```

### Comparing `learning_loop_node-0.9.2/learning_loop_node/detector/tests/test_outbox.py` & `learning_loop_node-0.9.3/learning_loop_node/detector/tests/test_outbox.py`

 * *Files identical despite different names*

### Comparing `learning_loop_node-0.9.2/learning_loop_node/detector/tests/test_relevance_filter.py` & `learning_loop_node-0.9.3/learning_loop_node/detector/tests/test_relevance_filter.py`

 * *Files identical despite different names*

### Comparing `learning_loop_node-0.9.2/learning_loop_node/detector/tests/testing_detector.py` & `learning_loop_node-0.9.3/learning_loop_node/detector/tests/testing_detector.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import logging
 
 import numpy as np
 
 from learning_loop_node import DetectorLogic
 from learning_loop_node.conftest import get_dummy_detections
-from learning_loop_node.data_classes import Detections
+from learning_loop_node.data_classes import Category, Detections, ModelInformation
 
 
 class TestingDetectorLogic(DetectorLogic):
     __test__ = False
 
     def __init__(self) -> None:
         super().__init__('mocked')
```

### Comparing `learning_loop_node-0.9.2/learning_loop_node/examples/novelty_score_updater.py` & `learning_loop_node-0.9.3/learning_loop_node/examples/novelty_score_updater.py`

 * *Files identical despite different names*

### Comparing `learning_loop_node-0.9.2/learning_loop_node/helpers/environment_reader.py` & `learning_loop_node-0.9.3/learning_loop_node/helpers/environment_reader.py`

 * *Files identical despite different names*

### Comparing `learning_loop_node-0.9.2/learning_loop_node/helpers/gdrive_downloader.py` & `learning_loop_node-0.9.3/learning_loop_node/helpers/gdrive_downloader.py`

 * *Files identical despite different names*

### Comparing `learning_loop_node-0.9.2/learning_loop_node/helpers/log_conf.py` & `learning_loop_node-0.9.3/learning_loop_node/helpers/log_conf.py`

 * *Files identical despite different names*

### Comparing `learning_loop_node-0.9.2/learning_loop_node/helpers/misc.py` & `learning_loop_node-0.9.3/learning_loop_node/helpers/misc.py`

 * *Files identical despite different names*

### Comparing `learning_loop_node-0.9.2/learning_loop_node/loop_communication.py` & `learning_loop_node-0.9.3/learning_loop_node/loop_communication.py`

 * *Files identical despite different names*

### Comparing `learning_loop_node-0.9.2/learning_loop_node/node.py` & `learning_loop_node-0.9.3/learning_loop_node/node.py`

 * *Files identical despite different names*

### Comparing `learning_loop_node-0.9.2/learning_loop_node/tests/conftest.py` & `learning_loop_node-0.9.3/learning_loop_node/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `learning_loop_node-0.9.2/learning_loop_node/tests/test_data/model.json` & `learning_loop_node-0.9.3/learning_loop_node/tests/test_data/model.json`

 * *Files identical despite different names*

### Comparing `learning_loop_node-0.9.2/learning_loop_node/tests/test_data_classes.py` & `learning_loop_node-0.9.3/learning_loop_node/tests/test_data_classes.py`

 * *Files identical despite different names*

### Comparing `learning_loop_node-0.9.2/learning_loop_node/tests/test_downloader.py` & `learning_loop_node-0.9.3/learning_loop_node/tests/test_downloader.py`

 * *Files identical despite different names*

### Comparing `learning_loop_node-0.9.2/learning_loop_node/tests/test_executor.py` & `learning_loop_node-0.9.3/learning_loop_node/tests/test_executor.py`

 * *Files identical despite different names*

### Comparing `learning_loop_node-0.9.2/learning_loop_node/tests/test_helper.py` & `learning_loop_node-0.9.3/learning_loop_node/tests/test_helper.py`

 * *Files identical despite different names*

### Comparing `learning_loop_node-0.9.2/learning_loop_node/tests/test_learning_loop_node.py` & `learning_loop_node-0.9.3/learning_loop_node/tests/test_learning_loop_node.py`

 * *Files identical despite different names*

### Comparing `learning_loop_node-0.9.2/learning_loop_node/trainer/downloader.py` & `learning_loop_node-0.9.3/learning_loop_node/trainer/downloader.py`

 * *Files identical despite different names*

### Comparing `learning_loop_node-0.9.2/learning_loop_node/trainer/executor.py` & `learning_loop_node-0.9.3/learning_loop_node/trainer/executor.py`

 * *Files identical despite different names*

### Comparing `learning_loop_node-0.9.2/learning_loop_node/trainer/io_helpers.py` & `learning_loop_node-0.9.3/learning_loop_node/trainer/io_helpers.py`

 * *Files identical despite different names*

### Comparing `learning_loop_node-0.9.2/learning_loop_node/trainer/rest/backdoor_controls.py` & `learning_loop_node-0.9.3/learning_loop_node/trainer/rest/backdoor_controls.py`

 * *Files identical despite different names*

### Comparing `learning_loop_node-0.9.2/learning_loop_node/trainer/rest/controls.py` & `learning_loop_node-0.9.3/learning_loop_node/trainer/rest/controls.py`

 * *Files identical despite different names*

### Comparing `learning_loop_node-0.9.2/learning_loop_node/trainer/tests/conftest.py` & `learning_loop_node-0.9.3/learning_loop_node/trainer/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `learning_loop_node-0.9.2/learning_loop_node/trainer/tests/state_helper.py` & `learning_loop_node-0.9.3/learning_loop_node/trainer/tests/state_helper.py`

 * *Files identical despite different names*

### Comparing `learning_loop_node-0.9.2/learning_loop_node/trainer/tests/states/test_state_cleanup.py` & `learning_loop_node-0.9.3/learning_loop_node/trainer/tests/states/test_state_cleanup.py`

 * *Files identical despite different names*

### Comparing `learning_loop_node-0.9.2/learning_loop_node/trainer/tests/states/test_state_detecting.py` & `learning_loop_node-0.9.3/learning_loop_node/trainer/tests/states/test_state_detecting.py`

 * *Files identical despite different names*

### Comparing `learning_loop_node-0.9.2/learning_loop_node/trainer/tests/states/test_state_download_train_model.py` & `learning_loop_node-0.9.3/learning_loop_node/trainer/tests/states/test_state_download_train_model.py`

 * *Files identical despite different names*

### Comparing `learning_loop_node-0.9.2/learning_loop_node/trainer/tests/states/test_state_prepare.py` & `learning_loop_node-0.9.3/learning_loop_node/trainer/tests/states/test_state_prepare.py`

 * *Files identical despite different names*

### Comparing `learning_loop_node-0.9.2/learning_loop_node/trainer/tests/states/test_state_sync_confusion_matrix.py` & `learning_loop_node-0.9.3/learning_loop_node/trainer/tests/states/test_state_sync_confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `learning_loop_node-0.9.2/learning_loop_node/trainer/tests/states/test_state_train.py` & `learning_loop_node-0.9.3/learning_loop_node/trainer/tests/states/test_state_train.py`

 * *Files identical despite different names*

### Comparing `learning_loop_node-0.9.2/learning_loop_node/trainer/tests/states/test_state_upload_detections.py` & `learning_loop_node-0.9.3/learning_loop_node/trainer/tests/states/test_state_upload_detections.py`

 * *Files identical despite different names*

### Comparing `learning_loop_node-0.9.2/learning_loop_node/trainer/tests/states/test_state_upload_model.py` & `learning_loop_node-0.9.3/learning_loop_node/trainer/tests/states/test_state_upload_model.py`

 * *Files identical despite different names*

### Comparing `learning_loop_node-0.9.2/learning_loop_node/trainer/tests/test_errors.py` & `learning_loop_node-0.9.3/learning_loop_node/trainer/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `learning_loop_node-0.9.2/learning_loop_node/trainer/tests/test_trainer_states.py` & `learning_loop_node-0.9.3/learning_loop_node/trainer/tests/test_trainer_states.py`

 * *Files identical despite different names*

### Comparing `learning_loop_node-0.9.2/learning_loop_node/trainer/tests/testing_trainer_logic.py` & `learning_loop_node-0.9.3/learning_loop_node/trainer/tests/testing_trainer_logic.py`

 * *Files identical despite different names*

### Comparing `learning_loop_node-0.9.2/learning_loop_node/trainer/trainer_logic.py` & `learning_loop_node-0.9.3/learning_loop_node/trainer/trainer_logic.py`

 * *Files identical despite different names*

### Comparing `learning_loop_node-0.9.2/learning_loop_node/trainer/trainer_node.py` & `learning_loop_node-0.9.3/learning_loop_node/trainer/trainer_node.py`

 * *Files identical despite different names*

### Comparing `learning_loop_node-0.9.2/learning_loop_node/trainer/training_syncronizer.py` & `learning_loop_node-0.9.3/learning_loop_node/trainer/training_syncronizer.py`

 * *Files identical despite different names*

### Comparing `learning_loop_node-0.9.2/pyproject.toml` & `learning_loop_node-0.9.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "learning_loop_node"
-version = "v0.9.2"
+version = "v0.9.3"
 description = "Python Library for Nodes which connect to the Zauberzeug Learning Loop"
 authors = ["Zauberzeug GmbH <info@zauberzeug.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/zauberzeug/learning_loop_node"
 
 [tool.poetry.dependencies]
```

### Comparing `learning_loop_node-0.9.2/PKG-INFO` & `learning_loop_node-0.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: learning-loop-node
-Version: 0.9.2
+Version: 0.9.3
 Summary: Python Library for Nodes which connect to the Zauberzeug Learning Loop
 Home-page: https://github.com/zauberzeug/learning_loop_node
 License: MIT
 Author: Zauberzeug GmbH
 Author-email: info@zauberzeug.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```


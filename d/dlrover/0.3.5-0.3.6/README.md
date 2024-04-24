# Comparing `tmp/dlrover-0.3.5-py3-none-any.whl.zip` & `tmp/dlrover-0.3.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,96 +1,97 @@
-Zip file size: 387948 bytes, number of entries: 233
+Zip file size: 397277 bytes, number of entries: 236
 -rw-r--r--  2.0 unx      411 b- defN 23-Mar-07 11:16 dlrover/Makefile
 -rw-r--r--  2.0 unx      599 b- defN 23-Mar-07 11:16 dlrover/__init__.py
 -rw-r--r--  2.0 unx     4439 b- defN 23-May-08 02:53 dlrover/proto/brain.proto
--rw-r--r--  2.0 unx    12755 b- defN 24-Mar-29 05:54 dlrover/proto/brain_pb2.py
--rw-r--r--  2.0 unx     5867 b- defN 24-Mar-29 05:54 dlrover/proto/brain_pb2_grpc.py
+-rw-r--r--  2.0 unx    12755 b- defN 24-Apr-24 06:10 dlrover/proto/brain_pb2.py
+-rw-r--r--  2.0 unx     5867 b- defN 24-Apr-24 06:10 dlrover/proto/brain_pb2_grpc.py
 -rw-r--r--  2.0 unx      463 b- defN 23-Nov-21 06:27 dlrover/proto/elastic_training.proto
--rw-r--r--  2.0 unx     1951 b- defN 24-Mar-29 05:54 dlrover/proto/elastic_training_pb2.py
--rw-r--r--  2.0 unx     4164 b- defN 24-Mar-29 05:54 dlrover/proto/elastic_training_pb2_grpc.py
+-rw-r--r--  2.0 unx     1951 b- defN 24-Apr-24 06:10 dlrover/proto/elastic_training_pb2.py
+-rw-r--r--  2.0 unx     4164 b- defN 24-Apr-24 06:10 dlrover/proto/elastic_training_pb2_grpc.py
 -rw-r--r--  2.0 unx      599 b- defN 23-Mar-07 11:16 dlrover/python/__init__.py
 -rw-r--r--  2.0 unx      599 b- defN 23-Mar-07 11:16 dlrover/python/brain/__init__.py
 -rw-r--r--  2.0 unx    11103 b- defN 23-Nov-23 02:06 dlrover/python/brain/client.py
 -rw-r--r--  2.0 unx      599 b- defN 23-Mar-07 11:16 dlrover/python/common/__init__.py
 -rw-r--r--  2.0 unx     7036 b- defN 24-Mar-26 01:58 dlrover/python/common/constants.py
 -rw-r--r--  2.0 unx     1715 b- defN 24-Mar-18 07:49 dlrover/python/common/env_utils.py
 -rw-r--r--  2.0 unx     7547 b- defN 24-Mar-21 04:14 dlrover/python/common/global_context.py
--rw-r--r--  2.0 unx     9787 b- defN 24-Mar-05 04:34 dlrover/python/common/grpc.py
+-rw-r--r--  2.0 unx     9966 b- defN 24-Apr-16 02:09 dlrover/python/common/grpc.py
 -rw-r--r--  2.0 unx     1377 b- defN 23-Nov-21 06:27 dlrover/python/common/log.py
--rw-r--r--  2.0 unx    18512 b- defN 24-Feb-06 01:58 dlrover/python/common/multi_process.py
+-rw-r--r--  2.0 unx    18440 b- defN 24-Apr-23 06:44 dlrover/python/common/multi_process.py
 -rw-r--r--  2.0 unx    11858 b- defN 24-Mar-26 01:58 dlrover/python/common/node.py
 -rw-r--r--  2.0 unx     1186 b- defN 24-Mar-07 06:35 dlrover/python/common/serialize.py
 -rw-r--r--  2.0 unx     1489 b- defN 24-Feb-20 02:57 dlrover/python/common/singleton.py
 -rw-r--r--  2.0 unx     8635 b- defN 24-Feb-06 06:42 dlrover/python/common/storage.py
 -rw-r--r--  2.0 unx      599 b- defN 23-Mar-07 11:16 dlrover/python/elastic_agent/__init__.py
--rw-r--r--  2.0 unx    14064 b- defN 24-Mar-04 05:56 dlrover/python/elastic_agent/master_client.py
+-rw-r--r--  2.0 unx    14237 b- defN 24-Apr-23 06:44 dlrover/python/elastic_agent/master_client.py
 -rw-r--r--  2.0 unx      599 b- defN 23-Nov-21 06:27 dlrover/python/elastic_agent/config/__init__.py
 -rw-r--r--  2.0 unx     3717 b- defN 24-Feb-20 02:57 dlrover/python/elastic_agent/config/paral_config_tuner.py
 -rw-r--r--  2.0 unx      599 b- defN 23-Mar-07 11:16 dlrover/python/elastic_agent/monitor/__init__.py
 -rw-r--r--  2.0 unx     5980 b- defN 24-Mar-05 07:05 dlrover/python/elastic_agent/monitor/resource.py
 -rw-r--r--  2.0 unx     4659 b- defN 24-Mar-26 09:59 dlrover/python/elastic_agent/monitor/training.py
 -rw-r--r--  2.0 unx      599 b- defN 23-Mar-07 11:16 dlrover/python/elastic_agent/sharding/__init__.py
 -rw-r--r--  2.0 unx    11734 b- defN 24-Feb-06 01:58 dlrover/python/elastic_agent/sharding/client.py
 -rw-r--r--  2.0 unx      599 b- defN 23-May-08 02:53 dlrover/python/elastic_agent/sychronization/__init__.py
 -rw-r--r--  2.0 unx     2686 b- defN 23-Nov-23 02:06 dlrover/python/elastic_agent/sychronization/sync_client.py
 -rw-r--r--  2.0 unx      599 b- defN 23-Mar-07 11:16 dlrover/python/elastic_agent/tensorflow/__init__.py
 -rw-r--r--  2.0 unx     3424 b- defN 24-Feb-06 01:58 dlrover/python/elastic_agent/tensorflow/elastic_ps.py
 -rw-r--r--  2.0 unx     4226 b- defN 24-Feb-06 01:58 dlrover/python/elastic_agent/tensorflow/hooks.py
 -rw-r--r--  2.0 unx     4556 b- defN 23-Mar-07 11:16 dlrover/python/elastic_agent/tensorflow/profile_extractor.py
 -rw-r--r--  2.0 unx      599 b- defN 23-May-08 02:53 dlrover/python/elastic_agent/torch/__init__.py
--rw-r--r--  2.0 unx    39197 b- defN 24-Mar-26 09:59 dlrover/python/elastic_agent/torch/ckpt_saver.py
+-rw-r--r--  2.0 unx    40769 b- defN 24-Apr-23 06:44 dlrover/python/elastic_agent/torch/ckpt_saver.py
 -rw-r--r--  2.0 unx     4594 b- defN 23-Nov-23 02:06 dlrover/python/elastic_agent/torch/master_kv_store.py
--rw-r--r--  2.0 unx    38955 b- defN 24-Mar-20 10:23 dlrover/python/elastic_agent/torch/training.py
+-rw-r--r--  2.0 unx    39591 b- defN 24-Apr-23 06:44 dlrover/python/elastic_agent/torch/training.py
 -rw-r--r--  2.0 unx      599 b- defN 23-Mar-07 11:16 dlrover/python/master/__init__.py
 -rw-r--r--  2.0 unx     3044 b- defN 24-Mar-28 12:07 dlrover/python/master/args.py
--rw-r--r--  2.0 unx    11296 b- defN 24-Mar-29 02:24 dlrover/python/master/dist_master.py
--rw-r--r--  2.0 unx     4375 b- defN 24-Jan-09 08:37 dlrover/python/master/local_master.py
+-rw-r--r--  2.0 unx    11296 b- defN 24-Apr-01 02:41 dlrover/python/master/dist_master.py
+-rw-r--r--  2.0 unx     4416 b- defN 24-Apr-18 06:28 dlrover/python/master/local_master.py
 -rw-r--r--  2.0 unx     2550 b- defN 24-Mar-05 07:32 dlrover/python/master/main.py
 -rw-r--r--  2.0 unx      928 b- defN 23-Nov-21 06:27 dlrover/python/master/master.py
--rw-r--r--  2.0 unx    22988 b- defN 24-Mar-04 05:56 dlrover/python/master/servicer.py
+-rw-r--r--  2.0 unx    23356 b- defN 24-Apr-17 05:53 dlrover/python/master/servicer.py
 -rw-r--r--  2.0 unx      599 b- defN 23-Nov-07 07:11 dlrover/python/master/cluster/__init__.py
 -rw-r--r--  2.0 unx     1124 b- defN 23-Nov-07 07:11 dlrover/python/master/cluster/quota.py
 -rw-r--r--  2.0 unx      599 b- defN 23-Mar-07 11:16 dlrover/python/master/elastic_training/__init__.py
 -rw-r--r--  2.0 unx     3494 b- defN 23-Mar-07 11:16 dlrover/python/master/elastic_training/elastic_ps.py
 -rw-r--r--  2.0 unx     1017 b- defN 23-Nov-07 07:11 dlrover/python/master/elastic_training/kv_store_service.py
--rw-r--r--  2.0 unx    19740 b- defN 24-Mar-26 01:58 dlrover/python/master/elastic_training/rdzv_manager.py
+-rw-r--r--  2.0 unx     2852 b- defN 24-Apr-23 06:44 dlrover/python/master/elastic_training/net_topology.py
+-rw-r--r--  2.0 unx    22102 b- defN 24-Apr-23 06:44 dlrover/python/master/elastic_training/rdzv_manager.py
 -rw-r--r--  2.0 unx     4971 b- defN 23-Nov-21 06:27 dlrover/python/master/elastic_training/sync_service.py
 -rw-r--r--  2.0 unx      599 b- defN 23-Nov-21 06:27 dlrover/python/master/hyperparams/__init__.py
 -rw-r--r--  2.0 unx     6818 b- defN 24-Feb-06 01:58 dlrover/python/master/hyperparams/simple_strategy_generator.py
 -rw-r--r--  2.0 unx     1000 b- defN 23-Nov-21 06:27 dlrover/python/master/hyperparams/strategy_generator.py
 -rw-r--r--  2.0 unx      599 b- defN 23-Mar-07 11:16 dlrover/python/master/monitor/__init__.py
 -rw-r--r--  2.0 unx     4490 b- defN 24-Mar-26 01:58 dlrover/python/master/monitor/error_monitor.py
 -rw-r--r--  2.0 unx     7384 b- defN 24-Mar-29 02:24 dlrover/python/master/monitor/speed_monitor.py
 -rw-r--r--  2.0 unx      599 b- defN 23-Mar-07 11:16 dlrover/python/master/node/__init__.py
--rw-r--r--  2.0 unx    34376 b- defN 24-Mar-29 02:24 dlrover/python/master/node/dist_job_manager.py
+-rw-r--r--  2.0 unx    34327 b- defN 24-Apr-23 06:44 dlrover/python/master/node/dist_job_manager.py
 -rw-r--r--  2.0 unx    13001 b- defN 24-Mar-26 01:58 dlrover/python/master/node/event_callback.py
 -rw-r--r--  2.0 unx    12665 b- defN 23-Dec-13 06:11 dlrover/python/master/node/job_auto_scaler.py
 -rw-r--r--  2.0 unx     3661 b- defN 24-Mar-04 05:56 dlrover/python/master/node/job_manager.py
 -rw-r--r--  2.0 unx     5342 b- defN 24-Mar-12 05:23 dlrover/python/master/node/local_job_manager.py
 -rw-r--r--  2.0 unx    14448 b- defN 23-Dec-21 04:12 dlrover/python/master/node/ps.py
 -rw-r--r--  2.0 unx     4094 b- defN 23-Nov-21 06:27 dlrover/python/master/node/status_flow.py
 -rw-r--r--  2.0 unx    13398 b- defN 23-Dec-21 04:12 dlrover/python/master/node/training_node.py
--rw-r--r--  2.0 unx    11211 b- defN 23-Dec-21 04:12 dlrover/python/master/node/worker.py
+-rw-r--r--  2.0 unx    11300 b- defN 24-Apr-23 06:44 dlrover/python/master/node/worker.py
 -rw-r--r--  2.0 unx      599 b- defN 23-Mar-07 11:16 dlrover/python/master/resource/__init__.py
 -rw-r--r--  2.0 unx     4187 b- defN 23-May-08 02:53 dlrover/python/master/resource/brain_optimizer.py
 -rw-r--r--  2.0 unx    21672 b- defN 24-Feb-23 09:24 dlrover/python/master/resource/job.py
 -rw-r--r--  2.0 unx    15828 b- defN 24-Feb-06 01:58 dlrover/python/master/resource/local_optimizer.py
 -rw-r--r--  2.0 unx     6187 b- defN 23-Nov-21 06:27 dlrover/python/master/resource/optimizer.py
 -rw-r--r--  2.0 unx      599 b- defN 23-Mar-07 11:16 dlrover/python/master/scaler/__init__.py
 -rw-r--r--  2.0 unx     2202 b- defN 23-Nov-23 02:06 dlrover/python/master/scaler/base_scaler.py
 -rw-r--r--  2.0 unx     8541 b- defN 23-Nov-23 02:06 dlrover/python/master/scaler/elasticjob_scaler.py
 -rw-r--r--  2.0 unx     1370 b- defN 23-Nov-21 06:27 dlrover/python/master/scaler/factory.py
--rw-r--r--  2.0 unx    24570 b- defN 24-Mar-07 06:35 dlrover/python/master/scaler/pod_scaler.py
+-rw-r--r--  2.0 unx    24649 b- defN 24-Apr-16 02:09 dlrover/python/master/scaler/pod_scaler.py
 -rw-r--r--  2.0 unx     4659 b- defN 23-Nov-23 02:06 dlrover/python/master/scaler/ray_scaler.py
 -rw-r--r--  2.0 unx      599 b- defN 23-Mar-07 11:16 dlrover/python/master/shard/__init__.py
 -rw-r--r--  2.0 unx     4574 b- defN 23-Nov-07 07:11 dlrover/python/master/shard/base_dataset_manager.py
 -rw-r--r--  2.0 unx     6964 b- defN 23-Nov-07 07:11 dlrover/python/master/shard/batch_dataset_manager.py
 -rw-r--r--  2.0 unx    16305 b- defN 24-Jan-30 06:31 dlrover/python/master/shard/dataset_splitter.py
 -rw-r--r--  2.0 unx     7064 b- defN 24-Jan-11 07:28 dlrover/python/master/shard/streaming_dataset_manager.py
--rw-r--r--  2.0 unx    11171 b- defN 24-Jan-11 07:19 dlrover/python/master/shard/task_manager.py
+-rw-r--r--  2.0 unx    11152 b- defN 24-Apr-01 02:35 dlrover/python/master/shard/task_manager.py
 -rw-r--r--  2.0 unx      599 b- defN 23-Mar-07 11:16 dlrover/python/master/stats/__init__.py
 -rw-r--r--  2.0 unx     6444 b- defN 23-Nov-21 06:27 dlrover/python/master/stats/job_collector.py
 -rw-r--r--  2.0 unx     8776 b- defN 24-Feb-20 02:57 dlrover/python/master/stats/reporter.py
 -rw-r--r--  2.0 unx     1567 b- defN 23-Mar-07 11:16 dlrover/python/master/stats/stats_backend.py
 -rw-r--r--  2.0 unx     4820 b- defN 23-Nov-21 06:27 dlrover/python/master/stats/training_metrics.py
 -rw-r--r--  2.0 unx      599 b- defN 23-Mar-07 11:16 dlrover/python/master/watcher/__init__.py
 -rw-r--r--  2.0 unx     1241 b- defN 23-Mar-07 11:16 dlrover/python/master/watcher/base_watcher.py
@@ -100,55 +101,56 @@
 -rw-r--r--  2.0 unx      599 b- defN 23-Mar-07 11:16 dlrover/python/scheduler/__init__.py
 -rw-r--r--  2.0 unx     1924 b- defN 23-Nov-21 06:27 dlrover/python/scheduler/factory.py
 -rw-r--r--  2.0 unx     4285 b- defN 24-Mar-29 02:24 dlrover/python/scheduler/job.py
 -rw-r--r--  2.0 unx    18558 b- defN 24-Mar-29 02:24 dlrover/python/scheduler/kubernetes.py
 -rw-r--r--  2.0 unx     7397 b- defN 23-Nov-21 06:27 dlrover/python/scheduler/ray.py
 -rw-r--r--  2.0 unx      599 b- defN 23-Mar-07 11:16 dlrover/python/tests/__init__.py
 -rw-r--r--  2.0 unx     2799 b- defN 24-Feb-06 01:58 dlrover/python/tests/test_agent_config_tuner.py
--rw-r--r--  2.0 unx     3405 b- defN 24-Mar-05 07:05 dlrover/python/tests/test_agent_monitor.py
+-rw-r--r--  2.0 unx     3405 b- defN 24-Apr-18 06:18 dlrover/python/tests/test_agent_monitor.py
 -rw-r--r--  2.0 unx     1049 b- defN 23-Mar-07 11:16 dlrover/python/tests/test_args.py
--rw-r--r--  2.0 unx     9327 b- defN 24-Feb-20 02:57 dlrover/python/tests/test_ckpt_saver.py
+-rw-r--r--  2.0 unx    10521 b- defN 24-Apr-23 06:44 dlrover/python/tests/test_ckpt_saver.py
 -rw-r--r--  2.0 unx     4583 b- defN 23-Nov-21 06:27 dlrover/python/tests/test_dataset_splitter.py
 -rw-r--r--  2.0 unx     4905 b- defN 23-Nov-21 06:27 dlrover/python/tests/test_dataset_task_manager.py
--rw-r--r--  2.0 unx    14821 b- defN 24-Mar-05 07:05 dlrover/python/tests/test_elastic_training_agent.py
+-rw-r--r--  2.0 unx    14928 b- defN 24-Apr-23 06:44 dlrover/python/tests/test_elastic_training_agent.py
 -rw-r--r--  2.0 unx     3383 b- defN 23-Nov-23 02:06 dlrover/python/tests/test_elasticjob_scaler.py
 -rw-r--r--  2.0 unx     1873 b- defN 23-Dec-22 03:13 dlrover/python/tests/test_env_utils.py
 -rw-r--r--  2.0 unx     1527 b- defN 24-Mar-12 05:23 dlrover/python/tests/test_error_monitor.py
 -rw-r--r--  2.0 unx     3635 b- defN 24-Mar-26 01:58 dlrover/python/tests/test_event_callback.py
 -rw-r--r--  2.0 unx     1268 b- defN 23-Nov-23 02:06 dlrover/python/tests/test_global_context.py
 -rw-r--r--  2.0 unx     2158 b- defN 23-Dec-26 03:16 dlrover/python/tests/test_grpc_utils.py
 -rw-r--r--  2.0 unx     5292 b- defN 23-Dec-21 04:12 dlrover/python/tests/test_job_auto_scaler.py
 -rw-r--r--  2.0 unx    21350 b- defN 24-Mar-21 07:24 dlrover/python/tests/test_job_manager.py
 -rw-r--r--  2.0 unx     2183 b- defN 23-Nov-21 06:27 dlrover/python/tests/test_job_params.py
 -rw-r--r--  2.0 unx     3188 b- defN 24-Mar-12 05:23 dlrover/python/tests/test_k8s_utils.py
 -rw-r--r--  2.0 unx     5920 b- defN 24-Feb-20 02:57 dlrover/python/tests/test_k8s_watcher.py
 -rw-r--r--  2.0 unx     9142 b- defN 23-Dec-21 04:12 dlrover/python/tests/test_local_optimizer.py
 -rw-r--r--  2.0 unx     5449 b- defN 24-Mar-05 07:32 dlrover/python/tests/test_master.py
--rw-r--r--  2.0 unx     5318 b- defN 24-Feb-27 07:38 dlrover/python/tests/test_master_client.py
--rw-r--r--  2.0 unx     3476 b- defN 24-Feb-06 01:58 dlrover/python/tests/test_multi_process.py
+-rw-r--r--  2.0 unx     5455 b- defN 24-Apr-16 02:09 dlrover/python/tests/test_master_client.py
+-rw-r--r--  2.0 unx     3773 b- defN 24-Apr-23 06:44 dlrover/python/tests/test_multi_process.py
+-rw-r--r--  2.0 unx     1816 b- defN 24-Apr-23 06:44 dlrover/python/tests/test_net_topology.py
 -rw-r--r--  2.0 unx     1943 b- defN 24-Feb-21 09:03 dlrover/python/tests/test_node.py
--rw-r--r--  2.0 unx     9260 b- defN 24-Mar-07 06:35 dlrover/python/tests/test_pod_scaler.py
+-rw-r--r--  2.0 unx     9506 b- defN 24-Apr-16 02:09 dlrover/python/tests/test_pod_scaler.py
 -rw-r--r--  2.0 unx     7411 b- defN 23-Nov-21 06:27 dlrover/python/tests/test_ps_manager.py
 -rw-r--r--  2.0 unx      599 b- defN 23-Mar-07 11:16 dlrover/python/tests/test_ray_client.py
 -rw-r--r--  2.0 unx     1976 b- defN 23-Nov-23 02:06 dlrover/python/tests/test_ray_job_args.py
 -rw-r--r--  2.0 unx      971 b- defN 23-Nov-21 06:27 dlrover/python/tests/test_ray_scaler.py
 -rw-r--r--  2.0 unx      599 b- defN 23-Mar-07 11:16 dlrover/python/tests/test_ray_watcher.py
--rw-r--r--  2.0 unx    12111 b- defN 23-Dec-21 04:12 dlrover/python/tests/test_rdzv_manager.py
+-rw-r--r--  2.0 unx    12564 b- defN 24-Apr-16 02:09 dlrover/python/tests/test_rdzv_manager.py
 -rw-r--r--  2.0 unx    11635 b- defN 23-Dec-21 04:12 dlrover/python/tests/test_resource_optimizer.py
--rw-r--r--  2.0 unx    17947 b- defN 24-Mar-04 05:56 dlrover/python/tests/test_servicer.py
+-rw-r--r--  2.0 unx    18420 b- defN 24-Apr-09 01:37 dlrover/python/tests/test_servicer.py
 -rw-r--r--  2.0 unx     3687 b- defN 23-Dec-21 04:12 dlrover/python/tests/test_sharding_client.py
--rw-r--r--  2.0 unx     1783 b- defN 23-Nov-21 06:27 dlrover/python/tests/test_speed_monitor.py
+-rw-r--r--  2.0 unx     1783 b- defN 24-Apr-01 02:29 dlrover/python/tests/test_speed_monitor.py
 -rw-r--r--  2.0 unx     1344 b- defN 23-Mar-07 11:16 dlrover/python/tests/test_state_backend.py
 -rw-r--r--  2.0 unx     3287 b- defN 24-Feb-06 01:58 dlrover/python/tests/test_stats_collector.py
 -rw-r--r--  2.0 unx     2703 b- defN 24-Feb-06 06:42 dlrover/python/tests/test_storage.py
 -rw-r--r--  2.0 unx     3303 b- defN 23-Nov-21 06:27 dlrover/python/tests/test_strategy_generator.py
 -rw-r--r--  2.0 unx     2460 b- defN 23-Nov-21 06:27 dlrover/python/tests/test_sync_service.py
 -rw-r--r--  2.0 unx     5425 b- defN 23-Dec-21 04:12 dlrover/python/tests/test_task_manager.py
--rw-r--r--  2.0 unx     8568 b- defN 24-Feb-23 09:24 dlrover/python/tests/test_utils.py
--rw-r--r--  2.0 unx     7206 b- defN 23-Dec-21 04:12 dlrover/python/tests/test_worker_manager.py
+-rw-r--r--  2.0 unx     8599 b- defN 24-Apr-18 06:28 dlrover/python/tests/test_utils.py
+-rw-r--r--  2.0 unx     7354 b- defN 24-Apr-23 06:44 dlrover/python/tests/test_worker_manager.py
 -rw-r--r--  2.0 unx      599 b- defN 23-Mar-07 11:16 dlrover/python/util/__init__.py
 -rw-r--r--  2.0 unx     3856 b- defN 23-Mar-07 11:16 dlrover/python/util/reflect_util.py
 -rw-r--r--  2.0 unx      599 b- defN 23-Mar-07 11:16 dlrover/python/util/actor_util/__init__.py
 -rw-r--r--  2.0 unx     1552 b- defN 23-Mar-07 11:16 dlrover/python/util/actor_util/parse_actor.py
 -rw-r--r--  2.0 unx      599 b- defN 23-Mar-07 11:16 dlrover/python/util/queue/__init__.py
 -rw-r--r--  2.0 unx     2834 b- defN 23-Mar-07 11:16 dlrover/python/util/queue/queue.py
 -rw-r--r--  2.0 unx      599 b- defN 23-Mar-07 11:16 dlrover/python/util/state/__init__.py
@@ -191,45 +193,46 @@
 -rw-r--r--  2.0 unx     5429 b- defN 23-Nov-07 07:11 dlrover/trainer/tensorflow/util/dataset_util.py
 -rw-r--r--  2.0 unx     8506 b- defN 23-Nov-07 07:11 dlrover/trainer/tensorflow/util/estimator_util.py
 -rw-r--r--  2.0 unx     1122 b- defN 23-Mar-07 11:16 dlrover/trainer/tensorflow/util/path_util.py
 -rw-r--r--  2.0 unx     1598 b- defN 23-May-08 02:53 dlrover/trainer/tensorflow/util/tf_env_util.py
 -rw-r--r--  2.0 unx    15226 b- defN 23-Nov-07 07:11 dlrover/trainer/tensorflow/util/tf_patch_util.py
 -rw-r--r--  2.0 unx     1104 b- defN 23-Mar-07 11:16 dlrover/trainer/tensorflow/util/tf_version_util.py
 -rw-r--r--  2.0 unx      599 b- defN 23-Jun-30 07:14 dlrover/trainer/torch/__init__.py
--rw-r--r--  2.0 unx    11797 b- defN 24-Mar-26 01:58 dlrover/trainer/torch/elastic_run.py
+-rw-r--r--  2.0 unx    11832 b- defN 24-Apr-18 02:40 dlrover/trainer/torch/elastic_run.py
 -rw-r--r--  2.0 unx      690 b- defN 23-Nov-07 07:11 dlrover/trainer/torch/main.py
 -rw-r--r--  2.0 unx      599 b- defN 23-Nov-21 06:27 dlrover/trainer/torch/elastic/__init__.py
 -rw-r--r--  2.0 unx     5422 b- defN 23-Nov-21 06:27 dlrover/trainer/torch/elastic/dataloader.py
--rw-r--r--  2.0 unx     5981 b- defN 23-Nov-21 06:27 dlrover/trainer/torch/elastic/sampler.py
+-rw-r--r--  2.0 unx     5981 b- defN 24-Apr-09 12:05 dlrover/trainer/torch/elastic/sampler.py
 -rw-r--r--  2.0 unx    11244 b- defN 24-Mar-26 08:26 dlrover/trainer/torch/elastic/trainer.py
 -rw-r--r--  2.0 unx      599 b- defN 23-Dec-22 03:13 dlrover/trainer/torch/flash_checkpoint/__init__.py
 -rw-r--r--  2.0 unx     2534 b- defN 24-Jan-10 08:04 dlrover/trainer/torch/flash_checkpoint/checkpointer.py
--rw-r--r--  2.0 unx     4189 b- defN 24-Mar-26 09:59 dlrover/trainer/torch/flash_checkpoint/ddp.py
--rw-r--r--  2.0 unx     7857 b- defN 24-Mar-18 03:05 dlrover/trainer/torch/flash_checkpoint/ddp_engine.py
--rw-r--r--  2.0 unx     8784 b- defN 24-Jan-31 07:40 dlrover/trainer/torch/flash_checkpoint/deepspeed.py
--rw-r--r--  2.0 unx     6101 b- defN 24-Feb-01 04:17 dlrover/trainer/torch/flash_checkpoint/deepspeed_engine.py
--rw-r--r--  2.0 unx    14158 b- defN 24-Mar-20 07:51 dlrover/trainer/torch/flash_checkpoint/engine.py
--rw-r--r--  2.0 unx     3961 b- defN 24-Jan-26 09:04 dlrover/trainer/torch/flash_checkpoint/fsdp.py
+-rw-r--r--  2.0 unx     4247 b- defN 24-Apr-23 06:44 dlrover/trainer/torch/flash_checkpoint/ddp.py
+-rw-r--r--  2.0 unx     8646 b- defN 24-Apr-23 06:44 dlrover/trainer/torch/flash_checkpoint/deepspeed.py
+-rw-r--r--  2.0 unx     6280 b- defN 24-Apr-23 06:44 dlrover/trainer/torch/flash_checkpoint/deepspeed_engine.py
+-rw-r--r--  2.0 unx    14280 b- defN 24-Apr-23 06:44 dlrover/trainer/torch/flash_checkpoint/engine.py
+-rw-r--r--  2.0 unx    10397 b- defN 24-Apr-23 06:44 dlrover/trainer/torch/flash_checkpoint/fsdp.py
 -rw-r--r--  2.0 unx    19976 b- defN 24-Feb-01 02:40 dlrover/trainer/torch/flash_checkpoint/fsdp_engine.py
+-rw-r--r--  2.0 unx     7885 b- defN 24-Apr-23 06:44 dlrover/trainer/torch/flash_checkpoint/full_ckpt_engine.py
+-rw-r--r--  2.0 unx    14246 b- defN 24-Apr-23 06:44 dlrover/trainer/torch/flash_checkpoint/hf_trainer.py
 -rw-r--r--  2.0 unx     7823 b- defN 24-Feb-20 02:57 dlrover/trainer/torch/flash_checkpoint/megatron.py
--rw-r--r--  2.0 unx    19611 b- defN 24-Mar-26 01:58 dlrover/trainer/torch/flash_checkpoint/megatron_dist_ckpt.py
--rw-r--r--  2.0 unx     9780 b- defN 24-Mar-20 07:51 dlrover/trainer/torch/flash_checkpoint/megatron_engine.py
+-rw-r--r--  2.0 unx    20464 b- defN 24-Apr-23 06:44 dlrover/trainer/torch/flash_checkpoint/megatron_dist_ckpt.py
+-rw-r--r--  2.0 unx     9626 b- defN 24-Apr-23 06:44 dlrover/trainer/torch/flash_checkpoint/megatron_engine.py
 -rw-r--r--  2.0 unx      599 b- defN 24-Mar-11 07:21 dlrover/trainer/torch/node_check/__init__.py
 -rw-r--r--  2.0 unx     1645 b- defN 24-Mar-12 05:23 dlrover/trainer/torch/node_check/ascend_npu.py
 -rw-r--r--  2.0 unx     1373 b- defN 24-Mar-12 05:23 dlrover/trainer/torch/node_check/nvidia_gpu.py
--rw-r--r--  2.0 unx     2890 b- defN 24-Mar-12 05:23 dlrover/trainer/torch/node_check/utils.py
+-rw-r--r--  2.0 unx     2890 b- defN 24-Apr-18 07:29 dlrover/trainer/torch/node_check/utils.py
 -rw-r--r--  2.0 unx      599 b- defN 23-Mar-07 11:16 dlrover/trainer/util/__init__.py
 -rw-r--r--  2.0 unx     2031 b- defN 23-Mar-07 11:16 dlrover/trainer/util/args_util.py
 -rw-r--r--  2.0 unx     6436 b- defN 24-Feb-20 02:57 dlrover/trainer/util/conf_util.py
 -rw-r--r--  2.0 unx     2863 b- defN 23-Mar-07 11:16 dlrover/trainer/util/log_util.py
 -rw-r--r--  2.0 unx      736 b- defN 23-Mar-07 11:16 dlrover/trainer/util/net_util.py
 -rw-r--r--  2.0 unx     3860 b- defN 23-Mar-07 11:16 dlrover/trainer/util/reflect_util.py
 -rw-r--r--  2.0 unx      599 b- defN 23-Mar-07 11:16 dlrover/trainer/worker/__init__.py
 -rw-r--r--  2.0 unx     3540 b- defN 23-Nov-07 07:11 dlrover/trainer/worker/tf_kubernetes_worker.py
 -rw-r--r--  2.0 unx     6927 b- defN 23-Nov-23 02:06 dlrover/trainer/worker/tf_ray_worker.py
--rw-r--r--  2.0 unx    13484 b- defN 24-Mar-29 05:54 dlrover-0.3.5.dist-info/LICENSE
--rw-r--r--  2.0 unx     1008 b- defN 24-Mar-29 05:54 dlrover-0.3.5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Mar-29 05:54 dlrover-0.3.5.dist-info/WHEEL
--rw-r--r--  2.0 unx       65 b- defN 24-Mar-29 05:54 dlrover-0.3.5.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        8 b- defN 24-Mar-29 05:54 dlrover-0.3.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx    22914 b- defN 24-Mar-29 05:54 dlrover-0.3.5.dist-info/RECORD
-233 files, 1234653 bytes uncompressed, 350790 bytes compressed:  71.6%
+-rw-r--r--  2.0 unx    13484 b- defN 24-Apr-24 06:10 dlrover-0.3.6.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1008 b- defN 24-Apr-24 06:10 dlrover-0.3.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-24 06:10 dlrover-0.3.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx       65 b- defN 24-Apr-24 06:10 dlrover-0.3.6.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        8 b- defN 24-Apr-24 06:10 dlrover-0.3.6.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx    23241 b- defN 24-Apr-24 06:10 dlrover-0.3.6.dist-info/RECORD
+236 files, 1269758 bytes uncompressed, 359585 bytes compressed:  71.7%
```

## zipnote {}

```diff
@@ -153,14 +153,17 @@
 
 Filename: dlrover/python/master/elastic_training/elastic_ps.py
 Comment: 
 
 Filename: dlrover/python/master/elastic_training/kv_store_service.py
 Comment: 
 
+Filename: dlrover/python/master/elastic_training/net_topology.py
+Comment: 
+
 Filename: dlrover/python/master/elastic_training/rdzv_manager.py
 Comment: 
 
 Filename: dlrover/python/master/elastic_training/sync_service.py
 Comment: 
 
 Filename: dlrover/python/master/hyperparams/__init__.py
@@ -372,14 +375,17 @@
 
 Filename: dlrover/python/tests/test_master_client.py
 Comment: 
 
 Filename: dlrover/python/tests/test_multi_process.py
 Comment: 
 
+Filename: dlrover/python/tests/test_net_topology.py
+Comment: 
+
 Filename: dlrover/python/tests/test_node.py
 Comment: 
 
 Filename: dlrover/python/tests/test_pod_scaler.py
 Comment: 
 
 Filename: dlrover/python/tests/test_ps_manager.py
@@ -609,17 +615,14 @@
 
 Filename: dlrover/trainer/torch/flash_checkpoint/checkpointer.py
 Comment: 
 
 Filename: dlrover/trainer/torch/flash_checkpoint/ddp.py
 Comment: 
 
-Filename: dlrover/trainer/torch/flash_checkpoint/ddp_engine.py
-Comment: 
-
 Filename: dlrover/trainer/torch/flash_checkpoint/deepspeed.py
 Comment: 
 
 Filename: dlrover/trainer/torch/flash_checkpoint/deepspeed_engine.py
 Comment: 
 
 Filename: dlrover/trainer/torch/flash_checkpoint/engine.py
@@ -627,14 +630,20 @@
 
 Filename: dlrover/trainer/torch/flash_checkpoint/fsdp.py
 Comment: 
 
 Filename: dlrover/trainer/torch/flash_checkpoint/fsdp_engine.py
 Comment: 
 
+Filename: dlrover/trainer/torch/flash_checkpoint/full_ckpt_engine.py
+Comment: 
+
+Filename: dlrover/trainer/torch/flash_checkpoint/hf_trainer.py
+Comment: 
+
 Filename: dlrover/trainer/torch/flash_checkpoint/megatron.py
 Comment: 
 
 Filename: dlrover/trainer/torch/flash_checkpoint/megatron_dist_ckpt.py
 Comment: 
 
 Filename: dlrover/trainer/torch/flash_checkpoint/megatron_engine.py
@@ -675,26 +684,26 @@
 
 Filename: dlrover/trainer/worker/tf_kubernetes_worker.py
 Comment: 
 
 Filename: dlrover/trainer/worker/tf_ray_worker.py
 Comment: 
 
-Filename: dlrover-0.3.5.dist-info/LICENSE
+Filename: dlrover-0.3.6.dist-info/LICENSE
 Comment: 
 
-Filename: dlrover-0.3.5.dist-info/METADATA
+Filename: dlrover-0.3.6.dist-info/METADATA
 Comment: 
 
-Filename: dlrover-0.3.5.dist-info/WHEEL
+Filename: dlrover-0.3.6.dist-info/WHEEL
 Comment: 
 
-Filename: dlrover-0.3.5.dist-info/entry_points.txt
+Filename: dlrover-0.3.6.dist-info/entry_points.txt
 Comment: 
 
-Filename: dlrover-0.3.5.dist-info/top_level.txt
+Filename: dlrover-0.3.6.dist-info/top_level.txt
 Comment: 
 
-Filename: dlrover-0.3.5.dist-info/RECORD
+Filename: dlrover-0.3.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## dlrover/python/common/grpc.py

```diff
@@ -322,30 +322,35 @@
 @dataclass
 class RendezvousRequest(Message):
     node_id: int = 0
     local_world_size: int = 0
     rdzv_name: str = ""
 
 
+@dataclass
 class CommWorldRequest(RendezvousRequest):
     pass
 
 
+@dataclass
 class JoinRendezvousRequest(RendezvousRequest):
-    pass
+    node_ip: str = ""  # The IP of node where the pod is located.
 
 
+@dataclass
 class WaitingNodeNumRequest(RendezvousRequest):
     pass
 
 
+@dataclass
 class NetworkReadyRequest(Message):
     pass
 
 
+@dataclass
 class StragglerExistRequest(Message):
     pass
 
 
 @dataclass
 class NetworkCheckResult(Message):
     nodes: List[int] = field(default_factory=list)
@@ -437,7 +442,12 @@
 
 
 @dataclass
 class ParallelConfig(Message):
     dataloader: DataLoaderConfig = DataLoaderConfig()
     optimizer: OptimizerConfig = OptimizerConfig()
     restart: bool = False
+
+
+@dataclass
+class NodeCheckpointState(Message):
+    step: int = 0
```

## dlrover/python/common/multi_process.py

```diff
@@ -78,24 +78,15 @@
     Create a socket client.
 
     Args:
         path (str): a file path.
 
     """
     client = socket.socket(socket.AF_UNIX, socket.SOCK_STREAM)
-    connected = False
-    for _ in range(30):
-        try:
-            client.connect(path)
-            connected = True
-            break
-        except (FileNotFoundError, ConnectionRefusedError):
-            time.sleep(0.5)
-    if not connected:
-        client.connect(path)
+    client.connect(path)
     return client
 
 
 def _socket_send(socket: socket.socket, message):
     """
     In the protocol, the first 4 bytes is the size of message.
     """
@@ -470,54 +461,58 @@
             sending process to update its dict.
     """
 
     def __init__(self, name="", create=False):
         super().__init__(name, create)
 
         self._dict = {}
+
+        # The queue is used to notify the saver waiting for a new dict.
         self._shared_queue = SharedQueue(
             name=f"shard_dict_{name}", create=self._create
         )
 
     def _sync(self):
         while True:
             connection, _ = self._server.accept()
             try:
                 recv_data = _socket_recv(connection)
                 msg: SocketRequest = pickle.loads(recv_data)
                 response = DictMessage()
                 if msg.method == "set":
                     self.set(**msg.args)
-                    self._shared_queue.get(1)
                 elif msg.method == "get":
                     response = DictMessage()
                     response.meta_dict = self.get(**msg.args)
                 response.status = SUCCESS_CODE
-            except Exception:
+            except Exception as e:
                 response = SocketResponse()
                 response.status = ERROR_CODE
+                logger.error(e)
+            finally:
+                if not self._shared_queue.empty():
+                    self._shared_queue.get(1)
             message = pickle.dumps(response)
             _socket_send(connection, message)
 
     def set(self, new_dict):
         """
         Set the dict to the remote shared dict.
 
         Args:
             new_dict (dict): a new dict to set.
         """
         self._dict = new_dict
         if not self._server:
             args = {"new_dict": self._dict}
             request = SocketRequest(method="set", args=args)
-            try:
-                self._shared_queue.put(1)
-                self._request(request)
-            except Exception:
-                logger.info("The recv process has breakdown.")
+            self._shared_queue.put(1)
+            response = self._request(request)
+            if response.status == ERROR_CODE:
+                raise RuntimeError("Fail to set metadata!")
 
     def get(self, local=False):
         """
         Returns a Python Dict from the remote shared Dict.
 
         If the writing instance sends the dict into the FIFO, the get method
         should wait for the sync thread to update the dict.
```

## dlrover/python/elastic_agent/master_client.py

```diff
@@ -28,19 +28,18 @@
     def wrapper(self, *args, **kwargs):
         retry = kwargs.get("retry", 10)
         execption = None
         for i in range(retry):
             try:
                 return func(self, *args, **kwargs)
             except Exception as e:
+                class_name = self.__class__.__name__
+                func_name = func.__name__
                 logger.warning(
-                    "Retry %s to %s.%s with failure",
-                    i,
-                    self.__class__.__name__,
-                    func.__name__,
+                    f"Retry {i} to {class_name}.{func_name} with failure",
                 )
                 execption = e
                 time.sleep(5)
         if execption:
             logger.error(execption)
             raise execption
 
@@ -73,18 +72,17 @@
         self._timeout = timeout
         self._master_addr = master_addr
         self._channel = grpc.build_channel(master_addr)
         logger.info("dlrover master addr is %s" % self._master_addr)
         self._stub = elastic_training_pb2_grpc.MasterStub(self._channel)
         self._node_id = node_id
         self._node_type = node_type
-        self._host = os.getenv("POD_IP", "localhost")
+        self._node_ip = os.getenv("NODE_IP", "")
         self._worker_local_process_id = int(os.getenv("LOCAL_RANK", 0))
         self._ddp_server_port = self.find_free_port()
-        self._host_name = os.getenv("POD_NAME", "")
 
     def __del__(self):
         if self._channel:
             self._channel.close()
 
     def close_channel(self):
         if self._channel:
@@ -99,15 +97,15 @@
             socket.socket(socket.AF_INET, socket.SOCK_STREAM)
         ) as sock:
             sock.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
             sock.bind(("localhost", 0))
             _, port = sock.getsockname()
             return port
 
-    # @retry_grpc_request
+    @retry_grpc_request
     def _report(self, message: grpc.Message):
         request = elastic_training_pb2.Message()
         request.node_id = self._node_id
         request.node_type = self._node_type
         request.data = message.serialize()
         return self._stub.report(request, timeout=self._timeout)
 
@@ -310,14 +308,15 @@
             return 0
 
     def join_rendezvous(self, node_rank, local_world_size, rdzv_name=""):
         request = grpc.JoinRendezvousRequest(
             node_id=node_rank,
             local_world_size=local_world_size,
             rdzv_name=rdzv_name,
+            node_ip=self._node_ip,
         )
         result: grpc.RendezvousState = self._get(request)
         return result.round
 
     def get_comm_world(self, rdzv_name, node_rank):
         request = grpc.CommWorldRequest(node_id=node_rank, rdzv_name=rdzv_name)
         result: grpc.RendezvousState = self._get(request)
@@ -386,14 +385,20 @@
         try:
             result: grpc.ParallelConfig = self._get(request)
             return result.restart
         except Exception:
             logger.warning("Fail to verify restarting training processes.")
             return False
 
+    def sync_checkpoint(self, step):
+        request = grpc.NodeCheckpointState()
+        request.step = step
+        response = self._report(request)
+        return response.success
+
     @classmethod
     def singleton_instance(cls, *args, **kwargs):
         if not cls._instance:
             with cls._instance_lock:
                 if not cls._instance:
                     cls._instance = build_master_client(*args, **kwargs)
         return cls._instance
```

## dlrover/python/elastic_agent/torch/ckpt_saver.py

```diff
@@ -32,14 +32,15 @@
 from dlrover.python.common.multi_process import (
     SharedDict,
     SharedLock,
     SharedMemory,
     SharedQueue,
 )
 from dlrover.python.common.serialize import ClassMeta
+from dlrover.python.elastic_agent.master_client import MasterClient
 
 DLROVER_CKPT_CONFIG_KEY = "_DLORVER_CKPT_CONFIG"
 
 
 class CheckpointSharedObjPrefix:
     SAVE_STEP_QNAME = "checkpoint_lock_rank_"
     META_NAME = "checkpoint_meta_"
@@ -229,14 +230,15 @@
             )
         else:
             self._shm_name = CheckpointSharedObjPrefix.SHM_NAME + str(
                 local_rank
             )
         self.shared_memory: Optional[SharedMemory] = None
         self.metadata = SharedDict(name=meta_name, create=host)
+        self._need_creation = True
 
     def close(self):
         if self.shared_memory:
             self.shared_memory.close()
 
     def unlink(self):
         if not self.shared_memory:
@@ -244,15 +246,15 @@
             self.init_shared_memory()
         if self.shared_memory:
             self.shared_memory.unlink()
         if self.metadata:
             self.metadata.unlink()
 
     def reset(self):
-        self.shared_memory = None
+        self._need_creation = True
 
     def _create_tensor_meta(self, value: torch.Tensor):
         """
         Create a tensor meta of a tensor and compute the total
         size of the state dict.
         """
         if not torch.is_tensor(value):
@@ -296,15 +298,15 @@
                 the second value is the state dict.
         """
         meta_dict = self.metadata.get()
         default_config = CheckpointConfig()
         config = meta_dict.get(DLROVER_CKPT_CONFIG_KEY, default_config)
         if not meta_dict or config.writing_shm:
             return {}
-        if self.shared_memory is None:
+        if self.shared_memory is None or self._need_creation:
             self.init_shared_memory(create=False)
         if not self.shared_memory:
             return {}
 
         state_dict = _read_state_dict_from_shm(meta_dict, self.shared_memory)
         return state_dict
 
@@ -320,14 +322,15 @@
             return True
         return False
 
     def init_shared_memory(self, create=False, size=0):
         self.shared_memory = _create_shared_memory(
             self._shm_name, create=create, size=size
         )
+        self._need_creation = False
 
     def get_checkpoint_config(self, default_config):
         """
         Get the configuration of checkpointing state dict in the shared
         memory.
 
         Returns:
@@ -484,14 +487,21 @@
                 cls._saver_instance.close()
             if callable(sigterm_handler):
                 sigterm_handler(signum, frame)
 
         signal.signal(signal.SIGINT, _clean_shm_handler)
         signal.signal(signal.SIGTERM, _save_shm_before_exiting)
 
+    def wait_saving_checkpoint(self):
+        """
+        Check whether the saver finishes writing the
+        latest checkpoint to the storage.
+        """
+        return self._writing_storage
+
     def close(self):
         """Clear the resource of the shared objects."""
         event = CheckpointEvent(type=CheckpointEventType.EXIT)
         if not self._event_queue.empty():
             self._event_queue._queue.get()
         self._event_queue.put(event)
         for i in range(self.local_shard_num):
@@ -508,30 +518,28 @@
         buffer into the storage.
         """
         logger.info("Async flash checkpoint saver starts!")
         while True:
             event: CheckpointEvent = self._event_queue.get()
             if event.type == CheckpointEventType.UPDATE_SHARD:
                 logger.info(
-                    "Reset the shared memory after the training starts."
+                    "Reset the shared memory after the training starts. "
                     f"The number of global shards is {event.global_shard_num}."
                 )
                 self.global_shard_num = event.global_shard_num
             elif event.type == CheckpointEventType.SAVE:
                 logger.info(
                     f"ShardingSaver save checkpoint to storage, event {event}"
                 )
                 self.save_step_checkpoint(event.step)
             elif event.type == CheckpointEventType.EXIT:
                 break
 
     def reset_shared_memory(self):
         self._stop_commit = True
-        for lock in self._shm_locks:
-            lock.release()
         for shm_handler in self._shm_handlers:
             shm_handler.reset()
 
     def _save_shard(
         self,
         step,
         local_shard_id: int,
@@ -616,61 +624,96 @@
             if all(i == step for i in steps):
                 return True
             time.sleep(1)
             if time.time() - start_time > timeout:
                 logger.info(f"The cached steps are {steps}")
                 return False
 
-    def save_shm_to_storage(self, timeout=120):
+    def save_shm_to_storage(self, timeout=60, master_client=None):
         """
         Save the state dict in the shared memory into the storage. The agent
         can call the method to save the state dict into the storage if the
         training process fails or the agent wants to restart training
         processes.
         """
         if any(
             [handler.no_checkpint_state() for handler in self._shm_handlers]
         ):
             logger.info(
                 "Skip because no any memory buffer with the state dict."
             )
             return
 
-        if self._writing_storage:
-            logger.info("Saver is writing to storage, waiting...")
-            start = time.time()
-            while self._writing_storage:
-                time.sleep(2)
-                elapsed_time = time.time() - start
-                if elapsed_time > timeout:
-                    logger.error("Saver writing to storage, timeout")
-                    return
-        if self._any_rank_locked():
-            # The training process does not release the lock because it fails
-            # when writing the state dict into the shared memory. The shared
-            # memory may be dirty and the saver cannot save it to the storage.
-            return
+        # Skip saving checkpiont if the step of checkpoint shard in the
+        # memory is not same.
         steps = []
         for shm_handler in self._shm_handlers:
             default_config = CheckpointConfig()
             config = shm_handler.get_checkpoint_config(default_config)
             steps.append(config.step)
         if len(set(steps)) > 1:
             logger.error(
                 "Skip because steps in shards are not "
                 f"inconsistent: {steps}"
             )
             return
+
         step = steps[0]
+        if master_client:
+            # If some nodes failed, the alive nodes do not need to save its
+            # checkpoint shards because some shards of failed node are missing.
+            synced = self._sync_node_checkpoint(master_client, step, timeout)
+            if not synced:
+                logger.info(
+                    "Skip saving the checkpoint from "
+                    "the memory to the storage."
+                )
+                self._stop_commit = True
+                return
+
+        # The training process does not release the lock because it fails
+        # when writing the state dict into the shared memory. The shared
+        # memory may be dirty and the saver cannot save it to the storage.
+        if self._writing_storage or self._any_rank_locked():
+            logger.info(
+                "Saver is writing the checkpoint to storage "
+                "and skips saving at the breakpoint."
+            )
+            return
+
         if step > self._latest_step:
             self.save_step_checkpoint(step)
             logger.info(
                 "Save the checkpointing state dict from the shared "
                 f"memory to storage, step: {step}."
             )
+        else:
+            logger.info(f"The checkpoint of step {step} has been saved.")
+
+    def _sync_node_checkpoint(
+        self, master_client: MasterClient, step: int, timeout: int
+    ):
+        """
+        Check whether all training node can save the checkpoint from the memory
+        to the storage. If some nodes fail, other nodes needs not to save
+        """
+        start = time.time()
+        while True:
+            success = master_client.sync_checkpoint(step)
+            if success:
+                return success
+            else:
+                time.sleep(3)
+                elapsed_time = time.time() - start
+                if elapsed_time > timeout:
+                    logger.info(
+                        "It is timeout to sync checkpoint "
+                        "bacause some nodes may fail."
+                    )
+                    return False
 
     @classmethod
     def reset(cls):
         """Reset the shared memory of all shards."""
         if cls._saver_instance is None:
             return
         cls._saver_instance.reset_shared_memory()
```

## dlrover/python/elastic_agent/torch/training.py

```diff
@@ -10,20 +10,20 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import copy
 import functools
 import json
 import os
+import shutil
 import signal
 import socket
 import tempfile
 import time
 import uuid
-from concurrent.futures import ThreadPoolExecutor
 from dataclasses import dataclass
 from datetime import datetime, timedelta
 from typing import Any, Callable, Dict, List, Optional, Union
 
 import torch
 import torch.distributed.elastic.timer as timer
 from torch.distributed import PrefixStore, Store
@@ -79,14 +79,17 @@
     from torch_npu.contrib import transfer_to_npu  # noqa: F401
 except (ModuleNotFoundError, ImportError):  # noqa: F841
     pass
 
 __all__ = ["launch_agent"]
 
 
+_DEFAULT_INTERVAL = 5
+
+
 def _set_paral_config():
     """
     Set up the directory and path for the parallelism configuration.
     """
     config_dir = os.path.dirname(ConfigPath.PARAL_CONFIG)
     os.makedirs(config_dir, exist_ok=True)
     os.environ[ConfigPath.ENV_PARAL_CONFIG] = ConfigPath.PARAL_CONFIG
@@ -262,30 +265,29 @@
                 else:
                     logger.info(
                         "The node is not in the world "
                         "and waits for more nodes."
                     )
                     if start_pending == 0:
                         start_pending = time.time()
-                    time.sleep(5)
+                    time.sleep(_DEFAULT_INTERVAL)
                     start_join = time.time()
                     if start_join - start_pending > self.pend_timeout:
                         raise TimeoutError(
                             f"Timeout {self.pend_timeout}s to wait more nodes"
                         )
                     continue
             elif time.time() - start_join > self.join_timeout:
                 timeout = self.join_timeout
                 err_msg = f"Timeout {timeout}s to complete rendezvous."
                 self._report_failure(
                     err_msg, level=TrainingExceptionLevel.RDZV_ERROR
                 )
                 raise TimeoutError(err_msg)
             time.sleep(3)
-        world = dict(sorted(world.items()))
         rank = list(world.keys()).index(self._node_rank)
         world_size = len(world)
         logger.info(
             f"The node {node_name} has joined round {round} of "
             f"the {self._name} rendezvous as rank {rank} in a world of size "
             f"{world_size}."
         )
@@ -378,17 +380,14 @@
         self._restart_count = 0
         self._remaining_failovers = self._remaining_restarts
         self._client = MasterClient.singleton_instance()
         if config.auto_tunning:
             self._paral_config_tuner = ParalConfigTuner.singleton_instance()
             self._paral_config_tuner.start()
 
-        self._save_ckpt_executor = ThreadPoolExecutor(max_workers=1)
-        self._save_ckpt_future = None
-
     @prof
     def _rendezvous(self, worker_group: WorkerGroup) -> None:
         r"""
         Runs rendezvous for the workers specified by worker spec.
         Assigns workers a new global rank and world size.
         Updates the rendezvous store for the worker group.
         """
@@ -582,14 +581,15 @@
             if state == WorkerState.SUCCEEDED:
                 logger.info(
                     f"[{role}] worker group successfully finished."
                     f" Waiting {self._exit_barrier_timeout} seconds "
                     "for other agents to finish."
                 )
                 self._exit_barrier()
+                self._wait_async_saver()
                 return run_result
             elif state in {WorkerState.UNHEALTHY, WorkerState.FAILED}:
                 logger.error(f"The worker fails with {run_result.failures}")
                 self._report_failure_to_master(run_result.failures)
                 self._save_ckpt_to_storage()
                 if self._remaining_failovers > 0:
                     logger.info(
@@ -607,24 +607,41 @@
                 # membership changes do not count as retries
                 if self._membership_changed(role, rdzv_handler):
                     self._save_ckpt_to_storage()
                     self._restart_workers(self._worker_group)
             else:
                 raise Exception(f"[{role}] Worker group in {state.name} state")
 
+    def _wait_async_saver(self):
+        """
+        The agent waits for saving the checkpoint from the shared memory
+        before exiting.
+        """
+        saver = AsyncCheckpointSaver.get_ckpt_saver()
+        if saver:
+            # Wait the saver finishes writing the checkpoint from the shared
+            # memory to the storage.
+            start_wait_time = time.time()
+            while saver.wait_saving_checkpoint():
+                time.sleep(_DEFAULT_INTERVAL)
+                wait_time = round(time.time() - start_wait_time, 2)
+                logger.info(
+                    "Wait for saving the checkpoint and "
+                    f"the waiting time is {wait_time}s."
+                )
+
     def _save_ckpt_to_storage(self):
         """
         The agent can save the checkpointing state dict in the shared
         memory into the storage before restarting training processes.
         """
         saver: AsyncCheckpointSaver = AsyncCheckpointSaver.get_ckpt_saver()
         if saver and self._config.save_at_breakpoint:
-            self._save_ckpt_future = self._save_ckpt_executor.submit(
-                saver.save_shm_to_storage
-            )
+            logger.info("Start saving checkpoint at the breakpoint.")
+            saver.save_shm_to_storage(master_client=self._client)
 
     def _stop_workers_to_restart(self):
         """
         The agent query from the dlrover job master to check whether to restart
         workers. If true, the agent firstly stops all workers.
         """
         restart = self._client.need_to_restart_training()
@@ -652,20 +669,14 @@
     def _restart_workers(self, worker_group: WorkerGroup):
         self._restart_count += 1
         self._remaining_restarts -= 1
         # Relase the shared memory lock before starting workers.
         AsyncCheckpointSaver.reset()
         super()._restart_workers(worker_group)
 
-    def _start_workers(self, worker_group: WorkerGroup):
-        if self._save_ckpt_future:
-            # Waiting the thread to save checkpoint finishes.
-            self._save_ckpt_future.result(timeout=600)
-        return super()._start_workers(worker_group)
-
     def _membership_changed(self, role, rdzv_handler: RendezvousHandler):
         # Timeout may happen when to query TCPStore.
         if self._config.network_check:
             num_nodes_waiting = self._client.num_nodes_waiting(
                 RendezvousName.NETWORK_CHECK
             )
         else:
@@ -676,18 +687,14 @@
                 f"[{role}] Detected {num_nodes_waiting} "
                 f"new nodes from group_rank={group_rank}; "
                 f"will restart worker group"
             )
             return True
         return False
 
-    def stop_executor(self):
-        """Shutdown the executor to save the checkpoint."""
-        self._save_ckpt_executor.shutdown()
-
 
 def launch_agent(
     config: ElasticLaunchConfig,
     entrypoint: Union[Callable, str, None],
     args: List[Any],
 ) -> Dict[int, Any]:
     if not config.run_id:
@@ -788,19 +795,18 @@
         raise
     except Exception:
         events.record(agent.get_event_failed())
         raise
     finally:
         if shutdown_rdzv:
             spec.rdzv_handler.shutdown()
-        agent.stop_executor()
         monitor.stop()
 
 
-class NetworkCheckElasticAgent(ElasticTrainingAgent):
+class NodeCheckElasticAgent(ElasticTrainingAgent):
     """
     An implementation of :py:class:`torchelastic.agent.server.ElasticAgent`
     that handles host-local workers. This agent will run 2 rounds allgather
     to check network available.
     Round 0: the job master splits nodes into groups and each group contains
         two nodes. The node in each group will execute an allgather task and
         report its result to the master. For example, a job has 4 nodes and
@@ -828,15 +834,15 @@
             config,
             entrypoint,
             spec,
             start_method,
             exit_barrier_timeout,
             log_dir,
         )
-        self._log_dir = log_dir or tempfile.mkdtemp(prefix="network_check_")
+        self._log_dir = log_dir or tempfile.mkdtemp(prefix="node_check_")
         self._check_round = 2
         self._config: ElasticLaunchConfig = config
 
     def run(self, role: str = DEFAULT_ROLE) -> bool:
         spec = self._worker_group.spec
         role = spec.role
 
@@ -844,15 +850,15 @@
             f"[{role}] starting workers for entrypoint: "
             f"{spec.get_entrypoint_name()}"
         )
         success = False
         fault_nodes = []
         stragglers = []
         for i in range(self._check_round):
-            result, elapsed_time = self._run_network_check()
+            result, elapsed_time = self._run_node_check()
             elapsed_time = round(elapsed_time, 3)
             logger.info(
                 f"Network check time of round {i} is {elapsed_time}"
                 f" and succeed is {result}."
             )
             status = NodeStatus.SUCCEEDED if result else NodeStatus.FAILED
             self._client.report_network_status(
@@ -890,63 +896,75 @@
             raise RuntimeError("This node is down.")
         elif self._node_rank in stragglers:
             logger.warn("This node is a straggler!")
             if self._config.exclude_straggler:
                 raise RuntimeError("The node is a straggler and exits.")
         return True
 
-    def _run_network_check(self, monitor_interval=3, timeout=300):
+    def _run_node_check(self, monitor_interval=3, timeout=300):
         self._initialize_workers(self._worker_group)
         start = time.time()
         succeed = False
+        output_dir = ConfigPath.NETWORK_CHECK_DATA_DIR
         while True:
             assert self._worker_group.state != WorkerState.INIT
             time.sleep(monitor_interval)
             run_result = self._monitor_workers(self._worker_group)
             state = run_result.state
             self._worker_group.state = state
             if state == WorkerState.HEALTHY:
                 if time.time() - start > timeout:
                     logger.error(f"Timeout {timeout} to check network.")
                     break
                 continue
-            elif state == WorkerState.SUCCEEDED:
+            elif state == WorkerState.SUCCEEDED or self._check_finished(
+                output_dir
+            ):
                 succeed = True
                 break
             else:
                 break
 
         if succeed:
-            elapsed_time = self._get_network_check_time()
+            elapsed_time = self._get_node_check_time(output_dir)
         else:
             elapsed_time = 3600
         return succeed, elapsed_time
 
-    def _get_network_check_time(self):
-        root = ConfigPath.NETWORK_CHECK_DATA_DIR
+    def _check_finished(self, result_dir):
+        if not os.path.exists(result_dir):
+            return False
+        num = len(os.listdir(result_dir))
+        self._worker_group.workers
+        return num == len(self._worker_group.workers)
+
+    def _get_node_check_time(self, result_dir):
         elapsed_time = 0
-        if not os.path.exists(root):
+        if not os.path.exists(result_dir):
             return elapsed_time
-        for filename in os.listdir(root):
-            path = os.path.join(root, filename)
+        for filename in os.listdir(result_dir):
+            path = os.path.join(result_dir, filename)
             with open(path, "r") as f:
                 data = f.read()
                 if not data:
                     continue
                 data = json.loads(data)
                 elapsed_time = max(elapsed_time, data.get("time", 0))
+        shutil.rmtree(dir, ignore_errors=True)
         return elapsed_time
 
 
 def network_check(
     config: ElasticLaunchConfig,
     entrypoint: Union[Callable, str, None],
     args: List[Any],
 ) -> bool:
     config = copy.deepcopy(config)
+
+    # Disable checking network when execute tasks to check network.
     config.network_check = False
     if not config.run_id:
         run_id = str(uuid.uuid4().int)
         logger.warning(
             f"config has no run_id, generated a random run_id: {run_id}"
         )
         config.run_id = run_id
@@ -993,15 +1011,15 @@
         args=tuple(args),
         rdzv_handler=rdzv_handler,
         max_restarts=0,
         monitor_interval=config.monitor_interval,
         master_addr=master_addr,
     )
 
-    agent = NetworkCheckElasticAgent(
+    agent = NodeCheckElasticAgent(
         node_rank=node_rank,
         config=config,
         entrypoint=entrypoint,
         spec=spec,
         start_method=config.start_method,
     )
```

## dlrover/python/master/local_master.py

```diff
@@ -105,13 +105,14 @@
     def stop(self):
         """
         Stop all the components.
         Make sure that the created services and components are shut down.
         """
         logger.info("Stopping master!")
         logger.info("Stopping RPC server!")
-        self._master_server.stop(grace=0.1)
+        self._master_server.stop(None)
+        # self._master_server.stop(grace=0.1)
         logger.info("RPC server stopped!")
         logger.info("Master stopped!")
 
     def request_stop(self, success, reason, msg=""):
         pass
```

## dlrover/python/master/servicer.py

```diff
@@ -106,16 +106,14 @@
             message = self._join_rendezvous(req_message)
         elif isinstance(req_message, grpc.WaitingNodeNumRequest):
             message = self._num_nodes_waiting(req_message.rdzv_name)
         elif isinstance(req_message, grpc.NetworkReadyRequest):
             message = self._check_fault_node()
         elif isinstance(req_message, grpc.StragglerExistRequest):
             message = self._check_straggler()
-        elif isinstance(req_message, grpc.JoinRendezvousRequest):
-            message = self._join_rendezvous(req_message)
         elif isinstance(req_message, grpc.CommWorldRequest):
             message = self._get_comm_world(req_message)
         elif isinstance(req_message, grpc.KeyValuePair):
             message = self._kv_store_get(req_message)
         elif isinstance(req_message, grpc.PsNodesRequest):
             message = self._query_ps_nodes()
         elif isinstance(req_message, grpc.TrainingStatusRequest):
@@ -232,15 +230,15 @@
         nodes, reason = rdzv_manager.get_straggler()
         res = grpc.NetworkCheckResult(nodes=nodes, reason=reason)
         return res
 
     def _join_rendezvous(self, request: grpc.JoinRendezvousRequest):
         rdzv_manager = self._rdzv_managers[request.rdzv_name]
         round = rdzv_manager.join_rendezvous(
-            request.node_id, request.local_world_size
+            request.node_id, request.local_world_size, request.node_ip
         )
         if request.rdzv_name == RendezvousName.NETWORK_CHECK:
             # The waiting node in the training rdzv should clear if
             # a worker join network-check rdzv.
             training_manager = self._rdzv_managers[
                 RendezvousName.ELASTIC_TRAINING
             ]
@@ -255,16 +253,16 @@
 
     def _get_comm_world(self, request: grpc.CommWorldRequest):
         rdzv_manager = self._rdzv_managers[request.rdzv_name]
         rdzv_round, group, nodes = rdzv_manager.get_comm_world(request.node_id)
         res = grpc.RendezvousState(world={})
         res.group = group
         res.round = rdzv_round
-        for rank_id, worker_num in nodes.items():
-            res.world[rank_id] = worker_num
+        for rank_id, meta in nodes.items():
+            res.world[rank_id] = meta.process_num
         return res
 
     def _kv_store_get(self, request: grpc.KeyValuePair):
         value = self._kv_store.get(request.key)
         res = grpc.KeyValuePair(request.key, value)
         return res
 
@@ -328,14 +326,16 @@
             success = self._ready_for_ps_relaunch()
         elif isinstance(message, grpc.KeyValuePair):
             success = self._kv_store_set(message)
         elif isinstance(message, grpc.ParallelConfig):
             success = self._report_paral_config(node_type, node_id, message)
         elif isinstance(message, grpc.HeartBeat):
             success = self._report_heartbeat(node_type, node_id, message)
+        elif isinstance(message, grpc.NodeCheckpointState):
+            success = self._sync_checkpoint(node_type, node_id, message)
 
         response.success = success
         return response
 
     def _ready_for_ps_relaunch(self):
         self._job_manager.post_ps_ready()
         return True
@@ -562,14 +562,22 @@
         self._job_manager.collect_node_heart_beat(
             node_type,
             node_id,
             message.timestamp,
         )
         return True
 
+    def _sync_checkpoint(
+        self, node_type, node_id, message: grpc.NodeCheckpointState
+    ):
+        if RendezvousName.ELASTIC_TRAINING not in self._rdzv_managers:
+            return False
+        rdzv_manager = self._rdzv_managers[RendezvousName.ELASTIC_TRAINING]
+        return rdzv_manager.sync_ckpt_nodes(node_id, message.step)
+
 
 def create_master_service(
     port,
     task_manager,
     job_manager,
     speed_monitor,
     rdzv_managers,
```

## dlrover/python/master/elastic_training/rdzv_manager.py

```diff
@@ -10,23 +10,29 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import math
 import time
 from abc import ABCMeta, abstractmethod
+from collections import OrderedDict
 from threading import Lock
-from typing import Dict, List
+from typing import Dict, List, Tuple
 
 from dlrover.python.common.constants import (
     NetworkFailureReason,
     RendezvousName,
 )
 from dlrover.python.common.log import default_logger as logger
 from dlrover.python.common.node import Node
+from dlrover.python.master.elastic_training.net_topology import (
+    DefaultTopologyQuerier,
+    DpTopologySorter,
+    NodeTopologyMeta,
+)
 
 
 class RendezvousParameters(object):
     """Holds the parameters to construct rendezvous.
     Args:
         min_nodes:
             The minimum number of nodes to admit to the rendezvous.
@@ -50,25 +56,31 @@
 
 
 class RendezvousManager(metaclass=ABCMeta):
     def __init__(self):
         self._lock = Lock()
         self._alive_nodes = set()
         self._released_workers = []
-        self._waiting_nodes: Dict[int, int] = {}
-        self._rdzv_nodes = {}
+        # key is the node rank.
+        self._waiting_nodes: Dict[int, NodeTopologyMeta] = {}
+        self._rdzv_nodes: Dict[int, NodeTopologyMeta] = OrderedDict()
         self._lastcall_time = 0
         self._rdzv_params = RendezvousParameters(0, 0)
         self._rdzv_round = 0
         self._node_unit = 1
         self._name = ""
         self._latest_rdzv_nodes = []
         self._start_rdzv_ts = 0
+        # key is the node rank, value is the time.
         self._node_rdzv_times: Dict[int, int] = {}
         self._latest_log_nodes_time = 0
+        # key is the node rank, value is the step.
+        self._save_ckpt_nodes: Dict[int, int] = {}
+        self._topology_querier = DefaultTopologyQuerier()
+        self._topology_sorter = DpTopologySorter()
 
     def get_min_nodes(self):
         return self._rdzv_params.min_nodes
 
     def get_rdzv_round(self):
         return self._rdzv_round
 
@@ -83,15 +95,16 @@
         """When a node is exited, the master will remove it from alive list."""
         if node.id in self._alive_nodes:
             self._alive_nodes.remove(node.id)
             logger.info(
                 f"Remove exited worker {node.name} from "
                 f"{self._name} rendezvous."
             )
-            self._waiting_nodes.pop(node.rank_index, 0)
+            self._waiting_nodes.pop(node.rank_index, None)
+            self._has_node_failed = True
 
     def update_rdzv_params(
         self, min_nodes, max_ndoes, waiting_timeout, node_unit
     ):
         """Update rendezvous parameters
         Args:
             min_nodes: The minimum number of nodes.
@@ -127,40 +140,44 @@
                 rdzv_completed = True
                 waiting_num = (
                     waiting_num // self._node_unit
                 ) * self._node_unit
 
         if rdzv_completed:
             node_ids = sorted(self._waiting_nodes.keys())[0:waiting_num]
-            self._rdzv_nodes = {}
+            self._rdzv_nodes = OrderedDict()
             for i in node_ids:
                 self._rdzv_nodes[i] = self._waiting_nodes[i]
             self._latest_rdzv_nodes = list(self._rdzv_nodes.keys())
-            self._waiting_nodes = dict(
-                set(self._waiting_nodes.items())
-                - set(self._rdzv_nodes.items())
-            )
+            extra_nodes = {}
+            for i in self._waiting_nodes.keys():
+                if i not in self._rdzv_nodes:
+                    extra_nodes[i] = self._waiting_nodes[i]
+            self._waiting_nodes = extra_nodes
             self._lastcall_time = 0
             self._log_rendezvous_info()
             if self._waiting_nodes:
+                waiting_node_ranks = sorted(list(self._waiting_nodes.keys()))
                 logger.warning(
                     f"Waiting nodes not in {self._rdzv_round} rendezvous "
-                    f"are {self._waiting_nodes}."
+                    f"are {waiting_node_ranks}."
                 )
         elif time.time() - self._latest_log_nodes_time > 60:
             self._latest_log_nodes_time = time.time()
+            waiting_node_ranks = sorted(list(self._waiting_nodes.keys()))
             logger.info(
-                f"Waiting nodes in rendezvous are {self._waiting_nodes}"
+                f"Waiting nodes in rendezvous are {waiting_node_ranks}"
             )
         return rdzv_completed
 
     def _log_rendezvous_info(self):
+        node_ranks = sorted(list(self._rdzv_nodes.keys()))
         logger.info(
             f"Completed {self._rdzv_round} round "
-            f"rendezvous of {self._name} is {self._rdzv_nodes} \n"
+            f"rendezvous of {self._name} is {node_ranks} \n"
             "The times of nodes to join rendezvous "
             f"are {self._node_rdzv_times}."
         )
         self._node_rdzv_times.clear()
         if self._start_rdzv_ts > 0:
             rdzv_time = round(time.time() - self._start_rdzv_ts, 2)
             logger.info(
@@ -178,30 +195,39 @@
                     nodes.append(node_id)
         return nodes
 
     def join_rendezvous(
         self,
         node_rank,
         local_world_size,
+        node_ip="",
     ):
         """The node joins the current rond rendezvous.
         Args:
             node_id: the node ID which is unique in an ElasticJob of DLrover.
             local_world_size: the local world size of a node.
 
         Returns:
             int: the number of rendezvous round.
         """
         with self._lock:
             if not self._waiting_nodes:
                 self._start_rdzv_ts = time.time()
             if node_rank in self._waiting_nodes:
                 return self._rdzv_round
-            self._waiting_nodes[node_rank] = local_world_size
-            self._rdzv_nodes = {}
+            asw, psw = self._topology_querier.query(node_ip)
+            meta = NodeTopologyMeta(
+                node_rank=node_rank,
+                node_ip=node_ip,
+                process_num=local_world_size,
+                asw=asw,
+                psw=psw,
+            )
+            self._waiting_nodes[node_rank] = meta
+            self._rdzv_nodes = OrderedDict()
             self._lastcall_time = time.time()
             self._node_rdzv_times[node_rank] = round(
                 self._lastcall_time - self._start_rdzv_ts, 2
             )
 
         return self._rdzv_round
 
@@ -224,16 +250,27 @@
         """The node will restart training processes if it
         re-joins the rendezvous."""
         for node_rank in self._waiting_nodes.keys():
             if node_rank in self._latest_rdzv_nodes:
                 return True
         return False
 
+    def sync_ckpt_nodes(self, node_id, step):
+        self._save_ckpt_nodes[node_id] = step
+        steps = set(self._save_ckpt_nodes.values())
+        if len(steps) > 1:
+            return False
+        if len(self._save_ckpt_nodes) == len(self._latest_rdzv_nodes):
+            return True
+        return False
+
     @abstractmethod
-    def get_comm_world(self, node_rank):
+    def get_comm_world(
+        self, node_rank
+    ) -> Tuple[int, int, Dict[int, NodeTopologyMeta]]:
         """Get communication world of all alive nodes.
 
         Args:
             node_rank: the id of node.
 
         Returns:
             rdzv_round: the round index.
@@ -267,15 +304,17 @@
     Elasticjob of DLRover, the node has an unique node ID.
     """
 
     def __init__(self):
         super().__init__()
         self._name = RendezvousName.ELASTIC_TRAINING
 
-    def get_comm_world(self, node_rank):
+    def get_comm_world(
+        self, node_rank
+    ) -> Tuple[int, int, Dict[int, NodeTopologyMeta]]:
         """Return the communication world if a round rendezvous is completed.
         The rendezvous is completed if one of the following conditions
         is satisfied:
         1. The size of waiting node list is equal to the max_nodes.
         2. The size of waiting node list is bigger than the min_nodes and
             equal to the size of alive node list. What's more, no more worker
             join the rendezvous in waiting_timeout.
@@ -287,14 +326,24 @@
             and the value is the local world size of the node.
         """
         with self._lock:
             if not self._rdzv_nodes:
                 rdzv_completed = self._check_rdzv_completed()
                 if rdzv_completed:
                     self._rdzv_round += 1
+                    self._rdzv_nodes = self._topology_sorter.sort(
+                        self._rdzv_nodes
+                    )
+                    ranks = list(self._rdzv_nodes.keys())
+                    node_ips = []
+                    for node_rank in ranks:
+                        node_ips.append(self._rdzv_nodes[node_rank].node_ip)
+                    logger.info(
+                        f"Node ranks are {ranks}.\n Node IPs are {node_ips}"
+                    )
             return self._rdzv_round, 0, self._rdzv_nodes
 
     def report_network_check_result(self, node_id, normal, elapsed_time):
         return
 
 
 class NetworkCheckRendezvousManager(RendezvousManager):
@@ -313,33 +362,39 @@
 
     def __init__(self):
         super().__init__()
         self._name = RendezvousName.NETWORK_CHECK
         self._node_status: Dict[int, bool] = {}
         self._node_times: Dict[int, float] = {}
         self._reported_nodes = set()
-        self._node_groups: List[Dict[int, int]] = []
+        self._node_groups: List[Dict[int, NodeTopologyMeta]] = []
         self._check_round = 2
         self._fault_nodes = set()
         self._straggler_nodes = set()
 
-    def get_comm_world(self, node_rank):
+    def get_comm_world(
+        self, node_rank
+    ) -> Tuple[int, int, Dict[int, NodeTopologyMeta]]:
         """Return the communication world if a round rendezvous is completed.
         The rendezvous is completed if one of the following conditions.
         """
         with self._lock:
             if not self._node_groups:
                 rdzv_completed = self._check_rdzv_completed()
                 if rdzv_completed:
                     self._fault_nodes.clear()
                     self._straggler_nodes.clear()
                     self._node_groups = self._group_nodes(self._rdzv_round)
+                    rank_groups = []
+                    for group in self._node_groups:
+                        ranks = [rank for rank in group.keys()]
+                        rank_groups.append(ranks)
                     logger.info(
-                        f"Round {self._rdzv_round} "
-                        f"node group: {self._node_groups}"
+                        f"Node groups of round {self._rdzv_round} "
+                        f"are: {rank_groups}."
                     )
                     if self._rdzv_round % 2 == 0:
                         self._clear_check_status()
                     self._reported_nodes = set()
                     self._rdzv_round += 1
             for i, group in enumerate(self._node_groups):
                 if node_rank in group:
@@ -358,16 +413,16 @@
         Round 1: group the abnormal node with a normal node like
             [{0:8, 2:8}, {1:8, 2:8}].
         """
         round = round % self._check_round
         node_groups: List[Dict[int, int]] = []
         if round == 0:
             group = {}
-            for node_id, local_world_size in self._rdzv_nodes.items():
-                group[node_id] = local_world_size
+            for node_id, meta in self._rdzv_nodes.items():
+                group[node_id] = meta
                 if len(group) == 2:
                     node_groups.append(group)
                     group = {}
             if len(group) == 1:
                 if len(node_groups) > 0:
                     node_groups[-1].update(group)
                 else:
@@ -431,26 +486,27 @@
                 f"are {self._node_times}"
             )
 
     def join_rendezvous(
         self,
         node_rank,
         local_world_size,
+        node_ip="",
     ):
         """The node joins the current rond rendezvous.
         Args:
             node_rank: the node rank which is unique in an
                 ElasticJob of DLrover.
             local_world_size: the local world size of a node.
 
         Returns:
             int: the number of rendezvous round.
         """
         self._node_groups.clear()
-        return super().join_rendezvous(node_rank, local_world_size)
+        return super().join_rendezvous(node_rank, local_world_size, node_ip)
 
     def check_fault_node(self):
         """Check whether the job has fault nodes. Each task contains 2 rounds
         allgather. If succeed, the round should be set to the multiples of 2.
         """
         with self._lock:
             reason = ""
```

## dlrover/python/master/node/dist_job_manager.py

```diff
@@ -330,17 +330,17 @@
         logger.info(
             "Create job autoscaler: %s", self._job_autoscaler.__class__
         )
 
     def _monitor_nodes(self):
         logger.info("Start monitoring nodes events.")
         while True:
-            nodes = self._node_watcher.list()
-            self._process_list_nodes(nodes)
             try:
+                nodes = self._node_watcher.list()
+                self._process_list_nodes(nodes)
                 if self._stop_monitor:
                     logger.info("Stop processing node events")
                     break
                 for event in self._node_watcher.watch():
                     try:
                         self._process_event(event)
                     except Exception as e:
@@ -671,23 +671,22 @@
             self._chief_manager.all_nodes_deleted()
             and self._worker_manager.all_nodes_deleted()
             and self._evaluator_manager.all_nodes_deleted()
         )
 
     def all_critical_node_completed(self):
         alive_critical_nodes = []
-        with self._lock:
-            for _, nodes in self._job_nodes.items():
-                for node in nodes.values():
-                    if node.critical and node.status in [
-                        NodeStatus.INITIAL,
-                        NodeStatus.PENDING,
-                        NodeStatus.RUNNING,
-                    ]:
-                        alive_critical_nodes.append(node.name)
+        for _, nodes in self._job_nodes.items():
+            for node in nodes.values():
+                if node.critical and node.status in [
+                    NodeStatus.INITIAL,
+                    NodeStatus.PENDING,
+                    NodeStatus.RUNNING,
+                ]:
+                    alive_critical_nodes.append(node.name)
 
         completed = not alive_critical_nodes
         if not completed:
             logger.info("Critical nodes %s are running.", alive_critical_nodes)
         return completed
 
     def remove_worker(self, worker_id):
@@ -813,15 +812,15 @@
         plan = self._worker_manager.remove_not_joined_rdzv_workers(
             worker_ranks
         )
         self._scaler.scale(plan)
 
     def pend_without_workers(self):
         """Check whether to wait for evicted workers."""
-        if self._worker_manager.has_failed_worker():
+        if self._worker_manager.has_exited_worker():
             return False
         elif self._worker_manager.wait_worker_restart():
             return True
         else:
             return False
 
     def handle_training_failure(
```

## dlrover/python/master/node/worker.py

```diff
@@ -260,18 +260,21 @@
             if node.rank_index in worker_ranks:
                 p = self.remove_node(node.id)
                 self._nodes[node_id].relaunchable = False
                 if p:
                     plan.merge(p)
         return plan
 
-    def has_failed_worker(self):
-        """Check whether there is failed worker except evicted workers."""
+    def has_exited_worker(self):
+        """Check whether there is exited worker except evicted workers."""
         for worker in self._nodes.values():
-            if worker.exit_reason == NodeExitReason.FATAL_ERROR:
+            if (
+                worker.exit_reason == NodeExitReason.FATAL_ERROR
+                or worker.status == NodeStatus.SUCCEEDED
+            ):
                 return True
         return False
 
     def wait_worker_restart(self):
         """Check whether there are workers tha have remaining retries."""
         for worker in self._nodes.values():
             if (
```

## dlrover/python/master/scaler/pod_scaler.py

```diff
@@ -10,14 +10,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import copy
 import json
 import os
+import socket
 import telnetlib
 import threading
 import time
 from typing import Dict, List, Optional
 
 from kubernetes import client
 from kubernetes.client import V1EnvVar, V1EnvVarSource, V1ObjectFieldSelector
@@ -506,14 +507,16 @@
 
     def _check_master_service_avaliable(self, host, port, timeout=15):
         """Verify that the master grpc servicer is available."""
         for _ in range(timeout):
             try:
                 telnetlib.Telnet(host=host, port=port, timeout=3)
                 return True
+            except socket.gaierror:
+                return False
             except Exception:
                 time.sleep(1)
         return False
 
     def _patch_tf_config_into_env(self, pod, node: Node, pod_stats, ps_addrs):
         if self._distribution_strategy == DistributionStrategy.PS and ps_addrs:
             tf_config = new_tf_config(
```

## dlrover/python/master/shard/task_manager.py

```diff
@@ -228,17 +228,16 @@
                         and cur - start
                         > max(
                             _TASK_TIMEOUT_THRESHOLD_SECS,
                             self._worker_restart_timeout,
                         )
                     ):
                         logger.info(
-                            "worker %d timeout with task %d, relaunch it",
-                            doing_task.node_id,
-                            task_id,
+                            f"The task {task_id} of {doing_task.node_type}-"
+                            f"{doing_task.node_id} is timeout."
                         )
                         dataset.report_task_status(task_id, success=False)
                         self._invoke_task_timeout_callback(doing_task.node_id)
                         break
             time.sleep(30)
 
     def get_dataset_checkpoint(self, dataset_name):
```

## dlrover/python/tests/test_ckpt_saver.py

```diff
@@ -14,14 +14,15 @@
 import os
 import signal
 import tempfile
 import threading
 import time
 import unittest
 from pathlib import Path
+from unittest import mock
 
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 
 from dlrover.python.common.constants import CheckpointConstant, NodeEnv
 from dlrover.python.common.multi_process import (
@@ -122,14 +123,16 @@
         for _ in range(10):
             if AsyncCheckpointSaver._saver_instance is None:
                 time.sleep(0.5)
             else:
                 break
         self.assertIsNotNone(AsyncCheckpointSaver._saver_instance)
         AsyncCheckpointSaver.reset()
+        wait = AsyncCheckpointSaver._saver_instance.wait_saving_checkpoint()
+        self.assertFalse(wait)
 
         # test notify multiple times,
         # see if it will skip and no exception raised
         sq.put(class_meta)
         sq.put(class_meta)
 
     def test_close_saver(self):
@@ -232,14 +235,39 @@
         with tempfile.TemporaryDirectory() as tmpdir:
             step_done_dir = os.path.join(tmpdir, ".done/10/")
             os.makedirs(step_done_dir, exist_ok=True)
             saver = DdpCheckpointSaver(tmpdir, self.storage.get_class_meta())
             saver.global_shard_num = 1
             saver.commit_checkpoint(100, step_done_dir, 2)
 
+    def test_save_shm_to_storage(self):
+        model = SimpleNet()
+        step = 100
+        state_dict = dict(
+            model=model.state_dict(),
+            step=step,
+        )
+        with tempfile.TemporaryDirectory() as tmpdir:
+            saver = DdpCheckpointSaver(tmpdir, self.storage.get_class_meta())
+            path = Path(tmpdir) / "checkpoint.pt"
+            paths = {CheckpointConstant.MODEL_STATES_NAME: path}
+            ckpt_config = CheckpointConfig(step=100, paths=paths)
+            state_dict = {
+                CheckpointConstant.MODEL_STATES_NAME: state_dict,
+                DLROVER_CKPT_CONFIG_KEY: ckpt_config,
+            }
+            saver._shm_handlers[0].save_state_dict(state_dict)
+            saver._writing_storage = True
+            saver.save_shm_to_storage()
+            self.assertFalse(saver._stop_commit)
+            saver._sync_node_checkpoint = mock.MagicMock(return_value=False)
+            saver.save_shm_to_storage(master_client=1)
+            self.assertTrue(saver._stop_commit)
+            saver.close()
+
 
 class FsdpCheckpointSaverTest(unittest.TestCase):
     def test_persist_storage(self):
         storage = PosixDiskStorage()
         with tempfile.TemporaryDirectory() as tmpdir:
             saver = FsdpDcpSaver(tmpdir, storage.get_class_meta())
             step = 100
```

## dlrover/python/tests/test_elastic_training_agent.py

```diff
@@ -35,15 +35,15 @@
     AsyncCheckpointSaver,
     DdpCheckpointSaver,
 )
 from dlrover.python.elastic_agent.torch.training import (
     ElasticLaunchConfig,
     ElasticTrainingAgent,
     MasterRendezvousHandler,
-    NetworkCheckElasticAgent,
+    NodeCheckElasticAgent,
     RendezvousOutSyncError,
     _get_local_ip,
     _set_paral_config,
 )
 from dlrover.python.tests.test_utils import start_local_master
 
 
@@ -300,17 +300,18 @@
             log_dir=self.config.log_dir,
         )
         storage = PosixDiskStorage()
         saver = DdpCheckpointSaver("/tmp/test", storage.get_class_meta())
         AsyncCheckpointSaver._saver_instance = saver
         agent._save_ckpt_to_storage()
         agent._stop_workers_to_restart()
+        agent._wait_async_saver()
 
 
-class NetworkCheckElasticAgentTest(unittest.TestCase):
+class NodeCheckElasticAgentTest(unittest.TestCase):
     def setUp(self) -> None:
         self._master, addr = start_local_master()
         MasterClient._instance = build_master_client(addr, 0.5)
         launch_config = LaunchConfig(
             min_nodes=2,
             max_nodes=2,
             nproc_per_node=8,
@@ -353,15 +354,15 @@
         )
 
     def tearDown(self):
         self._master.stop()
 
     def test_get_network_check_time(self):
         node_id = 0
-        agent = NetworkCheckElasticAgent(
+        agent = NodeCheckElasticAgent(
             node_rank=node_id,
             config=self.config,
             entrypoint="python",
             spec=self.spec,
             start_method=self.config.start_method,
             log_dir=self.config.log_dir,
         )
@@ -370,15 +371,17 @@
             shutil.rmtree(root)
         os.makedirs(root, exist_ok=True)
         for i in range(8):
             data = {"rank": i, "time": 100 + i}
             path = os.path.join(root, f"{i}.json")
             with open(path, "w") as f:
                 f.write(json.dumps(data))
-        t = agent._get_network_check_time()
+        finished = agent._check_finished(root)
+        self.assertTrue(finished)
+        t = agent._get_node_check_time(root)
         self.assertEqual(t, 107)
         if os.path.exists(root):
             shutil.rmtree(root)
 
 
 class MasterRendezvousHandlerTest(unittest.TestCase):
     def setUp(self) -> None:
```

## dlrover/python/tests/test_master_client.py

```diff
@@ -15,14 +15,15 @@
 import time
 import unittest
 
 from dlrover.python.common import grpc
 from dlrover.python.common.constants import (
     NodeStatus,
     NodeType,
+    RendezvousName,
     TrainingExceptionLevel,
 )
 from dlrover.python.elastic_agent.master_client import build_master_client
 from dlrover.python.tests.test_utils import start_local_master
 
 
 class MasterClientTest(unittest.TestCase):
@@ -121,14 +122,17 @@
         self.assertFalse(success)
 
         success = self._master_client.barrier("test-barrier", True)
         self.assertFalse(success)
 
         self._master_client.report_network_status(0, NodeStatus.SUCCEEDED, 10)
 
+        success = self._master_client.sync_checkpoint(100)
+        self.assertFalse(success)
+
     def test_get(self):
         nodes, failure = self._master_client.query_ps_nodes()
         self.assertEqual(len(nodes), 0)
         self.assertFalse(failure)
 
         status = self._master_client.query_training_status()
         self.assertEqual(status, 3)
@@ -144,10 +148,10 @@
         self.assertEqual(round, 0)
 
         config = self._master_client.get_paral_config()
         if config:
             self.assertIsInstance(config, grpc.ParallelConfig)
 
     def test_num_nodes_waiting(self):
-        rdzv_name = object()
+        rdzv_name = RendezvousName.ELASTIC_TRAINING
         num = self._master_client.num_nodes_waiting(rdzv_name)
         self.assertEqual(num, 0)
```

## dlrover/python/tests/test_multi_process.py

```diff
@@ -9,21 +9,24 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import os
 import unittest
+from unittest import mock
 
 from dlrover.python.common.multi_process import (
+    ERROR_CODE,
     SOCKET_TMP_DIR,
     SharedDict,
     SharedLock,
     SharedMemory,
     SharedQueue,
+    SocketResponse,
     clear_sock_dir,
     retry_socket,
 )
 
 
 class SocketTest(object):
     @retry_socket
@@ -84,14 +87,19 @@
         client_dict.set(new_dict)
         new_dict["a"] = 4
         client_dict.set(new_dict)
         d = server_dict.get()
         self.assertDictEqual(d, new_dict)
         d = client_dict.get()
         self.assertDictEqual(d, new_dict)
+        response = SocketResponse(status=ERROR_CODE)
+        client_dict._request = mock.MagicMock(return_value=response)
+        with self.assertRaises(RuntimeError):
+            client_dict.set(new_dict)
+        server_dict.unlink()
 
 
 class SharedMemoryTest(unittest.TestCase):
     def test_unlink(self):
         fanme = "test-shm"
         with self.assertRaises(ValueError):
             shm = SharedMemory(name=fanme, create=True, size=-1)
```

## dlrover/python/tests/test_pod_scaler.py

```diff
@@ -26,14 +26,15 @@
 
 def new_service_fn(node_type, node_id):
     return str(node_type) + "_" + str(node_id)
 
 
 class PodScalerTest(unittest.TestCase):
     def setUp(self) -> None:
+        os.environ["POD_IP"] = "127.0.0.1"
         mock_k8s_client()
 
     def test_init_pod_template(self):
         scaler = PodScaler("elasticjob-sample", "default")
         scaler.start()
         self.assertEqual(
             scaler._distribution_strategy,
@@ -55,15 +56,14 @@
                 "--training_steps=1000",
             ],
         )
 
     def test_create_pod(self):
         scaler = PodScaler("elasticjob-sample", "default")
         _dlrover_ctx.config_master_port()
-        os.environ["POD_IP"] = "127.0.0.1"
         passed = scaler._check_master_service_avaliable(
             "elasticjob-test-master", 2222, 2
         )
         self.assertFalse(passed)
 
         scaler.start()
         scaler._init_pod_config_by_job()
@@ -184,28 +184,33 @@
             Node(NodeType.WORKER, 3, NodeResource(0, 0))
         )
         plan_json = scale_plan.to_json()
         self.assertTrue("paral_config" not in plan_json)
         scaler.scale(scale_plan)
         self.assertFalse(scale_plan.empty())
         self.assertEqual(len(scaler._create_node_queue), 2)
+        scaler._create_node_queue.clear()
 
     def test_scale_thread(self):
         scaler = PodScaler("elasticjob-sample", "default")
         scaler.start()
         scaler._distribution_strategy = DistributionStrategy.PS
         resource = NodeResource(4, 8192)
         scale_plan = ScalePlan()
         scale_plan.launch_nodes.append(Node(NodeType.WORKER, 1, resource))
         scale_plan.ps_addrs = ["ps-0:22222"]
         scaler.scale(scale_plan)
+        self.assertEqual(len(scaler._create_node_queue), 1)
+        scaler._create_node_queue.clear()
         scale_plan = ScalePlan()
         scale_plan.launch_nodes.append(Node(NodeType.WORKER, 2, resource))
         scale_plan.ps_addrs = ["ps-0:22222"]
         scaler.scale(scale_plan)
+        self.assertEqual(len(scaler._create_node_queue), 1)
+        scaler._create_node_queue.clear()
 
     def test_new_tf_config(self):
         pod_stats = {NodeType.WORKER: 1}
 
         tf_config = new_tf_config(
             pod_stats, new_service_fn, NodeType.WORKER, 0, []
         )
```

## dlrover/python/tests/test_rdzv_manager.py

```diff
@@ -74,15 +74,15 @@
             rdzv_manager._node_rdzv_times, {0: 0.0, 1: 0.0, 2: 0.0}
         )
         round, _, world = rdzv_manager.get_comm_world(0)
         self.assertDictEqual(rdzv_manager._node_rdzv_times, {})
         self.assertEqual(round, 1)
         self.assertEqual(len(rdzv_manager._waiting_nodes), 0)
         self.assertEqual(len(rdzv_manager._rdzv_nodes), 3)
-        self.assertDictEqual(world, {0: 8, 1: 8, 2: 8})
+        self.assertListEqual(list(world.keys()), [0, 1, 2])
 
     def test_min_nodes(self):
         rdzv_manager = ElasticTrainingRendezvousManager()
         rdzv_manager.update_rdzv_params(2, 3, 0.1, 1)
         node_1 = Node("worker", 1)
         rdzv_manager.add_alive_node(node_1)
         node_0 = Node("worker", 0)
@@ -96,15 +96,15 @@
         self.assertEqual(len(rdzv_manager._waiting_nodes), 2)
         self.assertEqual(len(rdzv_manager._rdzv_nodes), 0)
         time.sleep(0.2)
         round, _, world = rdzv_manager.get_comm_world(1)
         self.assertEqual(round, 1)
         self.assertEqual(len(rdzv_manager._waiting_nodes), 0)
         self.assertEqual(len(rdzv_manager._rdzv_nodes), 2)
-        self.assertDictEqual(world, {0: 8, 1: 8})
+        self.assertListEqual(list(world.keys()), [0, 1])
 
     def test_min_nodes_with_unit(self):
         rdzv_manager = ElasticTrainingRendezvousManager()
         rdzv_manager.update_rdzv_params(8, 12, 0.1, 4)
         for i in range(10):
             node = Node("worker", i, name=f"worker-{i}")
             rdzv_manager.add_alive_node(node)
@@ -113,16 +113,15 @@
         self.assertEqual(len(rdzv_manager._waiting_nodes), 10)
         self.assertEqual(len(rdzv_manager._rdzv_nodes), 0)
         time.sleep(0.2)
         round, _, world = rdzv_manager.get_comm_world(1)
         self.assertEqual(round, 1)
         self.assertEqual(len(rdzv_manager._waiting_nodes), 2)
         self.assertEqual(len(rdzv_manager._rdzv_nodes), 8)
-        expected_world = {i: 8 for i in range(8)}
-        self.assertDictEqual(expected_world, world)
+        self.assertListEqual(list(world.keys()), list(range(8)))
         round, _, world = rdzv_manager.get_comm_world(9)
         self.assertEqual(round, 1)
         self.assertFalse(9 in world)
 
         # Test the number of waiting nodes is less than the node unit.
         rdzv_manager.join_rendezvous(10, 8)
         rdzv_manager.join_rendezvous(11, 8)
@@ -159,43 +158,43 @@
             round = rdzv_manager.join_rendezvous(i, 8)
         self.assertEqual(round, 0)
         round, group, world = rdzv_manager.get_comm_world(0)
         self.assertEqual(round, 1)
         self.assertEqual(group, 0)
         self.assertEqual(len(rdzv_manager._waiting_nodes), 0)
         self.assertEqual(len(rdzv_manager._rdzv_nodes), 4)
-        self.assertDictEqual(world, {0: 8, 1: 8})
+        self.assertListEqual(list(world.keys()), [0, 1])
         self.assertEqual(group, 0)
         round, group, world = rdzv_manager.get_comm_world(2)
         self.assertEqual(round, 1)
-        self.assertDictEqual(world, {2: 8, 3: 8})
+        self.assertListEqual(list(world.keys()), [2, 3])
         self.assertEqual(group, 1)
         for i in range(3):
             rdzv_manager.report_network_check_result(i, True, 0.0)
         rdzv_manager.report_network_check_result(3, False, 0.0)
 
         for i in range(4):
             round = rdzv_manager.join_rendezvous(i, 8)
         self.assertEqual(round, 1)
         round, group, world = rdzv_manager.get_comm_world(0)
         self.assertEqual(round, 2)
-        self.assertDictEqual(world, {3: 8, 0: 8})
+        self.assertListEqual(list(world.keys()), [0, 3])
         round, group, world = rdzv_manager.get_comm_world(1)
         self.assertEqual(round, 2)
-        self.assertDictEqual(world, {1: 8, 2: 8})
+        self.assertListEqual(list(world.keys()), [1, 2])
         self.assertEqual(group, 1)
         success, _ = rdzv_manager.check_fault_node()
         self.assertFalse(success)
 
         for i in range(4):
             round = rdzv_manager.join_rendezvous(i, 8)
         self.assertEqual(round, 2)
         round, group, world = rdzv_manager.get_comm_world(3)
         self.assertEqual(round, 3)
-        self.assertDictEqual(world, {2: 8, 3: 8})
+        self.assertListEqual(list(world.keys()), [2, 3])
         _, reason = rdzv_manager.check_fault_node()
         self.assertEqual(reason, NetworkFailureReason.WAITING_NODE)
         for i in range(3):
             rdzv_manager.report_network_check_result(i, True, 0.0)
         rdzv_manager.report_network_check_result(3, True, 0.0)
         nodes, _ = rdzv_manager.check_fault_node()
         self.assertListEqual(nodes, [])
@@ -204,15 +203,15 @@
         rdzv_manager = NetworkCheckRendezvousManager()
         rdzv_manager.update_rdzv_params(1, 1, 60, 1)
         rdzv_manager._alive_nodes = [0]
         round = rdzv_manager.join_rendezvous(0, 8)
         self.assertEqual(round, 0)
         round, _, world = rdzv_manager.get_comm_world(0)
         self.assertEqual(round, 1)
-        self.assertDictEqual(world, {0: 8})
+        self.assertListEqual(list(world.keys()), [0])
         rdzv_manager.report_network_check_result(0, True, 0.0)
         nodes, _ = rdzv_manager.check_fault_node()
         self.assertListEqual(nodes, [])
         rdzv_manager._clear_check_status()
         self.assertDictEqual(rdzv_manager._node_times, {})
         self.assertDictEqual(rdzv_manager._node_status, {})
 
@@ -224,29 +223,29 @@
             round = rdzv_manager.join_rendezvous(i, 8)
         self.assertEqual(round, 0)
         round, group, world = rdzv_manager.get_comm_world(0)
         self.assertEqual(round, 1)
         self.assertEqual(group, 0)
         round, group, world = rdzv_manager.get_comm_world(2)
         self.assertEqual(round, 1)
-        self.assertDictEqual(world, {2: 8, 3: 8})
+        self.assertListEqual(list(world.keys()), [2, 3])
         self.assertEqual(group, 1)
         for i in range(4):
             rdzv_manager.report_network_check_result(i, True, 5.0)
         for i in range(4, 6):
             rdzv_manager.report_network_check_result(i, True, 15.0)
         stragglers, _ = rdzv_manager.get_straggler()
         self.assertListEqual(stragglers, [4, 5])
 
         for i in range(6):
             round = rdzv_manager.join_rendezvous(i, 8)
         self.assertEqual(round, 1)
         round, group, world = rdzv_manager.get_comm_world(5)
         self.assertEqual(round, 2)
-        self.assertDictEqual(world, {0: 8, 5: 8})
+        self.assertListEqual(list(world.keys()), [0, 5])
 
         for i in [1, 2, 3, 4]:
             rdzv_manager.report_network_check_result(i, True, 5.0)
         for i in [0, 5]:
             rdzv_manager.report_network_check_result(i, True, 15.0)
         stragglers, _ = rdzv_manager.get_straggler()
         self.assertListEqual(stragglers, [5])
@@ -259,29 +258,39 @@
             round = rdzv_manager.join_rendezvous(i, 8)
         self.assertEqual(round, 0)
         round, group, world = rdzv_manager.get_comm_world(0)
         self.assertEqual(round, 1)
         self.assertEqual(group, 0)
         round, group, world = rdzv_manager.get_comm_world(2)
         self.assertEqual(round, 1)
-        self.assertDictEqual(world, {2: 8, 3: 8, 4: 8})
+        self.assertListEqual(list(world.keys()), [2, 3, 4])
         self.assertEqual(group, 1)
         for i in range(2):
             rdzv_manager.report_network_check_result(i, True, 15.0)
         for i in range(2, 5):
             rdzv_manager.report_network_check_result(i, True, 5.0)
         stragglers, _ = rdzv_manager.get_straggler()
         self.assertListEqual(stragglers, [0, 1])
 
         for i in range(5):
             round = rdzv_manager.join_rendezvous(i, 8)
         self.assertEqual(round, 1)
         round, group, world = rdzv_manager.get_comm_world(1)
         self.assertEqual(round, 2)
-        self.assertDictEqual(world, {1: 8, 2: 8})
+        self.assertListEqual(list(world.keys()), [2, 1])
 
         for i in [1, 2]:
             rdzv_manager.report_network_check_result(i, True, 15.0)
         for i in [0, 3, 4]:
             rdzv_manager.report_network_check_result(i, True, 5.0)
         stragglers, _ = rdzv_manager.get_straggler()
         self.assertListEqual(stragglers, [1])
+
+    def test_sync_ckpt_nodes(self):
+        rdzv_manager = ElasticTrainingRendezvousManager()
+        rdzv_manager._latest_rdzv_nodes = [0, 1]
+        success = rdzv_manager.sync_ckpt_nodes(0, 100)
+        self.assertFalse(success)
+        success = rdzv_manager.sync_ckpt_nodes(1, 100)
+        self.assertTrue(success)
+        success = rdzv_manager.sync_ckpt_nodes(1, 90)
+        self.assertFalse(success)
```

## dlrover/python/tests/test_servicer.py

```diff
@@ -388,14 +388,24 @@
         request.data = message.serialize()
         request.node_type = NodeType.WORKER
         request.node_id = 0
         self.servicer.report(request, None)
         worker0 = self.servicer._job_manager._job_nodes[NodeType.WORKER][0]
         self.assertEqual(worker0.heartbeat_time, ts)
 
+    def test_sync_checkpoint(self):
+        message = grpc.NodeCheckpointState(step=100)
+        et_name = RendezvousName.ELASTIC_TRAINING
+        rdzv_manager = self.servicer._rdzv_managers[et_name]
+        rdzv_manager._latest_rdzv_nodes = [0, 1]
+        success = self.servicer._sync_checkpoint(NodeType.WORKER, 0, message)
+        self.assertFalse(success)
+        success = self.servicer._sync_checkpoint(NodeType.WORKER, 1, message)
+        self.assertTrue(success)
+
 
 class MasterServicerForRayTest(unittest.TestCase):
     def setUp(self) -> None:
         ray.init = mock.MagicMock(return_value=True)
         params = MockRayJobArgs()
         params.initilize()
         speed_monitor = SpeedMonitor()
```

## dlrover/python/tests/test_utils.py

```diff
@@ -261,15 +261,16 @@
     )
     k8s_client.patch_service = mock.MagicMock(  # type: ignore
         return_value=True
     )
     k8s_client.get_service = mock.MagicMock(return_value=False)  # type: ignore
 
 
-def start_local_master():
+def start_local_master(port=12345):
     job_args = LocalJobArgs("local", "default", "test")
     job_args.initilize()
-    port = find_free_port()
+    if not port:
+        port = find_free_port()
     master = LocalJobMaster(port, job_args)
     master.prepare()
     addr = f"127.0.0.1:{port}"
     return master, addr
```

## dlrover/python/tests/test_worker_manager.py

```diff
@@ -153,21 +153,25 @@
             3,
             self._elastic_job.get_node_service_addr,
             self._elastic_job.get_node_name,
         )
         for node in worker_manager._nodes.values():
             node.status = NodeStatus.FAILED
             node.exit_reason = NodeExitReason.FATAL_ERROR
-        failed = worker_manager.has_failed_worker()
-        self.assertTrue(failed)
+        exited = worker_manager.has_exited_worker()
+        self.assertTrue(exited)
 
         for node in worker_manager._nodes.values():
             node.exit_reason = NodeExitReason.KILLED
-        failed = worker_manager.has_failed_worker()
-        self.assertFalse(failed)
+        exited = worker_manager.has_exited_worker()
+        self.assertFalse(exited)
+
+        worker_manager._nodes[0].status = NodeStatus.SUCCEEDED
+        exited = worker_manager.has_exited_worker()
+        self.assertTrue(exited)
 
         wait = worker_manager.wait_worker_restart()
         self.assertTrue(wait)
         for node in worker_manager._nodes.values():
             node.relaunch_count = node.max_relaunch_count
 
         wait = worker_manager.wait_worker_restart()
```

## dlrover/trainer/torch/elastic_run.py

```diff
@@ -144,29 +144,29 @@
         "--auto-config",
         action=check_env,
         help="Whether to automatically configure the nnodes "
         "and nproc_per_nodes.",
     )
     parser.add_argument(
         "--auto_tunning",
-        "--auto_tunning",
+        "--auto-tunning",
         action=check_env,
         help="Whether to auto-tune the parallel configuraion.",
     )
     parser.add_argument(
         "--exclude-straggler",
         "--exclude_straggler",
         action=check_env,
         help="Bool, The node will exit if the node is straggler and "
         "the argument is True. The argument only works when network-check "
         "is True.",
     )
     parser.add_argument(
-        "--save-at-breakpoint",
         "--save_at_breakpoint",
+        "--save-at-breakpoint",
         action=check_env,
         help="Bool. If True, the agent in the main process will save the "
         "checkpoint in the memory to the storage if the training "
         "process fails.",
     )
     parser.add_argument(
         "--accelerator",
@@ -285,15 +285,17 @@
     args,
 ) -> Tuple[ElasticLaunchConfig, Union[Callable, str], List[str]]:
     config, cmd, cmd_args = config_from_args(args)
     elastic_config = ElasticLaunchConfig(**config.__dict__)
     elastic_config.network_check = getattr(args, "network_check", False)
     elastic_config.auto_tunning = getattr(args, "auto_tunning", False)
     elastic_config.auto_config = getattr(args, "auto_config", False)
-    elastic_config.accelerator = getattr(args, "accelerator", "")
+    elastic_config.accelerator = getattr(
+        args, "accelerator", Accelerators.NVIDIA_GPU
+    )
     elastic_config.exclude_straggler = getattr(
         args, "exclude_straggler", False
     )
     elastic_config.set_node_unit(getattr(args, "node_unit", 1))
     elastic_config.save_at_breakpoint = getattr(
         args, "save_at_breakpoint", False
     )
```

## dlrover/trainer/torch/flash_checkpoint/ddp.py

```diff
@@ -15,20 +15,21 @@
 
 import torch.distributed as dist
 
 from dlrover.python.common.constants import CheckpointConstant
 from dlrover.python.common.storage import PosixDiskStorage
 
 from .checkpointer import Checkpointer, StorageType
-from .ddp_engine import DdpCheckpointEngine
+from .full_ckpt_engine import FullCheckpointEngine
 
 
 class DdpCheckpointer(Checkpointer):
     """
-    Flash checkpointer to save and load a DDP model.
+    Flash checkpointer to save and load a DDP model or a model state
+    dict with full weights.
 
     Args:
         checkpoint_dir: the directory to save the checkpoint.
         storage: A CheckpointStorage instance. The checkpointer will
             use a PosixStorage instance if the storage is not defined.
         local_shard_num (int): the number of shards on a node,
             The default is 1. If the model is partitioned on all ranks,
@@ -52,15 +53,15 @@
         >>>         checkpointer.save_checkpoint(
         >>>             step, state_dict, path, storage_type=StorageType.Memory
         >>>         )
         >>>     elif step % 100 == 0:
         >>>         checkpointer.save_checkpoint(
         >>>             step, state_dict, path, storage_type=StorageType.DISK
         >>>         )
-        >>> sate_dict = engine.load_checkpoint()
+        >>> sate_dict = checkpointer.load_checkpoint()
     """
 
     def __init__(
         self,
         checkpoint_dir: str,
         storage=None,
         local_shard_num=1,
@@ -69,15 +70,15 @@
     ):
         self.checkpoint_dir = checkpoint_dir
         if dist.is_initialized():
             self._rank = dist.get_rank()
         else:
             self._rank = 0
         self.storage = PosixDiskStorage() if not storage else storage
-        self._engine = DdpCheckpointEngine(
+        self._engine = FullCheckpointEngine(
             checkpoint_dir=checkpoint_dir,
             storage=self.storage,
             local_shard_num=local_shard_num,
             global_shard_num=global_shard_num,
             comm_backend=comm_backend,
         )
```

## dlrover/trainer/torch/flash_checkpoint/deepspeed.py

```diff
@@ -35,17 +35,17 @@
 _DS_MODEL_SD_FILE_SUFFIX = "model_states.pt"
 _DS_OPTIM_SD_FILE_SUFFIX = "optim_states.pt"
 
 torch_native_save = torch.save
 torch_native_load = torch.load
 
 
-class AsyncSaveEngine(CheckpointEngine):
+class AsyncCheckpointAgent(CheckpointEngine):
     """
-    The checkpoint engine to save/load checkpoint of DeepSpeed.
+    The checkpoint agent to save/load checkpoint of DeepSpeed.
 
     Attributes:
         model_sd: the state dict of a PyTorch model.
         model_path (str): the storage path to save the model state dict.
         optim_sd: the state dict of a DeepSpeed optimizer.
         optim_path (str): the storage path to save the optim state dict.
     """
@@ -64,20 +64,18 @@
             torch_native_save(state_dict, path)
             return
         if path.endswith(_DS_MODEL_SD_FILE_SUFFIX):
             sd_name = CheckpointConstant.MODEL_STATES_NAME
         elif path.endswith(_DS_OPTIM_SD_FILE_SUFFIX):
             sd_name = CheckpointConstant.OPTIM_STATES_NAME
         else:
-            raise ValueError(
-                f"The suffix of  {path} is not "
-                f"{_DS_MODEL_SD_FILE_SUFFIX} and {_DS_OPTIM_SD_FILE_SUFFIX}. "
-            )
-        self.state_dict[sd_name] = state_dict
-        self.paths[sd_name] = path
+            sd_name = path.split("/")[-1]
+        if sd_name:
+            self.state_dict[sd_name] = state_dict
+            self.paths[sd_name] = path
 
     def load(self, path: str, map_location=None):
         def load_func(path):
             return torch_native_load(path, map_location=map_location)
 
         sd_name = ""
         if path.endswith(_DS_MODEL_SD_FILE_SUFFIX):
@@ -137,16 +135,17 @@
         self._async_save_engine = DeepSpeedCheckpointEngine(
             checkpoint_dir,
             storage=self.storage,
             global_shard_num=global_shard_num,
             zero_stage=zero_stage,
             comm_backend=comm_backend,
         )
-        self._ckpt_engine = AsyncSaveEngine(self._async_save_engine.storage)
-        self.engine.checkpoint_engine = self._ckpt_engine
+        self._ckpt_agent = AsyncCheckpointAgent(
+            self._async_save_engine.storage
+        )
         self._local_rank = env_utils.get_local_rank()
         self._ds_tracer_file = os.path.join(
             self.checkpoint_dir, DeepSpeedCheckpointSaver.TRACER_FILE
         )
         self._dlrover_tracer_file = os.path.join(
             self.checkpoint_dir, CheckpointConstant.TRACER_FILE_NAME
         )
@@ -171,21 +170,21 @@
             )
         else:
             raise ValueError(f"No support storage type {storage_type}")
 
     def _save_checkpoint_to_memory(
         self, save_dir, tag=None, client_state={}, save_latest=True
     ):
-        torch.save = self._ckpt_engine.save
+        torch.save = self._ckpt_agent.save
         self.engine.save_checkpoint(save_dir, tag, client_state, save_latest)
         torch.save = torch_native_save
         self._async_save_engine.save_to_memory(
             tag,
-            self._ckpt_engine.state_dict,
-            self._ckpt_engine.paths,
+            self._ckpt_agent.state_dict,
+            self._ckpt_agent.paths,
         )
         self._update_tracer_file(tag)
 
     def _update_tracer_file(self, tag):
         """
         The method save_to_memory does not save the state dict into
         the storage. We need to restore the tracer file modified
@@ -201,21 +200,21 @@
             self.storage.write(content, self._ds_tracer_file)
         else:
             self.storage.safe_remove(self._ds_tracer_file)
 
     def _save_checkpoint_to_storage(
         self, save_dir, tag=None, client_state={}, save_latest=True
     ):
-        torch.save = self._ckpt_engine.save
+        torch.save = self._ckpt_agent.save
         self.engine.save_checkpoint(save_dir, tag, client_state, save_latest)
         torch.save = torch_native_save
         self._async_save_engine.save_to_storage(
             tag,
-            self._ckpt_engine.state_dict,
-            self._ckpt_engine.paths,
+            self._ckpt_agent.state_dict,
+            self._ckpt_agent.paths,
         )
 
     def load_checkpoint(
         self,
         load_dir,
         tag=None,
         load_module_strict=True,
@@ -226,16 +225,16 @@
     ):
         """
         Load a checkpointing state dict.
 
         Args:
             the same as the DeepSpeedEngine.load_checkpoint.
         """
-        self._ckpt_engine.state_dict = self._async_save_engine.load()
-        torch.load = self._ckpt_engine.load
+        self._ckpt_agent.state_dict = self._async_save_engine.load()
+        torch.load = self._ckpt_agent.load
         load_path, client_states = self.engine.load_checkpoint(
             load_dir=load_dir,
             tag=tag,
             load_module_strict=load_module_strict,
             load_optimizer_states=load_optimizer_states,
             load_lr_scheduler_states=load_lr_scheduler_states,
             load_module_only=load_module_only,
```

## dlrover/trainer/torch/flash_checkpoint/deepspeed_engine.py

```diff
@@ -85,15 +85,21 @@
             step (int): the global iteration step.
             state_dict (dict): the state dict of model and optimizer to save.
             paths (dict): the key is a category in
                 ["model_states", "optim_states"] of the state dict and
                 the value is the path of storage to save.
         """
         conf = CheckpointConfig(step=step, paths=paths)
-        return self.save_state_dict_to_memory(state_dict, conf)
+        import time
+
+        start = time.time()
+        success = self.save_state_dict_to_memory(state_dict, conf)
+        t = round(time.time() - start, 2)
+        print(f"Save Time is {t}s")
+        return success
 
     @timer
     def save_to_storage(self, step, state_dict, paths):
         """
         Asynchonously saves the state dict into the storage. It synchonously
         saves the state dict into the shared memory and put the path
         into a shared queue. The agent in the main process waits for the queue
@@ -103,25 +109,26 @@
         Args:
             step (int): the global iteration step.
             state_dict (dict): the state dict of model and optimizer to save.
             paths (dict): the key is a category in
                 ["model_states", "optim_states"] of the state dict and
                 the value is the path of storage to save.
         """
-        succeed = True
+        success = True
         if step > self._cached_step:
-            succeed = self.save_to_memory(step, state_dict, paths)
+            success = self.save_to_memory(step, state_dict, paths)
 
         if dist.is_initialized():
             dist.barrier()
 
         # Only local rank 0 to notify the saving event to the agent.
-        if self._local_rank == 0 and succeed:
+        if self._local_rank == 0 and success:
             event = CheckpointEvent(type=CheckpointEventType.SAVE, step=step)
             self._event_queue.put(event)
+        return success
 
     def get_local_shard_num(self):
         local_world_size = env_utils.get_local_world_size()
         global_shard_num = self.get_global_shard_num()
         return min(local_world_size, global_shard_num)
 
     def get_global_shard_num(self):
@@ -135,15 +142,15 @@
         The method firstly try to load the state dict from the shared memory.
         If there is no state dict in the shared memory, the method will
         load the state dict from the storage.
 
         Returns:
             A dict.
         """
-        state_dict = self.get_state_dict_from_memory()
+        _, state_dict = self.get_state_dict_from_memory()
         if state_dict:
             msd_name = CheckpointConstant.MODEL_STATES_NAME
             if msd_name not in state_dict and self.zero_stage in [1, 2]:
                 local_rank_0_shm_handler = SharedMemoryHandler(0, host=False)
                 # For stage 1,2, the model is not partitioned and only local
                 # rank 0 saves the model state dict into the CPU memory. Other
                 # local ranks need get the model state dict from the shared
```

## dlrover/trainer/torch/flash_checkpoint/engine.py

```diff
@@ -87,27 +87,30 @@
             succeed = False
     del t, outputs
     return succeed
 
 
 def timer(func):
     def wrapper(*args, **kwargs):
+        local_rank = env_utils.get_local_rank()
         start = time.time()
         result = func(*args, **kwargs)
         t = round(time.time() - start, 3)
-        logger.info(f"Function {func.__name__} cost {t}s")
+        logger.info(
+            f"Local rank {local_rank } execute {func.__name__} in {t}s."
+        )
         return result
 
     return wrapper
 
 
 def start_async_save():
     AsyncCheckpointSaver.start_async_saving_ckpt()
     while True:
-        time.sleep(36000)
+        time.sleep(60)
 
 
 def start_saver_process():
     """
     Start a process to to asynchronously save checkpoint if the training
     process is not launched by `dlrover-run`. This process will
     exit and cannot save the checkpoint after the training process exit.
@@ -289,15 +292,18 @@
             return False
 
         conf.rank = self._rank
         conf.group_rank = self._group_rank
         conf.world_size = self._world_size
 
         acquired = self._shm_lock.acquire(blocking=False)
-        logger.info(f"Acquired the lock of shared memory: {acquired}.")
+        logger.info(
+            f"{self._local_rank} acquired the lock of shared "
+            f"memory: {acquired}."
+        )
         all_rank_ready = check_all_rank_ready(self._saver_group, acquired)
         if not all_rank_ready or not state_dict:
             logger.info(
                 f"Rank {self._rank} skips the save the checkpoint "
                 f"in CPU memory since it is saving the latest "
                 "checkpoint from the CPU memory into the storage."
             )
@@ -318,18 +324,16 @@
         config = self._shm_handler.get_checkpoint_config(default_config)
         passed = verify_all_rank_step_consistent(
             self._loader_group, config.step
         )
         if passed and config.step > 0:
             state_dict = self._shm_handler.load_state_dict()
             state_dict.pop(DLROVER_CKPT_CONFIG_KEY, None)
-            logger.info(
-                f"Load step {config.step} checkpoint from the shared memory."
-            )
-        return state_dict
+            logger.info(f"Load checkpoint at step {config.step} from memory.")
+        return config.step, state_dict
 
     @abstractmethod
     def get_saving_ranks(self):
         pass
 
     @abstractmethod
     def get_saver_class(self):
```

## dlrover/trainer/torch/flash_checkpoint/fsdp.py

```diff
@@ -7,90 +7,271 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+import os
+
+import torch.distributed as dist
+import torch.distributed.checkpoint as dist_cp
+from torch.distributed.checkpoint.optimizer import (
+    load_sharded_optimizer_state_dict,
+)
+from torch.distributed.fsdp import FullStateDictConfig
+from torch.distributed.fsdp import FullyShardedDataParallel as FSDP
+from torch.distributed.fsdp import StateDictType
+from torch.distributed.fsdp.api import FullOptimStateDictConfig
+
 from dlrover.python.common.constants import CheckpointConstant
 from dlrover.python.common.storage import PosixDiskStorage
+from dlrover.trainer.torch.flash_checkpoint.full_ckpt_engine import (
+    FullCheckpointEngine,
+)
 
 from .checkpointer import Checkpointer, StorageType
 from .fsdp_engine import FsdpCheckpointEngine
 
 
-class FsdpCheckpointer(Checkpointer):
+class FsdpShardCheckpointer(Checkpointer):
     """
     Flash checkpointer saves and loads a FSDP module.
 
     Args:
         checkpoint_dir: the directory to save the checkpoint.
         storage: A CheckpointStorage instance. The checkpointer will
             use a PosixStorage instance if the storage is not defined.
         comm_backend (str): the backend to synchronize when saving the
             checkpoint to the memory.
 
     Examples::
-        >>> checkpointer = FsdpCheckpointer(checkpoint_dir)
+        >>> checkpointer = FsdpShardCheckpointer(checkpoint_dir)
         >>> # Save checkpoint
-        >>> with FSDP.state_dict_type(model, StateDictType.SHARDED_STATE_DICT):
-        >>>     state_dict = {
-        >>>         "model": model.state_dict(),
-        >>>         "optim": FSDP.optim_state_dict(model, optimizer),
-        >>>     }
-        >>> ckpt_dir = os.path.join(checkpoint_dir, str(step))
-        >>> if step % save_memory_interval == 0:
-        >>>     checkpointer.save_checkpoint(
-        >>>         step, state_dict, ckpt_dir, storage_type=StorageType.MEMORY
-        >>>     )
+        >>> extra_sd = {"step": step, "epoch": epoch}
         >>> if step % save_storage_interval == 0:
         >>>     checkpointer.save_checkpoint(
-        >>>         step, state_dict, ckpt_dir, storage_type=StorageType.DISK
+        >>>         step, state_dict, ckpt_dir
         >>>     )
         >>> # Load checkpoint
-        >>> with FSDP.state_dict_type(model, StateDictType.SHARDED_STATE_DICT):
-        >>> state_dict = {"model": model.state_dict()}
-        >>> storage_reader = checkpointer.get_storage_reader()
-        >>> if not storage_reader:
-        >>>     return
-        >>> dist_cp.load_state_dict(
-        >>>     state_dict=state_dict,
-        >>>     storage_reader=storage_reader,
-        >>> )
-        >>> model.load_state_dict(state_dict["model"])
-        >>> optim_state = load_sharded_optimizer_state_dict(
-        >>>     model_state_dict=state_dict["model"],
-        >>>     optimizer_key="optim",
-        >>>     storage_reader=storage_reader,
-        >>> )
-        >>> flattened_osd = FSDP.optim_state_dict_to_load(
-        >>>     model, optimizer, optim_state["optim"]
-        >>> )
-        >>> optimizer.load_state_dict(flattened_osd)
+        >>> checkpointer.load_checkpoint(model, optimzier)
     """
 
     def __init__(self, checkpoint_dir: str, storage=None, comm_backend=""):
+        self.checkpoint_dir = checkpoint_dir
         self.storage = PosixDiskStorage() if not storage else storage
         self._engine = FsdpCheckpointEngine(
             checkpoint_dir, self.storage, comm_backend
         )
 
     def save_checkpoint(
-        self, step, state_dict, path, storage_type=StorageType.DISK
+        self,
+        step,
+        model,
+        optimizer,
+        extra_sd={},
+        path="",
+        storage_type=StorageType.DISK,
     ):
+        """
+        Save a fsdp model and optimizer.
+
+        Args:
+            step(int): the iteration step.
+            model: A FSDP module.
+            optimizer: An optimizer to train a FSDP model.
+            extra_sd(dict): A dict to store customized arguements
+                in the chechkpoint.
+            path(str): A path to store the checkpoint.
+            storage_tyep: Save the checkpoint into the memory
+                if `StorageType.MEMORY` and into the dist
+                if `StorageType.DISK`.
+        """
+        with FSDP.state_dict_type(model, StateDictType.SHARDED_STATE_DICT):
+            state_dict = {
+                "model": model.state_dict(),
+                "optim": FSDP.optim_state_dict(model, optimizer),
+            }
+            state_dict.update(extra_sd)
+            if not path:
+                path = os.path.join(self.checkpoint_dir, str(step))
+            paths = {CheckpointConstant.MODEL_STATES_NAME: path}
+            if storage_type == StorageType.MEMORY:
+                self._engine.save_to_memory(step, state_dict, paths)
+            elif storage_type == StorageType.DISK:
+                if not path:
+                    raise ValueError(
+                        "path cannot be empty if storage type is disk!"
+                    )
+                self._engine.save_to_storage(step, state_dict, path)
+            else:
+                raise ValueError(f"No support storage type {storage_type}")
+
+    def load_checkpoint(self, model, optimizer, resume_path=""):
+        with FSDP.state_dict_type(model, StateDictType.SHARDED_STATE_DICT):
+            state_dict = {
+                "model": model.state_dict(),
+                "step": 0,
+                # cannot load the optimizer state_dict together
+                # with the model state_dict
+            }
+            storage_reader = self._engine.load(resume_path)
+            if not storage_reader:
+                return {}
+            dist_cp.load_state_dict(
+                state_dict=state_dict,
+                storage_reader=storage_reader,
+            )
+            model_sd = state_dict.pop("model", None)
+            if model_sd:
+                model.load_state_dict(model_sd)
+
+            optim_state = load_sharded_optimizer_state_dict(
+                model_state_dict=model_sd,
+                optimizer_key="optim",
+                storage_reader=storage_reader,
+            )
+
+            optim_sd = optim_state.pop("optim", None)
+            if optim_sd:
+                flattened_osd = FSDP.optim_state_dict_to_load(
+                    model, optimizer, optim_sd
+                )
+                optimizer.load_state_dict(flattened_osd)
+            return state_dict
+
+
+class FsdpFullCheckpointer(Checkpointer):
+    """
+    Flash checkpointer to save and load a FSDP full model.
+
+    Args:
+        checkpoint_dir: the directory to save the checkpoint.
+        storage: A CheckpointStorage instance. The checkpointer will
+            use a PosixStorage instance if the storage is not defined.
+        local_shard_num (int): the number of shards on a node,
+            The default is 1. If the model is partitioned on all ranks,
+            you should set the local_shard_num as the number of ranks
+            on a node.
+        global_shard_num (int): the number of shards across all ranks.
+            The default is 1.If the model is partitioned on all ranks,
+            you should set the local_shard_num as the number of all ranks.
+        comm_backend (str): the communcation backend to create a process group,
+            The default is the backend of general main process group.
+
+    Examples::
+        >>> checkpointer = FsdpFullCheckpointer(
+        >>>     checkpoint_dir="/tmp/checkpoint/"
+        >>> )
+        >>> for step, data in enumerate(dataloader):
+        >>>     ...
+        >>>     extra_sd = {"epoch": 10}
+        >>>     path = f"/tmp/checkpoint-{step}.pt"
+        >>>     if step % 100 == 0:
+        >>>         checkpointer.save_checkpoint(
+        >>>             step, model, optimizer, extra_sd, path
+        >>>         )
+        >>> sate_dict = checkpointer.load_checkpoint(model, optimizer)
+    """
+
+    def __init__(
+        self,
+        checkpoint_dir: str,
+        storage=None,
+        comm_backend="",
+    ):
+        self.checkpoint_dir = checkpoint_dir
+        if dist.is_initialized():
+            self._rank = dist.get_rank()
+        else:
+            self._rank = 0
+        self.storage = PosixDiskStorage() if not storage else storage
+        self._engine = FullCheckpointEngine(
+            checkpoint_dir=checkpoint_dir,
+            storage=self.storage,
+            local_shard_num=1,
+            global_shard_num=1,
+            comm_backend=comm_backend,
+        )
+
+    def save_checkpoint(
+        self,
+        step,
+        model,
+        optimizer,
+        extra_sd={},
+        path="",
+        storage_type=StorageType.DISK,
+    ):
+        """
+        Save a fsdp model and optimizer.
+
+        Args:
+            step(int): the iteration step.
+            model: A FSDP module.
+            optimizer: An optimizer to train a FSDP model.
+            extra_sd(dict): A dict to store customized arguements
+                in the chechkpoint.
+            path(str): A path to store the checkpoint.
+            storage_tyep: Save the checkpoint into the memory
+                if `StorageType.MEMORY` and into the dist
+                if `StorageType.DISK`.
+        """
+        if path == "":
+            ckpt_name = f"{step}/rank_{self._rank}.pt"
+            path = os.path.join(self.checkpoint_dir, ckpt_name)
+
+        with FSDP.state_dict_type(
+            model,
+            StateDictType.FULL_STATE_DICT,
+            FullStateDictConfig(rank0_only=False),
+            FullOptimStateDictConfig(rank0_only=False),
+        ):
+            msd = model.state_dict()
+            osd = FSDP.optim_state_dict(model, optimizer)
+        state_dict = {"model": msd, "optimizer": osd}
+        state_dict.update(extra_sd)
+
+        state_dict = {CheckpointConstant.MODEL_STATES_NAME: state_dict}
         paths = {CheckpointConstant.MODEL_STATES_NAME: path}
         if storage_type == StorageType.MEMORY:
             self._engine.save_to_memory(step, state_dict, paths)
         elif storage_type == StorageType.DISK:
             if not path:
                 raise ValueError(
                     "path cannot be empty if storage type is disk!"
                 )
-            self._engine.save_to_storage(step, state_dict, path)
+            if self._rank == 0:
+                self.storage.safe_rmtree(os.path.dirname(path))
+            self._engine.save_to_storage(step, state_dict, paths)
         else:
             raise ValueError(f"No support storage type {storage_type}")
 
-    def load_checkpoint(self, resume_path=""):
-        pass
+    def load_checkpoint(self, model, optimizer, resume_path=""):
+        """
+        Load a fsdp model and optimizer.
+
+        Args:
+            model: A FSDP module.
+            optimizer: An optimizer to train a FSDP model.
+            resume_path (str): the path to restore the checkpoint.
+        """
+        state_dict = self._engine.load(resume_path)
+        if not state_dict:
+            return {}
+        model_state_dict = state_dict.pop("model", {})
+        optim_state_dict = state_dict.pop("optimizer", {})
 
-    def get_storage_reader(self, resume_path=""):
-        return self._engine.load(resume_path)
+        with FSDP.state_dict_type(
+            model,
+            StateDictType.FULL_STATE_DICT,
+            FullStateDictConfig(rank0_only=False),
+            FullOptimStateDictConfig(rank0_only=False),
+        ):
+            optim_state_dict = FSDP.optim_state_dict_to_load(
+                model=model,
+                optim=optimizer,
+                optim_state_dict=optim_state_dict,
+            )
+        model.load_state_dict(model_state_dict)
+        optimizer.load_state_dict(optim_state_dict)
+        return state_dict
```

## dlrover/trainer/torch/flash_checkpoint/megatron_dist_ckpt.py

```diff
@@ -258,31 +258,47 @@
 
 def load_checkpoint(
     model,
     optimizer,
     opt_param_scheduler,
     load_arg="load",
     strict=True,
+    storage=None,
+    comm_backend="",
 ):
     """Load a model checkpoint and return the iteration.
     strict (bool): whether to strictly enforce that the keys in
         :attr:`state_dict` of the checkpoint match the names of
         parameters and buffers in model.
     """
     args = get_args()
     load_dir = getattr(args, load_arg)
 
-    model = unwrap_model(model)
+    checkpointer = MegatronDistCheckpointer.singleton_instance(
+        args.save,
+        storage=storage,
+        comm_backend=comm_backend,
+        use_distributed_optimizer=args.use_distributed_optimizer,
+    )
 
+    model = unwrap_model(model)
     (
         model_state_dict,
         opt_state_dict,
         checkpoint_name,
         release,
-    ) = _load_base_checkpoint(load_dir, rank0=False)
+    ) = _load_checkpoint_from_memory(checkpointer)
+
+    if not model_state_dict:
+        (
+            model_state_dict,
+            opt_state_dict,
+            checkpoint_name,
+            release,
+        ) = _load_base_checkpoint(load_dir, rank0=False)
 
     # Checkpoint not loaded.
     if model_state_dict is None:
 
         # Conditionally exit at this point.
         if args.exit_on_missing_checkpoint:
             print_rank_0(
@@ -443,20 +459,28 @@
         f"  successfully loaded checkpoint from {args.load} "
         f"at iteration {iteration}"
     )
 
     return iteration, num_floating_point_operations_so_far
 
 
+def _load_checkpoint_from_memory(checkpointer):
+    step, state_dict = checkpointer.engine.load()
+    model_state_dict = state_dict.get(CheckpointConstant.MODEL_STATES_NAME, {})
+    opt_state_dict = state_dict.get(CheckpointConstant.OPTIM_STATES_NAME, {})
+    checkpoint_name = "iter_{:07d}".format(step)
+    release = False
+    return model_state_dict, opt_state_dict, checkpoint_name, release
+
+
 def _load_base_checkpoint(load_dir, rank0=False):
     """Load the base state_dict from the given directory
 
     If rank0 is true, just loads rank 0 checkpoint, ignoring arguments.
     """
-
     # Read the tracker file and set the iteration.
     tracker_filename = get_checkpoint_tracker_filename(load_dir)
 
     # If no tracker file, return nothing
     if not os.path.isfile(tracker_filename):
         if not rank0:
             print_rank_0(
```

## dlrover/trainer/torch/flash_checkpoint/megatron_engine.py

```diff
@@ -136,18 +136,15 @@
         The method firstly try to load the state dict from the shared memory.
         If there is no state dict in the shared memory, the method will
         load the state dict from the storage.
 
         Returns:
             A dict.
         """
-        state_dict = self.get_state_dict_from_memory()
-        if state_dict:
-            return state_dict
-        return {}
+        return self.get_state_dict_from_memory()
 
 
 class MegatronDistCheckpointEngine(CheckpointEngine):
     """
     The checkpoint engine synchronously writes the state dict of
     Megatron-LM model and optimizer into
     the shared memory and notify the agent in main process to
@@ -251,11 +248,8 @@
         The method firstly try to load the state dict from the shared memory.
         If there is no state dict in the shared memory, the method will
         load the state dict from the storage.
 
         Returns:
             A dict.
         """
-        state_dict = self.get_state_dict_from_memory()
-        if state_dict:
-            return state_dict
-        return {}
+        return self.get_state_dict_from_memory()
```

## Comparing `dlrover/trainer/torch/flash_checkpoint/ddp_engine.py` & `dlrover/trainer/torch/flash_checkpoint/full_ckpt_engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,20 +26,20 @@
     CheckpointEventType,
     DdpCheckpointSaver,
 )
 
 from .engine import CheckpointEngine, timer
 
 
-class DdpCheckpointEngine(CheckpointEngine):
+class FullCheckpointEngine(CheckpointEngine):
     """
     Save the checkpoint state dict of DDP model into the memory or storage.
 
     Examples::
-        >>> engine = DdpCheckpointEngine(
+        >>> engine = FullCheckpointEngine(
         >>>     checkpoint_dir="/tmp/checkpoint/"
         >>> )
         >>> for step, data in enumerate(dataloader):
         >>>     ...
         >>>     state_dict = model.state_dict()
         >>>     path = f"/tmp/checkpoint-{step}.pt"
         >>>     if step % 5 == 0:
@@ -119,34 +119,35 @@
         Args:
             step (int): the global iteration step.
             state_dict (dict): the state dict of model and optimizer to save.
             paths (dict): the key is a category in
                 ["model_states", "optim_states"] of the state dict and
                 the value is the path of storage to save.
         """
-        succeed = True
+        success = True
         if step > self._cached_step:
-            succeed = self.save_to_memory(step, state_dict, paths)
+            success = self.save_to_memory(step, state_dict, paths)
         # Only rank 0 persist the checkpoint to the storage.
         if dist.is_initialized():
             dist.barrier()
-        if succeed and self._rank == 0:
+        if success and self._rank == 0:
             event = CheckpointEvent(type=CheckpointEventType.SAVE, step=step)
             self._event_queue.put(event)
+        return success
 
     def load(self, resume_path=""):
         """
         The method firstly try to load the state dict from the shared memory.
         If there is no state dict in the shared memory, the method will
         load the state dict from the storage.
 
         Returns:
             A dict.
         """
-        state_dict = self.get_state_dict_from_memory()
+        _, state_dict = self.get_state_dict_from_memory()
         if state_dict:
             logger.info("Load the state dict from the CPU memory buffer.")
             paths = list(state_dict.keys())
             if len(paths) > 1:
                 raise ValueError(
                     "The checkpoint shared memory must has only the"
                     f"state dict of one path. Now, paths are {paths}"
```

## Comparing `dlrover-0.3.5.dist-info/LICENSE` & `dlrover-0.3.6.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `dlrover-0.3.5.dist-info/METADATA` & `dlrover-0.3.6.dist-info/METADATA`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dlrover
-Version: 0.3.5
+Version: 0.3.6
 Summary: An Automatic Distributed Deep Learning Framework
 Home-page: https://github.com/intelligent-machine-learning/dlrover
 Author: Ant Group
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

## Comparing `dlrover-0.3.5.dist-info/RECORD` & `dlrover-0.3.6.dist-info/RECORD`

 * *Files 2% similar despite different names*

```diff
@@ -9,87 +9,88 @@
 dlrover/python/__init__.py,sha256=vpZVhqJNwDst1RQ-nODrcGkpDsrj9CwRLfYNGyL2D1E,599
 dlrover/python/brain/__init__.py,sha256=vpZVhqJNwDst1RQ-nODrcGkpDsrj9CwRLfYNGyL2D1E,599
 dlrover/python/brain/client.py,sha256=YntlTJz5_WnkeiSfPY6kRY15z5D5G8uNbbOAAyZTrvI,11103
 dlrover/python/common/__init__.py,sha256=vpZVhqJNwDst1RQ-nODrcGkpDsrj9CwRLfYNGyL2D1E,599
 dlrover/python/common/constants.py,sha256=X9HzV8-tGB8uwsdtQOITe7FAbrIbMs86VUtEHtm1AcE,7036
 dlrover/python/common/env_utils.py,sha256=8IQ_d8X1Z23CAUdc2XutLVMp1s_hkjXW1khIWnCsrVI,1715
 dlrover/python/common/global_context.py,sha256=X7YTAAC1Pd6cxleei3-H_QLFLWjUBQiyGSTwXejkF5A,7547
-dlrover/python/common/grpc.py,sha256=t0SsabSgld45VBPeh5n2iOvrp99vdkhJQra2dn6pTIA,9787
+dlrover/python/common/grpc.py,sha256=hZpSINdrmaj7YVXdUKglUN_dPAPfxiuSdMro1PAphSo,9966
 dlrover/python/common/log.py,sha256=s1m9hiuvEmUBC7MxSbSlMSJ-XzzHjt3A3BZXz9qtzM8,1377
-dlrover/python/common/multi_process.py,sha256=WEoDx1KhRMQx5T6qRSDVAXnuUnufsxP4Pqiu1RbUW7M,18512
+dlrover/python/common/multi_process.py,sha256=wy-hsjfWyuJkGQaCbeO-5KXxPWXF1Bq9ffPZuq-oflU,18440
 dlrover/python/common/node.py,sha256=d6Z25RRyptkErW57ENQASygRIAtTHI6sD6eZdCjELBU,11858
 dlrover/python/common/serialize.py,sha256=B2PLB4ROeasn8HiW0eOmUhMNmnFnZNg6Gsl-rhh1L9A,1186
 dlrover/python/common/singleton.py,sha256=TZp-_IcOFUDJ2l5AqYIkC0Ov0kqF3s_i3jDwkyQiHf8,1489
 dlrover/python/common/storage.py,sha256=5oywNBkDzop0_bNY0P5eu1QcQhMmntXrYwLXRkMb5Nw,8635
 dlrover/python/elastic_agent/__init__.py,sha256=vpZVhqJNwDst1RQ-nODrcGkpDsrj9CwRLfYNGyL2D1E,599
-dlrover/python/elastic_agent/master_client.py,sha256=ySdwj0tyxOgYy65YXXXxMpX5hMrWgkKfnev6-jaNmYA,14064
+dlrover/python/elastic_agent/master_client.py,sha256=n3_iZGmPP-H537c7YDJy9hUdkr-V2-6wcQtBzP3fH4k,14237
 dlrover/python/elastic_agent/config/__init__.py,sha256=vpZVhqJNwDst1RQ-nODrcGkpDsrj9CwRLfYNGyL2D1E,599
 dlrover/python/elastic_agent/config/paral_config_tuner.py,sha256=UwA_nOQspFd920JZQrO2OIlcQLyHL9MW4e_f2J61eF0,3717
 dlrover/python/elastic_agent/monitor/__init__.py,sha256=vpZVhqJNwDst1RQ-nODrcGkpDsrj9CwRLfYNGyL2D1E,599
 dlrover/python/elastic_agent/monitor/resource.py,sha256=SmcQU3HwV-UsrxJqil1W-fcUJY8Cc4YxRjAc9sonSsQ,5980
 dlrover/python/elastic_agent/monitor/training.py,sha256=G5MmNLxS26mTlzaN28KNhKmam1ND2-AuSfBo-XOjKHM,4659
 dlrover/python/elastic_agent/sharding/__init__.py,sha256=vpZVhqJNwDst1RQ-nODrcGkpDsrj9CwRLfYNGyL2D1E,599
 dlrover/python/elastic_agent/sharding/client.py,sha256=tXZwnb5gkTnKiPBkW29v0E5XtJU0aBrBLG8LEL7RqRU,11734
 dlrover/python/elastic_agent/sychronization/__init__.py,sha256=PPDUSDBrUEdum00XKyizIVb160YdBoWrFqQLcwmiJ9g,599
 dlrover/python/elastic_agent/sychronization/sync_client.py,sha256=KpZqNRc9B73jFgeEzDFlyDqbrYoFu2qcVHUIj4ozd-Y,2686
 dlrover/python/elastic_agent/tensorflow/__init__.py,sha256=vpZVhqJNwDst1RQ-nODrcGkpDsrj9CwRLfYNGyL2D1E,599
 dlrover/python/elastic_agent/tensorflow/elastic_ps.py,sha256=WcQ4aRYZD1WlkcYvqi5gifAzcSGFjATN7OinqHtSMBQ,3424
 dlrover/python/elastic_agent/tensorflow/hooks.py,sha256=TYelsg4pY0liS5Wfol3oPSqg23GEoKk-uOeWejb-e_8,4226
 dlrover/python/elastic_agent/tensorflow/profile_extractor.py,sha256=N7MsELFbfraXR9SY70XsE7v1T58CQUXbdCebRvyp6UQ,4556
 dlrover/python/elastic_agent/torch/__init__.py,sha256=PPDUSDBrUEdum00XKyizIVb160YdBoWrFqQLcwmiJ9g,599
-dlrover/python/elastic_agent/torch/ckpt_saver.py,sha256=iGQbPDYYub60ra7TGI9agMial9V30epeHa9ukL9rdXc,39197
+dlrover/python/elastic_agent/torch/ckpt_saver.py,sha256=t3IJyo0LDylKa6kkv_jI_dHKaktFbzuPpvDJY862YRU,40769
 dlrover/python/elastic_agent/torch/master_kv_store.py,sha256=-nN5erhZNAnpvLtusnDwTGoyOYVvk9DQlvAXFKWhjzE,4594
-dlrover/python/elastic_agent/torch/training.py,sha256=oBlHl39PumIkx0WhoGB0T_-uVqWO0fUkra7Mml8LhGc,38955
+dlrover/python/elastic_agent/torch/training.py,sha256=l7M9s2JLLjvSFdQ4MGR1T61CZFgahL6n9D2GS8NCV44,39591
 dlrover/python/master/__init__.py,sha256=vpZVhqJNwDst1RQ-nODrcGkpDsrj9CwRLfYNGyL2D1E,599
 dlrover/python/master/args.py,sha256=CxR4Pr9j7l5Ta19ILv7qNH5NuOfGtm682qhV_vR_iO4,3044
 dlrover/python/master/dist_master.py,sha256=3iEuSFOEmGUQNOM36HXQCG7XPXskT3w98bdjK_vngEA,11296
-dlrover/python/master/local_master.py,sha256=tNZWHrdcPkfZRm98ZbQiUkN2T7_KoZAYemh-3PWIqQI,4375
+dlrover/python/master/local_master.py,sha256=BvgwihVOSU--F-W59nFLGwv2TnS7IRUUkg5tnVkLRlQ,4416
 dlrover/python/master/main.py,sha256=dCMtDSu1PN8zTd2H6gACy6KyMmcdkOPA9rYVMg--LS8,2550
 dlrover/python/master/master.py,sha256=vE3WebhpEB8alBXUZku-jUXNGkLalK6JMYnEafGfKRs,928
-dlrover/python/master/servicer.py,sha256=v5xoflTizy2SLFhLapjsvUV9LBMrKXSSb4cFChh2_-0,22988
+dlrover/python/master/servicer.py,sha256=pDF1ul92Vmr0FUr2pkvZ0omVInOKVpFEnmofpSZBLzg,23356
 dlrover/python/master/cluster/__init__.py,sha256=PPDUSDBrUEdum00XKyizIVb160YdBoWrFqQLcwmiJ9g,599
 dlrover/python/master/cluster/quota.py,sha256=Kfzb8B1gV7xZXkwsGaiIjISDH9Q0mh1DqNLSBZzTWnw,1124
 dlrover/python/master/elastic_training/__init__.py,sha256=vpZVhqJNwDst1RQ-nODrcGkpDsrj9CwRLfYNGyL2D1E,599
 dlrover/python/master/elastic_training/elastic_ps.py,sha256=rhplRZ7sfT6hUDD1mPvI8Gpqy8M2RgaFqCI874pQ56Y,3494
 dlrover/python/master/elastic_training/kv_store_service.py,sha256=TTSz8pCc2wifmG_ecUREPDYFwcBgBm97H0G4n8Ta4xA,1017
-dlrover/python/master/elastic_training/rdzv_manager.py,sha256=KaabZxTNf0F9gN0DF-ZXahjjoRFnTp27YrDuh17DW2M,19740
+dlrover/python/master/elastic_training/net_topology.py,sha256=5Z8QudeA2x00Iu7WrlsHIpvGNiw3AKnQY19ajSOGHk0,2852
+dlrover/python/master/elastic_training/rdzv_manager.py,sha256=r0S0TpNX1nus_YvvjuOzftEawHZzfdeDAZgqosavj-o,22102
 dlrover/python/master/elastic_training/sync_service.py,sha256=EXlW9UlRrn4nO8DNh4WceRJYbNYAC0Z_u_-PSP8caX4,4971
 dlrover/python/master/hyperparams/__init__.py,sha256=PPDUSDBrUEdum00XKyizIVb160YdBoWrFqQLcwmiJ9g,599
 dlrover/python/master/hyperparams/simple_strategy_generator.py,sha256=dLAelo1uYfZUzpNwQV9JcP8JV8WAn9HbhGL_hxewJG0,6818
 dlrover/python/master/hyperparams/strategy_generator.py,sha256=PmrcEvdYWTEd3YK2tJySHlyWLLEcn9WBgWTRIJRwfZo,1000
 dlrover/python/master/monitor/__init__.py,sha256=vpZVhqJNwDst1RQ-nODrcGkpDsrj9CwRLfYNGyL2D1E,599
 dlrover/python/master/monitor/error_monitor.py,sha256=tuK57cWuD5WaRcQKVoV9dTTHOiaVW1Aa5PuxmM7ysHw,4490
 dlrover/python/master/monitor/speed_monitor.py,sha256=D3l6fWDarLrwiFlFMqJHfVG-re8WRSLopGBKbMBeXho,7384
 dlrover/python/master/node/__init__.py,sha256=vpZVhqJNwDst1RQ-nODrcGkpDsrj9CwRLfYNGyL2D1E,599
-dlrover/python/master/node/dist_job_manager.py,sha256=zRwHMjIj_Sm_o0Xjq-adOaqOk8PGUw6Hf9Xk3H4c9qQ,34376
+dlrover/python/master/node/dist_job_manager.py,sha256=4YIDDY_1r_et2gu12sl0fTt08hOs1mNldOEiWrQ99S4,34327
 dlrover/python/master/node/event_callback.py,sha256=bbFSeouRx7f5Fiq_XwG-b8_LFQk9BcBDyQUhzhNzviE,13001
 dlrover/python/master/node/job_auto_scaler.py,sha256=ppWqLUwdgcnY8Q3p-JFGaLOrKgzBfazOVsKnBf49lYo,12665
 dlrover/python/master/node/job_manager.py,sha256=AKnVtldVeCZWmhtVWaiKuNpva0m9VBcEu9sImLC71BI,3661
 dlrover/python/master/node/local_job_manager.py,sha256=qFq-R6Eokn3WpKy4BRWRM4YOYf9AqvGOjWpGXqIPry0,5342
 dlrover/python/master/node/ps.py,sha256=eN2FqehCvCd9SfR44M6SYMpISgCWK55_v_voB4YNPag,14448
 dlrover/python/master/node/status_flow.py,sha256=vtZgVEnCmqTdZuRnV17iIVnwumRW2mj6GwUeDiEHqU8,4094
 dlrover/python/master/node/training_node.py,sha256=_6V3mpXtHPo5yiWDyprhLdbSZC5KcStbvuaJ51gKj7Q,13398
-dlrover/python/master/node/worker.py,sha256=fCk5TclhU6mC5kMo2kDLMI2dq9gfDUnKSmkTbHrsnXw,11211
+dlrover/python/master/node/worker.py,sha256=OcvkJeS5KMenPUpSEfyO5puloOdHztSELNruajIcZgo,11300
 dlrover/python/master/resource/__init__.py,sha256=vpZVhqJNwDst1RQ-nODrcGkpDsrj9CwRLfYNGyL2D1E,599
 dlrover/python/master/resource/brain_optimizer.py,sha256=KPJICeSkW-aS7ci3o4Mv6pg2lnNBsBqqfi1jKuNuzg0,4187
 dlrover/python/master/resource/job.py,sha256=JqnruLKjJFXRsTROqHeZPkZxCw5PCFnf1avYVb-7y9A,21672
 dlrover/python/master/resource/local_optimizer.py,sha256=Qr4oGr7lDbDjcQIjx9ywEBjBvDCI-NoYW_nxvcIfDVY,15828
 dlrover/python/master/resource/optimizer.py,sha256=E5mGrzoSGbt23fK3k82uYniwazGdtCMpzV8D1a1P8fI,6187
 dlrover/python/master/scaler/__init__.py,sha256=vpZVhqJNwDst1RQ-nODrcGkpDsrj9CwRLfYNGyL2D1E,599
 dlrover/python/master/scaler/base_scaler.py,sha256=CgFgYPyJDgxRoV22dMfQTlVH5f7Sk_gaMgsW5oZuZtQ,2202
 dlrover/python/master/scaler/elasticjob_scaler.py,sha256=O3UuDaL68TS81FoTkahQ-smH_zGmWgwvmr9NFSzet7U,8541
 dlrover/python/master/scaler/factory.py,sha256=NcuKpxoAjrEMqzIsTZEnHOFEmY8LZtRBmFQrKucC04U,1370
-dlrover/python/master/scaler/pod_scaler.py,sha256=N4RIInfXf-wWgmMubO6zYwxGqYERYz2xh3NJzNKxNzg,24570
+dlrover/python/master/scaler/pod_scaler.py,sha256=ISefeQUwGgJbMP-rLIJzf_xNckePgjtZFxx1yvDy1OA,24649
 dlrover/python/master/scaler/ray_scaler.py,sha256=QVL8AWBQec9up0SFJjikURX529lJ4m0eYMSF2OGy_wA,4659
 dlrover/python/master/shard/__init__.py,sha256=vpZVhqJNwDst1RQ-nODrcGkpDsrj9CwRLfYNGyL2D1E,599
 dlrover/python/master/shard/base_dataset_manager.py,sha256=3jQ-kWrffGsGiCUE6_iLh9aug4GXVja-iWjM4lWcZaQ,4574
 dlrover/python/master/shard/batch_dataset_manager.py,sha256=mD8TEi-yww-4G7cTwL-9irEul49twD2HdRk-Y-_4KEw,6964
 dlrover/python/master/shard/dataset_splitter.py,sha256=HqYEgzZ2YwrschCFeXuAjOc8wpkvZsHwtNdEAnIx3m0,16305
 dlrover/python/master/shard/streaming_dataset_manager.py,sha256=vr_-JNbzwR0BkK2g1WIAuIwZXWaJCU6EtYI6EDVm1ZM,7064
-dlrover/python/master/shard/task_manager.py,sha256=R3X1uBh5huzrluSAKMSCzobcJ1Dul2jRuk8y9KVpWo0,11171
+dlrover/python/master/shard/task_manager.py,sha256=dus4fccMWnqFx5kIs1Gc6jwvhBLeEBg8HidyFc-y2Ww,11152
 dlrover/python/master/stats/__init__.py,sha256=vpZVhqJNwDst1RQ-nODrcGkpDsrj9CwRLfYNGyL2D1E,599
 dlrover/python/master/stats/job_collector.py,sha256=mUCl-ZH1maL5qWwaYGx5MXD8nQDfN0h3-IV7gxyCbM4,6444
 dlrover/python/master/stats/reporter.py,sha256=8xDz_C6lBFsiPu647Hqa7iE74xiJGorwaFWxph1a_5Q,8776
 dlrover/python/master/stats/stats_backend.py,sha256=iJGkngsGLkXEWdN_2jv9xSfELrzpA2ow4Nle93WE4cQ,1567
 dlrover/python/master/stats/training_metrics.py,sha256=gaio2HHKCDSpd00JkyKY6y4uW-Y7Yry4Qmyj1svVhls,4820
 dlrover/python/master/watcher/__init__.py,sha256=vpZVhqJNwDst1RQ-nODrcGkpDsrj9CwRLfYNGyL2D1E,599
 dlrover/python/master/watcher/base_watcher.py,sha256=OZkgRItgEMNC53hv59ciNKNc8fSKzX016zRIrINF0vQ,1241
@@ -101,53 +102,54 @@
 dlrover/python/scheduler/job.py,sha256=EQs2up1YqcRFzaDgQ709PCjVj_pgezIGsNOkz9hjf3E,4285
 dlrover/python/scheduler/kubernetes.py,sha256=ydID-miTeUmJX-_oodr01Di1uSmfETT-LHaD2FoOPx0,18558
 dlrover/python/scheduler/ray.py,sha256=3XOrX-6faq-PSzbKQ5ml3IuVqk82zIwWyptxD3ctYOk,7397
 dlrover/python/tests/__init__.py,sha256=PPDUSDBrUEdum00XKyizIVb160YdBoWrFqQLcwmiJ9g,599
 dlrover/python/tests/test_agent_config_tuner.py,sha256=6JGa3UJs2JbC8wo3WIPdwrXrqCZ0jUyfAcIe9xFv9ew,2799
 dlrover/python/tests/test_agent_monitor.py,sha256=HJuwwkDmZ8ncGn98uBftBM1ewPXS8ZwxiflbUWedqI8,3405
 dlrover/python/tests/test_args.py,sha256=xq0ZkOq0wXdyvjuQppwj8GPR0XmjAUFFcb8GmPe2l4I,1049
-dlrover/python/tests/test_ckpt_saver.py,sha256=2cTNW3z-AWQPl7pi4EgLCGDxD0wBAtPMAVqlHSHS51s,9327
+dlrover/python/tests/test_ckpt_saver.py,sha256=rOH_FLL3U_gbnEfgOnIGmhpoEGCRPophe-ZcxkOKS1o,10521
 dlrover/python/tests/test_dataset_splitter.py,sha256=8y2Y1wXThIlZ4f4atVqIxbrWNmUb6fJfyr3t-Xbr58E,4583
 dlrover/python/tests/test_dataset_task_manager.py,sha256=dStylhcl1DIDG6xWTkxXrMXKsvthVos2zu0ZlC5ewag,4905
-dlrover/python/tests/test_elastic_training_agent.py,sha256=ungmh8LW0rOJ5g_MgFdsjxr6XgXGeA6Ufmv2Bc2vHQI,14821
+dlrover/python/tests/test_elastic_training_agent.py,sha256=djm8z06xAU1q3pjHbz6ETD4Gj6SX8L88W3woRfp-4Jo,14928
 dlrover/python/tests/test_elasticjob_scaler.py,sha256=HB7255Ytru9VltWZkp9Wa3zgaHi4yHMffgLSmF6DrrY,3383
 dlrover/python/tests/test_env_utils.py,sha256=ZomqS03hXAfXYePP5rga9iOnN2Dsq6-0el6n84RLnao,1873
 dlrover/python/tests/test_error_monitor.py,sha256=ScPG7mArYtMGnDWA0ApcsMqdb3sWe3P-SuR0r0d975M,1527
 dlrover/python/tests/test_event_callback.py,sha256=ti3LClbn6yQQ4gN-svxWW5WGk4Hwsd35RdRkLu5OW_s,3635
 dlrover/python/tests/test_global_context.py,sha256=nUQflu6UPsbr5_o3OOZRYbyS7L674QMLazjo2f_OKS4,1268
 dlrover/python/tests/test_grpc_utils.py,sha256=NKe_hTlT3G3CpfZTY3TKImYkx5pgS3Q3RfbkLfVSZYU,2158
 dlrover/python/tests/test_job_auto_scaler.py,sha256=uVhD_zOqUEWI5rorGBra_W0jrancyHijhW4FXmfvMyM,5292
 dlrover/python/tests/test_job_manager.py,sha256=fizGmAhat8ccfojvBjr2GdT6xbllLT0cBl4tqziOn0w,21350
 dlrover/python/tests/test_job_params.py,sha256=WxvoIFzf5qW658Mehru5pwVBlfmjwyTt3oY4yeXD1uM,2183
 dlrover/python/tests/test_k8s_utils.py,sha256=VcgxfuYZl6hu6E-zhrLJmB-43ykaeoi3tNy7T4FxwQ8,3188
 dlrover/python/tests/test_k8s_watcher.py,sha256=dC5g7jxwuCoVTdbSRYEqYmhH_KpCRoTcXqU3wpqU6kU,5920
 dlrover/python/tests/test_local_optimizer.py,sha256=ngdzP_r2yNntECv1SnsabnCdVgtO4QRjCNy7JNHWAVg,9142
 dlrover/python/tests/test_master.py,sha256=MqkueLGrY05f11ude_omP-SKxPX5m2396KPzqWw9cVE,5449
-dlrover/python/tests/test_master_client.py,sha256=FDxfxy1SIIIFk0ocaXfIgV5CVUQDgit2YEiMT5nUneU,5318
-dlrover/python/tests/test_multi_process.py,sha256=A3jjd5CquVJaxGc-Iwh3AWP8YAH0GvVGUsX7xVaf-rU,3476
+dlrover/python/tests/test_master_client.py,sha256=bVfAID_KfMTSxR8-HSmCaGqVJbQAg_Ep_-2ke9b4Tkg,5455
+dlrover/python/tests/test_multi_process.py,sha256=shThZ-ZTB0cQTbbY3TDGMjw0FR6QCea3pFZO4olDx-4,3773
+dlrover/python/tests/test_net_topology.py,sha256=BHuEvjSy9zLmm_oB9SIz4TbqA4aGjoyP2KhuMcLwVjE,1816
 dlrover/python/tests/test_node.py,sha256=JfwSa_xHW8oChUyCKSmB5PTohF6gxxoCQEHxMe8pbXE,1943
-dlrover/python/tests/test_pod_scaler.py,sha256=LUXylZTnShndmnE877pW0Kfud7yoeb34qtHoU656qOg,9260
+dlrover/python/tests/test_pod_scaler.py,sha256=O_NHV1neCRuUOebd-ECmb9z1PhJ2OVDHOWlabOyhHnY,9506
 dlrover/python/tests/test_ps_manager.py,sha256=mZZYUUZT-apGUq3qH2pwe-1ObnG6F72XIl6gOtmMLe4,7411
 dlrover/python/tests/test_ray_client.py,sha256=PPDUSDBrUEdum00XKyizIVb160YdBoWrFqQLcwmiJ9g,599
 dlrover/python/tests/test_ray_job_args.py,sha256=0gSfBb3u-_GFCj9dOpRdvCJ6g0QFEbi3dudYFt6Pqdo,1976
 dlrover/python/tests/test_ray_scaler.py,sha256=xN4dPhtrMCzKdzckTwELdBbOtzdGbJQtODegm5Ku_KI,971
 dlrover/python/tests/test_ray_watcher.py,sha256=PPDUSDBrUEdum00XKyizIVb160YdBoWrFqQLcwmiJ9g,599
-dlrover/python/tests/test_rdzv_manager.py,sha256=-1BonNw9sy-LBtUbEncY2viBogzZmeJOFqqfh20nOWo,12111
+dlrover/python/tests/test_rdzv_manager.py,sha256=aTcoTMDvA6U7Kd-I6NwQnip0I0YQavq6v-psFTMatI4,12564
 dlrover/python/tests/test_resource_optimizer.py,sha256=R63qFU1nJ9gyMd675ft98IVGCjyWQmVC76uX0eBw-Bo,11635
-dlrover/python/tests/test_servicer.py,sha256=mZRzE_L7S2sE55JH0yhuAIxbdczXnI_WSB1HrRI6otA,17947
+dlrover/python/tests/test_servicer.py,sha256=zdZqm9tSC0XvdfxPix6h4TrF77dgNhAxaP89DIZq4X4,18420
 dlrover/python/tests/test_sharding_client.py,sha256=9fsp41zGpwo4tAmVtAg1OOynBteQ639Z6b7UT_40-ko,3687
 dlrover/python/tests/test_speed_monitor.py,sha256=5XBMjXWqyz2x3Ywn4G3f_E9njOOAknnYwyK1M9-U9ew,1783
 dlrover/python/tests/test_state_backend.py,sha256=uocRJZWt1RjcTshOYfseUUiT9Bl9x_7dSNI3cvExJPs,1344
 dlrover/python/tests/test_stats_collector.py,sha256=YZntX9yYoONRuGwaSzZiy5OUAmVy97SGSNAXd-pSkVs,3287
 dlrover/python/tests/test_storage.py,sha256=D_mfwnU5PaQ_3lV9myC1-qoUHZ71mgeZFpPlcqhhb9g,2703
 dlrover/python/tests/test_strategy_generator.py,sha256=onw1BfpQD9rfU9YbFB0LIHPFB54IlB9A0aS2eu6D0gw,3303
 dlrover/python/tests/test_sync_service.py,sha256=VAIi61kx7BLZKJI5qk-BHk-IC9lEoiD4OqLvPBIV5vk,2460
 dlrover/python/tests/test_task_manager.py,sha256=UE0fFwQrBFEM-LuLZl-vJYCaSM6q7OHI5MjtYdICYPo,5425
-dlrover/python/tests/test_utils.py,sha256=gJIlGJ2Oz-E4wh8xt7u8hpXZWVfqX0kL5uNuvTfh3jc,8568
-dlrover/python/tests/test_worker_manager.py,sha256=ooakx-h1Izsq_HKXG4cteplZpDLNM0yvFU80FzSNZTA,7206
+dlrover/python/tests/test_utils.py,sha256=laEXPiPmbHANWcEOAQTkvrvOHqfuZbD010Q3c18OcwM,8599
+dlrover/python/tests/test_worker_manager.py,sha256=-kST3cXREaz8me9PqDBtNz7wA6fsJuX0boTifIMVPPA,7354
 dlrover/python/util/__init__.py,sha256=PPDUSDBrUEdum00XKyizIVb160YdBoWrFqQLcwmiJ9g,599
 dlrover/python/util/reflect_util.py,sha256=6d__Wupk46-s5gwg5ChlZSJF5um4GDLhrZN-bz_oTnY,3856
 dlrover/python/util/actor_util/__init__.py,sha256=PPDUSDBrUEdum00XKyizIVb160YdBoWrFqQLcwmiJ9g,599
 dlrover/python/util/actor_util/parse_actor.py,sha256=QWQiECvoj4FVX1MnL_BtmCaZ3JHvcCvI-FWc8MVC2nA,1552
 dlrover/python/util/queue/__init__.py,sha256=PPDUSDBrUEdum00XKyizIVb160YdBoWrFqQLcwmiJ9g,599
 dlrover/python/util/queue/queue.py,sha256=aVR_a5vk6y5n5BAtMxBMA7XUhV04NUZfpDq7A1TKi8k,2834
 dlrover/python/util/state/__init__.py,sha256=PPDUSDBrUEdum00XKyizIVb160YdBoWrFqQLcwmiJ9g,599
@@ -190,44 +192,45 @@
 dlrover/trainer/tensorflow/util/dataset_util.py,sha256=qjz-NlmqBBwp-ztZrhegfJcvDYntjW2pFFzBLFuuPoM,5429
 dlrover/trainer/tensorflow/util/estimator_util.py,sha256=-ULYmgVFALFCd4oLGSbjZc3OQBl0dI26HUC9Uy2tnQc,8506
 dlrover/trainer/tensorflow/util/path_util.py,sha256=LQCCluOm2zR492dVuwW_z_hVtArgXVTkc1mnEjidHms,1122
 dlrover/trainer/tensorflow/util/tf_env_util.py,sha256=Zi0GaRhfHYytKVKcYNbTfh9E89hpRuADYzC0EyE3bjk,1598
 dlrover/trainer/tensorflow/util/tf_patch_util.py,sha256=8LjI9NclFCNPnZ63GIon0qgV7x5XqVUdDMFLkqugy-s,15226
 dlrover/trainer/tensorflow/util/tf_version_util.py,sha256=4zoYq-yImVA_6ymQCBdxwMCNMi8cT7_EQbe78uqq140,1104
 dlrover/trainer/torch/__init__.py,sha256=PPDUSDBrUEdum00XKyizIVb160YdBoWrFqQLcwmiJ9g,599
-dlrover/trainer/torch/elastic_run.py,sha256=XEImjClh3VJzh227E2Q0d8Rr54izG1hgzXWLRt5ajyg,11797
+dlrover/trainer/torch/elastic_run.py,sha256=oH5vVMLqHznj6AziPENFUg5d-dI1ZN__yOiz0Errloc,11832
 dlrover/trainer/torch/main.py,sha256=2lZr2YcXAFjKxYn4M4okmbThfnqd88BHUnMHh9jgYQk,690
 dlrover/trainer/torch/elastic/__init__.py,sha256=PPDUSDBrUEdum00XKyizIVb160YdBoWrFqQLcwmiJ9g,599
 dlrover/trainer/torch/elastic/dataloader.py,sha256=73-mMJyIEi0dOtHsyrYlOhD9vY00glRLP7USkPDfIOc,5422
 dlrover/trainer/torch/elastic/sampler.py,sha256=BLq3BUNiFQOMEAZn5LFdCoGzrptqoWpoApnuhd8RrPU,5981
 dlrover/trainer/torch/elastic/trainer.py,sha256=F_OclqqnTnMcc3fjTXQb5d0ZcG0rXM-GJ9RLrpH1wm8,11244
 dlrover/trainer/torch/flash_checkpoint/__init__.py,sha256=PPDUSDBrUEdum00XKyizIVb160YdBoWrFqQLcwmiJ9g,599
 dlrover/trainer/torch/flash_checkpoint/checkpointer.py,sha256=uh5SQgZZc_VH2PCGXlaJWhRtBDntq4oOX1nhTbuXyIU,2534
-dlrover/trainer/torch/flash_checkpoint/ddp.py,sha256=NydbiUqO3otDUh06mma6S4aHTVYF6qYDotj5Xk7t3LY,4189
-dlrover/trainer/torch/flash_checkpoint/ddp_engine.py,sha256=XrTMHVSFmqzjoqQqW7USn4Y-3f0iNqCFDORn25dRhlE,7857
-dlrover/trainer/torch/flash_checkpoint/deepspeed.py,sha256=yV0renuQJdxiR6OOT9N-8MwzaYwddn8_VAjGmNALAAM,8784
-dlrover/trainer/torch/flash_checkpoint/deepspeed_engine.py,sha256=8A5VSncvTniaAkFw8RHrAkgFV6dOH02uGycJ_U1eC0A,6101
-dlrover/trainer/torch/flash_checkpoint/engine.py,sha256=wP1jTA-mS3hYGtmE4eKX7wW7Xk2X7hj0TLjrzXaH92Y,14158
-dlrover/trainer/torch/flash_checkpoint/fsdp.py,sha256=DcjV19kGFCoHuV-GSMwgBAXYBsD590Y6xL6T1y3yWCE,3961
+dlrover/trainer/torch/flash_checkpoint/ddp.py,sha256=jyZtTcEbjHluGkSHYq9DdUs9C_tQXrrwhGcHdlj4P8I,4247
+dlrover/trainer/torch/flash_checkpoint/deepspeed.py,sha256=VnEWkFviXaerkhLeh1Mstlatot5NCcEUygMmQMerL24,8646
+dlrover/trainer/torch/flash_checkpoint/deepspeed_engine.py,sha256=OA-yFN8bit-KgzEpx7cuXiebowuU0z7tO2DX073TC60,6280
+dlrover/trainer/torch/flash_checkpoint/engine.py,sha256=SZJVB53sy7zvR77bxAId4AxuoNyaZJMSOmJ7DbzKUII,14280
+dlrover/trainer/torch/flash_checkpoint/fsdp.py,sha256=Cj5oEe_cHDOW2-QitPfQFduGS2Ym2QrQYKBI01KnhCo,10397
 dlrover/trainer/torch/flash_checkpoint/fsdp_engine.py,sha256=B90iLS8CaNsVzp7JOTmDNIuxFZp9lGfhoiGn7hYgabQ,19976
+dlrover/trainer/torch/flash_checkpoint/full_ckpt_engine.py,sha256=OmQ5ZmCqRh3OvWFj3uYWZbKumPhB7j9kYTFv1lp6quk,7885
+dlrover/trainer/torch/flash_checkpoint/hf_trainer.py,sha256=_ehKQc_8GPK30lE-mJUpVHMq21ySuvAjOsQ4K0u6eQM,14246
 dlrover/trainer/torch/flash_checkpoint/megatron.py,sha256=5V86EwbyawfT7nRlJqOBdml5M0BwDSnKAALpN38Cqds,7823
-dlrover/trainer/torch/flash_checkpoint/megatron_dist_ckpt.py,sha256=288teHhSHW1TLC3rtWoQDF8Pp9cEZiB9MvEMfHd7qrE,19611
-dlrover/trainer/torch/flash_checkpoint/megatron_engine.py,sha256=eQ2h_ujtNLPaD8AqS8OPzpWhr3qQXXAfsMkeuDjx3dI,9780
+dlrover/trainer/torch/flash_checkpoint/megatron_dist_ckpt.py,sha256=gp-rKa1_6nQalgitl2QNLH-fkFwAL4Ns25ZOx5RZuGY,20464
+dlrover/trainer/torch/flash_checkpoint/megatron_engine.py,sha256=uBcHmHqNDe7Sr0nzfQBE2yaNdraV2SeE2JGW4_5pEvo,9626
 dlrover/trainer/torch/node_check/__init__.py,sha256=wfC0_tw9vplJaggtrT0BB0RM7a2NmB4sfZVnI-sV58E,599
 dlrover/trainer/torch/node_check/ascend_npu.py,sha256=9mRCvnoUncLqxrPywlAPeKqdY9lBSSmn_YTU3q8PG50,1645
 dlrover/trainer/torch/node_check/nvidia_gpu.py,sha256=ZUvLHUEtRJSVXgNcvhHIrKaRRw5hD3-vSq4q-ewg9h4,1373
 dlrover/trainer/torch/node_check/utils.py,sha256=bnGua0UmYaWIh2P62ggC8y5zHmEgw9klcg2jKAj4pxw,2890
 dlrover/trainer/util/__init__.py,sha256=vpZVhqJNwDst1RQ-nODrcGkpDsrj9CwRLfYNGyL2D1E,599
 dlrover/trainer/util/args_util.py,sha256=cWIf8seZuB-CZDDj2451M93RhedlZOoiK7Wje_61RJ8,2031
 dlrover/trainer/util/conf_util.py,sha256=0Qzx2glA0nwYe335RRq8zV9Rx-i9tLVKz6Pzz5NO5fs,6436
 dlrover/trainer/util/log_util.py,sha256=v0sxOgR0IWQl6odSXFc1h-GTHyeeCb7-MlQuLjiTfrA,2863
 dlrover/trainer/util/net_util.py,sha256=RLWB5efGRUgaXMbJk0uzdLuyboNEcOVhbFJb-VXG2tI,736
 dlrover/trainer/util/reflect_util.py,sha256=6MSIuzdcKqODcrH35oWINzE-oQa-Y58XIxi3QPkJWGM,3860
 dlrover/trainer/worker/__init__.py,sha256=vpZVhqJNwDst1RQ-nODrcGkpDsrj9CwRLfYNGyL2D1E,599
 dlrover/trainer/worker/tf_kubernetes_worker.py,sha256=ItXRn7H6ts1XD12dIJD7me5L061dUXIBKHF5lpCAFqI,3540
 dlrover/trainer/worker/tf_ray_worker.py,sha256=AXXhQqiRBAwy0jWrw69HBVR4Qq8qSTPr4ivTrJ7EoSo,6927
-dlrover-0.3.5.dist-info/LICENSE,sha256=9-m2Y33Gdwo-6MPmAHTXF3nBJ7_HBvL5b9_ttmjvKiY,13484
-dlrover-0.3.5.dist-info/METADATA,sha256=F_Ew6VQpqsIOsL8YDF4ydT2tmpB970rSm4HERfsLRzA,1008
-dlrover-0.3.5.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-dlrover-0.3.5.dist-info/entry_points.txt,sha256=Yov3tA1wyZ8xs5vw1f6YW7XgzeGtClcj62FfLU9l7wY,65
-dlrover-0.3.5.dist-info/top_level.txt,sha256=DBXgCrSsRqJf0F1cJOaCbBv9tmdt3d7C6qEOFPBhCgg,8
-dlrover-0.3.5.dist-info/RECORD,,
+dlrover-0.3.6.dist-info/LICENSE,sha256=9-m2Y33Gdwo-6MPmAHTXF3nBJ7_HBvL5b9_ttmjvKiY,13484
+dlrover-0.3.6.dist-info/METADATA,sha256=Emo-UT6HbOlYQSVSJpd3pvHsozKnqKi74IHPQ761wzI,1008
+dlrover-0.3.6.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+dlrover-0.3.6.dist-info/entry_points.txt,sha256=Yov3tA1wyZ8xs5vw1f6YW7XgzeGtClcj62FfLU9l7wY,65
+dlrover-0.3.6.dist-info/top_level.txt,sha256=DBXgCrSsRqJf0F1cJOaCbBv9tmdt3d7C6qEOFPBhCgg,8
+dlrover-0.3.6.dist-info/RECORD,,
```


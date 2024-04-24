# Comparing `tmp/nucliadb-3.0.3.post447-py3-none-any.whl.zip` & `tmp/nucliadb-3.0.3.post450-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,458 +1,458 @@
-Zip file size: 755062 bytes, number of entries: 456
--rw-r--r--  2.0 unx     1135 b- defN 24-Apr-22 20:05 migrations/0001_bootstrap.py
--rw-r--r--  2.0 unx     1177 b- defN 24-Apr-22 20:05 migrations/0002_rollover_shards.py
--rw-r--r--  2.0 unx     2436 b- defN 24-Apr-22 20:05 migrations/0003_allfields_key.py
--rw-r--r--  2.0 unx     1177 b- defN 24-Apr-22 20:05 migrations/0004_rollover_shards.py
--rw-r--r--  2.0 unx     1177 b- defN 24-Apr-22 20:05 migrations/0005_rollover_shards.py
--rw-r--r--  2.0 unx     1024 b- defN 24-Apr-22 20:05 migrations/0006_rollover_shards.py
--rw-r--r--  2.0 unx     1301 b- defN 24-Apr-22 20:05 migrations/0008_cleanup_leftover_rollover_metadata.py
--rw-r--r--  2.0 unx     1378 b- defN 24-Apr-22 20:05 migrations/0009_upgrade_relations_and_texts_to_v2.py
--rw-r--r--  2.0 unx     1610 b- defN 24-Apr-22 20:05 migrations/0010_fix_corrupt_indexes.py
--rw-r--r--  2.0 unx     1843 b- defN 24-Apr-22 20:05 migrations/0011_materialize_labelset_ids.py
--rw-r--r--  2.0 unx     1443 b- defN 24-Apr-22 20:05 migrations/0012_rollover_shards.py
--rw-r--r--  2.0 unx     1024 b- defN 24-Apr-22 20:05 migrations/0013_rollover_shards.py
--rw-r--r--  2.0 unx     1382 b- defN 24-Apr-22 20:05 migrations/0014_rollover_shards.py
--rw-r--r--  2.0 unx     1462 b- defN 24-Apr-22 20:05 migrations/0015_targeted_rollover.py
--rw-r--r--  2.0 unx     2506 b- defN 24-Apr-22 20:05 migrations/0016_upgrade_to_paragraphs_v2.py
--rw-r--r--  2.0 unx     2100 b- defN 24-Apr-22 20:05 migrations/0017_multiple_writable_shards.py
--rw-r--r--  2.0 unx     2264 b- defN 24-Apr-22 20:05 migrations/0018_purge_orphan_kbslugs.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-22 20:05 migrations/__init__.py
--rw-r--r--  2.0 unx      891 b- defN 24-Apr-22 20:05 nucliadb/__init__.py
--rw-r--r--  2.0 unx     3733 b- defN 24-Apr-22 20:05 nucliadb/health.py
--rw-r--r--  2.0 unx    11626 b- defN 24-Apr-22 20:05 nucliadb/learning_proxy.py
--rw-r--r--  2.0 unx     4806 b- defN 24-Apr-22 20:05 nucliadb/metrics_exporter.py
--rw-r--r--  2.0 unx     2272 b- defN 24-Apr-22 20:05 nucliadb/openapi.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-22 20:05 nucliadb/py.typed
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-22 20:05 nucliadb/common/__init__.py
--rw-r--r--  2.0 unx     4905 b- defN 24-Apr-22 20:05 nucliadb/common/locking.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-22 20:05 nucliadb/common/cluster/__init__.py
--rw-r--r--  2.0 unx     5090 b- defN 24-Apr-22 20:05 nucliadb/common/cluster/base.py
--rw-r--r--  2.0 unx     1495 b- defN 24-Apr-22 20:05 nucliadb/common/cluster/exceptions.py
--rw-r--r--  2.0 unx     3658 b- defN 24-Apr-22 20:05 nucliadb/common/cluster/grpc_node_dummy.py
--rw-r--r--  2.0 unx     3429 b- defN 24-Apr-22 20:05 nucliadb/common/cluster/index_node.py
--rw-r--r--  2.0 unx    21231 b- defN 24-Apr-22 20:05 nucliadb/common/cluster/manager.py
--rw-r--r--  2.0 unx     8490 b- defN 24-Apr-22 20:05 nucliadb/common/cluster/rebalance.py
--rw-r--r--  2.0 unx    19593 b- defN 24-Apr-22 20:05 nucliadb/common/cluster/rollover.py
--rw-r--r--  2.0 unx     2713 b- defN 24-Apr-22 20:05 nucliadb/common/cluster/settings.py
--rw-r--r--  2.0 unx     5494 b- defN 24-Apr-22 20:05 nucliadb/common/cluster/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-22 20:05 nucliadb/common/cluster/discovery/__init__.py
--rw-r--r--  2.0 unx     6553 b- defN 24-Apr-22 20:05 nucliadb/common/cluster/discovery/base.py
--rw-r--r--  2.0 unx    12518 b- defN 24-Apr-22 20:05 nucliadb/common/cluster/discovery/k8s.py
--rw-r--r--  2.0 unx     1957 b- defN 24-Apr-22 20:05 nucliadb/common/cluster/discovery/manual.py
--rw-r--r--  2.0 unx     1737 b- defN 24-Apr-22 20:05 nucliadb/common/cluster/discovery/single.py
--rw-r--r--  2.0 unx     1139 b- defN 24-Apr-22 20:05 nucliadb/common/cluster/discovery/types.py
--rw-r--r--  2.0 unx     2548 b- defN 24-Apr-22 20:05 nucliadb/common/cluster/discovery/utils.py
--rw-r--r--  2.0 unx      833 b- defN 24-Apr-22 20:05 nucliadb/common/cluster/standalone/__init__.py
--rw-r--r--  2.0 unx    13707 b- defN 24-Apr-22 20:05 nucliadb/common/cluster/standalone/grpc_node_binding.py
--rw-r--r--  2.0 unx     4683 b- defN 24-Apr-22 20:05 nucliadb/common/cluster/standalone/index_node.py
--rw-r--r--  2.0 unx     3444 b- defN 24-Apr-22 20:05 nucliadb/common/cluster/standalone/service.py
--rw-r--r--  2.0 unx     3386 b- defN 24-Apr-22 20:05 nucliadb/common/cluster/standalone/utils.py
--rw-r--r--  2.0 unx     3498 b- defN 24-Apr-22 20:05 nucliadb/common/context/__init__.py
--rw-r--r--  2.0 unx     1628 b- defN 24-Apr-22 20:05 nucliadb/common/context/fastapi.py
--rw-r--r--  2.0 unx     1813 b- defN 24-Apr-22 20:05 nucliadb/common/datamanagers/__init__.py
--rw-r--r--  2.0 unx     1451 b- defN 24-Apr-22 20:05 nucliadb/common/datamanagers/cluster.py
--rw-r--r--  2.0 unx     5383 b- defN 24-Apr-22 20:05 nucliadb/common/datamanagers/entities.py
--rw-r--r--  2.0 unx      883 b- defN 24-Apr-22 20:05 nucliadb/common/datamanagers/exceptions.py
--rw-r--r--  2.0 unx     3994 b- defN 24-Apr-22 20:05 nucliadb/common/datamanagers/kb.py
--rw-r--r--  2.0 unx     5389 b- defN 24-Apr-22 20:05 nucliadb/common/datamanagers/labels.py
--rw-r--r--  2.0 unx     1599 b- defN 24-Apr-22 20:05 nucliadb/common/datamanagers/processing.py
--rw-r--r--  2.0 unx     7637 b- defN 24-Apr-22 20:05 nucliadb/common/datamanagers/resources.py
--rw-r--r--  2.0 unx     5633 b- defN 24-Apr-22 20:05 nucliadb/common/datamanagers/rollover.py
--rw-r--r--  2.0 unx     1681 b- defN 24-Apr-22 20:05 nucliadb/common/datamanagers/utils.py
--rw-r--r--  2.0 unx     2055 b- defN 24-Apr-22 20:05 nucliadb/common/datamanagers/vectorsets.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-22 20:05 nucliadb/common/http_clients/__init__.py
--rw-r--r--  2.0 unx     2146 b- defN 24-Apr-22 20:05 nucliadb/common/http_clients/auth.py
--rw-r--r--  2.0 unx     1100 b- defN 24-Apr-22 20:05 nucliadb/common/http_clients/exceptions.py
--rw-r--r--  2.0 unx     7155 b- defN 24-Apr-22 20:05 nucliadb/common/http_clients/processing.py
--rw-r--r--  2.0 unx     1540 b- defN 24-Apr-22 20:05 nucliadb/common/http_clients/pypi.py
--rw-r--r--  2.0 unx     1551 b- defN 24-Apr-22 20:05 nucliadb/common/http_clients/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-22 20:05 nucliadb/common/maindb/__init__.py
--rw-r--r--  2.0 unx     3449 b- defN 24-Apr-22 20:05 nucliadb/common/maindb/driver.py
--rw-r--r--  2.0 unx      946 b- defN 24-Apr-22 20:05 nucliadb/common/maindb/exceptions.py
--rw-r--r--  2.0 unx     6769 b- defN 24-Apr-22 20:05 nucliadb/common/maindb/local.py
--rw-r--r--  2.0 unx     8391 b- defN 24-Apr-22 20:05 nucliadb/common/maindb/pg.py
--rw-r--r--  2.0 unx     6053 b- defN 24-Apr-22 20:05 nucliadb/common/maindb/redis.py
--rw-r--r--  2.0 unx    14502 b- defN 24-Apr-22 20:05 nucliadb/common/maindb/tikv.py
--rw-r--r--  2.0 unx     4109 b- defN 24-Apr-22 20:05 nucliadb/common/maindb/utils.py
--rw-r--r--  2.0 unx      932 b- defN 24-Apr-22 20:05 nucliadb/export_import/__init__.py
--rw-r--r--  2.0 unx     6171 b- defN 24-Apr-22 20:05 nucliadb/export_import/datamanager.py
--rw-r--r--  2.0 unx     1949 b- defN 24-Apr-22 20:05 nucliadb/export_import/exceptions.py
--rw-r--r--  2.0 unx     7116 b- defN 24-Apr-22 20:05 nucliadb/export_import/exporter.py
--rw-r--r--  2.0 unx     4258 b- defN 24-Apr-22 20:05 nucliadb/export_import/importer.py
--rw-r--r--  2.0 unx     2063 b- defN 24-Apr-22 20:05 nucliadb/export_import/models.py
--rw-r--r--  2.0 unx     2571 b- defN 24-Apr-22 20:05 nucliadb/export_import/tasks.py
--rw-r--r--  2.0 unx    19270 b- defN 24-Apr-22 20:05 nucliadb/export_import/utils.py
--rw-r--r--  2.0 unx     1011 b- defN 24-Apr-22 20:05 nucliadb/ingest/__init__.py
--rw-r--r--  2.0 unx     7277 b- defN 24-Apr-22 20:05 nucliadb/ingest/app.py
--rw-r--r--  2.0 unx     1005 b- defN 24-Apr-22 20:05 nucliadb/ingest/cache.py
--rw-r--r--  2.0 unx     2484 b- defN 24-Apr-22 20:05 nucliadb/ingest/partitions.py
--rw-r--r--  2.0 unx    19541 b- defN 24-Apr-22 20:05 nucliadb/ingest/processing.py
--rw-r--r--  2.0 unx    20277 b- defN 24-Apr-22 20:05 nucliadb/ingest/serialize.py
--rw-r--r--  2.0 unx     3183 b- defN 24-Apr-22 20:05 nucliadb/ingest/settings.py
--rw-r--r--  2.0 unx     2314 b- defN 24-Apr-22 20:05 nucliadb/ingest/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-22 20:05 nucliadb/ingest/consumer/__init__.py
--rw-r--r--  2.0 unx    11563 b- defN 24-Apr-22 20:05 nucliadb/ingest/consumer/auditing.py
--rw-r--r--  2.0 unx    12159 b- defN 24-Apr-22 20:05 nucliadb/ingest/consumer/consumer.py
--rw-r--r--  2.0 unx     3788 b- defN 24-Apr-22 20:05 nucliadb/ingest/consumer/materializer.py
--rw-r--r--  2.0 unx     1075 b- defN 24-Apr-22 20:05 nucliadb/ingest/consumer/metrics.py
--rw-r--r--  2.0 unx     9543 b- defN 24-Apr-22 20:05 nucliadb/ingest/consumer/pull.py
--rw-r--r--  2.0 unx     6935 b- defN 24-Apr-22 20:05 nucliadb/ingest/consumer/service.py
--rw-r--r--  2.0 unx     4331 b- defN 24-Apr-22 20:05 nucliadb/ingest/consumer/shard_creator.py
--rw-r--r--  2.0 unx     2656 b- defN 24-Apr-22 20:05 nucliadb/ingest/consumer/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-22 20:05 nucliadb/ingest/fields/__init__.py
--rw-r--r--  2.0 unx    18433 b- defN 24-Apr-22 20:05 nucliadb/ingest/fields/base.py
--rw-r--r--  2.0 unx     6516 b- defN 24-Apr-22 20:05 nucliadb/ingest/fields/conversation.py
--rw-r--r--  2.0 unx     1223 b- defN 24-Apr-22 20:05 nucliadb/ingest/fields/date.py
--rw-r--r--  2.0 unx     1205 b- defN 24-Apr-22 20:05 nucliadb/ingest/fields/exceptions.py
--rw-r--r--  2.0 unx     5159 b- defN 24-Apr-22 20:05 nucliadb/ingest/fields/file.py
--rw-r--r--  2.0 unx     1547 b- defN 24-Apr-22 20:05 nucliadb/ingest/fields/generic.py
--rw-r--r--  2.0 unx     1235 b- defN 24-Apr-22 20:05 nucliadb/ingest/fields/keywordset.py
--rw-r--r--  2.0 unx     2250 b- defN 24-Apr-22 20:05 nucliadb/ingest/fields/layout.py
--rw-r--r--  2.0 unx     4084 b- defN 24-Apr-22 20:05 nucliadb/ingest/fields/link.py
--rw-r--r--  2.0 unx     1319 b- defN 24-Apr-22 20:05 nucliadb/ingest/fields/text.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-22 20:05 nucliadb/ingest/orm/__init__.py
--rw-r--r--  2.0 unx    28367 b- defN 24-Apr-22 20:05 nucliadb/ingest/orm/brain.py
--rw-r--r--  2.0 unx    15758 b- defN 24-Apr-22 20:05 nucliadb/ingest/orm/entities.py
--rw-r--r--  2.0 unx     1279 b- defN 24-Apr-22 20:05 nucliadb/ingest/orm/exceptions.py
--rw-r--r--  2.0 unx    18731 b- defN 24-Apr-22 20:05 nucliadb/ingest/orm/knowledgebox.py
--rw-r--r--  2.0 unx     1096 b- defN 24-Apr-22 20:05 nucliadb/ingest/orm/metrics.py
--rw-r--r--  2.0 unx    60647 b- defN 24-Apr-22 20:05 nucliadb/ingest/orm/resource.py
--rw-r--r--  2.0 unx     1739 b- defN 24-Apr-22 20:05 nucliadb/ingest/orm/synonyms.py
--rw-r--r--  2.0 unx     3683 b- defN 24-Apr-22 20:05 nucliadb/ingest/orm/utils.py
--rw-r--r--  2.0 unx    26460 b- defN 24-Apr-22 20:05 nucliadb/ingest/orm/processor/__init__.py
--rw-r--r--  2.0 unx     1690 b- defN 24-Apr-22 20:05 nucliadb/ingest/orm/processor/sequence_manager.py
--rw-r--r--  2.0 unx     2057 b- defN 24-Apr-22 20:05 nucliadb/ingest/service/__init__.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-22 20:05 nucliadb/ingest/service/exceptions.py
--rw-r--r--  2.0 unx    37355 b- defN 24-Apr-22 20:05 nucliadb/ingest/service/writer.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-22 20:05 nucliadb/ingest/tests/__init__.py
--rw-r--r--  2.0 unx     1157 b- defN 24-Apr-22 20:05 nucliadb/ingest/tests/conftest.py
--rw-r--r--  2.0 unx    24068 b- defN 24-Apr-22 20:05 nucliadb/ingest/tests/fixtures.py
--rw-r--r--  2.0 unx    62843 b- defN 24-Apr-22 20:05 nucliadb/ingest/tests/vectors.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-22 20:05 nucliadb/ingest/tests/integration/__init__.py
--rw-r--r--  2.0 unx      833 b- defN 24-Apr-22 20:05 nucliadb/ingest/tests/integration/consumer/__init__.py
--rw-r--r--  2.0 unx     2549 b- defN 24-Apr-22 20:05 nucliadb/ingest/tests/integration/consumer/test_auditing.py
--rw-r--r--  2.0 unx     2591 b- defN 24-Apr-22 20:05 nucliadb/ingest/tests/integration/consumer/test_materializer.py
--rw-r--r--  2.0 unx     4465 b- defN 24-Apr-22 20:05 nucliadb/ingest/tests/integration/consumer/test_pull.py
--rw-r--r--  2.0 unx     2763 b- defN 24-Apr-22 20:05 nucliadb/ingest/tests/integration/consumer/test_service.py
--rw-r--r--  2.0 unx     2019 b- defN 24-Apr-22 20:05 nucliadb/ingest/tests/integration/consumer/test_shard_creator.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-22 20:05 nucliadb/ingest/tests/integration/ingest/__init__.py
--rw-r--r--  2.0 unx    27334 b- defN 24-Apr-22 20:05 nucliadb/ingest/tests/integration/ingest/test_ingest.py
--rw-r--r--  2.0 unx     3040 b- defN 24-Apr-22 20:05 nucliadb/ingest/tests/integration/ingest/test_processing_engine.py
--rw-r--r--  2.0 unx     8586 b- defN 24-Apr-22 20:05 nucliadb/ingest/tests/integration/ingest/test_relations.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-22 20:05 nucliadb/ingest/tests/unit/__init__.py
--rw-r--r--  2.0 unx     1189 b- defN 24-Apr-22 20:05 nucliadb/ingest/tests/unit/test_cache.py
--rw-r--r--  2.0 unx     1432 b- defN 24-Apr-22 20:05 nucliadb/ingest/tests/unit/test_partitions.py
--rw-r--r--  2.0 unx     5807 b- defN 24-Apr-22 20:05 nucliadb/ingest/tests/unit/test_processing.py
--rw-r--r--  2.0 unx      978 b- defN 24-Apr-22 20:05 nucliadb/ingest/tests/unit/test_settings.py
--rw-r--r--  2.0 unx      833 b- defN 24-Apr-22 20:05 nucliadb/ingest/tests/unit/consumer/__init__.py
--rw-r--r--  2.0 unx     3981 b- defN 24-Apr-22 20:05 nucliadb/ingest/tests/unit/consumer/test_auditing.py
--rw-r--r--  2.0 unx     2472 b- defN 24-Apr-22 20:05 nucliadb/ingest/tests/unit/consumer/test_consumer.py
--rw-r--r--  2.0 unx     2063 b- defN 24-Apr-22 20:05 nucliadb/ingest/tests/unit/consumer/test_pull.py
--rw-r--r--  2.0 unx     4075 b- defN 24-Apr-22 20:05 nucliadb/ingest/tests/unit/consumer/test_shard_creator.py
--rw-r--r--  2.0 unx     1934 b- defN 24-Apr-22 20:05 nucliadb/ingest/tests/unit/consumer/test_utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-22 20:05 nucliadb/ingest/tests/unit/orm/__init__.py
--rw-r--r--  2.0 unx     9876 b- defN 24-Apr-22 20:05 nucliadb/ingest/tests/unit/orm/test_brain.py
--rw-r--r--  2.0 unx     2435 b- defN 24-Apr-22 20:05 nucliadb/ingest/tests/unit/orm/test_brain_vectors.py
--rw-r--r--  2.0 unx     1174 b- defN 24-Apr-22 20:05 nucliadb/ingest/tests/unit/orm/test_orm_utils.py
--rw-r--r--  2.0 unx     4045 b- defN 24-Apr-22 20:05 nucliadb/ingest/tests/unit/orm/test_processor.py
--rw-r--r--  2.0 unx    11005 b- defN 24-Apr-22 20:05 nucliadb/ingest/tests/unit/orm/test_resource.py
--rw-r--r--  2.0 unx     2216 b- defN 24-Apr-22 20:05 nucliadb/middleware/__init__.py
--rw-r--r--  2.0 unx     3912 b- defN 24-Apr-22 20:05 nucliadb/middleware/transaction.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-22 20:05 nucliadb/migrator/__init__.py
--rw-r--r--  2.0 unx     2119 b- defN 24-Apr-22 20:05 nucliadb/migrator/command.py
--rw-r--r--  2.0 unx     1334 b- defN 24-Apr-22 20:05 nucliadb/migrator/context.py
--rw-r--r--  2.0 unx     5104 b- defN 24-Apr-22 20:05 nucliadb/migrator/datamanager.py
--rw-r--r--  2.0 unx      889 b- defN 24-Apr-22 20:05 nucliadb/migrator/exceptions.py
--rw-r--r--  2.0 unx     9237 b- defN 24-Apr-22 20:05 nucliadb/migrator/migrator.py
--rw-r--r--  2.0 unx     1145 b- defN 24-Apr-22 20:05 nucliadb/migrator/models.py
--rw-r--r--  2.0 unx     1110 b- defN 24-Apr-22 20:05 nucliadb/migrator/settings.py
--rw-r--r--  2.0 unx     2346 b- defN 24-Apr-22 20:05 nucliadb/migrator/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-22 20:05 nucliadb/models/__init__.py
--rw-r--r--  2.0 unx     1599 b- defN 24-Apr-22 20:05 nucliadb/models/responses.py
--rw-r--r--  2.0 unx     6041 b- defN 24-Apr-22 20:05 nucliadb/purge/__init__.py
--rw-r--r--  2.0 unx     9364 b- defN 24-Apr-22 20:05 nucliadb/purge/orphan_shards.py
--rw-r--r--  2.0 unx     1328 b- defN 24-Apr-22 20:05 nucliadb/reader/__init__.py
--rw-r--r--  2.0 unx     3709 b- defN 24-Apr-22 20:05 nucliadb/reader/app.py
--rw-r--r--  2.0 unx     1366 b- defN 24-Apr-22 20:05 nucliadb/reader/lifecycle.py
--rw-r--r--  2.0 unx     1031 b- defN 24-Apr-22 20:05 nucliadb/reader/openapi.py
--rw-r--r--  2.0 unx     1447 b- defN 24-Apr-22 20:05 nucliadb/reader/run.py
--rw-r--r--  2.0 unx      872 b- defN 24-Apr-22 20:05 nucliadb/reader/api/__init__.py
--rw-r--r--  2.0 unx     2434 b- defN 24-Apr-22 20:05 nucliadb/reader/api/models.py
--rw-r--r--  2.0 unx     1110 b- defN 24-Apr-22 20:05 nucliadb/reader/api/v1/__init__.py
--rw-r--r--  2.0 unx    12368 b- defN 24-Apr-22 20:05 nucliadb/reader/api/v1/download.py
--rw-r--r--  2.0 unx     6450 b- defN 24-Apr-22 20:05 nucliadb/reader/api/v1/export_import.py
--rw-r--r--  2.0 unx     3632 b- defN 24-Apr-22 20:05 nucliadb/reader/api/v1/knowledgebox.py
--rw-r--r--  2.0 unx     2093 b- defN 24-Apr-22 20:05 nucliadb/reader/api/v1/learning_collector.py
--rw-r--r--  2.0 unx     4454 b- defN 24-Apr-22 20:05 nucliadb/reader/api/v1/learning_config.py
--rw-r--r--  2.0 unx    13928 b- defN 24-Apr-22 20:05 nucliadb/reader/api/v1/resource.py
--rw-r--r--  2.0 unx     1011 b- defN 24-Apr-22 20:05 nucliadb/reader/api/v1/router.py
--rw-r--r--  2.0 unx    13882 b- defN 24-Apr-22 20:05 nucliadb/reader/api/v1/services.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-22 20:05 nucliadb/reader/reader/__init__.py
--rw-r--r--  2.0 unx     8155 b- defN 24-Apr-22 20:05 nucliadb/reader/reader/notifications.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-22 20:05 nucliadb/reader/tests/__init__.py
--rw-r--r--  2.0 unx     1224 b- defN 24-Apr-22 20:05 nucliadb/reader/tests/conftest.py
--rw-r--r--  2.0 unx     4345 b- defN 24-Apr-22 20:05 nucliadb/reader/tests/fixtures.py
--rw-r--r--  2.0 unx     2748 b- defN 24-Apr-22 20:05 nucliadb/reader/tests/test_list_resources.py
--rw-r--r--  2.0 unx    10199 b- defN 24-Apr-22 20:05 nucliadb/reader/tests/test_reader_file_download.py
--rw-r--r--  2.0 unx    10586 b- defN 24-Apr-22 20:05 nucliadb/reader/tests/test_reader_resource.py
--rw-r--r--  2.0 unx     6535 b- defN 24-Apr-22 20:05 nucliadb/reader/tests/test_reader_resource_field.py
--rw-r--r--  2.0 unx     1535 b- defN 24-Apr-22 20:05 nucliadb/search/__init__.py
--rw-r--r--  2.0 unx     4905 b- defN 24-Apr-22 20:05 nucliadb/search/app.py
--rw-r--r--  2.0 unx     1956 b- defN 24-Apr-22 20:05 nucliadb/search/lifecycle.py
--rw-r--r--  2.0 unx     1016 b- defN 24-Apr-22 20:05 nucliadb/search/openapi.py
--rw-r--r--  2.0 unx    19798 b- defN 24-Apr-22 20:05 nucliadb/search/predict.py
--rw-r--r--  2.0 unx     1402 b- defN 24-Apr-22 20:05 nucliadb/search/run.py
--rw-r--r--  2.0 unx     1193 b- defN 24-Apr-22 20:05 nucliadb/search/settings.py
--rw-r--r--  2.0 unx     1037 b- defN 24-Apr-22 20:05 nucliadb/search/utilities.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-22 20:05 nucliadb/search/api/__init__.py
--rw-r--r--  2.0 unx     1272 b- defN 24-Apr-22 20:05 nucliadb/search/api/v1/__init__.py
--rw-r--r--  2.0 unx     9913 b- defN 24-Apr-22 20:05 nucliadb/search/api/v1/chat.py
--rw-r--r--  2.0 unx     2665 b- defN 24-Apr-22 20:05 nucliadb/search/api/v1/feedback.py
--rw-r--r--  2.0 unx     8804 b- defN 24-Apr-22 20:05 nucliadb/search/api/v1/find.py
--rw-r--r--  2.0 unx     7026 b- defN 24-Apr-22 20:05 nucliadb/search/api/v1/knowledgebox.py
--rw-r--r--  2.0 unx     3041 b- defN 24-Apr-22 20:05 nucliadb/search/api/v1/predict_proxy.py
--rw-r--r--  2.0 unx      988 b- defN 24-Apr-22 20:05 nucliadb/search/api/v1/router.py
--rw-r--r--  2.0 unx    18359 b- defN 24-Apr-22 20:05 nucliadb/search/api/v1/search.py
--rw-r--r--  2.0 unx     5928 b- defN 24-Apr-22 20:05 nucliadb/search/api/v1/suggest.py
--rw-r--r--  2.0 unx     2536 b- defN 24-Apr-22 20:05 nucliadb/search/api/v1/summarize.py
--rw-r--r--  2.0 unx     1412 b- defN 24-Apr-22 20:05 nucliadb/search/api/v1/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-22 20:05 nucliadb/search/api/v1/resource/__init__.py
--rw-r--r--  2.0 unx     6095 b- defN 24-Apr-22 20:05 nucliadb/search/api/v1/resource/ask.py
--rw-r--r--  2.0 unx     5887 b- defN 24-Apr-22 20:05 nucliadb/search/api/v1/resource/chat.py
--rw-r--r--  2.0 unx     5293 b- defN 24-Apr-22 20:05 nucliadb/search/api/v1/resource/search.py
--rw-r--r--  2.0 unx      833 b- defN 24-Apr-22 20:05 nucliadb/search/requesters/__init__.py
--rw-r--r--  2.0 unx     9070 b- defN 24-Apr-22 20:05 nucliadb/search/requesters/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-22 20:05 nucliadb/search/search/__init__.py
--rw-r--r--  2.0 unx     2746 b- defN 24-Apr-22 20:05 nucliadb/search/search/cache.py
--rw-r--r--  2.0 unx     1154 b- defN 24-Apr-22 20:05 nucliadb/search/search/exceptions.py
--rw-r--r--  2.0 unx     5465 b- defN 24-Apr-22 20:05 nucliadb/search/search/fetch.py
--rw-r--r--  2.0 unx     6513 b- defN 24-Apr-22 20:05 nucliadb/search/search/filters.py
--rw-r--r--  2.0 unx     4646 b- defN 24-Apr-22 20:05 nucliadb/search/search/find.py
--rw-r--r--  2.0 unx    17152 b- defN 24-Apr-22 20:05 nucliadb/search/search/find_merge.py
--rw-r--r--  2.0 unx    21282 b- defN 24-Apr-22 20:05 nucliadb/search/search/merge.py
--rw-r--r--  2.0 unx     1130 b- defN 24-Apr-22 20:05 nucliadb/search/search/metrics.py
--rw-r--r--  2.0 unx     8698 b- defN 24-Apr-22 20:05 nucliadb/search/search/paragraphs.py
--rw-r--r--  2.0 unx     3026 b- defN 24-Apr-22 20:05 nucliadb/search/search/predict_proxy.py
--rw-r--r--  2.0 unx    32831 b- defN 24-Apr-22 20:05 nucliadb/search/search/query.py
--rw-r--r--  2.0 unx     3149 b- defN 24-Apr-22 20:05 nucliadb/search/search/shards.py
--rw-r--r--  2.0 unx     5101 b- defN 24-Apr-22 20:05 nucliadb/search/search/summarize.py
--rw-r--r--  2.0 unx     2438 b- defN 24-Apr-22 20:05 nucliadb/search/search/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-22 20:05 nucliadb/search/search/chat/__init__.py
--rw-r--r--  2.0 unx     2058 b- defN 24-Apr-22 20:05 nucliadb/search/search/chat/images.py
--rw-r--r--  2.0 unx    20793 b- defN 24-Apr-22 20:05 nucliadb/search/search/chat/prompt.py
--rw-r--r--  2.0 unx    15347 b- defN 24-Apr-22 20:05 nucliadb/search/search/chat/query.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-22 20:05 nucliadb/search/tests/__init__.py
--rw-r--r--  2.0 unx     1295 b- defN 24-Apr-22 20:05 nucliadb/search/tests/conftest.py
--rw-r--r--  2.0 unx     6578 b- defN 24-Apr-22 20:05 nucliadb/search/tests/fixtures.py
--rw-r--r--  2.0 unx    15529 b- defN 24-Apr-22 20:05 nucliadb/search/tests/node.py
--rw-r--r--  2.0 unx      833 b- defN 24-Apr-22 20:05 nucliadb/search/tests/unit/__init__.py
--rw-r--r--  2.0 unx     2649 b- defN 24-Apr-22 20:05 nucliadb/search/tests/unit/test_app.py
--rw-r--r--  2.0 unx     3374 b- defN 24-Apr-22 20:05 nucliadb/search/tests/unit/test_find_merge.py
--rw-r--r--  2.0 unx     1400 b- defN 24-Apr-22 20:05 nucliadb/search/tests/unit/test_merge.py
--rw-r--r--  2.0 unx    17080 b- defN 24-Apr-22 20:05 nucliadb/search/tests/unit/test_predict.py
--rw-r--r--  2.0 unx     1317 b- defN 24-Apr-22 20:05 nucliadb/search/tests/unit/test_run.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-22 20:05 nucliadb/search/tests/unit/api/__init__.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-22 20:05 nucliadb/search/tests/unit/api/v1/__init__.py
--rw-r--r--  2.0 unx     2966 b- defN 24-Apr-22 20:05 nucliadb/search/tests/unit/api/v1/test_chat.py
--rw-r--r--  2.0 unx     2865 b- defN 24-Apr-22 20:05 nucliadb/search/tests/unit/api/v1/test_predict_proxy.py
--rw-r--r--  2.0 unx     2901 b- defN 24-Apr-22 20:05 nucliadb/search/tests/unit/api/v1/test_summarize.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-22 20:05 nucliadb/search/tests/unit/api/v1/resource/__init__.py
--rw-r--r--  2.0 unx     2411 b- defN 24-Apr-22 20:05 nucliadb/search/tests/unit/api/v1/resource/test_ask.py
--rw-r--r--  2.0 unx     3040 b- defN 24-Apr-22 20:05 nucliadb/search/tests/unit/api/v1/resource/test_chat.py
--rw-r--r--  2.0 unx      833 b- defN 24-Apr-22 20:05 nucliadb/search/tests/unit/search/__init__.py
--rw-r--r--  2.0 unx     8567 b- defN 24-Apr-22 20:05 nucliadb/search/tests/unit/search/test_chat_prompt.py
--rw-r--r--  2.0 unx     3736 b- defN 24-Apr-22 20:05 nucliadb/search/tests/unit/search/test_fetch.py
--rw-r--r--  2.0 unx     4306 b- defN 24-Apr-22 20:05 nucliadb/search/tests/unit/search/test_filters.py
--rw-r--r--  2.0 unx     4492 b- defN 24-Apr-22 20:05 nucliadb/search/tests/unit/search/test_paragraphs.py
--rw-r--r--  2.0 unx     3496 b- defN 24-Apr-22 20:05 nucliadb/search/tests/unit/search/test_predict_proxy.py
--rw-r--r--  2.0 unx     7001 b- defN 24-Apr-22 20:05 nucliadb/search/tests/unit/search/test_query.py
--rw-r--r--  2.0 unx      833 b- defN 24-Apr-22 20:05 nucliadb/search/tests/unit/search/requesters/__init__.py
--rw-r--r--  2.0 unx     6455 b- defN 24-Apr-22 20:05 nucliadb/search/tests/unit/search/requesters/test_utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-22 20:05 nucliadb/search/tests/unit/search/search/__init__.py
--rw-r--r--  2.0 unx     1759 b- defN 24-Apr-22 20:05 nucliadb/search/tests/unit/search/search/test_shards.py
--rw-r--r--  2.0 unx     2511 b- defN 24-Apr-22 20:05 nucliadb/search/tests/unit/search/search/test_utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-22 20:05 nucliadb/standalone/__init__.py
--rw-r--r--  2.0 unx     6746 b- defN 24-Apr-22 20:05 nucliadb/standalone/api_router.py
--rw-r--r--  2.0 unx     5763 b- defN 24-Apr-22 20:05 nucliadb/standalone/app.py
--rw-r--r--  2.0 unx     7800 b- defN 24-Apr-22 20:05 nucliadb/standalone/auth.py
--rw-r--r--  2.0 unx     5309 b- defN 24-Apr-22 20:05 nucliadb/standalone/config.py
--rw-r--r--  2.0 unx     6930 b- defN 24-Apr-22 20:05 nucliadb/standalone/introspect.py
--rw-r--r--  2.0 unx     2488 b- defN 24-Apr-22 20:05 nucliadb/standalone/lifecycle.py
--rw-r--r--  2.0 unx     1317 b- defN 24-Apr-22 20:05 nucliadb/standalone/purge.py
--rw-r--r--  2.0 unx     5336 b- defN 24-Apr-22 20:05 nucliadb/standalone/run.py
--rw-r--r--  2.0 unx     5781 b- defN 24-Apr-22 20:05 nucliadb/standalone/settings.py
--rw-r--r--  2.0 unx     3132 b- defN 24-Apr-22 20:05 nucliadb/standalone/versions.py
--rw-r--r--  2.0 unx     2285 b- defN 24-Apr-22 20:05 nucliadb/standalone/static/favicon.ico
--rw-r--r--  2.0 unx     3833 b- defN 24-Apr-22 20:05 nucliadb/standalone/static/index.html
--rw-r--r--  2.0 unx     2639 b- defN 24-Apr-22 20:05 nucliadb/standalone/static/logo.svg
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-22 20:05 nucliadb/standalone/tests/__init__.py
--rw-r--r--  2.0 unx     1294 b- defN 24-Apr-22 20:05 nucliadb/standalone/tests/conftest.py
--rw-r--r--  2.0 unx     1319 b- defN 24-Apr-22 20:05 nucliadb/standalone/tests/fixtures.py
--rw-r--r--  2.0 unx      833 b- defN 24-Apr-22 20:05 nucliadb/standalone/tests/unit/__init__.py
--rw-r--r--  2.0 unx     1722 b- defN 24-Apr-22 20:05 nucliadb/standalone/tests/unit/test_api_router.py
--rw-r--r--  2.0 unx     5509 b- defN 24-Apr-22 20:05 nucliadb/standalone/tests/unit/test_auth.py
--rw-r--r--  2.0 unx     1334 b- defN 24-Apr-22 20:05 nucliadb/standalone/tests/unit/test_introspect.py
--rw-r--r--  2.0 unx     1472 b- defN 24-Apr-22 20:05 nucliadb/standalone/tests/unit/test_run.py
--rw-r--r--  2.0 unx     1972 b- defN 24-Apr-22 20:05 nucliadb/standalone/tests/unit/test_versions.py
--rw-r--r--  2.0 unx     1037 b- defN 24-Apr-22 20:05 nucliadb/tasks/__init__.py
--rw-r--r--  2.0 unx     7655 b- defN 24-Apr-22 20:05 nucliadb/tasks/consumer.py
--rw-r--r--  2.0 unx      924 b- defN 24-Apr-22 20:05 nucliadb/tasks/logger.py
--rw-r--r--  2.0 unx     1378 b- defN 24-Apr-22 20:05 nucliadb/tasks/models.py
--rw-r--r--  2.0 unx     3457 b- defN 24-Apr-22 20:05 nucliadb/tasks/producer.py
--rw-r--r--  2.0 unx     1753 b- defN 24-Apr-22 20:05 nucliadb/tasks/registry.py
--rw-r--r--  2.0 unx     1360 b- defN 24-Apr-22 20:05 nucliadb/tasks/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-22 20:05 nucliadb/tests/__init__.py
--rw-r--r--  2.0 unx     1229 b- defN 24-Apr-22 20:05 nucliadb/tests/conftest.py
--rw-r--r--  2.0 unx    22365 b- defN 24-Apr-22 20:05 nucliadb/tests/fixtures.py
--rw-r--r--  2.0 unx     7549 b- defN 24-Apr-22 20:05 nucliadb/tests/tikv.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-22 20:05 nucliadb/tests/benchmarks/__init__.py
--rw-r--r--  2.0 unx     3032 b- defN 24-Apr-22 20:05 nucliadb/tests/benchmarks/test_search.py
--rw-r--r--  2.0 unx      919 b- defN 24-Apr-22 20:05 nucliadb/tests/knowledgeboxes/__init__.py
--rw-r--r--  2.0 unx     7002 b- defN 24-Apr-22 20:05 nucliadb/tests/knowledgeboxes/philosophy_books.py
--rw-r--r--  2.0 unx     3037 b- defN 24-Apr-22 20:05 nucliadb/tests/knowledgeboxes/ten_dummy_resources.py
--rw-r--r--  2.0 unx     1148 b- defN 24-Apr-22 20:05 nucliadb/tests/migrations/__init__.py
--rw-r--r--  2.0 unx     2726 b- defN 24-Apr-22 20:05 nucliadb/tests/migrations/test_migration_0017.py
--rw-r--r--  2.0 unx     3625 b- defN 24-Apr-22 20:05 nucliadb/tests/migrations/test_migration_0018.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-22 20:05 nucliadb/tests/unit/__init__.py
--rw-r--r--  2.0 unx     1487 b- defN 24-Apr-22 20:05 nucliadb/tests/unit/test_field_ids.py
--rw-r--r--  2.0 unx     2758 b- defN 24-Apr-22 20:05 nucliadb/tests/unit/test_health.py
--rw-r--r--  2.0 unx     1543 b- defN 24-Apr-22 20:05 nucliadb/tests/unit/test_kb_slugs.py
--rw-r--r--  2.0 unx     7892 b- defN 24-Apr-22 20:05 nucliadb/tests/unit/test_learning_proxy.py
--rw-r--r--  2.0 unx     2642 b- defN 24-Apr-22 20:05 nucliadb/tests/unit/test_metrics_exporter.py
--rw-r--r--  2.0 unx     1341 b- defN 24-Apr-22 20:05 nucliadb/tests/unit/test_openapi.py
--rw-r--r--  2.0 unx     3656 b- defN 24-Apr-22 20:05 nucliadb/tests/unit/test_purge.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-22 20:05 nucliadb/tests/unit/common/__init__.py
--rw-r--r--  2.0 unx     1268 b- defN 24-Apr-22 20:05 nucliadb/tests/unit/common/test_context.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-22 20:05 nucliadb/tests/unit/common/cluster/__init__.py
--rw-r--r--  2.0 unx    11955 b- defN 24-Apr-22 20:05 nucliadb/tests/unit/common/cluster/test_cluster.py
--rw-r--r--  2.0 unx     5387 b- defN 24-Apr-22 20:05 nucliadb/tests/unit/common/cluster/test_kb_shard_manager.py
--rw-r--r--  2.0 unx     9470 b- defN 24-Apr-22 20:05 nucliadb/tests/unit/common/cluster/test_rollover.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-22 20:05 nucliadb/tests/unit/common/cluster/discovery/__init__.py
--rw-r--r--  2.0 unx     5584 b- defN 24-Apr-22 20:05 nucliadb/tests/unit/common/cluster/discovery/test_k8s.py
--rw-r--r--  2.0 unx      833 b- defN 24-Apr-22 20:05 nucliadb/tests/unit/common/cluster/standalone/__init__.py
--rw-r--r--  2.0 unx     3750 b- defN 24-Apr-22 20:05 nucliadb/tests/unit/common/cluster/standalone/test_service.py
--rw-r--r--  2.0 unx     2114 b- defN 24-Apr-22 20:05 nucliadb/tests/unit/common/cluster/standalone/test_utils.py
--rw-r--r--  2.0 unx      833 b- defN 24-Apr-22 20:05 nucliadb/tests/unit/common/maindb/__init__.py
--rw-r--r--  2.0 unx     3579 b- defN 24-Apr-22 20:05 nucliadb/tests/unit/common/maindb/test_driver.py
--rw-r--r--  2.0 unx     1869 b- defN 24-Apr-22 20:05 nucliadb/tests/unit/common/maindb/test_tikv.py
--rw-r--r--  2.0 unx     2998 b- defN 24-Apr-22 20:05 nucliadb/tests/unit/common/maindb/test_utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-22 20:05 nucliadb/tests/unit/export_import/__init__.py
--rw-r--r--  2.0 unx     1435 b- defN 24-Apr-22 20:05 nucliadb/tests/unit/export_import/test_datamanager.py
--rw-r--r--  2.0 unx     9706 b- defN 24-Apr-22 20:05 nucliadb/tests/unit/export_import/test_utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-22 20:05 nucliadb/tests/unit/migrator/__init__.py
--rw-r--r--  2.0 unx     3233 b- defN 24-Apr-22 20:05 nucliadb/tests/unit/migrator/test_migrator.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-22 20:05 nucliadb/tests/unit/tasks/__init__.py
--rw-r--r--  2.0 unx     1375 b- defN 24-Apr-22 20:05 nucliadb/tests/unit/tasks/conftest.py
--rw-r--r--  2.0 unx     2714 b- defN 24-Apr-22 20:05 nucliadb/tests/unit/tasks/test_consumer.py
--rw-r--r--  2.0 unx     3189 b- defN 24-Apr-22 20:05 nucliadb/tests/unit/tasks/test_producer.py
--rw-r--r--  2.0 unx     1827 b- defN 24-Apr-22 20:05 nucliadb/tests/unit/tasks/test_tasks.py
--rw-r--r--  2.0 unx     2507 b- defN 24-Apr-22 20:05 nucliadb/tests/utils/__init__.py
--rw-r--r--  2.0 unx     1797 b- defN 24-Apr-22 20:05 nucliadb/tests/utils/aiohttp_session.py
--rw-r--r--  2.0 unx     2533 b- defN 24-Apr-22 20:05 nucliadb/tests/utils/entities.py
--rw-r--r--  2.0 unx     6327 b- defN 24-Apr-22 20:05 nucliadb/tests/utils/broker_messages/__init__.py
--rw-r--r--  2.0 unx     7557 b- defN 24-Apr-22 20:05 nucliadb/tests/utils/broker_messages/fields.py
--rw-r--r--  2.0 unx     1196 b- defN 24-Apr-22 20:05 nucliadb/tests/utils/broker_messages/helpers.py
--rw-r--r--  2.0 unx     1325 b- defN 24-Apr-22 20:05 nucliadb/train/__init__.py
--rw-r--r--  2.0 unx     3530 b- defN 24-Apr-22 20:05 nucliadb/train/app.py
--rw-r--r--  2.0 unx     3800 b- defN 24-Apr-22 20:05 nucliadb/train/generator.py
--rw-r--r--  2.0 unx     1698 b- defN 24-Apr-22 20:05 nucliadb/train/lifecycle.py
--rw-r--r--  2.0 unx     1198 b- defN 24-Apr-22 20:05 nucliadb/train/models.py
--rw-r--r--  2.0 unx     5706 b- defN 24-Apr-22 20:05 nucliadb/train/nodes.py
--rw-r--r--  2.0 unx     1400 b- defN 24-Apr-22 20:05 nucliadb/train/run.py
--rw-r--r--  2.0 unx     5926 b- defN 24-Apr-22 20:05 nucliadb/train/servicer.py
--rw-r--r--  2.0 unx     1415 b- defN 24-Apr-22 20:05 nucliadb/train/settings.py
--rw-r--r--  2.0 unx     1496 b- defN 24-Apr-22 20:05 nucliadb/train/types.py
--rw-r--r--  2.0 unx     3265 b- defN 24-Apr-22 20:05 nucliadb/train/upload.py
--rw-r--r--  2.0 unx     6420 b- defN 24-Apr-22 20:05 nucliadb/train/uploader.py
--rw-r--r--  2.0 unx     3179 b- defN 24-Apr-22 20:05 nucliadb/train/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-22 20:05 nucliadb/train/api/__init__.py
--rw-r--r--  2.0 unx     1479 b- defN 24-Apr-22 20:05 nucliadb/train/api/utils.py
--rw-r--r--  2.0 unx      928 b- defN 24-Apr-22 20:05 nucliadb/train/api/v1/__init__.py
--rw-r--r--  2.0 unx     2065 b- defN 24-Apr-22 20:05 nucliadb/train/api/v1/check.py
--rw-r--r--  2.0 unx      910 b- defN 24-Apr-22 20:05 nucliadb/train/api/v1/router.py
--rw-r--r--  2.0 unx     1905 b- defN 24-Apr-22 20:05 nucliadb/train/api/v1/shards.py
--rw-r--r--  2.0 unx     2129 b- defN 24-Apr-22 20:05 nucliadb/train/api/v1/trainset.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-22 20:05 nucliadb/train/generators/__init__.py
--rw-r--r--  2.0 unx     3723 b- defN 24-Apr-22 20:05 nucliadb/train/generators/field_classifier.py
--rw-r--r--  2.0 unx     6712 b- defN 24-Apr-22 20:05 nucliadb/train/generators/image_classifier.py
--rw-r--r--  2.0 unx     2789 b- defN 24-Apr-22 20:05 nucliadb/train/generators/paragraph_classifier.py
--rw-r--r--  2.0 unx     3590 b- defN 24-Apr-22 20:05 nucliadb/train/generators/paragraph_streaming.py
--rw-r--r--  2.0 unx     5372 b- defN 24-Apr-22 20:05 nucliadb/train/generators/question_answer_streaming.py
--rw-r--r--  2.0 unx     5160 b- defN 24-Apr-22 20:05 nucliadb/train/generators/sentence_classifier.py
--rw-r--r--  2.0 unx    10446 b- defN 24-Apr-22 20:05 nucliadb/train/generators/token_classifier.py
--rw-r--r--  2.0 unx     3877 b- defN 24-Apr-22 20:05 nucliadb/train/generators/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-22 20:05 nucliadb/train/tests/__init__.py
--rw-r--r--  2.0 unx     1125 b- defN 24-Apr-22 20:05 nucliadb/train/tests/conftest.py
--rw-r--r--  2.0 unx    11053 b- defN 24-Apr-22 20:05 nucliadb/train/tests/fixtures.py
--rw-r--r--  2.0 unx     4598 b- defN 24-Apr-22 20:05 nucliadb/train/tests/test_field_classification.py
--rw-r--r--  2.0 unx     2729 b- defN 24-Apr-22 20:05 nucliadb/train/tests/test_get_entities.py
--rw-r--r--  2.0 unx     1876 b- defN 24-Apr-22 20:05 nucliadb/train/tests/test_get_info.py
--rw-r--r--  2.0 unx     1382 b- defN 24-Apr-22 20:05 nucliadb/train/tests/test_get_ontology.py
--rw-r--r--  2.0 unx     2417 b- defN 24-Apr-22 20:05 nucliadb/train/tests/test_get_ontology_count.py
--rw-r--r--  2.0 unx     7669 b- defN 24-Apr-22 20:05 nucliadb/train/tests/test_image_classification.py
--rw-r--r--  2.0 unx     1416 b- defN 24-Apr-22 20:05 nucliadb/train/tests/test_list_fields.py
--rw-r--r--  2.0 unx     2944 b- defN 24-Apr-22 20:05 nucliadb/train/tests/test_list_paragraphs.py
--rw-r--r--  2.0 unx     1423 b- defN 24-Apr-22 20:05 nucliadb/train/tests/test_list_resources.py
--rw-r--r--  2.0 unx     2947 b- defN 24-Apr-22 20:05 nucliadb/train/tests/test_list_sentences.py
--rw-r--r--  2.0 unx     4645 b- defN 24-Apr-22 20:05 nucliadb/train/tests/test_paragraph_classification.py
--rw-r--r--  2.0 unx     4320 b- defN 24-Apr-22 20:05 nucliadb/train/tests/test_paragraph_streaming.py
--rw-r--r--  2.0 unx     8751 b- defN 24-Apr-22 20:05 nucliadb/train/tests/test_question_answer_streaming.py
--rw-r--r--  2.0 unx     5051 b- defN 24-Apr-22 20:05 nucliadb/train/tests/test_sentence_classification.py
--rw-r--r--  2.0 unx     5583 b- defN 24-Apr-22 20:05 nucliadb/train/tests/test_token_classification.py
--rw-r--r--  2.0 unx     3324 b- defN 24-Apr-22 20:05 nucliadb/train/tests/utils.py
--rw-r--r--  2.0 unx     1328 b- defN 24-Apr-22 20:05 nucliadb/writer/__init__.py
--rw-r--r--  2.0 unx     4268 b- defN 24-Apr-22 20:05 nucliadb/writer/app.py
--rw-r--r--  2.0 unx    19630 b- defN 24-Apr-22 20:05 nucliadb/writer/back_pressure.py
--rw-r--r--  2.0 unx      972 b- defN 24-Apr-22 20:05 nucliadb/writer/exceptions.py
--rw-r--r--  2.0 unx     1953 b- defN 24-Apr-22 20:05 nucliadb/writer/lifecycle.py
--rw-r--r--  2.0 unx     1032 b- defN 24-Apr-22 20:05 nucliadb/writer/openapi.py
--rw-r--r--  2.0 unx     1448 b- defN 24-Apr-22 20:05 nucliadb/writer/run.py
--rw-r--r--  2.0 unx     3074 b- defN 24-Apr-22 20:05 nucliadb/writer/settings.py
--rw-r--r--  2.0 unx     1036 b- defN 24-Apr-22 20:05 nucliadb/writer/utilities.py
--rw-r--r--  2.0 unx     1948 b- defN 24-Apr-22 20:05 nucliadb/writer/vectors.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-22 20:05 nucliadb/writer/api/__init__.py
--rw-r--r--  2.0 unx     1429 b- defN 24-Apr-22 20:05 nucliadb/writer/api/constants.py
--rw-r--r--  2.0 unx     1095 b- defN 24-Apr-22 20:05 nucliadb/writer/api/v1/__init__.py
--rw-r--r--  2.0 unx     6565 b- defN 24-Apr-22 20:05 nucliadb/writer/api/v1/export_import.py
--rw-r--r--  2.0 unx    28320 b- defN 24-Apr-22 20:05 nucliadb/writer/api/v1/field.py
--rw-r--r--  2.0 unx     5239 b- defN 24-Apr-22 20:05 nucliadb/writer/api/v1/knowledgebox.py
--rw-r--r--  2.0 unx     2052 b- defN 24-Apr-22 20:05 nucliadb/writer/api/v1/learning_config.py
--rw-r--r--  2.0 unx    19940 b- defN 24-Apr-22 20:05 nucliadb/writer/api/v1/resource.py
--rw-r--r--  2.0 unx     1034 b- defN 24-Apr-22 20:05 nucliadb/writer/api/v1/router.py
--rw-r--r--  2.0 unx    12733 b- defN 24-Apr-22 20:05 nucliadb/writer/api/v1/services.py
--rw-r--r--  2.0 unx    31464 b- defN 24-Apr-22 20:05 nucliadb/writer/api/v1/upload.py
--rw-r--r--  2.0 unx     1612 b- defN 24-Apr-22 20:05 nucliadb/writer/layouts/__init__.py
--rw-r--r--  2.0 unx     2115 b- defN 24-Apr-22 20:05 nucliadb/writer/layouts/v1.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-22 20:05 nucliadb/writer/resource/__init__.py
--rw-r--r--  2.0 unx     1425 b- defN 24-Apr-22 20:05 nucliadb/writer/resource/audit.py
--rw-r--r--  2.0 unx    10968 b- defN 24-Apr-22 20:05 nucliadb/writer/resource/basic.py
--rw-r--r--  2.0 unx    16319 b- defN 24-Apr-22 20:05 nucliadb/writer/resource/field.py
--rw-r--r--  2.0 unx     2022 b- defN 24-Apr-22 20:05 nucliadb/writer/resource/origin.py
--rw-r--r--  2.0 unx     1152 b- defN 24-Apr-22 20:05 nucliadb/writer/resource/slug.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-22 20:05 nucliadb/writer/tests/__init__.py
--rw-r--r--  2.0 unx     1200 b- defN 24-Apr-22 20:05 nucliadb/writer/tests/conftest.py
--rw-r--r--  2.0 unx     5971 b- defN 24-Apr-22 20:05 nucliadb/writer/tests/fixtures.py
--rw-r--r--  2.0 unx    15472 b- defN 24-Apr-22 20:05 nucliadb/writer/tests/test_fields.py
--rw-r--r--  2.0 unx    25913 b- defN 24-Apr-22 20:05 nucliadb/writer/tests/test_files.py
--rw-r--r--  2.0 unx     1729 b- defN 24-Apr-22 20:05 nucliadb/writer/tests/test_knowledgebox.py
--rw-r--r--  2.0 unx     4569 b- defN 24-Apr-22 20:05 nucliadb/writer/tests/test_reprocess_file_field.py
--rw-r--r--  2.0 unx    17449 b- defN 24-Apr-22 20:05 nucliadb/writer/tests/test_resources.py
--rw-r--r--  2.0 unx     5120 b- defN 24-Apr-22 20:05 nucliadb/writer/tests/test_service.py
--rw-r--r--  2.0 unx     6054 b- defN 24-Apr-22 20:05 nucliadb/writer/tests/test_tus.py
--rw-r--r--  2.0 unx     1287 b- defN 24-Apr-22 20:05 nucliadb/writer/tests/utils.py
--rw-r--r--  2.0 unx     5226 b- defN 24-Apr-22 20:05 nucliadb/writer/tus/__init__.py
--rw-r--r--  2.0 unx     5082 b- defN 24-Apr-22 20:05 nucliadb/writer/tus/dm.py
--rw-r--r--  2.0 unx     2186 b- defN 24-Apr-22 20:05 nucliadb/writer/tus/exceptions.py
--rw-r--r--  2.0 unx    14527 b- defN 24-Apr-22 20:05 nucliadb/writer/tus/gcs.py
--rw-r--r--  2.0 unx     5849 b- defN 24-Apr-22 20:05 nucliadb/writer/tus/local.py
--rw-r--r--  2.0 unx     4367 b- defN 24-Apr-22 20:05 nucliadb/writer/tus/pg.py
--rw-r--r--  2.0 unx     9069 b- defN 24-Apr-22 20:05 nucliadb/writer/tus/s3.py
--rw-r--r--  2.0 unx     4734 b- defN 24-Apr-22 20:05 nucliadb/writer/tus/storage.py
--rw-r--r--  2.0 unx     2556 b- defN 24-Apr-22 20:05 nucliadb/writer/tus/utils.py
--rw-r--r--  2.0 unx     4343 b- defN 24-Apr-22 20:06 nucliadb-3.0.3.post447.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-22 20:06 nucliadb-3.0.3.post447.dist-info/WHEEL
--rw-r--r--  2.0 unx     1268 b- defN 24-Apr-22 20:06 nucliadb-3.0.3.post447.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       20 b- defN 24-Apr-22 20:06 nucliadb-3.0.3.post447.dist-info/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 24-Apr-22 20:06 nucliadb-3.0.3.post447.dist-info/zip-safe
--rw-rw-r--  2.0 unx    42761 b- defN 24-Apr-22 20:06 nucliadb-3.0.3.post447.dist-info/RECORD
-456 files, 2247274 bytes uncompressed, 686684 bytes compressed:  69.5%
+Zip file size: 754424 bytes, number of entries: 456
+-rw-r--r--  2.0 unx     1135 b- defN 24-Apr-24 07:29 migrations/0001_bootstrap.py
+-rw-r--r--  2.0 unx     1177 b- defN 24-Apr-24 07:29 migrations/0002_rollover_shards.py
+-rw-r--r--  2.0 unx     2436 b- defN 24-Apr-24 07:29 migrations/0003_allfields_key.py
+-rw-r--r--  2.0 unx     1177 b- defN 24-Apr-24 07:29 migrations/0004_rollover_shards.py
+-rw-r--r--  2.0 unx     1177 b- defN 24-Apr-24 07:29 migrations/0005_rollover_shards.py
+-rw-r--r--  2.0 unx     1024 b- defN 24-Apr-24 07:29 migrations/0006_rollover_shards.py
+-rw-r--r--  2.0 unx     1301 b- defN 24-Apr-24 07:29 migrations/0008_cleanup_leftover_rollover_metadata.py
+-rw-r--r--  2.0 unx     1378 b- defN 24-Apr-24 07:29 migrations/0009_upgrade_relations_and_texts_to_v2.py
+-rw-r--r--  2.0 unx     1610 b- defN 24-Apr-24 07:29 migrations/0010_fix_corrupt_indexes.py
+-rw-r--r--  2.0 unx     1843 b- defN 24-Apr-24 07:29 migrations/0011_materialize_labelset_ids.py
+-rw-r--r--  2.0 unx     1443 b- defN 24-Apr-24 07:29 migrations/0012_rollover_shards.py
+-rw-r--r--  2.0 unx     1024 b- defN 24-Apr-24 07:29 migrations/0013_rollover_shards.py
+-rw-r--r--  2.0 unx     1382 b- defN 24-Apr-24 07:29 migrations/0014_rollover_shards.py
+-rw-r--r--  2.0 unx     1462 b- defN 24-Apr-24 07:29 migrations/0015_targeted_rollover.py
+-rw-r--r--  2.0 unx     2506 b- defN 24-Apr-24 07:29 migrations/0016_upgrade_to_paragraphs_v2.py
+-rw-r--r--  2.0 unx     2100 b- defN 24-Apr-24 07:29 migrations/0017_multiple_writable_shards.py
+-rw-r--r--  2.0 unx     2264 b- defN 24-Apr-24 07:29 migrations/0018_purge_orphan_kbslugs.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-24 07:29 migrations/__init__.py
+-rw-r--r--  2.0 unx      891 b- defN 24-Apr-24 07:29 nucliadb/__init__.py
+-rw-r--r--  2.0 unx     3733 b- defN 24-Apr-24 07:29 nucliadb/health.py
+-rw-r--r--  2.0 unx    11626 b- defN 24-Apr-24 07:29 nucliadb/learning_proxy.py
+-rw-r--r--  2.0 unx     4806 b- defN 24-Apr-24 07:29 nucliadb/metrics_exporter.py
+-rw-r--r--  2.0 unx     2272 b- defN 24-Apr-24 07:29 nucliadb/openapi.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-24 07:29 nucliadb/py.typed
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-24 07:29 nucliadb/common/__init__.py
+-rw-r--r--  2.0 unx     4905 b- defN 24-Apr-24 07:29 nucliadb/common/locking.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-24 07:29 nucliadb/common/cluster/__init__.py
+-rw-r--r--  2.0 unx     5090 b- defN 24-Apr-24 07:29 nucliadb/common/cluster/base.py
+-rw-r--r--  2.0 unx     1495 b- defN 24-Apr-24 07:29 nucliadb/common/cluster/exceptions.py
+-rw-r--r--  2.0 unx     3658 b- defN 24-Apr-24 07:29 nucliadb/common/cluster/grpc_node_dummy.py
+-rw-r--r--  2.0 unx     3429 b- defN 24-Apr-24 07:29 nucliadb/common/cluster/index_node.py
+-rw-r--r--  2.0 unx    21231 b- defN 24-Apr-24 07:29 nucliadb/common/cluster/manager.py
+-rw-r--r--  2.0 unx     8490 b- defN 24-Apr-24 07:29 nucliadb/common/cluster/rebalance.py
+-rw-r--r--  2.0 unx    19593 b- defN 24-Apr-24 07:29 nucliadb/common/cluster/rollover.py
+-rw-r--r--  2.0 unx     2713 b- defN 24-Apr-24 07:29 nucliadb/common/cluster/settings.py
+-rw-r--r--  2.0 unx     5494 b- defN 24-Apr-24 07:29 nucliadb/common/cluster/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-24 07:29 nucliadb/common/cluster/discovery/__init__.py
+-rw-r--r--  2.0 unx     6553 b- defN 24-Apr-24 07:29 nucliadb/common/cluster/discovery/base.py
+-rw-r--r--  2.0 unx    12518 b- defN 24-Apr-24 07:29 nucliadb/common/cluster/discovery/k8s.py
+-rw-r--r--  2.0 unx     1957 b- defN 24-Apr-24 07:29 nucliadb/common/cluster/discovery/manual.py
+-rw-r--r--  2.0 unx     1737 b- defN 24-Apr-24 07:29 nucliadb/common/cluster/discovery/single.py
+-rw-r--r--  2.0 unx     1139 b- defN 24-Apr-24 07:29 nucliadb/common/cluster/discovery/types.py
+-rw-r--r--  2.0 unx     2548 b- defN 24-Apr-24 07:29 nucliadb/common/cluster/discovery/utils.py
+-rw-r--r--  2.0 unx      833 b- defN 24-Apr-24 07:29 nucliadb/common/cluster/standalone/__init__.py
+-rw-r--r--  2.0 unx    13707 b- defN 24-Apr-24 07:29 nucliadb/common/cluster/standalone/grpc_node_binding.py
+-rw-r--r--  2.0 unx     4683 b- defN 24-Apr-24 07:29 nucliadb/common/cluster/standalone/index_node.py
+-rw-r--r--  2.0 unx     3444 b- defN 24-Apr-24 07:29 nucliadb/common/cluster/standalone/service.py
+-rw-r--r--  2.0 unx     3386 b- defN 24-Apr-24 07:29 nucliadb/common/cluster/standalone/utils.py
+-rw-r--r--  2.0 unx     3498 b- defN 24-Apr-24 07:29 nucliadb/common/context/__init__.py
+-rw-r--r--  2.0 unx     1628 b- defN 24-Apr-24 07:29 nucliadb/common/context/fastapi.py
+-rw-r--r--  2.0 unx     1813 b- defN 24-Apr-24 07:29 nucliadb/common/datamanagers/__init__.py
+-rw-r--r--  2.0 unx     1451 b- defN 24-Apr-24 07:29 nucliadb/common/datamanagers/cluster.py
+-rw-r--r--  2.0 unx     5383 b- defN 24-Apr-24 07:29 nucliadb/common/datamanagers/entities.py
+-rw-r--r--  2.0 unx      883 b- defN 24-Apr-24 07:29 nucliadb/common/datamanagers/exceptions.py
+-rw-r--r--  2.0 unx     3994 b- defN 24-Apr-24 07:29 nucliadb/common/datamanagers/kb.py
+-rw-r--r--  2.0 unx     5389 b- defN 24-Apr-24 07:29 nucliadb/common/datamanagers/labels.py
+-rw-r--r--  2.0 unx     1599 b- defN 24-Apr-24 07:29 nucliadb/common/datamanagers/processing.py
+-rw-r--r--  2.0 unx     7637 b- defN 24-Apr-24 07:29 nucliadb/common/datamanagers/resources.py
+-rw-r--r--  2.0 unx     5633 b- defN 24-Apr-24 07:29 nucliadb/common/datamanagers/rollover.py
+-rw-r--r--  2.0 unx     1681 b- defN 24-Apr-24 07:29 nucliadb/common/datamanagers/utils.py
+-rw-r--r--  2.0 unx     2055 b- defN 24-Apr-24 07:29 nucliadb/common/datamanagers/vectorsets.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-24 07:29 nucliadb/common/http_clients/__init__.py
+-rw-r--r--  2.0 unx     2146 b- defN 24-Apr-24 07:29 nucliadb/common/http_clients/auth.py
+-rw-r--r--  2.0 unx     1100 b- defN 24-Apr-24 07:29 nucliadb/common/http_clients/exceptions.py
+-rw-r--r--  2.0 unx     7155 b- defN 24-Apr-24 07:29 nucliadb/common/http_clients/processing.py
+-rw-r--r--  2.0 unx     1540 b- defN 24-Apr-24 07:29 nucliadb/common/http_clients/pypi.py
+-rw-r--r--  2.0 unx     1551 b- defN 24-Apr-24 07:29 nucliadb/common/http_clients/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-24 07:29 nucliadb/common/maindb/__init__.py
+-rw-r--r--  2.0 unx     3449 b- defN 24-Apr-24 07:29 nucliadb/common/maindb/driver.py
+-rw-r--r--  2.0 unx      946 b- defN 24-Apr-24 07:29 nucliadb/common/maindb/exceptions.py
+-rw-r--r--  2.0 unx     6769 b- defN 24-Apr-24 07:29 nucliadb/common/maindb/local.py
+-rw-r--r--  2.0 unx     8391 b- defN 24-Apr-24 07:29 nucliadb/common/maindb/pg.py
+-rw-r--r--  2.0 unx     6053 b- defN 24-Apr-24 07:29 nucliadb/common/maindb/redis.py
+-rw-r--r--  2.0 unx    14502 b- defN 24-Apr-24 07:29 nucliadb/common/maindb/tikv.py
+-rw-r--r--  2.0 unx     4109 b- defN 24-Apr-24 07:29 nucliadb/common/maindb/utils.py
+-rw-r--r--  2.0 unx      932 b- defN 24-Apr-24 07:29 nucliadb/export_import/__init__.py
+-rw-r--r--  2.0 unx     6171 b- defN 24-Apr-24 07:29 nucliadb/export_import/datamanager.py
+-rw-r--r--  2.0 unx     1949 b- defN 24-Apr-24 07:29 nucliadb/export_import/exceptions.py
+-rw-r--r--  2.0 unx     7116 b- defN 24-Apr-24 07:29 nucliadb/export_import/exporter.py
+-rw-r--r--  2.0 unx     4258 b- defN 24-Apr-24 07:29 nucliadb/export_import/importer.py
+-rw-r--r--  2.0 unx     2063 b- defN 24-Apr-24 07:29 nucliadb/export_import/models.py
+-rw-r--r--  2.0 unx     2571 b- defN 24-Apr-24 07:29 nucliadb/export_import/tasks.py
+-rw-r--r--  2.0 unx    19270 b- defN 24-Apr-24 07:29 nucliadb/export_import/utils.py
+-rw-r--r--  2.0 unx     1011 b- defN 24-Apr-24 07:29 nucliadb/ingest/__init__.py
+-rw-r--r--  2.0 unx     7277 b- defN 24-Apr-24 07:29 nucliadb/ingest/app.py
+-rw-r--r--  2.0 unx     1005 b- defN 24-Apr-24 07:29 nucliadb/ingest/cache.py
+-rw-r--r--  2.0 unx     2484 b- defN 24-Apr-24 07:29 nucliadb/ingest/partitions.py
+-rw-r--r--  2.0 unx    19541 b- defN 24-Apr-24 07:29 nucliadb/ingest/processing.py
+-rw-r--r--  2.0 unx    20277 b- defN 24-Apr-24 07:29 nucliadb/ingest/serialize.py
+-rw-r--r--  2.0 unx     3183 b- defN 24-Apr-24 07:29 nucliadb/ingest/settings.py
+-rw-r--r--  2.0 unx     2314 b- defN 24-Apr-24 07:29 nucliadb/ingest/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-24 07:29 nucliadb/ingest/consumer/__init__.py
+-rw-r--r--  2.0 unx    11563 b- defN 24-Apr-24 07:29 nucliadb/ingest/consumer/auditing.py
+-rw-r--r--  2.0 unx    12159 b- defN 24-Apr-24 07:29 nucliadb/ingest/consumer/consumer.py
+-rw-r--r--  2.0 unx     3788 b- defN 24-Apr-24 07:29 nucliadb/ingest/consumer/materializer.py
+-rw-r--r--  2.0 unx     1075 b- defN 24-Apr-24 07:29 nucliadb/ingest/consumer/metrics.py
+-rw-r--r--  2.0 unx     9543 b- defN 24-Apr-24 07:29 nucliadb/ingest/consumer/pull.py
+-rw-r--r--  2.0 unx     6935 b- defN 24-Apr-24 07:29 nucliadb/ingest/consumer/service.py
+-rw-r--r--  2.0 unx     4331 b- defN 24-Apr-24 07:29 nucliadb/ingest/consumer/shard_creator.py
+-rw-r--r--  2.0 unx     2656 b- defN 24-Apr-24 07:29 nucliadb/ingest/consumer/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-24 07:29 nucliadb/ingest/fields/__init__.py
+-rw-r--r--  2.0 unx    18433 b- defN 24-Apr-24 07:29 nucliadb/ingest/fields/base.py
+-rw-r--r--  2.0 unx     6516 b- defN 24-Apr-24 07:29 nucliadb/ingest/fields/conversation.py
+-rw-r--r--  2.0 unx     1223 b- defN 24-Apr-24 07:29 nucliadb/ingest/fields/date.py
+-rw-r--r--  2.0 unx     1205 b- defN 24-Apr-24 07:29 nucliadb/ingest/fields/exceptions.py
+-rw-r--r--  2.0 unx     5159 b- defN 24-Apr-24 07:29 nucliadb/ingest/fields/file.py
+-rw-r--r--  2.0 unx     1547 b- defN 24-Apr-24 07:29 nucliadb/ingest/fields/generic.py
+-rw-r--r--  2.0 unx     1235 b- defN 24-Apr-24 07:29 nucliadb/ingest/fields/keywordset.py
+-rw-r--r--  2.0 unx     2250 b- defN 24-Apr-24 07:29 nucliadb/ingest/fields/layout.py
+-rw-r--r--  2.0 unx     4084 b- defN 24-Apr-24 07:29 nucliadb/ingest/fields/link.py
+-rw-r--r--  2.0 unx     1319 b- defN 24-Apr-24 07:29 nucliadb/ingest/fields/text.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-24 07:29 nucliadb/ingest/orm/__init__.py
+-rw-r--r--  2.0 unx    28367 b- defN 24-Apr-24 07:29 nucliadb/ingest/orm/brain.py
+-rw-r--r--  2.0 unx    15758 b- defN 24-Apr-24 07:29 nucliadb/ingest/orm/entities.py
+-rw-r--r--  2.0 unx     1279 b- defN 24-Apr-24 07:29 nucliadb/ingest/orm/exceptions.py
+-rw-r--r--  2.0 unx    18731 b- defN 24-Apr-24 07:29 nucliadb/ingest/orm/knowledgebox.py
+-rw-r--r--  2.0 unx     1096 b- defN 24-Apr-24 07:29 nucliadb/ingest/orm/metrics.py
+-rw-r--r--  2.0 unx    60647 b- defN 24-Apr-24 07:29 nucliadb/ingest/orm/resource.py
+-rw-r--r--  2.0 unx     1739 b- defN 24-Apr-24 07:29 nucliadb/ingest/orm/synonyms.py
+-rw-r--r--  2.0 unx     3683 b- defN 24-Apr-24 07:29 nucliadb/ingest/orm/utils.py
+-rw-r--r--  2.0 unx    26460 b- defN 24-Apr-24 07:29 nucliadb/ingest/orm/processor/__init__.py
+-rw-r--r--  2.0 unx     1690 b- defN 24-Apr-24 07:29 nucliadb/ingest/orm/processor/sequence_manager.py
+-rw-r--r--  2.0 unx     2057 b- defN 24-Apr-24 07:29 nucliadb/ingest/service/__init__.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-24 07:29 nucliadb/ingest/service/exceptions.py
+-rw-r--r--  2.0 unx    37355 b- defN 24-Apr-24 07:29 nucliadb/ingest/service/writer.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-24 07:29 nucliadb/ingest/tests/__init__.py
+-rw-r--r--  2.0 unx     1157 b- defN 24-Apr-24 07:29 nucliadb/ingest/tests/conftest.py
+-rw-r--r--  2.0 unx    24068 b- defN 24-Apr-24 07:29 nucliadb/ingest/tests/fixtures.py
+-rw-r--r--  2.0 unx    62843 b- defN 24-Apr-24 07:29 nucliadb/ingest/tests/vectors.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-24 07:29 nucliadb/ingest/tests/integration/__init__.py
+-rw-r--r--  2.0 unx      833 b- defN 24-Apr-24 07:29 nucliadb/ingest/tests/integration/consumer/__init__.py
+-rw-r--r--  2.0 unx     2549 b- defN 24-Apr-24 07:29 nucliadb/ingest/tests/integration/consumer/test_auditing.py
+-rw-r--r--  2.0 unx     2591 b- defN 24-Apr-24 07:29 nucliadb/ingest/tests/integration/consumer/test_materializer.py
+-rw-r--r--  2.0 unx     4465 b- defN 24-Apr-24 07:29 nucliadb/ingest/tests/integration/consumer/test_pull.py
+-rw-r--r--  2.0 unx     2763 b- defN 24-Apr-24 07:29 nucliadb/ingest/tests/integration/consumer/test_service.py
+-rw-r--r--  2.0 unx     2019 b- defN 24-Apr-24 07:29 nucliadb/ingest/tests/integration/consumer/test_shard_creator.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-24 07:29 nucliadb/ingest/tests/integration/ingest/__init__.py
+-rw-r--r--  2.0 unx    27334 b- defN 24-Apr-24 07:29 nucliadb/ingest/tests/integration/ingest/test_ingest.py
+-rw-r--r--  2.0 unx     3040 b- defN 24-Apr-24 07:29 nucliadb/ingest/tests/integration/ingest/test_processing_engine.py
+-rw-r--r--  2.0 unx     8586 b- defN 24-Apr-24 07:29 nucliadb/ingest/tests/integration/ingest/test_relations.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-24 07:29 nucliadb/ingest/tests/unit/__init__.py
+-rw-r--r--  2.0 unx     1189 b- defN 24-Apr-24 07:29 nucliadb/ingest/tests/unit/test_cache.py
+-rw-r--r--  2.0 unx     1432 b- defN 24-Apr-24 07:29 nucliadb/ingest/tests/unit/test_partitions.py
+-rw-r--r--  2.0 unx     5807 b- defN 24-Apr-24 07:29 nucliadb/ingest/tests/unit/test_processing.py
+-rw-r--r--  2.0 unx      978 b- defN 24-Apr-24 07:29 nucliadb/ingest/tests/unit/test_settings.py
+-rw-r--r--  2.0 unx      833 b- defN 24-Apr-24 07:29 nucliadb/ingest/tests/unit/consumer/__init__.py
+-rw-r--r--  2.0 unx     3981 b- defN 24-Apr-24 07:29 nucliadb/ingest/tests/unit/consumer/test_auditing.py
+-rw-r--r--  2.0 unx     2472 b- defN 24-Apr-24 07:29 nucliadb/ingest/tests/unit/consumer/test_consumer.py
+-rw-r--r--  2.0 unx     2063 b- defN 24-Apr-24 07:29 nucliadb/ingest/tests/unit/consumer/test_pull.py
+-rw-r--r--  2.0 unx     4075 b- defN 24-Apr-24 07:29 nucliadb/ingest/tests/unit/consumer/test_shard_creator.py
+-rw-r--r--  2.0 unx     1934 b- defN 24-Apr-24 07:29 nucliadb/ingest/tests/unit/consumer/test_utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-24 07:29 nucliadb/ingest/tests/unit/orm/__init__.py
+-rw-r--r--  2.0 unx     9876 b- defN 24-Apr-24 07:29 nucliadb/ingest/tests/unit/orm/test_brain.py
+-rw-r--r--  2.0 unx     2435 b- defN 24-Apr-24 07:29 nucliadb/ingest/tests/unit/orm/test_brain_vectors.py
+-rw-r--r--  2.0 unx     1174 b- defN 24-Apr-24 07:29 nucliadb/ingest/tests/unit/orm/test_orm_utils.py
+-rw-r--r--  2.0 unx     4045 b- defN 24-Apr-24 07:29 nucliadb/ingest/tests/unit/orm/test_processor.py
+-rw-r--r--  2.0 unx    11005 b- defN 24-Apr-24 07:29 nucliadb/ingest/tests/unit/orm/test_resource.py
+-rw-r--r--  2.0 unx     2216 b- defN 24-Apr-24 07:29 nucliadb/middleware/__init__.py
+-rw-r--r--  2.0 unx     3912 b- defN 24-Apr-24 07:29 nucliadb/middleware/transaction.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-24 07:29 nucliadb/migrator/__init__.py
+-rw-r--r--  2.0 unx     2119 b- defN 24-Apr-24 07:29 nucliadb/migrator/command.py
+-rw-r--r--  2.0 unx     1334 b- defN 24-Apr-24 07:29 nucliadb/migrator/context.py
+-rw-r--r--  2.0 unx     5104 b- defN 24-Apr-24 07:29 nucliadb/migrator/datamanager.py
+-rw-r--r--  2.0 unx      889 b- defN 24-Apr-24 07:29 nucliadb/migrator/exceptions.py
+-rw-r--r--  2.0 unx     9237 b- defN 24-Apr-24 07:29 nucliadb/migrator/migrator.py
+-rw-r--r--  2.0 unx     1145 b- defN 24-Apr-24 07:29 nucliadb/migrator/models.py
+-rw-r--r--  2.0 unx     1110 b- defN 24-Apr-24 07:29 nucliadb/migrator/settings.py
+-rw-r--r--  2.0 unx     2346 b- defN 24-Apr-24 07:29 nucliadb/migrator/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-24 07:29 nucliadb/models/__init__.py
+-rw-r--r--  2.0 unx     1599 b- defN 24-Apr-24 07:29 nucliadb/models/responses.py
+-rw-r--r--  2.0 unx     6041 b- defN 24-Apr-24 07:29 nucliadb/purge/__init__.py
+-rw-r--r--  2.0 unx     9364 b- defN 24-Apr-24 07:29 nucliadb/purge/orphan_shards.py
+-rw-r--r--  2.0 unx     1328 b- defN 24-Apr-24 07:29 nucliadb/reader/__init__.py
+-rw-r--r--  2.0 unx     3709 b- defN 24-Apr-24 07:29 nucliadb/reader/app.py
+-rw-r--r--  2.0 unx     1366 b- defN 24-Apr-24 07:29 nucliadb/reader/lifecycle.py
+-rw-r--r--  2.0 unx     1031 b- defN 24-Apr-24 07:29 nucliadb/reader/openapi.py
+-rw-r--r--  2.0 unx     1447 b- defN 24-Apr-24 07:29 nucliadb/reader/run.py
+-rw-r--r--  2.0 unx      872 b- defN 24-Apr-24 07:29 nucliadb/reader/api/__init__.py
+-rw-r--r--  2.0 unx     2434 b- defN 24-Apr-24 07:29 nucliadb/reader/api/models.py
+-rw-r--r--  2.0 unx     1110 b- defN 24-Apr-24 07:29 nucliadb/reader/api/v1/__init__.py
+-rw-r--r--  2.0 unx    12368 b- defN 24-Apr-24 07:29 nucliadb/reader/api/v1/download.py
+-rw-r--r--  2.0 unx     6450 b- defN 24-Apr-24 07:29 nucliadb/reader/api/v1/export_import.py
+-rw-r--r--  2.0 unx     3632 b- defN 24-Apr-24 07:29 nucliadb/reader/api/v1/knowledgebox.py
+-rw-r--r--  2.0 unx     2093 b- defN 24-Apr-24 07:29 nucliadb/reader/api/v1/learning_collector.py
+-rw-r--r--  2.0 unx     4454 b- defN 24-Apr-24 07:29 nucliadb/reader/api/v1/learning_config.py
+-rw-r--r--  2.0 unx    13928 b- defN 24-Apr-24 07:29 nucliadb/reader/api/v1/resource.py
+-rw-r--r--  2.0 unx     1011 b- defN 24-Apr-24 07:29 nucliadb/reader/api/v1/router.py
+-rw-r--r--  2.0 unx    13882 b- defN 24-Apr-24 07:29 nucliadb/reader/api/v1/services.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-24 07:29 nucliadb/reader/reader/__init__.py
+-rw-r--r--  2.0 unx     8155 b- defN 24-Apr-24 07:29 nucliadb/reader/reader/notifications.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-24 07:29 nucliadb/reader/tests/__init__.py
+-rw-r--r--  2.0 unx     1224 b- defN 24-Apr-24 07:29 nucliadb/reader/tests/conftest.py
+-rw-r--r--  2.0 unx     4345 b- defN 24-Apr-24 07:29 nucliadb/reader/tests/fixtures.py
+-rw-r--r--  2.0 unx     2748 b- defN 24-Apr-24 07:29 nucliadb/reader/tests/test_list_resources.py
+-rw-r--r--  2.0 unx    10199 b- defN 24-Apr-24 07:29 nucliadb/reader/tests/test_reader_file_download.py
+-rw-r--r--  2.0 unx    10586 b- defN 24-Apr-24 07:29 nucliadb/reader/tests/test_reader_resource.py
+-rw-r--r--  2.0 unx     6535 b- defN 24-Apr-24 07:29 nucliadb/reader/tests/test_reader_resource_field.py
+-rw-r--r--  2.0 unx     1535 b- defN 24-Apr-24 07:29 nucliadb/search/__init__.py
+-rw-r--r--  2.0 unx     4905 b- defN 24-Apr-24 07:29 nucliadb/search/app.py
+-rw-r--r--  2.0 unx     1956 b- defN 24-Apr-24 07:29 nucliadb/search/lifecycle.py
+-rw-r--r--  2.0 unx     1016 b- defN 24-Apr-24 07:29 nucliadb/search/openapi.py
+-rw-r--r--  2.0 unx    18535 b- defN 24-Apr-24 07:29 nucliadb/search/predict.py
+-rw-r--r--  2.0 unx     1402 b- defN 24-Apr-24 07:29 nucliadb/search/run.py
+-rw-r--r--  2.0 unx     1193 b- defN 24-Apr-24 07:29 nucliadb/search/settings.py
+-rw-r--r--  2.0 unx     1037 b- defN 24-Apr-24 07:29 nucliadb/search/utilities.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-24 07:29 nucliadb/search/api/__init__.py
+-rw-r--r--  2.0 unx     1272 b- defN 24-Apr-24 07:29 nucliadb/search/api/v1/__init__.py
+-rw-r--r--  2.0 unx     9913 b- defN 24-Apr-24 07:29 nucliadb/search/api/v1/chat.py
+-rw-r--r--  2.0 unx     2665 b- defN 24-Apr-24 07:29 nucliadb/search/api/v1/feedback.py
+-rw-r--r--  2.0 unx     8804 b- defN 24-Apr-24 07:29 nucliadb/search/api/v1/find.py
+-rw-r--r--  2.0 unx     7026 b- defN 24-Apr-24 07:29 nucliadb/search/api/v1/knowledgebox.py
+-rw-r--r--  2.0 unx     3041 b- defN 24-Apr-24 07:29 nucliadb/search/api/v1/predict_proxy.py
+-rw-r--r--  2.0 unx      988 b- defN 24-Apr-24 07:29 nucliadb/search/api/v1/router.py
+-rw-r--r--  2.0 unx    18359 b- defN 24-Apr-24 07:29 nucliadb/search/api/v1/search.py
+-rw-r--r--  2.0 unx     5928 b- defN 24-Apr-24 07:29 nucliadb/search/api/v1/suggest.py
+-rw-r--r--  2.0 unx     2536 b- defN 24-Apr-24 07:29 nucliadb/search/api/v1/summarize.py
+-rw-r--r--  2.0 unx     1412 b- defN 24-Apr-24 07:29 nucliadb/search/api/v1/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-24 07:29 nucliadb/search/api/v1/resource/__init__.py
+-rw-r--r--  2.0 unx     6095 b- defN 24-Apr-24 07:29 nucliadb/search/api/v1/resource/ask.py
+-rw-r--r--  2.0 unx     5887 b- defN 24-Apr-24 07:29 nucliadb/search/api/v1/resource/chat.py
+-rw-r--r--  2.0 unx     5293 b- defN 24-Apr-24 07:29 nucliadb/search/api/v1/resource/search.py
+-rw-r--r--  2.0 unx      833 b- defN 24-Apr-24 07:29 nucliadb/search/requesters/__init__.py
+-rw-r--r--  2.0 unx     9070 b- defN 24-Apr-24 07:29 nucliadb/search/requesters/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-24 07:29 nucliadb/search/search/__init__.py
+-rw-r--r--  2.0 unx     2746 b- defN 24-Apr-24 07:29 nucliadb/search/search/cache.py
+-rw-r--r--  2.0 unx     1154 b- defN 24-Apr-24 07:29 nucliadb/search/search/exceptions.py
+-rw-r--r--  2.0 unx     5465 b- defN 24-Apr-24 07:29 nucliadb/search/search/fetch.py
+-rw-r--r--  2.0 unx     6513 b- defN 24-Apr-24 07:29 nucliadb/search/search/filters.py
+-rw-r--r--  2.0 unx     4646 b- defN 24-Apr-24 07:29 nucliadb/search/search/find.py
+-rw-r--r--  2.0 unx    17152 b- defN 24-Apr-24 07:29 nucliadb/search/search/find_merge.py
+-rw-r--r--  2.0 unx    21282 b- defN 24-Apr-24 07:29 nucliadb/search/search/merge.py
+-rw-r--r--  2.0 unx     1130 b- defN 24-Apr-24 07:29 nucliadb/search/search/metrics.py
+-rw-r--r--  2.0 unx     8698 b- defN 24-Apr-24 07:29 nucliadb/search/search/paragraphs.py
+-rw-r--r--  2.0 unx     3026 b- defN 24-Apr-24 07:29 nucliadb/search/search/predict_proxy.py
+-rw-r--r--  2.0 unx    31300 b- defN 24-Apr-24 07:29 nucliadb/search/search/query.py
+-rw-r--r--  2.0 unx     3149 b- defN 24-Apr-24 07:29 nucliadb/search/search/shards.py
+-rw-r--r--  2.0 unx     5101 b- defN 24-Apr-24 07:29 nucliadb/search/search/summarize.py
+-rw-r--r--  2.0 unx     2438 b- defN 24-Apr-24 07:29 nucliadb/search/search/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-24 07:29 nucliadb/search/search/chat/__init__.py
+-rw-r--r--  2.0 unx     2058 b- defN 24-Apr-24 07:29 nucliadb/search/search/chat/images.py
+-rw-r--r--  2.0 unx    20793 b- defN 24-Apr-24 07:29 nucliadb/search/search/chat/prompt.py
+-rw-r--r--  2.0 unx    15347 b- defN 24-Apr-24 07:29 nucliadb/search/search/chat/query.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-24 07:29 nucliadb/search/tests/__init__.py
+-rw-r--r--  2.0 unx     1295 b- defN 24-Apr-24 07:29 nucliadb/search/tests/conftest.py
+-rw-r--r--  2.0 unx     6578 b- defN 24-Apr-24 07:29 nucliadb/search/tests/fixtures.py
+-rw-r--r--  2.0 unx    15529 b- defN 24-Apr-24 07:29 nucliadb/search/tests/node.py
+-rw-r--r--  2.0 unx      833 b- defN 24-Apr-24 07:29 nucliadb/search/tests/unit/__init__.py
+-rw-r--r--  2.0 unx     2649 b- defN 24-Apr-24 07:29 nucliadb/search/tests/unit/test_app.py
+-rw-r--r--  2.0 unx     3374 b- defN 24-Apr-24 07:29 nucliadb/search/tests/unit/test_find_merge.py
+-rw-r--r--  2.0 unx     1400 b- defN 24-Apr-24 07:29 nucliadb/search/tests/unit/test_merge.py
+-rw-r--r--  2.0 unx    14729 b- defN 24-Apr-24 07:29 nucliadb/search/tests/unit/test_predict.py
+-rw-r--r--  2.0 unx     1317 b- defN 24-Apr-24 07:29 nucliadb/search/tests/unit/test_run.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-24 07:29 nucliadb/search/tests/unit/api/__init__.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-24 07:29 nucliadb/search/tests/unit/api/v1/__init__.py
+-rw-r--r--  2.0 unx     2966 b- defN 24-Apr-24 07:29 nucliadb/search/tests/unit/api/v1/test_chat.py
+-rw-r--r--  2.0 unx     2865 b- defN 24-Apr-24 07:29 nucliadb/search/tests/unit/api/v1/test_predict_proxy.py
+-rw-r--r--  2.0 unx     2901 b- defN 24-Apr-24 07:29 nucliadb/search/tests/unit/api/v1/test_summarize.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-24 07:29 nucliadb/search/tests/unit/api/v1/resource/__init__.py
+-rw-r--r--  2.0 unx     2411 b- defN 24-Apr-24 07:29 nucliadb/search/tests/unit/api/v1/resource/test_ask.py
+-rw-r--r--  2.0 unx     3040 b- defN 24-Apr-24 07:29 nucliadb/search/tests/unit/api/v1/resource/test_chat.py
+-rw-r--r--  2.0 unx      833 b- defN 24-Apr-24 07:29 nucliadb/search/tests/unit/search/__init__.py
+-rw-r--r--  2.0 unx     8567 b- defN 24-Apr-24 07:29 nucliadb/search/tests/unit/search/test_chat_prompt.py
+-rw-r--r--  2.0 unx     3736 b- defN 24-Apr-24 07:29 nucliadb/search/tests/unit/search/test_fetch.py
+-rw-r--r--  2.0 unx     4306 b- defN 24-Apr-24 07:29 nucliadb/search/tests/unit/search/test_filters.py
+-rw-r--r--  2.0 unx     4492 b- defN 24-Apr-24 07:29 nucliadb/search/tests/unit/search/test_paragraphs.py
+-rw-r--r--  2.0 unx     3496 b- defN 24-Apr-24 07:29 nucliadb/search/tests/unit/search/test_predict_proxy.py
+-rw-r--r--  2.0 unx     7001 b- defN 24-Apr-24 07:29 nucliadb/search/tests/unit/search/test_query.py
+-rw-r--r--  2.0 unx      833 b- defN 24-Apr-24 07:29 nucliadb/search/tests/unit/search/requesters/__init__.py
+-rw-r--r--  2.0 unx     6455 b- defN 24-Apr-24 07:29 nucliadb/search/tests/unit/search/requesters/test_utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-24 07:29 nucliadb/search/tests/unit/search/search/__init__.py
+-rw-r--r--  2.0 unx     1759 b- defN 24-Apr-24 07:29 nucliadb/search/tests/unit/search/search/test_shards.py
+-rw-r--r--  2.0 unx     2511 b- defN 24-Apr-24 07:29 nucliadb/search/tests/unit/search/search/test_utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-24 07:29 nucliadb/standalone/__init__.py
+-rw-r--r--  2.0 unx     6746 b- defN 24-Apr-24 07:29 nucliadb/standalone/api_router.py
+-rw-r--r--  2.0 unx     5763 b- defN 24-Apr-24 07:29 nucliadb/standalone/app.py
+-rw-r--r--  2.0 unx     7800 b- defN 24-Apr-24 07:29 nucliadb/standalone/auth.py
+-rw-r--r--  2.0 unx     5309 b- defN 24-Apr-24 07:29 nucliadb/standalone/config.py
+-rw-r--r--  2.0 unx     6930 b- defN 24-Apr-24 07:29 nucliadb/standalone/introspect.py
+-rw-r--r--  2.0 unx     2488 b- defN 24-Apr-24 07:29 nucliadb/standalone/lifecycle.py
+-rw-r--r--  2.0 unx     1317 b- defN 24-Apr-24 07:29 nucliadb/standalone/purge.py
+-rw-r--r--  2.0 unx     5336 b- defN 24-Apr-24 07:29 nucliadb/standalone/run.py
+-rw-r--r--  2.0 unx     5781 b- defN 24-Apr-24 07:29 nucliadb/standalone/settings.py
+-rw-r--r--  2.0 unx     3132 b- defN 24-Apr-24 07:29 nucliadb/standalone/versions.py
+-rw-r--r--  2.0 unx     2285 b- defN 24-Apr-24 07:29 nucliadb/standalone/static/favicon.ico
+-rw-r--r--  2.0 unx     3833 b- defN 24-Apr-24 07:29 nucliadb/standalone/static/index.html
+-rw-r--r--  2.0 unx     2639 b- defN 24-Apr-24 07:29 nucliadb/standalone/static/logo.svg
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-24 07:29 nucliadb/standalone/tests/__init__.py
+-rw-r--r--  2.0 unx     1294 b- defN 24-Apr-24 07:29 nucliadb/standalone/tests/conftest.py
+-rw-r--r--  2.0 unx     1319 b- defN 24-Apr-24 07:29 nucliadb/standalone/tests/fixtures.py
+-rw-r--r--  2.0 unx      833 b- defN 24-Apr-24 07:29 nucliadb/standalone/tests/unit/__init__.py
+-rw-r--r--  2.0 unx     1722 b- defN 24-Apr-24 07:29 nucliadb/standalone/tests/unit/test_api_router.py
+-rw-r--r--  2.0 unx     5509 b- defN 24-Apr-24 07:29 nucliadb/standalone/tests/unit/test_auth.py
+-rw-r--r--  2.0 unx     1334 b- defN 24-Apr-24 07:29 nucliadb/standalone/tests/unit/test_introspect.py
+-rw-r--r--  2.0 unx     1472 b- defN 24-Apr-24 07:29 nucliadb/standalone/tests/unit/test_run.py
+-rw-r--r--  2.0 unx     1972 b- defN 24-Apr-24 07:29 nucliadb/standalone/tests/unit/test_versions.py
+-rw-r--r--  2.0 unx     1037 b- defN 24-Apr-24 07:29 nucliadb/tasks/__init__.py
+-rw-r--r--  2.0 unx     7655 b- defN 24-Apr-24 07:29 nucliadb/tasks/consumer.py
+-rw-r--r--  2.0 unx      924 b- defN 24-Apr-24 07:29 nucliadb/tasks/logger.py
+-rw-r--r--  2.0 unx     1378 b- defN 24-Apr-24 07:29 nucliadb/tasks/models.py
+-rw-r--r--  2.0 unx     3457 b- defN 24-Apr-24 07:29 nucliadb/tasks/producer.py
+-rw-r--r--  2.0 unx     1753 b- defN 24-Apr-24 07:29 nucliadb/tasks/registry.py
+-rw-r--r--  2.0 unx     1360 b- defN 24-Apr-24 07:29 nucliadb/tasks/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-24 07:29 nucliadb/tests/__init__.py
+-rw-r--r--  2.0 unx     1229 b- defN 24-Apr-24 07:29 nucliadb/tests/conftest.py
+-rw-r--r--  2.0 unx    22365 b- defN 24-Apr-24 07:29 nucliadb/tests/fixtures.py
+-rw-r--r--  2.0 unx     7549 b- defN 24-Apr-24 07:29 nucliadb/tests/tikv.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-24 07:29 nucliadb/tests/benchmarks/__init__.py
+-rw-r--r--  2.0 unx     3032 b- defN 24-Apr-24 07:29 nucliadb/tests/benchmarks/test_search.py
+-rw-r--r--  2.0 unx      919 b- defN 24-Apr-24 07:29 nucliadb/tests/knowledgeboxes/__init__.py
+-rw-r--r--  2.0 unx     7002 b- defN 24-Apr-24 07:29 nucliadb/tests/knowledgeboxes/philosophy_books.py
+-rw-r--r--  2.0 unx     3037 b- defN 24-Apr-24 07:29 nucliadb/tests/knowledgeboxes/ten_dummy_resources.py
+-rw-r--r--  2.0 unx     1148 b- defN 24-Apr-24 07:29 nucliadb/tests/migrations/__init__.py
+-rw-r--r--  2.0 unx     2726 b- defN 24-Apr-24 07:29 nucliadb/tests/migrations/test_migration_0017.py
+-rw-r--r--  2.0 unx     3625 b- defN 24-Apr-24 07:29 nucliadb/tests/migrations/test_migration_0018.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-24 07:29 nucliadb/tests/unit/__init__.py
+-rw-r--r--  2.0 unx     1487 b- defN 24-Apr-24 07:29 nucliadb/tests/unit/test_field_ids.py
+-rw-r--r--  2.0 unx     2758 b- defN 24-Apr-24 07:29 nucliadb/tests/unit/test_health.py
+-rw-r--r--  2.0 unx     1543 b- defN 24-Apr-24 07:29 nucliadb/tests/unit/test_kb_slugs.py
+-rw-r--r--  2.0 unx     7892 b- defN 24-Apr-24 07:29 nucliadb/tests/unit/test_learning_proxy.py
+-rw-r--r--  2.0 unx     2642 b- defN 24-Apr-24 07:29 nucliadb/tests/unit/test_metrics_exporter.py
+-rw-r--r--  2.0 unx     1341 b- defN 24-Apr-24 07:29 nucliadb/tests/unit/test_openapi.py
+-rw-r--r--  2.0 unx     3656 b- defN 24-Apr-24 07:29 nucliadb/tests/unit/test_purge.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-24 07:29 nucliadb/tests/unit/common/__init__.py
+-rw-r--r--  2.0 unx     1268 b- defN 24-Apr-24 07:29 nucliadb/tests/unit/common/test_context.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-24 07:29 nucliadb/tests/unit/common/cluster/__init__.py
+-rw-r--r--  2.0 unx    11955 b- defN 24-Apr-24 07:29 nucliadb/tests/unit/common/cluster/test_cluster.py
+-rw-r--r--  2.0 unx     5387 b- defN 24-Apr-24 07:29 nucliadb/tests/unit/common/cluster/test_kb_shard_manager.py
+-rw-r--r--  2.0 unx     9470 b- defN 24-Apr-24 07:29 nucliadb/tests/unit/common/cluster/test_rollover.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-24 07:29 nucliadb/tests/unit/common/cluster/discovery/__init__.py
+-rw-r--r--  2.0 unx     5584 b- defN 24-Apr-24 07:29 nucliadb/tests/unit/common/cluster/discovery/test_k8s.py
+-rw-r--r--  2.0 unx      833 b- defN 24-Apr-24 07:29 nucliadb/tests/unit/common/cluster/standalone/__init__.py
+-rw-r--r--  2.0 unx     3750 b- defN 24-Apr-24 07:29 nucliadb/tests/unit/common/cluster/standalone/test_service.py
+-rw-r--r--  2.0 unx     2114 b- defN 24-Apr-24 07:29 nucliadb/tests/unit/common/cluster/standalone/test_utils.py
+-rw-r--r--  2.0 unx      833 b- defN 24-Apr-24 07:29 nucliadb/tests/unit/common/maindb/__init__.py
+-rw-r--r--  2.0 unx     3579 b- defN 24-Apr-24 07:29 nucliadb/tests/unit/common/maindb/test_driver.py
+-rw-r--r--  2.0 unx     1869 b- defN 24-Apr-24 07:29 nucliadb/tests/unit/common/maindb/test_tikv.py
+-rw-r--r--  2.0 unx     2998 b- defN 24-Apr-24 07:29 nucliadb/tests/unit/common/maindb/test_utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-24 07:29 nucliadb/tests/unit/export_import/__init__.py
+-rw-r--r--  2.0 unx     1435 b- defN 24-Apr-24 07:29 nucliadb/tests/unit/export_import/test_datamanager.py
+-rw-r--r--  2.0 unx     9706 b- defN 24-Apr-24 07:29 nucliadb/tests/unit/export_import/test_utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-24 07:29 nucliadb/tests/unit/migrator/__init__.py
+-rw-r--r--  2.0 unx     3233 b- defN 24-Apr-24 07:29 nucliadb/tests/unit/migrator/test_migrator.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-24 07:29 nucliadb/tests/unit/tasks/__init__.py
+-rw-r--r--  2.0 unx     1375 b- defN 24-Apr-24 07:29 nucliadb/tests/unit/tasks/conftest.py
+-rw-r--r--  2.0 unx     2714 b- defN 24-Apr-24 07:29 nucliadb/tests/unit/tasks/test_consumer.py
+-rw-r--r--  2.0 unx     3189 b- defN 24-Apr-24 07:29 nucliadb/tests/unit/tasks/test_producer.py
+-rw-r--r--  2.0 unx     1827 b- defN 24-Apr-24 07:29 nucliadb/tests/unit/tasks/test_tasks.py
+-rw-r--r--  2.0 unx     2507 b- defN 24-Apr-24 07:29 nucliadb/tests/utils/__init__.py
+-rw-r--r--  2.0 unx     1797 b- defN 24-Apr-24 07:29 nucliadb/tests/utils/aiohttp_session.py
+-rw-r--r--  2.0 unx     2533 b- defN 24-Apr-24 07:29 nucliadb/tests/utils/entities.py
+-rw-r--r--  2.0 unx     6327 b- defN 24-Apr-24 07:29 nucliadb/tests/utils/broker_messages/__init__.py
+-rw-r--r--  2.0 unx     7557 b- defN 24-Apr-24 07:29 nucliadb/tests/utils/broker_messages/fields.py
+-rw-r--r--  2.0 unx     1196 b- defN 24-Apr-24 07:29 nucliadb/tests/utils/broker_messages/helpers.py
+-rw-r--r--  2.0 unx     1325 b- defN 24-Apr-24 07:29 nucliadb/train/__init__.py
+-rw-r--r--  2.0 unx     3530 b- defN 24-Apr-24 07:29 nucliadb/train/app.py
+-rw-r--r--  2.0 unx     3800 b- defN 24-Apr-24 07:29 nucliadb/train/generator.py
+-rw-r--r--  2.0 unx     1698 b- defN 24-Apr-24 07:29 nucliadb/train/lifecycle.py
+-rw-r--r--  2.0 unx     1198 b- defN 24-Apr-24 07:29 nucliadb/train/models.py
+-rw-r--r--  2.0 unx     5706 b- defN 24-Apr-24 07:29 nucliadb/train/nodes.py
+-rw-r--r--  2.0 unx     1400 b- defN 24-Apr-24 07:29 nucliadb/train/run.py
+-rw-r--r--  2.0 unx     5926 b- defN 24-Apr-24 07:29 nucliadb/train/servicer.py
+-rw-r--r--  2.0 unx     1415 b- defN 24-Apr-24 07:29 nucliadb/train/settings.py
+-rw-r--r--  2.0 unx     1496 b- defN 24-Apr-24 07:29 nucliadb/train/types.py
+-rw-r--r--  2.0 unx     3265 b- defN 24-Apr-24 07:29 nucliadb/train/upload.py
+-rw-r--r--  2.0 unx     6420 b- defN 24-Apr-24 07:29 nucliadb/train/uploader.py
+-rw-r--r--  2.0 unx     3179 b- defN 24-Apr-24 07:29 nucliadb/train/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-24 07:29 nucliadb/train/api/__init__.py
+-rw-r--r--  2.0 unx     1479 b- defN 24-Apr-24 07:29 nucliadb/train/api/utils.py
+-rw-r--r--  2.0 unx      928 b- defN 24-Apr-24 07:29 nucliadb/train/api/v1/__init__.py
+-rw-r--r--  2.0 unx     2065 b- defN 24-Apr-24 07:29 nucliadb/train/api/v1/check.py
+-rw-r--r--  2.0 unx      910 b- defN 24-Apr-24 07:29 nucliadb/train/api/v1/router.py
+-rw-r--r--  2.0 unx     1905 b- defN 24-Apr-24 07:29 nucliadb/train/api/v1/shards.py
+-rw-r--r--  2.0 unx     2129 b- defN 24-Apr-24 07:29 nucliadb/train/api/v1/trainset.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-24 07:29 nucliadb/train/generators/__init__.py
+-rw-r--r--  2.0 unx     3723 b- defN 24-Apr-24 07:29 nucliadb/train/generators/field_classifier.py
+-rw-r--r--  2.0 unx     6712 b- defN 24-Apr-24 07:29 nucliadb/train/generators/image_classifier.py
+-rw-r--r--  2.0 unx     2789 b- defN 24-Apr-24 07:29 nucliadb/train/generators/paragraph_classifier.py
+-rw-r--r--  2.0 unx     3590 b- defN 24-Apr-24 07:29 nucliadb/train/generators/paragraph_streaming.py
+-rw-r--r--  2.0 unx     5372 b- defN 24-Apr-24 07:29 nucliadb/train/generators/question_answer_streaming.py
+-rw-r--r--  2.0 unx     5160 b- defN 24-Apr-24 07:29 nucliadb/train/generators/sentence_classifier.py
+-rw-r--r--  2.0 unx    10446 b- defN 24-Apr-24 07:29 nucliadb/train/generators/token_classifier.py
+-rw-r--r--  2.0 unx     3877 b- defN 24-Apr-24 07:29 nucliadb/train/generators/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-24 07:29 nucliadb/train/tests/__init__.py
+-rw-r--r--  2.0 unx     1125 b- defN 24-Apr-24 07:29 nucliadb/train/tests/conftest.py
+-rw-r--r--  2.0 unx    11053 b- defN 24-Apr-24 07:29 nucliadb/train/tests/fixtures.py
+-rw-r--r--  2.0 unx     4598 b- defN 24-Apr-24 07:29 nucliadb/train/tests/test_field_classification.py
+-rw-r--r--  2.0 unx     2729 b- defN 24-Apr-24 07:29 nucliadb/train/tests/test_get_entities.py
+-rw-r--r--  2.0 unx     1876 b- defN 24-Apr-24 07:29 nucliadb/train/tests/test_get_info.py
+-rw-r--r--  2.0 unx     1382 b- defN 24-Apr-24 07:29 nucliadb/train/tests/test_get_ontology.py
+-rw-r--r--  2.0 unx     2417 b- defN 24-Apr-24 07:29 nucliadb/train/tests/test_get_ontology_count.py
+-rw-r--r--  2.0 unx     7669 b- defN 24-Apr-24 07:29 nucliadb/train/tests/test_image_classification.py
+-rw-r--r--  2.0 unx     1416 b- defN 24-Apr-24 07:29 nucliadb/train/tests/test_list_fields.py
+-rw-r--r--  2.0 unx     2944 b- defN 24-Apr-24 07:29 nucliadb/train/tests/test_list_paragraphs.py
+-rw-r--r--  2.0 unx     1423 b- defN 24-Apr-24 07:29 nucliadb/train/tests/test_list_resources.py
+-rw-r--r--  2.0 unx     2947 b- defN 24-Apr-24 07:29 nucliadb/train/tests/test_list_sentences.py
+-rw-r--r--  2.0 unx     4645 b- defN 24-Apr-24 07:29 nucliadb/train/tests/test_paragraph_classification.py
+-rw-r--r--  2.0 unx     4320 b- defN 24-Apr-24 07:29 nucliadb/train/tests/test_paragraph_streaming.py
+-rw-r--r--  2.0 unx     8751 b- defN 24-Apr-24 07:29 nucliadb/train/tests/test_question_answer_streaming.py
+-rw-r--r--  2.0 unx     5051 b- defN 24-Apr-24 07:29 nucliadb/train/tests/test_sentence_classification.py
+-rw-r--r--  2.0 unx     5583 b- defN 24-Apr-24 07:29 nucliadb/train/tests/test_token_classification.py
+-rw-r--r--  2.0 unx     3324 b- defN 24-Apr-24 07:29 nucliadb/train/tests/utils.py
+-rw-r--r--  2.0 unx     1328 b- defN 24-Apr-24 07:29 nucliadb/writer/__init__.py
+-rw-r--r--  2.0 unx     4268 b- defN 24-Apr-24 07:29 nucliadb/writer/app.py
+-rw-r--r--  2.0 unx    19495 b- defN 24-Apr-24 07:29 nucliadb/writer/back_pressure.py
+-rw-r--r--  2.0 unx      972 b- defN 24-Apr-24 07:29 nucliadb/writer/exceptions.py
+-rw-r--r--  2.0 unx     1953 b- defN 24-Apr-24 07:29 nucliadb/writer/lifecycle.py
+-rw-r--r--  2.0 unx     1032 b- defN 24-Apr-24 07:29 nucliadb/writer/openapi.py
+-rw-r--r--  2.0 unx     1448 b- defN 24-Apr-24 07:29 nucliadb/writer/run.py
+-rw-r--r--  2.0 unx     3074 b- defN 24-Apr-24 07:29 nucliadb/writer/settings.py
+-rw-r--r--  2.0 unx     1036 b- defN 24-Apr-24 07:29 nucliadb/writer/utilities.py
+-rw-r--r--  2.0 unx     1948 b- defN 24-Apr-24 07:29 nucliadb/writer/vectors.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-24 07:29 nucliadb/writer/api/__init__.py
+-rw-r--r--  2.0 unx     1429 b- defN 24-Apr-24 07:29 nucliadb/writer/api/constants.py
+-rw-r--r--  2.0 unx     1095 b- defN 24-Apr-24 07:29 nucliadb/writer/api/v1/__init__.py
+-rw-r--r--  2.0 unx     6565 b- defN 24-Apr-24 07:29 nucliadb/writer/api/v1/export_import.py
+-rw-r--r--  2.0 unx    28578 b- defN 24-Apr-24 07:29 nucliadb/writer/api/v1/field.py
+-rw-r--r--  2.0 unx     5239 b- defN 24-Apr-24 07:29 nucliadb/writer/api/v1/knowledgebox.py
+-rw-r--r--  2.0 unx     2052 b- defN 24-Apr-24 07:29 nucliadb/writer/api/v1/learning_config.py
+-rw-r--r--  2.0 unx    19940 b- defN 24-Apr-24 07:29 nucliadb/writer/api/v1/resource.py
+-rw-r--r--  2.0 unx     1034 b- defN 24-Apr-24 07:29 nucliadb/writer/api/v1/router.py
+-rw-r--r--  2.0 unx    12733 b- defN 24-Apr-24 07:29 nucliadb/writer/api/v1/services.py
+-rw-r--r--  2.0 unx    31592 b- defN 24-Apr-24 07:29 nucliadb/writer/api/v1/upload.py
+-rw-r--r--  2.0 unx     1612 b- defN 24-Apr-24 07:29 nucliadb/writer/layouts/__init__.py
+-rw-r--r--  2.0 unx     2115 b- defN 24-Apr-24 07:29 nucliadb/writer/layouts/v1.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-24 07:29 nucliadb/writer/resource/__init__.py
+-rw-r--r--  2.0 unx     1425 b- defN 24-Apr-24 07:29 nucliadb/writer/resource/audit.py
+-rw-r--r--  2.0 unx    10968 b- defN 24-Apr-24 07:29 nucliadb/writer/resource/basic.py
+-rw-r--r--  2.0 unx    16319 b- defN 24-Apr-24 07:29 nucliadb/writer/resource/field.py
+-rw-r--r--  2.0 unx     2022 b- defN 24-Apr-24 07:29 nucliadb/writer/resource/origin.py
+-rw-r--r--  2.0 unx     1152 b- defN 24-Apr-24 07:29 nucliadb/writer/resource/slug.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-24 07:29 nucliadb/writer/tests/__init__.py
+-rw-r--r--  2.0 unx     1200 b- defN 24-Apr-24 07:29 nucliadb/writer/tests/conftest.py
+-rw-r--r--  2.0 unx     5971 b- defN 24-Apr-24 07:29 nucliadb/writer/tests/fixtures.py
+-rw-r--r--  2.0 unx    15472 b- defN 24-Apr-24 07:29 nucliadb/writer/tests/test_fields.py
+-rw-r--r--  2.0 unx    25913 b- defN 24-Apr-24 07:29 nucliadb/writer/tests/test_files.py
+-rw-r--r--  2.0 unx     1729 b- defN 24-Apr-24 07:29 nucliadb/writer/tests/test_knowledgebox.py
+-rw-r--r--  2.0 unx     4569 b- defN 24-Apr-24 07:29 nucliadb/writer/tests/test_reprocess_file_field.py
+-rw-r--r--  2.0 unx    17449 b- defN 24-Apr-24 07:29 nucliadb/writer/tests/test_resources.py
+-rw-r--r--  2.0 unx     5120 b- defN 24-Apr-24 07:29 nucliadb/writer/tests/test_service.py
+-rw-r--r--  2.0 unx     6054 b- defN 24-Apr-24 07:29 nucliadb/writer/tests/test_tus.py
+-rw-r--r--  2.0 unx     1287 b- defN 24-Apr-24 07:29 nucliadb/writer/tests/utils.py
+-rw-r--r--  2.0 unx     5226 b- defN 24-Apr-24 07:29 nucliadb/writer/tus/__init__.py
+-rw-r--r--  2.0 unx     5082 b- defN 24-Apr-24 07:29 nucliadb/writer/tus/dm.py
+-rw-r--r--  2.0 unx     2186 b- defN 24-Apr-24 07:29 nucliadb/writer/tus/exceptions.py
+-rw-r--r--  2.0 unx    14527 b- defN 24-Apr-24 07:29 nucliadb/writer/tus/gcs.py
+-rw-r--r--  2.0 unx     5849 b- defN 24-Apr-24 07:29 nucliadb/writer/tus/local.py
+-rw-r--r--  2.0 unx     4367 b- defN 24-Apr-24 07:29 nucliadb/writer/tus/pg.py
+-rw-r--r--  2.0 unx     9069 b- defN 24-Apr-24 07:29 nucliadb/writer/tus/s3.py
+-rw-r--r--  2.0 unx     4734 b- defN 24-Apr-24 07:29 nucliadb/writer/tus/storage.py
+-rw-r--r--  2.0 unx     2556 b- defN 24-Apr-24 07:29 nucliadb/writer/tus/utils.py
+-rw-r--r--  2.0 unx     4343 b- defN 24-Apr-24 07:30 nucliadb-3.0.3.post450.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-24 07:30 nucliadb-3.0.3.post450.dist-info/WHEEL
+-rw-r--r--  2.0 unx     1268 b- defN 24-Apr-24 07:30 nucliadb-3.0.3.post450.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       20 b- defN 24-Apr-24 07:30 nucliadb-3.0.3.post450.dist-info/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 24-Apr-24 07:30 nucliadb-3.0.3.post450.dist-info/zip-safe
+-rw-rw-r--  2.0 unx    42761 b- defN 24-Apr-24 07:30 nucliadb-3.0.3.post450.dist-info/RECORD
+456 files, 2242380 bytes uncompressed, 686046 bytes compressed:  69.4%
```

## zipnote {}

```diff
@@ -1344,26 +1344,26 @@
 
 Filename: nucliadb/writer/tus/storage.py
 Comment: 
 
 Filename: nucliadb/writer/tus/utils.py
 Comment: 
 
-Filename: nucliadb-3.0.3.post447.dist-info/METADATA
+Filename: nucliadb-3.0.3.post450.dist-info/METADATA
 Comment: 
 
-Filename: nucliadb-3.0.3.post447.dist-info/WHEEL
+Filename: nucliadb-3.0.3.post450.dist-info/WHEEL
 Comment: 
 
-Filename: nucliadb-3.0.3.post447.dist-info/entry_points.txt
+Filename: nucliadb-3.0.3.post450.dist-info/entry_points.txt
 Comment: 
 
-Filename: nucliadb-3.0.3.post447.dist-info/top_level.txt
+Filename: nucliadb-3.0.3.post450.dist-info/top_level.txt
 Comment: 
 
-Filename: nucliadb-3.0.3.post447.dist-info/zip-safe
+Filename: nucliadb-3.0.3.post450.dist-info/zip-safe
 Comment: 
 
-Filename: nucliadb-3.0.3.post447.dist-info/RECORD
+Filename: nucliadb-3.0.3.post450.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## nucliadb/search/predict.py

```diff
@@ -55,18 +55,14 @@
 
 class ProxiedPredictAPIError(Exception):
     def __init__(self, status: int, detail: str = ""):
         self.status = status
         self.detail = detail
 
 
-class PredictVectorMissing(Exception):
-    pass
-
-
 class NUAKeyMissingError(Exception):
     pass
 
 
 class RephraseError(Exception):
     pass
 
@@ -103,15 +99,14 @@
 
 predict_observer = metrics.Observer(
     "predict_engine",
     labels={"type": ""},
     error_mappings={
         "over_limits": LimitsExceededError,
         "predict_api_error": SendToPredictError,
-        "empty_vectors": PredictVectorMissing,
     },
 )
 
 
 RETRIABLE_EXCEPTIONS = (aiohttp.client_exceptions.ClientConnectorError,)
 MAX_TRIES = 2
 
@@ -363,36 +358,14 @@
             params=params,
             headers=self.get_predict_headers(kbid),
         )
         await self.check_response(resp, expected_status=200)
         data = await resp.json()
         return QueryInfo(**data)
 
-    @predict_observer.wrap({"type": "sentence"})
-    async def convert_sentence_to_vector(self, kbid: str, sentence: str) -> list[float]:
-        try:
-            self.check_nua_key_is_configured_for_onprem()
-        except NUAKeyMissingError:
-            logger.warning(
-                "Nuclia Service account is not defined so could not retrieve vectors for the query"
-            )
-            return []
-
-        resp = await self.make_request(
-            "GET",
-            url=self.get_predict_url(SENTENCE, kbid),
-            params={"text": sentence},
-            headers=self.get_predict_headers(kbid),
-        )
-        await self.check_response(resp, expected_status=200)
-        data = await resp.json()
-        if len(data["data"]) == 0:
-            raise PredictVectorMissing()
-        return data["data"]
-
     @predict_observer.wrap({"type": "entities"})
     async def detect_entities(self, kbid: str, sentence: str) -> list[RelationNode]:
         try:
             self.check_nua_key_is_configured_for_onprem()
         except NUAKeyMissingError:
             logger.warning(
                 "Nuclia Service account is not defined so could not retrieve entities from the query"
@@ -524,23 +497,14 @@
                 entities=TokenSearch(
                     tokens=[Ner(text="text", ner="PERSON", start=0, end=2)], time=0.0
                 ),
                 sentence=SentenceSearch(data=Q, time=0.0),
                 query=sentence,
             )
 
-    async def convert_sentence_to_vector(self, kbid: str, sentence: str) -> list[float]:
-        self.calls.append(("convert_sentence_to_vector", sentence))
-        if (
-            os.environ.get("TEST_SENTENCE_ENCODER") == "multilingual-2023-02-21"
-        ):  # pragma: no cover
-            return Qm2023
-        else:
-            return Q
-
     async def detect_entities(self, kbid: str, sentence: str) -> list[RelationNode]:
         self.calls.append(("detect_entities", sentence))
         dummy_data = os.environ.get("TEST_RELATIONS", None)
         if dummy_data is not None:  # pragma: no cover
             return convert_relations(json.loads(dummy_data))
         else:
             return DUMMY_RELATION_NODE
```

## nucliadb/search/search/query.py

```diff
@@ -25,19 +25,15 @@
 from async_lru import alru_cache
 from nucliadb_protos.noderesources_pb2 import Resource
 
 from nucliadb.common import datamanagers
 from nucliadb.ingest.orm.synonyms import Synonyms
 from nucliadb.middleware.transaction import get_read_only_transaction
 from nucliadb.search import logger
-from nucliadb.search.predict import (
-    PredictVectorMissing,
-    SendToPredictError,
-    convert_relations,
-)
+from nucliadb.search.predict import SendToPredictError, convert_relations
 from nucliadb.search.search.filters import (
     convert_to_node_filters,
     flat_filter_labels,
     has_classification_label_filters,
     split_labels_by_type,
     translate_label,
     translate_label_filters,
@@ -51,27 +47,23 @@
 from nucliadb_models.metadata import ResourceProcessingStatus
 from nucliadb_models.search import (
     Filter,
     MaxTokens,
     MinScore,
     QueryInfo,
     SearchOptions,
-    SentenceSearch,
     SortField,
     SortFieldMap,
     SortOptions,
     SortOrder,
     SortOrderMap,
     SuggestOptions,
-    TokenSearch,
 )
 from nucliadb_models.security import RequestSecurity
 from nucliadb_protos import knowledgebox_pb2, nodereader_pb2, utils_pb2
-from nucliadb_utils import const
-from nucliadb_utils.utilities import has_feature
 
 from .exceptions import InvalidQueryError
 
 INDEX_SORTABLE_FIELDS = [
     SortField.CREATED,
     SortField.MODIFIED,
 ]
@@ -85,20 +77,20 @@
     This class is an encapsulation of the different phases of the query and allow
     some stateful interaction with a query and different depenedencies during
     query parsing.
     """
 
     _min_score_task: Optional[asyncio.Task] = None
     _query_information_task: Optional[asyncio.Task] = None
-    _convert_vectors_task: Optional[asyncio.Task] = None
     _detected_entities_task: Optional[asyncio.Task] = None
     _entities_meta_cache_task: Optional[asyncio.Task] = None
     _deleted_entities_groups_task: Optional[asyncio.Task] = None
     _synonyms_task: Optional[asyncio.Task] = None
     _get_classification_labels_task: Optional[asyncio.Task] = None
+    _get_matryoshka_dimension_task: Optional[asyncio.Task] = None
 
     def __init__(
         self,
         *,
         kbid: str,
         features: list[SearchOptions],
         query: str,
@@ -146,59 +138,43 @@
         self.with_status = with_status
         self.with_synonyms = with_synonyms
         self.autofilter = autofilter
         self.key_filters = key_filters
         self.security = security
         self.generative_model = generative_model
         self.rephrase = rephrase
-        self.query_endpoint_enabled = has_feature(
-            const.Features.PREDICT_QUERY_ENDPOINT,
-            default=False,
-            context={"kbid": self.kbid},
-        )
+        self.query_endpoint_used = False
         if len(self.filters) > 0:
             self.filters = translate_label_filters(self.filters)
             self.flat_filter_labels = flat_filter_labels(self.filters)
         self.max_tokens = max_tokens
 
     def _get_default_semantic_min_score(self) -> Awaitable[float]:
         if self._min_score_task is None:  # pragma: no cover
             self._min_score_task = asyncio.create_task(
                 get_default_semantic_min_score(self.kbid)
             )
         return self._min_score_task
 
-    def _get_converted_vectors(self) -> Awaitable[list[float]]:
-        if self._convert_vectors_task is None:  # pragma: no cover
-            self._convert_vectors_task = asyncio.create_task(
-                convert_vectors(self.kbid, self.query)
-            )
-        return self._convert_vectors_task
-
     def _get_query_information(self) -> Awaitable[QueryInfo]:
-        if self.query_endpoint_enabled is False:
-            # XXX Can be removed once query endpoint is fully enabled
-            async def static_query():
-                return QueryInfo(
-                    visual_llm=False,
-                    max_context=300_000,
-                    entities=TokenSearch(tokens=[], time=0.0),
-                    sentence=SentenceSearch(data=[], time=0.0),
-                    query=self.query,
-                )
-
-            return static_query()
         if self._query_information_task is None:  # pragma: no cover
             self._query_information_task = asyncio.create_task(
                 query_information(
                     self.kbid, self.query, self.generative_model, self.rephrase
                 )
             )
         return self._query_information_task
 
+    def _get_matryoshka_dimension(self) -> Awaitable[Optional[int]]:
+        if self._get_matryoshka_dimension_task is None:
+            self._get_matryoshka_dimension_task = asyncio.create_task(
+                get_matryoshka_dimension_cached(self.kbid)
+            )
+        return self._get_matryoshka_dimension_task
+
     def _get_detected_entities(self) -> Awaitable[list[utils_pb2.RelationNode]]:
         if self._detected_entities_task is None:  # pragma: no cover
             self._detected_entities_task = asyncio.create_task(
                 detect_entities(self.kbid, self.query)
             )
         return self._detected_entities_task
 
@@ -239,28 +215,23 @@
             self.flat_filter_labels
         ):
             asyncio.ensure_future(self._get_classification_labels())
         if self.min_score.semantic is None:
             asyncio.ensure_future(self._get_default_semantic_min_score())
 
         if SearchOptions.VECTOR in self.features and self.user_vector is None:
-            if self.query_endpoint_enabled:
-                asyncio.ensure_future(self._get_query_information())
-            else:
-                asyncio.ensure_future(self._get_converted_vectors())
+            self.query_endpoint_used = True
+            asyncio.ensure_future(self._get_query_information())
+            asyncio.ensure_future(self._get_matryoshka_dimension())
 
         if (SearchOptions.RELATIONS in self.features or self.autofilter) and len(
             self.query
         ) > 0:
-            if (
-                not self.query_endpoint_enabled
-                or SearchOptions.VECTOR not in self.features
-                or self.user_vector is not None
-            ):
-                self.query_endpoint_enabled = False
+            if not self.query_endpoint_used:
+                # If we only need to detect entities, we don't need the query endpoint
                 asyncio.ensure_future(self._get_detected_entities())
             asyncio.ensure_future(self._get_entities_meta_cache())
             asyncio.ensure_future(self._get_deleted_entity_groups())
         if self.with_synonyms and self.query:
             asyncio.ensure_future(self._get_synomyns())
 
     async def parse(self) -> tuple[nodereader_pb2.SearchRequest, bool, list[str]]:
@@ -403,64 +374,42 @@
         incomplete = False
         if self.vectorset is not None:
             request.vectorset = self.vectorset
             node_features.inc({"type": "vectorset"})
 
         query_vector = None
         if self.user_vector is None:
-            if self.query_endpoint_enabled:
-                try:
-                    query_info = await self._get_query_information()
-                except SendToPredictError as err:
-                    logger.warning(
-                        f"Errors on predict api trying to embedd query: {err}"
-                    )
-                    incomplete = True
-                except PredictVectorMissing:
-                    logger.warning("Predict api returned an empty vector")
-                    incomplete = True
-                else:
-                    if query_info and query_info.sentence:
-                        query_vector = query_info.sentence.data
-                    else:
-                        incomplete = True
+            try:
+                query_info = await self._get_query_information()
+            except SendToPredictError as err:
+                logger.warning(f"Errors on predict api trying to embedd query: {err}")
+                incomplete = True
             else:
-                try:
-                    query_vector = await self._get_converted_vectors()
-                except SendToPredictError as err:
-                    logger.warning(
-                        f"Errors on predict api trying to embedd query: {err}"
-                    )
-                    incomplete = True
-                except PredictVectorMissing:
-                    logger.warning("Predict api returned an empty vector")
+                if query_info and query_info.sentence:
+                    query_vector = query_info.sentence.data
+                else:
                     incomplete = True
         else:
             query_vector = self.user_vector
-
         if query_vector is not None:
-            async with datamanagers.with_transaction(read_only=True) as txn:
-                dimension = await datamanagers.kb.get_matryoshka_vector_dimension(
-                    txn, kbid=self.kbid
-                )
-            if dimension is not None:
+            matryoshka_dimension = await self._get_matryoshka_dimension()
+            if matryoshka_dimension is not None:
                 # KB using a matryoshka embeddings model, cut the query vector
                 # accordingly
-                query_vector = query_vector[:dimension]
+                query_vector = query_vector[:matryoshka_dimension]
             request.vector.extend(query_vector)
-
         return incomplete
 
     async def parse_relation_search(
         self, request: nodereader_pb2.SearchRequest
     ) -> list[str]:
         autofilters = []
         relations_search = SearchOptions.RELATIONS in self.features
         if relations_search or self.autofilter:
-            if not self.query_endpoint_enabled:
+            if not self.query_endpoint_used:
                 detected_entities = await self._get_detected_entities()
             else:
                 query_info_result = await self._get_query_information()
                 if query_info_result.entities:
                     detected_entities = convert_relations(
                         query_info_result.entities.dict()
                     )
@@ -600,20 +549,14 @@
             request.order.field = sort
             request.order.type = sort_ord  # type: ignore
         request.fields.extend(fields)
 
     return request
 
 
-@query_parse_dependency_observer.wrap({"type": "convert_vectors"})
-async def convert_vectors(kbid: str, query: str) -> list[float]:
-    predict = get_predict()
-    return await predict.convert_sentence_to_vector(kbid, query)
-
-
 @query_parse_dependency_observer.wrap({"type": "query_information"})
 async def query_information(
     kbid: str,
     query: str,
     generative_model: Optional[str] = None,
     rephrase: bool = False,
 ) -> QueryInfo:
@@ -814,7 +757,19 @@
     for term in filters["and"]:
         # Nested expressions are not allowed with paragraph labels
         if "literal" not in term:
             raise InvalidQueryError(
                 "filters",
                 "Paragraph labels can only be used with 'all' filter",
             )
+
+
+@alru_cache(maxsize=None)
+async def get_matryoshka_dimension_cached(kbid: str) -> Optional[int]:
+    # This can be safely cached as the matryoshka dimension is not expected to change
+    return await get_matryoshka_dimension(kbid)
+
+
+@query_parse_dependency_observer.wrap({"type": "matryoshka_dimension"})
+async def get_matryoshka_dimension(kbid: str) -> Optional[int]:
+    txn = await get_read_only_transaction()
+    return await datamanagers.kb.get_matryoshka_vector_dimension(txn, kbid=kbid)
```

## nucliadb/search/tests/unit/test_predict.py

```diff
@@ -23,15 +23,14 @@
 import aiohttp
 import pytest
 from yarl import URL
 
 from nucliadb.search.predict import (
     DummyPredictEngine,
     PredictEngine,
-    PredictVectorMissing,
     ProxiedPredictAPIError,
     RephraseError,
     RephraseMissingContextError,
     SendToPredictError,
     _parse_rephrase_response,
     get_answer_generator,
 )
@@ -54,89 +53,25 @@
 async def test_dummy_predict_engine():
     pe = DummyPredictEngine()
     await pe.initialize()
     await pe.finalize()
     await pe.send_feedback("kbid", Mock(), "", "", "")
     assert await pe.rephrase_query("kbid", Mock())
     assert await pe.chat_query("kbid", Mock())
-    assert await pe.convert_sentence_to_vector("kbid", "some sentence")
     assert await pe.detect_entities("kbid", "some sentence")
     assert await pe.ask_document("kbid", "query", [["footext"]], "userid")
     assert await pe.summarize("kbid", Mock(resources={}))
 
 
 @pytest.mark.asyncio
 @pytest.mark.parametrize(
     "onprem,expected_url,expected_header,expected_header_value",
     [
         (
             True,
-            "{public_url}/api/v1/predict/sentence/kbid",
-            "X-STF-NUAKEY",
-            "Bearer {service_account}",
-        ),
-        (False, "{cluster}/api/v1/internal/predict/sentence", "X-STF-KBID", "{kbid}"),
-    ],
-)
-async def test_convert_sentence_ok(
-    onprem, expected_url, expected_header, expected_header_value
-):
-    service_account = "service-account"
-
-    pe = PredictEngine(
-        "cluster",
-        "public-{zone}",
-        service_account,
-        zone="zone1",
-        onprem=onprem,
-    )
-
-    pe.session = get_mocked_session(
-        "GET", 200, json={"data": [0.0, 0.1]}, context_manager=False
-    )
-
-    kbid = "kbid"
-    sentence = "some sentence"
-
-    assert await pe.convert_sentence_to_vector(kbid, sentence) == [0.0, 0.1]
-
-    path = expected_url.format(public_url=pe.public_url, cluster=pe.cluster_url)
-
-    headers = {
-        expected_header: expected_header_value.format(
-            kbid=kbid, service_account=service_account
-        )
-    }
-    pe.session.get.assert_awaited_once_with(
-        url=path,
-        params={"text": sentence},
-        headers=headers,
-    )
-
-
-@pytest.mark.asyncio
-@pytest.mark.parametrize("onprem", [True, False])
-async def test_convert_sentence_error(onprem):
-    pe = PredictEngine(
-        "cluster",
-        "public-{zone}",
-        "service-account",
-        onprem=onprem,
-    )
-    pe.session = get_mocked_session("GET", 400, json="uops!", context_manager=False)
-    with pytest.raises(ProxiedPredictAPIError):
-        await pe.convert_sentence_to_vector("kbid", "some sentence")
-
-
-@pytest.mark.asyncio
-@pytest.mark.parametrize(
-    "onprem,expected_url,expected_header,expected_header_value",
-    [
-        (
-            True,
             "{public_url}/api/v1/predict/tokens/kbid",
             "X-STF-NUAKEY",
             "Bearer {service_account}",
         ),
         (False, "{cluster}/api/v1/internal/predict/tokens", "X-STF-KBID", "{kbid}"),
     ],
 )
@@ -205,15 +140,14 @@
     return session
 
 
 @pytest.mark.asyncio
 @pytest.mark.parametrize(
     "method,args",
     [
-        ("convert_sentence_to_vector", ["kbid", "sentence"]),
         ("detect_entities", ["kbid", "sentence"]),
         ("chat_query", ["kbid", ChatModel(question="foo", user_id="bar")]),
         (
             "send_feedback",
             [
                 "kbid",
                 FeedbackRequest(ident="foo", good=True, task=FeedbackTasks.CHAT),
@@ -242,15 +176,14 @@
 
 @pytest.mark.parametrize(
     "method,args,exception,output",
     [
         ("chat_query", ["kbid", Mock()], True, None),
         ("rephrase_query", ["kbid", Mock()], True, None),
         ("send_feedback", ["kbid", MagicMock(), "", "", ""], False, None),
-        ("convert_sentence_to_vector", ["kbid", "sentence"], False, []),
         ("detect_entities", ["kbid", "sentence"], False, []),
         ("ask_document", ["kbid", "query", [["footext"]], "userid"], True, None),
         ("summarize", ["kbid", Mock(resources={})], True, None),
     ],
 )
 async def test_onprem_nuclia_service_account_not_configured(
     method, args, exception, output
@@ -264,28 +197,14 @@
     if exception:
         with pytest.raises(SendToPredictError):
             await getattr(pe, method)(*args)
     else:
         assert await getattr(pe, method)(*args) == output
 
 
-async def test_convert_sentence_to_vector_empty_vectors():
-    pe = PredictEngine(
-        "cluster",
-        "public-{zone}",
-        nuclia_service_account="foo",
-        onprem=True,
-    )
-    pe.session = get_mocked_session(
-        "GET", 200, json={"data": []}, context_manager=False
-    )
-    with pytest.raises(PredictVectorMissing):
-        await pe.convert_sentence_to_vector("kbid", "sentence")
-
-
 async def test_ask_document_onprem():
     pe = PredictEngine(
         "cluster",
         "public-{zone}",
         nuclia_service_account="foo",
         zone="europe1",
         onprem=True,
```

## nucliadb/writer/back_pressure.py

```diff
@@ -37,15 +37,14 @@
 from nucliadb.common.http_clients.processing import ProcessingHTTPClient
 from nucliadb.writer import logger
 from nucliadb.writer.settings import back_pressure_settings as settings
 from nucliadb_telemetry import metrics
 from nucliadb_utils import const
 from nucliadb_utils.nats import NatsConnectionManager
 from nucliadb_utils.settings import is_onprem_nucliadb
-from nucliadb_utils.utilities import has_feature
 
 __all__ = ["maybe_back_pressure"]
 
 
 back_pressure_observer = metrics.Observer("nucliadb_back_pressure", labels={"type": ""})
 
 
@@ -340,18 +339,17 @@
 async def maybe_back_pressure(
     request: Request, kbid: str, resource_uuid: Optional[str] = None
 ) -> None:
     """
     This function does system checks to see if we need to put back pressure on writes.
     In that case, a HTTP 429 will be raised with the estimated time to try again.
     """
-    if has_feature(const.Features.BACK_PRESSURE, context={"kbid": kbid}):
-        if not is_back_pressure_enabled() or is_onprem_nucliadb():
-            return
-        await back_pressure_checks(request, kbid, resource_uuid)
+    if not is_back_pressure_enabled() or is_onprem_nucliadb():
+        return
+    await back_pressure_checks(request, kbid, resource_uuid)
 
 
 async def back_pressure_checks(
     request: Request, kbid: str, resource_uuid: Optional[str] = None
 ):
     """
     Will raise a 429 if back pressure is needed:
```

## nucliadb/writer/api/v1/field.py

```diff
@@ -47,14 +47,15 @@
     parse_keywordset_field,
     parse_layout_field,
     parse_link_field,
     parse_text_field,
 )
 from nucliadb.writer.utilities import get_processing
 from nucliadb_models.resource import NucliaDBRoles
+from nucliadb_models.utils import FieldIdString
 from nucliadb_models.writer import ResourceFieldAdded, ResourceUpdated
 from nucliadb_utils.authentication import requires
 from nucliadb_utils.exceptions import LimitsExceededError, SendToProcessError
 from nucliadb_utils.transaction import TransactionCommitTimeoutError
 from nucliadb_utils.utilities import (
     get_partitioning,
     get_storage,
@@ -140,15 +141,15 @@
 )
 @requires(NucliaDBRoles.WRITER)
 @version(1)
 async def add_resource_field_text_rslug_prefix(
     request: Request,
     kbid: str,
     rslug: str,
-    field_id: str,
+    field_id: FieldIdString,
     field_payload: models.TextField,
 ) -> ResourceFieldAdded:
     return await _add_resource_field_text(
         request,
         kbid,
         field_id,
         field_payload,
@@ -165,15 +166,15 @@
 )
 @requires(NucliaDBRoles.WRITER)
 @version(1)
 async def add_resource_field_text_rid_prefix(
     request: Request,
     kbid: str,
     rid: str,
-    field_id: str,
+    field_id: FieldIdString,
     field_payload: models.TextField,
 ) -> ResourceFieldAdded:
     return await _add_resource_field_text(
         request,
         kbid,
         field_id,
         field_payload,
@@ -208,15 +209,15 @@
 )
 @requires(NucliaDBRoles.WRITER)
 @version(1)
 async def add_resource_field_link_rslug_prefix(
     request: Request,
     kbid: str,
     rslug: str,
-    field_id: str,
+    field_id: FieldIdString,
     field_payload: models.LinkField,
 ) -> ResourceFieldAdded:
     return await _add_resource_field_link(
         request, kbid, field_id, field_payload, rslug=rslug
     )
 
 
@@ -229,15 +230,15 @@
 )
 @requires(NucliaDBRoles.WRITER)
 @version(1)
 async def add_resource_field_link_rid_prefix(
     request: Request,
     kbid: str,
     rid: str,
-    field_id: str,
+    field_id: FieldIdString,
     field_payload: models.LinkField,
 ) -> ResourceFieldAdded:
     return await _add_resource_field_link(
         request, kbid, field_id, field_payload, rid=rid
     )
 
 
@@ -268,15 +269,15 @@
 )
 @requires(NucliaDBRoles.WRITER)
 @version(1)
 async def add_resource_field_keywordset_rslug_prefix(
     request: Request,
     kbid: str,
     rslug: str,
-    field_id: str,
+    field_id: FieldIdString,
     field_payload: models.FieldKeywordset,
 ) -> ResourceFieldAdded:
     return await _add_resource_field_keywordset(
         request, kbid, field_id, field_payload, rslug=rslug
     )
 
 
@@ -289,15 +290,15 @@
 )
 @requires(NucliaDBRoles.WRITER)
 @version(1)
 async def add_resource_field_keywordset_rid_prefix(
     request: Request,
     kbid: str,
     rid: str,
-    field_id: str,
+    field_id: FieldIdString,
     field_payload: models.FieldKeywordset,
 ) -> ResourceFieldAdded:
     return await _add_resource_field_keywordset(
         request, kbid, field_id, field_payload, rid=rid
     )
 
 
@@ -328,15 +329,15 @@
 )
 @requires(NucliaDBRoles.WRITER)
 @version(1)
 async def add_resource_field_datetime_rslug_prefix(
     request: Request,
     kbid: str,
     rslug: str,
-    field_id: str,
+    field_id: FieldIdString,
     field_payload: models.FieldDatetime,
 ) -> ResourceFieldAdded:
     return await _add_resource_field_datetime(
         request, kbid, field_id, field_payload, rslug=rslug
     )
 
 
@@ -349,15 +350,15 @@
 )
 @requires(NucliaDBRoles.WRITER)
 @version(1)
 async def add_resource_field_datetime_rid_prefix(
     request: Request,
     kbid: str,
     rid: str,
-    field_id: str,
+    field_id: FieldIdString,
     field_payload: models.FieldDatetime,
 ) -> ResourceFieldAdded:
     return await _add_resource_field_datetime(
         request, kbid, field_id, field_payload, rid=rid
     )
 
 
@@ -388,15 +389,15 @@
 )
 @requires(NucliaDBRoles.WRITER)
 @version(1)
 async def add_resource_field_layout_rslug_prefix(
     request: Request,
     kbid: str,
     rslug: str,
-    field_id: str,
+    field_id: FieldIdString,
     field_payload: models.InputLayoutField,
 ) -> ResourceFieldAdded:
     return await _add_resource_field_layout(
         request,
         kbid,
         field_id,
         field_payload,
@@ -413,15 +414,15 @@
 )
 @requires(NucliaDBRoles.WRITER)
 @version(1)
 async def add_resource_field_layout_rid_prefix(
     request: Request,
     kbid: str,
     rid: str,
-    field_id: str,
+    field_id: FieldIdString,
     field_payload: models.InputLayoutField,
 ) -> ResourceFieldAdded:
     return await _add_resource_field_layout(
         request, kbid, field_id, field_payload, rid=rid
     )
 
 
@@ -452,15 +453,15 @@
 )
 @requires(NucliaDBRoles.WRITER)
 @version(1)
 async def add_resource_field_conversation_rslug_prefix(
     request: Request,
     kbid: str,
     rslug: str,
-    field_id: str,
+    field_id: FieldIdString,
     field_payload: models.InputConversationField,
 ) -> ResourceFieldAdded:
     return await _add_resource_field_conversation(
         request, kbid, field_id, field_payload, rslug=rslug
     )
 
 
@@ -473,15 +474,15 @@
 )
 @requires(NucliaDBRoles.WRITER)
 @version(1)
 async def add_resource_field_conversation_rid_prefix(
     request: Request,
     kbid: str,
     rid: str,
-    field_id: str,
+    field_id: FieldIdString,
     field_payload: models.InputConversationField,
 ) -> ResourceFieldAdded:
     return await _add_resource_field_conversation(
         request, kbid, field_id, field_payload, rid=rid
     )
 
 
@@ -514,15 +515,15 @@
 )
 @requires(NucliaDBRoles.WRITER)
 @version(1)
 async def add_resource_field_file_rslug_prefix(
     request: Request,
     kbid: str,
     rslug: str,
-    field_id: str,
+    field_id: FieldIdString,
     field_payload: models.FileField,
     x_skip_store: bool = SKIP_STORE_DEFAULT,
 ) -> ResourceFieldAdded:
     return await _add_resource_field_file(
         request,
         kbid,
         field_id,
@@ -541,15 +542,15 @@
 )
 @requires(NucliaDBRoles.WRITER)
 @version(1)
 async def add_resource_field_file_rid_prefix(
     request: Request,
     kbid: str,
     rid: str,
-    field_id: str,
+    field_id: FieldIdString,
     field_payload: models.FileField,
     x_skip_store: bool = SKIP_STORE_DEFAULT,
 ) -> ResourceFieldAdded:
     return await _add_resource_field_file(
         request, kbid, field_id, field_payload, x_skip_store, rid=rid
     )
 
@@ -584,15 +585,15 @@
 )
 @requires(NucliaDBRoles.WRITER)
 @version(1)
 async def append_messages_to_conversation_field_rslug_prefix(
     request: Request,
     kbid: str,
     rslug: str,
-    field_id: str,
+    field_id: FieldIdString,
     messages: list[models.InputMessage],
 ) -> ResourceFieldAdded:
     return await _append_messages_to_conversation_field(
         request, kbid, field_id, messages, rslug=rslug
     )
 
 
@@ -605,15 +606,15 @@
 )
 @requires(NucliaDBRoles.WRITER)
 @version(1)
 async def append_messages_to_conversation_field_rid_prefix(
     request: Request,
     kbid: str,
     rid: str,
-    field_id: str,
+    field_id: FieldIdString,
     messages: list[models.InputMessage],
 ) -> ResourceFieldAdded:
     return await _append_messages_to_conversation_field(
         request, kbid, field_id, messages, rid=rid
     )
 
 
@@ -686,15 +687,15 @@
 )
 @requires(NucliaDBRoles.WRITER)
 @version(1)
 async def append_blocks_to_layout_field_rslug_prefix(
     request: Request,
     kbid: str,
     rslug: str,
-    field_id: str,
+    field_id: FieldIdString,
     blocks: dict[str, models.InputBlock],
 ) -> ResourceFieldAdded:
     return await _append_blocks_to_layout_field(
         request, kbid, field_id, blocks, rslug=rslug
     )
 
 
@@ -707,15 +708,15 @@
 )
 @requires(NucliaDBRoles.WRITER)
 @version(1)
 async def append_blocks_to_layout_field_rid_prefix(
     request: Request,
     kbid: str,
     rid: str,
-    field_id: str,
+    field_id: FieldIdString,
     blocks: dict[str, models.InputBlock],
 ) -> ResourceFieldAdded:
     return await _append_blocks_to_layout_field(
         request, kbid, field_id, blocks, rid=rid
     )
 
 
@@ -787,15 +788,15 @@
 @requires(NucliaDBRoles.WRITER)
 @version(1)
 async def delete_resource_field_rslug_prefix(
     request: Request,
     kbid: str,
     rslug: str,
     field_type: models.FieldTypeName,
-    field_id: str,
+    field_id: FieldIdString,
 ):
     return await _delete_resource_field(
         request,
         kbid,
         field_type,
         field_id,
         rslug=rslug,
@@ -812,15 +813,15 @@
 @requires(NucliaDBRoles.WRITER)
 @version(1)
 async def delete_resource_field_rid_prefix(
     request: Request,
     kbid: str,
     rid: str,
     field_type: models.FieldTypeName,
-    field_id: str,
+    field_id: FieldIdString,
 ):
     return await _delete_resource_field(request, kbid, field_type, field_id, rid=rid)
 
 
 async def _delete_resource_field(
     request: Request,
     kbid: str,
@@ -867,15 +868,15 @@
 )
 @requires(NucliaDBRoles.WRITER)
 @version(1)
 async def reprocess_file_field(
     request: Request,
     kbid: str,
     rid: str,
-    field_id: str,
+    field_id: FieldIdString,
     x_nucliadb_user: str = X_NUCLIADB_USER,
     x_file_password: Optional[str] = X_FILE_PASSWORD,
 ) -> ResourceUpdated:
     await maybe_back_pressure(request, kbid, resource_uuid=rid)
 
     transaction = get_transaction_utility()
     processing = get_processing()
```

## nucliadb/writer/api/v1/upload.py

```diff
@@ -66,14 +66,15 @@
     InvalidTUSMetadata,
     ResumableURINotAvailable,
 )
 from nucliadb.writer.tus.storage import FileStorageManager  # type: ignore
 from nucliadb.writer.tus.utils import parse_tus_metadata
 from nucliadb.writer.utilities import get_processing
 from nucliadb_models.resource import NucliaDBRoles
+from nucliadb_models.utils import FieldIdString
 from nucliadb_models.writer import CreateResourcePayload, ResourceFileUploaded
 from nucliadb_utils.authentication import requires_one
 from nucliadb_utils.exceptions import LimitsExceededError, SendToProcessError
 from nucliadb_utils.storages.storage import KB_RESOURCE_FIELD
 from nucliadb_utils.transaction import TransactionCommitTimeoutError
 from nucliadb_utils.utilities import (
     get_ingest,
@@ -144,15 +145,15 @@
 )
 @requires_one([NucliaDBRoles.WRITER])
 @version(1)
 async def tus_post_rslug_prefix(
     request: Request,
     kbid: str,
     rslug: str,
-    field: str,
+    field: FieldIdString,
     item: Optional[CreateResourcePayload] = None,
 ) -> Response:
     return await _tus_post(request, kbid, item=item, rslug=rslug, field=field)
 
 
 @api.post(
     f"/{KB_PREFIX}/{{kbid}}/{RESOURCE_PREFIX}/{{path_rid}}/file/{{field}}/{TUSUPLOAD}",
@@ -162,15 +163,15 @@
 )
 @requires_one([NucliaDBRoles.WRITER])
 @version(1)
 async def tus_post_rid_prefix(
     request: Request,
     kbid: str,
     path_rid: str,
-    field: str,
+    field: FieldIdString,
     item: Optional[CreateResourcePayload] = None,
 ) -> Response:
     return await _tus_post(request, kbid, item=item, path_rid=path_rid, field=field)
 
 
 @api.post(
     f"/{KB_PREFIX}/{{kbid}}/{TUSUPLOAD}",
@@ -323,15 +324,15 @@
 )
 @requires_one([NucliaDBRoles.WRITER])
 @version(1)
 async def tus_head_rslug_prefix(
     request: Request,
     kbid: str,
     rslug: str,
-    field: str,
+    field: FieldIdString,
     upload_id: str,
 ) -> Response:
     return await _tus_head(upload_id)
 
 
 @api.head(
     f"/{KB_PREFIX}/{{kbid}}/{RESOURCE_PREFIX}/{{path_rid}}/file/{{field}}/{TUSUPLOAD}/{{upload_id}}",
@@ -342,15 +343,15 @@
 )
 @requires_one([NucliaDBRoles.WRITER])
 @version(1)
 async def tus_head_rid_prefix(
     request: Request,
     kbid: str,
     path_rid: str,
-    field: str,
+    field: FieldIdString,
     upload_id: str,
 ) -> Response:
     return await _tus_head(upload_id)
 
 
 @api.head(
     f"/{KB_PREFIX}/{{kbid}}/{TUSUPLOAD}/{{upload_id}}",
@@ -399,15 +400,15 @@
 )
 @requires_one([NucliaDBRoles.WRITER])
 @version(1)
 async def tus_patch_rslug_prefix(
     request: Request,
     kbid: str,
     rslug: str,
-    field: str,
+    field: FieldIdString,
     upload_id: str,
 ) -> Response:
     return await tus_patch(request, kbid, upload_id, rslug=rslug, field=field)
 
 
 @api.patch(
     f"/{KB_PREFIX}/{{kbid}}/{RESOURCE_PREFIX}/{{rid}}/file/{{field}}/{TUSUPLOAD}/{{upload_id}}",
@@ -418,15 +419,15 @@
 )
 @requires_one([NucliaDBRoles.WRITER])
 @version(1)
 async def tus_patch_rid_prefix(
     request: Request,
     kbid: str,
     rid: str,
-    field: str,
+    field: FieldIdString,
     upload_id: str,
 ) -> Response:
     return await tus_patch(request, kbid, upload_id, rid=rid, field=field)
 
 
 @api.patch(
     f"/{KB_PREFIX}/{{kbid}}/{TUSUPLOAD}/{{upload_id}}",
@@ -604,15 +605,15 @@
 )
 @requires_one([NucliaDBRoles.WRITER])
 @version(1)
 async def upload_rslug_prefix(
     request: StarletteRequest,
     kbid: str,
     rslug: str,
-    field: str,
+    field: FieldIdString,
     x_filename: Optional[list[str]] = Header(None),  # type: ignore
     x_password: Optional[list[str]] = Header(None),  # type: ignore
     x_language: Optional[list[str]] = Header(None),  # type: ignore
     x_md5: Optional[list[str]] = Header(None),  # type: ignore
 ) -> ResourceFileUploaded:
     return await _upload(
         request,
@@ -635,15 +636,15 @@
 )
 @requires_one([NucliaDBRoles.WRITER])
 @version(1)
 async def upload_rid_prefix(
     request: StarletteRequest,
     kbid: str,
     path_rid: str,
-    field: str,
+    field: FieldIdString,
     x_filename: Optional[list[str]] = Header(None),  # type: ignore
     x_password: Optional[list[str]] = Header(None),  # type: ignore
     x_language: Optional[list[str]] = Header(None),  # type: ignore
     x_md5: Optional[list[str]] = Header(None),  # type: ignore
 ) -> ResourceFileUploaded:
     return await _upload(
         request,
```

## Comparing `nucliadb-3.0.3.post447.dist-info/METADATA` & `nucliadb-3.0.3.post450.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nucliadb
-Version: 3.0.3.post447
+Version: 3.0.3.post450
 Home-page: https://docs.nuclia.dev/docs/guides/nucliadb/intro
 Author: NucliaDB Community
 Author-email: nucliadb@nuclia.com
 License: BSD
 Project-URL: Nuclia, https://nuclia.com
 Project-URL: Github, https://github.com/nuclia/nucliadb
 Project-URL: Discord, https://discord.gg/8EvQwmsbzf
@@ -17,18 +17,18 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.9, <4
 Description-Content-Type: text/markdown
-Requires-Dist: nucliadb-telemetry[all] >=3.0.3.post447
-Requires-Dist: nucliadb-utils[cache,fastapi,storages] >=3.0.3.post447
-Requires-Dist: nucliadb-protos >=3.0.3.post447
-Requires-Dist: nucliadb-models >=3.0.3.post447
+Requires-Dist: nucliadb-telemetry[all] >=3.0.3.post450
+Requires-Dist: nucliadb-utils[cache,fastapi,storages] >=3.0.3.post450
+Requires-Dist: nucliadb-protos >=3.0.3.post450
+Requires-Dist: nucliadb-models >=3.0.3.post450
 Requires-Dist: nucliadb-admin-assets >=1.0.0.post1224
 Requires-Dist: nucliadb-node-binding >=2.26.0
 Requires-Dist: uvicorn <0.19.0
 Requires-Dist: pydantic-argparse
 Requires-Dist: aiohttp >=3.9.4
 Requires-Dist: lru-dict >=1.1.7
 Requires-Dist: backoff
```

## Comparing `nucliadb-3.0.3.post447.dist-info/entry_points.txt` & `nucliadb-3.0.3.post450.dist-info/entry_points.txt`

 * *Files identical despite different names*

## Comparing `nucliadb-3.0.3.post447.dist-info/RECORD` & `nucliadb-3.0.3.post450.dist-info/RECORD`

 * *Files 1% similar despite different names*

```diff
@@ -195,15 +195,15 @@
 nucliadb/reader/tests/test_reader_file_download.py,sha256=V_wLTRmSlYemSPLOBo3A_jhMBluro2sJiQwSsGGBx6I,10199
 nucliadb/reader/tests/test_reader_resource.py,sha256=A7XzHngspJxPqxzyMZ2Zg2Kp8SuDTi78Fo2rG1roLyo,10586
 nucliadb/reader/tests/test_reader_resource_field.py,sha256=YQ-U2mEGhs_rPGxcWPZmWLSEoCxBo3AVDtLZCtZrGb8,6535
 nucliadb/search/__init__.py,sha256=fwzdF6p7p9uDCtE38gTUxrRVIdbEDVQTAXWUMVKgSBM,1535
 nucliadb/search/app.py,sha256=azMj8BiaFr03pYQKcWSr2YqjB0FopJDeVKE2wwuj6pU,4905
 nucliadb/search/lifecycle.py,sha256=s6If2a78dcv4_71d-Q_uA6b9TaJCQOASUhqa2HcxfIw,1956
 nucliadb/search/openapi.py,sha256=t3Wo_4baTrfPftg2BHsyLWNZ1MYn7ZRdW7ht-wFOgRs,1016
-nucliadb/search/predict.py,sha256=gfhWT9SM316KWcztzMmXuCJwuD_aih-bWxG5gNjKhv4,19798
+nucliadb/search/predict.py,sha256=u_49fIHNlduVDxd7kbZJO5UYmgSyPSH-PVpu7OG9UOU,18535
 nucliadb/search/run.py,sha256=aFb-CXRi_C8YMpP_ivNj8KW1BYhADj88y8K9Lr_nUPI,1402
 nucliadb/search/settings.py,sha256=Nm4BkdNNdYfU1wGvvWMvlazRSlRGoae99GEdm48-bXI,1193
 nucliadb/search/utilities.py,sha256=9SsRDw0rJVXVoLBfF7rBb6q080h-thZc7u8uRcTiBeY,1037
 nucliadb/search/api/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
 nucliadb/search/api/v1/__init__.py,sha256=JH9NGhhyRzirOYY5_pDx5zGZVvpU3317lygSbEb0MFk,1272
 nucliadb/search/api/v1/chat.py,sha256=dNaU4Cfkbta9-buRsPb98s1gsfvvzVCQIoYp2yvICmk,9913
 nucliadb/search/api/v1/feedback.py,sha256=j0PGSGDSbwwS5clRDbU_iCxuISFOtf2DN9Ey-fVGpso,2665
@@ -228,15 +228,15 @@
 nucliadb/search/search/filters.py,sha256=HpTpaDjKmUZWkp5xFFqKHz3TYdKEVBk4jWb2ssIYa5g,6513
 nucliadb/search/search/find.py,sha256=cnWh2yC6Zq0XNG0c0ciycFr1APobbCF1Fye4fatxSIc,4646
 nucliadb/search/search/find_merge.py,sha256=vhq14MFE7N9-9SNlg66LNUr6YAhR9cW22oDpmjvQhL0,17152
 nucliadb/search/search/merge.py,sha256=-srmB1gZEuMa9c2_hLTD1ihjJwDhdB6wnp9b7ljxuIM,21282
 nucliadb/search/search/metrics.py,sha256=4xQm4Q0_-R1bgMtnrbm-YaClEFR8HE6wDk9lunCrhjo,1130
 nucliadb/search/search/paragraphs.py,sha256=8TTii45JvQ7SXsV9Z9ipt5QpYk7ux6PnlOkjKPfYz4A,8698
 nucliadb/search/search/predict_proxy.py,sha256=aOq1AzXkUdHtEmXsec07ffuMKGjlMu-NaUxb_IKme6U,3026
-nucliadb/search/search/query.py,sha256=HR5q_LbbXUKW6gtBPtjDYHBaNe6otRzKAP1ndGDcnlw,32831
+nucliadb/search/search/query.py,sha256=LjJjhnm1_XLbo2KFMJYkUH9Z_svbrsEJvw-evRNSPyA,31300
 nucliadb/search/search/shards.py,sha256=CiQHBPR-_IjtfaC_897adddH4sRSxgfTEURuFpoMLQs,3149
 nucliadb/search/search/summarize.py,sha256=bjncFFBv1R9g4OyhQSlGHFq5cJ8UvR8KrMgeKc-1AMU,5101
 nucliadb/search/search/utils.py,sha256=Gzjr9rFdwRfOgyDzX1Slz8DbcXLvavo0124S8II9omw,2438
 nucliadb/search/search/chat/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
 nucliadb/search/search/chat/images.py,sha256=AjPgCJaCzu19ruUJcEVaG_bEUmqzB65EH0mduMbkzAE,2058
 nucliadb/search/search/chat/prompt.py,sha256=W98mZrhrscjkxVJ02OM7veAQ1fjMrNDSZ1CUSaECCCk,20793
 nucliadb/search/search/chat/query.py,sha256=4wV6nwzNVA4skiUVM0ggBgdRR7BjYHZ801b87WAuIgI,15347
@@ -244,15 +244,15 @@
 nucliadb/search/tests/conftest.py,sha256=BhVEPbrIm7GKDHtnS7tc7WqCRReIL4MzzTjLQUWrLJY,1295
 nucliadb/search/tests/fixtures.py,sha256=a0q-mh15uvr97ebGTStcdONWx4AQ8rdkH772azMwMMg,6578
 nucliadb/search/tests/node.py,sha256=S1JT1Rq7K2w_4c-bjSUkazr7bDN_OvjTTuYv1Ut_j64,15529
 nucliadb/search/tests/unit/__init__.py,sha256=itSI7dtTwFP55YMX4iK7JzdMHS5CQVUiB1XzQu4UBh8,833
 nucliadb/search/tests/unit/test_app.py,sha256=3wr6_DTLdwhpk7Sske7EEqmGbaJSG4OH9Olw_KVszPw,2649
 nucliadb/search/tests/unit/test_find_merge.py,sha256=z_qLcXG8qdUegGkaEloG7wXXwoZyppeOnzUCcHAVq3w,3374
 nucliadb/search/tests/unit/test_merge.py,sha256=1uCdn3MZbUWs2WKFGJSJZgpm4xTtn5nvgurbo37l5B8,1400
-nucliadb/search/tests/unit/test_predict.py,sha256=V2EPtZwWMqu36OajrwxkyMCUV-ntDAngo2YoCk8dGMA,17080
+nucliadb/search/tests/unit/test_predict.py,sha256=TUEk2zGwAss0CpdoEtM3C3mxbn_tn9x3hg9SsDzJgrQ,14729
 nucliadb/search/tests/unit/test_run.py,sha256=7fDXkaEOSd8f3Cd7w5QWYeB4uGXA59M22MojR1auv0Y,1317
 nucliadb/search/tests/unit/api/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
 nucliadb/search/tests/unit/api/v1/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
 nucliadb/search/tests/unit/api/v1/test_chat.py,sha256=Ud6MDM7gLUV6PZQeCDA5vBcJ40Sf4fqNeWBwYWUOi-E,2966
 nucliadb/search/tests/unit/api/v1/test_predict_proxy.py,sha256=CuouBrldS3mpBZe3FlpkaW3R_cI8Db8o6bSFPW0ifmA,2865
 nucliadb/search/tests/unit/api/v1/test_summarize.py,sha256=4VQm-fegHLeBNBoNuoKbKM5FiqAML9m9QT7XNY3n2n4,2901
 nucliadb/search/tests/unit/api/v1/resource/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
@@ -397,33 +397,33 @@
 nucliadb/train/tests/test_paragraph_streaming.py,sha256=CMwGEDBQ3iwf7pldZfOBphFSYCvTLKPd1dDHgoHtslQ,4320
 nucliadb/train/tests/test_question_answer_streaming.py,sha256=URtFXd6sEy72Q1By5LtcwIPT5S_yQ0Ip8AjJPILUeDU,8751
 nucliadb/train/tests/test_sentence_classification.py,sha256=6cex9xJN1AGZhsVD1jG2JKYgZEmo09picNJkUrLjDDQ,5051
 nucliadb/train/tests/test_token_classification.py,sha256=fBS70sCKFWBjcaUDny9fg8qZgsQ5VtKBTPENFTgkHrk,5583
 nucliadb/train/tests/utils.py,sha256=J5UZoCz4Ss5b6SmZuyC7jJQlomQE8mDQ8E2OdYEV-gA,3324
 nucliadb/writer/__init__.py,sha256=HkfMuQR3CbbPU3g-A85Ibt8iwSTTADhLc0-pi3F3hvk,1328
 nucliadb/writer/app.py,sha256=Q55CmGR85wG5pjf_Ro-73QVWc7_wMpIt69xJSZ0kjCQ,4268
-nucliadb/writer/back_pressure.py,sha256=x50SQitYFC4yf0gkquLOZUnhenUJzDPaxjdbDauHUWc,19630
+nucliadb/writer/back_pressure.py,sha256=DPNeBVNQuRZzOEBMDmRIoeLDEuvRwwIGFBKNOQg3-xE,19495
 nucliadb/writer/exceptions.py,sha256=2dMvuoF68v3BZuyzaBEsbG6gusQqwLFcn47qm1zNdTc,972
 nucliadb/writer/lifecycle.py,sha256=gF9it0w98uBGCwzjs72e8mGi6H-qv_XAa2GGNBTOEDY,1953
 nucliadb/writer/openapi.py,sha256=thqCO1ht_RJgOkXs-aIsv8aXJrU5z8wo2n05l2_LqMs,1032
 nucliadb/writer/run.py,sha256=euVZ_rtHDXs-O1kB-Pt1Id8eft9CYVpWH3zJzEoEqls,1448
 nucliadb/writer/settings.py,sha256=A1JY7pFQzLPV0Vm0TSG6jPBR3dEMK76SknbeANTG4Hg,3074
 nucliadb/writer/utilities.py,sha256=AZ5qEny1Xm0IDsFtH13oJa2usvJZK8f0FdgF1LrnLCw,1036
 nucliadb/writer/vectors.py,sha256=cqiBtqAVTpG2kvR7VKUrhLfH8XQS8wEdE1q-CxVnhEw,1948
 nucliadb/writer/api/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
 nucliadb/writer/api/constants.py,sha256=b63uWvu7_bwg51R6EL5DaJwoT550Ih4GhVXzvEYLQNQ,1429
 nucliadb/writer/api/v1/__init__.py,sha256=FVn7N9VJ6bsEoy4TRnkclr4Umd5hECiwPXVqRnJ8BME,1095
 nucliadb/writer/api/v1/export_import.py,sha256=LrGg7y5Aq8xEnoYr529HG0g9LcF2UjP1VFpk9z1pJfE,6565
-nucliadb/writer/api/v1/field.py,sha256=rOY6qTXhrK17Betdv3ImwoqmX1XMc1fCXvoGyCjxMg8,28320
+nucliadb/writer/api/v1/field.py,sha256=PNHaaO37WRW2FxCaYq-PqthLPu0lOZdmrWX_R7axToc,28578
 nucliadb/writer/api/v1/knowledgebox.py,sha256=sFPPOsB2z-ljV51JP7oHMxUjejnJXMw93Pq8i-EMRkg,5239
 nucliadb/writer/api/v1/learning_config.py,sha256=GQN2d2N2IJLPX-S7hddTgrb7fDE8gCJ1MghgsIjBPKA,2052
 nucliadb/writer/api/v1/resource.py,sha256=x3hi_n4i9syK67v9LWdQZxGBImmnd95Rd7i2OqUHSW8,19940
 nucliadb/writer/api/v1/router.py,sha256=RjuoWLpZer6Kl2BW_wznpNo6XL3BOpdTGqXZCn3QrrQ,1034
 nucliadb/writer/api/v1/services.py,sha256=l7mNQVRTCoGem1fR8p2NYb6l3rLaWp9MMFlwaXONbFU,12733
-nucliadb/writer/api/v1/upload.py,sha256=XQz4RcMpDGWLbi03CPTJ4ZDIBtHeHspqkFzckLYspfM,31464
+nucliadb/writer/api/v1/upload.py,sha256=zjmMbINM5_HW0e94I2cXpBrpv53yBtnTFoOqBXILDIo,31592
 nucliadb/writer/layouts/__init__.py,sha256=Siod9W963CG5gJa20GSTw9VemAFgsMmJDbUspbrYAyE,1612
 nucliadb/writer/layouts/v1.py,sha256=Yc2idmfrpCS8js_XJByNWA_tmt2WeKoWvidLHoTPXoo,2115
 nucliadb/writer/resource/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
 nucliadb/writer/resource/audit.py,sha256=SXPu_hdNBlm9uCSl666UQL7hzMx9zYVbBLT_U7ro8Gs,1425
 nucliadb/writer/resource/basic.py,sha256=eSWW6u6U3e0KjjdFwp9YQokojoDepl5vmJfbE2MQACM,10968
 nucliadb/writer/resource/field.py,sha256=7Y1vfuKDv1b3e7NCjEvDg8mktGR1rnzHaC5_qNj-3YQ,16319
 nucliadb/writer/resource/origin.py,sha256=3Y2zVtG_v0U6uMbDhW9Yl7KKHKt5V3T5_v3iCpqdBEk,2022
@@ -444,13 +444,13 @@
 nucliadb/writer/tus/exceptions.py,sha256=CmxYKnHXpXug25DYV4SpVAU47SGD-NVBd7pNTRbWHyk,2186
 nucliadb/writer/tus/gcs.py,sha256=WykJZicWKRYkVB5_Fkb_1cVLovAk86IVkEn1VgEDufc,14527
 nucliadb/writer/tus/local.py,sha256=lIOoGaylnsxPBYGskcmKSHv7MsvwIYFS4soDLey_KSs,5849
 nucliadb/writer/tus/pg.py,sha256=JUK_xKsyNcKAvWOch8gUMTc_e1evI_3aC6-Y5gMk2jw,4367
 nucliadb/writer/tus/s3.py,sha256=a9mfPtjBW3QaTYY2r6P7u_Y13V6mBefZjWgV4juZzgE,9069
 nucliadb/writer/tus/storage.py,sha256=8iBOjWIcY6PawQq_rmSiBKi0Gl6J6Q5ad6L-9nLCcJ4,4734
 nucliadb/writer/tus/utils.py,sha256=MSdVbRsRSZVdkaum69_0wku7X3p5wlZf4nr6E0GMKbw,2556
-nucliadb-3.0.3.post447.dist-info/METADATA,sha256=lhIJkPYGbGm-qofvFJKVNrvg7i6lXAt11K6jrtI1H18,4343
-nucliadb-3.0.3.post447.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-nucliadb-3.0.3.post447.dist-info/entry_points.txt,sha256=XqGfgFDuY3zXQc8ewXM2TRVjTModIq851zOsgrmaXx4,1268
-nucliadb-3.0.3.post447.dist-info/top_level.txt,sha256=hwYhTVnX7jkQ9gJCkVrbqEG1M4lT2F_iPQND1fCzF80,20
-nucliadb-3.0.3.post447.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-nucliadb-3.0.3.post447.dist-info/RECORD,,
+nucliadb-3.0.3.post450.dist-info/METADATA,sha256=KdylbRdtE430_pgkXKAoPZVoE600MkQCYhEZpkz-RpQ,4343
+nucliadb-3.0.3.post450.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+nucliadb-3.0.3.post450.dist-info/entry_points.txt,sha256=XqGfgFDuY3zXQc8ewXM2TRVjTModIq851zOsgrmaXx4,1268
+nucliadb-3.0.3.post450.dist-info/top_level.txt,sha256=hwYhTVnX7jkQ9gJCkVrbqEG1M4lT2F_iPQND1fCzF80,20
+nucliadb-3.0.3.post450.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
+nucliadb-3.0.3.post450.dist-info/RECORD,,
```


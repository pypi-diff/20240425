# Comparing `tmp/nucliadb-3.0.3.post450-py3-none-any.whl.zip` & `tmp/nucliadb-3.0.3.post454-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,458 +1,457 @@
-Zip file size: 754424 bytes, number of entries: 456
--rw-r--r--  2.0 unx     1135 b- defN 24-Apr-24 07:29 migrations/0001_bootstrap.py
--rw-r--r--  2.0 unx     1177 b- defN 24-Apr-24 07:29 migrations/0002_rollover_shards.py
--rw-r--r--  2.0 unx     2436 b- defN 24-Apr-24 07:29 migrations/0003_allfields_key.py
--rw-r--r--  2.0 unx     1177 b- defN 24-Apr-24 07:29 migrations/0004_rollover_shards.py
--rw-r--r--  2.0 unx     1177 b- defN 24-Apr-24 07:29 migrations/0005_rollover_shards.py
--rw-r--r--  2.0 unx     1024 b- defN 24-Apr-24 07:29 migrations/0006_rollover_shards.py
--rw-r--r--  2.0 unx     1301 b- defN 24-Apr-24 07:29 migrations/0008_cleanup_leftover_rollover_metadata.py
--rw-r--r--  2.0 unx     1378 b- defN 24-Apr-24 07:29 migrations/0009_upgrade_relations_and_texts_to_v2.py
--rw-r--r--  2.0 unx     1610 b- defN 24-Apr-24 07:29 migrations/0010_fix_corrupt_indexes.py
--rw-r--r--  2.0 unx     1843 b- defN 24-Apr-24 07:29 migrations/0011_materialize_labelset_ids.py
--rw-r--r--  2.0 unx     1443 b- defN 24-Apr-24 07:29 migrations/0012_rollover_shards.py
--rw-r--r--  2.0 unx     1024 b- defN 24-Apr-24 07:29 migrations/0013_rollover_shards.py
--rw-r--r--  2.0 unx     1382 b- defN 24-Apr-24 07:29 migrations/0014_rollover_shards.py
--rw-r--r--  2.0 unx     1462 b- defN 24-Apr-24 07:29 migrations/0015_targeted_rollover.py
--rw-r--r--  2.0 unx     2506 b- defN 24-Apr-24 07:29 migrations/0016_upgrade_to_paragraphs_v2.py
--rw-r--r--  2.0 unx     2100 b- defN 24-Apr-24 07:29 migrations/0017_multiple_writable_shards.py
--rw-r--r--  2.0 unx     2264 b- defN 24-Apr-24 07:29 migrations/0018_purge_orphan_kbslugs.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-24 07:29 migrations/__init__.py
--rw-r--r--  2.0 unx      891 b- defN 24-Apr-24 07:29 nucliadb/__init__.py
--rw-r--r--  2.0 unx     3733 b- defN 24-Apr-24 07:29 nucliadb/health.py
--rw-r--r--  2.0 unx    11626 b- defN 24-Apr-24 07:29 nucliadb/learning_proxy.py
--rw-r--r--  2.0 unx     4806 b- defN 24-Apr-24 07:29 nucliadb/metrics_exporter.py
--rw-r--r--  2.0 unx     2272 b- defN 24-Apr-24 07:29 nucliadb/openapi.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-24 07:29 nucliadb/py.typed
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-24 07:29 nucliadb/common/__init__.py
--rw-r--r--  2.0 unx     4905 b- defN 24-Apr-24 07:29 nucliadb/common/locking.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-24 07:29 nucliadb/common/cluster/__init__.py
--rw-r--r--  2.0 unx     5090 b- defN 24-Apr-24 07:29 nucliadb/common/cluster/base.py
--rw-r--r--  2.0 unx     1495 b- defN 24-Apr-24 07:29 nucliadb/common/cluster/exceptions.py
--rw-r--r--  2.0 unx     3658 b- defN 24-Apr-24 07:29 nucliadb/common/cluster/grpc_node_dummy.py
--rw-r--r--  2.0 unx     3429 b- defN 24-Apr-24 07:29 nucliadb/common/cluster/index_node.py
--rw-r--r--  2.0 unx    21231 b- defN 24-Apr-24 07:29 nucliadb/common/cluster/manager.py
--rw-r--r--  2.0 unx     8490 b- defN 24-Apr-24 07:29 nucliadb/common/cluster/rebalance.py
--rw-r--r--  2.0 unx    19593 b- defN 24-Apr-24 07:29 nucliadb/common/cluster/rollover.py
--rw-r--r--  2.0 unx     2713 b- defN 24-Apr-24 07:29 nucliadb/common/cluster/settings.py
--rw-r--r--  2.0 unx     5494 b- defN 24-Apr-24 07:29 nucliadb/common/cluster/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-24 07:29 nucliadb/common/cluster/discovery/__init__.py
--rw-r--r--  2.0 unx     6553 b- defN 24-Apr-24 07:29 nucliadb/common/cluster/discovery/base.py
--rw-r--r--  2.0 unx    12518 b- defN 24-Apr-24 07:29 nucliadb/common/cluster/discovery/k8s.py
--rw-r--r--  2.0 unx     1957 b- defN 24-Apr-24 07:29 nucliadb/common/cluster/discovery/manual.py
--rw-r--r--  2.0 unx     1737 b- defN 24-Apr-24 07:29 nucliadb/common/cluster/discovery/single.py
--rw-r--r--  2.0 unx     1139 b- defN 24-Apr-24 07:29 nucliadb/common/cluster/discovery/types.py
--rw-r--r--  2.0 unx     2548 b- defN 24-Apr-24 07:29 nucliadb/common/cluster/discovery/utils.py
--rw-r--r--  2.0 unx      833 b- defN 24-Apr-24 07:29 nucliadb/common/cluster/standalone/__init__.py
--rw-r--r--  2.0 unx    13707 b- defN 24-Apr-24 07:29 nucliadb/common/cluster/standalone/grpc_node_binding.py
--rw-r--r--  2.0 unx     4683 b- defN 24-Apr-24 07:29 nucliadb/common/cluster/standalone/index_node.py
--rw-r--r--  2.0 unx     3444 b- defN 24-Apr-24 07:29 nucliadb/common/cluster/standalone/service.py
--rw-r--r--  2.0 unx     3386 b- defN 24-Apr-24 07:29 nucliadb/common/cluster/standalone/utils.py
--rw-r--r--  2.0 unx     3498 b- defN 24-Apr-24 07:29 nucliadb/common/context/__init__.py
--rw-r--r--  2.0 unx     1628 b- defN 24-Apr-24 07:29 nucliadb/common/context/fastapi.py
--rw-r--r--  2.0 unx     1813 b- defN 24-Apr-24 07:29 nucliadb/common/datamanagers/__init__.py
--rw-r--r--  2.0 unx     1451 b- defN 24-Apr-24 07:29 nucliadb/common/datamanagers/cluster.py
--rw-r--r--  2.0 unx     5383 b- defN 24-Apr-24 07:29 nucliadb/common/datamanagers/entities.py
--rw-r--r--  2.0 unx      883 b- defN 24-Apr-24 07:29 nucliadb/common/datamanagers/exceptions.py
--rw-r--r--  2.0 unx     3994 b- defN 24-Apr-24 07:29 nucliadb/common/datamanagers/kb.py
--rw-r--r--  2.0 unx     5389 b- defN 24-Apr-24 07:29 nucliadb/common/datamanagers/labels.py
--rw-r--r--  2.0 unx     1599 b- defN 24-Apr-24 07:29 nucliadb/common/datamanagers/processing.py
--rw-r--r--  2.0 unx     7637 b- defN 24-Apr-24 07:29 nucliadb/common/datamanagers/resources.py
--rw-r--r--  2.0 unx     5633 b- defN 24-Apr-24 07:29 nucliadb/common/datamanagers/rollover.py
--rw-r--r--  2.0 unx     1681 b- defN 24-Apr-24 07:29 nucliadb/common/datamanagers/utils.py
--rw-r--r--  2.0 unx     2055 b- defN 24-Apr-24 07:29 nucliadb/common/datamanagers/vectorsets.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-24 07:29 nucliadb/common/http_clients/__init__.py
--rw-r--r--  2.0 unx     2146 b- defN 24-Apr-24 07:29 nucliadb/common/http_clients/auth.py
--rw-r--r--  2.0 unx     1100 b- defN 24-Apr-24 07:29 nucliadb/common/http_clients/exceptions.py
--rw-r--r--  2.0 unx     7155 b- defN 24-Apr-24 07:29 nucliadb/common/http_clients/processing.py
--rw-r--r--  2.0 unx     1540 b- defN 24-Apr-24 07:29 nucliadb/common/http_clients/pypi.py
--rw-r--r--  2.0 unx     1551 b- defN 24-Apr-24 07:29 nucliadb/common/http_clients/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-24 07:29 nucliadb/common/maindb/__init__.py
--rw-r--r--  2.0 unx     3449 b- defN 24-Apr-24 07:29 nucliadb/common/maindb/driver.py
--rw-r--r--  2.0 unx      946 b- defN 24-Apr-24 07:29 nucliadb/common/maindb/exceptions.py
--rw-r--r--  2.0 unx     6769 b- defN 24-Apr-24 07:29 nucliadb/common/maindb/local.py
--rw-r--r--  2.0 unx     8391 b- defN 24-Apr-24 07:29 nucliadb/common/maindb/pg.py
--rw-r--r--  2.0 unx     6053 b- defN 24-Apr-24 07:29 nucliadb/common/maindb/redis.py
--rw-r--r--  2.0 unx    14502 b- defN 24-Apr-24 07:29 nucliadb/common/maindb/tikv.py
--rw-r--r--  2.0 unx     4109 b- defN 24-Apr-24 07:29 nucliadb/common/maindb/utils.py
--rw-r--r--  2.0 unx      932 b- defN 24-Apr-24 07:29 nucliadb/export_import/__init__.py
--rw-r--r--  2.0 unx     6171 b- defN 24-Apr-24 07:29 nucliadb/export_import/datamanager.py
--rw-r--r--  2.0 unx     1949 b- defN 24-Apr-24 07:29 nucliadb/export_import/exceptions.py
--rw-r--r--  2.0 unx     7116 b- defN 24-Apr-24 07:29 nucliadb/export_import/exporter.py
--rw-r--r--  2.0 unx     4258 b- defN 24-Apr-24 07:29 nucliadb/export_import/importer.py
--rw-r--r--  2.0 unx     2063 b- defN 24-Apr-24 07:29 nucliadb/export_import/models.py
--rw-r--r--  2.0 unx     2571 b- defN 24-Apr-24 07:29 nucliadb/export_import/tasks.py
--rw-r--r--  2.0 unx    19270 b- defN 24-Apr-24 07:29 nucliadb/export_import/utils.py
--rw-r--r--  2.0 unx     1011 b- defN 24-Apr-24 07:29 nucliadb/ingest/__init__.py
--rw-r--r--  2.0 unx     7277 b- defN 24-Apr-24 07:29 nucliadb/ingest/app.py
--rw-r--r--  2.0 unx     1005 b- defN 24-Apr-24 07:29 nucliadb/ingest/cache.py
--rw-r--r--  2.0 unx     2484 b- defN 24-Apr-24 07:29 nucliadb/ingest/partitions.py
--rw-r--r--  2.0 unx    19541 b- defN 24-Apr-24 07:29 nucliadb/ingest/processing.py
--rw-r--r--  2.0 unx    20277 b- defN 24-Apr-24 07:29 nucliadb/ingest/serialize.py
--rw-r--r--  2.0 unx     3183 b- defN 24-Apr-24 07:29 nucliadb/ingest/settings.py
--rw-r--r--  2.0 unx     2314 b- defN 24-Apr-24 07:29 nucliadb/ingest/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-24 07:29 nucliadb/ingest/consumer/__init__.py
--rw-r--r--  2.0 unx    11563 b- defN 24-Apr-24 07:29 nucliadb/ingest/consumer/auditing.py
--rw-r--r--  2.0 unx    12159 b- defN 24-Apr-24 07:29 nucliadb/ingest/consumer/consumer.py
--rw-r--r--  2.0 unx     3788 b- defN 24-Apr-24 07:29 nucliadb/ingest/consumer/materializer.py
--rw-r--r--  2.0 unx     1075 b- defN 24-Apr-24 07:29 nucliadb/ingest/consumer/metrics.py
--rw-r--r--  2.0 unx     9543 b- defN 24-Apr-24 07:29 nucliadb/ingest/consumer/pull.py
--rw-r--r--  2.0 unx     6935 b- defN 24-Apr-24 07:29 nucliadb/ingest/consumer/service.py
--rw-r--r--  2.0 unx     4331 b- defN 24-Apr-24 07:29 nucliadb/ingest/consumer/shard_creator.py
--rw-r--r--  2.0 unx     2656 b- defN 24-Apr-24 07:29 nucliadb/ingest/consumer/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-24 07:29 nucliadb/ingest/fields/__init__.py
--rw-r--r--  2.0 unx    18433 b- defN 24-Apr-24 07:29 nucliadb/ingest/fields/base.py
--rw-r--r--  2.0 unx     6516 b- defN 24-Apr-24 07:29 nucliadb/ingest/fields/conversation.py
--rw-r--r--  2.0 unx     1223 b- defN 24-Apr-24 07:29 nucliadb/ingest/fields/date.py
--rw-r--r--  2.0 unx     1205 b- defN 24-Apr-24 07:29 nucliadb/ingest/fields/exceptions.py
--rw-r--r--  2.0 unx     5159 b- defN 24-Apr-24 07:29 nucliadb/ingest/fields/file.py
--rw-r--r--  2.0 unx     1547 b- defN 24-Apr-24 07:29 nucliadb/ingest/fields/generic.py
--rw-r--r--  2.0 unx     1235 b- defN 24-Apr-24 07:29 nucliadb/ingest/fields/keywordset.py
--rw-r--r--  2.0 unx     2250 b- defN 24-Apr-24 07:29 nucliadb/ingest/fields/layout.py
--rw-r--r--  2.0 unx     4084 b- defN 24-Apr-24 07:29 nucliadb/ingest/fields/link.py
--rw-r--r--  2.0 unx     1319 b- defN 24-Apr-24 07:29 nucliadb/ingest/fields/text.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-24 07:29 nucliadb/ingest/orm/__init__.py
--rw-r--r--  2.0 unx    28367 b- defN 24-Apr-24 07:29 nucliadb/ingest/orm/brain.py
--rw-r--r--  2.0 unx    15758 b- defN 24-Apr-24 07:29 nucliadb/ingest/orm/entities.py
--rw-r--r--  2.0 unx     1279 b- defN 24-Apr-24 07:29 nucliadb/ingest/orm/exceptions.py
--rw-r--r--  2.0 unx    18731 b- defN 24-Apr-24 07:29 nucliadb/ingest/orm/knowledgebox.py
--rw-r--r--  2.0 unx     1096 b- defN 24-Apr-24 07:29 nucliadb/ingest/orm/metrics.py
--rw-r--r--  2.0 unx    60647 b- defN 24-Apr-24 07:29 nucliadb/ingest/orm/resource.py
--rw-r--r--  2.0 unx     1739 b- defN 24-Apr-24 07:29 nucliadb/ingest/orm/synonyms.py
--rw-r--r--  2.0 unx     3683 b- defN 24-Apr-24 07:29 nucliadb/ingest/orm/utils.py
--rw-r--r--  2.0 unx    26460 b- defN 24-Apr-24 07:29 nucliadb/ingest/orm/processor/__init__.py
--rw-r--r--  2.0 unx     1690 b- defN 24-Apr-24 07:29 nucliadb/ingest/orm/processor/sequence_manager.py
--rw-r--r--  2.0 unx     2057 b- defN 24-Apr-24 07:29 nucliadb/ingest/service/__init__.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-24 07:29 nucliadb/ingest/service/exceptions.py
--rw-r--r--  2.0 unx    37355 b- defN 24-Apr-24 07:29 nucliadb/ingest/service/writer.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-24 07:29 nucliadb/ingest/tests/__init__.py
--rw-r--r--  2.0 unx     1157 b- defN 24-Apr-24 07:29 nucliadb/ingest/tests/conftest.py
--rw-r--r--  2.0 unx    24068 b- defN 24-Apr-24 07:29 nucliadb/ingest/tests/fixtures.py
--rw-r--r--  2.0 unx    62843 b- defN 24-Apr-24 07:29 nucliadb/ingest/tests/vectors.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-24 07:29 nucliadb/ingest/tests/integration/__init__.py
--rw-r--r--  2.0 unx      833 b- defN 24-Apr-24 07:29 nucliadb/ingest/tests/integration/consumer/__init__.py
--rw-r--r--  2.0 unx     2549 b- defN 24-Apr-24 07:29 nucliadb/ingest/tests/integration/consumer/test_auditing.py
--rw-r--r--  2.0 unx     2591 b- defN 24-Apr-24 07:29 nucliadb/ingest/tests/integration/consumer/test_materializer.py
--rw-r--r--  2.0 unx     4465 b- defN 24-Apr-24 07:29 nucliadb/ingest/tests/integration/consumer/test_pull.py
--rw-r--r--  2.0 unx     2763 b- defN 24-Apr-24 07:29 nucliadb/ingest/tests/integration/consumer/test_service.py
--rw-r--r--  2.0 unx     2019 b- defN 24-Apr-24 07:29 nucliadb/ingest/tests/integration/consumer/test_shard_creator.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-24 07:29 nucliadb/ingest/tests/integration/ingest/__init__.py
--rw-r--r--  2.0 unx    27334 b- defN 24-Apr-24 07:29 nucliadb/ingest/tests/integration/ingest/test_ingest.py
--rw-r--r--  2.0 unx     3040 b- defN 24-Apr-24 07:29 nucliadb/ingest/tests/integration/ingest/test_processing_engine.py
--rw-r--r--  2.0 unx     8586 b- defN 24-Apr-24 07:29 nucliadb/ingest/tests/integration/ingest/test_relations.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-24 07:29 nucliadb/ingest/tests/unit/__init__.py
--rw-r--r--  2.0 unx     1189 b- defN 24-Apr-24 07:29 nucliadb/ingest/tests/unit/test_cache.py
--rw-r--r--  2.0 unx     1432 b- defN 24-Apr-24 07:29 nucliadb/ingest/tests/unit/test_partitions.py
--rw-r--r--  2.0 unx     5807 b- defN 24-Apr-24 07:29 nucliadb/ingest/tests/unit/test_processing.py
--rw-r--r--  2.0 unx      978 b- defN 24-Apr-24 07:29 nucliadb/ingest/tests/unit/test_settings.py
--rw-r--r--  2.0 unx      833 b- defN 24-Apr-24 07:29 nucliadb/ingest/tests/unit/consumer/__init__.py
--rw-r--r--  2.0 unx     3981 b- defN 24-Apr-24 07:29 nucliadb/ingest/tests/unit/consumer/test_auditing.py
--rw-r--r--  2.0 unx     2472 b- defN 24-Apr-24 07:29 nucliadb/ingest/tests/unit/consumer/test_consumer.py
--rw-r--r--  2.0 unx     2063 b- defN 24-Apr-24 07:29 nucliadb/ingest/tests/unit/consumer/test_pull.py
--rw-r--r--  2.0 unx     4075 b- defN 24-Apr-24 07:29 nucliadb/ingest/tests/unit/consumer/test_shard_creator.py
--rw-r--r--  2.0 unx     1934 b- defN 24-Apr-24 07:29 nucliadb/ingest/tests/unit/consumer/test_utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-24 07:29 nucliadb/ingest/tests/unit/orm/__init__.py
--rw-r--r--  2.0 unx     9876 b- defN 24-Apr-24 07:29 nucliadb/ingest/tests/unit/orm/test_brain.py
--rw-r--r--  2.0 unx     2435 b- defN 24-Apr-24 07:29 nucliadb/ingest/tests/unit/orm/test_brain_vectors.py
--rw-r--r--  2.0 unx     1174 b- defN 24-Apr-24 07:29 nucliadb/ingest/tests/unit/orm/test_orm_utils.py
--rw-r--r--  2.0 unx     4045 b- defN 24-Apr-24 07:29 nucliadb/ingest/tests/unit/orm/test_processor.py
--rw-r--r--  2.0 unx    11005 b- defN 24-Apr-24 07:29 nucliadb/ingest/tests/unit/orm/test_resource.py
--rw-r--r--  2.0 unx     2216 b- defN 24-Apr-24 07:29 nucliadb/middleware/__init__.py
--rw-r--r--  2.0 unx     3912 b- defN 24-Apr-24 07:29 nucliadb/middleware/transaction.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-24 07:29 nucliadb/migrator/__init__.py
--rw-r--r--  2.0 unx     2119 b- defN 24-Apr-24 07:29 nucliadb/migrator/command.py
--rw-r--r--  2.0 unx     1334 b- defN 24-Apr-24 07:29 nucliadb/migrator/context.py
--rw-r--r--  2.0 unx     5104 b- defN 24-Apr-24 07:29 nucliadb/migrator/datamanager.py
--rw-r--r--  2.0 unx      889 b- defN 24-Apr-24 07:29 nucliadb/migrator/exceptions.py
--rw-r--r--  2.0 unx     9237 b- defN 24-Apr-24 07:29 nucliadb/migrator/migrator.py
--rw-r--r--  2.0 unx     1145 b- defN 24-Apr-24 07:29 nucliadb/migrator/models.py
--rw-r--r--  2.0 unx     1110 b- defN 24-Apr-24 07:29 nucliadb/migrator/settings.py
--rw-r--r--  2.0 unx     2346 b- defN 24-Apr-24 07:29 nucliadb/migrator/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-24 07:29 nucliadb/models/__init__.py
--rw-r--r--  2.0 unx     1599 b- defN 24-Apr-24 07:29 nucliadb/models/responses.py
--rw-r--r--  2.0 unx     6041 b- defN 24-Apr-24 07:29 nucliadb/purge/__init__.py
--rw-r--r--  2.0 unx     9364 b- defN 24-Apr-24 07:29 nucliadb/purge/orphan_shards.py
--rw-r--r--  2.0 unx     1328 b- defN 24-Apr-24 07:29 nucliadb/reader/__init__.py
--rw-r--r--  2.0 unx     3709 b- defN 24-Apr-24 07:29 nucliadb/reader/app.py
--rw-r--r--  2.0 unx     1366 b- defN 24-Apr-24 07:29 nucliadb/reader/lifecycle.py
--rw-r--r--  2.0 unx     1031 b- defN 24-Apr-24 07:29 nucliadb/reader/openapi.py
--rw-r--r--  2.0 unx     1447 b- defN 24-Apr-24 07:29 nucliadb/reader/run.py
--rw-r--r--  2.0 unx      872 b- defN 24-Apr-24 07:29 nucliadb/reader/api/__init__.py
--rw-r--r--  2.0 unx     2434 b- defN 24-Apr-24 07:29 nucliadb/reader/api/models.py
--rw-r--r--  2.0 unx     1110 b- defN 24-Apr-24 07:29 nucliadb/reader/api/v1/__init__.py
--rw-r--r--  2.0 unx    12368 b- defN 24-Apr-24 07:29 nucliadb/reader/api/v1/download.py
--rw-r--r--  2.0 unx     6450 b- defN 24-Apr-24 07:29 nucliadb/reader/api/v1/export_import.py
--rw-r--r--  2.0 unx     3632 b- defN 24-Apr-24 07:29 nucliadb/reader/api/v1/knowledgebox.py
--rw-r--r--  2.0 unx     2093 b- defN 24-Apr-24 07:29 nucliadb/reader/api/v1/learning_collector.py
--rw-r--r--  2.0 unx     4454 b- defN 24-Apr-24 07:29 nucliadb/reader/api/v1/learning_config.py
--rw-r--r--  2.0 unx    13928 b- defN 24-Apr-24 07:29 nucliadb/reader/api/v1/resource.py
--rw-r--r--  2.0 unx     1011 b- defN 24-Apr-24 07:29 nucliadb/reader/api/v1/router.py
--rw-r--r--  2.0 unx    13882 b- defN 24-Apr-24 07:29 nucliadb/reader/api/v1/services.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-24 07:29 nucliadb/reader/reader/__init__.py
--rw-r--r--  2.0 unx     8155 b- defN 24-Apr-24 07:29 nucliadb/reader/reader/notifications.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-24 07:29 nucliadb/reader/tests/__init__.py
--rw-r--r--  2.0 unx     1224 b- defN 24-Apr-24 07:29 nucliadb/reader/tests/conftest.py
--rw-r--r--  2.0 unx     4345 b- defN 24-Apr-24 07:29 nucliadb/reader/tests/fixtures.py
--rw-r--r--  2.0 unx     2748 b- defN 24-Apr-24 07:29 nucliadb/reader/tests/test_list_resources.py
--rw-r--r--  2.0 unx    10199 b- defN 24-Apr-24 07:29 nucliadb/reader/tests/test_reader_file_download.py
--rw-r--r--  2.0 unx    10586 b- defN 24-Apr-24 07:29 nucliadb/reader/tests/test_reader_resource.py
--rw-r--r--  2.0 unx     6535 b- defN 24-Apr-24 07:29 nucliadb/reader/tests/test_reader_resource_field.py
--rw-r--r--  2.0 unx     1535 b- defN 24-Apr-24 07:29 nucliadb/search/__init__.py
--rw-r--r--  2.0 unx     4905 b- defN 24-Apr-24 07:29 nucliadb/search/app.py
--rw-r--r--  2.0 unx     1956 b- defN 24-Apr-24 07:29 nucliadb/search/lifecycle.py
--rw-r--r--  2.0 unx     1016 b- defN 24-Apr-24 07:29 nucliadb/search/openapi.py
--rw-r--r--  2.0 unx    18535 b- defN 24-Apr-24 07:29 nucliadb/search/predict.py
--rw-r--r--  2.0 unx     1402 b- defN 24-Apr-24 07:29 nucliadb/search/run.py
--rw-r--r--  2.0 unx     1193 b- defN 24-Apr-24 07:29 nucliadb/search/settings.py
--rw-r--r--  2.0 unx     1037 b- defN 24-Apr-24 07:29 nucliadb/search/utilities.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-24 07:29 nucliadb/search/api/__init__.py
--rw-r--r--  2.0 unx     1272 b- defN 24-Apr-24 07:29 nucliadb/search/api/v1/__init__.py
--rw-r--r--  2.0 unx     9913 b- defN 24-Apr-24 07:29 nucliadb/search/api/v1/chat.py
--rw-r--r--  2.0 unx     2665 b- defN 24-Apr-24 07:29 nucliadb/search/api/v1/feedback.py
--rw-r--r--  2.0 unx     8804 b- defN 24-Apr-24 07:29 nucliadb/search/api/v1/find.py
--rw-r--r--  2.0 unx     7026 b- defN 24-Apr-24 07:29 nucliadb/search/api/v1/knowledgebox.py
--rw-r--r--  2.0 unx     3041 b- defN 24-Apr-24 07:29 nucliadb/search/api/v1/predict_proxy.py
--rw-r--r--  2.0 unx      988 b- defN 24-Apr-24 07:29 nucliadb/search/api/v1/router.py
--rw-r--r--  2.0 unx    18359 b- defN 24-Apr-24 07:29 nucliadb/search/api/v1/search.py
--rw-r--r--  2.0 unx     5928 b- defN 24-Apr-24 07:29 nucliadb/search/api/v1/suggest.py
--rw-r--r--  2.0 unx     2536 b- defN 24-Apr-24 07:29 nucliadb/search/api/v1/summarize.py
--rw-r--r--  2.0 unx     1412 b- defN 24-Apr-24 07:29 nucliadb/search/api/v1/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-24 07:29 nucliadb/search/api/v1/resource/__init__.py
--rw-r--r--  2.0 unx     6095 b- defN 24-Apr-24 07:29 nucliadb/search/api/v1/resource/ask.py
--rw-r--r--  2.0 unx     5887 b- defN 24-Apr-24 07:29 nucliadb/search/api/v1/resource/chat.py
--rw-r--r--  2.0 unx     5293 b- defN 24-Apr-24 07:29 nucliadb/search/api/v1/resource/search.py
--rw-r--r--  2.0 unx      833 b- defN 24-Apr-24 07:29 nucliadb/search/requesters/__init__.py
--rw-r--r--  2.0 unx     9070 b- defN 24-Apr-24 07:29 nucliadb/search/requesters/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-24 07:29 nucliadb/search/search/__init__.py
--rw-r--r--  2.0 unx     2746 b- defN 24-Apr-24 07:29 nucliadb/search/search/cache.py
--rw-r--r--  2.0 unx     1154 b- defN 24-Apr-24 07:29 nucliadb/search/search/exceptions.py
--rw-r--r--  2.0 unx     5465 b- defN 24-Apr-24 07:29 nucliadb/search/search/fetch.py
--rw-r--r--  2.0 unx     6513 b- defN 24-Apr-24 07:29 nucliadb/search/search/filters.py
--rw-r--r--  2.0 unx     4646 b- defN 24-Apr-24 07:29 nucliadb/search/search/find.py
--rw-r--r--  2.0 unx    17152 b- defN 24-Apr-24 07:29 nucliadb/search/search/find_merge.py
--rw-r--r--  2.0 unx    21282 b- defN 24-Apr-24 07:29 nucliadb/search/search/merge.py
--rw-r--r--  2.0 unx     1130 b- defN 24-Apr-24 07:29 nucliadb/search/search/metrics.py
--rw-r--r--  2.0 unx     8698 b- defN 24-Apr-24 07:29 nucliadb/search/search/paragraphs.py
--rw-r--r--  2.0 unx     3026 b- defN 24-Apr-24 07:29 nucliadb/search/search/predict_proxy.py
--rw-r--r--  2.0 unx    31300 b- defN 24-Apr-24 07:29 nucliadb/search/search/query.py
--rw-r--r--  2.0 unx     3149 b- defN 24-Apr-24 07:29 nucliadb/search/search/shards.py
--rw-r--r--  2.0 unx     5101 b- defN 24-Apr-24 07:29 nucliadb/search/search/summarize.py
--rw-r--r--  2.0 unx     2438 b- defN 24-Apr-24 07:29 nucliadb/search/search/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-24 07:29 nucliadb/search/search/chat/__init__.py
--rw-r--r--  2.0 unx     2058 b- defN 24-Apr-24 07:29 nucliadb/search/search/chat/images.py
--rw-r--r--  2.0 unx    20793 b- defN 24-Apr-24 07:29 nucliadb/search/search/chat/prompt.py
--rw-r--r--  2.0 unx    15347 b- defN 24-Apr-24 07:29 nucliadb/search/search/chat/query.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-24 07:29 nucliadb/search/tests/__init__.py
--rw-r--r--  2.0 unx     1295 b- defN 24-Apr-24 07:29 nucliadb/search/tests/conftest.py
--rw-r--r--  2.0 unx     6578 b- defN 24-Apr-24 07:29 nucliadb/search/tests/fixtures.py
--rw-r--r--  2.0 unx    15529 b- defN 24-Apr-24 07:29 nucliadb/search/tests/node.py
--rw-r--r--  2.0 unx      833 b- defN 24-Apr-24 07:29 nucliadb/search/tests/unit/__init__.py
--rw-r--r--  2.0 unx     2649 b- defN 24-Apr-24 07:29 nucliadb/search/tests/unit/test_app.py
--rw-r--r--  2.0 unx     3374 b- defN 24-Apr-24 07:29 nucliadb/search/tests/unit/test_find_merge.py
--rw-r--r--  2.0 unx     1400 b- defN 24-Apr-24 07:29 nucliadb/search/tests/unit/test_merge.py
--rw-r--r--  2.0 unx    14729 b- defN 24-Apr-24 07:29 nucliadb/search/tests/unit/test_predict.py
--rw-r--r--  2.0 unx     1317 b- defN 24-Apr-24 07:29 nucliadb/search/tests/unit/test_run.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-24 07:29 nucliadb/search/tests/unit/api/__init__.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-24 07:29 nucliadb/search/tests/unit/api/v1/__init__.py
--rw-r--r--  2.0 unx     2966 b- defN 24-Apr-24 07:29 nucliadb/search/tests/unit/api/v1/test_chat.py
--rw-r--r--  2.0 unx     2865 b- defN 24-Apr-24 07:29 nucliadb/search/tests/unit/api/v1/test_predict_proxy.py
--rw-r--r--  2.0 unx     2901 b- defN 24-Apr-24 07:29 nucliadb/search/tests/unit/api/v1/test_summarize.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-24 07:29 nucliadb/search/tests/unit/api/v1/resource/__init__.py
--rw-r--r--  2.0 unx     2411 b- defN 24-Apr-24 07:29 nucliadb/search/tests/unit/api/v1/resource/test_ask.py
--rw-r--r--  2.0 unx     3040 b- defN 24-Apr-24 07:29 nucliadb/search/tests/unit/api/v1/resource/test_chat.py
--rw-r--r--  2.0 unx      833 b- defN 24-Apr-24 07:29 nucliadb/search/tests/unit/search/__init__.py
--rw-r--r--  2.0 unx     8567 b- defN 24-Apr-24 07:29 nucliadb/search/tests/unit/search/test_chat_prompt.py
--rw-r--r--  2.0 unx     3736 b- defN 24-Apr-24 07:29 nucliadb/search/tests/unit/search/test_fetch.py
--rw-r--r--  2.0 unx     4306 b- defN 24-Apr-24 07:29 nucliadb/search/tests/unit/search/test_filters.py
--rw-r--r--  2.0 unx     4492 b- defN 24-Apr-24 07:29 nucliadb/search/tests/unit/search/test_paragraphs.py
--rw-r--r--  2.0 unx     3496 b- defN 24-Apr-24 07:29 nucliadb/search/tests/unit/search/test_predict_proxy.py
--rw-r--r--  2.0 unx     7001 b- defN 24-Apr-24 07:29 nucliadb/search/tests/unit/search/test_query.py
--rw-r--r--  2.0 unx      833 b- defN 24-Apr-24 07:29 nucliadb/search/tests/unit/search/requesters/__init__.py
--rw-r--r--  2.0 unx     6455 b- defN 24-Apr-24 07:29 nucliadb/search/tests/unit/search/requesters/test_utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-24 07:29 nucliadb/search/tests/unit/search/search/__init__.py
--rw-r--r--  2.0 unx     1759 b- defN 24-Apr-24 07:29 nucliadb/search/tests/unit/search/search/test_shards.py
--rw-r--r--  2.0 unx     2511 b- defN 24-Apr-24 07:29 nucliadb/search/tests/unit/search/search/test_utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-24 07:29 nucliadb/standalone/__init__.py
--rw-r--r--  2.0 unx     6746 b- defN 24-Apr-24 07:29 nucliadb/standalone/api_router.py
--rw-r--r--  2.0 unx     5763 b- defN 24-Apr-24 07:29 nucliadb/standalone/app.py
--rw-r--r--  2.0 unx     7800 b- defN 24-Apr-24 07:29 nucliadb/standalone/auth.py
--rw-r--r--  2.0 unx     5309 b- defN 24-Apr-24 07:29 nucliadb/standalone/config.py
--rw-r--r--  2.0 unx     6930 b- defN 24-Apr-24 07:29 nucliadb/standalone/introspect.py
--rw-r--r--  2.0 unx     2488 b- defN 24-Apr-24 07:29 nucliadb/standalone/lifecycle.py
--rw-r--r--  2.0 unx     1317 b- defN 24-Apr-24 07:29 nucliadb/standalone/purge.py
--rw-r--r--  2.0 unx     5336 b- defN 24-Apr-24 07:29 nucliadb/standalone/run.py
--rw-r--r--  2.0 unx     5781 b- defN 24-Apr-24 07:29 nucliadb/standalone/settings.py
--rw-r--r--  2.0 unx     3132 b- defN 24-Apr-24 07:29 nucliadb/standalone/versions.py
--rw-r--r--  2.0 unx     2285 b- defN 24-Apr-24 07:29 nucliadb/standalone/static/favicon.ico
--rw-r--r--  2.0 unx     3833 b- defN 24-Apr-24 07:29 nucliadb/standalone/static/index.html
--rw-r--r--  2.0 unx     2639 b- defN 24-Apr-24 07:29 nucliadb/standalone/static/logo.svg
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-24 07:29 nucliadb/standalone/tests/__init__.py
--rw-r--r--  2.0 unx     1294 b- defN 24-Apr-24 07:29 nucliadb/standalone/tests/conftest.py
--rw-r--r--  2.0 unx     1319 b- defN 24-Apr-24 07:29 nucliadb/standalone/tests/fixtures.py
--rw-r--r--  2.0 unx      833 b- defN 24-Apr-24 07:29 nucliadb/standalone/tests/unit/__init__.py
--rw-r--r--  2.0 unx     1722 b- defN 24-Apr-24 07:29 nucliadb/standalone/tests/unit/test_api_router.py
--rw-r--r--  2.0 unx     5509 b- defN 24-Apr-24 07:29 nucliadb/standalone/tests/unit/test_auth.py
--rw-r--r--  2.0 unx     1334 b- defN 24-Apr-24 07:29 nucliadb/standalone/tests/unit/test_introspect.py
--rw-r--r--  2.0 unx     1472 b- defN 24-Apr-24 07:29 nucliadb/standalone/tests/unit/test_run.py
--rw-r--r--  2.0 unx     1972 b- defN 24-Apr-24 07:29 nucliadb/standalone/tests/unit/test_versions.py
--rw-r--r--  2.0 unx     1037 b- defN 24-Apr-24 07:29 nucliadb/tasks/__init__.py
--rw-r--r--  2.0 unx     7655 b- defN 24-Apr-24 07:29 nucliadb/tasks/consumer.py
--rw-r--r--  2.0 unx      924 b- defN 24-Apr-24 07:29 nucliadb/tasks/logger.py
--rw-r--r--  2.0 unx     1378 b- defN 24-Apr-24 07:29 nucliadb/tasks/models.py
--rw-r--r--  2.0 unx     3457 b- defN 24-Apr-24 07:29 nucliadb/tasks/producer.py
--rw-r--r--  2.0 unx     1753 b- defN 24-Apr-24 07:29 nucliadb/tasks/registry.py
--rw-r--r--  2.0 unx     1360 b- defN 24-Apr-24 07:29 nucliadb/tasks/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-24 07:29 nucliadb/tests/__init__.py
--rw-r--r--  2.0 unx     1229 b- defN 24-Apr-24 07:29 nucliadb/tests/conftest.py
--rw-r--r--  2.0 unx    22365 b- defN 24-Apr-24 07:29 nucliadb/tests/fixtures.py
--rw-r--r--  2.0 unx     7549 b- defN 24-Apr-24 07:29 nucliadb/tests/tikv.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-24 07:29 nucliadb/tests/benchmarks/__init__.py
--rw-r--r--  2.0 unx     3032 b- defN 24-Apr-24 07:29 nucliadb/tests/benchmarks/test_search.py
--rw-r--r--  2.0 unx      919 b- defN 24-Apr-24 07:29 nucliadb/tests/knowledgeboxes/__init__.py
--rw-r--r--  2.0 unx     7002 b- defN 24-Apr-24 07:29 nucliadb/tests/knowledgeboxes/philosophy_books.py
--rw-r--r--  2.0 unx     3037 b- defN 24-Apr-24 07:29 nucliadb/tests/knowledgeboxes/ten_dummy_resources.py
--rw-r--r--  2.0 unx     1148 b- defN 24-Apr-24 07:29 nucliadb/tests/migrations/__init__.py
--rw-r--r--  2.0 unx     2726 b- defN 24-Apr-24 07:29 nucliadb/tests/migrations/test_migration_0017.py
--rw-r--r--  2.0 unx     3625 b- defN 24-Apr-24 07:29 nucliadb/tests/migrations/test_migration_0018.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-24 07:29 nucliadb/tests/unit/__init__.py
--rw-r--r--  2.0 unx     1487 b- defN 24-Apr-24 07:29 nucliadb/tests/unit/test_field_ids.py
--rw-r--r--  2.0 unx     2758 b- defN 24-Apr-24 07:29 nucliadb/tests/unit/test_health.py
--rw-r--r--  2.0 unx     1543 b- defN 24-Apr-24 07:29 nucliadb/tests/unit/test_kb_slugs.py
--rw-r--r--  2.0 unx     7892 b- defN 24-Apr-24 07:29 nucliadb/tests/unit/test_learning_proxy.py
--rw-r--r--  2.0 unx     2642 b- defN 24-Apr-24 07:29 nucliadb/tests/unit/test_metrics_exporter.py
--rw-r--r--  2.0 unx     1341 b- defN 24-Apr-24 07:29 nucliadb/tests/unit/test_openapi.py
--rw-r--r--  2.0 unx     3656 b- defN 24-Apr-24 07:29 nucliadb/tests/unit/test_purge.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-24 07:29 nucliadb/tests/unit/common/__init__.py
--rw-r--r--  2.0 unx     1268 b- defN 24-Apr-24 07:29 nucliadb/tests/unit/common/test_context.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-24 07:29 nucliadb/tests/unit/common/cluster/__init__.py
--rw-r--r--  2.0 unx    11955 b- defN 24-Apr-24 07:29 nucliadb/tests/unit/common/cluster/test_cluster.py
--rw-r--r--  2.0 unx     5387 b- defN 24-Apr-24 07:29 nucliadb/tests/unit/common/cluster/test_kb_shard_manager.py
--rw-r--r--  2.0 unx     9470 b- defN 24-Apr-24 07:29 nucliadb/tests/unit/common/cluster/test_rollover.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-24 07:29 nucliadb/tests/unit/common/cluster/discovery/__init__.py
--rw-r--r--  2.0 unx     5584 b- defN 24-Apr-24 07:29 nucliadb/tests/unit/common/cluster/discovery/test_k8s.py
--rw-r--r--  2.0 unx      833 b- defN 24-Apr-24 07:29 nucliadb/tests/unit/common/cluster/standalone/__init__.py
--rw-r--r--  2.0 unx     3750 b- defN 24-Apr-24 07:29 nucliadb/tests/unit/common/cluster/standalone/test_service.py
--rw-r--r--  2.0 unx     2114 b- defN 24-Apr-24 07:29 nucliadb/tests/unit/common/cluster/standalone/test_utils.py
--rw-r--r--  2.0 unx      833 b- defN 24-Apr-24 07:29 nucliadb/tests/unit/common/maindb/__init__.py
--rw-r--r--  2.0 unx     3579 b- defN 24-Apr-24 07:29 nucliadb/tests/unit/common/maindb/test_driver.py
--rw-r--r--  2.0 unx     1869 b- defN 24-Apr-24 07:29 nucliadb/tests/unit/common/maindb/test_tikv.py
--rw-r--r--  2.0 unx     2998 b- defN 24-Apr-24 07:29 nucliadb/tests/unit/common/maindb/test_utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-24 07:29 nucliadb/tests/unit/export_import/__init__.py
--rw-r--r--  2.0 unx     1435 b- defN 24-Apr-24 07:29 nucliadb/tests/unit/export_import/test_datamanager.py
--rw-r--r--  2.0 unx     9706 b- defN 24-Apr-24 07:29 nucliadb/tests/unit/export_import/test_utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-24 07:29 nucliadb/tests/unit/migrator/__init__.py
--rw-r--r--  2.0 unx     3233 b- defN 24-Apr-24 07:29 nucliadb/tests/unit/migrator/test_migrator.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-24 07:29 nucliadb/tests/unit/tasks/__init__.py
--rw-r--r--  2.0 unx     1375 b- defN 24-Apr-24 07:29 nucliadb/tests/unit/tasks/conftest.py
--rw-r--r--  2.0 unx     2714 b- defN 24-Apr-24 07:29 nucliadb/tests/unit/tasks/test_consumer.py
--rw-r--r--  2.0 unx     3189 b- defN 24-Apr-24 07:29 nucliadb/tests/unit/tasks/test_producer.py
--rw-r--r--  2.0 unx     1827 b- defN 24-Apr-24 07:29 nucliadb/tests/unit/tasks/test_tasks.py
--rw-r--r--  2.0 unx     2507 b- defN 24-Apr-24 07:29 nucliadb/tests/utils/__init__.py
--rw-r--r--  2.0 unx     1797 b- defN 24-Apr-24 07:29 nucliadb/tests/utils/aiohttp_session.py
--rw-r--r--  2.0 unx     2533 b- defN 24-Apr-24 07:29 nucliadb/tests/utils/entities.py
--rw-r--r--  2.0 unx     6327 b- defN 24-Apr-24 07:29 nucliadb/tests/utils/broker_messages/__init__.py
--rw-r--r--  2.0 unx     7557 b- defN 24-Apr-24 07:29 nucliadb/tests/utils/broker_messages/fields.py
--rw-r--r--  2.0 unx     1196 b- defN 24-Apr-24 07:29 nucliadb/tests/utils/broker_messages/helpers.py
--rw-r--r--  2.0 unx     1325 b- defN 24-Apr-24 07:29 nucliadb/train/__init__.py
--rw-r--r--  2.0 unx     3530 b- defN 24-Apr-24 07:29 nucliadb/train/app.py
--rw-r--r--  2.0 unx     3800 b- defN 24-Apr-24 07:29 nucliadb/train/generator.py
--rw-r--r--  2.0 unx     1698 b- defN 24-Apr-24 07:29 nucliadb/train/lifecycle.py
--rw-r--r--  2.0 unx     1198 b- defN 24-Apr-24 07:29 nucliadb/train/models.py
--rw-r--r--  2.0 unx     5706 b- defN 24-Apr-24 07:29 nucliadb/train/nodes.py
--rw-r--r--  2.0 unx     1400 b- defN 24-Apr-24 07:29 nucliadb/train/run.py
--rw-r--r--  2.0 unx     5926 b- defN 24-Apr-24 07:29 nucliadb/train/servicer.py
--rw-r--r--  2.0 unx     1415 b- defN 24-Apr-24 07:29 nucliadb/train/settings.py
--rw-r--r--  2.0 unx     1496 b- defN 24-Apr-24 07:29 nucliadb/train/types.py
--rw-r--r--  2.0 unx     3265 b- defN 24-Apr-24 07:29 nucliadb/train/upload.py
--rw-r--r--  2.0 unx     6420 b- defN 24-Apr-24 07:29 nucliadb/train/uploader.py
--rw-r--r--  2.0 unx     3179 b- defN 24-Apr-24 07:29 nucliadb/train/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-24 07:29 nucliadb/train/api/__init__.py
--rw-r--r--  2.0 unx     1479 b- defN 24-Apr-24 07:29 nucliadb/train/api/utils.py
--rw-r--r--  2.0 unx      928 b- defN 24-Apr-24 07:29 nucliadb/train/api/v1/__init__.py
--rw-r--r--  2.0 unx     2065 b- defN 24-Apr-24 07:29 nucliadb/train/api/v1/check.py
--rw-r--r--  2.0 unx      910 b- defN 24-Apr-24 07:29 nucliadb/train/api/v1/router.py
--rw-r--r--  2.0 unx     1905 b- defN 24-Apr-24 07:29 nucliadb/train/api/v1/shards.py
--rw-r--r--  2.0 unx     2129 b- defN 24-Apr-24 07:29 nucliadb/train/api/v1/trainset.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-24 07:29 nucliadb/train/generators/__init__.py
--rw-r--r--  2.0 unx     3723 b- defN 24-Apr-24 07:29 nucliadb/train/generators/field_classifier.py
--rw-r--r--  2.0 unx     6712 b- defN 24-Apr-24 07:29 nucliadb/train/generators/image_classifier.py
--rw-r--r--  2.0 unx     2789 b- defN 24-Apr-24 07:29 nucliadb/train/generators/paragraph_classifier.py
--rw-r--r--  2.0 unx     3590 b- defN 24-Apr-24 07:29 nucliadb/train/generators/paragraph_streaming.py
--rw-r--r--  2.0 unx     5372 b- defN 24-Apr-24 07:29 nucliadb/train/generators/question_answer_streaming.py
--rw-r--r--  2.0 unx     5160 b- defN 24-Apr-24 07:29 nucliadb/train/generators/sentence_classifier.py
--rw-r--r--  2.0 unx    10446 b- defN 24-Apr-24 07:29 nucliadb/train/generators/token_classifier.py
--rw-r--r--  2.0 unx     3877 b- defN 24-Apr-24 07:29 nucliadb/train/generators/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-24 07:29 nucliadb/train/tests/__init__.py
--rw-r--r--  2.0 unx     1125 b- defN 24-Apr-24 07:29 nucliadb/train/tests/conftest.py
--rw-r--r--  2.0 unx    11053 b- defN 24-Apr-24 07:29 nucliadb/train/tests/fixtures.py
--rw-r--r--  2.0 unx     4598 b- defN 24-Apr-24 07:29 nucliadb/train/tests/test_field_classification.py
--rw-r--r--  2.0 unx     2729 b- defN 24-Apr-24 07:29 nucliadb/train/tests/test_get_entities.py
--rw-r--r--  2.0 unx     1876 b- defN 24-Apr-24 07:29 nucliadb/train/tests/test_get_info.py
--rw-r--r--  2.0 unx     1382 b- defN 24-Apr-24 07:29 nucliadb/train/tests/test_get_ontology.py
--rw-r--r--  2.0 unx     2417 b- defN 24-Apr-24 07:29 nucliadb/train/tests/test_get_ontology_count.py
--rw-r--r--  2.0 unx     7669 b- defN 24-Apr-24 07:29 nucliadb/train/tests/test_image_classification.py
--rw-r--r--  2.0 unx     1416 b- defN 24-Apr-24 07:29 nucliadb/train/tests/test_list_fields.py
--rw-r--r--  2.0 unx     2944 b- defN 24-Apr-24 07:29 nucliadb/train/tests/test_list_paragraphs.py
--rw-r--r--  2.0 unx     1423 b- defN 24-Apr-24 07:29 nucliadb/train/tests/test_list_resources.py
--rw-r--r--  2.0 unx     2947 b- defN 24-Apr-24 07:29 nucliadb/train/tests/test_list_sentences.py
--rw-r--r--  2.0 unx     4645 b- defN 24-Apr-24 07:29 nucliadb/train/tests/test_paragraph_classification.py
--rw-r--r--  2.0 unx     4320 b- defN 24-Apr-24 07:29 nucliadb/train/tests/test_paragraph_streaming.py
--rw-r--r--  2.0 unx     8751 b- defN 24-Apr-24 07:29 nucliadb/train/tests/test_question_answer_streaming.py
--rw-r--r--  2.0 unx     5051 b- defN 24-Apr-24 07:29 nucliadb/train/tests/test_sentence_classification.py
--rw-r--r--  2.0 unx     5583 b- defN 24-Apr-24 07:29 nucliadb/train/tests/test_token_classification.py
--rw-r--r--  2.0 unx     3324 b- defN 24-Apr-24 07:29 nucliadb/train/tests/utils.py
--rw-r--r--  2.0 unx     1328 b- defN 24-Apr-24 07:29 nucliadb/writer/__init__.py
--rw-r--r--  2.0 unx     4268 b- defN 24-Apr-24 07:29 nucliadb/writer/app.py
--rw-r--r--  2.0 unx    19495 b- defN 24-Apr-24 07:29 nucliadb/writer/back_pressure.py
--rw-r--r--  2.0 unx      972 b- defN 24-Apr-24 07:29 nucliadb/writer/exceptions.py
--rw-r--r--  2.0 unx     1953 b- defN 24-Apr-24 07:29 nucliadb/writer/lifecycle.py
--rw-r--r--  2.0 unx     1032 b- defN 24-Apr-24 07:29 nucliadb/writer/openapi.py
--rw-r--r--  2.0 unx     1448 b- defN 24-Apr-24 07:29 nucliadb/writer/run.py
--rw-r--r--  2.0 unx     3074 b- defN 24-Apr-24 07:29 nucliadb/writer/settings.py
--rw-r--r--  2.0 unx     1036 b- defN 24-Apr-24 07:29 nucliadb/writer/utilities.py
--rw-r--r--  2.0 unx     1948 b- defN 24-Apr-24 07:29 nucliadb/writer/vectors.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-24 07:29 nucliadb/writer/api/__init__.py
--rw-r--r--  2.0 unx     1429 b- defN 24-Apr-24 07:29 nucliadb/writer/api/constants.py
--rw-r--r--  2.0 unx     1095 b- defN 24-Apr-24 07:29 nucliadb/writer/api/v1/__init__.py
--rw-r--r--  2.0 unx     6565 b- defN 24-Apr-24 07:29 nucliadb/writer/api/v1/export_import.py
--rw-r--r--  2.0 unx    28578 b- defN 24-Apr-24 07:29 nucliadb/writer/api/v1/field.py
--rw-r--r--  2.0 unx     5239 b- defN 24-Apr-24 07:29 nucliadb/writer/api/v1/knowledgebox.py
--rw-r--r--  2.0 unx     2052 b- defN 24-Apr-24 07:29 nucliadb/writer/api/v1/learning_config.py
--rw-r--r--  2.0 unx    19940 b- defN 24-Apr-24 07:29 nucliadb/writer/api/v1/resource.py
--rw-r--r--  2.0 unx     1034 b- defN 24-Apr-24 07:29 nucliadb/writer/api/v1/router.py
--rw-r--r--  2.0 unx    12733 b- defN 24-Apr-24 07:29 nucliadb/writer/api/v1/services.py
--rw-r--r--  2.0 unx    31592 b- defN 24-Apr-24 07:29 nucliadb/writer/api/v1/upload.py
--rw-r--r--  2.0 unx     1612 b- defN 24-Apr-24 07:29 nucliadb/writer/layouts/__init__.py
--rw-r--r--  2.0 unx     2115 b- defN 24-Apr-24 07:29 nucliadb/writer/layouts/v1.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-24 07:29 nucliadb/writer/resource/__init__.py
--rw-r--r--  2.0 unx     1425 b- defN 24-Apr-24 07:29 nucliadb/writer/resource/audit.py
--rw-r--r--  2.0 unx    10968 b- defN 24-Apr-24 07:29 nucliadb/writer/resource/basic.py
--rw-r--r--  2.0 unx    16319 b- defN 24-Apr-24 07:29 nucliadb/writer/resource/field.py
--rw-r--r--  2.0 unx     2022 b- defN 24-Apr-24 07:29 nucliadb/writer/resource/origin.py
--rw-r--r--  2.0 unx     1152 b- defN 24-Apr-24 07:29 nucliadb/writer/resource/slug.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-24 07:29 nucliadb/writer/tests/__init__.py
--rw-r--r--  2.0 unx     1200 b- defN 24-Apr-24 07:29 nucliadb/writer/tests/conftest.py
--rw-r--r--  2.0 unx     5971 b- defN 24-Apr-24 07:29 nucliadb/writer/tests/fixtures.py
--rw-r--r--  2.0 unx    15472 b- defN 24-Apr-24 07:29 nucliadb/writer/tests/test_fields.py
--rw-r--r--  2.0 unx    25913 b- defN 24-Apr-24 07:29 nucliadb/writer/tests/test_files.py
--rw-r--r--  2.0 unx     1729 b- defN 24-Apr-24 07:29 nucliadb/writer/tests/test_knowledgebox.py
--rw-r--r--  2.0 unx     4569 b- defN 24-Apr-24 07:29 nucliadb/writer/tests/test_reprocess_file_field.py
--rw-r--r--  2.0 unx    17449 b- defN 24-Apr-24 07:29 nucliadb/writer/tests/test_resources.py
--rw-r--r--  2.0 unx     5120 b- defN 24-Apr-24 07:29 nucliadb/writer/tests/test_service.py
--rw-r--r--  2.0 unx     6054 b- defN 24-Apr-24 07:29 nucliadb/writer/tests/test_tus.py
--rw-r--r--  2.0 unx     1287 b- defN 24-Apr-24 07:29 nucliadb/writer/tests/utils.py
--rw-r--r--  2.0 unx     5226 b- defN 24-Apr-24 07:29 nucliadb/writer/tus/__init__.py
--rw-r--r--  2.0 unx     5082 b- defN 24-Apr-24 07:29 nucliadb/writer/tus/dm.py
--rw-r--r--  2.0 unx     2186 b- defN 24-Apr-24 07:29 nucliadb/writer/tus/exceptions.py
--rw-r--r--  2.0 unx    14527 b- defN 24-Apr-24 07:29 nucliadb/writer/tus/gcs.py
--rw-r--r--  2.0 unx     5849 b- defN 24-Apr-24 07:29 nucliadb/writer/tus/local.py
--rw-r--r--  2.0 unx     4367 b- defN 24-Apr-24 07:29 nucliadb/writer/tus/pg.py
--rw-r--r--  2.0 unx     9069 b- defN 24-Apr-24 07:29 nucliadb/writer/tus/s3.py
--rw-r--r--  2.0 unx     4734 b- defN 24-Apr-24 07:29 nucliadb/writer/tus/storage.py
--rw-r--r--  2.0 unx     2556 b- defN 24-Apr-24 07:29 nucliadb/writer/tus/utils.py
--rw-r--r--  2.0 unx     4343 b- defN 24-Apr-24 07:30 nucliadb-3.0.3.post450.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-24 07:30 nucliadb-3.0.3.post450.dist-info/WHEEL
--rw-r--r--  2.0 unx     1268 b- defN 24-Apr-24 07:30 nucliadb-3.0.3.post450.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       20 b- defN 24-Apr-24 07:30 nucliadb-3.0.3.post450.dist-info/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 24-Apr-24 07:30 nucliadb-3.0.3.post450.dist-info/zip-safe
--rw-rw-r--  2.0 unx    42761 b- defN 24-Apr-24 07:30 nucliadb-3.0.3.post450.dist-info/RECORD
-456 files, 2242380 bytes uncompressed, 686046 bytes compressed:  69.4%
+Zip file size: 752643 bytes, number of entries: 455
+-rw-r--r--  2.0 unx     1135 b- defN 24-Apr-25 10:10 migrations/0001_bootstrap.py
+-rw-r--r--  2.0 unx     1177 b- defN 24-Apr-25 10:10 migrations/0002_rollover_shards.py
+-rw-r--r--  2.0 unx     2436 b- defN 24-Apr-25 10:10 migrations/0003_allfields_key.py
+-rw-r--r--  2.0 unx     1177 b- defN 24-Apr-25 10:10 migrations/0004_rollover_shards.py
+-rw-r--r--  2.0 unx     1177 b- defN 24-Apr-25 10:10 migrations/0005_rollover_shards.py
+-rw-r--r--  2.0 unx     1024 b- defN 24-Apr-25 10:10 migrations/0006_rollover_shards.py
+-rw-r--r--  2.0 unx     1301 b- defN 24-Apr-25 10:10 migrations/0008_cleanup_leftover_rollover_metadata.py
+-rw-r--r--  2.0 unx     1378 b- defN 24-Apr-25 10:10 migrations/0009_upgrade_relations_and_texts_to_v2.py
+-rw-r--r--  2.0 unx     1610 b- defN 24-Apr-25 10:10 migrations/0010_fix_corrupt_indexes.py
+-rw-r--r--  2.0 unx     1843 b- defN 24-Apr-25 10:10 migrations/0011_materialize_labelset_ids.py
+-rw-r--r--  2.0 unx     1443 b- defN 24-Apr-25 10:10 migrations/0012_rollover_shards.py
+-rw-r--r--  2.0 unx     1024 b- defN 24-Apr-25 10:10 migrations/0013_rollover_shards.py
+-rw-r--r--  2.0 unx     1382 b- defN 24-Apr-25 10:10 migrations/0014_rollover_shards.py
+-rw-r--r--  2.0 unx     1462 b- defN 24-Apr-25 10:10 migrations/0015_targeted_rollover.py
+-rw-r--r--  2.0 unx     2506 b- defN 24-Apr-25 10:10 migrations/0016_upgrade_to_paragraphs_v2.py
+-rw-r--r--  2.0 unx     2100 b- defN 24-Apr-25 10:10 migrations/0017_multiple_writable_shards.py
+-rw-r--r--  2.0 unx     2264 b- defN 24-Apr-25 10:10 migrations/0018_purge_orphan_kbslugs.py
+-rw-r--r--  2.0 unx     2506 b- defN 24-Apr-25 10:10 migrations/0019_upgrade_to_paragraphs_v3.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-25 10:10 migrations/__init__.py
+-rw-r--r--  2.0 unx      891 b- defN 24-Apr-25 10:10 nucliadb/__init__.py
+-rw-r--r--  2.0 unx     3733 b- defN 24-Apr-25 10:10 nucliadb/health.py
+-rw-r--r--  2.0 unx    11626 b- defN 24-Apr-25 10:10 nucliadb/learning_proxy.py
+-rw-r--r--  2.0 unx     4806 b- defN 24-Apr-25 10:10 nucliadb/metrics_exporter.py
+-rw-r--r--  2.0 unx     2272 b- defN 24-Apr-25 10:10 nucliadb/openapi.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-25 10:10 nucliadb/py.typed
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-25 10:10 nucliadb/common/__init__.py
+-rw-r--r--  2.0 unx     4905 b- defN 24-Apr-25 10:10 nucliadb/common/locking.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-25 10:10 nucliadb/common/cluster/__init__.py
+-rw-r--r--  2.0 unx     4971 b- defN 24-Apr-25 10:10 nucliadb/common/cluster/base.py
+-rw-r--r--  2.0 unx     1495 b- defN 24-Apr-25 10:10 nucliadb/common/cluster/exceptions.py
+-rw-r--r--  2.0 unx     3658 b- defN 24-Apr-25 10:10 nucliadb/common/cluster/grpc_node_dummy.py
+-rw-r--r--  2.0 unx     3429 b- defN 24-Apr-25 10:10 nucliadb/common/cluster/index_node.py
+-rw-r--r--  2.0 unx    21231 b- defN 24-Apr-25 10:10 nucliadb/common/cluster/manager.py
+-rw-r--r--  2.0 unx     8490 b- defN 24-Apr-25 10:10 nucliadb/common/cluster/rebalance.py
+-rw-r--r--  2.0 unx    19593 b- defN 24-Apr-25 10:10 nucliadb/common/cluster/rollover.py
+-rw-r--r--  2.0 unx     2713 b- defN 24-Apr-25 10:10 nucliadb/common/cluster/settings.py
+-rw-r--r--  2.0 unx     5494 b- defN 24-Apr-25 10:10 nucliadb/common/cluster/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-25 10:10 nucliadb/common/cluster/discovery/__init__.py
+-rw-r--r--  2.0 unx     6553 b- defN 24-Apr-25 10:10 nucliadb/common/cluster/discovery/base.py
+-rw-r--r--  2.0 unx    12518 b- defN 24-Apr-25 10:10 nucliadb/common/cluster/discovery/k8s.py
+-rw-r--r--  2.0 unx     1957 b- defN 24-Apr-25 10:10 nucliadb/common/cluster/discovery/manual.py
+-rw-r--r--  2.0 unx     1737 b- defN 24-Apr-25 10:10 nucliadb/common/cluster/discovery/single.py
+-rw-r--r--  2.0 unx     1139 b- defN 24-Apr-25 10:10 nucliadb/common/cluster/discovery/types.py
+-rw-r--r--  2.0 unx     2548 b- defN 24-Apr-25 10:10 nucliadb/common/cluster/discovery/utils.py
+-rw-r--r--  2.0 unx      833 b- defN 24-Apr-25 10:10 nucliadb/common/cluster/standalone/__init__.py
+-rw-r--r--  2.0 unx    13707 b- defN 24-Apr-25 10:10 nucliadb/common/cluster/standalone/grpc_node_binding.py
+-rw-r--r--  2.0 unx     4683 b- defN 24-Apr-25 10:10 nucliadb/common/cluster/standalone/index_node.py
+-rw-r--r--  2.0 unx     3444 b- defN 24-Apr-25 10:10 nucliadb/common/cluster/standalone/service.py
+-rw-r--r--  2.0 unx     3386 b- defN 24-Apr-25 10:10 nucliadb/common/cluster/standalone/utils.py
+-rw-r--r--  2.0 unx     3498 b- defN 24-Apr-25 10:10 nucliadb/common/context/__init__.py
+-rw-r--r--  2.0 unx     1628 b- defN 24-Apr-25 10:10 nucliadb/common/context/fastapi.py
+-rw-r--r--  2.0 unx     1813 b- defN 24-Apr-25 10:10 nucliadb/common/datamanagers/__init__.py
+-rw-r--r--  2.0 unx     1451 b- defN 24-Apr-25 10:10 nucliadb/common/datamanagers/cluster.py
+-rw-r--r--  2.0 unx     5383 b- defN 24-Apr-25 10:10 nucliadb/common/datamanagers/entities.py
+-rw-r--r--  2.0 unx      883 b- defN 24-Apr-25 10:10 nucliadb/common/datamanagers/exceptions.py
+-rw-r--r--  2.0 unx     3994 b- defN 24-Apr-25 10:10 nucliadb/common/datamanagers/kb.py
+-rw-r--r--  2.0 unx     5389 b- defN 24-Apr-25 10:10 nucliadb/common/datamanagers/labels.py
+-rw-r--r--  2.0 unx     1599 b- defN 24-Apr-25 10:10 nucliadb/common/datamanagers/processing.py
+-rw-r--r--  2.0 unx     7637 b- defN 24-Apr-25 10:10 nucliadb/common/datamanagers/resources.py
+-rw-r--r--  2.0 unx     5633 b- defN 24-Apr-25 10:10 nucliadb/common/datamanagers/rollover.py
+-rw-r--r--  2.0 unx     1681 b- defN 24-Apr-25 10:10 nucliadb/common/datamanagers/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-25 10:10 nucliadb/common/http_clients/__init__.py
+-rw-r--r--  2.0 unx     2146 b- defN 24-Apr-25 10:10 nucliadb/common/http_clients/auth.py
+-rw-r--r--  2.0 unx     1100 b- defN 24-Apr-25 10:10 nucliadb/common/http_clients/exceptions.py
+-rw-r--r--  2.0 unx     7155 b- defN 24-Apr-25 10:10 nucliadb/common/http_clients/processing.py
+-rw-r--r--  2.0 unx     1540 b- defN 24-Apr-25 10:10 nucliadb/common/http_clients/pypi.py
+-rw-r--r--  2.0 unx     1551 b- defN 24-Apr-25 10:10 nucliadb/common/http_clients/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-25 10:10 nucliadb/common/maindb/__init__.py
+-rw-r--r--  2.0 unx     3449 b- defN 24-Apr-25 10:10 nucliadb/common/maindb/driver.py
+-rw-r--r--  2.0 unx      946 b- defN 24-Apr-25 10:10 nucliadb/common/maindb/exceptions.py
+-rw-r--r--  2.0 unx     6769 b- defN 24-Apr-25 10:10 nucliadb/common/maindb/local.py
+-rw-r--r--  2.0 unx     8391 b- defN 24-Apr-25 10:10 nucliadb/common/maindb/pg.py
+-rw-r--r--  2.0 unx     6053 b- defN 24-Apr-25 10:10 nucliadb/common/maindb/redis.py
+-rw-r--r--  2.0 unx    14502 b- defN 24-Apr-25 10:10 nucliadb/common/maindb/tikv.py
+-rw-r--r--  2.0 unx     4109 b- defN 24-Apr-25 10:10 nucliadb/common/maindb/utils.py
+-rw-r--r--  2.0 unx      932 b- defN 24-Apr-25 10:10 nucliadb/export_import/__init__.py
+-rw-r--r--  2.0 unx     6171 b- defN 24-Apr-25 10:10 nucliadb/export_import/datamanager.py
+-rw-r--r--  2.0 unx     1949 b- defN 24-Apr-25 10:10 nucliadb/export_import/exceptions.py
+-rw-r--r--  2.0 unx     7116 b- defN 24-Apr-25 10:10 nucliadb/export_import/exporter.py
+-rw-r--r--  2.0 unx     4258 b- defN 24-Apr-25 10:10 nucliadb/export_import/importer.py
+-rw-r--r--  2.0 unx     2063 b- defN 24-Apr-25 10:10 nucliadb/export_import/models.py
+-rw-r--r--  2.0 unx     2571 b- defN 24-Apr-25 10:10 nucliadb/export_import/tasks.py
+-rw-r--r--  2.0 unx    19270 b- defN 24-Apr-25 10:10 nucliadb/export_import/utils.py
+-rw-r--r--  2.0 unx     1011 b- defN 24-Apr-25 10:10 nucliadb/ingest/__init__.py
+-rw-r--r--  2.0 unx     7277 b- defN 24-Apr-25 10:10 nucliadb/ingest/app.py
+-rw-r--r--  2.0 unx     1005 b- defN 24-Apr-25 10:10 nucliadb/ingest/cache.py
+-rw-r--r--  2.0 unx     2484 b- defN 24-Apr-25 10:10 nucliadb/ingest/partitions.py
+-rw-r--r--  2.0 unx    19541 b- defN 24-Apr-25 10:10 nucliadb/ingest/processing.py
+-rw-r--r--  2.0 unx    20277 b- defN 24-Apr-25 10:10 nucliadb/ingest/serialize.py
+-rw-r--r--  2.0 unx     3183 b- defN 24-Apr-25 10:10 nucliadb/ingest/settings.py
+-rw-r--r--  2.0 unx     2314 b- defN 24-Apr-25 10:10 nucliadb/ingest/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-25 10:10 nucliadb/ingest/consumer/__init__.py
+-rw-r--r--  2.0 unx    11563 b- defN 24-Apr-25 10:10 nucliadb/ingest/consumer/auditing.py
+-rw-r--r--  2.0 unx    12159 b- defN 24-Apr-25 10:10 nucliadb/ingest/consumer/consumer.py
+-rw-r--r--  2.0 unx     3788 b- defN 24-Apr-25 10:10 nucliadb/ingest/consumer/materializer.py
+-rw-r--r--  2.0 unx     1075 b- defN 24-Apr-25 10:10 nucliadb/ingest/consumer/metrics.py
+-rw-r--r--  2.0 unx     9543 b- defN 24-Apr-25 10:10 nucliadb/ingest/consumer/pull.py
+-rw-r--r--  2.0 unx     6935 b- defN 24-Apr-25 10:10 nucliadb/ingest/consumer/service.py
+-rw-r--r--  2.0 unx     4331 b- defN 24-Apr-25 10:10 nucliadb/ingest/consumer/shard_creator.py
+-rw-r--r--  2.0 unx     2656 b- defN 24-Apr-25 10:10 nucliadb/ingest/consumer/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-25 10:10 nucliadb/ingest/fields/__init__.py
+-rw-r--r--  2.0 unx    18433 b- defN 24-Apr-25 10:10 nucliadb/ingest/fields/base.py
+-rw-r--r--  2.0 unx     6516 b- defN 24-Apr-25 10:10 nucliadb/ingest/fields/conversation.py
+-rw-r--r--  2.0 unx     1223 b- defN 24-Apr-25 10:10 nucliadb/ingest/fields/date.py
+-rw-r--r--  2.0 unx     1205 b- defN 24-Apr-25 10:10 nucliadb/ingest/fields/exceptions.py
+-rw-r--r--  2.0 unx     5159 b- defN 24-Apr-25 10:10 nucliadb/ingest/fields/file.py
+-rw-r--r--  2.0 unx     1547 b- defN 24-Apr-25 10:10 nucliadb/ingest/fields/generic.py
+-rw-r--r--  2.0 unx     1235 b- defN 24-Apr-25 10:10 nucliadb/ingest/fields/keywordset.py
+-rw-r--r--  2.0 unx     2250 b- defN 24-Apr-25 10:10 nucliadb/ingest/fields/layout.py
+-rw-r--r--  2.0 unx     4084 b- defN 24-Apr-25 10:10 nucliadb/ingest/fields/link.py
+-rw-r--r--  2.0 unx     1319 b- defN 24-Apr-25 10:10 nucliadb/ingest/fields/text.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-25 10:10 nucliadb/ingest/orm/__init__.py
+-rw-r--r--  2.0 unx    28367 b- defN 24-Apr-25 10:10 nucliadb/ingest/orm/brain.py
+-rw-r--r--  2.0 unx    15758 b- defN 24-Apr-25 10:10 nucliadb/ingest/orm/entities.py
+-rw-r--r--  2.0 unx     1279 b- defN 24-Apr-25 10:10 nucliadb/ingest/orm/exceptions.py
+-rw-r--r--  2.0 unx    17684 b- defN 24-Apr-25 10:10 nucliadb/ingest/orm/knowledgebox.py
+-rw-r--r--  2.0 unx     1096 b- defN 24-Apr-25 10:10 nucliadb/ingest/orm/metrics.py
+-rw-r--r--  2.0 unx    60647 b- defN 24-Apr-25 10:10 nucliadb/ingest/orm/resource.py
+-rw-r--r--  2.0 unx     1739 b- defN 24-Apr-25 10:10 nucliadb/ingest/orm/synonyms.py
+-rw-r--r--  2.0 unx     3683 b- defN 24-Apr-25 10:10 nucliadb/ingest/orm/utils.py
+-rw-r--r--  2.0 unx    26460 b- defN 24-Apr-25 10:10 nucliadb/ingest/orm/processor/__init__.py
+-rw-r--r--  2.0 unx     1690 b- defN 24-Apr-25 10:10 nucliadb/ingest/orm/processor/sequence_manager.py
+-rw-r--r--  2.0 unx     2057 b- defN 24-Apr-25 10:10 nucliadb/ingest/service/__init__.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-25 10:10 nucliadb/ingest/service/exceptions.py
+-rw-r--r--  2.0 unx    35455 b- defN 24-Apr-25 10:10 nucliadb/ingest/service/writer.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-25 10:10 nucliadb/ingest/tests/__init__.py
+-rw-r--r--  2.0 unx     1157 b- defN 24-Apr-25 10:10 nucliadb/ingest/tests/conftest.py
+-rw-r--r--  2.0 unx    24068 b- defN 24-Apr-25 10:10 nucliadb/ingest/tests/fixtures.py
+-rw-r--r--  2.0 unx    62843 b- defN 24-Apr-25 10:10 nucliadb/ingest/tests/vectors.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-25 10:10 nucliadb/ingest/tests/integration/__init__.py
+-rw-r--r--  2.0 unx      833 b- defN 24-Apr-25 10:10 nucliadb/ingest/tests/integration/consumer/__init__.py
+-rw-r--r--  2.0 unx     2549 b- defN 24-Apr-25 10:10 nucliadb/ingest/tests/integration/consumer/test_auditing.py
+-rw-r--r--  2.0 unx     2591 b- defN 24-Apr-25 10:10 nucliadb/ingest/tests/integration/consumer/test_materializer.py
+-rw-r--r--  2.0 unx     4465 b- defN 24-Apr-25 10:10 nucliadb/ingest/tests/integration/consumer/test_pull.py
+-rw-r--r--  2.0 unx     2763 b- defN 24-Apr-25 10:10 nucliadb/ingest/tests/integration/consumer/test_service.py
+-rw-r--r--  2.0 unx     2019 b- defN 24-Apr-25 10:10 nucliadb/ingest/tests/integration/consumer/test_shard_creator.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-25 10:10 nucliadb/ingest/tests/integration/ingest/__init__.py
+-rw-r--r--  2.0 unx    27334 b- defN 24-Apr-25 10:10 nucliadb/ingest/tests/integration/ingest/test_ingest.py
+-rw-r--r--  2.0 unx     3040 b- defN 24-Apr-25 10:10 nucliadb/ingest/tests/integration/ingest/test_processing_engine.py
+-rw-r--r--  2.0 unx     8586 b- defN 24-Apr-25 10:10 nucliadb/ingest/tests/integration/ingest/test_relations.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-25 10:10 nucliadb/ingest/tests/unit/__init__.py
+-rw-r--r--  2.0 unx     1189 b- defN 24-Apr-25 10:10 nucliadb/ingest/tests/unit/test_cache.py
+-rw-r--r--  2.0 unx     1432 b- defN 24-Apr-25 10:10 nucliadb/ingest/tests/unit/test_partitions.py
+-rw-r--r--  2.0 unx     5807 b- defN 24-Apr-25 10:10 nucliadb/ingest/tests/unit/test_processing.py
+-rw-r--r--  2.0 unx      978 b- defN 24-Apr-25 10:10 nucliadb/ingest/tests/unit/test_settings.py
+-rw-r--r--  2.0 unx      833 b- defN 24-Apr-25 10:10 nucliadb/ingest/tests/unit/consumer/__init__.py
+-rw-r--r--  2.0 unx     3981 b- defN 24-Apr-25 10:10 nucliadb/ingest/tests/unit/consumer/test_auditing.py
+-rw-r--r--  2.0 unx     2472 b- defN 24-Apr-25 10:10 nucliadb/ingest/tests/unit/consumer/test_consumer.py
+-rw-r--r--  2.0 unx     2063 b- defN 24-Apr-25 10:10 nucliadb/ingest/tests/unit/consumer/test_pull.py
+-rw-r--r--  2.0 unx     4075 b- defN 24-Apr-25 10:10 nucliadb/ingest/tests/unit/consumer/test_shard_creator.py
+-rw-r--r--  2.0 unx     1934 b- defN 24-Apr-25 10:10 nucliadb/ingest/tests/unit/consumer/test_utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-25 10:10 nucliadb/ingest/tests/unit/orm/__init__.py
+-rw-r--r--  2.0 unx     9876 b- defN 24-Apr-25 10:10 nucliadb/ingest/tests/unit/orm/test_brain.py
+-rw-r--r--  2.0 unx     2435 b- defN 24-Apr-25 10:10 nucliadb/ingest/tests/unit/orm/test_brain_vectors.py
+-rw-r--r--  2.0 unx     1174 b- defN 24-Apr-25 10:10 nucliadb/ingest/tests/unit/orm/test_orm_utils.py
+-rw-r--r--  2.0 unx     4045 b- defN 24-Apr-25 10:10 nucliadb/ingest/tests/unit/orm/test_processor.py
+-rw-r--r--  2.0 unx    11005 b- defN 24-Apr-25 10:10 nucliadb/ingest/tests/unit/orm/test_resource.py
+-rw-r--r--  2.0 unx     2216 b- defN 24-Apr-25 10:10 nucliadb/middleware/__init__.py
+-rw-r--r--  2.0 unx     3912 b- defN 24-Apr-25 10:10 nucliadb/middleware/transaction.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-25 10:10 nucliadb/migrator/__init__.py
+-rw-r--r--  2.0 unx     2119 b- defN 24-Apr-25 10:10 nucliadb/migrator/command.py
+-rw-r--r--  2.0 unx     1334 b- defN 24-Apr-25 10:10 nucliadb/migrator/context.py
+-rw-r--r--  2.0 unx     5104 b- defN 24-Apr-25 10:10 nucliadb/migrator/datamanager.py
+-rw-r--r--  2.0 unx      889 b- defN 24-Apr-25 10:10 nucliadb/migrator/exceptions.py
+-rw-r--r--  2.0 unx     9237 b- defN 24-Apr-25 10:10 nucliadb/migrator/migrator.py
+-rw-r--r--  2.0 unx     1145 b- defN 24-Apr-25 10:10 nucliadb/migrator/models.py
+-rw-r--r--  2.0 unx     1110 b- defN 24-Apr-25 10:10 nucliadb/migrator/settings.py
+-rw-r--r--  2.0 unx     2346 b- defN 24-Apr-25 10:10 nucliadb/migrator/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-25 10:10 nucliadb/models/__init__.py
+-rw-r--r--  2.0 unx     1599 b- defN 24-Apr-25 10:10 nucliadb/models/responses.py
+-rw-r--r--  2.0 unx     6041 b- defN 24-Apr-25 10:10 nucliadb/purge/__init__.py
+-rw-r--r--  2.0 unx     9364 b- defN 24-Apr-25 10:10 nucliadb/purge/orphan_shards.py
+-rw-r--r--  2.0 unx     1328 b- defN 24-Apr-25 10:10 nucliadb/reader/__init__.py
+-rw-r--r--  2.0 unx     3709 b- defN 24-Apr-25 10:10 nucliadb/reader/app.py
+-rw-r--r--  2.0 unx     1366 b- defN 24-Apr-25 10:10 nucliadb/reader/lifecycle.py
+-rw-r--r--  2.0 unx     1031 b- defN 24-Apr-25 10:10 nucliadb/reader/openapi.py
+-rw-r--r--  2.0 unx     1447 b- defN 24-Apr-25 10:10 nucliadb/reader/run.py
+-rw-r--r--  2.0 unx      872 b- defN 24-Apr-25 10:10 nucliadb/reader/api/__init__.py
+-rw-r--r--  2.0 unx     2434 b- defN 24-Apr-25 10:10 nucliadb/reader/api/models.py
+-rw-r--r--  2.0 unx     1110 b- defN 24-Apr-25 10:10 nucliadb/reader/api/v1/__init__.py
+-rw-r--r--  2.0 unx    12368 b- defN 24-Apr-25 10:10 nucliadb/reader/api/v1/download.py
+-rw-r--r--  2.0 unx     6450 b- defN 24-Apr-25 10:10 nucliadb/reader/api/v1/export_import.py
+-rw-r--r--  2.0 unx     3632 b- defN 24-Apr-25 10:10 nucliadb/reader/api/v1/knowledgebox.py
+-rw-r--r--  2.0 unx     2093 b- defN 24-Apr-25 10:10 nucliadb/reader/api/v1/learning_collector.py
+-rw-r--r--  2.0 unx     4454 b- defN 24-Apr-25 10:10 nucliadb/reader/api/v1/learning_config.py
+-rw-r--r--  2.0 unx    13928 b- defN 24-Apr-25 10:10 nucliadb/reader/api/v1/resource.py
+-rw-r--r--  2.0 unx     1011 b- defN 24-Apr-25 10:10 nucliadb/reader/api/v1/router.py
+-rw-r--r--  2.0 unx    12378 b- defN 24-Apr-25 10:10 nucliadb/reader/api/v1/services.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-25 10:10 nucliadb/reader/reader/__init__.py
+-rw-r--r--  2.0 unx     8155 b- defN 24-Apr-25 10:10 nucliadb/reader/reader/notifications.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-25 10:10 nucliadb/reader/tests/__init__.py
+-rw-r--r--  2.0 unx     1224 b- defN 24-Apr-25 10:10 nucliadb/reader/tests/conftest.py
+-rw-r--r--  2.0 unx     4345 b- defN 24-Apr-25 10:10 nucliadb/reader/tests/fixtures.py
+-rw-r--r--  2.0 unx     2748 b- defN 24-Apr-25 10:10 nucliadb/reader/tests/test_list_resources.py
+-rw-r--r--  2.0 unx    10199 b- defN 24-Apr-25 10:10 nucliadb/reader/tests/test_reader_file_download.py
+-rw-r--r--  2.0 unx    10586 b- defN 24-Apr-25 10:10 nucliadb/reader/tests/test_reader_resource.py
+-rw-r--r--  2.0 unx     6535 b- defN 24-Apr-25 10:10 nucliadb/reader/tests/test_reader_resource_field.py
+-rw-r--r--  2.0 unx     1535 b- defN 24-Apr-25 10:10 nucliadb/search/__init__.py
+-rw-r--r--  2.0 unx     4905 b- defN 24-Apr-25 10:10 nucliadb/search/app.py
+-rw-r--r--  2.0 unx     1956 b- defN 24-Apr-25 10:10 nucliadb/search/lifecycle.py
+-rw-r--r--  2.0 unx     1016 b- defN 24-Apr-25 10:10 nucliadb/search/openapi.py
+-rw-r--r--  2.0 unx    18535 b- defN 24-Apr-25 10:10 nucliadb/search/predict.py
+-rw-r--r--  2.0 unx     1402 b- defN 24-Apr-25 10:10 nucliadb/search/run.py
+-rw-r--r--  2.0 unx     1193 b- defN 24-Apr-25 10:10 nucliadb/search/settings.py
+-rw-r--r--  2.0 unx     1037 b- defN 24-Apr-25 10:10 nucliadb/search/utilities.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-25 10:10 nucliadb/search/api/__init__.py
+-rw-r--r--  2.0 unx     1272 b- defN 24-Apr-25 10:10 nucliadb/search/api/v1/__init__.py
+-rw-r--r--  2.0 unx     9913 b- defN 24-Apr-25 10:10 nucliadb/search/api/v1/chat.py
+-rw-r--r--  2.0 unx     2665 b- defN 24-Apr-25 10:10 nucliadb/search/api/v1/feedback.py
+-rw-r--r--  2.0 unx     8804 b- defN 24-Apr-25 10:10 nucliadb/search/api/v1/find.py
+-rw-r--r--  2.0 unx     6938 b- defN 24-Apr-25 10:10 nucliadb/search/api/v1/knowledgebox.py
+-rw-r--r--  2.0 unx     3041 b- defN 24-Apr-25 10:10 nucliadb/search/api/v1/predict_proxy.py
+-rw-r--r--  2.0 unx      988 b- defN 24-Apr-25 10:10 nucliadb/search/api/v1/router.py
+-rw-r--r--  2.0 unx    18325 b- defN 24-Apr-25 10:10 nucliadb/search/api/v1/search.py
+-rw-r--r--  2.0 unx     5928 b- defN 24-Apr-25 10:10 nucliadb/search/api/v1/suggest.py
+-rw-r--r--  2.0 unx     2536 b- defN 24-Apr-25 10:10 nucliadb/search/api/v1/summarize.py
+-rw-r--r--  2.0 unx     1412 b- defN 24-Apr-25 10:10 nucliadb/search/api/v1/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-25 10:10 nucliadb/search/api/v1/resource/__init__.py
+-rw-r--r--  2.0 unx     6095 b- defN 24-Apr-25 10:10 nucliadb/search/api/v1/resource/ask.py
+-rw-r--r--  2.0 unx     5887 b- defN 24-Apr-25 10:10 nucliadb/search/api/v1/resource/chat.py
+-rw-r--r--  2.0 unx     5293 b- defN 24-Apr-25 10:10 nucliadb/search/api/v1/resource/search.py
+-rw-r--r--  2.0 unx      833 b- defN 24-Apr-25 10:10 nucliadb/search/requesters/__init__.py
+-rw-r--r--  2.0 unx     9070 b- defN 24-Apr-25 10:10 nucliadb/search/requesters/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-25 10:10 nucliadb/search/search/__init__.py
+-rw-r--r--  2.0 unx     2746 b- defN 24-Apr-25 10:10 nucliadb/search/search/cache.py
+-rw-r--r--  2.0 unx     1154 b- defN 24-Apr-25 10:10 nucliadb/search/search/exceptions.py
+-rw-r--r--  2.0 unx     5465 b- defN 24-Apr-25 10:10 nucliadb/search/search/fetch.py
+-rw-r--r--  2.0 unx     6513 b- defN 24-Apr-25 10:10 nucliadb/search/search/filters.py
+-rw-r--r--  2.0 unx     4612 b- defN 24-Apr-25 10:10 nucliadb/search/search/find.py
+-rw-r--r--  2.0 unx    17152 b- defN 24-Apr-25 10:10 nucliadb/search/search/find_merge.py
+-rw-r--r--  2.0 unx    21282 b- defN 24-Apr-25 10:10 nucliadb/search/search/merge.py
+-rw-r--r--  2.0 unx     1130 b- defN 24-Apr-25 10:10 nucliadb/search/search/metrics.py
+-rw-r--r--  2.0 unx     8698 b- defN 24-Apr-25 10:10 nucliadb/search/search/paragraphs.py
+-rw-r--r--  2.0 unx     3026 b- defN 24-Apr-25 10:10 nucliadb/search/search/predict_proxy.py
+-rw-r--r--  2.0 unx    31084 b- defN 24-Apr-25 10:10 nucliadb/search/search/query.py
+-rw-r--r--  2.0 unx     3018 b- defN 24-Apr-25 10:10 nucliadb/search/search/shards.py
+-rw-r--r--  2.0 unx     5101 b- defN 24-Apr-25 10:10 nucliadb/search/search/summarize.py
+-rw-r--r--  2.0 unx     2438 b- defN 24-Apr-25 10:10 nucliadb/search/search/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-25 10:10 nucliadb/search/search/chat/__init__.py
+-rw-r--r--  2.0 unx     2058 b- defN 24-Apr-25 10:10 nucliadb/search/search/chat/images.py
+-rw-r--r--  2.0 unx    20793 b- defN 24-Apr-25 10:10 nucliadb/search/search/chat/prompt.py
+-rw-r--r--  2.0 unx    15347 b- defN 24-Apr-25 10:10 nucliadb/search/search/chat/query.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-25 10:10 nucliadb/search/tests/__init__.py
+-rw-r--r--  2.0 unx     1295 b- defN 24-Apr-25 10:10 nucliadb/search/tests/conftest.py
+-rw-r--r--  2.0 unx     6578 b- defN 24-Apr-25 10:10 nucliadb/search/tests/fixtures.py
+-rw-r--r--  2.0 unx    15529 b- defN 24-Apr-25 10:10 nucliadb/search/tests/node.py
+-rw-r--r--  2.0 unx      833 b- defN 24-Apr-25 10:10 nucliadb/search/tests/unit/__init__.py
+-rw-r--r--  2.0 unx     2649 b- defN 24-Apr-25 10:10 nucliadb/search/tests/unit/test_app.py
+-rw-r--r--  2.0 unx     3374 b- defN 24-Apr-25 10:10 nucliadb/search/tests/unit/test_find_merge.py
+-rw-r--r--  2.0 unx     1400 b- defN 24-Apr-25 10:10 nucliadb/search/tests/unit/test_merge.py
+-rw-r--r--  2.0 unx    14729 b- defN 24-Apr-25 10:10 nucliadb/search/tests/unit/test_predict.py
+-rw-r--r--  2.0 unx     1317 b- defN 24-Apr-25 10:10 nucliadb/search/tests/unit/test_run.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-25 10:10 nucliadb/search/tests/unit/api/__init__.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-25 10:10 nucliadb/search/tests/unit/api/v1/__init__.py
+-rw-r--r--  2.0 unx     2966 b- defN 24-Apr-25 10:10 nucliadb/search/tests/unit/api/v1/test_chat.py
+-rw-r--r--  2.0 unx     2865 b- defN 24-Apr-25 10:10 nucliadb/search/tests/unit/api/v1/test_predict_proxy.py
+-rw-r--r--  2.0 unx     2901 b- defN 24-Apr-25 10:10 nucliadb/search/tests/unit/api/v1/test_summarize.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-25 10:10 nucliadb/search/tests/unit/api/v1/resource/__init__.py
+-rw-r--r--  2.0 unx     2411 b- defN 24-Apr-25 10:10 nucliadb/search/tests/unit/api/v1/resource/test_ask.py
+-rw-r--r--  2.0 unx     3040 b- defN 24-Apr-25 10:10 nucliadb/search/tests/unit/api/v1/resource/test_chat.py
+-rw-r--r--  2.0 unx      833 b- defN 24-Apr-25 10:10 nucliadb/search/tests/unit/search/__init__.py
+-rw-r--r--  2.0 unx     8567 b- defN 24-Apr-25 10:10 nucliadb/search/tests/unit/search/test_chat_prompt.py
+-rw-r--r--  2.0 unx     3736 b- defN 24-Apr-25 10:10 nucliadb/search/tests/unit/search/test_fetch.py
+-rw-r--r--  2.0 unx     4306 b- defN 24-Apr-25 10:10 nucliadb/search/tests/unit/search/test_filters.py
+-rw-r--r--  2.0 unx     4492 b- defN 24-Apr-25 10:10 nucliadb/search/tests/unit/search/test_paragraphs.py
+-rw-r--r--  2.0 unx     3496 b- defN 24-Apr-25 10:10 nucliadb/search/tests/unit/search/test_predict_proxy.py
+-rw-r--r--  2.0 unx     7001 b- defN 24-Apr-25 10:10 nucliadb/search/tests/unit/search/test_query.py
+-rw-r--r--  2.0 unx      833 b- defN 24-Apr-25 10:10 nucliadb/search/tests/unit/search/requesters/__init__.py
+-rw-r--r--  2.0 unx     6455 b- defN 24-Apr-25 10:10 nucliadb/search/tests/unit/search/requesters/test_utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-25 10:10 nucliadb/search/tests/unit/search/search/__init__.py
+-rw-r--r--  2.0 unx     1759 b- defN 24-Apr-25 10:10 nucliadb/search/tests/unit/search/search/test_shards.py
+-rw-r--r--  2.0 unx     2511 b- defN 24-Apr-25 10:10 nucliadb/search/tests/unit/search/search/test_utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-25 10:10 nucliadb/standalone/__init__.py
+-rw-r--r--  2.0 unx     6746 b- defN 24-Apr-25 10:10 nucliadb/standalone/api_router.py
+-rw-r--r--  2.0 unx     5763 b- defN 24-Apr-25 10:10 nucliadb/standalone/app.py
+-rw-r--r--  2.0 unx     7800 b- defN 24-Apr-25 10:10 nucliadb/standalone/auth.py
+-rw-r--r--  2.0 unx     5309 b- defN 24-Apr-25 10:10 nucliadb/standalone/config.py
+-rw-r--r--  2.0 unx     6930 b- defN 24-Apr-25 10:10 nucliadb/standalone/introspect.py
+-rw-r--r--  2.0 unx     2488 b- defN 24-Apr-25 10:10 nucliadb/standalone/lifecycle.py
+-rw-r--r--  2.0 unx     1317 b- defN 24-Apr-25 10:10 nucliadb/standalone/purge.py
+-rw-r--r--  2.0 unx     5336 b- defN 24-Apr-25 10:10 nucliadb/standalone/run.py
+-rw-r--r--  2.0 unx     5781 b- defN 24-Apr-25 10:10 nucliadb/standalone/settings.py
+-rw-r--r--  2.0 unx     3132 b- defN 24-Apr-25 10:10 nucliadb/standalone/versions.py
+-rw-r--r--  2.0 unx     2285 b- defN 24-Apr-25 10:10 nucliadb/standalone/static/favicon.ico
+-rw-r--r--  2.0 unx     3833 b- defN 24-Apr-25 10:10 nucliadb/standalone/static/index.html
+-rw-r--r--  2.0 unx     2639 b- defN 24-Apr-25 10:10 nucliadb/standalone/static/logo.svg
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-25 10:10 nucliadb/standalone/tests/__init__.py
+-rw-r--r--  2.0 unx     1294 b- defN 24-Apr-25 10:10 nucliadb/standalone/tests/conftest.py
+-rw-r--r--  2.0 unx     1319 b- defN 24-Apr-25 10:10 nucliadb/standalone/tests/fixtures.py
+-rw-r--r--  2.0 unx      833 b- defN 24-Apr-25 10:10 nucliadb/standalone/tests/unit/__init__.py
+-rw-r--r--  2.0 unx     1722 b- defN 24-Apr-25 10:10 nucliadb/standalone/tests/unit/test_api_router.py
+-rw-r--r--  2.0 unx     5509 b- defN 24-Apr-25 10:10 nucliadb/standalone/tests/unit/test_auth.py
+-rw-r--r--  2.0 unx     1334 b- defN 24-Apr-25 10:10 nucliadb/standalone/tests/unit/test_introspect.py
+-rw-r--r--  2.0 unx     1472 b- defN 24-Apr-25 10:10 nucliadb/standalone/tests/unit/test_run.py
+-rw-r--r--  2.0 unx     1972 b- defN 24-Apr-25 10:10 nucliadb/standalone/tests/unit/test_versions.py
+-rw-r--r--  2.0 unx     1037 b- defN 24-Apr-25 10:10 nucliadb/tasks/__init__.py
+-rw-r--r--  2.0 unx     7655 b- defN 24-Apr-25 10:10 nucliadb/tasks/consumer.py
+-rw-r--r--  2.0 unx      924 b- defN 24-Apr-25 10:10 nucliadb/tasks/logger.py
+-rw-r--r--  2.0 unx     1378 b- defN 24-Apr-25 10:10 nucliadb/tasks/models.py
+-rw-r--r--  2.0 unx     3457 b- defN 24-Apr-25 10:10 nucliadb/tasks/producer.py
+-rw-r--r--  2.0 unx     1753 b- defN 24-Apr-25 10:10 nucliadb/tasks/registry.py
+-rw-r--r--  2.0 unx     1360 b- defN 24-Apr-25 10:10 nucliadb/tasks/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-25 10:10 nucliadb/tests/__init__.py
+-rw-r--r--  2.0 unx     1229 b- defN 24-Apr-25 10:10 nucliadb/tests/conftest.py
+-rw-r--r--  2.0 unx    22365 b- defN 24-Apr-25 10:10 nucliadb/tests/fixtures.py
+-rw-r--r--  2.0 unx     7549 b- defN 24-Apr-25 10:10 nucliadb/tests/tikv.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-25 10:10 nucliadb/tests/benchmarks/__init__.py
+-rw-r--r--  2.0 unx     3032 b- defN 24-Apr-25 10:10 nucliadb/tests/benchmarks/test_search.py
+-rw-r--r--  2.0 unx      919 b- defN 24-Apr-25 10:10 nucliadb/tests/knowledgeboxes/__init__.py
+-rw-r--r--  2.0 unx     7002 b- defN 24-Apr-25 10:10 nucliadb/tests/knowledgeboxes/philosophy_books.py
+-rw-r--r--  2.0 unx     3037 b- defN 24-Apr-25 10:10 nucliadb/tests/knowledgeboxes/ten_dummy_resources.py
+-rw-r--r--  2.0 unx     1148 b- defN 24-Apr-25 10:10 nucliadb/tests/migrations/__init__.py
+-rw-r--r--  2.0 unx     2726 b- defN 24-Apr-25 10:10 nucliadb/tests/migrations/test_migration_0017.py
+-rw-r--r--  2.0 unx     3625 b- defN 24-Apr-25 10:10 nucliadb/tests/migrations/test_migration_0018.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-25 10:10 nucliadb/tests/unit/__init__.py
+-rw-r--r--  2.0 unx     1487 b- defN 24-Apr-25 10:10 nucliadb/tests/unit/test_field_ids.py
+-rw-r--r--  2.0 unx     2758 b- defN 24-Apr-25 10:10 nucliadb/tests/unit/test_health.py
+-rw-r--r--  2.0 unx     1543 b- defN 24-Apr-25 10:10 nucliadb/tests/unit/test_kb_slugs.py
+-rw-r--r--  2.0 unx     7892 b- defN 24-Apr-25 10:10 nucliadb/tests/unit/test_learning_proxy.py
+-rw-r--r--  2.0 unx     2642 b- defN 24-Apr-25 10:10 nucliadb/tests/unit/test_metrics_exporter.py
+-rw-r--r--  2.0 unx     1341 b- defN 24-Apr-25 10:10 nucliadb/tests/unit/test_openapi.py
+-rw-r--r--  2.0 unx     3656 b- defN 24-Apr-25 10:10 nucliadb/tests/unit/test_purge.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-25 10:10 nucliadb/tests/unit/common/__init__.py
+-rw-r--r--  2.0 unx     1268 b- defN 24-Apr-25 10:10 nucliadb/tests/unit/common/test_context.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-25 10:10 nucliadb/tests/unit/common/cluster/__init__.py
+-rw-r--r--  2.0 unx    11955 b- defN 24-Apr-25 10:10 nucliadb/tests/unit/common/cluster/test_cluster.py
+-rw-r--r--  2.0 unx     5387 b- defN 24-Apr-25 10:10 nucliadb/tests/unit/common/cluster/test_kb_shard_manager.py
+-rw-r--r--  2.0 unx     9470 b- defN 24-Apr-25 10:10 nucliadb/tests/unit/common/cluster/test_rollover.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-25 10:10 nucliadb/tests/unit/common/cluster/discovery/__init__.py
+-rw-r--r--  2.0 unx     5584 b- defN 24-Apr-25 10:10 nucliadb/tests/unit/common/cluster/discovery/test_k8s.py
+-rw-r--r--  2.0 unx      833 b- defN 24-Apr-25 10:10 nucliadb/tests/unit/common/cluster/standalone/__init__.py
+-rw-r--r--  2.0 unx     3750 b- defN 24-Apr-25 10:10 nucliadb/tests/unit/common/cluster/standalone/test_service.py
+-rw-r--r--  2.0 unx     2114 b- defN 24-Apr-25 10:10 nucliadb/tests/unit/common/cluster/standalone/test_utils.py
+-rw-r--r--  2.0 unx      833 b- defN 24-Apr-25 10:10 nucliadb/tests/unit/common/maindb/__init__.py
+-rw-r--r--  2.0 unx     3579 b- defN 24-Apr-25 10:10 nucliadb/tests/unit/common/maindb/test_driver.py
+-rw-r--r--  2.0 unx     1869 b- defN 24-Apr-25 10:10 nucliadb/tests/unit/common/maindb/test_tikv.py
+-rw-r--r--  2.0 unx     2998 b- defN 24-Apr-25 10:10 nucliadb/tests/unit/common/maindb/test_utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-25 10:10 nucliadb/tests/unit/export_import/__init__.py
+-rw-r--r--  2.0 unx     1435 b- defN 24-Apr-25 10:10 nucliadb/tests/unit/export_import/test_datamanager.py
+-rw-r--r--  2.0 unx     9706 b- defN 24-Apr-25 10:10 nucliadb/tests/unit/export_import/test_utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-25 10:10 nucliadb/tests/unit/migrator/__init__.py
+-rw-r--r--  2.0 unx     3233 b- defN 24-Apr-25 10:10 nucliadb/tests/unit/migrator/test_migrator.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-25 10:10 nucliadb/tests/unit/tasks/__init__.py
+-rw-r--r--  2.0 unx     1375 b- defN 24-Apr-25 10:10 nucliadb/tests/unit/tasks/conftest.py
+-rw-r--r--  2.0 unx     2714 b- defN 24-Apr-25 10:10 nucliadb/tests/unit/tasks/test_consumer.py
+-rw-r--r--  2.0 unx     3189 b- defN 24-Apr-25 10:10 nucliadb/tests/unit/tasks/test_producer.py
+-rw-r--r--  2.0 unx     1827 b- defN 24-Apr-25 10:10 nucliadb/tests/unit/tasks/test_tasks.py
+-rw-r--r--  2.0 unx     2507 b- defN 24-Apr-25 10:10 nucliadb/tests/utils/__init__.py
+-rw-r--r--  2.0 unx     1797 b- defN 24-Apr-25 10:10 nucliadb/tests/utils/aiohttp_session.py
+-rw-r--r--  2.0 unx     2533 b- defN 24-Apr-25 10:10 nucliadb/tests/utils/entities.py
+-rw-r--r--  2.0 unx     6327 b- defN 24-Apr-25 10:10 nucliadb/tests/utils/broker_messages/__init__.py
+-rw-r--r--  2.0 unx     7557 b- defN 24-Apr-25 10:10 nucliadb/tests/utils/broker_messages/fields.py
+-rw-r--r--  2.0 unx     1196 b- defN 24-Apr-25 10:10 nucliadb/tests/utils/broker_messages/helpers.py
+-rw-r--r--  2.0 unx     1325 b- defN 24-Apr-25 10:10 nucliadb/train/__init__.py
+-rw-r--r--  2.0 unx     3530 b- defN 24-Apr-25 10:10 nucliadb/train/app.py
+-rw-r--r--  2.0 unx     3800 b- defN 24-Apr-25 10:10 nucliadb/train/generator.py
+-rw-r--r--  2.0 unx     1698 b- defN 24-Apr-25 10:10 nucliadb/train/lifecycle.py
+-rw-r--r--  2.0 unx     1198 b- defN 24-Apr-25 10:10 nucliadb/train/models.py
+-rw-r--r--  2.0 unx     5706 b- defN 24-Apr-25 10:10 nucliadb/train/nodes.py
+-rw-r--r--  2.0 unx     1400 b- defN 24-Apr-25 10:10 nucliadb/train/run.py
+-rw-r--r--  2.0 unx     5926 b- defN 24-Apr-25 10:10 nucliadb/train/servicer.py
+-rw-r--r--  2.0 unx     1415 b- defN 24-Apr-25 10:10 nucliadb/train/settings.py
+-rw-r--r--  2.0 unx     1496 b- defN 24-Apr-25 10:10 nucliadb/train/types.py
+-rw-r--r--  2.0 unx     3265 b- defN 24-Apr-25 10:10 nucliadb/train/upload.py
+-rw-r--r--  2.0 unx     6420 b- defN 24-Apr-25 10:10 nucliadb/train/uploader.py
+-rw-r--r--  2.0 unx     3179 b- defN 24-Apr-25 10:10 nucliadb/train/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-25 10:10 nucliadb/train/api/__init__.py
+-rw-r--r--  2.0 unx     1479 b- defN 24-Apr-25 10:10 nucliadb/train/api/utils.py
+-rw-r--r--  2.0 unx      928 b- defN 24-Apr-25 10:10 nucliadb/train/api/v1/__init__.py
+-rw-r--r--  2.0 unx     2065 b- defN 24-Apr-25 10:10 nucliadb/train/api/v1/check.py
+-rw-r--r--  2.0 unx      910 b- defN 24-Apr-25 10:10 nucliadb/train/api/v1/router.py
+-rw-r--r--  2.0 unx     1905 b- defN 24-Apr-25 10:10 nucliadb/train/api/v1/shards.py
+-rw-r--r--  2.0 unx     2129 b- defN 24-Apr-25 10:10 nucliadb/train/api/v1/trainset.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-25 10:10 nucliadb/train/generators/__init__.py
+-rw-r--r--  2.0 unx     3723 b- defN 24-Apr-25 10:10 nucliadb/train/generators/field_classifier.py
+-rw-r--r--  2.0 unx     6712 b- defN 24-Apr-25 10:10 nucliadb/train/generators/image_classifier.py
+-rw-r--r--  2.0 unx     2789 b- defN 24-Apr-25 10:10 nucliadb/train/generators/paragraph_classifier.py
+-rw-r--r--  2.0 unx     3590 b- defN 24-Apr-25 10:10 nucliadb/train/generators/paragraph_streaming.py
+-rw-r--r--  2.0 unx     5372 b- defN 24-Apr-25 10:10 nucliadb/train/generators/question_answer_streaming.py
+-rw-r--r--  2.0 unx     5160 b- defN 24-Apr-25 10:10 nucliadb/train/generators/sentence_classifier.py
+-rw-r--r--  2.0 unx    10446 b- defN 24-Apr-25 10:10 nucliadb/train/generators/token_classifier.py
+-rw-r--r--  2.0 unx     3877 b- defN 24-Apr-25 10:10 nucliadb/train/generators/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-25 10:10 nucliadb/train/tests/__init__.py
+-rw-r--r--  2.0 unx     1125 b- defN 24-Apr-25 10:10 nucliadb/train/tests/conftest.py
+-rw-r--r--  2.0 unx    11053 b- defN 24-Apr-25 10:10 nucliadb/train/tests/fixtures.py
+-rw-r--r--  2.0 unx     4598 b- defN 24-Apr-25 10:10 nucliadb/train/tests/test_field_classification.py
+-rw-r--r--  2.0 unx     2729 b- defN 24-Apr-25 10:10 nucliadb/train/tests/test_get_entities.py
+-rw-r--r--  2.0 unx     1876 b- defN 24-Apr-25 10:10 nucliadb/train/tests/test_get_info.py
+-rw-r--r--  2.0 unx     1382 b- defN 24-Apr-25 10:10 nucliadb/train/tests/test_get_ontology.py
+-rw-r--r--  2.0 unx     2417 b- defN 24-Apr-25 10:10 nucliadb/train/tests/test_get_ontology_count.py
+-rw-r--r--  2.0 unx     7669 b- defN 24-Apr-25 10:10 nucliadb/train/tests/test_image_classification.py
+-rw-r--r--  2.0 unx     1416 b- defN 24-Apr-25 10:10 nucliadb/train/tests/test_list_fields.py
+-rw-r--r--  2.0 unx     2944 b- defN 24-Apr-25 10:10 nucliadb/train/tests/test_list_paragraphs.py
+-rw-r--r--  2.0 unx     1423 b- defN 24-Apr-25 10:10 nucliadb/train/tests/test_list_resources.py
+-rw-r--r--  2.0 unx     2947 b- defN 24-Apr-25 10:10 nucliadb/train/tests/test_list_sentences.py
+-rw-r--r--  2.0 unx     4645 b- defN 24-Apr-25 10:10 nucliadb/train/tests/test_paragraph_classification.py
+-rw-r--r--  2.0 unx     4320 b- defN 24-Apr-25 10:10 nucliadb/train/tests/test_paragraph_streaming.py
+-rw-r--r--  2.0 unx     8751 b- defN 24-Apr-25 10:10 nucliadb/train/tests/test_question_answer_streaming.py
+-rw-r--r--  2.0 unx     5051 b- defN 24-Apr-25 10:10 nucliadb/train/tests/test_sentence_classification.py
+-rw-r--r--  2.0 unx     5583 b- defN 24-Apr-25 10:10 nucliadb/train/tests/test_token_classification.py
+-rw-r--r--  2.0 unx     3324 b- defN 24-Apr-25 10:10 nucliadb/train/tests/utils.py
+-rw-r--r--  2.0 unx     1328 b- defN 24-Apr-25 10:10 nucliadb/writer/__init__.py
+-rw-r--r--  2.0 unx     4268 b- defN 24-Apr-25 10:10 nucliadb/writer/app.py
+-rw-r--r--  2.0 unx    19495 b- defN 24-Apr-25 10:10 nucliadb/writer/back_pressure.py
+-rw-r--r--  2.0 unx      972 b- defN 24-Apr-25 10:10 nucliadb/writer/exceptions.py
+-rw-r--r--  2.0 unx     1953 b- defN 24-Apr-25 10:10 nucliadb/writer/lifecycle.py
+-rw-r--r--  2.0 unx     1032 b- defN 24-Apr-25 10:10 nucliadb/writer/openapi.py
+-rw-r--r--  2.0 unx     1448 b- defN 24-Apr-25 10:10 nucliadb/writer/run.py
+-rw-r--r--  2.0 unx     3074 b- defN 24-Apr-25 10:10 nucliadb/writer/settings.py
+-rw-r--r--  2.0 unx     1036 b- defN 24-Apr-25 10:10 nucliadb/writer/utilities.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-25 10:10 nucliadb/writer/api/__init__.py
+-rw-r--r--  2.0 unx     1429 b- defN 24-Apr-25 10:10 nucliadb/writer/api/constants.py
+-rw-r--r--  2.0 unx     1095 b- defN 24-Apr-25 10:10 nucliadb/writer/api/v1/__init__.py
+-rw-r--r--  2.0 unx     6565 b- defN 24-Apr-25 10:10 nucliadb/writer/api/v1/export_import.py
+-rw-r--r--  2.0 unx    28578 b- defN 24-Apr-25 10:10 nucliadb/writer/api/v1/field.py
+-rw-r--r--  2.0 unx     5239 b- defN 24-Apr-25 10:10 nucliadb/writer/api/v1/knowledgebox.py
+-rw-r--r--  2.0 unx     2052 b- defN 24-Apr-25 10:10 nucliadb/writer/api/v1/learning_config.py
+-rw-r--r--  2.0 unx    19940 b- defN 24-Apr-25 10:10 nucliadb/writer/api/v1/resource.py
+-rw-r--r--  2.0 unx     1034 b- defN 24-Apr-25 10:10 nucliadb/writer/api/v1/router.py
+-rw-r--r--  2.0 unx    10726 b- defN 24-Apr-25 10:10 nucliadb/writer/api/v1/services.py
+-rw-r--r--  2.0 unx    31701 b- defN 24-Apr-25 10:10 nucliadb/writer/api/v1/upload.py
+-rw-r--r--  2.0 unx     1612 b- defN 24-Apr-25 10:10 nucliadb/writer/layouts/__init__.py
+-rw-r--r--  2.0 unx     2115 b- defN 24-Apr-25 10:10 nucliadb/writer/layouts/v1.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-25 10:10 nucliadb/writer/resource/__init__.py
+-rw-r--r--  2.0 unx     1425 b- defN 24-Apr-25 10:10 nucliadb/writer/resource/audit.py
+-rw-r--r--  2.0 unx    10968 b- defN 24-Apr-25 10:10 nucliadb/writer/resource/basic.py
+-rw-r--r--  2.0 unx    16319 b- defN 24-Apr-25 10:10 nucliadb/writer/resource/field.py
+-rw-r--r--  2.0 unx     2022 b- defN 24-Apr-25 10:10 nucliadb/writer/resource/origin.py
+-rw-r--r--  2.0 unx     1152 b- defN 24-Apr-25 10:10 nucliadb/writer/resource/slug.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-25 10:10 nucliadb/writer/tests/__init__.py
+-rw-r--r--  2.0 unx     1200 b- defN 24-Apr-25 10:10 nucliadb/writer/tests/conftest.py
+-rw-r--r--  2.0 unx     5971 b- defN 24-Apr-25 10:10 nucliadb/writer/tests/fixtures.py
+-rw-r--r--  2.0 unx    15472 b- defN 24-Apr-25 10:10 nucliadb/writer/tests/test_fields.py
+-rw-r--r--  2.0 unx    25913 b- defN 24-Apr-25 10:10 nucliadb/writer/tests/test_files.py
+-rw-r--r--  2.0 unx     1729 b- defN 24-Apr-25 10:10 nucliadb/writer/tests/test_knowledgebox.py
+-rw-r--r--  2.0 unx     4569 b- defN 24-Apr-25 10:10 nucliadb/writer/tests/test_reprocess_file_field.py
+-rw-r--r--  2.0 unx    16938 b- defN 24-Apr-25 10:10 nucliadb/writer/tests/test_resources.py
+-rw-r--r--  2.0 unx     5120 b- defN 24-Apr-25 10:10 nucliadb/writer/tests/test_service.py
+-rw-r--r--  2.0 unx     6054 b- defN 24-Apr-25 10:10 nucliadb/writer/tests/test_tus.py
+-rw-r--r--  2.0 unx     1287 b- defN 24-Apr-25 10:10 nucliadb/writer/tests/utils.py
+-rw-r--r--  2.0 unx     5226 b- defN 24-Apr-25 10:10 nucliadb/writer/tus/__init__.py
+-rw-r--r--  2.0 unx     5082 b- defN 24-Apr-25 10:10 nucliadb/writer/tus/dm.py
+-rw-r--r--  2.0 unx     2186 b- defN 24-Apr-25 10:10 nucliadb/writer/tus/exceptions.py
+-rw-r--r--  2.0 unx    14527 b- defN 24-Apr-25 10:10 nucliadb/writer/tus/gcs.py
+-rw-r--r--  2.0 unx     5849 b- defN 24-Apr-25 10:10 nucliadb/writer/tus/local.py
+-rw-r--r--  2.0 unx     4367 b- defN 24-Apr-25 10:10 nucliadb/writer/tus/pg.py
+-rw-r--r--  2.0 unx     9069 b- defN 24-Apr-25 10:10 nucliadb/writer/tus/s3.py
+-rw-r--r--  2.0 unx     4734 b- defN 24-Apr-25 10:10 nucliadb/writer/tus/storage.py
+-rw-r--r--  2.0 unx     2556 b- defN 24-Apr-25 10:10 nucliadb/writer/tus/utils.py
+-rw-r--r--  2.0 unx     4343 b- defN 24-Apr-25 10:11 nucliadb-3.0.3.post454.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-25 10:11 nucliadb-3.0.3.post454.dist-info/WHEEL
+-rw-r--r--  2.0 unx     1268 b- defN 24-Apr-25 10:11 nucliadb-3.0.3.post454.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       20 b- defN 24-Apr-25 10:11 nucliadb-3.0.3.post454.dist-info/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 24-Apr-25 10:11 nucliadb-3.0.3.post454.dist-info/zip-safe
+-rw-rw-r--  2.0 unx    42679 b- defN 24-Apr-25 10:11 nucliadb-3.0.3.post454.dist-info/RECORD
+455 files, 2233319 bytes uncompressed, 684391 bytes compressed:  69.4%
```

## zipnote {}

```diff
@@ -45,14 +45,17 @@
 
 Filename: migrations/0017_multiple_writable_shards.py
 Comment: 
 
 Filename: migrations/0018_purge_orphan_kbslugs.py
 Comment: 
 
+Filename: migrations/0019_upgrade_to_paragraphs_v3.py
+Comment: 
+
 Filename: migrations/__init__.py
 Comment: 
 
 Filename: nucliadb/__init__.py
 Comment: 
 
 Filename: nucliadb/health.py
@@ -174,17 +177,14 @@
 
 Filename: nucliadb/common/datamanagers/rollover.py
 Comment: 
 
 Filename: nucliadb/common/datamanagers/utils.py
 Comment: 
 
-Filename: nucliadb/common/datamanagers/vectorsets.py
-Comment: 
-
 Filename: nucliadb/common/http_clients/__init__.py
 Comment: 
 
 Filename: nucliadb/common/http_clients/auth.py
 Comment: 
 
 Filename: nucliadb/common/http_clients/exceptions.py
@@ -1224,17 +1224,14 @@
 
 Filename: nucliadb/writer/settings.py
 Comment: 
 
 Filename: nucliadb/writer/utilities.py
 Comment: 
 
-Filename: nucliadb/writer/vectors.py
-Comment: 
-
 Filename: nucliadb/writer/api/__init__.py
 Comment: 
 
 Filename: nucliadb/writer/api/constants.py
 Comment: 
 
 Filename: nucliadb/writer/api/v1/__init__.py
@@ -1344,26 +1341,26 @@
 
 Filename: nucliadb/writer/tus/storage.py
 Comment: 
 
 Filename: nucliadb/writer/tus/utils.py
 Comment: 
 
-Filename: nucliadb-3.0.3.post450.dist-info/METADATA
+Filename: nucliadb-3.0.3.post454.dist-info/METADATA
 Comment: 
 
-Filename: nucliadb-3.0.3.post450.dist-info/WHEEL
+Filename: nucliadb-3.0.3.post454.dist-info/WHEEL
 Comment: 
 
-Filename: nucliadb-3.0.3.post450.dist-info/entry_points.txt
+Filename: nucliadb-3.0.3.post454.dist-info/entry_points.txt
 Comment: 
 
-Filename: nucliadb-3.0.3.post450.dist-info/top_level.txt
+Filename: nucliadb-3.0.3.post454.dist-info/top_level.txt
 Comment: 
 
-Filename: nucliadb-3.0.3.post450.dist-info/zip-safe
+Filename: nucliadb-3.0.3.post454.dist-info/zip-safe
 Comment: 
 
-Filename: nucliadb-3.0.3.post450.dist-info/RECORD
+Filename: nucliadb-3.0.3.post454.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## nucliadb/common/cluster/base.py

```diff
@@ -81,21 +81,17 @@
 
     async def stream_get_paragraphs(
         self, stream_request: nodereader_pb2.StreamRequest
     ) -> AsyncIterator[nodereader_pb2.ParagraphItem]:
         async for idandfacets in self.reader.Paragraphs(stream_request):  # type: ignore
             yield idandfacets
 
-    async def get_shard(
-        self, shard_id: str, vectorset: Optional[str] = None
-    ) -> noderesources_pb2.Shard:
+    async def get_shard(self, shard_id: str) -> noderesources_pb2.Shard:
         req = nodereader_pb2.GetShardRequest()
         req.shard_id.id = shard_id
-        if vectorset is not None:
-            req.vectorset = vectorset
         return await self.reader.GetShard(req)  # type: ignore
 
     async def new_shard(
         self,
         kbid: str,
         similarity: utils_pb2.VectorSimilarity.ValueType,
         release_channel: utils_pb2.ReleaseChannel.ValueType,
```

## nucliadb/ingest/orm/knowledgebox.py

```diff
@@ -26,15 +26,14 @@
 from nucliadb_protos.knowledgebox_pb2 import (
     KnowledgeBoxConfig,
     Labels,
     LabelSet,
     SemanticModelMetadata,
 )
 from nucliadb_protos.knowledgebox_pb2 import Synonyms as PBSynonyms
-from nucliadb_protos.knowledgebox_pb2 import VectorSet
 from nucliadb_protos.resources_pb2 import Basic
 from nucliadb_protos.utils_pb2 import ReleaseChannel
 
 from nucliadb.common import datamanagers
 from nucliadb.common.cluster.base import AbstractIndexNode
 from nucliadb.common.cluster.exceptions import ShardNotFound, ShardsNotFound
 from nucliadb.common.cluster.manager import get_index_node
@@ -242,40 +241,14 @@
 
         for shard in shards_obj.shards:
             for replica in shard.replicas:
                 node = get_index_node(replica.node)
                 if node is not None:
                     yield node, replica.shard.id
 
-    # Vectorset
-    async def get_vectorsets(self, response: writer_pb2.GetVectorSetsResponse):
-        vectorsets = await datamanagers.vectorsets.get_vectorsets(
-            self.txn, kbid=self.kbid
-        )
-        if vectorsets is not None:
-            response.vectorsets.CopyFrom(vectorsets)
-
-    async def set_vectorset(self, id: str, vs: VectorSet):
-        # For each Node on the KB add the vectorset
-        async for node, shard in self.iterate_kb_nodes():
-            await node.set_vectorset(shard, id, similarity=vs.similarity)
-
-        await datamanagers.vectorsets.set_vectorset(
-            self.txn, kbid=self.kbid, vectorset_id=id, vs=vs
-        )
-
-    async def del_vectorset(self, id: str):
-        await datamanagers.vectorsets.del_vectorset(
-            self.txn, kbid=self.kbid, vectorset_id=id
-        )
-
-        # For each Node on the KB delete the vectorset
-        async for node, shard in self.iterate_kb_nodes():
-            await node.del_vectorset(shard, id)
-
     # Labels
     async def set_labelset(self, id: str, labelset: LabelSet):
         await datamanagers.labels.set_labelset(
             self.txn, kbid=self.kbid, labelset_id=id, labelset=labelset
         )
 
     async def get_labels(self) -> Labels:
```

## nucliadb/ingest/service/writer.py

```diff
@@ -36,29 +36,26 @@
 )
 from nucliadb_protos.resources_pb2 import CloudFile
 from nucliadb_protos.writer_pb2 import (
     BinaryData,
     BrokerMessage,
     DelEntitiesRequest,
     DelLabelsRequest,
-    DelVectorSetRequest,
     ExtractedVectorsWrapper,
     FileRequest,
     FileUploaded,
     GetEntitiesGroupRequest,
     GetEntitiesGroupResponse,
     GetEntitiesRequest,
     GetEntitiesResponse,
     GetLabelSetRequest,
     GetLabelSetResponse,
     GetLabelsRequest,
     GetLabelsResponse,
     GetSynonymsResponse,
-    GetVectorSetsRequest,
-    GetVectorSetsResponse,
     IndexResource,
     IndexStatus,
     ListEntitiesGroupsRequest,
     ListEntitiesGroupsResponse,
     ListMembersRequest,
     ListMembersResponse,
     NewEntitiesGroupRequest,
@@ -67,15 +64,14 @@
     ResourceFieldExistsResponse,
     ResourceFieldId,
     ResourceIdRequest,
     ResourceIdResponse,
     SetEntitiesRequest,
     SetLabelsRequest,
     SetSynonymsRequest,
-    SetVectorSetRequest,
     SetVectorsRequest,
     SetVectorsResponse,
     UpdateEntitiesGroupRequest,
     UpdateEntitiesGroupResponse,
     UploadBinaryData,
     WriterStatusRequest,
     WriterStatusResponse,
@@ -373,56 +369,14 @@
                 await kbobj.get_labelset(request.labelset, response)
                 response.kb.uuid = kbobj.kbid
                 response.status = GetLabelSetResponse.Status.OK
             else:
                 response.status = GetLabelSetResponse.Status.NOTFOUND
             return response
 
-    async def GetVectorSets(  # type: ignore
-        self, request: GetVectorSetsRequest, context=None
-    ) -> GetVectorSetsResponse:
-        async with self.driver.transaction() as txn:
-            kbobj = await self.proc.get_kb_obj(txn, request.kb)
-            response = GetVectorSetsResponse()
-            if kbobj is not None:
-                await kbobj.get_vectorsets(response)
-                response.kb.uuid = kbobj.kbid
-                response.status = GetVectorSetsResponse.Status.OK
-            else:
-                response.status = GetVectorSetsResponse.Status.NOTFOUND
-            return response
-
-    async def DelVectorSet(  # type: ignore
-        self, request: DelVectorSetRequest, context=None
-    ) -> OpStatusWriter:
-        async with self.driver.transaction() as txn:
-            kbobj = await self.proc.get_kb_obj(txn, request.kb)
-            response = OpStatusWriter()
-            if kbobj is not None:
-                await kbobj.del_vectorset(request.vectorset)
-                response.status = OpStatusWriter.Status.OK
-                await txn.commit()
-            else:
-                response.status = OpStatusWriter.Status.NOTFOUND
-            return response
-
-    async def SetVectorSet(  # type: ignore
-        self, request: SetVectorSetRequest, context=None
-    ) -> OpStatusWriter:
-        async with self.driver.transaction() as txn:
-            kbobj = await self.proc.get_kb_obj(txn, request.kb)
-            response = OpStatusWriter()
-            if kbobj is not None:
-                await kbobj.set_vectorset(request.id, request.vectorset)
-                response.status = OpStatusWriter.Status.OK
-                await txn.commit()
-            else:
-                response.status = OpStatusWriter.Status.NOTFOUND
-            return response
-
     async def NewEntitiesGroup(  # type: ignore
         self, request: NewEntitiesGroupRequest, context=None
     ) -> NewEntitiesGroupResponse:
         response = NewEntitiesGroupResponse()
         async with self.driver.transaction() as txn:
             kbobj = await self.proc.get_kb_obj(txn, request.kb)
             if kbobj is None:
```

## nucliadb/reader/api/v1/services.py

```diff
@@ -29,16 +29,14 @@
     GetEntitiesGroupRequest,
     GetEntitiesGroupResponse,
     GetLabelSetRequest,
     GetLabelSetResponse,
     GetLabelsRequest,
     GetLabelsResponse,
     GetSynonymsResponse,
-    GetVectorSetsRequest,
-    GetVectorSetsResponse,
     ListEntitiesGroupsRequest,
     ListEntitiesGroupsResponse,
     OpStatusWriter,
 )
 from starlette.requests import Request
 
 from nucliadb.common import datamanagers
@@ -55,18 +53,16 @@
     EntitiesGroup,
     EntitiesGroupSummary,
     KnowledgeBoxEntities,
 )
 from nucliadb_models.labels import KnowledgeBoxLabels, LabelSet
 from nucliadb_models.resource import NucliaDBRoles
 from nucliadb_models.synonyms import KnowledgeBoxSynonyms
-from nucliadb_models.vectors import VectorSet, VectorSets
-from nucliadb_utils import const
 from nucliadb_utils.authentication import requires
-from nucliadb_utils.utilities import get_ingest, get_storage, has_feature
+from nucliadb_utils.utilities import get_ingest, get_storage
 
 
 @api.get(
     f"/{KB_PREFIX}/{{kbid}}/entitiesgroups",
     status_code=200,
     name="Get Knowledge Box Entities",
     response_model=KnowledgeBoxEntities,
@@ -207,48 +203,14 @@
     else:
         raise HTTPException(
             status_code=500, detail="Error on getting labelset on a Knowledge box"
         )
 
 
 @api.get(
-    f"/{KB_PREFIX}/{{kbid}}/vectorsets",
-    status_code=200,
-    name="Get Knowledge Box Vector Sets",
-    tags=["Knowledge Box Services"],
-    response_model=VectorSets,
-    openapi_extra={"x-operation_order": 1},
-)
-@requires(NucliaDBRoles.READER)
-@version(1)
-async def get_vectorsets(request: Request, kbid: str):
-    if not has_feature(const.Features.VECTORSETS_V2, context={"kbid": kbid}):
-        raise HTTPException(
-            status_code=404,
-            detail="Vectorsets API is not yet implemented",
-        )
-    ingest = get_ingest()
-    pbrequest: GetVectorSetsRequest = GetVectorSetsRequest()
-    pbrequest.kb.uuid = kbid
-
-    vectorsets: GetVectorSetsResponse = await ingest.GetVectorSets(pbrequest)  # type: ignore
-    if vectorsets.status == GetVectorSetsResponse.Status.OK:
-        result = VectorSets(vectorsets={})
-        for key, vector in vectorsets.vectorsets.vectorsets.items():
-            result.vectorsets[key] = VectorSet.from_message(vector)
-        return result
-    elif vectorsets.status == GetVectorSetsResponse.Status.NOTFOUND:
-        raise HTTPException(status_code=404, detail="VectorSet does not exist")
-    elif vectorsets.status == GetVectorSetsResponse.Status.ERROR:
-        raise HTTPException(
-            status_code=500, detail="Error on getting vectorset on a Knowledge box"
-        )
-
-
-@api.get(
     f"/{KB_PREFIX}/{{kbid}}/custom-synonyms",
     status_code=200,
     name="Get Knowledge Box Custom Synonyms",
     tags=["Knowledge Box Services"],
     response_model=KnowledgeBoxSynonyms,
     openapi_extra={"x-operation_order": 2},
 )
```

## nucliadb/search/api/v1/knowledgebox.py

```diff
@@ -80,15 +80,14 @@
     response_model_exclude_unset=True,
 )
 @requires_one([NucliaDBRoles.READER, NucliaDBRoles.MANAGER])
 @version(1)
 async def knowledgebox_counters(
     request: Request,
     kbid: str,
-    vectorset: str = fastapi_query(SearchParamDefaults.vectorset),
     debug: bool = fastapi_query(SearchParamDefaults.debug),
 ) -> KnowledgeboxCounters:
     shard_manager = get_shard_manager()
 
     try:
         shard_groups: list[PBShardObject] = await shard_manager.get_shards_by_kbid(kbid)
     except ShardsNotFound:
@@ -107,15 +106,15 @@
                 status_code=500,
                 detail="Couldn't retrieve counters right now, node not found",
             )
         else:
             if shard_id is not None:
                 # At least one node is alive for this shard group
                 # let's add it ot the query list if has a valid value
-                ops.append(get_shard(node, shard_id, vectorset=vectorset))
+                ops.append(get_shard(node, shard_id))
                 queried_shards.append(shard_id)
 
     if not ops:
         logger.info(f"No node found for any of this resources shards {kbid}")
         raise HTTPException(
             status_code=500,
             detail=f"No node found for any of this resources shards {kbid}",
```

## nucliadb/search/api/v1/search.py

```diff
@@ -428,15 +428,14 @@
         min_score=item.min_score,
         range_creation_start=item.range_creation_start,
         range_creation_end=item.range_creation_end,
         range_modification_start=item.range_modification_start,
         range_modification_end=item.range_modification_end,
         fields=item.fields,
         user_vector=item.vector,
-        vectorset=item.vectorset,
         with_duplicates=item.with_duplicates,
         with_status=with_status,
         with_synonyms=item.with_synonyms,
         autofilter=item.autofilter,
         security=item.security,
         rephrase=item.rephrase,
     )
```

## nucliadb/search/search/find.py

```diff
@@ -69,15 +69,14 @@
         min_score=item.min_score,
         range_creation_start=item.range_creation_start,
         range_creation_end=item.range_creation_end,
         range_modification_start=item.range_modification_start,
         range_modification_end=item.range_modification_end,
         fields=item.fields,
         user_vector=item.vector,
-        vectorset=item.vectorset,
         with_duplicates=item.with_duplicates,
         with_synonyms=item.with_synonyms,
         autofilter=item.autofilter,
         key_filters=item.resource_filters,
         security=item.security,
         generative_model=generative_model,
         rephrase=item.rephrase,
```

## nucliadb/search/search/query.py

```diff
@@ -102,15 +102,14 @@
         sort: Optional[SortOptions] = None,
         range_creation_start: Optional[datetime] = None,
         range_creation_end: Optional[datetime] = None,
         range_modification_start: Optional[datetime] = None,
         range_modification_end: Optional[datetime] = None,
         fields: Optional[list[str]] = None,
         user_vector: Optional[list[float]] = None,
-        vectorset: Optional[str] = None,
         with_duplicates: bool = False,
         with_status: Optional[ResourceProcessingStatus] = None,
         with_synonyms: bool = False,
         autofilter: bool = False,
         key_filters: Optional[list[str]] = None,
         security: Optional[RequestSecurity] = None,
         generative_model: Optional[str] = None,
@@ -129,15 +128,14 @@
         self.sort = sort
         self.range_creation_start = range_creation_start
         self.range_creation_end = range_creation_end
         self.range_modification_start = range_modification_start
         self.range_modification_end = range_modification_end
         self.fields = fields or []
         self.user_vector = user_vector
-        self.vectorset = vectorset
         self.with_duplicates = with_duplicates
         self.with_status = with_status
         self.with_synonyms = with_synonyms
         self.autofilter = autofilter
         self.key_filters = key_filters
         self.security = security
         self.generative_model = generative_model
@@ -368,18 +366,14 @@
     async def parse_vector_search(self, request: nodereader_pb2.SearchRequest) -> bool:
         if SearchOptions.VECTOR not in self.features:
             return False
 
         node_features.inc({"type": "vectors"})
 
         incomplete = False
-        if self.vectorset is not None:
-            request.vectorset = self.vectorset
-            node_features.inc({"type": "vectorset"})
-
         query_vector = None
         if self.user_vector is None:
             try:
                 query_info = await self._get_query_information()
             except SendToPredictError as err:
                 logger.warning(f"Errors on predict api trying to embedd query: {err}")
                 incomplete = True
```

## nucliadb/search/search/shards.py

```diff
@@ -14,15 +14,14 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 #
 import asyncio
-from typing import Optional
 
 from nucliadb_protos.nodereader_pb2 import (
     GetShardRequest,
     ParagraphSearchRequest,
     ParagraphSearchResponse,
     RelationSearchRequest,
     RelationSearchResponse,
@@ -51,21 +50,17 @@
     req = SearchRequest()
     req.CopyFrom(query)
     req.shard = shard
     with node_observer({"type": "search", "node_id": node.id}):
         return await node.reader.Search(req)  # type: ignore
 
 
-async def get_shard(
-    node: AbstractIndexNode, shard_id: str, vectorset: Optional[str] = None
-) -> Shard:
+async def get_shard(node: AbstractIndexNode, shard_id: str) -> Shard:
     req = GetShardRequest()
     req.shard_id.id = shard_id
-    if vectorset is not None:
-        req.vectorset = vectorset
     with node_observer({"type": "get_shard", "node_id": node.id}):
         return await node.reader.GetShard(req)  # type: ignore
 
 
 async def query_paragraph_shard(
     node: AbstractIndexNode, shard: str, query: ParagraphSearchRequest
 ) -> ParagraphSearchResponse:
```

## nucliadb/writer/api/v1/services.py

```diff
@@ -21,15 +21,14 @@
 from fastapi_versioning import version
 from nucliadb_protos.knowledgebox_pb2 import KnowledgeBoxID
 from nucliadb_protos.knowledgebox_pb2 import Label as LabelPB
 from nucliadb_protos.knowledgebox_pb2 import LabelSet as LabelSetPB
 from nucliadb_protos.writer_pb2 import (
     DelEntitiesRequest,
     DelLabelsRequest,
-    DelVectorSetRequest,
     NewEntitiesGroupRequest,
     NewEntitiesGroupResponse,
     OpStatusWriter,
     SetLabelsRequest,
     SetSynonymsRequest,
     UpdateEntitiesGroupRequest,
     UpdateEntitiesGroupResponse,
@@ -38,26 +37,23 @@
 
 from nucliadb.models.responses import (
     HTTPConflict,
     HTTPInternalServerError,
     HTTPNotFound,
 )
 from nucliadb.writer.api.v1.router import KB_PREFIX, api
-from nucliadb.writer.vectors import create_vectorset
 from nucliadb_models.entities import (
     CreateEntitiesGroupPayload,
     UpdateEntitiesGroupPayload,
 )
 from nucliadb_models.labels import LabelSet
 from nucliadb_models.resource import NucliaDBRoles
 from nucliadb_models.synonyms import KnowledgeBoxSynonyms
-from nucliadb_models.vectors import VectorSet
-from nucliadb_utils import const
 from nucliadb_utils.authentication import requires
-from nucliadb_utils.utilities import get_ingest, has_feature
+from nucliadb_utils.utilities import get_ingest
 
 
 @api.post(
     f"/{KB_PREFIX}/{{kbid}}/entitiesgroups",
     status_code=200,
     name="Create Knowledge Box Entities Group",
     tags=["Knowledge Box Services"],
@@ -244,63 +240,14 @@
     elif status.status == OpStatusWriter.Status.ERROR:
         raise HTTPException(
             status_code=500, detail="Error on deleting labels from a Knowledge box"
         )
     return Response(status_code=204)
 
 
-@api.post(
-    f"/{KB_PREFIX}/{{kbid}}/vectorset/{{vectorset}}",
-    status_code=200,
-    name="Set Knowledge Box VectorSet",
-    tags=["Knowledge Box Services"],
-    openapi_extra={"x-operation_order": 1},
-)
-@requires(NucliaDBRoles.WRITER)
-@version(1)
-async def set_vectorset(request: Request, kbid: str, vectorset: str, item: VectorSet):
-    if not has_feature(const.Features.VECTORSETS_V2, context={"kbid": kbid}):
-        raise HTTPException(
-            status_code=404,
-            detail="Vectorsets API is not yet implemented",
-        )
-    await create_vectorset(kbid, vectorset, item.dimension, similarity=item.similarity)
-
-
-@api.delete(
-    f"/{KB_PREFIX}/{{kbid}}/vectorset/{{vectorset}}",
-    status_code=200,
-    name="Delete Knowledge Box VectorSet",
-    tags=["Knowledge Box Services"],
-    openapi_extra={"x-operation_order": 3},
-)
-@requires(NucliaDBRoles.WRITER)
-@version(1)
-async def delete_vectorset(request: Request, kbid: str, vectorset: str):
-    if not has_feature(const.Features.VECTORSETS_V2, context={"kbid": kbid}):
-        raise HTTPException(
-            status_code=404,
-            detail="Vectorsets API is not yet implemented",
-        )
-    ingest = get_ingest()
-    pbrequest: DelVectorSetRequest = DelVectorSetRequest()
-    pbrequest.kb.uuid = kbid
-    pbrequest.vectorset = vectorset
-    status: OpStatusWriter = await ingest.DelVectorSet(pbrequest)  # type: ignore
-    if status.status == OpStatusWriter.Status.OK:
-        return None
-    elif status.status == OpStatusWriter.Status.NOTFOUND:
-        raise HTTPException(status_code=404, detail="Knowledge Box does not exist")
-    elif status.status == OpStatusWriter.Status.ERROR:
-        raise HTTPException(
-            status_code=500, detail="Error on deleting vectorset from a Knowledge box"
-        )
-    return Response(status_code=204)
-
-
 @api.put(
     f"/{KB_PREFIX}/{{kbid}}/custom-synonyms",
     status_code=204,
     name="Set Knowledge Box Custom Synonyms",
     tags=["Knowledge Box Services"],
     openapi_extra={"x-operation_order": 1},
 )
```

## nucliadb/writer/api/v1/upload.py

```diff
@@ -29,15 +29,15 @@
 from fastapi import HTTPException
 from fastapi.params import Header
 from fastapi.requests import Request
 from fastapi.responses import Response
 from fastapi_versioning import version  # type: ignore
 from grpc import StatusCode as GrpcStatusCode
 from grpc.aio import AioRpcError
-from nucliadb_protos.resources_pb2 import FieldFile
+from nucliadb_protos.resources_pb2 import FieldFile, Metadata
 from nucliadb_protos.writer_pb2 import (
     BrokerMessage,
     ResourceFieldExistsResponse,
     ResourceFieldId,
 )
 from starlette.requests import Request as StarletteRequest
 
@@ -937,14 +937,16 @@
     writer.files[field].ClearField("password")
 
     toprocess.filefield[field] = await processing.convert_internal_filefield_to_str(
         file_field, storage=storage
     )
 
     writer.source = BrokerMessage.MessageSource.WRITER
+    writer.basic.metadata.status = Metadata.Status.PENDING
+    writer.basic.metadata.useful = True
     try:
         await transaction.commit(writer, partition, wait=True)
     except TransactionCommitTimeoutError:
         raise HTTPException(
             status_code=501,
             detail="Inconsistent write. This resource will not be processed and may not be stored.",
         )
```

## nucliadb/writer/tests/test_resources.py

```diff
@@ -47,28 +47,14 @@
     TEST_TEXT_PAYLOAD,
 )
 from nucliadb_models.resource import NucliaDBRoles
 from nucliadb_utils.utilities import get_ingest
 
 
 @pytest.mark.asyncio
-@pytest.mark.xfail(reason="New vectorset api is not implemented yet")
-async def test_resource_crud_min(
-    writer_api: Callable[[list[str]], AsyncClient], knowledgebox_writer: str
-):
-    knowledgebox_id = knowledgebox_writer
-    async with writer_api([NucliaDBRoles.WRITER]) as client:
-        resp = await client.post(
-            f"/{KB_PREFIX}/{knowledgebox_id}/vectorset/base",
-            json={"dimension": 3, "similarity": "dot"},
-        )
-        assert resp.status_code == 200
-
-
-@pytest.mark.asyncio
 async def test_resource_crud(
     writer_api: Callable[[list[str]], AsyncClient], knowledgebox_writer: str
 ):
     knowledgebox_id = knowledgebox_writer
     async with writer_api([NucliaDBRoles.WRITER]) as client:
         # Test create resource
         resp = await client.post(
```

## Comparing `nucliadb-3.0.3.post450.dist-info/METADATA` & `nucliadb-3.0.3.post454.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nucliadb
-Version: 3.0.3.post450
+Version: 3.0.3.post454
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
-Requires-Dist: nucliadb-telemetry[all] >=3.0.3.post450
-Requires-Dist: nucliadb-utils[cache,fastapi,storages] >=3.0.3.post450
-Requires-Dist: nucliadb-protos >=3.0.3.post450
-Requires-Dist: nucliadb-models >=3.0.3.post450
+Requires-Dist: nucliadb-telemetry[all] >=3.0.3.post454
+Requires-Dist: nucliadb-utils[cache,fastapi,storages] >=3.0.3.post454
+Requires-Dist: nucliadb-protos >=3.0.3.post454
+Requires-Dist: nucliadb-models >=3.0.3.post454
 Requires-Dist: nucliadb-admin-assets >=1.0.0.post1224
 Requires-Dist: nucliadb-node-binding >=2.26.0
 Requires-Dist: uvicorn <0.19.0
 Requires-Dist: pydantic-argparse
 Requires-Dist: aiohttp >=3.9.4
 Requires-Dist: lru-dict >=1.1.7
 Requires-Dist: backoff
```

## Comparing `nucliadb-3.0.3.post450.dist-info/entry_points.txt` & `nucliadb-3.0.3.post454.dist-info/entry_points.txt`

 * *Files identical despite different names*

## Comparing `nucliadb-3.0.3.post450.dist-info/RECORD` & `nucliadb-3.0.3.post454.dist-info/RECORD`

 * *Files 0% similar despite different names*

```diff
@@ -11,25 +11,26 @@
 migrations/0012_rollover_shards.py,sha256=3ShFPB11vFEYvso5vc8NZwYhXwuA0R4inA16k15GAkI,1443
 migrations/0013_rollover_shards.py,sha256=c3IU8zinlWeVRN8T6o5eLpvGzkQOHX_Yz5xuFVRUy5U,1024
 migrations/0014_rollover_shards.py,sha256=24yLtXAwlVvCwtHLx9Tz-VWCzeMuy-0o3M6QNESi_Iw,1382
 migrations/0015_targeted_rollover.py,sha256=7C9XM8wg-bpkNyFh0xJuaGzOcE2WqU1BfqtInKAjTkw,1462
 migrations/0016_upgrade_to_paragraphs_v2.py,sha256=pOZUwTDfGoLjcSSKiWaN6FUvMDN95XNCBoux3u0dsmQ,2506
 migrations/0017_multiple_writable_shards.py,sha256=NY38wFVxSDXglkZE6DRnuN1DG_1kyZXr2j37C8VhyA0,2100
 migrations/0018_purge_orphan_kbslugs.py,sha256=3x5OsMb-JnP9y8_-ztYugk1RiXbOuthTFB-8I1XX3bk,2264
+migrations/0019_upgrade_to_paragraphs_v3.py,sha256=Jf1ljYQoLj1QExz9-tDIxI7QrwPhixIHxvQJvHOl6WA,2506
 migrations/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
 nucliadb/__init__.py,sha256=_abCmDJ_0ku483Os4UAjPX7Nywm39cQgAV_DiyjsKeQ,891
 nucliadb/health.py,sha256=zPwd3CAFJf9owhbadtyGLvHekOjX9ykvxLYWYxnD5eo,3733
 nucliadb/learning_proxy.py,sha256=6r_fFgE662yEFgNpgGNxc3KTfFiR78yiEN95Qir6ctI,11626
 nucliadb/metrics_exporter.py,sha256=PummIqtRLdpcONPIpRKBj_jGYnX7B9XZ2IO048bu2pM,4806
 nucliadb/openapi.py,sha256=wDiw0dVEvTpJvbatkJ0JZLkKm9RItZT5PWRHjqRfqTA,2272
 nucliadb/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 nucliadb/common/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
 nucliadb/common/locking.py,sha256=_168BClwNyXVentC7mk4_on0qof5G2y5VgTpOWvzJGk,4905
 nucliadb/common/cluster/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
-nucliadb/common/cluster/base.py,sha256=JNb-NhRBd7eLMpaiPsypxk0x1YUo2GIyfubhnjDuD6Y,5090
+nucliadb/common/cluster/base.py,sha256=z_JD-xNVPB6-6O_u8YMpyOPP3fRmimwq7LbA3EGqDnE,4971
 nucliadb/common/cluster/exceptions.py,sha256=V3c_fgH00GyJ-a5CaGLhwTuhwhUNR9YAGvS5jaRuc_Y,1495
 nucliadb/common/cluster/grpc_node_dummy.py,sha256=pBO675j-BptC5U_8Wi6uB19QSQTixgJP2MTzr8v6_Wk,3658
 nucliadb/common/cluster/index_node.py,sha256=WafWLzU1l7EHj1VyG0w6qi2BW_Izc8rFze6ZWbYvT9g,3429
 nucliadb/common/cluster/manager.py,sha256=JIb5jpfmBSjFPXxe4YQqWrQW3TD8iY-0a2HrqIGbThw,21231
 nucliadb/common/cluster/rebalance.py,sha256=RC5Q9Uic0__QHeukd2ANlWyd6AYKBzRm3FXhvwcwxCo,8490
 nucliadb/common/cluster/rollover.py,sha256=pvQbL-xGtEcSlLGsQnMDFj1Jr7_g7IMkj6ZQkH2a4Vo,19593
 nucliadb/common/cluster/settings.py,sha256=snENrNo9voc1TZ6uyBnuSHGoS2Ocga_Kn-W33nOlO-c,2713
@@ -54,15 +55,14 @@
 nucliadb/common/datamanagers/exceptions.py,sha256=Atz_PP_GGq4jgJaWcAkcRbHBoBaGcC9yJvFteylKtTE,883
 nucliadb/common/datamanagers/kb.py,sha256=zkG3lVbGFFLtjcTlJvJDtTY6S55xdty1nSlwI4xDEQ4,3994
 nucliadb/common/datamanagers/labels.py,sha256=2pN8RrFNTXLitDo44CS3AApjCjbv-2ALkqjwHVR_Mb0,5389
 nucliadb/common/datamanagers/processing.py,sha256=gdCHGzF2LiHOapsg4oaYFYNxACwaCbN1z3kw7iHTuNc,1599
 nucliadb/common/datamanagers/resources.py,sha256=HapnkdZznvxzZMUVLpMhY0sM8578hOq1WbrjVSNuNHg,7637
 nucliadb/common/datamanagers/rollover.py,sha256=gyF5EJ_-R3lunnXfj4JD7rdhh1l8lEWgwgRxeZHMpsw,5633
 nucliadb/common/datamanagers/utils.py,sha256=_Yp_s3zCeWCqtqSSO_PY7xgk2Vo0W9mVqQst2Mj2eFU,1681
-nucliadb/common/datamanagers/vectorsets.py,sha256=4CZkeQ0s0ITcneBSCGtGojdjqqaGu9ykPisYmEYv8IM,2055
 nucliadb/common/http_clients/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
 nucliadb/common/http_clients/auth.py,sha256=9A1k-H121W3lAFRl_XxGizcxUw_qw1STDZqJOC2Kpyw,2146
 nucliadb/common/http_clients/exceptions.py,sha256=47Y8OjkaGV_F18G07FpJhOzgWKUIexhlILyuVtICz8s,1100
 nucliadb/common/http_clients/processing.py,sha256=-J5Lxmlk4coboOWvYQ4gc88AIrvHzSV9bzVsedmslCQ,7155
 nucliadb/common/http_clients/pypi.py,sha256=VHIUjwJEJVntVUo_FRoXIo8sLmluy7sa9-iXSITcrMY,1540
 nucliadb/common/http_clients/utils.py,sha256=b7FCaOSf21UVE9OqDhBpWetxP2nguV_gKwBBb9dYifI,1551
 nucliadb/common/maindb/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
@@ -109,24 +109,24 @@
 nucliadb/ingest/fields/layout.py,sha256=clgBVGWArtkAEawDqCAu_hB9gVu5c6UT1Cf_5yrw47s,2250
 nucliadb/ingest/fields/link.py,sha256=6D1jlwX1ImU3RL1dVawXm2ChoB_s1_h5DOVGyW4q37M,4084
 nucliadb/ingest/fields/text.py,sha256=qMMH76gN--Ag1fPZ1I5G9ZPAi4U0i9jbqlrpYc3cMxg,1319
 nucliadb/ingest/orm/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
 nucliadb/ingest/orm/brain.py,sha256=Hq8c0TpHlJ2rT5oig3QX3xmSQZiB8YFURws5xj3-iuk,28367
 nucliadb/ingest/orm/entities.py,sha256=q027LfocE-KIqRNC1ZOSrrvt6x9NGrB25TZsOe0SyVk,15758
 nucliadb/ingest/orm/exceptions.py,sha256=GKr20V5xLv-WHBBHhr8lBChpW5oa9k18Xuiw-dIF9DM,1279
-nucliadb/ingest/orm/knowledgebox.py,sha256=28LLX4rhMVL7mqIAxSmRhTGSN_6rZSJu_Ct42Ut7gEY,18731
+nucliadb/ingest/orm/knowledgebox.py,sha256=-M_tkatSP8rFBG2gGN5Pe_i8Tk2KWlhgUhaCxiKVhxI,17684
 nucliadb/ingest/orm/metrics.py,sha256=OkwMSPKLZcKba0ZTwtTiIxwBgaLMX5ydhGieKvi2y7E,1096
 nucliadb/ingest/orm/resource.py,sha256=TWjYAqRRaZamT1ssWDGrQMmrxvu5R2X07zL13i7XxqY,60647
 nucliadb/ingest/orm/synonyms.py,sha256=tyOEGPfuJwhM5iYm4uNPjc2E8oWPk70DzZeuxVZ5alQ,1739
 nucliadb/ingest/orm/utils.py,sha256=0GwmyP0CqskAUqKbp0LAInYE64kt8locVqZ0HB04zlw,3683
 nucliadb/ingest/orm/processor/__init__.py,sha256=rdd6Eec4C3yhQYcrHLgwngLk3amMpih5h3N_8hYjqNk,26460
 nucliadb/ingest/orm/processor/sequence_manager.py,sha256=Mc9SA_NfzxTwovD5yGiAcdmen4pa-QNdsYcONIWeZPc,1690
 nucliadb/ingest/service/__init__.py,sha256=C_lkkjoHm0hDT2fZjEN4mpwXtU4bWthB-vM5-28-MBM,2057
 nucliadb/ingest/service/exceptions.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
-nucliadb/ingest/service/writer.py,sha256=xGsk2noVqKYnD8p_LYpzzand1tBiQKe13EJhfoMRHKc,37355
+nucliadb/ingest/service/writer.py,sha256=IxY1ddMH65OEhXOjTJS6TMVwqZ0yRJwNNKdoJCKk4j8,35455
 nucliadb/ingest/tests/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
 nucliadb/ingest/tests/conftest.py,sha256=yTepuxodMXl5vEMTzFfgos9wdRnYfxPffZQDYm3Ej-E,1157
 nucliadb/ingest/tests/fixtures.py,sha256=CeVkscwCn14PqPdfbjfR9u3FYgDKe_6kZG8nL75qjCU,24068
 nucliadb/ingest/tests/vectors.py,sha256=CcNKx-E8LPpyvRyljbmb-Tn_wST9Juw2CBoogWrKiTk,62843
 nucliadb/ingest/tests/integration/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
 nucliadb/ingest/tests/integration/consumer/__init__.py,sha256=itSI7dtTwFP55YMX4iK7JzdMHS5CQVUiB1XzQu4UBh8,833
 nucliadb/ingest/tests/integration/consumer/test_auditing.py,sha256=5VYFGUeaxd18mLtUfHCUPu9c1iAShNHNM5X_CSkIFSs,2549
@@ -181,15 +181,15 @@
 nucliadb/reader/api/v1/download.py,sha256=g4NwOO921Ok5WU6mYUYHRW0iK0p6rz6LttuMdMfGSs0,12368
 nucliadb/reader/api/v1/export_import.py,sha256=yybMDAaut_CPotTaiBGi52mMwQtx4V2UGPJEh-2ZYsg,6450
 nucliadb/reader/api/v1/knowledgebox.py,sha256=YeIxd6hAsTTerXqukvwm8N-2L6-FrMixrtAMw7JibLM,3632
 nucliadb/reader/api/v1/learning_collector.py,sha256=9K30TSYwsPJoAWynoJm5Yl3N7__QNy2T20Tw4jAvVpw,2093
 nucliadb/reader/api/v1/learning_config.py,sha256=vAZf1taIv3p_p48RJA9J1bPP1l4S1ALjXqrVWnlH42Q,4454
 nucliadb/reader/api/v1/resource.py,sha256=IFnuftz9F0eKIYs-73wA3LazHs4m58pbMoytyyrv-e0,13928
 nucliadb/reader/api/v1/router.py,sha256=eyNmEGSP9zHkCIG5XlAXl6sukq950B7gFT3X2peMtIE,1011
-nucliadb/reader/api/v1/services.py,sha256=rdOSU81-WXKIMb0IjrzVdixj1uhA0s2fB5qeOdjZ-sY,13882
+nucliadb/reader/api/v1/services.py,sha256=rZFk7rpWlhmh5EvOzf3XFGOVPl9RbJy9do8J464PTGs,12378
 nucliadb/reader/reader/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
 nucliadb/reader/reader/notifications.py,sha256=cPpcnyHr9prcsGvkq4JwZqHjbTEkpXVcPWoYA4Up5fU,8155
 nucliadb/reader/tests/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
 nucliadb/reader/tests/conftest.py,sha256=RH5huJVfSZ9cQgzEWC_xViGbXUelZFuHmrOnWb-FpEU,1224
 nucliadb/reader/tests/fixtures.py,sha256=pVrolKyIQaUA01Coe8WHG6OuliqREnzq8DJnnfPF8_k,4345
 nucliadb/reader/tests/test_list_resources.py,sha256=yKsG6MLh4_cB7Yhov0OoBAVCJCXnpuQmT453R1oVQ6Q,2748
 nucliadb/reader/tests/test_reader_file_download.py,sha256=V_wLTRmSlYemSPLOBo3A_jhMBluro2sJiQwSsGGBx6I,10199
@@ -204,40 +204,40 @@
 nucliadb/search/settings.py,sha256=Nm4BkdNNdYfU1wGvvWMvlazRSlRGoae99GEdm48-bXI,1193
 nucliadb/search/utilities.py,sha256=9SsRDw0rJVXVoLBfF7rBb6q080h-thZc7u8uRcTiBeY,1037
 nucliadb/search/api/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
 nucliadb/search/api/v1/__init__.py,sha256=JH9NGhhyRzirOYY5_pDx5zGZVvpU3317lygSbEb0MFk,1272
 nucliadb/search/api/v1/chat.py,sha256=dNaU4Cfkbta9-buRsPb98s1gsfvvzVCQIoYp2yvICmk,9913
 nucliadb/search/api/v1/feedback.py,sha256=j0PGSGDSbwwS5clRDbU_iCxuISFOtf2DN9Ey-fVGpso,2665
 nucliadb/search/api/v1/find.py,sha256=TvfV-KBUT52gpAgrWTtDOEkNTcKm69qma8mKl0p9mCQ,8804
-nucliadb/search/api/v1/knowledgebox.py,sha256=aWjGghS9uuxwOIbfRrRxEP6TXH5pIXxASG2utQMhGSk,7026
+nucliadb/search/api/v1/knowledgebox.py,sha256=hQ0wdBlHJVTwiRZgVCeNVwW_6f2bay88Hs9JMHgnx9M,6938
 nucliadb/search/api/v1/predict_proxy.py,sha256=2RME4enSpVXbNzboYQT1XhFFSgakDBgg3Wxj26mQglY,3041
 nucliadb/search/api/v1/router.py,sha256=mtT07rBZcVfpa49doaw9b1tj3sdi3qLH0gn9Io6NYM0,988
-nucliadb/search/api/v1/search.py,sha256=oVu-UevKCFU3-BrXoICBnNrIvfND4ENhivMpIoern2c,18359
+nucliadb/search/api/v1/search.py,sha256=M3NQ7xZDeWsEWpfZyNnivHj7NNk11K4rbbziqhj8Ihs,18325
 nucliadb/search/api/v1/suggest.py,sha256=zGNB-vFgwYUjp9vxBYr5KB2ucJhhhZJqK85tOUO6z0w,5928
 nucliadb/search/api/v1/summarize.py,sha256=-hzveoztY3Qy68V5bCbX07McG5TKFzCerA27rYOQW7o,2536
 nucliadb/search/api/v1/utils.py,sha256=zvZNUSYNjF28NnKdmBTwLbFF0kjzFUNIWaP3qCs3P9Q,1412
 nucliadb/search/api/v1/resource/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
 nucliadb/search/api/v1/resource/ask.py,sha256=9DXycgB0zXGjmZ9A51VVnJRkxI_tfL5LlT61-ADG6Es,6095
 nucliadb/search/api/v1/resource/chat.py,sha256=y3SIyr92oMQBrc5UKWsRLDFUCK3cgAKjxM0PBsNnu5Q,5887
 nucliadb/search/api/v1/resource/search.py,sha256=xIl_w70MpvC8Aqu89h4tXWNCZYaN9hxUUV04J1wK95w,5293
 nucliadb/search/requesters/__init__.py,sha256=itSI7dtTwFP55YMX4iK7JzdMHS5CQVUiB1XzQu4UBh8,833
 nucliadb/search/requesters/utils.py,sha256=UbWLBSIuZETkG0OoDDkL4XjC2Zmc5wWfofdJPufXmdw,9070
 nucliadb/search/search/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
 nucliadb/search/search/cache.py,sha256=86WwnknDYI00bd-kFf5MhN8TVFS2tfHzgobUHv_fAIA,2746
 nucliadb/search/search/exceptions.py,sha256=mbToQ-ghrv8ukLEv8S_-EZrgweWaIZZ5SIpoeuGDk6s,1154
 nucliadb/search/search/fetch.py,sha256=6S6s2s0JEP2QADDesbeN3XYPvTquMsTz9l0FKqQtSKU,5465
 nucliadb/search/search/filters.py,sha256=HpTpaDjKmUZWkp5xFFqKHz3TYdKEVBk4jWb2ssIYa5g,6513
-nucliadb/search/search/find.py,sha256=cnWh2yC6Zq0XNG0c0ciycFr1APobbCF1Fye4fatxSIc,4646
+nucliadb/search/search/find.py,sha256=_cGdIfSqpaxm01SqTbcQCQJtadeiL71HB4zEIBj1dM4,4612
 nucliadb/search/search/find_merge.py,sha256=vhq14MFE7N9-9SNlg66LNUr6YAhR9cW22oDpmjvQhL0,17152
 nucliadb/search/search/merge.py,sha256=-srmB1gZEuMa9c2_hLTD1ihjJwDhdB6wnp9b7ljxuIM,21282
 nucliadb/search/search/metrics.py,sha256=4xQm4Q0_-R1bgMtnrbm-YaClEFR8HE6wDk9lunCrhjo,1130
 nucliadb/search/search/paragraphs.py,sha256=8TTii45JvQ7SXsV9Z9ipt5QpYk7ux6PnlOkjKPfYz4A,8698
 nucliadb/search/search/predict_proxy.py,sha256=aOq1AzXkUdHtEmXsec07ffuMKGjlMu-NaUxb_IKme6U,3026
-nucliadb/search/search/query.py,sha256=LjJjhnm1_XLbo2KFMJYkUH9Z_svbrsEJvw-evRNSPyA,31300
-nucliadb/search/search/shards.py,sha256=CiQHBPR-_IjtfaC_897adddH4sRSxgfTEURuFpoMLQs,3149
+nucliadb/search/search/query.py,sha256=K7Q_lgeTRVsUT-vNCUGmbk_wOhSg2q1v9d8XYD6FJIE,31084
+nucliadb/search/search/shards.py,sha256=0p_BWLEVrK87htqhavZ2ixA2l253FPQnre3RpThtZco,3018
 nucliadb/search/search/summarize.py,sha256=bjncFFBv1R9g4OyhQSlGHFq5cJ8UvR8KrMgeKc-1AMU,5101
 nucliadb/search/search/utils.py,sha256=Gzjr9rFdwRfOgyDzX1Slz8DbcXLvavo0124S8II9omw,2438
 nucliadb/search/search/chat/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
 nucliadb/search/search/chat/images.py,sha256=AjPgCJaCzu19ruUJcEVaG_bEUmqzB65EH0mduMbkzAE,2058
 nucliadb/search/search/chat/prompt.py,sha256=W98mZrhrscjkxVJ02OM7veAQ1fjMrNDSZ1CUSaECCCk,20793
 nucliadb/search/search/chat/query.py,sha256=4wV6nwzNVA4skiUVM0ggBgdRR7BjYHZ801b87WAuIgI,15347
 nucliadb/search/tests/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
@@ -404,26 +404,25 @@
 nucliadb/writer/back_pressure.py,sha256=DPNeBVNQuRZzOEBMDmRIoeLDEuvRwwIGFBKNOQg3-xE,19495
 nucliadb/writer/exceptions.py,sha256=2dMvuoF68v3BZuyzaBEsbG6gusQqwLFcn47qm1zNdTc,972
 nucliadb/writer/lifecycle.py,sha256=gF9it0w98uBGCwzjs72e8mGi6H-qv_XAa2GGNBTOEDY,1953
 nucliadb/writer/openapi.py,sha256=thqCO1ht_RJgOkXs-aIsv8aXJrU5z8wo2n05l2_LqMs,1032
 nucliadb/writer/run.py,sha256=euVZ_rtHDXs-O1kB-Pt1Id8eft9CYVpWH3zJzEoEqls,1448
 nucliadb/writer/settings.py,sha256=A1JY7pFQzLPV0Vm0TSG6jPBR3dEMK76SknbeANTG4Hg,3074
 nucliadb/writer/utilities.py,sha256=AZ5qEny1Xm0IDsFtH13oJa2usvJZK8f0FdgF1LrnLCw,1036
-nucliadb/writer/vectors.py,sha256=cqiBtqAVTpG2kvR7VKUrhLfH8XQS8wEdE1q-CxVnhEw,1948
 nucliadb/writer/api/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
 nucliadb/writer/api/constants.py,sha256=b63uWvu7_bwg51R6EL5DaJwoT550Ih4GhVXzvEYLQNQ,1429
 nucliadb/writer/api/v1/__init__.py,sha256=FVn7N9VJ6bsEoy4TRnkclr4Umd5hECiwPXVqRnJ8BME,1095
 nucliadb/writer/api/v1/export_import.py,sha256=LrGg7y5Aq8xEnoYr529HG0g9LcF2UjP1VFpk9z1pJfE,6565
 nucliadb/writer/api/v1/field.py,sha256=PNHaaO37WRW2FxCaYq-PqthLPu0lOZdmrWX_R7axToc,28578
 nucliadb/writer/api/v1/knowledgebox.py,sha256=sFPPOsB2z-ljV51JP7oHMxUjejnJXMw93Pq8i-EMRkg,5239
 nucliadb/writer/api/v1/learning_config.py,sha256=GQN2d2N2IJLPX-S7hddTgrb7fDE8gCJ1MghgsIjBPKA,2052
 nucliadb/writer/api/v1/resource.py,sha256=x3hi_n4i9syK67v9LWdQZxGBImmnd95Rd7i2OqUHSW8,19940
 nucliadb/writer/api/v1/router.py,sha256=RjuoWLpZer6Kl2BW_wznpNo6XL3BOpdTGqXZCn3QrrQ,1034
-nucliadb/writer/api/v1/services.py,sha256=l7mNQVRTCoGem1fR8p2NYb6l3rLaWp9MMFlwaXONbFU,12733
-nucliadb/writer/api/v1/upload.py,sha256=zjmMbINM5_HW0e94I2cXpBrpv53yBtnTFoOqBXILDIo,31592
+nucliadb/writer/api/v1/services.py,sha256=vzE0ABaPHBpczxqDuDwpcUIF4OyOKIVhWZMtYDPEAo0,10726
+nucliadb/writer/api/v1/upload.py,sha256=q5V3XB2HoU7MDpGqP-tETnJkKQMtwUm3FWYxIz7xyok,31701
 nucliadb/writer/layouts/__init__.py,sha256=Siod9W963CG5gJa20GSTw9VemAFgsMmJDbUspbrYAyE,1612
 nucliadb/writer/layouts/v1.py,sha256=Yc2idmfrpCS8js_XJByNWA_tmt2WeKoWvidLHoTPXoo,2115
 nucliadb/writer/resource/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
 nucliadb/writer/resource/audit.py,sha256=SXPu_hdNBlm9uCSl666UQL7hzMx9zYVbBLT_U7ro8Gs,1425
 nucliadb/writer/resource/basic.py,sha256=eSWW6u6U3e0KjjdFwp9YQokojoDepl5vmJfbE2MQACM,10968
 nucliadb/writer/resource/field.py,sha256=7Y1vfuKDv1b3e7NCjEvDg8mktGR1rnzHaC5_qNj-3YQ,16319
 nucliadb/writer/resource/origin.py,sha256=3Y2zVtG_v0U6uMbDhW9Yl7KKHKt5V3T5_v3iCpqdBEk,2022
@@ -431,26 +430,26 @@
 nucliadb/writer/tests/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
 nucliadb/writer/tests/conftest.py,sha256=bmFKnuaqRqMCjtTp6c4V4R-qF59OPu0gW8-hp1TXFwk,1200
 nucliadb/writer/tests/fixtures.py,sha256=Ni66Iq-A6W8qqa6V6PwSzDq2BD9IINXlGexilVaDzPU,5971
 nucliadb/writer/tests/test_fields.py,sha256=fbzN0Bgu8HOLAqqYXO15JIqXN1bxr7mTTCTUuYhG85c,15472
 nucliadb/writer/tests/test_files.py,sha256=iIjpz04z7JHJ_woymNqE4P-BMJfn_CE9Wh2Fi30SbJk,25913
 nucliadb/writer/tests/test_knowledgebox.py,sha256=KPUGr4TsmHXSTfte40rY18ANUHaUYs_TD4DXCIlawt8,1729
 nucliadb/writer/tests/test_reprocess_file_field.py,sha256=4vq9ox-R0zlyIlX2fdaPLfNK64mdPU1r4ELM4of5PD8,4569
-nucliadb/writer/tests/test_resources.py,sha256=5HO5207B_bhP9HtJmlGKHjFw5pz-euBDnz1AH9uAa7Y,17449
+nucliadb/writer/tests/test_resources.py,sha256=l7i9dEh_Qb2f-4-gz9SpCI_f9RWJlYDSYddjkAoOvSg,16938
 nucliadb/writer/tests/test_service.py,sha256=bfV1qQVL5fq6w9NznllqLN8LS3hxRYsBjT2bs_rHWV4,5120
 nucliadb/writer/tests/test_tus.py,sha256=Dy98EhBCcmDSXlNfoPiQnLElTi1KEdybjVk8MtIAlJw,6054
 nucliadb/writer/tests/utils.py,sha256=eSyyTCMERC-EzeBrBAurSIZCpqgH67wc1wHZ1KjO1DM,1287
 nucliadb/writer/tus/__init__.py,sha256=J6d-4FHwJ_2DxYGWRtX2RBoPETW-fmBQp-sgVChaOJY,5226
 nucliadb/writer/tus/dm.py,sha256=VYTy56vU52W9QfX5ilDfRSUiCq3IgC81xs2Vcai5Thc,5082
 nucliadb/writer/tus/exceptions.py,sha256=CmxYKnHXpXug25DYV4SpVAU47SGD-NVBd7pNTRbWHyk,2186
 nucliadb/writer/tus/gcs.py,sha256=WykJZicWKRYkVB5_Fkb_1cVLovAk86IVkEn1VgEDufc,14527
 nucliadb/writer/tus/local.py,sha256=lIOoGaylnsxPBYGskcmKSHv7MsvwIYFS4soDLey_KSs,5849
 nucliadb/writer/tus/pg.py,sha256=JUK_xKsyNcKAvWOch8gUMTc_e1evI_3aC6-Y5gMk2jw,4367
 nucliadb/writer/tus/s3.py,sha256=a9mfPtjBW3QaTYY2r6P7u_Y13V6mBefZjWgV4juZzgE,9069
 nucliadb/writer/tus/storage.py,sha256=8iBOjWIcY6PawQq_rmSiBKi0Gl6J6Q5ad6L-9nLCcJ4,4734
 nucliadb/writer/tus/utils.py,sha256=MSdVbRsRSZVdkaum69_0wku7X3p5wlZf4nr6E0GMKbw,2556
-nucliadb-3.0.3.post450.dist-info/METADATA,sha256=KdylbRdtE430_pgkXKAoPZVoE600MkQCYhEZpkz-RpQ,4343
-nucliadb-3.0.3.post450.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-nucliadb-3.0.3.post450.dist-info/entry_points.txt,sha256=XqGfgFDuY3zXQc8ewXM2TRVjTModIq851zOsgrmaXx4,1268
-nucliadb-3.0.3.post450.dist-info/top_level.txt,sha256=hwYhTVnX7jkQ9gJCkVrbqEG1M4lT2F_iPQND1fCzF80,20
-nucliadb-3.0.3.post450.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-nucliadb-3.0.3.post450.dist-info/RECORD,,
+nucliadb-3.0.3.post454.dist-info/METADATA,sha256=9rGsw9MzvVl43tFKhJ0nw7_yRtJSsD6We50J2j5jjZc,4343
+nucliadb-3.0.3.post454.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+nucliadb-3.0.3.post454.dist-info/entry_points.txt,sha256=XqGfgFDuY3zXQc8ewXM2TRVjTModIq851zOsgrmaXx4,1268
+nucliadb-3.0.3.post454.dist-info/top_level.txt,sha256=hwYhTVnX7jkQ9gJCkVrbqEG1M4lT2F_iPQND1fCzF80,20
+nucliadb-3.0.3.post454.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
+nucliadb-3.0.3.post454.dist-info/RECORD,,
```


# Comparing `tmp/nucliadb-4.0.0.post539-py3-none-any.whl.zip` & `tmp/nucliadb-4.0.0.post540-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,464 +1,464 @@
-Zip file size: 765220 bytes, number of entries: 462
--rw-r--r--  2.0 unx     1135 b- defN 24-May-23 10:56 migrations/0001_bootstrap.py
--rw-r--r--  2.0 unx     1177 b- defN 24-May-23 10:56 migrations/0002_rollover_shards.py
--rw-r--r--  2.0 unx     2436 b- defN 24-May-23 10:56 migrations/0003_allfields_key.py
--rw-r--r--  2.0 unx     1177 b- defN 24-May-23 10:56 migrations/0004_rollover_shards.py
--rw-r--r--  2.0 unx     1177 b- defN 24-May-23 10:56 migrations/0005_rollover_shards.py
--rw-r--r--  2.0 unx     1024 b- defN 24-May-23 10:56 migrations/0006_rollover_shards.py
--rw-r--r--  2.0 unx     1301 b- defN 24-May-23 10:56 migrations/0008_cleanup_leftover_rollover_metadata.py
--rw-r--r--  2.0 unx     1378 b- defN 24-May-23 10:56 migrations/0009_upgrade_relations_and_texts_to_v2.py
--rw-r--r--  2.0 unx     1610 b- defN 24-May-23 10:56 migrations/0010_fix_corrupt_indexes.py
--rw-r--r--  2.0 unx     1843 b- defN 24-May-23 10:56 migrations/0011_materialize_labelset_ids.py
--rw-r--r--  2.0 unx     1443 b- defN 24-May-23 10:56 migrations/0012_rollover_shards.py
--rw-r--r--  2.0 unx     1024 b- defN 24-May-23 10:56 migrations/0013_rollover_shards.py
--rw-r--r--  2.0 unx     1382 b- defN 24-May-23 10:56 migrations/0014_rollover_shards.py
--rw-r--r--  2.0 unx     1462 b- defN 24-May-23 10:56 migrations/0015_targeted_rollover.py
--rw-r--r--  2.0 unx     2506 b- defN 24-May-23 10:56 migrations/0016_upgrade_to_paragraphs_v2.py
--rw-r--r--  2.0 unx     2100 b- defN 24-May-23 10:56 migrations/0017_multiple_writable_shards.py
--rw-r--r--  2.0 unx     2264 b- defN 24-May-23 10:56 migrations/0018_purge_orphan_kbslugs.py
--rw-r--r--  2.0 unx     2506 b- defN 24-May-23 10:56 migrations/0019_upgrade_to_paragraphs_v3.py
--rw-r--r--  2.0 unx     3282 b- defN 24-May-23 10:56 migrations/0020_drain_nodes_from_cluster.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-23 10:56 migrations/__init__.py
--rw-r--r--  2.0 unx      891 b- defN 24-May-23 10:56 nucliadb/__init__.py
--rw-r--r--  2.0 unx     3733 b- defN 24-May-23 10:56 nucliadb/health.py
--rw-r--r--  2.0 unx    11639 b- defN 24-May-23 10:56 nucliadb/learning_proxy.py
--rw-r--r--  2.0 unx     4806 b- defN 24-May-23 10:56 nucliadb/metrics_exporter.py
--rw-r--r--  2.0 unx     2272 b- defN 24-May-23 10:56 nucliadb/openapi.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-23 10:56 nucliadb/py.typed
--rw-r--r--  2.0 unx      835 b- defN 24-May-23 10:56 nucliadb/common/__init__.py
--rw-r--r--  2.0 unx     5175 b- defN 24-May-23 10:56 nucliadb/common/locking.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-23 10:56 nucliadb/common/cluster/__init__.py
--rw-r--r--  2.0 unx     5080 b- defN 24-May-23 10:56 nucliadb/common/cluster/base.py
--rw-r--r--  2.0 unx     1495 b- defN 24-May-23 10:56 nucliadb/common/cluster/exceptions.py
--rw-r--r--  2.0 unx     3793 b- defN 24-May-23 10:56 nucliadb/common/cluster/grpc_node_dummy.py
--rw-r--r--  2.0 unx     3429 b- defN 24-May-23 10:56 nucliadb/common/cluster/index_node.py
--rw-r--r--  2.0 unx    22091 b- defN 24-May-23 10:56 nucliadb/common/cluster/manager.py
--rw-r--r--  2.0 unx     8853 b- defN 24-May-23 10:56 nucliadb/common/cluster/rebalance.py
--rw-r--r--  2.0 unx    20209 b- defN 24-May-23 10:56 nucliadb/common/cluster/rollover.py
--rw-r--r--  2.0 unx     3016 b- defN 24-May-23 10:56 nucliadb/common/cluster/settings.py
--rw-r--r--  2.0 unx     5713 b- defN 24-May-23 10:56 nucliadb/common/cluster/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-23 10:56 nucliadb/common/cluster/discovery/__init__.py
--rw-r--r--  2.0 unx     6553 b- defN 24-May-23 10:56 nucliadb/common/cluster/discovery/base.py
--rw-r--r--  2.0 unx    12512 b- defN 24-May-23 10:56 nucliadb/common/cluster/discovery/k8s.py
--rw-r--r--  2.0 unx     1957 b- defN 24-May-23 10:56 nucliadb/common/cluster/discovery/manual.py
--rw-r--r--  2.0 unx     1737 b- defN 24-May-23 10:56 nucliadb/common/cluster/discovery/single.py
--rw-r--r--  2.0 unx     1139 b- defN 24-May-23 10:56 nucliadb/common/cluster/discovery/types.py
--rw-r--r--  2.0 unx     2548 b- defN 24-May-23 10:56 nucliadb/common/cluster/discovery/utils.py
--rw-r--r--  2.0 unx      833 b- defN 24-May-23 10:56 nucliadb/common/cluster/standalone/__init__.py
--rw-r--r--  2.0 unx    13712 b- defN 24-May-23 10:56 nucliadb/common/cluster/standalone/grpc_node_binding.py
--rw-r--r--  2.0 unx     4683 b- defN 24-May-23 10:56 nucliadb/common/cluster/standalone/index_node.py
--rw-r--r--  2.0 unx     3444 b- defN 24-May-23 10:56 nucliadb/common/cluster/standalone/service.py
--rw-r--r--  2.0 unx     3545 b- defN 24-May-23 10:56 nucliadb/common/cluster/standalone/utils.py
--rw-r--r--  2.0 unx     3440 b- defN 24-May-23 10:56 nucliadb/common/context/__init__.py
--rw-r--r--  2.0 unx     1628 b- defN 24-May-23 10:56 nucliadb/common/context/fastapi.py
--rw-r--r--  2.0 unx     1880 b- defN 24-May-23 10:56 nucliadb/common/datamanagers/__init__.py
--rw-r--r--  2.0 unx     1451 b- defN 24-May-23 10:56 nucliadb/common/datamanagers/cluster.py
--rw-r--r--  2.0 unx     5383 b- defN 24-May-23 10:56 nucliadb/common/datamanagers/entities.py
--rw-r--r--  2.0 unx      883 b- defN 24-May-23 10:56 nucliadb/common/datamanagers/exceptions.py
--rw-r--r--  2.0 unx     3994 b- defN 24-May-23 10:56 nucliadb/common/datamanagers/kb.py
--rw-r--r--  2.0 unx     5389 b- defN 24-May-23 10:56 nucliadb/common/datamanagers/labels.py
--rw-r--r--  2.0 unx     1599 b- defN 24-May-23 10:56 nucliadb/common/datamanagers/processing.py
--rw-r--r--  2.0 unx    12177 b- defN 24-May-23 10:56 nucliadb/common/datamanagers/resources.py
--rw-r--r--  2.0 unx     5634 b- defN 24-May-23 10:56 nucliadb/common/datamanagers/rollover.py
--rw-r--r--  2.0 unx     1548 b- defN 24-May-23 10:56 nucliadb/common/datamanagers/synonyms.py
--rw-r--r--  2.0 unx     1631 b- defN 24-May-23 10:56 nucliadb/common/datamanagers/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-23 10:56 nucliadb/common/http_clients/__init__.py
--rw-r--r--  2.0 unx     2146 b- defN 24-May-23 10:56 nucliadb/common/http_clients/auth.py
--rw-r--r--  2.0 unx     1100 b- defN 24-May-23 10:56 nucliadb/common/http_clients/exceptions.py
--rw-r--r--  2.0 unx     7155 b- defN 24-May-23 10:56 nucliadb/common/http_clients/processing.py
--rw-r--r--  2.0 unx     1540 b- defN 24-May-23 10:56 nucliadb/common/http_clients/pypi.py
--rw-r--r--  2.0 unx     1551 b- defN 24-May-23 10:56 nucliadb/common/http_clients/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-23 10:56 nucliadb/common/maindb/__init__.py
--rw-r--r--  2.0 unx     3449 b- defN 24-May-23 10:56 nucliadb/common/maindb/driver.py
--rw-r--r--  2.0 unx      946 b- defN 24-May-23 10:56 nucliadb/common/maindb/exceptions.py
--rw-r--r--  2.0 unx     6769 b- defN 24-May-23 10:56 nucliadb/common/maindb/local.py
--rw-r--r--  2.0 unx     8391 b- defN 24-May-23 10:56 nucliadb/common/maindb/pg.py
--rw-r--r--  2.0 unx     6053 b- defN 24-May-23 10:56 nucliadb/common/maindb/redis.py
--rw-r--r--  2.0 unx    14502 b- defN 24-May-23 10:56 nucliadb/common/maindb/tikv.py
--rw-r--r--  2.0 unx     4167 b- defN 24-May-23 10:56 nucliadb/common/maindb/utils.py
--rw-r--r--  2.0 unx      932 b- defN 24-May-23 10:56 nucliadb/export_import/__init__.py
--rw-r--r--  2.0 unx     6171 b- defN 24-May-23 10:56 nucliadb/export_import/datamanager.py
--rw-r--r--  2.0 unx     1949 b- defN 24-May-23 10:56 nucliadb/export_import/exceptions.py
--rw-r--r--  2.0 unx     7116 b- defN 24-May-23 10:56 nucliadb/export_import/exporter.py
--rw-r--r--  2.0 unx     4258 b- defN 24-May-23 10:56 nucliadb/export_import/importer.py
--rw-r--r--  2.0 unx     2063 b- defN 24-May-23 10:56 nucliadb/export_import/models.py
--rw-r--r--  2.0 unx     2571 b- defN 24-May-23 10:56 nucliadb/export_import/tasks.py
--rw-r--r--  2.0 unx    19401 b- defN 24-May-23 10:56 nucliadb/export_import/utils.py
--rw-r--r--  2.0 unx     1011 b- defN 24-May-23 10:56 nucliadb/ingest/__init__.py
--rw-r--r--  2.0 unx     7277 b- defN 24-May-23 10:56 nucliadb/ingest/app.py
--rw-r--r--  2.0 unx     1005 b- defN 24-May-23 10:56 nucliadb/ingest/cache.py
--rw-r--r--  2.0 unx     2484 b- defN 24-May-23 10:56 nucliadb/ingest/partitions.py
--rw-r--r--  2.0 unx    19904 b- defN 24-May-23 10:56 nucliadb/ingest/processing.py
--rw-r--r--  2.0 unx    20277 b- defN 24-May-23 10:56 nucliadb/ingest/serialize.py
--rw-r--r--  2.0 unx     3207 b- defN 24-May-23 10:56 nucliadb/ingest/settings.py
--rw-r--r--  2.0 unx     2314 b- defN 24-May-23 10:56 nucliadb/ingest/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-23 10:56 nucliadb/ingest/consumer/__init__.py
--rw-r--r--  2.0 unx     6918 b- defN 24-May-23 10:56 nucliadb/ingest/consumer/auditing.py
--rw-r--r--  2.0 unx    12174 b- defN 24-May-23 10:56 nucliadb/ingest/consumer/consumer.py
--rw-r--r--  2.0 unx     3945 b- defN 24-May-23 10:56 nucliadb/ingest/consumer/materializer.py
--rw-r--r--  2.0 unx     1075 b- defN 24-May-23 10:56 nucliadb/ingest/consumer/metrics.py
--rw-r--r--  2.0 unx     9543 b- defN 24-May-23 10:56 nucliadb/ingest/consumer/pull.py
--rw-r--r--  2.0 unx     6871 b- defN 24-May-23 10:56 nucliadb/ingest/consumer/service.py
--rw-r--r--  2.0 unx     4331 b- defN 24-May-23 10:56 nucliadb/ingest/consumer/shard_creator.py
--rw-r--r--  2.0 unx     2656 b- defN 24-May-23 10:56 nucliadb/ingest/consumer/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-23 10:56 nucliadb/ingest/fields/__init__.py
--rw-r--r--  2.0 unx    17461 b- defN 24-May-23 10:56 nucliadb/ingest/fields/base.py
--rw-r--r--  2.0 unx     6516 b- defN 24-May-23 10:56 nucliadb/ingest/fields/conversation.py
--rw-r--r--  2.0 unx     1223 b- defN 24-May-23 10:56 nucliadb/ingest/fields/date.py
--rw-r--r--  2.0 unx     1205 b- defN 24-May-23 10:56 nucliadb/ingest/fields/exceptions.py
--rw-r--r--  2.0 unx     4840 b- defN 24-May-23 10:56 nucliadb/ingest/fields/file.py
--rw-r--r--  2.0 unx     1547 b- defN 24-May-23 10:56 nucliadb/ingest/fields/generic.py
--rw-r--r--  2.0 unx     1235 b- defN 24-May-23 10:56 nucliadb/ingest/fields/keywordset.py
--rw-r--r--  2.0 unx     2250 b- defN 24-May-23 10:56 nucliadb/ingest/fields/layout.py
--rw-r--r--  2.0 unx     4212 b- defN 24-May-23 10:56 nucliadb/ingest/fields/link.py
--rw-r--r--  2.0 unx     1319 b- defN 24-May-23 10:56 nucliadb/ingest/fields/text.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-23 10:56 nucliadb/ingest/orm/__init__.py
--rw-r--r--  2.0 unx    28311 b- defN 24-May-23 10:56 nucliadb/ingest/orm/brain.py
--rw-r--r--  2.0 unx    15758 b- defN 24-May-23 10:56 nucliadb/ingest/orm/entities.py
--rw-r--r--  2.0 unx     1279 b- defN 24-May-23 10:56 nucliadb/ingest/orm/exceptions.py
--rw-r--r--  2.0 unx    15621 b- defN 24-May-23 10:56 nucliadb/ingest/orm/knowledgebox.py
--rw-r--r--  2.0 unx     1096 b- defN 24-May-23 10:56 nucliadb/ingest/orm/metrics.py
--rw-r--r--  2.0 unx    58955 b- defN 24-May-23 10:56 nucliadb/ingest/orm/resource.py
--rw-r--r--  2.0 unx     2685 b- defN 24-May-23 10:56 nucliadb/ingest/orm/utils.py
--rw-r--r--  2.0 unx    27042 b- defN 24-May-23 10:56 nucliadb/ingest/orm/processor/__init__.py
--rw-r--r--  2.0 unx     5090 b- defN 24-May-23 10:56 nucliadb/ingest/orm/processor/auditing.py
--rw-r--r--  2.0 unx     1690 b- defN 24-May-23 10:56 nucliadb/ingest/orm/processor/sequence_manager.py
--rw-r--r--  2.0 unx     2057 b- defN 24-May-23 10:56 nucliadb/ingest/service/__init__.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-23 10:56 nucliadb/ingest/service/exceptions.py
--rw-r--r--  2.0 unx    30462 b- defN 24-May-23 10:56 nucliadb/ingest/service/writer.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-23 10:56 nucliadb/ingest/tests/__init__.py
--rw-r--r--  2.0 unx     1157 b- defN 24-May-23 10:56 nucliadb/ingest/tests/conftest.py
--rw-r--r--  2.0 unx    24060 b- defN 24-May-23 10:56 nucliadb/ingest/tests/fixtures.py
--rw-r--r--  2.0 unx    62843 b- defN 24-May-23 10:56 nucliadb/ingest/tests/vectors.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-23 10:56 nucliadb/ingest/tests/integration/__init__.py
--rw-r--r--  2.0 unx      833 b- defN 24-May-23 10:56 nucliadb/ingest/tests/integration/consumer/__init__.py
--rw-r--r--  2.0 unx     2500 b- defN 24-May-23 10:56 nucliadb/ingest/tests/integration/consumer/test_auditing.py
--rw-r--r--  2.0 unx     3832 b- defN 24-May-23 10:56 nucliadb/ingest/tests/integration/consumer/test_materializer.py
--rw-r--r--  2.0 unx     4470 b- defN 24-May-23 10:56 nucliadb/ingest/tests/integration/consumer/test_pull.py
--rw-r--r--  2.0 unx     2763 b- defN 24-May-23 10:56 nucliadb/ingest/tests/integration/consumer/test_service.py
--rw-r--r--  2.0 unx     2019 b- defN 24-May-23 10:56 nucliadb/ingest/tests/integration/consumer/test_shard_creator.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-23 10:56 nucliadb/ingest/tests/integration/ingest/__init__.py
--rw-r--r--  2.0 unx    27247 b- defN 24-May-23 10:56 nucliadb/ingest/tests/integration/ingest/test_ingest.py
--rw-r--r--  2.0 unx     3040 b- defN 24-May-23 10:56 nucliadb/ingest/tests/integration/ingest/test_processing_engine.py
--rw-r--r--  2.0 unx     8586 b- defN 24-May-23 10:56 nucliadb/ingest/tests/integration/ingest/test_relations.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-23 10:56 nucliadb/ingest/tests/unit/__init__.py
--rw-r--r--  2.0 unx     1189 b- defN 24-May-23 10:56 nucliadb/ingest/tests/unit/test_cache.py
--rw-r--r--  2.0 unx     1432 b- defN 24-May-23 10:56 nucliadb/ingest/tests/unit/test_partitions.py
--rw-r--r--  2.0 unx     5807 b- defN 24-May-23 10:56 nucliadb/ingest/tests/unit/test_processing.py
--rw-r--r--  2.0 unx      978 b- defN 24-May-23 10:56 nucliadb/ingest/tests/unit/test_settings.py
--rw-r--r--  2.0 unx      833 b- defN 24-May-23 10:56 nucliadb/ingest/tests/unit/consumer/__init__.py
--rw-r--r--  2.0 unx     3885 b- defN 24-May-23 10:56 nucliadb/ingest/tests/unit/consumer/test_auditing.py
--rw-r--r--  2.0 unx     2472 b- defN 24-May-23 10:56 nucliadb/ingest/tests/unit/consumer/test_consumer.py
--rw-r--r--  2.0 unx     2063 b- defN 24-May-23 10:56 nucliadb/ingest/tests/unit/consumer/test_pull.py
--rw-r--r--  2.0 unx     4140 b- defN 24-May-23 10:56 nucliadb/ingest/tests/unit/consumer/test_shard_creator.py
--rw-r--r--  2.0 unx     1934 b- defN 24-May-23 10:56 nucliadb/ingest/tests/unit/consumer/test_utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-23 10:56 nucliadb/ingest/tests/unit/orm/__init__.py
--rw-r--r--  2.0 unx     9876 b- defN 24-May-23 10:56 nucliadb/ingest/tests/unit/orm/test_brain.py
--rw-r--r--  2.0 unx     2435 b- defN 24-May-23 10:56 nucliadb/ingest/tests/unit/orm/test_brain_vectors.py
--rw-r--r--  2.0 unx     1174 b- defN 24-May-23 10:56 nucliadb/ingest/tests/unit/orm/test_orm_utils.py
--rw-r--r--  2.0 unx     4045 b- defN 24-May-23 10:56 nucliadb/ingest/tests/unit/orm/test_processor.py
--rw-r--r--  2.0 unx    11033 b- defN 24-May-23 10:56 nucliadb/ingest/tests/unit/orm/test_resource.py
--rw-r--r--  2.0 unx     2216 b- defN 24-May-23 10:56 nucliadb/middleware/__init__.py
--rw-r--r--  2.0 unx     3912 b- defN 24-May-23 10:56 nucliadb/middleware/transaction.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-23 10:56 nucliadb/migrator/__init__.py
--rw-r--r--  2.0 unx     2119 b- defN 24-May-23 10:56 nucliadb/migrator/command.py
--rw-r--r--  2.0 unx     1334 b- defN 24-May-23 10:56 nucliadb/migrator/context.py
--rw-r--r--  2.0 unx     5104 b- defN 24-May-23 10:56 nucliadb/migrator/datamanager.py
--rw-r--r--  2.0 unx      889 b- defN 24-May-23 10:56 nucliadb/migrator/exceptions.py
--rw-r--r--  2.0 unx     9370 b- defN 24-May-23 10:56 nucliadb/migrator/migrator.py
--rw-r--r--  2.0 unx     1145 b- defN 24-May-23 10:56 nucliadb/migrator/models.py
--rw-r--r--  2.0 unx     1144 b- defN 24-May-23 10:56 nucliadb/migrator/settings.py
--rw-r--r--  2.0 unx     2346 b- defN 24-May-23 10:56 nucliadb/migrator/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-23 10:56 nucliadb/models/__init__.py
--rw-r--r--  2.0 unx     1599 b- defN 24-May-23 10:56 nucliadb/models/responses.py
--rw-r--r--  2.0 unx     6041 b- defN 24-May-23 10:56 nucliadb/purge/__init__.py
--rw-r--r--  2.0 unx     9364 b- defN 24-May-23 10:56 nucliadb/purge/orphan_shards.py
--rw-r--r--  2.0 unx     1328 b- defN 24-May-23 10:56 nucliadb/reader/__init__.py
--rw-r--r--  2.0 unx     3709 b- defN 24-May-23 10:56 nucliadb/reader/app.py
--rw-r--r--  2.0 unx     1366 b- defN 24-May-23 10:56 nucliadb/reader/lifecycle.py
--rw-r--r--  2.0 unx     1031 b- defN 24-May-23 10:56 nucliadb/reader/openapi.py
--rw-r--r--  2.0 unx     1447 b- defN 24-May-23 10:56 nucliadb/reader/run.py
--rw-r--r--  2.0 unx      872 b- defN 24-May-23 10:56 nucliadb/reader/api/__init__.py
--rw-r--r--  2.0 unx     2458 b- defN 24-May-23 10:56 nucliadb/reader/api/models.py
--rw-r--r--  2.0 unx     1110 b- defN 24-May-23 10:56 nucliadb/reader/api/v1/__init__.py
--rw-r--r--  2.0 unx    12392 b- defN 24-May-23 10:56 nucliadb/reader/api/v1/download.py
--rw-r--r--  2.0 unx     6459 b- defN 24-May-23 10:56 nucliadb/reader/api/v1/export_import.py
--rw-r--r--  2.0 unx     3641 b- defN 24-May-23 10:56 nucliadb/reader/api/v1/knowledgebox.py
--rw-r--r--  2.0 unx     2099 b- defN 24-May-23 10:56 nucliadb/reader/api/v1/learning_collector.py
--rw-r--r--  2.0 unx     4472 b- defN 24-May-23 10:56 nucliadb/reader/api/v1/learning_config.py
--rw-r--r--  2.0 unx    13951 b- defN 24-May-23 10:56 nucliadb/reader/api/v1/resource.py
--rw-r--r--  2.0 unx     1011 b- defN 24-May-23 10:56 nucliadb/reader/api/v1/router.py
--rw-r--r--  2.0 unx    12115 b- defN 24-May-23 10:56 nucliadb/reader/api/v1/services.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-23 10:56 nucliadb/reader/reader/__init__.py
--rw-r--r--  2.0 unx     7979 b- defN 24-May-23 10:56 nucliadb/reader/reader/notifications.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-23 10:56 nucliadb/reader/tests/__init__.py
--rw-r--r--  2.0 unx     1224 b- defN 24-May-23 10:56 nucliadb/reader/tests/conftest.py
--rw-r--r--  2.0 unx     4345 b- defN 24-May-23 10:56 nucliadb/reader/tests/fixtures.py
--rw-r--r--  2.0 unx     2748 b- defN 24-May-23 10:56 nucliadb/reader/tests/test_list_resources.py
--rw-r--r--  2.0 unx    10199 b- defN 24-May-23 10:56 nucliadb/reader/tests/test_reader_file_download.py
--rw-r--r--  2.0 unx    10586 b- defN 24-May-23 10:56 nucliadb/reader/tests/test_reader_resource.py
--rw-r--r--  2.0 unx     6535 b- defN 24-May-23 10:56 nucliadb/reader/tests/test_reader_resource_field.py
--rw-r--r--  2.0 unx     1535 b- defN 24-May-23 10:56 nucliadb/search/__init__.py
--rw-r--r--  2.0 unx     4905 b- defN 24-May-23 10:56 nucliadb/search/app.py
--rw-r--r--  2.0 unx     1956 b- defN 24-May-23 10:56 nucliadb/search/lifecycle.py
--rw-r--r--  2.0 unx     1016 b- defN 24-May-23 10:56 nucliadb/search/openapi.py
--rw-r--r--  2.0 unx    20665 b- defN 24-May-23 10:56 nucliadb/search/predict.py
--rw-r--r--  2.0 unx     1402 b- defN 24-May-23 10:56 nucliadb/search/run.py
--rw-r--r--  2.0 unx     1193 b- defN 24-May-23 10:56 nucliadb/search/settings.py
--rw-r--r--  2.0 unx     1037 b- defN 24-May-23 10:56 nucliadb/search/utilities.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-23 10:56 nucliadb/search/api/__init__.py
--rw-r--r--  2.0 unx     1298 b- defN 24-May-23 10:56 nucliadb/search/api/v1/__init__.py
--rw-r--r--  2.0 unx     3534 b- defN 24-May-23 10:56 nucliadb/search/api/v1/ask.py
--rw-r--r--  2.0 unx     9493 b- defN 24-May-23 10:56 nucliadb/search/api/v1/chat.py
--rw-r--r--  2.0 unx     2668 b- defN 24-May-23 10:56 nucliadb/search/api/v1/feedback.py
--rw-r--r--  2.0 unx     8795 b- defN 24-May-23 10:56 nucliadb/search/api/v1/find.py
--rw-r--r--  2.0 unx     6938 b- defN 24-May-23 10:56 nucliadb/search/api/v1/knowledgebox.py
--rw-r--r--  2.0 unx     3047 b- defN 24-May-23 10:56 nucliadb/search/api/v1/predict_proxy.py
--rw-r--r--  2.0 unx      988 b- defN 24-May-23 10:56 nucliadb/search/api/v1/router.py
--rw-r--r--  2.0 unx    19262 b- defN 24-May-23 10:56 nucliadb/search/api/v1/search.py
--rw-r--r--  2.0 unx     5970 b- defN 24-May-23 10:56 nucliadb/search/api/v1/suggest.py
--rw-r--r--  2.0 unx     2499 b- defN 24-May-23 10:56 nucliadb/search/api/v1/summarize.py
--rw-r--r--  2.0 unx     1434 b- defN 24-May-23 10:56 nucliadb/search/api/v1/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-23 10:56 nucliadb/search/api/v1/resource/__init__.py
--rw-r--r--  2.0 unx     4064 b- defN 24-May-23 10:56 nucliadb/search/api/v1/resource/ask.py
--rw-r--r--  2.0 unx     5821 b- defN 24-May-23 10:56 nucliadb/search/api/v1/resource/chat.py
--rw-r--r--  2.0 unx     5303 b- defN 24-May-23 10:56 nucliadb/search/api/v1/resource/search.py
--rw-r--r--  2.0 unx      833 b- defN 24-May-23 10:56 nucliadb/search/requesters/__init__.py
--rw-r--r--  2.0 unx     9111 b- defN 24-May-23 10:56 nucliadb/search/requesters/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-23 10:56 nucliadb/search/search/__init__.py
--rw-r--r--  2.0 unx     2746 b- defN 24-May-23 10:56 nucliadb/search/search/cache.py
--rw-r--r--  2.0 unx     1154 b- defN 24-May-23 10:56 nucliadb/search/search/exceptions.py
--rw-r--r--  2.0 unx     5465 b- defN 24-May-23 10:56 nucliadb/search/search/fetch.py
--rw-r--r--  2.0 unx     6513 b- defN 24-May-23 10:56 nucliadb/search/search/filters.py
--rw-r--r--  2.0 unx     4612 b- defN 24-May-23 10:56 nucliadb/search/search/find.py
--rw-r--r--  2.0 unx    17152 b- defN 24-May-23 10:56 nucliadb/search/search/find_merge.py
--rw-r--r--  2.0 unx    21282 b- defN 24-May-23 10:56 nucliadb/search/search/merge.py
--rw-r--r--  2.0 unx     1130 b- defN 24-May-23 10:56 nucliadb/search/search/metrics.py
--rw-r--r--  2.0 unx     8698 b- defN 24-May-23 10:56 nucliadb/search/search/paragraphs.py
--rw-r--r--  2.0 unx     3026 b- defN 24-May-23 10:56 nucliadb/search/search/predict_proxy.py
--rw-r--r--  2.0 unx    31093 b- defN 24-May-23 10:56 nucliadb/search/search/query.py
--rw-r--r--  2.0 unx     3018 b- defN 24-May-23 10:56 nucliadb/search/search/shards.py
--rw-r--r--  2.0 unx     5101 b- defN 24-May-23 10:56 nucliadb/search/search/summarize.py
--rw-r--r--  2.0 unx     2438 b- defN 24-May-23 10:56 nucliadb/search/search/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-23 10:56 nucliadb/search/search/chat/__init__.py
--rw-r--r--  2.0 unx    16676 b- defN 24-May-23 10:56 nucliadb/search/search/chat/ask.py
--rw-r--r--  2.0 unx     2058 b- defN 24-May-23 10:56 nucliadb/search/search/chat/images.py
--rw-r--r--  2.0 unx    20793 b- defN 24-May-23 10:56 nucliadb/search/search/chat/prompt.py
--rw-r--r--  2.0 unx    17543 b- defN 24-May-23 10:56 nucliadb/search/search/chat/query.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-23 10:56 nucliadb/search/tests/__init__.py
--rw-r--r--  2.0 unx     1295 b- defN 24-May-23 10:56 nucliadb/search/tests/conftest.py
--rw-r--r--  2.0 unx     6578 b- defN 24-May-23 10:56 nucliadb/search/tests/fixtures.py
--rw-r--r--  2.0 unx    15480 b- defN 24-May-23 10:56 nucliadb/search/tests/node.py
--rw-r--r--  2.0 unx      833 b- defN 24-May-23 10:56 nucliadb/search/tests/unit/__init__.py
--rw-r--r--  2.0 unx     2649 b- defN 24-May-23 10:56 nucliadb/search/tests/unit/test_app.py
--rw-r--r--  2.0 unx     3374 b- defN 24-May-23 10:56 nucliadb/search/tests/unit/test_find_merge.py
--rw-r--r--  2.0 unx     1400 b- defN 24-May-23 10:56 nucliadb/search/tests/unit/test_merge.py
--rw-r--r--  2.0 unx    15721 b- defN 24-May-23 10:56 nucliadb/search/tests/unit/test_predict.py
--rw-r--r--  2.0 unx     1328 b- defN 24-May-23 10:56 nucliadb/search/tests/unit/test_run.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-23 10:56 nucliadb/search/tests/unit/api/__init__.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-23 10:56 nucliadb/search/tests/unit/api/v1/__init__.py
--rw-r--r--  2.0 unx     3759 b- defN 24-May-23 10:56 nucliadb/search/tests/unit/api/v1/test_ask.py
--rw-r--r--  2.0 unx     2966 b- defN 24-May-23 10:56 nucliadb/search/tests/unit/api/v1/test_chat.py
--rw-r--r--  2.0 unx     2865 b- defN 24-May-23 10:56 nucliadb/search/tests/unit/api/v1/test_predict_proxy.py
--rw-r--r--  2.0 unx     2901 b- defN 24-May-23 10:56 nucliadb/search/tests/unit/api/v1/test_summarize.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-23 10:56 nucliadb/search/tests/unit/api/v1/resource/__init__.py
--rw-r--r--  2.0 unx     3040 b- defN 24-May-23 10:56 nucliadb/search/tests/unit/api/v1/resource/test_chat.py
--rw-r--r--  2.0 unx      833 b- defN 24-May-23 10:56 nucliadb/search/tests/unit/search/__init__.py
--rw-r--r--  2.0 unx     8586 b- defN 24-May-23 10:56 nucliadb/search/tests/unit/search/test_chat_prompt.py
--rw-r--r--  2.0 unx     3736 b- defN 24-May-23 10:56 nucliadb/search/tests/unit/search/test_fetch.py
--rw-r--r--  2.0 unx     4306 b- defN 24-May-23 10:56 nucliadb/search/tests/unit/search/test_filters.py
--rw-r--r--  2.0 unx     4492 b- defN 24-May-23 10:56 nucliadb/search/tests/unit/search/test_paragraphs.py
--rw-r--r--  2.0 unx     3496 b- defN 24-May-23 10:56 nucliadb/search/tests/unit/search/test_predict_proxy.py
--rw-r--r--  2.0 unx     5121 b- defN 24-May-23 10:56 nucliadb/search/tests/unit/search/test_query.py
--rw-r--r--  2.0 unx      833 b- defN 24-May-23 10:56 nucliadb/search/tests/unit/search/requesters/__init__.py
--rw-r--r--  2.0 unx     6455 b- defN 24-May-23 10:56 nucliadb/search/tests/unit/search/requesters/test_utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-23 10:56 nucliadb/search/tests/unit/search/search/__init__.py
--rw-r--r--  2.0 unx     1759 b- defN 24-May-23 10:56 nucliadb/search/tests/unit/search/search/test_shards.py
--rw-r--r--  2.0 unx     2511 b- defN 24-May-23 10:56 nucliadb/search/tests/unit/search/search/test_utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-23 10:56 nucliadb/standalone/__init__.py
--rw-r--r--  2.0 unx     6746 b- defN 24-May-23 10:56 nucliadb/standalone/api_router.py
--rw-r--r--  2.0 unx     5763 b- defN 24-May-23 10:56 nucliadb/standalone/app.py
--rw-r--r--  2.0 unx     7800 b- defN 24-May-23 10:56 nucliadb/standalone/auth.py
--rw-r--r--  2.0 unx     5313 b- defN 24-May-23 10:56 nucliadb/standalone/config.py
--rw-r--r--  2.0 unx     6986 b- defN 24-May-23 10:56 nucliadb/standalone/introspect.py
--rw-r--r--  2.0 unx     2488 b- defN 24-May-23 10:56 nucliadb/standalone/lifecycle.py
--rw-r--r--  2.0 unx     1980 b- defN 24-May-23 10:56 nucliadb/standalone/migrations.py
--rw-r--r--  2.0 unx     1322 b- defN 24-May-23 10:56 nucliadb/standalone/purge.py
--rw-r--r--  2.0 unx     5636 b- defN 24-May-23 10:56 nucliadb/standalone/run.py
--rw-r--r--  2.0 unx     5822 b- defN 24-May-23 10:56 nucliadb/standalone/settings.py
--rw-r--r--  2.0 unx     3132 b- defN 24-May-23 10:56 nucliadb/standalone/versions.py
--rw-r--r--  2.0 unx     2285 b- defN 24-May-23 10:56 nucliadb/standalone/static/favicon.ico
--rw-r--r--  2.0 unx     3833 b- defN 24-May-23 10:56 nucliadb/standalone/static/index.html
--rw-r--r--  2.0 unx     2639 b- defN 24-May-23 10:56 nucliadb/standalone/static/logo.svg
--rw-r--r--  2.0 unx      835 b- defN 24-May-23 10:56 nucliadb/standalone/tests/__init__.py
--rw-r--r--  2.0 unx     1294 b- defN 24-May-23 10:56 nucliadb/standalone/tests/conftest.py
--rw-r--r--  2.0 unx     1319 b- defN 24-May-23 10:56 nucliadb/standalone/tests/fixtures.py
--rw-r--r--  2.0 unx      833 b- defN 24-May-23 10:56 nucliadb/standalone/tests/unit/__init__.py
--rw-r--r--  2.0 unx     1722 b- defN 24-May-23 10:56 nucliadb/standalone/tests/unit/test_api_router.py
--rw-r--r--  2.0 unx     5509 b- defN 24-May-23 10:56 nucliadb/standalone/tests/unit/test_auth.py
--rw-r--r--  2.0 unx     1334 b- defN 24-May-23 10:56 nucliadb/standalone/tests/unit/test_introspect.py
--rw-r--r--  2.0 unx     1863 b- defN 24-May-23 10:56 nucliadb/standalone/tests/unit/test_migrations.py
--rw-r--r--  2.0 unx     1546 b- defN 24-May-23 10:56 nucliadb/standalone/tests/unit/test_run.py
--rw-r--r--  2.0 unx     1972 b- defN 24-May-23 10:56 nucliadb/standalone/tests/unit/test_versions.py
--rw-r--r--  2.0 unx     1037 b- defN 24-May-23 10:56 nucliadb/tasks/__init__.py
--rw-r--r--  2.0 unx     7655 b- defN 24-May-23 10:56 nucliadb/tasks/consumer.py
--rw-r--r--  2.0 unx      924 b- defN 24-May-23 10:56 nucliadb/tasks/logger.py
--rw-r--r--  2.0 unx     1378 b- defN 24-May-23 10:56 nucliadb/tasks/models.py
--rw-r--r--  2.0 unx     3457 b- defN 24-May-23 10:56 nucliadb/tasks/producer.py
--rw-r--r--  2.0 unx     1753 b- defN 24-May-23 10:56 nucliadb/tasks/registry.py
--rw-r--r--  2.0 unx     1360 b- defN 24-May-23 10:56 nucliadb/tasks/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-23 10:56 nucliadb/tests/__init__.py
--rw-r--r--  2.0 unx     1229 b- defN 24-May-23 10:56 nucliadb/tests/conftest.py
--rw-r--r--  2.0 unx    22365 b- defN 24-May-23 10:56 nucliadb/tests/fixtures.py
--rw-r--r--  2.0 unx     7549 b- defN 24-May-23 10:56 nucliadb/tests/tikv.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-23 10:56 nucliadb/tests/benchmarks/__init__.py
--rw-r--r--  2.0 unx     3032 b- defN 24-May-23 10:56 nucliadb/tests/benchmarks/test_search.py
--rw-r--r--  2.0 unx      919 b- defN 24-May-23 10:56 nucliadb/tests/knowledgeboxes/__init__.py
--rw-r--r--  2.0 unx     7002 b- defN 24-May-23 10:56 nucliadb/tests/knowledgeboxes/philosophy_books.py
--rw-r--r--  2.0 unx     3037 b- defN 24-May-23 10:56 nucliadb/tests/knowledgeboxes/ten_dummy_resources.py
--rw-r--r--  2.0 unx     1148 b- defN 24-May-23 10:56 nucliadb/tests/migrations/__init__.py
--rw-r--r--  2.0 unx     2726 b- defN 24-May-23 10:56 nucliadb/tests/migrations/test_migration_0017.py
--rw-r--r--  2.0 unx     3662 b- defN 24-May-23 10:56 nucliadb/tests/migrations/test_migration_0018.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-23 10:56 nucliadb/tests/unit/__init__.py
--rw-r--r--  2.0 unx     1487 b- defN 24-May-23 10:56 nucliadb/tests/unit/test_field_ids.py
--rw-r--r--  2.0 unx     2780 b- defN 24-May-23 10:56 nucliadb/tests/unit/test_health.py
--rw-r--r--  2.0 unx     1543 b- defN 24-May-23 10:56 nucliadb/tests/unit/test_kb_slugs.py
--rw-r--r--  2.0 unx     7892 b- defN 24-May-23 10:56 nucliadb/tests/unit/test_learning_proxy.py
--rw-r--r--  2.0 unx     2642 b- defN 24-May-23 10:56 nucliadb/tests/unit/test_metrics_exporter.py
--rw-r--r--  2.0 unx     1341 b- defN 24-May-23 10:56 nucliadb/tests/unit/test_openapi.py
--rw-r--r--  2.0 unx     3649 b- defN 24-May-23 10:56 nucliadb/tests/unit/test_purge.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-23 10:56 nucliadb/tests/unit/common/__init__.py
--rw-r--r--  2.0 unx     1268 b- defN 24-May-23 10:56 nucliadb/tests/unit/common/test_context.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-23 10:56 nucliadb/tests/unit/common/cluster/__init__.py
--rw-r--r--  2.0 unx    12240 b- defN 24-May-23 10:56 nucliadb/tests/unit/common/cluster/test_cluster.py
--rw-r--r--  2.0 unx     5387 b- defN 24-May-23 10:56 nucliadb/tests/unit/common/cluster/test_kb_shard_manager.py
--rw-r--r--  2.0 unx     1428 b- defN 24-May-23 10:56 nucliadb/tests/unit/common/cluster/test_rebalance.py
--rw-r--r--  2.0 unx     9465 b- defN 24-May-23 10:56 nucliadb/tests/unit/common/cluster/test_rollover.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-23 10:56 nucliadb/tests/unit/common/cluster/discovery/__init__.py
--rw-r--r--  2.0 unx     5627 b- defN 24-May-23 10:56 nucliadb/tests/unit/common/cluster/discovery/test_k8s.py
--rw-r--r--  2.0 unx      833 b- defN 24-May-23 10:56 nucliadb/tests/unit/common/cluster/standalone/__init__.py
--rw-r--r--  2.0 unx     3761 b- defN 24-May-23 10:56 nucliadb/tests/unit/common/cluster/standalone/test_service.py
--rw-r--r--  2.0 unx     2136 b- defN 24-May-23 10:56 nucliadb/tests/unit/common/cluster/standalone/test_utils.py
--rw-r--r--  2.0 unx      833 b- defN 24-May-23 10:56 nucliadb/tests/unit/common/maindb/__init__.py
--rw-r--r--  2.0 unx     3579 b- defN 24-May-23 10:56 nucliadb/tests/unit/common/maindb/test_driver.py
--rw-r--r--  2.0 unx     1869 b- defN 24-May-23 10:56 nucliadb/tests/unit/common/maindb/test_tikv.py
--rw-r--r--  2.0 unx     3213 b- defN 24-May-23 10:56 nucliadb/tests/unit/common/maindb/test_utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-23 10:56 nucliadb/tests/unit/export_import/__init__.py
--rw-r--r--  2.0 unx     1435 b- defN 24-May-23 10:56 nucliadb/tests/unit/export_import/test_datamanager.py
--rw-r--r--  2.0 unx     9706 b- defN 24-May-23 10:56 nucliadb/tests/unit/export_import/test_utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-23 10:56 nucliadb/tests/unit/migrator/__init__.py
--rw-r--r--  2.0 unx     3233 b- defN 24-May-23 10:56 nucliadb/tests/unit/migrator/test_migrator.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-23 10:56 nucliadb/tests/unit/tasks/__init__.py
--rw-r--r--  2.0 unx     1375 b- defN 24-May-23 10:56 nucliadb/tests/unit/tasks/conftest.py
--rw-r--r--  2.0 unx     2714 b- defN 24-May-23 10:56 nucliadb/tests/unit/tasks/test_consumer.py
--rw-r--r--  2.0 unx     3189 b- defN 24-May-23 10:56 nucliadb/tests/unit/tasks/test_producer.py
--rw-r--r--  2.0 unx     1827 b- defN 24-May-23 10:56 nucliadb/tests/unit/tasks/test_tasks.py
--rw-r--r--  2.0 unx     2507 b- defN 24-May-23 10:56 nucliadb/tests/utils/__init__.py
--rw-r--r--  2.0 unx     1797 b- defN 24-May-23 10:56 nucliadb/tests/utils/aiohttp_session.py
--rw-r--r--  2.0 unx     2533 b- defN 24-May-23 10:56 nucliadb/tests/utils/entities.py
--rw-r--r--  2.0 unx     6327 b- defN 24-May-23 10:56 nucliadb/tests/utils/broker_messages/__init__.py
--rw-r--r--  2.0 unx     7557 b- defN 24-May-23 10:56 nucliadb/tests/utils/broker_messages/fields.py
--rw-r--r--  2.0 unx     1196 b- defN 24-May-23 10:56 nucliadb/tests/utils/broker_messages/helpers.py
--rw-r--r--  2.0 unx     1325 b- defN 24-May-23 10:56 nucliadb/train/__init__.py
--rw-r--r--  2.0 unx     3530 b- defN 24-May-23 10:56 nucliadb/train/app.py
--rw-r--r--  2.0 unx     3800 b- defN 24-May-23 10:56 nucliadb/train/generator.py
--rw-r--r--  2.0 unx     1698 b- defN 24-May-23 10:56 nucliadb/train/lifecycle.py
--rw-r--r--  2.0 unx     1198 b- defN 24-May-23 10:56 nucliadb/train/models.py
--rw-r--r--  2.0 unx     5706 b- defN 24-May-23 10:56 nucliadb/train/nodes.py
--rw-r--r--  2.0 unx     1400 b- defN 24-May-23 10:56 nucliadb/train/run.py
--rw-r--r--  2.0 unx     5926 b- defN 24-May-23 10:56 nucliadb/train/servicer.py
--rw-r--r--  2.0 unx     1415 b- defN 24-May-23 10:56 nucliadb/train/settings.py
--rw-r--r--  2.0 unx     1496 b- defN 24-May-23 10:56 nucliadb/train/types.py
--rw-r--r--  2.0 unx     3265 b- defN 24-May-23 10:56 nucliadb/train/upload.py
--rw-r--r--  2.0 unx     6420 b- defN 24-May-23 10:56 nucliadb/train/uploader.py
--rw-r--r--  2.0 unx     3179 b- defN 24-May-23 10:56 nucliadb/train/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-23 10:56 nucliadb/train/api/__init__.py
--rw-r--r--  2.0 unx     1479 b- defN 24-May-23 10:56 nucliadb/train/api/utils.py
--rw-r--r--  2.0 unx      928 b- defN 24-May-23 10:56 nucliadb/train/api/v1/__init__.py
--rw-r--r--  2.0 unx     2071 b- defN 24-May-23 10:56 nucliadb/train/api/v1/check.py
--rw-r--r--  2.0 unx      910 b- defN 24-May-23 10:56 nucliadb/train/api/v1/router.py
--rw-r--r--  2.0 unx     1908 b- defN 24-May-23 10:56 nucliadb/train/api/v1/shards.py
--rw-r--r--  2.0 unx     2135 b- defN 24-May-23 10:56 nucliadb/train/api/v1/trainset.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-23 10:56 nucliadb/train/generators/__init__.py
--rw-r--r--  2.0 unx     3723 b- defN 24-May-23 10:56 nucliadb/train/generators/field_classifier.py
--rw-r--r--  2.0 unx     6712 b- defN 24-May-23 10:56 nucliadb/train/generators/image_classifier.py
--rw-r--r--  2.0 unx     2789 b- defN 24-May-23 10:56 nucliadb/train/generators/paragraph_classifier.py
--rw-r--r--  2.0 unx     3590 b- defN 24-May-23 10:56 nucliadb/train/generators/paragraph_streaming.py
--rw-r--r--  2.0 unx     5372 b- defN 24-May-23 10:56 nucliadb/train/generators/question_answer_streaming.py
--rw-r--r--  2.0 unx     5160 b- defN 24-May-23 10:56 nucliadb/train/generators/sentence_classifier.py
--rw-r--r--  2.0 unx    10446 b- defN 24-May-23 10:56 nucliadb/train/generators/token_classifier.py
--rw-r--r--  2.0 unx     3877 b- defN 24-May-23 10:56 nucliadb/train/generators/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-23 10:56 nucliadb/train/tests/__init__.py
--rw-r--r--  2.0 unx     1125 b- defN 24-May-23 10:56 nucliadb/train/tests/conftest.py
--rw-r--r--  2.0 unx    11053 b- defN 24-May-23 10:56 nucliadb/train/tests/fixtures.py
--rw-r--r--  2.0 unx     4598 b- defN 24-May-23 10:56 nucliadb/train/tests/test_field_classification.py
--rw-r--r--  2.0 unx     2729 b- defN 24-May-23 10:56 nucliadb/train/tests/test_get_entities.py
--rw-r--r--  2.0 unx     1876 b- defN 24-May-23 10:56 nucliadb/train/tests/test_get_info.py
--rw-r--r--  2.0 unx     1382 b- defN 24-May-23 10:56 nucliadb/train/tests/test_get_ontology.py
--rw-r--r--  2.0 unx     2417 b- defN 24-May-23 10:56 nucliadb/train/tests/test_get_ontology_count.py
--rw-r--r--  2.0 unx     7669 b- defN 24-May-23 10:56 nucliadb/train/tests/test_image_classification.py
--rw-r--r--  2.0 unx     1416 b- defN 24-May-23 10:56 nucliadb/train/tests/test_list_fields.py
--rw-r--r--  2.0 unx     2944 b- defN 24-May-23 10:56 nucliadb/train/tests/test_list_paragraphs.py
--rw-r--r--  2.0 unx     1423 b- defN 24-May-23 10:56 nucliadb/train/tests/test_list_resources.py
--rw-r--r--  2.0 unx     2947 b- defN 24-May-23 10:56 nucliadb/train/tests/test_list_sentences.py
--rw-r--r--  2.0 unx     4645 b- defN 24-May-23 10:56 nucliadb/train/tests/test_paragraph_classification.py
--rw-r--r--  2.0 unx     4320 b- defN 24-May-23 10:56 nucliadb/train/tests/test_paragraph_streaming.py
--rw-r--r--  2.0 unx     8751 b- defN 24-May-23 10:56 nucliadb/train/tests/test_question_answer_streaming.py
--rw-r--r--  2.0 unx     5051 b- defN 24-May-23 10:56 nucliadb/train/tests/test_sentence_classification.py
--rw-r--r--  2.0 unx     5583 b- defN 24-May-23 10:56 nucliadb/train/tests/test_token_classification.py
--rw-r--r--  2.0 unx     3324 b- defN 24-May-23 10:56 nucliadb/train/tests/utils.py
--rw-r--r--  2.0 unx     1328 b- defN 24-May-23 10:56 nucliadb/writer/__init__.py
--rw-r--r--  2.0 unx     4268 b- defN 24-May-23 10:56 nucliadb/writer/app.py
--rw-r--r--  2.0 unx    19483 b- defN 24-May-23 10:56 nucliadb/writer/back_pressure.py
--rw-r--r--  2.0 unx      972 b- defN 24-May-23 10:56 nucliadb/writer/exceptions.py
--rw-r--r--  2.0 unx     1953 b- defN 24-May-23 10:56 nucliadb/writer/lifecycle.py
--rw-r--r--  2.0 unx     1032 b- defN 24-May-23 10:56 nucliadb/writer/openapi.py
--rw-r--r--  2.0 unx     1448 b- defN 24-May-23 10:56 nucliadb/writer/run.py
--rw-r--r--  2.0 unx     3103 b- defN 24-May-23 10:56 nucliadb/writer/settings.py
--rw-r--r--  2.0 unx     1036 b- defN 24-May-23 10:56 nucliadb/writer/utilities.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-23 10:56 nucliadb/writer/api/__init__.py
--rw-r--r--  2.0 unx     1429 b- defN 24-May-23 10:56 nucliadb/writer/api/constants.py
--rw-r--r--  2.0 unx     1095 b- defN 24-May-23 10:56 nucliadb/writer/api/v1/__init__.py
--rw-r--r--  2.0 unx     6571 b- defN 24-May-23 10:56 nucliadb/writer/api/v1/export_import.py
--rw-r--r--  2.0 unx    24482 b- defN 24-May-23 10:56 nucliadb/writer/api/v1/field.py
--rw-r--r--  2.0 unx     5248 b- defN 24-May-23 10:56 nucliadb/writer/api/v1/knowledgebox.py
--rw-r--r--  2.0 unx     2058 b- defN 24-May-23 10:56 nucliadb/writer/api/v1/learning_config.py
--rw-r--r--  2.0 unx    18893 b- defN 24-May-23 10:56 nucliadb/writer/api/v1/resource.py
--rw-r--r--  2.0 unx     1034 b- defN 24-May-23 10:56 nucliadb/writer/api/v1/router.py
--rw-r--r--  2.0 unx    10216 b- defN 24-May-23 10:56 nucliadb/writer/api/v1/services.py
--rw-r--r--  2.0 unx    30857 b- defN 24-May-23 10:56 nucliadb/writer/api/v1/upload.py
--rw-r--r--  2.0 unx     1612 b- defN 24-May-23 10:56 nucliadb/writer/layouts/__init__.py
--rw-r--r--  2.0 unx     2115 b- defN 24-May-23 10:56 nucliadb/writer/layouts/v1.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-23 10:56 nucliadb/writer/resource/__init__.py
--rw-r--r--  2.0 unx     1425 b- defN 24-May-23 10:56 nucliadb/writer/resource/audit.py
--rw-r--r--  2.0 unx    10968 b- defN 24-May-23 10:56 nucliadb/writer/resource/basic.py
--rw-r--r--  2.0 unx    16740 b- defN 24-May-23 10:56 nucliadb/writer/resource/field.py
--rw-r--r--  2.0 unx     2022 b- defN 24-May-23 10:56 nucliadb/writer/resource/origin.py
--rw-r--r--  2.0 unx     1093 b- defN 24-May-23 10:56 nucliadb/writer/resource/slug.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-23 10:56 nucliadb/writer/tests/__init__.py
--rw-r--r--  2.0 unx     1200 b- defN 24-May-23 10:56 nucliadb/writer/tests/conftest.py
--rw-r--r--  2.0 unx     5971 b- defN 24-May-23 10:56 nucliadb/writer/tests/fixtures.py
--rw-r--r--  2.0 unx    15472 b- defN 24-May-23 10:56 nucliadb/writer/tests/test_fields.py
--rw-r--r--  2.0 unx    25999 b- defN 24-May-23 10:56 nucliadb/writer/tests/test_files.py
--rw-r--r--  2.0 unx     1729 b- defN 24-May-23 10:56 nucliadb/writer/tests/test_knowledgebox.py
--rw-r--r--  2.0 unx     4358 b- defN 24-May-23 10:56 nucliadb/writer/tests/test_reprocess_file_field.py
--rw-r--r--  2.0 unx    16694 b- defN 24-May-23 10:56 nucliadb/writer/tests/test_resources.py
--rw-r--r--  2.0 unx     5120 b- defN 24-May-23 10:56 nucliadb/writer/tests/test_service.py
--rw-r--r--  2.0 unx     6054 b- defN 24-May-23 10:56 nucliadb/writer/tests/test_tus.py
--rw-r--r--  2.0 unx     1287 b- defN 24-May-23 10:56 nucliadb/writer/tests/utils.py
--rw-r--r--  2.0 unx     5226 b- defN 24-May-23 10:56 nucliadb/writer/tus/__init__.py
--rw-r--r--  2.0 unx     5082 b- defN 24-May-23 10:56 nucliadb/writer/tus/dm.py
--rw-r--r--  2.0 unx     2186 b- defN 24-May-23 10:56 nucliadb/writer/tus/exceptions.py
--rw-r--r--  2.0 unx    14527 b- defN 24-May-23 10:56 nucliadb/writer/tus/gcs.py
--rw-r--r--  2.0 unx     5849 b- defN 24-May-23 10:56 nucliadb/writer/tus/local.py
--rw-r--r--  2.0 unx     4367 b- defN 24-May-23 10:56 nucliadb/writer/tus/pg.py
--rw-r--r--  2.0 unx     9069 b- defN 24-May-23 10:56 nucliadb/writer/tus/s3.py
--rw-r--r--  2.0 unx     4734 b- defN 24-May-23 10:56 nucliadb/writer/tus/storage.py
--rw-r--r--  2.0 unx     2556 b- defN 24-May-23 10:56 nucliadb/writer/tus/utils.py
--rw-r--r--  2.0 unx     4423 b- defN 24-May-23 10:57 nucliadb-4.0.0.post539.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-23 10:57 nucliadb-4.0.0.post539.dist-info/WHEEL
--rw-r--r--  2.0 unx     1268 b- defN 24-May-23 10:57 nucliadb-4.0.0.post539.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       20 b- defN 24-May-23 10:57 nucliadb-4.0.0.post539.dist-info/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 24-May-23 10:57 nucliadb-4.0.0.post539.dist-info/zip-safe
--rw-rw-r--  2.0 unx    43360 b- defN 24-May-23 10:57 nucliadb-4.0.0.post539.dist-info/RECORD
-462 files, 2259836 bytes uncompressed, 695874 bytes compressed:  69.2%
+Zip file size: 765780 bytes, number of entries: 462
+-rw-r--r--  2.0 unx     1135 b- defN 24-May-23 12:38 migrations/0001_bootstrap.py
+-rw-r--r--  2.0 unx     1177 b- defN 24-May-23 12:38 migrations/0002_rollover_shards.py
+-rw-r--r--  2.0 unx     2436 b- defN 24-May-23 12:38 migrations/0003_allfields_key.py
+-rw-r--r--  2.0 unx     1177 b- defN 24-May-23 12:38 migrations/0004_rollover_shards.py
+-rw-r--r--  2.0 unx     1177 b- defN 24-May-23 12:38 migrations/0005_rollover_shards.py
+-rw-r--r--  2.0 unx     1024 b- defN 24-May-23 12:38 migrations/0006_rollover_shards.py
+-rw-r--r--  2.0 unx     1301 b- defN 24-May-23 12:38 migrations/0008_cleanup_leftover_rollover_metadata.py
+-rw-r--r--  2.0 unx     1378 b- defN 24-May-23 12:38 migrations/0009_upgrade_relations_and_texts_to_v2.py
+-rw-r--r--  2.0 unx     1610 b- defN 24-May-23 12:38 migrations/0010_fix_corrupt_indexes.py
+-rw-r--r--  2.0 unx     1843 b- defN 24-May-23 12:38 migrations/0011_materialize_labelset_ids.py
+-rw-r--r--  2.0 unx     1443 b- defN 24-May-23 12:38 migrations/0012_rollover_shards.py
+-rw-r--r--  2.0 unx     1024 b- defN 24-May-23 12:38 migrations/0013_rollover_shards.py
+-rw-r--r--  2.0 unx     1382 b- defN 24-May-23 12:38 migrations/0014_rollover_shards.py
+-rw-r--r--  2.0 unx     1462 b- defN 24-May-23 12:38 migrations/0015_targeted_rollover.py
+-rw-r--r--  2.0 unx     2506 b- defN 24-May-23 12:38 migrations/0016_upgrade_to_paragraphs_v2.py
+-rw-r--r--  2.0 unx     2100 b- defN 24-May-23 12:38 migrations/0017_multiple_writable_shards.py
+-rw-r--r--  2.0 unx     2264 b- defN 24-May-23 12:38 migrations/0018_purge_orphan_kbslugs.py
+-rw-r--r--  2.0 unx     2506 b- defN 24-May-23 12:38 migrations/0019_upgrade_to_paragraphs_v3.py
+-rw-r--r--  2.0 unx     3282 b- defN 24-May-23 12:38 migrations/0020_drain_nodes_from_cluster.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-23 12:38 migrations/__init__.py
+-rw-r--r--  2.0 unx      891 b- defN 24-May-23 12:38 nucliadb/__init__.py
+-rw-r--r--  2.0 unx     3733 b- defN 24-May-23 12:38 nucliadb/health.py
+-rw-r--r--  2.0 unx    11639 b- defN 24-May-23 12:38 nucliadb/learning_proxy.py
+-rw-r--r--  2.0 unx     4806 b- defN 24-May-23 12:38 nucliadb/metrics_exporter.py
+-rw-r--r--  2.0 unx     2272 b- defN 24-May-23 12:38 nucliadb/openapi.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-23 12:38 nucliadb/py.typed
+-rw-r--r--  2.0 unx      835 b- defN 24-May-23 12:38 nucliadb/common/__init__.py
+-rw-r--r--  2.0 unx     5175 b- defN 24-May-23 12:38 nucliadb/common/locking.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-23 12:38 nucliadb/common/cluster/__init__.py
+-rw-r--r--  2.0 unx     5080 b- defN 24-May-23 12:38 nucliadb/common/cluster/base.py
+-rw-r--r--  2.0 unx     1495 b- defN 24-May-23 12:38 nucliadb/common/cluster/exceptions.py
+-rw-r--r--  2.0 unx     3793 b- defN 24-May-23 12:38 nucliadb/common/cluster/grpc_node_dummy.py
+-rw-r--r--  2.0 unx     3429 b- defN 24-May-23 12:38 nucliadb/common/cluster/index_node.py
+-rw-r--r--  2.0 unx    22091 b- defN 24-May-23 12:38 nucliadb/common/cluster/manager.py
+-rw-r--r--  2.0 unx     8853 b- defN 24-May-23 12:38 nucliadb/common/cluster/rebalance.py
+-rw-r--r--  2.0 unx    20209 b- defN 24-May-23 12:38 nucliadb/common/cluster/rollover.py
+-rw-r--r--  2.0 unx     3016 b- defN 24-May-23 12:38 nucliadb/common/cluster/settings.py
+-rw-r--r--  2.0 unx     5713 b- defN 24-May-23 12:38 nucliadb/common/cluster/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-23 12:38 nucliadb/common/cluster/discovery/__init__.py
+-rw-r--r--  2.0 unx     6553 b- defN 24-May-23 12:38 nucliadb/common/cluster/discovery/base.py
+-rw-r--r--  2.0 unx    12512 b- defN 24-May-23 12:38 nucliadb/common/cluster/discovery/k8s.py
+-rw-r--r--  2.0 unx     1957 b- defN 24-May-23 12:38 nucliadb/common/cluster/discovery/manual.py
+-rw-r--r--  2.0 unx     1737 b- defN 24-May-23 12:38 nucliadb/common/cluster/discovery/single.py
+-rw-r--r--  2.0 unx     1139 b- defN 24-May-23 12:38 nucliadb/common/cluster/discovery/types.py
+-rw-r--r--  2.0 unx     2548 b- defN 24-May-23 12:38 nucliadb/common/cluster/discovery/utils.py
+-rw-r--r--  2.0 unx      833 b- defN 24-May-23 12:38 nucliadb/common/cluster/standalone/__init__.py
+-rw-r--r--  2.0 unx    13712 b- defN 24-May-23 12:38 nucliadb/common/cluster/standalone/grpc_node_binding.py
+-rw-r--r--  2.0 unx     4683 b- defN 24-May-23 12:38 nucliadb/common/cluster/standalone/index_node.py
+-rw-r--r--  2.0 unx     3444 b- defN 24-May-23 12:38 nucliadb/common/cluster/standalone/service.py
+-rw-r--r--  2.0 unx     3545 b- defN 24-May-23 12:38 nucliadb/common/cluster/standalone/utils.py
+-rw-r--r--  2.0 unx     3440 b- defN 24-May-23 12:38 nucliadb/common/context/__init__.py
+-rw-r--r--  2.0 unx     1628 b- defN 24-May-23 12:38 nucliadb/common/context/fastapi.py
+-rw-r--r--  2.0 unx     1906 b- defN 24-May-23 12:38 nucliadb/common/datamanagers/__init__.py
+-rw-r--r--  2.0 unx     2651 b- defN 24-May-23 12:38 nucliadb/common/datamanagers/atomic.py
+-rw-r--r--  2.0 unx     1451 b- defN 24-May-23 12:38 nucliadb/common/datamanagers/cluster.py
+-rw-r--r--  2.0 unx     5383 b- defN 24-May-23 12:38 nucliadb/common/datamanagers/entities.py
+-rw-r--r--  2.0 unx      883 b- defN 24-May-23 12:38 nucliadb/common/datamanagers/exceptions.py
+-rw-r--r--  2.0 unx     3994 b- defN 24-May-23 12:38 nucliadb/common/datamanagers/kb.py
+-rw-r--r--  2.0 unx     5389 b- defN 24-May-23 12:38 nucliadb/common/datamanagers/labels.py
+-rw-r--r--  2.0 unx     1599 b- defN 24-May-23 12:38 nucliadb/common/datamanagers/processing.py
+-rw-r--r--  2.0 unx    12177 b- defN 24-May-23 12:38 nucliadb/common/datamanagers/resources.py
+-rw-r--r--  2.0 unx     5634 b- defN 24-May-23 12:38 nucliadb/common/datamanagers/rollover.py
+-rw-r--r--  2.0 unx     1548 b- defN 24-May-23 12:38 nucliadb/common/datamanagers/synonyms.py
+-rw-r--r--  2.0 unx     1631 b- defN 24-May-23 12:38 nucliadb/common/datamanagers/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-23 12:38 nucliadb/common/http_clients/__init__.py
+-rw-r--r--  2.0 unx     2146 b- defN 24-May-23 12:38 nucliadb/common/http_clients/auth.py
+-rw-r--r--  2.0 unx     1100 b- defN 24-May-23 12:38 nucliadb/common/http_clients/exceptions.py
+-rw-r--r--  2.0 unx     7155 b- defN 24-May-23 12:38 nucliadb/common/http_clients/processing.py
+-rw-r--r--  2.0 unx     1540 b- defN 24-May-23 12:38 nucliadb/common/http_clients/pypi.py
+-rw-r--r--  2.0 unx     1551 b- defN 24-May-23 12:38 nucliadb/common/http_clients/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-23 12:38 nucliadb/common/maindb/__init__.py
+-rw-r--r--  2.0 unx     3449 b- defN 24-May-23 12:38 nucliadb/common/maindb/driver.py
+-rw-r--r--  2.0 unx      946 b- defN 24-May-23 12:38 nucliadb/common/maindb/exceptions.py
+-rw-r--r--  2.0 unx     6769 b- defN 24-May-23 12:38 nucliadb/common/maindb/local.py
+-rw-r--r--  2.0 unx     8391 b- defN 24-May-23 12:38 nucliadb/common/maindb/pg.py
+-rw-r--r--  2.0 unx     6053 b- defN 24-May-23 12:38 nucliadb/common/maindb/redis.py
+-rw-r--r--  2.0 unx    14502 b- defN 24-May-23 12:38 nucliadb/common/maindb/tikv.py
+-rw-r--r--  2.0 unx     4167 b- defN 24-May-23 12:38 nucliadb/common/maindb/utils.py
+-rw-r--r--  2.0 unx      932 b- defN 24-May-23 12:38 nucliadb/export_import/__init__.py
+-rw-r--r--  2.0 unx     6171 b- defN 24-May-23 12:38 nucliadb/export_import/datamanager.py
+-rw-r--r--  2.0 unx     1949 b- defN 24-May-23 12:38 nucliadb/export_import/exceptions.py
+-rw-r--r--  2.0 unx     7116 b- defN 24-May-23 12:38 nucliadb/export_import/exporter.py
+-rw-r--r--  2.0 unx     4258 b- defN 24-May-23 12:38 nucliadb/export_import/importer.py
+-rw-r--r--  2.0 unx     2063 b- defN 24-May-23 12:38 nucliadb/export_import/models.py
+-rw-r--r--  2.0 unx     2571 b- defN 24-May-23 12:38 nucliadb/export_import/tasks.py
+-rw-r--r--  2.0 unx    19401 b- defN 24-May-23 12:38 nucliadb/export_import/utils.py
+-rw-r--r--  2.0 unx     1011 b- defN 24-May-23 12:38 nucliadb/ingest/__init__.py
+-rw-r--r--  2.0 unx     7277 b- defN 24-May-23 12:38 nucliadb/ingest/app.py
+-rw-r--r--  2.0 unx     1005 b- defN 24-May-23 12:38 nucliadb/ingest/cache.py
+-rw-r--r--  2.0 unx     2484 b- defN 24-May-23 12:38 nucliadb/ingest/partitions.py
+-rw-r--r--  2.0 unx    19904 b- defN 24-May-23 12:38 nucliadb/ingest/processing.py
+-rw-r--r--  2.0 unx    20277 b- defN 24-May-23 12:38 nucliadb/ingest/serialize.py
+-rw-r--r--  2.0 unx     3207 b- defN 24-May-23 12:38 nucliadb/ingest/settings.py
+-rw-r--r--  2.0 unx     2314 b- defN 24-May-23 12:38 nucliadb/ingest/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-23 12:38 nucliadb/ingest/consumer/__init__.py
+-rw-r--r--  2.0 unx     6918 b- defN 24-May-23 12:38 nucliadb/ingest/consumer/auditing.py
+-rw-r--r--  2.0 unx    12174 b- defN 24-May-23 12:38 nucliadb/ingest/consumer/consumer.py
+-rw-r--r--  2.0 unx     3945 b- defN 24-May-23 12:38 nucliadb/ingest/consumer/materializer.py
+-rw-r--r--  2.0 unx     1075 b- defN 24-May-23 12:38 nucliadb/ingest/consumer/metrics.py
+-rw-r--r--  2.0 unx     9543 b- defN 24-May-23 12:38 nucliadb/ingest/consumer/pull.py
+-rw-r--r--  2.0 unx     6871 b- defN 24-May-23 12:38 nucliadb/ingest/consumer/service.py
+-rw-r--r--  2.0 unx     4331 b- defN 24-May-23 12:38 nucliadb/ingest/consumer/shard_creator.py
+-rw-r--r--  2.0 unx     2656 b- defN 24-May-23 12:38 nucliadb/ingest/consumer/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-23 12:38 nucliadb/ingest/fields/__init__.py
+-rw-r--r--  2.0 unx    17461 b- defN 24-May-23 12:38 nucliadb/ingest/fields/base.py
+-rw-r--r--  2.0 unx     6516 b- defN 24-May-23 12:38 nucliadb/ingest/fields/conversation.py
+-rw-r--r--  2.0 unx     1223 b- defN 24-May-23 12:38 nucliadb/ingest/fields/date.py
+-rw-r--r--  2.0 unx     1205 b- defN 24-May-23 12:38 nucliadb/ingest/fields/exceptions.py
+-rw-r--r--  2.0 unx     4840 b- defN 24-May-23 12:38 nucliadb/ingest/fields/file.py
+-rw-r--r--  2.0 unx     1547 b- defN 24-May-23 12:38 nucliadb/ingest/fields/generic.py
+-rw-r--r--  2.0 unx     1235 b- defN 24-May-23 12:38 nucliadb/ingest/fields/keywordset.py
+-rw-r--r--  2.0 unx     2250 b- defN 24-May-23 12:38 nucliadb/ingest/fields/layout.py
+-rw-r--r--  2.0 unx     4212 b- defN 24-May-23 12:38 nucliadb/ingest/fields/link.py
+-rw-r--r--  2.0 unx     1319 b- defN 24-May-23 12:38 nucliadb/ingest/fields/text.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-23 12:38 nucliadb/ingest/orm/__init__.py
+-rw-r--r--  2.0 unx    28311 b- defN 24-May-23 12:38 nucliadb/ingest/orm/brain.py
+-rw-r--r--  2.0 unx    15758 b- defN 24-May-23 12:38 nucliadb/ingest/orm/entities.py
+-rw-r--r--  2.0 unx     1279 b- defN 24-May-23 12:38 nucliadb/ingest/orm/exceptions.py
+-rw-r--r--  2.0 unx    15621 b- defN 24-May-23 12:38 nucliadb/ingest/orm/knowledgebox.py
+-rw-r--r--  2.0 unx     1096 b- defN 24-May-23 12:38 nucliadb/ingest/orm/metrics.py
+-rw-r--r--  2.0 unx    58955 b- defN 24-May-23 12:38 nucliadb/ingest/orm/resource.py
+-rw-r--r--  2.0 unx     2685 b- defN 24-May-23 12:38 nucliadb/ingest/orm/utils.py
+-rw-r--r--  2.0 unx    27042 b- defN 24-May-23 12:38 nucliadb/ingest/orm/processor/__init__.py
+-rw-r--r--  2.0 unx     5090 b- defN 24-May-23 12:38 nucliadb/ingest/orm/processor/auditing.py
+-rw-r--r--  2.0 unx     1690 b- defN 24-May-23 12:38 nucliadb/ingest/orm/processor/sequence_manager.py
+-rw-r--r--  2.0 unx     2057 b- defN 24-May-23 12:38 nucliadb/ingest/service/__init__.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-23 12:38 nucliadb/ingest/service/exceptions.py
+-rw-r--r--  2.0 unx    30462 b- defN 24-May-23 12:38 nucliadb/ingest/service/writer.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-23 12:38 nucliadb/ingest/tests/__init__.py
+-rw-r--r--  2.0 unx     1157 b- defN 24-May-23 12:38 nucliadb/ingest/tests/conftest.py
+-rw-r--r--  2.0 unx    24060 b- defN 24-May-23 12:38 nucliadb/ingest/tests/fixtures.py
+-rw-r--r--  2.0 unx    62843 b- defN 24-May-23 12:38 nucliadb/ingest/tests/vectors.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-23 12:38 nucliadb/ingest/tests/integration/__init__.py
+-rw-r--r--  2.0 unx      833 b- defN 24-May-23 12:38 nucliadb/ingest/tests/integration/consumer/__init__.py
+-rw-r--r--  2.0 unx     2500 b- defN 24-May-23 12:38 nucliadb/ingest/tests/integration/consumer/test_auditing.py
+-rw-r--r--  2.0 unx     3832 b- defN 24-May-23 12:38 nucliadb/ingest/tests/integration/consumer/test_materializer.py
+-rw-r--r--  2.0 unx     4470 b- defN 24-May-23 12:38 nucliadb/ingest/tests/integration/consumer/test_pull.py
+-rw-r--r--  2.0 unx     2763 b- defN 24-May-23 12:38 nucliadb/ingest/tests/integration/consumer/test_service.py
+-rw-r--r--  2.0 unx     2019 b- defN 24-May-23 12:38 nucliadb/ingest/tests/integration/consumer/test_shard_creator.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-23 12:38 nucliadb/ingest/tests/integration/ingest/__init__.py
+-rw-r--r--  2.0 unx    27247 b- defN 24-May-23 12:38 nucliadb/ingest/tests/integration/ingest/test_ingest.py
+-rw-r--r--  2.0 unx     3040 b- defN 24-May-23 12:38 nucliadb/ingest/tests/integration/ingest/test_processing_engine.py
+-rw-r--r--  2.0 unx     8586 b- defN 24-May-23 12:38 nucliadb/ingest/tests/integration/ingest/test_relations.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-23 12:38 nucliadb/ingest/tests/unit/__init__.py
+-rw-r--r--  2.0 unx     1189 b- defN 24-May-23 12:38 nucliadb/ingest/tests/unit/test_cache.py
+-rw-r--r--  2.0 unx     1432 b- defN 24-May-23 12:38 nucliadb/ingest/tests/unit/test_partitions.py
+-rw-r--r--  2.0 unx     5807 b- defN 24-May-23 12:38 nucliadb/ingest/tests/unit/test_processing.py
+-rw-r--r--  2.0 unx      978 b- defN 24-May-23 12:38 nucliadb/ingest/tests/unit/test_settings.py
+-rw-r--r--  2.0 unx      833 b- defN 24-May-23 12:38 nucliadb/ingest/tests/unit/consumer/__init__.py
+-rw-r--r--  2.0 unx     3885 b- defN 24-May-23 12:38 nucliadb/ingest/tests/unit/consumer/test_auditing.py
+-rw-r--r--  2.0 unx     2472 b- defN 24-May-23 12:38 nucliadb/ingest/tests/unit/consumer/test_consumer.py
+-rw-r--r--  2.0 unx     2063 b- defN 24-May-23 12:38 nucliadb/ingest/tests/unit/consumer/test_pull.py
+-rw-r--r--  2.0 unx     4140 b- defN 24-May-23 12:38 nucliadb/ingest/tests/unit/consumer/test_shard_creator.py
+-rw-r--r--  2.0 unx     1934 b- defN 24-May-23 12:38 nucliadb/ingest/tests/unit/consumer/test_utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-23 12:38 nucliadb/ingest/tests/unit/orm/__init__.py
+-rw-r--r--  2.0 unx     9876 b- defN 24-May-23 12:38 nucliadb/ingest/tests/unit/orm/test_brain.py
+-rw-r--r--  2.0 unx     2435 b- defN 24-May-23 12:38 nucliadb/ingest/tests/unit/orm/test_brain_vectors.py
+-rw-r--r--  2.0 unx     1174 b- defN 24-May-23 12:38 nucliadb/ingest/tests/unit/orm/test_orm_utils.py
+-rw-r--r--  2.0 unx     4045 b- defN 24-May-23 12:38 nucliadb/ingest/tests/unit/orm/test_processor.py
+-rw-r--r--  2.0 unx    11033 b- defN 24-May-23 12:38 nucliadb/ingest/tests/unit/orm/test_resource.py
+-rw-r--r--  2.0 unx     2216 b- defN 24-May-23 12:38 nucliadb/middleware/__init__.py
+-rw-r--r--  2.0 unx     3912 b- defN 24-May-23 12:38 nucliadb/middleware/transaction.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-23 12:38 nucliadb/migrator/__init__.py
+-rw-r--r--  2.0 unx     2119 b- defN 24-May-23 12:38 nucliadb/migrator/command.py
+-rw-r--r--  2.0 unx     1334 b- defN 24-May-23 12:38 nucliadb/migrator/context.py
+-rw-r--r--  2.0 unx     5104 b- defN 24-May-23 12:38 nucliadb/migrator/datamanager.py
+-rw-r--r--  2.0 unx      889 b- defN 24-May-23 12:38 nucliadb/migrator/exceptions.py
+-rw-r--r--  2.0 unx     9370 b- defN 24-May-23 12:38 nucliadb/migrator/migrator.py
+-rw-r--r--  2.0 unx     1145 b- defN 24-May-23 12:38 nucliadb/migrator/models.py
+-rw-r--r--  2.0 unx     1144 b- defN 24-May-23 12:38 nucliadb/migrator/settings.py
+-rw-r--r--  2.0 unx     2346 b- defN 24-May-23 12:38 nucliadb/migrator/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-23 12:38 nucliadb/models/__init__.py
+-rw-r--r--  2.0 unx     1599 b- defN 24-May-23 12:38 nucliadb/models/responses.py
+-rw-r--r--  2.0 unx     6041 b- defN 24-May-23 12:38 nucliadb/purge/__init__.py
+-rw-r--r--  2.0 unx     9364 b- defN 24-May-23 12:38 nucliadb/purge/orphan_shards.py
+-rw-r--r--  2.0 unx     1328 b- defN 24-May-23 12:38 nucliadb/reader/__init__.py
+-rw-r--r--  2.0 unx     3709 b- defN 24-May-23 12:38 nucliadb/reader/app.py
+-rw-r--r--  2.0 unx     1366 b- defN 24-May-23 12:38 nucliadb/reader/lifecycle.py
+-rw-r--r--  2.0 unx     1031 b- defN 24-May-23 12:38 nucliadb/reader/openapi.py
+-rw-r--r--  2.0 unx     1447 b- defN 24-May-23 12:38 nucliadb/reader/run.py
+-rw-r--r--  2.0 unx      872 b- defN 24-May-23 12:38 nucliadb/reader/api/__init__.py
+-rw-r--r--  2.0 unx     2458 b- defN 24-May-23 12:38 nucliadb/reader/api/models.py
+-rw-r--r--  2.0 unx     1110 b- defN 24-May-23 12:38 nucliadb/reader/api/v1/__init__.py
+-rw-r--r--  2.0 unx    12392 b- defN 24-May-23 12:38 nucliadb/reader/api/v1/download.py
+-rw-r--r--  2.0 unx     6459 b- defN 24-May-23 12:38 nucliadb/reader/api/v1/export_import.py
+-rw-r--r--  2.0 unx     3641 b- defN 24-May-23 12:38 nucliadb/reader/api/v1/knowledgebox.py
+-rw-r--r--  2.0 unx     2099 b- defN 24-May-23 12:38 nucliadb/reader/api/v1/learning_collector.py
+-rw-r--r--  2.0 unx     4472 b- defN 24-May-23 12:38 nucliadb/reader/api/v1/learning_config.py
+-rw-r--r--  2.0 unx    13951 b- defN 24-May-23 12:38 nucliadb/reader/api/v1/resource.py
+-rw-r--r--  2.0 unx     1011 b- defN 24-May-23 12:38 nucliadb/reader/api/v1/router.py
+-rw-r--r--  2.0 unx    12115 b- defN 24-May-23 12:38 nucliadb/reader/api/v1/services.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-23 12:38 nucliadb/reader/reader/__init__.py
+-rw-r--r--  2.0 unx     7979 b- defN 24-May-23 12:38 nucliadb/reader/reader/notifications.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-23 12:38 nucliadb/reader/tests/__init__.py
+-rw-r--r--  2.0 unx     1224 b- defN 24-May-23 12:38 nucliadb/reader/tests/conftest.py
+-rw-r--r--  2.0 unx     4345 b- defN 24-May-23 12:38 nucliadb/reader/tests/fixtures.py
+-rw-r--r--  2.0 unx     2748 b- defN 24-May-23 12:38 nucliadb/reader/tests/test_list_resources.py
+-rw-r--r--  2.0 unx    10199 b- defN 24-May-23 12:38 nucliadb/reader/tests/test_reader_file_download.py
+-rw-r--r--  2.0 unx    10586 b- defN 24-May-23 12:38 nucliadb/reader/tests/test_reader_resource.py
+-rw-r--r--  2.0 unx     6535 b- defN 24-May-23 12:38 nucliadb/reader/tests/test_reader_resource_field.py
+-rw-r--r--  2.0 unx     1535 b- defN 24-May-23 12:38 nucliadb/search/__init__.py
+-rw-r--r--  2.0 unx     4905 b- defN 24-May-23 12:38 nucliadb/search/app.py
+-rw-r--r--  2.0 unx     1956 b- defN 24-May-23 12:38 nucliadb/search/lifecycle.py
+-rw-r--r--  2.0 unx     1016 b- defN 24-May-23 12:38 nucliadb/search/openapi.py
+-rw-r--r--  2.0 unx    20665 b- defN 24-May-23 12:38 nucliadb/search/predict.py
+-rw-r--r--  2.0 unx     1402 b- defN 24-May-23 12:38 nucliadb/search/run.py
+-rw-r--r--  2.0 unx     1193 b- defN 24-May-23 12:38 nucliadb/search/settings.py
+-rw-r--r--  2.0 unx     1037 b- defN 24-May-23 12:38 nucliadb/search/utilities.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-23 12:38 nucliadb/search/api/__init__.py
+-rw-r--r--  2.0 unx     1298 b- defN 24-May-23 12:38 nucliadb/search/api/v1/__init__.py
+-rw-r--r--  2.0 unx     3534 b- defN 24-May-23 12:38 nucliadb/search/api/v1/ask.py
+-rw-r--r--  2.0 unx     9493 b- defN 24-May-23 12:38 nucliadb/search/api/v1/chat.py
+-rw-r--r--  2.0 unx     2668 b- defN 24-May-23 12:38 nucliadb/search/api/v1/feedback.py
+-rw-r--r--  2.0 unx     8795 b- defN 24-May-23 12:38 nucliadb/search/api/v1/find.py
+-rw-r--r--  2.0 unx     6938 b- defN 24-May-23 12:38 nucliadb/search/api/v1/knowledgebox.py
+-rw-r--r--  2.0 unx     3047 b- defN 24-May-23 12:38 nucliadb/search/api/v1/predict_proxy.py
+-rw-r--r--  2.0 unx      988 b- defN 24-May-23 12:38 nucliadb/search/api/v1/router.py
+-rw-r--r--  2.0 unx    19262 b- defN 24-May-23 12:38 nucliadb/search/api/v1/search.py
+-rw-r--r--  2.0 unx     5970 b- defN 24-May-23 12:38 nucliadb/search/api/v1/suggest.py
+-rw-r--r--  2.0 unx     2499 b- defN 24-May-23 12:38 nucliadb/search/api/v1/summarize.py
+-rw-r--r--  2.0 unx     1434 b- defN 24-May-23 12:38 nucliadb/search/api/v1/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-23 12:38 nucliadb/search/api/v1/resource/__init__.py
+-rw-r--r--  2.0 unx     4064 b- defN 24-May-23 12:38 nucliadb/search/api/v1/resource/ask.py
+-rw-r--r--  2.0 unx     5821 b- defN 24-May-23 12:38 nucliadb/search/api/v1/resource/chat.py
+-rw-r--r--  2.0 unx     5303 b- defN 24-May-23 12:38 nucliadb/search/api/v1/resource/search.py
+-rw-r--r--  2.0 unx      833 b- defN 24-May-23 12:38 nucliadb/search/requesters/__init__.py
+-rw-r--r--  2.0 unx     9111 b- defN 24-May-23 12:38 nucliadb/search/requesters/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-23 12:38 nucliadb/search/search/__init__.py
+-rw-r--r--  2.0 unx     2746 b- defN 24-May-23 12:38 nucliadb/search/search/cache.py
+-rw-r--r--  2.0 unx     1154 b- defN 24-May-23 12:38 nucliadb/search/search/exceptions.py
+-rw-r--r--  2.0 unx     5465 b- defN 24-May-23 12:38 nucliadb/search/search/fetch.py
+-rw-r--r--  2.0 unx     6513 b- defN 24-May-23 12:38 nucliadb/search/search/filters.py
+-rw-r--r--  2.0 unx     4612 b- defN 24-May-23 12:38 nucliadb/search/search/find.py
+-rw-r--r--  2.0 unx    17152 b- defN 24-May-23 12:38 nucliadb/search/search/find_merge.py
+-rw-r--r--  2.0 unx    21282 b- defN 24-May-23 12:38 nucliadb/search/search/merge.py
+-rw-r--r--  2.0 unx     1130 b- defN 24-May-23 12:38 nucliadb/search/search/metrics.py
+-rw-r--r--  2.0 unx     8698 b- defN 24-May-23 12:38 nucliadb/search/search/paragraphs.py
+-rw-r--r--  2.0 unx     3026 b- defN 24-May-23 12:38 nucliadb/search/search/predict_proxy.py
+-rw-r--r--  2.0 unx    31093 b- defN 24-May-23 12:38 nucliadb/search/search/query.py
+-rw-r--r--  2.0 unx     3018 b- defN 24-May-23 12:38 nucliadb/search/search/shards.py
+-rw-r--r--  2.0 unx     5101 b- defN 24-May-23 12:38 nucliadb/search/search/summarize.py
+-rw-r--r--  2.0 unx     2438 b- defN 24-May-23 12:38 nucliadb/search/search/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-23 12:38 nucliadb/search/search/chat/__init__.py
+-rw-r--r--  2.0 unx    16676 b- defN 24-May-23 12:38 nucliadb/search/search/chat/ask.py
+-rw-r--r--  2.0 unx     2058 b- defN 24-May-23 12:38 nucliadb/search/search/chat/images.py
+-rw-r--r--  2.0 unx    20793 b- defN 24-May-23 12:38 nucliadb/search/search/chat/prompt.py
+-rw-r--r--  2.0 unx    17543 b- defN 24-May-23 12:38 nucliadb/search/search/chat/query.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-23 12:38 nucliadb/search/tests/__init__.py
+-rw-r--r--  2.0 unx     1295 b- defN 24-May-23 12:38 nucliadb/search/tests/conftest.py
+-rw-r--r--  2.0 unx     6578 b- defN 24-May-23 12:38 nucliadb/search/tests/fixtures.py
+-rw-r--r--  2.0 unx    15480 b- defN 24-May-23 12:38 nucliadb/search/tests/node.py
+-rw-r--r--  2.0 unx      833 b- defN 24-May-23 12:38 nucliadb/search/tests/unit/__init__.py
+-rw-r--r--  2.0 unx     2649 b- defN 24-May-23 12:38 nucliadb/search/tests/unit/test_app.py
+-rw-r--r--  2.0 unx     3374 b- defN 24-May-23 12:38 nucliadb/search/tests/unit/test_find_merge.py
+-rw-r--r--  2.0 unx     1400 b- defN 24-May-23 12:38 nucliadb/search/tests/unit/test_merge.py
+-rw-r--r--  2.0 unx    15721 b- defN 24-May-23 12:38 nucliadb/search/tests/unit/test_predict.py
+-rw-r--r--  2.0 unx     1328 b- defN 24-May-23 12:38 nucliadb/search/tests/unit/test_run.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-23 12:38 nucliadb/search/tests/unit/api/__init__.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-23 12:38 nucliadb/search/tests/unit/api/v1/__init__.py
+-rw-r--r--  2.0 unx     3759 b- defN 24-May-23 12:38 nucliadb/search/tests/unit/api/v1/test_ask.py
+-rw-r--r--  2.0 unx     2966 b- defN 24-May-23 12:38 nucliadb/search/tests/unit/api/v1/test_chat.py
+-rw-r--r--  2.0 unx     2865 b- defN 24-May-23 12:38 nucliadb/search/tests/unit/api/v1/test_predict_proxy.py
+-rw-r--r--  2.0 unx     2901 b- defN 24-May-23 12:38 nucliadb/search/tests/unit/api/v1/test_summarize.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-23 12:38 nucliadb/search/tests/unit/api/v1/resource/__init__.py
+-rw-r--r--  2.0 unx     3040 b- defN 24-May-23 12:38 nucliadb/search/tests/unit/api/v1/resource/test_chat.py
+-rw-r--r--  2.0 unx      833 b- defN 24-May-23 12:38 nucliadb/search/tests/unit/search/__init__.py
+-rw-r--r--  2.0 unx     8586 b- defN 24-May-23 12:38 nucliadb/search/tests/unit/search/test_chat_prompt.py
+-rw-r--r--  2.0 unx     3736 b- defN 24-May-23 12:38 nucliadb/search/tests/unit/search/test_fetch.py
+-rw-r--r--  2.0 unx     4306 b- defN 24-May-23 12:38 nucliadb/search/tests/unit/search/test_filters.py
+-rw-r--r--  2.0 unx     4492 b- defN 24-May-23 12:38 nucliadb/search/tests/unit/search/test_paragraphs.py
+-rw-r--r--  2.0 unx     3496 b- defN 24-May-23 12:38 nucliadb/search/tests/unit/search/test_predict_proxy.py
+-rw-r--r--  2.0 unx     5121 b- defN 24-May-23 12:38 nucliadb/search/tests/unit/search/test_query.py
+-rw-r--r--  2.0 unx      833 b- defN 24-May-23 12:38 nucliadb/search/tests/unit/search/requesters/__init__.py
+-rw-r--r--  2.0 unx     6455 b- defN 24-May-23 12:38 nucliadb/search/tests/unit/search/requesters/test_utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-23 12:38 nucliadb/search/tests/unit/search/search/__init__.py
+-rw-r--r--  2.0 unx     1759 b- defN 24-May-23 12:38 nucliadb/search/tests/unit/search/search/test_shards.py
+-rw-r--r--  2.0 unx     2511 b- defN 24-May-23 12:38 nucliadb/search/tests/unit/search/search/test_utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-23 12:38 nucliadb/standalone/__init__.py
+-rw-r--r--  2.0 unx     6746 b- defN 24-May-23 12:38 nucliadb/standalone/api_router.py
+-rw-r--r--  2.0 unx     5763 b- defN 24-May-23 12:38 nucliadb/standalone/app.py
+-rw-r--r--  2.0 unx     7800 b- defN 24-May-23 12:38 nucliadb/standalone/auth.py
+-rw-r--r--  2.0 unx     5313 b- defN 24-May-23 12:38 nucliadb/standalone/config.py
+-rw-r--r--  2.0 unx     6986 b- defN 24-May-23 12:38 nucliadb/standalone/introspect.py
+-rw-r--r--  2.0 unx     2488 b- defN 24-May-23 12:38 nucliadb/standalone/lifecycle.py
+-rw-r--r--  2.0 unx     1980 b- defN 24-May-23 12:38 nucliadb/standalone/migrations.py
+-rw-r--r--  2.0 unx     1322 b- defN 24-May-23 12:38 nucliadb/standalone/purge.py
+-rw-r--r--  2.0 unx     5636 b- defN 24-May-23 12:38 nucliadb/standalone/run.py
+-rw-r--r--  2.0 unx     5822 b- defN 24-May-23 12:38 nucliadb/standalone/settings.py
+-rw-r--r--  2.0 unx     3132 b- defN 24-May-23 12:38 nucliadb/standalone/versions.py
+-rw-r--r--  2.0 unx     2285 b- defN 24-May-23 12:38 nucliadb/standalone/static/favicon.ico
+-rw-r--r--  2.0 unx     3833 b- defN 24-May-23 12:38 nucliadb/standalone/static/index.html
+-rw-r--r--  2.0 unx     2639 b- defN 24-May-23 12:38 nucliadb/standalone/static/logo.svg
+-rw-r--r--  2.0 unx      835 b- defN 24-May-23 12:38 nucliadb/standalone/tests/__init__.py
+-rw-r--r--  2.0 unx     1294 b- defN 24-May-23 12:38 nucliadb/standalone/tests/conftest.py
+-rw-r--r--  2.0 unx     1319 b- defN 24-May-23 12:38 nucliadb/standalone/tests/fixtures.py
+-rw-r--r--  2.0 unx      833 b- defN 24-May-23 12:38 nucliadb/standalone/tests/unit/__init__.py
+-rw-r--r--  2.0 unx     1722 b- defN 24-May-23 12:38 nucliadb/standalone/tests/unit/test_api_router.py
+-rw-r--r--  2.0 unx     5509 b- defN 24-May-23 12:38 nucliadb/standalone/tests/unit/test_auth.py
+-rw-r--r--  2.0 unx     1334 b- defN 24-May-23 12:38 nucliadb/standalone/tests/unit/test_introspect.py
+-rw-r--r--  2.0 unx     1863 b- defN 24-May-23 12:38 nucliadb/standalone/tests/unit/test_migrations.py
+-rw-r--r--  2.0 unx     1546 b- defN 24-May-23 12:38 nucliadb/standalone/tests/unit/test_run.py
+-rw-r--r--  2.0 unx     1972 b- defN 24-May-23 12:38 nucliadb/standalone/tests/unit/test_versions.py
+-rw-r--r--  2.0 unx     1037 b- defN 24-May-23 12:38 nucliadb/tasks/__init__.py
+-rw-r--r--  2.0 unx     7655 b- defN 24-May-23 12:38 nucliadb/tasks/consumer.py
+-rw-r--r--  2.0 unx      924 b- defN 24-May-23 12:38 nucliadb/tasks/logger.py
+-rw-r--r--  2.0 unx     1378 b- defN 24-May-23 12:38 nucliadb/tasks/models.py
+-rw-r--r--  2.0 unx     3457 b- defN 24-May-23 12:38 nucliadb/tasks/producer.py
+-rw-r--r--  2.0 unx     1753 b- defN 24-May-23 12:38 nucliadb/tasks/registry.py
+-rw-r--r--  2.0 unx     1360 b- defN 24-May-23 12:38 nucliadb/tasks/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-23 12:38 nucliadb/tests/__init__.py
+-rw-r--r--  2.0 unx     1229 b- defN 24-May-23 12:38 nucliadb/tests/conftest.py
+-rw-r--r--  2.0 unx    22365 b- defN 24-May-23 12:38 nucliadb/tests/fixtures.py
+-rw-r--r--  2.0 unx     7549 b- defN 24-May-23 12:38 nucliadb/tests/tikv.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-23 12:38 nucliadb/tests/benchmarks/__init__.py
+-rw-r--r--  2.0 unx     3032 b- defN 24-May-23 12:38 nucliadb/tests/benchmarks/test_search.py
+-rw-r--r--  2.0 unx      919 b- defN 24-May-23 12:38 nucliadb/tests/knowledgeboxes/__init__.py
+-rw-r--r--  2.0 unx     7002 b- defN 24-May-23 12:38 nucliadb/tests/knowledgeboxes/philosophy_books.py
+-rw-r--r--  2.0 unx     3037 b- defN 24-May-23 12:38 nucliadb/tests/knowledgeboxes/ten_dummy_resources.py
+-rw-r--r--  2.0 unx     1148 b- defN 24-May-23 12:38 nucliadb/tests/migrations/__init__.py
+-rw-r--r--  2.0 unx     2726 b- defN 24-May-23 12:38 nucliadb/tests/migrations/test_migration_0017.py
+-rw-r--r--  2.0 unx     3662 b- defN 24-May-23 12:38 nucliadb/tests/migrations/test_migration_0018.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-23 12:38 nucliadb/tests/unit/__init__.py
+-rw-r--r--  2.0 unx     1487 b- defN 24-May-23 12:38 nucliadb/tests/unit/test_field_ids.py
+-rw-r--r--  2.0 unx     2780 b- defN 24-May-23 12:38 nucliadb/tests/unit/test_health.py
+-rw-r--r--  2.0 unx     1543 b- defN 24-May-23 12:38 nucliadb/tests/unit/test_kb_slugs.py
+-rw-r--r--  2.0 unx     7892 b- defN 24-May-23 12:38 nucliadb/tests/unit/test_learning_proxy.py
+-rw-r--r--  2.0 unx     2642 b- defN 24-May-23 12:38 nucliadb/tests/unit/test_metrics_exporter.py
+-rw-r--r--  2.0 unx     1341 b- defN 24-May-23 12:38 nucliadb/tests/unit/test_openapi.py
+-rw-r--r--  2.0 unx     3649 b- defN 24-May-23 12:38 nucliadb/tests/unit/test_purge.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-23 12:38 nucliadb/tests/unit/common/__init__.py
+-rw-r--r--  2.0 unx     1268 b- defN 24-May-23 12:38 nucliadb/tests/unit/common/test_context.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-23 12:38 nucliadb/tests/unit/common/cluster/__init__.py
+-rw-r--r--  2.0 unx    12240 b- defN 24-May-23 12:38 nucliadb/tests/unit/common/cluster/test_cluster.py
+-rw-r--r--  2.0 unx     5387 b- defN 24-May-23 12:38 nucliadb/tests/unit/common/cluster/test_kb_shard_manager.py
+-rw-r--r--  2.0 unx     1428 b- defN 24-May-23 12:38 nucliadb/tests/unit/common/cluster/test_rebalance.py
+-rw-r--r--  2.0 unx     9465 b- defN 24-May-23 12:38 nucliadb/tests/unit/common/cluster/test_rollover.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-23 12:38 nucliadb/tests/unit/common/cluster/discovery/__init__.py
+-rw-r--r--  2.0 unx     5627 b- defN 24-May-23 12:38 nucliadb/tests/unit/common/cluster/discovery/test_k8s.py
+-rw-r--r--  2.0 unx      833 b- defN 24-May-23 12:38 nucliadb/tests/unit/common/cluster/standalone/__init__.py
+-rw-r--r--  2.0 unx     3761 b- defN 24-May-23 12:38 nucliadb/tests/unit/common/cluster/standalone/test_service.py
+-rw-r--r--  2.0 unx     2136 b- defN 24-May-23 12:38 nucliadb/tests/unit/common/cluster/standalone/test_utils.py
+-rw-r--r--  2.0 unx      833 b- defN 24-May-23 12:38 nucliadb/tests/unit/common/maindb/__init__.py
+-rw-r--r--  2.0 unx     3579 b- defN 24-May-23 12:38 nucliadb/tests/unit/common/maindb/test_driver.py
+-rw-r--r--  2.0 unx     1869 b- defN 24-May-23 12:38 nucliadb/tests/unit/common/maindb/test_tikv.py
+-rw-r--r--  2.0 unx     3213 b- defN 24-May-23 12:38 nucliadb/tests/unit/common/maindb/test_utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-23 12:38 nucliadb/tests/unit/export_import/__init__.py
+-rw-r--r--  2.0 unx     1435 b- defN 24-May-23 12:38 nucliadb/tests/unit/export_import/test_datamanager.py
+-rw-r--r--  2.0 unx     9706 b- defN 24-May-23 12:38 nucliadb/tests/unit/export_import/test_utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-23 12:38 nucliadb/tests/unit/migrator/__init__.py
+-rw-r--r--  2.0 unx     3233 b- defN 24-May-23 12:38 nucliadb/tests/unit/migrator/test_migrator.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-23 12:38 nucliadb/tests/unit/tasks/__init__.py
+-rw-r--r--  2.0 unx     1375 b- defN 24-May-23 12:38 nucliadb/tests/unit/tasks/conftest.py
+-rw-r--r--  2.0 unx     2714 b- defN 24-May-23 12:38 nucliadb/tests/unit/tasks/test_consumer.py
+-rw-r--r--  2.0 unx     3189 b- defN 24-May-23 12:38 nucliadb/tests/unit/tasks/test_producer.py
+-rw-r--r--  2.0 unx     1827 b- defN 24-May-23 12:38 nucliadb/tests/unit/tasks/test_tasks.py
+-rw-r--r--  2.0 unx     2507 b- defN 24-May-23 12:38 nucliadb/tests/utils/__init__.py
+-rw-r--r--  2.0 unx     1797 b- defN 24-May-23 12:38 nucliadb/tests/utils/aiohttp_session.py
+-rw-r--r--  2.0 unx     2533 b- defN 24-May-23 12:38 nucliadb/tests/utils/entities.py
+-rw-r--r--  2.0 unx     6327 b- defN 24-May-23 12:38 nucliadb/tests/utils/broker_messages/__init__.py
+-rw-r--r--  2.0 unx     7557 b- defN 24-May-23 12:38 nucliadb/tests/utils/broker_messages/fields.py
+-rw-r--r--  2.0 unx     1196 b- defN 24-May-23 12:38 nucliadb/tests/utils/broker_messages/helpers.py
+-rw-r--r--  2.0 unx     1325 b- defN 24-May-23 12:38 nucliadb/train/__init__.py
+-rw-r--r--  2.0 unx     3530 b- defN 24-May-23 12:38 nucliadb/train/app.py
+-rw-r--r--  2.0 unx     3800 b- defN 24-May-23 12:38 nucliadb/train/generator.py
+-rw-r--r--  2.0 unx     1698 b- defN 24-May-23 12:38 nucliadb/train/lifecycle.py
+-rw-r--r--  2.0 unx     1198 b- defN 24-May-23 12:38 nucliadb/train/models.py
+-rw-r--r--  2.0 unx     5706 b- defN 24-May-23 12:38 nucliadb/train/nodes.py
+-rw-r--r--  2.0 unx     1400 b- defN 24-May-23 12:38 nucliadb/train/run.py
+-rw-r--r--  2.0 unx     5926 b- defN 24-May-23 12:38 nucliadb/train/servicer.py
+-rw-r--r--  2.0 unx     1415 b- defN 24-May-23 12:38 nucliadb/train/settings.py
+-rw-r--r--  2.0 unx     1496 b- defN 24-May-23 12:38 nucliadb/train/types.py
+-rw-r--r--  2.0 unx     3265 b- defN 24-May-23 12:38 nucliadb/train/upload.py
+-rw-r--r--  2.0 unx     6420 b- defN 24-May-23 12:38 nucliadb/train/uploader.py
+-rw-r--r--  2.0 unx     3179 b- defN 24-May-23 12:38 nucliadb/train/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-23 12:38 nucliadb/train/api/__init__.py
+-rw-r--r--  2.0 unx     1479 b- defN 24-May-23 12:38 nucliadb/train/api/utils.py
+-rw-r--r--  2.0 unx      928 b- defN 24-May-23 12:38 nucliadb/train/api/v1/__init__.py
+-rw-r--r--  2.0 unx     2071 b- defN 24-May-23 12:38 nucliadb/train/api/v1/check.py
+-rw-r--r--  2.0 unx      910 b- defN 24-May-23 12:38 nucliadb/train/api/v1/router.py
+-rw-r--r--  2.0 unx     1908 b- defN 24-May-23 12:38 nucliadb/train/api/v1/shards.py
+-rw-r--r--  2.0 unx     2135 b- defN 24-May-23 12:38 nucliadb/train/api/v1/trainset.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-23 12:38 nucliadb/train/generators/__init__.py
+-rw-r--r--  2.0 unx     3723 b- defN 24-May-23 12:38 nucliadb/train/generators/field_classifier.py
+-rw-r--r--  2.0 unx     6712 b- defN 24-May-23 12:38 nucliadb/train/generators/image_classifier.py
+-rw-r--r--  2.0 unx     2789 b- defN 24-May-23 12:38 nucliadb/train/generators/paragraph_classifier.py
+-rw-r--r--  2.0 unx     3590 b- defN 24-May-23 12:38 nucliadb/train/generators/paragraph_streaming.py
+-rw-r--r--  2.0 unx     5372 b- defN 24-May-23 12:38 nucliadb/train/generators/question_answer_streaming.py
+-rw-r--r--  2.0 unx     5160 b- defN 24-May-23 12:38 nucliadb/train/generators/sentence_classifier.py
+-rw-r--r--  2.0 unx    10446 b- defN 24-May-23 12:38 nucliadb/train/generators/token_classifier.py
+-rw-r--r--  2.0 unx     3877 b- defN 24-May-23 12:38 nucliadb/train/generators/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-23 12:38 nucliadb/train/tests/__init__.py
+-rw-r--r--  2.0 unx     1125 b- defN 24-May-23 12:38 nucliadb/train/tests/conftest.py
+-rw-r--r--  2.0 unx    11053 b- defN 24-May-23 12:38 nucliadb/train/tests/fixtures.py
+-rw-r--r--  2.0 unx     4598 b- defN 24-May-23 12:38 nucliadb/train/tests/test_field_classification.py
+-rw-r--r--  2.0 unx     2729 b- defN 24-May-23 12:38 nucliadb/train/tests/test_get_entities.py
+-rw-r--r--  2.0 unx     1876 b- defN 24-May-23 12:38 nucliadb/train/tests/test_get_info.py
+-rw-r--r--  2.0 unx     1382 b- defN 24-May-23 12:38 nucliadb/train/tests/test_get_ontology.py
+-rw-r--r--  2.0 unx     2417 b- defN 24-May-23 12:38 nucliadb/train/tests/test_get_ontology_count.py
+-rw-r--r--  2.0 unx     7669 b- defN 24-May-23 12:38 nucliadb/train/tests/test_image_classification.py
+-rw-r--r--  2.0 unx     1416 b- defN 24-May-23 12:38 nucliadb/train/tests/test_list_fields.py
+-rw-r--r--  2.0 unx     2944 b- defN 24-May-23 12:38 nucliadb/train/tests/test_list_paragraphs.py
+-rw-r--r--  2.0 unx     1423 b- defN 24-May-23 12:38 nucliadb/train/tests/test_list_resources.py
+-rw-r--r--  2.0 unx     2947 b- defN 24-May-23 12:38 nucliadb/train/tests/test_list_sentences.py
+-rw-r--r--  2.0 unx     4645 b- defN 24-May-23 12:38 nucliadb/train/tests/test_paragraph_classification.py
+-rw-r--r--  2.0 unx     4320 b- defN 24-May-23 12:38 nucliadb/train/tests/test_paragraph_streaming.py
+-rw-r--r--  2.0 unx     8751 b- defN 24-May-23 12:38 nucliadb/train/tests/test_question_answer_streaming.py
+-rw-r--r--  2.0 unx     5051 b- defN 24-May-23 12:38 nucliadb/train/tests/test_sentence_classification.py
+-rw-r--r--  2.0 unx     5583 b- defN 24-May-23 12:38 nucliadb/train/tests/test_token_classification.py
+-rw-r--r--  2.0 unx     3324 b- defN 24-May-23 12:38 nucliadb/train/tests/utils.py
+-rw-r--r--  2.0 unx     1328 b- defN 24-May-23 12:38 nucliadb/writer/__init__.py
+-rw-r--r--  2.0 unx     4268 b- defN 24-May-23 12:38 nucliadb/writer/app.py
+-rw-r--r--  2.0 unx    19483 b- defN 24-May-23 12:38 nucliadb/writer/back_pressure.py
+-rw-r--r--  2.0 unx      972 b- defN 24-May-23 12:38 nucliadb/writer/exceptions.py
+-rw-r--r--  2.0 unx     1953 b- defN 24-May-23 12:38 nucliadb/writer/lifecycle.py
+-rw-r--r--  2.0 unx     1032 b- defN 24-May-23 12:38 nucliadb/writer/openapi.py
+-rw-r--r--  2.0 unx     1448 b- defN 24-May-23 12:38 nucliadb/writer/run.py
+-rw-r--r--  2.0 unx     3103 b- defN 24-May-23 12:38 nucliadb/writer/settings.py
+-rw-r--r--  2.0 unx     1036 b- defN 24-May-23 12:38 nucliadb/writer/utilities.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-23 12:38 nucliadb/writer/api/__init__.py
+-rw-r--r--  2.0 unx     1429 b- defN 24-May-23 12:38 nucliadb/writer/api/constants.py
+-rw-r--r--  2.0 unx     1095 b- defN 24-May-23 12:38 nucliadb/writer/api/v1/__init__.py
+-rw-r--r--  2.0 unx     6421 b- defN 24-May-23 12:38 nucliadb/writer/api/v1/export_import.py
+-rw-r--r--  2.0 unx    24482 b- defN 24-May-23 12:38 nucliadb/writer/api/v1/field.py
+-rw-r--r--  2.0 unx     5248 b- defN 24-May-23 12:38 nucliadb/writer/api/v1/knowledgebox.py
+-rw-r--r--  2.0 unx     2058 b- defN 24-May-23 12:38 nucliadb/writer/api/v1/learning_config.py
+-rw-r--r--  2.0 unx    18628 b- defN 24-May-23 12:38 nucliadb/writer/api/v1/resource.py
+-rw-r--r--  2.0 unx     1034 b- defN 24-May-23 12:38 nucliadb/writer/api/v1/router.py
+-rw-r--r--  2.0 unx    10216 b- defN 24-May-23 12:38 nucliadb/writer/api/v1/services.py
+-rw-r--r--  2.0 unx    30985 b- defN 24-May-23 12:38 nucliadb/writer/api/v1/upload.py
+-rw-r--r--  2.0 unx     1612 b- defN 24-May-23 12:38 nucliadb/writer/layouts/__init__.py
+-rw-r--r--  2.0 unx     2115 b- defN 24-May-23 12:38 nucliadb/writer/layouts/v1.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-23 12:38 nucliadb/writer/resource/__init__.py
+-rw-r--r--  2.0 unx     1425 b- defN 24-May-23 12:38 nucliadb/writer/resource/audit.py
+-rw-r--r--  2.0 unx    10968 b- defN 24-May-23 12:38 nucliadb/writer/resource/basic.py
+-rw-r--r--  2.0 unx    16740 b- defN 24-May-23 12:38 nucliadb/writer/resource/field.py
+-rw-r--r--  2.0 unx     2022 b- defN 24-May-23 12:38 nucliadb/writer/resource/origin.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-23 12:38 nucliadb/writer/tests/__init__.py
+-rw-r--r--  2.0 unx     1200 b- defN 24-May-23 12:38 nucliadb/writer/tests/conftest.py
+-rw-r--r--  2.0 unx     5971 b- defN 24-May-23 12:38 nucliadb/writer/tests/fixtures.py
+-rw-r--r--  2.0 unx    15472 b- defN 24-May-23 12:38 nucliadb/writer/tests/test_fields.py
+-rw-r--r--  2.0 unx    25999 b- defN 24-May-23 12:38 nucliadb/writer/tests/test_files.py
+-rw-r--r--  2.0 unx     1729 b- defN 24-May-23 12:38 nucliadb/writer/tests/test_knowledgebox.py
+-rw-r--r--  2.0 unx     4400 b- defN 24-May-23 12:38 nucliadb/writer/tests/test_reprocess_file_field.py
+-rw-r--r--  2.0 unx    16857 b- defN 24-May-23 12:38 nucliadb/writer/tests/test_resources.py
+-rw-r--r--  2.0 unx     5120 b- defN 24-May-23 12:38 nucliadb/writer/tests/test_service.py
+-rw-r--r--  2.0 unx     6054 b- defN 24-May-23 12:38 nucliadb/writer/tests/test_tus.py
+-rw-r--r--  2.0 unx     1287 b- defN 24-May-23 12:38 nucliadb/writer/tests/utils.py
+-rw-r--r--  2.0 unx     5226 b- defN 24-May-23 12:38 nucliadb/writer/tus/__init__.py
+-rw-r--r--  2.0 unx     5082 b- defN 24-May-23 12:38 nucliadb/writer/tus/dm.py
+-rw-r--r--  2.0 unx     2186 b- defN 24-May-23 12:38 nucliadb/writer/tus/exceptions.py
+-rw-r--r--  2.0 unx    14527 b- defN 24-May-23 12:38 nucliadb/writer/tus/gcs.py
+-rw-r--r--  2.0 unx     5849 b- defN 24-May-23 12:38 nucliadb/writer/tus/local.py
+-rw-r--r--  2.0 unx     4367 b- defN 24-May-23 12:38 nucliadb/writer/tus/pg.py
+-rw-r--r--  2.0 unx     9069 b- defN 24-May-23 12:38 nucliadb/writer/tus/s3.py
+-rw-r--r--  2.0 unx     4734 b- defN 24-May-23 12:38 nucliadb/writer/tus/storage.py
+-rw-r--r--  2.0 unx     2556 b- defN 24-May-23 12:38 nucliadb/writer/tus/utils.py
+-rw-r--r--  2.0 unx     4423 b- defN 24-May-23 12:40 nucliadb-4.0.0.post540.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-23 12:40 nucliadb-4.0.0.post540.dist-info/WHEEL
+-rw-r--r--  2.0 unx     1268 b- defN 24-May-23 12:40 nucliadb-4.0.0.post540.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       20 b- defN 24-May-23 12:40 nucliadb-4.0.0.post540.dist-info/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 24-May-23 12:39 nucliadb-4.0.0.post540.dist-info/zip-safe
+-rw-rw-r--  2.0 unx    43366 b- defN 24-May-23 12:40 nucliadb-4.0.0.post540.dist-info/RECORD
+462 files, 2261344 bytes uncompressed, 696422 bytes compressed:  69.2%
```

## zipnote {}

```diff
@@ -153,14 +153,17 @@
 
 Filename: nucliadb/common/context/fastapi.py
 Comment: 
 
 Filename: nucliadb/common/datamanagers/__init__.py
 Comment: 
 
+Filename: nucliadb/common/datamanagers/atomic.py
+Comment: 
+
 Filename: nucliadb/common/datamanagers/cluster.py
 Comment: 
 
 Filename: nucliadb/common/datamanagers/entities.py
 Comment: 
 
 Filename: nucliadb/common/datamanagers/exceptions.py
@@ -1299,17 +1302,14 @@
 
 Filename: nucliadb/writer/resource/field.py
 Comment: 
 
 Filename: nucliadb/writer/resource/origin.py
 Comment: 
 
-Filename: nucliadb/writer/resource/slug.py
-Comment: 
-
 Filename: nucliadb/writer/tests/__init__.py
 Comment: 
 
 Filename: nucliadb/writer/tests/conftest.py
 Comment: 
 
 Filename: nucliadb/writer/tests/fixtures.py
@@ -1362,26 +1362,26 @@
 
 Filename: nucliadb/writer/tus/storage.py
 Comment: 
 
 Filename: nucliadb/writer/tus/utils.py
 Comment: 
 
-Filename: nucliadb-4.0.0.post539.dist-info/METADATA
+Filename: nucliadb-4.0.0.post540.dist-info/METADATA
 Comment: 
 
-Filename: nucliadb-4.0.0.post539.dist-info/WHEEL
+Filename: nucliadb-4.0.0.post540.dist-info/WHEEL
 Comment: 
 
-Filename: nucliadb-4.0.0.post539.dist-info/entry_points.txt
+Filename: nucliadb-4.0.0.post540.dist-info/entry_points.txt
 Comment: 
 
-Filename: nucliadb-4.0.0.post539.dist-info/top_level.txt
+Filename: nucliadb-4.0.0.post540.dist-info/top_level.txt
 Comment: 
 
-Filename: nucliadb-4.0.0.post539.dist-info/zip-safe
+Filename: nucliadb-4.0.0.post540.dist-info/zip-safe
 Comment: 
 
-Filename: nucliadb-4.0.0.post539.dist-info/RECORD
+Filename: nucliadb-4.0.0.post540.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## nucliadb/common/datamanagers/__init__.py

```diff
@@ -25,27 +25,29 @@
 #   - Transactions are managed OUTSIDE of the datamanagers module
 #   - There shouldn't be ANY db commits in the datamanagers module, that is handled outside right now.
 #   - Module level functions only
 #   - First argument is always a transaction, all other arguments are keyword arguments and must be explicit
 #     (better for readability and code editors)
 # ==============================================================================
 from . import (
+    atomic,
     cluster,
     entities,
     exceptions,
     kb,
     labels,
     processing,
     resources,
     rollover,
     synonyms,
 )
 from .utils import with_transaction
 
 __all__ = (
+    "atomic",
     "cluster",
     "entities",
     "exceptions",
     "kb",
     "labels",
     "processing",
     "resources",
```

## nucliadb/writer/api/v1/export_import.py

```diff
@@ -58,17 +58,16 @@
     tags=["Knowledge Boxes"],
     response_model=CreateExportResponse,
 )
 @requires_one([NucliaDBRoles.MANAGER, NucliaDBRoles.WRITER])
 @version(1)
 async def start_kb_export_endpoint(request: Request, kbid: str):
     context = get_app_context(request.app)
-    async with datamanagers.with_transaction(read_only=True) as txn:
-        if not await datamanagers.kb.exists_kb(txn, kbid=kbid):
-            return HTTPClientError(status_code=404, detail="Knowledge Box not found")
+    if not await datamanagers.atomic.kb.exists_kb(kbid=kbid):
+        return HTTPClientError(status_code=404, detail="Knowledge Box not found")
 
     export_id = uuid4().hex
     if in_standalone_mode():
         # In standalone mode, exports are generated at download time.
         # We simply return an export_id to keep the API consistent with hosted nucliadb.
         return CreateExportResponse(export_id=export_id)
     else:
@@ -83,17 +82,16 @@
     tags=["Knowledge Boxes"],
     response_model=CreateImportResponse,
 )
 @requires_one([NucliaDBRoles.MANAGER, NucliaDBRoles.WRITER])
 @version(1)
 async def start_kb_import_endpoint(request: Request, kbid: str):
     context = get_app_context(request.app)
-    async with datamanagers.with_transaction(read_only=True) as txn:
-        if not await datamanagers.kb.exists_kb(txn, kbid=kbid):
-            return HTTPClientError(status_code=404, detail="Knowledge Box not found")
+    if not await datamanagers.atomic.kb.exists_kb(kbid=kbid):
+        return HTTPClientError(status_code=404, detail="Knowledge Box not found")
 
     await maybe_back_pressure(request, kbid)
 
     stream = stream_compatible_with_kb(kbid, request.stream())
     try:
         import_id = uuid4().hex
         if in_standalone_mode():
```

## nucliadb/writer/api/v1/resource.py

```diff
@@ -51,15 +51,14 @@
     parse_basic,
     parse_basic_modify,
     set_status,
     set_status_modify,
 )
 from nucliadb.writer.resource.field import extract_fields, parse_fields
 from nucliadb.writer.resource.origin import parse_extra, parse_origin
-from nucliadb.writer.resource.slug import resource_slug_exists
 from nucliadb.writer.utilities import get_processing
 from nucliadb_models.resource import NucliaDBRoles
 from nucliadb_models.writer import (
     CreateResourcePayload,
     ResourceCreated,
     ResourceUpdated,
     UpdateResourcePayload,
@@ -115,15 +114,17 @@
     toprocess.kbid = kbid
     writer.uuid = uuid
     toprocess.uuid = uuid
     toprocess.source = Source.HTTP
     toprocess.title = item.title
 
     if item.slug:
-        if await resource_slug_exists(kbid, item.slug):
+        from nucliadb.common import datamanagers
+
+        if await datamanagers.atomic.resources.slug_exists(kbid=kbid, slug=item.slug):
             raise HTTPException(
                 status_code=409, detail=f"Resource slug {item.slug} already exists"
             )
         writer.slug = item.slug
         toprocess.slug = item.slug
 
     parse_audit(writer.audit, request)
@@ -571,34 +572,24 @@
     index_req.reindex_vectors = reindex_vectors
 
     await ingest.ReIndex(index_req)  # type: ignore
     return Response(status_code=200)
 
 
 async def get_rid_from_slug_or_raise_error(kbid: str, rslug: str) -> str:
-    async with datamanagers.with_transaction(read_only=True) as txn:
-        rid = await datamanagers.resources.get_resource_uuid_from_slug(
-            txn, kbid=kbid, slug=rslug
-        )
+    rid = await datamanagers.atomic.resources.get_resource_uuid_from_slug(
+        kbid=kbid, slug=rslug
+    )
     if not rid:
         raise HTTPException(status_code=404, detail="Resource does not exist")
     return rid
 
 
-async def resource_exists(kbid: str, rid: str) -> bool:
-    async with datamanagers.with_transaction(read_only=True) as txn:
-        exists = await datamanagers.resources.resource_exists(txn, kbid=kbid, rid=rid)
-    return exists
-
-
-async def validate_rid_exists_or_raise_error(
-    kbid: str,
-    rid: str,
-):
-    if not (await resource_exists(kbid, rid)):
+async def validate_rid_exists_or_raise_error(kbid: str, rid: str):
+    if not (await datamanagers.atomic.resources.resource_exists(kbid=kbid, rid=rid)):
         raise HTTPException(status_code=404, detail="Resource does not exist")
 
 
 def maybe_mark_reindex(message: BrokerMessage, item: UpdateResourcePayload):
     if needs_resource_reindex(item):
         message.reindex = True
```

## nucliadb/writer/api/v1/upload.py

```diff
@@ -31,21 +31,21 @@
 from fastapi.requests import Request
 from fastapi.responses import Response
 from fastapi_versioning import version  # type: ignore
 from nucliadb_protos.resources_pb2 import FieldFile, Metadata
 from nucliadb_protos.writer_pb2 import BrokerMessage
 from starlette.requests import Request as StarletteRequest
 
+from nucliadb.common import datamanagers
 from nucliadb.ingest.orm.utils import set_title
 from nucliadb.ingest.processing import PushPayload, Source
 from nucliadb.models.responses import HTTPClientError
 from nucliadb.writer import SERVICE_NAME
 from nucliadb.writer.api.v1.resource import (
     get_rid_from_slug_or_raise_error,
-    resource_exists,
     validate_rid_exists_or_raise_error,
 )
 from nucliadb.writer.back_pressure import maybe_back_pressure
 from nucliadb.writer.resource.audit import parse_audit
 from nucliadb.writer.resource.basic import parse_basic
 from nucliadb.writer.resource.field import parse_fields
 from nucliadb.writer.resource.origin import parse_extra, parse_origin
@@ -787,25 +787,27 @@
 
     This function assumes KB exists
     """
 
     if rid is None:
         # we are going to create a new resource and a field
         if md5 is not None:
-            exists = await resource_exists(kbid, md5)
+            exists = await datamanagers.atomic.resources.resource_exists(
+                kbid=kbid, rid=md5
+            )
             if exists:
                 raise HTTPConflict(
                     "A resource with the same uploaded file already exists"
                 )
             rid = md5
         else:
             rid = uuid.uuid4().hex
     else:
         # we're adding a field to a resource
-        exists = await resource_exists(kbid, rid)
+        exists = await datamanagers.atomic.resources.resource_exists(kbid=kbid, rid=rid)
         if not exists:
             raise HTTPNotFound("Resource is not found or not yet available")
 
     if field is None:
         if md5 is None:
             field = uuid.uuid4().hex
         else:
```

## nucliadb/writer/tests/test_reprocess_file_field.py

```diff
@@ -18,16 +18,16 @@
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 #
 from typing import AsyncIterator
 from unittest.mock import AsyncMock
 
 import pytest
 
+from nucliadb.common import datamanagers
 from nucliadb.ingest.processing import ProcessingInfo
-from nucliadb.writer.api.v1.resource import resource_exists
 from nucliadb.writer.api.v1.router import KB_PREFIX, RESOURCE_PREFIX, RESOURCES_PREFIX
 from nucliadb.writer.tests.utils import load_file_as_FileB64_payload
 from nucliadb.writer.utilities import get_processing
 from nucliadb_models.resource import NucliaDBRoles, QueueType
 
 
 @pytest.fixture(scope="function")
@@ -67,15 +67,17 @@
                     }
                 },
             },
         )
         assert resp.status_code == 201
         rid = resp.json()["uuid"]
 
-        assert (await resource_exists(kbid, rid)) is True
+        assert (
+            await datamanagers.atomic.resources.resource_exists(kbid=kbid, rid=rid)
+        ) is True
 
     yield kbid, rid, field_id
 
     async with writer_api(roles=[NucliaDBRoles.WRITER]) as client:
         resp = await client.delete(
             f"/{KB_PREFIX}/{kbid}/{RESOURCE_PREFIX}/{rid}",
         )
```

## nucliadb/writer/tests/test_resources.py

```diff
@@ -21,19 +21,19 @@
 from typing import Any, Callable, Optional
 from unittest.mock import AsyncMock  # type: ignore
 
 import pytest
 from httpx import AsyncClient
 
 import nucliadb_models
+from nucliadb.common import datamanagers
 from nucliadb.common.maindb.local import LocalDriver
 from nucliadb.common.maindb.redis import RedisDriver
 from nucliadb.ingest.orm.resource import Resource
 from nucliadb.ingest.processing import PushPayload
-from nucliadb.writer.api.v1.resource import resource_exists
 from nucliadb.writer.api.v1.router import (
     KB_PREFIX,
     RESOURCE_PREFIX,
     RESOURCES_PREFIX,
     RSLUG_PREFIX,
 )
 from nucliadb.writer.tests.test_fields import (
@@ -215,15 +215,19 @@
         assert resp.status_code == 201
         data = resp.json()
         assert "uuid" in data
         assert "seqid" in data
         assert "elapsed" in data
         rid = data["uuid"]
 
-        assert (await resource_exists(knowledgebox_id, rid)) is True
+        assert (
+            await datamanagers.atomic.resources.resource_exists(
+                kbid=knowledgebox_id, rid=rid
+            )
+        ) is True
 
         # Test update resource
         resp = await client.patch(
             f"/{KB_PREFIX}/{knowledgebox_id}/{RESOURCE_PREFIX}/{rid}",
             json={},
         )
         assert resp.status_code == 200
@@ -237,15 +241,19 @@
         assert resp.status_code == 404
 
         resp = await client.delete(
             f"/{KB_PREFIX}/{knowledgebox_id}/{RESOURCE_PREFIX}/{rid}",
         )
         assert resp.status_code == 204
 
-        assert (await resource_exists(knowledgebox_id, rid)) is False
+        assert (
+            await datamanagers.atomic.resources.resource_exists(
+                kbid=knowledgebox_id, rid=rid
+            )
+        ) is False
 
 
 @pytest.mark.asyncio
 async def test_reprocess_resource(
     writer_api: Callable[..., AsyncClient],
     test_resource: Resource,
     mocker,
```

## Comparing `nucliadb-4.0.0.post539.dist-info/METADATA` & `nucliadb-4.0.0.post540.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nucliadb
-Version: 4.0.0.post539
+Version: 4.0.0.post540
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
-Requires-Dist: nucliadb-telemetry[all] >=4.0.0.post539
-Requires-Dist: nucliadb-utils[cache,fastapi,storages] >=4.0.0.post539
-Requires-Dist: nucliadb-protos >=4.0.0.post539
-Requires-Dist: nucliadb-models >=4.0.0.post539
+Requires-Dist: nucliadb-telemetry[all] >=4.0.0.post540
+Requires-Dist: nucliadb-utils[cache,fastapi,storages] >=4.0.0.post540
+Requires-Dist: nucliadb-protos >=4.0.0.post540
+Requires-Dist: nucliadb-models >=4.0.0.post540
 Requires-Dist: nucliadb-admin-assets >=1.0.0.post1224
 Requires-Dist: nucliadb-node-binding >=2.26.0
 Requires-Dist: uvicorn <0.19.0
 Requires-Dist: argdantic
 Requires-Dist: aiohttp >=3.9.4
 Requires-Dist: lru-dict >=1.1.7
 Requires-Dist: backoff
```

## Comparing `nucliadb-4.0.0.post539.dist-info/entry_points.txt` & `nucliadb-4.0.0.post540.dist-info/entry_points.txt`

 * *Files identical despite different names*

## Comparing `nucliadb-4.0.0.post539.dist-info/RECORD` & `nucliadb-4.0.0.post540.dist-info/RECORD`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,16 @@
 nucliadb/common/cluster/standalone/__init__.py,sha256=itSI7dtTwFP55YMX4iK7JzdMHS5CQVUiB1XzQu4UBh8,833
 nucliadb/common/cluster/standalone/grpc_node_binding.py,sha256=Rgw6w8vICjieoqhvhoHZ6mUgXbJpyXHvqpFPQ96N1yA,13712
 nucliadb/common/cluster/standalone/index_node.py,sha256=aKpkAEosp9qbd-77fYgE1AAnDc-6ER05cA_HJtkeBT0,4683
 nucliadb/common/cluster/standalone/service.py,sha256=tJI5Gc-cu4uprC84bcLQr4CMW0hBS9T2YX_Ex6zeyuI,3444
 nucliadb/common/cluster/standalone/utils.py,sha256=Y6Ni9P5piE9EeacQb4L5-o_TisAk2fl4btLwAV3tt8g,3545
 nucliadb/common/context/__init__.py,sha256=BuPPLOpTTzgD4oRb6mgmjPu-gRIaq4NeZTjx8FxAIV0,3440
 nucliadb/common/context/fastapi.py,sha256=qsxQ8s5dl67uCATrwdJCXA9JDfVn3DqxgsiWf6MUJhE,1628
-nucliadb/common/datamanagers/__init__.py,sha256=BEBU1dnrSWjQIe1DzBN5jJJHyR4C_Bp2_GDivoxPlrg,1880
+nucliadb/common/datamanagers/__init__.py,sha256=poRbdgWsxkqTjVRUvj4wx6zfSsiXSBT6Dm7ydkp35Ps,1906
+nucliadb/common/datamanagers/atomic.py,sha256=m2wDWIEq8EXugvhsJI7fePsdse5SsH0Y8Fl5C8lrDOM,2651
 nucliadb/common/datamanagers/cluster.py,sha256=Rc_gWufL-Fx3zQ7WlgCFYBPQD9fPjUvHkyW0QK6hBSg,1451
 nucliadb/common/datamanagers/entities.py,sha256=vQe_xdyqqsII0wmqKWp1yxVTFmB67Tc6bnVxezRUVK0,5383
 nucliadb/common/datamanagers/exceptions.py,sha256=Atz_PP_GGq4jgJaWcAkcRbHBoBaGcC9yJvFteylKtTE,883
 nucliadb/common/datamanagers/kb.py,sha256=zkG3lVbGFFLtjcTlJvJDtTY6S55xdty1nSlwI4xDEQ4,3994
 nucliadb/common/datamanagers/labels.py,sha256=2pN8RrFNTXLitDo44CS3AApjCjbv-2ALkqjwHVR_Mb0,5389
 nucliadb/common/datamanagers/processing.py,sha256=gdCHGzF2LiHOapsg4oaYFYNxACwaCbN1z3kw7iHTuNc,1599
 nucliadb/common/datamanagers/resources.py,sha256=7YI2-KN22fXbj9FqKGZQGN-bUH26hCt9CBrJUtAclsI,12177
@@ -414,49 +415,48 @@
 nucliadb/writer/openapi.py,sha256=thqCO1ht_RJgOkXs-aIsv8aXJrU5z8wo2n05l2_LqMs,1032
 nucliadb/writer/run.py,sha256=euVZ_rtHDXs-O1kB-Pt1Id8eft9CYVpWH3zJzEoEqls,1448
 nucliadb/writer/settings.py,sha256=EGY6ZKg-BTKD0xPRIam7EN_FxAQEU_eb5ywNCQOQEg0,3103
 nucliadb/writer/utilities.py,sha256=AZ5qEny1Xm0IDsFtH13oJa2usvJZK8f0FdgF1LrnLCw,1036
 nucliadb/writer/api/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
 nucliadb/writer/api/constants.py,sha256=b63uWvu7_bwg51R6EL5DaJwoT550Ih4GhVXzvEYLQNQ,1429
 nucliadb/writer/api/v1/__init__.py,sha256=FVn7N9VJ6bsEoy4TRnkclr4Umd5hECiwPXVqRnJ8BME,1095
-nucliadb/writer/api/v1/export_import.py,sha256=SucHn2UX0hKRpfs_AYv8MNq-DPu1DIlSORd_K4N-cjk,6571
+nucliadb/writer/api/v1/export_import.py,sha256=9Gqxq1EAPOXCX80F2G7s0UVkvMV1Kgwo66o5sHn2KGY,6421
 nucliadb/writer/api/v1/field.py,sha256=Yi0F1IUin2TaQXyh9QDSwwzrqfjKw7nrAVbfnhl7z3o,24482
 nucliadb/writer/api/v1/knowledgebox.py,sha256=624Uv5_UHacWLv1p2YoMAR7oFPUlM9VgmiwsuJezqWk,5248
 nucliadb/writer/api/v1/learning_config.py,sha256=GaYaagjBrVG9ZxrWQyVQfqGMQV3tAJjqJ5CStaKhktU,2058
-nucliadb/writer/api/v1/resource.py,sha256=BBgRL4pQydm1arcsRCV-Y8FB1OBDggjQ9yZzxGVWivg,18893
+nucliadb/writer/api/v1/resource.py,sha256=-pqZi7riP-EF-eGJsttko5PVA_-0I1oE5SuIxORTKB8,18628
 nucliadb/writer/api/v1/router.py,sha256=RjuoWLpZer6Kl2BW_wznpNo6XL3BOpdTGqXZCn3QrrQ,1034
 nucliadb/writer/api/v1/services.py,sha256=uK6XZnbw3zGT83SzPMFgQPLLU4IFrT3g-0_VOj2DXbA,10216
-nucliadb/writer/api/v1/upload.py,sha256=hkyXA_YlvH5j9jdf48rdmUuSf8T29hUXwBD0DNgLUP0,30857
+nucliadb/writer/api/v1/upload.py,sha256=6TZpT-_g4MdnKGxE6vWs0065HvwZjDPXFdUpEXgUlZ8,30985
 nucliadb/writer/layouts/__init__.py,sha256=Siod9W963CG5gJa20GSTw9VemAFgsMmJDbUspbrYAyE,1612
 nucliadb/writer/layouts/v1.py,sha256=Yc2idmfrpCS8js_XJByNWA_tmt2WeKoWvidLHoTPXoo,2115
 nucliadb/writer/resource/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
 nucliadb/writer/resource/audit.py,sha256=SXPu_hdNBlm9uCSl666UQL7hzMx9zYVbBLT_U7ro8Gs,1425
 nucliadb/writer/resource/basic.py,sha256=eSWW6u6U3e0KjjdFwp9YQokojoDepl5vmJfbE2MQACM,10968
 nucliadb/writer/resource/field.py,sha256=woPN-1bIC6eMXtvggMuvcVwbNAGLpS7GIz8pkO9UNz4,16740
 nucliadb/writer/resource/origin.py,sha256=3Y2zVtG_v0U6uMbDhW9Yl7KKHKt5V3T5_v3iCpqdBEk,2022
-nucliadb/writer/resource/slug.py,sha256=CMhnYBJIrKHshv5T93sGygBXtU5UY_AOYC-B7DC5DOQ,1093
 nucliadb/writer/tests/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
 nucliadb/writer/tests/conftest.py,sha256=bmFKnuaqRqMCjtTp6c4V4R-qF59OPu0gW8-hp1TXFwk,1200
 nucliadb/writer/tests/fixtures.py,sha256=Ni66Iq-A6W8qqa6V6PwSzDq2BD9IINXlGexilVaDzPU,5971
 nucliadb/writer/tests/test_fields.py,sha256=fbzN0Bgu8HOLAqqYXO15JIqXN1bxr7mTTCTUuYhG85c,15472
 nucliadb/writer/tests/test_files.py,sha256=V-YB-ceSVCMmiVuXeH7BKl00GmC7t0ZyjUPAKqMr048,25999
 nucliadb/writer/tests/test_knowledgebox.py,sha256=KPUGr4TsmHXSTfte40rY18ANUHaUYs_TD4DXCIlawt8,1729
-nucliadb/writer/tests/test_reprocess_file_field.py,sha256=O37eL7RR4vLDFTjZ3UFh0att9PqimJM9sUt1yIPh7Ss,4358
-nucliadb/writer/tests/test_resources.py,sha256=gxCuJzCwcynos6ZDhaLZGRRZ2ZWuUGhL4heqECR4pLk,16694
+nucliadb/writer/tests/test_reprocess_file_field.py,sha256=MClPDagdcnpemIRpE_W7OeWTNRnYYK1xUm_BJOwRKdI,4400
+nucliadb/writer/tests/test_resources.py,sha256=Oqbby4QuiDZW1JLkIB68g6PK6gIt78KUjQnLdrySSGE,16857
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
-nucliadb-4.0.0.post539.dist-info/METADATA,sha256=nHAQsdm1L2Ib7mrKaUB9-2bJSImAtAHzGPZvIrkMnZE,4423
-nucliadb-4.0.0.post539.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-nucliadb-4.0.0.post539.dist-info/entry_points.txt,sha256=XqGfgFDuY3zXQc8ewXM2TRVjTModIq851zOsgrmaXx4,1268
-nucliadb-4.0.0.post539.dist-info/top_level.txt,sha256=hwYhTVnX7jkQ9gJCkVrbqEG1M4lT2F_iPQND1fCzF80,20
-nucliadb-4.0.0.post539.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-nucliadb-4.0.0.post539.dist-info/RECORD,,
+nucliadb-4.0.0.post540.dist-info/METADATA,sha256=3KWfIg1jgK7MVs1bvOYVS6hgGoKgXM5CNImi4awYQ9Y,4423
+nucliadb-4.0.0.post540.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+nucliadb-4.0.0.post540.dist-info/entry_points.txt,sha256=XqGfgFDuY3zXQc8ewXM2TRVjTModIq851zOsgrmaXx4,1268
+nucliadb-4.0.0.post540.dist-info/top_level.txt,sha256=hwYhTVnX7jkQ9gJCkVrbqEG1M4lT2F_iPQND1fCzF80,20
+nucliadb-4.0.0.post540.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
+nucliadb-4.0.0.post540.dist-info/RECORD,,
```


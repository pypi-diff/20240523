# Comparing `tmp/nucliadb-4.0.0.post538-py3-none-any.whl.zip` & `tmp/nucliadb-4.0.0.post539-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,464 +1,464 @@
-Zip file size: 765268 bytes, number of entries: 462
--rw-r--r--  2.0 unx     1135 b- defN 24-May-23 09:31 migrations/0001_bootstrap.py
--rw-r--r--  2.0 unx     1177 b- defN 24-May-23 09:31 migrations/0002_rollover_shards.py
--rw-r--r--  2.0 unx     2436 b- defN 24-May-23 09:31 migrations/0003_allfields_key.py
--rw-r--r--  2.0 unx     1177 b- defN 24-May-23 09:31 migrations/0004_rollover_shards.py
--rw-r--r--  2.0 unx     1177 b- defN 24-May-23 09:31 migrations/0005_rollover_shards.py
--rw-r--r--  2.0 unx     1024 b- defN 24-May-23 09:31 migrations/0006_rollover_shards.py
--rw-r--r--  2.0 unx     1301 b- defN 24-May-23 09:31 migrations/0008_cleanup_leftover_rollover_metadata.py
--rw-r--r--  2.0 unx     1378 b- defN 24-May-23 09:31 migrations/0009_upgrade_relations_and_texts_to_v2.py
--rw-r--r--  2.0 unx     1610 b- defN 24-May-23 09:31 migrations/0010_fix_corrupt_indexes.py
--rw-r--r--  2.0 unx     1843 b- defN 24-May-23 09:31 migrations/0011_materialize_labelset_ids.py
--rw-r--r--  2.0 unx     1443 b- defN 24-May-23 09:31 migrations/0012_rollover_shards.py
--rw-r--r--  2.0 unx     1024 b- defN 24-May-23 09:31 migrations/0013_rollover_shards.py
--rw-r--r--  2.0 unx     1382 b- defN 24-May-23 09:31 migrations/0014_rollover_shards.py
--rw-r--r--  2.0 unx     1462 b- defN 24-May-23 09:31 migrations/0015_targeted_rollover.py
--rw-r--r--  2.0 unx     2506 b- defN 24-May-23 09:31 migrations/0016_upgrade_to_paragraphs_v2.py
--rw-r--r--  2.0 unx     2100 b- defN 24-May-23 09:31 migrations/0017_multiple_writable_shards.py
--rw-r--r--  2.0 unx     2264 b- defN 24-May-23 09:31 migrations/0018_purge_orphan_kbslugs.py
--rw-r--r--  2.0 unx     2506 b- defN 24-May-23 09:31 migrations/0019_upgrade_to_paragraphs_v3.py
--rw-r--r--  2.0 unx     3282 b- defN 24-May-23 09:31 migrations/0020_drain_nodes_from_cluster.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-23 09:31 migrations/__init__.py
--rw-r--r--  2.0 unx      891 b- defN 24-May-23 09:31 nucliadb/__init__.py
--rw-r--r--  2.0 unx     3733 b- defN 24-May-23 09:31 nucliadb/health.py
--rw-r--r--  2.0 unx    11639 b- defN 24-May-23 09:31 nucliadb/learning_proxy.py
--rw-r--r--  2.0 unx     4806 b- defN 24-May-23 09:31 nucliadb/metrics_exporter.py
--rw-r--r--  2.0 unx     2272 b- defN 24-May-23 09:31 nucliadb/openapi.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-23 09:31 nucliadb/py.typed
--rw-r--r--  2.0 unx      835 b- defN 24-May-23 09:31 nucliadb/common/__init__.py
--rw-r--r--  2.0 unx     5175 b- defN 24-May-23 09:31 nucliadb/common/locking.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-23 09:31 nucliadb/common/cluster/__init__.py
--rw-r--r--  2.0 unx     5080 b- defN 24-May-23 09:31 nucliadb/common/cluster/base.py
--rw-r--r--  2.0 unx     1495 b- defN 24-May-23 09:31 nucliadb/common/cluster/exceptions.py
--rw-r--r--  2.0 unx     3793 b- defN 24-May-23 09:31 nucliadb/common/cluster/grpc_node_dummy.py
--rw-r--r--  2.0 unx     3429 b- defN 24-May-23 09:31 nucliadb/common/cluster/index_node.py
--rw-r--r--  2.0 unx    22091 b- defN 24-May-23 09:31 nucliadb/common/cluster/manager.py
--rw-r--r--  2.0 unx     8853 b- defN 24-May-23 09:31 nucliadb/common/cluster/rebalance.py
--rw-r--r--  2.0 unx    20209 b- defN 24-May-23 09:31 nucliadb/common/cluster/rollover.py
--rw-r--r--  2.0 unx     3016 b- defN 24-May-23 09:31 nucliadb/common/cluster/settings.py
--rw-r--r--  2.0 unx     5713 b- defN 24-May-23 09:31 nucliadb/common/cluster/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-23 09:31 nucliadb/common/cluster/discovery/__init__.py
--rw-r--r--  2.0 unx     6553 b- defN 24-May-23 09:31 nucliadb/common/cluster/discovery/base.py
--rw-r--r--  2.0 unx    12512 b- defN 24-May-23 09:31 nucliadb/common/cluster/discovery/k8s.py
--rw-r--r--  2.0 unx     1957 b- defN 24-May-23 09:31 nucliadb/common/cluster/discovery/manual.py
--rw-r--r--  2.0 unx     1737 b- defN 24-May-23 09:31 nucliadb/common/cluster/discovery/single.py
--rw-r--r--  2.0 unx     1139 b- defN 24-May-23 09:31 nucliadb/common/cluster/discovery/types.py
--rw-r--r--  2.0 unx     2548 b- defN 24-May-23 09:31 nucliadb/common/cluster/discovery/utils.py
--rw-r--r--  2.0 unx      833 b- defN 24-May-23 09:31 nucliadb/common/cluster/standalone/__init__.py
--rw-r--r--  2.0 unx    13712 b- defN 24-May-23 09:31 nucliadb/common/cluster/standalone/grpc_node_binding.py
--rw-r--r--  2.0 unx     4683 b- defN 24-May-23 09:31 nucliadb/common/cluster/standalone/index_node.py
--rw-r--r--  2.0 unx     3444 b- defN 24-May-23 09:31 nucliadb/common/cluster/standalone/service.py
--rw-r--r--  2.0 unx     3545 b- defN 24-May-23 09:31 nucliadb/common/cluster/standalone/utils.py
--rw-r--r--  2.0 unx     3440 b- defN 24-May-23 09:31 nucliadb/common/context/__init__.py
--rw-r--r--  2.0 unx     1628 b- defN 24-May-23 09:31 nucliadb/common/context/fastapi.py
--rw-r--r--  2.0 unx     1880 b- defN 24-May-23 09:31 nucliadb/common/datamanagers/__init__.py
--rw-r--r--  2.0 unx     1451 b- defN 24-May-23 09:31 nucliadb/common/datamanagers/cluster.py
--rw-r--r--  2.0 unx     5383 b- defN 24-May-23 09:31 nucliadb/common/datamanagers/entities.py
--rw-r--r--  2.0 unx      883 b- defN 24-May-23 09:31 nucliadb/common/datamanagers/exceptions.py
--rw-r--r--  2.0 unx     3994 b- defN 24-May-23 09:31 nucliadb/common/datamanagers/kb.py
--rw-r--r--  2.0 unx     5389 b- defN 24-May-23 09:31 nucliadb/common/datamanagers/labels.py
--rw-r--r--  2.0 unx     1599 b- defN 24-May-23 09:31 nucliadb/common/datamanagers/processing.py
--rw-r--r--  2.0 unx     8719 b- defN 24-May-23 09:31 nucliadb/common/datamanagers/resources.py
--rw-r--r--  2.0 unx     5634 b- defN 24-May-23 09:31 nucliadb/common/datamanagers/rollover.py
--rw-r--r--  2.0 unx     1548 b- defN 24-May-23 09:31 nucliadb/common/datamanagers/synonyms.py
--rw-r--r--  2.0 unx     1631 b- defN 24-May-23 09:31 nucliadb/common/datamanagers/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-23 09:31 nucliadb/common/http_clients/__init__.py
--rw-r--r--  2.0 unx     2146 b- defN 24-May-23 09:31 nucliadb/common/http_clients/auth.py
--rw-r--r--  2.0 unx     1100 b- defN 24-May-23 09:31 nucliadb/common/http_clients/exceptions.py
--rw-r--r--  2.0 unx     7155 b- defN 24-May-23 09:31 nucliadb/common/http_clients/processing.py
--rw-r--r--  2.0 unx     1540 b- defN 24-May-23 09:31 nucliadb/common/http_clients/pypi.py
--rw-r--r--  2.0 unx     1551 b- defN 24-May-23 09:31 nucliadb/common/http_clients/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-23 09:31 nucliadb/common/maindb/__init__.py
--rw-r--r--  2.0 unx     3449 b- defN 24-May-23 09:31 nucliadb/common/maindb/driver.py
--rw-r--r--  2.0 unx      946 b- defN 24-May-23 09:31 nucliadb/common/maindb/exceptions.py
--rw-r--r--  2.0 unx     6769 b- defN 24-May-23 09:31 nucliadb/common/maindb/local.py
--rw-r--r--  2.0 unx     8391 b- defN 24-May-23 09:31 nucliadb/common/maindb/pg.py
--rw-r--r--  2.0 unx     6053 b- defN 24-May-23 09:31 nucliadb/common/maindb/redis.py
--rw-r--r--  2.0 unx    14502 b- defN 24-May-23 09:31 nucliadb/common/maindb/tikv.py
--rw-r--r--  2.0 unx     4167 b- defN 24-May-23 09:31 nucliadb/common/maindb/utils.py
--rw-r--r--  2.0 unx      932 b- defN 24-May-23 09:31 nucliadb/export_import/__init__.py
--rw-r--r--  2.0 unx     6171 b- defN 24-May-23 09:31 nucliadb/export_import/datamanager.py
--rw-r--r--  2.0 unx     1949 b- defN 24-May-23 09:31 nucliadb/export_import/exceptions.py
--rw-r--r--  2.0 unx     7116 b- defN 24-May-23 09:31 nucliadb/export_import/exporter.py
--rw-r--r--  2.0 unx     4258 b- defN 24-May-23 09:31 nucliadb/export_import/importer.py
--rw-r--r--  2.0 unx     2063 b- defN 24-May-23 09:31 nucliadb/export_import/models.py
--rw-r--r--  2.0 unx     2571 b- defN 24-May-23 09:31 nucliadb/export_import/tasks.py
--rw-r--r--  2.0 unx    19401 b- defN 24-May-23 09:31 nucliadb/export_import/utils.py
--rw-r--r--  2.0 unx     1011 b- defN 24-May-23 09:31 nucliadb/ingest/__init__.py
--rw-r--r--  2.0 unx     7277 b- defN 24-May-23 09:31 nucliadb/ingest/app.py
--rw-r--r--  2.0 unx     1005 b- defN 24-May-23 09:31 nucliadb/ingest/cache.py
--rw-r--r--  2.0 unx     2484 b- defN 24-May-23 09:31 nucliadb/ingest/partitions.py
--rw-r--r--  2.0 unx    19904 b- defN 24-May-23 09:31 nucliadb/ingest/processing.py
--rw-r--r--  2.0 unx    20277 b- defN 24-May-23 09:31 nucliadb/ingest/serialize.py
--rw-r--r--  2.0 unx     3207 b- defN 24-May-23 09:31 nucliadb/ingest/settings.py
--rw-r--r--  2.0 unx     2314 b- defN 24-May-23 09:31 nucliadb/ingest/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-23 09:31 nucliadb/ingest/consumer/__init__.py
--rw-r--r--  2.0 unx     6918 b- defN 24-May-23 09:31 nucliadb/ingest/consumer/auditing.py
--rw-r--r--  2.0 unx    12174 b- defN 24-May-23 09:31 nucliadb/ingest/consumer/consumer.py
--rw-r--r--  2.0 unx     3945 b- defN 24-May-23 09:31 nucliadb/ingest/consumer/materializer.py
--rw-r--r--  2.0 unx     1075 b- defN 24-May-23 09:31 nucliadb/ingest/consumer/metrics.py
--rw-r--r--  2.0 unx     9543 b- defN 24-May-23 09:31 nucliadb/ingest/consumer/pull.py
--rw-r--r--  2.0 unx     6871 b- defN 24-May-23 09:31 nucliadb/ingest/consumer/service.py
--rw-r--r--  2.0 unx     4331 b- defN 24-May-23 09:31 nucliadb/ingest/consumer/shard_creator.py
--rw-r--r--  2.0 unx     2656 b- defN 24-May-23 09:31 nucliadb/ingest/consumer/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-23 09:31 nucliadb/ingest/fields/__init__.py
--rw-r--r--  2.0 unx    17461 b- defN 24-May-23 09:31 nucliadb/ingest/fields/base.py
--rw-r--r--  2.0 unx     6516 b- defN 24-May-23 09:31 nucliadb/ingest/fields/conversation.py
--rw-r--r--  2.0 unx     1223 b- defN 24-May-23 09:31 nucliadb/ingest/fields/date.py
--rw-r--r--  2.0 unx     1205 b- defN 24-May-23 09:31 nucliadb/ingest/fields/exceptions.py
--rw-r--r--  2.0 unx     4840 b- defN 24-May-23 09:31 nucliadb/ingest/fields/file.py
--rw-r--r--  2.0 unx     1547 b- defN 24-May-23 09:31 nucliadb/ingest/fields/generic.py
--rw-r--r--  2.0 unx     1235 b- defN 24-May-23 09:31 nucliadb/ingest/fields/keywordset.py
--rw-r--r--  2.0 unx     2250 b- defN 24-May-23 09:31 nucliadb/ingest/fields/layout.py
--rw-r--r--  2.0 unx     4212 b- defN 24-May-23 09:31 nucliadb/ingest/fields/link.py
--rw-r--r--  2.0 unx     1319 b- defN 24-May-23 09:31 nucliadb/ingest/fields/text.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-23 09:31 nucliadb/ingest/orm/__init__.py
--rw-r--r--  2.0 unx    28311 b- defN 24-May-23 09:31 nucliadb/ingest/orm/brain.py
--rw-r--r--  2.0 unx    15758 b- defN 24-May-23 09:31 nucliadb/ingest/orm/entities.py
--rw-r--r--  2.0 unx     1279 b- defN 24-May-23 09:31 nucliadb/ingest/orm/exceptions.py
--rw-r--r--  2.0 unx    16028 b- defN 24-May-23 09:31 nucliadb/ingest/orm/knowledgebox.py
--rw-r--r--  2.0 unx     1096 b- defN 24-May-23 09:31 nucliadb/ingest/orm/metrics.py
--rw-r--r--  2.0 unx    60311 b- defN 24-May-23 09:31 nucliadb/ingest/orm/resource.py
--rw-r--r--  2.0 unx     3683 b- defN 24-May-23 09:31 nucliadb/ingest/orm/utils.py
--rw-r--r--  2.0 unx    27042 b- defN 24-May-23 09:31 nucliadb/ingest/orm/processor/__init__.py
--rw-r--r--  2.0 unx     5090 b- defN 24-May-23 09:31 nucliadb/ingest/orm/processor/auditing.py
--rw-r--r--  2.0 unx     1690 b- defN 24-May-23 09:31 nucliadb/ingest/orm/processor/sequence_manager.py
--rw-r--r--  2.0 unx     2057 b- defN 24-May-23 09:31 nucliadb/ingest/service/__init__.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-23 09:31 nucliadb/ingest/service/exceptions.py
--rw-r--r--  2.0 unx    30462 b- defN 24-May-23 09:31 nucliadb/ingest/service/writer.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-23 09:31 nucliadb/ingest/tests/__init__.py
--rw-r--r--  2.0 unx     1157 b- defN 24-May-23 09:31 nucliadb/ingest/tests/conftest.py
--rw-r--r--  2.0 unx    24060 b- defN 24-May-23 09:31 nucliadb/ingest/tests/fixtures.py
--rw-r--r--  2.0 unx    62843 b- defN 24-May-23 09:31 nucliadb/ingest/tests/vectors.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-23 09:31 nucliadb/ingest/tests/integration/__init__.py
--rw-r--r--  2.0 unx      833 b- defN 24-May-23 09:31 nucliadb/ingest/tests/integration/consumer/__init__.py
--rw-r--r--  2.0 unx     2500 b- defN 24-May-23 09:31 nucliadb/ingest/tests/integration/consumer/test_auditing.py
--rw-r--r--  2.0 unx     3832 b- defN 24-May-23 09:31 nucliadb/ingest/tests/integration/consumer/test_materializer.py
--rw-r--r--  2.0 unx     4470 b- defN 24-May-23 09:31 nucliadb/ingest/tests/integration/consumer/test_pull.py
--rw-r--r--  2.0 unx     2763 b- defN 24-May-23 09:31 nucliadb/ingest/tests/integration/consumer/test_service.py
--rw-r--r--  2.0 unx     2019 b- defN 24-May-23 09:31 nucliadb/ingest/tests/integration/consumer/test_shard_creator.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-23 09:31 nucliadb/ingest/tests/integration/ingest/__init__.py
--rw-r--r--  2.0 unx    27247 b- defN 24-May-23 09:31 nucliadb/ingest/tests/integration/ingest/test_ingest.py
--rw-r--r--  2.0 unx     3040 b- defN 24-May-23 09:31 nucliadb/ingest/tests/integration/ingest/test_processing_engine.py
--rw-r--r--  2.0 unx     8586 b- defN 24-May-23 09:31 nucliadb/ingest/tests/integration/ingest/test_relations.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-23 09:31 nucliadb/ingest/tests/unit/__init__.py
--rw-r--r--  2.0 unx     1189 b- defN 24-May-23 09:31 nucliadb/ingest/tests/unit/test_cache.py
--rw-r--r--  2.0 unx     1432 b- defN 24-May-23 09:31 nucliadb/ingest/tests/unit/test_partitions.py
--rw-r--r--  2.0 unx     5807 b- defN 24-May-23 09:31 nucliadb/ingest/tests/unit/test_processing.py
--rw-r--r--  2.0 unx      978 b- defN 24-May-23 09:31 nucliadb/ingest/tests/unit/test_settings.py
--rw-r--r--  2.0 unx      833 b- defN 24-May-23 09:31 nucliadb/ingest/tests/unit/consumer/__init__.py
--rw-r--r--  2.0 unx     3885 b- defN 24-May-23 09:31 nucliadb/ingest/tests/unit/consumer/test_auditing.py
--rw-r--r--  2.0 unx     2472 b- defN 24-May-23 09:31 nucliadb/ingest/tests/unit/consumer/test_consumer.py
--rw-r--r--  2.0 unx     2063 b- defN 24-May-23 09:31 nucliadb/ingest/tests/unit/consumer/test_pull.py
--rw-r--r--  2.0 unx     4140 b- defN 24-May-23 09:31 nucliadb/ingest/tests/unit/consumer/test_shard_creator.py
--rw-r--r--  2.0 unx     1934 b- defN 24-May-23 09:31 nucliadb/ingest/tests/unit/consumer/test_utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-23 09:31 nucliadb/ingest/tests/unit/orm/__init__.py
--rw-r--r--  2.0 unx     9876 b- defN 24-May-23 09:31 nucliadb/ingest/tests/unit/orm/test_brain.py
--rw-r--r--  2.0 unx     2435 b- defN 24-May-23 09:31 nucliadb/ingest/tests/unit/orm/test_brain_vectors.py
--rw-r--r--  2.0 unx     1174 b- defN 24-May-23 09:31 nucliadb/ingest/tests/unit/orm/test_orm_utils.py
--rw-r--r--  2.0 unx     4045 b- defN 24-May-23 09:31 nucliadb/ingest/tests/unit/orm/test_processor.py
--rw-r--r--  2.0 unx    11033 b- defN 24-May-23 09:31 nucliadb/ingest/tests/unit/orm/test_resource.py
--rw-r--r--  2.0 unx     2216 b- defN 24-May-23 09:31 nucliadb/middleware/__init__.py
--rw-r--r--  2.0 unx     3912 b- defN 24-May-23 09:31 nucliadb/middleware/transaction.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-23 09:31 nucliadb/migrator/__init__.py
--rw-r--r--  2.0 unx     2119 b- defN 24-May-23 09:31 nucliadb/migrator/command.py
--rw-r--r--  2.0 unx     1334 b- defN 24-May-23 09:31 nucliadb/migrator/context.py
--rw-r--r--  2.0 unx     5104 b- defN 24-May-23 09:31 nucliadb/migrator/datamanager.py
--rw-r--r--  2.0 unx      889 b- defN 24-May-23 09:31 nucliadb/migrator/exceptions.py
--rw-r--r--  2.0 unx     9370 b- defN 24-May-23 09:31 nucliadb/migrator/migrator.py
--rw-r--r--  2.0 unx     1145 b- defN 24-May-23 09:31 nucliadb/migrator/models.py
--rw-r--r--  2.0 unx     1144 b- defN 24-May-23 09:31 nucliadb/migrator/settings.py
--rw-r--r--  2.0 unx     2346 b- defN 24-May-23 09:31 nucliadb/migrator/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-23 09:31 nucliadb/models/__init__.py
--rw-r--r--  2.0 unx     1599 b- defN 24-May-23 09:31 nucliadb/models/responses.py
--rw-r--r--  2.0 unx     6041 b- defN 24-May-23 09:31 nucliadb/purge/__init__.py
--rw-r--r--  2.0 unx     9364 b- defN 24-May-23 09:31 nucliadb/purge/orphan_shards.py
--rw-r--r--  2.0 unx     1328 b- defN 24-May-23 09:31 nucliadb/reader/__init__.py
--rw-r--r--  2.0 unx     3709 b- defN 24-May-23 09:31 nucliadb/reader/app.py
--rw-r--r--  2.0 unx     1366 b- defN 24-May-23 09:31 nucliadb/reader/lifecycle.py
--rw-r--r--  2.0 unx     1031 b- defN 24-May-23 09:31 nucliadb/reader/openapi.py
--rw-r--r--  2.0 unx     1447 b- defN 24-May-23 09:31 nucliadb/reader/run.py
--rw-r--r--  2.0 unx      872 b- defN 24-May-23 09:31 nucliadb/reader/api/__init__.py
--rw-r--r--  2.0 unx     2458 b- defN 24-May-23 09:31 nucliadb/reader/api/models.py
--rw-r--r--  2.0 unx     1110 b- defN 24-May-23 09:31 nucliadb/reader/api/v1/__init__.py
--rw-r--r--  2.0 unx    12392 b- defN 24-May-23 09:31 nucliadb/reader/api/v1/download.py
--rw-r--r--  2.0 unx     6459 b- defN 24-May-23 09:31 nucliadb/reader/api/v1/export_import.py
--rw-r--r--  2.0 unx     3641 b- defN 24-May-23 09:31 nucliadb/reader/api/v1/knowledgebox.py
--rw-r--r--  2.0 unx     2099 b- defN 24-May-23 09:31 nucliadb/reader/api/v1/learning_collector.py
--rw-r--r--  2.0 unx     4472 b- defN 24-May-23 09:31 nucliadb/reader/api/v1/learning_config.py
--rw-r--r--  2.0 unx    13951 b- defN 24-May-23 09:31 nucliadb/reader/api/v1/resource.py
--rw-r--r--  2.0 unx     1011 b- defN 24-May-23 09:31 nucliadb/reader/api/v1/router.py
--rw-r--r--  2.0 unx    12115 b- defN 24-May-23 09:31 nucliadb/reader/api/v1/services.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-23 09:31 nucliadb/reader/reader/__init__.py
--rw-r--r--  2.0 unx     7988 b- defN 24-May-23 09:31 nucliadb/reader/reader/notifications.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-23 09:31 nucliadb/reader/tests/__init__.py
--rw-r--r--  2.0 unx     1224 b- defN 24-May-23 09:31 nucliadb/reader/tests/conftest.py
--rw-r--r--  2.0 unx     4345 b- defN 24-May-23 09:31 nucliadb/reader/tests/fixtures.py
--rw-r--r--  2.0 unx     2748 b- defN 24-May-23 09:31 nucliadb/reader/tests/test_list_resources.py
--rw-r--r--  2.0 unx    10199 b- defN 24-May-23 09:31 nucliadb/reader/tests/test_reader_file_download.py
--rw-r--r--  2.0 unx    10586 b- defN 24-May-23 09:31 nucliadb/reader/tests/test_reader_resource.py
--rw-r--r--  2.0 unx     6535 b- defN 24-May-23 09:31 nucliadb/reader/tests/test_reader_resource_field.py
--rw-r--r--  2.0 unx     1535 b- defN 24-May-23 09:31 nucliadb/search/__init__.py
--rw-r--r--  2.0 unx     4905 b- defN 24-May-23 09:31 nucliadb/search/app.py
--rw-r--r--  2.0 unx     1956 b- defN 24-May-23 09:31 nucliadb/search/lifecycle.py
--rw-r--r--  2.0 unx     1016 b- defN 24-May-23 09:31 nucliadb/search/openapi.py
--rw-r--r--  2.0 unx    20665 b- defN 24-May-23 09:31 nucliadb/search/predict.py
--rw-r--r--  2.0 unx     1402 b- defN 24-May-23 09:31 nucliadb/search/run.py
--rw-r--r--  2.0 unx     1193 b- defN 24-May-23 09:31 nucliadb/search/settings.py
--rw-r--r--  2.0 unx     1037 b- defN 24-May-23 09:31 nucliadb/search/utilities.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-23 09:31 nucliadb/search/api/__init__.py
--rw-r--r--  2.0 unx     1298 b- defN 24-May-23 09:31 nucliadb/search/api/v1/__init__.py
--rw-r--r--  2.0 unx     3534 b- defN 24-May-23 09:31 nucliadb/search/api/v1/ask.py
--rw-r--r--  2.0 unx     9493 b- defN 24-May-23 09:31 nucliadb/search/api/v1/chat.py
--rw-r--r--  2.0 unx     2668 b- defN 24-May-23 09:31 nucliadb/search/api/v1/feedback.py
--rw-r--r--  2.0 unx     8795 b- defN 24-May-23 09:31 nucliadb/search/api/v1/find.py
--rw-r--r--  2.0 unx     6938 b- defN 24-May-23 09:31 nucliadb/search/api/v1/knowledgebox.py
--rw-r--r--  2.0 unx     3047 b- defN 24-May-23 09:31 nucliadb/search/api/v1/predict_proxy.py
--rw-r--r--  2.0 unx      988 b- defN 24-May-23 09:31 nucliadb/search/api/v1/router.py
--rw-r--r--  2.0 unx    19262 b- defN 24-May-23 09:31 nucliadb/search/api/v1/search.py
--rw-r--r--  2.0 unx     5970 b- defN 24-May-23 09:31 nucliadb/search/api/v1/suggest.py
--rw-r--r--  2.0 unx     2499 b- defN 24-May-23 09:31 nucliadb/search/api/v1/summarize.py
--rw-r--r--  2.0 unx     1434 b- defN 24-May-23 09:31 nucliadb/search/api/v1/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-23 09:31 nucliadb/search/api/v1/resource/__init__.py
--rw-r--r--  2.0 unx     4064 b- defN 24-May-23 09:31 nucliadb/search/api/v1/resource/ask.py
--rw-r--r--  2.0 unx     5821 b- defN 24-May-23 09:31 nucliadb/search/api/v1/resource/chat.py
--rw-r--r--  2.0 unx     5303 b- defN 24-May-23 09:31 nucliadb/search/api/v1/resource/search.py
--rw-r--r--  2.0 unx      833 b- defN 24-May-23 09:31 nucliadb/search/requesters/__init__.py
--rw-r--r--  2.0 unx     9111 b- defN 24-May-23 09:31 nucliadb/search/requesters/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-23 09:31 nucliadb/search/search/__init__.py
--rw-r--r--  2.0 unx     2746 b- defN 24-May-23 09:31 nucliadb/search/search/cache.py
--rw-r--r--  2.0 unx     1154 b- defN 24-May-23 09:31 nucliadb/search/search/exceptions.py
--rw-r--r--  2.0 unx     5465 b- defN 24-May-23 09:31 nucliadb/search/search/fetch.py
--rw-r--r--  2.0 unx     6513 b- defN 24-May-23 09:31 nucliadb/search/search/filters.py
--rw-r--r--  2.0 unx     4612 b- defN 24-May-23 09:31 nucliadb/search/search/find.py
--rw-r--r--  2.0 unx    17152 b- defN 24-May-23 09:31 nucliadb/search/search/find_merge.py
--rw-r--r--  2.0 unx    21282 b- defN 24-May-23 09:31 nucliadb/search/search/merge.py
--rw-r--r--  2.0 unx     1130 b- defN 24-May-23 09:31 nucliadb/search/search/metrics.py
--rw-r--r--  2.0 unx     8698 b- defN 24-May-23 09:31 nucliadb/search/search/paragraphs.py
--rw-r--r--  2.0 unx     3026 b- defN 24-May-23 09:31 nucliadb/search/search/predict_proxy.py
--rw-r--r--  2.0 unx    31093 b- defN 24-May-23 09:31 nucliadb/search/search/query.py
--rw-r--r--  2.0 unx     3018 b- defN 24-May-23 09:31 nucliadb/search/search/shards.py
--rw-r--r--  2.0 unx     5101 b- defN 24-May-23 09:31 nucliadb/search/search/summarize.py
--rw-r--r--  2.0 unx     2438 b- defN 24-May-23 09:31 nucliadb/search/search/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-23 09:31 nucliadb/search/search/chat/__init__.py
--rw-r--r--  2.0 unx    16676 b- defN 24-May-23 09:31 nucliadb/search/search/chat/ask.py
--rw-r--r--  2.0 unx     2058 b- defN 24-May-23 09:31 nucliadb/search/search/chat/images.py
--rw-r--r--  2.0 unx    20793 b- defN 24-May-23 09:31 nucliadb/search/search/chat/prompt.py
--rw-r--r--  2.0 unx    17543 b- defN 24-May-23 09:31 nucliadb/search/search/chat/query.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-23 09:31 nucliadb/search/tests/__init__.py
--rw-r--r--  2.0 unx     1295 b- defN 24-May-23 09:31 nucliadb/search/tests/conftest.py
--rw-r--r--  2.0 unx     6578 b- defN 24-May-23 09:31 nucliadb/search/tests/fixtures.py
--rw-r--r--  2.0 unx    15480 b- defN 24-May-23 09:31 nucliadb/search/tests/node.py
--rw-r--r--  2.0 unx      833 b- defN 24-May-23 09:31 nucliadb/search/tests/unit/__init__.py
--rw-r--r--  2.0 unx     2649 b- defN 24-May-23 09:31 nucliadb/search/tests/unit/test_app.py
--rw-r--r--  2.0 unx     3374 b- defN 24-May-23 09:31 nucliadb/search/tests/unit/test_find_merge.py
--rw-r--r--  2.0 unx     1400 b- defN 24-May-23 09:31 nucliadb/search/tests/unit/test_merge.py
--rw-r--r--  2.0 unx    15721 b- defN 24-May-23 09:31 nucliadb/search/tests/unit/test_predict.py
--rw-r--r--  2.0 unx     1328 b- defN 24-May-23 09:31 nucliadb/search/tests/unit/test_run.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-23 09:31 nucliadb/search/tests/unit/api/__init__.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-23 09:31 nucliadb/search/tests/unit/api/v1/__init__.py
--rw-r--r--  2.0 unx     3759 b- defN 24-May-23 09:31 nucliadb/search/tests/unit/api/v1/test_ask.py
--rw-r--r--  2.0 unx     2966 b- defN 24-May-23 09:31 nucliadb/search/tests/unit/api/v1/test_chat.py
--rw-r--r--  2.0 unx     2865 b- defN 24-May-23 09:31 nucliadb/search/tests/unit/api/v1/test_predict_proxy.py
--rw-r--r--  2.0 unx     2901 b- defN 24-May-23 09:31 nucliadb/search/tests/unit/api/v1/test_summarize.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-23 09:31 nucliadb/search/tests/unit/api/v1/resource/__init__.py
--rw-r--r--  2.0 unx     3040 b- defN 24-May-23 09:31 nucliadb/search/tests/unit/api/v1/resource/test_chat.py
--rw-r--r--  2.0 unx      833 b- defN 24-May-23 09:31 nucliadb/search/tests/unit/search/__init__.py
--rw-r--r--  2.0 unx     8586 b- defN 24-May-23 09:31 nucliadb/search/tests/unit/search/test_chat_prompt.py
--rw-r--r--  2.0 unx     3736 b- defN 24-May-23 09:31 nucliadb/search/tests/unit/search/test_fetch.py
--rw-r--r--  2.0 unx     4306 b- defN 24-May-23 09:31 nucliadb/search/tests/unit/search/test_filters.py
--rw-r--r--  2.0 unx     4492 b- defN 24-May-23 09:31 nucliadb/search/tests/unit/search/test_paragraphs.py
--rw-r--r--  2.0 unx     3496 b- defN 24-May-23 09:31 nucliadb/search/tests/unit/search/test_predict_proxy.py
--rw-r--r--  2.0 unx     5121 b- defN 24-May-23 09:31 nucliadb/search/tests/unit/search/test_query.py
--rw-r--r--  2.0 unx      833 b- defN 24-May-23 09:31 nucliadb/search/tests/unit/search/requesters/__init__.py
--rw-r--r--  2.0 unx     6455 b- defN 24-May-23 09:31 nucliadb/search/tests/unit/search/requesters/test_utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-23 09:31 nucliadb/search/tests/unit/search/search/__init__.py
--rw-r--r--  2.0 unx     1759 b- defN 24-May-23 09:31 nucliadb/search/tests/unit/search/search/test_shards.py
--rw-r--r--  2.0 unx     2511 b- defN 24-May-23 09:31 nucliadb/search/tests/unit/search/search/test_utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-23 09:31 nucliadb/standalone/__init__.py
--rw-r--r--  2.0 unx     6746 b- defN 24-May-23 09:31 nucliadb/standalone/api_router.py
--rw-r--r--  2.0 unx     5763 b- defN 24-May-23 09:31 nucliadb/standalone/app.py
--rw-r--r--  2.0 unx     7800 b- defN 24-May-23 09:31 nucliadb/standalone/auth.py
--rw-r--r--  2.0 unx     5313 b- defN 24-May-23 09:31 nucliadb/standalone/config.py
--rw-r--r--  2.0 unx     6986 b- defN 24-May-23 09:31 nucliadb/standalone/introspect.py
--rw-r--r--  2.0 unx     2488 b- defN 24-May-23 09:31 nucliadb/standalone/lifecycle.py
--rw-r--r--  2.0 unx     1980 b- defN 24-May-23 09:31 nucliadb/standalone/migrations.py
--rw-r--r--  2.0 unx     1322 b- defN 24-May-23 09:31 nucliadb/standalone/purge.py
--rw-r--r--  2.0 unx     5636 b- defN 24-May-23 09:31 nucliadb/standalone/run.py
--rw-r--r--  2.0 unx     5822 b- defN 24-May-23 09:31 nucliadb/standalone/settings.py
--rw-r--r--  2.0 unx     3132 b- defN 24-May-23 09:31 nucliadb/standalone/versions.py
--rw-r--r--  2.0 unx     2285 b- defN 24-May-23 09:31 nucliadb/standalone/static/favicon.ico
--rw-r--r--  2.0 unx     3833 b- defN 24-May-23 09:31 nucliadb/standalone/static/index.html
--rw-r--r--  2.0 unx     2639 b- defN 24-May-23 09:31 nucliadb/standalone/static/logo.svg
--rw-r--r--  2.0 unx      835 b- defN 24-May-23 09:31 nucliadb/standalone/tests/__init__.py
--rw-r--r--  2.0 unx     1294 b- defN 24-May-23 09:31 nucliadb/standalone/tests/conftest.py
--rw-r--r--  2.0 unx     1319 b- defN 24-May-23 09:31 nucliadb/standalone/tests/fixtures.py
--rw-r--r--  2.0 unx      833 b- defN 24-May-23 09:31 nucliadb/standalone/tests/unit/__init__.py
--rw-r--r--  2.0 unx     1722 b- defN 24-May-23 09:31 nucliadb/standalone/tests/unit/test_api_router.py
--rw-r--r--  2.0 unx     5509 b- defN 24-May-23 09:31 nucliadb/standalone/tests/unit/test_auth.py
--rw-r--r--  2.0 unx     1334 b- defN 24-May-23 09:31 nucliadb/standalone/tests/unit/test_introspect.py
--rw-r--r--  2.0 unx     1863 b- defN 24-May-23 09:31 nucliadb/standalone/tests/unit/test_migrations.py
--rw-r--r--  2.0 unx     1546 b- defN 24-May-23 09:31 nucliadb/standalone/tests/unit/test_run.py
--rw-r--r--  2.0 unx     1972 b- defN 24-May-23 09:31 nucliadb/standalone/tests/unit/test_versions.py
--rw-r--r--  2.0 unx     1037 b- defN 24-May-23 09:31 nucliadb/tasks/__init__.py
--rw-r--r--  2.0 unx     7655 b- defN 24-May-23 09:31 nucliadb/tasks/consumer.py
--rw-r--r--  2.0 unx      924 b- defN 24-May-23 09:31 nucliadb/tasks/logger.py
--rw-r--r--  2.0 unx     1378 b- defN 24-May-23 09:31 nucliadb/tasks/models.py
--rw-r--r--  2.0 unx     3457 b- defN 24-May-23 09:31 nucliadb/tasks/producer.py
--rw-r--r--  2.0 unx     1753 b- defN 24-May-23 09:31 nucliadb/tasks/registry.py
--rw-r--r--  2.0 unx     1360 b- defN 24-May-23 09:31 nucliadb/tasks/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-23 09:31 nucliadb/tests/__init__.py
--rw-r--r--  2.0 unx     1229 b- defN 24-May-23 09:31 nucliadb/tests/conftest.py
--rw-r--r--  2.0 unx    22365 b- defN 24-May-23 09:31 nucliadb/tests/fixtures.py
--rw-r--r--  2.0 unx     7549 b- defN 24-May-23 09:31 nucliadb/tests/tikv.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-23 09:31 nucliadb/tests/benchmarks/__init__.py
--rw-r--r--  2.0 unx     3032 b- defN 24-May-23 09:31 nucliadb/tests/benchmarks/test_search.py
--rw-r--r--  2.0 unx      919 b- defN 24-May-23 09:31 nucliadb/tests/knowledgeboxes/__init__.py
--rw-r--r--  2.0 unx     7002 b- defN 24-May-23 09:31 nucliadb/tests/knowledgeboxes/philosophy_books.py
--rw-r--r--  2.0 unx     3037 b- defN 24-May-23 09:31 nucliadb/tests/knowledgeboxes/ten_dummy_resources.py
--rw-r--r--  2.0 unx     1148 b- defN 24-May-23 09:31 nucliadb/tests/migrations/__init__.py
--rw-r--r--  2.0 unx     2726 b- defN 24-May-23 09:31 nucliadb/tests/migrations/test_migration_0017.py
--rw-r--r--  2.0 unx     3662 b- defN 24-May-23 09:31 nucliadb/tests/migrations/test_migration_0018.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-23 09:31 nucliadb/tests/unit/__init__.py
--rw-r--r--  2.0 unx     1487 b- defN 24-May-23 09:31 nucliadb/tests/unit/test_field_ids.py
--rw-r--r--  2.0 unx     2780 b- defN 24-May-23 09:31 nucliadb/tests/unit/test_health.py
--rw-r--r--  2.0 unx     1543 b- defN 24-May-23 09:31 nucliadb/tests/unit/test_kb_slugs.py
--rw-r--r--  2.0 unx     7892 b- defN 24-May-23 09:31 nucliadb/tests/unit/test_learning_proxy.py
--rw-r--r--  2.0 unx     2642 b- defN 24-May-23 09:31 nucliadb/tests/unit/test_metrics_exporter.py
--rw-r--r--  2.0 unx     1341 b- defN 24-May-23 09:31 nucliadb/tests/unit/test_openapi.py
--rw-r--r--  2.0 unx     3649 b- defN 24-May-23 09:31 nucliadb/tests/unit/test_purge.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-23 09:31 nucliadb/tests/unit/common/__init__.py
--rw-r--r--  2.0 unx     1268 b- defN 24-May-23 09:31 nucliadb/tests/unit/common/test_context.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-23 09:31 nucliadb/tests/unit/common/cluster/__init__.py
--rw-r--r--  2.0 unx    12240 b- defN 24-May-23 09:31 nucliadb/tests/unit/common/cluster/test_cluster.py
--rw-r--r--  2.0 unx     5387 b- defN 24-May-23 09:31 nucliadb/tests/unit/common/cluster/test_kb_shard_manager.py
--rw-r--r--  2.0 unx     1428 b- defN 24-May-23 09:31 nucliadb/tests/unit/common/cluster/test_rebalance.py
--rw-r--r--  2.0 unx     9465 b- defN 24-May-23 09:31 nucliadb/tests/unit/common/cluster/test_rollover.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-23 09:31 nucliadb/tests/unit/common/cluster/discovery/__init__.py
--rw-r--r--  2.0 unx     5627 b- defN 24-May-23 09:31 nucliadb/tests/unit/common/cluster/discovery/test_k8s.py
--rw-r--r--  2.0 unx      833 b- defN 24-May-23 09:31 nucliadb/tests/unit/common/cluster/standalone/__init__.py
--rw-r--r--  2.0 unx     3761 b- defN 24-May-23 09:31 nucliadb/tests/unit/common/cluster/standalone/test_service.py
--rw-r--r--  2.0 unx     2136 b- defN 24-May-23 09:31 nucliadb/tests/unit/common/cluster/standalone/test_utils.py
--rw-r--r--  2.0 unx      833 b- defN 24-May-23 09:31 nucliadb/tests/unit/common/maindb/__init__.py
--rw-r--r--  2.0 unx     3579 b- defN 24-May-23 09:31 nucliadb/tests/unit/common/maindb/test_driver.py
--rw-r--r--  2.0 unx     1869 b- defN 24-May-23 09:31 nucliadb/tests/unit/common/maindb/test_tikv.py
--rw-r--r--  2.0 unx     3213 b- defN 24-May-23 09:31 nucliadb/tests/unit/common/maindb/test_utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-23 09:31 nucliadb/tests/unit/export_import/__init__.py
--rw-r--r--  2.0 unx     1435 b- defN 24-May-23 09:31 nucliadb/tests/unit/export_import/test_datamanager.py
--rw-r--r--  2.0 unx     9706 b- defN 24-May-23 09:31 nucliadb/tests/unit/export_import/test_utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-23 09:31 nucliadb/tests/unit/migrator/__init__.py
--rw-r--r--  2.0 unx     3233 b- defN 24-May-23 09:31 nucliadb/tests/unit/migrator/test_migrator.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-23 09:31 nucliadb/tests/unit/tasks/__init__.py
--rw-r--r--  2.0 unx     1375 b- defN 24-May-23 09:31 nucliadb/tests/unit/tasks/conftest.py
--rw-r--r--  2.0 unx     2714 b- defN 24-May-23 09:31 nucliadb/tests/unit/tasks/test_consumer.py
--rw-r--r--  2.0 unx     3189 b- defN 24-May-23 09:31 nucliadb/tests/unit/tasks/test_producer.py
--rw-r--r--  2.0 unx     1827 b- defN 24-May-23 09:31 nucliadb/tests/unit/tasks/test_tasks.py
--rw-r--r--  2.0 unx     2507 b- defN 24-May-23 09:31 nucliadb/tests/utils/__init__.py
--rw-r--r--  2.0 unx     1797 b- defN 24-May-23 09:31 nucliadb/tests/utils/aiohttp_session.py
--rw-r--r--  2.0 unx     2533 b- defN 24-May-23 09:31 nucliadb/tests/utils/entities.py
--rw-r--r--  2.0 unx     6327 b- defN 24-May-23 09:31 nucliadb/tests/utils/broker_messages/__init__.py
--rw-r--r--  2.0 unx     7557 b- defN 24-May-23 09:31 nucliadb/tests/utils/broker_messages/fields.py
--rw-r--r--  2.0 unx     1196 b- defN 24-May-23 09:31 nucliadb/tests/utils/broker_messages/helpers.py
--rw-r--r--  2.0 unx     1325 b- defN 24-May-23 09:31 nucliadb/train/__init__.py
--rw-r--r--  2.0 unx     3530 b- defN 24-May-23 09:31 nucliadb/train/app.py
--rw-r--r--  2.0 unx     3800 b- defN 24-May-23 09:31 nucliadb/train/generator.py
--rw-r--r--  2.0 unx     1698 b- defN 24-May-23 09:31 nucliadb/train/lifecycle.py
--rw-r--r--  2.0 unx     1198 b- defN 24-May-23 09:31 nucliadb/train/models.py
--rw-r--r--  2.0 unx     5706 b- defN 24-May-23 09:31 nucliadb/train/nodes.py
--rw-r--r--  2.0 unx     1400 b- defN 24-May-23 09:31 nucliadb/train/run.py
--rw-r--r--  2.0 unx     5926 b- defN 24-May-23 09:31 nucliadb/train/servicer.py
--rw-r--r--  2.0 unx     1415 b- defN 24-May-23 09:31 nucliadb/train/settings.py
--rw-r--r--  2.0 unx     1496 b- defN 24-May-23 09:31 nucliadb/train/types.py
--rw-r--r--  2.0 unx     3265 b- defN 24-May-23 09:31 nucliadb/train/upload.py
--rw-r--r--  2.0 unx     6420 b- defN 24-May-23 09:31 nucliadb/train/uploader.py
--rw-r--r--  2.0 unx     3179 b- defN 24-May-23 09:31 nucliadb/train/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-23 09:31 nucliadb/train/api/__init__.py
--rw-r--r--  2.0 unx     1479 b- defN 24-May-23 09:31 nucliadb/train/api/utils.py
--rw-r--r--  2.0 unx      928 b- defN 24-May-23 09:31 nucliadb/train/api/v1/__init__.py
--rw-r--r--  2.0 unx     2071 b- defN 24-May-23 09:31 nucliadb/train/api/v1/check.py
--rw-r--r--  2.0 unx      910 b- defN 24-May-23 09:31 nucliadb/train/api/v1/router.py
--rw-r--r--  2.0 unx     1908 b- defN 24-May-23 09:31 nucliadb/train/api/v1/shards.py
--rw-r--r--  2.0 unx     2135 b- defN 24-May-23 09:31 nucliadb/train/api/v1/trainset.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-23 09:31 nucliadb/train/generators/__init__.py
--rw-r--r--  2.0 unx     3723 b- defN 24-May-23 09:31 nucliadb/train/generators/field_classifier.py
--rw-r--r--  2.0 unx     6712 b- defN 24-May-23 09:31 nucliadb/train/generators/image_classifier.py
--rw-r--r--  2.0 unx     2789 b- defN 24-May-23 09:31 nucliadb/train/generators/paragraph_classifier.py
--rw-r--r--  2.0 unx     3590 b- defN 24-May-23 09:31 nucliadb/train/generators/paragraph_streaming.py
--rw-r--r--  2.0 unx     5372 b- defN 24-May-23 09:31 nucliadb/train/generators/question_answer_streaming.py
--rw-r--r--  2.0 unx     5160 b- defN 24-May-23 09:31 nucliadb/train/generators/sentence_classifier.py
--rw-r--r--  2.0 unx    10446 b- defN 24-May-23 09:31 nucliadb/train/generators/token_classifier.py
--rw-r--r--  2.0 unx     3877 b- defN 24-May-23 09:31 nucliadb/train/generators/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-23 09:31 nucliadb/train/tests/__init__.py
--rw-r--r--  2.0 unx     1125 b- defN 24-May-23 09:31 nucliadb/train/tests/conftest.py
--rw-r--r--  2.0 unx    11053 b- defN 24-May-23 09:31 nucliadb/train/tests/fixtures.py
--rw-r--r--  2.0 unx     4598 b- defN 24-May-23 09:31 nucliadb/train/tests/test_field_classification.py
--rw-r--r--  2.0 unx     2729 b- defN 24-May-23 09:31 nucliadb/train/tests/test_get_entities.py
--rw-r--r--  2.0 unx     1876 b- defN 24-May-23 09:31 nucliadb/train/tests/test_get_info.py
--rw-r--r--  2.0 unx     1382 b- defN 24-May-23 09:31 nucliadb/train/tests/test_get_ontology.py
--rw-r--r--  2.0 unx     2417 b- defN 24-May-23 09:31 nucliadb/train/tests/test_get_ontology_count.py
--rw-r--r--  2.0 unx     7669 b- defN 24-May-23 09:31 nucliadb/train/tests/test_image_classification.py
--rw-r--r--  2.0 unx     1416 b- defN 24-May-23 09:31 nucliadb/train/tests/test_list_fields.py
--rw-r--r--  2.0 unx     2944 b- defN 24-May-23 09:31 nucliadb/train/tests/test_list_paragraphs.py
--rw-r--r--  2.0 unx     1423 b- defN 24-May-23 09:31 nucliadb/train/tests/test_list_resources.py
--rw-r--r--  2.0 unx     2947 b- defN 24-May-23 09:31 nucliadb/train/tests/test_list_sentences.py
--rw-r--r--  2.0 unx     4645 b- defN 24-May-23 09:31 nucliadb/train/tests/test_paragraph_classification.py
--rw-r--r--  2.0 unx     4320 b- defN 24-May-23 09:31 nucliadb/train/tests/test_paragraph_streaming.py
--rw-r--r--  2.0 unx     8751 b- defN 24-May-23 09:31 nucliadb/train/tests/test_question_answer_streaming.py
--rw-r--r--  2.0 unx     5051 b- defN 24-May-23 09:31 nucliadb/train/tests/test_sentence_classification.py
--rw-r--r--  2.0 unx     5583 b- defN 24-May-23 09:31 nucliadb/train/tests/test_token_classification.py
--rw-r--r--  2.0 unx     3324 b- defN 24-May-23 09:31 nucliadb/train/tests/utils.py
--rw-r--r--  2.0 unx     1328 b- defN 24-May-23 09:31 nucliadb/writer/__init__.py
--rw-r--r--  2.0 unx     4268 b- defN 24-May-23 09:31 nucliadb/writer/app.py
--rw-r--r--  2.0 unx    19483 b- defN 24-May-23 09:31 nucliadb/writer/back_pressure.py
--rw-r--r--  2.0 unx      972 b- defN 24-May-23 09:31 nucliadb/writer/exceptions.py
--rw-r--r--  2.0 unx     1953 b- defN 24-May-23 09:31 nucliadb/writer/lifecycle.py
--rw-r--r--  2.0 unx     1032 b- defN 24-May-23 09:31 nucliadb/writer/openapi.py
--rw-r--r--  2.0 unx     1448 b- defN 24-May-23 09:31 nucliadb/writer/run.py
--rw-r--r--  2.0 unx     3103 b- defN 24-May-23 09:31 nucliadb/writer/settings.py
--rw-r--r--  2.0 unx     1036 b- defN 24-May-23 09:31 nucliadb/writer/utilities.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-23 09:31 nucliadb/writer/api/__init__.py
--rw-r--r--  2.0 unx     1429 b- defN 24-May-23 09:31 nucliadb/writer/api/constants.py
--rw-r--r--  2.0 unx     1095 b- defN 24-May-23 09:31 nucliadb/writer/api/v1/__init__.py
--rw-r--r--  2.0 unx     6571 b- defN 24-May-23 09:31 nucliadb/writer/api/v1/export_import.py
--rw-r--r--  2.0 unx    24482 b- defN 24-May-23 09:31 nucliadb/writer/api/v1/field.py
--rw-r--r--  2.0 unx     5248 b- defN 24-May-23 09:31 nucliadb/writer/api/v1/knowledgebox.py
--rw-r--r--  2.0 unx     2058 b- defN 24-May-23 09:31 nucliadb/writer/api/v1/learning_config.py
--rw-r--r--  2.0 unx    18893 b- defN 24-May-23 09:31 nucliadb/writer/api/v1/resource.py
--rw-r--r--  2.0 unx     1034 b- defN 24-May-23 09:31 nucliadb/writer/api/v1/router.py
--rw-r--r--  2.0 unx    10216 b- defN 24-May-23 09:31 nucliadb/writer/api/v1/services.py
--rw-r--r--  2.0 unx    30857 b- defN 24-May-23 09:31 nucliadb/writer/api/v1/upload.py
--rw-r--r--  2.0 unx     1612 b- defN 24-May-23 09:31 nucliadb/writer/layouts/__init__.py
--rw-r--r--  2.0 unx     2115 b- defN 24-May-23 09:31 nucliadb/writer/layouts/v1.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-23 09:31 nucliadb/writer/resource/__init__.py
--rw-r--r--  2.0 unx     1425 b- defN 24-May-23 09:31 nucliadb/writer/resource/audit.py
--rw-r--r--  2.0 unx    10968 b- defN 24-May-23 09:31 nucliadb/writer/resource/basic.py
--rw-r--r--  2.0 unx    16740 b- defN 24-May-23 09:31 nucliadb/writer/resource/field.py
--rw-r--r--  2.0 unx     2022 b- defN 24-May-23 09:31 nucliadb/writer/resource/origin.py
--rw-r--r--  2.0 unx     1152 b- defN 24-May-23 09:31 nucliadb/writer/resource/slug.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-23 09:31 nucliadb/writer/tests/__init__.py
--rw-r--r--  2.0 unx     1200 b- defN 24-May-23 09:31 nucliadb/writer/tests/conftest.py
--rw-r--r--  2.0 unx     5971 b- defN 24-May-23 09:31 nucliadb/writer/tests/fixtures.py
--rw-r--r--  2.0 unx    15472 b- defN 24-May-23 09:31 nucliadb/writer/tests/test_fields.py
--rw-r--r--  2.0 unx    25999 b- defN 24-May-23 09:31 nucliadb/writer/tests/test_files.py
--rw-r--r--  2.0 unx     1729 b- defN 24-May-23 09:31 nucliadb/writer/tests/test_knowledgebox.py
--rw-r--r--  2.0 unx     4358 b- defN 24-May-23 09:31 nucliadb/writer/tests/test_reprocess_file_field.py
--rw-r--r--  2.0 unx    16694 b- defN 24-May-23 09:31 nucliadb/writer/tests/test_resources.py
--rw-r--r--  2.0 unx     5120 b- defN 24-May-23 09:31 nucliadb/writer/tests/test_service.py
--rw-r--r--  2.0 unx     6054 b- defN 24-May-23 09:31 nucliadb/writer/tests/test_tus.py
--rw-r--r--  2.0 unx     1287 b- defN 24-May-23 09:31 nucliadb/writer/tests/utils.py
--rw-r--r--  2.0 unx     5226 b- defN 24-May-23 09:31 nucliadb/writer/tus/__init__.py
--rw-r--r--  2.0 unx     5082 b- defN 24-May-23 09:31 nucliadb/writer/tus/dm.py
--rw-r--r--  2.0 unx     2186 b- defN 24-May-23 09:31 nucliadb/writer/tus/exceptions.py
--rw-r--r--  2.0 unx    14527 b- defN 24-May-23 09:31 nucliadb/writer/tus/gcs.py
--rw-r--r--  2.0 unx     5849 b- defN 24-May-23 09:31 nucliadb/writer/tus/local.py
--rw-r--r--  2.0 unx     4367 b- defN 24-May-23 09:31 nucliadb/writer/tus/pg.py
--rw-r--r--  2.0 unx     9069 b- defN 24-May-23 09:31 nucliadb/writer/tus/s3.py
--rw-r--r--  2.0 unx     4734 b- defN 24-May-23 09:31 nucliadb/writer/tus/storage.py
--rw-r--r--  2.0 unx     2556 b- defN 24-May-23 09:31 nucliadb/writer/tus/utils.py
--rw-r--r--  2.0 unx     4423 b- defN 24-May-23 09:32 nucliadb-4.0.0.post538.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-23 09:32 nucliadb-4.0.0.post538.dist-info/WHEEL
--rw-r--r--  2.0 unx     1268 b- defN 24-May-23 09:32 nucliadb-4.0.0.post538.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       20 b- defN 24-May-23 09:32 nucliadb-4.0.0.post538.dist-info/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 24-May-23 09:32 nucliadb-4.0.0.post538.dist-info/zip-safe
--rw-rw-r--  2.0 unx    43359 b- defN 24-May-23 09:32 nucliadb-4.0.0.post538.dist-info/RECORD
-462 files, 2259206 bytes uncompressed, 695922 bytes compressed:  69.2%
+Zip file size: 765220 bytes, number of entries: 462
+-rw-r--r--  2.0 unx     1135 b- defN 24-May-23 10:56 migrations/0001_bootstrap.py
+-rw-r--r--  2.0 unx     1177 b- defN 24-May-23 10:56 migrations/0002_rollover_shards.py
+-rw-r--r--  2.0 unx     2436 b- defN 24-May-23 10:56 migrations/0003_allfields_key.py
+-rw-r--r--  2.0 unx     1177 b- defN 24-May-23 10:56 migrations/0004_rollover_shards.py
+-rw-r--r--  2.0 unx     1177 b- defN 24-May-23 10:56 migrations/0005_rollover_shards.py
+-rw-r--r--  2.0 unx     1024 b- defN 24-May-23 10:56 migrations/0006_rollover_shards.py
+-rw-r--r--  2.0 unx     1301 b- defN 24-May-23 10:56 migrations/0008_cleanup_leftover_rollover_metadata.py
+-rw-r--r--  2.0 unx     1378 b- defN 24-May-23 10:56 migrations/0009_upgrade_relations_and_texts_to_v2.py
+-rw-r--r--  2.0 unx     1610 b- defN 24-May-23 10:56 migrations/0010_fix_corrupt_indexes.py
+-rw-r--r--  2.0 unx     1843 b- defN 24-May-23 10:56 migrations/0011_materialize_labelset_ids.py
+-rw-r--r--  2.0 unx     1443 b- defN 24-May-23 10:56 migrations/0012_rollover_shards.py
+-rw-r--r--  2.0 unx     1024 b- defN 24-May-23 10:56 migrations/0013_rollover_shards.py
+-rw-r--r--  2.0 unx     1382 b- defN 24-May-23 10:56 migrations/0014_rollover_shards.py
+-rw-r--r--  2.0 unx     1462 b- defN 24-May-23 10:56 migrations/0015_targeted_rollover.py
+-rw-r--r--  2.0 unx     2506 b- defN 24-May-23 10:56 migrations/0016_upgrade_to_paragraphs_v2.py
+-rw-r--r--  2.0 unx     2100 b- defN 24-May-23 10:56 migrations/0017_multiple_writable_shards.py
+-rw-r--r--  2.0 unx     2264 b- defN 24-May-23 10:56 migrations/0018_purge_orphan_kbslugs.py
+-rw-r--r--  2.0 unx     2506 b- defN 24-May-23 10:56 migrations/0019_upgrade_to_paragraphs_v3.py
+-rw-r--r--  2.0 unx     3282 b- defN 24-May-23 10:56 migrations/0020_drain_nodes_from_cluster.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-23 10:56 migrations/__init__.py
+-rw-r--r--  2.0 unx      891 b- defN 24-May-23 10:56 nucliadb/__init__.py
+-rw-r--r--  2.0 unx     3733 b- defN 24-May-23 10:56 nucliadb/health.py
+-rw-r--r--  2.0 unx    11639 b- defN 24-May-23 10:56 nucliadb/learning_proxy.py
+-rw-r--r--  2.0 unx     4806 b- defN 24-May-23 10:56 nucliadb/metrics_exporter.py
+-rw-r--r--  2.0 unx     2272 b- defN 24-May-23 10:56 nucliadb/openapi.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-23 10:56 nucliadb/py.typed
+-rw-r--r--  2.0 unx      835 b- defN 24-May-23 10:56 nucliadb/common/__init__.py
+-rw-r--r--  2.0 unx     5175 b- defN 24-May-23 10:56 nucliadb/common/locking.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-23 10:56 nucliadb/common/cluster/__init__.py
+-rw-r--r--  2.0 unx     5080 b- defN 24-May-23 10:56 nucliadb/common/cluster/base.py
+-rw-r--r--  2.0 unx     1495 b- defN 24-May-23 10:56 nucliadb/common/cluster/exceptions.py
+-rw-r--r--  2.0 unx     3793 b- defN 24-May-23 10:56 nucliadb/common/cluster/grpc_node_dummy.py
+-rw-r--r--  2.0 unx     3429 b- defN 24-May-23 10:56 nucliadb/common/cluster/index_node.py
+-rw-r--r--  2.0 unx    22091 b- defN 24-May-23 10:56 nucliadb/common/cluster/manager.py
+-rw-r--r--  2.0 unx     8853 b- defN 24-May-23 10:56 nucliadb/common/cluster/rebalance.py
+-rw-r--r--  2.0 unx    20209 b- defN 24-May-23 10:56 nucliadb/common/cluster/rollover.py
+-rw-r--r--  2.0 unx     3016 b- defN 24-May-23 10:56 nucliadb/common/cluster/settings.py
+-rw-r--r--  2.0 unx     5713 b- defN 24-May-23 10:56 nucliadb/common/cluster/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-23 10:56 nucliadb/common/cluster/discovery/__init__.py
+-rw-r--r--  2.0 unx     6553 b- defN 24-May-23 10:56 nucliadb/common/cluster/discovery/base.py
+-rw-r--r--  2.0 unx    12512 b- defN 24-May-23 10:56 nucliadb/common/cluster/discovery/k8s.py
+-rw-r--r--  2.0 unx     1957 b- defN 24-May-23 10:56 nucliadb/common/cluster/discovery/manual.py
+-rw-r--r--  2.0 unx     1737 b- defN 24-May-23 10:56 nucliadb/common/cluster/discovery/single.py
+-rw-r--r--  2.0 unx     1139 b- defN 24-May-23 10:56 nucliadb/common/cluster/discovery/types.py
+-rw-r--r--  2.0 unx     2548 b- defN 24-May-23 10:56 nucliadb/common/cluster/discovery/utils.py
+-rw-r--r--  2.0 unx      833 b- defN 24-May-23 10:56 nucliadb/common/cluster/standalone/__init__.py
+-rw-r--r--  2.0 unx    13712 b- defN 24-May-23 10:56 nucliadb/common/cluster/standalone/grpc_node_binding.py
+-rw-r--r--  2.0 unx     4683 b- defN 24-May-23 10:56 nucliadb/common/cluster/standalone/index_node.py
+-rw-r--r--  2.0 unx     3444 b- defN 24-May-23 10:56 nucliadb/common/cluster/standalone/service.py
+-rw-r--r--  2.0 unx     3545 b- defN 24-May-23 10:56 nucliadb/common/cluster/standalone/utils.py
+-rw-r--r--  2.0 unx     3440 b- defN 24-May-23 10:56 nucliadb/common/context/__init__.py
+-rw-r--r--  2.0 unx     1628 b- defN 24-May-23 10:56 nucliadb/common/context/fastapi.py
+-rw-r--r--  2.0 unx     1880 b- defN 24-May-23 10:56 nucliadb/common/datamanagers/__init__.py
+-rw-r--r--  2.0 unx     1451 b- defN 24-May-23 10:56 nucliadb/common/datamanagers/cluster.py
+-rw-r--r--  2.0 unx     5383 b- defN 24-May-23 10:56 nucliadb/common/datamanagers/entities.py
+-rw-r--r--  2.0 unx      883 b- defN 24-May-23 10:56 nucliadb/common/datamanagers/exceptions.py
+-rw-r--r--  2.0 unx     3994 b- defN 24-May-23 10:56 nucliadb/common/datamanagers/kb.py
+-rw-r--r--  2.0 unx     5389 b- defN 24-May-23 10:56 nucliadb/common/datamanagers/labels.py
+-rw-r--r--  2.0 unx     1599 b- defN 24-May-23 10:56 nucliadb/common/datamanagers/processing.py
+-rw-r--r--  2.0 unx    12177 b- defN 24-May-23 10:56 nucliadb/common/datamanagers/resources.py
+-rw-r--r--  2.0 unx     5634 b- defN 24-May-23 10:56 nucliadb/common/datamanagers/rollover.py
+-rw-r--r--  2.0 unx     1548 b- defN 24-May-23 10:56 nucliadb/common/datamanagers/synonyms.py
+-rw-r--r--  2.0 unx     1631 b- defN 24-May-23 10:56 nucliadb/common/datamanagers/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-23 10:56 nucliadb/common/http_clients/__init__.py
+-rw-r--r--  2.0 unx     2146 b- defN 24-May-23 10:56 nucliadb/common/http_clients/auth.py
+-rw-r--r--  2.0 unx     1100 b- defN 24-May-23 10:56 nucliadb/common/http_clients/exceptions.py
+-rw-r--r--  2.0 unx     7155 b- defN 24-May-23 10:56 nucliadb/common/http_clients/processing.py
+-rw-r--r--  2.0 unx     1540 b- defN 24-May-23 10:56 nucliadb/common/http_clients/pypi.py
+-rw-r--r--  2.0 unx     1551 b- defN 24-May-23 10:56 nucliadb/common/http_clients/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-23 10:56 nucliadb/common/maindb/__init__.py
+-rw-r--r--  2.0 unx     3449 b- defN 24-May-23 10:56 nucliadb/common/maindb/driver.py
+-rw-r--r--  2.0 unx      946 b- defN 24-May-23 10:56 nucliadb/common/maindb/exceptions.py
+-rw-r--r--  2.0 unx     6769 b- defN 24-May-23 10:56 nucliadb/common/maindb/local.py
+-rw-r--r--  2.0 unx     8391 b- defN 24-May-23 10:56 nucliadb/common/maindb/pg.py
+-rw-r--r--  2.0 unx     6053 b- defN 24-May-23 10:56 nucliadb/common/maindb/redis.py
+-rw-r--r--  2.0 unx    14502 b- defN 24-May-23 10:56 nucliadb/common/maindb/tikv.py
+-rw-r--r--  2.0 unx     4167 b- defN 24-May-23 10:56 nucliadb/common/maindb/utils.py
+-rw-r--r--  2.0 unx      932 b- defN 24-May-23 10:56 nucliadb/export_import/__init__.py
+-rw-r--r--  2.0 unx     6171 b- defN 24-May-23 10:56 nucliadb/export_import/datamanager.py
+-rw-r--r--  2.0 unx     1949 b- defN 24-May-23 10:56 nucliadb/export_import/exceptions.py
+-rw-r--r--  2.0 unx     7116 b- defN 24-May-23 10:56 nucliadb/export_import/exporter.py
+-rw-r--r--  2.0 unx     4258 b- defN 24-May-23 10:56 nucliadb/export_import/importer.py
+-rw-r--r--  2.0 unx     2063 b- defN 24-May-23 10:56 nucliadb/export_import/models.py
+-rw-r--r--  2.0 unx     2571 b- defN 24-May-23 10:56 nucliadb/export_import/tasks.py
+-rw-r--r--  2.0 unx    19401 b- defN 24-May-23 10:56 nucliadb/export_import/utils.py
+-rw-r--r--  2.0 unx     1011 b- defN 24-May-23 10:56 nucliadb/ingest/__init__.py
+-rw-r--r--  2.0 unx     7277 b- defN 24-May-23 10:56 nucliadb/ingest/app.py
+-rw-r--r--  2.0 unx     1005 b- defN 24-May-23 10:56 nucliadb/ingest/cache.py
+-rw-r--r--  2.0 unx     2484 b- defN 24-May-23 10:56 nucliadb/ingest/partitions.py
+-rw-r--r--  2.0 unx    19904 b- defN 24-May-23 10:56 nucliadb/ingest/processing.py
+-rw-r--r--  2.0 unx    20277 b- defN 24-May-23 10:56 nucliadb/ingest/serialize.py
+-rw-r--r--  2.0 unx     3207 b- defN 24-May-23 10:56 nucliadb/ingest/settings.py
+-rw-r--r--  2.0 unx     2314 b- defN 24-May-23 10:56 nucliadb/ingest/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-23 10:56 nucliadb/ingest/consumer/__init__.py
+-rw-r--r--  2.0 unx     6918 b- defN 24-May-23 10:56 nucliadb/ingest/consumer/auditing.py
+-rw-r--r--  2.0 unx    12174 b- defN 24-May-23 10:56 nucliadb/ingest/consumer/consumer.py
+-rw-r--r--  2.0 unx     3945 b- defN 24-May-23 10:56 nucliadb/ingest/consumer/materializer.py
+-rw-r--r--  2.0 unx     1075 b- defN 24-May-23 10:56 nucliadb/ingest/consumer/metrics.py
+-rw-r--r--  2.0 unx     9543 b- defN 24-May-23 10:56 nucliadb/ingest/consumer/pull.py
+-rw-r--r--  2.0 unx     6871 b- defN 24-May-23 10:56 nucliadb/ingest/consumer/service.py
+-rw-r--r--  2.0 unx     4331 b- defN 24-May-23 10:56 nucliadb/ingest/consumer/shard_creator.py
+-rw-r--r--  2.0 unx     2656 b- defN 24-May-23 10:56 nucliadb/ingest/consumer/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-23 10:56 nucliadb/ingest/fields/__init__.py
+-rw-r--r--  2.0 unx    17461 b- defN 24-May-23 10:56 nucliadb/ingest/fields/base.py
+-rw-r--r--  2.0 unx     6516 b- defN 24-May-23 10:56 nucliadb/ingest/fields/conversation.py
+-rw-r--r--  2.0 unx     1223 b- defN 24-May-23 10:56 nucliadb/ingest/fields/date.py
+-rw-r--r--  2.0 unx     1205 b- defN 24-May-23 10:56 nucliadb/ingest/fields/exceptions.py
+-rw-r--r--  2.0 unx     4840 b- defN 24-May-23 10:56 nucliadb/ingest/fields/file.py
+-rw-r--r--  2.0 unx     1547 b- defN 24-May-23 10:56 nucliadb/ingest/fields/generic.py
+-rw-r--r--  2.0 unx     1235 b- defN 24-May-23 10:56 nucliadb/ingest/fields/keywordset.py
+-rw-r--r--  2.0 unx     2250 b- defN 24-May-23 10:56 nucliadb/ingest/fields/layout.py
+-rw-r--r--  2.0 unx     4212 b- defN 24-May-23 10:56 nucliadb/ingest/fields/link.py
+-rw-r--r--  2.0 unx     1319 b- defN 24-May-23 10:56 nucliadb/ingest/fields/text.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-23 10:56 nucliadb/ingest/orm/__init__.py
+-rw-r--r--  2.0 unx    28311 b- defN 24-May-23 10:56 nucliadb/ingest/orm/brain.py
+-rw-r--r--  2.0 unx    15758 b- defN 24-May-23 10:56 nucliadb/ingest/orm/entities.py
+-rw-r--r--  2.0 unx     1279 b- defN 24-May-23 10:56 nucliadb/ingest/orm/exceptions.py
+-rw-r--r--  2.0 unx    15621 b- defN 24-May-23 10:56 nucliadb/ingest/orm/knowledgebox.py
+-rw-r--r--  2.0 unx     1096 b- defN 24-May-23 10:56 nucliadb/ingest/orm/metrics.py
+-rw-r--r--  2.0 unx    58955 b- defN 24-May-23 10:56 nucliadb/ingest/orm/resource.py
+-rw-r--r--  2.0 unx     2685 b- defN 24-May-23 10:56 nucliadb/ingest/orm/utils.py
+-rw-r--r--  2.0 unx    27042 b- defN 24-May-23 10:56 nucliadb/ingest/orm/processor/__init__.py
+-rw-r--r--  2.0 unx     5090 b- defN 24-May-23 10:56 nucliadb/ingest/orm/processor/auditing.py
+-rw-r--r--  2.0 unx     1690 b- defN 24-May-23 10:56 nucliadb/ingest/orm/processor/sequence_manager.py
+-rw-r--r--  2.0 unx     2057 b- defN 24-May-23 10:56 nucliadb/ingest/service/__init__.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-23 10:56 nucliadb/ingest/service/exceptions.py
+-rw-r--r--  2.0 unx    30462 b- defN 24-May-23 10:56 nucliadb/ingest/service/writer.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-23 10:56 nucliadb/ingest/tests/__init__.py
+-rw-r--r--  2.0 unx     1157 b- defN 24-May-23 10:56 nucliadb/ingest/tests/conftest.py
+-rw-r--r--  2.0 unx    24060 b- defN 24-May-23 10:56 nucliadb/ingest/tests/fixtures.py
+-rw-r--r--  2.0 unx    62843 b- defN 24-May-23 10:56 nucliadb/ingest/tests/vectors.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-23 10:56 nucliadb/ingest/tests/integration/__init__.py
+-rw-r--r--  2.0 unx      833 b- defN 24-May-23 10:56 nucliadb/ingest/tests/integration/consumer/__init__.py
+-rw-r--r--  2.0 unx     2500 b- defN 24-May-23 10:56 nucliadb/ingest/tests/integration/consumer/test_auditing.py
+-rw-r--r--  2.0 unx     3832 b- defN 24-May-23 10:56 nucliadb/ingest/tests/integration/consumer/test_materializer.py
+-rw-r--r--  2.0 unx     4470 b- defN 24-May-23 10:56 nucliadb/ingest/tests/integration/consumer/test_pull.py
+-rw-r--r--  2.0 unx     2763 b- defN 24-May-23 10:56 nucliadb/ingest/tests/integration/consumer/test_service.py
+-rw-r--r--  2.0 unx     2019 b- defN 24-May-23 10:56 nucliadb/ingest/tests/integration/consumer/test_shard_creator.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-23 10:56 nucliadb/ingest/tests/integration/ingest/__init__.py
+-rw-r--r--  2.0 unx    27247 b- defN 24-May-23 10:56 nucliadb/ingest/tests/integration/ingest/test_ingest.py
+-rw-r--r--  2.0 unx     3040 b- defN 24-May-23 10:56 nucliadb/ingest/tests/integration/ingest/test_processing_engine.py
+-rw-r--r--  2.0 unx     8586 b- defN 24-May-23 10:56 nucliadb/ingest/tests/integration/ingest/test_relations.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-23 10:56 nucliadb/ingest/tests/unit/__init__.py
+-rw-r--r--  2.0 unx     1189 b- defN 24-May-23 10:56 nucliadb/ingest/tests/unit/test_cache.py
+-rw-r--r--  2.0 unx     1432 b- defN 24-May-23 10:56 nucliadb/ingest/tests/unit/test_partitions.py
+-rw-r--r--  2.0 unx     5807 b- defN 24-May-23 10:56 nucliadb/ingest/tests/unit/test_processing.py
+-rw-r--r--  2.0 unx      978 b- defN 24-May-23 10:56 nucliadb/ingest/tests/unit/test_settings.py
+-rw-r--r--  2.0 unx      833 b- defN 24-May-23 10:56 nucliadb/ingest/tests/unit/consumer/__init__.py
+-rw-r--r--  2.0 unx     3885 b- defN 24-May-23 10:56 nucliadb/ingest/tests/unit/consumer/test_auditing.py
+-rw-r--r--  2.0 unx     2472 b- defN 24-May-23 10:56 nucliadb/ingest/tests/unit/consumer/test_consumer.py
+-rw-r--r--  2.0 unx     2063 b- defN 24-May-23 10:56 nucliadb/ingest/tests/unit/consumer/test_pull.py
+-rw-r--r--  2.0 unx     4140 b- defN 24-May-23 10:56 nucliadb/ingest/tests/unit/consumer/test_shard_creator.py
+-rw-r--r--  2.0 unx     1934 b- defN 24-May-23 10:56 nucliadb/ingest/tests/unit/consumer/test_utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-23 10:56 nucliadb/ingest/tests/unit/orm/__init__.py
+-rw-r--r--  2.0 unx     9876 b- defN 24-May-23 10:56 nucliadb/ingest/tests/unit/orm/test_brain.py
+-rw-r--r--  2.0 unx     2435 b- defN 24-May-23 10:56 nucliadb/ingest/tests/unit/orm/test_brain_vectors.py
+-rw-r--r--  2.0 unx     1174 b- defN 24-May-23 10:56 nucliadb/ingest/tests/unit/orm/test_orm_utils.py
+-rw-r--r--  2.0 unx     4045 b- defN 24-May-23 10:56 nucliadb/ingest/tests/unit/orm/test_processor.py
+-rw-r--r--  2.0 unx    11033 b- defN 24-May-23 10:56 nucliadb/ingest/tests/unit/orm/test_resource.py
+-rw-r--r--  2.0 unx     2216 b- defN 24-May-23 10:56 nucliadb/middleware/__init__.py
+-rw-r--r--  2.0 unx     3912 b- defN 24-May-23 10:56 nucliadb/middleware/transaction.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-23 10:56 nucliadb/migrator/__init__.py
+-rw-r--r--  2.0 unx     2119 b- defN 24-May-23 10:56 nucliadb/migrator/command.py
+-rw-r--r--  2.0 unx     1334 b- defN 24-May-23 10:56 nucliadb/migrator/context.py
+-rw-r--r--  2.0 unx     5104 b- defN 24-May-23 10:56 nucliadb/migrator/datamanager.py
+-rw-r--r--  2.0 unx      889 b- defN 24-May-23 10:56 nucliadb/migrator/exceptions.py
+-rw-r--r--  2.0 unx     9370 b- defN 24-May-23 10:56 nucliadb/migrator/migrator.py
+-rw-r--r--  2.0 unx     1145 b- defN 24-May-23 10:56 nucliadb/migrator/models.py
+-rw-r--r--  2.0 unx     1144 b- defN 24-May-23 10:56 nucliadb/migrator/settings.py
+-rw-r--r--  2.0 unx     2346 b- defN 24-May-23 10:56 nucliadb/migrator/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-23 10:56 nucliadb/models/__init__.py
+-rw-r--r--  2.0 unx     1599 b- defN 24-May-23 10:56 nucliadb/models/responses.py
+-rw-r--r--  2.0 unx     6041 b- defN 24-May-23 10:56 nucliadb/purge/__init__.py
+-rw-r--r--  2.0 unx     9364 b- defN 24-May-23 10:56 nucliadb/purge/orphan_shards.py
+-rw-r--r--  2.0 unx     1328 b- defN 24-May-23 10:56 nucliadb/reader/__init__.py
+-rw-r--r--  2.0 unx     3709 b- defN 24-May-23 10:56 nucliadb/reader/app.py
+-rw-r--r--  2.0 unx     1366 b- defN 24-May-23 10:56 nucliadb/reader/lifecycle.py
+-rw-r--r--  2.0 unx     1031 b- defN 24-May-23 10:56 nucliadb/reader/openapi.py
+-rw-r--r--  2.0 unx     1447 b- defN 24-May-23 10:56 nucliadb/reader/run.py
+-rw-r--r--  2.0 unx      872 b- defN 24-May-23 10:56 nucliadb/reader/api/__init__.py
+-rw-r--r--  2.0 unx     2458 b- defN 24-May-23 10:56 nucliadb/reader/api/models.py
+-rw-r--r--  2.0 unx     1110 b- defN 24-May-23 10:56 nucliadb/reader/api/v1/__init__.py
+-rw-r--r--  2.0 unx    12392 b- defN 24-May-23 10:56 nucliadb/reader/api/v1/download.py
+-rw-r--r--  2.0 unx     6459 b- defN 24-May-23 10:56 nucliadb/reader/api/v1/export_import.py
+-rw-r--r--  2.0 unx     3641 b- defN 24-May-23 10:56 nucliadb/reader/api/v1/knowledgebox.py
+-rw-r--r--  2.0 unx     2099 b- defN 24-May-23 10:56 nucliadb/reader/api/v1/learning_collector.py
+-rw-r--r--  2.0 unx     4472 b- defN 24-May-23 10:56 nucliadb/reader/api/v1/learning_config.py
+-rw-r--r--  2.0 unx    13951 b- defN 24-May-23 10:56 nucliadb/reader/api/v1/resource.py
+-rw-r--r--  2.0 unx     1011 b- defN 24-May-23 10:56 nucliadb/reader/api/v1/router.py
+-rw-r--r--  2.0 unx    12115 b- defN 24-May-23 10:56 nucliadb/reader/api/v1/services.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-23 10:56 nucliadb/reader/reader/__init__.py
+-rw-r--r--  2.0 unx     7979 b- defN 24-May-23 10:56 nucliadb/reader/reader/notifications.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-23 10:56 nucliadb/reader/tests/__init__.py
+-rw-r--r--  2.0 unx     1224 b- defN 24-May-23 10:56 nucliadb/reader/tests/conftest.py
+-rw-r--r--  2.0 unx     4345 b- defN 24-May-23 10:56 nucliadb/reader/tests/fixtures.py
+-rw-r--r--  2.0 unx     2748 b- defN 24-May-23 10:56 nucliadb/reader/tests/test_list_resources.py
+-rw-r--r--  2.0 unx    10199 b- defN 24-May-23 10:56 nucliadb/reader/tests/test_reader_file_download.py
+-rw-r--r--  2.0 unx    10586 b- defN 24-May-23 10:56 nucliadb/reader/tests/test_reader_resource.py
+-rw-r--r--  2.0 unx     6535 b- defN 24-May-23 10:56 nucliadb/reader/tests/test_reader_resource_field.py
+-rw-r--r--  2.0 unx     1535 b- defN 24-May-23 10:56 nucliadb/search/__init__.py
+-rw-r--r--  2.0 unx     4905 b- defN 24-May-23 10:56 nucliadb/search/app.py
+-rw-r--r--  2.0 unx     1956 b- defN 24-May-23 10:56 nucliadb/search/lifecycle.py
+-rw-r--r--  2.0 unx     1016 b- defN 24-May-23 10:56 nucliadb/search/openapi.py
+-rw-r--r--  2.0 unx    20665 b- defN 24-May-23 10:56 nucliadb/search/predict.py
+-rw-r--r--  2.0 unx     1402 b- defN 24-May-23 10:56 nucliadb/search/run.py
+-rw-r--r--  2.0 unx     1193 b- defN 24-May-23 10:56 nucliadb/search/settings.py
+-rw-r--r--  2.0 unx     1037 b- defN 24-May-23 10:56 nucliadb/search/utilities.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-23 10:56 nucliadb/search/api/__init__.py
+-rw-r--r--  2.0 unx     1298 b- defN 24-May-23 10:56 nucliadb/search/api/v1/__init__.py
+-rw-r--r--  2.0 unx     3534 b- defN 24-May-23 10:56 nucliadb/search/api/v1/ask.py
+-rw-r--r--  2.0 unx     9493 b- defN 24-May-23 10:56 nucliadb/search/api/v1/chat.py
+-rw-r--r--  2.0 unx     2668 b- defN 24-May-23 10:56 nucliadb/search/api/v1/feedback.py
+-rw-r--r--  2.0 unx     8795 b- defN 24-May-23 10:56 nucliadb/search/api/v1/find.py
+-rw-r--r--  2.0 unx     6938 b- defN 24-May-23 10:56 nucliadb/search/api/v1/knowledgebox.py
+-rw-r--r--  2.0 unx     3047 b- defN 24-May-23 10:56 nucliadb/search/api/v1/predict_proxy.py
+-rw-r--r--  2.0 unx      988 b- defN 24-May-23 10:56 nucliadb/search/api/v1/router.py
+-rw-r--r--  2.0 unx    19262 b- defN 24-May-23 10:56 nucliadb/search/api/v1/search.py
+-rw-r--r--  2.0 unx     5970 b- defN 24-May-23 10:56 nucliadb/search/api/v1/suggest.py
+-rw-r--r--  2.0 unx     2499 b- defN 24-May-23 10:56 nucliadb/search/api/v1/summarize.py
+-rw-r--r--  2.0 unx     1434 b- defN 24-May-23 10:56 nucliadb/search/api/v1/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-23 10:56 nucliadb/search/api/v1/resource/__init__.py
+-rw-r--r--  2.0 unx     4064 b- defN 24-May-23 10:56 nucliadb/search/api/v1/resource/ask.py
+-rw-r--r--  2.0 unx     5821 b- defN 24-May-23 10:56 nucliadb/search/api/v1/resource/chat.py
+-rw-r--r--  2.0 unx     5303 b- defN 24-May-23 10:56 nucliadb/search/api/v1/resource/search.py
+-rw-r--r--  2.0 unx      833 b- defN 24-May-23 10:56 nucliadb/search/requesters/__init__.py
+-rw-r--r--  2.0 unx     9111 b- defN 24-May-23 10:56 nucliadb/search/requesters/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-23 10:56 nucliadb/search/search/__init__.py
+-rw-r--r--  2.0 unx     2746 b- defN 24-May-23 10:56 nucliadb/search/search/cache.py
+-rw-r--r--  2.0 unx     1154 b- defN 24-May-23 10:56 nucliadb/search/search/exceptions.py
+-rw-r--r--  2.0 unx     5465 b- defN 24-May-23 10:56 nucliadb/search/search/fetch.py
+-rw-r--r--  2.0 unx     6513 b- defN 24-May-23 10:56 nucliadb/search/search/filters.py
+-rw-r--r--  2.0 unx     4612 b- defN 24-May-23 10:56 nucliadb/search/search/find.py
+-rw-r--r--  2.0 unx    17152 b- defN 24-May-23 10:56 nucliadb/search/search/find_merge.py
+-rw-r--r--  2.0 unx    21282 b- defN 24-May-23 10:56 nucliadb/search/search/merge.py
+-rw-r--r--  2.0 unx     1130 b- defN 24-May-23 10:56 nucliadb/search/search/metrics.py
+-rw-r--r--  2.0 unx     8698 b- defN 24-May-23 10:56 nucliadb/search/search/paragraphs.py
+-rw-r--r--  2.0 unx     3026 b- defN 24-May-23 10:56 nucliadb/search/search/predict_proxy.py
+-rw-r--r--  2.0 unx    31093 b- defN 24-May-23 10:56 nucliadb/search/search/query.py
+-rw-r--r--  2.0 unx     3018 b- defN 24-May-23 10:56 nucliadb/search/search/shards.py
+-rw-r--r--  2.0 unx     5101 b- defN 24-May-23 10:56 nucliadb/search/search/summarize.py
+-rw-r--r--  2.0 unx     2438 b- defN 24-May-23 10:56 nucliadb/search/search/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-23 10:56 nucliadb/search/search/chat/__init__.py
+-rw-r--r--  2.0 unx    16676 b- defN 24-May-23 10:56 nucliadb/search/search/chat/ask.py
+-rw-r--r--  2.0 unx     2058 b- defN 24-May-23 10:56 nucliadb/search/search/chat/images.py
+-rw-r--r--  2.0 unx    20793 b- defN 24-May-23 10:56 nucliadb/search/search/chat/prompt.py
+-rw-r--r--  2.0 unx    17543 b- defN 24-May-23 10:56 nucliadb/search/search/chat/query.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-23 10:56 nucliadb/search/tests/__init__.py
+-rw-r--r--  2.0 unx     1295 b- defN 24-May-23 10:56 nucliadb/search/tests/conftest.py
+-rw-r--r--  2.0 unx     6578 b- defN 24-May-23 10:56 nucliadb/search/tests/fixtures.py
+-rw-r--r--  2.0 unx    15480 b- defN 24-May-23 10:56 nucliadb/search/tests/node.py
+-rw-r--r--  2.0 unx      833 b- defN 24-May-23 10:56 nucliadb/search/tests/unit/__init__.py
+-rw-r--r--  2.0 unx     2649 b- defN 24-May-23 10:56 nucliadb/search/tests/unit/test_app.py
+-rw-r--r--  2.0 unx     3374 b- defN 24-May-23 10:56 nucliadb/search/tests/unit/test_find_merge.py
+-rw-r--r--  2.0 unx     1400 b- defN 24-May-23 10:56 nucliadb/search/tests/unit/test_merge.py
+-rw-r--r--  2.0 unx    15721 b- defN 24-May-23 10:56 nucliadb/search/tests/unit/test_predict.py
+-rw-r--r--  2.0 unx     1328 b- defN 24-May-23 10:56 nucliadb/search/tests/unit/test_run.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-23 10:56 nucliadb/search/tests/unit/api/__init__.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-23 10:56 nucliadb/search/tests/unit/api/v1/__init__.py
+-rw-r--r--  2.0 unx     3759 b- defN 24-May-23 10:56 nucliadb/search/tests/unit/api/v1/test_ask.py
+-rw-r--r--  2.0 unx     2966 b- defN 24-May-23 10:56 nucliadb/search/tests/unit/api/v1/test_chat.py
+-rw-r--r--  2.0 unx     2865 b- defN 24-May-23 10:56 nucliadb/search/tests/unit/api/v1/test_predict_proxy.py
+-rw-r--r--  2.0 unx     2901 b- defN 24-May-23 10:56 nucliadb/search/tests/unit/api/v1/test_summarize.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-23 10:56 nucliadb/search/tests/unit/api/v1/resource/__init__.py
+-rw-r--r--  2.0 unx     3040 b- defN 24-May-23 10:56 nucliadb/search/tests/unit/api/v1/resource/test_chat.py
+-rw-r--r--  2.0 unx      833 b- defN 24-May-23 10:56 nucliadb/search/tests/unit/search/__init__.py
+-rw-r--r--  2.0 unx     8586 b- defN 24-May-23 10:56 nucliadb/search/tests/unit/search/test_chat_prompt.py
+-rw-r--r--  2.0 unx     3736 b- defN 24-May-23 10:56 nucliadb/search/tests/unit/search/test_fetch.py
+-rw-r--r--  2.0 unx     4306 b- defN 24-May-23 10:56 nucliadb/search/tests/unit/search/test_filters.py
+-rw-r--r--  2.0 unx     4492 b- defN 24-May-23 10:56 nucliadb/search/tests/unit/search/test_paragraphs.py
+-rw-r--r--  2.0 unx     3496 b- defN 24-May-23 10:56 nucliadb/search/tests/unit/search/test_predict_proxy.py
+-rw-r--r--  2.0 unx     5121 b- defN 24-May-23 10:56 nucliadb/search/tests/unit/search/test_query.py
+-rw-r--r--  2.0 unx      833 b- defN 24-May-23 10:56 nucliadb/search/tests/unit/search/requesters/__init__.py
+-rw-r--r--  2.0 unx     6455 b- defN 24-May-23 10:56 nucliadb/search/tests/unit/search/requesters/test_utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-23 10:56 nucliadb/search/tests/unit/search/search/__init__.py
+-rw-r--r--  2.0 unx     1759 b- defN 24-May-23 10:56 nucliadb/search/tests/unit/search/search/test_shards.py
+-rw-r--r--  2.0 unx     2511 b- defN 24-May-23 10:56 nucliadb/search/tests/unit/search/search/test_utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-23 10:56 nucliadb/standalone/__init__.py
+-rw-r--r--  2.0 unx     6746 b- defN 24-May-23 10:56 nucliadb/standalone/api_router.py
+-rw-r--r--  2.0 unx     5763 b- defN 24-May-23 10:56 nucliadb/standalone/app.py
+-rw-r--r--  2.0 unx     7800 b- defN 24-May-23 10:56 nucliadb/standalone/auth.py
+-rw-r--r--  2.0 unx     5313 b- defN 24-May-23 10:56 nucliadb/standalone/config.py
+-rw-r--r--  2.0 unx     6986 b- defN 24-May-23 10:56 nucliadb/standalone/introspect.py
+-rw-r--r--  2.0 unx     2488 b- defN 24-May-23 10:56 nucliadb/standalone/lifecycle.py
+-rw-r--r--  2.0 unx     1980 b- defN 24-May-23 10:56 nucliadb/standalone/migrations.py
+-rw-r--r--  2.0 unx     1322 b- defN 24-May-23 10:56 nucliadb/standalone/purge.py
+-rw-r--r--  2.0 unx     5636 b- defN 24-May-23 10:56 nucliadb/standalone/run.py
+-rw-r--r--  2.0 unx     5822 b- defN 24-May-23 10:56 nucliadb/standalone/settings.py
+-rw-r--r--  2.0 unx     3132 b- defN 24-May-23 10:56 nucliadb/standalone/versions.py
+-rw-r--r--  2.0 unx     2285 b- defN 24-May-23 10:56 nucliadb/standalone/static/favicon.ico
+-rw-r--r--  2.0 unx     3833 b- defN 24-May-23 10:56 nucliadb/standalone/static/index.html
+-rw-r--r--  2.0 unx     2639 b- defN 24-May-23 10:56 nucliadb/standalone/static/logo.svg
+-rw-r--r--  2.0 unx      835 b- defN 24-May-23 10:56 nucliadb/standalone/tests/__init__.py
+-rw-r--r--  2.0 unx     1294 b- defN 24-May-23 10:56 nucliadb/standalone/tests/conftest.py
+-rw-r--r--  2.0 unx     1319 b- defN 24-May-23 10:56 nucliadb/standalone/tests/fixtures.py
+-rw-r--r--  2.0 unx      833 b- defN 24-May-23 10:56 nucliadb/standalone/tests/unit/__init__.py
+-rw-r--r--  2.0 unx     1722 b- defN 24-May-23 10:56 nucliadb/standalone/tests/unit/test_api_router.py
+-rw-r--r--  2.0 unx     5509 b- defN 24-May-23 10:56 nucliadb/standalone/tests/unit/test_auth.py
+-rw-r--r--  2.0 unx     1334 b- defN 24-May-23 10:56 nucliadb/standalone/tests/unit/test_introspect.py
+-rw-r--r--  2.0 unx     1863 b- defN 24-May-23 10:56 nucliadb/standalone/tests/unit/test_migrations.py
+-rw-r--r--  2.0 unx     1546 b- defN 24-May-23 10:56 nucliadb/standalone/tests/unit/test_run.py
+-rw-r--r--  2.0 unx     1972 b- defN 24-May-23 10:56 nucliadb/standalone/tests/unit/test_versions.py
+-rw-r--r--  2.0 unx     1037 b- defN 24-May-23 10:56 nucliadb/tasks/__init__.py
+-rw-r--r--  2.0 unx     7655 b- defN 24-May-23 10:56 nucliadb/tasks/consumer.py
+-rw-r--r--  2.0 unx      924 b- defN 24-May-23 10:56 nucliadb/tasks/logger.py
+-rw-r--r--  2.0 unx     1378 b- defN 24-May-23 10:56 nucliadb/tasks/models.py
+-rw-r--r--  2.0 unx     3457 b- defN 24-May-23 10:56 nucliadb/tasks/producer.py
+-rw-r--r--  2.0 unx     1753 b- defN 24-May-23 10:56 nucliadb/tasks/registry.py
+-rw-r--r--  2.0 unx     1360 b- defN 24-May-23 10:56 nucliadb/tasks/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-23 10:56 nucliadb/tests/__init__.py
+-rw-r--r--  2.0 unx     1229 b- defN 24-May-23 10:56 nucliadb/tests/conftest.py
+-rw-r--r--  2.0 unx    22365 b- defN 24-May-23 10:56 nucliadb/tests/fixtures.py
+-rw-r--r--  2.0 unx     7549 b- defN 24-May-23 10:56 nucliadb/tests/tikv.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-23 10:56 nucliadb/tests/benchmarks/__init__.py
+-rw-r--r--  2.0 unx     3032 b- defN 24-May-23 10:56 nucliadb/tests/benchmarks/test_search.py
+-rw-r--r--  2.0 unx      919 b- defN 24-May-23 10:56 nucliadb/tests/knowledgeboxes/__init__.py
+-rw-r--r--  2.0 unx     7002 b- defN 24-May-23 10:56 nucliadb/tests/knowledgeboxes/philosophy_books.py
+-rw-r--r--  2.0 unx     3037 b- defN 24-May-23 10:56 nucliadb/tests/knowledgeboxes/ten_dummy_resources.py
+-rw-r--r--  2.0 unx     1148 b- defN 24-May-23 10:56 nucliadb/tests/migrations/__init__.py
+-rw-r--r--  2.0 unx     2726 b- defN 24-May-23 10:56 nucliadb/tests/migrations/test_migration_0017.py
+-rw-r--r--  2.0 unx     3662 b- defN 24-May-23 10:56 nucliadb/tests/migrations/test_migration_0018.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-23 10:56 nucliadb/tests/unit/__init__.py
+-rw-r--r--  2.0 unx     1487 b- defN 24-May-23 10:56 nucliadb/tests/unit/test_field_ids.py
+-rw-r--r--  2.0 unx     2780 b- defN 24-May-23 10:56 nucliadb/tests/unit/test_health.py
+-rw-r--r--  2.0 unx     1543 b- defN 24-May-23 10:56 nucliadb/tests/unit/test_kb_slugs.py
+-rw-r--r--  2.0 unx     7892 b- defN 24-May-23 10:56 nucliadb/tests/unit/test_learning_proxy.py
+-rw-r--r--  2.0 unx     2642 b- defN 24-May-23 10:56 nucliadb/tests/unit/test_metrics_exporter.py
+-rw-r--r--  2.0 unx     1341 b- defN 24-May-23 10:56 nucliadb/tests/unit/test_openapi.py
+-rw-r--r--  2.0 unx     3649 b- defN 24-May-23 10:56 nucliadb/tests/unit/test_purge.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-23 10:56 nucliadb/tests/unit/common/__init__.py
+-rw-r--r--  2.0 unx     1268 b- defN 24-May-23 10:56 nucliadb/tests/unit/common/test_context.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-23 10:56 nucliadb/tests/unit/common/cluster/__init__.py
+-rw-r--r--  2.0 unx    12240 b- defN 24-May-23 10:56 nucliadb/tests/unit/common/cluster/test_cluster.py
+-rw-r--r--  2.0 unx     5387 b- defN 24-May-23 10:56 nucliadb/tests/unit/common/cluster/test_kb_shard_manager.py
+-rw-r--r--  2.0 unx     1428 b- defN 24-May-23 10:56 nucliadb/tests/unit/common/cluster/test_rebalance.py
+-rw-r--r--  2.0 unx     9465 b- defN 24-May-23 10:56 nucliadb/tests/unit/common/cluster/test_rollover.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-23 10:56 nucliadb/tests/unit/common/cluster/discovery/__init__.py
+-rw-r--r--  2.0 unx     5627 b- defN 24-May-23 10:56 nucliadb/tests/unit/common/cluster/discovery/test_k8s.py
+-rw-r--r--  2.0 unx      833 b- defN 24-May-23 10:56 nucliadb/tests/unit/common/cluster/standalone/__init__.py
+-rw-r--r--  2.0 unx     3761 b- defN 24-May-23 10:56 nucliadb/tests/unit/common/cluster/standalone/test_service.py
+-rw-r--r--  2.0 unx     2136 b- defN 24-May-23 10:56 nucliadb/tests/unit/common/cluster/standalone/test_utils.py
+-rw-r--r--  2.0 unx      833 b- defN 24-May-23 10:56 nucliadb/tests/unit/common/maindb/__init__.py
+-rw-r--r--  2.0 unx     3579 b- defN 24-May-23 10:56 nucliadb/tests/unit/common/maindb/test_driver.py
+-rw-r--r--  2.0 unx     1869 b- defN 24-May-23 10:56 nucliadb/tests/unit/common/maindb/test_tikv.py
+-rw-r--r--  2.0 unx     3213 b- defN 24-May-23 10:56 nucliadb/tests/unit/common/maindb/test_utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-23 10:56 nucliadb/tests/unit/export_import/__init__.py
+-rw-r--r--  2.0 unx     1435 b- defN 24-May-23 10:56 nucliadb/tests/unit/export_import/test_datamanager.py
+-rw-r--r--  2.0 unx     9706 b- defN 24-May-23 10:56 nucliadb/tests/unit/export_import/test_utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-23 10:56 nucliadb/tests/unit/migrator/__init__.py
+-rw-r--r--  2.0 unx     3233 b- defN 24-May-23 10:56 nucliadb/tests/unit/migrator/test_migrator.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-23 10:56 nucliadb/tests/unit/tasks/__init__.py
+-rw-r--r--  2.0 unx     1375 b- defN 24-May-23 10:56 nucliadb/tests/unit/tasks/conftest.py
+-rw-r--r--  2.0 unx     2714 b- defN 24-May-23 10:56 nucliadb/tests/unit/tasks/test_consumer.py
+-rw-r--r--  2.0 unx     3189 b- defN 24-May-23 10:56 nucliadb/tests/unit/tasks/test_producer.py
+-rw-r--r--  2.0 unx     1827 b- defN 24-May-23 10:56 nucliadb/tests/unit/tasks/test_tasks.py
+-rw-r--r--  2.0 unx     2507 b- defN 24-May-23 10:56 nucliadb/tests/utils/__init__.py
+-rw-r--r--  2.0 unx     1797 b- defN 24-May-23 10:56 nucliadb/tests/utils/aiohttp_session.py
+-rw-r--r--  2.0 unx     2533 b- defN 24-May-23 10:56 nucliadb/tests/utils/entities.py
+-rw-r--r--  2.0 unx     6327 b- defN 24-May-23 10:56 nucliadb/tests/utils/broker_messages/__init__.py
+-rw-r--r--  2.0 unx     7557 b- defN 24-May-23 10:56 nucliadb/tests/utils/broker_messages/fields.py
+-rw-r--r--  2.0 unx     1196 b- defN 24-May-23 10:56 nucliadb/tests/utils/broker_messages/helpers.py
+-rw-r--r--  2.0 unx     1325 b- defN 24-May-23 10:56 nucliadb/train/__init__.py
+-rw-r--r--  2.0 unx     3530 b- defN 24-May-23 10:56 nucliadb/train/app.py
+-rw-r--r--  2.0 unx     3800 b- defN 24-May-23 10:56 nucliadb/train/generator.py
+-rw-r--r--  2.0 unx     1698 b- defN 24-May-23 10:56 nucliadb/train/lifecycle.py
+-rw-r--r--  2.0 unx     1198 b- defN 24-May-23 10:56 nucliadb/train/models.py
+-rw-r--r--  2.0 unx     5706 b- defN 24-May-23 10:56 nucliadb/train/nodes.py
+-rw-r--r--  2.0 unx     1400 b- defN 24-May-23 10:56 nucliadb/train/run.py
+-rw-r--r--  2.0 unx     5926 b- defN 24-May-23 10:56 nucliadb/train/servicer.py
+-rw-r--r--  2.0 unx     1415 b- defN 24-May-23 10:56 nucliadb/train/settings.py
+-rw-r--r--  2.0 unx     1496 b- defN 24-May-23 10:56 nucliadb/train/types.py
+-rw-r--r--  2.0 unx     3265 b- defN 24-May-23 10:56 nucliadb/train/upload.py
+-rw-r--r--  2.0 unx     6420 b- defN 24-May-23 10:56 nucliadb/train/uploader.py
+-rw-r--r--  2.0 unx     3179 b- defN 24-May-23 10:56 nucliadb/train/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-23 10:56 nucliadb/train/api/__init__.py
+-rw-r--r--  2.0 unx     1479 b- defN 24-May-23 10:56 nucliadb/train/api/utils.py
+-rw-r--r--  2.0 unx      928 b- defN 24-May-23 10:56 nucliadb/train/api/v1/__init__.py
+-rw-r--r--  2.0 unx     2071 b- defN 24-May-23 10:56 nucliadb/train/api/v1/check.py
+-rw-r--r--  2.0 unx      910 b- defN 24-May-23 10:56 nucliadb/train/api/v1/router.py
+-rw-r--r--  2.0 unx     1908 b- defN 24-May-23 10:56 nucliadb/train/api/v1/shards.py
+-rw-r--r--  2.0 unx     2135 b- defN 24-May-23 10:56 nucliadb/train/api/v1/trainset.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-23 10:56 nucliadb/train/generators/__init__.py
+-rw-r--r--  2.0 unx     3723 b- defN 24-May-23 10:56 nucliadb/train/generators/field_classifier.py
+-rw-r--r--  2.0 unx     6712 b- defN 24-May-23 10:56 nucliadb/train/generators/image_classifier.py
+-rw-r--r--  2.0 unx     2789 b- defN 24-May-23 10:56 nucliadb/train/generators/paragraph_classifier.py
+-rw-r--r--  2.0 unx     3590 b- defN 24-May-23 10:56 nucliadb/train/generators/paragraph_streaming.py
+-rw-r--r--  2.0 unx     5372 b- defN 24-May-23 10:56 nucliadb/train/generators/question_answer_streaming.py
+-rw-r--r--  2.0 unx     5160 b- defN 24-May-23 10:56 nucliadb/train/generators/sentence_classifier.py
+-rw-r--r--  2.0 unx    10446 b- defN 24-May-23 10:56 nucliadb/train/generators/token_classifier.py
+-rw-r--r--  2.0 unx     3877 b- defN 24-May-23 10:56 nucliadb/train/generators/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-23 10:56 nucliadb/train/tests/__init__.py
+-rw-r--r--  2.0 unx     1125 b- defN 24-May-23 10:56 nucliadb/train/tests/conftest.py
+-rw-r--r--  2.0 unx    11053 b- defN 24-May-23 10:56 nucliadb/train/tests/fixtures.py
+-rw-r--r--  2.0 unx     4598 b- defN 24-May-23 10:56 nucliadb/train/tests/test_field_classification.py
+-rw-r--r--  2.0 unx     2729 b- defN 24-May-23 10:56 nucliadb/train/tests/test_get_entities.py
+-rw-r--r--  2.0 unx     1876 b- defN 24-May-23 10:56 nucliadb/train/tests/test_get_info.py
+-rw-r--r--  2.0 unx     1382 b- defN 24-May-23 10:56 nucliadb/train/tests/test_get_ontology.py
+-rw-r--r--  2.0 unx     2417 b- defN 24-May-23 10:56 nucliadb/train/tests/test_get_ontology_count.py
+-rw-r--r--  2.0 unx     7669 b- defN 24-May-23 10:56 nucliadb/train/tests/test_image_classification.py
+-rw-r--r--  2.0 unx     1416 b- defN 24-May-23 10:56 nucliadb/train/tests/test_list_fields.py
+-rw-r--r--  2.0 unx     2944 b- defN 24-May-23 10:56 nucliadb/train/tests/test_list_paragraphs.py
+-rw-r--r--  2.0 unx     1423 b- defN 24-May-23 10:56 nucliadb/train/tests/test_list_resources.py
+-rw-r--r--  2.0 unx     2947 b- defN 24-May-23 10:56 nucliadb/train/tests/test_list_sentences.py
+-rw-r--r--  2.0 unx     4645 b- defN 24-May-23 10:56 nucliadb/train/tests/test_paragraph_classification.py
+-rw-r--r--  2.0 unx     4320 b- defN 24-May-23 10:56 nucliadb/train/tests/test_paragraph_streaming.py
+-rw-r--r--  2.0 unx     8751 b- defN 24-May-23 10:56 nucliadb/train/tests/test_question_answer_streaming.py
+-rw-r--r--  2.0 unx     5051 b- defN 24-May-23 10:56 nucliadb/train/tests/test_sentence_classification.py
+-rw-r--r--  2.0 unx     5583 b- defN 24-May-23 10:56 nucliadb/train/tests/test_token_classification.py
+-rw-r--r--  2.0 unx     3324 b- defN 24-May-23 10:56 nucliadb/train/tests/utils.py
+-rw-r--r--  2.0 unx     1328 b- defN 24-May-23 10:56 nucliadb/writer/__init__.py
+-rw-r--r--  2.0 unx     4268 b- defN 24-May-23 10:56 nucliadb/writer/app.py
+-rw-r--r--  2.0 unx    19483 b- defN 24-May-23 10:56 nucliadb/writer/back_pressure.py
+-rw-r--r--  2.0 unx      972 b- defN 24-May-23 10:56 nucliadb/writer/exceptions.py
+-rw-r--r--  2.0 unx     1953 b- defN 24-May-23 10:56 nucliadb/writer/lifecycle.py
+-rw-r--r--  2.0 unx     1032 b- defN 24-May-23 10:56 nucliadb/writer/openapi.py
+-rw-r--r--  2.0 unx     1448 b- defN 24-May-23 10:56 nucliadb/writer/run.py
+-rw-r--r--  2.0 unx     3103 b- defN 24-May-23 10:56 nucliadb/writer/settings.py
+-rw-r--r--  2.0 unx     1036 b- defN 24-May-23 10:56 nucliadb/writer/utilities.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-23 10:56 nucliadb/writer/api/__init__.py
+-rw-r--r--  2.0 unx     1429 b- defN 24-May-23 10:56 nucliadb/writer/api/constants.py
+-rw-r--r--  2.0 unx     1095 b- defN 24-May-23 10:56 nucliadb/writer/api/v1/__init__.py
+-rw-r--r--  2.0 unx     6571 b- defN 24-May-23 10:56 nucliadb/writer/api/v1/export_import.py
+-rw-r--r--  2.0 unx    24482 b- defN 24-May-23 10:56 nucliadb/writer/api/v1/field.py
+-rw-r--r--  2.0 unx     5248 b- defN 24-May-23 10:56 nucliadb/writer/api/v1/knowledgebox.py
+-rw-r--r--  2.0 unx     2058 b- defN 24-May-23 10:56 nucliadb/writer/api/v1/learning_config.py
+-rw-r--r--  2.0 unx    18893 b- defN 24-May-23 10:56 nucliadb/writer/api/v1/resource.py
+-rw-r--r--  2.0 unx     1034 b- defN 24-May-23 10:56 nucliadb/writer/api/v1/router.py
+-rw-r--r--  2.0 unx    10216 b- defN 24-May-23 10:56 nucliadb/writer/api/v1/services.py
+-rw-r--r--  2.0 unx    30857 b- defN 24-May-23 10:56 nucliadb/writer/api/v1/upload.py
+-rw-r--r--  2.0 unx     1612 b- defN 24-May-23 10:56 nucliadb/writer/layouts/__init__.py
+-rw-r--r--  2.0 unx     2115 b- defN 24-May-23 10:56 nucliadb/writer/layouts/v1.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-23 10:56 nucliadb/writer/resource/__init__.py
+-rw-r--r--  2.0 unx     1425 b- defN 24-May-23 10:56 nucliadb/writer/resource/audit.py
+-rw-r--r--  2.0 unx    10968 b- defN 24-May-23 10:56 nucliadb/writer/resource/basic.py
+-rw-r--r--  2.0 unx    16740 b- defN 24-May-23 10:56 nucliadb/writer/resource/field.py
+-rw-r--r--  2.0 unx     2022 b- defN 24-May-23 10:56 nucliadb/writer/resource/origin.py
+-rw-r--r--  2.0 unx     1093 b- defN 24-May-23 10:56 nucliadb/writer/resource/slug.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-23 10:56 nucliadb/writer/tests/__init__.py
+-rw-r--r--  2.0 unx     1200 b- defN 24-May-23 10:56 nucliadb/writer/tests/conftest.py
+-rw-r--r--  2.0 unx     5971 b- defN 24-May-23 10:56 nucliadb/writer/tests/fixtures.py
+-rw-r--r--  2.0 unx    15472 b- defN 24-May-23 10:56 nucliadb/writer/tests/test_fields.py
+-rw-r--r--  2.0 unx    25999 b- defN 24-May-23 10:56 nucliadb/writer/tests/test_files.py
+-rw-r--r--  2.0 unx     1729 b- defN 24-May-23 10:56 nucliadb/writer/tests/test_knowledgebox.py
+-rw-r--r--  2.0 unx     4358 b- defN 24-May-23 10:56 nucliadb/writer/tests/test_reprocess_file_field.py
+-rw-r--r--  2.0 unx    16694 b- defN 24-May-23 10:56 nucliadb/writer/tests/test_resources.py
+-rw-r--r--  2.0 unx     5120 b- defN 24-May-23 10:56 nucliadb/writer/tests/test_service.py
+-rw-r--r--  2.0 unx     6054 b- defN 24-May-23 10:56 nucliadb/writer/tests/test_tus.py
+-rw-r--r--  2.0 unx     1287 b- defN 24-May-23 10:56 nucliadb/writer/tests/utils.py
+-rw-r--r--  2.0 unx     5226 b- defN 24-May-23 10:56 nucliadb/writer/tus/__init__.py
+-rw-r--r--  2.0 unx     5082 b- defN 24-May-23 10:56 nucliadb/writer/tus/dm.py
+-rw-r--r--  2.0 unx     2186 b- defN 24-May-23 10:56 nucliadb/writer/tus/exceptions.py
+-rw-r--r--  2.0 unx    14527 b- defN 24-May-23 10:56 nucliadb/writer/tus/gcs.py
+-rw-r--r--  2.0 unx     5849 b- defN 24-May-23 10:56 nucliadb/writer/tus/local.py
+-rw-r--r--  2.0 unx     4367 b- defN 24-May-23 10:56 nucliadb/writer/tus/pg.py
+-rw-r--r--  2.0 unx     9069 b- defN 24-May-23 10:56 nucliadb/writer/tus/s3.py
+-rw-r--r--  2.0 unx     4734 b- defN 24-May-23 10:56 nucliadb/writer/tus/storage.py
+-rw-r--r--  2.0 unx     2556 b- defN 24-May-23 10:56 nucliadb/writer/tus/utils.py
+-rw-r--r--  2.0 unx     4423 b- defN 24-May-23 10:57 nucliadb-4.0.0.post539.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-23 10:57 nucliadb-4.0.0.post539.dist-info/WHEEL
+-rw-r--r--  2.0 unx     1268 b- defN 24-May-23 10:57 nucliadb-4.0.0.post539.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       20 b- defN 24-May-23 10:57 nucliadb-4.0.0.post539.dist-info/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 24-May-23 10:57 nucliadb-4.0.0.post539.dist-info/zip-safe
+-rw-rw-r--  2.0 unx    43360 b- defN 24-May-23 10:57 nucliadb-4.0.0.post539.dist-info/RECORD
+462 files, 2259836 bytes uncompressed, 695874 bytes compressed:  69.2%
```

## zipnote {}

```diff
@@ -1362,26 +1362,26 @@
 
 Filename: nucliadb/writer/tus/storage.py
 Comment: 
 
 Filename: nucliadb/writer/tus/utils.py
 Comment: 
 
-Filename: nucliadb-4.0.0.post538.dist-info/METADATA
+Filename: nucliadb-4.0.0.post539.dist-info/METADATA
 Comment: 
 
-Filename: nucliadb-4.0.0.post538.dist-info/WHEEL
+Filename: nucliadb-4.0.0.post539.dist-info/WHEEL
 Comment: 
 
-Filename: nucliadb-4.0.0.post538.dist-info/entry_points.txt
+Filename: nucliadb-4.0.0.post539.dist-info/entry_points.txt
 Comment: 
 
-Filename: nucliadb-4.0.0.post538.dist-info/top_level.txt
+Filename: nucliadb-4.0.0.post539.dist-info/top_level.txt
 Comment: 
 
-Filename: nucliadb-4.0.0.post538.dist-info/zip-safe
+Filename: nucliadb-4.0.0.post539.dist-info/zip-safe
 Comment: 
 
-Filename: nucliadb-4.0.0.post538.dist-info/RECORD
+Filename: nucliadb-4.0.0.post539.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## nucliadb/common/datamanagers/resources.py

```diff
@@ -24,45 +24,205 @@
 from nucliadb.common.datamanagers.utils import get_kv_pb
 from nucliadb.common.maindb.driver import Transaction
 from nucliadb.common.maindb.exceptions import ConflictError, NotFoundError
 
 # These should be refactored
 from nucliadb.ingest.orm.resource import KB_RESOURCE_SLUG, KB_RESOURCE_SLUG_BASE
 from nucliadb.ingest.orm.resource import Resource as ResourceORM
-from nucliadb.ingest.orm.utils import get_basic, set_basic
+from nucliadb.ingest.settings import settings as ingest_settings
 from nucliadb_protos import noderesources_pb2, resources_pb2, writer_pb2
 from nucliadb_utils.utilities import get_storage
 
 from .utils import with_transaction
 
-KB_MATERIALIZED_RESOURCES_COUNT = "/kbs/{kbid}/materialized/resources/count"
+KB_RESOURCE_BASIC = "/kbs/{kbid}/r/{uuid}"
+KB_RESOURCE_BASIC_FS = "/kbs/{kbid}/r/{uuid}/basic"  # Only used on FS driver
+KB_RESOURCE_ORIGIN = "/kbs/{kbid}/r/{uuid}/origin"
+KB_RESOURCE_EXTRA = "/kbs/{kbid}/r/{uuid}/extra"
+KB_RESOURCE_SECURITY = "/kbs/{kbid}/r/{uuid}/security"
+KB_RESOURCE_RELATIONS = "/kbs/{kbid}/r/{uuid}/relations"
+
 KB_RESOURCE_SHARD = "/kbs/{kbid}/r/{uuid}/shard"
+
 KB_RESOURCE_ALL_FIELDS = "/kbs/{kbid}/r/{uuid}/allfields"
+KB_MATERIALIZED_RESOURCES_COUNT = "/kbs/{kbid}/materialized/resources/count"
 
 
-@backoff.on_exception(
-    backoff.expo, (Exception,), jitter=backoff.random_jitter, max_tries=3
-)
-async def _iter_resource_slugs(*, kbid: str) -> AsyncGenerator[str, None]:
-    async with with_transaction() as txn:
-        async for key in txn.keys(
-            match=KB_RESOURCE_SLUG_BASE.format(kbid=kbid), count=-1
-        ):
-            yield key.split("/")[-1]
+async def resource_exists(txn: Transaction, *, kbid: str, rid: str) -> bool:
+    basic = await get_basic_raw(txn, kbid=kbid, rid=rid)
+    return basic is not None
+
+
+# id and slug
+
+
+async def get_resource_uuid_from_slug(
+    txn: Transaction, *, kbid: str, slug: str
+) -> Optional[str]:
+    encoded_uuid = await txn.get(KB_RESOURCE_SLUG.format(kbid=kbid, slug=slug))
+    if not encoded_uuid:
+        return None
+    return encoded_uuid.decode()
+
+
+async def slug_exists(txn: Transaction, *, kbid: str, slug: str) -> bool:
+    key = KB_RESOURCE_SLUG.format(kbid=kbid, slug=slug)
+    encoded_slug: Optional[bytes] = await txn.get(key)
+    return encoded_slug not in (None, b"")
+
+
+async def modify_slug(txn: Transaction, *, kbid: str, rid: str, new_slug: str) -> str:
+    basic = await get_basic(txn, kbid=kbid, rid=rid)
+    if basic is None:
+        raise NotFoundError()
+    old_slug = basic.slug
+
+    uuid_for_new_slug = await get_resource_uuid_from_slug(txn, kbid=kbid, slug=new_slug)
+    if uuid_for_new_slug is not None:
+        if uuid_for_new_slug == rid:
+            # Nothing to change
+            return old_slug
+        else:
+            raise ConflictError(f"Slug {new_slug} already exists")
+    key = KB_RESOURCE_SLUG.format(kbid=kbid, slug=old_slug)
+    await txn.delete(key)
+    key = KB_RESOURCE_SLUG.format(kbid=kbid, slug=new_slug)
+    await txn.set(key, rid.encode())
+    basic.slug = new_slug
+    await set_basic(txn, kbid=kbid, rid=rid, basic=basic)
+    return old_slug
+
+
+# resource-shard
 
 
 @backoff.on_exception(
     backoff.expo, (Exception,), jitter=backoff.random_jitter, max_tries=3
 )
-async def _get_resource_ids_from_slugs(kbid: str, slugs: list[str]) -> list[str]:
-    async with with_transaction() as txn:
-        rids = await txn.batch_get(
-            [KB_RESOURCE_SLUG.format(kbid=kbid, slug=slug) for slug in slugs]
+async def get_resource_shard_id(
+    txn: Transaction, *, kbid: str, rid: str
+) -> Optional[str]:
+    shard = await txn.get(KB_RESOURCE_SHARD.format(kbid=kbid, uuid=rid))
+    if shard is not None:
+        return shard.decode()
+    else:
+        return None
+
+
+async def set_resource_shard_id(txn: Transaction, *, kbid: str, rid: str, shard: str):
+    await txn.set(KB_RESOURCE_SHARD.format(kbid=kbid, uuid=rid), shard.encode())
+
+
+# Basic
+
+
+async def get_basic(
+    txn: Transaction, *, kbid: str, rid: str
+) -> Optional[resources_pb2.Basic]:
+    raw = await get_basic_raw(txn, kbid=kbid, rid=rid)
+    if raw is None:
+        return None
+    basic = resources_pb2.Basic()
+    basic.ParseFromString(raw)
+    return basic
+
+
+async def get_basic_raw(txn: Transaction, *, kbid: str, rid: str) -> Optional[bytes]:
+    if ingest_settings.driver == "local":
+        raw_basic = await txn.get(KB_RESOURCE_BASIC_FS.format(kbid=kbid, uuid=rid))
+    else:
+        raw_basic = await txn.get(KB_RESOURCE_BASIC.format(kbid=kbid, uuid=rid))
+    return raw_basic
+
+
+async def set_basic(
+    txn: Transaction, *, kbid: str, rid: str, basic: resources_pb2.Basic
+):
+    if ingest_settings.driver == "local":
+        await txn.set(
+            KB_RESOURCE_BASIC_FS.format(kbid=kbid, uuid=rid),
+            basic.SerializeToString(),
         )
-    return [rid.decode() for rid in rids if rid is not None]
+    else:
+        await txn.set(
+            KB_RESOURCE_BASIC.format(kbid=kbid, uuid=rid),
+            basic.SerializeToString(),
+        )
+
+
+# Origin
+
+
+async def get_origin(
+    txn: Transaction, *, kbid: str, rid: str
+) -> Optional[resources_pb2.Origin]:
+    key = KB_RESOURCE_ORIGIN.format(kbid=kbid, uuid=rid)
+    return await get_kv_pb(txn, key, resources_pb2.Origin)
+
+
+async def set_origin(
+    txn: Transaction, *, kbid: str, rid: str, origin: resources_pb2.Origin
+):
+    key = KB_RESOURCE_ORIGIN.format(kbid=kbid, uuid=rid)
+    await txn.set(key, origin.SerializeToString())
+
+
+# Extra
+
+
+async def get_extra(
+    txn: Transaction, *, kbid: str, rid: str
+) -> Optional[resources_pb2.Extra]:
+    key = KB_RESOURCE_EXTRA.format(kbid=kbid, uuid=rid)
+    return await get_kv_pb(txn, key, resources_pb2.Extra)
+
+
+async def set_extra(
+    txn: Transaction, *, kbid: str, rid: str, extra: resources_pb2.Extra
+):
+    key = KB_RESOURCE_EXTRA.format(kbid=kbid, uuid=rid)
+    await txn.set(key, extra.SerializeToString())
+
+
+# Security
+
+
+async def get_security(
+    txn: Transaction, *, kbid: str, rid: str
+) -> Optional[resources_pb2.Security]:
+    key = KB_RESOURCE_SECURITY.format(kbid=kbid, uuid=rid)
+    return await get_kv_pb(txn, key, resources_pb2.Security)
+
+
+async def set_security(
+    txn: Transaction, *, kbid: str, rid: str, security: resources_pb2.Security
+):
+    key = KB_RESOURCE_SECURITY.format(kbid=kbid, uuid=rid)
+    await txn.set(key, security.SerializeToString())
+
+
+# Relations
+
+
+async def get_relations(
+    txn: Transaction, *, kbid: str, rid: str
+) -> Optional[resources_pb2.Relations]:
+    key = KB_RESOURCE_RELATIONS.format(kbid=kbid, uuid=rid)
+    return await get_kv_pb(txn, key, resources_pb2.Relations)
+
+
+async def set_relations(
+    txn: Transaction, *, kbid: str, rid: str, relations: resources_pb2.Relations
+):
+    key = KB_RESOURCE_RELATIONS.format(kbid=kbid, uuid=rid)
+    await txn.set(key, relations.SerializeToString())
+
+
+# KB resource ids (this functions use internal transactions, breaking the
+# datamanager contract. We should rethink them at some point)
 
 
 async def iterate_resource_ids(*, kbid: str) -> AsyncGenerator[str, None]:
     """
     Currently, the implementation of this is optimizing for reducing
     how long a transaction will be open since the caller controls
     how long each item that is yielded will be processed.
@@ -80,62 +240,34 @@
         for rid in await _get_resource_ids_from_slugs(kbid=kbid, slugs=batch):
             yield rid
 
 
 @backoff.on_exception(
     backoff.expo, (Exception,), jitter=backoff.random_jitter, max_tries=3
 )
-async def get_resource_shard_id(
-    txn: Transaction, *, kbid: str, rid: str
-) -> Optional[str]:
-    shard = await txn.get(KB_RESOURCE_SHARD.format(kbid=kbid, uuid=rid))
-    if shard is not None:
-        return shard.decode()
-    else:
-        return None
+async def _iter_resource_slugs(*, kbid: str) -> AsyncGenerator[str, None]:
+    async with with_transaction() as txn:
+        async for key in txn.keys(
+            match=KB_RESOURCE_SLUG_BASE.format(kbid=kbid), count=-1
+        ):
+            yield key.split("/")[-1]
 
 
 @backoff.on_exception(
     backoff.expo, (Exception,), jitter=backoff.random_jitter, max_tries=3
 )
-async def get_resource(
-    txn: Transaction, *, kbid: str, rid: str
-) -> Optional[ResourceORM]:
-    """
-    Not ideal to return Resource type here but refactoring would
-    require a lot of changes.
-
-    At least this isolated that dependency here.
-    """
-    # prevent circulat imports -- this is not ideal that we have the ORM mix here.
-    from nucliadb.ingest.orm.knowledgebox import KnowledgeBox as KnowledgeBoxORM
-
-    kb_orm = KnowledgeBoxORM(txn, await get_storage(), kbid)
-    return await kb_orm.get(rid)
-
-
-async def resource_exists(txn: Transaction, *, kbid: str, rid: str) -> bool:
-    basic = await get_basic(txn, kbid, rid)
-    return basic is not None
-
+async def _get_resource_ids_from_slugs(kbid: str, slugs: list[str]) -> list[str]:
+    async with with_transaction() as txn:
+        rids = await txn.batch_get(
+            [KB_RESOURCE_SLUG.format(kbid=kbid, slug=slug) for slug in slugs]
+        )
+    return [rid.decode() for rid in rids if rid is not None]
 
-@backoff.on_exception(
-    backoff.expo, (Exception,), jitter=backoff.random_jitter, max_tries=3
-)
-async def get_resource_index_message(
-    txn: Transaction, *, kbid: str, rid: str
-) -> Optional[noderesources_pb2.Resource]:
-    # prevent circulat imports -- this is not ideal that we have the ORM mix here.
-    from nucliadb.ingest.orm.knowledgebox import KnowledgeBox as KnowledgeBoxORM
 
-    kb_orm = KnowledgeBoxORM(txn, await get_storage(), kbid)
-    res = await kb_orm.get(rid)
-    if res is None:
-        return None
-    return (await res.generate_index_message()).brain
+# KB resource count (materialized key)
 
 
 async def calculate_number_of_resources(txn: Transaction, *, kbid: str) -> int:
     """
     Calculate the number of resources in a knowledgebox.
 
     This is usually not very fast at all.
@@ -164,71 +296,15 @@
 
 async def set_number_of_resources(txn: Transaction, kbid: str, value: int) -> None:
     await txn.set(
         KB_MATERIALIZED_RESOURCES_COUNT.format(kbid=kbid), str(value).encode()
     )
 
 
-async def get_broker_message(
-    txn: Transaction, *, kbid: str, rid: str
-) -> Optional[writer_pb2.BrokerMessage]:
-    resource = await get_resource(txn, kbid=kbid, rid=rid)
-    if resource is None:
-        return None
-
-    resource.disable_vectors = False
-    resource.txn = txn
-    bm = await resource.generate_broker_message()
-    return bm
-
-
-async def get_resource_basic(
-    txn: Transaction, *, kbid: str, rid: str
-) -> Optional[resources_pb2.Basic]:
-    raw_basic = await get_basic(txn, kbid, rid)
-    if not raw_basic:
-        return None
-    basic = resources_pb2.Basic()
-    basic.ParseFromString(raw_basic)
-    return basic
-
-
-async def get_resource_uuid_from_slug(
-    txn: Transaction, *, kbid: str, slug: str
-) -> Optional[str]:
-    encoded_uuid = await txn.get(KB_RESOURCE_SLUG.format(kbid=kbid, slug=slug))
-    if not encoded_uuid:
-        return None
-    return encoded_uuid.decode()
-
-
-async def modify_slug(txn: Transaction, *, kbid: str, rid: str, new_slug: str) -> str:
-    basic = await get_resource_basic(txn, kbid=kbid, rid=rid)
-    if basic is None:
-        raise NotFoundError()
-    old_slug = basic.slug
-
-    uuid_for_new_slug = await get_resource_uuid_from_slug(txn, kbid=kbid, slug=new_slug)
-    if uuid_for_new_slug is not None:
-        if uuid_for_new_slug == rid:
-            # Nothing to change
-            return old_slug
-        else:
-            raise ConflictError(f"Slug {new_slug} already exists")
-    key = KB_RESOURCE_SLUG.format(kbid=kbid, slug=old_slug)
-    await txn.delete(key)
-    key = KB_RESOURCE_SLUG.format(kbid=kbid, slug=new_slug)
-    await txn.set(key, rid.encode())
-    basic.slug = new_slug
-    await set_basic(txn, kbid, rid, basic)
-    return old_slug
-
-
-async def set_resource_shard_id(txn: Transaction, *, kbid: str, rid: str, shard: str):
-    await txn.set(KB_RESOURCE_SHARD.format(kbid=kbid, uuid=rid), shard.encode())
+# Fields (materialized key with all field ids)
 
 
 async def get_all_field_ids(
     txn: Transaction, *, kbid: str, rid: str
 ) -> Optional[resources_pb2.AllFieldIDs]:
     key = KB_RESOURCE_ALL_FIELDS.format(kbid=kbid, uuid=rid)
     return await get_kv_pb(txn, key, resources_pb2.AllFieldIDs)
@@ -247,7 +323,58 @@
     fields = await get_all_field_ids(txn, kbid=kbid, rid=rid)
     if fields is None:
         return False
     for resource_field_id in fields.fields:
         if field_id == resource_field_id:
             return True
     return False
+
+
+# ORM mix (this functions shouldn't belong here)
+
+
+async def get_broker_message(
+    txn: Transaction, *, kbid: str, rid: str
+) -> Optional[writer_pb2.BrokerMessage]:
+    resource = await get_resource(txn, kbid=kbid, rid=rid)
+    if resource is None:
+        return None
+
+    resource.disable_vectors = False
+    resource.txn = txn
+    bm = await resource.generate_broker_message()
+    return bm
+
+
+@backoff.on_exception(
+    backoff.expo, (Exception,), jitter=backoff.random_jitter, max_tries=3
+)
+async def get_resource(
+    txn: Transaction, *, kbid: str, rid: str
+) -> Optional[ResourceORM]:
+    """
+    Not ideal to return Resource type here but refactoring would
+    require a lot of changes.
+
+    At least this isolated that dependency here.
+    """
+    # prevent circulat imports -- this is not ideal that we have the ORM mix here.
+    from nucliadb.ingest.orm.knowledgebox import KnowledgeBox as KnowledgeBoxORM
+
+    kb_orm = KnowledgeBoxORM(txn, await get_storage(), kbid)
+    return await kb_orm.get(rid)
+
+
+@backoff.on_exception(
+    backoff.expo, (Exception,), jitter=backoff.random_jitter, max_tries=3
+)
+async def get_resource_index_message(
+    txn: Transaction, *, kbid: str, rid: str
+) -> Optional[noderesources_pb2.Resource]:
+    # prevent circulat imports -- this is not ideal that we have the ORM mix here.
+    from nucliadb.ingest.orm.knowledgebox import KnowledgeBox as KnowledgeBoxORM
+
+    kb_orm = KnowledgeBoxORM(txn, await get_storage(), kbid)
+    res = await kb_orm.get(rid)
+    if res is None:
+        return None
+    return (await res.generate_index_message()).brain
```

## nucliadb/ingest/orm/knowledgebox.py

```diff
@@ -40,20 +40,15 @@
 from nucliadb.ingest import SERVICE_NAME, logger
 from nucliadb.ingest.orm.exceptions import KnowledgeBoxConflict
 from nucliadb.ingest.orm.resource import (
     KB_RESOURCE_SLUG,
     KB_RESOURCE_SLUG_BASE,
     Resource,
 )
-from nucliadb.ingest.orm.utils import (
-    choose_matryoshka_dimension,
-    compute_paragraph_key,
-    get_basic,
-    set_basic,
-)
+from nucliadb.ingest.orm.utils import choose_matryoshka_dimension, compute_paragraph_key
 from nucliadb.migrator.utils import get_latest_version
 from nucliadb_protos import writer_pb2
 from nucliadb_utils.storages.storage import Storage
 from nucliadb_utils.utilities import get_audit, get_storage
 
 # XXX Eventually all these keys should be moved to datamanagers.kb
 KB_RESOURCE = "/kbs/{kbid}/r/{uuid}"
@@ -331,33 +326,32 @@
                 return None
         for shard in pb.shards:
             if shard.shard == shard_id:
                 return shard
         return None
 
     async def get(self, uuid: str) -> Optional[Resource]:
-        raw_basic = await get_basic(self.txn, self.kbid, uuid)
-        if raw_basic:
-            return Resource(
-                txn=self.txn,
-                storage=self.storage,
-                kb=self,
-                uuid=uuid,
-                basic=Resource.parse_basic(raw_basic),
-                disable_vectors=False,
-            )
-        else:
+        basic = await datamanagers.resources.get_basic(
+            self.txn, kbid=self.kbid, rid=uuid
+        )
+        if basic is None:
             return None
+        return Resource(
+            txn=self.txn,
+            storage=self.storage,
+            kb=self,
+            uuid=uuid,
+            basic=basic,
+            disable_vectors=False,
+        )
 
     async def delete_resource(self, uuid: str):
-        raw_basic = await get_basic(self.txn, self.kbid, uuid)
-        if raw_basic:
-            basic = Resource.parse_basic(raw_basic)
-        else:
-            basic = None
+        basic = await datamanagers.resources.get_basic(
+            self.txn, kbid=self.kbid, rid=uuid
+        )
 
         async for key in self.txn.keys(
             KB_RESOURCE.format(kbid=self.kbid, uuid=uuid), count=-1
         ):
             await self.txn.delete(key)
 
         if basic and basic.slug:
@@ -366,51 +360,43 @@
                 await self.txn.delete(slug_key)
             except Exception:
                 pass
 
         await self.storage.delete_resource(self.kbid, uuid)
 
     async def get_resource_uuid_by_slug(self, slug: str) -> Optional[str]:
-        uuid = await self.txn.get(KB_RESOURCE_SLUG.format(kbid=self.kbid, slug=slug))
-        if uuid is not None:
-            return uuid.decode()
-        else:
-            return None
+        return await datamanagers.resources.get_resource_uuid_from_slug(
+            self.txn, kbid=self.kbid, slug=slug
+        )
 
     async def get_unique_slug(self, uuid: str, slug: str) -> str:
         key = KB_RESOURCE_SLUG.format(kbid=self.kbid, slug=slug)
         key_ok = False
         while key_ok is False:
             found = await self.txn.get(key)
             if found and found.decode() != uuid:
                 slug += ".c"
                 key = KB_RESOURCE_SLUG.format(kbid=self.kbid, slug=slug)
             else:
                 key_ok = True
         return slug
 
-    @classmethod
-    async def resource_slug_exists(
-        self, txn: Transaction, kbid: str, slug: str
-    ) -> bool:
-        key = KB_RESOURCE_SLUG.format(kbid=kbid, slug=slug)
-        encoded_slug: Optional[bytes] = await txn.get(key)
-        return encoded_slug not in (None, b"")
-
     async def add_resource(
         self, uuid: str, slug: str, basic: Optional[Basic] = None
     ) -> Resource:
         if basic is None:
             basic = Basic()
         if slug == "":
             slug = uuid
         slug = await self.get_unique_slug(uuid, slug)
         basic.slug = slug
         fix_paragraph_annotation_keys(uuid, basic)
-        await set_basic(self.txn, self.kbid, uuid, basic)
+        await datamanagers.resources.set_basic(
+            self.txn, kbid=self.kbid, rid=uuid, basic=basic
+        )
         return Resource(
             storage=self.storage,
             txn=self.txn,
             kb=self,
             uuid=uuid,
             basic=basic,
             disable_vectors=False,
```

## nucliadb/ingest/orm/resource.py

```diff
@@ -71,29 +71,24 @@
 from nucliadb.ingest.fields.generic import VALID_GENERIC_FIELDS, Generic
 from nucliadb.ingest.fields.keywordset import Keywordset
 from nucliadb.ingest.fields.layout import Layout
 from nucliadb.ingest.fields.link import Link
 from nucliadb.ingest.fields.text import Text
 from nucliadb.ingest.orm.brain import FilePagePositions, ResourceBrain
 from nucliadb.ingest.orm.metrics import processor_observer
-from nucliadb.ingest.orm.utils import get_basic, set_basic
 from nucliadb_models.common import CloudLink
 from nucliadb_models.writer import GENERIC_MIME_TYPE
 from nucliadb_protos import utils_pb2, writer_pb2
 from nucliadb_utils.storages.storage import Storage
 
 if TYPE_CHECKING:  # pragma: no cover
     from nucliadb.ingest.orm.knowledgebox import KnowledgeBox
 
 logger = logging.getLogger(__name__)
 
-KB_RESOURCE_ORIGIN = "/kbs/{kbid}/r/{uuid}/origin"
-KB_RESOURCE_EXTRA = "/kbs/{kbid}/r/{uuid}/extra"
-KB_RESOURCE_SECURITY = "/kbs/{kbid}/r/{uuid}/security"
-KB_RESOURCE_RELATIONS = "/kbs/{kbid}/r/{uuid}/relations"
 KB_RESOURCE_FIELDS = "/kbs/{kbid}/r/{uuid}/f/"
 KB_RESOURCE_SLUG_BASE = "/kbs/{kbid}/s/"
 KB_RESOURCE_SLUG = f"{KB_RESOURCE_SLUG_BASE}{{slug}}"
 KB_FIELDS: dict[int, Type] = {
     FieldType.LAYOUT: Layout,
     FieldType.TEXT: Text,
     FieldType.FILE: File,
@@ -171,40 +166,21 @@
         self._indexer = indexer
 
     async def set_slug(self):
         basic = await self.get_basic()
         new_key = KB_RESOURCE_SLUG.format(kbid=self.kb.kbid, slug=basic.slug)
         await self.txn.set(new_key, self.uuid.encode())
 
-    @staticmethod
-    def parse_basic(payload: bytes) -> PBBasic:
-        pb = PBBasic()
-        if payload is None:
-            return None
-
-        pb.ParseFromString(payload)
-        return pb
-
-    async def exists(self) -> bool:
-        exists = True
-        if self.basic is None:
-            payload = await get_basic(self.txn, self.kb.kbid, self.uuid)
-            if payload is not None:
-                pb = PBBasic()
-                pb.ParseFromString(payload)
-                self.basic = pb
-            else:
-                exists = False
-        return exists
-
     # Basic
     async def get_basic(self) -> Optional[PBBasic]:
         if self.basic is None:
-            payload = await get_basic(self.txn, self.kb.kbid, self.uuid)
-            self.basic = self.parse_basic(payload) if payload is not None else PBBasic()
+            basic = await datamanagers.resources.get_basic(
+                self.txn, kbid=self.kb.kbid, rid=self.uuid
+            )
+            self.basic = basic if basic is not None else PBBasic()
         return self.basic
 
     def set_processing_status(self, current_basic: PBBasic, basic_in_payload: PBBasic):
         self._previous_status = current_basic.metadata.status
         if basic_in_payload.HasField("metadata") and basic_in_payload.metadata.useful:
             current_basic.metadata.status = basic_in_payload.metadata.status
 
@@ -276,102 +252,82 @@
                         )
 
         # Some basic fields are computed off field metadata.
         # This means we need to recompute upon field deletions.
         if deleted_fields is not None and len(deleted_fields) > 0:
             remove_field_classifications(self.basic, deleted_fields=deleted_fields)
 
-        await set_basic(self.txn, self.kb.kbid, self.uuid, self.basic)
+        await datamanagers.resources.set_basic(
+            self.txn, kbid=self.kb.kbid, rid=self.uuid, basic=self.basic
+        )
         self.modified = True
 
     # Origin
     async def get_origin(self) -> Optional[PBOrigin]:
         if self.origin is None:
-            pb = PBOrigin()
-            payload = await self.txn.get(
-                KB_RESOURCE_ORIGIN.format(kbid=self.kb.kbid, uuid=self.uuid)
+            origin = await datamanagers.resources.get_origin(
+                self.txn, kbid=self.kb.kbid, rid=self.uuid
             )
-            if payload is None:
-                return None
-
-            pb.ParseFromString(payload)
-            self.origin = pb
+            self.origin = origin
         return self.origin
 
     async def set_origin(self, payload: PBOrigin):
-        await self.txn.set(
-            KB_RESOURCE_ORIGIN.format(kbid=self.kb.kbid, uuid=self.uuid),
-            payload.SerializeToString(),
+        await datamanagers.resources.set_origin(
+            self.txn, kbid=self.kb.kbid, rid=self.uuid, origin=payload
         )
         self.modified = True
         self.origin = payload
 
     # Extra
     async def get_extra(self) -> Optional[PBExtra]:
         if self.extra is None:
-            pb = PBExtra()
-            payload = await self.txn.get(
-                KB_RESOURCE_EXTRA.format(kbid=self.kb.kbid, uuid=self.uuid)
+            extra = await datamanagers.resources.get_extra(
+                self.txn, kbid=self.kb.kbid, rid=self.uuid
             )
-            if payload is None:
-                return None
-            pb.ParseFromString(payload)
-            self.extra = pb
+            self.extra = extra
         return self.extra
 
     async def set_extra(self, payload: PBExtra):
-        key = KB_RESOURCE_EXTRA.format(kbid=self.kb.kbid, uuid=self.uuid)
-        await self.txn.set(
-            key,
-            payload.SerializeToString(),
+        await datamanagers.resources.set_extra(
+            self.txn, kbid=self.kb.kbid, rid=self.uuid, extra=payload
         )
         self.modified = True
         self.extra = payload
 
     # Security
     async def get_security(self) -> Optional[utils_pb2.Security]:
         if self.security is None:
-            pb = utils_pb2.Security()
-            key = KB_RESOURCE_SECURITY.format(kbid=self.kb.kbid, uuid=self.uuid)
-            payload = await self.txn.get(key)
-            if payload is None:
-                return None
-            pb.ParseFromString(payload)
-            self.security = pb
+            security = await datamanagers.resources.get_security(
+                self.txn, kbid=self.kb.kbid, rid=self.uuid
+            )
+            self.security = security
         return self.security
 
     async def set_security(self, payload: utils_pb2.Security) -> None:
-        key = KB_RESOURCE_SECURITY.format(kbid=self.kb.kbid, uuid=self.uuid)
-        await self.txn.set(
-            key,
-            payload.SerializeToString(),
+        await datamanagers.resources.set_security(
+            self.txn, kbid=self.kb.kbid, rid=self.uuid, security=payload
         )
         self.modified = True
         self.security = payload
 
     # Relations
     async def get_relations(self) -> Optional[PBRelations]:
         if self.relations is None:
-            pb = PBRelations()
-            payload = await self.txn.get(
-                KB_RESOURCE_RELATIONS.format(kbid=self.kb.kbid, uuid=self.uuid)
+            relations = await datamanagers.resources.get_relations(
+                self.txn, kbid=self.kb.kbid, rid=self.uuid
             )
-            if payload is None:
-                return None
-            pb.ParseFromString(payload)
-            self.relations = pb
+            self.relations = relations
         return self.relations
 
     async def set_relations(self, payload: list[PBRelation]):
         relations = PBRelations()
         for relation in payload:
             relations.relations.append(relation)
-        await self.txn.set(
-            KB_RESOURCE_RELATIONS.format(kbid=self.kb.kbid, uuid=self.uuid),
-            relations.SerializeToString(),
+        await datamanagers.resources.set_relations(
+            self.txn, kbid=self.kb.kbid, rid=self.uuid, relations=relations
         )
         self.modified = True
         self.relations = relations
 
     @processor_observer.wrap({"type": "generate_index_message"})
     async def generate_index_message(self) -> ResourceBrain:
         brain = ResourceBrain(rid=self.uuid)
```

## nucliadb/ingest/orm/utils.py

```diff
@@ -14,55 +14,27 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 import urllib.parse
-from typing import Optional
 
 from nucliadb_protos.resources_pb2 import (
-    Basic,
     ExtractedTextWrapper,
     FieldComputedMetadataWrapper,
     FieldType,
     Metadata,
     Paragraph,
 )
 from nucliadb_protos.writer_pb2 import BrokerMessage
 
-from nucliadb.common.maindb.driver import Transaction
 from nucliadb.ingest.processing import PushPayload
-from nucliadb.ingest.settings import settings as ingest_settings
 from nucliadb_models.text import PushTextFormat, Text
 
-KB_RESOURCE_BASIC_FS = "/kbs/{kbid}/r/{uuid}/basic"  # Only used on FS driver
-KB_RESOURCE_BASIC = "/kbs/{kbid}/r/{uuid}"
-
-
-async def set_basic(txn: Transaction, kbid: str, uuid: str, basic: Basic):
-    if ingest_settings.driver == "local":
-        await txn.set(
-            KB_RESOURCE_BASIC_FS.format(kbid=kbid, uuid=uuid),
-            basic.SerializeToString(),
-        )
-    else:
-        await txn.set(
-            KB_RESOURCE_BASIC.format(kbid=kbid, uuid=uuid),
-            basic.SerializeToString(),
-        )
-
-
-async def get_basic(txn: Transaction, kbid: str, uuid: str) -> Optional[bytes]:
-    if ingest_settings.driver == "local":
-        raw_basic = await txn.get(KB_RESOURCE_BASIC_FS.format(kbid=kbid, uuid=uuid))
-    else:
-        raw_basic = await txn.get(KB_RESOURCE_BASIC.format(kbid=kbid, uuid=uuid))
-    return raw_basic
-
 
 def set_title(writer: BrokerMessage, toprocess: PushPayload, title: str):
     title = urllib.parse.unquote(title)
     writer.basic.title = title
     etw = ExtractedTextWrapper()
     etw.field.field = "title"
     etw.field.field_type = FieldType.GENERIC
```

## nucliadb/reader/reader/notifications.py

```diff
@@ -213,15 +213,15 @@
     return resource_title
 
 
 async def get_resource_title(
     kv_driver: Driver, kbid: str, resource_uuid: str
 ) -> Optional[str]:
     async with kv_driver.transaction(read_only=True) as txn:
-        basic = await datamanagers.resources.get_resource_basic(
+        basic = await datamanagers.resources.get_basic(
             txn, kbid=kbid, rid=resource_uuid
         )
         if basic is None:
             return None
         return basic.title
```

## nucliadb/writer/resource/slug.py

```diff
@@ -14,15 +14,13 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 #
 
-from nucliadb.common.maindb.utils import get_driver
-from nucliadb.ingest.orm.knowledgebox import KnowledgeBox
+from nucliadb.common import datamanagers
 
 
 async def resource_slug_exists(kbid: str, slug: str) -> bool:
-    driver = get_driver()
-    async with driver.transaction() as txn:
-        return await KnowledgeBox.resource_slug_exists(txn, kbid, slug)
+    async with datamanagers.with_transaction(read_only=True) as txn:
+        return await datamanagers.resources.slug_exists(txn, kbid=kbid, slug=slug)
```

## Comparing `nucliadb-4.0.0.post538.dist-info/METADATA` & `nucliadb-4.0.0.post539.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nucliadb
-Version: 4.0.0.post538
+Version: 4.0.0.post539
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
-Requires-Dist: nucliadb-telemetry[all] >=4.0.0.post538
-Requires-Dist: nucliadb-utils[cache,fastapi,storages] >=4.0.0.post538
-Requires-Dist: nucliadb-protos >=4.0.0.post538
-Requires-Dist: nucliadb-models >=4.0.0.post538
+Requires-Dist: nucliadb-telemetry[all] >=4.0.0.post539
+Requires-Dist: nucliadb-utils[cache,fastapi,storages] >=4.0.0.post539
+Requires-Dist: nucliadb-protos >=4.0.0.post539
+Requires-Dist: nucliadb-models >=4.0.0.post539
 Requires-Dist: nucliadb-admin-assets >=1.0.0.post1224
 Requires-Dist: nucliadb-node-binding >=2.26.0
 Requires-Dist: uvicorn <0.19.0
 Requires-Dist: argdantic
 Requires-Dist: aiohttp >=3.9.4
 Requires-Dist: lru-dict >=1.1.7
 Requires-Dist: backoff
```

## Comparing `nucliadb-4.0.0.post538.dist-info/entry_points.txt` & `nucliadb-4.0.0.post539.dist-info/entry_points.txt`

 * *Files identical despite different names*

## Comparing `nucliadb-4.0.0.post538.dist-info/RECORD` & `nucliadb-4.0.0.post539.dist-info/RECORD`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 nucliadb/common/datamanagers/__init__.py,sha256=BEBU1dnrSWjQIe1DzBN5jJJHyR4C_Bp2_GDivoxPlrg,1880
 nucliadb/common/datamanagers/cluster.py,sha256=Rc_gWufL-Fx3zQ7WlgCFYBPQD9fPjUvHkyW0QK6hBSg,1451
 nucliadb/common/datamanagers/entities.py,sha256=vQe_xdyqqsII0wmqKWp1yxVTFmB67Tc6bnVxezRUVK0,5383
 nucliadb/common/datamanagers/exceptions.py,sha256=Atz_PP_GGq4jgJaWcAkcRbHBoBaGcC9yJvFteylKtTE,883
 nucliadb/common/datamanagers/kb.py,sha256=zkG3lVbGFFLtjcTlJvJDtTY6S55xdty1nSlwI4xDEQ4,3994
 nucliadb/common/datamanagers/labels.py,sha256=2pN8RrFNTXLitDo44CS3AApjCjbv-2ALkqjwHVR_Mb0,5389
 nucliadb/common/datamanagers/processing.py,sha256=gdCHGzF2LiHOapsg4oaYFYNxACwaCbN1z3kw7iHTuNc,1599
-nucliadb/common/datamanagers/resources.py,sha256=5RA4m_YhUJGSm7Ygq3ytcEQEk1eZNddELRKfHoQN0LU,8719
+nucliadb/common/datamanagers/resources.py,sha256=7YI2-KN22fXbj9FqKGZQGN-bUH26hCt9CBrJUtAclsI,12177
 nucliadb/common/datamanagers/rollover.py,sha256=oxrvnCWM69MG7liMekwQx8TXuNzwixEKJT_--f5Uf-0,5634
 nucliadb/common/datamanagers/synonyms.py,sha256=f7m3N7SXoYSDWvrNDcAeWoWVAHKI8ByZhnBrZ8rVdec,1548
 nucliadb/common/datamanagers/utils.py,sha256=Ll17Pbn1AunTUcGjrk7F2d1SJ0RBOejdmAAlE1BaNmM,1631
 nucliadb/common/http_clients/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
 nucliadb/common/http_clients/auth.py,sha256=9A1k-H121W3lAFRl_XxGizcxUw_qw1STDZqJOC2Kpyw,2146
 nucliadb/common/http_clients/exceptions.py,sha256=47Y8OjkaGV_F18G07FpJhOzgWKUIexhlILyuVtICz8s,1100
 nucliadb/common/http_clients/processing.py,sha256=-J5Lxmlk4coboOWvYQ4gc88AIrvHzSV9bzVsedmslCQ,7155
@@ -111,18 +111,18 @@
 nucliadb/ingest/fields/layout.py,sha256=clgBVGWArtkAEawDqCAu_hB9gVu5c6UT1Cf_5yrw47s,2250
 nucliadb/ingest/fields/link.py,sha256=kwV3KxSn6bZNYBBHljMEN9qNXPlNv80guoKqQib8ivc,4212
 nucliadb/ingest/fields/text.py,sha256=qMMH76gN--Ag1fPZ1I5G9ZPAi4U0i9jbqlrpYc3cMxg,1319
 nucliadb/ingest/orm/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
 nucliadb/ingest/orm/brain.py,sha256=qayvpXdkR_Hq7tw7UmDK8-BH-vFNuRdmkW2EWyk1lLs,28311
 nucliadb/ingest/orm/entities.py,sha256=q027LfocE-KIqRNC1ZOSrrvt6x9NGrB25TZsOe0SyVk,15758
 nucliadb/ingest/orm/exceptions.py,sha256=GKr20V5xLv-WHBBHhr8lBChpW5oa9k18Xuiw-dIF9DM,1279
-nucliadb/ingest/orm/knowledgebox.py,sha256=BKz-jaklScOqFC-NLqWi0PBBNkbU4wGOfa5jcJPUIcg,16028
+nucliadb/ingest/orm/knowledgebox.py,sha256=MquwOlw5hI_yzZtVsZ3mZc86loOouj-w5a6_f1naTKQ,15621
 nucliadb/ingest/orm/metrics.py,sha256=OkwMSPKLZcKba0ZTwtTiIxwBgaLMX5ydhGieKvi2y7E,1096
-nucliadb/ingest/orm/resource.py,sha256=z41OtA0TaEsohQcoLd5UJUKXHTMy_w9KVxJcRkMCajo,60311
-nucliadb/ingest/orm/utils.py,sha256=0GwmyP0CqskAUqKbp0LAInYE64kt8locVqZ0HB04zlw,3683
+nucliadb/ingest/orm/resource.py,sha256=vIpyFpftCgj4sBi5FfRlTLOxJnBuG57uyYH4DK0p6U4,58955
+nucliadb/ingest/orm/utils.py,sha256=A3_EsRw7Nub54qZPF08cv391caxpLQWJURR0_5qP9mU,2685
 nucliadb/ingest/orm/processor/__init__.py,sha256=sVQkEd-TGjTUMHGXJS3IIEtydLD-jSOoAYQK05pO_rA,27042
 nucliadb/ingest/orm/processor/auditing.py,sha256=M8YLnqEJMCvjYATqIRQS2KpJyhyxxoZvBfpxxppKGOI,5090
 nucliadb/ingest/orm/processor/sequence_manager.py,sha256=Mc9SA_NfzxTwovD5yGiAcdmen4pa-QNdsYcONIWeZPc,1690
 nucliadb/ingest/service/__init__.py,sha256=C_lkkjoHm0hDT2fZjEN4mpwXtU4bWthB-vM5-28-MBM,2057
 nucliadb/ingest/service/exceptions.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
 nucliadb/ingest/service/writer.py,sha256=OffZlErS9ndAEnTptFnbwOJqEXujvKd9Dbsgf5vSh3I,30462
 nucliadb/ingest/tests/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
@@ -185,15 +185,15 @@
 nucliadb/reader/api/v1/knowledgebox.py,sha256=Pd71iqTVRgx5u_Gb2LegDTQ3gGTKbVLsAvgcZne5_lM,3641
 nucliadb/reader/api/v1/learning_collector.py,sha256=6XDrfEZffqPrFYGj9TDfWOS1wcy3n9DRu35aH6-2WRA,2099
 nucliadb/reader/api/v1/learning_config.py,sha256=T1bxwsNDnVaeW9lkO4WTO9RHjz6GhYCJwvS1_MNYTes,4472
 nucliadb/reader/api/v1/resource.py,sha256=GkCjExN6wUyIKKgZ9FliDFcPj_VGMhw9KJobYWZf5N8,13951
 nucliadb/reader/api/v1/router.py,sha256=eyNmEGSP9zHkCIG5XlAXl6sukq950B7gFT3X2peMtIE,1011
 nucliadb/reader/api/v1/services.py,sha256=OSQXi-QcuhS_LDzwzntiLgP16jIYwTn48iypdzYayTQ,12115
 nucliadb/reader/reader/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
-nucliadb/reader/reader/notifications.py,sha256=2In2E-2FUawjqNWKaxqrw_rB2hTzgAXVV5yFhF4gHOA,7988
+nucliadb/reader/reader/notifications.py,sha256=Hfs2QUguAKeMrH0oaG3e7eDBJSCumNMb1kuXk_DFEKU,7979
 nucliadb/reader/tests/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
 nucliadb/reader/tests/conftest.py,sha256=RH5huJVfSZ9cQgzEWC_xViGbXUelZFuHmrOnWb-FpEU,1224
 nucliadb/reader/tests/fixtures.py,sha256=pVrolKyIQaUA01Coe8WHG6OuliqREnzq8DJnnfPF8_k,4345
 nucliadb/reader/tests/test_list_resources.py,sha256=yKsG6MLh4_cB7Yhov0OoBAVCJCXnpuQmT453R1oVQ6Q,2748
 nucliadb/reader/tests/test_reader_file_download.py,sha256=V_wLTRmSlYemSPLOBo3A_jhMBluro2sJiQwSsGGBx6I,10199
 nucliadb/reader/tests/test_reader_resource.py,sha256=A7XzHngspJxPqxzyMZ2Zg2Kp8SuDTi78Fo2rG1roLyo,10586
 nucliadb/reader/tests/test_reader_resource_field.py,sha256=YQ-U2mEGhs_rPGxcWPZmWLSEoCxBo3AVDtLZCtZrGb8,6535
@@ -429,15 +429,15 @@
 nucliadb/writer/layouts/__init__.py,sha256=Siod9W963CG5gJa20GSTw9VemAFgsMmJDbUspbrYAyE,1612
 nucliadb/writer/layouts/v1.py,sha256=Yc2idmfrpCS8js_XJByNWA_tmt2WeKoWvidLHoTPXoo,2115
 nucliadb/writer/resource/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
 nucliadb/writer/resource/audit.py,sha256=SXPu_hdNBlm9uCSl666UQL7hzMx9zYVbBLT_U7ro8Gs,1425
 nucliadb/writer/resource/basic.py,sha256=eSWW6u6U3e0KjjdFwp9YQokojoDepl5vmJfbE2MQACM,10968
 nucliadb/writer/resource/field.py,sha256=woPN-1bIC6eMXtvggMuvcVwbNAGLpS7GIz8pkO9UNz4,16740
 nucliadb/writer/resource/origin.py,sha256=3Y2zVtG_v0U6uMbDhW9Yl7KKHKt5V3T5_v3iCpqdBEk,2022
-nucliadb/writer/resource/slug.py,sha256=Brjbo6DgVFgDZF6rdUqjXnr3oLmAhWHKW2Xk-ZRRQO0,1152
+nucliadb/writer/resource/slug.py,sha256=CMhnYBJIrKHshv5T93sGygBXtU5UY_AOYC-B7DC5DOQ,1093
 nucliadb/writer/tests/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
 nucliadb/writer/tests/conftest.py,sha256=bmFKnuaqRqMCjtTp6c4V4R-qF59OPu0gW8-hp1TXFwk,1200
 nucliadb/writer/tests/fixtures.py,sha256=Ni66Iq-A6W8qqa6V6PwSzDq2BD9IINXlGexilVaDzPU,5971
 nucliadb/writer/tests/test_fields.py,sha256=fbzN0Bgu8HOLAqqYXO15JIqXN1bxr7mTTCTUuYhG85c,15472
 nucliadb/writer/tests/test_files.py,sha256=V-YB-ceSVCMmiVuXeH7BKl00GmC7t0ZyjUPAKqMr048,25999
 nucliadb/writer/tests/test_knowledgebox.py,sha256=KPUGr4TsmHXSTfte40rY18ANUHaUYs_TD4DXCIlawt8,1729
 nucliadb/writer/tests/test_reprocess_file_field.py,sha256=O37eL7RR4vLDFTjZ3UFh0att9PqimJM9sUt1yIPh7Ss,4358
@@ -450,13 +450,13 @@
 nucliadb/writer/tus/exceptions.py,sha256=CmxYKnHXpXug25DYV4SpVAU47SGD-NVBd7pNTRbWHyk,2186
 nucliadb/writer/tus/gcs.py,sha256=WykJZicWKRYkVB5_Fkb_1cVLovAk86IVkEn1VgEDufc,14527
 nucliadb/writer/tus/local.py,sha256=lIOoGaylnsxPBYGskcmKSHv7MsvwIYFS4soDLey_KSs,5849
 nucliadb/writer/tus/pg.py,sha256=JUK_xKsyNcKAvWOch8gUMTc_e1evI_3aC6-Y5gMk2jw,4367
 nucliadb/writer/tus/s3.py,sha256=a9mfPtjBW3QaTYY2r6P7u_Y13V6mBefZjWgV4juZzgE,9069
 nucliadb/writer/tus/storage.py,sha256=8iBOjWIcY6PawQq_rmSiBKi0Gl6J6Q5ad6L-9nLCcJ4,4734
 nucliadb/writer/tus/utils.py,sha256=MSdVbRsRSZVdkaum69_0wku7X3p5wlZf4nr6E0GMKbw,2556
-nucliadb-4.0.0.post538.dist-info/METADATA,sha256=H6PtOwbnXttNeJPk7FDLhdUUMS7qtF1K6JhxK_dQ1w8,4423
-nucliadb-4.0.0.post538.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-nucliadb-4.0.0.post538.dist-info/entry_points.txt,sha256=XqGfgFDuY3zXQc8ewXM2TRVjTModIq851zOsgrmaXx4,1268
-nucliadb-4.0.0.post538.dist-info/top_level.txt,sha256=hwYhTVnX7jkQ9gJCkVrbqEG1M4lT2F_iPQND1fCzF80,20
-nucliadb-4.0.0.post538.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-nucliadb-4.0.0.post538.dist-info/RECORD,,
+nucliadb-4.0.0.post539.dist-info/METADATA,sha256=nHAQsdm1L2Ib7mrKaUB9-2bJSImAtAHzGPZvIrkMnZE,4423
+nucliadb-4.0.0.post539.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+nucliadb-4.0.0.post539.dist-info/entry_points.txt,sha256=XqGfgFDuY3zXQc8ewXM2TRVjTModIq851zOsgrmaXx4,1268
+nucliadb-4.0.0.post539.dist-info/top_level.txt,sha256=hwYhTVnX7jkQ9gJCkVrbqEG1M4lT2F_iPQND1fCzF80,20
+nucliadb-4.0.0.post539.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
+nucliadb-4.0.0.post539.dist-info/RECORD,,
```


# Comparing `tmp/ffun-1.5.3.tar.gz` & `tmp/ffun-1.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ffun-1.5.3.tar", max compression
+gzip compressed data, was "ffun-1.5.4.tar", max compression
```

## Comparing `ffun-1.5.3.tar` & `ffun-1.5.4.tar`

### file list

```diff
@@ -1,231 +1,235 @@
--rw-r--r--   0        0        0      344 2024-05-22 13:04:51.379570 ffun-1.5.3/README.md
--rw-r--r--   0        0        0        0 2024-05-22 13:04:51.379570 ffun-1.5.3/ffun/__init__.py
--rw-r--r--   0        0        0        0 2024-05-22 13:04:51.379570 ffun-1.5.3/ffun/api/__init__.py
--rw-r--r--   0        0        0    10249 2024-05-22 13:04:51.379570 ffun-1.5.3/ffun/api/entities.py
--rw-r--r--   0        0        0    13637 2024-05-22 13:04:51.379570 ffun-1.5.3/ffun/api/http_handlers.py
--rw-r--r--   0        0        0      245 2024-05-22 13:04:51.379570 ffun-1.5.3/ffun/api/settings.py
--rw-r--r--   0        0        0        0 2024-05-22 13:04:51.379570 ffun-1.5.3/ffun/application/__init__.py
--rw-r--r--   0        0        0     4314 2024-05-22 13:04:51.379570 ffun-1.5.3/ffun/application/application.py
--rw-r--r--   0        0        0      115 2024-05-22 13:04:51.379570 ffun-1.5.3/ffun/application/errors.py
--rw-r--r--   0        0        0       68 2024-05-22 13:04:51.379570 ffun-1.5.3/ffun/application/resources.py
--rw-r--r--   0        0        0     1635 2024-05-22 13:04:51.379570 ffun-1.5.3/ffun/application/settings.py
--rw-r--r--   0        0        0        0 2024-05-22 13:04:51.379570 ffun-1.5.3/ffun/application/tests/__init__.py
--rw-r--r--   0        0        0      422 2024-05-22 13:04:51.379570 ffun-1.5.3/ffun/application/tests/test_settings.py
--rw-r--r--   0        0        0     3724 2024-05-22 13:04:51.379570 ffun-1.5.3/ffun/application/user_settings.py
--rw-r--r--   0        0        0      281 2024-05-22 13:04:51.379570 ffun-1.5.3/ffun/application/utils.py
--rw-r--r--   0        0        0     1252 2024-05-22 13:04:51.379570 ffun-1.5.3/ffun/application/workers.py
--rw-r--r--   0        0        0        0 2024-05-22 13:04:51.379570 ffun-1.5.3/ffun/auth/__init__.py
--rw-r--r--   0        0        0      984 2024-05-22 13:04:51.379570 ffun-1.5.3/ffun/auth/dependencies.py
--rw-r--r--   0        0        0      828 2024-05-22 13:04:51.379570 ffun-1.5.3/ffun/auth/settings.py
--rw-r--r--   0        0        0     2800 2024-05-22 13:04:51.379570 ffun-1.5.3/ffun/auth/supertokens.py
--rw-r--r--   0        0        0        0 2024-05-22 13:04:51.379570 ffun-1.5.3/ffun/cli/__init__.py
--rw-r--r--   0        0        0      174 2024-05-22 13:04:51.379570 ffun-1.5.3/ffun/cli/application.py
--rw-r--r--   0        0        0      439 2024-05-22 13:04:51.379570 ffun-1.5.3/ffun/cli/cli.py
--rw-r--r--   0        0        0        0 2024-05-22 13:04:51.379570 ffun-1.5.3/ffun/cli/commands/__init__.py
--rw-r--r--   0        0        0      732 2024-05-22 13:04:51.379570 ffun-1.5.3/ffun/cli/commands/configs.py
--rw-r--r--   0        0        0     1050 2024-05-22 13:04:51.379570 ffun-1.5.3/ffun/cli/commands/entries.py
--rw-r--r--   0        0        0     1393 2024-05-22 13:04:51.379570 ffun-1.5.3/ffun/cli/commands/failed_entries.py
--rw-r--r--   0        0        0      538 2024-05-22 13:04:51.379570 ffun-1.5.3/ffun/cli/commands/meta.py
--rw-r--r--   0        0        0     1001 2024-05-22 13:04:51.379570 ffun-1.5.3/ffun/cli/commands/supertokens.py
--rw-r--r--   0        0        0      884 2024-05-22 13:04:51.379570 ffun-1.5.3/ffun/cli/commands/workers.py
--rw-r--r--   0        0        0      209 2024-05-22 13:04:51.379570 ffun-1.5.3/ffun/cli/commands/yoyo.py
--rw-r--r--   0        0        0     1333 2024-05-22 13:04:51.379570 ffun-1.5.3/ffun/conftest.py
--rw-r--r--   0        0        0        0 2024-05-22 13:04:51.379570 ffun-1.5.3/ffun/core/__init__.py
--rw-r--r--   0        0        0      631 2024-05-22 13:04:51.379570 ffun-1.5.3/ffun/core/api.py
--rw-r--r--   0        0        0     3139 2024-05-22 13:04:51.379570 ffun-1.5.3/ffun/core/background_tasks.py
--rw-r--r--   0        0        0      493 2024-05-22 13:04:51.379570 ffun-1.5.3/ffun/core/entities.py
--rw-r--r--   0        0        0      552 2024-05-22 13:04:51.379570 ffun-1.5.3/ffun/core/errors.py
--rw-r--r--   0        0        0     2773 2024-05-22 13:04:51.379570 ffun-1.5.3/ffun/core/json.py
--rw-r--r--   0        0        0     5440 2024-05-22 13:04:51.379570 ffun-1.5.3/ffun/core/logging.py
--rw-r--r--   0        0        0     1516 2024-05-22 13:04:51.379570 ffun-1.5.3/ffun/core/middlewares.py
--rw-r--r--   0        0        0      882 2024-05-22 13:04:51.379570 ffun-1.5.3/ffun/core/migrations.py
--rw-r--r--   0        0        0     4019 2024-05-22 13:04:51.379570 ffun-1.5.3/ffun/core/postgresql.py
--rw-r--r--   0        0        0      695 2024-05-22 13:04:51.379570 ffun-1.5.3/ffun/core/register.py
--rw-r--r--   0        0        0     1442 2024-05-22 13:04:51.379570 ffun-1.5.3/ffun/core/sentry.py
--rw-r--r--   0        0        0      347 2024-05-22 13:04:51.379570 ffun-1.5.3/ffun/core/settings.py
--rw-r--r--   0        0        0        0 2024-05-22 13:04:51.379570 ffun-1.5.3/ffun/core/tests/__init__.py
--rw-r--r--   0        0        0     4551 2024-05-22 13:04:51.379570 ffun-1.5.3/ffun/core/tests/helpers.py
--rw-r--r--   0        0        0       82 2024-05-22 13:04:51.379570 ffun-1.5.3/ffun/core/tests/make.py
--rw-r--r--   0        0        0      486 2024-05-22 13:04:51.379570 ffun-1.5.3/ffun/core/text.py
--rw-r--r--   0        0        0     1088 2024-05-22 13:04:51.379570 ffun-1.5.3/ffun/core/utils.py
--rw-r--r--   0        0        0        0 2024-05-22 13:04:51.379570 ffun-1.5.3/ffun/domain/__init__.py
--rw-r--r--   0        0        0        0 2024-05-22 13:04:51.379570 ffun-1.5.3/ffun/domain/tests/__init__.py
--rw-r--r--   0        0        0     6590 2024-05-22 13:04:51.379570 ffun-1.5.3/ffun/domain/tests/test_urls.py
--rw-r--r--   0        0        0     3811 2024-05-22 13:04:51.379570 ffun-1.5.3/ffun/domain/urls.py
--rw-r--r--   0        0        0        0 2024-05-22 13:04:51.379570 ffun-1.5.3/ffun/feeds/__init__.py
--rw-r--r--   0        0        0      826 2024-05-22 13:04:51.379570 ffun-1.5.3/ffun/feeds/domain.py
--rw-r--r--   0        0        0     1905 2024-05-22 13:04:51.379570 ffun-1.5.3/ffun/feeds/entities.py
--rw-r--r--   0        0        0      131 2024-05-22 13:04:51.379570 ffun-1.5.3/ffun/feeds/errors.py
--rw-r--r--   0        0        0     1027 2024-05-22 13:04:51.379570 ffun-1.5.3/ffun/feeds/migrations/20230329_01_ilwfq-feeds-table.py
--rw-r--r--   0        0        0      641 2024-05-22 13:04:51.379570 ffun-1.5.3/ffun/feeds/migrations/20230426_01_IiF5m-add-title-and-description.py
--rw-r--r--   0        0        0      561 2024-05-22 13:04:51.379570 ffun-1.5.3/ffun/feeds/migrations/20240504_01_vBDVJ-column-for-feed-unique-id.py
--rw-r--r--   0        0        0      531 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/feeds/migrations/20240504_02_gEapd-fill-uids-for-feeds.py
--rw-r--r--   0        0        0      725 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/feeds/migrations/20240512_01_jL7Mt-turn-on-unique-uids.py
--rw-r--r--   0        0        0     4062 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/feeds/operations.py
--rw-r--r--   0        0        0        0 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/feeds/tests/__init__.py
--rw-r--r--   0        0        0     1512 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/feeds/tests/fixtures.py
--rw-r--r--   0        0        0     1178 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/feeds/tests/make.py
--rw-r--r--   0        0        0      445 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/feeds/tests/test_domain.py
--rw-r--r--   0        0        0     7782 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/feeds/tests/test_operations.py
--rw-r--r--   0        0        0        0 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/feeds_collections/__init__.py
--rw-r--r--   0        0        0      495 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/feeds_collections/collections/artificial_intelligence.py
--rw-r--r--   0        0        0     1357 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/feeds_collections/collections/gamedev.py
--rw-r--r--   0        0        0      777 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/feeds_collections/domain.py
--rw-r--r--   0        0        0      128 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/feeds_collections/entities.py
--rw-r--r--   0        0        0      573 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/feeds_collections/predefines.py
--rw-r--r--   0        0        0        0 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/feeds_collections/tests/__init__.py
--rw-r--r--   0        0        0      684 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/feeds_collections/tests/fixtures.py
--rw-r--r--   0        0        0        0 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/feeds_discoverer/__init__.py
--rw-r--r--   0        0        0     3974 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/feeds_discoverer/domain.py
--rw-r--r--   0        0        0        0 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/feeds_links/__init__.py
--rw-r--r--   0        0        0      553 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/feeds_links/domain.py
--rw-r--r--   0        0        0      163 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/feeds_links/entities.py
--rw-r--r--   0        0        0      810 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/feeds_links/migrations/20230427_01_9HuHj-add-feeds-links.py
--rw-r--r--   0        0        0     2326 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/feeds_links/operations.py
--rw-r--r--   0        0        0        0 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/feeds_links/tests/__init__.py
--rw-r--r--   0        0        0     2908 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/feeds_links/tests/test_operations.py
--rw-r--r--   0        0        0        0 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/librarian/__init__.py
--rw-r--r--   0        0        0     5182 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/librarian/background_processors.py
--rw-r--r--   0        0        0     3759 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/librarian/domain.py
--rw-r--r--   0        0        0      205 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/librarian/entities.py
--rw-r--r--   0        0        0      217 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/librarian/errors.py
--rw-r--r--   0        0        0     2101 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/librarian/migrations/20240313_01_Yv74T-processors-pointers.py
--rw-r--r--   0        0        0     3035 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/librarian/migrations/20240319_01_MTJyn-migrate-to-processors-queue.py
--rw-r--r--   0        0        0     5112 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/librarian/operations.py
--rw-r--r--   0        0        0        0 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/librarian/processors/__init__.py
--rw-r--r--   0        0        0     1255 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/librarian/processors/base.py
--rw-r--r--   0        0        0     1548 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/librarian/processors/domain.py
--rw-r--r--   0        0        0      468 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/librarian/processors/native_tags.py
--rw-r--r--   0        0        0     3295 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/librarian/processors/openai_chat_3_5.py
--rw-r--r--   0        0        0     4421 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/librarian/processors/openai_chat_3_5_functions.py
--rw-r--r--   0        0        0        0 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/librarian/processors/tests/__init__.py
--rw-r--r--   0        0        0     1139 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/librarian/processors/tests/test_upper_case_title.py
--rw-r--r--   0        0        0      434 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/librarian/processors/upper_case_title.py
--rw-r--r--   0        0        0     1089 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/librarian/settings.py
--rw-r--r--   0        0        0        0 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/librarian/tests/__init__.py
--rw-r--r--   0        0        0      845 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/librarian/tests/fixtures.py
--rw-r--r--   0        0        0      487 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/librarian/tests/helpers.py
--rw-r--r--   0        0        0      553 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/librarian/tests/make.py
--rw-r--r--   0        0        0     4104 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/librarian/tests/test_background_processors.py
--rw-r--r--   0        0        0    13605 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/librarian/tests/test_domain.py
--rw-r--r--   0        0        0    14031 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/librarian/tests/test_operations.py
--rw-r--r--   0        0        0        0 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/library/__init__.py
--rw-r--r--   0        0        0     1476 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/library/domain.py
--rw-r--r--   0        0        0     1168 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/library/entities.py
--rw-r--r--   0        0        0      149 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/library/errors.py
--rw-r--r--   0        0        0     1498 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/library/migrations/20230331_01_UsHwp-entries-table.py
--rw-r--r--   0        0        0     1288 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/library/migrations/20230427_01_pv33u-fix-entries-unique-index.py
--rw-r--r--   0        0        0      710 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/library/migrations/20230514_01_Bwb35-processed-state.py
--rw-r--r--   0        0        0     1125 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/library/migrations/20240315_01_tWftt-optimize-l-entries.py
--rw-r--r--   0        0        0     1003 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/library/migrations/20240503_01_Bmzw6-remove-l-entry-process-info.py
--rw-r--r--   0        0        0     1194 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/library/migrations/20240506_01_My4vi-remove-duplicated-entries-from-feeds.py
--rw-r--r--   0        0        0      784 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/library/migrations/20240506_02_zQdSl-fix-unique-index-on-l-entries.py
--rw-r--r--   0        0        0     5926 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/library/operations.py
--rw-r--r--   0        0        0        0 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/library/tests/__init__.py
--rw-r--r--   0        0        0      799 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/library/tests/fixtures.py
--rw-r--r--   0        0        0     1663 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/library/tests/make.py
--rw-r--r--   0        0        0     1414 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/library/tests/test_domain.py
--rw-r--r--   0        0        0    15331 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/library/tests/test_operations.py
--rw-r--r--   0        0        0        0 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/loader/__init__.py
--rw-r--r--   0        0        0      882 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/loader/background_loader.py
--rw-r--r--   0        0        0    11775 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/loader/domain.py
--rw-r--r--   0        0        0      181 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/loader/errors.py
--rw-r--r--   0        0        0      477 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/loader/settings.py
--rw-r--r--   0        0        0        0 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/loader/tests/__init__.py
--rw-r--r--   0        0        0     8583 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/loader/tests/test_domain.py
--rw-r--r--   0        0        0        0 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/markers/__init__.py
--rw-r--r--   0        0        0      504 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/markers/domain.py
--rw-r--r--   0        0        0       57 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/markers/entities.py
--rw-r--r--   0        0        0      855 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/markers/migrations/20230419_01_9vMm5-markers-tables.py
--rw-r--r--   0        0        0     2447 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/markers/operations.py
--rw-r--r--   0        0        0        0 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/markers/tests/__init__.py
--rw-r--r--   0        0        0     4835 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/markers/tests/test_operations.py
--rw-r--r--   0        0        0        0 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/meta/__init__.py
--rw-r--r--   0        0        0     3557 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/meta/domain.py
--rw-r--r--   0        0        0      345 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/meta/migrations/20240512_01_0F799-unity-duplicated-feeds.py
--rw-r--r--   0        0        0      246 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/meta/settings.py
--rw-r--r--   0        0        0        0 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/meta/tests/__init__.py
--rw-r--r--   0        0        0    15939 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/meta/tests/test_domain.py
--rw-r--r--   0        0        0        0 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/ontology/__init__.py
--rw-r--r--   0        0        0     3840 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/ontology/domain.py
--rw-r--r--   0        0        0     1683 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/ontology/entities.py
--rw-r--r--   0        0        0     1092 2024-05-22 13:04:51.387570 ffun-1.5.3/ffun/ontology/migrations/20230404_01_ZUBsm-ontology-tables.py
--rw-r--r--   0        0        0      520 2024-05-22 13:04:51.387570 ffun-1.5.3/ffun/ontology/migrations/20230617_01_XDdNG-rename-tags-names-to-uid.py
--rw-r--r--   0        0        0      799 2024-05-22 13:04:51.387570 ffun-1.5.3/ffun/ontology/migrations/20230617_02_L0MmA-tags-relationship-processor-tracking.py
--rw-r--r--   0        0        0     1008 2024-05-22 13:04:51.387570 ffun-1.5.3/ffun/ontology/migrations/20230617_03_de7vS-tags-properties.py
--rw-r--r--   0        0        0     6307 2024-05-22 13:04:51.387570 ffun-1.5.3/ffun/ontology/operations.py
--rw-r--r--   0        0        0        0 2024-05-22 13:04:51.387570 ffun-1.5.3/ffun/ontology/tests/__init__.py
--rw-r--r--   0        0        0      834 2024-05-22 13:04:51.387570 ffun-1.5.3/ffun/ontology/tests/fixtures.py
--rw-r--r--   0        0        0      408 2024-05-22 13:04:51.387570 ffun-1.5.3/ffun/ontology/tests/helpers.py
--rw-r--r--   0        0        0     9964 2024-05-22 13:04:51.387570 ffun-1.5.3/ffun/ontology/tests/test_operations.py
--rw-r--r--   0        0        0        0 2024-05-22 13:04:51.387570 ffun-1.5.3/ffun/openai/__init__.py
--rw-r--r--   0        0        0     5962 2024-05-22 13:04:51.387570 ffun-1.5.3/ffun/openai/client.py
--rw-r--r--   0        0        0      612 2024-05-22 13:04:51.387570 ffun-1.5.3/ffun/openai/entities.py
--rw-r--r--   0        0        0      150 2024-05-22 13:04:51.387570 ffun-1.5.3/ffun/openai/errors.py
--rw-r--r--   0        0        0     7597 2024-05-22 13:04:51.387570 ffun-1.5.3/ffun/openai/keys_rotator.py
--rw-r--r--   0        0        0     1919 2024-05-22 13:04:51.387570 ffun-1.5.3/ffun/openai/keys_statuses.py
--rw-r--r--   0        0        0      372 2024-05-22 13:04:51.387570 ffun-1.5.3/ffun/openai/settings.py
--rw-r--r--   0        0        0        0 2024-05-22 13:04:51.387570 ffun-1.5.3/ffun/openai/tests/__init__.py
--rw-r--r--   0        0        0      130 2024-05-22 13:04:51.387570 ffun-1.5.3/ffun/openai/tests/conftest.py
--rw-r--r--   0        0        0     2518 2024-05-22 13:04:51.387570 ffun-1.5.3/ffun/openai/tests/fixtures.py
--rw-r--r--   0        0        0    19734 2024-05-22 13:04:51.387570 ffun-1.5.3/ffun/openai/tests/test_keys_rotator.py
--rw-r--r--   0        0        0     2833 2024-05-22 13:04:51.387570 ffun-1.5.3/ffun/openai/tests/test_keys_statuses.py
--rw-r--r--   0        0        0        0 2024-05-22 13:04:51.387570 ffun-1.5.3/ffun/parsers/__init__.py
--rw-r--r--   0        0        0      228 2024-05-22 13:04:51.387570 ffun-1.5.3/ffun/parsers/domain.py
--rw-r--r--   0        0        0      560 2024-05-22 13:04:51.387570 ffun-1.5.3/ffun/parsers/entities.py
--rw-r--r--   0        0        0     2355 2024-05-22 13:04:51.387570 ffun-1.5.3/ffun/parsers/feed.py
--rw-r--r--   0        0        0     1325 2024-05-22 13:04:51.387570 ffun-1.5.3/ffun/parsers/feedly.py
--rw-r--r--   0        0        0        0 2024-05-22 13:04:51.387570 ffun-1.5.3/ffun/parsers/tests/__init__.py
--rw-r--r--   0        0        0     1219 2024-05-22 13:04:51.387570 ffun-1.5.3/ffun/parsers/tests/feeds_fixtures/atom_with_relative_news_links.xml
--rw-r--r--   0        0        0      639 2024-05-22 13:04:51.387570 ffun-1.5.3/ffun/parsers/tests/feeds_fixtures/atom_with_relative_news_links.xml.expected.json
--rw-r--r--   0        0        0     4745 2024-05-22 13:04:51.387570 ffun-1.5.3/ffun/parsers/tests/feeds_fixtures/wordpress_rss_2_0_feed.xml
--rw-r--r--   0        0        0     1072 2024-05-22 13:04:51.387570 ffun-1.5.3/ffun/parsers/tests/feeds_fixtures/wordpress_rss_2_0_feed.xml.expected.json
--rw-r--r--   0        0        0      966 2024-05-22 13:04:51.387570 ffun-1.5.3/ffun/parsers/tests/make.py
--rw-r--r--   0        0        0     1205 2024-05-22 13:04:51.387570 ffun-1.5.3/ffun/parsers/tests/test_feed.py
--rw-r--r--   0        0        0        0 2024-05-22 13:04:51.387570 ffun-1.5.3/ffun/resources/__init__.py
--rw-r--r--   0        0        0      769 2024-05-22 13:04:51.387570 ffun-1.5.3/ffun/resources/domain.py
--rw-r--r--   0        0        0      280 2024-05-22 13:04:51.387570 ffun-1.5.3/ffun/resources/entities.py
--rw-r--r--   0        0        0      120 2024-05-22 13:04:51.387570 ffun-1.5.3/ffun/resources/errors.py
--rw-r--r--   0        0        0      865 2024-05-22 13:04:51.387570 ffun-1.5.3/ffun/resources/migrations/20230702_01_LEEES-resources-table.py
--rw-r--r--   0        0        0     3984 2024-05-22 13:04:51.387570 ffun-1.5.3/ffun/resources/operations.py
--rw-r--r--   0        0        0        0 2024-05-22 13:04:51.387570 ffun-1.5.3/ffun/resources/tests/__init__.py
--rw-r--r--   0        0        0     1945 2024-05-22 13:04:51.387570 ffun-1.5.3/ffun/resources/tests/test_domain.py
--rw-r--r--   0        0        0     9480 2024-05-22 13:04:51.387570 ffun-1.5.3/ffun/resources/tests/test_operations.py
--rw-r--r--   0        0        0        0 2024-05-22 13:04:51.387570 ffun-1.5.3/ffun/scores/__init__.py
--rw-r--r--   0        0        0      884 2024-05-22 13:04:51.387570 ffun-1.5.3/ffun/scores/domain.py
--rw-r--r--   0        0        0      250 2024-05-22 13:04:51.387570 ffun-1.5.3/ffun/scores/entities.py
--rw-r--r--   0        0        0      104 2024-05-22 13:04:51.387570 ffun-1.5.3/ffun/scores/errors.py
--rw-r--r--   0        0        0      851 2024-05-22 13:04:51.387570 ffun-1.5.3/ffun/scores/migrations/20230417_01_0XYOQ-scores-tables.py
--rw-r--r--   0        0        0      603 2024-05-22 13:04:51.387570 ffun-1.5.3/ffun/scores/migrations/20230813_01_l7qop-updated-at-field.py
--rw-r--r--   0        0        0     2603 2024-05-22 13:04:51.387570 ffun-1.5.3/ffun/scores/operations.py
--rw-r--r--   0        0        0        0 2024-05-22 13:04:51.387570 ffun-1.5.3/ffun/scores/tests/__init__.py
--rw-r--r--   0        0        0     1239 2024-05-22 13:04:51.387570 ffun-1.5.3/ffun/scores/tests/test_domain.py
--rw-r--r--   0        0        0     6810 2024-05-22 13:04:51.387570 ffun-1.5.3/ffun/scores/tests/test_operations.py
--rw-r--r--   0        0        0        0 2024-05-22 13:04:51.387570 ffun-1.5.3/ffun/tags/__init__.py
--rw-r--r--   0        0        0     1578 2024-05-22 13:04:51.387570 ffun-1.5.3/ffun/tags/converters.py
--rw-r--r--   0        0        0        0 2024-05-22 13:04:51.387570 ffun-1.5.3/ffun/tags/tests/__init__.py
--rw-r--r--   0        0        0     1352 2024-05-22 13:04:51.387570 ffun-1.5.3/ffun/tags/tests/test_converters.py
--rw-r--r--   0        0        0        0 2024-05-22 13:04:51.387570 ffun-1.5.3/ffun/user_settings/__init__.py
--rw-r--r--   0        0        0     1842 2024-05-22 13:04:51.387570 ffun-1.5.3/ffun/user_settings/domain.py
--rw-r--r--   0        0        0       54 2024-05-22 13:04:51.387570 ffun-1.5.3/ffun/user_settings/entities.py
--rw-r--r--   0        0        0      137 2024-05-22 13:04:51.387570 ffun-1.5.3/ffun/user_settings/errors.py
--rw-r--r--   0        0        0      732 2024-05-22 13:04:51.387570 ffun-1.5.3/ffun/user_settings/migrations/20230701_01_7zBP0-settings-table.py
--rw-r--r--   0        0        0      534 2024-05-22 13:04:51.387570 ffun-1.5.3/ffun/user_settings/migrations/20230911_01_5vjXI-index-to-search-by-value.py
--rw-r--r--   0        0        0     1748 2024-05-22 13:04:51.387570 ffun-1.5.3/ffun/user_settings/operations.py
--rw-r--r--   0        0        0      581 2024-05-22 13:04:51.387570 ffun-1.5.3/ffun/user_settings/settings.py
--rw-r--r--   0        0        0      508 2024-05-22 13:04:51.387570 ffun-1.5.3/ffun/user_settings/tests/asserts.py
--rw-r--r--   0        0        0     6956 2024-05-22 13:04:51.387570 ffun-1.5.3/ffun/user_settings/tests/test_domain.py
--rw-r--r--   0        0        0     5492 2024-05-22 13:04:51.387570 ffun-1.5.3/ffun/user_settings/tests/test_operations.py
--rw-r--r--   0        0        0     2297 2024-05-22 13:04:51.387570 ffun-1.5.3/ffun/user_settings/types.py
--rw-r--r--   0        0        0      489 2024-05-22 13:04:51.387570 ffun-1.5.3/ffun/user_settings/values.py
--rw-r--r--   0        0        0        0 2024-05-22 13:04:51.387570 ffun-1.5.3/ffun/users/__init__.py
--rw-r--r--   0        0        0      586 2024-05-22 13:04:51.387570 ffun-1.5.3/ffun/users/domain.py
--rw-r--r--   0        0        0      161 2024-05-22 13:04:51.387570 ffun-1.5.3/ffun/users/entities.py
--rw-r--r--   0        0        0      111 2024-05-22 13:04:51.387570 ffun-1.5.3/ffun/users/errors.py
--rw-r--r--   0        0        0      718 2024-05-22 13:04:51.387570 ffun-1.5.3/ffun/users/migrations/20230527_01_soIr3-users-mapping.py
--rw-r--r--   0        0        0     1232 2024-05-22 13:04:51.387570 ffun-1.5.3/ffun/users/operations.py
--rw-r--r--   0        0        0        0 2024-05-22 13:04:51.387570 ffun-1.5.3/ffun/users/tests/__init__.py
--rw-r--r--   0        0        0     1101 2024-05-22 13:04:51.387570 ffun-1.5.3/ffun/users/tests/fixtures.py
--rw-r--r--   0        0        0      348 2024-05-22 13:04:51.387570 ffun-1.5.3/ffun/users/tests/make.py
--rw-r--r--   0        0        0     4263 2024-05-22 13:04:58.883531 ffun-1.5.3/pyproject.toml
--rw-r--r--   0        0        0     2901 1970-01-01 00:00:00.000000 ffun-1.5.3/PKG-INFO
+-rw-r--r--   0        0        0      344 2024-05-23 16:38:10.122613 ffun-1.5.4/README.md
+-rw-r--r--   0        0        0        0 2024-05-23 16:38:10.122613 ffun-1.5.4/ffun/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-23 16:38:10.122613 ffun-1.5.4/ffun/api/__init__.py
+-rw-r--r--   0        0        0    10256 2024-05-23 16:38:10.122613 ffun-1.5.4/ffun/api/entities.py
+-rw-r--r--   0        0        0    13637 2024-05-23 16:38:10.122613 ffun-1.5.4/ffun/api/http_handlers.py
+-rw-r--r--   0        0        0      245 2024-05-23 16:38:10.122613 ffun-1.5.4/ffun/api/settings.py
+-rw-r--r--   0        0        0        0 2024-05-23 16:38:10.122613 ffun-1.5.4/ffun/application/__init__.py
+-rw-r--r--   0        0        0     4314 2024-05-23 16:38:10.122613 ffun-1.5.4/ffun/application/application.py
+-rw-r--r--   0        0        0      115 2024-05-23 16:38:10.122613 ffun-1.5.4/ffun/application/errors.py
+-rw-r--r--   0        0        0       68 2024-05-23 16:38:10.122613 ffun-1.5.4/ffun/application/resources.py
+-rw-r--r--   0        0        0     1635 2024-05-23 16:38:10.122613 ffun-1.5.4/ffun/application/settings.py
+-rw-r--r--   0        0        0        0 2024-05-23 16:38:10.122613 ffun-1.5.4/ffun/application/tests/__init__.py
+-rw-r--r--   0        0        0      422 2024-05-23 16:38:10.122613 ffun-1.5.4/ffun/application/tests/test_settings.py
+-rw-r--r--   0        0        0     3724 2024-05-23 16:38:10.122613 ffun-1.5.4/ffun/application/user_settings.py
+-rw-r--r--   0        0        0      281 2024-05-23 16:38:10.122613 ffun-1.5.4/ffun/application/utils.py
+-rw-r--r--   0        0        0     1252 2024-05-23 16:38:10.122613 ffun-1.5.4/ffun/application/workers.py
+-rw-r--r--   0        0        0        0 2024-05-23 16:38:10.122613 ffun-1.5.4/ffun/auth/__init__.py
+-rw-r--r--   0        0        0      984 2024-05-23 16:38:10.122613 ffun-1.5.4/ffun/auth/dependencies.py
+-rw-r--r--   0        0        0      828 2024-05-23 16:38:10.122613 ffun-1.5.4/ffun/auth/settings.py
+-rw-r--r--   0        0        0     2800 2024-05-23 16:38:10.122613 ffun-1.5.4/ffun/auth/supertokens.py
+-rw-r--r--   0        0        0        0 2024-05-23 16:38:10.122613 ffun-1.5.4/ffun/cli/__init__.py
+-rw-r--r--   0        0        0      174 2024-05-23 16:38:10.122613 ffun-1.5.4/ffun/cli/application.py
+-rw-r--r--   0        0        0      439 2024-05-23 16:38:10.122613 ffun-1.5.4/ffun/cli/cli.py
+-rw-r--r--   0        0        0        0 2024-05-23 16:38:10.122613 ffun-1.5.4/ffun/cli/commands/__init__.py
+-rw-r--r--   0        0        0      732 2024-05-23 16:38:10.122613 ffun-1.5.4/ffun/cli/commands/configs.py
+-rw-r--r--   0        0        0     1050 2024-05-23 16:38:10.122613 ffun-1.5.4/ffun/cli/commands/entries.py
+-rw-r--r--   0        0        0     1393 2024-05-23 16:38:10.122613 ffun-1.5.4/ffun/cli/commands/failed_entries.py
+-rw-r--r--   0        0        0      538 2024-05-23 16:38:10.122613 ffun-1.5.4/ffun/cli/commands/meta.py
+-rw-r--r--   0        0        0     1001 2024-05-23 16:38:10.122613 ffun-1.5.4/ffun/cli/commands/supertokens.py
+-rw-r--r--   0        0        0      884 2024-05-23 16:38:10.122613 ffun-1.5.4/ffun/cli/commands/workers.py
+-rw-r--r--   0        0        0      209 2024-05-23 16:38:10.122613 ffun-1.5.4/ffun/cli/commands/yoyo.py
+-rw-r--r--   0        0        0     1333 2024-05-23 16:38:10.122613 ffun-1.5.4/ffun/conftest.py
+-rw-r--r--   0        0        0        0 2024-05-23 16:38:10.122613 ffun-1.5.4/ffun/core/__init__.py
+-rw-r--r--   0        0        0      631 2024-05-23 16:38:10.122613 ffun-1.5.4/ffun/core/api.py
+-rw-r--r--   0        0        0     3139 2024-05-23 16:38:10.122613 ffun-1.5.4/ffun/core/background_tasks.py
+-rw-r--r--   0        0        0      493 2024-05-23 16:38:10.122613 ffun-1.5.4/ffun/core/entities.py
+-rw-r--r--   0        0        0      552 2024-05-23 16:38:10.122613 ffun-1.5.4/ffun/core/errors.py
+-rw-r--r--   0        0        0     2773 2024-05-23 16:38:10.122613 ffun-1.5.4/ffun/core/json.py
+-rw-r--r--   0        0        0     5440 2024-05-23 16:38:10.122613 ffun-1.5.4/ffun/core/logging.py
+-rw-r--r--   0        0        0     1516 2024-05-23 16:38:10.122613 ffun-1.5.4/ffun/core/middlewares.py
+-rw-r--r--   0        0        0      882 2024-05-23 16:38:10.122613 ffun-1.5.4/ffun/core/migrations.py
+-rw-r--r--   0        0        0     4019 2024-05-23 16:38:10.122613 ffun-1.5.4/ffun/core/postgresql.py
+-rw-r--r--   0        0        0      695 2024-05-23 16:38:10.122613 ffun-1.5.4/ffun/core/register.py
+-rw-r--r--   0        0        0     1442 2024-05-23 16:38:10.122613 ffun-1.5.4/ffun/core/sentry.py
+-rw-r--r--   0        0        0      347 2024-05-23 16:38:10.122613 ffun-1.5.4/ffun/core/settings.py
+-rw-r--r--   0        0        0        0 2024-05-23 16:38:10.122613 ffun-1.5.4/ffun/core/tests/__init__.py
+-rw-r--r--   0        0        0     4551 2024-05-23 16:38:10.122613 ffun-1.5.4/ffun/core/tests/helpers.py
+-rw-r--r--   0        0        0       82 2024-05-23 16:38:10.122613 ffun-1.5.4/ffun/core/tests/make.py
+-rw-r--r--   0        0        0      486 2024-05-23 16:38:10.122613 ffun-1.5.4/ffun/core/text.py
+-rw-r--r--   0        0        0     1088 2024-05-23 16:38:10.122613 ffun-1.5.4/ffun/core/utils.py
+-rw-r--r--   0        0        0        0 2024-05-23 16:38:10.122613 ffun-1.5.4/ffun/domain/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-23 16:38:10.122613 ffun-1.5.4/ffun/domain/tests/__init__.py
+-rw-r--r--   0        0        0     6690 2024-05-23 16:38:10.122613 ffun-1.5.4/ffun/domain/tests/test_urls.py
+-rw-r--r--   0        0        0     4096 2024-05-23 16:38:10.122613 ffun-1.5.4/ffun/domain/urls.py
+-rw-r--r--   0        0        0        0 2024-05-23 16:38:10.122613 ffun-1.5.4/ffun/feeds/__init__.py
+-rw-r--r--   0        0        0      826 2024-05-23 16:38:10.122613 ffun-1.5.4/ffun/feeds/domain.py
+-rw-r--r--   0        0        0     1937 2024-05-23 16:38:10.122613 ffun-1.5.4/ffun/feeds/entities.py
+-rw-r--r--   0        0        0      131 2024-05-23 16:38:10.122613 ffun-1.5.4/ffun/feeds/errors.py
+-rw-r--r--   0        0        0     1027 2024-05-23 16:38:10.122613 ffun-1.5.4/ffun/feeds/migrations/20230329_01_ilwfq-feeds-table.py
+-rw-r--r--   0        0        0      641 2024-05-23 16:38:10.122613 ffun-1.5.4/ffun/feeds/migrations/20230426_01_IiF5m-add-title-and-description.py
+-rw-r--r--   0        0        0      561 2024-05-23 16:38:10.122613 ffun-1.5.4/ffun/feeds/migrations/20240504_01_vBDVJ-column-for-feed-unique-id.py
+-rw-r--r--   0        0        0      531 2024-05-23 16:38:10.122613 ffun-1.5.4/ffun/feeds/migrations/20240504_02_gEapd-fill-uids-for-feeds.py
+-rw-r--r--   0        0        0      725 2024-05-23 16:38:10.122613 ffun-1.5.4/ffun/feeds/migrations/20240512_01_jL7Mt-turn-on-unique-uids.py
+-rw-r--r--   0        0        0     4062 2024-05-23 16:38:10.122613 ffun-1.5.4/ffun/feeds/operations.py
+-rw-r--r--   0        0        0        0 2024-05-23 16:38:10.122613 ffun-1.5.4/ffun/feeds/tests/__init__.py
+-rw-r--r--   0        0        0     1512 2024-05-23 16:38:10.122613 ffun-1.5.4/ffun/feeds/tests/fixtures.py
+-rw-r--r--   0        0        0     1178 2024-05-23 16:38:10.122613 ffun-1.5.4/ffun/feeds/tests/make.py
+-rw-r--r--   0        0        0      445 2024-05-23 16:38:10.122613 ffun-1.5.4/ffun/feeds/tests/test_domain.py
+-rw-r--r--   0        0        0     7782 2024-05-23 16:38:10.122613 ffun-1.5.4/ffun/feeds/tests/test_operations.py
+-rw-r--r--   0        0        0        0 2024-05-23 16:38:10.122613 ffun-1.5.4/ffun/feeds_collections/__init__.py
+-rw-r--r--   0        0        0      495 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/feeds_collections/collections/artificial_intelligence.py
+-rw-r--r--   0        0        0     1357 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/feeds_collections/collections/gamedev.py
+-rw-r--r--   0        0        0      777 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/feeds_collections/domain.py
+-rw-r--r--   0        0        0      128 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/feeds_collections/entities.py
+-rw-r--r--   0        0        0      573 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/feeds_collections/predefines.py
+-rw-r--r--   0        0        0        0 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/feeds_collections/tests/__init__.py
+-rw-r--r--   0        0        0      684 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/feeds_collections/tests/fixtures.py
+-rw-r--r--   0        0        0        0 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/feeds_discoverer/__init__.py
+-rw-r--r--   0        0        0     3974 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/feeds_discoverer/domain.py
+-rw-r--r--   0        0        0        0 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/feeds_links/__init__.py
+-rw-r--r--   0        0        0      553 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/feeds_links/domain.py
+-rw-r--r--   0        0        0      163 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/feeds_links/entities.py
+-rw-r--r--   0        0        0      810 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/feeds_links/migrations/20230427_01_9HuHj-add-feeds-links.py
+-rw-r--r--   0        0        0     2326 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/feeds_links/operations.py
+-rw-r--r--   0        0        0        0 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/feeds_links/tests/__init__.py
+-rw-r--r--   0        0        0     2908 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/feeds_links/tests/test_operations.py
+-rw-r--r--   0        0        0        0 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/librarian/__init__.py
+-rw-r--r--   0        0        0     5182 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/librarian/background_processors.py
+-rw-r--r--   0        0        0     3759 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/librarian/domain.py
+-rw-r--r--   0        0        0      205 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/librarian/entities.py
+-rw-r--r--   0        0        0      217 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/librarian/errors.py
+-rw-r--r--   0        0        0     2101 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/librarian/migrations/20240313_01_Yv74T-processors-pointers.py
+-rw-r--r--   0        0        0     3035 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/librarian/migrations/20240319_01_MTJyn-migrate-to-processors-queue.py
+-rw-r--r--   0        0        0     5112 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/librarian/operations.py
+-rw-r--r--   0        0        0        0 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/librarian/processors/__init__.py
+-rw-r--r--   0        0        0     1255 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/librarian/processors/base.py
+-rw-r--r--   0        0        0     1548 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/librarian/processors/domain.py
+-rw-r--r--   0        0        0      468 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/librarian/processors/native_tags.py
+-rw-r--r--   0        0        0     3295 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/librarian/processors/openai_chat_3_5.py
+-rw-r--r--   0        0        0     4421 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/librarian/processors/openai_chat_3_5_functions.py
+-rw-r--r--   0        0        0        0 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/librarian/processors/tests/__init__.py
+-rw-r--r--   0        0        0     1139 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/librarian/processors/tests/test_upper_case_title.py
+-rw-r--r--   0        0        0      434 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/librarian/processors/upper_case_title.py
+-rw-r--r--   0        0        0     1089 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/librarian/settings.py
+-rw-r--r--   0        0        0        0 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/librarian/tests/__init__.py
+-rw-r--r--   0        0        0      845 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/librarian/tests/fixtures.py
+-rw-r--r--   0        0        0      487 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/librarian/tests/helpers.py
+-rw-r--r--   0        0        0      553 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/librarian/tests/make.py
+-rw-r--r--   0        0        0     4104 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/librarian/tests/test_background_processors.py
+-rw-r--r--   0        0        0    13605 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/librarian/tests/test_domain.py
+-rw-r--r--   0        0        0    14031 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/librarian/tests/test_operations.py
+-rw-r--r--   0        0        0        0 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/library/__init__.py
+-rw-r--r--   0        0        0     1509 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/library/domain.py
+-rw-r--r--   0        0        0     1168 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/library/entities.py
+-rw-r--r--   0        0        0      149 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/library/errors.py
+-rw-r--r--   0        0        0     1498 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/library/migrations/20230331_01_UsHwp-entries-table.py
+-rw-r--r--   0        0        0     1288 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/library/migrations/20230427_01_pv33u-fix-entries-unique-index.py
+-rw-r--r--   0        0        0      710 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/library/migrations/20230514_01_Bwb35-processed-state.py
+-rw-r--r--   0        0        0     1125 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/library/migrations/20240315_01_tWftt-optimize-l-entries.py
+-rw-r--r--   0        0        0     1003 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/library/migrations/20240503_01_Bmzw6-remove-l-entry-process-info.py
+-rw-r--r--   0        0        0     1194 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/library/migrations/20240506_01_My4vi-remove-duplicated-entries-from-feeds.py
+-rw-r--r--   0        0        0      784 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/library/migrations/20240506_02_zQdSl-fix-unique-index-on-l-entries.py
+-rw-r--r--   0        0        0     5926 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/library/operations.py
+-rw-r--r--   0        0        0        0 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/library/tests/__init__.py
+-rw-r--r--   0        0        0      799 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/library/tests/fixtures.py
+-rw-r--r--   0        0        0     1663 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/library/tests/make.py
+-rw-r--r--   0        0        0     1414 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/library/tests/test_domain.py
+-rw-r--r--   0        0        0    15331 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/library/tests/test_operations.py
+-rw-r--r--   0        0        0        0 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/loader/__init__.py
+-rw-r--r--   0        0        0     1218 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/loader/background_loader.py
+-rw-r--r--   0        0        0     5498 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/loader/domain.py
+-rw-r--r--   0        0        0       82 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/loader/entities.py
+-rw-r--r--   0        0        0      226 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/loader/errors.py
+-rw-r--r--   0        0        0      738 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/loader/migrations/20240522_01_xXZJ9-proxy-states-table.py
+-rw-r--r--   0        0        0     9568 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/loader/operations.py
+-rw-r--r--   0        0        0      647 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/loader/settings.py
+-rw-r--r--   0        0        0        0 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/loader/tests/__init__.py
+-rw-r--r--   0        0        0     9569 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/loader/tests/test_domain.py
+-rw-r--r--   0        0        0     3558 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/loader/tests/test_operations.py
+-rw-r--r--   0        0        0        0 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/markers/__init__.py
+-rw-r--r--   0        0        0      504 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/markers/domain.py
+-rw-r--r--   0        0        0       57 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/markers/entities.py
+-rw-r--r--   0        0        0      855 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/markers/migrations/20230419_01_9vMm5-markers-tables.py
+-rw-r--r--   0        0        0     2447 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/markers/operations.py
+-rw-r--r--   0        0        0        0 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/markers/tests/__init__.py
+-rw-r--r--   0        0        0     4835 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/markers/tests/test_operations.py
+-rw-r--r--   0        0        0        0 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/meta/__init__.py
+-rw-r--r--   0        0        0     3557 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/meta/domain.py
+-rw-r--r--   0        0        0      345 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/meta/migrations/20240512_01_0F799-unity-duplicated-feeds.py
+-rw-r--r--   0        0        0      246 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/meta/settings.py
+-rw-r--r--   0        0        0        0 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/meta/tests/__init__.py
+-rw-r--r--   0        0        0    15939 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/meta/tests/test_domain.py
+-rw-r--r--   0        0        0        0 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/ontology/__init__.py
+-rw-r--r--   0        0        0     3840 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/ontology/domain.py
+-rw-r--r--   0        0        0     1683 2024-05-23 16:38:10.126613 ffun-1.5.4/ffun/ontology/entities.py
+-rw-r--r--   0        0        0     1092 2024-05-23 16:38:10.130612 ffun-1.5.4/ffun/ontology/migrations/20230404_01_ZUBsm-ontology-tables.py
+-rw-r--r--   0        0        0      520 2024-05-23 16:38:10.130612 ffun-1.5.4/ffun/ontology/migrations/20230617_01_XDdNG-rename-tags-names-to-uid.py
+-rw-r--r--   0        0        0      799 2024-05-23 16:38:10.130612 ffun-1.5.4/ffun/ontology/migrations/20230617_02_L0MmA-tags-relationship-processor-tracking.py
+-rw-r--r--   0        0        0     1008 2024-05-23 16:38:10.130612 ffun-1.5.4/ffun/ontology/migrations/20230617_03_de7vS-tags-properties.py
+-rw-r--r--   0        0        0     6307 2024-05-23 16:38:10.130612 ffun-1.5.4/ffun/ontology/operations.py
+-rw-r--r--   0        0        0        0 2024-05-23 16:38:10.130612 ffun-1.5.4/ffun/ontology/tests/__init__.py
+-rw-r--r--   0        0        0      834 2024-05-23 16:38:10.130612 ffun-1.5.4/ffun/ontology/tests/fixtures.py
+-rw-r--r--   0        0        0      408 2024-05-23 16:38:10.130612 ffun-1.5.4/ffun/ontology/tests/helpers.py
+-rw-r--r--   0        0        0     9964 2024-05-23 16:38:10.130612 ffun-1.5.4/ffun/ontology/tests/test_operations.py
+-rw-r--r--   0        0        0        0 2024-05-23 16:38:10.130612 ffun-1.5.4/ffun/openai/__init__.py
+-rw-r--r--   0        0        0     5962 2024-05-23 16:38:10.130612 ffun-1.5.4/ffun/openai/client.py
+-rw-r--r--   0        0        0      612 2024-05-23 16:38:10.130612 ffun-1.5.4/ffun/openai/entities.py
+-rw-r--r--   0        0        0      150 2024-05-23 16:38:10.130612 ffun-1.5.4/ffun/openai/errors.py
+-rw-r--r--   0        0        0     7597 2024-05-23 16:38:10.130612 ffun-1.5.4/ffun/openai/keys_rotator.py
+-rw-r--r--   0        0        0     1919 2024-05-23 16:38:10.130612 ffun-1.5.4/ffun/openai/keys_statuses.py
+-rw-r--r--   0        0        0      372 2024-05-23 16:38:10.130612 ffun-1.5.4/ffun/openai/settings.py
+-rw-r--r--   0        0        0        0 2024-05-23 16:38:10.130612 ffun-1.5.4/ffun/openai/tests/__init__.py
+-rw-r--r--   0        0        0      130 2024-05-23 16:38:10.130612 ffun-1.5.4/ffun/openai/tests/conftest.py
+-rw-r--r--   0        0        0     2518 2024-05-23 16:38:10.130612 ffun-1.5.4/ffun/openai/tests/fixtures.py
+-rw-r--r--   0        0        0    19734 2024-05-23 16:38:10.130612 ffun-1.5.4/ffun/openai/tests/test_keys_rotator.py
+-rw-r--r--   0        0        0     2833 2024-05-23 16:38:10.130612 ffun-1.5.4/ffun/openai/tests/test_keys_statuses.py
+-rw-r--r--   0        0        0        0 2024-05-23 16:38:10.130612 ffun-1.5.4/ffun/parsers/__init__.py
+-rw-r--r--   0        0        0      228 2024-05-23 16:38:10.130612 ffun-1.5.4/ffun/parsers/domain.py
+-rw-r--r--   0        0        0      567 2024-05-23 16:38:10.130612 ffun-1.5.4/ffun/parsers/entities.py
+-rw-r--r--   0        0        0     2362 2024-05-23 16:38:10.130612 ffun-1.5.4/ffun/parsers/feed.py
+-rw-r--r--   0        0        0     1325 2024-05-23 16:38:10.130612 ffun-1.5.4/ffun/parsers/feedly.py
+-rw-r--r--   0        0        0        0 2024-05-23 16:38:10.130612 ffun-1.5.4/ffun/parsers/tests/__init__.py
+-rw-r--r--   0        0        0     1219 2024-05-23 16:38:10.130612 ffun-1.5.4/ffun/parsers/tests/feeds_fixtures/atom_with_relative_news_links.xml
+-rw-r--r--   0        0        0      639 2024-05-23 16:38:10.130612 ffun-1.5.4/ffun/parsers/tests/feeds_fixtures/atom_with_relative_news_links.xml.expected.json
+-rw-r--r--   0        0        0     4745 2024-05-23 16:38:10.130612 ffun-1.5.4/ffun/parsers/tests/feeds_fixtures/wordpress_rss_2_0_feed.xml
+-rw-r--r--   0        0        0     1072 2024-05-23 16:38:10.130612 ffun-1.5.4/ffun/parsers/tests/feeds_fixtures/wordpress_rss_2_0_feed.xml.expected.json
+-rw-r--r--   0        0        0      966 2024-05-23 16:38:10.130612 ffun-1.5.4/ffun/parsers/tests/make.py
+-rw-r--r--   0        0        0     1205 2024-05-23 16:38:10.130612 ffun-1.5.4/ffun/parsers/tests/test_feed.py
+-rw-r--r--   0        0        0        0 2024-05-23 16:38:10.130612 ffun-1.5.4/ffun/resources/__init__.py
+-rw-r--r--   0        0        0      769 2024-05-23 16:38:10.130612 ffun-1.5.4/ffun/resources/domain.py
+-rw-r--r--   0        0        0      280 2024-05-23 16:38:10.130612 ffun-1.5.4/ffun/resources/entities.py
+-rw-r--r--   0        0        0      120 2024-05-23 16:38:10.130612 ffun-1.5.4/ffun/resources/errors.py
+-rw-r--r--   0        0        0      865 2024-05-23 16:38:10.130612 ffun-1.5.4/ffun/resources/migrations/20230702_01_LEEES-resources-table.py
+-rw-r--r--   0        0        0     3984 2024-05-23 16:38:10.130612 ffun-1.5.4/ffun/resources/operations.py
+-rw-r--r--   0        0        0        0 2024-05-23 16:38:10.130612 ffun-1.5.4/ffun/resources/tests/__init__.py
+-rw-r--r--   0        0        0     1945 2024-05-23 16:38:10.130612 ffun-1.5.4/ffun/resources/tests/test_domain.py
+-rw-r--r--   0        0        0     9480 2024-05-23 16:38:10.130612 ffun-1.5.4/ffun/resources/tests/test_operations.py
+-rw-r--r--   0        0        0        0 2024-05-23 16:38:10.130612 ffun-1.5.4/ffun/scores/__init__.py
+-rw-r--r--   0        0        0      884 2024-05-23 16:38:10.130612 ffun-1.5.4/ffun/scores/domain.py
+-rw-r--r--   0        0        0      250 2024-05-23 16:38:10.130612 ffun-1.5.4/ffun/scores/entities.py
+-rw-r--r--   0        0        0      104 2024-05-23 16:38:10.130612 ffun-1.5.4/ffun/scores/errors.py
+-rw-r--r--   0        0        0      851 2024-05-23 16:38:10.130612 ffun-1.5.4/ffun/scores/migrations/20230417_01_0XYOQ-scores-tables.py
+-rw-r--r--   0        0        0      603 2024-05-23 16:38:10.130612 ffun-1.5.4/ffun/scores/migrations/20230813_01_l7qop-updated-at-field.py
+-rw-r--r--   0        0        0     2603 2024-05-23 16:38:10.130612 ffun-1.5.4/ffun/scores/operations.py
+-rw-r--r--   0        0        0        0 2024-05-23 16:38:10.130612 ffun-1.5.4/ffun/scores/tests/__init__.py
+-rw-r--r--   0        0        0     1239 2024-05-23 16:38:10.130612 ffun-1.5.4/ffun/scores/tests/test_domain.py
+-rw-r--r--   0        0        0     6810 2024-05-23 16:38:10.130612 ffun-1.5.4/ffun/scores/tests/test_operations.py
+-rw-r--r--   0        0        0        0 2024-05-23 16:38:10.130612 ffun-1.5.4/ffun/tags/__init__.py
+-rw-r--r--   0        0        0     1578 2024-05-23 16:38:10.130612 ffun-1.5.4/ffun/tags/converters.py
+-rw-r--r--   0        0        0        0 2024-05-23 16:38:10.130612 ffun-1.5.4/ffun/tags/tests/__init__.py
+-rw-r--r--   0        0        0     1352 2024-05-23 16:38:10.130612 ffun-1.5.4/ffun/tags/tests/test_converters.py
+-rw-r--r--   0        0        0        0 2024-05-23 16:38:10.130612 ffun-1.5.4/ffun/user_settings/__init__.py
+-rw-r--r--   0        0        0     1842 2024-05-23 16:38:10.130612 ffun-1.5.4/ffun/user_settings/domain.py
+-rw-r--r--   0        0        0       54 2024-05-23 16:38:10.130612 ffun-1.5.4/ffun/user_settings/entities.py
+-rw-r--r--   0        0        0      137 2024-05-23 16:38:10.130612 ffun-1.5.4/ffun/user_settings/errors.py
+-rw-r--r--   0        0        0      732 2024-05-23 16:38:10.130612 ffun-1.5.4/ffun/user_settings/migrations/20230701_01_7zBP0-settings-table.py
+-rw-r--r--   0        0        0      534 2024-05-23 16:38:10.130612 ffun-1.5.4/ffun/user_settings/migrations/20230911_01_5vjXI-index-to-search-by-value.py
+-rw-r--r--   0        0        0     1748 2024-05-23 16:38:10.130612 ffun-1.5.4/ffun/user_settings/operations.py
+-rw-r--r--   0        0        0      581 2024-05-23 16:38:10.130612 ffun-1.5.4/ffun/user_settings/settings.py
+-rw-r--r--   0        0        0      508 2024-05-23 16:38:10.130612 ffun-1.5.4/ffun/user_settings/tests/asserts.py
+-rw-r--r--   0        0        0     6956 2024-05-23 16:38:10.130612 ffun-1.5.4/ffun/user_settings/tests/test_domain.py
+-rw-r--r--   0        0        0     5492 2024-05-23 16:38:10.130612 ffun-1.5.4/ffun/user_settings/tests/test_operations.py
+-rw-r--r--   0        0        0     2297 2024-05-23 16:38:10.130612 ffun-1.5.4/ffun/user_settings/types.py
+-rw-r--r--   0        0        0      489 2024-05-23 16:38:10.130612 ffun-1.5.4/ffun/user_settings/values.py
+-rw-r--r--   0        0        0        0 2024-05-23 16:38:10.130612 ffun-1.5.4/ffun/users/__init__.py
+-rw-r--r--   0        0        0      586 2024-05-23 16:38:10.130612 ffun-1.5.4/ffun/users/domain.py
+-rw-r--r--   0        0        0      161 2024-05-23 16:38:10.130612 ffun-1.5.4/ffun/users/entities.py
+-rw-r--r--   0        0        0      111 2024-05-23 16:38:10.130612 ffun-1.5.4/ffun/users/errors.py
+-rw-r--r--   0        0        0      718 2024-05-23 16:38:10.130612 ffun-1.5.4/ffun/users/migrations/20230527_01_soIr3-users-mapping.py
+-rw-r--r--   0        0        0     1232 2024-05-23 16:38:10.130612 ffun-1.5.4/ffun/users/operations.py
+-rw-r--r--   0        0        0        0 2024-05-23 16:38:10.130612 ffun-1.5.4/ffun/users/tests/__init__.py
+-rw-r--r--   0        0        0     1101 2024-05-23 16:38:10.130612 ffun-1.5.4/ffun/users/tests/fixtures.py
+-rw-r--r--   0        0        0      348 2024-05-23 16:38:10.130612 ffun-1.5.4/ffun/users/tests/make.py
+-rw-r--r--   0        0        0     4263 2024-05-23 16:38:17.154599 ffun-1.5.4/pyproject.toml
+-rw-r--r--   0        0        0     2901 1970-01-01 00:00:00.000000 ffun-1.5.4/PKG-INFO
```

### Comparing `ffun-1.5.3/ffun/api/entities.py` & `ffun-1.5.4/ffun/api/entities.py`

 * *Files 0% similar despite different names*

```diff
@@ -111,15 +111,15 @@
             updatedAt=rule.updated_at,
         )
 
 
 class EntryInfo(BaseEntity):
     title: str
     body: str
-    url: str
+    url: str | None
     published_at: datetime.datetime
 
     @classmethod
     def from_internal(cls, entry: p_entities.EntryInfo) -> "EntryInfo":
         return cls(title=entry.title, body=entry.body, url=entry.external_url, published_at=entry.published_at)
```

### Comparing `ffun-1.5.3/ffun/api/http_handlers.py` & `ffun-1.5.4/ffun/api/http_handlers.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.3/ffun/application/application.py` & `ffun-1.5.4/ffun/application/application.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.3/ffun/application/settings.py` & `ffun-1.5.4/ffun/application/settings.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.3/ffun/application/user_settings.py` & `ffun-1.5.4/ffun/application/user_settings.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.3/ffun/application/workers.py` & `ffun-1.5.4/ffun/application/workers.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.3/ffun/auth/dependencies.py` & `ffun-1.5.4/ffun/auth/dependencies.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.3/ffun/auth/settings.py` & `ffun-1.5.4/ffun/auth/settings.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.3/ffun/auth/supertokens.py` & `ffun-1.5.4/ffun/auth/supertokens.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.3/ffun/cli/commands/configs.py` & `ffun-1.5.4/ffun/cli/commands/configs.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.3/ffun/cli/commands/entries.py` & `ffun-1.5.4/ffun/cli/commands/entries.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.3/ffun/cli/commands/failed_entries.py` & `ffun-1.5.4/ffun/cli/commands/failed_entries.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.3/ffun/cli/commands/meta.py` & `ffun-1.5.4/ffun/cli/commands/meta.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.3/ffun/cli/commands/supertokens.py` & `ffun-1.5.4/ffun/cli/commands/supertokens.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.3/ffun/cli/commands/workers.py` & `ffun-1.5.4/ffun/cli/commands/workers.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.3/ffun/conftest.py` & `ffun-1.5.4/ffun/conftest.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.3/ffun/core/api.py` & `ffun-1.5.4/ffun/core/api.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.3/ffun/core/background_tasks.py` & `ffun-1.5.4/ffun/core/background_tasks.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.3/ffun/core/errors.py` & `ffun-1.5.4/ffun/core/errors.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.3/ffun/core/json.py` & `ffun-1.5.4/ffun/core/json.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.3/ffun/core/logging.py` & `ffun-1.5.4/ffun/core/logging.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.3/ffun/core/middlewares.py` & `ffun-1.5.4/ffun/core/middlewares.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.3/ffun/core/migrations.py` & `ffun-1.5.4/ffun/core/migrations.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.3/ffun/core/postgresql.py` & `ffun-1.5.4/ffun/core/postgresql.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.3/ffun/core/register.py` & `ffun-1.5.4/ffun/core/register.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.3/ffun/core/sentry.py` & `ffun-1.5.4/ffun/core/sentry.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.3/ffun/core/tests/helpers.py` & `ffun-1.5.4/ffun/core/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.3/ffun/core/utils.py` & `ffun-1.5.4/ffun/core/utils.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.3/ffun/domain/tests/test_urls.py` & `ffun-1.5.4/ffun/domain/tests/test_urls.py`

 * *Files 4% similar despite different names*

```diff
@@ -70,14 +70,15 @@
             ("https://example.com/path/a/b?c=d", "https://example.com/path/a/b?c=d"),
             ("http://another.domain:666/path/a/b?c=d", "http://another.domain:666/path/a/b?c=d"),
             ("/path/a/b?c=d", "https://example.com/path/a/b?c=d"),
             (
                 "magnet:?xt=urn:btih:123456789abcdef0123456789abcdef0123456789&dn=Example+File.mp4&tr=udp%3A%2F%2Ftracker.example.com%3A80",  # noqa
                 "magnet:?xt=urn:btih:123456789abcdef0123456789abcdef0123456789&dn=Example+File.mp4&tr=udp%3A%2F%2Ftracker.example.com%3A80",  # noqa
             ),
+            ("http://www.usinenouvelle.comhttps://www.usine-digitale.fr/article/christophe", None),
         ],
     )
     def test(self, url: str, normalized_url: str) -> None:
         assert urls.normalize_external_url(url, original_url="https://example.com") == normalized_url
 
 
 class TestUrlToUid:
```

### Comparing `ffun-1.5.3/ffun/domain/urls.py` & `ffun-1.5.4/ffun/domain/urls.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 import re
 import unicodedata
 from urllib.parse import quote_plus, unquote
 
 from furl import furl
 from orderedmultidict import omdict
 
+from ffun.core import logging
+
+logger = logging.get_module_logger()
+
+
 RE_SCHEMA = re.compile(r"^(\w+):")
 
 
 # TODO: maybe switch to https://github.com/tktech/can_ada
 
 
 # TODO: add tests
@@ -26,19 +31,29 @@
     if "." not in url.split("/")[0]:
         # if there is no domain, just return the url
         return url
 
     return f"//{url}"
 
 
-def normalize_classic_url(url: str, original_url: str) -> str:
+def normalize_classic_url(url: str, original_url: str) -> str | None:
     url = _fake_schema_for_url(url)
     original_url = _fake_schema_for_url(original_url)
 
-    external_url = furl(url)
+    try:
+        external_url = furl(url)
+    except ValueError as e:
+        error = str(e)
+
+        logger.warning("invalid_url", url=url, error=error)
+
+        if "Invalid port" in error:
+            return None
+
+        raise
 
     f_original_url = furl(original_url)
 
     if not external_url.scheme:
         external_url.set(scheme=f_original_url.scheme)
 
     if not external_url.netloc:
@@ -56,15 +71,15 @@
     return url.startswith("magnet:")
 
 
 def normalize_magnetic_url(url: str) -> str:
     return url
 
 
-def normalize_external_url(url: str, original_url: str) -> str:
+def normalize_external_url(url: str, original_url: str) -> str | None:
     if is_magnetic_url(url):
         return normalize_magnetic_url(url)
 
     return normalize_classic_url(url, original_url)
 
 
 def url_to_uid(url: str) -> str:
```

### Comparing `ffun-1.5.3/ffun/feeds/domain.py` & `ffun-1.5.4/ffun/feeds/domain.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.3/ffun/feeds/entities.py` & `ffun-1.5.4/ffun/feeds/entities.py`

 * *Files 5% similar despite different names*

```diff
@@ -45,14 +45,15 @@
     protocol_unknown = 3000
     protocol_no_entries_in_feed = 3001
 
     proxy_could_not_resolve_host = 4001
     proxy_connection_refused = 4002
     proxy_connection_403 = 4003
     proxy_no_route_to_host = 4004
+    proxy_connection_502 = 4005
 
 
 class Feed(BaseEntity):
     id: uuid.UUID
     url: str
     state: FeedState = FeedState.not_loaded
     last_error: FeedError | None = None
```

### Comparing `ffun-1.5.3/ffun/feeds/migrations/20230329_01_ilwfq-feeds-table.py` & `ffun-1.5.4/ffun/feeds/migrations/20230329_01_ilwfq-feeds-table.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.3/ffun/feeds/migrations/20230426_01_IiF5m-add-title-and-description.py` & `ffun-1.5.4/ffun/feeds/migrations/20230426_01_IiF5m-add-title-and-description.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.3/ffun/feeds/migrations/20240504_01_vBDVJ-column-for-feed-unique-id.py` & `ffun-1.5.4/ffun/feeds/migrations/20240504_01_vBDVJ-column-for-feed-unique-id.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.3/ffun/feeds/migrations/20240504_02_gEapd-fill-uids-for-feeds.py` & `ffun-1.5.4/ffun/feeds/migrations/20240504_02_gEapd-fill-uids-for-feeds.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.3/ffun/feeds/migrations/20240512_01_jL7Mt-turn-on-unique-uids.py` & `ffun-1.5.4/ffun/feeds/migrations/20240512_01_jL7Mt-turn-on-unique-uids.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.3/ffun/feeds/operations.py` & `ffun-1.5.4/ffun/feeds/operations.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.3/ffun/feeds/tests/fixtures.py` & `ffun-1.5.4/ffun/feeds/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.3/ffun/feeds/tests/make.py` & `ffun-1.5.4/ffun/feeds/tests/make.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.3/ffun/feeds/tests/test_operations.py` & `ffun-1.5.4/ffun/feeds/tests/test_operations.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.3/ffun/feeds_collections/collections/gamedev.py` & `ffun-1.5.4/ffun/feeds_collections/collections/gamedev.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.3/ffun/feeds_collections/domain.py` & `ffun-1.5.4/ffun/feeds_collections/domain.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.3/ffun/feeds_collections/predefines.py` & `ffun-1.5.4/ffun/feeds_collections/predefines.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.3/ffun/feeds_collections/tests/fixtures.py` & `ffun-1.5.4/ffun/feeds_collections/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.3/ffun/feeds_discoverer/domain.py` & `ffun-1.5.4/ffun/feeds_discoverer/domain.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.3/ffun/feeds_links/domain.py` & `ffun-1.5.4/ffun/feeds_links/domain.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.3/ffun/feeds_links/migrations/20230427_01_9HuHj-add-feeds-links.py` & `ffun-1.5.4/ffun/feeds_links/migrations/20230427_01_9HuHj-add-feeds-links.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.3/ffun/feeds_links/operations.py` & `ffun-1.5.4/ffun/feeds_links/operations.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.3/ffun/feeds_links/tests/test_operations.py` & `ffun-1.5.4/ffun/feeds_links/tests/test_operations.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.3/ffun/librarian/background_processors.py` & `ffun-1.5.4/ffun/librarian/background_processors.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.3/ffun/librarian/domain.py` & `ffun-1.5.4/ffun/librarian/domain.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.3/ffun/librarian/migrations/20240313_01_Yv74T-processors-pointers.py` & `ffun-1.5.4/ffun/librarian/migrations/20240313_01_Yv74T-processors-pointers.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.3/ffun/librarian/migrations/20240319_01_MTJyn-migrate-to-processors-queue.py` & `ffun-1.5.4/ffun/librarian/migrations/20240319_01_MTJyn-migrate-to-processors-queue.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.3/ffun/librarian/operations.py` & `ffun-1.5.4/ffun/librarian/operations.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.3/ffun/librarian/processors/base.py` & `ffun-1.5.4/ffun/librarian/processors/base.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.3/ffun/librarian/processors/domain.py` & `ffun-1.5.4/ffun/librarian/processors/domain.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.3/ffun/librarian/processors/openai_chat_3_5.py` & `ffun-1.5.4/ffun/librarian/processors/openai_chat_3_5.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.3/ffun/librarian/processors/openai_chat_3_5_functions.py` & `ffun-1.5.4/ffun/librarian/processors/openai_chat_3_5_functions.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.3/ffun/librarian/processors/tests/test_upper_case_title.py` & `ffun-1.5.4/ffun/librarian/processors/tests/test_upper_case_title.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.3/ffun/librarian/settings.py` & `ffun-1.5.4/ffun/librarian/settings.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.3/ffun/librarian/tests/fixtures.py` & `ffun-1.5.4/ffun/librarian/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.3/ffun/librarian/tests/make.py` & `ffun-1.5.4/ffun/librarian/tests/make.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.3/ffun/librarian/tests/test_background_processors.py` & `ffun-1.5.4/ffun/librarian/tests/test_background_processors.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.3/ffun/librarian/tests/test_domain.py` & `ffun-1.5.4/ffun/librarian/tests/test_domain.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.3/ffun/librarian/tests/test_operations.py` & `ffun-1.5.4/ffun/librarian/tests/test_operations.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.3/ffun/library/domain.py` & `ffun-1.5.4/ffun/library/domain.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,11 +30,11 @@
 
     changes = []
 
     if new_external_url != entry.external_url:
         changes.append(
             EntryChange(id=entry.id, field="external_url", old_value=entry.external_url, new_value=new_external_url)
         )
-        if apply:
+        if apply and new_external_url is not None:
             await operations.update_external_url(entry.id, new_external_url)
 
     return changes
```

### Comparing `ffun-1.5.3/ffun/library/entities.py` & `ffun-1.5.4/ffun/library/entities.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.3/ffun/library/migrations/20230331_01_UsHwp-entries-table.py` & `ffun-1.5.4/ffun/library/migrations/20230331_01_UsHwp-entries-table.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.3/ffun/library/migrations/20230427_01_pv33u-fix-entries-unique-index.py` & `ffun-1.5.4/ffun/library/migrations/20230427_01_pv33u-fix-entries-unique-index.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.3/ffun/library/migrations/20230514_01_Bwb35-processed-state.py` & `ffun-1.5.4/ffun/library/migrations/20230514_01_Bwb35-processed-state.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.3/ffun/library/migrations/20240315_01_tWftt-optimize-l-entries.py` & `ffun-1.5.4/ffun/library/migrations/20240315_01_tWftt-optimize-l-entries.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.3/ffun/library/migrations/20240503_01_Bmzw6-remove-l-entry-process-info.py` & `ffun-1.5.4/ffun/library/migrations/20240503_01_Bmzw6-remove-l-entry-process-info.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.3/ffun/library/migrations/20240506_01_My4vi-remove-duplicated-entries-from-feeds.py` & `ffun-1.5.4/ffun/library/migrations/20240506_01_My4vi-remove-duplicated-entries-from-feeds.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.3/ffun/library/migrations/20240506_02_zQdSl-fix-unique-index-on-l-entries.py` & `ffun-1.5.4/ffun/library/migrations/20240506_02_zQdSl-fix-unique-index-on-l-entries.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.3/ffun/library/operations.py` & `ffun-1.5.4/ffun/library/operations.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.3/ffun/library/tests/fixtures.py` & `ffun-1.5.4/ffun/library/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.3/ffun/library/tests/make.py` & `ffun-1.5.4/ffun/library/tests/make.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.3/ffun/library/tests/test_domain.py` & `ffun-1.5.4/ffun/library/tests/test_domain.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.3/ffun/library/tests/test_operations.py` & `ffun-1.5.4/ffun/library/tests/test_operations.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.3/ffun/loader/background_loader.py` & `ffun-1.5.4/ffun/loader/background_loader.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,28 +1,34 @@
 import asyncio
 import datetime
 from typing import Any
 
-from ffun.core import logging
+from ffun.core import logging, utils
 from ffun.core.background_tasks import InfiniteTask
 from ffun.feeds import domain as f_domain
 from ffun.loader import domain
 from ffun.loader.settings import settings
 
 logger = logging.get_module_logger()
 
 
+# TODO: tests
 class FeedsLoader(InfiniteTask):
-    __slots__ = ("_loaders_number",)
+    __slots__ = ("_loaders_number", "_last_proxies_check")
 
     def __init__(self, loaders_number: int = settings.loaders_number, **kwargs: Any) -> None:
         super().__init__(**kwargs)
         self._loaders_number = loaders_number
+        self._last_proxies_check = datetime.datetime.fromtimestamp(0, tz=datetime.timezone.utc)
 
     async def single_run(self) -> None:
+        if utils.now() - self._last_proxies_check > settings.proxy_available_check_period:
+            await domain.check_proxies_availability()
+            self._last_proxies_check = utils.now()
+
         feeds = await f_domain.get_next_feeds_to_load(
             number=self._loaders_number, loaded_before=datetime.datetime.utcnow() - settings.minimum_period
         )
 
         tasks = [domain.process_feed(feed=feed) for feed in feeds]
 
         await asyncio.gather(*tasks, return_exceptions=True)
```

### Comparing `ffun-1.5.3/ffun/loader/domain.py` & `ffun-1.5.4/ffun/loader/operations.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,52 +1,39 @@
+import asyncio
 import ssl
-import uuid
 
 import anyio
 import httpx
-from furl import furl
+from pypika import PostgreSQLQuery
+from pypika import functions as pypika_fn
 
-from ffun.core import logging, utils
-from ffun.feeds import domain as f_domain
-from ffun.feeds.entities import Feed, FeedError, FeedState
-from ffun.feeds_collections import domain as fc_domain
-from ffun.feeds_links import domain as fl_domain
-from ffun.library import domain as l_domain
-from ffun.library import entities as l_entities
+from ffun.core import logging
+from ffun.core.postgresql import execute
+from ffun.feeds.entities import FeedError
 from ffun.loader import errors
-from ffun.loader.settings import Proxy, settings
-from ffun.meta import domain as meta_domain
+from ffun.loader.entities import ProxyState
+from ffun.loader.settings import Proxy
 from ffun.parsers import entities as p_entities
 from ffun.parsers.domain import parse_feed
 
 logger = logging.get_module_logger()
 
 
-_user_agent: str = "unknown"
-
-
-# TODO: tests
-def initialize(user_agent: str) -> None:
-    global _user_agent
-
-    _user_agent = user_agent
-
-
 # TODO: tests
 async def load_content(  # noqa: CFQ001, CCR001, C901 # pylint: disable=R0912, R0915
-    url: str, proxy: Proxy
+    url: str, proxy: Proxy, user_agent: str
 ) -> httpx.Response:
     error_code = FeedError.network_unknown
 
     log = logger.bind(url=url, proxy=proxy.name, function="load_content")
 
     try:
         log.info("loading_feed")
 
-        async with httpx.AsyncClient(proxies=proxy.url, headers={"user-agent": _user_agent}) as client:
+        async with httpx.AsyncClient(proxies=proxy.url, headers={"user-agent": user_agent}) as client:
             response = await client.get(url, follow_redirects=True)
 
     except httpx.RemoteProtocolError as e:
         message = str(e)
 
         if "illegal request line" in message:
             # TODO: at least part of such errors are caused by wrong HTTP protocol
@@ -150,14 +137,17 @@
             error_code = FeedError.proxy_connection_refused
         elif "TUN_ERR" in message and "EHOSTUNREACH" in message:
             log.warning("proxy_no_route_to_host")
             error_code = FeedError.proxy_no_route_to_host
         elif "403" in message:
             log.warning("proxy_connection_403")
             error_code = FeedError.proxy_connection_403
+        elif "502" in message:
+            log.warning("proxy_connection_502")
+            error_code = FeedError.proxy_connection_502
         else:
             log.exception("unknown_proxy_error_while_loading_feed")
 
         raise errors.LoadError(feed_error_code=error_code) from e
 
     except httpx.DecodingError as e:
         log.warning("network_decoding_error")
@@ -208,112 +198,57 @@
 
     if not feed_info.entries:
         raise errors.LoadError(feed_error_code=FeedError.protocol_no_entries_in_feed)
 
     return feed_info
 
 
-# TODO: tests
-async def load_content_with_proxies(url: str) -> httpx.Response:  # noqa: CCR001
-    url_object = furl(url)
-
-    first_exception = None
-
-    # We try different protocols because users often make mistakes in the urls
-    # to fix them we unity similar urls like http://example.com and https://example.com
-    # => we need to check both protocols
-    #
-    # For now it is straightforward solution, but it should work
-    # Most of the domains should support HTTPS => HTTP urls will not be used
-    # but in case of full problem with url, we'll be doing unnecessary requests
-    # and in case of HTTP-only urls we'll be doing unnecessary requests too
-    #
-    # TODO: build a separate system of choosing protocol for the url with caching and periodic checks
-    for protocol in ("https", "http"):
-        url_object.scheme = protocol
-
-        for proxy in settings.proxies:
-            try:
-                return await load_content(str(url_object), proxy)
-            except Exception as e:
-                if first_exception is None:
-                    first_exception = e
-
-    # in case of error raise the first exception occurred
-    # because we should use the most common proxy first
-    raise first_exception  # type: ignore
-
-
-async def detect_orphaned(feed_id: uuid.UUID) -> bool:
-    if await fc_domain.is_feed_in_collections(feed_id):
-        return False
-
-    if await fl_domain.has_linked_users(feed_id):
-        return False
-
-    logger.info("feed_has_no_linked_users")
-    await f_domain.mark_feed_as_orphaned(feed_id)
-
-    return True
-
-
-# TODO: tests
-async def extract_feed_info(feed: Feed) -> p_entities.FeedInfo | None:
+async def check_proxy(proxy: Proxy, url: str, user_agent: str) -> bool:
     try:
-        response = await load_content_with_proxies(feed.url)
-        content = await decode_content(response)
-        feed_info = await parse_content(content, original_url=feed.url)
-    except errors.LoadError as e:
-        logger.info("feed_load_error", error_code=e.feed_error_code)
-        await f_domain.mark_feed_as_failed(feed.id, state=FeedState.damaged, error=e.feed_error_code)
-        return None
-
-    logger.info("feed_loaded", entries_number=len(feed_info.entries))
-
-    return feed_info
+        async with httpx.AsyncClient(proxies=proxy.url, headers={"user-agent": user_agent}) as client:
+            response = await client.head(url)
+    except Exception as e:
+        logger.info("proxy_check_error", proxy=proxy.name, url=url, error=str(e))
+        return False
 
+    logger.info("proxy_check", proxy=proxy.name, url=url, status_code=response.status_code)
 
-async def sync_feed_info(feed: Feed, feed_info: p_entities.FeedInfo) -> None:
-    if feed_info.title == feed.title and feed_info.description == feed.description:
-        return
+    return response.status_code == 200
 
-    await f_domain.update_feed_info(feed.id, title=feed_info.title, description=feed_info.description)
 
+async def is_proxy_available(proxy: Proxy, anchors: list[str], user_agent: str) -> bool:
+    tasks = [check_proxy(proxy, url, user_agent) for url in anchors]
 
-async def store_entries(feed_id: uuid.UUID, entries: list[p_entities.EntryInfo]) -> None:
-    external_ids = [entry.external_id for entry in entries]
+    results = await asyncio.gather(*tasks, return_exceptions=True)
 
-    stored_entries_external_ids = await l_domain.check_stored_entries_by_external_ids(feed_id, external_ids)
+    return any(result for result in results)
 
-    entries_to_store = [entry for entry in entries if entry.external_id not in stored_entries_external_ids]
 
-    prepared_entries = [
-        l_entities.Entry(feed_id=feed_id, id=uuid.uuid4(), cataloged_at=utils.now(), **entry_info.model_dump())
-        for entry_info in entries_to_store
-    ]
+async def get_proxy_states(names: list[str]) -> dict[str, ProxyState]:
+    sql = """
+    SELECT name, state
+    FROM lr_proxy_states
+    WHERE name = ANY(%(names)s)
+    """
 
-    await l_domain.catalog_entries(entries=prepared_entries)
+    rows = await execute(sql, {"names": names})
 
-    logger.info("entries_stored", entries_number=len(prepared_entries))
+    states = {name: ProxyState.available for name in names}
 
+    for row in rows:
+        states[row["name"]] = ProxyState(row["state"])
 
-@logging.bound_function()
-async def process_feed(feed: Feed) -> None:
-    logger.info("loading_feed")
+    return states
 
-    if await detect_orphaned(feed.id):
-        return
 
-    feed_info = await extract_feed_info(feed)
-
-    if feed_info is None:
+async def update_proxy_states(states: dict[str, ProxyState]) -> None:
+    if not states:
         return
 
-    await sync_feed_info(feed, feed_info)
-
-    await store_entries(feed.id, feed_info.entries)
+    query = PostgreSQLQuery.into("lr_proxy_states").columns("name", "state", "updated_at")
 
-    await meta_domain.limit_entries_for_feed(feed.id)
+    for name, state in states.items():
+        query = query.insert(name, state, pypika_fn.Now())
 
-    await f_domain.mark_feed_as_loaded(feed.id)
+    query = query.on_conflict("name").do_update("state").do_update("updated_at", pypika_fn.Now())
 
-    logger.info("entries_loaded")
+    await execute(str(query))
```

### Comparing `ffun-1.5.3/ffun/loader/tests/test_domain.py` & `ffun-1.5.4/ffun/loader/tests/test_domain.py`

 * *Files 24% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 
 from ffun.core.tests.helpers import assert_logs
 from ffun.feeds import domain as f_domain
 from ffun.feeds import entities as f_entities
 from ffun.feeds_links import domain as fl_domain
 from ffun.library import domain as l_domain
 from ffun.library import entities as l_entities
-from ffun.loader.domain import detect_orphaned, process_feed, store_entries, sync_feed_info
+from ffun.loader.domain import check_proxies_availability, detect_orphaned, process_feed, store_entries, sync_feed_info
+from ffun.loader.settings import Proxy, settings
 from ffun.parsers import entities as p_entities
 from ffun.parsers.tests import make as p_make
 
 
 def assert_entriy_equal_to_info(entry_info: p_entities.EntryInfo, entry: l_entities.Entry) -> None:
     assert entry.title == entry_info.title
     assert entry.body == entry_info.body
@@ -240,7 +241,34 @@
             await process_feed(feed=saved_feed)
 
         assert_logs(logs, feed_has_no_entries_tail=0, feed_entries_tail_removed=1)
 
         loaded_entries = await l_domain.get_entries_by_filter([saved_feed.id], limit=n + 1)
 
         assert len(loaded_entries) == m
+
+
+class TestCheckProxiesAvailability:
+    @pytest.mark.asyncio
+    async def test_no_proxies(self, mocker: MockerFixture) -> None:
+        mocker.patch("ffun.loader.settings.settings.proxies", [])
+
+        is_proxy_available = mocker.patch("ffun.loader.operations.is_proxy_available")
+
+        await check_proxies_availability()
+
+        is_proxy_available.assert_not_called()
+
+    @pytest.mark.asyncio
+    async def test_proxies(self, mocker: MockerFixture) -> None:
+        n = 3
+
+        proxies = [Proxy(name=uuid.uuid4().hex, url=None) for _ in range(n)]
+
+        mocker.patch("ffun.loader.settings.settings.proxies", proxies)
+
+        is_proxy_available = mocker.patch("ffun.loader.operations.is_proxy_available")
+
+        await check_proxies_availability()
+
+        for proxy in proxies:
+            is_proxy_available.assert_any_call(proxy=proxy, anchors=settings.proxy_anchors, user_agent="unknown")
```

### Comparing `ffun-1.5.3/ffun/markers/migrations/20230419_01_9vMm5-markers-tables.py` & `ffun-1.5.4/ffun/markers/migrations/20230419_01_9vMm5-markers-tables.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.3/ffun/markers/operations.py` & `ffun-1.5.4/ffun/markers/operations.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.3/ffun/markers/tests/test_operations.py` & `ffun-1.5.4/ffun/markers/tests/test_operations.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.3/ffun/meta/domain.py` & `ffun-1.5.4/ffun/meta/domain.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.3/ffun/meta/tests/test_domain.py` & `ffun-1.5.4/ffun/meta/tests/test_domain.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.3/ffun/ontology/domain.py` & `ffun-1.5.4/ffun/ontology/domain.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.3/ffun/ontology/entities.py` & `ffun-1.5.4/ffun/ontology/entities.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.3/ffun/ontology/migrations/20230404_01_ZUBsm-ontology-tables.py` & `ffun-1.5.4/ffun/ontology/migrations/20230404_01_ZUBsm-ontology-tables.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.3/ffun/ontology/migrations/20230617_01_XDdNG-rename-tags-names-to-uid.py` & `ffun-1.5.4/ffun/ontology/migrations/20230617_01_XDdNG-rename-tags-names-to-uid.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.3/ffun/ontology/migrations/20230617_02_L0MmA-tags-relationship-processor-tracking.py` & `ffun-1.5.4/ffun/ontology/migrations/20230617_02_L0MmA-tags-relationship-processor-tracking.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.3/ffun/ontology/migrations/20230617_03_de7vS-tags-properties.py` & `ffun-1.5.4/ffun/ontology/migrations/20230617_03_de7vS-tags-properties.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.3/ffun/ontology/operations.py` & `ffun-1.5.4/ffun/ontology/operations.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.3/ffun/ontology/tests/fixtures.py` & `ffun-1.5.4/ffun/ontology/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.3/ffun/ontology/tests/test_operations.py` & `ffun-1.5.4/ffun/ontology/tests/test_operations.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.3/ffun/openai/client.py` & `ffun-1.5.4/ffun/openai/client.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.3/ffun/openai/entities.py` & `ffun-1.5.4/ffun/openai/entities.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.3/ffun/openai/keys_rotator.py` & `ffun-1.5.4/ffun/openai/keys_rotator.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.3/ffun/openai/keys_statuses.py` & `ffun-1.5.4/ffun/openai/keys_statuses.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.3/ffun/openai/tests/fixtures.py` & `ffun-1.5.4/ffun/openai/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.3/ffun/openai/tests/test_keys_rotator.py` & `ffun-1.5.4/ffun/openai/tests/test_keys_rotator.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.3/ffun/openai/tests/test_keys_statuses.py` & `ffun-1.5.4/ffun/openai/tests/test_keys_statuses.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.3/ffun/parsers/entities.py` & `ffun-1.5.4/ffun/parsers/entities.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import pydantic
 
 
 class EntryInfo(pydantic.BaseModel):
     title: str
     body: str
     external_id: str
-    external_url: str
+    external_url: str | None
     external_tags: set[str]
     published_at: datetime.datetime
 
     def log_info(self) -> dict[str, Any]:
         return {"title": self.title, "external_url": self.external_url}
```

### Comparing `ffun-1.5.3/ffun/parsers/feed.py` & `ffun-1.5.4/ffun/parsers/feed.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 # not the best solution, but it works for now
 # TODO: we should use more formal way to detect uniqueness of entry
 # TODO: external id must be normalized
 def _extract_external_id(entry: Any) -> str:
     return entry.get("link")  # type: ignore
 
 
-def _extract_external_url(entry: Any, original_url: str) -> str:
+def _extract_external_url(entry: Any, original_url: str) -> str | None:
     url = entry.get("link")
 
     return urls.normalize_external_url(url, original_url)
 
 
 def parse_feed(content: str, original_url: str) -> FeedInfo | None:
     channel = feedparser.parse(content)
```

### Comparing `ffun-1.5.3/ffun/parsers/feedly.py` & `ffun-1.5.4/ffun/parsers/feedly.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.3/ffun/parsers/tests/feeds_fixtures/atom_with_relative_news_links.xml` & `ffun-1.5.4/ffun/parsers/tests/feeds_fixtures/atom_with_relative_news_links.xml`

 * *Files identical despite different names*

### Comparing `ffun-1.5.3/ffun/parsers/tests/feeds_fixtures/atom_with_relative_news_links.xml.expected.json` & `ffun-1.5.4/ffun/parsers/tests/feeds_fixtures/atom_with_relative_news_links.xml.expected.json`

 * *Files identical despite different names*

### Comparing `ffun-1.5.3/ffun/parsers/tests/feeds_fixtures/wordpress_rss_2_0_feed.xml` & `ffun-1.5.4/ffun/parsers/tests/feeds_fixtures/wordpress_rss_2_0_feed.xml`

 * *Files identical despite different names*

### Comparing `ffun-1.5.3/ffun/parsers/tests/feeds_fixtures/wordpress_rss_2_0_feed.xml.expected.json` & `ffun-1.5.4/ffun/parsers/tests/feeds_fixtures/wordpress_rss_2_0_feed.xml.expected.json`

 * *Files identical despite different names*

### Comparing `ffun-1.5.3/ffun/parsers/tests/make.py` & `ffun-1.5.4/ffun/parsers/tests/make.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.3/ffun/parsers/tests/test_feed.py` & `ffun-1.5.4/ffun/parsers/tests/test_feed.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.3/ffun/resources/domain.py` & `ffun-1.5.4/ffun/resources/domain.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.3/ffun/resources/migrations/20230702_01_LEEES-resources-table.py` & `ffun-1.5.4/ffun/resources/migrations/20230702_01_LEEES-resources-table.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.3/ffun/resources/operations.py` & `ffun-1.5.4/ffun/resources/operations.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.3/ffun/resources/tests/test_domain.py` & `ffun-1.5.4/ffun/resources/tests/test_domain.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.3/ffun/resources/tests/test_operations.py` & `ffun-1.5.4/ffun/resources/tests/test_operations.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.3/ffun/scores/domain.py` & `ffun-1.5.4/ffun/scores/domain.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.3/ffun/scores/migrations/20230417_01_0XYOQ-scores-tables.py` & `ffun-1.5.4/ffun/scores/migrations/20230417_01_0XYOQ-scores-tables.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.3/ffun/scores/migrations/20230813_01_l7qop-updated-at-field.py` & `ffun-1.5.4/ffun/scores/migrations/20230813_01_l7qop-updated-at-field.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.3/ffun/scores/operations.py` & `ffun-1.5.4/ffun/scores/operations.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.3/ffun/scores/tests/test_domain.py` & `ffun-1.5.4/ffun/scores/tests/test_domain.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.3/ffun/scores/tests/test_operations.py` & `ffun-1.5.4/ffun/scores/tests/test_operations.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.3/ffun/tags/converters.py` & `ffun-1.5.4/ffun/tags/converters.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.3/ffun/tags/tests/test_converters.py` & `ffun-1.5.4/ffun/tags/tests/test_converters.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.3/ffun/user_settings/domain.py` & `ffun-1.5.4/ffun/user_settings/domain.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.3/ffun/user_settings/migrations/20230701_01_7zBP0-settings-table.py` & `ffun-1.5.4/ffun/user_settings/migrations/20230701_01_7zBP0-settings-table.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.3/ffun/user_settings/migrations/20230911_01_5vjXI-index-to-search-by-value.py` & `ffun-1.5.4/ffun/user_settings/migrations/20230911_01_5vjXI-index-to-search-by-value.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.3/ffun/user_settings/operations.py` & `ffun-1.5.4/ffun/user_settings/operations.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.3/ffun/user_settings/settings.py` & `ffun-1.5.4/ffun/user_settings/settings.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.3/ffun/user_settings/tests/test_domain.py` & `ffun-1.5.4/ffun/user_settings/tests/test_domain.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.3/ffun/user_settings/tests/test_operations.py` & `ffun-1.5.4/ffun/user_settings/tests/test_operations.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.3/ffun/user_settings/types.py` & `ffun-1.5.4/ffun/user_settings/types.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.3/ffun/users/domain.py` & `ffun-1.5.4/ffun/users/domain.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.3/ffun/users/migrations/20230527_01_soIr3-users-mapping.py` & `ffun-1.5.4/ffun/users/migrations/20230527_01_soIr3-users-mapping.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.3/ffun/users/operations.py` & `ffun-1.5.4/ffun/users/operations.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.3/ffun/users/tests/fixtures.py` & `ffun-1.5.4/ffun/users/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.3/pyproject.toml` & `ffun-1.5.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ffun"
-version = "1.5.3"
+version = "1.5.4"
 description = "Backend for the Feeds Fun — web-based news reader"
 repository = "https://github.com/Tiendil/feeds.fun"
 authors = ["Aliaksei Yaletski (Tiendil) <a.eletsky@gmail.com>"]
 license = " BSD-3-Clause"
 readme = "README.md"
 homepage = "https://feeds.fun"
 keywords = ["news", "news-reader", "news-aggregator",
```

### Comparing `ffun-1.5.3/PKG-INFO` & `ffun-1.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ffun
-Version: 1.5.3
+Version: 1.5.4
 Summary: Backend for the Feeds Fun — web-based news reader
 Home-page: https://feeds.fun
 License:  BSD-3-Clause
 Keywords: news,news-reader,news-aggregator,rss,rss-reader,rss-aggregator,feed,feed-reader,feed-aggregator,atom,self-hosted
 Author: Aliaksei Yaletski (Tiendil)
 Author-email: a.eletsky@gmail.com
 Requires-Python: >=3.11,<4.0
```


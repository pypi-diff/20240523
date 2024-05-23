# Comparing `tmp/sentry_sdk-2.3.0.tar.gz` & `tmp/sentry_sdk-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sentry_sdk-2.3.0.tar", last modified: Thu May 23 08:26:37 2024, max compression
+gzip compressed data, was "sentry_sdk-2.3.1.tar", last modified: Thu May 23 12:40:34 2024, max compression
```

## Comparing `sentry_sdk-2.3.0.tar` & `sentry_sdk-2.3.1.tar`

### file list

```diff
@@ -1,184 +1,184 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:26:37.739165 sentry_sdk-2.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    10173 2024-05-23 08:26:37.739165 sentry_sdk-2.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5325 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:26:37.707165 sentry_sdk-2.3.0/sentry_sdk/
--rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/sentry_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3066 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/sentry_sdk/_compat.py
--rw-r--r--   0 runner    (1001) docker     (127)     5382 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/sentry_sdk/_lru_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)    11259 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/sentry_sdk/_queue.py
--rw-r--r--   0 runner    (1001) docker     (127)     6701 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/sentry_sdk/_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     3745 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/sentry_sdk/_werkzeug.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:26:37.711166 sentry_sdk-2.3.0/sentry_sdk/ai/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/sentry_sdk/ai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2956 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/sentry_sdk/ai/monitoring.py
--rw-r--r--   0 runner    (1001) docker     (127)      961 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/sentry_sdk/ai/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10018 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/sentry_sdk/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/sentry_sdk/attachments.py
--rw-r--r--   0 runner    (1001) docker     (127)    29194 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/sentry_sdk/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    16248 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/sentry_sdk/consts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:26:37.711166 sentry_sdk-2.3.0/sentry_sdk/crons/
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/sentry_sdk/crons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/sentry_sdk/crons/api.py
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/sentry_sdk/crons/consts.py
--rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/sentry_sdk/crons/decorator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:26:37.711166 sentry_sdk-2.3.0/sentry_sdk/db/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/sentry_sdk/db/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:26:37.711166 sentry_sdk-2.3.0/sentry_sdk/db/explain_plan/
--rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/sentry_sdk/db/explain_plan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/sentry_sdk/db/explain_plan/django.py
--rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/sentry_sdk/db/explain_plan/sqlalchemy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/sentry_sdk/debug.py
--rw-r--r--   0 runner    (1001) docker     (127)     9923 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/sentry_sdk/envelope.py
--rw-r--r--   0 runner    (1001) docker     (127)    27085 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/sentry_sdk/hub.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:26:37.719165 sentry_sdk-2.3.0/sentry_sdk/integrations/
--rw-r--r--   0 runner    (1001) docker     (127)     7794 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/sentry_sdk/integrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3197 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/sentry_sdk/integrations/_asgi_common.py
--rw-r--r--   0 runner    (1001) docker     (127)     5636 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/sentry_sdk/integrations/_wsgi_common.py
--rw-r--r--   0 runner    (1001) docker     (127)    11565 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/sentry_sdk/integrations/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (127)     6446 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/sentry_sdk/integrations/anthropic.py
--rw-r--r--   0 runner    (1001) docker     (127)      922 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/sentry_sdk/integrations/argv.py
--rw-r--r--   0 runner    (1001) docker     (127)     5939 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/sentry_sdk/integrations/ariadne.py
--rw-r--r--   0 runner    (1001) docker     (127)     7200 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/sentry_sdk/integrations/arq.py
--rw-r--r--   0 runner    (1001) docker     (127)    11600 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/sentry_sdk/integrations/asgi.py
--rw-r--r--   0 runner    (1001) docker     (127)     3091 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/sentry_sdk/integrations/asyncio.py
--rw-r--r--   0 runner    (1001) docker     (127)     6180 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/sentry_sdk/integrations/asyncpg.py
--rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/sentry_sdk/integrations/atexit.py
--rw-r--r--   0 runner    (1001) docker     (127)    15627 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/sentry_sdk/integrations/aws_lambda.py
--rw-r--r--   0 runner    (1001) docker     (127)     5192 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/sentry_sdk/integrations/beam.py
--rw-r--r--   0 runner    (1001) docker     (127)     4475 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/sentry_sdk/integrations/boto3.py
--rw-r--r--   0 runner    (1001) docker     (127)     5800 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/sentry_sdk/integrations/bottle.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:26:37.723165 sentry_sdk-2.3.0/sentry_sdk/integrations/celery/
--rw-r--r--   0 runner    (1001) docker     (127)    17139 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/sentry_sdk/integrations/celery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9813 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/sentry_sdk/integrations/celery/beat.py
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/sentry_sdk/integrations/celery/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4721 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/sentry_sdk/integrations/chalice.py
--rw-r--r--   0 runner    (1001) docker     (127)     5149 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/sentry_sdk/integrations/clickhouse_driver.py
--rw-r--r--   0 runner    (1001) docker     (127)     6755 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/sentry_sdk/integrations/cloud_resource_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     9081 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/sentry_sdk/integrations/cohere.py
--rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/sentry_sdk/integrations/dedupe.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:26:37.723165 sentry_sdk-2.3.0/sentry_sdk/integrations/django/
--rw-r--r--   0 runner    (1001) docker     (127)    24043 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/sentry_sdk/integrations/django/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7691 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/sentry_sdk/integrations/django/asgi.py
--rw-r--r--   0 runner    (1001) docker     (127)     6081 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/sentry_sdk/integrations/django/caching.py
--rw-r--r--   0 runner    (1001) docker     (127)     5770 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/sentry_sdk/integrations/django/middleware.py
--rw-r--r--   0 runner    (1001) docker     (127)     3063 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/sentry_sdk/integrations/django/signals_handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5683 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/sentry_sdk/integrations/django/templates.py
--rw-r--r--   0 runner    (1001) docker     (127)     4957 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/sentry_sdk/integrations/django/transactions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2836 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/sentry_sdk/integrations/django/views.py
--rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/sentry_sdk/integrations/excepthook.py
--rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/sentry_sdk/integrations/executing.py
--rw-r--r--   0 runner    (1001) docker     (127)     9347 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/sentry_sdk/integrations/falcon.py
--rw-r--r--   0 runner    (1001) docker     (127)     4573 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/sentry_sdk/integrations/fastapi.py
--rw-r--r--   0 runner    (1001) docker     (127)     7706 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/sentry_sdk/integrations/flask.py
--rw-r--r--   0 runner    (1001) docker     (127)     8149 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/sentry_sdk/integrations/gcp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2906 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/sentry_sdk/integrations/gnu_backtrace.py
--rw-r--r--   0 runner    (1001) docker     (127)     4386 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/sentry_sdk/integrations/gql.py
--rw-r--r--   0 runner    (1001) docker     (127)     3636 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/sentry_sdk/integrations/graphene.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:26:37.723165 sentry_sdk-2.3.0/sentry_sdk/integrations/grpc/
--rw-r--r--   0 runner    (1001) docker     (127)     4979 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/sentry_sdk/integrations/grpc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:26:37.723165 sentry_sdk-2.3.0/sentry_sdk/integrations/grpc/aio/
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/sentry_sdk/integrations/grpc/aio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3075 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/sentry_sdk/integrations/grpc/aio/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3866 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/sentry_sdk/integrations/grpc/aio/server.py
--rw-r--r--   0 runner    (1001) docker     (127)     3249 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/sentry_sdk/integrations/grpc/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2389 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/sentry_sdk/integrations/grpc/server.py
--rw-r--r--   0 runner    (1001) docker     (127)     5199 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/sentry_sdk/integrations/httpx.py
--rw-r--r--   0 runner    (1001) docker     (127)     5260 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/sentry_sdk/integrations/huey.py
--rw-r--r--   0 runner    (1001) docker     (127)     6478 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/sentry_sdk/integrations/huggingface_hub.py
--rw-r--r--   0 runner    (1001) docker     (127)    17445 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/sentry_sdk/integrations/langchain.py
--rw-r--r--   0 runner    (1001) docker     (127)     9592 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/sentry_sdk/integrations/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     3011 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/sentry_sdk/integrations/loguru.py
--rw-r--r--   0 runner    (1001) docker     (127)      831 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/sentry_sdk/integrations/modules.py
--rw-r--r--   0 runner    (1001) docker     (127)    10249 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/sentry_sdk/integrations/openai.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:26:37.723165 sentry_sdk-2.3.0/sentry_sdk/integrations/opentelemetry/
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/sentry_sdk/integrations/opentelemetry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/sentry_sdk/integrations/opentelemetry/consts.py
--rw-r--r--   0 runner    (1001) docker     (127)     5830 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/sentry_sdk/integrations/opentelemetry/integration.py
--rw-r--r--   0 runner    (1001) docker     (127)     3731 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/sentry_sdk/integrations/opentelemetry/propagator.py
--rw-r--r--   0 runner    (1001) docker     (127)    12225 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/sentry_sdk/integrations/opentelemetry/span_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4539 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/sentry_sdk/integrations/pure_eval.py
--rw-r--r--   0 runner    (1001) docker     (127)     5994 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/sentry_sdk/integrations/pymongo.py
--rw-r--r--   0 runner    (1001) docker     (127)     7151 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/sentry_sdk/integrations/pyramid.py
--rw-r--r--   0 runner    (1001) docker     (127)     7193 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/sentry_sdk/integrations/quart.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:26:37.727165 sentry_sdk-2.3.0/sentry_sdk/integrations/redis/
--rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/sentry_sdk/integrations/redis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3649 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/sentry_sdk/integrations/redis/_async_common.py
--rw-r--r--   0 runner    (1001) docker     (127)     3439 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/sentry_sdk/integrations/redis/_sync_common.py
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/sentry_sdk/integrations/redis/consts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:26:37.727165 sentry_sdk-2.3.0/sentry_sdk/integrations/redis/modules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/sentry_sdk/integrations/redis/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/sentry_sdk/integrations/redis/modules/caches.py
--rw-r--r--   0 runner    (1001) docker     (127)     2046 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/sentry_sdk/integrations/redis/modules/queries.py
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/sentry_sdk/integrations/redis/rb.py
--rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/sentry_sdk/integrations/redis/redis.py
--rw-r--r--   0 runner    (1001) docker     (127)     3343 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/sentry_sdk/integrations/redis/redis_cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/sentry_sdk/integrations/redis/redis_py_cluster_legacy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3450 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/sentry_sdk/integrations/redis/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5297 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/sentry_sdk/integrations/rq.py
--rw-r--r--   0 runner    (1001) docker     (127)    13164 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/sentry_sdk/integrations/sanic.py
--rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/sentry_sdk/integrations/serverless.py
--rw-r--r--   0 runner    (1001) docker     (127)     2906 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/sentry_sdk/integrations/socket.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:26:37.727165 sentry_sdk-2.3.0/sentry_sdk/integrations/spark/
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/sentry_sdk/integrations/spark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8276 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/sentry_sdk/integrations/spark/spark_driver.py
--rw-r--r--   0 runner    (1001) docker     (127)     3747 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/sentry_sdk/integrations/spark/spark_worker.py
--rw-r--r--   0 runner    (1001) docker     (127)     4865 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/sentry_sdk/integrations/sqlalchemy.py
--rw-r--r--   0 runner    (1001) docker     (127)    23511 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/sentry_sdk/integrations/starlette.py
--rw-r--r--   0 runner    (1001) docker     (127)     9871 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/sentry_sdk/integrations/starlite.py
--rw-r--r--   0 runner    (1001) docker     (127)     8346 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/sentry_sdk/integrations/stdlib.py
--rw-r--r--   0 runner    (1001) docker     (127)    14566 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/sentry_sdk/integrations/strawberry.py
--rw-r--r--   0 runner    (1001) docker     (127)     4033 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/sentry_sdk/integrations/threading.py
--rw-r--r--   0 runner    (1001) docker     (127)     7185 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/sentry_sdk/integrations/tornado.py
--rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/sentry_sdk/integrations/trytond.py
--rw-r--r--   0 runner    (1001) docker     (127)     9870 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/sentry_sdk/integrations/wsgi.py
--rw-r--r--   0 runner    (1001) docker     (127)    29729 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/sentry_sdk/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     3720 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/sentry_sdk/monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)    33332 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/sentry_sdk/profiler.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/sentry_sdk/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    57822 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/sentry_sdk/scope.py
--rw-r--r--   0 runner    (1001) docker     (127)     5082 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/sentry_sdk/scrubber.py
--rw-r--r--   0 runner    (1001) docker     (127)    12729 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/sentry_sdk/serializer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5581 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/sentry_sdk/session.py
--rw-r--r--   0 runner    (1001) docker     (127)     7822 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/sentry_sdk/sessions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/sentry_sdk/spotlight.py
--rw-r--r--   0 runner    (1001) docker     (127)    39492 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/sentry_sdk/tracing.py
--rw-r--r--   0 runner    (1001) docker     (127)    21048 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/sentry_sdk/tracing_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    21002 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/sentry_sdk/transport.py
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/sentry_sdk/types.py
--rw-r--r--   0 runner    (1001) docker     (127)    56591 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/sentry_sdk/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4475 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/sentry_sdk/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:26:37.731165 sentry_sdk-2.3.0/sentry_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10173 2024-05-23 08:26:37.000000 sentry_sdk-2.3.0/sentry_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5364 2024-05-23 08:26:37.000000 sentry_sdk-2.3.0/sentry_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 08:26:37.000000 sentry_sdk-2.3.0/sentry_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 08:26:37.000000 sentry_sdk-2.3.0/sentry_sdk.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-05-23 08:26:37.000000 sentry_sdk-2.3.0/sentry_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-23 08:26:37.000000 sentry_sdk-2.3.0/sentry_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 08:26:37.739165 sentry_sdk-2.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3993 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:26:37.731165 sentry_sdk-2.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4975 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    23697 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/tests/test_basics.py
--rw-r--r--   0 runner    (1001) docker     (127)    36053 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3409 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/tests/test_conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    13795 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/tests/test_crons.py
--rw-r--r--   0 runner    (1001) docker     (127)     8057 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/tests/test_envelope.py
--rw-r--r--   0 runner    (1001) docker     (127)     8578 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/tests/test_exceptiongroup.py
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/tests/test_lru_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)    29128 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/tests/test_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     2563 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/tests/test_monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     8686 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/tests/test_new_scopes_compat.py
--rw-r--r--   0 runner    (1001) docker     (127)    17288 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/tests/test_new_scopes_compat_event.py
--rw-r--r--   0 runner    (1001) docker     (127)    23653 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/tests/test_profiler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2409 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/tests/test_propagationcontext.py
--rw-r--r--   0 runner    (1001) docker     (127)    26931 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/tests/test_scope.py
--rw-r--r--   0 runner    (1001) docker     (127)     5357 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/tests/test_scrubber.py
--rw-r--r--   0 runner    (1001) docker     (127)     4578 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/tests/test_serializer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4098 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/tests/test_sessions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/tests/test_spotlight.py
--rw-r--r--   0 runner    (1001) docker     (127)    18754 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/tests/test_transport.py
--rw-r--r--   0 runner    (1001) docker     (127)      760 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/tests/test_types.py
--rw-r--r--   0 runner    (1001) docker     (127)    26384 2024-05-23 08:26:29.000000 sentry_sdk-2.3.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 12:40:34.327058 sentry_sdk-2.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    10173 2024-05-23 12:40:34.327058 sentry_sdk-2.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5325 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 12:40:34.299058 sentry_sdk-2.3.1/sentry_sdk/
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/sentry_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3066 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/sentry_sdk/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5382 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/sentry_sdk/_lru_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11259 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/sentry_sdk/_queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6701 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/sentry_sdk/_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3745 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/sentry_sdk/_werkzeug.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 12:40:34.299058 sentry_sdk-2.3.1/sentry_sdk/ai/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/sentry_sdk/ai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2956 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/sentry_sdk/ai/monitoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/sentry_sdk/ai/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10018 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/sentry_sdk/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/sentry_sdk/attachments.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29194 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/sentry_sdk/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16248 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/sentry_sdk/consts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 12:40:34.303058 sentry_sdk-2.3.1/sentry_sdk/crons/
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/sentry_sdk/crons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/sentry_sdk/crons/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/sentry_sdk/crons/consts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/sentry_sdk/crons/decorator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 12:40:34.303058 sentry_sdk-2.3.1/sentry_sdk/db/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/sentry_sdk/db/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 12:40:34.303058 sentry_sdk-2.3.1/sentry_sdk/db/explain_plan/
+-rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/sentry_sdk/db/explain_plan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/sentry_sdk/db/explain_plan/django.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/sentry_sdk/db/explain_plan/sqlalchemy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/sentry_sdk/debug.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9923 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/sentry_sdk/envelope.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27085 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/sentry_sdk/hub.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 12:40:34.311058 sentry_sdk-2.3.1/sentry_sdk/integrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     7794 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/sentry_sdk/integrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3197 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/sentry_sdk/integrations/_asgi_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5636 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/sentry_sdk/integrations/_wsgi_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11565 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/sentry_sdk/integrations/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6446 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/sentry_sdk/integrations/anthropic.py
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/sentry_sdk/integrations/argv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5939 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/sentry_sdk/integrations/ariadne.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7200 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/sentry_sdk/integrations/arq.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11600 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/sentry_sdk/integrations/asgi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3091 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/sentry_sdk/integrations/asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6180 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/sentry_sdk/integrations/asyncpg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/sentry_sdk/integrations/atexit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15627 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/sentry_sdk/integrations/aws_lambda.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5192 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/sentry_sdk/integrations/beam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4475 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/sentry_sdk/integrations/boto3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5800 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/sentry_sdk/integrations/bottle.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 12:40:34.311058 sentry_sdk-2.3.1/sentry_sdk/integrations/celery/
+-rw-r--r--   0 runner    (1001) docker     (127)    17139 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/sentry_sdk/integrations/celery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9813 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/sentry_sdk/integrations/celery/beat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/sentry_sdk/integrations/celery/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4721 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/sentry_sdk/integrations/chalice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5149 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/sentry_sdk/integrations/clickhouse_driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6755 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/sentry_sdk/integrations/cloud_resource_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9081 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/sentry_sdk/integrations/cohere.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/sentry_sdk/integrations/dedupe.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 12:40:34.311058 sentry_sdk-2.3.1/sentry_sdk/integrations/django/
+-rw-r--r--   0 runner    (1001) docker     (127)    24043 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/sentry_sdk/integrations/django/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7691 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/sentry_sdk/integrations/django/asgi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6081 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/sentry_sdk/integrations/django/caching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5770 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/sentry_sdk/integrations/django/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3063 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/sentry_sdk/integrations/django/signals_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5683 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/sentry_sdk/integrations/django/templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4957 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/sentry_sdk/integrations/django/transactions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2836 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/sentry_sdk/integrations/django/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2419 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/sentry_sdk/integrations/excepthook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/sentry_sdk/integrations/executing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9347 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/sentry_sdk/integrations/falcon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4573 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/sentry_sdk/integrations/fastapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7706 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/sentry_sdk/integrations/flask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8149 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/sentry_sdk/integrations/gcp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2906 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/sentry_sdk/integrations/gnu_backtrace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4386 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/sentry_sdk/integrations/gql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3636 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/sentry_sdk/integrations/graphene.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 12:40:34.315058 sentry_sdk-2.3.1/sentry_sdk/integrations/grpc/
+-rw-r--r--   0 runner    (1001) docker     (127)     4979 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/sentry_sdk/integrations/grpc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 12:40:34.315058 sentry_sdk-2.3.1/sentry_sdk/integrations/grpc/aio/
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/sentry_sdk/integrations/grpc/aio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3075 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/sentry_sdk/integrations/grpc/aio/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3866 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/sentry_sdk/integrations/grpc/aio/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3249 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/sentry_sdk/integrations/grpc/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2389 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/sentry_sdk/integrations/grpc/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5199 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/sentry_sdk/integrations/httpx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5260 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/sentry_sdk/integrations/huey.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6478 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/sentry_sdk/integrations/huggingface_hub.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17445 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/sentry_sdk/integrations/langchain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9592 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/sentry_sdk/integrations/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3011 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/sentry_sdk/integrations/loguru.py
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/sentry_sdk/integrations/modules.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10249 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/sentry_sdk/integrations/openai.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 12:40:34.315058 sentry_sdk-2.3.1/sentry_sdk/integrations/opentelemetry/
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/sentry_sdk/integrations/opentelemetry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/sentry_sdk/integrations/opentelemetry/consts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5830 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/sentry_sdk/integrations/opentelemetry/integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3731 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/sentry_sdk/integrations/opentelemetry/propagator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12225 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/sentry_sdk/integrations/opentelemetry/span_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4539 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/sentry_sdk/integrations/pure_eval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5994 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/sentry_sdk/integrations/pymongo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7151 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/sentry_sdk/integrations/pyramid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7193 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/sentry_sdk/integrations/quart.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 12:40:34.315058 sentry_sdk-2.3.1/sentry_sdk/integrations/redis/
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/sentry_sdk/integrations/redis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3649 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/sentry_sdk/integrations/redis/_async_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3439 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/sentry_sdk/integrations/redis/_sync_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/sentry_sdk/integrations/redis/consts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 12:40:34.315058 sentry_sdk-2.3.1/sentry_sdk/integrations/redis/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/sentry_sdk/integrations/redis/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/sentry_sdk/integrations/redis/modules/caches.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2046 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/sentry_sdk/integrations/redis/modules/queries.py
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/sentry_sdk/integrations/redis/rb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/sentry_sdk/integrations/redis/redis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3343 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/sentry_sdk/integrations/redis/redis_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/sentry_sdk/integrations/redis/redis_py_cluster_legacy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/sentry_sdk/integrations/redis/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5297 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/sentry_sdk/integrations/rq.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13164 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/sentry_sdk/integrations/sanic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/sentry_sdk/integrations/serverless.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2906 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/sentry_sdk/integrations/socket.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 12:40:34.315058 sentry_sdk-2.3.1/sentry_sdk/integrations/spark/
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/sentry_sdk/integrations/spark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8276 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/sentry_sdk/integrations/spark/spark_driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3747 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/sentry_sdk/integrations/spark/spark_worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4865 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/sentry_sdk/integrations/sqlalchemy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23511 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/sentry_sdk/integrations/starlette.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9871 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/sentry_sdk/integrations/starlite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8346 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/sentry_sdk/integrations/stdlib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14566 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/sentry_sdk/integrations/strawberry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4033 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/sentry_sdk/integrations/threading.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7185 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/sentry_sdk/integrations/tornado.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/sentry_sdk/integrations/trytond.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9870 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/sentry_sdk/integrations/wsgi.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29729 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/sentry_sdk/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3720 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/sentry_sdk/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33332 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/sentry_sdk/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/sentry_sdk/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    57822 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/sentry_sdk/scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5082 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/sentry_sdk/scrubber.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12729 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/sentry_sdk/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5581 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/sentry_sdk/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7822 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/sentry_sdk/sessions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/sentry_sdk/spotlight.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39492 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/sentry_sdk/tracing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21048 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/sentry_sdk/tracing_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21002 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/sentry_sdk/transport.py
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/sentry_sdk/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56591 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/sentry_sdk/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4475 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/sentry_sdk/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 12:40:34.319058 sentry_sdk-2.3.1/sentry_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10173 2024-05-23 12:40:34.000000 sentry_sdk-2.3.1/sentry_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5364 2024-05-23 12:40:34.000000 sentry_sdk-2.3.1/sentry_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 12:40:34.000000 sentry_sdk-2.3.1/sentry_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 12:40:34.000000 sentry_sdk-2.3.1/sentry_sdk.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-05-23 12:40:34.000000 sentry_sdk-2.3.1/sentry_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-23 12:40:34.000000 sentry_sdk-2.3.1/sentry_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 12:40:34.327058 sentry_sdk-2.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3993 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 12:40:34.319058 sentry_sdk-2.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4975 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23697 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/tests/test_basics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36053 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3409 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/tests/test_conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13795 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/tests/test_crons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8057 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/tests/test_envelope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8578 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/tests/test_exceptiongroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/tests/test_lru_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29128 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/tests/test_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2563 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/tests/test_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8686 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/tests/test_new_scopes_compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17288 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/tests/test_new_scopes_compat_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23653 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/tests/test_profiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2409 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/tests/test_propagationcontext.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26931 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/tests/test_scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5357 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/tests/test_scrubber.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4578 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/tests/test_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4098 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/tests/test_sessions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/tests/test_spotlight.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18754 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/tests/test_transport.py
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/tests/test_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26384 2024-05-23 12:40:25.000000 sentry_sdk-2.3.1/tests/test_utils.py
```

### Comparing `sentry_sdk-2.3.0/LICENSE` & `sentry_sdk-2.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.3.0/PKG-INFO` & `sentry_sdk-2.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sentry-sdk
-Version: 2.3.0
+Version: 2.3.1
 Summary: Python client for Sentry (https://sentry.io)
 Home-page: https://github.com/getsentry/sentry-python
 Author: Sentry Team and Contributors
 Author-email: hello@sentry.io
 License: MIT
 Project-URL: Documentation, https://docs.sentry.io/platforms/python/
 Project-URL: Changelog, https://github.com/getsentry/sentry-python/blob/master/CHANGELOG.md
```

### Comparing `sentry_sdk-2.3.0/README.md` & `sentry_sdk-2.3.1/README.md`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.3.0/sentry_sdk/__init__.py` & `sentry_sdk-2.3.1/sentry_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.3.0/sentry_sdk/_compat.py` & `sentry_sdk-2.3.1/sentry_sdk/_compat.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.3.0/sentry_sdk/_lru_cache.py` & `sentry_sdk-2.3.1/sentry_sdk/_lru_cache.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.3.0/sentry_sdk/_queue.py` & `sentry_sdk-2.3.1/sentry_sdk/_queue.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.3.0/sentry_sdk/_types.py` & `sentry_sdk-2.3.1/sentry_sdk/_types.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.3.0/sentry_sdk/_werkzeug.py` & `sentry_sdk-2.3.1/sentry_sdk/_werkzeug.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.3.0/sentry_sdk/ai/monitoring.py` & `sentry_sdk-2.3.1/sentry_sdk/ai/monitoring.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.3.0/sentry_sdk/ai/utils.py` & `sentry_sdk-2.3.1/sentry_sdk/ai/utils.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.3.0/sentry_sdk/api.py` & `sentry_sdk-2.3.1/sentry_sdk/api.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.3.0/sentry_sdk/attachments.py` & `sentry_sdk-2.3.1/sentry_sdk/attachments.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.3.0/sentry_sdk/client.py` & `sentry_sdk-2.3.1/sentry_sdk/client.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.3.0/sentry_sdk/consts.py` & `sentry_sdk-2.3.1/sentry_sdk/consts.py`

 * *Files 0% similar despite different names*

```diff
@@ -504,8 +504,8 @@
     return dict(zip(a.args[-len(defaults) :], defaults))
 
 
 DEFAULT_OPTIONS = _get_default_options()
 del _get_default_options
 
 
-VERSION = "2.3.0"
+VERSION = "2.3.1"
```

### Comparing `sentry_sdk-2.3.0/sentry_sdk/crons/api.py` & `sentry_sdk-2.3.1/sentry_sdk/crons/api.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.3.0/sentry_sdk/crons/decorator.py` & `sentry_sdk-2.3.1/sentry_sdk/crons/decorator.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.3.0/sentry_sdk/db/explain_plan/__init__.py` & `sentry_sdk-2.3.1/sentry_sdk/db/explain_plan/__init__.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.3.0/sentry_sdk/db/explain_plan/django.py` & `sentry_sdk-2.3.1/sentry_sdk/db/explain_plan/django.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.3.0/sentry_sdk/db/explain_plan/sqlalchemy.py` & `sentry_sdk-2.3.1/sentry_sdk/db/explain_plan/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.3.0/sentry_sdk/debug.py` & `sentry_sdk-2.3.1/sentry_sdk/debug.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.3.0/sentry_sdk/envelope.py` & `sentry_sdk-2.3.1/sentry_sdk/envelope.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.3.0/sentry_sdk/hub.py` & `sentry_sdk-2.3.1/sentry_sdk/hub.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.3.0/sentry_sdk/integrations/__init__.py` & `sentry_sdk-2.3.1/sentry_sdk/integrations/__init__.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.3.0/sentry_sdk/integrations/_asgi_common.py` & `sentry_sdk-2.3.1/sentry_sdk/integrations/_asgi_common.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.3.0/sentry_sdk/integrations/_wsgi_common.py` & `sentry_sdk-2.3.1/sentry_sdk/integrations/_wsgi_common.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.3.0/sentry_sdk/integrations/aiohttp.py` & `sentry_sdk-2.3.1/sentry_sdk/integrations/aiohttp.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.3.0/sentry_sdk/integrations/anthropic.py` & `sentry_sdk-2.3.1/sentry_sdk/integrations/anthropic.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.3.0/sentry_sdk/integrations/argv.py` & `sentry_sdk-2.3.1/sentry_sdk/integrations/argv.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.3.0/sentry_sdk/integrations/ariadne.py` & `sentry_sdk-2.3.1/sentry_sdk/integrations/ariadne.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.3.0/sentry_sdk/integrations/arq.py` & `sentry_sdk-2.3.1/sentry_sdk/integrations/arq.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.3.0/sentry_sdk/integrations/asgi.py` & `sentry_sdk-2.3.1/sentry_sdk/integrations/asgi.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.3.0/sentry_sdk/integrations/asyncio.py` & `sentry_sdk-2.3.1/sentry_sdk/integrations/asyncio.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.3.0/sentry_sdk/integrations/asyncpg.py` & `sentry_sdk-2.3.1/sentry_sdk/integrations/asyncpg.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.3.0/sentry_sdk/integrations/atexit.py` & `sentry_sdk-2.3.1/sentry_sdk/integrations/atexit.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.3.0/sentry_sdk/integrations/aws_lambda.py` & `sentry_sdk-2.3.1/sentry_sdk/integrations/aws_lambda.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.3.0/sentry_sdk/integrations/beam.py` & `sentry_sdk-2.3.1/sentry_sdk/integrations/beam.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.3.0/sentry_sdk/integrations/boto3.py` & `sentry_sdk-2.3.1/sentry_sdk/integrations/boto3.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.3.0/sentry_sdk/integrations/bottle.py` & `sentry_sdk-2.3.1/sentry_sdk/integrations/bottle.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.3.0/sentry_sdk/integrations/celery/__init__.py` & `sentry_sdk-2.3.1/sentry_sdk/integrations/celery/__init__.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.3.0/sentry_sdk/integrations/celery/beat.py` & `sentry_sdk-2.3.1/sentry_sdk/integrations/celery/beat.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.3.0/sentry_sdk/integrations/celery/utils.py` & `sentry_sdk-2.3.1/sentry_sdk/integrations/celery/utils.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.3.0/sentry_sdk/integrations/chalice.py` & `sentry_sdk-2.3.1/sentry_sdk/integrations/chalice.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.3.0/sentry_sdk/integrations/clickhouse_driver.py` & `sentry_sdk-2.3.1/sentry_sdk/integrations/clickhouse_driver.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.3.0/sentry_sdk/integrations/cloud_resource_context.py` & `sentry_sdk-2.3.1/sentry_sdk/integrations/cloud_resource_context.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.3.0/sentry_sdk/integrations/cohere.py` & `sentry_sdk-2.3.1/sentry_sdk/integrations/cohere.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.3.0/sentry_sdk/integrations/dedupe.py` & `sentry_sdk-2.3.1/sentry_sdk/integrations/dedupe.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.3.0/sentry_sdk/integrations/django/__init__.py` & `sentry_sdk-2.3.1/sentry_sdk/integrations/django/__init__.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.3.0/sentry_sdk/integrations/django/asgi.py` & `sentry_sdk-2.3.1/sentry_sdk/integrations/django/asgi.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.3.0/sentry_sdk/integrations/django/caching.py` & `sentry_sdk-2.3.1/sentry_sdk/integrations/django/caching.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.3.0/sentry_sdk/integrations/django/middleware.py` & `sentry_sdk-2.3.1/sentry_sdk/integrations/django/middleware.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.3.0/sentry_sdk/integrations/django/signals_handlers.py` & `sentry_sdk-2.3.1/sentry_sdk/integrations/django/signals_handlers.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.3.0/sentry_sdk/integrations/django/templates.py` & `sentry_sdk-2.3.1/sentry_sdk/integrations/django/templates.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.3.0/sentry_sdk/integrations/django/transactions.py` & `sentry_sdk-2.3.1/sentry_sdk/integrations/django/transactions.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.3.0/sentry_sdk/integrations/django/views.py` & `sentry_sdk-2.3.1/sentry_sdk/integrations/django/views.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.3.0/sentry_sdk/integrations/excepthook.py` & `sentry_sdk-2.3.1/sentry_sdk/integrations/excepthook.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import sys
 
 import sentry_sdk
 from sentry_sdk.utils import (
     capture_internal_exceptions,
-    ensure_integration_enabled,
     event_from_exception,
 )
 from sentry_sdk.integrations import Integration
 
 from sentry_sdk._types import TYPE_CHECKING
 
 if TYPE_CHECKING:
@@ -43,19 +42,24 @@
     def setup_once():
         # type: () -> None
         sys.excepthook = _make_excepthook(sys.excepthook)
 
 
 def _make_excepthook(old_excepthook):
     # type: (Excepthook) -> Excepthook
-    @ensure_integration_enabled(ExcepthookIntegration, old_excepthook)
     def sentry_sdk_excepthook(type_, value, traceback):
         # type: (Type[BaseException], BaseException, Optional[TracebackType]) -> None
         integration = sentry_sdk.get_client().get_integration(ExcepthookIntegration)
 
+        # Note: If  we replace this with ensure_integration_enabled then
+        # we break the exceptiongroup backport;
+        # See: https://github.com/getsentry/sentry-python/issues/3097
+        if integration is None:
+            return old_excepthook(type_, value, traceback)
+
         if _should_send(integration.always_run):
             with capture_internal_exceptions():
                 event, hint = event_from_exception(
                     (type_, value, traceback),
                     client_options=sentry_sdk.get_client().options,
                     mechanism={"type": "excepthook", "handled": False},
                 )
```

### Comparing `sentry_sdk-2.3.0/sentry_sdk/integrations/executing.py` & `sentry_sdk-2.3.1/sentry_sdk/integrations/executing.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.3.0/sentry_sdk/integrations/falcon.py` & `sentry_sdk-2.3.1/sentry_sdk/integrations/falcon.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.3.0/sentry_sdk/integrations/fastapi.py` & `sentry_sdk-2.3.1/sentry_sdk/integrations/fastapi.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.3.0/sentry_sdk/integrations/flask.py` & `sentry_sdk-2.3.1/sentry_sdk/integrations/flask.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.3.0/sentry_sdk/integrations/gcp.py` & `sentry_sdk-2.3.1/sentry_sdk/integrations/gcp.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.3.0/sentry_sdk/integrations/gnu_backtrace.py` & `sentry_sdk-2.3.1/sentry_sdk/integrations/gnu_backtrace.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.3.0/sentry_sdk/integrations/gql.py` & `sentry_sdk-2.3.1/sentry_sdk/integrations/gql.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.3.0/sentry_sdk/integrations/graphene.py` & `sentry_sdk-2.3.1/sentry_sdk/integrations/graphene.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.3.0/sentry_sdk/integrations/grpc/__init__.py` & `sentry_sdk-2.3.1/sentry_sdk/integrations/grpc/__init__.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.3.0/sentry_sdk/integrations/grpc/aio/client.py` & `sentry_sdk-2.3.1/sentry_sdk/integrations/grpc/aio/client.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.3.0/sentry_sdk/integrations/grpc/aio/server.py` & `sentry_sdk-2.3.1/sentry_sdk/integrations/grpc/aio/server.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.3.0/sentry_sdk/integrations/grpc/client.py` & `sentry_sdk-2.3.1/sentry_sdk/integrations/grpc/client.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.3.0/sentry_sdk/integrations/grpc/server.py` & `sentry_sdk-2.3.1/sentry_sdk/integrations/grpc/server.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.3.0/sentry_sdk/integrations/httpx.py` & `sentry_sdk-2.3.1/sentry_sdk/integrations/httpx.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.3.0/sentry_sdk/integrations/huey.py` & `sentry_sdk-2.3.1/sentry_sdk/integrations/huey.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.3.0/sentry_sdk/integrations/huggingface_hub.py` & `sentry_sdk-2.3.1/sentry_sdk/integrations/huggingface_hub.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.3.0/sentry_sdk/integrations/langchain.py` & `sentry_sdk-2.3.1/sentry_sdk/integrations/langchain.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.3.0/sentry_sdk/integrations/logging.py` & `sentry_sdk-2.3.1/sentry_sdk/integrations/logging.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.3.0/sentry_sdk/integrations/loguru.py` & `sentry_sdk-2.3.1/sentry_sdk/integrations/loguru.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.3.0/sentry_sdk/integrations/modules.py` & `sentry_sdk-2.3.1/sentry_sdk/integrations/modules.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.3.0/sentry_sdk/integrations/openai.py` & `sentry_sdk-2.3.1/sentry_sdk/integrations/openai.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.3.0/sentry_sdk/integrations/opentelemetry/integration.py` & `sentry_sdk-2.3.1/sentry_sdk/integrations/opentelemetry/integration.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.3.0/sentry_sdk/integrations/opentelemetry/propagator.py` & `sentry_sdk-2.3.1/sentry_sdk/integrations/opentelemetry/propagator.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.3.0/sentry_sdk/integrations/opentelemetry/span_processor.py` & `sentry_sdk-2.3.1/sentry_sdk/integrations/opentelemetry/span_processor.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.3.0/sentry_sdk/integrations/pure_eval.py` & `sentry_sdk-2.3.1/sentry_sdk/integrations/pure_eval.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.3.0/sentry_sdk/integrations/pymongo.py` & `sentry_sdk-2.3.1/sentry_sdk/integrations/pymongo.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.3.0/sentry_sdk/integrations/pyramid.py` & `sentry_sdk-2.3.1/sentry_sdk/integrations/pyramid.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.3.0/sentry_sdk/integrations/quart.py` & `sentry_sdk-2.3.1/sentry_sdk/integrations/quart.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.3.0/sentry_sdk/integrations/redis/__init__.py` & `sentry_sdk-2.3.1/sentry_sdk/integrations/redis/__init__.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.3.0/sentry_sdk/integrations/redis/_async_common.py` & `sentry_sdk-2.3.1/sentry_sdk/integrations/redis/_async_common.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.3.0/sentry_sdk/integrations/redis/_sync_common.py` & `sentry_sdk-2.3.1/sentry_sdk/integrations/redis/_sync_common.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.3.0/sentry_sdk/integrations/redis/modules/caches.py` & `sentry_sdk-2.3.1/sentry_sdk/integrations/redis/modules/caches.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.3.0/sentry_sdk/integrations/redis/modules/queries.py` & `sentry_sdk-2.3.1/sentry_sdk/integrations/redis/modules/queries.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.3.0/sentry_sdk/integrations/redis/rb.py` & `sentry_sdk-2.3.1/sentry_sdk/integrations/redis/rb.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.3.0/sentry_sdk/integrations/redis/redis.py` & `sentry_sdk-2.3.1/sentry_sdk/integrations/redis/redis.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.3.0/sentry_sdk/integrations/redis/redis_cluster.py` & `sentry_sdk-2.3.1/sentry_sdk/integrations/redis/redis_cluster.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.3.0/sentry_sdk/integrations/redis/redis_py_cluster_legacy.py` & `sentry_sdk-2.3.1/sentry_sdk/integrations/redis/redis_py_cluster_legacy.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.3.0/sentry_sdk/integrations/redis/utils.py` & `sentry_sdk-2.3.1/sentry_sdk/integrations/redis/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -49,29 +49,35 @@
     """
     Gets the keys (or keys) from the given method_name.
     The method_name could be a redis command or a django caching command
     """
     key = ""
     if args is not None and method_name.lower() in _MULTI_KEY_COMMANDS:
         # for example redis "mget"
-        key = ", ".join(args)
+        key = ", ".join(x.decode() if isinstance(x, bytes) else x for x in args)
+
     elif args is not None and len(args) >= 1:
         # for example django "set_many/get_many" or redis "get"
-        key = args[0]
+        key = args[0].decode() if isinstance(args[0], bytes) else args[0]
+
     elif kwargs is not None and "key" in kwargs:
         # this is a legacy case for older versions of django (I guess)
-        key = kwargs["key"]
+        key = (
+            kwargs["key"].decode()
+            if isinstance(kwargs["key"], bytes)
+            else kwargs["key"]
+        )
 
     if isinstance(key, dict):
         # Django caching set_many() has a dictionary {"key": "data", "key2": "data2"}
         # as argument. In this case only return the keys of the dictionary (to not leak data)
-        key = ", ".join(key.keys())
+        key = ", ".join(x.decode() if isinstance(x, bytes) else x for x in key.keys())
 
     if isinstance(key, list):
-        key = ", ".join(key)
+        key = ", ".join(x.decode() if isinstance(x, bytes) else x for x in key)
 
     return str(key)
 
 
 def _parse_rediscluster_command(command):
     # type: (Any) -> Sequence[Any]
     return command.args
```

### Comparing `sentry_sdk-2.3.0/sentry_sdk/integrations/rq.py` & `sentry_sdk-2.3.1/sentry_sdk/integrations/rq.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.3.0/sentry_sdk/integrations/sanic.py` & `sentry_sdk-2.3.1/sentry_sdk/integrations/sanic.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.3.0/sentry_sdk/integrations/serverless.py` & `sentry_sdk-2.3.1/sentry_sdk/integrations/serverless.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.3.0/sentry_sdk/integrations/socket.py` & `sentry_sdk-2.3.1/sentry_sdk/integrations/socket.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.3.0/sentry_sdk/integrations/spark/spark_driver.py` & `sentry_sdk-2.3.1/sentry_sdk/integrations/spark/spark_driver.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.3.0/sentry_sdk/integrations/spark/spark_worker.py` & `sentry_sdk-2.3.1/sentry_sdk/integrations/spark/spark_worker.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.3.0/sentry_sdk/integrations/sqlalchemy.py` & `sentry_sdk-2.3.1/sentry_sdk/integrations/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.3.0/sentry_sdk/integrations/starlette.py` & `sentry_sdk-2.3.1/sentry_sdk/integrations/starlette.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.3.0/sentry_sdk/integrations/starlite.py` & `sentry_sdk-2.3.1/sentry_sdk/integrations/starlite.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.3.0/sentry_sdk/integrations/stdlib.py` & `sentry_sdk-2.3.1/sentry_sdk/integrations/stdlib.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.3.0/sentry_sdk/integrations/strawberry.py` & `sentry_sdk-2.3.1/sentry_sdk/integrations/strawberry.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.3.0/sentry_sdk/integrations/threading.py` & `sentry_sdk-2.3.1/sentry_sdk/integrations/threading.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.3.0/sentry_sdk/integrations/tornado.py` & `sentry_sdk-2.3.1/sentry_sdk/integrations/tornado.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.3.0/sentry_sdk/integrations/trytond.py` & `sentry_sdk-2.3.1/sentry_sdk/integrations/trytond.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.3.0/sentry_sdk/integrations/wsgi.py` & `sentry_sdk-2.3.1/sentry_sdk/integrations/wsgi.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.3.0/sentry_sdk/metrics.py` & `sentry_sdk-2.3.1/sentry_sdk/metrics.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.3.0/sentry_sdk/monitor.py` & `sentry_sdk-2.3.1/sentry_sdk/monitor.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.3.0/sentry_sdk/profiler.py` & `sentry_sdk-2.3.1/sentry_sdk/profiler.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.3.0/sentry_sdk/scope.py` & `sentry_sdk-2.3.1/sentry_sdk/scope.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.3.0/sentry_sdk/scrubber.py` & `sentry_sdk-2.3.1/sentry_sdk/scrubber.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.3.0/sentry_sdk/serializer.py` & `sentry_sdk-2.3.1/sentry_sdk/serializer.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.3.0/sentry_sdk/session.py` & `sentry_sdk-2.3.1/sentry_sdk/session.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.3.0/sentry_sdk/sessions.py` & `sentry_sdk-2.3.1/sentry_sdk/sessions.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.3.0/sentry_sdk/spotlight.py` & `sentry_sdk-2.3.1/sentry_sdk/spotlight.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.3.0/sentry_sdk/tracing.py` & `sentry_sdk-2.3.1/sentry_sdk/tracing.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.3.0/sentry_sdk/tracing_utils.py` & `sentry_sdk-2.3.1/sentry_sdk/tracing_utils.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.3.0/sentry_sdk/transport.py` & `sentry_sdk-2.3.1/sentry_sdk/transport.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.3.0/sentry_sdk/types.py` & `sentry_sdk-2.3.1/sentry_sdk/types.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.3.0/sentry_sdk/utils.py` & `sentry_sdk-2.3.1/sentry_sdk/utils.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.3.0/sentry_sdk/worker.py` & `sentry_sdk-2.3.1/sentry_sdk/worker.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.3.0/sentry_sdk.egg-info/PKG-INFO` & `sentry_sdk-2.3.1/sentry_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sentry-sdk
-Version: 2.3.0
+Version: 2.3.1
 Summary: Python client for Sentry (https://sentry.io)
 Home-page: https://github.com/getsentry/sentry-python
 Author: Sentry Team and Contributors
 Author-email: hello@sentry.io
 License: MIT
 Project-URL: Documentation, https://docs.sentry.io/platforms/python/
 Project-URL: Changelog, https://github.com/getsentry/sentry-python/blob/master/CHANGELOG.md
```

### Comparing `sentry_sdk-2.3.0/sentry_sdk.egg-info/SOURCES.txt` & `sentry_sdk-2.3.1/sentry_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.3.0/sentry_sdk.egg-info/requires.txt` & `sentry_sdk-2.3.1/sentry_sdk.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.3.0/setup.py` & `sentry_sdk-2.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 def get_file_text(file_name):
     with open(os.path.join(here, file_name)) as in_file:
         return in_file.read()
 
 
 setup(
     name="sentry-sdk",
-    version="2.3.0",
+    version="2.3.1",
     author="Sentry Team and Contributors",
     author_email="hello@sentry.io",
     url="https://github.com/getsentry/sentry-python",
     project_urls={
         "Documentation": "https://docs.sentry.io/platforms/python/",
         "Changelog": "https://github.com/getsentry/sentry-python/blob/master/CHANGELOG.md",
     },
```

### Comparing `sentry_sdk-2.3.0/tests/test_api.py` & `sentry_sdk-2.3.1/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.3.0/tests/test_basics.py` & `sentry_sdk-2.3.1/tests/test_basics.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.3.0/tests/test_client.py` & `sentry_sdk-2.3.1/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.3.0/tests/test_conftest.py` & `sentry_sdk-2.3.1/tests/test_conftest.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.3.0/tests/test_crons.py` & `sentry_sdk-2.3.1/tests/test_crons.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.3.0/tests/test_envelope.py` & `sentry_sdk-2.3.1/tests/test_envelope.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.3.0/tests/test_exceptiongroup.py` & `sentry_sdk-2.3.1/tests/test_exceptiongroup.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.3.0/tests/test_lru_cache.py` & `sentry_sdk-2.3.1/tests/test_lru_cache.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.3.0/tests/test_metrics.py` & `sentry_sdk-2.3.1/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.3.0/tests/test_monitor.py` & `sentry_sdk-2.3.1/tests/test_monitor.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.3.0/tests/test_new_scopes_compat.py` & `sentry_sdk-2.3.1/tests/test_new_scopes_compat.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.3.0/tests/test_new_scopes_compat_event.py` & `sentry_sdk-2.3.1/tests/test_new_scopes_compat_event.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.3.0/tests/test_profiler.py` & `sentry_sdk-2.3.1/tests/test_profiler.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.3.0/tests/test_propagationcontext.py` & `sentry_sdk-2.3.1/tests/test_propagationcontext.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.3.0/tests/test_scope.py` & `sentry_sdk-2.3.1/tests/test_scope.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.3.0/tests/test_scrubber.py` & `sentry_sdk-2.3.1/tests/test_scrubber.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.3.0/tests/test_serializer.py` & `sentry_sdk-2.3.1/tests/test_serializer.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.3.0/tests/test_sessions.py` & `sentry_sdk-2.3.1/tests/test_sessions.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.3.0/tests/test_spotlight.py` & `sentry_sdk-2.3.1/tests/test_spotlight.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.3.0/tests/test_transport.py` & `sentry_sdk-2.3.1/tests/test_transport.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.3.0/tests/test_types.py` & `sentry_sdk-2.3.1/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.3.0/tests/test_utils.py` & `sentry_sdk-2.3.1/tests/test_utils.py`

 * *Files identical despite different names*


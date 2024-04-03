# Comparing `tmp/sentry-sdk-2.0.0rc2.tar.gz` & `tmp/sentry-sdk-2.0.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sentry-sdk-2.0.0rc2.tar", last modified: Wed Mar 13 14:06:35 2024, max compression
+gzip compressed data, was "sentry-sdk-2.0.0rc3.tar", last modified: Wed Mar 20 14:56:01 2024, max compression
```

## Comparing `sentry-sdk-2.0.0rc2.tar` & `sentry-sdk-2.0.0rc3.tar`

### file list

```diff
@@ -1,159 +1,160 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 14:06:35.367158 sentry-sdk-2.0.0rc2/
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-03-13 14:06:19.000000 sentry-sdk-2.0.0rc2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-03-13 14:06:19.000000 sentry-sdk-2.0.0rc2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    10412 2024-03-13 14:06:35.367158 sentry-sdk-2.0.0rc2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5960 2024-03-13 14:06:19.000000 sentry-sdk-2.0.0rc2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-03-13 14:06:19.000000 sentry-sdk-2.0.0rc2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 14:06:35.347158 sentry-sdk-2.0.0rc2/sentry_sdk/
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-03-13 14:06:19.000000 sentry-sdk-2.0.0rc2/sentry_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3066 2024-03-13 14:06:19.000000 sentry-sdk-2.0.0rc2/sentry_sdk/_compat.py
--rw-r--r--   0 runner    (1001) docker     (127)     5382 2024-03-13 14:06:19.000000 sentry-sdk-2.0.0rc2/sentry_sdk/_lru_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)    11259 2024-03-13 14:06:19.000000 sentry-sdk-2.0.0rc2/sentry_sdk/_queue.py
--rw-r--r--   0 runner    (1001) docker     (127)     5604 2024-03-13 14:06:19.000000 sentry-sdk-2.0.0rc2/sentry_sdk/_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     3745 2024-03-13 14:06:19.000000 sentry-sdk-2.0.0rc2/sentry_sdk/_werkzeug.py
--rw-r--r--   0 runner    (1001) docker     (127)     8071 2024-03-13 14:06:19.000000 sentry-sdk-2.0.0rc2/sentry_sdk/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-03-13 14:06:19.000000 sentry-sdk-2.0.0rc2/sentry_sdk/attachments.py
--rw-r--r--   0 runner    (1001) docker     (127)    28898 2024-03-13 14:06:19.000000 sentry-sdk-2.0.0rc2/sentry_sdk/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    11424 2024-03-13 14:06:19.000000 sentry-sdk-2.0.0rc2/sentry_sdk/consts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 14:06:35.347158 sentry-sdk-2.0.0rc2/sentry_sdk/crons/
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-03-13 14:06:19.000000 sentry-sdk-2.0.0rc2/sentry_sdk/crons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-03-13 14:06:19.000000 sentry-sdk-2.0.0rc2/sentry_sdk/crons/api.py
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-03-13 14:06:19.000000 sentry-sdk-2.0.0rc2/sentry_sdk/crons/consts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-03-13 14:06:19.000000 sentry-sdk-2.0.0rc2/sentry_sdk/crons/decorator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 14:06:35.347158 sentry-sdk-2.0.0rc2/sentry_sdk/db/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 14:06:19.000000 sentry-sdk-2.0.0rc2/sentry_sdk/db/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 14:06:35.347158 sentry-sdk-2.0.0rc2/sentry_sdk/db/explain_plan/
--rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-03-13 14:06:19.000000 sentry-sdk-2.0.0rc2/sentry_sdk/db/explain_plan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-03-13 14:06:19.000000 sentry-sdk-2.0.0rc2/sentry_sdk/db/explain_plan/django.py
--rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-03-13 14:06:19.000000 sentry-sdk-2.0.0rc2/sentry_sdk/db/explain_plan/sqlalchemy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-03-13 14:06:19.000000 sentry-sdk-2.0.0rc2/sentry_sdk/debug.py
--rw-r--r--   0 runner    (1001) docker     (127)     9916 2024-03-13 14:06:19.000000 sentry-sdk-2.0.0rc2/sentry_sdk/envelope.py
--rw-r--r--   0 runner    (1001) docker     (127)    26839 2024-03-13 14:06:19.000000 sentry-sdk-2.0.0rc2/sentry_sdk/hub.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 14:06:35.355158 sentry-sdk-2.0.0rc2/sentry_sdk/integrations/
--rw-r--r--   0 runner    (1001) docker     (127)     7541 2024-03-13 14:06:19.000000 sentry-sdk-2.0.0rc2/sentry_sdk/integrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3197 2024-03-13 14:06:19.000000 sentry-sdk-2.0.0rc2/sentry_sdk/integrations/_asgi_common.py
--rw-r--r--   0 runner    (1001) docker     (127)     5634 2024-03-13 14:06:19.000000 sentry-sdk-2.0.0rc2/sentry_sdk/integrations/_wsgi_common.py
--rw-r--r--   0 runner    (1001) docker     (127)    11543 2024-03-13 14:06:19.000000 sentry-sdk-2.0.0rc2/sentry_sdk/integrations/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-03-13 14:06:19.000000 sentry-sdk-2.0.0rc2/sentry_sdk/integrations/argv.py
--rw-r--r--   0 runner    (1001) docker     (127)     6228 2024-03-13 14:06:19.000000 sentry-sdk-2.0.0rc2/sentry_sdk/integrations/ariadne.py
--rw-r--r--   0 runner    (1001) docker     (127)     7150 2024-03-13 14:06:19.000000 sentry-sdk-2.0.0rc2/sentry_sdk/integrations/arq.py
--rw-r--r--   0 runner    (1001) docker     (127)    11861 2024-03-13 14:06:19.000000 sentry-sdk-2.0.0rc2/sentry_sdk/integrations/asgi.py
--rw-r--r--   0 runner    (1001) docker     (127)     3132 2024-03-13 14:06:19.000000 sentry-sdk-2.0.0rc2/sentry_sdk/integrations/asyncio.py
--rw-r--r--   0 runner    (1001) docker     (127)     6300 2024-03-13 14:06:19.000000 sentry-sdk-2.0.0rc2/sentry_sdk/integrations/asyncpg.py
--rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-03-13 14:06:19.000000 sentry-sdk-2.0.0rc2/sentry_sdk/integrations/atexit.py
--rw-r--r--   0 runner    (1001) docker     (127)    15821 2024-03-13 14:06:19.000000 sentry-sdk-2.0.0rc2/sentry_sdk/integrations/aws_lambda.py
--rw-r--r--   0 runner    (1001) docker     (127)     5619 2024-03-13 14:06:19.000000 sentry-sdk-2.0.0rc2/sentry_sdk/integrations/beam.py
--rw-r--r--   0 runner    (1001) docker     (127)     4491 2024-03-13 14:06:19.000000 sentry-sdk-2.0.0rc2/sentry_sdk/integrations/boto3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6413 2024-03-13 14:06:19.000000 sentry-sdk-2.0.0rc2/sentry_sdk/integrations/bottle.py
--rw-r--r--   0 runner    (1001) docker     (127)    19799 2024-03-13 14:06:19.000000 sentry-sdk-2.0.0rc2/sentry_sdk/integrations/celery.py
--rw-r--r--   0 runner    (1001) docker     (127)     4742 2024-03-13 14:06:19.000000 sentry-sdk-2.0.0rc2/sentry_sdk/integrations/chalice.py
--rw-r--r--   0 runner    (1001) docker     (127)     5109 2024-03-13 14:06:19.000000 sentry-sdk-2.0.0rc2/sentry_sdk/integrations/clickhouse_driver.py
--rw-r--r--   0 runner    (1001) docker     (127)     6755 2024-03-13 14:06:19.000000 sentry-sdk-2.0.0rc2/sentry_sdk/integrations/cloud_resource_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-03-13 14:06:19.000000 sentry-sdk-2.0.0rc2/sentry_sdk/integrations/dedupe.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 14:06:35.359158 sentry-sdk-2.0.0rc2/sentry_sdk/integrations/django/
--rw-r--r--   0 runner    (1001) docker     (127)    23932 2024-03-13 14:06:19.000000 sentry-sdk-2.0.0rc2/sentry_sdk/integrations/django/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7060 2024-03-13 14:06:19.000000 sentry-sdk-2.0.0rc2/sentry_sdk/integrations/django/asgi.py
--rw-r--r--   0 runner    (1001) docker     (127)     3633 2024-03-13 14:06:19.000000 sentry-sdk-2.0.0rc2/sentry_sdk/integrations/django/caching.py
--rw-r--r--   0 runner    (1001) docker     (127)     5778 2024-03-13 14:06:19.000000 sentry-sdk-2.0.0rc2/sentry_sdk/integrations/django/middleware.py
--rw-r--r--   0 runner    (1001) docker     (127)     2979 2024-03-13 14:06:19.000000 sentry-sdk-2.0.0rc2/sentry_sdk/integrations/django/signals_handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5702 2024-03-13 14:06:19.000000 sentry-sdk-2.0.0rc2/sentry_sdk/integrations/django/templates.py
--rw-r--r--   0 runner    (1001) docker     (127)     4957 2024-03-13 14:06:19.000000 sentry-sdk-2.0.0rc2/sentry_sdk/integrations/django/transactions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2891 2024-03-13 14:06:19.000000 sentry-sdk-2.0.0rc2/sentry_sdk/integrations/django/views.py
--rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-03-13 14:06:19.000000 sentry-sdk-2.0.0rc2/sentry_sdk/integrations/excepthook.py
--rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-03-13 14:06:19.000000 sentry-sdk-2.0.0rc2/sentry_sdk/integrations/executing.py
--rw-r--r--   0 runner    (1001) docker     (127)     9448 2024-03-13 14:06:19.000000 sentry-sdk-2.0.0rc2/sentry_sdk/integrations/falcon.py
--rw-r--r--   0 runner    (1001) docker     (127)     4665 2024-03-13 14:06:19.000000 sentry-sdk-2.0.0rc2/sentry_sdk/integrations/fastapi.py
--rw-r--r--   0 runner    (1001) docker     (127)     7788 2024-03-13 14:06:19.000000 sentry-sdk-2.0.0rc2/sentry_sdk/integrations/flask.py
--rw-r--r--   0 runner    (1001) docker     (127)     8210 2024-03-13 14:06:19.000000 sentry-sdk-2.0.0rc2/sentry_sdk/integrations/gcp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2906 2024-03-13 14:06:19.000000 sentry-sdk-2.0.0rc2/sentry_sdk/integrations/gnu_backtrace.py
--rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-03-13 14:06:19.000000 sentry-sdk-2.0.0rc2/sentry_sdk/integrations/gql.py
--rw-r--r--   0 runner    (1001) docker     (127)     3746 2024-03-13 14:06:19.000000 sentry-sdk-2.0.0rc2/sentry_sdk/integrations/graphene.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 14:06:35.359158 sentry-sdk-2.0.0rc2/sentry_sdk/integrations/grpc/
--rw-r--r--   0 runner    (1001) docker     (127)     4979 2024-03-13 14:06:19.000000 sentry-sdk-2.0.0rc2/sentry_sdk/integrations/grpc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 14:06:35.359158 sentry-sdk-2.0.0rc2/sentry_sdk/integrations/grpc/aio/
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-03-13 14:06:19.000000 sentry-sdk-2.0.0rc2/sentry_sdk/integrations/grpc/aio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-03-13 14:06:19.000000 sentry-sdk-2.0.0rc2/sentry_sdk/integrations/grpc/aio/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3878 2024-03-13 14:06:19.000000 sentry-sdk-2.0.0rc2/sentry_sdk/integrations/grpc/aio/server.py
--rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-03-13 14:06:19.000000 sentry-sdk-2.0.0rc2/sentry_sdk/integrations/grpc/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-03-13 14:06:19.000000 sentry-sdk-2.0.0rc2/sentry_sdk/integrations/grpc/server.py
--rw-r--r--   0 runner    (1001) docker     (127)     5005 2024-03-13 14:06:19.000000 sentry-sdk-2.0.0rc2/sentry_sdk/integrations/httpx.py
--rw-r--r--   0 runner    (1001) docker     (127)     5452 2024-03-13 14:06:19.000000 sentry-sdk-2.0.0rc2/sentry_sdk/integrations/huey.py
--rw-r--r--   0 runner    (1001) docker     (127)     9526 2024-03-13 14:06:19.000000 sentry-sdk-2.0.0rc2/sentry_sdk/integrations/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     3011 2024-03-13 14:06:19.000000 sentry-sdk-2.0.0rc2/sentry_sdk/integrations/loguru.py
--rw-r--r--   0 runner    (1001) docker     (127)      832 2024-03-13 14:06:19.000000 sentry-sdk-2.0.0rc2/sentry_sdk/integrations/modules.py
--rw-r--r--   0 runner    (1001) docker     (127)    11242 2024-03-13 14:06:19.000000 sentry-sdk-2.0.0rc2/sentry_sdk/integrations/openai.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 14:06:35.359158 sentry-sdk-2.0.0rc2/sentry_sdk/integrations/opentelemetry/
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-03-13 14:06:19.000000 sentry-sdk-2.0.0rc2/sentry_sdk/integrations/opentelemetry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-03-13 14:06:19.000000 sentry-sdk-2.0.0rc2/sentry_sdk/integrations/opentelemetry/consts.py
--rw-r--r--   0 runner    (1001) docker     (127)     5830 2024-03-13 14:06:19.000000 sentry-sdk-2.0.0rc2/sentry_sdk/integrations/opentelemetry/integration.py
--rw-r--r--   0 runner    (1001) docker     (127)     3731 2024-03-13 14:06:19.000000 sentry-sdk-2.0.0rc2/sentry_sdk/integrations/opentelemetry/propagator.py
--rw-r--r--   0 runner    (1001) docker     (127)    12375 2024-03-13 14:06:19.000000 sentry-sdk-2.0.0rc2/sentry_sdk/integrations/opentelemetry/span_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4514 2024-03-13 14:06:19.000000 sentry-sdk-2.0.0rc2/sentry_sdk/integrations/pure_eval.py
--rw-r--r--   0 runner    (1001) docker     (127)     5968 2024-03-13 14:06:19.000000 sentry-sdk-2.0.0rc2/sentry_sdk/integrations/pymongo.py
--rw-r--r--   0 runner    (1001) docker     (127)     7371 2024-03-13 14:06:19.000000 sentry-sdk-2.0.0rc2/sentry_sdk/integrations/pyramid.py
--rw-r--r--   0 runner    (1001) docker     (127)     7425 2024-03-13 14:06:19.000000 sentry-sdk-2.0.0rc2/sentry_sdk/integrations/quart.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 14:06:35.359158 sentry-sdk-2.0.0rc2/sentry_sdk/integrations/redis/
--rw-r--r--   0 runner    (1001) docker     (127)    11911 2024-03-13 14:06:19.000000 sentry-sdk-2.0.0rc2/sentry_sdk/integrations/redis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2590 2024-03-13 14:06:19.000000 sentry-sdk-2.0.0rc2/sentry_sdk/integrations/redis/asyncio.py
--rw-r--r--   0 runner    (1001) docker     (127)     5634 2024-03-13 14:06:19.000000 sentry-sdk-2.0.0rc2/sentry_sdk/integrations/rq.py
--rw-r--r--   0 runner    (1001) docker     (127)    13269 2024-03-13 14:06:19.000000 sentry-sdk-2.0.0rc2/sentry_sdk/integrations/sanic.py
--rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-03-13 14:06:19.000000 sentry-sdk-2.0.0rc2/sentry_sdk/integrations/serverless.py
--rw-r--r--   0 runner    (1001) docker     (127)     2905 2024-03-13 14:06:19.000000 sentry-sdk-2.0.0rc2/sentry_sdk/integrations/socket.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 14:06:35.359158 sentry-sdk-2.0.0rc2/sentry_sdk/integrations/spark/
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-03-13 14:06:19.000000 sentry-sdk-2.0.0rc2/sentry_sdk/integrations/spark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8475 2024-03-13 14:06:19.000000 sentry-sdk-2.0.0rc2/sentry_sdk/integrations/spark/spark_driver.py
--rw-r--r--   0 runner    (1001) docker     (127)     3973 2024-03-13 14:06:19.000000 sentry-sdk-2.0.0rc2/sentry_sdk/integrations/spark/spark_worker.py
--rw-r--r--   0 runner    (1001) docker     (127)     4965 2024-03-13 14:06:19.000000 sentry-sdk-2.0.0rc2/sentry_sdk/integrations/sqlalchemy.py
--rw-r--r--   0 runner    (1001) docker     (127)    24176 2024-03-13 14:06:19.000000 sentry-sdk-2.0.0rc2/sentry_sdk/integrations/starlette.py
--rw-r--r--   0 runner    (1001) docker     (127)    10215 2024-03-13 14:06:19.000000 sentry-sdk-2.0.0rc2/sentry_sdk/integrations/starlite.py
--rw-r--r--   0 runner    (1001) docker     (127)     8331 2024-03-13 14:06:19.000000 sentry-sdk-2.0.0rc2/sentry_sdk/integrations/stdlib.py
--rw-r--r--   0 runner    (1001) docker     (127)    14881 2024-03-13 14:06:19.000000 sentry-sdk-2.0.0rc2/sentry_sdk/integrations/strawberry.py
--rw-r--r--   0 runner    (1001) docker     (127)     4048 2024-03-13 14:06:19.000000 sentry-sdk-2.0.0rc2/sentry_sdk/integrations/threading.py
--rw-r--r--   0 runner    (1001) docker     (127)     7287 2024-03-13 14:06:19.000000 sentry-sdk-2.0.0rc2/sentry_sdk/integrations/tornado.py
--rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-03-13 14:06:19.000000 sentry-sdk-2.0.0rc2/sentry_sdk/integrations/trytond.py
--rw-r--r--   0 runner    (1001) docker     (127)     9870 2024-03-13 14:06:19.000000 sentry-sdk-2.0.0rc2/sentry_sdk/integrations/wsgi.py
--rw-r--r--   0 runner    (1001) docker     (127)    29397 2024-03-13 14:06:19.000000 sentry-sdk-2.0.0rc2/sentry_sdk/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     3720 2024-03-13 14:06:19.000000 sentry-sdk-2.0.0rc2/sentry_sdk/monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)    35123 2024-03-13 14:06:19.000000 sentry-sdk-2.0.0rc2/sentry_sdk/profiler.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 14:06:19.000000 sentry-sdk-2.0.0rc2/sentry_sdk/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    56795 2024-03-13 14:06:19.000000 sentry-sdk-2.0.0rc2/sentry_sdk/scope.py
--rw-r--r--   0 runner    (1001) docker     (127)     5082 2024-03-13 14:06:19.000000 sentry-sdk-2.0.0rc2/sentry_sdk/scrubber.py
--rw-r--r--   0 runner    (1001) docker     (127)    12729 2024-03-13 14:06:19.000000 sentry-sdk-2.0.0rc2/sentry_sdk/serializer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5581 2024-03-13 14:06:19.000000 sentry-sdk-2.0.0rc2/sentry_sdk/session.py
--rw-r--r--   0 runner    (1001) docker     (127)     7822 2024-03-13 14:06:19.000000 sentry-sdk-2.0.0rc2/sentry_sdk/sessions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-03-13 14:06:19.000000 sentry-sdk-2.0.0rc2/sentry_sdk/spotlight.py
--rw-r--r--   0 runner    (1001) docker     (127)    35876 2024-03-13 14:06:19.000000 sentry-sdk-2.0.0rc2/sentry_sdk/tracing.py
--rw-r--r--   0 runner    (1001) docker     (127)    17380 2024-03-13 14:06:19.000000 sentry-sdk-2.0.0rc2/sentry_sdk/tracing_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    19162 2024-03-13 14:06:19.000000 sentry-sdk-2.0.0rc2/sentry_sdk/transport.py
--rw-r--r--   0 runner    (1001) docker     (127)    49432 2024-03-13 14:06:19.000000 sentry-sdk-2.0.0rc2/sentry_sdk/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4475 2024-03-13 14:06:19.000000 sentry-sdk-2.0.0rc2/sentry_sdk/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 14:06:35.363158 sentry-sdk-2.0.0rc2/sentry_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10412 2024-03-13 14:06:35.000000 sentry-sdk-2.0.0rc2/sentry_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4518 2024-03-13 14:06:35.000000 sentry-sdk-2.0.0rc2/sentry_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-13 14:06:35.000000 sentry-sdk-2.0.0rc2/sentry_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-13 14:06:35.000000 sentry-sdk-2.0.0rc2/sentry_sdk.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-03-13 14:06:35.000000 sentry-sdk-2.0.0rc2/sentry_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-13 14:06:35.000000 sentry-sdk-2.0.0rc2/sentry_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-13 14:06:35.367158 sentry-sdk-2.0.0rc2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3787 2024-03-13 14:06:19.000000 sentry-sdk-2.0.0rc2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 14:06:35.363158 sentry-sdk-2.0.0rc2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4000 2024-03-13 14:06:19.000000 sentry-sdk-2.0.0rc2/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    23265 2024-03-13 14:06:19.000000 sentry-sdk-2.0.0rc2/tests/test_basics.py
--rw-r--r--   0 runner    (1001) docker     (127)    36053 2024-03-13 14:06:19.000000 sentry-sdk-2.0.0rc2/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3409 2024-03-13 14:06:19.000000 sentry-sdk-2.0.0rc2/tests/test_conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     8036 2024-03-13 14:06:19.000000 sentry-sdk-2.0.0rc2/tests/test_crons.py
--rw-r--r--   0 runner    (1001) docker     (127)     8057 2024-03-13 14:06:19.000000 sentry-sdk-2.0.0rc2/tests/test_envelope.py
--rw-r--r--   0 runner    (1001) docker     (127)     8578 2024-03-13 14:06:19.000000 sentry-sdk-2.0.0rc2/tests/test_exceptiongroup.py
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-03-13 14:06:19.000000 sentry-sdk-2.0.0rc2/tests/test_lru_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)    31256 2024-03-13 14:06:19.000000 sentry-sdk-2.0.0rc2/tests/test_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     2563 2024-03-13 14:06:19.000000 sentry-sdk-2.0.0rc2/tests/test_monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     8686 2024-03-13 14:06:19.000000 sentry-sdk-2.0.0rc2/tests/test_new_scopes_compat.py
--rw-r--r--   0 runner    (1001) docker     (127)    17155 2024-03-13 14:06:19.000000 sentry-sdk-2.0.0rc2/tests/test_new_scopes_compat_event.py
--rw-r--r--   0 runner    (1001) docker     (127)    25221 2024-03-13 14:06:19.000000 sentry-sdk-2.0.0rc2/tests/test_profiler.py
--rw-r--r--   0 runner    (1001) docker     (127)    25413 2024-03-13 14:06:19.000000 sentry-sdk-2.0.0rc2/tests/test_scope.py
--rw-r--r--   0 runner    (1001) docker     (127)     5293 2024-03-13 14:06:19.000000 sentry-sdk-2.0.0rc2/tests/test_scrubber.py
--rw-r--r--   0 runner    (1001) docker     (127)     4578 2024-03-13 14:06:19.000000 sentry-sdk-2.0.0rc2/tests/test_serializer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4098 2024-03-13 14:06:19.000000 sentry-sdk-2.0.0rc2/tests/test_sessions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-03-13 14:06:19.000000 sentry-sdk-2.0.0rc2/tests/test_spotlight.py
--rw-r--r--   0 runner    (1001) docker     (127)    12900 2024-03-13 14:06:19.000000 sentry-sdk-2.0.0rc2/tests/test_transport.py
--rw-r--r--   0 runner    (1001) docker     (127)    17396 2024-03-13 14:06:19.000000 sentry-sdk-2.0.0rc2/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 14:56:01.517714 sentry-sdk-2.0.0rc3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    10503 2024-03-20 14:56:01.517714 sentry-sdk-2.0.0rc3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5960 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 14:56:01.493714 sentry-sdk-2.0.0rc3/sentry_sdk/
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3066 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5382 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/_lru_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11259 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/_queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5604 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3745 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/_werkzeug.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8071 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/attachments.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29194 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11464 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/consts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 14:56:01.497714 sentry-sdk-2.0.0rc3/sentry_sdk/crons/
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/crons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/crons/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/crons/consts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/crons/decorator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 14:56:01.497714 sentry-sdk-2.0.0rc3/sentry_sdk/db/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/db/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 14:56:01.497714 sentry-sdk-2.0.0rc3/sentry_sdk/db/explain_plan/
+-rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/db/explain_plan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/db/explain_plan/django.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/db/explain_plan/sqlalchemy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/debug.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9916 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/envelope.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26979 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/hub.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 14:56:01.505714 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     7541 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3197 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/_asgi_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5634 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/_wsgi_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11502 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/argv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5939 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/ariadne.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7150 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/arq.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11861 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/asgi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3132 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6072 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/asyncpg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/atexit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15845 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/aws_lambda.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5619 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/beam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4491 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/boto3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6413 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/bottle.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21673 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/celery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4742 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/chalice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5109 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/clickhouse_driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6755 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/cloud_resource_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/dedupe.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 14:56:01.505714 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/django/
+-rw-r--r--   0 runner    (1001) docker     (127)    23338 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/django/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6820 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/django/asgi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3622 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/django/caching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5770 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/django/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2970 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/django/signals_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5736 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/django/templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4957 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/django/transactions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2836 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/django/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2151 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/excepthook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/executing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9448 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/falcon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4543 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/fastapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7788 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/flask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8210 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/gcp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2906 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/gnu_backtrace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4386 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/gql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3746 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/graphene.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 14:56:01.505714 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/grpc/
+-rw-r--r--   0 runner    (1001) docker     (127)     4979 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/grpc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 14:56:01.509714 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/grpc/aio/
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/grpc/aio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/grpc/aio/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3878 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/grpc/aio/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/grpc/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/grpc/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5165 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/httpx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5452 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/huey.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9592 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3011 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/loguru.py
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/modules.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11005 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/openai.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 14:56:01.509714 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/opentelemetry/
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/opentelemetry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/opentelemetry/consts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5830 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/opentelemetry/integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3731 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/opentelemetry/propagator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12375 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/opentelemetry/span_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4514 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/pure_eval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5968 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/pymongo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7371 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/pyramid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7425 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/quart.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 14:56:01.509714 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/redis/
+-rw-r--r--   0 runner    (1001) docker     (127)    11834 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/redis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/redis/asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5634 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/rq.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13269 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/sanic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/serverless.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2905 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/socket.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 14:56:01.509714 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/spark/
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/spark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8475 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/spark/spark_driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3973 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/spark/spark_worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4908 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/sqlalchemy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24176 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/starlette.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10215 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/starlite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8346 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/stdlib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14881 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/strawberry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4048 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/threading.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7287 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/tornado.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/trytond.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9870 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/wsgi.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29397 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3720 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35123 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    57353 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5082 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/scrubber.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12729 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5581 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7822 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/sessions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/spotlight.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35876 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/tracing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17304 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/tracing_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20392 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/transport.py
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52142 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4475 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 14:56:01.513714 sentry-sdk-2.0.0rc3/sentry_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10503 2024-03-20 14:56:01.000000 sentry-sdk-2.0.0rc3/sentry_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4538 2024-03-20 14:56:01.000000 sentry-sdk-2.0.0rc3/sentry_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-20 14:56:01.000000 sentry-sdk-2.0.0rc3/sentry_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-20 14:56:01.000000 sentry-sdk-2.0.0rc3/sentry_sdk.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-03-20 14:56:01.000000 sentry-sdk-2.0.0rc3/sentry_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-20 14:56:01.000000 sentry-sdk-2.0.0rc3/sentry_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-20 14:56:01.517714 sentry-sdk-2.0.0rc3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3836 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 14:56:01.513714 sentry-sdk-2.0.0rc3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4000 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23265 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/tests/test_basics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36053 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3409 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/tests/test_conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8036 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/tests/test_crons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8057 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/tests/test_envelope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8578 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/tests/test_exceptiongroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/tests/test_lru_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31256 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/tests/test_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2563 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/tests/test_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8686 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/tests/test_new_scopes_compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17155 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/tests/test_new_scopes_compat_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25221 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/tests/test_profiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25744 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/tests/test_scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5293 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/tests/test_scrubber.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4578 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/tests/test_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4098 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/tests/test_sessions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/tests/test_spotlight.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15025 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/tests/test_transport.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19715 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/tests/test_utils.py
```

### Comparing `sentry-sdk-2.0.0rc2/LICENSE` & `sentry-sdk-2.0.0rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc2/PKG-INFO` & `sentry-sdk-2.0.0rc3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sentry-sdk
-Version: 2.0.0rc2
+Version: 2.0.0rc3
 Summary: Python client for Sentry (https://sentry.io)
 Home-page: https://github.com/getsentry/sentry-python
 Author: Sentry Team and Contributors
 Author-email: hello@sentry.io
 License: MIT
 Project-URL: Documentation, https://docs.sentry.io/platforms/python/
 Project-URL: Changelog, https://github.com/getsentry/sentry-python/blob/master/CHANGELOG.md
@@ -36,14 +36,16 @@
 Requires-Dist: asyncpg>=0.23; extra == "asyncpg"
 Provides-Extra: beam
 Requires-Dist: apache-beam>=2.12; extra == "beam"
 Provides-Extra: bottle
 Requires-Dist: bottle>=0.12.13; extra == "bottle"
 Provides-Extra: celery
 Requires-Dist: celery>=3; extra == "celery"
+Provides-Extra: celery-redbeat
+Requires-Dist: celery-redbeat>=2; extra == "celery-redbeat"
 Provides-Extra: chalice
 Requires-Dist: chalice>=1.16.0; extra == "chalice"
 Provides-Extra: clickhouse-driver
 Requires-Dist: clickhouse-driver>=0.2.0; extra == "clickhouse-driver"
 Provides-Extra: django
 Requires-Dist: django>=1.8; extra == "django"
 Provides-Extra: falcon
```

### Comparing `sentry-sdk-2.0.0rc2/README.md` & `sentry-sdk-2.0.0rc3/README.md`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc2/sentry_sdk/__init__.py` & `sentry-sdk-2.0.0rc3/sentry_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc2/sentry_sdk/_compat.py` & `sentry-sdk-2.0.0rc3/sentry_sdk/_compat.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc2/sentry_sdk/_lru_cache.py` & `sentry-sdk-2.0.0rc3/sentry_sdk/_lru_cache.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc2/sentry_sdk/_queue.py` & `sentry-sdk-2.0.0rc3/sentry_sdk/_queue.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc2/sentry_sdk/_types.py` & `sentry-sdk-2.0.0rc3/sentry_sdk/_types.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc2/sentry_sdk/_werkzeug.py` & `sentry-sdk-2.0.0rc3/sentry_sdk/_werkzeug.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc2/sentry_sdk/api.py` & `sentry-sdk-2.0.0rc3/sentry_sdk/api.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc2/sentry_sdk/attachments.py` & `sentry-sdk-2.0.0rc3/sentry_sdk/attachments.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc2/sentry_sdk/client.py` & `sentry-sdk-2.0.0rc3/sentry_sdk/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -399,14 +399,23 @@
         """
         .. versionadded:: 2.0.0
 
         Returns whether the client is active (able to send data to Sentry)
         """
         return True
 
+    def should_send_default_pii(self):
+        # type: () -> bool
+        """
+        .. versionadded:: 2.0.0
+
+        Returns whether the client should send default PII (Personally Identifiable Information) data to Sentry.
+        """
+        return self.options.get("send_default_pii", False)
+
     @property
     def dsn(self):
         # type: () -> Optional[str]
         """Returns the configured DSN as string."""
         return self.options["dsn"]
 
     def _prepare_event(
```

### Comparing `sentry-sdk-2.0.0rc2/sentry_sdk/consts.py` & `sentry-sdk-2.0.0rc3/sentry_sdk/consts.py`

 * *Files 1% similar despite different names*

```diff
@@ -270,14 +270,15 @@
         sample_rate=1.0,  # type: float
         send_default_pii=False,  # type: bool
         http_proxy=None,  # type: Optional[str]
         https_proxy=None,  # type: Optional[str]
         ignore_errors=[],  # type: Sequence[Union[type, str]]  # noqa: B006
         max_request_body_size="medium",  # type: str
         socket_options=None,  # type: Optional[List[Tuple[int, int, int | bytes]]]
+        keep_alive=False,  # type: bool
         before_send=None,  # type: Optional[EventProcessor]
         before_breadcrumb=None,  # type: Optional[BreadcrumbProcessor]
         debug=None,  # type: Optional[bool]
         attach_stacktrace=False,  # type: bool
         ca_certs=None,  # type: Optional[str]
         propagate_traces=True,  # type: bool
         traces_sample_rate=None,  # type: Optional[float]
@@ -326,8 +327,8 @@
     return dict(zip(a.args[-len(defaults) :], defaults))
 
 
 DEFAULT_OPTIONS = _get_default_options()
 del _get_default_options
 
 
-VERSION = "2.0.0rc2"
+VERSION = "2.0.0rc3"
```

### Comparing `sentry-sdk-2.0.0rc2/sentry_sdk/crons/api.py` & `sentry-sdk-2.0.0rc3/sentry_sdk/crons/api.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc2/sentry_sdk/crons/decorator.py` & `sentry-sdk-2.0.0rc3/sentry_sdk/crons/decorator.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc2/sentry_sdk/db/explain_plan/__init__.py` & `sentry-sdk-2.0.0rc3/sentry_sdk/db/explain_plan/__init__.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc2/sentry_sdk/db/explain_plan/django.py` & `sentry-sdk-2.0.0rc3/sentry_sdk/db/explain_plan/django.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc2/sentry_sdk/db/explain_plan/sqlalchemy.py` & `sentry-sdk-2.0.0rc3/sentry_sdk/db/explain_plan/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc2/sentry_sdk/debug.py` & `sentry-sdk-2.0.0rc3/sentry_sdk/debug.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc2/sentry_sdk/envelope.py` & `sentry-sdk-2.0.0rc3/sentry_sdk/envelope.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc2/sentry_sdk/hub.py` & `sentry-sdk-2.0.0rc3/sentry_sdk/hub.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,18 +56,20 @@
 
 
 _local = ContextVar("sentry_current_hub")
 
 
 def _should_send_default_pii():
     # type: () -> bool
+    # TODO: Migrate existing code to `scope.should_send_default_pii()` and remove this function.
+    # New code should not use this function!
     client = Hub.current.client
     if not client:
         return False
-    return client.options["send_default_pii"]
+    return client.should_send_default_pii()
 
 
 class _InitGuard:
     def __init__(self, client):
         # type: (Client) -> None
         self._client = client
```

### Comparing `sentry-sdk-2.0.0rc2/sentry_sdk/integrations/__init__.py` & `sentry-sdk-2.0.0rc3/sentry_sdk/integrations/__init__.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc2/sentry_sdk/integrations/_asgi_common.py` & `sentry-sdk-2.0.0rc3/sentry_sdk/integrations/_asgi_common.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc2/sentry_sdk/integrations/_wsgi_common.py` & `sentry-sdk-2.0.0rc3/sentry_sdk/integrations/_wsgi_common.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc2/sentry_sdk/integrations/aiohttp.py` & `sentry-sdk-2.0.0rc3/sentry_sdk/integrations/aiohttp.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 import sys
 import weakref
 
+import sentry_sdk
 from sentry_sdk.api import continue_trace
 from sentry_sdk.consts import OP, SPANDATA
-from sentry_sdk.hub import Hub
 from sentry_sdk.integrations import Integration, DidNotEnable
 from sentry_sdk.integrations.logging import ignore_logger
 from sentry_sdk.scope import Scope
-from sentry_sdk.sessions import auto_session_tracking
+from sentry_sdk.sessions import auto_session_tracking_scope
 from sentry_sdk.integrations._wsgi_common import (
     _filter_headers,
     request_body_within_bounds,
 )
 from sentry_sdk.tracing import (
     BAGGAGE_HEADER_NAME,
     SOURCE_FOR_STYLE,
     TRANSACTION_SOURCE_ROUTE,
 )
 from sentry_sdk.tracing_utils import should_propagate_trace
 from sentry_sdk.utils import (
     capture_internal_exceptions,
+    ensure_integration_enabled,
+    ensure_integration_enabled_async,
     event_from_exception,
     logger,
     parse_url,
     parse_version,
     reraise,
     transaction_from_function,
     HAS_REAL_CONTEXTVARS,
@@ -92,69 +94,65 @@
                 " or aiocontextvars package." + CONTEXTVARS_ERROR_MESSAGE
             )
 
         ignore_logger("aiohttp.server")
 
         old_handle = Application._handle
 
+        @ensure_integration_enabled_async(AioHttpIntegration, old_handle)
         async def sentry_app_handle(self, request, *args, **kwargs):
             # type: (Any, Request, *Any, **Any) -> Any
-            hub = Hub.current
-            if hub.get_integration(AioHttpIntegration) is None:
-                return await old_handle(self, request, *args, **kwargs)
-
             weak_request = weakref.ref(request)
 
-            with Hub(hub) as hub:
-                with auto_session_tracking(hub, session_mode="request"):
+            with sentry_sdk.isolation_scope() as scope:
+                with auto_session_tracking_scope(scope, session_mode="request"):
                     # Scope data will not leak between requests because aiohttp
                     # create a task to wrap each request.
-                    with hub.configure_scope() as scope:
-                        scope.clear_breadcrumbs()
-                        scope.add_event_processor(_make_request_processor(weak_request))
+                    scope.generate_propagation_context()
+                    scope.clear_breadcrumbs()
+                    scope.add_event_processor(_make_request_processor(weak_request))
 
                     headers = dict(request.headers)
                     transaction = continue_trace(
                         headers,
                         op=OP.HTTP_SERVER,
                         # If this transaction name makes it to the UI, AIOHTTP's
                         # URL resolver did not find a route or died trying.
                         name="generic AIOHTTP request",
                         source=TRANSACTION_SOURCE_ROUTE,
                     )
-                    with hub.start_transaction(
+                    with sentry_sdk.start_transaction(
                         transaction,
                         custom_sampling_context={"aiohttp_request": request},
                     ):
                         try:
                             response = await old_handle(self, request)
                         except HTTPException as e:
                             transaction.set_http_status(e.status_code)
                             raise
                         except (asyncio.CancelledError, ConnectionResetError):
                             transaction.set_status("cancelled")
                             raise
                         except Exception:
                             # This will probably map to a 500 but seems like we
                             # have no way to tell. Do not set span status.
-                            reraise(*_capture_exception(hub))
+                            reraise(*_capture_exception())
 
                         transaction.set_http_status(response.status)
                         return response
 
         Application._handle = sentry_app_handle
 
         old_urldispatcher_resolve = UrlDispatcher.resolve
 
         async def sentry_urldispatcher_resolve(self, request):
             # type: (UrlDispatcher, Request) -> UrlMappingMatchInfo
             rv = await old_urldispatcher_resolve(self, request)
 
-            hub = Hub.current
-            integration = hub.get_integration(AioHttpIntegration)
+            integration = sentry_sdk.get_client().get_integration(AioHttpIntegration)
 
             name = None
 
             try:
                 if integration.transaction_style == "handler_name":
                     name = transaction_from_function(rv.handler)
                 elif integration.transaction_style == "method_and_path_pattern":
@@ -172,57 +170,57 @@
 
             return rv
 
         UrlDispatcher.resolve = sentry_urldispatcher_resolve
 
         old_client_session_init = ClientSession.__init__
 
+        @ensure_integration_enabled(AioHttpIntegration, old_client_session_init)
         def init(*args, **kwargs):
             # type: (Any, Any) -> None
-            hub = Hub.current
-            if hub.get_integration(AioHttpIntegration) is None:
-                return old_client_session_init(*args, **kwargs)
-
             client_trace_configs = list(kwargs.get("trace_configs") or ())
             trace_config = create_trace_config()
             client_trace_configs.append(trace_config)
 
             kwargs["trace_configs"] = client_trace_configs
             return old_client_session_init(*args, **kwargs)
 
         ClientSession.__init__ = init
 
 
 def create_trace_config():
     # type: () -> TraceConfig
+
     async def on_request_start(session, trace_config_ctx, params):
         # type: (ClientSession, SimpleNamespace, TraceRequestStartParams) -> None
-        hub = Hub.current
-        if hub.get_integration(AioHttpIntegration) is None:
+        client = sentry_sdk.get_client()
+        if client.get_integration(AioHttpIntegration) is None:
             return
 
         method = params.method.upper()
 
         parsed_url = None
         with capture_internal_exceptions():
             parsed_url = parse_url(str(params.url), sanitize=False)
 
-        span = hub.start_span(
+        span = sentry_sdk.start_span(
             op=OP.HTTP_CLIENT,
             description="%s %s"
             % (method, parsed_url.url if parsed_url else SENSITIVE_DATA_SUBSTITUTE),
         )
         span.set_data(SPANDATA.HTTP_METHOD, method)
         if parsed_url is not None:
             span.set_data("url", parsed_url.url)
             span.set_data(SPANDATA.HTTP_QUERY, parsed_url.query)
             span.set_data(SPANDATA.HTTP_FRAGMENT, parsed_url.fragment)
 
-        if should_propagate_trace(hub, str(params.url)):
-            for key, value in hub.iter_trace_propagation_headers(span):
+        if should_propagate_trace(client, str(params.url)):
+            for key, value in Scope.get_current_scope().iter_trace_propagation_headers(
+                span=span
+            ):
                 logger.debug(
                     "[Tracing] Adding `{key}` header {value} to outgoing request to {url}.".format(
                         key=key, value=value, url=params.url
                     )
                 )
                 if key == BAGGAGE_HEADER_NAME and params.headers.get(
                     BAGGAGE_HEADER_NAME
@@ -271,50 +269,48 @@
                 request.host,
                 request.path,
             )
 
             request_info["query_string"] = request.query_string
             request_info["method"] = request.method
             request_info["env"] = {"REMOTE_ADDR": request.remote}
-
-            hub = Hub.current
             request_info["headers"] = _filter_headers(dict(request.headers))
 
             # Just attach raw data here if it is within bounds, if available.
             # Unfortunately there's no way to get structured data from aiohttp
             # without awaiting on some coroutine.
-            request_info["data"] = get_aiohttp_request_data(hub, request)
+            request_info["data"] = get_aiohttp_request_data(request)
 
         return event
 
     return aiohttp_processor
 
 
-def _capture_exception(hub):
-    # type: (Hub) -> ExcInfo
+def _capture_exception():
+    # type: () -> ExcInfo
     exc_info = sys.exc_info()
     event, hint = event_from_exception(
         exc_info,
-        client_options=hub.client.options,  # type: ignore
+        client_options=sentry_sdk.get_client().options,
         mechanism={"type": "aiohttp", "handled": False},
     )
-    hub.capture_event(event, hint=hint)
+    sentry_sdk.capture_event(event, hint=hint)
     return exc_info
 
 
 BODY_NOT_READ_MESSAGE = "[Can't show request body due to implementation details.]"
 
 
-def get_aiohttp_request_data(hub, request):
-    # type: (Hub, Request) -> Union[Optional[str], AnnotatedValue]
+def get_aiohttp_request_data(request):
+    # type: (Request) -> Union[Optional[str], AnnotatedValue]
     bytes_body = request._read_bytes
 
     if bytes_body is not None:
         # we have body to show
-        if not request_body_within_bounds(hub.client, len(bytes_body)):
+        if not request_body_within_bounds(sentry_sdk.get_client(), len(bytes_body)):
             return AnnotatedValue.removed_because_over_size_limit()
 
         encoding = request.charset or "utf-8"
         return bytes_body.decode(encoding, "replace")
 
     if request.can_read_body:
         # body exists but we can't show it
```

### Comparing `sentry-sdk-2.0.0rc2/sentry_sdk/integrations/argv.py` & `sentry-sdk-2.0.0rc3/sentry_sdk/integrations/argv.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import sys
 
-from sentry_sdk.hub import Hub
+import sentry_sdk
 from sentry_sdk.integrations import Integration
 from sentry_sdk.scope import add_global_event_processor
 
 from sentry_sdk._types import TYPE_CHECKING
 
 if TYPE_CHECKING:
     from typing import Optional
@@ -17,15 +17,15 @@
 
     @staticmethod
     def setup_once():
         # type: () -> None
         @add_global_event_processor
         def processor(event, hint):
             # type: (Event, Optional[Hint]) -> Optional[Event]
-            if Hub.current.get_integration(ArgvIntegration) is not None:
+            if sentry_sdk.get_client().get_integration(ArgvIntegration) is not None:
                 extra = event.setdefault("extra", {})
                 # If some event processor decided to set extra to e.g. an
                 # `int`, don't crash. Not here.
                 if isinstance(extra, dict):
                     extra["sys.argv"] = sys.argv
 
             return event
```

### Comparing `sentry-sdk-2.0.0rc2/sentry_sdk/integrations/ariadne.py` & `sentry-sdk-2.0.0rc3/sentry_sdk/integrations/ariadne.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 from importlib import import_module
 
-from sentry_sdk.hub import Hub, _should_send_default_pii
+from sentry_sdk import get_client, capture_event
 from sentry_sdk.integrations import DidNotEnable, Integration
 from sentry_sdk.integrations.logging import ignore_logger
 from sentry_sdk.integrations._wsgi_common import request_body_within_bounds
+from sentry_sdk.scope import Scope, should_send_default_pii
 from sentry_sdk.utils import (
     capture_internal_exceptions,
+    ensure_integration_enabled,
     event_from_exception,
     package_version,
 )
 from sentry_sdk._types import TYPE_CHECKING
 
 try:
     # importing like this is necessary due to name shadowing in ariadne
@@ -47,81 +49,68 @@
 
 def _patch_graphql():
     # type: () -> None
     old_parse_query = ariadne_graphql.parse_query
     old_handle_errors = ariadne_graphql.handle_graphql_errors
     old_handle_query_result = ariadne_graphql.handle_query_result
 
+    @ensure_integration_enabled(AriadneIntegration, old_parse_query)
     def _sentry_patched_parse_query(context_value, query_parser, data):
         # type: (Optional[Any], Optional[QueryParser], Any) -> DocumentNode
-        hub = Hub.current
-        integration = hub.get_integration(AriadneIntegration)
-        if integration is None:
-            return old_parse_query(context_value, query_parser, data)
-
-        with hub.configure_scope() as scope:
-            event_processor = _make_request_event_processor(data)
-            scope.add_event_processor(event_processor)
+        event_processor = _make_request_event_processor(data)
+        Scope.get_isolation_scope().add_event_processor(event_processor)
 
         result = old_parse_query(context_value, query_parser, data)
         return result
 
+    @ensure_integration_enabled(AriadneIntegration, old_handle_errors)
     def _sentry_patched_handle_graphql_errors(errors, *args, **kwargs):
         # type: (List[GraphQLError], Any, Any) -> GraphQLResult
-        hub = Hub.current
-        integration = hub.get_integration(AriadneIntegration)
-        if integration is None:
-            return old_handle_errors(errors, *args, **kwargs)
-
         result = old_handle_errors(errors, *args, **kwargs)
 
-        with hub.configure_scope() as scope:
-            event_processor = _make_response_event_processor(result[1])
-            scope.add_event_processor(event_processor)
+        event_processor = _make_response_event_processor(result[1])
+        Scope.get_isolation_scope().add_event_processor(event_processor)
 
-        if hub.client:
+        client = get_client()
+        if client.is_active():
             with capture_internal_exceptions():
                 for error in errors:
                     event, hint = event_from_exception(
                         error,
-                        client_options=hub.client.options,
+                        client_options=client.options,
                         mechanism={
-                            "type": integration.identifier,
+                            "type": AriadneIntegration.identifier,
                             "handled": False,
                         },
                     )
-                    hub.capture_event(event, hint=hint)
+                    capture_event(event, hint=hint)
 
         return result
 
+    @ensure_integration_enabled(AriadneIntegration, old_handle_query_result)
     def _sentry_patched_handle_query_result(result, *args, **kwargs):
         # type: (Any, Any, Any) -> GraphQLResult
-        hub = Hub.current
-        integration = hub.get_integration(AriadneIntegration)
-        if integration is None:
-            return old_handle_query_result(result, *args, **kwargs)
-
         query_result = old_handle_query_result(result, *args, **kwargs)
 
-        with hub.configure_scope() as scope:
-            event_processor = _make_response_event_processor(query_result[1])
-            scope.add_event_processor(event_processor)
+        event_processor = _make_response_event_processor(query_result[1])
+        Scope.get_isolation_scope().add_event_processor(event_processor)
 
-        if hub.client:
+        client = get_client()
+        if client.is_active():
             with capture_internal_exceptions():
                 for error in result.errors or []:
                     event, hint = event_from_exception(
                         error,
-                        client_options=hub.client.options,
+                        client_options=client.options,
                         mechanism={
-                            "type": integration.identifier,
+                            "type": AriadneIntegration.identifier,
                             "handled": False,
                         },
                     )
-                    hub.capture_event(event, hint=hint)
+                    capture_event(event, hint=hint)
 
         return query_result
 
     ariadne_graphql.parse_query = _sentry_patched_parse_query  # type: ignore
     ariadne_graphql.handle_graphql_errors = _sentry_patched_handle_graphql_errors  # type: ignore
     ariadne_graphql.handle_query_result = _sentry_patched_handle_query_result  # type: ignore
 
@@ -139,16 +128,16 @@
             try:
                 content_length = int(
                     (data.get("headers") or {}).get("Content-Length", 0)
                 )
             except (TypeError, ValueError):
                 return event
 
-            if _should_send_default_pii() and request_body_within_bounds(
-                Hub.current.client, content_length
+            if should_send_default_pii() and request_body_within_bounds(
+                get_client(), content_length
             ):
                 request_info = event.setdefault("request", {})
                 request_info["api_target"] = "graphql"
                 request_info["data"] = data
 
             elif event.get("request", {}).get("data"):
                 del event["request"]["data"]
@@ -161,15 +150,15 @@
 def _make_response_event_processor(response):
     # type: (Dict[str, Any]) -> EventProcessor
     """Add response data to the event's response context."""
 
     def inner(event, hint):
         # type: (Event, dict[str, Any]) -> Event
         with capture_internal_exceptions():
-            if _should_send_default_pii() and response.get("errors"):
+            if should_send_default_pii() and response.get("errors"):
                 contexts = event.setdefault("contexts", {})
                 contexts["response"] = {
                     "data": response,
                 }
 
         return event
```

### Comparing `sentry-sdk-2.0.0rc2/sentry_sdk/integrations/arq.py` & `sentry-sdk-2.0.0rc3/sentry_sdk/integrations/arq.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc2/sentry_sdk/integrations/asgi.py` & `sentry-sdk-2.0.0rc3/sentry_sdk/integrations/asgi.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc2/sentry_sdk/integrations/asyncio.py` & `sentry-sdk-2.0.0rc3/sentry_sdk/integrations/asyncio.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc2/sentry_sdk/integrations/asyncpg.py` & `sentry-sdk-2.0.0rc3/sentry_sdk/integrations/asyncpg.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,22 @@
 from __future__ import annotations
 import contextlib
 from typing import Any, TypeVar, Callable, Awaitable, Iterator
 
-from sentry_sdk import Hub
+import sentry_sdk
 from sentry_sdk.consts import OP, SPANDATA
 from sentry_sdk.integrations import Integration, DidNotEnable
 from sentry_sdk.tracing import Span
 from sentry_sdk.tracing_utils import add_query_source, record_sql_queries
-from sentry_sdk.utils import parse_version, capture_internal_exceptions
+from sentry_sdk.utils import (
+    ensure_integration_enabled,
+    ensure_integration_enabled_async,
+    parse_version,
+    capture_internal_exceptions,
+)
 
 try:
     import asyncpg  # type: ignore[import-not-found]
     from asyncpg.cursor import BaseCursor  # type: ignore
 
 except ImportError:
     raise DidNotEnable("asyncpg not installed.")
@@ -50,102 +55,86 @@
 
 
 T = TypeVar("T")
 
 
 def _wrap_execute(f: Callable[..., Awaitable[T]]) -> Callable[..., Awaitable[T]]:
     async def _inner(*args: Any, **kwargs: Any) -> T:
-        hub = Hub.current
-        integration = hub.get_integration(AsyncPGIntegration)
+        integration = sentry_sdk.get_client().get_integration(AsyncPGIntegration)
 
         # Avoid recording calls to _execute twice.
         # Calls to Connection.execute with args also call
         # Connection._execute, which is recorded separately
         # args[0] = the connection object, args[1] is the query
         if integration is None or len(args) > 2:
             return await f(*args, **kwargs)
 
         query = args[1]
-        with record_sql_queries(
-            hub, None, query, None, None, executemany=False
-        ) as span:
+        with record_sql_queries(None, query, None, None, executemany=False) as span:
             res = await f(*args, **kwargs)
 
         with capture_internal_exceptions():
-            add_query_source(hub, span)
+            add_query_source(span)
 
         return res
 
     return _inner
 
 
 SubCursor = TypeVar("SubCursor", bound=BaseCursor)
 
 
 @contextlib.contextmanager
 def _record(
-    hub: Hub,
     cursor: SubCursor | None,
     query: str,
     params_list: tuple[Any, ...] | None,
     *,
     executemany: bool = False,
 ) -> Iterator[Span]:
-    integration = hub.get_integration(AsyncPGIntegration)
-    if not integration._record_params:
+    integration = sentry_sdk.get_client().get_integration(AsyncPGIntegration)
+    if integration is not None and not integration._record_params:
         params_list = None
 
     param_style = "pyformat" if params_list else None
 
     with record_sql_queries(
-        hub,
         cursor,
         query,
         params_list,
         param_style,
         executemany=executemany,
         record_cursor_repr=cursor is not None,
     ) as span:
         yield span
 
 
 def _wrap_connection_method(
     f: Callable[..., Awaitable[T]], *, executemany: bool = False
 ) -> Callable[..., Awaitable[T]]:
+    @ensure_integration_enabled_async(AsyncPGIntegration, f)
     async def _inner(*args: Any, **kwargs: Any) -> T:
-        hub = Hub.current
-        integration = hub.get_integration(AsyncPGIntegration)
-
-        if integration is None:
-            return await f(*args, **kwargs)
-
         query = args[1]
         params_list = args[2] if len(args) > 2 else None
-        with _record(hub, None, query, params_list, executemany=executemany) as span:
+        with _record(None, query, params_list, executemany=executemany) as span:
             _set_db_data(span, args[0])
             res = await f(*args, **kwargs)
 
         return res
 
     return _inner
 
 
 def _wrap_cursor_creation(f: Callable[..., T]) -> Callable[..., T]:
+    @ensure_integration_enabled(AsyncPGIntegration, f)
     def _inner(*args: Any, **kwargs: Any) -> T:  # noqa: N807
-        hub = Hub.current
-        integration = hub.get_integration(AsyncPGIntegration)
-
-        if integration is None:
-            return f(*args, **kwargs)
-
         query = args[1]
         params_list = args[2] if len(args) > 2 else None
 
         with _record(
-            hub,
             None,
             query,
             params_list,
             executemany=False,
         ) as span:
             _set_db_data(span, args[0])
             res = f(*args, **kwargs)
@@ -153,38 +142,35 @@
 
         return res
 
     return _inner
 
 
 def _wrap_connect_addr(f: Callable[..., Awaitable[T]]) -> Callable[..., Awaitable[T]]:
+    @ensure_integration_enabled_async(AsyncPGIntegration, f)
     async def _inner(*args: Any, **kwargs: Any) -> T:
-        hub = Hub.current
-        integration = hub.get_integration(AsyncPGIntegration)
-
-        if integration is None:
-            return await f(*args, **kwargs)
-
         user = kwargs["params"].user
         database = kwargs["params"].database
 
-        with hub.start_span(op=OP.DB, description="connect") as span:
+        with sentry_sdk.start_span(op=OP.DB, description="connect") as span:
             span.set_data(SPANDATA.DB_SYSTEM, "postgresql")
             addr = kwargs.get("addr")
             if addr:
                 try:
                     span.set_data(SPANDATA.SERVER_ADDRESS, addr[0])
                     span.set_data(SPANDATA.SERVER_PORT, addr[1])
                 except IndexError:
                     pass
             span.set_data(SPANDATA.DB_NAME, database)
             span.set_data(SPANDATA.DB_USER, user)
 
             with capture_internal_exceptions():
-                hub.add_breadcrumb(message="connect", category="query", data=span._data)
+                sentry_sdk.add_breadcrumb(
+                    message="connect", category="query", data=span._data
+                )
             res = await f(*args, **kwargs)
 
         return res
 
     return _inner
```

### Comparing `sentry-sdk-2.0.0rc2/sentry_sdk/integrations/atexit.py` & `sentry-sdk-2.0.0rc3/sentry_sdk/integrations/atexit.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import os
 import sys
 import atexit
 
-from sentry_sdk.hub import Hub
+import sentry_sdk
+from sentry_sdk import Scope
 from sentry_sdk.utils import logger
 from sentry_sdk.integrations import Integration
 
 from sentry_sdk._types import TYPE_CHECKING
 
 if TYPE_CHECKING:
     from typing import Any
@@ -42,18 +43,14 @@
     @staticmethod
     def setup_once():
         # type: () -> None
         @atexit.register
         def _shutdown():
             # type: () -> None
             logger.debug("atexit: got shutdown signal")
-            hub = Hub.main
-            integration = hub.get_integration(AtexitIntegration)
+            client = sentry_sdk.get_client()
+            integration = client.get_integration(AtexitIntegration)
             if integration is not None:
                 logger.debug("atexit: shutting down client")
 
-                # If there is a session on the hub, close it now.
-                hub.end_session()
-
-                # If an integration is there, a client has to be there.
-                client = hub.client  # type: Any
+                Scope.get_isolation_scope().end_session()
                 client.close(callback=integration.callback)
```

### Comparing `sentry-sdk-2.0.0rc2/sentry_sdk/integrations/aws_lambda.py` & `sentry-sdk-2.0.0rc3/sentry_sdk/integrations/aws_lambda.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,15 +76,15 @@
         #
         # In some cases, it is a list (if the user is batch-invoking their
         # function, for example), in which case we'll use the first entry as a
         # representative from which to try pulling request data. (Presumably it
         # will be the same for all events in the list, since they're all hitting
         # the lambda in the same request.)
 
-        if isinstance(aws_event, list):
+        if isinstance(aws_event, list) and len(aws_event) >= 1:
             request_data = aws_event[0]
             batch_size = len(aws_event)
         else:
             request_data = aws_event
             batch_size = 1
 
         if not isinstance(request_data, dict):
```

### Comparing `sentry-sdk-2.0.0rc2/sentry_sdk/integrations/beam.py` & `sentry-sdk-2.0.0rc3/sentry_sdk/integrations/beam.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc2/sentry_sdk/integrations/boto3.py` & `sentry-sdk-2.0.0rc3/sentry_sdk/integrations/boto3.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc2/sentry_sdk/integrations/bottle.py` & `sentry-sdk-2.0.0rc3/sentry_sdk/integrations/bottle.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc2/sentry_sdk/integrations/celery.py` & `sentry-sdk-2.0.0rc3/sentry_sdk/integrations/celery.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 import sys
 import time
 from functools import wraps
 
+import sentry_sdk
 from sentry_sdk.api import continue_trace
 from sentry_sdk.consts import OP
 from sentry_sdk.crons import capture_checkin, MonitorStatus
-from sentry_sdk.hub import Hub
 from sentry_sdk import isolation_scope
 from sentry_sdk.integrations import Integration, DidNotEnable
 from sentry_sdk.integrations.logging import ignore_logger
 from sentry_sdk.tracing import BAGGAGE_HEADER_NAME, TRANSACTION_SOURCE_TASK
 from sentry_sdk._types import TYPE_CHECKING
 from sentry_sdk.scope import Scope
 from sentry_sdk.utils import (
     capture_internal_exceptions,
     event_from_exception,
+    ensure_integration_enabled,
     logger,
     match_regex_list,
     reraise,
 )
 
 if TYPE_CHECKING:
     from typing import Any
@@ -52,14 +53,19 @@
         task_failure,
         task_success,
         task_retry,
     )
 except ImportError:
     raise DidNotEnable("Celery not installed")
 
+try:
+    from redbeat.schedulers import RedBeatScheduler  # type: ignore
+except ImportError:
+    RedBeatScheduler = None
+
 
 CELERY_CONTROL_FLOW_EXCEPTIONS = (Retry, Ignore, Reject)
 
 
 class CeleryIntegration(Integration):
     identifier = "celery"
 
@@ -72,14 +78,15 @@
         # type: (bool, bool, Optional[List[str]]) -> None
         self.propagate_traces = propagate_traces
         self.monitor_beat_tasks = monitor_beat_tasks
         self.exclude_beat_tasks = exclude_beat_tasks
 
         if monitor_beat_tasks:
             _patch_beat_apply_entry()
+            _patch_redbeat_maybe_due()
             _setup_celery_beat_signals()
 
     @staticmethod
     def setup_once():
         # type: () -> None
         if CELERY_VERSION < (3,):
             raise DidNotEnable("Celery 3 or newer required.")
@@ -143,25 +150,21 @@
         # type: (Any, Any, Any) -> None
         return None
 
 
 def _wrap_apply_async(f):
     # type: (F) -> F
     @wraps(f)
+    @ensure_integration_enabled(CeleryIntegration, f)
     def apply_async(*args, **kwargs):
         # type: (*Any, **Any) -> Any
-        hub = Hub.current
-        integration = hub.get_integration(CeleryIntegration)
-
-        if integration is None:
-            return f(*args, **kwargs)
-
         # Note: kwargs can contain headers=None, so no setdefault!
         # Unsure which backend though.
         kwarg_headers = kwargs.get("headers") or {}
+        integration = sentry_sdk.get_client().get_integration(CeleryIntegration)
         propagate_traces = kwarg_headers.pop(
             "sentry-propagate-traces", integration.propagate_traces
         )
 
         if not propagate_traces:
             return f(*args, **kwargs)
 
@@ -169,23 +172,23 @@
             task_started_from_beat = args[1][0] == "BEAT"
         except (IndexError, TypeError):
             task_started_from_beat = False
 
         task = args[0]
 
         span_mgr = (
-            hub.start_span(op=OP.QUEUE_SUBMIT_CELERY, description=task.name)
+            sentry_sdk.start_span(op=OP.QUEUE_SUBMIT_CELERY, description=task.name)
             if not task_started_from_beat
             else NoOpMgr()
         )  # type: Union[Span, NoOpMgr]
 
         with span_mgr as span:
             with capture_internal_exceptions():
                 headers = (
-                    dict(hub.iter_trace_propagation_headers(span))
+                    dict(Scope.get_current_scope().iter_trace_propagation_headers(span))
                     if span is not None
                     else {}
                 )
                 if integration.monitor_beat_tasks:
                     headers.update(
                         {
                             "sentry-monitor-start-timestamp-s": "%.9f"
@@ -236,20 +239,17 @@
     # Need to wrap tracer for pushing the scope before prerun is sent, and
     # popping it after postrun is sent.
     #
     # This is the reason we don't use signals for hooking in the first place.
     # Also because in Celery 3, signal dispatch returns early if one handler
     # crashes.
     @wraps(f)
+    @ensure_integration_enabled(CeleryIntegration, f)
     def _inner(*args, **kwargs):
         # type: (*Any, **Any) -> Any
-        hub = Hub.current
-        if hub.get_integration(CeleryIntegration) is None:
-            return f(*args, **kwargs)
-
         with isolation_scope() as scope:
             scope._name = "celery"
             scope.clear_breadcrumbs()
             scope.add_event_processor(_make_event_processor(task, *args, **kwargs))
 
             transaction = None
 
@@ -264,15 +264,15 @@
                 )
                 transaction.name = task.name
                 transaction.set_status("ok")
 
             if transaction is None:
                 return f(*args, **kwargs)
 
-            with hub.start_transaction(
+            with sentry_sdk.start_transaction(
                 transaction,
                 custom_sampling_context={
                     "celery_job": {
                         "task": task.name,
                         # for some reason, args[1] is a list if non-empty but a
                         # tuple if empty
                         "args": list(args[1]),
@@ -335,42 +335,39 @@
         return event
 
     return event_processor
 
 
 def _capture_exception(task, exc_info):
     # type: (Any, ExcInfo) -> None
-    hub = Hub.current
-
-    if hub.get_integration(CeleryIntegration) is None:
+    client = sentry_sdk.get_client()
+    if client.get_integration(CeleryIntegration) is None:
         return
+
     if isinstance(exc_info[1], CELERY_CONTROL_FLOW_EXCEPTIONS):
         # ??? Doesn't map to anything
-        _set_status(hub, "aborted")
+        _set_status("aborted")
         return
 
-    _set_status(hub, "internal_error")
+    _set_status("internal_error")
 
     if hasattr(task, "throws") and isinstance(exc_info[1], task.throws):
         return
 
-    # If an integration is there, a client has to be there.
-    client = hub.client  # type: Any
-
     event, hint = event_from_exception(
         exc_info,
         client_options=client.options,
         mechanism={"type": "celery", "handled": False},
     )
 
-    hub.capture_event(event, hint=hint)
+    sentry_sdk.capture_event(event, hint=hint)
 
 
-def _set_status(hub, status):
-    # type: (Hub, str) -> None
+def _set_status(status):
+    # type: (str) -> None
     with capture_internal_exceptions():
         scope = Scope.get_current_scope()
         if scope.span is not None:
             scope.span.set_status(status)
 
 
 def _patch_worker_exit():
@@ -384,17 +381,19 @@
 
     def sentry_workloop(*args, **kwargs):
         # type: (*Any, **Any) -> Any
         try:
             return old_workloop(*args, **kwargs)
         finally:
             with capture_internal_exceptions():
-                hub = Hub.current
-                if hub.get_integration(CeleryIntegration) is not None:
-                    hub.flush()
+                if (
+                    sentry_sdk.get_client().get_integration(CeleryIntegration)
+                    is not None
+                ):
+                    sentry_sdk.flush()
 
     Worker.workloop = sentry_workloop
 
 
 def _get_headers(task):
     # type: (Task) -> Dict[str, Any]
     headers = task.request.get("headers") or {}
@@ -483,62 +482,114 @@
     return monitor_config
 
 
 def _patch_beat_apply_entry():
     # type: () -> None
     original_apply_entry = Scheduler.apply_entry
 
+    @ensure_integration_enabled(CeleryIntegration, original_apply_entry)
     def sentry_apply_entry(*args, **kwargs):
         # type: (*Any, **Any) -> None
         scheduler, schedule_entry = args
         app = scheduler.app
 
         celery_schedule = schedule_entry.schedule
         monitor_name = schedule_entry.name
 
-        hub = Hub.current
-        integration = hub.get_integration(CeleryIntegration)
-        if integration is None:
-            return original_apply_entry(*args, **kwargs)
-
+        integration = sentry_sdk.get_client().get_integration(CeleryIntegration)
         if match_regex_list(monitor_name, integration.exclude_beat_tasks):
             return original_apply_entry(*args, **kwargs)
 
-        with hub.configure_scope() as scope:
-            # When tasks are started from Celery Beat, make sure each task has its own trace.
-            scope.set_new_propagation_context()
-
-            monitor_config = _get_monitor_config(celery_schedule, app, monitor_name)
-
-            is_supported_schedule = bool(monitor_config)
-            if is_supported_schedule:
-                headers = schedule_entry.options.pop("headers", {})
-                headers.update(
-                    {
-                        "sentry-monitor-slug": monitor_name,
-                        "sentry-monitor-config": monitor_config,
-                    }
-                )
+        # When tasks are started from Celery Beat, make sure each task has its own trace.
+        scope = Scope.get_isolation_scope()
+        scope.set_new_propagation_context()
+
+        monitor_config = _get_monitor_config(celery_schedule, app, monitor_name)
+
+        is_supported_schedule = bool(monitor_config)
+        if is_supported_schedule:
+            headers = schedule_entry.options.pop("headers", {})
+            headers.update(
+                {
+                    "sentry-monitor-slug": monitor_name,
+                    "sentry-monitor-config": monitor_config,
+                }
+            )
 
-                check_in_id = capture_checkin(
-                    monitor_slug=monitor_name,
-                    monitor_config=monitor_config,
-                    status=MonitorStatus.IN_PROGRESS,
-                )
-                headers.update({"sentry-monitor-check-in-id": check_in_id})
+            check_in_id = capture_checkin(
+                monitor_slug=monitor_name,
+                monitor_config=monitor_config,
+                status=MonitorStatus.IN_PROGRESS,
+            )
+            headers.update({"sentry-monitor-check-in-id": check_in_id})
 
-                # Set the Sentry configuration in the options of the ScheduleEntry.
-                # Those will be picked up in `apply_async` and added to the headers.
-                schedule_entry.options["headers"] = headers
+            # Set the Sentry configuration in the options of the ScheduleEntry.
+            # Those will be picked up in `apply_async` and added to the headers.
+            schedule_entry.options["headers"] = headers
 
-            return original_apply_entry(*args, **kwargs)
+        return original_apply_entry(*args, **kwargs)
 
     Scheduler.apply_entry = sentry_apply_entry
 
 
+def _patch_redbeat_maybe_due():
+    # type: () -> None
+
+    if RedBeatScheduler is None:
+        return
+
+    original_maybe_due = RedBeatScheduler.maybe_due
+
+    def sentry_maybe_due(*args, **kwargs):
+        # type: (*Any, **Any) -> None
+        scheduler, schedule_entry = args
+        app = scheduler.app
+
+        celery_schedule = schedule_entry.schedule
+        monitor_name = schedule_entry.name
+
+        integration = sentry_sdk.get_client().get_integration(CeleryIntegration)
+        if integration is None:
+            return original_maybe_due(*args, **kwargs)
+
+        if match_regex_list(monitor_name, integration.exclude_beat_tasks):
+            return original_maybe_due(*args, **kwargs)
+
+        # When tasks are started from Celery Beat, make sure each task has its own trace.
+        scope = Scope.get_isolation_scope()
+        scope.set_new_propagation_context()
+
+        monitor_config = _get_monitor_config(celery_schedule, app, monitor_name)
+
+        is_supported_schedule = bool(monitor_config)
+        if is_supported_schedule:
+            headers = schedule_entry.options.pop("headers", {})
+            headers.update(
+                {
+                    "sentry-monitor-slug": monitor_name,
+                    "sentry-monitor-config": monitor_config,
+                }
+            )
+
+            check_in_id = capture_checkin(
+                monitor_slug=monitor_name,
+                monitor_config=monitor_config,
+                status=MonitorStatus.IN_PROGRESS,
+            )
+            headers.update({"sentry-monitor-check-in-id": check_in_id})
+
+            # Set the Sentry configuration in the options of the ScheduleEntry.
+            # Those will be picked up in `apply_async` and added to the headers.
+            schedule_entry.options["headers"] = headers
+
+        return original_maybe_due(*args, **kwargs)
+
+    RedBeatScheduler.maybe_due = sentry_maybe_due
+
+
 def _setup_celery_beat_signals():
     # type: () -> None
     task_success.connect(crons_task_success)
     task_failure.connect(crons_task_failure)
     task_retry.connect(crons_task_retry)
```

### Comparing `sentry-sdk-2.0.0rc2/sentry_sdk/integrations/chalice.py` & `sentry-sdk-2.0.0rc3/sentry_sdk/integrations/chalice.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc2/sentry_sdk/integrations/clickhouse_driver.py` & `sentry-sdk-2.0.0rc3/sentry_sdk/integrations/clickhouse_driver.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc2/sentry_sdk/integrations/cloud_resource_context.py` & `sentry-sdk-2.0.0rc3/sentry_sdk/integrations/cloud_resource_context.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc2/sentry_sdk/integrations/dedupe.py` & `sentry-sdk-2.0.0rc3/sentry_sdk/integrations/dedupe.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from sentry_sdk.hub import Hub
+import sentry_sdk
 from sentry_sdk.utils import ContextVar
 from sentry_sdk.integrations import Integration
 from sentry_sdk.scope import add_global_event_processor
 
 from sentry_sdk._types import TYPE_CHECKING
 
 if TYPE_CHECKING:
@@ -23,16 +23,15 @@
         # type: () -> None
         @add_global_event_processor
         def processor(event, hint):
             # type: (Event, Optional[Hint]) -> Optional[Event]
             if hint is None:
                 return event
 
-            integration = Hub.current.get_integration(DedupeIntegration)
-
+            integration = sentry_sdk.get_client().get_integration(DedupeIntegration)
             if integration is None:
                 return event
 
             exc_info = hint.get("exc_info", None)
             if exc_info is None:
                 return event
```

### Comparing `sentry-sdk-2.0.0rc2/sentry_sdk/integrations/django/__init__.py` & `sentry-sdk-2.0.0rc3/sentry_sdk/integrations/django/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 import inspect
 import sys
 import threading
 import weakref
 from importlib import import_module
 
+import sentry_sdk
 from sentry_sdk._types import TYPE_CHECKING
 from sentry_sdk.consts import OP, SPANDATA
 from sentry_sdk.db.explain_plan.django import attach_explain_plan_to_span
-from sentry_sdk.hub import Hub, _should_send_default_pii
-from sentry_sdk.scope import Scope, add_global_event_processor
+from sentry_sdk.scope import Scope, add_global_event_processor, should_send_default_pii
 from sentry_sdk.serializer import add_global_repr_processor
 from sentry_sdk.tracing import SOURCE_FOR_STYLE, TRANSACTION_SOURCE_URL
 from sentry_sdk.tracing_utils import add_query_source, record_sql_queries
 from sentry_sdk.utils import (
     AnnotatedValue,
     HAS_REAL_CONTEXTVARS,
     CONTEXTVARS_ERROR_MESSAGE,
     SENSITIVE_DATA_SUBSTITUTE,
     logger,
     capture_internal_exceptions,
+    ensure_integration_enabled,
     event_from_exception,
     transaction_from_function,
     walk_exception_chain,
 )
 from sentry_sdk.integrations import Integration, DidNotEnable
 from sentry_sdk.integrations.logging import ignore_logger
 from sentry_sdk.integrations.wsgi import SentryWsgiMiddleware
@@ -142,19 +143,17 @@
         ignore_logger("django.server")
         ignore_logger("django.request")
 
         from django.core.handlers.wsgi import WSGIHandler
 
         old_app = WSGIHandler.__call__
 
+        @ensure_integration_enabled(DjangoIntegration, old_app)
         def sentry_patched_wsgi_handler(self, environ, start_response):
             # type: (Any, Dict[str, str], Callable[..., Any]) -> _ScopedResponse
-            if Hub.current.get_integration(DjangoIntegration) is None:
-                return old_app(self, environ, start_response)
-
             bound_old_app = old_app.__get__(self, WSGIHandler)
 
             from django.conf import settings
 
             use_x_forwarded_for = settings.USE_X_FORWARDED_HOST
 
             return SentryWsgiMiddleware(bound_old_app, use_x_forwarded_for)(
@@ -225,19 +224,14 @@
                 from django.db.models.query import QuerySet
             except Exception:
                 return NotImplemented
 
             if not isinstance(value, QuerySet) or value._result_cache:
                 return NotImplemented
 
-            # Do not call Hub.get_integration here. It is intentional that
-            # running under a new hub does not suddenly start executing
-            # querysets. This might be surprising to the user but it's likely
-            # less annoying.
-
             return "<%s from %s at 0x%x>" % (
                 value.__class__.__name__,
                 value.__module__,
                 id(value),
             )
 
         _patch_channels()
@@ -396,16 +390,16 @@
                 )
     except Exception:
         pass
 
 
 def _before_get_response(request):
     # type: (WSGIRequest) -> None
-    hub = Hub.current
-    integration = hub.get_integration(DjangoIntegration)
+    integration = sentry_sdk.get_client().get_integration(DjangoIntegration)
+
     if integration is None:
         return
 
     _patch_drf()
 
     scope = Scope.get_current_scope()
     # Rely on WSGI middleware to start a trace
@@ -427,16 +421,15 @@
         return
 
     _set_transaction_name_and_source(scope, transaction_style, request)
 
 
 def _after_get_response(request):
     # type: (WSGIRequest) -> None
-    hub = Hub.current
-    integration = hub.get_integration(DjangoIntegration)
+    integration = sentry_sdk.get_client().get_integration(DjangoIntegration)
     if integration is None or integration.transaction_style != "url":
         return
 
     scope = Scope.get_current_scope()
     _attempt_resolve_again(request, scope, integration.transaction_style)
 
 
@@ -486,41 +479,38 @@
                 request = drf_request
         except AttributeError:
             pass
 
         with capture_internal_exceptions():
             DjangoRequestExtractor(request).extract_into_event(event)
 
-        if _should_send_default_pii():
+        if should_send_default_pii():
             with capture_internal_exceptions():
                 _set_user_info(request, event)
 
         return event
 
     return wsgi_request_event_processor
 
 
 def _got_request_exception(request=None, **kwargs):
     # type: (WSGIRequest, **Any) -> None
-    hub = Hub.current
-    integration = hub.get_integration(DjangoIntegration)
+    client = sentry_sdk.get_client()
+    integration = client.get_integration(DjangoIntegration)
     if integration is not None:
         if request is not None and integration.transaction_style == "url":
             scope = Scope.get_current_scope()
             _attempt_resolve_again(request, scope, integration.transaction_style)
 
-        # If an integration is there, a client has to be there.
-        client = hub.client  # type: Any
-
         event, hint = event_from_exception(
             sys.exc_info(),
             client_options=client.options,
             mechanism={"type": "django", "handled": False},
         )
-        hub.capture_event(event, hint=hint)
+        sentry_sdk.capture_event(event, hint=hint)
 
 
 class DjangoRequestExtractor(RequestExtractor):
     def env(self):
         # type: () -> Dict[str, str]
         return self.request.META
 
@@ -608,82 +598,75 @@
         real_execute = CursorWrapper.execute
         real_executemany = CursorWrapper.executemany
         real_connect = BaseDatabaseWrapper.connect
     except AttributeError:
         # This won't work on Django versions < 1.6
         return
 
+    @ensure_integration_enabled(DjangoIntegration, real_execute)
     def execute(self, sql, params=None):
         # type: (CursorWrapper, Any, Optional[Any]) -> Any
-        hub = Hub.current
-        if hub.get_integration(DjangoIntegration) is None:
-            return real_execute(self, sql, params)
-
         with record_sql_queries(
-            hub, self.cursor, sql, params, paramstyle="format", executemany=False
+            self.cursor, sql, params, paramstyle="format", executemany=False
         ) as span:
             _set_db_data(span, self)
-            if hub.client:
-                options = hub.client.options["_experiments"].get("attach_explain_plans")
-                if options is not None:
-                    attach_explain_plan_to_span(
-                        span,
-                        self.cursor.connection,
-                        sql,
-                        params,
-                        self.mogrify,
-                        options,
-                    )
+            options = (
+                sentry_sdk.get_client()
+                .options["_experiments"]
+                .get("attach_explain_plans")
+            )
+            if options is not None:
+                attach_explain_plan_to_span(
+                    span,
+                    self.cursor.connection,
+                    sql,
+                    params,
+                    self.mogrify,
+                    options,
+                )
             result = real_execute(self, sql, params)
 
         with capture_internal_exceptions():
-            add_query_source(hub, span)
+            add_query_source(span)
 
         return result
 
+    @ensure_integration_enabled(DjangoIntegration, real_executemany)
     def executemany(self, sql, param_list):
         # type: (CursorWrapper, Any, List[Any]) -> Any
-        hub = Hub.current
-        if hub.get_integration(DjangoIntegration) is None:
-            return real_executemany(self, sql, param_list)
-
         with record_sql_queries(
-            hub, self.cursor, sql, param_list, paramstyle="format", executemany=True
+            self.cursor, sql, param_list, paramstyle="format", executemany=True
         ) as span:
             _set_db_data(span, self)
 
             result = real_executemany(self, sql, param_list)
 
         with capture_internal_exceptions():
-            add_query_source(hub, span)
+            add_query_source(span)
 
         return result
 
+    @ensure_integration_enabled(DjangoIntegration, real_connect)
     def connect(self):
         # type: (BaseDatabaseWrapper) -> None
-        hub = Hub.current
-        if hub.get_integration(DjangoIntegration) is None:
-            return real_connect(self)
-
         with capture_internal_exceptions():
-            hub.add_breadcrumb(message="connect", category="query")
+            sentry_sdk.add_breadcrumb(message="connect", category="query")
 
-        with hub.start_span(op=OP.DB, description="connect") as span:
+        with sentry_sdk.start_span(op=OP.DB, description="connect") as span:
             _set_db_data(span, self)
             return real_connect(self)
 
     CursorWrapper.execute = execute
     CursorWrapper.executemany = executemany
     BaseDatabaseWrapper.connect = connect
     ignore_logger("django.db.backends")
 
 
 def _set_db_data(span, cursor_or_db):
     # type: (Span, Any) -> None
-
     db = cursor_or_db.db if hasattr(cursor_or_db, "db") else cursor_or_db
     vendor = db.vendor
     span.set_data(SPANDATA.DB_SYSTEM, vendor)
 
     # Some custom backends override `__getattr__`, making it look like `cursor_or_db`
     # actually has a `connection` and the `connection` has a `get_dsn_parameters`
     # attribute, only to throw an error once you actually want to call it.
```

### Comparing `sentry-sdk-2.0.0rc2/sentry_sdk/integrations/django/asgi.py` & `sentry-sdk-2.0.0rc3/sentry_sdk/integrations/django/asgi.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,21 +7,26 @@
 """
 
 import asyncio
 import functools
 
 from django.core.handlers.wsgi import WSGIRequest
 
-from sentry_sdk import Hub
+import sentry_sdk
+from sentry_sdk import Scope
 from sentry_sdk._types import TYPE_CHECKING
 from sentry_sdk.consts import OP
-from sentry_sdk.hub import _should_send_default_pii
 
 from sentry_sdk.integrations.asgi import SentryAsgiMiddleware
-from sentry_sdk.utils import capture_internal_exceptions
+from sentry_sdk.scope import should_send_default_pii
+from sentry_sdk.utils import (
+    capture_internal_exceptions,
+    ensure_integration_enabled,
+    ensure_integration_enabled_async,
+)
 
 
 if TYPE_CHECKING:
     from collections.abc import Callable
     from typing import Any, Union
 
     from django.core.handlers.asgi import ASGIRequest
@@ -47,15 +52,15 @@
 
         if type(request) == WSGIRequest:
             return event
 
         with capture_internal_exceptions():
             DjangoRequestExtractor(request).extract_into_event(event)
 
-        if _should_send_default_pii():
+        if should_send_default_pii():
             with capture_internal_exceptions():
                 _set_user_info(request, event)
 
         return event
 
     return asgi_request_event_processor
 
@@ -63,45 +68,37 @@
 def patch_django_asgi_handler_impl(cls):
     # type: (Any) -> None
 
     from sentry_sdk.integrations.django import DjangoIntegration
 
     old_app = cls.__call__
 
+    @ensure_integration_enabled_async(DjangoIntegration, old_app)
     async def sentry_patched_asgi_handler(self, scope, receive, send):
         # type: (Any, Any, Any, Any) -> Any
-        hub = Hub.current
-        integration = hub.get_integration(DjangoIntegration)
-        if integration is None:
-            return await old_app(self, scope, receive, send)
-
         middleware = SentryAsgiMiddleware(
             old_app.__get__(self, cls), unsafe_context_data=True
         )._run_asgi3
 
         return await middleware(scope, receive, send)
 
     cls.__call__ = sentry_patched_asgi_handler
 
     modern_django_asgi_support = hasattr(cls, "create_request")
     if modern_django_asgi_support:
         old_create_request = cls.create_request
 
+        @ensure_integration_enabled(DjangoIntegration, old_create_request)
         def sentry_patched_create_request(self, *args, **kwargs):
             # type: (Any, *Any, **Any) -> Any
-            hub = Hub.current
-            integration = hub.get_integration(DjangoIntegration)
-            if integration is None:
-                return old_create_request(self, *args, **kwargs)
-
-            with hub.configure_scope() as scope:
-                request, error_response = old_create_request(self, *args, **kwargs)
-                scope.add_event_processor(_make_asgi_request_event_processor(request))
+            request, error_response = old_create_request(self, *args, **kwargs)
+            scope = Scope.get_isolation_scope()
+            scope.add_event_processor(_make_asgi_request_event_processor(request))
 
-                return request, error_response
+            return request, error_response
 
         cls.create_request = sentry_patched_create_request
 
 
 def patch_get_response_async(cls, _before_get_response):
     # type: (Any, Any) -> None
     old_get_response_async = cls.get_response_async
@@ -119,47 +116,44 @@
 
     import channels  # type: ignore
     from sentry_sdk.integrations.django import DjangoIntegration
 
     if channels.__version__ < "3.0.0":
         old_app = cls.__call__
 
+        @ensure_integration_enabled_async(DjangoIntegration, old_app)
         async def sentry_patched_asgi_handler(self, receive, send):
             # type: (Any, Any, Any) -> Any
-            if Hub.current.get_integration(DjangoIntegration) is None:
-                return await old_app(self, receive, send)
-
             middleware = SentryAsgiMiddleware(
                 lambda _scope: old_app.__get__(self, cls), unsafe_context_data=True
             )
 
             return await middleware(self.scope)(receive, send)
 
         cls.__call__ = sentry_patched_asgi_handler
 
     else:
         # The ASGI handler in Channels >= 3 has the same signature as
         # the Django handler.
         patch_django_asgi_handler_impl(cls)
 
 
-def wrap_async_view(hub, callback):
-    # type: (Hub, Any) -> Any
+def wrap_async_view(callback):
+    # type: (Any) -> Any
     @functools.wraps(callback)
     async def sentry_wrapped_callback(request, *args, **kwargs):
         # type: (Any, *Any, **Any) -> Any
-
-        with hub.configure_scope() as sentry_scope:
-            if sentry_scope.profile is not None:
-                sentry_scope.profile.update_active_thread_id()
-
-            with hub.start_span(
-                op=OP.VIEW_RENDER, description=request.resolver_match.view_name
-            ):
-                return await callback(request, *args, **kwargs)
+        sentry_scope = Scope.get_isolation_scope()
+        if sentry_scope.profile is not None:
+            sentry_scope.profile.update_active_thread_id()
+
+        with sentry_sdk.start_span(
+            op=OP.VIEW_RENDER, description=request.resolver_match.view_name
+        ):
+            return await callback(request, *args, **kwargs)
 
     return sentry_wrapped_callback
 
 
 def _asgi_middleware_mixin_factory(_check_middleware_span):
     # type: (Callable[..., Any]) -> Any
     """
```

### Comparing `sentry-sdk-2.0.0rc2/sentry_sdk/integrations/django/caching.py` & `sentry-sdk-2.0.0rc3/sentry_sdk/integrations/django/caching.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import functools
 from typing import TYPE_CHECKING
 
 from django import VERSION as DJANGO_VERSION
 from django.core.cache import CacheHandler
 
-from sentry_sdk import Hub
+import sentry_sdk
 from sentry_sdk.consts import OP, SPANDATA
+from sentry_sdk.utils import ensure_integration_enabled
 
 
 if TYPE_CHECKING:
     from typing import Any
     from typing import Callable
 
 
@@ -31,39 +32,37 @@
     return description
 
 
 def _patch_cache_method(cache, method_name):
     # type: (CacheHandler, str) -> None
     from sentry_sdk.integrations.django import DjangoIntegration
 
+    original_method = getattr(cache, method_name)
+
+    @ensure_integration_enabled(DjangoIntegration, original_method)
     def _instrument_call(cache, method_name, original_method, args, kwargs):
         # type: (CacheHandler, str, Callable[..., Any], Any, Any) -> Any
-        hub = Hub.current
-        integration = hub.get_integration(DjangoIntegration)
-        if integration is None or not integration.cache_spans:
-            return original_method(*args, **kwargs)
-
         description = _get_span_description(method_name, args, kwargs)
 
-        with hub.start_span(op=OP.CACHE_GET_ITEM, description=description) as span:
+        with sentry_sdk.start_span(
+            op=OP.CACHE_GET_ITEM, description=description
+        ) as span:
             value = original_method(*args, **kwargs)
 
             if value:
                 span.set_data(SPANDATA.CACHE_HIT, True)
 
                 size = len(str(value))
                 span.set_data(SPANDATA.CACHE_ITEM_SIZE, size)
 
             else:
                 span.set_data(SPANDATA.CACHE_HIT, False)
 
             return value
 
-    original_method = getattr(cache, method_name)
-
     @functools.wraps(original_method)
     def sentry_method(*args, **kwargs):
         # type: (*Any, **Any) -> Any
         return _instrument_call(cache, method_name, original_method, args, kwargs)
 
     setattr(cache, method_name, sentry_method)
 
@@ -85,16 +84,16 @@
             original_get_item = CacheHandler.__getitem__
 
             @functools.wraps(original_get_item)
             def sentry_get_item(self, alias):
                 # type: (CacheHandler, str) -> Any
                 cache = original_get_item(self, alias)
 
-                integration = Hub.current.get_integration(DjangoIntegration)
-                if integration and integration.cache_spans:
+                integration = sentry_sdk.get_client().get_integration(DjangoIntegration)
+                if integration is not None and integration.cache_spans:
                     _patch_cache(cache)
 
                 return cache
 
             CacheHandler.__getitem__ = sentry_get_item
             CacheHandler._sentry_patched = True
 
@@ -102,15 +101,15 @@
             original_create_connection = CacheHandler.create_connection
 
             @functools.wraps(original_create_connection)
             def sentry_create_connection(self, alias):
                 # type: (CacheHandler, str) -> Any
                 cache = original_create_connection(self, alias)
 
-                integration = Hub.current.get_integration(DjangoIntegration)
-                if integration and integration.cache_spans:
+                integration = sentry_sdk.get_client().get_integration(DjangoIntegration)
+                if integration is not None and integration.cache_spans:
                     _patch_cache(cache)
 
                 return cache
 
             CacheHandler.create_connection = sentry_create_connection
             CacheHandler._sentry_patched = True
```

### Comparing `sentry-sdk-2.0.0rc2/sentry_sdk/integrations/django/middleware.py` & `sentry-sdk-2.0.0rc3/sentry_sdk/integrations/django/middleware.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 Create spans from Django middleware invocations
 """
 
 from functools import wraps
 
 from django import VERSION as DJANGO_VERSION
 
-from sentry_sdk import Hub
+import sentry_sdk
 from sentry_sdk._types import TYPE_CHECKING
 from sentry_sdk.consts import OP
 from sentry_sdk.utils import (
     ContextVar,
     transaction_from_function,
     capture_internal_exceptions,
 )
@@ -67,27 +67,26 @@
 
 def _wrap_middleware(middleware, middleware_name):
     # type: (Any, str) -> Any
     from sentry_sdk.integrations.django import DjangoIntegration
 
     def _check_middleware_span(old_method):
         # type: (Callable[..., Any]) -> Optional[Span]
-        hub = Hub.current
-        integration = hub.get_integration(DjangoIntegration)
+        integration = sentry_sdk.get_client().get_integration(DjangoIntegration)
         if integration is None or not integration.middleware_spans:
             return None
 
         function_name = transaction_from_function(old_method)
 
         description = middleware_name
         function_basename = getattr(old_method, "__name__", None)
         if function_basename:
             description = "{}.{}".format(description, function_basename)
 
-        middleware_span = hub.start_span(
+        middleware_span = sentry_sdk.start_span(
             op=OP.MIDDLEWARE_DJANGO, description=description
         )
         middleware_span.set_tag("django.function_name", function_name)
         middleware_span.set_tag("django.middleware_name", middleware_name)
 
         return middleware_span
```

### Comparing `sentry-sdk-2.0.0rc2/sentry_sdk/integrations/django/signals_handlers.py` & `sentry-sdk-2.0.0rc3/sentry_sdk/integrations/django/signals_handlers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from functools import wraps
 
 from django.dispatch import Signal
 
-from sentry_sdk import Hub
+import sentry_sdk
 from sentry_sdk._types import TYPE_CHECKING
 from sentry_sdk.consts import OP
 from sentry_sdk.integrations.django import DJANGO_VERSION
 
 
 if TYPE_CHECKING:
     from collections.abc import Callable
@@ -48,38 +48,36 @@
     """
     from sentry_sdk.integrations.django import DjangoIntegration
 
     old_live_receivers = Signal._live_receivers
 
     def _sentry_live_receivers(self, sender):
         # type: (Signal, Any) -> Union[tuple[list[Callable[..., Any]], list[Callable[..., Any]]], list[Callable[..., Any]]]
-        hub = Hub.current
-
         if DJANGO_VERSION >= (5, 0):
             sync_receivers, async_receivers = old_live_receivers(self, sender)
         else:
             sync_receivers = old_live_receivers(self, sender)
             async_receivers = []
 
         def sentry_sync_receiver_wrapper(receiver):
             # type: (Callable[..., Any]) -> Callable[..., Any]
             @wraps(receiver)
             def wrapper(*args, **kwargs):
                 # type: (Any, Any) -> Any
                 signal_name = _get_receiver_name(receiver)
-                with hub.start_span(
+                with sentry_sdk.start_span(
                     op=OP.EVENT_DJANGO,
                     description=signal_name,
                 ) as span:
                     span.set_data("signal", signal_name)
                     return receiver(*args, **kwargs)
 
             return wrapper
 
-        integration = hub.get_integration(DjangoIntegration)
+        integration = sentry_sdk.get_client().get_integration(DjangoIntegration)
         if integration and integration.signals_spans:
             for idx, receiver in enumerate(sync_receivers):
                 sync_receivers[idx] = sentry_sync_receiver_wrapper(receiver)
 
         if DJANGO_VERSION >= (5, 0):
             return sync_receivers, async_receivers
         else:
```

### Comparing `sentry-sdk-2.0.0rc2/sentry_sdk/integrations/django/templates.py` & `sentry-sdk-2.0.0rc3/sentry_sdk/integrations/django/templates.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 import functools
 
 from django.template import TemplateSyntaxError
 from django.utils.safestring import mark_safe
 from django import VERSION as DJANGO_VERSION
 
-from sentry_sdk import Hub
+import sentry_sdk
+from sentry_sdk import Scope
 from sentry_sdk._types import TYPE_CHECKING
 from sentry_sdk.consts import OP
+from sentry_sdk.utils import ensure_integration_enabled
 
 if TYPE_CHECKING:
     from typing import Any
     from typing import Dict
     from typing import Optional
     from typing import Iterator
     from typing import Tuple
@@ -61,19 +63,18 @@
     from sentry_sdk.integrations.django import DjangoIntegration
 
     real_rendered_content = SimpleTemplateResponse.rendered_content
 
     @property  # type: ignore
     def rendered_content(self):
         # type: (SimpleTemplateResponse) -> str
-        hub = Hub.current
-        if hub.get_integration(DjangoIntegration) is None:
+        if sentry_sdk.get_client().get_integration(DjangoIntegration) is None:
             return real_rendered_content.fget(self)
 
-        with hub.start_span(
+        with sentry_sdk.start_span(
             op=OP.TEMPLATE_RENDER,
             description=_get_template_name_description(self.template_name),
         ) as span:
             span.set_data("context", self.context_data)
             return real_rendered_content.fget(self)
 
     SimpleTemplateResponse.rendered_content = rendered_content
@@ -81,26 +82,26 @@
     if DJANGO_VERSION < (1, 7):
         return
     import django.shortcuts
 
     real_render = django.shortcuts.render
 
     @functools.wraps(real_render)
+    @ensure_integration_enabled(DjangoIntegration, real_render)
     def render(request, template_name, context=None, *args, **kwargs):
         # type: (django.http.HttpRequest, str, Optional[Dict[str, Any]], *Any, **Any) -> django.http.HttpResponse
-        hub = Hub.current
-        if hub.get_integration(DjangoIntegration) is None:
-            return real_render(request, template_name, context, *args, **kwargs)
 
         # Inject trace meta tags into template context
         context = context or {}
         if "sentry_trace_meta" not in context:
-            context["sentry_trace_meta"] = mark_safe(hub.trace_propagation_meta())
+            context["sentry_trace_meta"] = mark_safe(
+                Scope.get_current_scope().trace_propagation_meta()
+            )
 
-        with hub.start_span(
+        with sentry_sdk.start_span(
             op=OP.TEMPLATE_RENDER,
             description=_get_template_name_description(template_name),
         ) as span:
             span.set_data("context", context)
             return real_render(request, template_name, context, *args, **kwargs)
 
     django.shortcuts.render = render
```

### Comparing `sentry-sdk-2.0.0rc2/sentry_sdk/integrations/django/transactions.py` & `sentry-sdk-2.0.0rc3/sentry_sdk/integrations/django/transactions.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc2/sentry_sdk/integrations/django/views.py` & `sentry-sdk-2.0.0rc3/sentry_sdk/integrations/django/views.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import functools
 
+import sentry_sdk
+from sentry_sdk import Scope
 from sentry_sdk.consts import OP
-from sentry_sdk.hub import Hub
 from sentry_sdk._types import TYPE_CHECKING
 
 if TYPE_CHECKING:
     from typing import Any
 
 
 try:
@@ -28,60 +29,58 @@
     from sentry_sdk.integrations.django import DjangoIntegration
 
     old_make_view_atomic = BaseHandler.make_view_atomic
     old_render = SimpleTemplateResponse.render
 
     def sentry_patched_render(self):
         # type: (SimpleTemplateResponse) -> Any
-        hub = Hub.current
-        with hub.start_span(
+        with sentry_sdk.start_span(
             op=OP.VIEW_RESPONSE_RENDER, description="serialize response"
         ):
             return old_render(self)
 
     @functools.wraps(old_make_view_atomic)
     def sentry_patched_make_view_atomic(self, *args, **kwargs):
         # type: (Any, *Any, **Any) -> Any
         callback = old_make_view_atomic(self, *args, **kwargs)
 
         # XXX: The wrapper function is created for every request. Find more
         # efficient way to wrap views (or build a cache?)
 
-        hub = Hub.current
-        integration = hub.get_integration(DjangoIntegration)
+        integration = sentry_sdk.get_client().get_integration(DjangoIntegration)
         if integration is not None and integration.middleware_spans:
             is_async_view = (
                 iscoroutinefunction is not None
                 and wrap_async_view is not None
                 and iscoroutinefunction(callback)
             )
             if is_async_view:
-                sentry_wrapped_callback = wrap_async_view(hub, callback)
+                sentry_wrapped_callback = wrap_async_view(callback)
             else:
-                sentry_wrapped_callback = _wrap_sync_view(hub, callback)
+                sentry_wrapped_callback = _wrap_sync_view(callback)
 
         else:
             sentry_wrapped_callback = callback
 
         return sentry_wrapped_callback
 
     SimpleTemplateResponse.render = sentry_patched_render
     BaseHandler.make_view_atomic = sentry_patched_make_view_atomic
 
 
-def _wrap_sync_view(hub, callback):
-    # type: (Hub, Any) -> Any
+def _wrap_sync_view(callback):
+    # type: (Any) -> Any
     @functools.wraps(callback)
     def sentry_wrapped_callback(request, *args, **kwargs):
         # type: (Any, *Any, **Any) -> Any
-        with hub.configure_scope() as sentry_scope:
-            # set the active thread id to the handler thread for sync views
-            # this isn't necessary for async views since that runs on main
-            if sentry_scope.profile is not None:
-                sentry_scope.profile.update_active_thread_id()
-
-            with hub.start_span(
-                op=OP.VIEW_RENDER, description=request.resolver_match.view_name
-            ):
-                return callback(request, *args, **kwargs)
+        sentry_scope = Scope.get_isolation_scope()
+        # set the active thread id to the handler thread for sync views
+        # this isn't necessary for async views since that runs on main
+        if sentry_scope.profile is not None:
+            sentry_scope.profile.update_active_thread_id()
+
+        with sentry_sdk.start_span(
+            op=OP.VIEW_RENDER, description=request.resolver_match.view_name
+        ):
+            return callback(request, *args, **kwargs)
 
     return sentry_wrapped_callback
```

### Comparing `sentry-sdk-2.0.0rc2/sentry_sdk/integrations/excepthook.py` & `sentry-sdk-2.0.0rc3/sentry_sdk/integrations/excepthook.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import sys
 
-from sentry_sdk.hub import Hub
+import sentry_sdk
 from sentry_sdk.utils import capture_internal_exceptions, event_from_exception
 from sentry_sdk.integrations import Integration
 
 from sentry_sdk._types import TYPE_CHECKING
 
 if TYPE_CHECKING:
     from typing import Callable
@@ -41,28 +41,24 @@
         sys.excepthook = _make_excepthook(sys.excepthook)
 
 
 def _make_excepthook(old_excepthook):
     # type: (Excepthook) -> Excepthook
     def sentry_sdk_excepthook(type_, value, traceback):
         # type: (Type[BaseException], BaseException, Optional[TracebackType]) -> None
-        hub = Hub.current
-        integration = hub.get_integration(ExcepthookIntegration)
+        integration = sentry_sdk.get_client().get_integration(ExcepthookIntegration)
 
         if integration is not None and _should_send(integration.always_run):
-            # If an integration is there, a client has to be there.
-            client = hub.client  # type: Any
-
             with capture_internal_exceptions():
                 event, hint = event_from_exception(
                     (type_, value, traceback),
-                    client_options=client.options,
+                    client_options=sentry_sdk.get_client().options,
                     mechanism={"type": "excepthook", "handled": False},
                 )
-                hub.capture_event(event, hint=hint)
+                sentry_sdk.capture_event(event, hint=hint)
 
         return old_excepthook(type_, value, traceback)
 
     return sentry_sdk_excepthook
 
 
 def _should_send(always_run=False):
```

### Comparing `sentry-sdk-2.0.0rc2/sentry_sdk/integrations/executing.py` & `sentry-sdk-2.0.0rc3/sentry_sdk/integrations/executing.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc2/sentry_sdk/integrations/falcon.py` & `sentry-sdk-2.0.0rc3/sentry_sdk/integrations/falcon.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc2/sentry_sdk/integrations/fastapi.py` & `sentry-sdk-2.0.0rc3/sentry_sdk/integrations/fastapi.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 import asyncio
 from copy import deepcopy
 from functools import wraps
 
+import sentry_sdk
 from sentry_sdk._types import TYPE_CHECKING
-from sentry_sdk.hub import Hub, _should_send_default_pii
 from sentry_sdk.integrations import DidNotEnable
-from sentry_sdk.scope import Scope
+from sentry_sdk.scope import Scope, should_send_default_pii
 from sentry_sdk.tracing import SOURCE_FOR_STYLE, TRANSACTION_SOURCE_ROUTE
-from sentry_sdk.utils import transaction_from_function, logger
+from sentry_sdk.utils import (
+    transaction_from_function,
+    logger,
+    ensure_integration_enabled_async,
+)
 
 if TYPE_CHECKING:
     from typing import Any, Callable, Dict
     from sentry_sdk._types import Event
 
 try:
     from sentry_sdk.integrations.starlette import (
@@ -80,61 +84,57 @@
             and not asyncio.iscoroutinefunction(dependant.call)
         ):
             old_call = dependant.call
 
             @wraps(old_call)
             def _sentry_call(*args, **kwargs):
                 # type: (*Any, **Any) -> Any
-                hub = Hub.current
-                with hub.configure_scope() as sentry_scope:
-                    if sentry_scope.profile is not None:
-                        sentry_scope.profile.update_active_thread_id()
-                    return old_call(*args, **kwargs)
+                sentry_scope = Scope.get_isolation_scope()
+                if sentry_scope.profile is not None:
+                    sentry_scope.profile.update_active_thread_id()
+                return old_call(*args, **kwargs)
 
             dependant.call = _sentry_call
 
         old_app = old_get_request_handler(*args, **kwargs)
 
+        @ensure_integration_enabled_async(FastApiIntegration, old_app)
         async def _sentry_app(*args, **kwargs):
             # type: (*Any, **Any) -> Any
-            hub = Hub.current
-            integration = hub.get_integration(FastApiIntegration)
-            if integration is None:
-                return await old_app(*args, **kwargs)
-
+            integration = sentry_sdk.get_client().get_integration(FastApiIntegration)
             request = args[0]
 
             _set_transaction_name_and_source(
                 Scope.get_current_scope(), integration.transaction_style, request
             )
-            with hub.configure_scope() as sentry_scope:
-                extractor = StarletteRequestExtractor(request)
-                info = await extractor.extract_request_info()
-
-                def _make_request_event_processor(req, integration):
-                    # type: (Any, Any) -> Callable[[Event, Dict[str, Any]], Event]
-                    def event_processor(event, hint):
-                        # type: (Event, Dict[str, Any]) -> Event
-
-                        # Extract information from request
-                        request_info = event.get("request", {})
-                        if info:
-                            if "cookies" in info and _should_send_default_pii():
-                                request_info["cookies"] = info["cookies"]
-                            if "data" in info:
-                                request_info["data"] = info["data"]
-                        event["request"] = deepcopy(request_info)
-
-                        return event
-
-                    return event_processor
-
-                sentry_scope._name = FastApiIntegration.identifier
-                sentry_scope.add_event_processor(
-                    _make_request_event_processor(request, integration)
-                )
+            sentry_scope = Scope.get_isolation_scope()
+            extractor = StarletteRequestExtractor(request)
+            info = await extractor.extract_request_info()
+
+            def _make_request_event_processor(req, integration):
+                # type: (Any, Any) -> Callable[[Event, Dict[str, Any]], Event]
+                def event_processor(event, hint):
+                    # type: (Event, Dict[str, Any]) -> Event
+
+                    # Extract information from request
+                    request_info = event.get("request", {})
+                    if info:
+                        if "cookies" in info and should_send_default_pii():
+                            request_info["cookies"] = info["cookies"]
+                        if "data" in info:
+                            request_info["data"] = info["data"]
+                    event["request"] = deepcopy(request_info)
+
+                    return event
+
+                return event_processor
+
+            sentry_scope._name = FastApiIntegration.identifier
+            sentry_scope.add_event_processor(
+                _make_request_event_processor(request, integration)
+            )
 
             return await old_app(*args, **kwargs)
 
         return _sentry_app
 
     fastapi.routing.get_request_handler = _sentry_get_request_handler
```

### Comparing `sentry-sdk-2.0.0rc2/sentry_sdk/integrations/flask.py` & `sentry-sdk-2.0.0rc3/sentry_sdk/integrations/flask.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc2/sentry_sdk/integrations/gcp.py` & `sentry-sdk-2.0.0rc3/sentry_sdk/integrations/gcp.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc2/sentry_sdk/integrations/gnu_backtrace.py` & `sentry-sdk-2.0.0rc3/sentry_sdk/integrations/gnu_backtrace.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc2/sentry_sdk/integrations/gql.py` & `sentry-sdk-2.0.0rc3/sentry_sdk/integrations/gql.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,16 @@
-from sentry_sdk.utils import event_from_exception, parse_version
-from sentry_sdk.hub import Hub, _should_send_default_pii
+import sentry_sdk
+from sentry_sdk.utils import (
+    event_from_exception,
+    ensure_integration_enabled,
+    parse_version,
+)
+
 from sentry_sdk.integrations import DidNotEnable, Integration
+from sentry_sdk.scope import Scope, should_send_default_pii
 
 try:
     import gql  # type: ignore[import-not-found]
     from graphql import print_ast, get_operation_ast, DocumentNode, VariableDefinitionNode  # type: ignore[import-not-found]
     from gql.transport import Transport, AsyncTransport  # type: ignore[import-not-found]
     from gql.transport.exceptions import TransportQueryError  # type: ignore[import-not-found]
 except ImportError:
@@ -81,33 +87,30 @@
     return request_info
 
 
 def _patch_execute():
     # type: () -> None
     real_execute = gql.Client.execute
 
+    @ensure_integration_enabled(GQLIntegration, real_execute)
     def sentry_patched_execute(self, document, *args, **kwargs):
         # type: (gql.Client, DocumentNode, Any, Any) -> Any
-        hub = Hub.current
-        if hub.get_integration(GQLIntegration) is None:
-            return real_execute(self, document, *args, **kwargs)
-
-        with Hub.current.configure_scope() as scope:
-            scope.add_event_processor(_make_gql_event_processor(self, document))
+        scope = Scope.get_isolation_scope()
+        scope.add_event_processor(_make_gql_event_processor(self, document))
 
         try:
             return real_execute(self, document, *args, **kwargs)
         except TransportQueryError as e:
             event, hint = event_from_exception(
                 e,
-                client_options=hub.client.options if hub.client is not None else None,
+                client_options=sentry_sdk.get_client().options,
                 mechanism={"type": "gql", "handled": False},
             )
 
-            hub.capture_event(event, hint)
+            sentry_sdk.capture_event(event, hint)
             raise e
 
     gql.Client.execute = sentry_patched_execute
 
 
 def _make_gql_event_processor(client, document):
     # type: (gql.Client, DocumentNode) -> EventProcessor
@@ -122,15 +125,15 @@
         request.update(
             {
                 "api_target": "graphql",
                 **_request_info_from_transport(client.transport),
             }
         )
 
-        if _should_send_default_pii():
+        if should_send_default_pii():
             request["data"] = _data_from_document(document)
             contexts = event.setdefault("contexts", {})
             response = contexts.setdefault("response", {})
             response.update(
                 {
                     "data": {"errors": errors},
                     "type": response,
```

### Comparing `sentry-sdk-2.0.0rc2/sentry_sdk/integrations/graphene.py` & `sentry-sdk-2.0.0rc3/sentry_sdk/integrations/graphene.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc2/sentry_sdk/integrations/grpc/__init__.py` & `sentry-sdk-2.0.0rc3/sentry_sdk/integrations/grpc/__init__.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc2/sentry_sdk/integrations/grpc/aio/client.py` & `sentry-sdk-2.0.0rc3/sentry_sdk/integrations/grpc/aio/client.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc2/sentry_sdk/integrations/grpc/aio/server.py` & `sentry-sdk-2.0.0rc3/sentry_sdk/integrations/grpc/aio/server.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc2/sentry_sdk/integrations/grpc/client.py` & `sentry-sdk-2.0.0rc3/sentry_sdk/integrations/grpc/client.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc2/sentry_sdk/integrations/grpc/server.py` & `sentry-sdk-2.0.0rc3/sentry_sdk/integrations/grpc/server.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc2/sentry_sdk/integrations/httpx.py` & `sentry-sdk-2.0.0rc3/sentry_sdk/integrations/httpx.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,18 @@
-from sentry_sdk import Hub
+import sentry_sdk
 from sentry_sdk.consts import OP, SPANDATA
 from sentry_sdk.integrations import Integration, DidNotEnable
+from sentry_sdk.scope import Scope
 from sentry_sdk.tracing import BAGGAGE_HEADER_NAME
 from sentry_sdk.tracing_utils import should_propagate_trace
 from sentry_sdk.utils import (
     SENSITIVE_DATA_SUBSTITUTE,
     capture_internal_exceptions,
+    ensure_integration_enabled,
+    ensure_integration_enabled_async,
     logger,
     parse_url,
 )
 
 from sentry_sdk._types import TYPE_CHECKING
 
 if TYPE_CHECKING:
@@ -38,40 +41,40 @@
         _install_httpx_async_client()
 
 
 def _install_httpx_client():
     # type: () -> None
     real_send = Client.send
 
+    @ensure_integration_enabled(HttpxIntegration, real_send)
     def send(self, request, **kwargs):
         # type: (Client, Request, **Any) -> Response
-        hub = Hub.current
-        if hub.get_integration(HttpxIntegration) is None:
-            return real_send(self, request, **kwargs)
-
         parsed_url = None
         with capture_internal_exceptions():
             parsed_url = parse_url(str(request.url), sanitize=False)
 
-        with hub.start_span(
+        with sentry_sdk.start_span(
             op=OP.HTTP_CLIENT,
             description="%s %s"
             % (
                 request.method,
                 parsed_url.url if parsed_url else SENSITIVE_DATA_SUBSTITUTE,
             ),
         ) as span:
             span.set_data(SPANDATA.HTTP_METHOD, request.method)
             if parsed_url is not None:
                 span.set_data("url", parsed_url.url)
                 span.set_data(SPANDATA.HTTP_QUERY, parsed_url.query)
                 span.set_data(SPANDATA.HTTP_FRAGMENT, parsed_url.fragment)
 
-            if should_propagate_trace(hub, str(request.url)):
-                for key, value in hub.iter_trace_propagation_headers():
+            if should_propagate_trace(sentry_sdk.get_client(), str(request.url)):
+                for (
+                    key,
+                    value,
+                ) in Scope.get_current_scope().iter_trace_propagation_headers():
                     logger.debug(
                         "[Tracing] Adding `{key}` header {value} to outgoing request to {url}.".format(
                             key=key, value=value, url=request.url
                         )
                     )
                     if key == BAGGAGE_HEADER_NAME and request.headers.get(
                         BAGGAGE_HEADER_NAME
@@ -91,40 +94,40 @@
     Client.send = send
 
 
 def _install_httpx_async_client():
     # type: () -> None
     real_send = AsyncClient.send
 
+    @ensure_integration_enabled_async(HttpxIntegration, real_send)
     async def send(self, request, **kwargs):
         # type: (AsyncClient, Request, **Any) -> Response
-        hub = Hub.current
-        if hub.get_integration(HttpxIntegration) is None:
-            return await real_send(self, request, **kwargs)
-
         parsed_url = None
         with capture_internal_exceptions():
             parsed_url = parse_url(str(request.url), sanitize=False)
 
-        with hub.start_span(
+        with sentry_sdk.start_span(
             op=OP.HTTP_CLIENT,
             description="%s %s"
             % (
                 request.method,
                 parsed_url.url if parsed_url else SENSITIVE_DATA_SUBSTITUTE,
             ),
         ) as span:
             span.set_data(SPANDATA.HTTP_METHOD, request.method)
             if parsed_url is not None:
                 span.set_data("url", parsed_url.url)
                 span.set_data(SPANDATA.HTTP_QUERY, parsed_url.query)
                 span.set_data(SPANDATA.HTTP_FRAGMENT, parsed_url.fragment)
 
-            if should_propagate_trace(hub, str(request.url)):
-                for key, value in hub.iter_trace_propagation_headers():
+            if should_propagate_trace(sentry_sdk.get_client(), str(request.url)):
+                for (
+                    key,
+                    value,
+                ) in Scope.get_current_scope().iter_trace_propagation_headers():
                     logger.debug(
                         "[Tracing] Adding `{key}` header {value} to outgoing request to {url}.".format(
                             key=key, value=value, url=request.url
                         )
                     )
                     if key == BAGGAGE_HEADER_NAME and request.headers.get(
                         BAGGAGE_HEADER_NAME
```

### Comparing `sentry-sdk-2.0.0rc2/sentry_sdk/integrations/huey.py` & `sentry-sdk-2.0.0rc3/sentry_sdk/integrations/huey.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc2/sentry_sdk/integrations/logging.py` & `sentry-sdk-2.0.0rc3/sentry_sdk/integrations/logging.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import logging
 from datetime import datetime, timezone
 from fnmatch import fnmatch
 
-from sentry_sdk.hub import Hub
+import sentry_sdk
 from sentry_sdk.utils import (
     to_string,
     event_from_exception,
     current_stacktrace,
     capture_internal_exceptions,
 )
 from sentry_sdk.integrations import Integration
@@ -97,15 +97,17 @@
                 return old_callhandlers(self, record)
             finally:
                 # This check is done twice, once also here before we even get
                 # the integration.  Otherwise we have a high chance of getting
                 # into a recursion error when the integration is resolved
                 # (this also is slower).
                 if ignored_loggers is not None and record.name not in ignored_loggers:
-                    integration = Hub.current.get_integration(LoggingIntegration)
+                    integration = sentry_sdk.get_client().get_integration(
+                        LoggingIntegration
+                    )
                     if integration is not None:
                         integration._handle_record(record)
 
         logging.Logger.callHandlers = sentry_patched_callhandlers  # type: ignore
 
 
 class _BaseHandler(logging.Handler, object):
@@ -177,19 +179,19 @@
             return self._emit(record)
 
     def _emit(self, record):
         # type: (LogRecord) -> None
         if not self._can_record(record):
             return
 
-        hub = Hub.current
-        if hub.client is None:
+        client = sentry_sdk.get_client()
+        if not client.is_active():
             return
 
-        client_options = hub.client.options
+        client_options = client.options
 
         # exc_info might be None or (None, None, None)
         #
         # exc_info may also be any falsy value due to Python stdlib being
         # liberal with what it receives and Celery's billiard being "liberal"
         # with what it sends. See
         # https://github.com/getsentry/sentry-python/issues/904
@@ -246,15 +248,15 @@
             event["logentry"] = {
                 "message": to_string(record.msg),
                 "params": record.args,
             }
 
         event["extra"] = self._extra_from_record(record)
 
-        hub.capture_event(event, hint=hint)
+        sentry_sdk.capture_event(event, hint=hint)
 
 
 # Legacy name
 SentryHandler = EventHandler
 
 
 class BreadcrumbHandler(_BaseHandler):
@@ -271,15 +273,15 @@
             return self._emit(record)
 
     def _emit(self, record):
         # type: (LogRecord) -> None
         if not self._can_record(record):
             return
 
-        Hub.current.add_breadcrumb(
+        sentry_sdk.add_breadcrumb(
             self._breadcrumb_from_record(record), hint={"log_record": record}
         )
 
     def _breadcrumb_from_record(self, record):
         # type: (LogRecord) -> Dict[str, Any]
         return {
             "type": "log",
```

### Comparing `sentry-sdk-2.0.0rc2/sentry_sdk/integrations/loguru.py` & `sentry-sdk-2.0.0rc3/sentry_sdk/integrations/loguru.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc2/sentry_sdk/integrations/modules.py` & `sentry-sdk-2.0.0rc3/sentry_sdk/integrations/modules.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from sentry_sdk.hub import Hub
+import sentry_sdk
 from sentry_sdk.integrations import Integration
 from sentry_sdk.scope import add_global_event_processor
 from sentry_sdk.utils import _get_installed_modules
 
 from sentry_sdk._types import TYPE_CHECKING
 
 if TYPE_CHECKING:
@@ -18,12 +18,12 @@
         # type: () -> None
         @add_global_event_processor
         def processor(event, hint):
             # type: (Event, Any) -> Event
             if event.get("type") == "transaction":
                 return event
 
-            if Hub.current.get_integration(ModulesIntegration) is None:
+            if sentry_sdk.get_client().get_integration(ModulesIntegration) is None:
                 return event
 
             event["modules"] = _get_installed_modules()
             return event
```

### Comparing `sentry-sdk-2.0.0rc2/sentry_sdk/integrations/openai.py` & `sentry-sdk-2.0.0rc3/sentry_sdk/integrations/openai.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,17 +4,22 @@
 from sentry_sdk._types import TYPE_CHECKING
 
 if TYPE_CHECKING:
     from typing import Any, Iterable, List, Optional, Callable, Iterator
     from sentry_sdk.tracing import Span
 
 import sentry_sdk
-from sentry_sdk.hub import Hub, _should_send_default_pii
+from sentry_sdk.scope import should_send_default_pii
 from sentry_sdk.integrations import DidNotEnable, Integration
-from sentry_sdk.utils import logger, capture_internal_exceptions, event_from_exception
+from sentry_sdk.utils import (
+    logger,
+    capture_internal_exceptions,
+    event_from_exception,
+    ensure_integration_enabled,
+)
 
 try:
     from openai.resources.chat.completions import Completions
     from openai.resources import Embeddings
 
     if TYPE_CHECKING:
         from openai.types.chat import ChatCompletionMessageParam, ChatCompletionChunk
@@ -58,24 +63,22 @@
     @staticmethod
     def setup_once():
         # type: () -> None
         Completions.create = _wrap_chat_completion_create(Completions.create)
         Embeddings.create = _wrap_embeddings_create(Embeddings.create)
 
 
-def _capture_exception(hub, exc):
-    # type: (Hub, Any) -> None
-
-    if hub.client is not None:
-        event, hint = event_from_exception(
-            exc,
-            client_options=hub.client.options,
-            mechanism={"type": "openai", "handled": False},
-        )
-        hub.capture_event(event, hint=hint)
+def _capture_exception(exc):
+    # type: (Any) -> None
+    event, hint = event_from_exception(
+        exc,
+        client_options=sentry_sdk.get_client().options,
+        mechanism={"type": "openai", "handled": False},
+    )
+    sentry_sdk.capture_event(event, hint=hint)
 
 
 def _normalize_data(data):
     # type: (Any) -> Any
 
     # convert pydantic data (e.g. OpenAI v1+) to json compatible format
     if hasattr(data, "model_dump"):
@@ -141,24 +144,17 @@
     if total_tokens != 0:
         set_data_normalized(span, TOTAL_TOKENS_USED, total_tokens)
 
 
 def _wrap_chat_completion_create(f):
     # type: (Callable[..., Any]) -> Callable[..., Any]
     @wraps(f)
+    @ensure_integration_enabled(OpenAIIntegration, f)
     def new_chat_completion(*args, **kwargs):
         # type: (*Any, **Any) -> Any
-        hub = Hub.current
-        if not hub:
-            return f(*args, **kwargs)
-
-        integration = hub.get_integration(OpenAIIntegration)  # type: OpenAIIntegration
-        if not integration:
-            return f(*args, **kwargs)
-
         if "messages" not in kwargs:
             # invalid call (in all versions of openai), let it return error
             return f(*args, **kwargs)
 
         try:
             iter(kwargs["messages"])
         except TypeError:
@@ -173,27 +169,29 @@
         span = sentry_sdk.start_span(
             op=consts.OP.OPENAI_CHAT_COMPLETIONS_CREATE, description="Chat Completion"
         )
         span.__enter__()
         try:
             res = f(*args, **kwargs)
         except Exception as e:
-            _capture_exception(Hub.current, e)
+            _capture_exception(e)
             span.__exit__(None, None, None)
             raise e from None
 
+        integration = sentry_sdk.get_client().get_integration(OpenAIIntegration)
+
         with capture_internal_exceptions():
-            if _should_send_default_pii() and integration.include_prompts:
+            if should_send_default_pii() and integration.include_prompts:
                 set_data_normalized(span, "ai.input_messages", messages)
 
             set_data_normalized(span, "ai.model_id", model)
             set_data_normalized(span, "ai.streaming", streaming)
 
             if hasattr(res, "choices"):
-                if _should_send_default_pii() and integration.include_prompts:
+                if should_send_default_pii() and integration.include_prompts:
                     set_data_normalized(
                         span,
                         "ai.responses",
                         list(map(lambda x: x.message, res.choices)),
                     )
                 _calculate_chat_completion_usage(messages, res, span)
                 span.__exit__(None, None, None)
@@ -219,15 +217,15 @@
                                     choice_index += 1
                             yield x
                         if len(data_buf) > 0:
                             all_responses = list(
                                 map(lambda chunk: "".join(chunk), data_buf)
                             )
                             if (
-                                _should_send_default_pii()
+                                should_send_default_pii()
                                 and integration.include_prompts
                             ):
                                 set_data_normalized(span, "ai.responses", all_responses)
                             _calculate_chat_completion_usage(
                                 messages, res, span, all_responses
                             )
                     span.__exit__(None, None, None)
@@ -241,46 +239,39 @@
     return new_chat_completion
 
 
 def _wrap_embeddings_create(f):
     # type: (Callable[..., Any]) -> Callable[..., Any]
 
     @wraps(f)
+    @ensure_integration_enabled(OpenAIIntegration, f)
     def new_embeddings_create(*args, **kwargs):
         # type: (*Any, **Any) -> Any
-
-        hub = Hub.current
-        if not hub:
-            return f(*args, **kwargs)
-
-        integration = hub.get_integration(OpenAIIntegration)  # type: OpenAIIntegration
-        if not integration:
-            return f(*args, **kwargs)
-
         with sentry_sdk.start_span(
             op=consts.OP.OPENAI_EMBEDDINGS_CREATE,
             description="OpenAI Embedding Creation",
         ) as span:
+            integration = sentry_sdk.get_client().get_integration(OpenAIIntegration)
             if "input" in kwargs and (
-                _should_send_default_pii() and integration.include_prompts
+                should_send_default_pii() and integration.include_prompts
             ):
                 if isinstance(kwargs["input"], str):
                     set_data_normalized(span, "ai.input_messages", [kwargs["input"]])
                 elif (
                     isinstance(kwargs["input"], list)
                     and len(kwargs["input"]) > 0
                     and isinstance(kwargs["input"][0], str)
                 ):
                     set_data_normalized(span, "ai.input_messages", kwargs["input"])
             if "model" in kwargs:
                 set_data_normalized(span, "ai.model_id", kwargs["model"])
             try:
                 response = f(*args, **kwargs)
             except Exception as e:
-                _capture_exception(Hub.current, e)
+                _capture_exception(e)
                 raise e from None
 
             prompt_tokens = 0
             total_tokens = 0
             if hasattr(response, "usage"):
                 if hasattr(response.usage, "prompt_tokens") and isinstance(
                     response.usage.prompt_tokens, int
```

### Comparing `sentry-sdk-2.0.0rc2/sentry_sdk/integrations/opentelemetry/integration.py` & `sentry-sdk-2.0.0rc3/sentry_sdk/integrations/opentelemetry/integration.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc2/sentry_sdk/integrations/opentelemetry/propagator.py` & `sentry-sdk-2.0.0rc3/sentry_sdk/integrations/opentelemetry/propagator.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc2/sentry_sdk/integrations/opentelemetry/span_processor.py` & `sentry-sdk-2.0.0rc3/sentry_sdk/integrations/opentelemetry/span_processor.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc2/sentry_sdk/integrations/pure_eval.py` & `sentry-sdk-2.0.0rc3/sentry_sdk/integrations/pure_eval.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc2/sentry_sdk/integrations/pymongo.py` & `sentry-sdk-2.0.0rc3/sentry_sdk/integrations/pymongo.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc2/sentry_sdk/integrations/pyramid.py` & `sentry-sdk-2.0.0rc3/sentry_sdk/integrations/pyramid.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc2/sentry_sdk/integrations/quart.py` & `sentry-sdk-2.0.0rc3/sentry_sdk/integrations/quart.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc2/sentry_sdk/integrations/redis/__init__.py` & `sentry-sdk-2.0.0rc3/sentry_sdk/integrations/redis/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,16 @@
-from sentry_sdk import Hub
+import sentry_sdk
 from sentry_sdk.consts import OP, SPANDATA
 from sentry_sdk.hub import _should_send_default_pii
 from sentry_sdk.integrations import Integration, DidNotEnable
 from sentry_sdk._types import TYPE_CHECKING
 from sentry_sdk.utils import (
     SENSITIVE_DATA_SUBSTITUTE,
     capture_internal_exceptions,
+    ensure_integration_enabled,
     logger,
 )
 
 if TYPE_CHECKING:
     from collections.abc import Callable
     from typing import Any, Dict, Sequence
     from redis import Redis, RedisCluster
@@ -172,22 +173,18 @@
         )
 
 
 def patch_redis_pipeline(pipeline_cls, is_cluster, get_command_args_fn, set_db_data_fn):
     # type: (Any, bool, Any, Callable[[Span, Any], None]) -> None
     old_execute = pipeline_cls.execute
 
+    @ensure_integration_enabled(RedisIntegration, old_execute)
     def sentry_patched_execute(self, *args, **kwargs):
         # type: (Any, *Any, **Any) -> Any
-        hub = Hub.current
-
-        if hub.get_integration(RedisIntegration) is None:
-            return old_execute(self, *args, **kwargs)
-
-        with hub.start_span(
+        with sentry_sdk.start_span(
             op=OP.DB_REDIS, description="redis.pipeline.execute"
         ) as span:
             with capture_internal_exceptions():
                 set_db_data_fn(span, self)
                 _set_pipeline_data(
                     span,
                     is_cluster,
@@ -205,31 +202,27 @@
     # type: (Any, bool, Callable[[Span, Any], None]) -> None
     """
     This function can be used to instrument custom redis client classes or
     subclasses.
     """
     old_execute_command = cls.execute_command
 
+    @ensure_integration_enabled(RedisIntegration, old_execute_command)
     def sentry_patched_execute_command(self, name, *args, **kwargs):
         # type: (Any, str, *Any, **Any) -> Any
-        hub = Hub.current
-        integration = hub.get_integration(RedisIntegration)
-
-        if integration is None:
-            return old_execute_command(self, name, *args, **kwargs)
-
+        integration = sentry_sdk.get_client().get_integration(RedisIntegration)
         description = _get_span_description(name, *args)
 
         data_should_be_truncated = (
             integration.max_data_size and len(description) > integration.max_data_size
         )
         if data_should_be_truncated:
             description = description[: integration.max_data_size - len("...")] + "..."
 
-        with hub.start_span(op=OP.DB_REDIS, description=description) as span:
+        with sentry_sdk.start_span(op=OP.DB_REDIS, description=description) as span:
             set_db_data_fn(span, self)
             _set_client_data(span, is_cluster, name, *args)
 
             return old_execute_command(self, name, *args, **kwargs)
 
     cls.execute_command = sentry_patched_execute_command
```

### Comparing `sentry-sdk-2.0.0rc2/sentry_sdk/integrations/redis/asyncio.py` & `sentry-sdk-2.0.0rc3/sentry_sdk/integrations/redis/asyncio.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,70 +1,65 @@
-from sentry_sdk import Hub
+import sentry_sdk
 from sentry_sdk.consts import OP
 from sentry_sdk.integrations.redis import (
     RedisIntegration,
     _get_span_description,
     _set_client_data,
     _set_pipeline_data,
 )
 from sentry_sdk._types import TYPE_CHECKING
 from sentry_sdk.tracing import Span
-from sentry_sdk.utils import capture_internal_exceptions
+from sentry_sdk.utils import (
+    capture_internal_exceptions,
+    ensure_integration_enabled_async,
+)
 
 if TYPE_CHECKING:
     from collections.abc import Callable
     from typing import Any, Union
     from redis.asyncio.client import Pipeline, StrictRedis
     from redis.asyncio.cluster import ClusterPipeline, RedisCluster
 
 
 def patch_redis_async_pipeline(
     pipeline_cls, is_cluster, get_command_args_fn, set_db_data_fn
 ):
     # type: (Union[type[Pipeline[Any]], type[ClusterPipeline[Any]]], bool, Any, Callable[[Span, Any], None]) -> None
     old_execute = pipeline_cls.execute
 
+    @ensure_integration_enabled_async(RedisIntegration, old_execute)
     async def _sentry_execute(self, *args, **kwargs):
         # type: (Any, *Any, **Any) -> Any
-        hub = Hub.current
-
-        if hub.get_integration(RedisIntegration) is None:
-            return await old_execute(self, *args, **kwargs)
-
-        with hub.start_span(
+        with sentry_sdk.start_span(
             op=OP.DB_REDIS, description="redis.pipeline.execute"
         ) as span:
             with capture_internal_exceptions():
                 set_db_data_fn(span, self)
                 _set_pipeline_data(
                     span,
                     is_cluster,
                     get_command_args_fn,
                     False if is_cluster else self.is_transaction,
                     self._command_stack if is_cluster else self.command_stack,
                 )
 
             return await old_execute(self, *args, **kwargs)
 
-    pipeline_cls.execute = _sentry_execute  # type: ignore[method-assign]
+    pipeline_cls.execute = _sentry_execute  # type: ignore
 
 
 def patch_redis_async_client(cls, is_cluster, set_db_data_fn):
     # type: (Union[type[StrictRedis[Any]], type[RedisCluster[Any]]], bool, Callable[[Span, Any], None]) -> None
     old_execute_command = cls.execute_command
 
+    @ensure_integration_enabled_async(RedisIntegration, old_execute_command)  # type: ignore
     async def _sentry_execute_command(self, name, *args, **kwargs):
         # type: (Any, str, *Any, **Any) -> Any
-        hub = Hub.current
-
-        if hub.get_integration(RedisIntegration) is None:
-            return await old_execute_command(self, name, *args, **kwargs)
-
         description = _get_span_description(name, *args)
 
-        with hub.start_span(op=OP.DB_REDIS, description=description) as span:
+        with sentry_sdk.start_span(op=OP.DB_REDIS, description=description) as span:
             set_db_data_fn(span, self)
             _set_client_data(span, is_cluster, name, *args)
 
             return await old_execute_command(self, name, *args, **kwargs)
 
-    cls.execute_command = _sentry_execute_command  # type: ignore[method-assign]
+    cls.execute_command = _sentry_execute_command  # type: ignore
```

### Comparing `sentry-sdk-2.0.0rc2/sentry_sdk/integrations/rq.py` & `sentry-sdk-2.0.0rc3/sentry_sdk/integrations/rq.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc2/sentry_sdk/integrations/sanic.py` & `sentry-sdk-2.0.0rc3/sentry_sdk/integrations/sanic.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc2/sentry_sdk/integrations/serverless.py` & `sentry-sdk-2.0.0rc3/sentry_sdk/integrations/serverless.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc2/sentry_sdk/integrations/socket.py` & `sentry-sdk-2.0.0rc3/sentry_sdk/integrations/socket.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc2/sentry_sdk/integrations/spark/spark_driver.py` & `sentry-sdk-2.0.0rc3/sentry_sdk/integrations/spark/spark_driver.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc2/sentry_sdk/integrations/spark/spark_worker.py` & `sentry-sdk-2.0.0rc3/sentry_sdk/integrations/spark/spark_worker.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc2/sentry_sdk/integrations/sqlalchemy.py` & `sentry-sdk-2.0.0rc3/sentry_sdk/integrations/sqlalchemy.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
+import sentry_sdk
 from sentry_sdk._types import TYPE_CHECKING
 from sentry_sdk.consts import SPANDATA
 from sentry_sdk.db.explain_plan.sqlalchemy import attach_explain_plan_to_span
-from sentry_sdk.hub import Hub
 from sentry_sdk.integrations import Integration, DidNotEnable
 from sentry_sdk.tracing_utils import add_query_source, record_sql_queries
 from sentry_sdk.utils import capture_internal_exceptions, parse_version
 
 try:
     from sqlalchemy.engine import Engine  # type: ignore
     from sqlalchemy.event import listen  # type: ignore
@@ -43,63 +43,61 @@
         listen(Engine, "handle_error", _handle_error)
 
 
 def _before_cursor_execute(
     conn, cursor, statement, parameters, context, executemany, *args
 ):
     # type: (Any, Any, Any, Any, Any, bool, *Any) -> None
-    hub = Hub.current
-    if hub.get_integration(SqlalchemyIntegration) is None:
+    if sentry_sdk.get_client().get_integration(SqlalchemyIntegration) is None:
         return
 
     ctx_mgr = record_sql_queries(
-        hub,
         cursor,
         statement,
         parameters,
         paramstyle=context and context.dialect and context.dialect.paramstyle or None,
         executemany=executemany,
     )
     context._sentry_sql_span_manager = ctx_mgr
 
     span = ctx_mgr.__enter__()
 
     if span is not None:
         _set_db_data(span, conn)
-        if hub.client:
-            options = hub.client.options["_experiments"].get("attach_explain_plans")
-            if options is not None:
-                attach_explain_plan_to_span(
-                    span,
-                    conn,
-                    statement,
-                    parameters,
-                    options,
-                )
+        options = (
+            sentry_sdk.get_client().options["_experiments"].get("attach_explain_plans")
+        )
+        if options is not None:
+            attach_explain_plan_to_span(
+                span,
+                conn,
+                statement,
+                parameters,
+                options,
+            )
         context._sentry_sql_span = span
 
 
 def _after_cursor_execute(conn, cursor, statement, parameters, context, *args):
     # type: (Any, Any, Any, Any, Any, *Any) -> None
-    hub = Hub.current
-    if hub.get_integration(SqlalchemyIntegration) is None:
+    if sentry_sdk.get_client().get_integration(SqlalchemyIntegration) is None:
         return
 
     ctx_mgr = getattr(
         context, "_sentry_sql_span_manager", None
     )  # type: Optional[ContextManager[Any]]
 
     if ctx_mgr is not None:
         context._sentry_sql_span_manager = None
         ctx_mgr.__exit__(None, None, None)
 
     span = getattr(context, "_sentry_sql_span", None)  # type: Optional[Span]
     if span is not None:
         with capture_internal_exceptions():
-            add_query_source(hub, span)
+            add_query_source(span)
 
 
 def _handle_error(context, *args):
     # type: (Any, *Any) -> None
     execution_context = context.execution_context
     if execution_context is None:
         return
```

### Comparing `sentry-sdk-2.0.0rc2/sentry_sdk/integrations/starlette.py` & `sentry-sdk-2.0.0rc3/sentry_sdk/integrations/starlette.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc2/sentry_sdk/integrations/starlite.py` & `sentry-sdk-2.0.0rc3/sentry_sdk/integrations/starlite.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc2/sentry_sdk/integrations/stdlib.py` & `sentry-sdk-2.0.0rc3/sentry_sdk/integrations/stdlib.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import os
 import subprocess
 import sys
 import platform
 from http.client import HTTPConnection
 
+import sentry_sdk
 from sentry_sdk.consts import OP, SPANDATA
-from sentry_sdk.hub import Hub
 from sentry_sdk.integrations import Integration
-from sentry_sdk.scope import add_global_event_processor
+from sentry_sdk.scope import Scope, add_global_event_processor
 from sentry_sdk.tracing_utils import EnvironHeaders, should_propagate_trace
 from sentry_sdk.utils import (
     SENSITIVE_DATA_SUBSTITUTE,
     capture_internal_exceptions,
+    ensure_integration_enabled,
     is_sentry_url,
     logger,
     safe_repr,
     parse_url,
 )
 from sentry_sdk._types import TYPE_CHECKING
 
@@ -44,36 +45,37 @@
         # type: () -> None
         _install_httplib()
         _install_subprocess()
 
         @add_global_event_processor
         def add_python_runtime_context(event, hint):
             # type: (Event, Hint) -> Optional[Event]
-            if Hub.current.get_integration(StdlibIntegration) is not None:
+            if sentry_sdk.get_client().get_integration(StdlibIntegration) is not None:
                 contexts = event.setdefault("contexts", {})
                 if isinstance(contexts, dict) and "runtime" not in contexts:
                     contexts["runtime"] = _RUNTIME_CONTEXT
 
             return event
 
 
 def _install_httplib():
     # type: () -> None
     real_putrequest = HTTPConnection.putrequest
     real_getresponse = HTTPConnection.getresponse
 
     def putrequest(self, method, url, *args, **kwargs):
         # type: (HTTPConnection, str, str, *Any, **Any) -> Any
-        hub = Hub.current
-
         host = self.host
         port = self.port
         default_port = self.default_port
 
-        if hub.get_integration(StdlibIntegration) is None or is_sentry_url(hub, host):
+        client = sentry_sdk.get_client()
+        if client.get_integration(StdlibIntegration) is None or is_sentry_url(
+            client, host
+        ):
             return real_putrequest(self, method, url, *args, **kwargs)
 
         real_url = url
         if real_url is None or not real_url.startswith(("http://", "https://")):
             real_url = "%s://%s%s%s" % (
                 default_port == 443 and "https" or "http",
                 host,
@@ -81,30 +83,32 @@
                 url,
             )
 
         parsed_url = None
         with capture_internal_exceptions():
             parsed_url = parse_url(real_url, sanitize=False)
 
-        span = hub.start_span(
+        span = sentry_sdk.start_span(
             op=OP.HTTP_CLIENT,
             description="%s %s"
             % (method, parsed_url.url if parsed_url else SENSITIVE_DATA_SUBSTITUTE),
         )
 
         span.set_data(SPANDATA.HTTP_METHOD, method)
         if parsed_url is not None:
             span.set_data("url", parsed_url.url)
             span.set_data(SPANDATA.HTTP_QUERY, parsed_url.query)
             span.set_data(SPANDATA.HTTP_FRAGMENT, parsed_url.fragment)
 
         rv = real_putrequest(self, method, url, *args, **kwargs)
 
-        if should_propagate_trace(hub, real_url):
-            for key, value in hub.iter_trace_propagation_headers(span):
+        if should_propagate_trace(client, real_url):
+            for key, value in Scope.get_current_scope().iter_trace_propagation_headers(
+                span=span
+            ):
                 logger.debug(
                     "[Tracing] Adding `{key}` header {value} to outgoing request to {real_url}.".format(
                         key=key, value=value, real_url=real_url
                     )
                 )
                 self.putheader(key, value)
 
@@ -162,21 +166,17 @@
     return rv
 
 
 def _install_subprocess():
     # type: () -> None
     old_popen_init = subprocess.Popen.__init__
 
+    @ensure_integration_enabled(StdlibIntegration, old_popen_init)
     def sentry_patched_popen_init(self, *a, **kw):
         # type: (subprocess.Popen[Any], *Any, **Any) -> None
-
-        hub = Hub.current
-        if hub.get_integration(StdlibIntegration) is None:
-            return old_popen_init(self, *a, **kw)
-
         # Convert from tuple to list to be able to set values.
         a = list(a)
 
         args = _init_argument(a, kw, "args", 0) or []
         cwd = _init_argument(a, kw, "cwd", 9)
 
         # if args is not a list or tuple (and e.g. some iterator instead),
@@ -193,16 +193,18 @@
                 description = " ".join(map(str, args))
 
         if description is None:
             description = safe_repr(args)
 
         env = None
 
-        with hub.start_span(op=OP.SUBPROCESS, description=description) as span:
-            for k, v in hub.iter_trace_propagation_headers(span):
+        with sentry_sdk.start_span(op=OP.SUBPROCESS, description=description) as span:
+            for k, v in Scope.get_current_scope().iter_trace_propagation_headers(
+                span=span
+            ):
                 if env is None:
                     env = _init_argument(
                         a, kw, "env", 10, lambda x: dict(x or os.environ)
                     )
                 env["SUBPROCESS_" + k.upper().replace("-", "_")] = v
 
             if cwd:
@@ -213,37 +215,29 @@
             span.set_tag("subprocess.pid", self.pid)
             return rv
 
     subprocess.Popen.__init__ = sentry_patched_popen_init  # type: ignore
 
     old_popen_wait = subprocess.Popen.wait
 
+    @ensure_integration_enabled(StdlibIntegration, old_popen_wait)
     def sentry_patched_popen_wait(self, *a, **kw):
         # type: (subprocess.Popen[Any], *Any, **Any) -> Any
-        hub = Hub.current
-
-        if hub.get_integration(StdlibIntegration) is None:
-            return old_popen_wait(self, *a, **kw)
-
-        with hub.start_span(op=OP.SUBPROCESS_WAIT) as span:
+        with sentry_sdk.start_span(op=OP.SUBPROCESS_WAIT) as span:
             span.set_tag("subprocess.pid", self.pid)
             return old_popen_wait(self, *a, **kw)
 
     subprocess.Popen.wait = sentry_patched_popen_wait  # type: ignore
 
     old_popen_communicate = subprocess.Popen.communicate
 
+    @ensure_integration_enabled(StdlibIntegration, old_popen_communicate)
     def sentry_patched_popen_communicate(self, *a, **kw):
         # type: (subprocess.Popen[Any], *Any, **Any) -> Any
-        hub = Hub.current
-
-        if hub.get_integration(StdlibIntegration) is None:
-            return old_popen_communicate(self, *a, **kw)
-
-        with hub.start_span(op=OP.SUBPROCESS_COMMUNICATE) as span:
+        with sentry_sdk.start_span(op=OP.SUBPROCESS_COMMUNICATE) as span:
             span.set_tag("subprocess.pid", self.pid)
             return old_popen_communicate(self, *a, **kw)
 
     subprocess.Popen.communicate = sentry_patched_popen_communicate  # type: ignore
 
 
 def get_subprocess_traceparent_headers():
```

### Comparing `sentry-sdk-2.0.0rc2/sentry_sdk/integrations/strawberry.py` & `sentry-sdk-2.0.0rc3/sentry_sdk/integrations/strawberry.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc2/sentry_sdk/integrations/threading.py` & `sentry-sdk-2.0.0rc3/sentry_sdk/integrations/threading.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc2/sentry_sdk/integrations/tornado.py` & `sentry-sdk-2.0.0rc3/sentry_sdk/integrations/tornado.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc2/sentry_sdk/integrations/trytond.py` & `sentry-sdk-2.0.0rc3/sentry_sdk/integrations/trytond.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc2/sentry_sdk/integrations/wsgi.py` & `sentry-sdk-2.0.0rc3/sentry_sdk/integrations/wsgi.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc2/sentry_sdk/metrics.py` & `sentry-sdk-2.0.0rc3/sentry_sdk/metrics.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc2/sentry_sdk/monitor.py` & `sentry-sdk-2.0.0rc3/sentry_sdk/monitor.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc2/sentry_sdk/profiler.py` & `sentry-sdk-2.0.0rc3/sentry_sdk/profiler.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc2/sentry_sdk/scope.py` & `sentry-sdk-2.0.0rc3/sentry_sdk/scope.py`

 * *Files 1% similar despite different names*

```diff
@@ -708,21 +708,36 @@
 
         self._profile = None  # type: Optional[Profile]
 
         self._propagation_context = None
 
     @_attr_setter
     def level(self, value):
-        # type: (Optional[LogLevelStr]) -> None
-        """When set this overrides the level. Deprecated in favor of set_level."""
+        # type: (LogLevelStr) -> None
+        """
+        When set this overrides the level.
+
+        .. deprecated:: 1.0.0
+            Use :func:`set_level` instead.
+
+        :param value: The level to set.
+        """
+        logger.warning(
+            "Deprecated: use .set_level() instead. This will be removed in the future."
+        )
+
         self._level = value
 
     def set_level(self, value):
-        # type: (Optional[LogLevelStr]) -> None
-        """Sets the level for the scope."""
+        # type: (LogLevelStr) -> None
+        """
+        Sets the level for the scope.
+
+        :param value: The level to set.
+        """
         self._level = value
 
     @_attr_setter
     def fingerprint(self, value):
         # type: (Optional[List[str]]) -> None
         """When set this overrides the default fingerprint."""
         self._fingerprint = value
@@ -823,37 +838,43 @@
 
     @profile.setter
     def profile(self, profile):
         # type: (Optional[Profile]) -> None
 
         self._profile = profile
 
-    def set_tag(
-        self,
-        key,  # type: str
-        value,  # type: Any
-    ):
-        # type: (...) -> None
-        """Sets a tag for a key to a specific value."""
+    def set_tag(self, key, value):
+        # type: (str, Any) -> None
+        """
+        Sets a tag for a key to a specific value.
+
+        :param key: Key of the tag to set.
+
+        :param value: Value of the tag to set.
+        """
         self._tags[key] = value
 
-    def remove_tag(
-        self, key  # type: str
-    ):
-        # type: (...) -> None
-        """Removes a specific tag."""
+    def remove_tag(self, key):
+        # type: (str) -> None
+        """
+        Removes a specific tag.
+
+        :param key: Key of the tag to remove.
+        """
         self._tags.pop(key, None)
 
     def set_context(
         self,
         key,  # type: str
         value,  # type: Dict[str, Any]
     ):
         # type: (...) -> None
-        """Binds a context at a certain key to a specific value."""
+        """
+        Binds a context at a certain key to a specific value.
+        """
         self._contexts[key] = value
 
     def remove_context(
         self, key  # type: str
     ):
         # type: (...) -> None
         """Removes a context."""
@@ -1633,9 +1654,15 @@
 
     finally:
         # restore original scopes
         _current_scope.reset(current_token)
         _isolation_scope.reset(isolation_token)
 
 
+def should_send_default_pii():
+    # type: () -> bool
+    """Shortcut for `Scope.get_client().should_send_default_pii()`."""
+    return Scope.get_client().should_send_default_pii()
+
+
 # Circular imports
 from sentry_sdk.client import NonRecordingClient
```

### Comparing `sentry-sdk-2.0.0rc2/sentry_sdk/scrubber.py` & `sentry-sdk-2.0.0rc3/sentry_sdk/scrubber.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc2/sentry_sdk/serializer.py` & `sentry-sdk-2.0.0rc3/sentry_sdk/serializer.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc2/sentry_sdk/session.py` & `sentry-sdk-2.0.0rc3/sentry_sdk/session.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc2/sentry_sdk/sessions.py` & `sentry-sdk-2.0.0rc3/sentry_sdk/sessions.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc2/sentry_sdk/spotlight.py` & `sentry-sdk-2.0.0rc3/sentry_sdk/spotlight.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc2/sentry_sdk/tracing.py` & `sentry-sdk-2.0.0rc3/sentry_sdk/tracing.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc2/sentry_sdk/tracing_utils.py` & `sentry-sdk-2.0.0rc3/sentry_sdk/tracing_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -101,28 +101,25 @@
             or options.get("traces_sampler") is not None
         )
     )
 
 
 @contextlib.contextmanager
 def record_sql_queries(
-    hub,  # type: sentry_sdk.Hub
     cursor,  # type: Any
     query,  # type: Any
     params_list,  # type:  Any
     paramstyle,  # type: Optional[str]
     executemany,  # type: bool
     record_cursor_repr=False,  # type: bool
 ):
     # type: (...) -> Generator[sentry_sdk.tracing.Span, None, None]
 
     # TODO: Bring back capturing of params by default
-    if hub.client and hub.client.options["_experiments"].get(
-        "record_sql_params", False
-    ):
+    if sentry_sdk.get_client().options["_experiments"].get("record_sql_params", False):
         if not params_list or params_list == [None]:
             params_list = None
 
         if paramstyle == "pyformat":
             paramstyle = "format"
     else:
         params_list = None
@@ -137,17 +134,17 @@
         data["db.paramstyle"] = paramstyle
     if executemany:
         data["db.executemany"] = True
     if record_cursor_repr and cursor is not None:
         data["db.cursor"] = cursor
 
     with capture_internal_exceptions():
-        hub.add_breadcrumb(message=query, category="query", data=data)
+        sentry_sdk.add_breadcrumb(message=query, category="query", data=data)
 
-    with hub.start_span(op=OP.DB, description=query) as span:
+    with sentry_sdk.start_span(op=OP.DB, description=query) as span:
         for k, v in data.items():
             span.set_data(k, v)
         yield span
 
 
 def maybe_create_breadcrumbs_from_span(scope, span):
     # type: (sentry_sdk.Scope, sentry_sdk.tracing.Span) -> None
@@ -163,20 +160,20 @@
             type="subprocess",
             category="subprocess",
             message=span.description,
             data=span._data,
         )
 
 
-def add_query_source(hub, span):
-    # type: (sentry_sdk.Hub, sentry_sdk.tracing.Span) -> None
+def add_query_source(span):
+    # type: (sentry_sdk.tracing.Span) -> None
     """
     Adds OTel compatible source code information to the span
     """
-    client = sentry_sdk.Scope.get_client()
+    client = sentry_sdk.get_client()
     if not client.is_active():
         return
 
     if span.timestamp is None or span.start_timestamp is None:
         return
 
     should_add_query_source = client.options.get("enable_db_query_source", True)
@@ -471,23 +468,22 @@
 
         if include_third_party:
             items.append(self.third_party_items)
 
         return ",".join(items)
 
 
-def should_propagate_trace(hub, url):
-    # type: (sentry_sdk.Hub, str) -> bool
+def should_propagate_trace(client, url):
+    # type: (sentry_sdk.client.BaseClient, str) -> bool
     """
-    Returns True if url matches trace_propagation_targets configured in the given hub. Otherwise, returns False.
+    Returns True if url matches trace_propagation_targets configured in the given client. Otherwise, returns False.
     """
-    client = hub.client  # type: Any
     trace_propagation_targets = client.options["trace_propagation_targets"]
 
-    if is_sentry_url(hub, url):
+    if is_sentry_url(client, url):
         return False
 
     return match_regex_list(url, trace_propagation_targets, substring_matching=True)
 
 
 def normalize_incoming_data(incoming_data):
     # type: (Dict[str, Any]) -> Dict[str, Any]
```

### Comparing `sentry-sdk-2.0.0rc2/sentry_sdk/transport.py` & `sentry-sdk-2.0.0rc3/sentry_sdk/transport.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,44 +1,61 @@
 from abc import ABC, abstractmethod
 import io
-import warnings
-import urllib3
-import certifi
 import gzip
+import socket
 import time
+import warnings
 from datetime import datetime, timedelta, timezone
 from collections import defaultdict
 from urllib.request import getproxies
 
+import urllib3
+import certifi
+
 from sentry_sdk.consts import EndpointType
 from sentry_sdk.utils import Dsn, logger, capture_internal_exceptions
 from sentry_sdk.worker import BackgroundWorker
 from sentry_sdk.envelope import Envelope, Item, PayloadRef
-
 from sentry_sdk._types import TYPE_CHECKING
 
 if TYPE_CHECKING:
     from typing import Any
     from typing import Callable
     from typing import Dict
     from typing import Iterable
+    from typing import List
     from typing import Optional
     from typing import Tuple
     from typing import Type
     from typing import Union
     from typing import DefaultDict
 
     from urllib3.poolmanager import PoolManager
     from urllib3.poolmanager import ProxyManager
 
     from sentry_sdk._types import Event
 
     DataCategory = Optional[str]
 
 
+KEEP_ALIVE_SOCKET_OPTIONS = []
+for option in [
+    (socket.SOL_SOCKET, lambda: getattr(socket, "SO_KEEPALIVE"), 1),  # noqa: B009
+    (socket.SOL_TCP, lambda: getattr(socket, "TCP_KEEPIDLE"), 45),  # noqa: B009
+    (socket.SOL_TCP, lambda: getattr(socket, "TCP_KEEPINTVL"), 10),  # noqa: B009
+    (socket.SOL_TCP, lambda: getattr(socket, "TCP_KEEPCNT"), 6),  # noqa: B009
+]:
+    try:
+        KEEP_ALIVE_SOCKET_OPTIONS.append((option[0], option[1](), option[2]))
+    except AttributeError:
+        # a specific option might not be available on specific systems,
+        # e.g. TCP_KEEPIDLE doesn't exist on macOS
+        pass
+
+
 class Transport(ABC):
     """Baseclass for all transports.
 
     A transport is used to send an event to sentry.
     """
 
     parsed_dsn = None  # type: Optional[Dsn]
@@ -420,16 +437,30 @@
         # type: (Optional[Any]) -> Dict[str, Any]
         options = {
             "num_pools": self._num_pools,
             "cert_reqs": "CERT_REQUIRED",
             "ca_certs": ca_certs or certifi.where(),
         }
 
-        if self.options["socket_options"]:
-            options["socket_options"] = self.options["socket_options"]
+        socket_options = None  # type: Optional[List[Tuple[int, int, int | bytes]]]
+
+        if self.options["socket_options"] is not None:
+            socket_options = self.options["socket_options"]
+
+        if self.options["keep_alive"]:
+            if socket_options is None:
+                socket_options = []
+
+            used_options = {(o[0], o[1]) for o in socket_options}
+            for default_option in KEEP_ALIVE_SOCKET_OPTIONS:
+                if (default_option[0], default_option[1]) not in used_options:
+                    socket_options.append(default_option)
+
+        if socket_options is not None:
+            options["socket_options"] = socket_options
 
         return options
 
     def _in_no_proxy(self, parsed_dsn):
         # type: (Dsn) -> bool
         no_proxy = getproxies().get("no")
         if not no_proxy:
```

### Comparing `sentry-sdk-2.0.0rc2/sentry_sdk/utils.py` & `sentry-sdk-2.0.0rc3/sentry_sdk/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,49 +10,58 @@
 import sys
 import threading
 import time
 from collections import namedtuple
 from copy import copy
 from datetime import datetime
 from decimal import Decimal
-from functools import partial, partialmethod
+from functools import partial, partialmethod, wraps
 from numbers import Real
 from urllib.parse import parse_qs, unquote, urlencode, urlsplit, urlunsplit
 
 try:
     # Python 3.11
     from builtins import BaseExceptionGroup
 except ImportError:
     # Python 3.10 and below
     BaseExceptionGroup = None  # type: ignore
 
 import sentry_sdk
+import sentry_sdk.hub
 from sentry_sdk._compat import PY37
 from sentry_sdk._types import TYPE_CHECKING
 from sentry_sdk.consts import DEFAULT_MAX_VALUE_LENGTH, EndpointType
 
 if TYPE_CHECKING:
+    from collections.abc import Awaitable
+
     from types import FrameType, TracebackType
     from typing import (
         Any,
         Callable,
         ContextManager,
         Dict,
         Iterator,
         List,
         NoReturn,
         Optional,
+        ParamSpec,
         Set,
         Tuple,
         Type,
+        TypeVar,
         Union,
     )
 
+    import sentry_sdk.integrations
     from sentry_sdk._types import Event, ExcInfo
 
+    P = ParamSpec("P")
+    R = TypeVar("R")
+
 
 epoch = datetime(1970, 1, 1)
 
 # The logger is created here but initialized in the debug support module
 logger = logging.getLogger("sentry_sdk.errors")
 
 _installed_modules = None
@@ -1545,24 +1554,24 @@
         matched = re.search(item_matcher, item)
         if matched:
             return True
 
     return False
 
 
-def is_sentry_url(hub, url):
-    # type: (sentry_sdk.Hub, str) -> bool
+def is_sentry_url(client, url):
+    # type: (sentry_sdk.client.BaseClient, str) -> bool
     """
     Determines whether the given URL matches the Sentry DSN.
     """
     return (
-        hub.client is not None
-        and hub.client.transport is not None
-        and hub.client.transport.parsed_dsn is not None
-        and hub.client.transport.parsed_dsn.netloc in url
+        client is not None
+        and client.transport is not None
+        and client.transport.parsed_dsn is not None
+        and client.transport.parsed_dsn.netloc in url
     )
 
 
 def _generate_installed_modules():
     # type: () -> Iterator[Tuple[str, str]]
     try:
         from importlib import metadata
@@ -1618,14 +1627,82 @@
     # type: (Optional[Type[BaseException]], Optional[BaseException], Optional[Any]) -> NoReturn
     assert value is not None
     if value.__traceback__ is not tb:
         raise value.with_traceback(tb)
     raise value
 
 
+def ensure_integration_enabled(
+    integration,  # type: type[sentry_sdk.integrations.Integration]
+    original_function,  # type: Callable[P, R]
+):
+    # type: (...) -> Callable[[Callable[P, R]], Callable[P, R]]
+    """
+    Ensures a given integration is enabled prior to calling a Sentry-patched function.
+
+    The function takes as its parameters the integration that must be enabled and the original
+    function that the SDK is patching. The function returns a function that takes the
+    decorated (Sentry-patched) function as its parameter, and returns a function that, when
+    called, checks whether the given integration is enabled. If the integration is enabled, the
+    function calls the decorated, Sentry-patched function. If the integration is not enabled,
+    the original function is called.
+
+    The function also takes care of preserving the original function's signature and docstring.
+
+    Example usage:
+
+    ```python
+    @ensure_integration_enabled(MyIntegration, my_function)
+    def patch_my_function():
+        with sentry_sdk.start_transaction(...):
+            return my_function()
+    ```
+    """
+
+    def patcher(sentry_patched_function):
+        # type: (Callable[P, R]) -> Callable[P, R]
+        @wraps(original_function)
+        def runner(*args: "P.args", **kwargs: "P.kwargs"):
+            # type: (...) -> R
+            if sentry_sdk.get_client().get_integration(integration) is None:
+                return original_function(*args, **kwargs)
+
+            return sentry_patched_function(*args, **kwargs)
+
+        return runner
+
+    return patcher
+
+
+def ensure_integration_enabled_async(
+    integration,  # type: type[sentry_sdk.integrations.Integration]
+    original_function,  # type: Callable[P, Awaitable[R]]
+):
+    # type: (...) -> Callable[[Callable[P, Awaitable[R]]], Callable[P, Awaitable[R]]]
+    """
+    Version of `ensure_integration_enabled` for decorating async functions.
+
+    Please refer to the `ensure_integration_enabled` documentation for more information.
+    """
+
+    def patcher(sentry_patched_function):
+        # type: (Callable[P, Awaitable[R]]) -> Callable[P, Awaitable[R]]
+        @wraps(original_function)
+        async def runner(*args: "P.args", **kwargs: "P.kwargs"):
+            # type: (...) -> R
+            if sentry_sdk.get_client().get_integration(integration) is None:
+                return await original_function(*args, **kwargs)
+
+            return await sentry_patched_function(*args, **kwargs)
+
+        return runner
+
+    return patcher
+
+
 if PY37:
 
     def nanosecond_time():
         # type: () -> int
         return time.perf_counter_ns()
 
 else:
```

### Comparing `sentry-sdk-2.0.0rc2/sentry_sdk/worker.py` & `sentry-sdk-2.0.0rc3/sentry_sdk/worker.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc2/sentry_sdk.egg-info/PKG-INFO` & `sentry-sdk-2.0.0rc3/sentry_sdk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sentry-sdk
-Version: 2.0.0rc2
+Version: 2.0.0rc3
 Summary: Python client for Sentry (https://sentry.io)
 Home-page: https://github.com/getsentry/sentry-python
 Author: Sentry Team and Contributors
 Author-email: hello@sentry.io
 License: MIT
 Project-URL: Documentation, https://docs.sentry.io/platforms/python/
 Project-URL: Changelog, https://github.com/getsentry/sentry-python/blob/master/CHANGELOG.md
@@ -36,14 +36,16 @@
 Requires-Dist: asyncpg>=0.23; extra == "asyncpg"
 Provides-Extra: beam
 Requires-Dist: apache-beam>=2.12; extra == "beam"
 Provides-Extra: bottle
 Requires-Dist: bottle>=0.12.13; extra == "bottle"
 Provides-Extra: celery
 Requires-Dist: celery>=3; extra == "celery"
+Provides-Extra: celery-redbeat
+Requires-Dist: celery-redbeat>=2; extra == "celery-redbeat"
 Provides-Extra: chalice
 Requires-Dist: chalice>=1.16.0; extra == "chalice"
 Provides-Extra: clickhouse-driver
 Requires-Dist: clickhouse-driver>=0.2.0; extra == "clickhouse-driver"
 Provides-Extra: django
 Requires-Dist: django>=1.8; extra == "django"
 Provides-Extra: falcon
```

### Comparing `sentry-sdk-2.0.0rc2/sentry_sdk.egg-info/SOURCES.txt` & `sentry-sdk-2.0.0rc3/sentry_sdk.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 sentry_sdk/serializer.py
 sentry_sdk/session.py
 sentry_sdk/sessions.py
 sentry_sdk/spotlight.py
 sentry_sdk/tracing.py
 sentry_sdk/tracing_utils.py
 sentry_sdk/transport.py
+sentry_sdk/types.py
 sentry_sdk/utils.py
 sentry_sdk/worker.py
 sentry_sdk.egg-info/PKG-INFO
 sentry_sdk.egg-info/SOURCES.txt
 sentry_sdk.egg-info/dependency_links.txt
 sentry_sdk.egg-info/not-zip-safe
 sentry_sdk.egg-info/requires.txt
```

### Comparing `sentry-sdk-2.0.0rc2/sentry_sdk.egg-info/requires.txt` & `sentry-sdk-2.0.0rc3/sentry_sdk.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,17 @@
 
 [bottle]
 bottle>=0.12.13
 
 [celery]
 celery>=3
 
+[celery-redbeat]
+celery-redbeat>=2
+
 [chalice]
 chalice>=1.16.0
 
 [clickhouse-driver]
 clickhouse-driver>=0.2.0
 
 [django]
```

### Comparing `sentry-sdk-2.0.0rc2/setup.py` & `sentry-sdk-2.0.0rc3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 def get_file_text(file_name):
     with open(os.path.join(here, file_name)) as in_file:
         return in_file.read()
 
 
 setup(
     name="sentry-sdk",
-    version="2.0.0rc2",
+    version="2.0.0rc3",
     author="Sentry Team and Contributors",
     author_email="hello@sentry.io",
     url="https://github.com/getsentry/sentry-python",
     project_urls={
         "Documentation": "https://docs.sentry.io/platforms/python/",
         "Changelog": "https://github.com/getsentry/sentry-python/blob/master/CHANGELOG.md",
     },
@@ -45,14 +45,15 @@
     extras_require={
         "aiohttp": ["aiohttp>=3.5"],
         "arq": ["arq>=0.23"],
         "asyncpg": ["asyncpg>=0.23"],
         "beam": ["apache-beam>=2.12"],
         "bottle": ["bottle>=0.12.13"],
         "celery": ["celery>=3"],
+        "celery-redbeat": ["celery-redbeat>=2"],
         "chalice": ["chalice>=1.16.0"],
         "clickhouse-driver": ["clickhouse-driver>=0.2.0"],
         "django": ["django>=1.8"],
         "falcon": ["falcon>=1.4"],
         "fastapi": ["fastapi>=0.79.0"],
         "flask": ["flask>=0.11", "blinker>=1.1", "markupsafe"],
         "grpcio": ["grpcio>=1.21.1"],
```

### Comparing `sentry-sdk-2.0.0rc2/tests/test_api.py` & `sentry-sdk-2.0.0rc3/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc2/tests/test_basics.py` & `sentry-sdk-2.0.0rc3/tests/test_basics.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc2/tests/test_client.py` & `sentry-sdk-2.0.0rc3/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc2/tests/test_conftest.py` & `sentry-sdk-2.0.0rc3/tests/test_conftest.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc2/tests/test_crons.py` & `sentry-sdk-2.0.0rc3/tests/test_crons.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc2/tests/test_envelope.py` & `sentry-sdk-2.0.0rc3/tests/test_envelope.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc2/tests/test_exceptiongroup.py` & `sentry-sdk-2.0.0rc3/tests/test_exceptiongroup.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc2/tests/test_lru_cache.py` & `sentry-sdk-2.0.0rc3/tests/test_lru_cache.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc2/tests/test_metrics.py` & `sentry-sdk-2.0.0rc3/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc2/tests/test_monitor.py` & `sentry-sdk-2.0.0rc3/tests/test_monitor.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc2/tests/test_new_scopes_compat.py` & `sentry-sdk-2.0.0rc3/tests/test_new_scopes_compat.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc2/tests/test_new_scopes_compat_event.py` & `sentry-sdk-2.0.0rc3/tests/test_new_scopes_compat_event.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc2/tests/test_profiler.py` & `sentry-sdk-2.0.0rc3/tests/test_profiler.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc2/tests/test_scope.py` & `sentry-sdk-2.0.0rc3/tests/test_scope.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,21 @@
 import sentry_sdk
 from sentry_sdk import (
     capture_exception,
     isolation_scope,
     new_scope,
 )
 from sentry_sdk.client import Client, NonRecordingClient
-from sentry_sdk.scope import Scope, ScopeType, use_isolation_scope, use_scope
+from sentry_sdk.scope import (
+    Scope,
+    ScopeType,
+    use_isolation_scope,
+    use_scope,
+    should_send_default_pii,
+)
 
 
 def test_copying():
     s1 = Scope()
     s1.fingerprint = {}
     s1.set_tag("foo", "bar")
 
@@ -774,7 +780,19 @@
 
     (envelope,) = envelopes
     transaction = envelope.items[0].get_transaction_event()
 
     assert transaction["tags"] == {"isolation_scope1": 1, "current_scope2": 1, "trx": 1}
     assert transaction["spans"][0]["tags"] == {"a": 1}
     assert transaction["spans"][1]["tags"] == {"b": 1}
+
+
+def test_should_send_default_pii_true(sentry_init):
+    sentry_init(send_default_pii=True)
+
+    assert should_send_default_pii() is True
+
+
+def test_should_send_default_pii_false(sentry_init):
+    sentry_init(send_default_pii=False)
+
+    assert should_send_default_pii() is False
```

### Comparing `sentry-sdk-2.0.0rc2/tests/test_scrubber.py` & `sentry-sdk-2.0.0rc3/tests/test_scrubber.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc2/tests/test_serializer.py` & `sentry-sdk-2.0.0rc3/tests/test_serializer.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc2/tests/test_sessions.py` & `sentry-sdk-2.0.0rc3/tests/test_sessions.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc2/tests/test_spotlight.py` & `sentry-sdk-2.0.0rc3/tests/test_spotlight.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc2/tests/test_utils.py` & `sentry-sdk-2.0.0rc3/tests/test_utils.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import re
 import sys
 from unittest import mock
 
 import pytest
 
 import sentry_sdk
+from sentry_sdk.integrations import Integration
 from sentry_sdk.utils import (
     Components,
     Dsn,
     get_default_release,
     get_error_message,
     get_git_revision,
     is_valid_sample_rate,
@@ -17,17 +18,29 @@
     parse_url,
     parse_version,
     safe_str,
     sanitize_url,
     serialize_frame,
     is_sentry_url,
     _get_installed_modules,
+    ensure_integration_enabled,
+    ensure_integration_enabled_async,
 )
 
 
+class TestIntegration(Integration):
+    """
+    Test integration for testing ensure_integration_enabled and
+    ensure_integration_enabled_async decorators.
+    """
+
+    identifier = "test"
+    setup_once = mock.MagicMock()
+
+
 def _normalize_distribution_name(name):
     # type: (str) -> str
     """Normalize distribution name according to PEP-0503.
 
     See:
     https://peps.python.org/pep-0503/#normalized-names
     for more details.
@@ -424,49 +437,46 @@
     ],
 )
 def test_parse_version(version, expected_result):
     assert parse_version(version) == expected_result
 
 
 @pytest.fixture
-def mock_hub_with_dsn_netloc():
+def mock_client_with_dsn_netloc():
     """
     Returns a mocked hub with a DSN netloc of "abcd1234.ingest.sentry.io".
     """
+    mock_client = mock.Mock(spec=sentry_sdk.Client)
+    mock_client.transport = mock.Mock(spec=sentry_sdk.Transport)
+    mock_client.transport.parsed_dsn = mock.Mock(spec=Dsn)
 
-    mock_hub = mock.Mock(spec=sentry_sdk.Hub)
-    mock_hub.client = mock.Mock(spec=sentry_sdk.Client)
-    mock_hub.client.transport = mock.Mock(spec=sentry_sdk.Transport)
-    mock_hub.client.transport.parsed_dsn = mock.Mock(spec=Dsn)
-
-    mock_hub.client.transport.parsed_dsn.netloc = "abcd1234.ingest.sentry.io"
+    mock_client.transport.parsed_dsn.netloc = "abcd1234.ingest.sentry.io"
 
-    return mock_hub
+    return mock_client
 
 
 @pytest.mark.parametrize(
     ["test_url", "is_sentry_url_expected"],
     [
         ["https://asdf@abcd1234.ingest.sentry.io/123456789", True],
         ["https://asdf@abcd1234.ingest.notsentry.io/123456789", False],
     ],
 )
-def test_is_sentry_url_true(test_url, is_sentry_url_expected, mock_hub_with_dsn_netloc):
-    ret_val = is_sentry_url(mock_hub_with_dsn_netloc, test_url)
+def test_is_sentry_url_true(
+    test_url, is_sentry_url_expected, mock_client_with_dsn_netloc
+):
+    ret_val = is_sentry_url(mock_client_with_dsn_netloc, test_url)
 
     assert ret_val == is_sentry_url_expected
 
 
 def test_is_sentry_url_no_client():
-    hub = mock.Mock()
-    hub.client = None
-
     test_url = "https://asdf@abcd1234.ingest.sentry.io/123456789"
 
-    ret_val = is_sentry_url(hub, test_url)
+    ret_val = is_sentry_url(None, test_url)
 
     assert not ret_val
 
 
 @pytest.mark.parametrize(
     "error,expected_result",
     [
@@ -563,7 +573,79 @@
 
 
 def test_default_release_empty_string():
     with mock.patch("sentry_sdk.utils.get_git_revision", return_value=""):
         release = get_default_release()
 
     assert release is None
+
+
+def test_ensure_integration_enabled_integration_enabled(sentry_init):
+    def original_function():
+        return "original"
+
+    def function_to_patch():
+        return "patched"
+
+    sentry_init(integrations=[TestIntegration()])
+
+    # Test the decorator by applying to function_to_patch
+    patched_function = ensure_integration_enabled(TestIntegration, original_function)(
+        function_to_patch
+    )
+
+    assert patched_function() == "patched"
+
+
+def test_ensure_integration_enabled_integration_disabled(sentry_init):
+    def original_function():
+        return "original"
+
+    def function_to_patch():
+        return "patched"
+
+    sentry_init(integrations=[])  # TestIntegration is disabled
+
+    # Test the decorator by applying to function_to_patch
+    patched_function = ensure_integration_enabled(TestIntegration, original_function)(
+        function_to_patch
+    )
+
+    assert patched_function() == "original"
+
+
+@pytest.mark.asyncio
+async def test_ensure_integration_enabled_async_integration_enabled(sentry_init):
+    # Setup variables and functions for the test
+    async def original_function():
+        return "original"
+
+    async def function_to_patch():
+        return "patched"
+
+    sentry_init(integrations=[TestIntegration()])
+
+    # Test the decorator by applying to function_to_patch
+    patched_function = ensure_integration_enabled_async(
+        TestIntegration, original_function
+    )(function_to_patch)
+
+    assert await patched_function() == "patched"
+
+
+@pytest.mark.asyncio
+async def test_ensure_integration_enabled_async_integration_disabled(sentry_init):
+    # Setup variables and functions for the test
+    async def original_function():
+        return "original"
+
+    async def function_to_patch():
+        return "patched"
+
+    sentry_init(integrations=[])  # TestIntegration is disabled
+
+    # Test the decorator by applying to function_to_patch
+    patched_function = ensure_integration_enabled_async(
+        TestIntegration, original_function
+    )(function_to_patch)
+
+    assert await patched_function() == "original"
```


# Comparing `tmp/sentry-sdk-2.0.0rc3.tar.gz` & `tmp/sentry-sdk-2.0.0rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sentry-sdk-2.0.0rc3.tar", last modified: Wed Mar 20 14:56:01 2024, max compression
+gzip compressed data, was "sentry-sdk-2.0.0rc4.tar", last modified: Wed Apr  3 08:02:44 2024, max compression
```

## Comparing `sentry-sdk-2.0.0rc3.tar` & `sentry-sdk-2.0.0rc4.tar`

### file list

```diff
@@ -1,160 +1,164 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 14:56:01.517714 sentry-sdk-2.0.0rc3/
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    10503 2024-03-20 14:56:01.517714 sentry-sdk-2.0.0rc3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5960 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 14:56:01.493714 sentry-sdk-2.0.0rc3/sentry_sdk/
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3066 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/_compat.py
--rw-r--r--   0 runner    (1001) docker     (127)     5382 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/_lru_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)    11259 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/_queue.py
--rw-r--r--   0 runner    (1001) docker     (127)     5604 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     3745 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/_werkzeug.py
--rw-r--r--   0 runner    (1001) docker     (127)     8071 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/attachments.py
--rw-r--r--   0 runner    (1001) docker     (127)    29194 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    11464 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/consts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 14:56:01.497714 sentry-sdk-2.0.0rc3/sentry_sdk/crons/
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/crons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/crons/api.py
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/crons/consts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/crons/decorator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 14:56:01.497714 sentry-sdk-2.0.0rc3/sentry_sdk/db/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/db/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 14:56:01.497714 sentry-sdk-2.0.0rc3/sentry_sdk/db/explain_plan/
--rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/db/explain_plan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/db/explain_plan/django.py
--rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/db/explain_plan/sqlalchemy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/debug.py
--rw-r--r--   0 runner    (1001) docker     (127)     9916 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/envelope.py
--rw-r--r--   0 runner    (1001) docker     (127)    26979 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/hub.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 14:56:01.505714 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/
--rw-r--r--   0 runner    (1001) docker     (127)     7541 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3197 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/_asgi_common.py
--rw-r--r--   0 runner    (1001) docker     (127)     5634 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/_wsgi_common.py
--rw-r--r--   0 runner    (1001) docker     (127)    11502 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (127)      922 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/argv.py
--rw-r--r--   0 runner    (1001) docker     (127)     5939 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/ariadne.py
--rw-r--r--   0 runner    (1001) docker     (127)     7150 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/arq.py
--rw-r--r--   0 runner    (1001) docker     (127)    11861 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/asgi.py
--rw-r--r--   0 runner    (1001) docker     (127)     3132 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/asyncio.py
--rw-r--r--   0 runner    (1001) docker     (127)     6072 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/asyncpg.py
--rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/atexit.py
--rw-r--r--   0 runner    (1001) docker     (127)    15845 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/aws_lambda.py
--rw-r--r--   0 runner    (1001) docker     (127)     5619 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/beam.py
--rw-r--r--   0 runner    (1001) docker     (127)     4491 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/boto3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6413 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/bottle.py
--rw-r--r--   0 runner    (1001) docker     (127)    21673 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/celery.py
--rw-r--r--   0 runner    (1001) docker     (127)     4742 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/chalice.py
--rw-r--r--   0 runner    (1001) docker     (127)     5109 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/clickhouse_driver.py
--rw-r--r--   0 runner    (1001) docker     (127)     6755 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/cloud_resource_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/dedupe.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 14:56:01.505714 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/django/
--rw-r--r--   0 runner    (1001) docker     (127)    23338 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/django/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6820 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/django/asgi.py
--rw-r--r--   0 runner    (1001) docker     (127)     3622 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/django/caching.py
--rw-r--r--   0 runner    (1001) docker     (127)     5770 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/django/middleware.py
--rw-r--r--   0 runner    (1001) docker     (127)     2970 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/django/signals_handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5736 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/django/templates.py
--rw-r--r--   0 runner    (1001) docker     (127)     4957 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/django/transactions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2836 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/django/views.py
--rw-r--r--   0 runner    (1001) docker     (127)     2151 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/excepthook.py
--rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/executing.py
--rw-r--r--   0 runner    (1001) docker     (127)     9448 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/falcon.py
--rw-r--r--   0 runner    (1001) docker     (127)     4543 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/fastapi.py
--rw-r--r--   0 runner    (1001) docker     (127)     7788 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/flask.py
--rw-r--r--   0 runner    (1001) docker     (127)     8210 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/gcp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2906 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/gnu_backtrace.py
--rw-r--r--   0 runner    (1001) docker     (127)     4386 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/gql.py
--rw-r--r--   0 runner    (1001) docker     (127)     3746 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/graphene.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 14:56:01.505714 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/grpc/
--rw-r--r--   0 runner    (1001) docker     (127)     4979 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/grpc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 14:56:01.509714 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/grpc/aio/
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/grpc/aio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/grpc/aio/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3878 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/grpc/aio/server.py
--rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/grpc/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/grpc/server.py
--rw-r--r--   0 runner    (1001) docker     (127)     5165 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/httpx.py
--rw-r--r--   0 runner    (1001) docker     (127)     5452 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/huey.py
--rw-r--r--   0 runner    (1001) docker     (127)     9592 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     3011 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/loguru.py
--rw-r--r--   0 runner    (1001) docker     (127)      831 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/modules.py
--rw-r--r--   0 runner    (1001) docker     (127)    11005 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/openai.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 14:56:01.509714 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/opentelemetry/
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/opentelemetry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/opentelemetry/consts.py
--rw-r--r--   0 runner    (1001) docker     (127)     5830 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/opentelemetry/integration.py
--rw-r--r--   0 runner    (1001) docker     (127)     3731 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/opentelemetry/propagator.py
--rw-r--r--   0 runner    (1001) docker     (127)    12375 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/opentelemetry/span_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4514 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/pure_eval.py
--rw-r--r--   0 runner    (1001) docker     (127)     5968 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/pymongo.py
--rw-r--r--   0 runner    (1001) docker     (127)     7371 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/pyramid.py
--rw-r--r--   0 runner    (1001) docker     (127)     7425 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/quart.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 14:56:01.509714 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/redis/
--rw-r--r--   0 runner    (1001) docker     (127)    11834 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/redis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/redis/asyncio.py
--rw-r--r--   0 runner    (1001) docker     (127)     5634 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/rq.py
--rw-r--r--   0 runner    (1001) docker     (127)    13269 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/sanic.py
--rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/serverless.py
--rw-r--r--   0 runner    (1001) docker     (127)     2905 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/socket.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 14:56:01.509714 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/spark/
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/spark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8475 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/spark/spark_driver.py
--rw-r--r--   0 runner    (1001) docker     (127)     3973 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/spark/spark_worker.py
--rw-r--r--   0 runner    (1001) docker     (127)     4908 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/sqlalchemy.py
--rw-r--r--   0 runner    (1001) docker     (127)    24176 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/starlette.py
--rw-r--r--   0 runner    (1001) docker     (127)    10215 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/starlite.py
--rw-r--r--   0 runner    (1001) docker     (127)     8346 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/stdlib.py
--rw-r--r--   0 runner    (1001) docker     (127)    14881 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/strawberry.py
--rw-r--r--   0 runner    (1001) docker     (127)     4048 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/threading.py
--rw-r--r--   0 runner    (1001) docker     (127)     7287 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/tornado.py
--rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/trytond.py
--rw-r--r--   0 runner    (1001) docker     (127)     9870 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/integrations/wsgi.py
--rw-r--r--   0 runner    (1001) docker     (127)    29397 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     3720 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)    35123 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/profiler.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    57353 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/scope.py
--rw-r--r--   0 runner    (1001) docker     (127)     5082 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/scrubber.py
--rw-r--r--   0 runner    (1001) docker     (127)    12729 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/serializer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5581 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/session.py
--rw-r--r--   0 runner    (1001) docker     (127)     7822 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/sessions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/spotlight.py
--rw-r--r--   0 runner    (1001) docker     (127)    35876 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/tracing.py
--rw-r--r--   0 runner    (1001) docker     (127)    17304 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/tracing_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    20392 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/transport.py
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/types.py
--rw-r--r--   0 runner    (1001) docker     (127)    52142 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4475 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/sentry_sdk/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 14:56:01.513714 sentry-sdk-2.0.0rc3/sentry_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10503 2024-03-20 14:56:01.000000 sentry-sdk-2.0.0rc3/sentry_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4538 2024-03-20 14:56:01.000000 sentry-sdk-2.0.0rc3/sentry_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-20 14:56:01.000000 sentry-sdk-2.0.0rc3/sentry_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-20 14:56:01.000000 sentry-sdk-2.0.0rc3/sentry_sdk.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-03-20 14:56:01.000000 sentry-sdk-2.0.0rc3/sentry_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-20 14:56:01.000000 sentry-sdk-2.0.0rc3/sentry_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-20 14:56:01.517714 sentry-sdk-2.0.0rc3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3836 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 14:56:01.513714 sentry-sdk-2.0.0rc3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4000 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    23265 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/tests/test_basics.py
--rw-r--r--   0 runner    (1001) docker     (127)    36053 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3409 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/tests/test_conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     8036 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/tests/test_crons.py
--rw-r--r--   0 runner    (1001) docker     (127)     8057 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/tests/test_envelope.py
--rw-r--r--   0 runner    (1001) docker     (127)     8578 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/tests/test_exceptiongroup.py
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/tests/test_lru_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)    31256 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/tests/test_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     2563 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/tests/test_monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     8686 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/tests/test_new_scopes_compat.py
--rw-r--r--   0 runner    (1001) docker     (127)    17155 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/tests/test_new_scopes_compat_event.py
--rw-r--r--   0 runner    (1001) docker     (127)    25221 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/tests/test_profiler.py
--rw-r--r--   0 runner    (1001) docker     (127)    25744 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/tests/test_scope.py
--rw-r--r--   0 runner    (1001) docker     (127)     5293 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/tests/test_scrubber.py
--rw-r--r--   0 runner    (1001) docker     (127)     4578 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/tests/test_serializer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4098 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/tests/test_sessions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/tests/test_spotlight.py
--rw-r--r--   0 runner    (1001) docker     (127)    15025 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/tests/test_transport.py
--rw-r--r--   0 runner    (1001) docker     (127)    19715 2024-03-20 14:55:49.000000 sentry-sdk-2.0.0rc3/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:02:44.958354 sentry-sdk-2.0.0rc4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    10503 2024-04-03 08:02:44.958354 sentry-sdk-2.0.0rc4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5960 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:02:44.938353 sentry-sdk-2.0.0rc4/sentry_sdk/
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3066 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5382 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/_lru_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11259 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/_queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5604 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3745 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/_werkzeug.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9593 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/attachments.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29194 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11782 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/consts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:02:44.938353 sentry-sdk-2.0.0rc4/sentry_sdk/crons/
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/crons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/crons/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/crons/consts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2841 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/crons/decorator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:02:44.938353 sentry-sdk-2.0.0rc4/sentry_sdk/db/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/db/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:02:44.938353 sentry-sdk-2.0.0rc4/sentry_sdk/db/explain_plan/
+-rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/db/explain_plan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/db/explain_plan/django.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/db/explain_plan/sqlalchemy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/debug.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9916 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/envelope.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27085 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/hub.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:02:44.946354 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     7541 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3197 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/_asgi_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5636 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/_wsgi_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11478 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/argv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5939 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/ariadne.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6919 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/arq.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11600 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/asgi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3091 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6027 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/asyncpg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/atexit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15627 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/aws_lambda.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5192 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/beam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4475 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/boto3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5800 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/bottle.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:02:44.946354 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/celery/
+-rw-r--r--   0 runner    (1001) docker     (127)    13809 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/celery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9721 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/celery/beat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/celery/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4721 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/chalice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5064 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/clickhouse_driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6755 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/cloud_resource_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/dedupe.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:02:44.950353 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/django/
+-rw-r--r--   0 runner    (1001) docker     (127)    23345 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/django/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6820 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/django/asgi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3622 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/django/caching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5770 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/django/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2970 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/django/signals_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5683 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/django/templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4957 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/django/transactions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2836 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/django/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/excepthook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/executing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9347 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/falcon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4543 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/fastapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7706 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/flask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8149 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/gcp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2906 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/gnu_backtrace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4386 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/gql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3594 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/graphene.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:02:44.950353 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/grpc/
+-rw-r--r--   0 runner    (1001) docker     (127)     4979 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/grpc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:02:44.950353 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/grpc/aio/
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/grpc/aio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3075 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/grpc/aio/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3866 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/grpc/aio/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3249 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/grpc/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2389 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/grpc/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5165 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/httpx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5260 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/huey.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9592 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3011 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/loguru.py
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/modules.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11005 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/openai.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:02:44.950353 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/opentelemetry/
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/opentelemetry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/opentelemetry/consts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5830 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/opentelemetry/integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3731 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/opentelemetry/propagator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12225 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/opentelemetry/span_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4539 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/pure_eval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5994 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/pymongo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7151 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/pyramid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7091 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/quart.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:02:44.950353 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/redis/
+-rw-r--r--   0 runner    (1001) docker     (127)    11834 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/redis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/redis/asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5297 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/rq.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13017 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/sanic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/serverless.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2906 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/socket.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:02:44.950353 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/spark/
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/spark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8276 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/spark/spark_driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3747 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/spark/spark_worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4865 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/sqlalchemy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23504 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/starlette.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9835 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/starlite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8346 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/stdlib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14478 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/strawberry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4033 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/threading.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7185 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/tornado.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/trytond.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9870 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/integrations/wsgi.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29397 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3720 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33304 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    57649 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5082 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/scrubber.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12729 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5581 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7822 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/sessions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/spotlight.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38456 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/tracing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17304 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/tracing_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20392 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/transport.py
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56248 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4475 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/sentry_sdk/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:02:44.954354 sentry-sdk-2.0.0rc4/sentry_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10503 2024-04-03 08:02:44.000000 sentry-sdk-2.0.0rc4/sentry_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-04-03 08:02:44.000000 sentry-sdk-2.0.0rc4/sentry_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 08:02:44.000000 sentry-sdk-2.0.0rc4/sentry_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 08:02:44.000000 sentry-sdk-2.0.0rc4/sentry_sdk.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-04-03 08:02:44.000000 sentry-sdk-2.0.0rc4/sentry_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-03 08:02:44.000000 sentry-sdk-2.0.0rc4/sentry_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 08:02:44.958354 sentry-sdk-2.0.0rc4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3836 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:02:44.954354 sentry-sdk-2.0.0rc4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4000 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23265 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/tests/test_basics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36053 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3409 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/tests/test_conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13795 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/tests/test_crons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8057 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/tests/test_envelope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8578 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/tests/test_exceptiongroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/tests/test_lru_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31256 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/tests/test_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2563 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/tests/test_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8686 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/tests/test_new_scopes_compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17288 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/tests/test_new_scopes_compat_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23653 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/tests/test_profiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25744 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/tests/test_scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5357 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/tests/test_scrubber.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4578 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/tests/test_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4098 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/tests/test_sessions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/tests/test_spotlight.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15025 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/tests/test_transport.py
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/tests/test_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26384 2024-04-03 08:02:36.000000 sentry-sdk-2.0.0rc4/tests/test_utils.py
```

### Comparing `sentry-sdk-2.0.0rc3/LICENSE` & `sentry-sdk-2.0.0rc4/LICENSE`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc3/PKG-INFO` & `sentry-sdk-2.0.0rc4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sentry-sdk
-Version: 2.0.0rc3
+Version: 2.0.0rc4
 Summary: Python client for Sentry (https://sentry.io)
 Home-page: https://github.com/getsentry/sentry-python
 Author: Sentry Team and Contributors
 Author-email: hello@sentry.io
 License: MIT
 Project-URL: Documentation, https://docs.sentry.io/platforms/python/
 Project-URL: Changelog, https://github.com/getsentry/sentry-python/blob/master/CHANGELOG.md
```

### Comparing `sentry-sdk-2.0.0rc3/README.md` & `sentry-sdk-2.0.0rc4/README.md`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc3/sentry_sdk/__init__.py` & `sentry-sdk-2.0.0rc4/sentry_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc3/sentry_sdk/_compat.py` & `sentry-sdk-2.0.0rc4/sentry_sdk/_compat.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc3/sentry_sdk/_lru_cache.py` & `sentry-sdk-2.0.0rc4/sentry_sdk/_lru_cache.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc3/sentry_sdk/_queue.py` & `sentry-sdk-2.0.0rc4/sentry_sdk/_queue.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc3/sentry_sdk/_types.py` & `sentry-sdk-2.0.0rc4/sentry_sdk/_types.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc3/sentry_sdk/_werkzeug.py` & `sentry-sdk-2.0.0rc4/sentry_sdk/_werkzeug.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc3/sentry_sdk/api.py` & `sentry-sdk-2.0.0rc4/sentry_sdk/api.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import inspect
 from contextlib import contextmanager
 
 from sentry_sdk import tracing_utils, Client
 from sentry_sdk._types import TYPE_CHECKING
+from sentry_sdk.consts import INSTRUMENTER
 from sentry_sdk.scope import Scope, _ScopeManager, new_scope, isolation_scope
 from sentry_sdk.tracing import NoOpSpan, Transaction
 
 if TYPE_CHECKING:
     from typing import Any
     from typing import Dict
     from typing import Generator
@@ -24,17 +25,17 @@
         Event,
         Hint,
         Breadcrumb,
         BreadcrumbHint,
         ExcInfo,
         MeasurementUnit,
         LogLevelStr,
+        SamplingContext,
     )
-    from sentry_sdk.scope import StartTransactionKwargs
-    from sentry_sdk.tracing import Span
+    from sentry_sdk.tracing import Span, TransactionKwargs
 
     T = TypeVar("T")
     F = TypeVar("F", bound=Callable[..., Any])
 else:
 
     def overload(x):
         # type: (T) -> T
@@ -278,18 +279,52 @@
     # type: (...) -> Span
     return Scope.get_current_scope().start_span(**kwargs)
 
 
 @scopemethod
 def start_transaction(
     transaction=None,  # type: Optional[Transaction]
-    **kwargs,  # type: Unpack[StartTransactionKwargs]
+    instrumenter=INSTRUMENTER.SENTRY,  # type: str
+    custom_sampling_context=None,  # type: Optional[SamplingContext]
+    **kwargs,  # type: Unpack[TransactionKwargs]
 ):
     # type: (...) -> Union[Transaction, NoOpSpan]
-    return Scope.get_current_scope().start_transaction(transaction, **kwargs)
+    """
+    Start and return a transaction on the current scope.
+
+    Start an existing transaction if given, otherwise create and start a new
+    transaction with kwargs.
+
+    This is the entry point to manual tracing instrumentation.
+
+    A tree structure can be built by adding child spans to the transaction,
+    and child spans to other spans. To start a new child span within the
+    transaction or any span, call the respective `.start_child()` method.
+
+    Every child span must be finished before the transaction is finished,
+    otherwise the unfinished spans are discarded.
+
+    When used as context managers, spans and transactions are automatically
+    finished at the end of the `with` block. If not using context managers,
+    call the `.finish()` method.
+
+    When the transaction is finished, it will be sent to Sentry with all its
+    finished child spans.
+
+    :param transaction: The transaction to start. If omitted, we create and
+        start a new transaction.
+    :param instrumenter: This parameter is meant for internal use only.
+    :param custom_sampling_context: The transaction's custom sampling context.
+    :param kwargs: Optional keyword arguments to be passed to the Transaction
+        constructor. See :py:class:`sentry_sdk.tracing.Transaction` for
+        available arguments.
+    """
+    return Scope.get_current_scope().start_transaction(
+        transaction, instrumenter, custom_sampling_context, **kwargs
+    )
 
 
 def set_measurement(name, value, unit=""):
     # type: (str, float, MeasurementUnit) -> None
     transaction = Scope.get_current_scope().transaction
     if transaction is not None:
         transaction.set_measurement(name, value, unit)
```

### Comparing `sentry-sdk-2.0.0rc3/sentry_sdk/attachments.py` & `sentry-sdk-2.0.0rc4/sentry_sdk/attachments.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc3/sentry_sdk/client.py` & `sentry-sdk-2.0.0rc4/sentry_sdk/client.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc3/sentry_sdk/consts.py` & `sentry-sdk-2.0.0rc4/sentry_sdk/consts.py`

 * *Files 3% similar despite different names*

```diff
@@ -197,14 +197,26 @@
 
     CODE_NAMESPACE = "code.namespace"
     """
     The "namespace" within which `code.function` is defined. Usually the qualified class or module name, such that `code.namespace` + some separator + `code.function` form a unique identifier for the code unit.
     Example: "http.handler"
     """
 
+    THREAD_ID = "thread.id"
+    """
+    Identifier of a thread from where the span originated. This should be a string.
+    Example: "7972576320"
+    """
+
+    THREAD_NAME = "thread.name"
+    """
+    Label identifying a thread from where the span originated. This should be a string.
+    Example: "MainThread"
+    """
+
 
 class OP:
     CACHE_GET_ITEM = "cache.get_item"
     DB = "db"
     DB_REDIS = "db.redis"
     EVENT_DJANGO = "event.django"
     FUNCTION = "function"
@@ -327,8 +339,8 @@
     return dict(zip(a.args[-len(defaults) :], defaults))
 
 
 DEFAULT_OPTIONS = _get_default_options()
 del _get_default_options
 
 
-VERSION = "2.0.0rc3"
+VERSION = "2.0.0rc4"
```

### Comparing `sentry-sdk-2.0.0rc3/sentry_sdk/crons/api.py` & `sentry-sdk-2.0.0rc4/sentry_sdk/crons/api.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import uuid
 
-from sentry_sdk import Hub
+import sentry_sdk
 from sentry_sdk._types import TYPE_CHECKING
 
 
 if TYPE_CHECKING:
     from typing import Any, Dict, Optional
     from sentry_sdk._types import Event
 
@@ -13,15 +13,15 @@
     monitor_slug=None,
     check_in_id=None,
     status=None,
     duration_s=None,
     monitor_config=None,
 ):
     # type: (Optional[str], Optional[str], Optional[str], Optional[float], Optional[Dict[str, Any]]) -> Event
-    options = Hub.current.client.options if Hub.current.client else {}
+    options = sentry_sdk.get_client().options
     check_in_id = check_in_id or uuid.uuid4().hex  # type: str
 
     check_in = {
         "type": "check_in",
         "monitor_slug": monitor_slug,
         "check_in_id": check_in_id,
         "status": status,
@@ -48,11 +48,10 @@
         monitor_slug=monitor_slug,
         check_in_id=check_in_id,
         status=status,
         duration_s=duration,
         monitor_config=monitor_config,
     )
 
-    hub = Hub.current
-    hub.capture_event(check_in_event)
+    sentry_sdk.capture_event(check_in_event)
 
     return check_in_event["check_in_id"]
```

### Comparing `sentry-sdk-2.0.0rc3/sentry_sdk/db/explain_plan/__init__.py` & `sentry-sdk-2.0.0rc4/sentry_sdk/db/explain_plan/__init__.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc3/sentry_sdk/db/explain_plan/django.py` & `sentry-sdk-2.0.0rc4/sentry_sdk/db/explain_plan/django.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc3/sentry_sdk/db/explain_plan/sqlalchemy.py` & `sentry-sdk-2.0.0rc4/sentry_sdk/db/explain_plan/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc3/sentry_sdk/debug.py` & `sentry-sdk-2.0.0rc4/sentry_sdk/debug.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc3/sentry_sdk/envelope.py` & `sentry-sdk-2.0.0rc4/sentry_sdk/envelope.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc3/sentry_sdk/hub.py` & `sentry-sdk-2.0.0rc4/sentry_sdk/hub.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,17 +38,18 @@
     from sentry_sdk._types import (
         Event,
         Hint,
         Breadcrumb,
         BreadcrumbHint,
         ExcInfo,
         LogLevelStr,
+        SamplingContext,
     )
     from sentry_sdk.consts import ClientConstructor
-    from sentry_sdk.scope import StartTransactionKwargs
+    from sentry_sdk.tracing import TransactionKwargs
 
     T = TypeVar("T")
 
 else:
 
     def overload(x):
         # type: (T) -> T
@@ -468,17 +469,21 @@
 
         For supported `**kwargs` see :py:class:`sentry_sdk.tracing.Span`.
         """
         scope = Scope.get_current_scope()
         return scope.start_span(instrumenter=instrumenter, **kwargs)
 
     def start_transaction(
-        self, transaction=None, instrumenter=INSTRUMENTER.SENTRY, **kwargs
+        self,
+        transaction=None,
+        instrumenter=INSTRUMENTER.SENTRY,
+        custom_sampling_context=None,
+        **kwargs
     ):
-        # type: (Optional[Transaction], str, Unpack[StartTransactionKwargs]) -> Union[Transaction, NoOpSpan]
+        # type: (Optional[Transaction], str, Optional[SamplingContext], Unpack[TransactionKwargs]) -> Union[Transaction, NoOpSpan]
         """
         .. deprecated:: 2.0.0
             This function is deprecated and will be removed in a future release.
             Please use :py:meth:`sentry_sdk.Scope.start_transaction` instead.
 
         Start and return a transaction.
 
@@ -507,15 +512,15 @@
 
         # For backwards compatibility, we allow passing the scope as the hub.
         # We need a major release to make this nice. (if someone searches the code: deprecated)
         # Type checking disabled for this line because deprecated keys are not allowed in the type signature.
         kwargs["hub"] = scope  # type: ignore
 
         return scope.start_transaction(
-            transaction=transaction, instrumenter=instrumenter, **kwargs
+            transaction, instrumenter, custom_sampling_context, **kwargs
         )
 
     def continue_trace(self, environ_or_headers, op=None, name=None, source=None):
         # type: (Dict[str, Any], Optional[str], Optional[str], Optional[str]) -> Transaction
         """
         .. deprecated:: 2.0.0
             This function is deprecated and will be removed in a future release.
```

### Comparing `sentry-sdk-2.0.0rc3/sentry_sdk/integrations/__init__.py` & `sentry-sdk-2.0.0rc4/sentry_sdk/integrations/__init__.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc3/sentry_sdk/integrations/_asgi_common.py` & `sentry-sdk-2.0.0rc4/sentry_sdk/integrations/_asgi_common.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc3/sentry_sdk/integrations/_wsgi_common.py` & `sentry-sdk-2.0.0rc4/sentry_sdk/integrations/_wsgi_common.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 import json
 from copy import deepcopy
 
-from sentry_sdk.hub import Hub, _should_send_default_pii
+import sentry_sdk
+from sentry_sdk.scope import should_send_default_pii
 from sentry_sdk.utils import AnnotatedValue
 from sentry_sdk._types import TYPE_CHECKING
 
 try:
     from django.http.request import RawPostDataException
 except ImportError:
     RawPostDataException = None
 
 
 if TYPE_CHECKING:
-    import sentry_sdk
-
     from typing import Any
     from typing import Dict
     from typing import Mapping
     from typing import Optional
     from typing import Union
     from sentry_sdk._types import Event
 
@@ -63,24 +62,24 @@
 
     def __init__(self, request):
         # type: (Any) -> None
         self.request = request
 
     def extract_into_event(self, event):
         # type: (Event) -> None
-        client = Hub.current.client
-        if client is None:
+        client = sentry_sdk.get_client()
+        if not client.is_active():
             return
 
         data = None  # type: Optional[Union[AnnotatedValue, Dict[str, Any]]]
 
         content_length = self.content_length()
         request_info = event.get("request", {})
 
-        if _should_send_default_pii():
+        if should_send_default_pii():
             request_info["cookies"] = dict(self.cookies())
 
         if not request_body_within_bounds(client, content_length):
             data = AnnotatedValue.removed_because_over_size_limit()
         else:
             # First read the raw body data
             # It is important to read this first because if it is Django
@@ -186,15 +185,15 @@
         or (mt.startswith("application/"))
         and mt.endswith("+json")
     )
 
 
 def _filter_headers(headers):
     # type: (Mapping[str, str]) -> Mapping[str, Union[AnnotatedValue, str]]
-    if _should_send_default_pii():
+    if should_send_default_pii():
         return headers
 
     return {
         k: (
             v
             if k.upper().replace("-", "_") not in SENSITIVE_HEADERS
             else AnnotatedValue.removed_because_over_size_limit()
```

### Comparing `sentry-sdk-2.0.0rc3/sentry_sdk/integrations/aiohttp.py` & `sentry-sdk-2.0.0rc4/sentry_sdk/integrations/aiohttp.py`

 * *Files 1% similar despite different names*

```diff
@@ -186,20 +186,17 @@
 
         ClientSession.__init__ = init
 
 
 def create_trace_config():
     # type: () -> TraceConfig
 
+    @ensure_integration_enabled_async(AioHttpIntegration)
     async def on_request_start(session, trace_config_ctx, params):
         # type: (ClientSession, SimpleNamespace, TraceRequestStartParams) -> None
-        client = sentry_sdk.get_client()
-        if client.get_integration(AioHttpIntegration) is None:
-            return
-
         method = params.method.upper()
 
         parsed_url = None
         with capture_internal_exceptions():
             parsed_url = parse_url(str(params.url), sanitize=False)
 
         span = sentry_sdk.start_span(
@@ -209,14 +206,16 @@
         )
         span.set_data(SPANDATA.HTTP_METHOD, method)
         if parsed_url is not None:
             span.set_data("url", parsed_url.url)
             span.set_data(SPANDATA.HTTP_QUERY, parsed_url.query)
             span.set_data(SPANDATA.HTTP_FRAGMENT, parsed_url.fragment)
 
+        client = sentry_sdk.get_client()
+
         if should_propagate_trace(client, str(params.url)):
             for key, value in Scope.get_current_scope().iter_trace_propagation_headers(
                 span=span
             ):
                 logger.debug(
                     "[Tracing] Adding `{key}` header {value} to outgoing request to {url}.".format(
                         key=key, value=value, url=params.url
```

### Comparing `sentry-sdk-2.0.0rc3/sentry_sdk/integrations/argv.py` & `sentry-sdk-2.0.0rc4/sentry_sdk/integrations/argv.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc3/sentry_sdk/integrations/ariadne.py` & `sentry-sdk-2.0.0rc4/sentry_sdk/integrations/ariadne.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc3/sentry_sdk/integrations/arq.py` & `sentry-sdk-2.0.0rc4/sentry_sdk/integrations/arq.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import sys
 
+import sentry_sdk
 from sentry_sdk._types import TYPE_CHECKING
-from sentry_sdk import Hub
 from sentry_sdk.consts import OP
-from sentry_sdk.hub import _should_send_default_pii
 from sentry_sdk.integrations import DidNotEnable, Integration
 from sentry_sdk.integrations.logging import ignore_logger
-from sentry_sdk.scope import Scope
+from sentry_sdk.scope import Scope, should_send_default_pii
 from sentry_sdk.tracing import Transaction, TRANSACTION_SOURCE_TASK
 from sentry_sdk.utils import (
     capture_internal_exceptions,
+    ensure_integration_enabled,
+    ensure_integration_enabled_async,
     event_from_exception,
     SENSITIVE_DATA_SUBSTITUTE,
     parse_version,
     reraise,
 )
 
 try:
@@ -66,50 +67,42 @@
         ignore_logger("arq.worker")
 
 
 def patch_enqueue_job():
     # type: () -> None
     old_enqueue_job = ArqRedis.enqueue_job
 
+    @ensure_integration_enabled_async(ArqIntegration, old_enqueue_job)
     async def _sentry_enqueue_job(self, function, *args, **kwargs):
         # type: (ArqRedis, str, *Any, **Any) -> Optional[Job]
-        hub = Hub.current
-
-        if hub.get_integration(ArqIntegration) is None:
-            return await old_enqueue_job(self, function, *args, **kwargs)
-
-        with hub.start_span(op=OP.QUEUE_SUBMIT_ARQ, description=function):
+        with sentry_sdk.start_span(op=OP.QUEUE_SUBMIT_ARQ, description=function):
             return await old_enqueue_job(self, function, *args, **kwargs)
 
     ArqRedis.enqueue_job = _sentry_enqueue_job
 
 
 def patch_run_job():
     # type: () -> None
     old_run_job = Worker.run_job
 
+    @ensure_integration_enabled_async(ArqIntegration, old_run_job)
     async def _sentry_run_job(self, job_id, score):
         # type: (Worker, str, int) -> None
-        hub = Hub(Hub.current)
-
-        if hub.get_integration(ArqIntegration) is None:
-            return await old_run_job(self, job_id, score)
-
-        with hub.push_scope() as scope:
+        with sentry_sdk.isolation_scope() as scope:
             scope._name = "arq"
             scope.clear_breadcrumbs()
 
             transaction = Transaction(
                 name="unknown arq task",
                 status="ok",
                 op=OP.QUEUE_TASK_ARQ,
                 source=TRANSACTION_SOURCE_TASK,
             )
 
-            with hub.start_transaction(transaction):
+            with sentry_sdk.start_transaction(transaction):
                 return await old_run_job(self, job_id, score)
 
     Worker.run_job = _sentry_run_job
 
 
 def _capture_exception(exc_info):
     # type: (ExcInfo) -> None
@@ -123,15 +116,15 @@
         scope.transaction.set_status("internal_error")
 
     event, hint = event_from_exception(
         exc_info,
         client_options=Scope.get_client().options,
         mechanism={"type": ArqIntegration.identifier, "handled": False},
     )
-    scope.capture_event(event, hint=hint)
+    sentry_sdk.capture_event(event, hint=hint)
 
 
 def _make_event_processor(ctx, *args, **kwargs):
     # type: (Dict[Any, Any], *Any, **Any) -> EventProcessor
     def event_processor(event, hint):
         # type: (Event, Hint) -> Optional[Event]
 
@@ -144,36 +137,34 @@
             tags = event.setdefault("tags", {})
             tags["arq_task_id"] = ctx["job_id"]
             tags["arq_task_retry"] = ctx["job_try"] > 1
             extra = event.setdefault("extra", {})
             extra["arq-job"] = {
                 "task": ctx["job_name"],
                 "args": (
-                    args if _should_send_default_pii() else SENSITIVE_DATA_SUBSTITUTE
+                    args if should_send_default_pii() else SENSITIVE_DATA_SUBSTITUTE
                 ),
                 "kwargs": (
-                    kwargs if _should_send_default_pii() else SENSITIVE_DATA_SUBSTITUTE
+                    kwargs if should_send_default_pii() else SENSITIVE_DATA_SUBSTITUTE
                 ),
                 "retry": ctx["job_try"],
             }
 
         return event
 
     return event_processor
 
 
 def _wrap_coroutine(name, coroutine):
     # type: (str, WorkerCoroutine) -> WorkerCoroutine
+
+    @ensure_integration_enabled_async(ArqIntegration, coroutine)
     async def _sentry_coroutine(ctx, *args, **kwargs):
         # type: (Dict[Any, Any], *Any, **Any) -> Any
-        hub = Hub.current
-        if hub.get_integration(ArqIntegration) is None:
-            return await coroutine(ctx, *args, **kwargs)
-
-        hub.scope.add_event_processor(
+        Scope.get_isolation_scope().add_event_processor(
             _make_event_processor({**ctx, "job_name": name}, *args, **kwargs)
         )
 
         try:
             result = await coroutine(ctx, *args, **kwargs)
         except Exception:
             exc_info = sys.exc_info()
@@ -185,21 +176,17 @@
     return _sentry_coroutine
 
 
 def patch_create_worker():
     # type: () -> None
     old_create_worker = arq.worker.create_worker
 
+    @ensure_integration_enabled(ArqIntegration, old_create_worker)
     def _sentry_create_worker(*args, **kwargs):
         # type: (*Any, **Any) -> Worker
-        hub = Hub.current
-
-        if hub.get_integration(ArqIntegration) is None:
-            return old_create_worker(*args, **kwargs)
-
         settings_cls = args[0]
 
         if hasattr(settings_cls, "functions"):
             settings_cls.functions = [
                 _get_arq_function(func) for func in settings_cls.functions
             ]
         if hasattr(settings_cls, "cron_jobs"):
```

### Comparing `sentry-sdk-2.0.0rc3/sentry_sdk/integrations/asgi.py` & `sentry-sdk-2.0.0rc4/sentry_sdk/integrations/asgi.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,25 +5,25 @@
 """
 
 import asyncio
 import inspect
 from copy import deepcopy
 from functools import partial
 
+import sentry_sdk
 from sentry_sdk._types import TYPE_CHECKING
 from sentry_sdk.api import continue_trace
 from sentry_sdk.consts import OP
-from sentry_sdk.hub import Hub
 
 from sentry_sdk.integrations._asgi_common import (
     _get_headers,
     _get_request_data,
     _get_url,
 )
-from sentry_sdk.sessions import auto_session_tracking
+from sentry_sdk.sessions import auto_session_tracking_scope
 from sentry_sdk.tracing import (
     SOURCE_FOR_STYLE,
     TRANSACTION_SOURCE_ROUTE,
     TRANSACTION_SOURCE_URL,
     TRANSACTION_SOURCE_COMPONENT,
 )
 from sentry_sdk.utils import (
@@ -50,25 +50,23 @@
 _asgi_middleware_applied = ContextVar("sentry_asgi_middleware_applied")
 
 _DEFAULT_TRANSACTION_NAME = "generic ASGI request"
 
 TRANSACTION_STYLE_VALUES = ("endpoint", "url")
 
 
-def _capture_exception(hub, exc, mechanism_type="asgi"):
-    # type: (Hub, Any, str) -> None
+def _capture_exception(exc, mechanism_type="asgi"):
+    # type: (Any, str) -> None
 
-    # Check client here as it might have been unset while streaming response
-    if hub.client is not None:
-        event, hint = event_from_exception(
-            exc,
-            client_options=hub.client.options,
-            mechanism={"type": mechanism_type, "handled": False},
-        )
-        hub.capture_event(event, hint=hint)
+    event, hint = event_from_exception(
+        exc,
+        client_options=sentry_sdk.get_client().options,
+        mechanism={"type": mechanism_type, "handled": False},
+    )
+    sentry_sdk.capture_event(event, hint=hint)
 
 
 def _looks_like_asgi3(app):
     # type: (Any) -> bool
     """
     Try to figure out if an application object supports ASGI3.
 
@@ -153,27 +151,25 @@
             try:
                 if asgi_version == 2:
                     return await self.app(scope)(receive, send)
                 else:
                     return await self.app(scope, receive, send)
 
             except Exception as exc:
-                _capture_exception(Hub.current, exc, mechanism_type=self.mechanism_type)
+                _capture_exception(exc, mechanism_type=self.mechanism_type)
                 raise exc from None
 
         _asgi_middleware_applied.set(True)
         try:
-            hub = Hub(Hub.current)
-            with hub:
-                with auto_session_tracking(hub, session_mode="request"):
-                    with hub.configure_scope() as sentry_scope:
-                        sentry_scope.clear_breadcrumbs()
-                        sentry_scope._name = "asgi"
-                        processor = partial(self.event_processor, asgi_scope=scope)
-                        sentry_scope.add_event_processor(processor)
+            with sentry_sdk.isolation_scope() as sentry_scope:
+                with auto_session_tracking_scope(sentry_scope, session_mode="request"):
+                    sentry_scope.clear_breadcrumbs()
+                    sentry_scope._name = "asgi"
+                    processor = partial(self.event_processor, asgi_scope=scope)
+                    sentry_scope.add_event_processor(processor)
 
                     ty = scope["type"]
                     (
                         transaction_name,
                         transaction_source,
                     ) = self._get_transaction_name_and_source(
                         self.transaction_style,
@@ -204,15 +200,15 @@
                     transaction.set_tag("asgi.type", ty)
                     logger.debug(
                         "[ASGI] Set transaction name and source on transaction: '%s' / '%s'",
                         transaction.name,
                         transaction.source,
                     )
 
-                    with hub.start_transaction(
+                    with sentry_sdk.start_transaction(
                         transaction, custom_sampling_context={"asgi_scope": scope}
                     ):
                         logger.debug("[ASGI] Started transaction: %s", transaction)
                         try:
 
                             async def _sentry_wrapped_send(event):
                                 # type: (Dict[str, Any]) -> Any
@@ -231,17 +227,15 @@
                                     receive, _sentry_wrapped_send
                                 )
                             else:
                                 return await self.app(
                                     scope, receive, _sentry_wrapped_send
                                 )
                         except Exception as exc:
-                            _capture_exception(
-                                hub, exc, mechanism_type=self.mechanism_type
-                            )
+                            _capture_exception(exc, mechanism_type=self.mechanism_type)
                             raise exc from None
         finally:
             _asgi_middleware_applied.set(False)
 
     def event_processor(self, event, hint, asgi_scope):
         # type: (Event, Hint, Any) -> Optional[Event]
         request_data = event.get("request", {})
```

### Comparing `sentry-sdk-2.0.0rc3/sentry_sdk/integrations/asyncio.py` & `sentry-sdk-2.0.0rc4/sentry_sdk/integrations/asyncio.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import sys
 
+import sentry_sdk
 from sentry_sdk.consts import OP
-from sentry_sdk.hub import Hub
 from sentry_sdk.integrations import Integration, DidNotEnable
 from sentry_sdk._types import TYPE_CHECKING
 from sentry_sdk.utils import event_from_exception, reraise
 
 try:
     import asyncio
     from asyncio.tasks import Task
@@ -37,23 +37,24 @@
         orig_task_factory = loop.get_task_factory()
 
         def _sentry_task_factory(loop, coro, **kwargs):
             # type: (asyncio.AbstractEventLoop, Coroutine[Any, Any, Any], Any) -> asyncio.Future[Any]
 
             async def _coro_creating_hub_and_span():
                 # type: () -> Any
-                hub = Hub(Hub.current)
                 result = None
 
-                with hub:
-                    with hub.start_span(op=OP.FUNCTION, description=get_name(coro)):
+                with sentry_sdk.isolation_scope():
+                    with sentry_sdk.start_span(
+                        op=OP.FUNCTION, description=get_name(coro)
+                    ):
                         try:
                             result = await coro
                         except Exception:
-                            reraise(*_capture_exception(hub))
+                            reraise(*_capture_exception())
 
                 return result
 
             # Trying to use user set task factory (if there is one)
             if orig_task_factory:
                 return orig_task_factory(loop, _coro_creating_hub_and_span(), **kwargs)
 
@@ -72,29 +73,28 @@
 
         loop.set_task_factory(_sentry_task_factory)  # type: ignore
     except RuntimeError:
         # When there is no running loop, we have nothing to patch.
         pass
 
 
-def _capture_exception(hub):
-    # type: (Hub) -> ExcInfo
+def _capture_exception():
+    # type: () -> ExcInfo
     exc_info = sys.exc_info()
 
-    integration = hub.get_integration(AsyncioIntegration)
-    if integration is not None:
-        # If an integration is there, a client has to be there.
-        client = hub.client  # type: Any
+    client = sentry_sdk.get_client()
 
+    integration = client.get_integration(AsyncioIntegration)
+    if integration is not None:
         event, hint = event_from_exception(
             exc_info,
             client_options=client.options,
             mechanism={"type": "asyncio", "handled": False},
         )
-        hub.capture_event(event, hint=hint)
+        sentry_sdk.capture_event(event, hint=hint)
 
     return exc_info
 
 
 class AsyncioIntegration(Integration):
     identifier = "asyncio"
```

### Comparing `sentry-sdk-2.0.0rc3/sentry_sdk/integrations/asyncpg.py` & `sentry-sdk-2.0.0rc4/sentry_sdk/integrations/asyncpg.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,22 +54,21 @@
         )
 
 
 T = TypeVar("T")
 
 
 def _wrap_execute(f: Callable[..., Awaitable[T]]) -> Callable[..., Awaitable[T]]:
+    @ensure_integration_enabled_async(AsyncPGIntegration, f)
     async def _inner(*args: Any, **kwargs: Any) -> T:
-        integration = sentry_sdk.get_client().get_integration(AsyncPGIntegration)
-
         # Avoid recording calls to _execute twice.
         # Calls to Connection.execute with args also call
         # Connection._execute, which is recorded separately
         # args[0] = the connection object, args[1] is the query
-        if integration is None or len(args) > 2:
+        if len(args) > 2:
             return await f(*args, **kwargs)
 
         query = args[1]
         with record_sql_queries(None, query, None, None, executemany=False) as span:
             res = await f(*args, **kwargs)
 
         with capture_internal_exceptions():
```

### Comparing `sentry-sdk-2.0.0rc3/sentry_sdk/integrations/atexit.py` & `sentry-sdk-2.0.0rc4/sentry_sdk/integrations/atexit.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import sys
 import atexit
 
 import sentry_sdk
 from sentry_sdk import Scope
 from sentry_sdk.utils import logger
 from sentry_sdk.integrations import Integration
-
+from sentry_sdk.utils import ensure_integration_enabled
 from sentry_sdk._types import TYPE_CHECKING
 
 if TYPE_CHECKING:
     from typing import Any
     from typing import Optional
 
 
@@ -40,17 +40,17 @@
             callback = default_callback
         self.callback = callback
 
     @staticmethod
     def setup_once():
         # type: () -> None
         @atexit.register
+        @ensure_integration_enabled(AtexitIntegration)
         def _shutdown():
             # type: () -> None
             logger.debug("atexit: got shutdown signal")
             client = sentry_sdk.get_client()
             integration = client.get_integration(AtexitIntegration)
-            if integration is not None:
-                logger.debug("atexit: shutting down client")
 
-                Scope.get_isolation_scope().end_session()
-                client.close(callback=integration.callback)
+            logger.debug("atexit: shutting down client")
+            Scope.get_isolation_scope().end_session()
+            client.close(callback=integration.callback)
```

### Comparing `sentry-sdk-2.0.0rc3/sentry_sdk/integrations/aws_lambda.py` & `sentry-sdk-2.0.0rc4/sentry_sdk/integrations/aws_lambda.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 import sys
 from copy import deepcopy
 from datetime import datetime, timedelta, timezone
 from os import environ
 
+import sentry_sdk
 from sentry_sdk.api import continue_trace
 from sentry_sdk.consts import OP
-from sentry_sdk.hub import Hub, _should_send_default_pii
+from sentry_sdk.scope import Scope, should_send_default_pii
 from sentry_sdk.tracing import TRANSACTION_SOURCE_COMPONENT
 from sentry_sdk.utils import (
     AnnotatedValue,
     capture_internal_exceptions,
+    ensure_integration_enabled,
     event_from_exception,
     logger,
     TimeoutThread,
     reraise,
 )
 from sentry_sdk.integrations import Integration
 from sentry_sdk.integrations._wsgi_common import _filter_headers
@@ -32,45 +34,39 @@
 # Constants
 TIMEOUT_WARNING_BUFFER = 1500  # Buffer time required to send timeout warning to Sentry
 MILLIS_TO_SECONDS = 1000.0
 
 
 def _wrap_init_error(init_error):
     # type: (F) -> F
+    @ensure_integration_enabled(AwsLambdaIntegration, init_error)
     def sentry_init_error(*args, **kwargs):
         # type: (*Any, **Any) -> Any
-
-        hub = Hub.current
-        integration = hub.get_integration(AwsLambdaIntegration)
-        if integration is None:
-            return init_error(*args, **kwargs)
-
-        # If an integration is there, a client has to be there.
-        client = hub.client  # type: Any
+        client = sentry_sdk.get_client()
 
         with capture_internal_exceptions():
-            with hub.configure_scope() as scope:
-                scope.clear_breadcrumbs()
+            Scope.get_isolation_scope().clear_breadcrumbs()
 
             exc_info = sys.exc_info()
             if exc_info and all(exc_info):
                 sentry_event, hint = event_from_exception(
                     exc_info,
                     client_options=client.options,
                     mechanism={"type": "aws_lambda", "handled": False},
                 )
-                hub.capture_event(sentry_event, hint=hint)
+                sentry_sdk.capture_event(sentry_event, hint=hint)
 
         return init_error(*args, **kwargs)
 
     return sentry_init_error  # type: ignore
 
 
 def _wrap_handler(handler):
     # type: (F) -> F
+    @ensure_integration_enabled(AwsLambdaIntegration, handler)
     def sentry_handler(aws_event, aws_context, *args, **kwargs):
         # type: (Any, Any, *Any, **Any) -> Any
 
         # Per https://docs.aws.amazon.com/lambda/latest/dg/python-handler.html,
         # `event` here is *likely* a dictionary, but also might be a number of
         # other types (str, int, float, None).
         #
@@ -89,24 +85,20 @@
 
         if not isinstance(request_data, dict):
             # If we're not dealing with a dictionary, we won't be able to get
             # headers, path, http method, etc in any case, so it's fine that
             # this is empty
             request_data = {}
 
-        hub = Hub.current
-        integration = hub.get_integration(AwsLambdaIntegration)
-        if integration is None:
-            return handler(aws_event, aws_context, *args, **kwargs)
+        client = sentry_sdk.get_client()
+        integration = client.get_integration(AwsLambdaIntegration)
 
-        # If an integration is there, a client has to be there.
-        client = hub.client  # type: Any
         configured_time = aws_context.get_remaining_time_in_millis()
 
-        with hub.push_scope() as scope:
+        with sentry_sdk.isolation_scope() as scope:
             timeout_thread = None
             with capture_internal_exceptions():
                 scope.clear_breadcrumbs()
                 scope.add_event_processor(
                     _make_request_event_processor(
                         request_data, aws_context, configured_time
                     )
@@ -144,15 +136,15 @@
 
             transaction = continue_trace(
                 headers,
                 op=OP.FUNCTION_AWS,
                 name=aws_context.function_name,
                 source=TRANSACTION_SOURCE_COMPONENT,
             )
-            with hub.start_transaction(
+            with sentry_sdk.start_transaction(
                 transaction,
                 custom_sampling_context={
                     "aws_event": aws_event,
                     "aws_context": aws_context,
                 },
             ):
                 try:
@@ -160,32 +152,32 @@
                 except Exception:
                     exc_info = sys.exc_info()
                     sentry_event, hint = event_from_exception(
                         exc_info,
                         client_options=client.options,
                         mechanism={"type": "aws_lambda", "handled": False},
                     )
-                    hub.capture_event(sentry_event, hint=hint)
+                    sentry_sdk.capture_event(sentry_event, hint=hint)
                     reraise(*exc_info)
                 finally:
                     if timeout_thread:
                         timeout_thread.stop()
 
     return sentry_handler  # type: ignore
 
 
 def _drain_queue():
     # type: () -> None
     with capture_internal_exceptions():
-        hub = Hub.current
-        integration = hub.get_integration(AwsLambdaIntegration)
+        client = sentry_sdk.get_client()
+        integration = client.get_integration(AwsLambdaIntegration)
         if integration is not None:
             # Flush out the event queue before AWS kills the
             # process.
-            hub.flush()
+            client.flush()
 
 
 class AwsLambdaIntegration(Integration):
     identifier = "aws_lambda"
 
     def __init__(self, timeout_warning=False):
         # type: (bool) -> None
@@ -354,15 +346,15 @@
 
         if "queryStringParameters" in aws_event:
             request["query_string"] = aws_event["queryStringParameters"]
 
         if "headers" in aws_event:
             request["headers"] = _filter_headers(aws_event["headers"])
 
-        if _should_send_default_pii():
+        if should_send_default_pii():
             user_info = sentry_event.setdefault("user", {})
 
             identity = aws_event.get("identity")
             if identity is None:
                 identity = {}
 
             id = identity.get("userArn")
```

### Comparing `sentry-sdk-2.0.0rc3/sentry_sdk/integrations/beam.py` & `sentry-sdk-2.0.0rc4/sentry_sdk/integrations/beam.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 import sys
 import types
 from functools import wraps
 
-from sentry_sdk.hub import Hub
-from sentry_sdk.utils import capture_internal_exceptions, event_from_exception, reraise
+import sentry_sdk
 from sentry_sdk.integrations import Integration
 from sentry_sdk.integrations.logging import ignore_logger
+from sentry_sdk.utils import (
+    capture_internal_exceptions,
+    ensure_integration_enabled,
+    event_from_exception,
+    reraise,
+)
 from sentry_sdk._types import TYPE_CHECKING
 
 if TYPE_CHECKING:
     from typing import Any
     from typing import Iterator
     from typing import TypeVar
-    from typing import Optional
     from typing import Callable
 
-    from sentry_sdk.client import BaseClient
     from sentry_sdk._types import ExcInfo
 
     T = TypeVar("T")
     F = TypeVar("F", bound=Callable[..., Any])
 
 
 WRAPPED_FUNC = "_wrapped_{}_"
@@ -109,74 +112,64 @@
     return _inspect
 
 
 def _wrap_task_call(func):
     # type: (F) -> F
     """
     Wrap task call with a try catch to get exceptions.
-    Pass the client on to raise_exception so it can get rebinded.
     """
-    client = Hub.current.client
 
     @wraps(func)
     def _inner(*args, **kwargs):
         # type: (*Any, **Any) -> Any
         try:
             gen = func(*args, **kwargs)
         except Exception:
-            raise_exception(client)
+            raise_exception()
 
         if not isinstance(gen, types.GeneratorType):
             return gen
-        return _wrap_generator_call(gen, client)
+        return _wrap_generator_call(gen)
 
     setattr(_inner, USED_FUNC, True)
     return _inner  # type: ignore
 
 
-def _capture_exception(exc_info, hub):
-    # type: (ExcInfo, Hub) -> None
+@ensure_integration_enabled(BeamIntegration)
+def _capture_exception(exc_info):
+    # type: (ExcInfo) -> None
     """
     Send Beam exception to Sentry.
     """
-    integration = hub.get_integration(BeamIntegration)
-    if integration is None:
-        return
-
-    client = hub.client
-    if client is None:
-        return
+    client = sentry_sdk.get_client()
 
     event, hint = event_from_exception(
         exc_info,
         client_options=client.options,
         mechanism={"type": "beam", "handled": False},
     )
-    hub.capture_event(event, hint=hint)
+    sentry_sdk.capture_event(event, hint=hint)
 
 
-def raise_exception(client):
-    # type: (Optional[BaseClient]) -> None
+def raise_exception():
+    # type: () -> None
     """
-    Raise an exception. If the client is not in the hub, rebind it.
+    Raise an exception.
     """
-    hub = Hub.current
-    if hub.client is None:
-        hub.bind_client(client)
     exc_info = sys.exc_info()
     with capture_internal_exceptions():
-        _capture_exception(exc_info, hub)
+        _capture_exception(exc_info)
     reraise(*exc_info)
 
 
-def _wrap_generator_call(gen, client):
-    # type: (Iterator[T], Optional[BaseClient]) -> Iterator[T]
+def _wrap_generator_call(gen):
+    # type: (Iterator[T]) -> Iterator[T]
     """
     Wrap the generator to handle any failures.
     """
     while True:
         try:
             yield next(gen)
         except StopIteration:
             break
         except Exception:
-            raise_exception(client)
+            raise_exception()
```

### Comparing `sentry-sdk-2.0.0rc3/sentry_sdk/integrations/boto3.py` & `sentry-sdk-2.0.0rc4/sentry_sdk/integrations/boto3.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,21 @@
 from functools import partial
 
-from sentry_sdk import Hub
+import sentry_sdk
 from sentry_sdk.consts import OP, SPANDATA
 from sentry_sdk.integrations import Integration, DidNotEnable
 from sentry_sdk.tracing import Span
 
 from sentry_sdk._types import TYPE_CHECKING
-from sentry_sdk.utils import capture_internal_exceptions, parse_url, parse_version
+from sentry_sdk.utils import (
+    capture_internal_exceptions,
+    ensure_integration_enabled,
+    parse_url,
+    parse_version,
+)
 
 if TYPE_CHECKING:
     from typing import Any
     from typing import Dict
     from typing import Optional
     from typing import Type
 
@@ -53,23 +58,19 @@
             )
             meta.events.register("after-call", _sentry_after_call)
             meta.events.register("after-call-error", _sentry_after_call_error)
 
         BaseClient.__init__ = sentry_patched_init
 
 
+@ensure_integration_enabled(Boto3Integration)
 def _sentry_request_created(service_id, request, operation_name, **kwargs):
     # type: (str, AWSRequest, str, **Any) -> None
-    hub = Hub.current
-    if hub.get_integration(Boto3Integration) is None:
-        return
-
     description = "aws.%s.%s" % (service_id, operation_name)
-    span = hub.start_span(
-        hub=hub,
+    span = sentry_sdk.start_span(
         op=OP.HTTP_CLIENT,
         description=description,
     )
 
     with capture_internal_exceptions():
         parsed_url = parse_url(request.url, sanitize=False)
         span.set_data("aws.request.url", parsed_url.url)
```

### Comparing `sentry-sdk-2.0.0rc3/sentry_sdk/integrations/bottle.py` & `sentry-sdk-2.0.0rc4/sentry_sdk/integrations/bottle.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,20 @@
-from sentry_sdk.hub import Hub
+import sentry_sdk
 from sentry_sdk.tracing import SOURCE_FOR_STYLE
 from sentry_sdk.utils import (
     capture_internal_exceptions,
+    ensure_integration_enabled,
     event_from_exception,
     parse_version,
     transaction_from_function,
 )
 from sentry_sdk.integrations import Integration, DidNotEnable
 from sentry_sdk.integrations.wsgi import SentryWsgiMiddleware
 from sentry_sdk.integrations._wsgi_common import RequestExtractor
-
+from sentry_sdk.scope import Scope
 from sentry_sdk._types import TYPE_CHECKING
 
 if TYPE_CHECKING:
     from sentry_sdk.integrations.wsgi import _ScopedResponse
     from typing import Any
     from typing import Dict
     from typing import Callable
@@ -51,95 +52,73 @@
                 % (transaction_style, TRANSACTION_STYLE_VALUES)
             )
         self.transaction_style = transaction_style
 
     @staticmethod
     def setup_once():
         # type: () -> None
-
         version = parse_version(BOTTLE_VERSION)
 
         if version is None:
             raise DidNotEnable("Unparsable Bottle version: {}".format(BOTTLE_VERSION))
 
         if version < (0, 12):
             raise DidNotEnable("Bottle 0.12 or newer required.")
 
-        # monkey patch method Bottle.__call__
         old_app = Bottle.__call__
 
+        @ensure_integration_enabled(BottleIntegration, old_app)
         def sentry_patched_wsgi_app(self, environ, start_response):
             # type: (Any, Dict[str, str], Callable[..., Any]) -> _ScopedResponse
-
-            hub = Hub.current
-            integration = hub.get_integration(BottleIntegration)
-            if integration is None:
-                return old_app(self, environ, start_response)
-
             return SentryWsgiMiddleware(lambda *a, **kw: old_app(self, *a, **kw))(
                 environ, start_response
             )
 
         Bottle.__call__ = sentry_patched_wsgi_app
 
-        # monkey patch method Bottle._handle
         old_handle = Bottle._handle
 
+        @ensure_integration_enabled(BottleIntegration, old_handle)
         def _patched_handle(self, environ):
             # type: (Bottle, Dict[str, Any]) -> Any
-            hub = Hub.current
-            integration = hub.get_integration(BottleIntegration)
-            if integration is None:
-                return old_handle(self, environ)
-
-            # create new scope
-            scope_manager = hub.push_scope()
-
-            with scope_manager:
-                app = self
-                with hub.configure_scope() as scope:
-                    scope._name = "bottle"
-                    scope.add_event_processor(
-                        _make_request_event_processor(app, bottle_request, integration)
-                    )
-                res = old_handle(self, environ)
+            integration = sentry_sdk.get_client().get_integration(BottleIntegration)
+
+            scope = Scope.get_isolation_scope()
+            scope._name = "bottle"
+            scope.add_event_processor(
+                _make_request_event_processor(self, bottle_request, integration)
+            )
+            res = old_handle(self, environ)
 
-            # scope cleanup
             return res
 
         Bottle._handle = _patched_handle
 
-        # monkey patch method Route._make_callback
         old_make_callback = Route._make_callback
 
+        @ensure_integration_enabled(BottleIntegration, old_make_callback)
         def patched_make_callback(self, *args, **kwargs):
             # type: (Route, *object, **object) -> Any
-            hub = Hub.current
-            integration = hub.get_integration(BottleIntegration)
+            client = sentry_sdk.get_client()
             prepared_callback = old_make_callback(self, *args, **kwargs)
-            if integration is None:
-                return prepared_callback
-
-            # If an integration is there, a client has to be there.
-            client = hub.client  # type: Any
 
             def wrapped_callback(*args, **kwargs):
                 # type: (*object, **object) -> Any
 
                 try:
                     res = prepared_callback(*args, **kwargs)
                 except HTTPResponse:
                     raise
                 except Exception as exception:
                     event, hint = event_from_exception(
                         exception,
                         client_options=client.options,
                         mechanism={"type": "bottle", "handled": False},
                     )
-                    hub.capture_event(event, hint=hint)
+                    sentry_sdk.capture_event(event, hint=hint)
                     raise exception
 
                 return res
 
             return wrapped_callback
 
         Route._make_callback = patched_make_callback
```

### Comparing `sentry-sdk-2.0.0rc3/sentry_sdk/integrations/chalice.py` & `sentry-sdk-2.0.0rc4/sentry_sdk/integrations/chalice.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import sys
 from functools import wraps
 
-from sentry_sdk.hub import Hub
+import sentry_sdk
 from sentry_sdk.integrations import Integration, DidNotEnable
 from sentry_sdk.integrations.aws_lambda import _make_request_event_processor
 from sentry_sdk.tracing import TRANSACTION_SOURCE_COMPONENT
 from sentry_sdk.utils import (
     capture_internal_exceptions,
     event_from_exception,
     parse_version,
@@ -29,45 +29,43 @@
 
     F = TypeVar("F", bound=Callable[..., Any])
 
 
 class EventSourceHandler(ChaliceEventSourceHandler):  # type: ignore
     def __call__(self, event, context):
         # type: (Any, Any) -> Any
-        hub = Hub.current
-        client = hub.client  # type: Any
+        client = sentry_sdk.get_client()
 
-        with hub.push_scope() as scope:
+        with sentry_sdk.isolation_scope() as scope:
             with capture_internal_exceptions():
                 configured_time = context.get_remaining_time_in_millis()
                 scope.add_event_processor(
                     _make_request_event_processor(event, context, configured_time)
                 )
             try:
                 return ChaliceEventSourceHandler.__call__(self, event, context)
             except Exception:
                 exc_info = sys.exc_info()
                 event, hint = event_from_exception(
                     exc_info,
                     client_options=client.options,
                     mechanism={"type": "chalice", "handled": False},
                 )
-                hub.capture_event(event, hint=hint)
-                hub.flush()
+                sentry_sdk.capture_event(event, hint=hint)
+                client.flush()
                 reraise(*exc_info)
 
 
 def _get_view_function_response(app, view_function, function_args):
     # type: (Any, F, Any) -> F
     @wraps(view_function)
     def wrapped_view_function(**function_args):
         # type: (**Any) -> Any
-        hub = Hub.current
-        client = hub.client  # type: Any
-        with hub.push_scope() as scope:
+        client = sentry_sdk.get_client()
+        with sentry_sdk.isolation_scope() as scope:
             with capture_internal_exceptions():
                 configured_time = app.lambda_context.get_remaining_time_in_millis()
                 scope.set_transaction_name(
                     app.lambda_context.function_name,
                     source=TRANSACTION_SOURCE_COMPONENT,
                 )
 
@@ -85,16 +83,16 @@
                     raise
                 exc_info = sys.exc_info()
                 event, hint = event_from_exception(
                     exc_info,
                     client_options=client.options,
                     mechanism={"type": "chalice", "handled": False},
                 )
-                hub.capture_event(event, hint=hint)
-                hub.flush()
+                sentry_sdk.capture_event(event, hint=hint)
+                client.flush()
                 raise
 
     return wrapped_view_function  # type: ignore
 
 
 class ChaliceIntegration(Integration):
     identifier = "chalice"
```

### Comparing `sentry-sdk-2.0.0rc3/sentry_sdk/integrations/clickhouse_driver.py` & `sentry-sdk-2.0.0rc4/sentry_sdk/integrations/clickhouse_driver.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-from sentry_sdk import Hub
+import sentry_sdk
 from sentry_sdk.consts import OP, SPANDATA
-from sentry_sdk.hub import _should_send_default_pii
 from sentry_sdk.integrations import Integration, DidNotEnable
 from sentry_sdk.tracing import Span
 from sentry_sdk._types import TYPE_CHECKING
-from sentry_sdk.utils import capture_internal_exceptions
+from sentry_sdk.scope import should_send_default_pii
+from sentry_sdk.utils import capture_internal_exceptions, ensure_integration_enabled
 
 from typing import TypeVar
 
 # Hack to get new Python features working in older versions
 # without introducing a hard dependency on `typing_extensions`
 # from: https://stackoverflow.com/a/71944042/300572
 if TYPE_CHECKING:
@@ -70,35 +70,33 @@
 
 
 P = ParamSpec("P")
 T = TypeVar("T")
 
 
 def _wrap_start(f: Callable[P, T]) -> Callable[P, T]:
+    @ensure_integration_enabled(ClickhouseDriverIntegration, f)
     def _inner(*args: P.args, **kwargs: P.kwargs) -> T:
-        hub = Hub.current
-        if hub.get_integration(ClickhouseDriverIntegration) is None:
-            return f(*args, **kwargs)
         connection = args[0]
         query = args[1]
         query_id = args[2] if len(args) > 2 else kwargs.get("query_id")
         params = args[3] if len(args) > 3 else kwargs.get("params")
 
-        span = hub.start_span(op=OP.DB, description=query)
+        span = sentry_sdk.start_span(op=OP.DB, description=query)
 
         connection._sentry_span = span  # type: ignore[attr-defined]
 
         _set_db_data(span, connection)
 
         span.set_data("query", query)
 
         if query_id:
             span.set_data("db.query_id", query_id)
 
-        if params and _should_send_default_pii():
+        if params and should_send_default_pii():
             span.set_data("db.params", params)
 
         # run the original code
         ret = f(*args, **kwargs)
 
         return ret
 
@@ -108,15 +106,15 @@
 def _wrap_end(f: Callable[P, T]) -> Callable[P, T]:
     def _inner_end(*args: P.args, **kwargs: P.kwargs) -> T:
         res = f(*args, **kwargs)
         instance = args[0]
         span = instance.connection._sentry_span  # type: ignore[attr-defined]
 
         if span is not None:
-            if res is not None and _should_send_default_pii():
+            if res is not None and should_send_default_pii():
                 span.set_data("db.result", res)
 
             with capture_internal_exceptions():
                 span.scope.add_breadcrumb(
                     message=span._data.pop("query"), category="query", data=span._data
                 )
 
@@ -131,15 +129,15 @@
     def _inner_send_data(*args: P.args, **kwargs: P.kwargs) -> T:
         instance = args[0]  # type: clickhouse_driver.client.Client
         data = args[2]
         span = instance.connection._sentry_span
 
         _set_db_data(span, instance.connection)
 
-        if _should_send_default_pii():
+        if should_send_default_pii():
             db_params = span._data.get("db.params", [])
             db_params.extend(data)
             span.set_data("db.params", db_params)
 
         return f(*args, **kwargs)
 
     return _inner_send_data
```

### Comparing `sentry-sdk-2.0.0rc3/sentry_sdk/integrations/cloud_resource_context.py` & `sentry-sdk-2.0.0rc4/sentry_sdk/integrations/cloud_resource_context.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc3/sentry_sdk/integrations/dedupe.py` & `sentry-sdk-2.0.0rc4/sentry_sdk/integrations/dedupe.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc3/sentry_sdk/integrations/django/__init__.py` & `sentry-sdk-2.0.0rc4/sentry_sdk/integrations/django/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -388,21 +388,19 @@
                 scope.transaction = transaction_from_function(
                     getattr(handler, "view_class", handler)
                 )
     except Exception:
         pass
 
 
+@ensure_integration_enabled(DjangoIntegration)
 def _before_get_response(request):
     # type: (WSGIRequest) -> None
     integration = sentry_sdk.get_client().get_integration(DjangoIntegration)
 
-    if integration is None:
-        return
-
     _patch_drf()
 
     scope = Scope.get_current_scope()
     # Rely on WSGI middleware to start a trace
     _set_transaction_name_and_source(scope, integration.transaction_style, request)
 
     scope.add_event_processor(
@@ -419,18 +417,19 @@
     """
     if not hasattr(request, "urlconf"):
         return
 
     _set_transaction_name_and_source(scope, transaction_style, request)
 
 
+@ensure_integration_enabled(DjangoIntegration)
 def _after_get_response(request):
     # type: (WSGIRequest) -> None
     integration = sentry_sdk.get_client().get_integration(DjangoIntegration)
-    if integration is None or integration.transaction_style != "url":
+    if integration.transaction_style != "url":
         return
 
     scope = Scope.get_current_scope()
     _attempt_resolve_again(request, scope, integration.transaction_style)
 
 
 def _patch_get_response():
@@ -488,29 +487,30 @@
                 _set_user_info(request, event)
 
         return event
 
     return wsgi_request_event_processor
 
 
+@ensure_integration_enabled(DjangoIntegration)
 def _got_request_exception(request=None, **kwargs):
     # type: (WSGIRequest, **Any) -> None
     client = sentry_sdk.get_client()
     integration = client.get_integration(DjangoIntegration)
-    if integration is not None:
-        if request is not None and integration.transaction_style == "url":
-            scope = Scope.get_current_scope()
-            _attempt_resolve_again(request, scope, integration.transaction_style)
-
-        event, hint = event_from_exception(
-            sys.exc_info(),
-            client_options=client.options,
-            mechanism={"type": "django", "handled": False},
-        )
-        sentry_sdk.capture_event(event, hint=hint)
+
+    if request is not None and integration.transaction_style == "url":
+        scope = Scope.get_current_scope()
+        _attempt_resolve_again(request, scope, integration.transaction_style)
+
+    event, hint = event_from_exception(
+        sys.exc_info(),
+        client_options=client.options,
+        mechanism={"type": "django", "handled": False},
+    )
+    sentry_sdk.capture_event(event, hint=hint)
 
 
 class DjangoRequestExtractor(RequestExtractor):
     def env(self):
         # type: () -> Dict[str, str]
         return self.request.META
```

### Comparing `sentry-sdk-2.0.0rc3/sentry_sdk/integrations/django/asgi.py` & `sentry-sdk-2.0.0rc4/sentry_sdk/integrations/django/asgi.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc3/sentry_sdk/integrations/django/caching.py` & `sentry-sdk-2.0.0rc4/sentry_sdk/integrations/django/caching.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc3/sentry_sdk/integrations/django/middleware.py` & `sentry-sdk-2.0.0rc4/sentry_sdk/integrations/django/middleware.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc3/sentry_sdk/integrations/django/signals_handlers.py` & `sentry-sdk-2.0.0rc4/sentry_sdk/integrations/django/signals_handlers.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc3/sentry_sdk/integrations/django/templates.py` & `sentry-sdk-2.0.0rc4/sentry_sdk/integrations/django/templates.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,19 +61,17 @@
     # type: () -> None
     from django.template.response import SimpleTemplateResponse
     from sentry_sdk.integrations.django import DjangoIntegration
 
     real_rendered_content = SimpleTemplateResponse.rendered_content
 
     @property  # type: ignore
+    @ensure_integration_enabled(DjangoIntegration, real_rendered_content.fget)
     def rendered_content(self):
         # type: (SimpleTemplateResponse) -> str
-        if sentry_sdk.get_client().get_integration(DjangoIntegration) is None:
-            return real_rendered_content.fget(self)
-
         with sentry_sdk.start_span(
             op=OP.TEMPLATE_RENDER,
             description=_get_template_name_description(self.template_name),
         ) as span:
             span.set_data("context", self.context_data)
             return real_rendered_content.fget(self)
```

### Comparing `sentry-sdk-2.0.0rc3/sentry_sdk/integrations/django/transactions.py` & `sentry-sdk-2.0.0rc4/sentry_sdk/integrations/django/transactions.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc3/sentry_sdk/integrations/django/views.py` & `sentry-sdk-2.0.0rc4/sentry_sdk/integrations/django/views.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc3/sentry_sdk/integrations/excepthook.py` & `sentry-sdk-2.0.0rc4/sentry_sdk/integrations/excepthook.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 import sys
 
 import sentry_sdk
-from sentry_sdk.utils import capture_internal_exceptions, event_from_exception
+from sentry_sdk.utils import (
+    capture_internal_exceptions,
+    ensure_integration_enabled,
+    event_from_exception,
+)
 from sentry_sdk.integrations import Integration
 
 from sentry_sdk._types import TYPE_CHECKING
 
 if TYPE_CHECKING:
     from typing import Callable
     from typing import Any
@@ -39,19 +43,20 @@
     def setup_once():
         # type: () -> None
         sys.excepthook = _make_excepthook(sys.excepthook)
 
 
 def _make_excepthook(old_excepthook):
     # type: (Excepthook) -> Excepthook
+    @ensure_integration_enabled(ExcepthookIntegration, old_excepthook)
     def sentry_sdk_excepthook(type_, value, traceback):
         # type: (Type[BaseException], BaseException, Optional[TracebackType]) -> None
         integration = sentry_sdk.get_client().get_integration(ExcepthookIntegration)
 
-        if integration is not None and _should_send(integration.always_run):
+        if _should_send(integration.always_run):
             with capture_internal_exceptions():
                 event, hint = event_from_exception(
                     (type_, value, traceback),
                     client_options=sentry_sdk.get_client().options,
                     mechanism={"type": "excepthook", "handled": False},
                 )
                 sentry_sdk.capture_event(event, hint=hint)
```

### Comparing `sentry-sdk-2.0.0rc3/sentry_sdk/integrations/executing.py` & `sentry-sdk-2.0.0rc4/sentry_sdk/integrations/executing.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from sentry_sdk import Hub
+import sentry_sdk
 from sentry_sdk._types import TYPE_CHECKING
 from sentry_sdk.integrations import Integration, DidNotEnable
 from sentry_sdk.scope import add_global_event_processor
 from sentry_sdk.utils import walk_exception_chain, iter_stacks
 
 if TYPE_CHECKING:
     from typing import Optional
@@ -21,15 +21,15 @@
     @staticmethod
     def setup_once():
         # type: () -> None
 
         @add_global_event_processor
         def add_executing_info(event, hint):
             # type: (Event, Optional[Hint]) -> Optional[Event]
-            if Hub.current.get_integration(ExecutingIntegration) is None:
+            if sentry_sdk.get_client().get_integration(ExecutingIntegration) is None:
                 return event
 
             if hint is None:
                 return event
 
             exc_info = hint.get("exc_info", None)
```

### Comparing `sentry-sdk-2.0.0rc3/sentry_sdk/integrations/falcon.py` & `sentry-sdk-2.0.0rc4/sentry_sdk/integrations/falcon.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,16 @@
-from sentry_sdk.hub import Hub
+import sentry_sdk
 from sentry_sdk.integrations import Integration, DidNotEnable
 from sentry_sdk.integrations._wsgi_common import RequestExtractor
 from sentry_sdk.integrations.wsgi import SentryWsgiMiddleware
+from sentry_sdk.scope import Scope
 from sentry_sdk.tracing import SOURCE_FOR_STYLE
 from sentry_sdk.utils import (
     capture_internal_exceptions,
+    ensure_integration_enabled,
     event_from_exception,
     parse_version,
 )
 
 from sentry_sdk._types import TYPE_CHECKING
 
 if TYPE_CHECKING:
@@ -96,22 +98,21 @@
 
 
 class SentryFalconMiddleware:
     """Captures exceptions in Falcon requests and send to Sentry"""
 
     def process_request(self, req, resp, *args, **kwargs):
         # type: (Any, Any, *Any, **Any) -> None
-        hub = Hub.current
-        integration = hub.get_integration(FalconIntegration)
+        integration = sentry_sdk.get_client().get_integration(FalconIntegration)
         if integration is None:
             return
 
-        with hub.configure_scope() as scope:
-            scope._name = "falcon"
-            scope.add_event_processor(_make_request_event_processor(req, integration))
+        scope = Scope.get_isolation_scope()
+        scope._name = "falcon"
+        scope.add_event_processor(_make_request_event_processor(req, integration))
 
 
 TRANSACTION_STYLE_VALUES = ("uri_template", "path")
 
 
 class FalconIntegration(Integration):
     identifier = "falcon"
@@ -146,16 +147,15 @@
 
 def _patch_wsgi_app():
     # type: () -> None
     original_wsgi_app = falcon_app_class.__call__
 
     def sentry_patched_wsgi_app(self, env, start_response):
         # type: (falcon.API, Any, Any) -> Any
-        hub = Hub.current
-        integration = hub.get_integration(FalconIntegration)
+        integration = sentry_sdk.get_client().get_integration(FalconIntegration)
         if integration is None:
             return original_wsgi_app(self, env, start_response)
 
         sentry_wrapped = SentryWsgiMiddleware(
             lambda envi, start_resp: original_wsgi_app(self, envi, start_resp)
         )
 
@@ -164,14 +164,15 @@
     falcon_app_class.__call__ = sentry_patched_wsgi_app
 
 
 def _patch_handle_exception():
     # type: () -> None
     original_handle_exception = falcon_app_class._handle_exception
 
+    @ensure_integration_enabled(FalconIntegration, original_handle_exception)
     def sentry_patched_handle_exception(self, *args):
         # type: (falcon.API, *Any) -> Any
         # NOTE(jmagnusson): falcon 2.0 changed falcon.API._handle_exception
         # method signature from `(ex, req, resp, params)` to
         # `(req, resp, ex, params)`
         ex = response = None
         with capture_internal_exceptions():
@@ -184,27 +185,21 @@
 
         if ex is None or response is None:
             # Both ex and response should have a non-None value at this point; otherwise,
             # there is an error with the SDK that will have been captured in the
             # capture_internal_exceptions block above.
             return was_handled
 
-        hub = Hub.current
-        integration = hub.get_integration(FalconIntegration)
-
-        if integration is not None and _exception_leads_to_http_5xx(ex, response):
-            # If an integration is there, a client has to be there.
-            client = hub.client  # type: Any
-
+        if _exception_leads_to_http_5xx(ex, response):
             event, hint = event_from_exception(
                 ex,
-                client_options=client.options,
+                client_options=sentry_sdk.get_client().options,
                 mechanism={"type": "falcon", "handled": False},
             )
-            hub.capture_event(event, hint=hint)
+            sentry_sdk.capture_event(event, hint=hint)
 
         return was_handled
 
     falcon_app_class._handle_exception = sentry_patched_handle_exception
 
 
 def _patch_prepare_middleware():
@@ -215,16 +210,15 @@
         middleware=None, independent_middleware=False, asgi=False
     ):
         # type: (Any, Any, bool) -> Any
         if asgi:
             # We don't support ASGI Falcon apps, so we don't patch anything here
             return original_prepare_middleware(middleware, independent_middleware, asgi)
 
-        hub = Hub.current
-        integration = hub.get_integration(FalconIntegration)
+        integration = sentry_sdk.get_client().get_integration(FalconIntegration)
         if integration is not None:
             middleware = [SentryFalconMiddleware()] + (middleware or [])
 
         # We intentionally omit the asgi argument here, since the default is False anyways,
         # and this way, we remain backwards-compatible with pre-3.0.0 Falcon versions.
         return original_prepare_middleware(middleware, independent_middleware)
```

### Comparing `sentry-sdk-2.0.0rc3/sentry_sdk/integrations/fastapi.py` & `sentry-sdk-2.0.0rc4/sentry_sdk/integrations/fastapi.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc3/sentry_sdk/integrations/flask.py` & `sentry-sdk-2.0.0rc4/sentry_sdk/integrations/flask.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,17 @@
+import sentry_sdk
 from sentry_sdk._types import TYPE_CHECKING
-from sentry_sdk.hub import Hub, _should_send_default_pii
 from sentry_sdk.integrations import DidNotEnable, Integration
 from sentry_sdk.integrations._wsgi_common import RequestExtractor
 from sentry_sdk.integrations.wsgi import SentryWsgiMiddleware
-from sentry_sdk.scope import Scope
+from sentry_sdk.scope import Scope, should_send_default_pii
 from sentry_sdk.tracing import SOURCE_FOR_STYLE
 from sentry_sdk.utils import (
     capture_internal_exceptions,
+    ensure_integration_enabled,
     event_from_exception,
     package_version,
 )
 
 if TYPE_CHECKING:
     from typing import Any, Callable, Dict, Union
 
@@ -73,31 +74,31 @@
         request_started.connect(_request_started)
         got_request_exception.connect(_capture_exception)
 
         old_app = Flask.__call__
 
         def sentry_patched_wsgi_app(self, environ, start_response):
             # type: (Any, Dict[str, str], Callable[..., Any]) -> _ScopedResponse
-            if Hub.current.get_integration(FlaskIntegration) is None:
+            if sentry_sdk.get_client().get_integration(FlaskIntegration) is None:
                 return old_app(self, environ, start_response)
 
             return SentryWsgiMiddleware(lambda *a, **kw: old_app(self, *a, **kw))(
                 environ, start_response
             )
 
         Flask.__call__ = sentry_patched_wsgi_app
 
 
 def _add_sentry_trace(sender, template, context, **extra):
     # type: (Flask, Any, Dict[str, Any], **Any) -> None
     if "sentry_trace" in context:
         return
 
-    hub = Hub.current
-    trace_meta = Markup(hub.trace_propagation_meta())
+    scope = Scope.get_current_scope()
+    trace_meta = Markup(scope.trace_propagation_meta())
     context["sentry_trace"] = trace_meta  # for backwards compatibility
     context["sentry_trace_meta"] = trace_meta
 
 
 def _set_transaction_name_and_source(scope, transaction_style, request):
     # type: (Scope, str, Request) -> None
     try:
@@ -109,32 +110,29 @@
             name_for_style[transaction_style],
             source=SOURCE_FOR_STYLE[transaction_style],
         )
     except Exception:
         pass
 
 
+@ensure_integration_enabled(FlaskIntegration)
 def _request_started(app, **kwargs):
     # type: (Flask, **Any) -> None
-    hub = Hub.current
-    integration = hub.get_integration(FlaskIntegration)
-    if integration is None:
-        return
-
+    integration = sentry_sdk.get_client().get_integration(FlaskIntegration)
     request = flask_request._get_current_object()
 
     # Set the transaction name and source here,
     # but rely on WSGI middleware to actually start the transaction
     _set_transaction_name_and_source(
         Scope.get_current_scope(), integration.transaction_style, request
     )
 
-    with hub.configure_scope() as scope:
-        evt_processor = _make_request_event_processor(app, request, integration)
-        scope.add_event_processor(evt_processor)
+    scope = Scope.get_isolation_scope()
+    evt_processor = _make_request_event_processor(app, request, integration)
+    scope.add_event_processor(evt_processor)
 
 
 class FlaskRequestExtractor(RequestExtractor):
     def env(self):
         # type: () -> Dict[str, str]
         return self.request.environ
 
@@ -181,39 +179,33 @@
         # another thread.
         if request is None:
             return event
 
         with capture_internal_exceptions():
             FlaskRequestExtractor(request).extract_into_event(event)
 
-        if _should_send_default_pii():
+        if should_send_default_pii():
             with capture_internal_exceptions():
                 _add_user_to_event(event)
 
         return event
 
     return inner
 
 
+@ensure_integration_enabled(FlaskIntegration)
 def _capture_exception(sender, exception, **kwargs):
     # type: (Flask, Union[ValueError, BaseException], **Any) -> None
-    hub = Hub.current
-    if hub.get_integration(FlaskIntegration) is None:
-        return
-
-    # If an integration is there, a client has to be there.
-    client = hub.client  # type: Any
-
     event, hint = event_from_exception(
         exception,
-        client_options=client.options,
+        client_options=sentry_sdk.get_client().options,
         mechanism={"type": "flask", "handled": False},
     )
 
-    hub.capture_event(event, hint=hint)
+    sentry_sdk.capture_event(event, hint=hint)
 
 
 def _add_user_to_event(event):
     # type: (Event) -> None
     if flask_login is None:
         return
```

### Comparing `sentry-sdk-2.0.0rc3/sentry_sdk/integrations/gcp.py` & `sentry-sdk-2.0.0rc4/sentry_sdk/integrations/gcp.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 import sys
 from copy import deepcopy
 from datetime import datetime, timedelta, timezone
 from os import environ
 
+import sentry_sdk
 from sentry_sdk.api import continue_trace
 from sentry_sdk.consts import OP
-from sentry_sdk.hub import Hub, _should_send_default_pii
+from sentry_sdk.integrations import Integration
+from sentry_sdk.integrations._wsgi_common import _filter_headers
+from sentry_sdk.scope import should_send_default_pii
 from sentry_sdk.tracing import TRANSACTION_SOURCE_COMPONENT
 from sentry_sdk.utils import (
     AnnotatedValue,
     capture_internal_exceptions,
+    ensure_integration_enabled,
     event_from_exception,
     logger,
     TimeoutThread,
     reraise,
 )
-from sentry_sdk.integrations import Integration
-from sentry_sdk.integrations._wsgi_common import _filter_headers
 
 from sentry_sdk._types import TYPE_CHECKING
 
 # Constants
 TIMEOUT_WARNING_BUFFER = 1.5  # Buffer time required to send timeout warning to Sentry
 MILLIS_TO_SECONDS = 1000.0
 
@@ -33,37 +35,33 @@
     from sentry_sdk._types import EventProcessor, Event, Hint
 
     F = TypeVar("F", bound=Callable[..., Any])
 
 
 def _wrap_func(func):
     # type: (F) -> F
+    @ensure_integration_enabled(GcpIntegration, func)
     def sentry_func(functionhandler, gcp_event, *args, **kwargs):
         # type: (Any, Any, *Any, **Any) -> Any
+        client = sentry_sdk.get_client()
 
-        hub = Hub.current
-        integration = hub.get_integration(GcpIntegration)
-        if integration is None:
-            return func(functionhandler, gcp_event, *args, **kwargs)
-
-        # If an integration is there, a client has to be there.
-        client = hub.client  # type: Any
+        integration = client.get_integration(GcpIntegration)
 
         configured_time = environ.get("FUNCTION_TIMEOUT_SEC")
         if not configured_time:
             logger.debug(
                 "The configured timeout could not be fetched from Cloud Functions configuration."
             )
             return func(functionhandler, gcp_event, *args, **kwargs)
 
         configured_time = int(configured_time)
 
         initial_time = datetime.now(timezone.utc)
 
-        with hub.push_scope() as scope:
+        with sentry_sdk.isolation_scope() as scope:
             with capture_internal_exceptions():
                 scope.clear_breadcrumbs()
                 scope.add_event_processor(
                     _make_request_event_processor(
                         gcp_event, configured_time, initial_time
                     )
                 )
@@ -96,33 +94,33 @@
                     "function_entry_point": environ.get("ENTRY_POINT"),
                     "function_identity": environ.get("FUNCTION_IDENTITY"),
                     "function_region": environ.get("FUNCTION_REGION"),
                     "function_project": environ.get("GCP_PROJECT"),
                 },
                 "gcp_event": gcp_event,
             }
-            with hub.start_transaction(
+            with sentry_sdk.start_transaction(
                 transaction, custom_sampling_context=sampling_context
             ):
                 try:
                     return func(functionhandler, gcp_event, *args, **kwargs)
                 except Exception:
                     exc_info = sys.exc_info()
                     sentry_event, hint = event_from_exception(
                         exc_info,
                         client_options=client.options,
                         mechanism={"type": "gcp", "handled": False},
                     )
-                    hub.capture_event(sentry_event, hint=hint)
+                    sentry_sdk.capture_event(sentry_event, hint=hint)
                     reraise(*exc_info)
                 finally:
                     if timeout_thread:
                         timeout_thread.stop()
                     # Flush out the event queue
-                    hub.flush()
+                    client.flush()
 
     return sentry_func  # type: ignore
 
 
 class GcpIntegration(Integration):
     identifier = "gcp"
 
@@ -183,15 +181,15 @@
 
         if hasattr(gcp_event, "query_string"):
             request["query_string"] = gcp_event.query_string.decode("utf-8")
 
         if hasattr(gcp_event, "headers"):
             request["headers"] = _filter_headers(gcp_event.headers)
 
-        if _should_send_default_pii():
+        if should_send_default_pii():
             if hasattr(gcp_event, "data"):
                 request["data"] = gcp_event.data
         else:
             if hasattr(gcp_event, "data"):
                 # Unfortunately couldn't find a way to get structured body from GCP
                 # event. Meaning every body is unstructured to us.
                 request["data"] = AnnotatedValue.removed_because_raw_data()
```

### Comparing `sentry-sdk-2.0.0rc3/sentry_sdk/integrations/gnu_backtrace.py` & `sentry-sdk-2.0.0rc4/sentry_sdk/integrations/gnu_backtrace.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc3/sentry_sdk/integrations/gql.py` & `sentry-sdk-2.0.0rc4/sentry_sdk/integrations/gql.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc3/sentry_sdk/integrations/graphene.py` & `sentry-sdk-2.0.0rc4/sentry_sdk/integrations/graphene.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,14 @@
-from sentry_sdk.hub import Hub, _should_send_default_pii
+import sentry_sdk
 from sentry_sdk.integrations import DidNotEnable, Integration
+from sentry_sdk.scope import Scope, should_send_default_pii
 from sentry_sdk.utils import (
     capture_internal_exceptions,
+    ensure_integration_enabled,
+    ensure_integration_enabled_async,
     event_from_exception,
     package_version,
 )
 from sentry_sdk._types import TYPE_CHECKING
 
 
 try:
@@ -40,73 +43,65 @@
 
 
 def _patch_graphql():
     # type: () -> None
     old_graphql_sync = graphene_schema.graphql_sync
     old_graphql_async = graphene_schema.graphql
 
+    @ensure_integration_enabled(GrapheneIntegration, old_graphql_sync)
     def _sentry_patched_graphql_sync(schema, source, *args, **kwargs):
         # type: (GraphQLSchema, Union[str, Source], Any, Any) -> ExecutionResult
-        hub = Hub.current
-        integration = hub.get_integration(GrapheneIntegration)
-        if integration is None:
-            return old_graphql_sync(schema, source, *args, **kwargs)
-
-        with hub.configure_scope() as scope:
-            scope.add_event_processor(_event_processor)
+        scope = Scope.get_isolation_scope()
+        scope.add_event_processor(_event_processor)
 
         result = old_graphql_sync(schema, source, *args, **kwargs)
 
         with capture_internal_exceptions():
             for error in result.errors or []:
                 event, hint = event_from_exception(
                     error,
-                    client_options=hub.client.options if hub.client else None,
+                    client_options=sentry_sdk.get_client().options,
                     mechanism={
-                        "type": integration.identifier,
+                        "type": GrapheneIntegration.identifier,
                         "handled": False,
                     },
                 )
-                hub.capture_event(event, hint=hint)
+                sentry_sdk.capture_event(event, hint=hint)
 
         return result
 
+    @ensure_integration_enabled_async(GrapheneIntegration, old_graphql_async)
     async def _sentry_patched_graphql_async(schema, source, *args, **kwargs):
         # type: (GraphQLSchema, Union[str, Source], Any, Any) -> ExecutionResult
-        hub = Hub.current
-        integration = hub.get_integration(GrapheneIntegration)
-        if integration is None:
-            return await old_graphql_async(schema, source, *args, **kwargs)
-
-        with hub.configure_scope() as scope:
-            scope.add_event_processor(_event_processor)
+        scope = Scope.get_isolation_scope()
+        scope.add_event_processor(_event_processor)
 
         result = await old_graphql_async(schema, source, *args, **kwargs)
 
         with capture_internal_exceptions():
             for error in result.errors or []:
                 event, hint = event_from_exception(
                     error,
-                    client_options=hub.client.options if hub.client else None,
+                    client_options=sentry_sdk.get_client().options,
                     mechanism={
-                        "type": integration.identifier,
+                        "type": GrapheneIntegration.identifier,
                         "handled": False,
                     },
                 )
-                hub.capture_event(event, hint=hint)
+                sentry_sdk.capture_event(event, hint=hint)
 
         return result
 
     graphene_schema.graphql_sync = _sentry_patched_graphql_sync
     graphene_schema.graphql = _sentry_patched_graphql_async
 
 
 def _event_processor(event, hint):
     # type: (Event, Dict[str, Any]) -> Event
-    if _should_send_default_pii():
+    if should_send_default_pii():
         request_info = event.setdefault("request", {})
         request_info["api_target"] = "graphql"
 
     elif event.get("request", {}).get("data"):
         del event["request"]["data"]
 
     return event
```

### Comparing `sentry-sdk-2.0.0rc3/sentry_sdk/integrations/grpc/__init__.py` & `sentry-sdk-2.0.0rc4/sentry_sdk/integrations/grpc/__init__.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc3/sentry_sdk/integrations/grpc/aio/client.py` & `sentry-sdk-2.0.0rc4/sentry_sdk/integrations/grpc/aio/client.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,27 +5,28 @@
     UnaryStreamClientInterceptor,
     ClientCallDetails,
     UnaryUnaryCall,
     UnaryStreamCall,
 )
 from google.protobuf.message import Message
 
-from sentry_sdk import Hub
+import sentry_sdk
 from sentry_sdk.consts import OP
+from sentry_sdk.scope import Scope
 
 
 class ClientInterceptor:
     @staticmethod
-    def _update_client_call_details_metadata_from_hub(
-        client_call_details: ClientCallDetails, hub: Hub
+    def _update_client_call_details_metadata_from_scope(
+        client_call_details: ClientCallDetails,
     ) -> ClientCallDetails:
         metadata = (
             list(client_call_details.metadata) if client_call_details.metadata else []
         )
-        for key, value in hub.iter_trace_propagation_headers():
+        for key, value in Scope.get_current_scope().iter_trace_propagation_headers():
             metadata.append((key, value))
 
         client_call_details = ClientCallDetails(
             method=client_call_details.method,
             timeout=client_call_details.timeout,
             metadata=metadata,
             credentials=client_call_details.credentials,
@@ -38,25 +39,24 @@
 class SentryUnaryUnaryClientInterceptor(ClientInterceptor, UnaryUnaryClientInterceptor):  # type: ignore
     async def intercept_unary_unary(
         self,
         continuation: Callable[[ClientCallDetails, Message], UnaryUnaryCall],
         client_call_details: ClientCallDetails,
         request: Message,
     ) -> Union[UnaryUnaryCall, Message]:
-        hub = Hub.current
         method = client_call_details.method
 
-        with hub.start_span(
+        with sentry_sdk.start_span(
             op=OP.GRPC_CLIENT, description="unary unary call to %s" % method.decode()
         ) as span:
             span.set_data("type", "unary unary")
             span.set_data("method", method)
 
-            client_call_details = self._update_client_call_details_metadata_from_hub(
-                client_call_details, hub
+            client_call_details = self._update_client_call_details_metadata_from_scope(
+                client_call_details
             )
 
             response = await continuation(client_call_details, request)
             status_code = await response.code()
             span.set_data("code", status_code.name)
 
             return response
@@ -67,25 +67,24 @@
 ):
     async def intercept_unary_stream(
         self,
         continuation: Callable[[ClientCallDetails, Message], UnaryStreamCall],
         client_call_details: ClientCallDetails,
         request: Message,
     ) -> Union[AsyncIterable[Any], UnaryStreamCall]:
-        hub = Hub.current
         method = client_call_details.method
 
-        with hub.start_span(
+        with sentry_sdk.start_span(
             op=OP.GRPC_CLIENT, description="unary stream call to %s" % method.decode()
         ) as span:
             span.set_data("type", "unary stream")
             span.set_data("method", method)
 
-            client_call_details = self._update_client_call_details_metadata_from_hub(
-                client_call_details, hub
+            client_call_details = self._update_client_call_details_metadata_from_scope(
+                client_call_details
             )
 
             response = await continuation(client_call_details, request)
             # status_code = await response.code()
             # span.set_data("code", status_code)
 
             return response
```

### Comparing `sentry-sdk-2.0.0rc3/sentry_sdk/integrations/grpc/aio/server.py` & `sentry-sdk-2.0.0rc4/sentry_sdk/integrations/grpc/aio/server.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-from sentry_sdk import Hub
-from sentry_sdk._types import MYPY
+import sentry_sdk
+from sentry_sdk._types import TYPE_CHECKING
 from sentry_sdk.consts import OP
 from sentry_sdk.integrations import DidNotEnable
 from sentry_sdk.tracing import Transaction, TRANSACTION_SOURCE_CUSTOM
 from sentry_sdk.utils import event_from_exception
 
-if MYPY:
+if TYPE_CHECKING:
     from collections.abc import Awaitable, Callable
     from typing import Any
 
 
 try:
     import grpc
     from grpc import HandlerCallDetails, RpcMethodHandler
@@ -35,35 +35,33 @@
 
             async def wrapped(request, context):
                 # type: (Any, ServicerContext) -> Any
                 name = self._find_method_name(context)
                 if not name:
                     return await handler(request, context)
 
-                hub = Hub.current
-
                 # What if the headers are empty?
                 transaction = Transaction.continue_from_headers(
                     dict(context.invocation_metadata()),
                     op=OP.GRPC_SERVER,
                     name=name,
                     source=TRANSACTION_SOURCE_CUSTOM,
                 )
 
-                with hub.start_transaction(transaction=transaction):
+                with sentry_sdk.start_transaction(transaction=transaction):
                     try:
                         return await handler.unary_unary(request, context)
                     except AbortError:
                         raise
                     except Exception as exc:
                         event, hint = event_from_exception(
                             exc,
                             mechanism={"type": "grpc", "handled": False},
                         )
-                        hub.capture_event(event, hint=hint)
+                        sentry_sdk.capture_event(event, hint=hint)
                         raise
 
         elif not handler.request_streaming and handler.response_streaming:
             handler_factory = grpc.unary_stream_rpc_method_handler
 
             async def wrapped(request, context):  # type: ignore
                 # type: (Any, ServicerContext) -> Any
```

### Comparing `sentry-sdk-2.0.0rc3/sentry_sdk/integrations/grpc/client.py` & `sentry-sdk-2.0.0rc4/sentry_sdk/integrations/grpc/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
-from sentry_sdk import Hub
-from sentry_sdk._types import MYPY
+import sentry_sdk
+from sentry_sdk._types import TYPE_CHECKING
 from sentry_sdk.consts import OP
 from sentry_sdk.integrations import DidNotEnable
+from sentry_sdk.scope import Scope
 
-if MYPY:
+if TYPE_CHECKING:
     from typing import Any, Callable, Iterator, Iterable, Union
 
 try:
     import grpc
     from grpc import ClientCallDetails, Call
     from grpc._interceptor import _UnaryOutcome
     from grpc.aio._interceptor import UnaryStreamCall
@@ -19,62 +20,60 @@
 class ClientInterceptor(
     grpc.UnaryUnaryClientInterceptor, grpc.UnaryStreamClientInterceptor  # type: ignore
 ):
     _is_intercepted = False
 
     def intercept_unary_unary(self, continuation, client_call_details, request):
         # type: (ClientInterceptor, Callable[[ClientCallDetails, Message], _UnaryOutcome], ClientCallDetails, Message) -> _UnaryOutcome
-        hub = Hub.current
         method = client_call_details.method
 
-        with hub.start_span(
+        with sentry_sdk.start_span(
             op=OP.GRPC_CLIENT, description="unary unary call to %s" % method
         ) as span:
             span.set_data("type", "unary unary")
             span.set_data("method", method)
 
-            client_call_details = self._update_client_call_details_metadata_from_hub(
-                client_call_details, hub
+            client_call_details = self._update_client_call_details_metadata_from_scope(
+                client_call_details
             )
 
             response = continuation(client_call_details, request)
             span.set_data("code", response.code().name)
 
             return response
 
     def intercept_unary_stream(self, continuation, client_call_details, request):
         # type: (ClientInterceptor, Callable[[ClientCallDetails, Message], Union[Iterable[Any], UnaryStreamCall]], ClientCallDetails, Message) -> Union[Iterator[Message], Call]
-        hub = Hub.current
         method = client_call_details.method
 
-        with hub.start_span(
+        with sentry_sdk.start_span(
             op=OP.GRPC_CLIENT, description="unary stream call to %s" % method
         ) as span:
             span.set_data("type", "unary stream")
             span.set_data("method", method)
 
-            client_call_details = self._update_client_call_details_metadata_from_hub(
-                client_call_details, hub
+            client_call_details = self._update_client_call_details_metadata_from_scope(
+                client_call_details
             )
 
             response = continuation(
                 client_call_details, request
             )  # type: UnaryStreamCall
             # Setting code on unary-stream leads to execution getting stuck
             # span.set_data("code", response.code().name)
 
             return response
 
     @staticmethod
-    def _update_client_call_details_metadata_from_hub(client_call_details, hub):
-        # type: (ClientCallDetails, Hub) -> ClientCallDetails
+    def _update_client_call_details_metadata_from_scope(client_call_details):
+        # type: (ClientCallDetails) -> ClientCallDetails
         metadata = (
             list(client_call_details.metadata) if client_call_details.metadata else []
         )
-        for key, value in hub.iter_trace_propagation_headers():
+        for key, value in Scope.get_current_scope().iter_trace_propagation_headers():
             metadata.append((key, value))
 
         client_call_details = grpc._interceptor._ClientCallDetails(
             method=client_call_details.method,
             timeout=client_call_details.timeout,
             metadata=metadata,
             credentials=client_call_details.credentials,
```

### Comparing `sentry-sdk-2.0.0rc3/sentry_sdk/integrations/grpc/server.py` & `sentry-sdk-2.0.0rc4/sentry_sdk/integrations/grpc/server.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-from sentry_sdk import Hub
-from sentry_sdk._types import MYPY
+import sentry_sdk
+from sentry_sdk._types import TYPE_CHECKING
 from sentry_sdk.consts import OP
 from sentry_sdk.integrations import DidNotEnable
 from sentry_sdk.tracing import Transaction, TRANSACTION_SOURCE_CUSTOM
 
-if MYPY:
+if TYPE_CHECKING:
     from typing import Callable, Optional
     from google.protobuf.message import Message
 
 try:
     import grpc
     from grpc import ServicerContext, HandlerCallDetails, RpcMethodHandler
 except ImportError:
@@ -26,35 +26,34 @@
         # type: (ServerInterceptor, Callable[[HandlerCallDetails], RpcMethodHandler], HandlerCallDetails) -> RpcMethodHandler
         handler = continuation(handler_call_details)
         if not handler or not handler.unary_unary:
             return handler
 
         def behavior(request, context):
             # type: (Message, ServicerContext) -> Message
-            hub = Hub(Hub.current)
+            with sentry_sdk.isolation_scope():
+                name = self._find_method_name(context)
 
-            name = self._find_method_name(context)
+                if name:
+                    metadata = dict(context.invocation_metadata())
 
-            if name:
-                metadata = dict(context.invocation_metadata())
-
-                transaction = Transaction.continue_from_headers(
-                    metadata,
-                    op=OP.GRPC_SERVER,
-                    name=name,
-                    source=TRANSACTION_SOURCE_CUSTOM,
-                )
-
-                with hub.start_transaction(transaction=transaction):
-                    try:
-                        return handler.unary_unary(request, context)
-                    except BaseException as e:
-                        raise e
-            else:
-                return handler.unary_unary(request, context)
+                    transaction = Transaction.continue_from_headers(
+                        metadata,
+                        op=OP.GRPC_SERVER,
+                        name=name,
+                        source=TRANSACTION_SOURCE_CUSTOM,
+                    )
+
+                    with sentry_sdk.start_transaction(transaction=transaction):
+                        try:
+                            return handler.unary_unary(request, context)
+                        except BaseException as e:
+                            raise e
+                else:
+                    return handler.unary_unary(request, context)
 
         return grpc.unary_unary_rpc_method_handler(
             behavior,
             request_deserializer=handler.request_deserializer,
             response_serializer=handler.response_serializer,
         )
```

### Comparing `sentry-sdk-2.0.0rc3/sentry_sdk/integrations/httpx.py` & `sentry-sdk-2.0.0rc4/sentry_sdk/integrations/httpx.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc3/sentry_sdk/integrations/huey.py` & `sentry-sdk-2.0.0rc4/sentry_sdk/integrations/huey.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import sys
 from datetime import datetime
 
+import sentry_sdk
 from sentry_sdk._types import TYPE_CHECKING
-from sentry_sdk import Hub
 from sentry_sdk.api import continue_trace, get_baggage, get_traceparent
 from sentry_sdk.consts import OP
-from sentry_sdk.hub import _should_send_default_pii
 from sentry_sdk.integrations import DidNotEnable, Integration
+from sentry_sdk.scope import Scope, should_send_default_pii
 from sentry_sdk.tracing import (
     BAGGAGE_HEADER_NAME,
     SENTRY_TRACE_HEADER_NAME,
     TRANSACTION_SOURCE_TASK,
 )
-from sentry_sdk.scope import Scope
 from sentry_sdk.utils import (
     capture_internal_exceptions,
+    ensure_integration_enabled,
     event_from_exception,
     SENSITIVE_DATA_SUBSTITUTE,
     reraise,
 )
 
 if TYPE_CHECKING:
     from typing import Any, Callable, Optional, Union, TypeVar
@@ -48,22 +48,18 @@
         patch_execute()
 
 
 def patch_enqueue():
     # type: () -> None
     old_enqueue = Huey.enqueue
 
+    @ensure_integration_enabled(HueyIntegration, old_enqueue)
     def _sentry_enqueue(self, task):
         # type: (Huey, Task) -> Optional[Union[Result, ResultGroup]]
-        hub = Hub.current
-
-        if hub.get_integration(HueyIntegration) is None:
-            return old_enqueue(self, task)
-
-        with hub.start_span(op=OP.QUEUE_SUBMIT_HUEY, description=task.name):
+        with sentry_sdk.start_span(op=OP.QUEUE_SUBMIT_HUEY, description=task.name):
             if not isinstance(task, PeriodicTask):
                 # Attach trace propagation data to task kwargs. We do
                 # not do this for periodic tasks, as these don't
                 # really have an originating transaction.
                 task.kwargs["sentry_headers"] = {
                     BAGGAGE_HEADER_NAME: get_baggage(),
                     SENTRY_TRACE_HEADER_NAME: get_traceparent(),
@@ -83,20 +79,20 @@
             tags["huey_task_id"] = task.id
             tags["huey_task_retry"] = task.default_retries > task.retries
             extra = event.setdefault("extra", {})
             extra["huey-job"] = {
                 "task": task.name,
                 "args": (
                     task.args
-                    if _should_send_default_pii()
+                    if should_send_default_pii()
                     else SENSITIVE_DATA_SUBSTITUTE
                 ),
                 "kwargs": (
                     task.kwargs
-                    if _should_send_default_pii()
+                    if should_send_default_pii()
                     else SENSITIVE_DATA_SUBSTITUTE
                 ),
                 "retry": (task.default_retries or 0) - task.retries,
             }
 
         return event
 
@@ -118,20 +114,18 @@
         mechanism={"type": HueyIntegration.identifier, "handled": False},
     )
     scope.capture_event(event, hint=hint)
 
 
 def _wrap_task_execute(func):
     # type: (F) -> F
+
+    @ensure_integration_enabled(HueyIntegration, func)
     def _sentry_execute(*args, **kwargs):
         # type: (*Any, **Any) -> Any
-        hub = Hub.current
-        if hub.get_integration(HueyIntegration) is None:
-            return func(*args, **kwargs)
-
         try:
             result = func(*args, **kwargs)
         except Exception:
             exc_info = sys.exc_info()
             _capture_exception(exc_info)
             reraise(*exc_info)
 
@@ -140,22 +134,18 @@
     return _sentry_execute  # type: ignore
 
 
 def patch_execute():
     # type: () -> None
     old_execute = Huey._execute
 
+    @ensure_integration_enabled(HueyIntegration, old_execute)
     def _sentry_execute(self, task, timestamp=None):
         # type: (Huey, Task, Optional[datetime]) -> Any
-        hub = Hub.current
-
-        if hub.get_integration(HueyIntegration) is None:
-            return old_execute(self, task, timestamp)
-
-        with hub.push_scope() as scope:
+        with sentry_sdk.isolation_scope() as scope:
             with capture_internal_exceptions():
                 scope._name = "huey"
                 scope.clear_breadcrumbs()
                 scope.add_event_processor(_make_event_processor(task))
 
             sentry_headers = task.kwargs.pop("sentry_headers", None)
 
@@ -167,11 +157,11 @@
             )
             transaction.set_status("ok")
 
             if not getattr(task, "_sentry_is_patched", False):
                 task.execute = _wrap_task_execute(task.execute)
                 task._sentry_is_patched = True
 
-            with hub.start_transaction(transaction):
+            with sentry_sdk.start_transaction(transaction):
                 return old_execute(self, task, timestamp)
 
     Huey._execute = _sentry_execute
```

### Comparing `sentry-sdk-2.0.0rc3/sentry_sdk/integrations/logging.py` & `sentry-sdk-2.0.0rc4/sentry_sdk/integrations/logging.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc3/sentry_sdk/integrations/loguru.py` & `sentry-sdk-2.0.0rc4/sentry_sdk/integrations/loguru.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc3/sentry_sdk/integrations/modules.py` & `sentry-sdk-2.0.0rc4/sentry_sdk/integrations/modules.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc3/sentry_sdk/integrations/openai.py` & `sentry-sdk-2.0.0rc4/sentry_sdk/integrations/openai.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc3/sentry_sdk/integrations/opentelemetry/integration.py` & `sentry-sdk-2.0.0rc4/sentry_sdk/integrations/opentelemetry/integration.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc3/sentry_sdk/integrations/opentelemetry/propagator.py` & `sentry-sdk-2.0.0rc4/sentry_sdk/integrations/opentelemetry/propagator.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc3/sentry_sdk/integrations/opentelemetry/span_processor.py` & `sentry-sdk-2.0.0rc4/sentry_sdk/integrations/opentelemetry/span_processor.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,16 +12,16 @@
     Span as OTelSpan,
     SpanKind,
 )
 from opentelemetry.trace.span import (  # type: ignore
     INVALID_SPAN_ID,
     INVALID_TRACE_ID,
 )
+from sentry_sdk import get_client, start_transaction
 from sentry_sdk.consts import INSTRUMENTER
-from sentry_sdk.hub import Hub
 from sentry_sdk.integrations.opentelemetry.consts import (
     SENTRY_BAGGAGE_KEY,
     SENTRY_TRACE_KEY,
 )
 from sentry_sdk.scope import add_global_event_processor
 from sentry_sdk.tracing import Transaction, Span as SentrySpan
 from sentry_sdk.utils import Dsn
@@ -36,19 +36,17 @@
 
 OPEN_TELEMETRY_CONTEXT = "otel"
 SPAN_MAX_TIME_OPEN_MINUTES = 10
 
 
 def link_trace_context_to_error_event(event, otel_span_map):
     # type: (Event, Dict[str, Union[Transaction, SentrySpan]]) -> Event
-    hub = Hub.current
-    if not hub:
-        return event
+    client = get_client()
 
-    if hub.client and hub.client.options["instrumenter"] != INSTRUMENTER.OTEL:
+    if client.options["instrumenter"] != INSTRUMENTER.OTEL:
         return event
 
     if hasattr(event, "type") and event["type"] == "transaction":
         return event
 
     otel_span = get_current_span()
     if not otel_span:
@@ -112,33 +110,31 @@
             # prune old buckets
             elif current_time_minutes - span_start_minutes > SPAN_MAX_TIME_OPEN_MINUTES:
                 for span_id in self.open_spans.pop(span_start_minutes):
                     self.otel_span_map.pop(span_id, None)
 
     def on_start(self, otel_span, parent_context=None):
         # type: (OTelSpan, Optional[SpanContext]) -> None
-        hub = Hub.current
-        if not hub:
-            return
+        client = get_client()
 
-        if not hub.client or (hub.client and not hub.client.dsn):
+        if not client.dsn:
             return
 
         try:
-            _ = Dsn(hub.client.dsn or "")
+            _ = Dsn(client.dsn)
         except Exception:
             return
 
-        if hub.client and hub.client.options["instrumenter"] != INSTRUMENTER.OTEL:
+        if client.options["instrumenter"] != INSTRUMENTER.OTEL:
             return
 
         if not otel_span.get_span_context().is_valid:
             return
 
-        if self._is_sentry_span(hub, otel_span):
+        if self._is_sentry_span(otel_span):
             return
 
         trace_data = self._get_trace_data(otel_span, parent_context)
 
         parent_span_id = trace_data["parent_span_id"]
         sentry_parent_span = (
             self.otel_span_map.get(parent_span_id, None) if parent_span_id else None
@@ -151,15 +147,15 @@
                 description=otel_span.name,
                 start_timestamp=datetime.fromtimestamp(
                     otel_span.start_time / 1e9, timezone.utc
                 ),  # OTel spans have nanosecond precision
                 instrumenter=INSTRUMENTER.OTEL,
             )
         else:
-            sentry_span = hub.start_transaction(
+            sentry_span = start_transaction(
                 name=otel_span.name,
                 span_id=trace_data["span_id"],
                 parent_span_id=parent_span_id,
                 trace_id=trace_data["trace_id"],
                 baggage=trace_data["baggage"],
                 start_timestamp=datetime.fromtimestamp(
                     otel_span.start_time / 1e9, timezone.utc
@@ -175,19 +171,17 @@
         self.open_spans.setdefault(span_start_in_minutes, set()).add(
             trace_data["span_id"]
         )
         self._prune_old_spans()
 
     def on_end(self, otel_span):
         # type: (OTelSpan) -> None
-        hub = Hub.current
-        if not hub:
-            return
+        client = get_client()
 
-        if hub.client and hub.client.options["instrumenter"] != INSTRUMENTER.OTEL:
+        if client.options["instrumenter"] != INSTRUMENTER.OTEL:
             return
 
         span_context = otel_span.get_span_context()
         if not span_context.is_valid:
             return
 
         span_id = format_span_id(span_context.span_id)
@@ -215,22 +209,26 @@
 
         span_start_in_minutes = int(
             otel_span.start_time / 1e9 / 60
         )  # OTel spans have nanosecond precision
         self.open_spans.setdefault(span_start_in_minutes, set()).discard(span_id)
         self._prune_old_spans()
 
-    def _is_sentry_span(self, hub, otel_span):
-        # type: (Hub, OTelSpan) -> bool
+    def _is_sentry_span(self, otel_span):
+        # type: (OTelSpan) -> bool
         """
         Break infinite loop:
         HTTP requests to Sentry are caught by OTel and send again to Sentry.
         """
         otel_span_url = otel_span.attributes.get(SpanAttributes.HTTP_URL, None)
-        dsn_url = hub.client and Dsn(hub.client.dsn or "").netloc
+
+        dsn_url = None
+        client = get_client()
+        if client.dsn:
+            dsn_url = Dsn(client.dsn).netloc
 
         if otel_span_url and dsn_url in otel_span_url:
             return True
 
         return False
 
     def _get_otel_context(self, otel_span):
```

### Comparing `sentry-sdk-2.0.0rc3/sentry_sdk/integrations/pure_eval.py` & `sentry-sdk-2.0.0rc4/sentry_sdk/integrations/pure_eval.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import ast
 
-from sentry_sdk import Hub, serializer
+import sentry_sdk
+from sentry_sdk import serializer
 from sentry_sdk._types import TYPE_CHECKING
 from sentry_sdk.integrations import Integration, DidNotEnable
 from sentry_sdk.scope import add_global_event_processor
 from sentry_sdk.utils import walk_exception_chain, iter_stacks
 
 if TYPE_CHECKING:
     from typing import Optional, Dict, Any, Tuple, List
@@ -35,15 +36,15 @@
     @staticmethod
     def setup_once():
         # type: () -> None
 
         @add_global_event_processor
         def add_executing_info(event, hint):
             # type: (Event, Optional[Hint]) -> Optional[Event]
-            if Hub.current.get_integration(PureEvalIntegration) is None:
+            if sentry_sdk.get_client().get_integration(PureEvalIntegration) is None:
                 return event
 
             if hint is None:
                 return event
 
             exc_info = hint.get("exc_info", None)
```

### Comparing `sentry-sdk-2.0.0rc3/sentry_sdk/integrations/pymongo.py` & `sentry-sdk-2.0.0rc4/sentry_sdk/integrations/pymongo.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import copy
 
-from sentry_sdk import Hub
+import sentry_sdk
 from sentry_sdk.consts import SPANDATA
-from sentry_sdk.hub import _should_send_default_pii
 from sentry_sdk.integrations import DidNotEnable, Integration
+from sentry_sdk.scope import should_send_default_pii
 from sentry_sdk.tracing import Span
 from sentry_sdk.utils import capture_internal_exceptions
 
 from sentry_sdk._types import TYPE_CHECKING
 
 try:
     from pymongo import monitoring
@@ -112,17 +112,17 @@
 
     def _operation_key(self, event):
         # type: (Union[CommandFailedEvent, CommandStartedEvent, CommandSucceededEvent]) -> int
         return event.request_id
 
     def started(self, event):
         # type: (CommandStartedEvent) -> None
-        hub = Hub.current
-        if hub.get_integration(PyMongoIntegration) is None:
+        if sentry_sdk.get_client().get_integration(PyMongoIntegration) is None:
             return
+
         with capture_internal_exceptions():
             command = dict(copy.deepcopy(event.command))
 
             command.pop("$db", None)
             command.pop("$clusterTime", None)
             command.pop("$signature", None)
 
@@ -148,48 +148,48 @@
 
             try:
                 lsid = command.pop("lsid")["id"]
                 data["operation_ids"]["session"] = str(lsid)
             except KeyError:
                 pass
 
-            if not _should_send_default_pii():
+            if not should_send_default_pii():
                 command = _strip_pii(command)
 
             query = "{} {}".format(event.command_name, command)
-            span = hub.start_span(op=op, description=query)
+            span = sentry_sdk.start_span(op=op, description=query)
 
             for tag, value in tags.items():
                 span.set_tag(tag, value)
 
             for key, value in data.items():
                 span.set_data(key, value)
 
             with capture_internal_exceptions():
-                hub.add_breadcrumb(message=query, category="query", type=op, data=tags)
+                sentry_sdk.add_breadcrumb(
+                    message=query, category="query", type=op, data=tags
+                )
 
             self._ongoing_operations[self._operation_key(event)] = span.__enter__()
 
     def failed(self, event):
         # type: (CommandFailedEvent) -> None
-        hub = Hub.current
-        if hub.get_integration(PyMongoIntegration) is None:
+        if sentry_sdk.get_client().get_integration(PyMongoIntegration) is None:
             return
 
         try:
             span = self._ongoing_operations.pop(self._operation_key(event))
             span.set_status("internal_error")
             span.__exit__(None, None, None)
         except KeyError:
             return
 
     def succeeded(self, event):
         # type: (CommandSucceededEvent) -> None
-        hub = Hub.current
-        if hub.get_integration(PyMongoIntegration) is None:
+        if sentry_sdk.get_client().get_integration(PyMongoIntegration) is None:
             return
 
         try:
             span = self._ongoing_operations.pop(self._operation_key(event))
             span.set_status("ok")
             span.__exit__(None, None, None)
         except KeyError:
```

### Comparing `sentry-sdk-2.0.0rc3/sentry_sdk/integrations/pyramid.py` & `sentry-sdk-2.0.0rc4/sentry_sdk/integrations/pyramid.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 import os
 import sys
 import weakref
 
-from sentry_sdk.hub import Hub, _should_send_default_pii
-from sentry_sdk.scope import Scope
+import sentry_sdk
+from sentry_sdk.integrations import Integration, DidNotEnable
+from sentry_sdk.integrations._wsgi_common import RequestExtractor
+from sentry_sdk.integrations.wsgi import SentryWsgiMiddleware
+from sentry_sdk.scope import Scope, should_send_default_pii
 from sentry_sdk.tracing import SOURCE_FOR_STYLE
 from sentry_sdk.utils import (
     capture_internal_exceptions,
+    ensure_integration_enabled,
     event_from_exception,
     reraise,
 )
-from sentry_sdk.integrations import Integration, DidNotEnable
-from sentry_sdk.integrations._wsgi_common import RequestExtractor
-from sentry_sdk.integrations.wsgi import SentryWsgiMiddleware
+from sentry_sdk._types import TYPE_CHECKING
 
 try:
     from pyramid.httpexceptions import HTTPException
     from pyramid.request import Request
 except ImportError:
     raise DidNotEnable("Pyramid not installed")
 
-from sentry_sdk._types import TYPE_CHECKING
 
 if TYPE_CHECKING:
     from pyramid.response import Response
     from typing import Any
     from sentry_sdk.integrations.wsgi import _ScopedResponse
     from typing import Callable
     from typing import Dict
@@ -67,27 +68,26 @@
     @staticmethod
     def setup_once():
         # type: () -> None
         from pyramid import router
 
         old_call_view = router._call_view
 
+        @ensure_integration_enabled(PyramidIntegration, old_call_view)
         def sentry_patched_call_view(registry, request, *args, **kwargs):
             # type: (Any, Request, *Any, **Any) -> Response
-            hub = Hub.current
-            integration = hub.get_integration(PyramidIntegration)
+            integration = sentry_sdk.get_client().get_integration(PyramidIntegration)
 
-            if integration is not None:
-                _set_transaction_name_and_source(
-                    Scope.get_current_scope(), integration.transaction_style, request
-                )
-                with hub.configure_scope() as scope:
-                    scope.add_event_processor(
-                        _make_event_processor(weakref.ref(request), integration)
-                    )
+            _set_transaction_name_and_source(
+                Scope.get_current_scope(), integration.transaction_style, request
+            )
+            scope = Scope.get_isolation_scope()
+            scope.add_event_processor(
+                _make_event_processor(weakref.ref(request), integration)
+            )
 
             return old_call_view(registry, request, *args, **kwargs)
 
         router._call_view = sentry_patched_call_view
 
         if hasattr(Request, "invoke_exception_view"):
             old_invoke_exception_view = Request.invoke_exception_view
@@ -96,31 +96,28 @@
                 # type: (Request, *Any, **Any) -> Any
                 rv = old_invoke_exception_view(self, *args, **kwargs)
 
                 if (
                     self.exc_info
                     and all(self.exc_info)
                     and rv.status_int == 500
-                    and Hub.current.get_integration(PyramidIntegration) is not None
+                    and sentry_sdk.get_client().get_integration(PyramidIntegration)
+                    is not None
                 ):
                     _capture_exception(self.exc_info)
 
                 return rv
 
             Request.invoke_exception_view = sentry_patched_invoke_exception_view
 
         old_wsgi_call = router.Router.__call__
 
+        @ensure_integration_enabled(PyramidIntegration, old_wsgi_call)
         def sentry_patched_wsgi_call(self, environ, start_response):
             # type: (Any, Dict[str, str], Callable[..., Any]) -> _ScopedResponse
-            hub = Hub.current
-            integration = hub.get_integration(PyramidIntegration)
-            if integration is None:
-                return old_wsgi_call(self, environ, start_response)
-
             def sentry_patched_inner_wsgi_call(environ, start_response):
                 # type: (Dict[str, Any], Callable[..., Any]) -> Any
                 try:
                     return old_wsgi_call(self, environ, start_response)
                 except Exception:
                     einfo = sys.exc_info()
                     _capture_exception(einfo)
@@ -129,32 +126,27 @@
             return SentryWsgiMiddleware(sentry_patched_inner_wsgi_call)(
                 environ, start_response
             )
 
         router.Router.__call__ = sentry_patched_wsgi_call
 
 
+@ensure_integration_enabled(PyramidIntegration)
 def _capture_exception(exc_info):
     # type: (ExcInfo) -> None
     if exc_info[0] is None or issubclass(exc_info[0], HTTPException):
         return
-    hub = Hub.current
-    if hub.get_integration(PyramidIntegration) is None:
-        return
-
-    # If an integration is there, a client has to be there.
-    client = hub.client  # type: Any
 
     event, hint = event_from_exception(
         exc_info,
-        client_options=client.options,
+        client_options=sentry_sdk.get_client().options,
         mechanism={"type": "pyramid", "handled": False},
     )
 
-    hub.capture_event(event, hint=hint)
+    sentry_sdk.capture_event(event, hint=hint)
 
 
 def _set_transaction_name_and_source(scope, transaction_style, request):
     # type: (Scope, str, Request) -> None
     try:
         name_for_style = {
             "route_name": request.matched_route.name,
@@ -217,15 +209,15 @@
         request = weak_request()
         if request is None:
             return event
 
         with capture_internal_exceptions():
             PyramidRequestExtractor(request).extract_into_event(event)
 
-        if _should_send_default_pii():
+        if should_send_default_pii():
             with capture_internal_exceptions():
                 user_info = event.setdefault("user", {})
                 user_info.setdefault("id", authenticated_userid(request))
 
         return event
 
     return pyramid_event_processor
```

### Comparing `sentry-sdk-2.0.0rc3/sentry_sdk/integrations/quart.py` & `sentry-sdk-2.0.0rc4/sentry_sdk/integrations/quart.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 import asyncio
 import inspect
 import threading
 from functools import wraps
 
-from sentry_sdk.hub import _should_send_default_pii, Hub
+import sentry_sdk
 from sentry_sdk.integrations import DidNotEnable, Integration
 from sentry_sdk.integrations._wsgi_common import _filter_headers
 from sentry_sdk.integrations.asgi import SentryAsgiMiddleware
-from sentry_sdk.scope import Scope
+from sentry_sdk.scope import Scope, should_send_default_pii
 from sentry_sdk.tracing import SOURCE_FOR_STYLE
 from sentry_sdk.utils import (
     capture_internal_exceptions,
+    ensure_integration_enabled,
+    ensure_integration_enabled_async,
     event_from_exception,
 )
 from sentry_sdk._types import TYPE_CHECKING
 
 if TYPE_CHECKING:
     from typing import Any
     from typing import Union
@@ -82,19 +84,17 @@
         patch_scaffold_route()
 
 
 def patch_asgi_app():
     # type: () -> None
     old_app = Quart.__call__
 
+    @ensure_integration_enabled(QuartIntegration, old_app)
     async def sentry_patched_asgi_app(self, scope, receive, send):
         # type: (Any, Any, Any, Any) -> Any
-        if Hub.current.get_integration(QuartIntegration) is None:
-            return await old_app(self, scope, receive, send)
-
         middleware = SentryAsgiMiddleware(lambda *a, **kw: old_app(self, *a, **kw))
         middleware.__call__ = middleware._run_asgi3
         return await middleware(scope, receive, send)
 
     Quart.__call__ = sentry_patched_asgi_app
 
 
@@ -110,28 +110,24 @@
             # type: (Any) -> Any
 
             if inspect.isfunction(old_func) and not asyncio.iscoroutinefunction(
                 old_func
             ):
 
                 @wraps(old_func)
+                @ensure_integration_enabled(QuartIntegration, old_func)
                 def _sentry_func(*args, **kwargs):
                     # type: (*Any, **Any) -> Any
-                    hub = Hub.current
-                    integration = hub.get_integration(QuartIntegration)
-                    if integration is None:
-                        return old_func(*args, **kwargs)
-
-                    with hub.configure_scope() as sentry_scope:
-                        if sentry_scope.profile is not None:
-                            sentry_scope.profile.active_thread_id = (
-                                threading.current_thread().ident
-                            )
+                    scope = Scope.get_isolation_scope()
+                    if scope.profile is not None:
+                        scope.profile.active_thread_id = (
+                            threading.current_thread().ident
+                        )
 
-                        return old_func(*args, **kwargs)
+                    return old_func(*args, **kwargs)
 
                 return old_decorator(_sentry_func)
 
             return old_decorator(old_func)
 
         return decorator
 
@@ -150,37 +146,33 @@
             name_for_style[transaction_style],
             source=SOURCE_FOR_STYLE[transaction_style],
         )
     except Exception:
         pass
 
 
+@ensure_integration_enabled_async(QuartIntegration)
 async def _request_websocket_started(app, **kwargs):
     # type: (Quart, **Any) -> None
-    hub = Hub.current
-    integration = hub.get_integration(QuartIntegration)
-    if integration is None:
-        return
+    integration = sentry_sdk.get_client().get_integration(QuartIntegration)
 
     if has_request_context():
         request_websocket = request._get_current_object()
     if has_websocket_context():
         request_websocket = websocket._get_current_object()
 
     # Set the transaction name here, but rely on ASGI middleware
     # to actually start the transaction
     _set_transaction_name_and_source(
         Scope.get_current_scope(), integration.transaction_style, request_websocket
     )
 
-    with hub.configure_scope() as scope:
-        evt_processor = _make_request_event_processor(
-            app, request_websocket, integration
-        )
-        scope.add_event_processor(evt_processor)
+    scope = Scope.get_isolation_scope()
+    evt_processor = _make_request_event_processor(app, request_websocket, integration)
+    scope.add_event_processor(evt_processor)
 
 
 def _make_request_event_processor(app, request, integration):
     # type: (Quart, Request, QuartIntegration) -> EventProcessor
     def inner(event, hint):
         # type: (Event, dict[str, Any]) -> Event
         # if the request is gone we are fine not logging the data from
@@ -195,39 +187,33 @@
 
             request_info = event.setdefault("request", {})
             request_info["url"] = request.url
             request_info["query_string"] = request.query_string
             request_info["method"] = request.method
             request_info["headers"] = _filter_headers(dict(request.headers))
 
-            if _should_send_default_pii():
+            if should_send_default_pii():
                 request_info["env"] = {"REMOTE_ADDR": request.access_route[0]}
                 _add_user_to_event(event)
 
         return event
 
     return inner
 
 
+@ensure_integration_enabled_async(QuartIntegration)
 async def _capture_exception(sender, exception, **kwargs):
     # type: (Quart, Union[ValueError, BaseException], **Any) -> None
-    hub = Hub.current
-    if hub.get_integration(QuartIntegration) is None:
-        return
-
-    # If an integration is there, a client has to be there.
-    client = hub.client  # type: Any
-
     event, hint = event_from_exception(
         exception,
-        client_options=client.options,
+        client_options=sentry_sdk.get_client().options,
         mechanism={"type": "quart", "handled": False},
     )
 
-    hub.capture_event(event, hint=hint)
+    sentry_sdk.capture_event(event, hint=hint)
 
 
 def _add_user_to_event(event):
     # type: (Event) -> None
     if quart_auth is None:
         return
```

### Comparing `sentry-sdk-2.0.0rc3/sentry_sdk/integrations/redis/__init__.py` & `sentry-sdk-2.0.0rc4/sentry_sdk/integrations/redis/__init__.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc3/sentry_sdk/integrations/redis/asyncio.py` & `sentry-sdk-2.0.0rc4/sentry_sdk/integrations/redis/asyncio.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc3/sentry_sdk/integrations/rq.py` & `sentry-sdk-2.0.0rc4/sentry_sdk/integrations/rq.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import weakref
 
+import sentry_sdk
 from sentry_sdk.consts import OP
 from sentry_sdk.api import continue_trace
-from sentry_sdk.hub import Hub
 from sentry_sdk.integrations import DidNotEnable, Integration
 from sentry_sdk.integrations.logging import ignore_logger
 from sentry_sdk.tracing import TRANSACTION_SOURCE_TASK
 from sentry_sdk.scope import Scope
 from sentry_sdk.utils import (
     capture_internal_exceptions,
+    ensure_integration_enabled,
     event_from_exception,
     format_timestamp,
     parse_version,
 )
 
 try:
     from rq.queue import Queue
@@ -47,49 +48,41 @@
             raise DidNotEnable("Unparsable RQ version: {}".format(RQ_VERSION))
 
         if version < (0, 6):
             raise DidNotEnable("RQ 0.6 or newer is required.")
 
         old_perform_job = Worker.perform_job
 
+        @ensure_integration_enabled(RqIntegration, old_perform_job)
         def sentry_patched_perform_job(self, job, *args, **kwargs):
             # type: (Any, Job, *Queue, **Any) -> bool
-            hub = Hub.current
-            integration = hub.get_integration(RqIntegration)
-
-            if integration is None:
-                return old_perform_job(self, job, *args, **kwargs)
-
-            client = hub.client
-            assert client is not None
-
-            with hub.push_scope() as scope:
+            with sentry_sdk.new_scope() as scope:
                 scope.clear_breadcrumbs()
                 scope.add_event_processor(_make_event_processor(weakref.ref(job)))
 
                 transaction = continue_trace(
                     job.meta.get("_sentry_trace_headers") or {},
                     op=OP.QUEUE_TASK_RQ,
                     name="unknown RQ task",
                     source=TRANSACTION_SOURCE_TASK,
                 )
 
                 with capture_internal_exceptions():
                     transaction.name = job.func_name
 
-                with hub.start_transaction(
+                with sentry_sdk.start_transaction(
                     transaction, custom_sampling_context={"rq_job": job}
                 ):
                     rv = old_perform_job(self, job, *args, **kwargs)
 
             if self.is_horse:
                 # We're inside of a forked process and RQ is
                 # about to call `os._exit`. Make sure that our
                 # events get sent out.
-                client.flush()
+                sentry_sdk.get_client().flush()
 
             return rv
 
         Worker.perform_job = sentry_patched_perform_job
 
         old_handle_exception = Worker.handle_exception
 
@@ -102,23 +95,22 @@
 
             return old_handle_exception(self, job, *exc_info, **kwargs)
 
         Worker.handle_exception = sentry_patched_handle_exception
 
         old_enqueue_job = Queue.enqueue_job
 
+        @ensure_integration_enabled(RqIntegration, old_enqueue_job)
         def sentry_patched_enqueue_job(self, job, **kwargs):
             # type: (Queue, Any, **Any) -> Any
-            hub = Hub.current
-            if hub.get_integration(RqIntegration) is not None:
-                scope = Scope.get_current_scope()
-                if scope.span is not None:
-                    job.meta["_sentry_trace_headers"] = dict(
-                        scope.iter_trace_propagation_headers()
-                    )
+            scope = Scope.get_current_scope()
+            if scope.span is not None:
+                job.meta["_sentry_trace_headers"] = dict(
+                    scope.iter_trace_propagation_headers()
+                )
 
             return old_enqueue_job(self, job, **kwargs)
 
         Queue.enqueue_job = sentry_patched_enqueue_job
 
         ignore_logger("rq.worker")
 
@@ -154,21 +146,16 @@
         return event
 
     return event_processor
 
 
 def _capture_exception(exc_info, **kwargs):
     # type: (ExcInfo, **Any) -> None
-    hub = Hub.current
-    if hub.get_integration(RqIntegration) is None:
-        return
-
-    # If an integration is there, a client has to be there.
-    client = hub.client  # type: Any
+    client = sentry_sdk.get_client()
 
     event, hint = event_from_exception(
         exc_info,
         client_options=client.options,
         mechanism={"type": "rq", "handled": False},
     )
 
-    hub.capture_event(event, hint=hint)
+    sentry_sdk.capture_event(event, hint=hint)
```

### Comparing `sentry-sdk-2.0.0rc3/sentry_sdk/integrations/sanic.py` & `sentry-sdk-2.0.0rc4/sentry_sdk/integrations/sanic.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 import sys
 import weakref
 from inspect import isawaitable
 from urllib.parse import urlsplit
 
+import sentry_sdk
 from sentry_sdk import continue_trace
 from sentry_sdk.consts import OP
-from sentry_sdk.hub import Hub
+from sentry_sdk.integrations import Integration, DidNotEnable
+from sentry_sdk.integrations._wsgi_common import RequestExtractor, _filter_headers
+from sentry_sdk.integrations.logging import ignore_logger
 from sentry_sdk.tracing import TRANSACTION_SOURCE_COMPONENT, TRANSACTION_SOURCE_URL
 from sentry_sdk.scope import Scope
 from sentry_sdk.utils import (
     capture_internal_exceptions,
+    ensure_integration_enabled,
+    ensure_integration_enabled_async,
     event_from_exception,
     HAS_REAL_CONTEXTVARS,
     CONTEXTVARS_ERROR_MESSAGE,
     parse_version,
     reraise,
 )
-from sentry_sdk.integrations import Integration, DidNotEnable
-from sentry_sdk.integrations._wsgi_common import RequestExtractor, _filter_headers
-from sentry_sdk.integrations.logging import ignore_logger
-
 from sentry_sdk._types import TYPE_CHECKING
 
 if TYPE_CHECKING:
     from collections.abc import Container
     from typing import Any
     from typing import Callable
     from typing import Optional
@@ -158,81 +159,80 @@
     ErrorHandler.lookup = _sentry_error_handler_lookup
 
 
 async def _startup(self):
     # type: (Sanic) -> None
     # This happens about as early in the lifecycle as possible, just after the
     # Request object is created. The body has not yet been consumed.
-    self.signal("http.lifecycle.request")(_hub_enter)
+    self.signal("http.lifecycle.request")(_context_enter)
 
     # This happens after the handler is complete. In v21.9 this signal is not
     # dispatched when there is an exception. Therefore we need to close out
-    # and call _hub_exit from the custom exception handler as well.
+    # and call _context_exit from the custom exception handler as well.
     # See https://github.com/sanic-org/sanic/issues/2297
-    self.signal("http.lifecycle.response")(_hub_exit)
+    self.signal("http.lifecycle.response")(_context_exit)
 
     # This happens inside of request handling immediately after the route
     # has been identified by the router.
     self.signal("http.routing.after")(_set_transaction)
 
     # The above signals need to be declared before this can be called.
     await old_startup(self)
 
 
-async def _hub_enter(request):
+async def _context_enter(request):
     # type: (Request) -> None
-    hub = Hub.current
     request.ctx._sentry_do_integration = (
-        hub.get_integration(SanicIntegration) is not None
+        sentry_sdk.get_client().get_integration(SanicIntegration) is not None
     )
 
     if not request.ctx._sentry_do_integration:
         return
 
     weak_request = weakref.ref(request)
-    request.ctx._sentry_hub = Hub(hub)
-    request.ctx._sentry_hub.__enter__()
-
-    with request.ctx._sentry_hub.configure_scope() as scope:
-        scope.clear_breadcrumbs()
-        scope.add_event_processor(_make_request_processor(weak_request))
+    request.ctx._sentry_scope = sentry_sdk.isolation_scope()
+    scope = request.ctx._sentry_scope.__enter__()
+    scope.clear_breadcrumbs()
+    scope.add_event_processor(_make_request_processor(weak_request))
 
     transaction = continue_trace(
         dict(request.headers),
         op=OP.HTTP_SERVER,
         # Unless the request results in a 404 error, the name and source will get overwritten in _set_transaction
         name=request.path,
         source=TRANSACTION_SOURCE_URL,
     )
-    request.ctx._sentry_transaction = request.ctx._sentry_hub.start_transaction(
+    request.ctx._sentry_transaction = sentry_sdk.start_transaction(
         transaction
     ).__enter__()
 
 
-async def _hub_exit(request, response=None):
+async def _context_exit(request, response=None):
     # type: (Request, Optional[BaseHTTPResponse]) -> None
     with capture_internal_exceptions():
         if not request.ctx._sentry_do_integration:
             return
 
-        integration = Hub.current.get_integration(SanicIntegration)  # type: Integration
+        integration = sentry_sdk.get_client().get_integration(
+            SanicIntegration
+        )  # type: Integration
 
         response_status = None if response is None else response.status
 
         # This capture_internal_exceptions block has been intentionally nested here, so that in case an exception
         # happens while trying to end the transaction, we still attempt to exit the hub.
         with capture_internal_exceptions():
             request.ctx._sentry_transaction.set_http_status(response_status)
             request.ctx._sentry_transaction.sampled &= (
                 isinstance(integration, SanicIntegration)
                 and response_status not in integration._unsampled_statuses
             )
             request.ctx._sentry_transaction.__exit__(None, None, None)
 
-        request.ctx._sentry_hub.__exit__(None, None, None)
+        request.ctx._sentry_scope.__exit__(None, None, None)
 
 
 async def _set_transaction(request, route, **_):
     # type: (Request, Route, **Any) -> None
     if request.ctx._sentry_do_integration:
         with capture_internal_exceptions():
             scope = Scope.get_current_scope()
@@ -244,15 +244,15 @@
     # type: (Any, Exception, *Any, **Any) -> Optional[object]
     _capture_exception(exception)
     old_error_handler = old_error_handler_lookup(self, exception, *args, **kwargs)
 
     if old_error_handler is None:
         return None
 
-    if Hub.current.get_integration(SanicIntegration) is None:
+    if sentry_sdk.get_client().get_integration(SanicIntegration) is None:
         return old_error_handler
 
     async def sentry_wrapped_error_handler(request, exception):
         # type: (Request, Exception) -> Any
         try:
             response = old_error_handler(request, exception)
             if isawaitable(response):
@@ -265,87 +265,75 @@
             exc_info = sys.exc_info()
             _capture_exception(exc_info)
             reraise(*exc_info)
         finally:
             # As mentioned in previous comment in _startup, this can be removed
             # after https://github.com/sanic-org/sanic/issues/2297 is resolved
             if SanicIntegration.version and SanicIntegration.version == (21, 9):
-                await _hub_exit(request)
+                await _context_exit(request)
 
     return sentry_wrapped_error_handler
 
 
+@ensure_integration_enabled_async(SanicIntegration, old_handle_request)
 async def _legacy_handle_request(self, request, *args, **kwargs):
     # type: (Any, Request, *Any, **Any) -> Any
-    hub = Hub.current
-    if hub.get_integration(SanicIntegration) is None:
-        return old_handle_request(self, request, *args, **kwargs)
-
     weak_request = weakref.ref(request)
 
-    with Hub(hub) as hub:
-        with hub.configure_scope() as scope:
-            scope.clear_breadcrumbs()
-            scope.add_event_processor(_make_request_processor(weak_request))
+    with sentry_sdk.isolation_scope() as scope:
+        scope.clear_breadcrumbs()
+        scope.add_event_processor(_make_request_processor(weak_request))
 
         response = old_handle_request(self, request, *args, **kwargs)
         if isawaitable(response):
             response = await response
 
         return response
 
 
 def _legacy_router_get(self, *args):
     # type: (Any, Union[Any, Request]) -> Any
     rv = old_router_get(self, *args)
-    hub = Hub.current
-    if hub.get_integration(SanicIntegration) is not None:
+    if sentry_sdk.get_client().get_integration(SanicIntegration) is not None:
         with capture_internal_exceptions():
-            with hub.configure_scope() as scope:
-                if SanicIntegration.version and SanicIntegration.version >= (21, 3):
-                    # Sanic versions above and including 21.3 append the app name to the
-                    # route name, and so we need to remove it from Route name so the
-                    # transaction name is consistent across all versions
-                    sanic_app_name = self.ctx.app.name
-                    sanic_route = rv[0].name
-
-                    if sanic_route.startswith("%s." % sanic_app_name):
-                        # We add a 1 to the len of the sanic_app_name because there is a dot
-                        # that joins app name and the route name
-                        # Format: app_name.route_name
-                        sanic_route = sanic_route[len(sanic_app_name) + 1 :]
-
-                    scope.set_transaction_name(
-                        sanic_route, source=TRANSACTION_SOURCE_COMPONENT
-                    )
-                else:
-                    scope.set_transaction_name(
-                        rv[0].__name__, source=TRANSACTION_SOURCE_COMPONENT
-                    )
+            scope = Scope.get_isolation_scope()
+            if SanicIntegration.version and SanicIntegration.version >= (21, 3):
+                # Sanic versions above and including 21.3 append the app name to the
+                # route name, and so we need to remove it from Route name so the
+                # transaction name is consistent across all versions
+                sanic_app_name = self.ctx.app.name
+                sanic_route = rv[0].name
+
+                if sanic_route.startswith("%s." % sanic_app_name):
+                    # We add a 1 to the len of the sanic_app_name because there is a dot
+                    # that joins app name and the route name
+                    # Format: app_name.route_name
+                    sanic_route = sanic_route[len(sanic_app_name) + 1 :]
+
+                scope.set_transaction_name(
+                    sanic_route, source=TRANSACTION_SOURCE_COMPONENT
+                )
+            else:
+                scope.set_transaction_name(
+                    rv[0].__name__, source=TRANSACTION_SOURCE_COMPONENT
+                )
 
     return rv
 
 
+@ensure_integration_enabled(SanicIntegration)
 def _capture_exception(exception):
     # type: (Union[Tuple[Optional[type], Optional[BaseException], Any], BaseException]) -> None
-    hub = Hub.current
-    integration = hub.get_integration(SanicIntegration)
-    if integration is None:
-        return
-
-    # If an integration is there, a client has to be there.
-    client = hub.client  # type: Any
-
     with capture_internal_exceptions():
         event, hint = event_from_exception(
             exception,
-            client_options=client.options,
+            client_options=sentry_sdk.get_client().options,
             mechanism={"type": "sanic", "handled": False},
         )
-        hub.capture_event(event, hint=hint)
+        sentry_sdk.capture_event(event, hint=hint)
 
 
 def _make_request_processor(weak_request):
     # type: (Callable[[], Request]) -> EventProcessor
     def sanic_processor(event, hint):
         # type: (Event, Optional[Hint]) -> Optional[Event]
```

### Comparing `sentry-sdk-2.0.0rc3/sentry_sdk/integrations/serverless.py` & `sentry-sdk-2.0.0rc4/sentry_sdk/integrations/serverless.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import sys
 from functools import wraps
 
-from sentry_sdk.hub import Hub
+import sentry_sdk
 from sentry_sdk.utils import event_from_exception, reraise
 from sentry_sdk._types import TYPE_CHECKING
 
 if TYPE_CHECKING:
     from typing import Any
     from typing import Callable
     from typing import TypeVar
@@ -38,45 +38,39 @@
 def serverless_function(f=None, flush=True):  # noqa
     # type: (Optional[F], bool) -> Union[F, Callable[[F], F]]
     def wrapper(f):
         # type: (F) -> F
         @wraps(f)
         def inner(*args, **kwargs):
             # type: (*Any, **Any) -> Any
-            with Hub(Hub.current) as hub:
-                with hub.configure_scope() as scope:
-                    scope.clear_breadcrumbs()
+            with sentry_sdk.isolation_scope() as scope:
+                scope.clear_breadcrumbs()
 
                 try:
                     return f(*args, **kwargs)
                 except Exception:
                     _capture_and_reraise()
                 finally:
                     if flush:
-                        _flush_client()
+                        sentry_sdk.flush()
 
         return inner  # type: ignore
 
     if f is None:
         return wrapper
     else:
         return wrapper(f)
 
 
 def _capture_and_reraise():
     # type: () -> None
     exc_info = sys.exc_info()
-    hub = Hub.current
-    if hub.client is not None:
+    client = sentry_sdk.get_client()
+    if client.is_active():
         event, hint = event_from_exception(
             exc_info,
-            client_options=hub.client.options,
+            client_options=client.options,
             mechanism={"type": "serverless", "handled": False},
         )
-        hub.capture_event(event, hint=hint)
+        sentry_sdk.capture_event(event, hint=hint)
 
     reraise(*exc_info)
-
-
-def _flush_client():
-    # type: () -> None
-    return Hub.current.flush()
```

### Comparing `sentry-sdk-2.0.0rc3/sentry_sdk/integrations/socket.py` & `sentry-sdk-2.0.0rc4/sentry_sdk/integrations/socket.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import socket
-from sentry_sdk import Hub
+
+import sentry_sdk
 from sentry_sdk._types import MYPY
 from sentry_sdk.consts import OP
 from sentry_sdk.integrations import Integration
 
 if MYPY:
     from socket import AddressFamily, SocketKind
     from typing import Tuple, Optional, Union, List
@@ -43,21 +44,19 @@
 
     def create_connection(
         address,
         timeout=socket._GLOBAL_DEFAULT_TIMEOUT,  # type: ignore
         source_address=None,
     ):
         # type: (Tuple[Optional[str], int], Optional[float], Optional[Tuple[Union[bytearray, bytes, str], int]])-> socket.socket
-        hub = Hub.current
-        if hub.get_integration(SocketIntegration) is None:
-            return real_create_connection(
-                address=address, timeout=timeout, source_address=source_address
-            )
+        integration = sentry_sdk.get_client().get_integration(SocketIntegration)
+        if integration is None:
+            return real_create_connection(address, timeout, source_address)
 
-        with hub.start_span(
+        with sentry_sdk.start_span(
             op=OP.SOCKET_CONNECTION,
             description=_get_span_description(address[0], address[1]),
         ) as span:
             span.set_data("address", address)
             span.set_data("timeout", timeout)
             span.set_data("source_address", source_address)
 
@@ -70,19 +69,19 @@
 
 def _patch_getaddrinfo():
     # type: () -> None
     real_getaddrinfo = socket.getaddrinfo
 
     def getaddrinfo(host, port, family=0, type=0, proto=0, flags=0):
         # type: (Union[bytes, str, None], Union[str, int, None], int, int, int, int) -> List[Tuple[AddressFamily, SocketKind, int, str, Union[Tuple[str, int], Tuple[str, int, int, int]]]]
-        hub = Hub.current
-        if hub.get_integration(SocketIntegration) is None:
+        integration = sentry_sdk.get_client().get_integration(SocketIntegration)
+        if integration is None:
             return real_getaddrinfo(host, port, family, type, proto, flags)
 
-        with hub.start_span(
+        with sentry_sdk.start_span(
             op=OP.SOCKET_DNS, description=_get_span_description(host, port)
         ) as span:
             span.set_data("host", host)
             span.set_data("port", port)
 
             return real_getaddrinfo(host, port, family, type, proto, flags)
```

### Comparing `sentry-sdk-2.0.0rc3/sentry_sdk/integrations/spark/spark_driver.py` & `sentry-sdk-2.0.0rc4/sentry_sdk/integrations/spark/spark_driver.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from sentry_sdk import configure_scope
-from sentry_sdk.hub import Hub
+import sentry_sdk
 from sentry_sdk.integrations import Integration
-from sentry_sdk.utils import capture_internal_exceptions
+from sentry_sdk.scope import Scope
+from sentry_sdk.utils import capture_internal_exceptions, ensure_integration_enabled
 
 from sentry_sdk._types import TYPE_CHECKING
 
 if TYPE_CHECKING:
     from typing import Any
     from typing import Optional
 
@@ -52,59 +52,55 @@
 
 def patch_spark_context_init():
     # type: () -> None
     from pyspark import SparkContext
 
     spark_context_init = SparkContext._do_init
 
+    @ensure_integration_enabled(SparkIntegration, spark_context_init)
     def _sentry_patched_spark_context_init(self, *args, **kwargs):
         # type: (SparkContext, *Any, **Any) -> Optional[Any]
-        init = spark_context_init(self, *args, **kwargs)
-
-        if Hub.current.get_integration(SparkIntegration) is None:
-            return init
-
         _start_sentry_listener(self)
         _set_app_properties()
 
-        with configure_scope() as scope:
+        scope = Scope.get_isolation_scope()
 
-            @scope.add_event_processor
-            def process_event(event, hint):
-                # type: (Event, Hint) -> Optional[Event]
-                with capture_internal_exceptions():
-                    if Hub.current.get_integration(SparkIntegration) is None:
-                        return event
-
-                    event.setdefault("user", {}).setdefault("id", self.sparkUser())
-
-                    event.setdefault("tags", {}).setdefault(
-                        "executor.id", self._conf.get("spark.executor.id")
-                    )
-                    event["tags"].setdefault(
-                        "spark-submit.deployMode",
-                        self._conf.get("spark.submit.deployMode"),
-                    )
-                    event["tags"].setdefault(
-                        "driver.host", self._conf.get("spark.driver.host")
-                    )
-                    event["tags"].setdefault(
-                        "driver.port", self._conf.get("spark.driver.port")
-                    )
-                    event["tags"].setdefault("spark_version", self.version)
-                    event["tags"].setdefault("app_name", self.appName)
-                    event["tags"].setdefault("application_id", self.applicationId)
-                    event["tags"].setdefault("master", self.master)
-                    event["tags"].setdefault("spark_home", self.sparkHome)
+        @scope.add_event_processor
+        def process_event(event, hint):
+            # type: (Event, Hint) -> Optional[Event]
+            with capture_internal_exceptions():
+                if sentry_sdk.get_client().get_integration(SparkIntegration) is None:
+                    return event
+
+                event.setdefault("user", {}).setdefault("id", self.sparkUser())
+
+                event.setdefault("tags", {}).setdefault(
+                    "executor.id", self._conf.get("spark.executor.id")
+                )
+                event["tags"].setdefault(
+                    "spark-submit.deployMode",
+                    self._conf.get("spark.submit.deployMode"),
+                )
+                event["tags"].setdefault(
+                    "driver.host", self._conf.get("spark.driver.host")
+                )
+                event["tags"].setdefault(
+                    "driver.port", self._conf.get("spark.driver.port")
+                )
+                event["tags"].setdefault("spark_version", self.version)
+                event["tags"].setdefault("app_name", self.appName)
+                event["tags"].setdefault("application_id", self.applicationId)
+                event["tags"].setdefault("master", self.master)
+                event["tags"].setdefault("spark_home", self.sparkHome)
 
-                    event.setdefault("extra", {}).setdefault("web_url", self.uiWebUrl)
+                event.setdefault("extra", {}).setdefault("web_url", self.uiWebUrl)
 
-                return event
+            return event
 
-        return init
+        return spark_context_init(self, *args, **kwargs)
 
     SparkContext._do_init = _sentry_patched_spark_context_init
 
 
 class SparkListener:
     def onApplicationEnd(self, applicationEnd):  # noqa: N802,N803
         # type: (Any) -> None
@@ -205,22 +201,18 @@
         pass
 
     class Java:
         implements = ["org.apache.spark.scheduler.SparkListenerInterface"]
 
 
 class SentryListener(SparkListener):
-    def __init__(self):
-        # type: () -> None
-        self.hub = Hub.current
-
     def onJobStart(self, jobStart):  # noqa: N802,N803
         # type: (Any) -> None
         message = "Job {} Started".format(jobStart.jobId())
-        self.hub.add_breadcrumb(level="info", message=message)
+        sentry_sdk.add_breadcrumb(level="info", message=message)
         _set_app_properties()
 
     def onJobEnd(self, jobEnd):  # noqa: N802,N803
         # type: (Any) -> None
         level = ""
         message = ""
         data = {"result": jobEnd.jobResult().toString()}
@@ -228,22 +220,22 @@
         if jobEnd.jobResult().toString() == "JobSucceeded":
             level = "info"
             message = "Job {} Ended".format(jobEnd.jobId())
         else:
             level = "warning"
             message = "Job {} Failed".format(jobEnd.jobId())
 
-        self.hub.add_breadcrumb(level=level, message=message, data=data)
+        sentry_sdk.add_breadcrumb(level=level, message=message, data=data)
 
     def onStageSubmitted(self, stageSubmitted):  # noqa: N802,N803
         # type: (Any) -> None
         stage_info = stageSubmitted.stageInfo()
         message = "Stage {} Submitted".format(stage_info.stageId())
         data = {"attemptId": stage_info.attemptId(), "name": stage_info.name()}
-        self.hub.add_breadcrumb(level="info", message=message, data=data)
+        sentry_sdk.add_breadcrumb(level="info", message=message, data=data)
         _set_app_properties()
 
     def onStageCompleted(self, stageCompleted):  # noqa: N802,N803
         # type: (Any) -> None
         from py4j.protocol import Py4JJavaError  # type: ignore
 
         stage_info = stageCompleted.stageInfo()
@@ -256,8 +248,8 @@
             data["reason"] = stage_info.failureReason().get()
             message = "Stage {} Failed".format(stage_info.stageId())
             level = "warning"
         except Py4JJavaError:
             message = "Stage {} Completed".format(stage_info.stageId())
             level = "info"
 
-        self.hub.add_breadcrumb(level=level, message=message, data=data)
+        sentry_sdk.add_breadcrumb(level=level, message=message, data=data)
```

### Comparing `sentry-sdk-2.0.0rc3/sentry_sdk/integrations/spark/spark_worker.py` & `sentry-sdk-2.0.0rc4/sentry_sdk/integrations/spark/spark_worker.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import sys
 
-from sentry_sdk import configure_scope
-from sentry_sdk.hub import Hub
+import sentry_sdk
 from sentry_sdk.integrations import Integration
+from sentry_sdk.scope import Scope
 from sentry_sdk.utils import (
     capture_internal_exceptions,
     exc_info_from_error,
     single_exception_from_error_tuple,
     walk_exception_chain,
     event_hint_with_exc_info,
 )
@@ -27,96 +27,91 @@
     def setup_once():
         # type: () -> None
         import pyspark.daemon as original_daemon
 
         original_daemon.worker_main = _sentry_worker_main
 
 
-def _capture_exception(exc_info, hub):
-    # type: (ExcInfo, Hub) -> None
-    client = hub.client
-
-    client_options = client.options  # type: ignore
+def _capture_exception(exc_info):
+    # type: (ExcInfo) -> None
+    client = sentry_sdk.get_client()
 
     mechanism = {"type": "spark", "handled": False}
 
     exc_info = exc_info_from_error(exc_info)
 
     exc_type, exc_value, tb = exc_info
     rv = []
 
     # On Exception worker will call sys.exit(-1), so we can ignore SystemExit and similar errors
     for exc_type, exc_value, tb in walk_exception_chain(exc_info):
         if exc_type not in (SystemExit, EOFError, ConnectionResetError):
             rv.append(
                 single_exception_from_error_tuple(
-                    exc_type, exc_value, tb, client_options, mechanism
+                    exc_type, exc_value, tb, client.options, mechanism
                 )
             )
 
     if rv:
         rv.reverse()
         hint = event_hint_with_exc_info(exc_info)
         event = {"level": "error", "exception": {"values": rv}}  # type: Event
 
         _tag_task_context()
 
-        hub.capture_event(event, hint=hint)
+        sentry_sdk.capture_event(event, hint=hint)
 
 
 def _tag_task_context():
     # type: () -> None
     from pyspark.taskcontext import TaskContext
 
-    with configure_scope() as scope:
-
-        @scope.add_event_processor
-        def process_event(event, hint):
-            # type: (Event, Hint) -> Optional[Event]
-            with capture_internal_exceptions():
-                integration = Hub.current.get_integration(SparkWorkerIntegration)
-                task_context = TaskContext.get()
+    scope = Scope.get_isolation_scope()
 
-                if integration is None or task_context is None:
-                    return event
+    @scope.add_event_processor
+    def process_event(event, hint):
+        # type: (Event, Hint) -> Optional[Event]
+        with capture_internal_exceptions():
+            integration = sentry_sdk.get_client().get_integration(
+                SparkWorkerIntegration
+            )
+            task_context = TaskContext.get()
 
-                event.setdefault("tags", {}).setdefault(
-                    "stageId", str(task_context.stageId())
-                )
-                event["tags"].setdefault("partitionId", str(task_context.partitionId()))
-                event["tags"].setdefault(
-                    "attemptNumber", str(task_context.attemptNumber())
-                )
-                event["tags"].setdefault(
-                    "taskAttemptId", str(task_context.taskAttemptId())
-                )
+            if integration is None or task_context is None:
+                return event
 
-                if task_context._localProperties:
-                    if "sentry_app_name" in task_context._localProperties:
-                        event["tags"].setdefault(
-                            "app_name", task_context._localProperties["sentry_app_name"]
-                        )
-                        event["tags"].setdefault(
-                            "application_id",
-                            task_context._localProperties["sentry_application_id"],
-                        )
-
-                    if "callSite.short" in task_context._localProperties:
-                        event.setdefault("extra", {}).setdefault(
-                            "callSite", task_context._localProperties["callSite.short"]
-                        )
+            event.setdefault("tags", {}).setdefault(
+                "stageId", str(task_context.stageId())
+            )
+            event["tags"].setdefault("partitionId", str(task_context.partitionId()))
+            event["tags"].setdefault("attemptNumber", str(task_context.attemptNumber()))
+            event["tags"].setdefault("taskAttemptId", str(task_context.taskAttemptId()))
+
+            if task_context._localProperties:
+                if "sentry_app_name" in task_context._localProperties:
+                    event["tags"].setdefault(
+                        "app_name", task_context._localProperties["sentry_app_name"]
+                    )
+                    event["tags"].setdefault(
+                        "application_id",
+                        task_context._localProperties["sentry_application_id"],
+                    )
+
+                if "callSite.short" in task_context._localProperties:
+                    event.setdefault("extra", {}).setdefault(
+                        "callSite", task_context._localProperties["callSite.short"]
+                    )
 
-            return event
+        return event
 
 
 def _sentry_worker_main(*args, **kwargs):
     # type: (*Optional[Any], **Optional[Any]) -> None
     import pyspark.worker as original_worker
 
     try:
         original_worker.main(*args, **kwargs)
     except SystemExit:
-        if Hub.current.get_integration(SparkWorkerIntegration) is not None:
-            hub = Hub.current
+        if sentry_sdk.get_client().get_integration(SparkWorkerIntegration) is not None:
             exc_info = sys.exc_info()
             with capture_internal_exceptions():
-                _capture_exception(exc_info, hub)
+                _capture_exception(exc_info)
```

### Comparing `sentry-sdk-2.0.0rc3/sentry_sdk/integrations/sqlalchemy.py` & `sentry-sdk-2.0.0rc4/sentry_sdk/integrations/sqlalchemy.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 import sentry_sdk
 from sentry_sdk._types import TYPE_CHECKING
 from sentry_sdk.consts import SPANDATA
 from sentry_sdk.db.explain_plan.sqlalchemy import attach_explain_plan_to_span
 from sentry_sdk.integrations import Integration, DidNotEnable
 from sentry_sdk.tracing_utils import add_query_source, record_sql_queries
-from sentry_sdk.utils import capture_internal_exceptions, parse_version
+from sentry_sdk.utils import (
+    capture_internal_exceptions,
+    ensure_integration_enabled,
+    parse_version,
+)
 
 try:
     from sqlalchemy.engine import Engine  # type: ignore
     from sqlalchemy.event import listen  # type: ignore
     from sqlalchemy import __version__ as SQLALCHEMY_VERSION  # type: ignore
 except ImportError:
     raise DidNotEnable("SQLAlchemy not installed.")
@@ -39,21 +43,19 @@
             raise DidNotEnable("SQLAlchemy 1.2 or newer required.")
 
         listen(Engine, "before_cursor_execute", _before_cursor_execute)
         listen(Engine, "after_cursor_execute", _after_cursor_execute)
         listen(Engine, "handle_error", _handle_error)
 
 
+@ensure_integration_enabled(SqlalchemyIntegration)
 def _before_cursor_execute(
     conn, cursor, statement, parameters, context, executemany, *args
 ):
     # type: (Any, Any, Any, Any, Any, bool, *Any) -> None
-    if sentry_sdk.get_client().get_integration(SqlalchemyIntegration) is None:
-        return
-
     ctx_mgr = record_sql_queries(
         cursor,
         statement,
         parameters,
         paramstyle=context and context.dialect and context.dialect.paramstyle or None,
         executemany=executemany,
     )
@@ -73,19 +75,17 @@
                 statement,
                 parameters,
                 options,
             )
         context._sentry_sql_span = span
 
 
+@ensure_integration_enabled(SqlalchemyIntegration)
 def _after_cursor_execute(conn, cursor, statement, parameters, context, *args):
     # type: (Any, Any, Any, Any, Any, *Any) -> None
-    if sentry_sdk.get_client().get_integration(SqlalchemyIntegration) is None:
-        return
-
     ctx_mgr = getattr(
         context, "_sentry_sql_span_manager", None
     )  # type: Optional[ContextManager[Any]]
 
     if ctx_mgr is not None:
         context._sentry_sql_span_manager = None
         ctx_mgr.__exit__(None, None, None)
```

### Comparing `sentry-sdk-2.0.0rc3/sentry_sdk/integrations/starlette.py` & `sentry-sdk-2.0.0rc4/sentry_sdk/integrations/starlette.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,39 +1,40 @@
 import asyncio
 import functools
 from copy import deepcopy
 
+import sentry_sdk
 from sentry_sdk._types import TYPE_CHECKING
 from sentry_sdk.consts import OP
-from sentry_sdk.hub import Hub, _should_send_default_pii
 from sentry_sdk.integrations import DidNotEnable, Integration
 from sentry_sdk.integrations._wsgi_common import (
     _is_json_content_type,
     request_body_within_bounds,
 )
 from sentry_sdk.integrations.asgi import SentryAsgiMiddleware
-from sentry_sdk.scope import Scope
+from sentry_sdk.scope import Scope, should_send_default_pii
 from sentry_sdk.tracing import (
     SOURCE_FOR_STYLE,
     TRANSACTION_SOURCE_COMPONENT,
     TRANSACTION_SOURCE_ROUTE,
 )
 from sentry_sdk.utils import (
     AnnotatedValue,
     capture_internal_exceptions,
+    ensure_integration_enabled,
+    ensure_integration_enabled_async,
     event_from_exception,
     logger,
     parse_version,
     transaction_from_function,
 )
 
 if TYPE_CHECKING:
     from typing import Any, Awaitable, Callable, Dict, Optional, Tuple
 
-    from sentry_sdk.scope import Scope as SentryScope
     from sentry_sdk._types import Event
 
 try:
     import starlette  # type: ignore
     from starlette import __version__ as STARLETTE_VERSION
     from starlette.applications import Starlette  # type: ignore
     from starlette.datastructures import UploadFile  # type: ignore
@@ -100,92 +101,85 @@
 
 def _enable_span_for_middleware(middleware_class):
     # type: (Any) -> type
     old_call = middleware_class.__call__
 
     async def _create_span_call(app, scope, receive, send, **kwargs):
         # type: (Any, Dict[str, Any], Callable[[], Awaitable[Dict[str, Any]]], Callable[[Dict[str, Any]], Awaitable[None]], Any) -> None
-        hub = Hub.current
-        integration = hub.get_integration(StarletteIntegration)
-        if integration is not None:
-            middleware_name = app.__class__.__name__
-
-            # Update transaction name with middleware name
-            name, source = _get_transaction_from_middleware(app, scope, integration)
-            if name is not None:
-                Scope.get_current_scope().set_transaction_name(
-                    name,
-                    source=source,
-                )
+        integration = sentry_sdk.get_client().get_integration(StarletteIntegration)
+        if integration is None:
+            return await old_call(app, scope, receive, send, **kwargs)
 
-            with hub.start_span(
-                op=OP.MIDDLEWARE_STARLETTE, description=middleware_name
-            ) as middleware_span:
-                middleware_span.set_tag("starlette.middleware_name", middleware_name)
-
-                # Creating spans for the "receive" callback
-                async def _sentry_receive(*args, **kwargs):
-                    # type: (*Any, **Any) -> Any
-                    hub = Hub.current
-                    with hub.start_span(
-                        op=OP.MIDDLEWARE_STARLETTE_RECEIVE,
-                        description=getattr(receive, "__qualname__", str(receive)),
-                    ) as span:
-                        span.set_tag("starlette.middleware_name", middleware_name)
-                        return await receive(*args, **kwargs)
-
-                receive_name = getattr(receive, "__name__", str(receive))
-                receive_patched = receive_name == "_sentry_receive"
-                new_receive = _sentry_receive if not receive_patched else receive
-
-                # Creating spans for the "send" callback
-                async def _sentry_send(*args, **kwargs):
-                    # type: (*Any, **Any) -> Any
-                    hub = Hub.current
-                    with hub.start_span(
-                        op=OP.MIDDLEWARE_STARLETTE_SEND,
-                        description=getattr(send, "__qualname__", str(send)),
-                    ) as span:
-                        span.set_tag("starlette.middleware_name", middleware_name)
-                        return await send(*args, **kwargs)
-
-                send_name = getattr(send, "__name__", str(send))
-                send_patched = send_name == "_sentry_send"
-                new_send = _sentry_send if not send_patched else send
+        middleware_name = app.__class__.__name__
 
-                return await old_call(app, scope, new_receive, new_send, **kwargs)
+        # Update transaction name with middleware name
+        name, source = _get_transaction_from_middleware(app, scope, integration)
+        if name is not None:
+            Scope.get_current_scope().set_transaction_name(
+                name,
+                source=source,
+            )
 
-        else:
-            return await old_call(app, scope, receive, send, **kwargs)
+        with sentry_sdk.start_span(
+            op=OP.MIDDLEWARE_STARLETTE, description=middleware_name
+        ) as middleware_span:
+            middleware_span.set_tag("starlette.middleware_name", middleware_name)
+
+            # Creating spans for the "receive" callback
+            async def _sentry_receive(*args, **kwargs):
+                # type: (*Any, **Any) -> Any
+                with sentry_sdk.start_span(
+                    op=OP.MIDDLEWARE_STARLETTE_RECEIVE,
+                    description=getattr(receive, "__qualname__", str(receive)),
+                ) as span:
+                    span.set_tag("starlette.middleware_name", middleware_name)
+                    return await receive(*args, **kwargs)
+
+            receive_name = getattr(receive, "__name__", str(receive))
+            receive_patched = receive_name == "_sentry_receive"
+            new_receive = _sentry_receive if not receive_patched else receive
+
+            # Creating spans for the "send" callback
+            async def _sentry_send(*args, **kwargs):
+                # type: (*Any, **Any) -> Any
+                with sentry_sdk.start_span(
+                    op=OP.MIDDLEWARE_STARLETTE_SEND,
+                    description=getattr(send, "__qualname__", str(send)),
+                ) as span:
+                    span.set_tag("starlette.middleware_name", middleware_name)
+                    return await send(*args, **kwargs)
+
+            send_name = getattr(send, "__name__", str(send))
+            send_patched = send_name == "_sentry_send"
+            new_send = _sentry_send if not send_patched else send
+
+            return await old_call(app, scope, new_receive, new_send, **kwargs)
 
     not_yet_patched = old_call.__name__ not in [
         "_create_span_call",
         "_sentry_authenticationmiddleware_call",
         "_sentry_exceptionmiddleware_call",
     ]
 
     if not_yet_patched:
         middleware_class.__call__ = _create_span_call
 
     return middleware_class
 
 
+@ensure_integration_enabled(StarletteIntegration)
 def _capture_exception(exception, handled=False):
     # type: (BaseException, **Any) -> None
-    hub = Hub.current
-    if hub.get_integration(StarletteIntegration) is None:
-        return
-
     event, hint = event_from_exception(
         exception,
-        client_options=hub.client.options if hub.client else None,
+        client_options=sentry_sdk.get_client().options,
         mechanism={"type": StarletteIntegration.identifier, "handled": handled},
     )
 
-    hub.capture_event(event, hint=hint)
+    sentry_sdk.capture_event(event, hint=hint)
 
 
 def patch_exception_middleware(middleware_class):
     # type: (Any) -> None
     """
     Capture all exceptions in Starlette app and
     also extract user information.
@@ -252,47 +246,44 @@
             # This is why we do it here.
             _add_user_to_sentry_scope(scope)
             await old_call(self, scope, receive, send)
 
         middleware_class.__call__ = _sentry_exceptionmiddleware_call
 
 
+@ensure_integration_enabled(StarletteIntegration)
 def _add_user_to_sentry_scope(scope):
     # type: (Dict[str, Any]) -> None
     """
     Extracts user information from the ASGI scope and
     adds it to Sentry's scope.
     """
     if "user" not in scope:
         return
 
-    if not _should_send_default_pii():
+    if not should_send_default_pii():
         return
 
-    hub = Hub.current
-    if hub.get_integration(StarletteIntegration) is None:
-        return
+    user_info = {}  # type: Dict[str, Any]
+    starlette_user = scope["user"]
 
-    with hub.configure_scope() as sentry_scope:
-        user_info = {}  # type: Dict[str, Any]
-        starlette_user = scope["user"]
-
-        username = getattr(starlette_user, "username", None)
-        if username:
-            user_info.setdefault("username", starlette_user.username)
-
-        user_id = getattr(starlette_user, "id", None)
-        if user_id:
-            user_info.setdefault("id", starlette_user.id)
-
-        email = getattr(starlette_user, "email", None)
-        if email:
-            user_info.setdefault("email", starlette_user.email)
+    username = getattr(starlette_user, "username", None)
+    if username:
+        user_info.setdefault("username", starlette_user.username)
+
+    user_id = getattr(starlette_user, "id", None)
+    if user_id:
+        user_info.setdefault("id", starlette_user.id)
+
+    email = getattr(starlette_user, "email", None)
+    if email:
+        user_info.setdefault("email", starlette_user.email)
 
-        sentry_scope.user = user_info
+    sentry_scope = Scope.get_isolation_scope()
+    sentry_scope.user = user_info
 
 
 def patch_authentication_middleware(middleware_class):
     # type: (Any) -> None
     """
     Add user information to Sentry scope.
     """
@@ -342,19 +333,18 @@
 def patch_asgi_app():
     # type: () -> None
     """
     Instrument Starlette ASGI app using the SentryAsgiMiddleware.
     """
     old_app = Starlette.__call__
 
+    @ensure_integration_enabled_async(StarletteIntegration, old_app)
     async def _sentry_patched_asgi_app(self, scope, receive, send):
         # type: (Starlette, StarletteScope, Receive, Send) -> None
-        integration = Hub.current.get_integration(StarletteIntegration)
-        if integration is None:
-            return await old_app(self, scope, receive, send)
+        integration = sentry_sdk.get_client().get_integration(StarletteIntegration)
 
         middleware = SentryAsgiMiddleware(
             lambda *a, **kw: old_app(self, *a, **kw),
             mechanism_type=StarletteIntegration.identifier,
             transaction_style=integration.transaction_style,
         )
 
@@ -383,94 +373,95 @@
     def _sentry_request_response(func):
         # type: (Callable[[Any], Any]) -> ASGIApp
         old_func = func
 
         is_coroutine = _is_async_callable(old_func)
         if is_coroutine:
 
+            @ensure_integration_enabled_async(StarletteIntegration, old_func)
             async def _sentry_async_func(*args, **kwargs):
                 # type: (*Any, **Any) -> Any
-                hub = Hub.current
-                integration = hub.get_integration(StarletteIntegration)
-                if integration is None:
-                    return await old_func(*args, **kwargs)
+                integration = sentry_sdk.get_client().get_integration(
+                    StarletteIntegration
+                )
 
                 request = args[0]
 
                 _set_transaction_name_and_source(
                     Scope.get_current_scope(), integration.transaction_style, request
                 )
 
-                with hub.configure_scope() as sentry_scope:
-                    extractor = StarletteRequestExtractor(request)
-                    info = await extractor.extract_request_info()
-
-                    def _make_request_event_processor(req, integration):
-                        # type: (Any, Any) -> Callable[[Event, dict[str, Any]], Event]
-                        def event_processor(event, hint):
-                            # type: (Event, Dict[str, Any]) -> Event
-
-                            # Add info from request to event
-                            request_info = event.get("request", {})
-                            if info:
-                                if "cookies" in info:
-                                    request_info["cookies"] = info["cookies"]
-                                if "data" in info:
-                                    request_info["data"] = info["data"]
-                            event["request"] = deepcopy(request_info)
+                sentry_scope = Scope.get_isolation_scope()
+                extractor = StarletteRequestExtractor(request)
+                info = await extractor.extract_request_info()
+
+                def _make_request_event_processor(req, integration):
+                    # type: (Any, Any) -> Callable[[Event, dict[str, Any]], Event]
+                    def event_processor(event, hint):
+                        # type: (Event, Dict[str, Any]) -> Event
+
+                        # Add info from request to event
+                        request_info = event.get("request", {})
+                        if info:
+                            if "cookies" in info:
+                                request_info["cookies"] = info["cookies"]
+                            if "data" in info:
+                                request_info["data"] = info["data"]
+                        event["request"] = deepcopy(request_info)
 
-                            return event
+                        return event
 
-                        return event_processor
+                    return event_processor
 
                 sentry_scope._name = StarletteIntegration.identifier
                 sentry_scope.add_event_processor(
                     _make_request_event_processor(request, integration)
                 )
 
                 return await old_func(*args, **kwargs)
 
             func = _sentry_async_func
+
         else:
 
+            @ensure_integration_enabled(StarletteIntegration, old_func)
             def _sentry_sync_func(*args, **kwargs):
                 # type: (*Any, **Any) -> Any
-                hub = Hub.current
-                integration = hub.get_integration(StarletteIntegration)
-                if integration is None:
-                    return old_func(*args, **kwargs)
-
-                with hub.configure_scope() as sentry_scope:
-                    if sentry_scope.profile is not None:
-                        sentry_scope.profile.update_active_thread_id()
+                integration = sentry_sdk.get_client().get_integration(
+                    StarletteIntegration
+                )
+                sentry_scope = Scope.get_isolation_scope()
 
-                    request = args[0]
+                if sentry_scope.profile is not None:
+                    sentry_scope.profile.update_active_thread_id()
 
-                    _set_transaction_name_and_source(
-                        sentry_scope, integration.transaction_style, request
-                    )
+                request = args[0]
 
-                    extractor = StarletteRequestExtractor(request)
-                    cookies = extractor.extract_cookies_from_request()
+                _set_transaction_name_and_source(
+                    sentry_scope, integration.transaction_style, request
+                )
+
+                extractor = StarletteRequestExtractor(request)
+                cookies = extractor.extract_cookies_from_request()
 
-                    def _make_request_event_processor(req, integration):
-                        # type: (Any, Any) -> Callable[[Event, dict[str, Any]], Event]
-                        def event_processor(event, hint):
-                            # type: (Event, dict[str, Any]) -> Event
+                def _make_request_event_processor(req, integration):
+                    # type: (Any, Any) -> Callable[[Event, dict[str, Any]], Event]
+                    def event_processor(event, hint):
+                        # type: (Event, dict[str, Any]) -> Event
 
-                            # Extract information from request
-                            request_info = event.get("request", {})
-                            if cookies:
-                                request_info["cookies"] = cookies
+                        # Extract information from request
+                        request_info = event.get("request", {})
+                        if cookies:
+                            request_info["cookies"] = cookies
 
-                            event["request"] = deepcopy(request_info)
+                        event["request"] = deepcopy(request_info)
 
-                            return event
+                        return event
 
-                        return event_processor
+                    return event_processor
 
                 sentry_scope._name = StarletteIntegration.identifier
                 sentry_scope.add_event_processor(
                     _make_request_event_processor(request, integration)
                 )
 
                 return old_func(*args, **kwargs)
@@ -503,16 +494,15 @@
 
     if not_yet_patched:
 
         def _sentry_jinja2templates_init(self, *args, **kwargs):
             # type: (Jinja2Templates, *Any, **Any) -> None
             def add_sentry_trace_meta(request):
                 # type: (Request) -> Dict[str, Any]
-                hub = Hub.current
-                trace_meta = Markup(hub.trace_propagation_meta())
+                trace_meta = Markup(Scope.get_current_scope().trace_propagation_meta())
                 return {
                     "sentry_trace_meta": trace_meta,
                 }
 
             kwargs.setdefault("context_processors", [])
 
             if add_sentry_trace_meta not in kwargs["context_processors"]:
@@ -533,35 +523,29 @@
 
     def __init__(self, request):
         # type: (StarletteRequestExtractor, Request) -> None
         self.request = request
 
     def extract_cookies_from_request(self):
         # type: (StarletteRequestExtractor) -> Optional[Dict[str, Any]]
-        client = Hub.current.client
-        if client is None:
-            return None
-
         cookies = None  # type: Optional[Dict[str, Any]]
-        if _should_send_default_pii():
+        if should_send_default_pii():
             cookies = self.cookies()
 
         return cookies
 
     async def extract_request_info(self):
         # type: (StarletteRequestExtractor) -> Optional[Dict[str, Any]]
-        client = Hub.current.client
-        if client is None:
-            return None
+        client = sentry_sdk.get_client()
 
         request_info = {}  # type: Dict[str, Any]
 
         with capture_internal_exceptions():
             # Add cookies
-            if _should_send_default_pii():
+            if should_send_default_pii():
                 request_info["cookies"] = self.cookies()
 
             # If there is no body, just return the cookies
             content_length = await self.content_length()
             if not content_length:
                 return request_info
 
@@ -644,15 +628,15 @@
         if match[0] == Match.FULL:
             return route.path
 
     return None
 
 
 def _set_transaction_name_and_source(scope, transaction_style, request):
-    # type: (SentryScope, str, Any) -> None
+    # type: (Scope, str, Any) -> None
     name = None
     source = SOURCE_FOR_STYLE[transaction_style]
 
     if transaction_style == "endpoint":
         endpoint = request.scope.get("endpoint")
         if endpoint:
             name = transaction_from_function(endpoint) or None
```

### Comparing `sentry-sdk-2.0.0rc3/sentry_sdk/integrations/starlite.py` & `sentry-sdk-2.0.0rc4/sentry_sdk/integrations/starlite.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,35 +1,42 @@
 from typing import TYPE_CHECKING
 
+import sentry_sdk
 from sentry_sdk.consts import OP
-from sentry_sdk.hub import Hub, _should_send_default_pii
 from sentry_sdk.integrations import DidNotEnable, Integration
 from sentry_sdk.integrations.asgi import SentryAsgiMiddleware
+from sentry_sdk.scope import Scope as SentryScope, should_send_default_pii
 from sentry_sdk.tracing import SOURCE_FOR_STYLE, TRANSACTION_SOURCE_ROUTE
-from sentry_sdk.utils import event_from_exception, transaction_from_function
+from sentry_sdk.utils import (
+    ensure_integration_enabled,
+    ensure_integration_enabled_async,
+    event_from_exception,
+    transaction_from_function,
+)
 
 try:
     from starlite import Request, Starlite, State  # type: ignore
     from starlite.handlers.base import BaseRouteHandler  # type: ignore
     from starlite.middleware import DefineMiddleware  # type: ignore
     from starlite.plugins.base import get_plugin_for_value  # type: ignore
     from starlite.routes.http import HTTPRoute  # type: ignore
     from starlite.utils import ConnectionDataExtractor, is_async_callable, Ref  # type: ignore
     from pydantic import BaseModel  # type: ignore
 
     if TYPE_CHECKING:
         from typing import Any, Dict, List, Optional, Union
         from starlite.types import (  # type: ignore
             ASGIApp,
+            Hint,
             HTTPReceiveMessage,
             HTTPScope,
             Message,
             Middleware,
             Receive,
-            Scope,
+            Scope as StarliteScope,
             Send,
             WebSocketReceiveMessage,
         )
         from starlite import MiddlewareProtocol
         from sentry_sdk._types import Event
 except ImportError:
     raise DidNotEnable("Starlite is not installed")
@@ -110,136 +117,132 @@
 
     if isinstance(middleware, DefineMiddleware):
         old_call: "ASGIApp" = middleware.middleware.__call__
     else:
         old_call = middleware.__call__
 
     async def _create_span_call(
-        self: "MiddlewareProtocol", scope: "Scope", receive: "Receive", send: "Send"
+        self: "MiddlewareProtocol",
+        scope: "StarliteScope",
+        receive: "Receive",
+        send: "Send",
     ) -> None:
-        hub = Hub.current
-        integration = hub.get_integration(StarliteIntegration)
-        if integration is not None:
-            middleware_name = self.__class__.__name__
-            with hub.start_span(
-                op=OP.MIDDLEWARE_STARLITE, description=middleware_name
-            ) as middleware_span:
-                middleware_span.set_tag("starlite.middleware_name", middleware_name)
-
-                # Creating spans for the "receive" callback
-                async def _sentry_receive(
-                    *args: "Any", **kwargs: "Any"
-                ) -> "Union[HTTPReceiveMessage, WebSocketReceiveMessage]":
-                    hub = Hub.current
-                    with hub.start_span(
-                        op=OP.MIDDLEWARE_STARLITE_RECEIVE,
-                        description=getattr(receive, "__qualname__", str(receive)),
-                    ) as span:
-                        span.set_tag("starlite.middleware_name", middleware_name)
-                        return await receive(*args, **kwargs)
-
-                receive_name = getattr(receive, "__name__", str(receive))
-                receive_patched = receive_name == "_sentry_receive"
-                new_receive = _sentry_receive if not receive_patched else receive
-
-                # Creating spans for the "send" callback
-                async def _sentry_send(message: "Message") -> None:
-                    hub = Hub.current
-                    with hub.start_span(
-                        op=OP.MIDDLEWARE_STARLITE_SEND,
-                        description=getattr(send, "__qualname__", str(send)),
-                    ) as span:
-                        span.set_tag("starlite.middleware_name", middleware_name)
-                        return await send(message)
-
-                send_name = getattr(send, "__name__", str(send))
-                send_patched = send_name == "_sentry_send"
-                new_send = _sentry_send if not send_patched else send
-
-                return await old_call(self, scope, new_receive, new_send)
-        else:
+        if sentry_sdk.get_client().get_integration(StarliteIntegration) is None:
             return await old_call(self, scope, receive, send)
 
+        middleware_name = self.__class__.__name__
+        with sentry_sdk.start_span(
+            op=OP.MIDDLEWARE_STARLITE, description=middleware_name
+        ) as middleware_span:
+            middleware_span.set_tag("starlite.middleware_name", middleware_name)
+
+            # Creating spans for the "receive" callback
+            async def _sentry_receive(
+                *args: "Any", **kwargs: "Any"
+            ) -> "Union[HTTPReceiveMessage, WebSocketReceiveMessage]":
+                with sentry_sdk.start_span(
+                    op=OP.MIDDLEWARE_STARLITE_RECEIVE,
+                    description=getattr(receive, "__qualname__", str(receive)),
+                ) as span:
+                    span.set_tag("starlite.middleware_name", middleware_name)
+                    return await receive(*args, **kwargs)
+
+            receive_name = getattr(receive, "__name__", str(receive))
+            receive_patched = receive_name == "_sentry_receive"
+            new_receive = _sentry_receive if not receive_patched else receive
+
+            # Creating spans for the "send" callback
+            async def _sentry_send(message: "Message") -> None:
+                with sentry_sdk.start_span(
+                    op=OP.MIDDLEWARE_STARLITE_SEND,
+                    description=getattr(send, "__qualname__", str(send)),
+                ) as span:
+                    span.set_tag("starlite.middleware_name", middleware_name)
+                    return await send(message)
+
+            send_name = getattr(send, "__name__", str(send))
+            send_patched = send_name == "_sentry_send"
+            new_send = _sentry_send if not send_patched else send
+
+            return await old_call(self, scope, new_receive, new_send)
+
     not_yet_patched = old_call.__name__ not in ["_create_span_call"]
 
     if not_yet_patched:
         if isinstance(middleware, DefineMiddleware):
             middleware.middleware.__call__ = _create_span_call
         else:
             middleware.__call__ = _create_span_call
 
     return middleware
 
 
 def patch_http_route_handle() -> None:
     old_handle = HTTPRoute.handle
 
+    @ensure_integration_enabled_async(StarliteIntegration, old_handle)
     async def handle_wrapper(
         self: "HTTPRoute", scope: "HTTPScope", receive: "Receive", send: "Send"
     ) -> None:
-        hub = Hub.current
-        integration: StarliteIntegration = hub.get_integration(StarliteIntegration)
-        if integration is None:
-            return await old_handle(self, scope, receive, send)
-
-        with hub.configure_scope() as sentry_scope:
-            request: "Request[Any, Any]" = scope["app"].request_class(
-                scope=scope, receive=receive, send=send
+
+        sentry_scope = SentryScope.get_isolation_scope()
+        request: "Request[Any, Any]" = scope["app"].request_class(
+            scope=scope, receive=receive, send=send
+        )
+        extracted_request_data = ConnectionDataExtractor(
+            parse_body=True, parse_query=True
+        )(request)
+        body = extracted_request_data.pop("body")
+
+        request_data = await body
+
+        def event_processor(event: "Event", _: "Hint") -> "Event":
+            route_handler = scope.get("route_handler")
+
+            request_info = event.get("request", {})
+            request_info["content_length"] = len(scope.get("_body", b""))
+            if should_send_default_pii():
+                request_info["cookies"] = extracted_request_data["cookies"]
+            if request_data is not None:
+                request_info["data"] = request_data
+
+            func = None
+            if route_handler.name is not None:
+                tx_name = route_handler.name
+            elif isinstance(route_handler.fn, Ref):
+                func = route_handler.fn.value
+            else:
+                func = route_handler.fn
+            if func is not None:
+                tx_name = transaction_from_function(func)
+
+            tx_info = {"source": SOURCE_FOR_STYLE["endpoint"]}
+
+            if not tx_name:
+                tx_name = _DEFAULT_TRANSACTION_NAME
+                tx_info = {"source": TRANSACTION_SOURCE_ROUTE}
+
+            event.update(
+                {
+                    "request": request_info,
+                    "transaction": tx_name,
+                    "transaction_info": tx_info,
+                }
             )
-            extracted_request_data = ConnectionDataExtractor(
-                parse_body=True, parse_query=True
-            )(request)
-            body = extracted_request_data.pop("body")
-
-            request_data = await body
-
-            def event_processor(event: "Event", _: "Dict[str, Any]") -> "Event":
-                route_handler = scope.get("route_handler")
-
-                request_info = event.get("request", {})
-                request_info["content_length"] = len(scope.get("_body", b""))
-                if _should_send_default_pii():
-                    request_info["cookies"] = extracted_request_data["cookies"]
-                if request_data is not None:
-                    request_info["data"] = request_data
-
-                func = None
-                if route_handler.name is not None:
-                    tx_name = route_handler.name
-                elif isinstance(route_handler.fn, Ref):
-                    func = route_handler.fn.value
-                else:
-                    func = route_handler.fn
-                if func is not None:
-                    tx_name = transaction_from_function(func)
-
-                tx_info = {"source": SOURCE_FOR_STYLE["endpoint"]}
-
-                if not tx_name:
-                    tx_name = _DEFAULT_TRANSACTION_NAME
-                    tx_info = {"source": TRANSACTION_SOURCE_ROUTE}
-
-                event.update(
-                    {
-                        "request": request_info,
-                        "transaction": tx_name,
-                        "transaction_info": tx_info,
-                    }
-                )
-                return event
+            return event
 
-            sentry_scope._name = StarliteIntegration.identifier
-            sentry_scope.add_event_processor(event_processor)
+        sentry_scope._name = StarliteIntegration.identifier
+        sentry_scope.add_event_processor(event_processor)
 
-            return await old_handle(self, scope, receive, send)
+        return await old_handle(self, scope, receive, send)
 
     HTTPRoute.handle = handle_wrapper
 
 
-def retrieve_user_from_scope(scope: "Scope") -> "Optional[Dict[str, Any]]":
+def retrieve_user_from_scope(scope: "StarliteScope") -> "Optional[Dict[str, Any]]":
     scope_user = scope.get("user", {})
     if not scope_user:
         return None
     if isinstance(scope_user, dict):
         return scope_user
     if isinstance(scope_user, BaseModel):
         return scope_user.dict()
@@ -249,26 +252,23 @@
     plugin = get_plugin_for_value(scope_user)
     if plugin and not is_async_callable(plugin.to_dict):
         return plugin.to_dict(scope_user)
 
     return None
 
 
-def exception_handler(exc: Exception, scope: "Scope", _: "State") -> None:
-    hub = Hub.current
-    if hub.get_integration(StarliteIntegration) is None:
-        return
-
+@ensure_integration_enabled(StarliteIntegration)
+def exception_handler(exc: Exception, scope: "StarliteScope", _: "State") -> None:
     user_info: "Optional[Dict[str, Any]]" = None
-    if _should_send_default_pii():
+    if should_send_default_pii():
         user_info = retrieve_user_from_scope(scope)
     if user_info and isinstance(user_info, dict):
-        with hub.configure_scope() as sentry_scope:
-            sentry_scope.set_user(user_info)
+        sentry_scope = SentryScope.get_isolation_scope()
+        sentry_scope.set_user(user_info)
 
     event, hint = event_from_exception(
         exc,
-        client_options=hub.client.options if hub.client else None,
+        client_options=sentry_sdk.get_client().options,
         mechanism={"type": StarliteIntegration.identifier, "handled": False},
     )
 
-    hub.capture_event(event, hint=hint)
+    sentry_sdk.capture_event(event, hint=hint)
```

### Comparing `sentry-sdk-2.0.0rc3/sentry_sdk/integrations/stdlib.py` & `sentry-sdk-2.0.0rc4/sentry_sdk/integrations/stdlib.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc3/sentry_sdk/integrations/strawberry.py` & `sentry-sdk-2.0.0rc4/sentry_sdk/integrations/strawberry.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 import hashlib
 from inspect import isawaitable
 
-from sentry_sdk import configure_scope, start_span
+import sentry_sdk
 from sentry_sdk.consts import OP
 from sentry_sdk.integrations import Integration, DidNotEnable
 from sentry_sdk.integrations.logging import ignore_logger
-from sentry_sdk.hub import Hub, _should_send_default_pii
+from sentry_sdk.scope import Scope, should_send_default_pii
 from sentry_sdk.utils import (
     capture_internal_exceptions,
+    ensure_integration_enabled,
+    ensure_integration_enabled_async,
     event_from_exception,
     logger,
     package_version,
     _get_installed_modules,
 )
 from sentry_sdk._types import TYPE_CHECKING
 
@@ -79,20 +81,18 @@
         _patch_views()
 
 
 def _patch_schema_init():
     # type: () -> None
     old_schema_init = Schema.__init__
 
+    @ensure_integration_enabled(StrawberryIntegration, old_schema_init)
     def _sentry_patched_schema_init(self, *args, **kwargs):
         # type: (Schema, Any, Any) -> None
-        integration = Hub.current.get_integration(StrawberryIntegration)
-        if integration is None:
-            return old_schema_init(self, *args, **kwargs)
-
+        integration = sentry_sdk.get_client().get_integration(StrawberryIntegration)
         extensions = kwargs.get("extensions") or []
 
         if integration.async_execution is not None:
             should_use_async_extension = integration.async_execution
         else:
             # try to figure it out ourselves
             should_use_async_extension = _guess_if_using_async(extensions)
@@ -161,29 +161,27 @@
             operation_type = "subscription"
             op = OP.GRAPHQL_SUBSCRIPTION
 
         description = operation_type
         if self._operation_name:
             description += " {}".format(self._operation_name)
 
-        Hub.current.add_breadcrumb(
+        sentry_sdk.add_breadcrumb(
             category="graphql.operation",
             data={
                 "operation_name": self._operation_name,
                 "operation_type": operation_type,
             },
         )
 
-        with configure_scope() as scope:
-            if scope.span:
-                self.graphql_span = scope.span.start_child(
-                    op=op, description=description
-                )
-            else:
-                self.graphql_span = start_span(op=op, description=description)
+        scope = Scope.get_isolation_scope()
+        if scope.span:
+            self.graphql_span = scope.span.start_child(op=op, description=description)
+        else:
+            self.graphql_span = sentry_sdk.start_span(op=op, description=description)
 
         self.graphql_span.set_data("graphql.operation.type", operation_type)
         self.graphql_span.set_data("graphql.operation.name", self._operation_name)
         self.graphql_span.set_data("graphql.document", self.execution_context.query)
         self.graphql_span.set_data("graphql.resource_name", self._resource_name)
 
         yield
@@ -261,47 +259,35 @@
 
 
 def _patch_execute():
     # type: () -> None
     old_execute_async = strawberry_schema.execute
     old_execute_sync = strawberry_schema.execute_sync
 
+    @ensure_integration_enabled_async(StrawberryIntegration, old_execute_async)
     async def _sentry_patched_execute_async(*args, **kwargs):
         # type: (Any, Any) -> ExecutionResult
-        hub = Hub.current
-        integration = hub.get_integration(StrawberryIntegration)
-        if integration is None:
-            return await old_execute_async(*args, **kwargs)
-
         result = await old_execute_async(*args, **kwargs)
 
         if "execution_context" in kwargs and result.errors:
-            with hub.configure_scope() as scope:
-                event_processor = _make_request_event_processor(
-                    kwargs["execution_context"]
-                )
-                scope.add_event_processor(event_processor)
+            scope = Scope.get_isolation_scope()
+            event_processor = _make_request_event_processor(kwargs["execution_context"])
+            scope.add_event_processor(event_processor)
 
         return result
 
+    @ensure_integration_enabled(StrawberryIntegration, old_execute_sync)
     def _sentry_patched_execute_sync(*args, **kwargs):
         # type: (Any, Any) -> ExecutionResult
-        hub = Hub.current
-        integration = hub.get_integration(StrawberryIntegration)
-        if integration is None:
-            return old_execute_sync(*args, **kwargs)
-
         result = old_execute_sync(*args, **kwargs)
 
         if "execution_context" in kwargs and result.errors:
-            with hub.configure_scope() as scope:
-                event_processor = _make_request_event_processor(
-                    kwargs["execution_context"]
-                )
-                scope.add_event_processor(event_processor)
+            scope = Scope.get_isolation_scope()
+            event_processor = _make_request_event_processor(kwargs["execution_context"])
+            scope.add_event_processor(event_processor)
 
         return result
 
     strawberry_schema.execute = _sentry_patched_execute_async
     strawberry_schema.execute_sync = _sentry_patched_execute_sync
 
 
@@ -316,39 +302,35 @@
         _sentry_patched_handle_errors(self, errors, response_data)
 
     def _sentry_patched_sync_view_handle_errors(self, errors, response_data):
         # type: (Any, List[GraphQLError], GraphQLHTTPResponse) -> None
         old_sync_view_handle_errors(self, errors, response_data)
         _sentry_patched_handle_errors(self, errors, response_data)
 
+    @ensure_integration_enabled(StrawberryIntegration)
     def _sentry_patched_handle_errors(self, errors, response_data):
         # type: (Any, List[GraphQLError], GraphQLHTTPResponse) -> None
-        hub = Hub.current
-        integration = hub.get_integration(StrawberryIntegration)
-        if integration is None:
-            return
-
         if not errors:
             return
 
-        with hub.configure_scope() as scope:
-            event_processor = _make_response_event_processor(response_data)
-            scope.add_event_processor(event_processor)
+        scope = Scope.get_isolation_scope()
+        event_processor = _make_response_event_processor(response_data)
+        scope.add_event_processor(event_processor)
 
         with capture_internal_exceptions():
             for error in errors:
                 event, hint = event_from_exception(
                     error,
-                    client_options=hub.client.options if hub.client else None,
+                    client_options=sentry_sdk.get_client().options,
                     mechanism={
-                        "type": integration.identifier,
+                        "type": StrawberryIntegration.identifier,
                         "handled": False,
                     },
                 )
-                hub.capture_event(event, hint=hint)
+                sentry_sdk.capture_event(event, hint=hint)
 
     async_base_view.AsyncBaseHTTPView._handle_errors = (
         _sentry_patched_async_view_handle_errors
     )
     sync_base_view.SyncBaseHTTPView._handle_errors = (
         _sentry_patched_sync_view_handle_errors
     )
@@ -356,15 +338,15 @@
 
 def _make_request_event_processor(execution_context):
     # type: (ExecutionContext) -> EventProcessor
 
     def inner(event, hint):
         # type: (Event, dict[str, Any]) -> Event
         with capture_internal_exceptions():
-            if _should_send_default_pii():
+            if should_send_default_pii():
                 request_data = event.setdefault("request", {})
                 request_data["api_target"] = "graphql"
 
                 if not request_data.get("data"):
                     data = {"query": execution_context.query}
 
                     if execution_context.variables:
@@ -387,15 +369,15 @@
 
 def _make_response_event_processor(response_data):
     # type: (GraphQLHTTPResponse) -> EventProcessor
 
     def inner(event, hint):
         # type: (Event, dict[str, Any]) -> Event
         with capture_internal_exceptions():
-            if _should_send_default_pii():
+            if should_send_default_pii():
                 contexts = event.setdefault("contexts", {})
                 contexts["response"] = {"data": response_data}
 
         return event
 
     return inner
```

### Comparing `sentry-sdk-2.0.0rc3/sentry_sdk/integrations/threading.py` & `sentry-sdk-2.0.0rc4/sentry_sdk/integrations/threading.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from threading import Thread, current_thread
 
 import sentry_sdk
 from sentry_sdk._types import TYPE_CHECKING
 from sentry_sdk.integrations import Integration
 from sentry_sdk.scope import Scope, use_isolation_scope, use_scope
 from sentry_sdk.utils import (
+    ensure_integration_enabled,
     event_from_exception,
     capture_internal_exceptions,
     logger,
     reraise,
 )
 
 if TYPE_CHECKING:
@@ -45,38 +46,38 @@
 
     @staticmethod
     def setup_once():
         # type: () -> None
         old_start = Thread.start
 
         @wraps(old_start)
+        @ensure_integration_enabled(ThreadingIntegration, old_start)
         def sentry_start(self, *a, **kw):
             # type: (Thread, *Any, **Any) -> Any
             integration = sentry_sdk.get_client().get_integration(ThreadingIntegration)
-            if integration is not None:
-                if integration.propagate_scope:
-                    isolation_scope = sentry_sdk.Scope.get_isolation_scope()
-                    current_scope = sentry_sdk.Scope.get_current_scope()
-                else:
-                    isolation_scope = None
-                    current_scope = None
-
-                # Patching instance methods in `start()` creates a reference cycle if
-                # done in a naive way. See
-                # https://github.com/getsentry/sentry-python/pull/434
-                #
-                # In threading module, using current_thread API will access current thread instance
-                # without holding it to avoid a reference cycle in an easier way.
-                with capture_internal_exceptions():
-                    new_run = _wrap_run(
-                        isolation_scope,
-                        current_scope,
-                        getattr(self.run, "__func__", self.run),
-                    )
-                    self.run = new_run  # type: ignore
+            if integration.propagate_scope:
+                isolation_scope = sentry_sdk.Scope.get_isolation_scope()
+                current_scope = sentry_sdk.Scope.get_current_scope()
+            else:
+                isolation_scope = None
+                current_scope = None
+
+            # Patching instance methods in `start()` creates a reference cycle if
+            # done in a naive way. See
+            # https://github.com/getsentry/sentry-python/pull/434
+            #
+            # In threading module, using current_thread API will access current thread instance
+            # without holding it to avoid a reference cycle in an easier way.
+            with capture_internal_exceptions():
+                new_run = _wrap_run(
+                    isolation_scope,
+                    current_scope,
+                    getattr(self.run, "__func__", self.run),
+                )
+                self.run = new_run  # type: ignore
 
             return old_start(self, *a, **kw)
 
         Thread.start = sentry_start  # type: ignore
 
 
 def _wrap_run(isolation_scope_to_use, current_scope_to_use, old_run_func):
```

### Comparing `sentry-sdk-2.0.0rc3/sentry_sdk/integrations/tornado.py` & `sentry-sdk-2.0.0rc4/sentry_sdk/integrations/tornado.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 import weakref
 import contextlib
 from inspect import iscoroutinefunction
 
+import sentry_sdk
 from sentry_sdk.api import continue_trace
 from sentry_sdk.consts import OP
-from sentry_sdk.hub import Hub, _should_send_default_pii
+from sentry_sdk.scope import should_send_default_pii
 from sentry_sdk.tracing import (
     TRANSACTION_SOURCE_COMPONENT,
     TRANSACTION_SOURCE_ROUTE,
 )
 from sentry_sdk.utils import (
     HAS_REAL_CONTEXTVARS,
     CONTEXTVARS_ERROR_MESSAGE,
+    ensure_integration_enabled,
     event_from_exception,
     capture_internal_exceptions,
     transaction_from_function,
 )
 from sentry_sdk.integrations import Integration, DidNotEnable
 from sentry_sdk.integrations._wsgi_common import (
     RequestExtractor,
@@ -45,16 +47,16 @@
 
 class TornadoIntegration(Integration):
     identifier = "tornado"
 
     @staticmethod
     def setup_once():
         # type: () -> None
-        if TORNADO_VERSION < (5, 0):
-            raise DidNotEnable("Tornado 5+ required")
+        if TORNADO_VERSION < (6, 0):
+            raise DidNotEnable("Tornado 6.0+ required")
 
         if not HAS_REAL_CONTEXTVARS:
             # Tornado is async. We better have contextvars or we're going to leak
             # state between requests.
             raise DidNotEnable(
                 "The tornado integration for Sentry requires Python 3.7+ or the aiocontextvars package"
                 + CONTEXTVARS_ERROR_MESSAGE
@@ -94,65 +96,58 @@
 
         RequestHandler.log_exception = sentry_log_exception
 
 
 @contextlib.contextmanager
 def _handle_request_impl(self):
     # type: (RequestHandler) -> Generator[None, None, None]
-    hub = Hub.current
-    integration = hub.get_integration(TornadoIntegration)
+    integration = sentry_sdk.get_client().get_integration(TornadoIntegration)
 
     if integration is None:
         yield
 
     weak_handler = weakref.ref(self)
 
-    with Hub(hub) as hub:
+    with sentry_sdk.isolation_scope() as scope:
         headers = self.request.headers
 
-        with hub.configure_scope() as scope:
-            scope.clear_breadcrumbs()
-            processor = _make_event_processor(weak_handler)
-            scope.add_event_processor(processor)
+        scope.clear_breadcrumbs()
+        processor = _make_event_processor(weak_handler)
+        scope.add_event_processor(processor)
 
         transaction = continue_trace(
             headers,
             op=OP.HTTP_SERVER,
             # Like with all other integrations, this is our
             # fallback transaction in case there is no route.
             # sentry_urldispatcher_resolve is responsible for
             # setting a transaction name later.
             name="generic Tornado request",
             source=TRANSACTION_SOURCE_ROUTE,
         )
 
-        with hub.start_transaction(
+        with sentry_sdk.start_transaction(
             transaction, custom_sampling_context={"tornado_request": self.request}
         ):
             yield
 
 
+@ensure_integration_enabled(TornadoIntegration)
 def _capture_exception(ty, value, tb):
     # type: (type, BaseException, Any) -> None
-    hub = Hub.current
-    if hub.get_integration(TornadoIntegration) is None:
-        return
     if isinstance(value, HTTPError):
         return
 
-    # If an integration is there, a client has to be there.
-    client = hub.client  # type: Any
-
     event, hint = event_from_exception(
         (ty, value, tb),
-        client_options=client.options,
+        client_options=sentry_sdk.get_client().options,
         mechanism={"type": "tornado", "handled": False},
     )
 
-    hub.capture_event(event, hint=hint)
+    sentry_sdk.capture_event(event, hint=hint)
 
 
 def _make_event_processor(weak_handler):
     # type: (Callable[[], RequestHandler]) -> EventProcessor
     def tornado_processor(event, hint):
         # type: (Event, dict[str, Any]) -> Event
         handler = weak_handler()
@@ -180,15 +175,15 @@
 
             request_info["query_string"] = request.query
             request_info["method"] = request.method
             request_info["env"] = {"REMOTE_ADDR": request.remote_ip}
             request_info["headers"] = _filter_headers(dict(request.headers))
 
         with capture_internal_exceptions():
-            if handler.current_user and _should_send_default_pii():
+            if handler.current_user and should_send_default_pii():
                 event.setdefault("user", {}).setdefault("is_authenticated", True)
 
         return event
 
     return tornado_processor
```

### Comparing `sentry-sdk-2.0.0rc3/sentry_sdk/integrations/trytond.py` & `sentry-sdk-2.0.0rc4/sentry_sdk/integrations/trytond.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,49 +1,41 @@
-import sentry_sdk.hub
-import sentry_sdk.utils
-import sentry_sdk.integrations
-import sentry_sdk.integrations.wsgi
-from sentry_sdk._types import TYPE_CHECKING
+import sentry_sdk
+from sentry_sdk.integrations import Integration
+from sentry_sdk.integrations.wsgi import SentryWsgiMiddleware
+from sentry_sdk.utils import ensure_integration_enabled, event_from_exception
 
 from trytond.exceptions import TrytonException  # type: ignore
 from trytond.wsgi import app  # type: ignore
 
-if TYPE_CHECKING:
-    from typing import Any
-
 
 # TODO: trytond-worker, trytond-cron and trytond-admin intergations
 
 
-class TrytondWSGIIntegration(sentry_sdk.integrations.Integration):
+class TrytondWSGIIntegration(Integration):
     identifier = "trytond_wsgi"
 
     def __init__(self):  # type: () -> None
         pass
 
     @staticmethod
     def setup_once():  # type: () -> None
-        app.wsgi_app = sentry_sdk.integrations.wsgi.SentryWsgiMiddleware(app.wsgi_app)
+        app.wsgi_app = SentryWsgiMiddleware(app.wsgi_app)
 
+        @ensure_integration_enabled(TrytondWSGIIntegration)
         def error_handler(e):  # type: (Exception) -> None
-            hub = sentry_sdk.hub.Hub.current
-
-            if hub.get_integration(TrytondWSGIIntegration) is None:
-                return
-            elif isinstance(e, TrytonException):
+            if isinstance(e, TrytonException):
                 return
             else:
-                # If an integration is there, a client has to be there.
-                client = hub.client  # type: Any
-                event, hint = sentry_sdk.utils.event_from_exception(
+                client = sentry_sdk.get_client()
+                event, hint = event_from_exception(
                     e,
                     client_options=client.options,
                     mechanism={"type": "trytond", "handled": False},
                 )
-                hub.capture_event(event, hint=hint)
+                sentry_sdk.capture_event(event, hint=hint)
 
         # Expected error handlers signature was changed
         # when the error_handler decorator was introduced
         # in Tryton-5.4
         if hasattr(app, "error_handler"):
 
             @app.error_handler
```

### Comparing `sentry-sdk-2.0.0rc3/sentry_sdk/integrations/wsgi.py` & `sentry-sdk-2.0.0rc4/sentry_sdk/integrations/wsgi.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc3/sentry_sdk/metrics.py` & `sentry-sdk-2.0.0rc4/sentry_sdk/metrics.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc3/sentry_sdk/monitor.py` & `sentry-sdk-2.0.0rc4/sentry_sdk/monitor.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc3/sentry_sdk/profiler.py` & `sentry-sdk-2.0.0rc4/sentry_sdk/profiler.py`

 * *Files 3% similar despite different names*

```diff
@@ -39,14 +39,16 @@
 import sentry_sdk
 from sentry_sdk._compat import PY311
 from sentry_sdk._lru_cache import LRUCache
 from sentry_sdk._types import TYPE_CHECKING
 from sentry_sdk.utils import (
     capture_internal_exception,
     filename_for_module,
+    get_current_thread_meta,
+    is_gevent,
     is_valid_sample_rate,
     logger,
     nanosecond_time,
     set_in_app_in_frames,
 )
 
 if TYPE_CHECKING:
@@ -123,40 +125,24 @@
     StackId = Tuple[int, int]
 
     ExtractedStack = Tuple[StackId, FrameIds, List[ProcessedFrame]]
     ExtractedSample = Sequence[Tuple[ThreadId, ExtractedStack]]
 
 
 try:
-    from gevent import get_hub as get_gevent_hub  # type: ignore
-    from gevent.monkey import get_original, is_module_patched  # type: ignore
+    from gevent.monkey import get_original  # type: ignore
     from gevent.threadpool import ThreadPool  # type: ignore
 
     thread_sleep = get_original("time", "sleep")
 except ImportError:
-
-    def get_gevent_hub():
-        # type: () -> Any
-        return None
-
     thread_sleep = time.sleep
 
-    def is_module_patched(*args, **kwargs):
-        # type: (*Any, **Any) -> bool
-        # unable to import from gevent means no modules have been patched
-        return False
-
     ThreadPool = None
 
 
-def is_gevent():
-    # type: () -> bool
-    return is_module_patched("threading") or is_module_patched("_thread")
-
-
 _scheduler = None  # type: Optional[Scheduler]
 
 # The default sampling frequency to use. This is set at 101 in order to
 # mitigate the effects of lockstep sampling.
 DEFAULT_SAMPLING_FREQUENCY = 101
 
 
@@ -391,60 +377,14 @@
         # we've done all we can, time to give up and return what we have
         return name
 
 
 MAX_PROFILE_DURATION_NS = int(3e10)  # 30 seconds
 
 
-def get_current_thread_id(thread=None):
-    # type: (Optional[threading.Thread]) -> Optional[int]
-    """
-    Try to get the id of the current thread, with various fall backs.
-    """
-
-    # if a thread is specified, that takes priority
-    if thread is not None:
-        try:
-            thread_id = thread.ident
-            if thread_id is not None:
-                return thread_id
-        except AttributeError:
-            pass
-
-    # if the app is using gevent, we should look at the gevent hub first
-    # as the id there differs from what the threading module reports
-    if is_gevent():
-        gevent_hub = get_gevent_hub()
-        if gevent_hub is not None:
-            try:
-                # this is undocumented, so wrap it in try except to be safe
-                return gevent_hub.thread_ident
-            except AttributeError:
-                pass
-
-    # use the current thread's id if possible
-    try:
-        current_thread_id = threading.current_thread().ident
-        if current_thread_id is not None:
-            return current_thread_id
-    except AttributeError:
-        pass
-
-    # if we can't get the current thread id, fall back to the main thread id
-    try:
-        main_thread_id = threading.main_thread().ident
-        if main_thread_id is not None:
-            return main_thread_id
-    except AttributeError:
-        pass
-
-    # we've tried everything, time to give up
-    return None
-
-
 class Profile:
     def __init__(
         self,
         transaction,  # type: sentry_sdk.tracing.Transaction
         hub=None,  # type: Optional[sentry_sdk.Hub]
         scheduler=None,  # type: Optional[Scheduler]
     ):
@@ -458,15 +398,15 @@
         #
         # We cannot keep a reference to the transaction around here because it'll create
         # a reference cycle. So we opt to pull out just the necessary attributes.
         self.sampled = transaction.sampled  # type: Optional[bool]
 
         # Various framework integrations are capable of overwriting the active thread id.
         # If it is set to `None` at the end of the profile, we fall back to the default.
-        self._default_active_thread_id = get_current_thread_id() or 0  # type: int
+        self._default_active_thread_id = get_current_thread_meta()[0] or 0  # type: int
         self.active_thread_id = None  # type: Optional[int]
 
         try:
             self.start_ns = transaction._start_timestamp_monotonic_ns  # type: int
         except AttributeError:
             self.start_ns = 0
 
@@ -481,15 +421,15 @@
 
         self.unique_samples = 0
 
         transaction._profile = self
 
     def update_active_thread_id(self):
         # type: () -> None
-        self.active_thread_id = get_current_thread_id()
+        self.active_thread_id = get_current_thread_meta()[0]
         logger.debug(
             "[Profiling] updating active thread id to {tid}".format(
                 tid=self.active_thread_id
             )
         )
 
     def _set_initial_sampling_decision(self, sampling_context):
```

### Comparing `sentry-sdk-2.0.0rc3/sentry_sdk/scope.py` & `sentry-sdk-2.0.0rc4/sentry_sdk/scope.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,18 +66,14 @@
         Type,
     )
 
     from sentry_sdk.tracing import TransactionKwargs
 
     import sentry_sdk
 
-    class StartTransactionKwargs(TransactionKwargs, total=False):
-        client: Optional["sentry_sdk.Client"]
-        custom_sampling_context: SamplingContext
-
     P = ParamSpec("P")
     R = TypeVar("R")
 
     F = TypeVar("F", bound=Callable[..., Any])
     T = TypeVar("T")
 
 
@@ -962,17 +958,21 @@
         else:
             logger.info("before breadcrumb dropped breadcrumb (%s)", crumb)
 
         while len(self._breadcrumbs) > max_breadcrumbs:
             self._breadcrumbs.popleft()
 
     def start_transaction(
-        self, transaction=None, instrumenter=INSTRUMENTER.SENTRY, **kwargs
+        self,
+        transaction=None,
+        instrumenter=INSTRUMENTER.SENTRY,
+        custom_sampling_context=None,
+        **kwargs
     ):
-        # type: (Optional[Transaction], str, Unpack[StartTransactionKwargs]) -> Union[Transaction, NoOpSpan]
+        # type: (Optional[Transaction], str, Optional[SamplingContext], Unpack[TransactionKwargs]) -> Union[Transaction, NoOpSpan]
         """
         Start and return a transaction.
 
         Start an existing transaction if given, otherwise create and start a new
         transaction with kwargs.
 
         This is the entry point to manual tracing instrumentation.
@@ -987,26 +987,32 @@
         When used as context managers, spans and transactions are automatically
         finished at the end of the `with` block. If not using context managers,
         call the `.finish()` method.
 
         When the transaction is finished, it will be sent to Sentry with all its
         finished child spans.
 
-        For supported `**kwargs` see :py:class:`sentry_sdk.tracing.Transaction`.
+        :param transaction: The transaction to start. If omitted, we create and
+            start a new transaction.
+        :param instrumenter: This parameter is meant for internal use only.
+        :param custom_sampling_context: The transaction's custom sampling context.
+        :param kwargs: Optional keyword arguments to be passed to the Transaction
+            constructor. See :py:class:`sentry_sdk.tracing.Transaction` for
+            available arguments.
         """
         kwargs.setdefault("scope", self)
 
         client = Scope.get_client()
 
         configuration_instrumenter = client.options["instrumenter"]
 
         if instrumenter != configuration_instrumenter:
             return NoOpSpan()
 
-        custom_sampling_context = kwargs.pop("custom_sampling_context", {})
+        custom_sampling_context = custom_sampling_context or {}
 
         # kwargs at this point has type TransactionKwargs, since we have removed
         # the client and custom_sampling_context from it.
         transaction_kwargs = kwargs  # type: TransactionKwargs
 
         # if we haven't been given a transaction, make one
         if transaction is None:
```

### Comparing `sentry-sdk-2.0.0rc3/sentry_sdk/scrubber.py` & `sentry-sdk-2.0.0rc4/sentry_sdk/scrubber.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc3/sentry_sdk/serializer.py` & `sentry-sdk-2.0.0rc4/sentry_sdk/serializer.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc3/sentry_sdk/session.py` & `sentry-sdk-2.0.0rc4/sentry_sdk/session.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc3/sentry_sdk/sessions.py` & `sentry-sdk-2.0.0rc4/sentry_sdk/sessions.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc3/sentry_sdk/spotlight.py` & `sentry-sdk-2.0.0rc4/sentry_sdk/spotlight.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc3/sentry_sdk/tracing.py` & `sentry-sdk-2.0.0rc4/sentry_sdk/tracing.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 import uuid
 import random
 from datetime import datetime, timedelta, timezone
 
 import sentry_sdk
-from sentry_sdk.consts import INSTRUMENTER
-from sentry_sdk.utils import is_valid_sample_rate, logger, nanosecond_time
-from sentry_sdk.consts import SPANDATA
+from sentry_sdk.consts import INSTRUMENTER, SPANDATA
+from sentry_sdk.utils import (
+    get_current_thread_meta,
+    is_valid_sample_rate,
+    logger,
+    nanosecond_time,
+)
 from sentry_sdk._types import TYPE_CHECKING
 
 
 if TYPE_CHECKING:
     from collections.abc import Callable, Mapping, MutableMapping
     from typing import Any
     from typing import Dict
@@ -28,32 +32,77 @@
     R = TypeVar("R")
 
     import sentry_sdk.profiler
     from sentry_sdk._types import Event, MeasurementUnit, SamplingContext
 
     class SpanKwargs(TypedDict, total=False):
         trace_id: str
+        """
+        The trace ID of the root span. If this new span is to be the root span,
+        omit this parameter, and a new trace ID will be generated.
+        """
+
         span_id: str
+        """The span ID of this span. If omitted, a new span ID will be generated."""
+
         parent_span_id: str
+        """The span ID of the parent span, if applicable."""
+
         same_process_as_parent: bool
+        """Whether this span is in the same process as the parent span."""
+
         sampled: bool
+        """
+        Whether the span should be sampled. Overrides the default sampling decision
+        for this span when provided.
+        """
+
         op: str
+        """
+        The span's operation. A list of recommended values is available here:
+        https://develop.sentry.dev/sdk/performance/span-operations/
+        """
+
         description: str
-        # hub: Optional[sentry_sdk.Hub] is deprecated, and therefore omitted here!
+        """A description of what operation is being performed within the span."""
+
+        hub: Optional["sentry_sdk.Hub"]
+        """The hub to use for this span. This argument is DEPRECATED. Please use the `scope` parameter, instead."""
+
         status: str
-        # transaction: str is deprecated, and therefore omitted here!
+        """The span's status. Possible values are listed at https://develop.sentry.dev/sdk/event-payloads/span/"""
+
         containing_transaction: Optional["Transaction"]
+        """The transaction that this span belongs to."""
+
         start_timestamp: Optional[Union[datetime, float]]
+        """
+        The timestamp when the span started. If omitted, the current time
+        will be used.
+        """
+
         scope: "sentry_sdk.Scope"
+        """The scope to use for this span. If not provided, we use the current scope."""
 
     class TransactionKwargs(SpanKwargs, total=False):
         name: str
+        """Identifier of the transaction. Will show up in the Sentry UI."""
+
         source: str
+        """
+        A string describing the source of the transaction name. This will be used to determine the transaction's type.
+        See https://develop.sentry.dev/sdk/event-payloads/transaction/#transaction-annotations for more information.
+        Default "custom".
+        """
+
         parent_sampled: bool
+        """Whether the parent transaction was sampled. If True this transaction will be kept, if False it will be discarded."""
+
         baggage: "Baggage"
+        """The W3C baggage header value. (see https://www.w3.org/TR/baggage/)"""
 
 
 BAGGAGE_HEADER_NAME = "baggage"
 SENTRY_TRACE_HEADER_NAME = "sentry-trace"
 
 
 # Transaction source
@@ -104,15 +153,37 @@
             span._span_recorder = None
         else:
             self.spans.append(span)
 
 
 class Span:
     """A span holds timing information of a block of code.
-    Spans can have multiple child spans thus forming a span tree."""
+    Spans can have multiple child spans thus forming a span tree.
+
+    :param trace_id: The trace ID of the root span. If this new span is to be the root span,
+        omit this parameter, and a new trace ID will be generated.
+    :param span_id: The span ID of this span. If omitted, a new span ID will be generated.
+    :param parent_span_id: The span ID of the parent span, if applicable.
+    :param same_process_as_parent: Whether this span is in the same process as the parent span.
+    :param sampled: Whether the span should be sampled. Overrides the default sampling decision
+        for this span when provided.
+    :param op: The span's operation. A list of recommended values is available here:
+        https://develop.sentry.dev/sdk/performance/span-operations/
+    :param description: A description of what operation is being performed within the span.
+    :param hub: The hub to use for this span.
+
+        .. deprecated:: 2.0.0
+            Please use the `scope` parameter, instead.
+    :param status: The span's status. Possible values are listed at
+        https://develop.sentry.dev/sdk/event-payloads/span/
+    :param containing_transaction: The transaction that this span belongs to.
+    :param start_timestamp: The timestamp when the span started. If omitted, the current time
+        will be used.
+    :param scope: The scope to use for this span. If not provided, we use the current scope.
+    """
 
     __slots__ = (
         "trace_id",
         "span_id",
         "parent_span_id",
         "same_process_as_parent",
         "sampled",
@@ -128,40 +199,25 @@
         "hub",
         "_context_manager_state",
         "_containing_transaction",
         "_local_aggregator",
         "scope",
     )
 
-    def __new__(cls, **kwargs):
-        # type: (**Any) -> Any
-        """
-        Backwards-compatible implementation of Span and Transaction
-        creation.
-        """
-
-        # TODO: consider removing this in a future release.
-        # This is for backwards compatibility with releases before Transaction
-        # existed, to allow for a smoother transition.
-        if "transaction" in kwargs:
-            return object.__new__(Transaction)
-        return object.__new__(cls)
-
     def __init__(
         self,
         trace_id=None,  # type: Optional[str]
         span_id=None,  # type: Optional[str]
         parent_span_id=None,  # type: Optional[str]
         same_process_as_parent=True,  # type: bool
         sampled=None,  # type: Optional[bool]
         op=None,  # type: Optional[str]
         description=None,  # type: Optional[str]
         hub=None,  # type: Optional[sentry_sdk.Hub]  # deprecated
         status=None,  # type: Optional[str]
-        transaction=None,  # type: Optional[str] # deprecated
         containing_transaction=None,  # type: Optional[Transaction]
         start_timestamp=None,  # type: Optional[Union[datetime, float]]
         scope=None,  # type: Optional[sentry_sdk.Scope]
     ):
         # type: (...) -> None
         self.trace_id = trace_id or uuid.uuid4().hex
         self.span_id = span_id or uuid.uuid4().hex[16:]
@@ -190,14 +246,17 @@
 
         #: End timestamp of span
         self.timestamp = None  # type: Optional[datetime]
 
         self._span_recorder = None  # type: Optional[_SpanRecorder]
         self._local_aggregator = None  # type: Optional[LocalAggregator]
 
+        thread_id, thread_name = get_current_thread_meta()
+        self.set_thread(thread_id, thread_name)
+
     # TODO this should really live on the Transaction class rather than the Span
     # class
     def init_span_recorder(self, maxlen):
         # type: (int) -> None
         if self._span_recorder is None:
             self._span_recorder = _SpanRecorder(maxlen)
 
@@ -425,14 +484,23 @@
         # type: (str, Any) -> None
         self._data[key] = value
 
     def set_status(self, value):
         # type: (str) -> None
         self.status = value
 
+    def set_thread(self, thread_id, thread_name):
+        # type: (Optional[int], Optional[str]) -> None
+
+        if thread_id is not None:
+            self.set_data(SPANDATA.THREAD_ID, str(thread_id))
+
+            if thread_name is not None:
+                self.set_data(SPANDATA.THREAD_NAME, thread_name)
+
     def set_http_status(self, http_status):
         # type: (int) -> None
         self.set_tag(
             "http.status_code", str(http_status)
         )  # we keep this for backwards compatability
         self.set_data(SPANDATA.HTTP_STATUS_CODE, http_status)
 
@@ -558,15 +626,29 @@
             )
 
         return rv
 
 
 class Transaction(Span):
     """The Transaction is the root element that holds all the spans
-    for Sentry performance instrumentation."""
+    for Sentry performance instrumentation.
+
+    :param name: Identifier of the transaction.
+        Will show up in the Sentry UI.
+    :param parent_sampled: Whether the parent transaction was sampled.
+        If True this transaction will be kept, if False it will be discarded.
+    :param baggage: The W3C baggage header value.
+        (see https://www.w3.org/TR/baggage/)
+    :param source: A string describing the source of the transaction name.
+        This will be used to determine the transaction's type.
+        See https://develop.sentry.dev/sdk/event-payloads/transaction/#transaction-annotations
+        for more information. Default "custom".
+    :param kwargs: Additional arguments to be passed to the Span constructor.
+        See :py:class:`sentry_sdk.tracing.Span` for available arguments.
+    """
 
     __slots__ = (
         "name",
         "source",
         "parent_sampled",
         # used to create baggage value for head SDKs in dynamic sampling
         "sample_rate",
@@ -581,36 +663,14 @@
         name="",  # type: str
         parent_sampled=None,  # type: Optional[bool]
         baggage=None,  # type: Optional[Baggage]
         source=TRANSACTION_SOURCE_CUSTOM,  # type: str
         **kwargs,  # type: Unpack[SpanKwargs]
     ):
         # type: (...) -> None
-        """Constructs a new Transaction.
-
-        :param name: Identifier of the transaction.
-            Will show up in the Sentry UI.
-        :param parent_sampled: Whether the parent transaction was sampled.
-            If True this transaction will be kept, if False it will be discarded.
-        :param baggage: The W3C baggage header value.
-            (see https://www.w3.org/TR/baggage/)
-        :param source: A string describing the source of the transaction name.
-            This will be used to determine the transaction's type.
-            See https://develop.sentry.dev/sdk/event-payloads/transaction/#transaction-annotations
-            for more information. Default "custom".
-        """
-        # TODO: consider removing this in a future release.
-        # This is for backwards compatibility with releases before Transaction
-        # existed, to allow for a smoother transition.
-        if not name and "transaction" in kwargs:
-            logger.warning(
-                "Deprecated: use Transaction(name=...) to create transactions "
-                "instead of Span(transaction=...)."
-            )
-            name = kwargs.pop("transaction")  # type: ignore
 
         super().__init__(**kwargs)
 
         self.name = name
         self.source = source
         self.sample_rate = None  # type: Optional[float]
         self.parent_sampled = parent_sampled
```

### Comparing `sentry-sdk-2.0.0rc3/sentry_sdk/tracing_utils.py` & `sentry-sdk-2.0.0rc4/sentry_sdk/tracing_utils.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc3/sentry_sdk/transport.py` & `sentry-sdk-2.0.0rc4/sentry_sdk/transport.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc3/sentry_sdk/utils.py` & `sentry-sdk-2.0.0rc4/sentry_sdk/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,20 +34,22 @@
 if TYPE_CHECKING:
     from collections.abc import Awaitable
 
     from types import FrameType, TracebackType
     from typing import (
         Any,
         Callable,
+        cast,
         ContextManager,
         Dict,
         Iterator,
         List,
         NoReturn,
         Optional,
+        overload,
         ParamSpec,
         Set,
         Tuple,
         Type,
         TypeVar,
         Union,
     )
@@ -1627,17 +1629,47 @@
     # type: (Optional[Type[BaseException]], Optional[BaseException], Optional[Any]) -> NoReturn
     assert value is not None
     if value.__traceback__ is not tb:
         raise value.with_traceback(tb)
     raise value
 
 
+def _no_op(*_a, **_k):
+    # type: (*Any, **Any) -> None
+    """No-op function for ensure_integration_enabled."""
+    pass
+
+
+async def _no_op_async(*_a, **_k):
+    # type: (*Any, **Any) -> None
+    """No-op function for ensure_integration_enabled_async."""
+    pass
+
+
+if TYPE_CHECKING:
+
+    @overload
+    def ensure_integration_enabled(
+        integration,  # type: type[sentry_sdk.integrations.Integration]
+        original_function,  # type: Callable[P, R]
+    ):
+        # type: (...) -> Callable[[Callable[P, R]], Callable[P, R]]
+        ...
+
+    @overload
+    def ensure_integration_enabled(
+        integration,  # type: type[sentry_sdk.integrations.Integration]
+    ):
+        # type: (...) -> Callable[[Callable[P, None]], Callable[P, None]]
+        ...
+
+
 def ensure_integration_enabled(
     integration,  # type: type[sentry_sdk.integrations.Integration]
-    original_function,  # type: Callable[P, R]
+    original_function=_no_op,  # type: Union[Callable[P, R], Callable[P, None]]
 ):
     # type: (...) -> Callable[[Callable[P, R]], Callable[P, R]]
     """
     Ensures a given integration is enabled prior to calling a Sentry-patched function.
 
     The function takes as its parameters the integration that must be enabled and the original
     function that the SDK is patching. The function returns a function that takes the
@@ -1653,52 +1685,85 @@
     ```python
     @ensure_integration_enabled(MyIntegration, my_function)
     def patch_my_function():
         with sentry_sdk.start_transaction(...):
             return my_function()
     ```
     """
+    if TYPE_CHECKING:
+        # Type hint to ensure the default function has the right typing. The overloads
+        # ensure the default _no_op function is only used when R is None.
+        original_function = cast(Callable[P, R], original_function)
 
     def patcher(sentry_patched_function):
         # type: (Callable[P, R]) -> Callable[P, R]
-        @wraps(original_function)
         def runner(*args: "P.args", **kwargs: "P.kwargs"):
             # type: (...) -> R
             if sentry_sdk.get_client().get_integration(integration) is None:
                 return original_function(*args, **kwargs)
 
             return sentry_patched_function(*args, **kwargs)
 
-        return runner
+        if original_function is _no_op:
+            return wraps(sentry_patched_function)(runner)
+
+        return wraps(original_function)(runner)
 
     return patcher
 
 
-def ensure_integration_enabled_async(
+if TYPE_CHECKING:
+
+    # mypy has some trouble with the overloads, hence the ignore[no-overload-impl]
+    @overload  # type: ignore[no-overload-impl]
+    def ensure_integration_enabled_async(
+        integration,  # type: type[sentry_sdk.integrations.Integration]
+        original_function,  # type: Callable[P, Awaitable[R]]
+    ):
+        # type: (...) -> Callable[[Callable[P, Awaitable[R]]], Callable[P, Awaitable[R]]]
+        ...
+
+    @overload
+    def ensure_integration_enabled_async(
+        integration,  # type: type[sentry_sdk.integrations.Integration]
+    ):
+        # type: (...) -> Callable[[Callable[P, Awaitable[None]]], Callable[P, Awaitable[None]]]
+        ...
+
+
+# The ignore[no-redef] also needed because mypy is struggling with these overloads.
+def ensure_integration_enabled_async(  # type: ignore[no-redef]
     integration,  # type: type[sentry_sdk.integrations.Integration]
-    original_function,  # type: Callable[P, Awaitable[R]]
+    original_function=_no_op_async,  # type: Union[Callable[P, Awaitable[R]], Callable[P, Awaitable[None]]]
 ):
     # type: (...) -> Callable[[Callable[P, Awaitable[R]]], Callable[P, Awaitable[R]]]
     """
     Version of `ensure_integration_enabled` for decorating async functions.
 
     Please refer to the `ensure_integration_enabled` documentation for more information.
     """
 
+    if TYPE_CHECKING:
+        # Type hint to ensure the default function has the right typing. The overloads
+        # ensure the default _no_op function is only used when R is None.
+        original_function = cast(Callable[P, Awaitable[R]], original_function)
+
     def patcher(sentry_patched_function):
         # type: (Callable[P, Awaitable[R]]) -> Callable[P, Awaitable[R]]
-        @wraps(original_function)
         async def runner(*args: "P.args", **kwargs: "P.kwargs"):
             # type: (...) -> R
             if sentry_sdk.get_client().get_integration(integration) is None:
                 return await original_function(*args, **kwargs)
 
             return await sentry_patched_function(*args, **kwargs)
 
-        return runner
+        if original_function is _no_op_async:
+            return wraps(sentry_patched_function)(runner)
+
+        return wraps(original_function)(runner)
 
     return patcher
 
 
 if PY37:
 
     def nanosecond_time():
@@ -1714,19 +1779,75 @@
 
 def now():
     # type: () -> float
     return time.perf_counter()
 
 
 try:
+    from gevent import get_hub as get_gevent_hub
     from gevent.monkey import is_module_patched
 except ImportError:
 
+    def get_gevent_hub():
+        # type: () -> Any
+        return None
+
     def is_module_patched(*args, **kwargs):
         # type: (*Any, **Any) -> bool
         # unable to import from gevent means no modules have been patched
         return False
 
 
 def is_gevent():
     # type: () -> bool
     return is_module_patched("threading") or is_module_patched("_thread")
+
+
+def get_current_thread_meta(thread=None):
+    # type: (Optional[threading.Thread]) -> Tuple[Optional[int], Optional[str]]
+    """
+    Try to get the id of the current thread, with various fall backs.
+    """
+
+    # if a thread is specified, that takes priority
+    if thread is not None:
+        try:
+            thread_id = thread.ident
+            thread_name = thread.name
+            if thread_id is not None:
+                return thread_id, thread_name
+        except AttributeError:
+            pass
+
+    # if the app is using gevent, we should look at the gevent hub first
+    # as the id there differs from what the threading module reports
+    if is_gevent():
+        gevent_hub = get_gevent_hub()
+        if gevent_hub is not None:
+            try:
+                # this is undocumented, so wrap it in try except to be safe
+                return gevent_hub.thread_ident, None
+            except AttributeError:
+                pass
+
+    # use the current thread's id if possible
+    try:
+        thread = threading.current_thread()
+        thread_id = thread.ident
+        thread_name = thread.name
+        if thread_id is not None:
+            return thread_id, thread_name
+    except AttributeError:
+        pass
+
+    # if we can't get the current thread id, fall back to the main thread id
+    try:
+        thread = threading.main_thread()
+        thread_id = thread.ident
+        thread_name = thread.name
+        if thread_id is not None:
+            return thread_id, thread_name
+    except AttributeError:
+        pass
+
+    # we've tried everything, time to give up
+    return None, None
```

### Comparing `sentry-sdk-2.0.0rc3/sentry_sdk/worker.py` & `sentry-sdk-2.0.0rc4/sentry_sdk/worker.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc3/sentry_sdk.egg-info/PKG-INFO` & `sentry-sdk-2.0.0rc4/sentry_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sentry-sdk
-Version: 2.0.0rc3
+Version: 2.0.0rc4
 Summary: Python client for Sentry (https://sentry.io)
 Home-page: https://github.com/getsentry/sentry-python
 Author: Sentry Team and Contributors
 Author-email: hello@sentry.io
 License: MIT
 Project-URL: Documentation, https://docs.sentry.io/platforms/python/
 Project-URL: Changelog, https://github.com/getsentry/sentry-python/blob/master/CHANGELOG.md
```

### Comparing `sentry-sdk-2.0.0rc3/sentry_sdk.egg-info/SOURCES.txt` & `sentry-sdk-2.0.0rc4/sentry_sdk.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -57,15 +57,14 @@
 sentry_sdk/integrations/asyncio.py
 sentry_sdk/integrations/asyncpg.py
 sentry_sdk/integrations/atexit.py
 sentry_sdk/integrations/aws_lambda.py
 sentry_sdk/integrations/beam.py
 sentry_sdk/integrations/boto3.py
 sentry_sdk/integrations/bottle.py
-sentry_sdk/integrations/celery.py
 sentry_sdk/integrations/chalice.py
 sentry_sdk/integrations/clickhouse_driver.py
 sentry_sdk/integrations/cloud_resource_context.py
 sentry_sdk/integrations/dedupe.py
 sentry_sdk/integrations/excepthook.py
 sentry_sdk/integrations/executing.py
 sentry_sdk/integrations/falcon.py
@@ -94,14 +93,17 @@
 sentry_sdk/integrations/starlite.py
 sentry_sdk/integrations/stdlib.py
 sentry_sdk/integrations/strawberry.py
 sentry_sdk/integrations/threading.py
 sentry_sdk/integrations/tornado.py
 sentry_sdk/integrations/trytond.py
 sentry_sdk/integrations/wsgi.py
+sentry_sdk/integrations/celery/__init__.py
+sentry_sdk/integrations/celery/beat.py
+sentry_sdk/integrations/celery/utils.py
 sentry_sdk/integrations/django/__init__.py
 sentry_sdk/integrations/django/asgi.py
 sentry_sdk/integrations/django/caching.py
 sentry_sdk/integrations/django/middleware.py
 sentry_sdk/integrations/django/signals_handlers.py
 sentry_sdk/integrations/django/templates.py
 sentry_sdk/integrations/django/transactions.py
@@ -137,8 +139,9 @@
 tests/test_profiler.py
 tests/test_scope.py
 tests/test_scrubber.py
 tests/test_serializer.py
 tests/test_sessions.py
 tests/test_spotlight.py
 tests/test_transport.py
+tests/test_types.py
 tests/test_utils.py
```

### Comparing `sentry-sdk-2.0.0rc3/sentry_sdk.egg-info/requires.txt` & `sentry-sdk-2.0.0rc4/sentry_sdk.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc3/setup.py` & `sentry-sdk-2.0.0rc4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 def get_file_text(file_name):
     with open(os.path.join(here, file_name)) as in_file:
         return in_file.read()
 
 
 setup(
     name="sentry-sdk",
-    version="2.0.0rc3",
+    version="2.0.0rc4",
     author="Sentry Team and Contributors",
     author_email="hello@sentry.io",
     url="https://github.com/getsentry/sentry-python",
     project_urls={
         "Documentation": "https://docs.sentry.io/platforms/python/",
         "Changelog": "https://github.com/getsentry/sentry-python/blob/master/CHANGELOG.md",
     },
```

### Comparing `sentry-sdk-2.0.0rc3/tests/test_api.py` & `sentry-sdk-2.0.0rc4/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc3/tests/test_basics.py` & `sentry-sdk-2.0.0rc4/tests/test_basics.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc3/tests/test_client.py` & `sentry-sdk-2.0.0rc4/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc3/tests/test_conftest.py` & `sentry-sdk-2.0.0rc4/tests/test_conftest.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc3/tests/test_envelope.py` & `sentry-sdk-2.0.0rc4/tests/test_envelope.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc3/tests/test_exceptiongroup.py` & `sentry-sdk-2.0.0rc4/tests/test_exceptiongroup.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc3/tests/test_lru_cache.py` & `sentry-sdk-2.0.0rc4/tests/test_lru_cache.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc3/tests/test_metrics.py` & `sentry-sdk-2.0.0rc4/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc3/tests/test_monitor.py` & `sentry-sdk-2.0.0rc4/tests/test_monitor.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc3/tests/test_new_scopes_compat.py` & `sentry-sdk-2.0.0rc4/tests/test_new_scopes_compat.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc3/tests/test_new_scopes_compat_event.py` & `sentry-sdk-2.0.0rc4/tests/test_new_scopes_compat_event.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
                         "stacktrace": {
                             "frames": [
                                 {
                                     "filename": "tests/test_new_scopes_compat_event.py",
                                     "abs_path": mock.ANY,
                                     "function": "_faulty_function",
                                     "module": "tests.test_new_scopes_compat_event",
-                                    "lineno": 236,
+                                    "lineno": 240,
                                     "pre_context": [
                                         "    return create_expected_transaction_event",
                                         "",
                                         "",
                                         "def _faulty_function():",
                                         "    try:",
                                     ],
@@ -170,14 +170,18 @@
                 },
             },
             "tags": {"tag1": "tag1_value", "tag2": "tag2_value"},
             "timestamp": mock.ANY,
             "start_timestamp": mock.ANY,
             "spans": [
                 {
+                    "data": {
+                        "thread.id": mock.ANY,
+                        "thread.name": "MainThread",
+                    },
                     "trace_id": trx.trace_id,
                     "span_id": span.span_id,
                     "parent_span_id": span.parent_span_id,
                     "same_process_as_parent": True,
                     "op": "test_span",
                     "description": None,
                     "start_timestamp": mock.ANY,
@@ -309,15 +313,14 @@
         before_breadcrumb=_test_before_breadcrumb,
         event_scrubber=EventScrubber(
             denylist=DEFAULT_DENYLIST
             + ["should_be_removed_by_event_scrubber", "sys.argv"]
         ),
         send_default_pii=False,
         traces_sample_rate=1.0,
-        debug=True,
     )
 
 
 #
 # The actual Tests start here!
 #
```

### Comparing `sentry-sdk-2.0.0rc3/tests/test_profiler.py` & `sentry-sdk-2.0.0rc4/tests/test_profiler.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,21 +13,19 @@
     GeventScheduler,
     Profile,
     Scheduler,
     ThreadScheduler,
     extract_frame,
     extract_stack,
     frame_id,
-    get_current_thread_id,
     get_frame_name,
     setup_profiler,
 )
 from sentry_sdk.tracing import Transaction
 from sentry_sdk._lru_cache import LRUCache
-from sentry_sdk._queue import Queue
 
 try:
     import gevent
 except ImportError:
     gevent = None
 
 
@@ -531,78 +529,14 @@
         # DO NOT use `==` for the assertion here since we are
         # testing for identity, and using `==` would test for
         # equality which would always pass since we're extract
         # the same stack.
         assert frame1 is frame2, i
 
 
-def test_get_current_thread_id_explicit_thread():
-    results = Queue(maxsize=1)
-
-    def target1():
-        pass
-
-    def target2():
-        results.put(get_current_thread_id(thread1))
-
-    thread1 = threading.Thread(target=target1)
-    thread1.start()
-
-    thread2 = threading.Thread(target=target2)
-    thread2.start()
-
-    thread2.join()
-    thread1.join()
-
-    assert thread1.ident == results.get(timeout=1)
-
-
-@requires_gevent
-def test_get_current_thread_id_gevent_in_thread():
-    results = Queue(maxsize=1)
-
-    def target():
-        job = gevent.spawn(get_current_thread_id)
-        job.join()
-        results.put(job.value)
-
-    thread = threading.Thread(target=target)
-    thread.start()
-    thread.join()
-    assert thread.ident == results.get(timeout=1)
-
-
-def test_get_current_thread_id_running_thread():
-    results = Queue(maxsize=1)
-
-    def target():
-        results.put(get_current_thread_id())
-
-    thread = threading.Thread(target=target)
-    thread.start()
-    thread.join()
-    assert thread.ident == results.get(timeout=1)
-
-
-def test_get_current_thread_id_main_thread():
-    results = Queue(maxsize=1)
-
-    def target():
-        # mock that somehow the current thread doesn't exist
-        with mock.patch("threading.current_thread", side_effect=[None]):
-            results.put(get_current_thread_id())
-
-    thread_id = threading.main_thread().ident
-
-    thread = threading.Thread(target=target)
-    thread.start()
-    thread.join()
-    assert thread_id == results.get(timeout=1)
-
-
 def get_scheduler_threads(scheduler):
     return [thread for thread in threading.enumerate() if thread.name == scheduler.name]
 
 
 @pytest.mark.parametrize(
     ("scheduler_class",),
     [
```

### Comparing `sentry-sdk-2.0.0rc3/tests/test_scope.py` & `sentry-sdk-2.0.0rc4/tests/test_scope.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc3/tests/test_scrubber.py` & `sentry-sdk-2.0.0rc4/tests/test_scrubber.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import sys
 import logging
 
 from sentry_sdk import capture_exception, capture_event, start_transaction, start_span
 from sentry_sdk.utils import event_from_exception
 from sentry_sdk.scrubber import EventScrubber
+from tests.conftest import ApproxDict
 
 
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.DEBUG)
 
 
 def test_request_scrubbing(sentry_init, capture_events):
@@ -117,15 +118,17 @@
 
     with start_transaction(name="hi"):
         with start_span(op="foo", description="bar") as span:
             span.set_data("password", "secret")
             span.set_data("datafoo", "databar")
 
     (event,) = events
-    assert event["spans"][0]["data"] == {"password": "[Filtered]", "datafoo": "databar"}
+    assert event["spans"][0]["data"] == ApproxDict(
+        {"password": "[Filtered]", "datafoo": "databar"}
+    )
     assert event["_meta"]["spans"] == {
         "0": {"data": {"password": {"": {"rem": [["!config", "s"]]}}}}
     }
 
 
 def test_custom_denylist(sentry_init, capture_events):
     sentry_init(event_scrubber=EventScrubber(denylist=["my_sensitive_var"]))
```

### Comparing `sentry-sdk-2.0.0rc3/tests/test_serializer.py` & `sentry-sdk-2.0.0rc4/tests/test_serializer.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc3/tests/test_sessions.py` & `sentry-sdk-2.0.0rc4/tests/test_sessions.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc3/tests/test_spotlight.py` & `sentry-sdk-2.0.0rc4/tests/test_spotlight.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc3/tests/test_transport.py` & `sentry-sdk-2.0.0rc4/tests/test_transport.py`

 * *Files identical despite different names*


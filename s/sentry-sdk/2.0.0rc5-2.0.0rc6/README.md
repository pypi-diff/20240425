# Comparing `tmp/sentry-sdk-2.0.0rc5.tar.gz` & `tmp/sentry_sdk-2.0.0rc6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sentry-sdk-2.0.0rc5.tar", last modified: Wed Apr 10 14:23:05 2024, max compression
+gzip compressed data, was "sentry_sdk-2.0.0rc6.tar", last modified: Tue Apr 23 12:01:43 2024, max compression
```

## Comparing `sentry-sdk-2.0.0rc5.tar` & `sentry_sdk-2.0.0rc6.tar`

### file list

```diff
@@ -1,164 +1,164 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:23:05.517917 sentry-sdk-2.0.0rc5/
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    10503 2024-04-10 14:23:05.517917 sentry-sdk-2.0.0rc5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5960 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:23:05.493917 sentry-sdk-2.0.0rc5/sentry_sdk/
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3066 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/_compat.py
--rw-r--r--   0 runner    (1001) docker     (127)     5382 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/_lru_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)    11259 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/_queue.py
--rw-r--r--   0 runner    (1001) docker     (127)     6478 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     3745 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/_werkzeug.py
--rw-r--r--   0 runner    (1001) docker     (127)     9593 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/attachments.py
--rw-r--r--   0 runner    (1001) docker     (127)    29194 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    11744 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/consts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:23:05.497918 sentry-sdk-2.0.0rc5/sentry_sdk/crons/
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/crons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/crons/api.py
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/crons/consts.py
--rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/crons/decorator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:23:05.497918 sentry-sdk-2.0.0rc5/sentry_sdk/db/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/db/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:23:05.497918 sentry-sdk-2.0.0rc5/sentry_sdk/db/explain_plan/
--rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/db/explain_plan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/db/explain_plan/django.py
--rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/db/explain_plan/sqlalchemy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/debug.py
--rw-r--r--   0 runner    (1001) docker     (127)     9923 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/envelope.py
--rw-r--r--   0 runner    (1001) docker     (127)    27085 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/hub.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:23:05.505917 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/
--rw-r--r--   0 runner    (1001) docker     (127)     7541 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3197 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/_asgi_common.py
--rw-r--r--   0 runner    (1001) docker     (127)     5636 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/_wsgi_common.py
--rw-r--r--   0 runner    (1001) docker     (127)    11478 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/argv.py
--rw-r--r--   0 runner    (1001) docker     (127)     5939 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/ariadne.py
--rw-r--r--   0 runner    (1001) docker     (127)     6919 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/arq.py
--rw-r--r--   0 runner    (1001) docker     (127)    11600 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/asgi.py
--rw-r--r--   0 runner    (1001) docker     (127)     3091 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/asyncio.py
--rw-r--r--   0 runner    (1001) docker     (127)     6027 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/asyncpg.py
--rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/atexit.py
--rw-r--r--   0 runner    (1001) docker     (127)    15627 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/aws_lambda.py
--rw-r--r--   0 runner    (1001) docker     (127)     5192 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/beam.py
--rw-r--r--   0 runner    (1001) docker     (127)     4475 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/boto3.py
--rw-r--r--   0 runner    (1001) docker     (127)     5800 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/bottle.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:23:05.505917 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/celery/
--rw-r--r--   0 runner    (1001) docker     (127)    13809 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/celery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9813 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/celery/beat.py
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/celery/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4721 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/chalice.py
--rw-r--r--   0 runner    (1001) docker     (127)     5064 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/clickhouse_driver.py
--rw-r--r--   0 runner    (1001) docker     (127)     6755 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/cloud_resource_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/dedupe.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:23:05.505917 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/django/
--rw-r--r--   0 runner    (1001) docker     (127)    23519 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/django/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6820 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/django/asgi.py
--rw-r--r--   0 runner    (1001) docker     (127)     3622 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/django/caching.py
--rw-r--r--   0 runner    (1001) docker     (127)     5770 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/django/middleware.py
--rw-r--r--   0 runner    (1001) docker     (127)     3063 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/django/signals_handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5683 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/django/templates.py
--rw-r--r--   0 runner    (1001) docker     (127)     4957 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/django/transactions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2836 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/django/views.py
--rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/excepthook.py
--rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/executing.py
--rw-r--r--   0 runner    (1001) docker     (127)     9347 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/falcon.py
--rw-r--r--   0 runner    (1001) docker     (127)     4543 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/fastapi.py
--rw-r--r--   0 runner    (1001) docker     (127)     7706 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/flask.py
--rw-r--r--   0 runner    (1001) docker     (127)     8149 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/gcp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2906 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/gnu_backtrace.py
--rw-r--r--   0 runner    (1001) docker     (127)     4386 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/gql.py
--rw-r--r--   0 runner    (1001) docker     (127)     3594 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/graphene.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:23:05.505917 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/grpc/
--rw-r--r--   0 runner    (1001) docker     (127)     4979 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/grpc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:23:05.509918 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/grpc/aio/
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/grpc/aio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3075 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/grpc/aio/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3866 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/grpc/aio/server.py
--rw-r--r--   0 runner    (1001) docker     (127)     3249 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/grpc/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2389 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/grpc/server.py
--rw-r--r--   0 runner    (1001) docker     (127)     5165 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/httpx.py
--rw-r--r--   0 runner    (1001) docker     (127)     5260 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/huey.py
--rw-r--r--   0 runner    (1001) docker     (127)     9592 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     3011 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/loguru.py
--rw-r--r--   0 runner    (1001) docker     (127)      831 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/modules.py
--rw-r--r--   0 runner    (1001) docker     (127)    11005 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/openai.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:23:05.509918 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/opentelemetry/
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/opentelemetry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/opentelemetry/consts.py
--rw-r--r--   0 runner    (1001) docker     (127)     5830 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/opentelemetry/integration.py
--rw-r--r--   0 runner    (1001) docker     (127)     3731 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/opentelemetry/propagator.py
--rw-r--r--   0 runner    (1001) docker     (127)    12225 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/opentelemetry/span_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4539 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/pure_eval.py
--rw-r--r--   0 runner    (1001) docker     (127)     5994 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/pymongo.py
--rw-r--r--   0 runner    (1001) docker     (127)     7151 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/pyramid.py
--rw-r--r--   0 runner    (1001) docker     (127)     7091 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/quart.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:23:05.509918 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/redis/
--rw-r--r--   0 runner    (1001) docker     (127)    11834 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/redis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/redis/asyncio.py
--rw-r--r--   0 runner    (1001) docker     (127)     5297 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/rq.py
--rw-r--r--   0 runner    (1001) docker     (127)    13127 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/sanic.py
--rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/serverless.py
--rw-r--r--   0 runner    (1001) docker     (127)     2906 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/socket.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:23:05.509918 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/spark/
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/spark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8276 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/spark/spark_driver.py
--rw-r--r--   0 runner    (1001) docker     (127)     3747 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/spark/spark_worker.py
--rw-r--r--   0 runner    (1001) docker     (127)     4865 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/sqlalchemy.py
--rw-r--r--   0 runner    (1001) docker     (127)    23504 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/starlette.py
--rw-r--r--   0 runner    (1001) docker     (127)     9835 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/starlite.py
--rw-r--r--   0 runner    (1001) docker     (127)     8346 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/stdlib.py
--rw-r--r--   0 runner    (1001) docker     (127)    14574 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/strawberry.py
--rw-r--r--   0 runner    (1001) docker     (127)     4033 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/threading.py
--rw-r--r--   0 runner    (1001) docker     (127)     7185 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/tornado.py
--rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/trytond.py
--rw-r--r--   0 runner    (1001) docker     (127)     9870 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/integrations/wsgi.py
--rw-r--r--   0 runner    (1001) docker     (127)    29725 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     3720 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)    33332 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/profiler.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    57649 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/scope.py
--rw-r--r--   0 runner    (1001) docker     (127)     5082 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/scrubber.py
--rw-r--r--   0 runner    (1001) docker     (127)    12729 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/serializer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5581 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/session.py
--rw-r--r--   0 runner    (1001) docker     (127)     7822 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/sessions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/spotlight.py
--rw-r--r--   0 runner    (1001) docker     (127)    38456 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/tracing.py
--rw-r--r--   0 runner    (1001) docker     (127)    17304 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/tracing_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    21002 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/transport.py
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/types.py
--rw-r--r--   0 runner    (1001) docker     (127)    56591 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4475 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/sentry_sdk/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:23:05.513918 sentry-sdk-2.0.0rc5/sentry_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10503 2024-04-10 14:23:05.000000 sentry-sdk-2.0.0rc5/sentry_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-04-10 14:23:05.000000 sentry-sdk-2.0.0rc5/sentry_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 14:23:05.000000 sentry-sdk-2.0.0rc5/sentry_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 14:23:05.000000 sentry-sdk-2.0.0rc5/sentry_sdk.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-04-10 14:23:05.000000 sentry-sdk-2.0.0rc5/sentry_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-10 14:23:05.000000 sentry-sdk-2.0.0rc5/sentry_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 14:23:05.517917 sentry-sdk-2.0.0rc5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3836 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:23:05.513918 sentry-sdk-2.0.0rc5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4000 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    23225 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/tests/test_basics.py
--rw-r--r--   0 runner    (1001) docker     (127)    36053 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3409 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/tests/test_conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    13795 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/tests/test_crons.py
--rw-r--r--   0 runner    (1001) docker     (127)     8057 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/tests/test_envelope.py
--rw-r--r--   0 runner    (1001) docker     (127)     8578 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/tests/test_exceptiongroup.py
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/tests/test_lru_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)    29128 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/tests/test_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     2563 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/tests/test_monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     8686 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/tests/test_new_scopes_compat.py
--rw-r--r--   0 runner    (1001) docker     (127)    17288 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/tests/test_new_scopes_compat_event.py
--rw-r--r--   0 runner    (1001) docker     (127)    23653 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/tests/test_profiler.py
--rw-r--r--   0 runner    (1001) docker     (127)    25744 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/tests/test_scope.py
--rw-r--r--   0 runner    (1001) docker     (127)     5357 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/tests/test_scrubber.py
--rw-r--r--   0 runner    (1001) docker     (127)     4578 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/tests/test_serializer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4098 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/tests/test_sessions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/tests/test_spotlight.py
--rw-r--r--   0 runner    (1001) docker     (127)    18754 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/tests/test_transport.py
--rw-r--r--   0 runner    (1001) docker     (127)      760 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/tests/test_types.py
--rw-r--r--   0 runner    (1001) docker     (127)    26384 2024-04-10 14:22:56.000000 sentry-sdk-2.0.0rc5/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:01:43.673097 sentry_sdk-2.0.0rc6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-04-23 12:01:35.000000 sentry_sdk-2.0.0rc6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-23 12:01:35.000000 sentry_sdk-2.0.0rc6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    10503 2024-04-23 12:01:43.673097 sentry_sdk-2.0.0rc6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5960 2024-04-23 12:01:35.000000 sentry_sdk-2.0.0rc6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-23 12:01:35.000000 sentry_sdk-2.0.0rc6/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:01:43.649097 sentry_sdk-2.0.0rc6/sentry_sdk/
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-23 12:01:35.000000 sentry_sdk-2.0.0rc6/sentry_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3066 2024-04-23 12:01:35.000000 sentry_sdk-2.0.0rc6/sentry_sdk/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5382 2024-04-23 12:01:35.000000 sentry_sdk-2.0.0rc6/sentry_sdk/_lru_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11259 2024-04-23 12:01:35.000000 sentry_sdk-2.0.0rc6/sentry_sdk/_queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6478 2024-04-23 12:01:35.000000 sentry_sdk-2.0.0rc6/sentry_sdk/_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3745 2024-04-23 12:01:35.000000 sentry_sdk-2.0.0rc6/sentry_sdk/_werkzeug.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9593 2024-04-23 12:01:35.000000 sentry_sdk-2.0.0rc6/sentry_sdk/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-04-23 12:01:35.000000 sentry_sdk-2.0.0rc6/sentry_sdk/attachments.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29194 2024-04-23 12:01:35.000000 sentry_sdk-2.0.0rc6/sentry_sdk/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11744 2024-04-23 12:01:35.000000 sentry_sdk-2.0.0rc6/sentry_sdk/consts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:01:43.653097 sentry_sdk-2.0.0rc6/sentry_sdk/crons/
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-23 12:01:35.000000 sentry_sdk-2.0.0rc6/sentry_sdk/crons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-04-23 12:01:35.000000 sentry_sdk-2.0.0rc6/sentry_sdk/crons/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-23 12:01:35.000000 sentry_sdk-2.0.0rc6/sentry_sdk/crons/consts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-04-23 12:01:35.000000 sentry_sdk-2.0.0rc6/sentry_sdk/crons/decorator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:01:43.653097 sentry_sdk-2.0.0rc6/sentry_sdk/db/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 12:01:35.000000 sentry_sdk-2.0.0rc6/sentry_sdk/db/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:01:43.653097 sentry_sdk-2.0.0rc6/sentry_sdk/db/explain_plan/
+-rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-04-23 12:01:35.000000 sentry_sdk-2.0.0rc6/sentry_sdk/db/explain_plan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-04-23 12:01:35.000000 sentry_sdk-2.0.0rc6/sentry_sdk/db/explain_plan/django.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-04-23 12:01:35.000000 sentry_sdk-2.0.0rc6/sentry_sdk/db/explain_plan/sqlalchemy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-23 12:01:35.000000 sentry_sdk-2.0.0rc6/sentry_sdk/debug.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9923 2024-04-23 12:01:35.000000 sentry_sdk-2.0.0rc6/sentry_sdk/envelope.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27085 2024-04-23 12:01:35.000000 sentry_sdk-2.0.0rc6/sentry_sdk/hub.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:01:43.661097 sentry_sdk-2.0.0rc6/sentry_sdk/integrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     7541 2024-04-23 12:01:35.000000 sentry_sdk-2.0.0rc6/sentry_sdk/integrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3197 2024-04-23 12:01:35.000000 sentry_sdk-2.0.0rc6/sentry_sdk/integrations/_asgi_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5636 2024-04-23 12:01:35.000000 sentry_sdk-2.0.0rc6/sentry_sdk/integrations/_wsgi_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11478 2024-04-23 12:01:35.000000 sentry_sdk-2.0.0rc6/sentry_sdk/integrations/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-23 12:01:35.000000 sentry_sdk-2.0.0rc6/sentry_sdk/integrations/argv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5939 2024-04-23 12:01:35.000000 sentry_sdk-2.0.0rc6/sentry_sdk/integrations/ariadne.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6919 2024-04-23 12:01:35.000000 sentry_sdk-2.0.0rc6/sentry_sdk/integrations/arq.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11600 2024-04-23 12:01:35.000000 sentry_sdk-2.0.0rc6/sentry_sdk/integrations/asgi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3091 2024-04-23 12:01:35.000000 sentry_sdk-2.0.0rc6/sentry_sdk/integrations/asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6027 2024-04-23 12:01:35.000000 sentry_sdk-2.0.0rc6/sentry_sdk/integrations/asyncpg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-04-23 12:01:35.000000 sentry_sdk-2.0.0rc6/sentry_sdk/integrations/atexit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15627 2024-04-23 12:01:35.000000 sentry_sdk-2.0.0rc6/sentry_sdk/integrations/aws_lambda.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5192 2024-04-23 12:01:35.000000 sentry_sdk-2.0.0rc6/sentry_sdk/integrations/beam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4475 2024-04-23 12:01:35.000000 sentry_sdk-2.0.0rc6/sentry_sdk/integrations/boto3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5800 2024-04-23 12:01:35.000000 sentry_sdk-2.0.0rc6/sentry_sdk/integrations/bottle.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:01:43.661097 sentry_sdk-2.0.0rc6/sentry_sdk/integrations/celery/
+-rw-r--r--   0 runner    (1001) docker     (127)    13057 2024-04-23 12:01:35.000000 sentry_sdk-2.0.0rc6/sentry_sdk/integrations/celery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9813 2024-04-23 12:01:35.000000 sentry_sdk-2.0.0rc6/sentry_sdk/integrations/celery/beat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-04-23 12:01:35.000000 sentry_sdk-2.0.0rc6/sentry_sdk/integrations/celery/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4721 2024-04-23 12:01:35.000000 sentry_sdk-2.0.0rc6/sentry_sdk/integrations/chalice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5064 2024-04-23 12:01:35.000000 sentry_sdk-2.0.0rc6/sentry_sdk/integrations/clickhouse_driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6755 2024-04-23 12:01:35.000000 sentry_sdk-2.0.0rc6/sentry_sdk/integrations/cloud_resource_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-04-23 12:01:35.000000 sentry_sdk-2.0.0rc6/sentry_sdk/integrations/dedupe.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:01:43.661097 sentry_sdk-2.0.0rc6/sentry_sdk/integrations/django/
+-rw-r--r--   0 runner    (1001) docker     (127)    23519 2024-04-23 12:01:35.000000 sentry_sdk-2.0.0rc6/sentry_sdk/integrations/django/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6820 2024-04-23 12:01:35.000000 sentry_sdk-2.0.0rc6/sentry_sdk/integrations/django/asgi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3622 2024-04-23 12:01:35.000000 sentry_sdk-2.0.0rc6/sentry_sdk/integrations/django/caching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5770 2024-04-23 12:01:35.000000 sentry_sdk-2.0.0rc6/sentry_sdk/integrations/django/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3063 2024-04-23 12:01:35.000000 sentry_sdk-2.0.0rc6/sentry_sdk/integrations/django/signals_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5683 2024-04-23 12:01:35.000000 sentry_sdk-2.0.0rc6/sentry_sdk/integrations/django/templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4957 2024-04-23 12:01:35.000000 sentry_sdk-2.0.0rc6/sentry_sdk/integrations/django/transactions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2836 2024-04-23 12:01:35.000000 sentry_sdk-2.0.0rc6/sentry_sdk/integrations/django/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-04-23 12:01:35.000000 sentry_sdk-2.0.0rc6/sentry_sdk/integrations/excepthook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-04-23 12:01:35.000000 sentry_sdk-2.0.0rc6/sentry_sdk/integrations/executing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9347 2024-04-23 12:01:35.000000 sentry_sdk-2.0.0rc6/sentry_sdk/integrations/falcon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4543 2024-04-23 12:01:35.000000 sentry_sdk-2.0.0rc6/sentry_sdk/integrations/fastapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7706 2024-04-23 12:01:35.000000 sentry_sdk-2.0.0rc6/sentry_sdk/integrations/flask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8149 2024-04-23 12:01:35.000000 sentry_sdk-2.0.0rc6/sentry_sdk/integrations/gcp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2906 2024-04-23 12:01:35.000000 sentry_sdk-2.0.0rc6/sentry_sdk/integrations/gnu_backtrace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4386 2024-04-23 12:01:35.000000 sentry_sdk-2.0.0rc6/sentry_sdk/integrations/gql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3594 2024-04-23 12:01:35.000000 sentry_sdk-2.0.0rc6/sentry_sdk/integrations/graphene.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:01:43.665097 sentry_sdk-2.0.0rc6/sentry_sdk/integrations/grpc/
+-rw-r--r--   0 runner    (1001) docker     (127)     4979 2024-04-23 12:01:35.000000 sentry_sdk-2.0.0rc6/sentry_sdk/integrations/grpc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:01:43.665097 sentry_sdk-2.0.0rc6/sentry_sdk/integrations/grpc/aio/
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-23 12:01:35.000000 sentry_sdk-2.0.0rc6/sentry_sdk/integrations/grpc/aio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3075 2024-04-23 12:01:35.000000 sentry_sdk-2.0.0rc6/sentry_sdk/integrations/grpc/aio/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3866 2024-04-23 12:01:35.000000 sentry_sdk-2.0.0rc6/sentry_sdk/integrations/grpc/aio/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3249 2024-04-23 12:01:35.000000 sentry_sdk-2.0.0rc6/sentry_sdk/integrations/grpc/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2389 2024-04-23 12:01:35.000000 sentry_sdk-2.0.0rc6/sentry_sdk/integrations/grpc/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5165 2024-04-23 12:01:35.000000 sentry_sdk-2.0.0rc6/sentry_sdk/integrations/httpx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5260 2024-04-23 12:01:35.000000 sentry_sdk-2.0.0rc6/sentry_sdk/integrations/huey.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9592 2024-04-23 12:01:35.000000 sentry_sdk-2.0.0rc6/sentry_sdk/integrations/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3011 2024-04-23 12:01:35.000000 sentry_sdk-2.0.0rc6/sentry_sdk/integrations/loguru.py
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-04-23 12:01:35.000000 sentry_sdk-2.0.0rc6/sentry_sdk/integrations/modules.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11005 2024-04-23 12:01:35.000000 sentry_sdk-2.0.0rc6/sentry_sdk/integrations/openai.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:01:43.665097 sentry_sdk-2.0.0rc6/sentry_sdk/integrations/opentelemetry/
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-23 12:01:35.000000 sentry_sdk-2.0.0rc6/sentry_sdk/integrations/opentelemetry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-23 12:01:35.000000 sentry_sdk-2.0.0rc6/sentry_sdk/integrations/opentelemetry/consts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5830 2024-04-23 12:01:35.000000 sentry_sdk-2.0.0rc6/sentry_sdk/integrations/opentelemetry/integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3731 2024-04-23 12:01:35.000000 sentry_sdk-2.0.0rc6/sentry_sdk/integrations/opentelemetry/propagator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12225 2024-04-23 12:01:35.000000 sentry_sdk-2.0.0rc6/sentry_sdk/integrations/opentelemetry/span_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4539 2024-04-23 12:01:35.000000 sentry_sdk-2.0.0rc6/sentry_sdk/integrations/pure_eval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5994 2024-04-23 12:01:35.000000 sentry_sdk-2.0.0rc6/sentry_sdk/integrations/pymongo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7151 2024-04-23 12:01:35.000000 sentry_sdk-2.0.0rc6/sentry_sdk/integrations/pyramid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7091 2024-04-23 12:01:35.000000 sentry_sdk-2.0.0rc6/sentry_sdk/integrations/quart.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:01:43.665097 sentry_sdk-2.0.0rc6/sentry_sdk/integrations/redis/
+-rw-r--r--   0 runner    (1001) docker     (127)    11834 2024-04-23 12:01:35.000000 sentry_sdk-2.0.0rc6/sentry_sdk/integrations/redis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-04-23 12:01:35.000000 sentry_sdk-2.0.0rc6/sentry_sdk/integrations/redis/asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5297 2024-04-23 12:01:35.000000 sentry_sdk-2.0.0rc6/sentry_sdk/integrations/rq.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13127 2024-04-23 12:01:35.000000 sentry_sdk-2.0.0rc6/sentry_sdk/integrations/sanic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-04-23 12:01:35.000000 sentry_sdk-2.0.0rc6/sentry_sdk/integrations/serverless.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2906 2024-04-23 12:01:35.000000 sentry_sdk-2.0.0rc6/sentry_sdk/integrations/socket.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:01:43.665097 sentry_sdk-2.0.0rc6/sentry_sdk/integrations/spark/
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-23 12:01:35.000000 sentry_sdk-2.0.0rc6/sentry_sdk/integrations/spark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8276 2024-04-23 12:01:35.000000 sentry_sdk-2.0.0rc6/sentry_sdk/integrations/spark/spark_driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3747 2024-04-23 12:01:35.000000 sentry_sdk-2.0.0rc6/sentry_sdk/integrations/spark/spark_worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4865 2024-04-23 12:01:35.000000 sentry_sdk-2.0.0rc6/sentry_sdk/integrations/sqlalchemy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23504 2024-04-23 12:01:35.000000 sentry_sdk-2.0.0rc6/sentry_sdk/integrations/starlette.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9835 2024-04-23 12:01:35.000000 sentry_sdk-2.0.0rc6/sentry_sdk/integrations/starlite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8346 2024-04-23 12:01:35.000000 sentry_sdk-2.0.0rc6/sentry_sdk/integrations/stdlib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14574 2024-04-23 12:01:35.000000 sentry_sdk-2.0.0rc6/sentry_sdk/integrations/strawberry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4033 2024-04-23 12:01:35.000000 sentry_sdk-2.0.0rc6/sentry_sdk/integrations/threading.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7185 2024-04-23 12:01:35.000000 sentry_sdk-2.0.0rc6/sentry_sdk/integrations/tornado.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-04-23 12:01:35.000000 sentry_sdk-2.0.0rc6/sentry_sdk/integrations/trytond.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9870 2024-04-23 12:01:35.000000 sentry_sdk-2.0.0rc6/sentry_sdk/integrations/wsgi.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29725 2024-04-23 12:01:35.000000 sentry_sdk-2.0.0rc6/sentry_sdk/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3720 2024-04-23 12:01:35.000000 sentry_sdk-2.0.0rc6/sentry_sdk/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33332 2024-04-23 12:01:35.000000 sentry_sdk-2.0.0rc6/sentry_sdk/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 12:01:35.000000 sentry_sdk-2.0.0rc6/sentry_sdk/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    57649 2024-04-23 12:01:35.000000 sentry_sdk-2.0.0rc6/sentry_sdk/scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5082 2024-04-23 12:01:35.000000 sentry_sdk-2.0.0rc6/sentry_sdk/scrubber.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12729 2024-04-23 12:01:35.000000 sentry_sdk-2.0.0rc6/sentry_sdk/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5581 2024-04-23 12:01:35.000000 sentry_sdk-2.0.0rc6/sentry_sdk/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7822 2024-04-23 12:01:35.000000 sentry_sdk-2.0.0rc6/sentry_sdk/sessions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-04-23 12:01:35.000000 sentry_sdk-2.0.0rc6/sentry_sdk/spotlight.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38456 2024-04-23 12:01:35.000000 sentry_sdk-2.0.0rc6/sentry_sdk/tracing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17304 2024-04-23 12:01:35.000000 sentry_sdk-2.0.0rc6/sentry_sdk/tracing_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21002 2024-04-23 12:01:35.000000 sentry_sdk-2.0.0rc6/sentry_sdk/transport.py
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-04-23 12:01:35.000000 sentry_sdk-2.0.0rc6/sentry_sdk/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56591 2024-04-23 12:01:35.000000 sentry_sdk-2.0.0rc6/sentry_sdk/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4475 2024-04-23 12:01:35.000000 sentry_sdk-2.0.0rc6/sentry_sdk/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:01:43.669097 sentry_sdk-2.0.0rc6/sentry_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10503 2024-04-23 12:01:43.000000 sentry_sdk-2.0.0rc6/sentry_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-04-23 12:01:43.000000 sentry_sdk-2.0.0rc6/sentry_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 12:01:43.000000 sentry_sdk-2.0.0rc6/sentry_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 12:01:43.000000 sentry_sdk-2.0.0rc6/sentry_sdk.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-04-23 12:01:43.000000 sentry_sdk-2.0.0rc6/sentry_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-23 12:01:43.000000 sentry_sdk-2.0.0rc6/sentry_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 12:01:43.673097 sentry_sdk-2.0.0rc6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3836 2024-04-23 12:01:35.000000 sentry_sdk-2.0.0rc6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:01:43.669097 sentry_sdk-2.0.0rc6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4000 2024-04-23 12:01:35.000000 sentry_sdk-2.0.0rc6/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23225 2024-04-23 12:01:35.000000 sentry_sdk-2.0.0rc6/tests/test_basics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36053 2024-04-23 12:01:35.000000 sentry_sdk-2.0.0rc6/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3409 2024-04-23 12:01:35.000000 sentry_sdk-2.0.0rc6/tests/test_conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13795 2024-04-23 12:01:35.000000 sentry_sdk-2.0.0rc6/tests/test_crons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8057 2024-04-23 12:01:35.000000 sentry_sdk-2.0.0rc6/tests/test_envelope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8578 2024-04-23 12:01:35.000000 sentry_sdk-2.0.0rc6/tests/test_exceptiongroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-04-23 12:01:35.000000 sentry_sdk-2.0.0rc6/tests/test_lru_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29128 2024-04-23 12:01:35.000000 sentry_sdk-2.0.0rc6/tests/test_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2563 2024-04-23 12:01:35.000000 sentry_sdk-2.0.0rc6/tests/test_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8686 2024-04-23 12:01:35.000000 sentry_sdk-2.0.0rc6/tests/test_new_scopes_compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17288 2024-04-23 12:01:35.000000 sentry_sdk-2.0.0rc6/tests/test_new_scopes_compat_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23653 2024-04-23 12:01:35.000000 sentry_sdk-2.0.0rc6/tests/test_profiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25744 2024-04-23 12:01:35.000000 sentry_sdk-2.0.0rc6/tests/test_scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5357 2024-04-23 12:01:35.000000 sentry_sdk-2.0.0rc6/tests/test_scrubber.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4578 2024-04-23 12:01:35.000000 sentry_sdk-2.0.0rc6/tests/test_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4098 2024-04-23 12:01:35.000000 sentry_sdk-2.0.0rc6/tests/test_sessions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-04-23 12:01:35.000000 sentry_sdk-2.0.0rc6/tests/test_spotlight.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18754 2024-04-23 12:01:35.000000 sentry_sdk-2.0.0rc6/tests/test_transport.py
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-04-23 12:01:35.000000 sentry_sdk-2.0.0rc6/tests/test_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26384 2024-04-23 12:01:35.000000 sentry_sdk-2.0.0rc6/tests/test_utils.py
```

### Comparing `sentry-sdk-2.0.0rc5/LICENSE` & `sentry_sdk-2.0.0rc6/LICENSE`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc5/PKG-INFO` & `sentry_sdk-2.0.0rc6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sentry-sdk
-Version: 2.0.0rc5
+Version: 2.0.0rc6
 Summary: Python client for Sentry (https://sentry.io)
 Home-page: https://github.com/getsentry/sentry-python
 Author: Sentry Team and Contributors
 Author-email: hello@sentry.io
 License: MIT
 Project-URL: Documentation, https://docs.sentry.io/platforms/python/
 Project-URL: Changelog, https://github.com/getsentry/sentry-python/blob/master/CHANGELOG.md
```

### Comparing `sentry-sdk-2.0.0rc5/README.md` & `sentry_sdk-2.0.0rc6/README.md`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc5/sentry_sdk/__init__.py` & `sentry_sdk-2.0.0rc6/sentry_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc5/sentry_sdk/_compat.py` & `sentry_sdk-2.0.0rc6/sentry_sdk/_compat.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc5/sentry_sdk/_lru_cache.py` & `sentry_sdk-2.0.0rc6/sentry_sdk/_lru_cache.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc5/sentry_sdk/_queue.py` & `sentry_sdk-2.0.0rc6/sentry_sdk/_queue.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc5/sentry_sdk/_types.py` & `sentry_sdk-2.0.0rc6/sentry_sdk/_types.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc5/sentry_sdk/_werkzeug.py` & `sentry_sdk-2.0.0rc6/sentry_sdk/_werkzeug.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc5/sentry_sdk/api.py` & `sentry_sdk-2.0.0rc6/sentry_sdk/api.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc5/sentry_sdk/attachments.py` & `sentry_sdk-2.0.0rc6/sentry_sdk/attachments.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc5/sentry_sdk/client.py` & `sentry_sdk-2.0.0rc6/sentry_sdk/client.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc5/sentry_sdk/consts.py` & `sentry_sdk-2.0.0rc6/sentry_sdk/consts.py`

 * *Files 0% similar despite different names*

```diff
@@ -341,8 +341,8 @@
     return dict(zip(a.args[-len(defaults) :], defaults))
 
 
 DEFAULT_OPTIONS = _get_default_options()
 del _get_default_options
 
 
-VERSION = "2.0.0rc5"
+VERSION = "2.0.0rc6"
```

### Comparing `sentry-sdk-2.0.0rc5/sentry_sdk/crons/api.py` & `sentry_sdk-2.0.0rc6/sentry_sdk/crons/api.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc5/sentry_sdk/crons/decorator.py` & `sentry_sdk-2.0.0rc6/sentry_sdk/crons/decorator.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc5/sentry_sdk/db/explain_plan/__init__.py` & `sentry_sdk-2.0.0rc6/sentry_sdk/db/explain_plan/__init__.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc5/sentry_sdk/db/explain_plan/django.py` & `sentry_sdk-2.0.0rc6/sentry_sdk/db/explain_plan/django.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc5/sentry_sdk/db/explain_plan/sqlalchemy.py` & `sentry_sdk-2.0.0rc6/sentry_sdk/db/explain_plan/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc5/sentry_sdk/debug.py` & `sentry_sdk-2.0.0rc6/sentry_sdk/debug.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc5/sentry_sdk/envelope.py` & `sentry_sdk-2.0.0rc6/sentry_sdk/envelope.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc5/sentry_sdk/hub.py` & `sentry_sdk-2.0.0rc6/sentry_sdk/hub.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc5/sentry_sdk/integrations/__init__.py` & `sentry_sdk-2.0.0rc6/sentry_sdk/integrations/__init__.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc5/sentry_sdk/integrations/_asgi_common.py` & `sentry_sdk-2.0.0rc6/sentry_sdk/integrations/_asgi_common.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc5/sentry_sdk/integrations/_wsgi_common.py` & `sentry_sdk-2.0.0rc6/sentry_sdk/integrations/_wsgi_common.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc5/sentry_sdk/integrations/aiohttp.py` & `sentry_sdk-2.0.0rc6/sentry_sdk/integrations/aiohttp.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc5/sentry_sdk/integrations/argv.py` & `sentry_sdk-2.0.0rc6/sentry_sdk/integrations/argv.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc5/sentry_sdk/integrations/ariadne.py` & `sentry_sdk-2.0.0rc6/sentry_sdk/integrations/ariadne.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc5/sentry_sdk/integrations/arq.py` & `sentry_sdk-2.0.0rc6/sentry_sdk/integrations/arq.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc5/sentry_sdk/integrations/asgi.py` & `sentry_sdk-2.0.0rc6/sentry_sdk/integrations/asgi.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc5/sentry_sdk/integrations/asyncio.py` & `sentry_sdk-2.0.0rc6/sentry_sdk/integrations/asyncio.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc5/sentry_sdk/integrations/asyncpg.py` & `sentry_sdk-2.0.0rc6/sentry_sdk/integrations/asyncpg.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc5/sentry_sdk/integrations/atexit.py` & `sentry_sdk-2.0.0rc6/sentry_sdk/integrations/atexit.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc5/sentry_sdk/integrations/aws_lambda.py` & `sentry_sdk-2.0.0rc6/sentry_sdk/integrations/aws_lambda.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc5/sentry_sdk/integrations/beam.py` & `sentry_sdk-2.0.0rc6/sentry_sdk/integrations/beam.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc5/sentry_sdk/integrations/boto3.py` & `sentry_sdk-2.0.0rc6/sentry_sdk/integrations/boto3.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc5/sentry_sdk/integrations/bottle.py` & `sentry_sdk-2.0.0rc6/sentry_sdk/integrations/bottle.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc5/sentry_sdk/integrations/celery/__init__.py` & `sentry_sdk-2.0.0rc6/sentry_sdk/integrations/celery/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,33 +7,33 @@
 from sentry_sdk.consts import OP
 from sentry_sdk.integrations import Integration, DidNotEnable
 from sentry_sdk.integrations.celery.beat import (
     _patch_beat_apply_entry,
     _patch_redbeat_maybe_due,
     _setup_celery_beat_signals,
 )
-from sentry_sdk.integrations.celery.utils import NoOpMgr, _now_seconds_since_epoch
+from sentry_sdk.integrations.celery.utils import _now_seconds_since_epoch
 from sentry_sdk.integrations.logging import ignore_logger
 from sentry_sdk.tracing import BAGGAGE_HEADER_NAME, TRANSACTION_SOURCE_TASK
 from sentry_sdk._types import TYPE_CHECKING
 from sentry_sdk.scope import Scope
+from sentry_sdk.tracing_utils import Baggage
 from sentry_sdk.utils import (
     capture_internal_exceptions,
     ensure_integration_enabled,
     event_from_exception,
     reraise,
 )
 
 if TYPE_CHECKING:
     from typing import Any
     from typing import Callable
     from typing import List
     from typing import Optional
     from typing import TypeVar
-    from typing import Union
 
     from sentry_sdk._types import EventProcessor, Event, Hint, ExcInfo
     from sentry_sdk.tracing import Span
 
     F = TypeVar("F", bound=Callable[..., Any])
 
 
@@ -151,112 +151,107 @@
                     ]
 
         return event
 
     return event_processor
 
 
-def _wrap_apply_async(f):
-    # type: (F) -> F
+def _update_celery_task_headers(original_headers, span, monitor_beat_tasks):
+    # type: (dict[str, Any], Optional[Span], bool) -> dict[str, Any]
     """
-    Apply_async is always called to put a task in the queue. This is called by the
-    celery client (for example the Django project or the Celery Beat process)
+    Updates the headers of the Celery task with the tracing information
+    and eventually Sentry Crons monitoring information for beat tasks.
     """
+    updated_headers = original_headers.copy()
+    with capture_internal_exceptions():
+        headers = {}
+        if span is not None:
+            headers = dict(
+                Scope.get_current_scope().iter_trace_propagation_headers(span=span)
+            )
 
-    @wraps(f)
-    @ensure_integration_enabled(CeleryIntegration, f)
-    def apply_async(*args, **kwargs):
-        # type: (*Any, **Any) -> Any
-        task = args[0]
+        if monitor_beat_tasks:
+            headers.update(
+                {
+                    "sentry-monitor-start-timestamp-s": "%.9f"
+                    % _now_seconds_since_epoch(),
+                }
+            )
 
-        # Do not create a span when the task is a Celery Beat task
-        # (Because we do not have a transaction in that case)
-        span_mgr = (
-            sentry_sdk.start_span(op=OP.QUEUE_SUBMIT_CELERY, description=task.name)
-            if not Scope.get_isolation_scope()._name == "celery-beat"
-            else NoOpMgr()
-        )  # type: Union[Span, NoOpMgr]
-
-        with span_mgr as span:
-            incoming_headers = kwargs.get("headers") or {}
-            integration = sentry_sdk.get_client().get_integration(CeleryIntegration)
-
-            # If Sentry Crons monitoring for Celery Beat tasks is enabled
-            # add start timestamp of task,
-            if integration is not None and integration.monitor_beat_tasks:
-                incoming_headers.update(
-                    {
-                        "sentry-monitor-start-timestamp-s": "%.9f"
-                        % _now_seconds_since_epoch(),
-                    }
+        if headers:
+            existing_baggage = updated_headers.get(BAGGAGE_HEADER_NAME)
+            sentry_baggage = headers.get(BAGGAGE_HEADER_NAME)
+
+            combined_baggage = sentry_baggage or existing_baggage
+            if sentry_baggage and existing_baggage:
+                # Merge incoming and sentry baggage, where the sentry trace information
+                # in the incoming baggage takes precedence and the third-party items
+                # are concatenated.
+                incoming = Baggage.from_incoming_header(existing_baggage)
+                combined = Baggage.from_incoming_header(sentry_baggage)
+                combined.sentry_items.update(incoming.sentry_items)
+                combined.third_party_items = ",".join(
+                    [
+                        x
+                        for x in [
+                            combined.third_party_items,
+                            incoming.third_party_items,
+                        ]
+                        if x is not None and x != ""
+                    ]
                 )
+                combined_baggage = combined.serialize(include_third_party=True)
 
-            # Propagate Sentry trace information into the Celery task if desired
-            default_propagate_traces = (
-                integration.propagate_traces if integration is not None else True
-            )
-            propagate_traces = incoming_headers.pop(
-                "sentry-propagate-traces", default_propagate_traces
-            )
-
-            if propagate_traces:
-                with capture_internal_exceptions():
-                    sentry_trace_headers = dict(
-                        Scope.get_current_scope().iter_trace_propagation_headers(
-                            span=span
-                        )
-                    )
-                    # Set Sentry trace data in the headers of the Celery task
-                    if sentry_trace_headers:
-                        # Make sure we don't overwrite existing baggage
-                        incoming_baggage = incoming_headers.get(BAGGAGE_HEADER_NAME)
-                        sentry_baggage = sentry_trace_headers.get(BAGGAGE_HEADER_NAME)
-
-                        combined_baggage = sentry_baggage or incoming_baggage
-                        if sentry_baggage and incoming_baggage:
-                            combined_baggage = "{},{}".format(
-                                incoming_baggage,
-                                sentry_baggage,
-                            )
-
-                        # Set Sentry trace data to the headers of the Celery task
-                        incoming_headers.update(sentry_trace_headers)
-
-                        if combined_baggage:
-                            incoming_headers[BAGGAGE_HEADER_NAME] = combined_baggage
-
-                        # Set sentry trace data also to the inner headers of the Celery task
-                        # https://github.com/celery/celery/issues/4875
-                        #
-                        # Need to setdefault the inner headers too since other
-                        # tracing tools (dd-trace-py) also employ this exact
-                        # workaround and we don't want to break them.
-                        incoming_headers.setdefault("headers", {}).update(
-                            sentry_trace_headers
-                        )
-                        if combined_baggage:
-                            incoming_headers["headers"][
-                                BAGGAGE_HEADER_NAME
-                            ] = combined_baggage
+            updated_headers.update(headers)
+            if combined_baggage:
+                updated_headers[BAGGAGE_HEADER_NAME] = combined_baggage
 
-            # Add the Sentry options potentially added in `sentry_sdk.integrations.beat.sentry_apply_entry`
-            # to the inner headers (done when auto-instrumenting Celery Beat tasks)
             # https://github.com/celery/celery/issues/4875
             #
             # Need to setdefault the inner headers too since other
             # tracing tools (dd-trace-py) also employ this exact
             # workaround and we don't want to break them.
-            incoming_headers.setdefault("headers", {})
-            for key, value in incoming_headers.items():
+            updated_headers.setdefault("headers", {}).update(headers)
+            if combined_baggage:
+                updated_headers["headers"][BAGGAGE_HEADER_NAME] = combined_baggage
+
+            # Add the Sentry options potentially added in `sentry_apply_entry`
+            # to the headers (done when auto-instrumenting Celery Beat tasks)
+            for key, value in updated_headers.items():
                 if key.startswith("sentry-"):
-                    incoming_headers["headers"][key] = value
+                    updated_headers["headers"][key] = value
+
+    return updated_headers
+
+
+def _wrap_apply_async(f):
+    # type: (F) -> F
+    @wraps(f)
+    @ensure_integration_enabled(CeleryIntegration, f)
+    def apply_async(*args, **kwargs):
+        # type: (*Any, **Any) -> Any
+        # Note: kwargs can contain headers=None, so no setdefault!
+        # Unsure which backend though.
+        kwarg_headers = kwargs.get("headers") or {}
+        integration = sentry_sdk.get_client().get_integration(CeleryIntegration)
+        propagate_traces = kwarg_headers.pop(
+            "sentry-propagate-traces", integration.propagate_traces
+        )
 
-            # Run the task (with updated headers in kwargs)
-            kwargs["headers"] = incoming_headers
+        if not propagate_traces:
+            return f(*args, **kwargs)
 
+        task = args[0]
+
+        with sentry_sdk.start_span(
+            op=OP.QUEUE_SUBMIT_CELERY, description=task.name
+        ) as span:
+            kwargs["headers"] = _update_celery_task_headers(
+                kwarg_headers, span, integration.monitor_beat_tasks
+            )
             return f(*args, **kwargs)
 
     return apply_async  # type: ignore
 
 
 def _wrap_tracer(task, f):
     # type: (Any, F) -> F
```

### Comparing `sentry-sdk-2.0.0rc5/sentry_sdk/integrations/celery/beat.py` & `sentry_sdk-2.0.0rc6/sentry_sdk/integrations/celery/beat.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc5/sentry_sdk/integrations/celery/utils.py` & `sentry_sdk-2.0.0rc6/sentry_sdk/integrations/celery/utils.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc5/sentry_sdk/integrations/chalice.py` & `sentry_sdk-2.0.0rc6/sentry_sdk/integrations/chalice.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc5/sentry_sdk/integrations/clickhouse_driver.py` & `sentry_sdk-2.0.0rc6/sentry_sdk/integrations/clickhouse_driver.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc5/sentry_sdk/integrations/cloud_resource_context.py` & `sentry_sdk-2.0.0rc6/sentry_sdk/integrations/cloud_resource_context.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc5/sentry_sdk/integrations/dedupe.py` & `sentry_sdk-2.0.0rc6/sentry_sdk/integrations/dedupe.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc5/sentry_sdk/integrations/django/__init__.py` & `sentry_sdk-2.0.0rc6/sentry_sdk/integrations/django/__init__.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc5/sentry_sdk/integrations/django/asgi.py` & `sentry_sdk-2.0.0rc6/sentry_sdk/integrations/django/asgi.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc5/sentry_sdk/integrations/django/caching.py` & `sentry_sdk-2.0.0rc6/sentry_sdk/integrations/django/caching.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc5/sentry_sdk/integrations/django/middleware.py` & `sentry_sdk-2.0.0rc6/sentry_sdk/integrations/django/middleware.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc5/sentry_sdk/integrations/django/signals_handlers.py` & `sentry_sdk-2.0.0rc6/sentry_sdk/integrations/django/signals_handlers.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc5/sentry_sdk/integrations/django/templates.py` & `sentry_sdk-2.0.0rc6/sentry_sdk/integrations/django/templates.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc5/sentry_sdk/integrations/django/transactions.py` & `sentry_sdk-2.0.0rc6/sentry_sdk/integrations/django/transactions.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc5/sentry_sdk/integrations/django/views.py` & `sentry_sdk-2.0.0rc6/sentry_sdk/integrations/django/views.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc5/sentry_sdk/integrations/excepthook.py` & `sentry_sdk-2.0.0rc6/sentry_sdk/integrations/excepthook.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc5/sentry_sdk/integrations/executing.py` & `sentry_sdk-2.0.0rc6/sentry_sdk/integrations/executing.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc5/sentry_sdk/integrations/falcon.py` & `sentry_sdk-2.0.0rc6/sentry_sdk/integrations/falcon.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc5/sentry_sdk/integrations/fastapi.py` & `sentry_sdk-2.0.0rc6/sentry_sdk/integrations/fastapi.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc5/sentry_sdk/integrations/flask.py` & `sentry_sdk-2.0.0rc6/sentry_sdk/integrations/flask.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc5/sentry_sdk/integrations/gcp.py` & `sentry_sdk-2.0.0rc6/sentry_sdk/integrations/gcp.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc5/sentry_sdk/integrations/gnu_backtrace.py` & `sentry_sdk-2.0.0rc6/sentry_sdk/integrations/gnu_backtrace.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc5/sentry_sdk/integrations/gql.py` & `sentry_sdk-2.0.0rc6/sentry_sdk/integrations/gql.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc5/sentry_sdk/integrations/graphene.py` & `sentry_sdk-2.0.0rc6/sentry_sdk/integrations/graphene.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc5/sentry_sdk/integrations/grpc/__init__.py` & `sentry_sdk-2.0.0rc6/sentry_sdk/integrations/grpc/__init__.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc5/sentry_sdk/integrations/grpc/aio/client.py` & `sentry_sdk-2.0.0rc6/sentry_sdk/integrations/grpc/aio/client.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc5/sentry_sdk/integrations/grpc/aio/server.py` & `sentry_sdk-2.0.0rc6/sentry_sdk/integrations/grpc/aio/server.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc5/sentry_sdk/integrations/grpc/client.py` & `sentry_sdk-2.0.0rc6/sentry_sdk/integrations/grpc/client.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc5/sentry_sdk/integrations/grpc/server.py` & `sentry_sdk-2.0.0rc6/sentry_sdk/integrations/grpc/server.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc5/sentry_sdk/integrations/httpx.py` & `sentry_sdk-2.0.0rc6/sentry_sdk/integrations/httpx.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc5/sentry_sdk/integrations/huey.py` & `sentry_sdk-2.0.0rc6/sentry_sdk/integrations/huey.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc5/sentry_sdk/integrations/logging.py` & `sentry_sdk-2.0.0rc6/sentry_sdk/integrations/logging.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc5/sentry_sdk/integrations/loguru.py` & `sentry_sdk-2.0.0rc6/sentry_sdk/integrations/loguru.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc5/sentry_sdk/integrations/modules.py` & `sentry_sdk-2.0.0rc6/sentry_sdk/integrations/modules.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc5/sentry_sdk/integrations/openai.py` & `sentry_sdk-2.0.0rc6/sentry_sdk/integrations/openai.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc5/sentry_sdk/integrations/opentelemetry/integration.py` & `sentry_sdk-2.0.0rc6/sentry_sdk/integrations/opentelemetry/integration.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc5/sentry_sdk/integrations/opentelemetry/propagator.py` & `sentry_sdk-2.0.0rc6/sentry_sdk/integrations/opentelemetry/propagator.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc5/sentry_sdk/integrations/opentelemetry/span_processor.py` & `sentry_sdk-2.0.0rc6/sentry_sdk/integrations/opentelemetry/span_processor.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc5/sentry_sdk/integrations/pure_eval.py` & `sentry_sdk-2.0.0rc6/sentry_sdk/integrations/pure_eval.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc5/sentry_sdk/integrations/pymongo.py` & `sentry_sdk-2.0.0rc6/sentry_sdk/integrations/pymongo.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc5/sentry_sdk/integrations/pyramid.py` & `sentry_sdk-2.0.0rc6/sentry_sdk/integrations/pyramid.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc5/sentry_sdk/integrations/quart.py` & `sentry_sdk-2.0.0rc6/sentry_sdk/integrations/quart.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc5/sentry_sdk/integrations/redis/__init__.py` & `sentry_sdk-2.0.0rc6/sentry_sdk/integrations/redis/__init__.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc5/sentry_sdk/integrations/redis/asyncio.py` & `sentry_sdk-2.0.0rc6/sentry_sdk/integrations/redis/asyncio.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc5/sentry_sdk/integrations/rq.py` & `sentry_sdk-2.0.0rc6/sentry_sdk/integrations/rq.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc5/sentry_sdk/integrations/sanic.py` & `sentry_sdk-2.0.0rc6/sentry_sdk/integrations/sanic.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc5/sentry_sdk/integrations/serverless.py` & `sentry_sdk-2.0.0rc6/sentry_sdk/integrations/serverless.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc5/sentry_sdk/integrations/socket.py` & `sentry_sdk-2.0.0rc6/sentry_sdk/integrations/socket.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc5/sentry_sdk/integrations/spark/spark_driver.py` & `sentry_sdk-2.0.0rc6/sentry_sdk/integrations/spark/spark_driver.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc5/sentry_sdk/integrations/spark/spark_worker.py` & `sentry_sdk-2.0.0rc6/sentry_sdk/integrations/spark/spark_worker.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc5/sentry_sdk/integrations/sqlalchemy.py` & `sentry_sdk-2.0.0rc6/sentry_sdk/integrations/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc5/sentry_sdk/integrations/starlette.py` & `sentry_sdk-2.0.0rc6/sentry_sdk/integrations/starlette.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc5/sentry_sdk/integrations/starlite.py` & `sentry_sdk-2.0.0rc6/sentry_sdk/integrations/starlite.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc5/sentry_sdk/integrations/stdlib.py` & `sentry_sdk-2.0.0rc6/sentry_sdk/integrations/stdlib.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc5/sentry_sdk/integrations/strawberry.py` & `sentry_sdk-2.0.0rc6/sentry_sdk/integrations/strawberry.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc5/sentry_sdk/integrations/threading.py` & `sentry_sdk-2.0.0rc6/sentry_sdk/integrations/threading.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc5/sentry_sdk/integrations/tornado.py` & `sentry_sdk-2.0.0rc6/sentry_sdk/integrations/tornado.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc5/sentry_sdk/integrations/trytond.py` & `sentry_sdk-2.0.0rc6/sentry_sdk/integrations/trytond.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc5/sentry_sdk/integrations/wsgi.py` & `sentry_sdk-2.0.0rc6/sentry_sdk/integrations/wsgi.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc5/sentry_sdk/metrics.py` & `sentry_sdk-2.0.0rc6/sentry_sdk/metrics.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc5/sentry_sdk/monitor.py` & `sentry_sdk-2.0.0rc6/sentry_sdk/monitor.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc5/sentry_sdk/profiler.py` & `sentry_sdk-2.0.0rc6/sentry_sdk/profiler.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc5/sentry_sdk/scope.py` & `sentry_sdk-2.0.0rc6/sentry_sdk/scope.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc5/sentry_sdk/scrubber.py` & `sentry_sdk-2.0.0rc6/sentry_sdk/scrubber.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc5/sentry_sdk/serializer.py` & `sentry_sdk-2.0.0rc6/sentry_sdk/serializer.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc5/sentry_sdk/session.py` & `sentry_sdk-2.0.0rc6/sentry_sdk/session.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc5/sentry_sdk/sessions.py` & `sentry_sdk-2.0.0rc6/sentry_sdk/sessions.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc5/sentry_sdk/spotlight.py` & `sentry_sdk-2.0.0rc6/sentry_sdk/spotlight.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc5/sentry_sdk/tracing.py` & `sentry_sdk-2.0.0rc6/sentry_sdk/tracing.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc5/sentry_sdk/tracing_utils.py` & `sentry_sdk-2.0.0rc6/sentry_sdk/tracing_utils.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc5/sentry_sdk/transport.py` & `sentry_sdk-2.0.0rc6/sentry_sdk/transport.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc5/sentry_sdk/types.py` & `sentry_sdk-2.0.0rc6/sentry_sdk/types.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc5/sentry_sdk/utils.py` & `sentry_sdk-2.0.0rc6/sentry_sdk/utils.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc5/sentry_sdk/worker.py` & `sentry_sdk-2.0.0rc6/sentry_sdk/worker.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc5/sentry_sdk.egg-info/PKG-INFO` & `sentry_sdk-2.0.0rc6/sentry_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sentry-sdk
-Version: 2.0.0rc5
+Version: 2.0.0rc6
 Summary: Python client for Sentry (https://sentry.io)
 Home-page: https://github.com/getsentry/sentry-python
 Author: Sentry Team and Contributors
 Author-email: hello@sentry.io
 License: MIT
 Project-URL: Documentation, https://docs.sentry.io/platforms/python/
 Project-URL: Changelog, https://github.com/getsentry/sentry-python/blob/master/CHANGELOG.md
```

### Comparing `sentry-sdk-2.0.0rc5/sentry_sdk.egg-info/SOURCES.txt` & `sentry_sdk-2.0.0rc6/sentry_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc5/sentry_sdk.egg-info/requires.txt` & `sentry_sdk-2.0.0rc6/sentry_sdk.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc5/setup.py` & `sentry_sdk-2.0.0rc6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 def get_file_text(file_name):
     with open(os.path.join(here, file_name)) as in_file:
         return in_file.read()
 
 
 setup(
     name="sentry-sdk",
-    version="2.0.0rc5",
+    version="2.0.0rc6",
     author="Sentry Team and Contributors",
     author_email="hello@sentry.io",
     url="https://github.com/getsentry/sentry-python",
     project_urls={
         "Documentation": "https://docs.sentry.io/platforms/python/",
         "Changelog": "https://github.com/getsentry/sentry-python/blob/master/CHANGELOG.md",
     },
```

### Comparing `sentry-sdk-2.0.0rc5/tests/test_api.py` & `sentry_sdk-2.0.0rc6/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc5/tests/test_basics.py` & `sentry_sdk-2.0.0rc6/tests/test_basics.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc5/tests/test_client.py` & `sentry_sdk-2.0.0rc6/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc5/tests/test_conftest.py` & `sentry_sdk-2.0.0rc6/tests/test_conftest.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc5/tests/test_crons.py` & `sentry_sdk-2.0.0rc6/tests/test_crons.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc5/tests/test_envelope.py` & `sentry_sdk-2.0.0rc6/tests/test_envelope.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc5/tests/test_exceptiongroup.py` & `sentry_sdk-2.0.0rc6/tests/test_exceptiongroup.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc5/tests/test_lru_cache.py` & `sentry_sdk-2.0.0rc6/tests/test_lru_cache.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc5/tests/test_metrics.py` & `sentry_sdk-2.0.0rc6/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc5/tests/test_monitor.py` & `sentry_sdk-2.0.0rc6/tests/test_monitor.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc5/tests/test_new_scopes_compat.py` & `sentry_sdk-2.0.0rc6/tests/test_new_scopes_compat.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc5/tests/test_new_scopes_compat_event.py` & `sentry_sdk-2.0.0rc6/tests/test_new_scopes_compat_event.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc5/tests/test_profiler.py` & `sentry_sdk-2.0.0rc6/tests/test_profiler.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc5/tests/test_scope.py` & `sentry_sdk-2.0.0rc6/tests/test_scope.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc5/tests/test_scrubber.py` & `sentry_sdk-2.0.0rc6/tests/test_scrubber.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc5/tests/test_serializer.py` & `sentry_sdk-2.0.0rc6/tests/test_serializer.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc5/tests/test_sessions.py` & `sentry_sdk-2.0.0rc6/tests/test_sessions.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc5/tests/test_spotlight.py` & `sentry_sdk-2.0.0rc6/tests/test_spotlight.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc5/tests/test_transport.py` & `sentry_sdk-2.0.0rc6/tests/test_transport.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc5/tests/test_types.py` & `sentry_sdk-2.0.0rc6/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `sentry-sdk-2.0.0rc5/tests/test_utils.py` & `sentry_sdk-2.0.0rc6/tests/test_utils.py`

 * *Files identical despite different names*


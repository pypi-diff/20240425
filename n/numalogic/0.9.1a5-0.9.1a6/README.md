# Comparing `tmp/numalogic-0.9.1a5.tar.gz` & `tmp/numalogic-0.9.1a6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "numalogic-0.9.1a5.tar", max compression
+gzip compressed data, was "numalogic-0.9.1a6.tar", max compression
```

## Comparing `numalogic-0.9.1a5.tar` & `numalogic-0.9.1a6.tar`

### file list

```diff
@@ -1,106 +1,106 @@
--rw-r--r--   0        0        0    11357 2024-04-23 21:43:22.905017 numalogic-0.9.1a5/LICENSE
--rw-r--r--   0        0        0     5244 2024-04-23 21:43:22.905017 numalogic-0.9.1a5/README.md
--rw-r--r--   0        0        0      676 2024-04-23 21:43:22.925017 numalogic-0.9.1a5/numalogic/__init__.py
--rw-r--r--   0        0        0     1016 2024-04-23 21:43:22.925017 numalogic-0.9.1a5/numalogic/_constants.py
--rw-r--r--   0        0        0      413 2024-04-23 21:43:22.925017 numalogic-0.9.1a5/numalogic/backtest/__init__.py
--rw-r--r--   0        0        0      248 2024-04-23 21:43:22.925017 numalogic-0.9.1a5/numalogic/backtest/_constants.py
--rw-r--r--   0        0        0    15806 2024-04-23 21:43:22.925017 numalogic-0.9.1a5/numalogic/backtest/_prom.py
--rw-r--r--   0        0        0     1636 2024-04-23 21:43:22.925017 numalogic-0.9.1a5/numalogic/base.py
--rw-r--r--   0        0        0     1102 2024-04-23 21:43:22.925017 numalogic-0.9.1a5/numalogic/blocks/__init__.py
--rw-r--r--   0        0        0     4672 2024-04-23 21:43:22.925017 numalogic-0.9.1a5/numalogic/blocks/_base.py
--rw-r--r--   0        0        0     3229 2024-04-23 21:43:22.925017 numalogic-0.9.1a5/numalogic/blocks/_nn.py
--rw-r--r--   0        0        0     3906 2024-04-23 21:43:22.925017 numalogic-0.9.1a5/numalogic/blocks/_transform.py
--rw-r--r--   0        0        0     5776 2024-04-23 21:43:22.925017 numalogic-0.9.1a5/numalogic/blocks/pipeline.py
--rw-r--r--   0        0        0     1271 2024-04-23 21:43:22.925017 numalogic-0.9.1a5/numalogic/config/__init__.py
--rw-r--r--   0        0        0     4818 2024-04-23 21:43:22.925017 numalogic-0.9.1a5/numalogic/config/_config.py
--rw-r--r--   0        0        0     7543 2024-04-23 21:43:22.925017 numalogic-0.9.1a5/numalogic/config/factory.py
--rw-r--r--   0        0        0      550 2024-04-23 21:43:22.925017 numalogic-0.9.1a5/numalogic/connectors/__init__.py
--rw-r--r--   0        0        0      689 2024-04-23 21:43:22.925017 numalogic-0.9.1a5/numalogic/connectors/_base.py
--rw-r--r--   0        0        0     1709 2024-04-23 21:43:22.925017 numalogic-0.9.1a5/numalogic/connectors/_config.py
--rw-r--r--   0        0        0      157 2024-04-23 21:43:22.925017 numalogic-0.9.1a5/numalogic/connectors/druid/__init__.py
--rw-r--r--   0        0        0     9647 2024-04-23 21:43:22.925017 numalogic-0.9.1a5/numalogic/connectors/druid/_druid.py
--rw-r--r--   0        0        0      765 2024-04-23 21:43:22.925017 numalogic-0.9.1a5/numalogic/connectors/druid/aggregators.py
--rw-r--r--   0        0        0      696 2024-04-23 21:43:22.925017 numalogic-0.9.1a5/numalogic/connectors/druid/postaggregator.py
--rw-r--r--   0        0        0    10150 2024-04-23 21:43:22.925017 numalogic-0.9.1a5/numalogic/connectors/prometheus.py
--rw-r--r--   0        0        0       79 2024-04-23 21:43:22.925017 numalogic-0.9.1a5/numalogic/connectors/rds/__init__.py
--rw-r--r--   0        0        0     5022 2024-04-23 21:43:22.925017 numalogic-0.9.1a5/numalogic/connectors/rds/_base.py
--rw-r--r--   0        0        0     2608 2024-04-23 21:43:22.925017 numalogic-0.9.1a5/numalogic/connectors/rds/_rds.py
--rw-r--r--   0        0        0        0 2024-04-23 21:43:22.929017 numalogic-0.9.1a5/numalogic/connectors/rds/db/__init__.py
--rw-r--r--   0        0        0     1061 2024-04-23 21:43:22.929017 numalogic-0.9.1a5/numalogic/connectors/rds/db/factory.py
--rw-r--r--   0        0        0     4193 2024-04-23 21:43:22.929017 numalogic-0.9.1a5/numalogic/connectors/rds/db/mysql_fetcher.py
--rw-r--r--   0        0        0     2734 2024-04-23 21:43:22.929017 numalogic-0.9.1a5/numalogic/connectors/redis.py
--rw-r--r--   0        0        0        0 2024-04-23 21:43:22.929017 numalogic-0.9.1a5/numalogic/connectors/utils/__init__.py
--rw-r--r--   0        0        0        0 2024-04-23 21:43:22.929017 numalogic-0.9.1a5/numalogic/connectors/utils/aws/__init__.py
--rw-r--r--   0        0        0     5637 2024-04-23 21:43:22.929017 numalogic-0.9.1a5/numalogic/connectors/utils/aws/boto3_client_manager.py
--rw-r--r--   0        0        0     4636 2024-04-23 21:43:22.929017 numalogic-0.9.1a5/numalogic/connectors/utils/aws/config.py
--rw-r--r--   0        0        0     1265 2024-04-23 21:43:22.929017 numalogic-0.9.1a5/numalogic/connectors/utils/aws/db_configurations.py
--rw-r--r--   0        0        0     1738 2024-04-23 21:43:22.929017 numalogic-0.9.1a5/numalogic/connectors/utils/aws/exceptions.py
--rw-r--r--   0        0        0     3346 2024-04-23 21:43:22.929017 numalogic-0.9.1a5/numalogic/connectors/utils/aws/sts_client_manager.py
--rw-r--r--   0        0        0     2181 2024-04-23 21:43:22.929017 numalogic-0.9.1a5/numalogic/connectors/utils/enum.py
--rw-r--r--   0        0        0        0 2024-04-23 21:43:22.929017 numalogic-0.9.1a5/numalogic/models/__init__.py
--rw-r--r--   0        0        0      668 2024-04-23 21:43:22.929017 numalogic-0.9.1a5/numalogic/models/autoencoder/__init__.py
--rw-r--r--   0        0        0     3419 2024-04-23 21:43:22.929017 numalogic-0.9.1a5/numalogic/models/autoencoder/base.py
--rw-r--r--   0        0        0      581 2024-04-23 21:43:22.929017 numalogic-0.9.1a5/numalogic/models/autoencoder/variants/__init__.py
--rw-r--r--   0        0        0    11705 2024-04-23 21:43:22.929017 numalogic-0.9.1a5/numalogic/models/autoencoder/variants/conv.py
--rw-r--r--   0        0        0     6599 2024-04-23 21:43:22.929017 numalogic-0.9.1a5/numalogic/models/autoencoder/variants/lstm.py
--rw-r--r--   0        0        0    14335 2024-04-23 21:43:22.929017 numalogic-0.9.1a5/numalogic/models/autoencoder/variants/transformer.py
--rw-r--r--   0        0        0     8420 2024-04-23 21:43:22.929017 numalogic-0.9.1a5/numalogic/models/autoencoder/variants/vanilla.py
--rw-r--r--   0        0        0        0 2024-04-23 21:43:22.929017 numalogic-0.9.1a5/numalogic/models/forecast/__init__.py
--rw-r--r--   0        0        0      158 2024-04-23 21:43:22.929017 numalogic-0.9.1a5/numalogic/models/forecast/variants/__init__.py
--rw-r--r--   0        0        0     4289 2024-04-23 21:43:22.929017 numalogic-0.9.1a5/numalogic/models/forecast/variants/naive.py
--rw-r--r--   0        0        0      489 2024-04-23 21:43:22.929017 numalogic-0.9.1a5/numalogic/models/threshold/__init__.py
--rw-r--r--   0        0        0     7531 2024-04-23 21:43:22.929017 numalogic-0.9.1a5/numalogic/models/threshold/_mahalanobis.py
--rw-r--r--   0        0        0     2943 2024-04-23 21:43:22.929017 numalogic-0.9.1a5/numalogic/models/threshold/_median.py
--rw-r--r--   0        0        0     4720 2024-04-23 21:43:22.929017 numalogic-0.9.1a5/numalogic/models/threshold/_static.py
--rw-r--r--   0        0        0     2462 2024-04-23 21:43:22.929017 numalogic-0.9.1a5/numalogic/models/threshold/_std.py
--rw-r--r--   0        0        0       77 2024-04-23 21:43:22.929017 numalogic-0.9.1a5/numalogic/models/vae/__init__.py
--rw-r--r--   0        0        0     2046 2024-04-23 21:43:22.929017 numalogic-0.9.1a5/numalogic/models/vae/base.py
--rw-r--r--   0        0        0     1536 2024-04-23 21:43:22.929017 numalogic-0.9.1a5/numalogic/models/vae/layer.py
--rw-r--r--   0        0        0       82 2024-04-23 21:43:22.929017 numalogic-0.9.1a5/numalogic/models/vae/variants/__init__.py
--rw-r--r--   0        0        0     7916 2024-04-23 21:43:22.929017 numalogic-0.9.1a5/numalogic/models/vae/variants/conv.py
--rw-r--r--   0        0        0      975 2024-04-23 21:43:22.929017 numalogic-0.9.1a5/numalogic/monitoring/__init__.py
--rw-r--r--   0        0        0     3906 2024-04-23 21:43:22.929017 numalogic-0.9.1a5/numalogic/monitoring/metrics.py
--rw-r--r--   0        0        0     1282 2024-04-23 21:43:22.929017 numalogic-0.9.1a5/numalogic/registry/__init__.py
--rw-r--r--   0        0        0      651 2024-04-23 21:43:22.929017 numalogic-0.9.1a5/numalogic/registry/_serialize.py
--rw-r--r--   0        0        0     6734 2024-04-23 21:43:22.929017 numalogic-0.9.1a5/numalogic/registry/artifact.py
--rw-r--r--   0        0        0    15564 2024-04-23 21:43:22.929017 numalogic-0.9.1a5/numalogic/registry/dynamodb_registry.py
--rw-r--r--   0        0        0     3334 2024-04-23 21:43:22.929017 numalogic-0.9.1a5/numalogic/registry/localcache.py
--rw-r--r--   0        0        0    13536 2024-04-23 21:43:22.929017 numalogic-0.9.1a5/numalogic/registry/mlflow_registry.py
--rw-r--r--   0        0        0    16600 2024-04-23 21:43:22.929017 numalogic-0.9.1a5/numalogic/registry/redis_registry.py
--rw-r--r--   0        0        0      841 2024-04-23 21:43:22.929017 numalogic-0.9.1a5/numalogic/synthetic/__init__.py
--rw-r--r--   0        0        0    12457 2024-04-23 21:43:22.929017 numalogic-0.9.1a5/numalogic/synthetic/anomalies.py
--rw-r--r--   0        0        0     1637 2024-04-23 21:43:22.929017 numalogic-0.9.1a5/numalogic/synthetic/sparsity.py
--rw-r--r--   0        0        0     4739 2024-04-23 21:43:22.929017 numalogic-0.9.1a5/numalogic/synthetic/timeseries.py
--rw-r--r--   0        0        0        0 2024-04-23 21:43:22.929017 numalogic-0.9.1a5/numalogic/tools/__init__.py
--rw-r--r--   0        0        0      631 2024-04-23 21:43:22.929017 numalogic-0.9.1a5/numalogic/tools/aggregators.py
--rw-r--r--   0        0        0     3615 2024-04-23 21:43:22.929017 numalogic-0.9.1a5/numalogic/tools/callbacks.py
--rw-r--r--   0        0        0    10245 2024-04-23 21:43:22.929017 numalogic-0.9.1a5/numalogic/tools/data.py
--rw-r--r--   0        0        0     2545 2024-04-23 21:43:22.929017 numalogic-0.9.1a5/numalogic/tools/exceptions.py
--rw-r--r--   0        0        0     3168 2024-04-23 21:43:22.929017 numalogic-0.9.1a5/numalogic/tools/trainer.py
--rw-r--r--   0        0        0     2237 2024-04-23 21:43:22.929017 numalogic-0.9.1a5/numalogic/tools/types.py
--rw-r--r--   0        0        0     1418 2024-04-23 21:43:22.929017 numalogic-0.9.1a5/numalogic/transforms/__init__.py
--rw-r--r--   0        0        0     4006 2024-04-23 21:43:22.929017 numalogic-0.9.1a5/numalogic/transforms/_movavg.py
--rw-r--r--   0        0        0     2252 2024-04-23 21:43:22.929017 numalogic-0.9.1a5/numalogic/transforms/_postprocess.py
--rw-r--r--   0        0        0     4772 2024-04-23 21:43:22.929017 numalogic-0.9.1a5/numalogic/transforms/_scaler.py
--rw-r--r--   0        0        0     5178 2024-04-23 21:43:22.929017 numalogic-0.9.1a5/numalogic/transforms/_stateless.py
--rw-r--r--   0        0        0     3560 2024-04-23 21:43:22.929017 numalogic-0.9.1a5/numalogic/udfs/README.md
--rw-r--r--   0        0        0     1232 2024-04-23 21:43:22.929017 numalogic-0.9.1a5/numalogic/udfs/__init__.py
--rw-r--r--   0        0        0     1937 2024-04-23 21:43:22.929017 numalogic-0.9.1a5/numalogic/udfs/__main__.py
--rw-r--r--   0        0        0     5192 2024-04-23 21:43:22.929017 numalogic-0.9.1a5/numalogic/udfs/_base.py
--rw-r--r--   0        0        0     3711 2024-04-23 21:43:22.929017 numalogic-0.9.1a5/numalogic/udfs/_config.py
--rw-r--r--   0        0        0     1060 2024-04-23 21:43:22.929017 numalogic-0.9.1a5/numalogic/udfs/_logger.py
--rw-r--r--   0        0        0     4923 2024-04-23 21:43:22.929017 numalogic-0.9.1a5/numalogic/udfs/_metrics.py
--rw-r--r--   0        0        0     3376 2024-04-23 21:43:22.929017 numalogic-0.9.1a5/numalogic/udfs/entities.py
--rw-r--r--   0        0        0     4298 2024-04-23 21:43:22.929017 numalogic-0.9.1a5/numalogic/udfs/factory.py
--rw-r--r--   0        0        0     7349 2024-04-23 21:43:22.929017 numalogic-0.9.1a5/numalogic/udfs/inference.py
--rw-r--r--   0        0        0     2196 2024-04-23 21:43:22.929017 numalogic-0.9.1a5/numalogic/udfs/payloadtx.py
--rw-r--r--   0        0        0    15595 2024-04-23 21:43:22.929017 numalogic-0.9.1a5/numalogic/udfs/postprocess.py
--rw-r--r--   0        0        0     9286 2024-04-23 21:43:22.929017 numalogic-0.9.1a5/numalogic/udfs/preprocess.py
--rw-r--r--   0        0        0     5581 2024-04-23 21:43:22.929017 numalogic-0.9.1a5/numalogic/udfs/staticthresh.py
--rw-r--r--   0        0        0    14920 2024-04-23 21:43:22.929017 numalogic-0.9.1a5/numalogic/udfs/tools.py
--rw-r--r--   0        0        0      229 2024-04-23 21:43:22.933017 numalogic-0.9.1a5/numalogic/udfs/trainer/__init__.py
--rw-r--r--   0        0        0    13821 2024-04-23 21:43:22.933017 numalogic-0.9.1a5/numalogic/udfs/trainer/_base.py
--rw-r--r--   0        0        0     5187 2024-04-23 21:43:22.933017 numalogic-0.9.1a5/numalogic/udfs/trainer/_druid.py
--rw-r--r--   0        0        0     3816 2024-04-23 21:43:22.933017 numalogic-0.9.1a5/numalogic/udfs/trainer/_prom.py
--rw-r--r--   0        0        0     3032 2024-04-23 21:43:22.933017 numalogic-0.9.1a5/pyproject.toml
--rw-r--r--   0        0        0     6954 1970-01-01 00:00:00.000000 numalogic-0.9.1a5/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-25 01:13:07.723840 numalogic-0.9.1a6/LICENSE
+-rw-r--r--   0        0        0     5244 2024-04-25 01:13:07.723840 numalogic-0.9.1a6/README.md
+-rw-r--r--   0        0        0      676 2024-04-25 01:13:07.743840 numalogic-0.9.1a6/numalogic/__init__.py
+-rw-r--r--   0        0        0     1016 2024-04-25 01:13:07.743840 numalogic-0.9.1a6/numalogic/_constants.py
+-rw-r--r--   0        0        0      413 2024-04-25 01:13:07.743840 numalogic-0.9.1a6/numalogic/backtest/__init__.py
+-rw-r--r--   0        0        0      248 2024-04-25 01:13:07.743840 numalogic-0.9.1a6/numalogic/backtest/_constants.py
+-rw-r--r--   0        0        0    16031 2024-04-25 01:13:07.743840 numalogic-0.9.1a6/numalogic/backtest/_prom.py
+-rw-r--r--   0        0        0     1636 2024-04-25 01:13:07.743840 numalogic-0.9.1a6/numalogic/base.py
+-rw-r--r--   0        0        0     1102 2024-04-25 01:13:07.743840 numalogic-0.9.1a6/numalogic/blocks/__init__.py
+-rw-r--r--   0        0        0     4672 2024-04-25 01:13:07.743840 numalogic-0.9.1a6/numalogic/blocks/_base.py
+-rw-r--r--   0        0        0     3229 2024-04-25 01:13:07.743840 numalogic-0.9.1a6/numalogic/blocks/_nn.py
+-rw-r--r--   0        0        0     3906 2024-04-25 01:13:07.743840 numalogic-0.9.1a6/numalogic/blocks/_transform.py
+-rw-r--r--   0        0        0     5776 2024-04-25 01:13:07.743840 numalogic-0.9.1a6/numalogic/blocks/pipeline.py
+-rw-r--r--   0        0        0     1271 2024-04-25 01:13:07.743840 numalogic-0.9.1a6/numalogic/config/__init__.py
+-rw-r--r--   0        0        0     4818 2024-04-25 01:13:07.743840 numalogic-0.9.1a6/numalogic/config/_config.py
+-rw-r--r--   0        0        0     7543 2024-04-25 01:13:07.743840 numalogic-0.9.1a6/numalogic/config/factory.py
+-rw-r--r--   0        0        0      550 2024-04-25 01:13:07.743840 numalogic-0.9.1a6/numalogic/connectors/__init__.py
+-rw-r--r--   0        0        0      689 2024-04-25 01:13:07.743840 numalogic-0.9.1a6/numalogic/connectors/_base.py
+-rw-r--r--   0        0        0     1709 2024-04-25 01:13:07.743840 numalogic-0.9.1a6/numalogic/connectors/_config.py
+-rw-r--r--   0        0        0      157 2024-04-25 01:13:07.743840 numalogic-0.9.1a6/numalogic/connectors/druid/__init__.py
+-rw-r--r--   0        0        0     9647 2024-04-25 01:13:07.743840 numalogic-0.9.1a6/numalogic/connectors/druid/_druid.py
+-rw-r--r--   0        0        0      765 2024-04-25 01:13:07.743840 numalogic-0.9.1a6/numalogic/connectors/druid/aggregators.py
+-rw-r--r--   0        0        0      696 2024-04-25 01:13:07.743840 numalogic-0.9.1a6/numalogic/connectors/druid/postaggregator.py
+-rw-r--r--   0        0        0    10150 2024-04-25 01:13:07.743840 numalogic-0.9.1a6/numalogic/connectors/prometheus.py
+-rw-r--r--   0        0        0       79 2024-04-25 01:13:07.743840 numalogic-0.9.1a6/numalogic/connectors/rds/__init__.py
+-rw-r--r--   0        0        0     5022 2024-04-25 01:13:07.743840 numalogic-0.9.1a6/numalogic/connectors/rds/_base.py
+-rw-r--r--   0        0        0     2608 2024-04-25 01:13:07.743840 numalogic-0.9.1a6/numalogic/connectors/rds/_rds.py
+-rw-r--r--   0        0        0        0 2024-04-25 01:13:07.743840 numalogic-0.9.1a6/numalogic/connectors/rds/db/__init__.py
+-rw-r--r--   0        0        0     1061 2024-04-25 01:13:07.747840 numalogic-0.9.1a6/numalogic/connectors/rds/db/factory.py
+-rw-r--r--   0        0        0     4193 2024-04-25 01:13:07.747840 numalogic-0.9.1a6/numalogic/connectors/rds/db/mysql_fetcher.py
+-rw-r--r--   0        0        0     2734 2024-04-25 01:13:07.747840 numalogic-0.9.1a6/numalogic/connectors/redis.py
+-rw-r--r--   0        0        0        0 2024-04-25 01:13:07.747840 numalogic-0.9.1a6/numalogic/connectors/utils/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-25 01:13:07.747840 numalogic-0.9.1a6/numalogic/connectors/utils/aws/__init__.py
+-rw-r--r--   0        0        0     5637 2024-04-25 01:13:07.747840 numalogic-0.9.1a6/numalogic/connectors/utils/aws/boto3_client_manager.py
+-rw-r--r--   0        0        0     4636 2024-04-25 01:13:07.747840 numalogic-0.9.1a6/numalogic/connectors/utils/aws/config.py
+-rw-r--r--   0        0        0     1265 2024-04-25 01:13:07.747840 numalogic-0.9.1a6/numalogic/connectors/utils/aws/db_configurations.py
+-rw-r--r--   0        0        0     1738 2024-04-25 01:13:07.747840 numalogic-0.9.1a6/numalogic/connectors/utils/aws/exceptions.py
+-rw-r--r--   0        0        0     3346 2024-04-25 01:13:07.747840 numalogic-0.9.1a6/numalogic/connectors/utils/aws/sts_client_manager.py
+-rw-r--r--   0        0        0     2181 2024-04-25 01:13:07.747840 numalogic-0.9.1a6/numalogic/connectors/utils/enum.py
+-rw-r--r--   0        0        0        0 2024-04-25 01:13:07.747840 numalogic-0.9.1a6/numalogic/models/__init__.py
+-rw-r--r--   0        0        0      668 2024-04-25 01:13:07.747840 numalogic-0.9.1a6/numalogic/models/autoencoder/__init__.py
+-rw-r--r--   0        0        0     3419 2024-04-25 01:13:07.747840 numalogic-0.9.1a6/numalogic/models/autoencoder/base.py
+-rw-r--r--   0        0        0      581 2024-04-25 01:13:07.747840 numalogic-0.9.1a6/numalogic/models/autoencoder/variants/__init__.py
+-rw-r--r--   0        0        0    11705 2024-04-25 01:13:07.747840 numalogic-0.9.1a6/numalogic/models/autoencoder/variants/conv.py
+-rw-r--r--   0        0        0     6599 2024-04-25 01:13:07.747840 numalogic-0.9.1a6/numalogic/models/autoencoder/variants/lstm.py
+-rw-r--r--   0        0        0    14335 2024-04-25 01:13:07.747840 numalogic-0.9.1a6/numalogic/models/autoencoder/variants/transformer.py
+-rw-r--r--   0        0        0     8562 2024-04-25 01:13:07.747840 numalogic-0.9.1a6/numalogic/models/autoencoder/variants/vanilla.py
+-rw-r--r--   0        0        0        0 2024-04-25 01:13:07.747840 numalogic-0.9.1a6/numalogic/models/forecast/__init__.py
+-rw-r--r--   0        0        0      158 2024-04-25 01:13:07.747840 numalogic-0.9.1a6/numalogic/models/forecast/variants/__init__.py
+-rw-r--r--   0        0        0     4289 2024-04-25 01:13:07.747840 numalogic-0.9.1a6/numalogic/models/forecast/variants/naive.py
+-rw-r--r--   0        0        0      489 2024-04-25 01:13:07.747840 numalogic-0.9.1a6/numalogic/models/threshold/__init__.py
+-rw-r--r--   0        0        0     7531 2024-04-25 01:13:07.747840 numalogic-0.9.1a6/numalogic/models/threshold/_mahalanobis.py
+-rw-r--r--   0        0        0     2943 2024-04-25 01:13:07.747840 numalogic-0.9.1a6/numalogic/models/threshold/_median.py
+-rw-r--r--   0        0        0     4720 2024-04-25 01:13:07.747840 numalogic-0.9.1a6/numalogic/models/threshold/_static.py
+-rw-r--r--   0        0        0     2462 2024-04-25 01:13:07.747840 numalogic-0.9.1a6/numalogic/models/threshold/_std.py
+-rw-r--r--   0        0        0       77 2024-04-25 01:13:07.747840 numalogic-0.9.1a6/numalogic/models/vae/__init__.py
+-rw-r--r--   0        0        0     2046 2024-04-25 01:13:07.747840 numalogic-0.9.1a6/numalogic/models/vae/base.py
+-rw-r--r--   0        0        0     1536 2024-04-25 01:13:07.747840 numalogic-0.9.1a6/numalogic/models/vae/layer.py
+-rw-r--r--   0        0        0       82 2024-04-25 01:13:07.747840 numalogic-0.9.1a6/numalogic/models/vae/variants/__init__.py
+-rw-r--r--   0        0        0     7916 2024-04-25 01:13:07.747840 numalogic-0.9.1a6/numalogic/models/vae/variants/conv.py
+-rw-r--r--   0        0        0      975 2024-04-25 01:13:07.747840 numalogic-0.9.1a6/numalogic/monitoring/__init__.py
+-rw-r--r--   0        0        0     3906 2024-04-25 01:13:07.747840 numalogic-0.9.1a6/numalogic/monitoring/metrics.py
+-rw-r--r--   0        0        0     1282 2024-04-25 01:13:07.747840 numalogic-0.9.1a6/numalogic/registry/__init__.py
+-rw-r--r--   0        0        0      651 2024-04-25 01:13:07.747840 numalogic-0.9.1a6/numalogic/registry/_serialize.py
+-rw-r--r--   0        0        0     6734 2024-04-25 01:13:07.747840 numalogic-0.9.1a6/numalogic/registry/artifact.py
+-rw-r--r--   0        0        0    15564 2024-04-25 01:13:07.747840 numalogic-0.9.1a6/numalogic/registry/dynamodb_registry.py
+-rw-r--r--   0        0        0     3334 2024-04-25 01:13:07.747840 numalogic-0.9.1a6/numalogic/registry/localcache.py
+-rw-r--r--   0        0        0    13536 2024-04-25 01:13:07.747840 numalogic-0.9.1a6/numalogic/registry/mlflow_registry.py
+-rw-r--r--   0        0        0    16600 2024-04-25 01:13:07.747840 numalogic-0.9.1a6/numalogic/registry/redis_registry.py
+-rw-r--r--   0        0        0      841 2024-04-25 01:13:07.747840 numalogic-0.9.1a6/numalogic/synthetic/__init__.py
+-rw-r--r--   0        0        0    12457 2024-04-25 01:13:07.747840 numalogic-0.9.1a6/numalogic/synthetic/anomalies.py
+-rw-r--r--   0        0        0     1637 2024-04-25 01:13:07.747840 numalogic-0.9.1a6/numalogic/synthetic/sparsity.py
+-rw-r--r--   0        0        0     4739 2024-04-25 01:13:07.747840 numalogic-0.9.1a6/numalogic/synthetic/timeseries.py
+-rw-r--r--   0        0        0        0 2024-04-25 01:13:07.747840 numalogic-0.9.1a6/numalogic/tools/__init__.py
+-rw-r--r--   0        0        0      631 2024-04-25 01:13:07.747840 numalogic-0.9.1a6/numalogic/tools/aggregators.py
+-rw-r--r--   0        0        0     3615 2024-04-25 01:13:07.747840 numalogic-0.9.1a6/numalogic/tools/callbacks.py
+-rw-r--r--   0        0        0    10279 2024-04-25 01:13:07.747840 numalogic-0.9.1a6/numalogic/tools/data.py
+-rw-r--r--   0        0        0     2545 2024-04-25 01:13:07.747840 numalogic-0.9.1a6/numalogic/tools/exceptions.py
+-rw-r--r--   0        0        0     3168 2024-04-25 01:13:07.747840 numalogic-0.9.1a6/numalogic/tools/trainer.py
+-rw-r--r--   0        0        0     2237 2024-04-25 01:13:07.747840 numalogic-0.9.1a6/numalogic/tools/types.py
+-rw-r--r--   0        0        0     1418 2024-04-25 01:13:07.747840 numalogic-0.9.1a6/numalogic/transforms/__init__.py
+-rw-r--r--   0        0        0     4006 2024-04-25 01:13:07.747840 numalogic-0.9.1a6/numalogic/transforms/_movavg.py
+-rw-r--r--   0        0        0     2252 2024-04-25 01:13:07.747840 numalogic-0.9.1a6/numalogic/transforms/_postprocess.py
+-rw-r--r--   0        0        0     4772 2024-04-25 01:13:07.747840 numalogic-0.9.1a6/numalogic/transforms/_scaler.py
+-rw-r--r--   0        0        0     5178 2024-04-25 01:13:07.747840 numalogic-0.9.1a6/numalogic/transforms/_stateless.py
+-rw-r--r--   0        0        0     3560 2024-04-25 01:13:07.747840 numalogic-0.9.1a6/numalogic/udfs/README.md
+-rw-r--r--   0        0        0     1232 2024-04-25 01:13:07.747840 numalogic-0.9.1a6/numalogic/udfs/__init__.py
+-rw-r--r--   0        0        0     1937 2024-04-25 01:13:07.747840 numalogic-0.9.1a6/numalogic/udfs/__main__.py
+-rw-r--r--   0        0        0     5192 2024-04-25 01:13:07.747840 numalogic-0.9.1a6/numalogic/udfs/_base.py
+-rw-r--r--   0        0        0     3711 2024-04-25 01:13:07.747840 numalogic-0.9.1a6/numalogic/udfs/_config.py
+-rw-r--r--   0        0        0     1060 2024-04-25 01:13:07.747840 numalogic-0.9.1a6/numalogic/udfs/_logger.py
+-rw-r--r--   0        0        0     4923 2024-04-25 01:13:07.747840 numalogic-0.9.1a6/numalogic/udfs/_metrics.py
+-rw-r--r--   0        0        0     3376 2024-04-25 01:13:07.747840 numalogic-0.9.1a6/numalogic/udfs/entities.py
+-rw-r--r--   0        0        0     4298 2024-04-25 01:13:07.747840 numalogic-0.9.1a6/numalogic/udfs/factory.py
+-rw-r--r--   0        0        0     7317 2024-04-25 01:13:07.747840 numalogic-0.9.1a6/numalogic/udfs/inference.py
+-rw-r--r--   0        0        0     2196 2024-04-25 01:13:07.747840 numalogic-0.9.1a6/numalogic/udfs/payloadtx.py
+-rw-r--r--   0        0        0    15595 2024-04-25 01:13:07.747840 numalogic-0.9.1a6/numalogic/udfs/postprocess.py
+-rw-r--r--   0        0        0     9286 2024-04-25 01:13:07.747840 numalogic-0.9.1a6/numalogic/udfs/preprocess.py
+-rw-r--r--   0        0        0     5581 2024-04-25 01:13:07.747840 numalogic-0.9.1a6/numalogic/udfs/staticthresh.py
+-rw-r--r--   0        0        0    14920 2024-04-25 01:13:07.747840 numalogic-0.9.1a6/numalogic/udfs/tools.py
+-rw-r--r--   0        0        0      229 2024-04-25 01:13:07.751840 numalogic-0.9.1a6/numalogic/udfs/trainer/__init__.py
+-rw-r--r--   0        0        0    14056 2024-04-25 01:13:07.751840 numalogic-0.9.1a6/numalogic/udfs/trainer/_base.py
+-rw-r--r--   0        0        0     5187 2024-04-25 01:13:07.751840 numalogic-0.9.1a6/numalogic/udfs/trainer/_druid.py
+-rw-r--r--   0        0        0     3816 2024-04-25 01:13:07.751840 numalogic-0.9.1a6/numalogic/udfs/trainer/_prom.py
+-rw-r--r--   0        0        0     3032 2024-04-25 01:13:07.751840 numalogic-0.9.1a6/pyproject.toml
+-rw-r--r--   0        0        0     6954 1970-01-01 00:00:00.000000 numalogic-0.9.1a6/PKG-INFO
```

### Comparing `numalogic-0.9.1a5/LICENSE` & `numalogic-0.9.1a6/LICENSE`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a5/README.md` & `numalogic-0.9.1a6/README.md`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a5/numalogic/__init__.py` & `numalogic-0.9.1a6/numalogic/__init__.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a5/numalogic/_constants.py` & `numalogic-0.9.1a6/numalogic/_constants.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a5/numalogic/backtest/_prom.py` & `numalogic-0.9.1a6/numalogic/backtest/_prom.py`

 * *Files 2% similar despite different names*

```diff
@@ -133,17 +133,22 @@
             df = df[self.metrics]
 
         df_train, _ = self._split_data(df)
 
         x_train = df_train.to_numpy(dtype=np.float32)
         LOGGER.info("Training data shape: %s", x_train.shape)
 
+        if self.nlconf.trainer.transforms:
+            train_txs = PreprocessFactory().get_pipeline_instance(self.nlconf.trainer.transforms)
+        else:
+            train_txs = None
         artifacts = UDFFactory.get_udf_cls("promtrainer").compute(
             model=ModelFactory().get_instance(self.nlconf.model),
             input_=x_train,
+            trainer_transform=train_txs,
             preproc_clf=PreprocessFactory().get_pipeline_instance(self.nlconf.preprocess),
             threshold_clf=ThresholdFactory().get_instance(self.nlconf.threshold),
             numalogic_cfg=self.nlconf,
         )
         artifacts_dict = {
             "model": artifacts["inference"].artifact,
             "preproc_clf": artifacts["preproc_clf"].artifact,
```

### Comparing `numalogic-0.9.1a5/numalogic/base.py` & `numalogic-0.9.1a6/numalogic/base.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a5/numalogic/blocks/__init__.py` & `numalogic-0.9.1a6/numalogic/blocks/__init__.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a5/numalogic/blocks/_base.py` & `numalogic-0.9.1a6/numalogic/blocks/_base.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a5/numalogic/blocks/_nn.py` & `numalogic-0.9.1a6/numalogic/blocks/_nn.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a5/numalogic/blocks/_transform.py` & `numalogic-0.9.1a6/numalogic/blocks/_transform.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a5/numalogic/blocks/pipeline.py` & `numalogic-0.9.1a6/numalogic/blocks/pipeline.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a5/numalogic/config/__init__.py` & `numalogic-0.9.1a6/numalogic/config/__init__.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a5/numalogic/config/_config.py` & `numalogic-0.9.1a6/numalogic/config/_config.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a5/numalogic/config/factory.py` & `numalogic-0.9.1a6/numalogic/config/factory.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a5/numalogic/connectors/__init__.py` & `numalogic-0.9.1a6/numalogic/connectors/__init__.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a5/numalogic/connectors/_base.py` & `numalogic-0.9.1a6/numalogic/connectors/_base.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a5/numalogic/connectors/_config.py` & `numalogic-0.9.1a6/numalogic/connectors/_config.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a5/numalogic/connectors/druid/_druid.py` & `numalogic-0.9.1a6/numalogic/connectors/druid/_druid.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a5/numalogic/connectors/druid/aggregators.py` & `numalogic-0.9.1a6/numalogic/connectors/druid/aggregators.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a5/numalogic/connectors/druid/postaggregator.py` & `numalogic-0.9.1a6/numalogic/connectors/druid/postaggregator.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a5/numalogic/connectors/prometheus.py` & `numalogic-0.9.1a6/numalogic/connectors/prometheus.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a5/numalogic/connectors/rds/_base.py` & `numalogic-0.9.1a6/numalogic/connectors/rds/_base.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a5/numalogic/connectors/rds/_rds.py` & `numalogic-0.9.1a6/numalogic/connectors/rds/_rds.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a5/numalogic/connectors/rds/db/factory.py` & `numalogic-0.9.1a6/numalogic/connectors/rds/db/factory.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a5/numalogic/connectors/rds/db/mysql_fetcher.py` & `numalogic-0.9.1a6/numalogic/connectors/rds/db/mysql_fetcher.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a5/numalogic/connectors/redis.py` & `numalogic-0.9.1a6/numalogic/connectors/redis.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a5/numalogic/connectors/utils/aws/boto3_client_manager.py` & `numalogic-0.9.1a6/numalogic/connectors/utils/aws/boto3_client_manager.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a5/numalogic/connectors/utils/aws/config.py` & `numalogic-0.9.1a6/numalogic/connectors/utils/aws/config.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a5/numalogic/connectors/utils/aws/db_configurations.py` & `numalogic-0.9.1a6/numalogic/connectors/utils/aws/db_configurations.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a5/numalogic/connectors/utils/aws/exceptions.py` & `numalogic-0.9.1a6/numalogic/connectors/utils/aws/exceptions.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a5/numalogic/connectors/utils/aws/sts_client_manager.py` & `numalogic-0.9.1a6/numalogic/connectors/utils/aws/sts_client_manager.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a5/numalogic/connectors/utils/enum.py` & `numalogic-0.9.1a6/numalogic/connectors/utils/enum.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a5/numalogic/models/autoencoder/__init__.py` & `numalogic-0.9.1a6/numalogic/models/autoencoder/__init__.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a5/numalogic/models/autoencoder/base.py` & `numalogic-0.9.1a6/numalogic/models/autoencoder/base.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a5/numalogic/models/autoencoder/variants/__init__.py` & `numalogic-0.9.1a6/numalogic/models/autoencoder/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a5/numalogic/models/autoencoder/variants/conv.py` & `numalogic-0.9.1a6/numalogic/models/autoencoder/variants/conv.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a5/numalogic/models/autoencoder/variants/lstm.py` & `numalogic-0.9.1a6/numalogic/models/autoencoder/variants/lstm.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a5/numalogic/models/autoencoder/variants/transformer.py` & `numalogic-0.9.1a6/numalogic/models/autoencoder/variants/transformer.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a5/numalogic/models/autoencoder/variants/vanilla.py` & `numalogic-0.9.1a6/numalogic/models/autoencoder/variants/vanilla.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,26 +55,28 @@
         layers = nn.ModuleList()
         start_layersize = self.seq_len
 
         for lsize in layersizes[:-1]:
             layers.extend(
                 [
                     nn.Linear(start_layersize, lsize),
-                    nn.BatchNorm1d(self.n_features),
+                    # nn.BatchNorm1d(self.n_features),
                     nn.Tanh(),
                     nn.Dropout(p=self.dropout_p),
                 ]
             )
             start_layersize = lsize
 
         layers.extend(
             [
                 nn.Linear(start_layersize, layersizes[-1]),
-                nn.BatchNorm1d(self.n_features),
-                nn.ReLU(),
+                # nn.BatchNorm1d(self.n_features),
+                # nn.ReLU(),
+                nn.Tanh(),
+                nn.Dropout(p=self.dropout_p),
             ]
         )
         return layers
 
     def forward(self, x: Tensor) -> Tensor:
         return self.encoder(x)
 
@@ -116,15 +118,15 @@
         """
         layers = nn.ModuleList()
 
         for idx, _ in enumerate(layersizes[:-1]):
             layers.extend(
                 [
                     nn.Linear(layersizes[idx], layersizes[idx + 1]),
-                    nn.BatchNorm1d(self.n_features),
+                    # nn.BatchNorm1d(self.n_features),
                     nn.Tanh(),
                     nn.Dropout(p=self.dropout_p),
                 ]
             )
 
         layers.append(nn.Linear(layersizes[-1], self.seq_len))
         return layers
@@ -186,22 +188,22 @@
 
     def forward(self, batch: Tensor) -> tuple[Tensor, Tensor]:
         batch = torch.swapdims(batch, 1, 2)
         encoded = self.encoder(batch)
         decoded = self.decoder(encoded)
         return encoded, torch.swapdims(decoded, 1, 2)
 
-    def _get_reconstruction_loss(self, batch: Tensor):
+    def _get_reconstruction_loss(self, batch: Tensor, reduction="mean") -> Tensor:
         _, recon = self.forward(batch)
-        return self.criterion(batch, recon)
+        return 0.5 * self.criterion(batch, recon, reduction=reduction)
 
     def predict_step(self, batch: Tensor, batch_idx: int, dataloader_idx: int = 0):
         """Returns reconstruction for streaming input."""
         recon = self.reconstruction(batch)
-        return self.criterion(batch, recon, reduction="none")
+        return 0.5 * self.criterion(batch, recon, reduction="none")
 
 
 class SparseVanillaAE(VanillaAE):
     r"""Sparse Autoencoder for a fully connected network.
     It inherits from VanillaAE class and serves as a wrapper around base network models.
     Sparse Autoencoder is a type of autoencoder that applies sparsity constraint.
     This helps in achieving information bottleneck even when the number of hidden units is huge.
```

### Comparing `numalogic-0.9.1a5/numalogic/models/forecast/variants/naive.py` & `numalogic-0.9.1a6/numalogic/models/forecast/variants/naive.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a5/numalogic/models/threshold/_mahalanobis.py` & `numalogic-0.9.1a6/numalogic/models/threshold/_mahalanobis.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a5/numalogic/models/threshold/_median.py` & `numalogic-0.9.1a6/numalogic/models/threshold/_median.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a5/numalogic/models/threshold/_static.py` & `numalogic-0.9.1a6/numalogic/models/threshold/_static.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a5/numalogic/models/threshold/_std.py` & `numalogic-0.9.1a6/numalogic/models/threshold/_std.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a5/numalogic/models/vae/base.py` & `numalogic-0.9.1a6/numalogic/models/vae/base.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a5/numalogic/models/vae/layer.py` & `numalogic-0.9.1a6/numalogic/models/vae/layer.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a5/numalogic/models/vae/variants/conv.py` & `numalogic-0.9.1a6/numalogic/models/vae/variants/conv.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a5/numalogic/monitoring/__init__.py` & `numalogic-0.9.1a6/numalogic/monitoring/__init__.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a5/numalogic/monitoring/metrics.py` & `numalogic-0.9.1a6/numalogic/monitoring/metrics.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a5/numalogic/registry/__init__.py` & `numalogic-0.9.1a6/numalogic/registry/__init__.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a5/numalogic/registry/_serialize.py` & `numalogic-0.9.1a6/numalogic/registry/_serialize.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a5/numalogic/registry/artifact.py` & `numalogic-0.9.1a6/numalogic/registry/artifact.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a5/numalogic/registry/dynamodb_registry.py` & `numalogic-0.9.1a6/numalogic/registry/dynamodb_registry.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a5/numalogic/registry/localcache.py` & `numalogic-0.9.1a6/numalogic/registry/localcache.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a5/numalogic/registry/mlflow_registry.py` & `numalogic-0.9.1a6/numalogic/registry/mlflow_registry.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a5/numalogic/registry/redis_registry.py` & `numalogic-0.9.1a6/numalogic/registry/redis_registry.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a5/numalogic/synthetic/__init__.py` & `numalogic-0.9.1a6/numalogic/synthetic/__init__.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a5/numalogic/synthetic/anomalies.py` & `numalogic-0.9.1a6/numalogic/synthetic/anomalies.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a5/numalogic/synthetic/sparsity.py` & `numalogic-0.9.1a6/numalogic/synthetic/sparsity.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a5/numalogic/synthetic/timeseries.py` & `numalogic-0.9.1a6/numalogic/synthetic/timeseries.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a5/numalogic/tools/aggregators.py` & `numalogic-0.9.1a6/numalogic/tools/aggregators.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a5/numalogic/tools/callbacks.py` & `numalogic-0.9.1a6/numalogic/tools/callbacks.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a5/numalogic/tools/data.py` & `numalogic-0.9.1a6/numalogic/tools/data.py`

 * *Files 0% similar despite different names*

```diff
@@ -187,15 +187,15 @@
             start = idx.start or 0
             stop = min(idx.stop, raw_data_size) if idx.stop else raw_data_size
             for i in range(start, stop - self._seq_len + 1, self._stride):
                 output.append(self._data[i : (i + self._seq_len)])
             return np.stack(output)
         if idx >= len(self):
             raise IndexError(f"{idx} out of bound!")
-        return self._data[idx : idx + self._seq_len]
+        return self._data[(idx * self._stride) : (idx * self._stride) + self._seq_len]
 
 
 class StreamingDataLoader(DataLoader):
     """
     A DataLoader for convenience that uses StreamingDataset for handling time series data.
 
     Args:
```

### Comparing `numalogic-0.9.1a5/numalogic/tools/exceptions.py` & `numalogic-0.9.1a6/numalogic/tools/exceptions.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a5/numalogic/tools/trainer.py` & `numalogic-0.9.1a6/numalogic/tools/trainer.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a5/numalogic/tools/types.py` & `numalogic-0.9.1a6/numalogic/tools/types.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a5/numalogic/transforms/__init__.py` & `numalogic-0.9.1a6/numalogic/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a5/numalogic/transforms/_movavg.py` & `numalogic-0.9.1a6/numalogic/transforms/_movavg.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a5/numalogic/transforms/_postprocess.py` & `numalogic-0.9.1a6/numalogic/transforms/_postprocess.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a5/numalogic/transforms/_scaler.py` & `numalogic-0.9.1a6/numalogic/transforms/_scaler.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a5/numalogic/transforms/_stateless.py` & `numalogic-0.9.1a6/numalogic/transforms/_stateless.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a5/numalogic/udfs/README.md` & `numalogic-0.9.1a6/numalogic/udfs/README.md`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a5/numalogic/udfs/__init__.py` & `numalogic-0.9.1a6/numalogic/udfs/__init__.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a5/numalogic/udfs/__main__.py` & `numalogic-0.9.1a6/numalogic/udfs/__main__.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a5/numalogic/udfs/_base.py` & `numalogic-0.9.1a6/numalogic/udfs/_base.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a5/numalogic/udfs/_config.py` & `numalogic-0.9.1a6/numalogic/udfs/_config.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a5/numalogic/udfs/_logger.py` & `numalogic-0.9.1a6/numalogic/udfs/_logger.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a5/numalogic/udfs/_metrics.py` & `numalogic-0.9.1a6/numalogic/udfs/_metrics.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a5/numalogic/udfs/entities.py` & `numalogic-0.9.1a6/numalogic/udfs/entities.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a5/numalogic/udfs/factory.py` & `numalogic-0.9.1a6/numalogic/udfs/factory.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a5/numalogic/udfs/inference.py` & `numalogic-0.9.1a6/numalogic/udfs/inference.py`

 * *Files 0% similar despite different names*

```diff
@@ -80,16 +80,15 @@
         ------
             RuntimeError: If model forward pass fails
         """
         x = torch.from_numpy(input_).unsqueeze(0)
         model.eval()
         try:
             with torch.no_grad():
-                _, out = model.forward(x)
-                recon_err = model.criterion(out, x, reduction="none")
+                recon_err = model._get_reconstruction_loss(x, reduction="none")
         except Exception as err:
             raise RuntimeError("Model forward pass failed!") from err
         return np.ascontiguousarray(recon_err).squeeze(0)
 
     @UDF_TIME.time()
     def exec(self, keys: list[str], datum: Datum) -> Messages:
         """
```

### Comparing `numalogic-0.9.1a5/numalogic/udfs/payloadtx.py` & `numalogic-0.9.1a6/numalogic/udfs/payloadtx.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a5/numalogic/udfs/postprocess.py` & `numalogic-0.9.1a6/numalogic/udfs/postprocess.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a5/numalogic/udfs/preprocess.py` & `numalogic-0.9.1a6/numalogic/udfs/preprocess.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a5/numalogic/udfs/staticthresh.py` & `numalogic-0.9.1a6/numalogic/udfs/staticthresh.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a5/numalogic/udfs/tools.py` & `numalogic-0.9.1a6/numalogic/udfs/tools.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a5/numalogic/udfs/trainer/_base.py` & `numalogic-0.9.1a6/numalogic/udfs/trainer/_base.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,14 +29,15 @@
     MSG_PROCESSED_COUNTER,
     UDF_TIME,
     _increment_counter,
     _add_summary,
 )
 from numalogic.udfs.entities import TrainerPayload
 from numalogic.udfs.tools import TrainMsgDeduplicator
+import torch
 
 _struct_log = configure_logger()
 
 
 class TrainerUDF(NumalogicUDF):
     """
     Trainer UDF for Numalogic.
@@ -116,16 +117,20 @@
 
         train_ds = StreamingDataset(input_, model.seq_len, stride=trainer_cfg.ds_stride)
         trainer = TimeseriesTrainer(**asdict(trainer_cfg.pltrainer_conf))
         trainer.fit(
             model, train_dataloaders=DataLoader(train_ds, batch_size=trainer_cfg.batch_size)
         )
         train_reconerr = trainer.predict(
-            model, dataloaders=DataLoader(train_ds, batch_size=trainer_cfg.batch_size)
-        ).numpy()
+            model,
+            dataloaders=DataLoader(train_ds, batch_size=trainer_cfg.batch_size),
+            unbatch=False,
+        )
+        train_reconerr = torch.mean(train_reconerr, dim=1).numpy()
+
         dict_artifacts["inference"] = KeyedArtifact(
             dkeys=[numalogic_cfg.model.name], artifact=model, stateful=numalogic_cfg.model.stateful
         )
 
         if threshold_clf:
             threshold_clf.fit(train_reconerr)
             _struct_log.debug("Fit data using threshold model")
@@ -229,20 +234,20 @@
         logger.debug("Data fetched", uuid=payload.uuid, shape=df.shape)
 
         # Construct feature array
         x_train, nan_counter, inf_counter = self.get_feature_arr(df, _conf.metrics)
         _add_summary(
             summary=NAN_SUMMARY,
             labels=_metric_label_values,
-            data=nan_counter,
+            data=np.sum(nan_counter),
         )
         _add_summary(
             summary=INF_SUMMARY,
             labels=_metric_label_values,
-            data=inf_counter,
+            data=np.sum(inf_counter),
         )
 
         # Initialize artifacts
         preproc_clf = self._construct_clf(_conf.numalogic_conf.preprocess)
         trainer_transform = self._construct_clf(_conf.numalogic_conf.trainer.transforms)
         model = self._model_factory.get_instance(_conf.numalogic_conf.model)
         thresh_clf = self._thresh_factory.get_instance(_conf.numalogic_conf.threshold)
@@ -359,37 +364,38 @@
 
     # TODO: Use a custom impute in transforms module
     @staticmethod
     def get_feature_arr(
         raw_df: pd.DataFrame,
         metrics: list[str],
         fill_value: float = 0.0,
-    ) -> tuple[npt.NDArray[float], float, float]:
+    ) -> tuple[npt.NDArray[float], pd.Series, pd.Series]:
         """
         Get feature array from the raw dataframe.
 
         Args:
             raw_df: Raw dataframe
             metrics: List of metrics
             fill_value: Value to fill missing values with
 
         Returns
         -------
             Numpy array
             nan_counter: Number of nan values
             inf_counter: Number of inf values
         """
-        nan_counter = 0
-        for col in metrics:
+        nan_counter = np.zeros(len(metrics), dtype=int)
+        inf_counter = np.zeros(len(metrics), dtype=int)
+        for idx, col in enumerate(metrics):
             if col not in raw_df.columns:
                 raw_df[col] = fill_value
-                nan_counter += len(raw_df)
+                nan_counter[idx] += len(raw_df)
         feat_df = raw_df[metrics]
-        nan_counter += raw_df.isna().sum().all()
-        inf_counter = np.isinf(feat_df).sum().all()
+        nan_counter += feat_df.isna().sum()
+        inf_counter = np.isinf(feat_df).sum()
         feat_df = feat_df.fillna(fill_value).replace([np.inf, -np.inf], fill_value)
         return feat_df.to_numpy(dtype=np.float32), nan_counter, inf_counter
 
     def fetch_data(self, payload: TrainerPayload) -> Optional[pd.DataFrame]:
         """
         Fetch data from a data connector.
```

### Comparing `numalogic-0.9.1a5/numalogic/udfs/trainer/_druid.py` & `numalogic-0.9.1a6/numalogic/udfs/trainer/_druid.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a5/numalogic/udfs/trainer/_prom.py` & `numalogic-0.9.1a6/numalogic/udfs/trainer/_prom.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a5/pyproject.toml` & `numalogic-0.9.1a6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "numalogic"
-version = "0.9.1a5"
+version = "0.9.1a6"
 description = "Collection of operational Machine Learning models and tools."
 authors = ["Numalogic Developers"]
 packages = [{ include = "numalogic" }]
 readme = "README.md"
 license = "Apache-2.0"
 maintainers = [
     "Avik Basu <avikbasu93@gmail.com>",
```

### Comparing `numalogic-0.9.1a5/PKG-INFO` & `numalogic-0.9.1a6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: numalogic
-Version: 0.9.1a5
+Version: 0.9.1a6
 Summary: Collection of operational Machine Learning models and tools.
 Home-page: https://numalogic.numaproj.io/
 License: Apache-2.0
 Author: Numalogic Developers
 Maintainer: Avik Basu
 Maintainer-email: avikbasu93@gmail.com
 Requires-Python: >=3.9,<3.12
```


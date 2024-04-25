# Comparing `tmp/fiddler-client-3.1.0.dev1.tar.gz` & `tmp/fiddler-client-3.1.0.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fiddler-client-3.1.0.dev1.tar", last modified: Tue Apr  9 16:33:41 2024, max compression
+gzip compressed data, was "fiddler-client-3.1.0.dev2.tar", last modified: Fri Apr 19 12:21:13 2024, max compression
```

## Comparing `fiddler-client-3.1.0.dev1.tar` & `fiddler-client-3.1.0.dev2.tar`

### file list

```diff
@@ -1,126 +1,126 @@
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-09 16:33:41.733792 fiddler-client-3.1.0.dev1/
--rw-r--r--   0 runner    (1001) runner    (1001)      559 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/LICENSE.txt
--rw-r--r--   0 runner    (1001) runner    (1001)       42 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/MANIFEST.in
--rw-r--r--   0 runner    (1001) runner    (1001)    20672 2024-04-09 16:33:41.733792 fiddler-client-3.1.0.dev1/PKG-INFO
--rw-r--r--   0 runner    (1001) runner    (1001)    19978 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/PUBLIC.md
--rw-r--r--   0 runner    (1001) runner    (1001)     2165 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/README.md
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-09 16:33:41.713794 fiddler-client-3.1.0.dev1/fiddler/
--rw-r--r--   0 runner    (1001) runner    (1001)       11 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/VERSION
--rw-r--r--   0 runner    (1001) runner    (1001)     3757 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/__init__.py
--rw-r--r--   0 runner    (1001) runner    (1001)      217 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/configs.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5677 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/connection.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-09 16:33:41.713794 fiddler-client-3.1.0.dev1/fiddler/constants/
--rw-r--r--   0 runner    (1001) runner    (1001)        0 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/constants/__init__.py
--rw-r--r--   0 runner    (1001) runner    (1001)      512 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/constants/alert_rule.py
--rw-r--r--   0 runner    (1001) runner    (1001)      233 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/constants/baseline.py
--rw-r--r--   0 runner    (1001) runner    (1001)      400 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/constants/common.py
--rw-r--r--   0 runner    (1001) runner    (1001)      126 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/constants/dataset.py
--rw-r--r--   0 runner    (1001) runner    (1001)      114 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/constants/events.py
--rw-r--r--   0 runner    (1001) runner    (1001)      233 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/constants/job.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1706 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/constants/model.py
--rw-r--r--   0 runner    (1001) runner    (1001)      278 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/constants/model_deployment.py
--rw-r--r--   0 runner    (1001) runner    (1001)      214 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/constants/xai.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1820 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/decorators.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-09 16:33:41.713794 fiddler-client-3.1.0.dev1/fiddler/entities/
--rw-r--r--   0 runner    (1001) runner    (1001)        0 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/entities/__init__.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3564 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/entities/alert_record.py
--rw-r--r--   0 runner    (1001) runner    (1001)    11569 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/entities/alert_rule.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2106 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/entities/base.py
--rw-r--r--   0 runner    (1001) runner    (1001)     7907 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/entities/baseline.py
--rw-r--r--   0 runner    (1001) runner    (1001)     6568 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/entities/custom_expression.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4399 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/entities/dataset.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4291 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/entities/events.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4710 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/entities/file.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5220 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/entities/job.py
--rw-r--r--   0 runner    (1001) runner    (1001)    18503 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/entities/model.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5520 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/entities/model_artifact.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3769 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/entities/model_deployment.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1074 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/entities/organization.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4631 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/entities/project.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3077 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/entities/surrogate.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1243 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/entities/user.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3798 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/entities/webhook.py
--rw-r--r--   0 runner    (1001) runner    (1001)    20250 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/entities/xai.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2221 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/exceptions.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-09 16:33:41.713794 fiddler-client-3.1.0.dev1/fiddler/libs/
--rw-r--r--   0 runner    (1001) runner    (1001)        0 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/libs/__init__.py
--rw-r--r--   0 runner    (1001) runner    (1001)     6027 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/libs/http_client.py
--rw-r--r--   0 runner    (1001) runner    (1001)      512 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/libs/json_encoder.py
--rw-r--r--   0 runner    (1001) runner    (1001)    15995 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/libs/semver.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-09 16:33:41.713794 fiddler-client-3.1.0.dev1/fiddler/packtools/
--rw-r--r--   0 runner    (1001) runner    (1001)        0 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/packtools/__init__.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4637 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/packtools/gem.py
--rw-r--r--   0 runner    (1001) runner    (1001)     7941 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/packtools/keras_ig_helpers.py
--rw-r--r--   0 runner    (1001) runner    (1001)    15799 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/packtools/project_attributions_helpers.py
--rw-r--r--   0 runner    (1001) runner    (1001)    10467 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/packtools/template_model.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-09 16:33:41.733792 fiddler-client-3.1.0.dev1/fiddler/schemas/
--rw-r--r--   0 runner    (1001) runner    (1001)        0 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/schemas/__init__.py
--rw-r--r--   0 runner    (1001) runner    (1001)      668 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/schemas/alert_record.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1222 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/schemas/alert_rule.py
--rw-r--r--   0 runner    (1001) runner    (1001)      189 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/schemas/base.py
--rw-r--r--   0 runner    (1001) runner    (1001)      933 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/schemas/baseline.py
--rw-r--r--   0 runner    (1001) runner    (1001)      844 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/schemas/custom_expression.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5382 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/schemas/custom_features.py
--rw-r--r--   0 runner    (1001) runner    (1001)      657 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/schemas/dataset.py
--rw-r--r--   0 runner    (1001) runner    (1001)      409 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/schemas/events.py
--rw-r--r--   0 runner    (1001) runner    (1001)      462 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/schemas/file.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1325 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/schemas/filter_query.py
--rw-r--r--   0 runner    (1001) runner    (1001)      354 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/schemas/job.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1378 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/schemas/model.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1128 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/schemas/model_deployment.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1914 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/schemas/model_schema.py
--rw-r--r--   0 runner    (1001) runner    (1001)      642 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/schemas/model_spec.py
--rw-r--r--   0 runner    (1001) runner    (1001)      691 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/schemas/model_task_params.py
--rw-r--r--   0 runner    (1001) runner    (1001)      281 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/schemas/organization.py
--rw-r--r--   0 runner    (1001) runner    (1001)      379 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/schemas/project.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1166 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/schemas/response.py
--rw-r--r--   0 runner    (1001) runner    (1001)      500 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/schemas/server_info.py
--rw-r--r--   0 runner    (1001) runner    (1001)      137 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/schemas/user.py
--rw-r--r--   0 runner    (1001) runner    (1001)      464 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/schemas/webhook.py
--rw-r--r--   0 runner    (1001) runner    (1001)      739 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/schemas/xai.py
--rw-r--r--   0 runner    (1001) runner    (1001)      313 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/schemas/xai_params.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-09 16:33:41.733792 fiddler-client-3.1.0.dev1/fiddler/tests/
--rw-r--r--   0 runner    (1001) runner    (1001)        0 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-09 16:33:41.733792 fiddler-client-3.1.0.dev1/fiddler/tests/apis/
--rw-r--r--   0 runner    (1001) runner    (1001)        0 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/tests/apis/__init__.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3118 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/tests/apis/test_alert_record.py
--rw-r--r--   0 runner    (1001) runner    (1001)    11231 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/tests/apis/test_alert_rule.py
--rw-r--r--   0 runner    (1001) runner    (1001)     7494 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/tests/apis/test_baseline.py
--rw-r--r--   0 runner    (1001) runner    (1001)     8208 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/tests/apis/test_custom_metric.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4636 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/tests/apis/test_dataset.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5134 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/tests/apis/test_events.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4501 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/tests/apis/test_files.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5089 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/tests/apis/test_generate_model.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1891 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/tests/apis/test_job.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2453 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/tests/apis/test_mixin.py
--rw-r--r--   0 runner    (1001) runner    (1001)    18346 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/tests/apis/test_model.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5635 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/tests/apis/test_model_artifact.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2441 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/tests/apis/test_model_deployment.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4443 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/tests/apis/test_model_surrogate.py
--rw-r--r--   0 runner    (1001) runner    (1001)     6015 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/tests/apis/test_project.py
--rw-r--r--   0 runner    (1001) runner    (1001)     7804 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/tests/apis/test_segment.py
--rw-r--r--   0 runner    (1001) runner    (1001)     6440 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/tests/apis/test_webhook.py
--rw-r--r--   0 runner    (1001) runner    (1001)    28590 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/tests/apis/test_xai.py
--rw-r--r--   0 runner    (1001) runner    (1001)      840 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/tests/conftest.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1102 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/tests/constants.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1865 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/tests/test_connection.py
--rw-r--r--   0 runner    (1001) runner    (1001)      783 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/tests/test_json_encoder.py
--rw-r--r--   0 runner    (1001) runner    (1001)      312 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/tests/test_logger.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3333 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/tests/test_utils.py
--rw-r--r--   0 runner    (1001) runner    (1001)      335 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/tests/utils.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-09 16:33:41.733792 fiddler-client-3.1.0.dev1/fiddler/utils/
--rw-r--r--   0 runner    (1001) runner    (1001)       53 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/utils/__init__.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2908 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/utils/helpers.py
--rw-r--r--   0 runner    (1001) runner    (1001)      669 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/utils/logger.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2203 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/utils/model_generator.py
--rw-r--r--   0 runner    (1001) runner    (1001)      408 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/utils/validations.py
--rw-r--r--   0 runner    (1001) runner    (1001)      531 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/utils/version.py
--rw-r--r--   0 runner    (1001) runner    (1001)      140 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/version.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-09 16:33:41.733792 fiddler-client-3.1.0.dev1/fiddler_client.egg-info/
--rw-r--r--   0 runner    (1001) runner    (1001)    20672 2024-04-09 16:33:41.000000 fiddler-client-3.1.0.dev1/fiddler_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) runner    (1001)     3321 2024-04-09 16:33:41.000000 fiddler-client-3.1.0.dev1/fiddler_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) runner    (1001)        1 2024-04-09 16:33:41.000000 fiddler-client-3.1.0.dev1/fiddler_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) runner    (1001)      137 2024-04-09 16:33:41.000000 fiddler-client-3.1.0.dev1/fiddler_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) runner    (1001)        8 2024-04-09 16:33:41.000000 fiddler-client-3.1.0.dev1/fiddler_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) runner    (1001)       38 2024-04-09 16:33:41.733792 fiddler-client-3.1.0.dev1/setup.cfg
--rw-r--r--   0 runner    (1001) runner    (1001)     1102 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/setup.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-19 12:21:13.158824 fiddler-client-3.1.0.dev2/
+-rw-r--r--   0 runner    (1001) runner    (1001)      559 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) runner    (1001)       42 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) runner    (1001)     1549 2024-04-19 12:21:13.158824 fiddler-client-3.1.0.dev2/PKG-INFO
+-rw-r--r--   0 runner    (1001) runner    (1001)      855 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/PUBLIC.md
+-rw-r--r--   0 runner    (1001) runner    (1001)     2165 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/README.md
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-19 12:21:13.138823 fiddler-client-3.1.0.dev2/fiddler/
+-rw-r--r--   0 runner    (1001) runner    (1001)       11 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/VERSION
+-rw-r--r--   0 runner    (1001) runner    (1001)     3757 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/__init__.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      217 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/configs.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5677 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/connection.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-19 12:21:13.138823 fiddler-client-3.1.0.dev2/fiddler/constants/
+-rw-r--r--   0 runner    (1001) runner    (1001)        0 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/constants/__init__.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      512 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/constants/alert_rule.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      233 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/constants/baseline.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      400 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/constants/common.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      126 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/constants/dataset.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      114 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/constants/events.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      233 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/constants/job.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1706 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/constants/model.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      278 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/constants/model_deployment.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      214 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/constants/xai.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1820 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/decorators.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-19 12:21:13.148823 fiddler-client-3.1.0.dev2/fiddler/entities/
+-rw-r--r--   0 runner    (1001) runner    (1001)        0 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/entities/__init__.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3564 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/entities/alert_record.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    11569 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/entities/alert_rule.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2106 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/entities/base.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     7907 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/entities/baseline.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     6568 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/entities/custom_expression.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4399 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/entities/dataset.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4291 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/entities/events.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4710 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/entities/file.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5220 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/entities/job.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    18613 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/entities/model.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5520 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/entities/model_artifact.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3769 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/entities/model_deployment.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1074 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/entities/organization.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4631 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/entities/project.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3077 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/entities/surrogate.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1243 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/entities/user.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3798 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/entities/webhook.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    20250 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/entities/xai.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2221 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/exceptions.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-19 12:21:13.148823 fiddler-client-3.1.0.dev2/fiddler/libs/
+-rw-r--r--   0 runner    (1001) runner    (1001)        0 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/libs/__init__.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     6027 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/libs/http_client.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      512 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/libs/json_encoder.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    15995 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/libs/semver.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-19 12:21:13.148823 fiddler-client-3.1.0.dev2/fiddler/packtools/
+-rw-r--r--   0 runner    (1001) runner    (1001)        0 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/packtools/__init__.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4637 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/packtools/gem.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     7941 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/packtools/keras_ig_helpers.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    15799 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/packtools/project_attributions_helpers.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    10467 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/packtools/template_model.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-19 12:21:13.148823 fiddler-client-3.1.0.dev2/fiddler/schemas/
+-rw-r--r--   0 runner    (1001) runner    (1001)        0 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      668 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/schemas/alert_record.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1222 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/schemas/alert_rule.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      189 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/schemas/base.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      933 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/schemas/baseline.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      844 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/schemas/custom_expression.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5531 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/schemas/custom_features.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      657 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/schemas/dataset.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      409 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/schemas/events.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      462 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/schemas/file.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1325 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/schemas/filter_query.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      354 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/schemas/job.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1405 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/schemas/model.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1128 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/schemas/model_deployment.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1914 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/schemas/model_schema.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      941 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/schemas/model_spec.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      691 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/schemas/model_task_params.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      281 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/schemas/organization.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      379 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/schemas/project.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1166 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/schemas/response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      500 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/schemas/server_info.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      137 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/schemas/user.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      464 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/schemas/webhook.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      739 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/schemas/xai.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      313 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/schemas/xai_params.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-19 12:21:13.148823 fiddler-client-3.1.0.dev2/fiddler/tests/
+-rw-r--r--   0 runner    (1001) runner    (1001)        0 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-19 12:21:13.158824 fiddler-client-3.1.0.dev2/fiddler/tests/apis/
+-rw-r--r--   0 runner    (1001) runner    (1001)        0 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/tests/apis/__init__.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3118 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/tests/apis/test_alert_record.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    11231 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/tests/apis/test_alert_rule.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     7494 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/tests/apis/test_baseline.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     8208 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/tests/apis/test_custom_metric.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4636 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/tests/apis/test_dataset.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5134 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/tests/apis/test_events.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4501 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/tests/apis/test_files.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5089 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/tests/apis/test_generate_model.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1891 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/tests/apis/test_job.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2517 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/tests/apis/test_mixin.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    18346 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/tests/apis/test_model.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5635 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/tests/apis/test_model_artifact.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2441 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/tests/apis/test_model_deployment.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4443 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/tests/apis/test_model_surrogate.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     6015 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/tests/apis/test_project.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     7804 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/tests/apis/test_segment.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     6440 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/tests/apis/test_webhook.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    28590 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/tests/apis/test_xai.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      840 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/tests/conftest.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1102 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/tests/constants.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1865 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/tests/test_connection.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      783 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/tests/test_json_encoder.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      312 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/tests/test_logger.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3333 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      335 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/tests/utils.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-19 12:21:13.158824 fiddler-client-3.1.0.dev2/fiddler/utils/
+-rw-r--r--   0 runner    (1001) runner    (1001)       53 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/utils/__init__.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2908 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/utils/helpers.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      669 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/utils/logger.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2203 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/utils/model_generator.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      408 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/utils/validations.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      531 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/utils/version.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      140 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/fiddler/version.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-19 12:21:13.158824 fiddler-client-3.1.0.dev2/fiddler_client.egg-info/
+-rw-r--r--   0 runner    (1001) runner    (1001)     1549 2024-04-19 12:21:13.000000 fiddler-client-3.1.0.dev2/fiddler_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) runner    (1001)     3321 2024-04-19 12:21:13.000000 fiddler-client-3.1.0.dev2/fiddler_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) runner    (1001)        1 2024-04-19 12:21:13.000000 fiddler-client-3.1.0.dev2/fiddler_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) runner    (1001)      137 2024-04-19 12:21:13.000000 fiddler-client-3.1.0.dev2/fiddler_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) runner    (1001)        8 2024-04-19 12:21:13.000000 fiddler-client-3.1.0.dev2/fiddler_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) runner    (1001)       38 2024-04-19 12:21:13.158824 fiddler-client-3.1.0.dev2/setup.cfg
+-rw-r--r--   0 runner    (1001) runner    (1001)     1102 2024-04-19 12:21:07.000000 fiddler-client-3.1.0.dev2/setup.py
```

### Comparing `fiddler-client-3.1.0.dev1/LICENSE.txt` & `fiddler-client-3.1.0.dev2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev1/README.md` & `fiddler-client-3.1.0.dev2/README.md`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev1/fiddler/__init__.py` & `fiddler-client-3.1.0.dev2/fiddler/__init__.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev1/fiddler/connection.py` & `fiddler-client-3.1.0.dev2/fiddler/connection.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev1/fiddler/constants/alert_rule.py` & `fiddler-client-3.1.0.dev2/fiddler/constants/alert_rule.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev1/fiddler/constants/model.py` & `fiddler-client-3.1.0.dev2/fiddler/constants/model.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev1/fiddler/decorators.py` & `fiddler-client-3.1.0.dev2/fiddler/decorators.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev1/fiddler/entities/alert_record.py` & `fiddler-client-3.1.0.dev2/fiddler/entities/alert_record.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev1/fiddler/entities/alert_rule.py` & `fiddler-client-3.1.0.dev2/fiddler/entities/alert_rule.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev1/fiddler/entities/base.py` & `fiddler-client-3.1.0.dev2/fiddler/entities/base.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev1/fiddler/entities/baseline.py` & `fiddler-client-3.1.0.dev2/fiddler/entities/baseline.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev1/fiddler/entities/custom_expression.py` & `fiddler-client-3.1.0.dev2/fiddler/entities/custom_expression.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev1/fiddler/entities/dataset.py` & `fiddler-client-3.1.0.dev2/fiddler/entities/dataset.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev1/fiddler/entities/events.py` & `fiddler-client-3.1.0.dev2/fiddler/entities/events.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev1/fiddler/entities/file.py` & `fiddler-client-3.1.0.dev2/fiddler/entities/file.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev1/fiddler/entities/job.py` & `fiddler-client-3.1.0.dev2/fiddler/entities/job.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev1/fiddler/entities/model.py` & `fiddler-client-3.1.0.dev2/fiddler/entities/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -544,14 +544,15 @@
         return job
 
 
 @dataclass
 class ModelCompact:
     id: UUID
     name: str
+    version: str | None = None
 
     def fetch(self) -> Model:
         """Fetch model instance"""
         return Model.get(id_=self.id)
 
 
 class ModelCompactMixin:
@@ -561,8 +562,12 @@
         response = getattr(self, '_resp', None)
         if not response or not hasattr(response, 'model'):
             raise AttributeError(
                 'This property is available only for objects generated from API '
                 'response.'
             )
 
-        return ModelCompact(id=response.model.id, name=response.model.name)
+        return ModelCompact(
+            id=response.model.id,
+            name=response.model.name,
+            version=response.model.version,
+        )
```

### Comparing `fiddler-client-3.1.0.dev1/fiddler/entities/model_artifact.py` & `fiddler-client-3.1.0.dev2/fiddler/entities/model_artifact.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev1/fiddler/entities/model_deployment.py` & `fiddler-client-3.1.0.dev2/fiddler/entities/model_deployment.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev1/fiddler/entities/organization.py` & `fiddler-client-3.1.0.dev2/fiddler/entities/organization.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev1/fiddler/entities/project.py` & `fiddler-client-3.1.0.dev2/fiddler/entities/project.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev1/fiddler/entities/surrogate.py` & `fiddler-client-3.1.0.dev2/fiddler/entities/surrogate.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev1/fiddler/entities/user.py` & `fiddler-client-3.1.0.dev2/fiddler/entities/user.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev1/fiddler/entities/webhook.py` & `fiddler-client-3.1.0.dev2/fiddler/entities/webhook.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev1/fiddler/entities/xai.py` & `fiddler-client-3.1.0.dev2/fiddler/entities/xai.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev1/fiddler/exceptions.py` & `fiddler-client-3.1.0.dev2/fiddler/exceptions.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev1/fiddler/libs/http_client.py` & `fiddler-client-3.1.0.dev2/fiddler/libs/http_client.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev1/fiddler/libs/json_encoder.py` & `fiddler-client-3.1.0.dev2/fiddler/libs/json_encoder.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev1/fiddler/libs/semver.py` & `fiddler-client-3.1.0.dev2/fiddler/libs/semver.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev1/fiddler/packtools/gem.py` & `fiddler-client-3.1.0.dev2/fiddler/packtools/gem.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev1/fiddler/packtools/keras_ig_helpers.py` & `fiddler-client-3.1.0.dev2/fiddler/packtools/keras_ig_helpers.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev1/fiddler/packtools/project_attributions_helpers.py` & `fiddler-client-3.1.0.dev2/fiddler/packtools/project_attributions_helpers.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev1/fiddler/packtools/template_model.py` & `fiddler-client-3.1.0.dev2/fiddler/packtools/template_model.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev1/fiddler/schemas/alert_record.py` & `fiddler-client-3.1.0.dev2/fiddler/schemas/alert_record.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev1/fiddler/schemas/alert_rule.py` & `fiddler-client-3.1.0.dev2/fiddler/schemas/alert_rule.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev1/fiddler/schemas/baseline.py` & `fiddler-client-3.1.0.dev2/fiddler/schemas/baseline.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev1/fiddler/schemas/custom_expression.py` & `fiddler-client-3.1.0.dev2/fiddler/schemas/custom_expression.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev1/fiddler/schemas/custom_features.py` & `fiddler-client-3.1.0.dev2/fiddler/schemas/custom_features.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,31 +1,25 @@
-from typing import Any, Dict, List, Optional, Type, TypeVar
+from typing import Any, Dict, List, Optional, Type, TypeVar, Literal
 
 from pydantic import BaseModel, validator
 
 from fiddler.configs import DEFAULT_NUM_CLUSTERS, DEFAULT_NUM_TAGS
 from fiddler.constants.model import CustomFeatureType
 
 CustomFeatureTypeVar = TypeVar('CustomFeatureTypeVar', bound='CustomFeature')
 
 
 class CustomFeature(BaseModel):
     name: str
-    type: CustomFeatureType
-    n_clusters: Optional[int] = DEFAULT_NUM_CLUSTERS
-    centroids: Optional[List] = None
-
-    @validator('n_clusters')
-    def validate_n_clusters(cls, value: int) -> int:  # noqa: N805
-        if value < 0:
-            raise ValueError('n_clusters must be greater than 0')
-        return value
+    type: Any
 
     class Config:
         allow_mutation = False
+        use_enum_values = True
+        discriminator = 'type'
 
     @classmethod
     def from_columns(
         cls, custom_name: str, cols: List[str], n_clusters: int = DEFAULT_NUM_CLUSTERS
     ) -> 'Multivariate':
         return Multivariate(
             name=custom_name,
@@ -49,20 +43,21 @@
 
         raise ValueError(f'Unsupported feature type: {feature_type}')
 
     def to_dict(self) -> Dict[str, Any]:
         return_dict: Dict[str, Any] = {
             'name': self.name,
             'type': self.type.value,
-            'n_clusters': self.n_clusters,
         }
         if isinstance(self, Multivariate):
             return_dict['columns'] = self.columns
+            return_dict['n_clusters'] = self.n_clusters
         elif isinstance(self, VectorFeature):
             return_dict['column'] = self.column
+            return_dict['n_clusters'] = self.n_clusters
             if isinstance(self, (ImageEmbedding, TextEmbedding)):
                 return_dict['source_column'] = self.source_column
                 if isinstance(self, TextEmbedding):
                     return_dict['n_tags'] = self.n_tags
         elif isinstance(self, Enrichment):
             return_dict['columns'] = self.columns
             return_dict['enrichment'] = self.enrichment
@@ -70,56 +65,62 @@
         else:
             raise ValueError(f'Unsupported feature type: {self.type} {type(self)}')
 
         return return_dict
 
 
 class Multivariate(CustomFeature):
-    type: CustomFeatureType = CustomFeatureType.FROM_COLUMNS
+    type: Literal['FROM_COLUMNS'] = CustomFeatureType.FROM_COLUMNS.value
+    n_clusters: Optional[int] = DEFAULT_NUM_CLUSTERS
+    centroids: Optional[List] = None
     columns: List[str]
     monitor_components: bool = False
 
     @validator('columns')
     def validate_columns(cls, value: List[str]) -> List[str]:  # noqa: N805
         if len(value) < 2:
             raise ValueError('Multivariate columns must be greater than 1')
         return value
 
+    @validator('n_clusters')
+    def validate_n_clusters(cls, value: int) -> int:  # noqa: N805
+        if value < 0:
+            raise ValueError('n_clusters must be greater than 0')
+        return value
+
 
 class VectorFeature(CustomFeature):
-    type: CustomFeatureType = CustomFeatureType.FROM_VECTOR
-    source_column: Optional[str] = None
+    type: Literal['FROM_VECTOR'] = CustomFeatureType.FROM_VECTOR.value
+    n_clusters: Optional[int] = DEFAULT_NUM_CLUSTERS
+    centroids: Optional[List] = None
     column: str
 
+    @validator('n_clusters')
+    def validate_n_clusters(cls, value: int) -> int:  # noqa: N805
+        if value < 0:
+            raise ValueError('n_clusters must be greater than 0')
+        return value
+
 
 class TextEmbedding(VectorFeature):
-    type: CustomFeatureType = CustomFeatureType.FROM_TEXT_EMBEDDING
+    type: Literal['FROM_TEXT_EMBEDDING'] = CustomFeatureType.FROM_TEXT_EMBEDDING.value  # type: ignore
+    source_column: str
     n_tags: Optional[int] = DEFAULT_NUM_TAGS
-
-    @validator('source_column')
-    def validate_source_column(cls, value: str) -> str:  # noqa: N805
-        if value is None:
-            raise ValueError('source_column must be specified')
-        return value
+    tf_idf: Optional[Dict[str, List]] = None
 
     @validator('n_tags')
     def validate_n_tags(cls, value: int) -> int:  # noqa: N805
         if value < 0:
             raise ValueError('n_tags must be greater than 0')
         return value
 
 
 class ImageEmbedding(VectorFeature):
-    type: CustomFeatureType = CustomFeatureType.FROM_IMAGE_EMBEDDING
-
-    @validator('source_column')
-    def validate_source_column(cls, value: str) -> str:  # noqa: N805
-        if value is None:
-            raise ValueError('source_column must be specified')
-        return value
+    type: Literal['FROM_IMAGE_EMBEDDING'] = CustomFeatureType.FROM_IMAGE_EMBEDDING.value  # type: ignore
+    source_column: str
 
 
 class Enrichment(CustomFeature):
     """
     Represents an enrichment feature in a data processing or machine learning context.
 
     This class inherits from CustomFeature and is used to apply specific enrichment
@@ -130,15 +131,15 @@
         type (CustomFeatureType): The type of the custom feature, set to ENRICHMENT.
         columns (List[str]): The list of input column names in the dataset used to generate the enrichment.
         enrichment (str): A string identifier for the type of enrichment to be applied.
         config (Dict[str, Any]): A dictionary containing configuration options for the enrichment.
     """
 
     # Setting the feature type to ENRICHMENT
-    type: CustomFeatureType = CustomFeatureType.ENRICHMENT
+    type: Literal['ENRICHMENT'] = CustomFeatureType.ENRICHMENT.value
 
     # List of input column names used to generate the enrichment
     columns: List[str]
 
     # String identifier for the enrichment to be applied. e.g. "embedding" or "toxicity"
     enrichment: str
```

### Comparing `fiddler-client-3.1.0.dev1/fiddler/schemas/dataset.py` & `fiddler-client-3.1.0.dev2/fiddler/schemas/dataset.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev1/fiddler/schemas/filter_query.py` & `fiddler-client-3.1.0.dev2/fiddler/schemas/filter_query.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev1/fiddler/schemas/model.py` & `fiddler-client-3.1.0.dev2/fiddler/schemas/model.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from fiddler.schemas.user import UserCompactResp
 from fiddler.schemas.xai_params import XaiParams
 
 
 class ModelCompactResp(BaseModel):
     id: UUID
     name: str
+    version: Optional[str]
 
 
 class ModelResp(BaseModel):
     id: UUID
     name: str
     version: str
     input_type: str
```

### Comparing `fiddler-client-3.1.0.dev1/fiddler/schemas/model_deployment.py` & `fiddler-client-3.1.0.dev2/fiddler/schemas/model_deployment.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev1/fiddler/schemas/model_schema.py` & `fiddler-client-3.1.0.dev2/fiddler/schemas/model_schema.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev1/fiddler/schemas/model_task_params.py` & `fiddler-client-3.1.0.dev2/fiddler/schemas/model_task_params.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev1/fiddler/schemas/response.py` & `fiddler-client-3.1.0.dev2/fiddler/schemas/response.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev1/fiddler/schemas/xai.py` & `fiddler-client-3.1.0.dev2/fiddler/schemas/xai.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev1/fiddler/tests/apis/test_alert_record.py` & `fiddler-client-3.1.0.dev2/fiddler/tests/apis/test_alert_record.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev1/fiddler/tests/apis/test_alert_rule.py` & `fiddler-client-3.1.0.dev2/fiddler/tests/apis/test_alert_rule.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev1/fiddler/tests/apis/test_baseline.py` & `fiddler-client-3.1.0.dev2/fiddler/tests/apis/test_baseline.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev1/fiddler/tests/apis/test_custom_metric.py` & `fiddler-client-3.1.0.dev2/fiddler/tests/apis/test_custom_metric.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev1/fiddler/tests/apis/test_dataset.py` & `fiddler-client-3.1.0.dev2/fiddler/tests/apis/test_dataset.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev1/fiddler/tests/apis/test_events.py` & `fiddler-client-3.1.0.dev2/fiddler/tests/apis/test_events.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev1/fiddler/tests/apis/test_files.py` & `fiddler-client-3.1.0.dev2/fiddler/tests/apis/test_files.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev1/fiddler/tests/apis/test_generate_model.py` & `fiddler-client-3.1.0.dev2/fiddler/tests/apis/test_generate_model.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev1/fiddler/tests/apis/test_job.py` & `fiddler-client-3.1.0.dev2/fiddler/tests/apis/test_job.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev1/fiddler/tests/apis/test_mixin.py` & `fiddler-client-3.1.0.dev2/fiddler/tests/apis/test_mixin.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 from fiddler.tests.constants import (
     BASELINE_ID,
     BASELINE_NAME,
     DATASET_ID,
     DATASET_NAME,
     MODEL_ID,
     MODEL_NAME,
+    MODEL_VERSION,
     PROJECT_ID,
     PROJECT_NAME,
     USER_EMAIL,
     USER_ID,
     USER_NAME,
 )
 
@@ -35,15 +36,17 @@
     BaselineCompactMixin,
     CreatedByMixin,
     UpdatedByMixin,
 ):
     def __init__(self) -> None:
         self._resp = mock.MagicMock()
         self._resp.project = ProjectCompactResp(id=PROJECT_ID, name=PROJECT_NAME)
-        self._resp.model = ModelCompactResp(id=MODEL_ID, name=MODEL_NAME)
+        self._resp.model = ModelCompactResp(
+            id=MODEL_ID, name=MODEL_NAME, version=MODEL_VERSION
+        )
         self._resp.dataset = DatasetCompactResp(
             id=DATASET_ID, name=DATASET_NAME, type=EnvType.PRE_PRODUCTION
         )
         self._resp.baseline = BaselineCompactResp(id=BASELINE_ID, name=BASELINE_NAME)
         self._resp.created_by = UserCompactResp(
             id=USER_ID, full_name=USER_NAME, email=USER_EMAIL
         )
```

### Comparing `fiddler-client-3.1.0.dev1/fiddler/tests/apis/test_model.py` & `fiddler-client-3.1.0.dev2/fiddler/tests/apis/test_model.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev1/fiddler/tests/apis/test_model_artifact.py` & `fiddler-client-3.1.0.dev2/fiddler/tests/apis/test_model_artifact.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev1/fiddler/tests/apis/test_model_deployment.py` & `fiddler-client-3.1.0.dev2/fiddler/tests/apis/test_model_deployment.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev1/fiddler/tests/apis/test_model_surrogate.py` & `fiddler-client-3.1.0.dev2/fiddler/tests/apis/test_model_surrogate.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev1/fiddler/tests/apis/test_project.py` & `fiddler-client-3.1.0.dev2/fiddler/tests/apis/test_project.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev1/fiddler/tests/apis/test_segment.py` & `fiddler-client-3.1.0.dev2/fiddler/tests/apis/test_segment.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev1/fiddler/tests/apis/test_webhook.py` & `fiddler-client-3.1.0.dev2/fiddler/tests/apis/test_webhook.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev1/fiddler/tests/apis/test_xai.py` & `fiddler-client-3.1.0.dev2/fiddler/tests/apis/test_xai.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev1/fiddler/tests/conftest.py` & `fiddler-client-3.1.0.dev2/fiddler/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev1/fiddler/tests/constants.py` & `fiddler-client-3.1.0.dev2/fiddler/tests/constants.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev1/fiddler/tests/test_connection.py` & `fiddler-client-3.1.0.dev2/fiddler/tests/test_connection.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev1/fiddler/tests/test_json_encoder.py` & `fiddler-client-3.1.0.dev2/fiddler/tests/test_json_encoder.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev1/fiddler/tests/test_utils.py` & `fiddler-client-3.1.0.dev2/fiddler/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev1/fiddler/utils/helpers.py` & `fiddler-client-3.1.0.dev2/fiddler/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev1/fiddler/utils/logger.py` & `fiddler-client-3.1.0.dev2/fiddler/utils/logger.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev1/fiddler/utils/model_generator.py` & `fiddler-client-3.1.0.dev2/fiddler/utils/model_generator.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev1/fiddler/utils/version.py` & `fiddler-client-3.1.0.dev2/fiddler/utils/version.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev1/fiddler_client.egg-info/SOURCES.txt` & `fiddler-client-3.1.0.dev2/fiddler_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev1/setup.py` & `fiddler-client-3.1.0.dev2/setup.py`

 * *Files identical despite different names*


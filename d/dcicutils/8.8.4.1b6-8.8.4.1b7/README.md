# Comparing `tmp/dcicutils-8.8.4.1b6.tar.gz` & `tmp/dcicutils-8.8.4.1b7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcicutils-8.8.4.1b6.tar", max compression
+gzip compressed data, was "dcicutils-8.8.4.1b7.tar", max compression
```

## Comparing `dcicutils-8.8.4.1b6.tar` & `dcicutils-8.8.4.1b7.tar`

### file list

```diff
@@ -1,79 +1,79 @@
--rw-r--r--   0        0        0     1102 2024-04-24 23:02:33.576722 dcicutils-8.8.4.1b6/LICENSE.txt
--rw-r--r--   0        0        0     1166 2024-04-24 23:02:33.576722 dcicutils-8.8.4.1b6/README.rst
--rw-r--r--   0        0        0        0 2024-04-24 23:02:33.576722 dcicutils-8.8.4.1b6/dcicutils/__init__.py
--rw-r--r--   0        0        0     5115 2024-04-24 23:02:33.576722 dcicutils-8.8.4.1b6/dcicutils/base.py
--rwxr-xr-x   0        0        0    51434 2024-04-24 23:02:33.576722 dcicutils-8.8.4.1b6/dcicutils/beanstalk_utils.py
--rw-r--r--   0        0        0    34669 2024-04-24 23:02:33.576722 dcicutils-8.8.4.1b6/dcicutils/bundle_utils.py
--rw-r--r--   0        0        0     3295 2024-04-24 23:02:33.576722 dcicutils-8.8.4.1b6/dcicutils/captured_output.py
--rw-r--r--   0        0        0    13786 2024-04-24 23:02:33.576722 dcicutils-8.8.4.1b6/dcicutils/cloudformation_utils.py
--rw-r--r--   0        0        0     1155 2024-04-24 23:02:33.576722 dcicutils-8.8.4.1b6/dcicutils/codebuild_utils.py
--rw-r--r--   0        0        0    15285 2024-04-24 23:02:33.576722 dcicutils-8.8.4.1b6/dcicutils/command_utils.py
--rw-r--r--   0        0        0     3955 2024-04-24 23:02:33.576722 dcicutils-8.8.4.1b6/dcicutils/common.py
--rw-r--r--   0        0        0     2015 2024-04-24 23:02:33.576722 dcicutils-8.8.4.1b6/dcicutils/contribution_scripts.py
--rw-r--r--   0        0        0    25653 2024-04-24 23:02:33.576722 dcicutils-8.8.4.1b6/dcicutils/contribution_utils.py
--rw-r--r--   0        0        0    11113 2024-04-24 23:02:33.576722 dcicutils-8.8.4.1b6/dcicutils/creds_utils.py
--rw-r--r--   0        0        0     7626 2024-04-24 23:02:33.576722 dcicutils-8.8.4.1b6/dcicutils/data_readers.py
--rw-r--r--   0        0        0     3098 2024-04-24 23:02:33.576722 dcicutils-8.8.4.1b6/dcicutils/data_utils.py
--rw-r--r--   0        0        0    13499 2024-04-24 23:02:33.576722 dcicutils-8.8.4.1b6/dcicutils/datetime_utils.py
--rw-r--r--   0        0        0    69908 2024-04-24 23:02:33.576722 dcicutils-8.8.4.1b6/dcicutils/deployment_utils.py
--rw-r--r--   0        0        0     8118 2024-04-24 23:02:33.576722 dcicutils-8.8.4.1b6/dcicutils/diff_utils.py
--rw-r--r--   0        0        0     1747 2024-04-24 23:02:33.576722 dcicutils-8.8.4.1b6/dcicutils/docker_utils.py
--rw-r--r--   0        0        0    19474 2024-04-24 23:02:33.576722 dcicutils-8.8.4.1b6/dcicutils/ecr_scripts.py
--rw-r--r--   0        0        0    13079 2024-04-24 23:02:33.576722 dcicutils-8.8.4.1b6/dcicutils/ecr_utils.py
--rw-r--r--   0        0        0     3590 2024-04-24 23:02:33.576722 dcicutils-8.8.4.1b6/dcicutils/ecs_utils.py
--rw-r--r--   0        0        0     6356 2024-04-24 23:02:33.576722 dcicutils-8.8.4.1b6/dcicutils/env_base.py
--rw-r--r--   0        0        0     9444 2024-04-24 23:02:33.576722 dcicutils-8.8.4.1b6/dcicutils/env_manager.py
--rw-r--r--   0        0        0     3909 2024-04-24 23:02:33.576722 dcicutils-8.8.4.1b6/dcicutils/env_scripts.py
--rw-r--r--   0        0        0    46970 2024-04-24 23:02:33.576722 dcicutils-8.8.4.1b6/dcicutils/env_utils.py
--rw-r--r--   0        0        0    29032 2024-04-24 23:02:33.576722 dcicutils-8.8.4.1b6/dcicutils/env_utils_legacy.py
--rw-r--r--   0        0        0     7541 2024-04-24 23:02:33.576722 dcicutils-8.8.4.1b6/dcicutils/es_utils.py
--rw-r--r--   0        0        0     9931 2024-04-24 23:02:33.576722 dcicutils-8.8.4.1b6/dcicutils/exceptions.py
--rw-r--r--   0        0        0    36918 2024-04-24 23:02:33.576722 dcicutils-8.8.4.1b6/dcicutils/ff_mocks.py
--rw-r--r--   0        0        0    73123 2024-04-24 23:02:33.576722 dcicutils-8.8.4.1b6/dcicutils/ff_utils.py
--rw-r--r--   0        0        0     3653 2024-04-24 23:02:33.576722 dcicutils-8.8.4.1b6/dcicutils/file_utils.py
--rw-r--r--   0        0        0    10026 2024-04-24 23:02:33.576722 dcicutils-8.8.4.1b6/dcicutils/function_cache_decorator.py
--rw-r--r--   0        0        0    34149 2024-04-24 23:02:33.576722 dcicutils-8.8.4.1b6/dcicutils/glacier_utils.py
--rw-r--r--   0        0        0      807 2024-04-24 23:02:33.576722 dcicutils-8.8.4.1b6/dcicutils/http_utils.py
--rw-r--r--   0        0        0    11502 2024-04-24 23:02:33.576722 dcicutils-8.8.4.1b6/dcicutils/jh_utils.py
--rw-r--r--   0        0        0    16225 2024-04-24 23:02:33.576722 dcicutils-8.8.4.1b6/dcicutils/kibana/dashboards.json
--rw-r--r--   0        0        0     2164 2024-04-24 23:02:33.576722 dcicutils-8.8.4.1b6/dcicutils/kibana/readme.md
--rw-r--r--   0        0        0    28151 2024-04-24 23:02:33.576722 dcicutils-8.8.4.1b6/dcicutils/lang_utils.py
--rw-r--r--   0        0        0      278 2024-04-24 23:02:33.576722 dcicutils-8.8.4.1b6/dcicutils/license_policies/c4-infrastructure.jsonc
--rw-r--r--   0        0        0      296 2024-04-24 23:02:33.576722 dcicutils-8.8.4.1b6/dcicutils/license_policies/c4-python-infrastructure.jsonc
--rw-r--r--   0        0        0     5790 2024-04-24 23:02:33.576722 dcicutils-8.8.4.1b6/dcicutils/license_policies/park-lab-common-server.jsonc
--rw-r--r--   0        0        0    18864 2024-04-24 23:02:33.576722 dcicutils-8.8.4.1b6/dcicutils/license_policies/park-lab-common.jsonc
--rw-r--r--   0        0        0     3260 2024-04-24 23:02:33.576722 dcicutils-8.8.4.1b6/dcicutils/license_policies/park-lab-gpl-pipeline.jsonc
--rw-r--r--   0        0        0      283 2024-04-24 23:02:33.576722 dcicutils-8.8.4.1b6/dcicutils/license_policies/park-lab-pipeline.jsonc
--rw-r--r--   0        0        0    46978 2024-04-24 23:02:33.576722 dcicutils-8.8.4.1b6/dcicutils/license_utils.py
--rw-r--r--   0        0        0    10883 2024-04-24 23:02:33.580722 dcicutils-8.8.4.1b6/dcicutils/log_utils.py
--rw-r--r--   0        0        0   105530 2024-04-24 23:02:33.580722 dcicutils-8.8.4.1b6/dcicutils/misc_utils.py
--rw-r--r--   0        0        0     5963 2024-04-24 23:02:33.580722 dcicutils-8.8.4.1b6/dcicutils/obfuscation_utils.py
--rw-r--r--   0        0        0     1017 2024-04-24 23:02:33.580722 dcicutils-8.8.4.1b6/dcicutils/opensearch_utils.py
--rw-r--r--   0        0        0    15422 2024-04-24 23:02:33.580722 dcicutils-8.8.4.1b6/dcicutils/portal_object_utils.py
--rw-r--r--   0        0        0    30779 2024-04-24 23:02:33.580722 dcicutils-8.8.4.1b6/dcicutils/portal_utils.py
--rw-r--r--   0        0        0    19468 2024-04-24 23:02:33.580722 dcicutils-8.8.4.1b6/dcicutils/progress_bar.py
--rw-r--r--   0        0        0    31250 2024-04-24 23:02:33.580722 dcicutils-8.8.4.1b6/dcicutils/project_utils.py
--rw-r--r--   0        0        0    20534 2024-04-24 23:02:33.580722 dcicutils-8.8.4.1b6/dcicutils/qa_checkers.py
--rw-r--r--   0        0        0   160208 2024-04-24 23:02:33.580722 dcicutils-8.8.4.1b6/dcicutils/qa_utils.py
--rw-r--r--   0        0        0     7055 2024-04-24 23:02:33.580722 dcicutils-8.8.4.1b6/dcicutils/redis_tools.py
--rw-r--r--   0        0        0     6462 2024-04-24 23:02:33.580722 dcicutils-8.8.4.1b6/dcicutils/redis_utils.py
--rw-r--r--   0        0        0    28868 2024-04-24 23:02:33.580722 dcicutils-8.8.4.1b6/dcicutils/s3_utils.py
--rw-r--r--   0        0        0    10095 2024-04-24 23:02:33.580722 dcicutils-8.8.4.1b6/dcicutils/schema_utils.py
--rw-r--r--   0        0        0    13889 2024-04-24 23:02:33.580722 dcicutils-8.8.4.1b6/dcicutils/scripts/publish_to_pypi.py
--rw-r--r--   0        0        0     4184 2024-04-24 23:02:33.580722 dcicutils-8.8.4.1b6/dcicutils/scripts/run_license_checker.py
--rw-r--r--   0        0        0    26262 2024-04-24 23:02:33.580722 dcicutils-8.8.4.1b6/dcicutils/scripts/view_portal_object.py
--rw-r--r--   0        0        0    19745 2024-04-24 23:02:33.580722 dcicutils-8.8.4.1b6/dcicutils/secrets_utils.py
--rw-r--r--   0        0        0    33629 2024-04-24 23:02:33.580722 dcicutils-8.8.4.1b6/dcicutils/sheet_utils.py
--rw-r--r--   0        0        0    22961 2024-04-24 23:02:33.580722 dcicutils-8.8.4.1b6/dcicutils/snapshot_utils.py
--rw-r--r--   0        0        0     9707 2024-04-24 23:02:33.580722 dcicutils-8.8.4.1b6/dcicutils/ssl_certificate_utils.py
--rw-r--r--   0        0        0    61238 2024-04-24 23:02:33.580722 dcicutils-8.8.4.1b6/dcicutils/structured_data.py
--rw-r--r--   0        0        0     2895 2024-04-24 23:02:33.580722 dcicutils-8.8.4.1b6/dcicutils/submitr/progress_constants.py
--rw-r--r--   0        0        0     3467 2024-04-24 23:02:33.580722 dcicutils-8.8.4.1b6/dcicutils/submitr/ref_lookup_strategy.py
--rw-r--r--   0        0        0     8082 2024-04-24 23:02:33.580722 dcicutils-8.8.4.1b6/dcicutils/task_utils.py
--rw-r--r--   0        0        0     2295 2024-04-24 23:02:33.580722 dcicutils-8.8.4.1b6/dcicutils/tmpfile_utils.py
--rw-r--r--   0        0        0     1769 2024-04-24 23:02:33.580722 dcicutils-8.8.4.1b6/dcicutils/trace_utils.py
--rw-r--r--   0        0        0    14797 2024-04-24 23:02:33.580722 dcicutils-8.8.4.1b6/dcicutils/validation_utils.py
--rw-r--r--   0        0        0     4343 2024-04-24 23:02:33.580722 dcicutils-8.8.4.1b6/dcicutils/variant_utils.py
--rw-r--r--   0        0        0     3265 2024-04-24 23:02:33.580722 dcicutils-8.8.4.1b6/dcicutils/zip_utils.py
--rw-r--r--   0        0        0     4733 2024-04-24 23:02:33.580722 dcicutils-8.8.4.1b6/pyproject.toml
--rw-r--r--   0        0        0     3396 1970-01-01 00:00:00.000000 dcicutils-8.8.4.1b6/PKG-INFO
+-rw-r--r--   0        0        0     1102 2024-04-24 23:15:47.708251 dcicutils-8.8.4.1b7/LICENSE.txt
+-rw-r--r--   0        0        0     1166 2024-04-24 23:15:47.708251 dcicutils-8.8.4.1b7/README.rst
+-rw-r--r--   0        0        0        0 2024-04-24 23:15:47.708251 dcicutils-8.8.4.1b7/dcicutils/__init__.py
+-rw-r--r--   0        0        0     5115 2024-04-24 23:15:47.708251 dcicutils-8.8.4.1b7/dcicutils/base.py
+-rwxr-xr-x   0        0        0    51434 2024-04-24 23:15:47.708251 dcicutils-8.8.4.1b7/dcicutils/beanstalk_utils.py
+-rw-r--r--   0        0        0    34669 2024-04-24 23:15:47.712251 dcicutils-8.8.4.1b7/dcicutils/bundle_utils.py
+-rw-r--r--   0        0        0     3295 2024-04-24 23:15:47.712251 dcicutils-8.8.4.1b7/dcicutils/captured_output.py
+-rw-r--r--   0        0        0    13786 2024-04-24 23:15:47.712251 dcicutils-8.8.4.1b7/dcicutils/cloudformation_utils.py
+-rw-r--r--   0        0        0     1155 2024-04-24 23:15:47.712251 dcicutils-8.8.4.1b7/dcicutils/codebuild_utils.py
+-rw-r--r--   0        0        0    15285 2024-04-24 23:15:47.712251 dcicutils-8.8.4.1b7/dcicutils/command_utils.py
+-rw-r--r--   0        0        0     3955 2024-04-24 23:15:47.712251 dcicutils-8.8.4.1b7/dcicutils/common.py
+-rw-r--r--   0        0        0     2015 2024-04-24 23:15:47.712251 dcicutils-8.8.4.1b7/dcicutils/contribution_scripts.py
+-rw-r--r--   0        0        0    25653 2024-04-24 23:15:47.712251 dcicutils-8.8.4.1b7/dcicutils/contribution_utils.py
+-rw-r--r--   0        0        0    11113 2024-04-24 23:15:47.712251 dcicutils-8.8.4.1b7/dcicutils/creds_utils.py
+-rw-r--r--   0        0        0     7626 2024-04-24 23:15:47.712251 dcicutils-8.8.4.1b7/dcicutils/data_readers.py
+-rw-r--r--   0        0        0     3098 2024-04-24 23:15:47.712251 dcicutils-8.8.4.1b7/dcicutils/data_utils.py
+-rw-r--r--   0        0        0    13499 2024-04-24 23:15:47.712251 dcicutils-8.8.4.1b7/dcicutils/datetime_utils.py
+-rw-r--r--   0        0        0    69908 2024-04-24 23:15:47.712251 dcicutils-8.8.4.1b7/dcicutils/deployment_utils.py
+-rw-r--r--   0        0        0     8118 2024-04-24 23:15:47.712251 dcicutils-8.8.4.1b7/dcicutils/diff_utils.py
+-rw-r--r--   0        0        0     1747 2024-04-24 23:15:47.712251 dcicutils-8.8.4.1b7/dcicutils/docker_utils.py
+-rw-r--r--   0        0        0    19474 2024-04-24 23:15:47.712251 dcicutils-8.8.4.1b7/dcicutils/ecr_scripts.py
+-rw-r--r--   0        0        0    13079 2024-04-24 23:15:47.712251 dcicutils-8.8.4.1b7/dcicutils/ecr_utils.py
+-rw-r--r--   0        0        0     3590 2024-04-24 23:15:47.712251 dcicutils-8.8.4.1b7/dcicutils/ecs_utils.py
+-rw-r--r--   0        0        0     6356 2024-04-24 23:15:47.712251 dcicutils-8.8.4.1b7/dcicutils/env_base.py
+-rw-r--r--   0        0        0     9444 2024-04-24 23:15:47.712251 dcicutils-8.8.4.1b7/dcicutils/env_manager.py
+-rw-r--r--   0        0        0     3909 2024-04-24 23:15:47.712251 dcicutils-8.8.4.1b7/dcicutils/env_scripts.py
+-rw-r--r--   0        0        0    46970 2024-04-24 23:15:47.712251 dcicutils-8.8.4.1b7/dcicutils/env_utils.py
+-rw-r--r--   0        0        0    29032 2024-04-24 23:15:47.712251 dcicutils-8.8.4.1b7/dcicutils/env_utils_legacy.py
+-rw-r--r--   0        0        0     7541 2024-04-24 23:15:47.712251 dcicutils-8.8.4.1b7/dcicutils/es_utils.py
+-rw-r--r--   0        0        0     9931 2024-04-24 23:15:47.712251 dcicutils-8.8.4.1b7/dcicutils/exceptions.py
+-rw-r--r--   0        0        0    36918 2024-04-24 23:15:47.712251 dcicutils-8.8.4.1b7/dcicutils/ff_mocks.py
+-rw-r--r--   0        0        0    73123 2024-04-24 23:15:47.712251 dcicutils-8.8.4.1b7/dcicutils/ff_utils.py
+-rw-r--r--   0        0        0     3653 2024-04-24 23:15:47.712251 dcicutils-8.8.4.1b7/dcicutils/file_utils.py
+-rw-r--r--   0        0        0    10026 2024-04-24 23:15:47.712251 dcicutils-8.8.4.1b7/dcicutils/function_cache_decorator.py
+-rw-r--r--   0        0        0    34149 2024-04-24 23:15:47.712251 dcicutils-8.8.4.1b7/dcicutils/glacier_utils.py
+-rw-r--r--   0        0        0      807 2024-04-24 23:15:47.712251 dcicutils-8.8.4.1b7/dcicutils/http_utils.py
+-rw-r--r--   0        0        0    11502 2024-04-24 23:15:47.712251 dcicutils-8.8.4.1b7/dcicutils/jh_utils.py
+-rw-r--r--   0        0        0    16225 2024-04-24 23:15:47.712251 dcicutils-8.8.4.1b7/dcicutils/kibana/dashboards.json
+-rw-r--r--   0        0        0     2164 2024-04-24 23:15:47.712251 dcicutils-8.8.4.1b7/dcicutils/kibana/readme.md
+-rw-r--r--   0        0        0    28151 2024-04-24 23:15:47.712251 dcicutils-8.8.4.1b7/dcicutils/lang_utils.py
+-rw-r--r--   0        0        0      278 2024-04-24 23:15:47.712251 dcicutils-8.8.4.1b7/dcicutils/license_policies/c4-infrastructure.jsonc
+-rw-r--r--   0        0        0      296 2024-04-24 23:15:47.712251 dcicutils-8.8.4.1b7/dcicutils/license_policies/c4-python-infrastructure.jsonc
+-rw-r--r--   0        0        0     5790 2024-04-24 23:15:47.712251 dcicutils-8.8.4.1b7/dcicutils/license_policies/park-lab-common-server.jsonc
+-rw-r--r--   0        0        0    18864 2024-04-24 23:15:47.712251 dcicutils-8.8.4.1b7/dcicutils/license_policies/park-lab-common.jsonc
+-rw-r--r--   0        0        0     3260 2024-04-24 23:15:47.712251 dcicutils-8.8.4.1b7/dcicutils/license_policies/park-lab-gpl-pipeline.jsonc
+-rw-r--r--   0        0        0      283 2024-04-24 23:15:47.712251 dcicutils-8.8.4.1b7/dcicutils/license_policies/park-lab-pipeline.jsonc
+-rw-r--r--   0        0        0    46978 2024-04-24 23:15:47.712251 dcicutils-8.8.4.1b7/dcicutils/license_utils.py
+-rw-r--r--   0        0        0    10883 2024-04-24 23:15:47.712251 dcicutils-8.8.4.1b7/dcicutils/log_utils.py
+-rw-r--r--   0        0        0   105530 2024-04-24 23:15:47.712251 dcicutils-8.8.4.1b7/dcicutils/misc_utils.py
+-rw-r--r--   0        0        0     5963 2024-04-24 23:15:47.712251 dcicutils-8.8.4.1b7/dcicutils/obfuscation_utils.py
+-rw-r--r--   0        0        0     1017 2024-04-24 23:15:47.712251 dcicutils-8.8.4.1b7/dcicutils/opensearch_utils.py
+-rw-r--r--   0        0        0    15422 2024-04-24 23:15:47.712251 dcicutils-8.8.4.1b7/dcicutils/portal_object_utils.py
+-rw-r--r--   0        0        0    30779 2024-04-24 23:15:47.712251 dcicutils-8.8.4.1b7/dcicutils/portal_utils.py
+-rw-r--r--   0        0        0    19468 2024-04-24 23:15:47.712251 dcicutils-8.8.4.1b7/dcicutils/progress_bar.py
+-rw-r--r--   0        0        0    31250 2024-04-24 23:15:47.716251 dcicutils-8.8.4.1b7/dcicutils/project_utils.py
+-rw-r--r--   0        0        0    20534 2024-04-24 23:15:47.716251 dcicutils-8.8.4.1b7/dcicutils/qa_checkers.py
+-rw-r--r--   0        0        0   160208 2024-04-24 23:15:47.716251 dcicutils-8.8.4.1b7/dcicutils/qa_utils.py
+-rw-r--r--   0        0        0     7055 2024-04-24 23:15:47.716251 dcicutils-8.8.4.1b7/dcicutils/redis_tools.py
+-rw-r--r--   0        0        0     6462 2024-04-24 23:15:47.716251 dcicutils-8.8.4.1b7/dcicutils/redis_utils.py
+-rw-r--r--   0        0        0    28868 2024-04-24 23:15:47.716251 dcicutils-8.8.4.1b7/dcicutils/s3_utils.py
+-rw-r--r--   0        0        0    10095 2024-04-24 23:15:47.716251 dcicutils-8.8.4.1b7/dcicutils/schema_utils.py
+-rw-r--r--   0        0        0    13889 2024-04-24 23:15:47.716251 dcicutils-8.8.4.1b7/dcicutils/scripts/publish_to_pypi.py
+-rw-r--r--   0        0        0     4184 2024-04-24 23:15:47.716251 dcicutils-8.8.4.1b7/dcicutils/scripts/run_license_checker.py
+-rw-r--r--   0        0        0    26262 2024-04-24 23:15:47.716251 dcicutils-8.8.4.1b7/dcicutils/scripts/view_portal_object.py
+-rw-r--r--   0        0        0    19745 2024-04-24 23:15:47.716251 dcicutils-8.8.4.1b7/dcicutils/secrets_utils.py
+-rw-r--r--   0        0        0    33629 2024-04-24 23:15:47.716251 dcicutils-8.8.4.1b7/dcicutils/sheet_utils.py
+-rw-r--r--   0        0        0    22961 2024-04-24 23:15:47.716251 dcicutils-8.8.4.1b7/dcicutils/snapshot_utils.py
+-rw-r--r--   0        0        0     9707 2024-04-24 23:15:47.716251 dcicutils-8.8.4.1b7/dcicutils/ssl_certificate_utils.py
+-rw-r--r--   0        0        0    61238 2024-04-24 23:15:47.716251 dcicutils-8.8.4.1b7/dcicutils/structured_data.py
+-rw-r--r--   0        0        0     2895 2024-04-24 23:15:47.716251 dcicutils-8.8.4.1b7/dcicutils/submitr/progress_constants.py
+-rw-r--r--   0        0        0     3467 2024-04-24 23:15:47.716251 dcicutils-8.8.4.1b7/dcicutils/submitr/ref_lookup_strategy.py
+-rw-r--r--   0        0        0     8082 2024-04-24 23:15:47.716251 dcicutils-8.8.4.1b7/dcicutils/task_utils.py
+-rw-r--r--   0        0        0     2340 2024-04-24 23:15:47.716251 dcicutils-8.8.4.1b7/dcicutils/tmpfile_utils.py
+-rw-r--r--   0        0        0     1769 2024-04-24 23:15:47.716251 dcicutils-8.8.4.1b7/dcicutils/trace_utils.py
+-rw-r--r--   0        0        0    14797 2024-04-24 23:15:47.716251 dcicutils-8.8.4.1b7/dcicutils/validation_utils.py
+-rw-r--r--   0        0        0     4343 2024-04-24 23:15:47.716251 dcicutils-8.8.4.1b7/dcicutils/variant_utils.py
+-rw-r--r--   0        0        0     3265 2024-04-24 23:15:47.716251 dcicutils-8.8.4.1b7/dcicutils/zip_utils.py
+-rw-r--r--   0        0        0     4733 2024-04-24 23:15:47.716251 dcicutils-8.8.4.1b7/pyproject.toml
+-rw-r--r--   0        0        0     3396 1970-01-01 00:00:00.000000 dcicutils-8.8.4.1b7/PKG-INFO
```

### Comparing `dcicutils-8.8.4.1b6/LICENSE.txt` & `dcicutils-8.8.4.1b7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b6/README.rst` & `dcicutils-8.8.4.1b7/README.rst`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b6/dcicutils/base.py` & `dcicutils-8.8.4.1b7/dcicutils/base.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b6/dcicutils/beanstalk_utils.py` & `dcicutils-8.8.4.1b7/dcicutils/beanstalk_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b6/dcicutils/bundle_utils.py` & `dcicutils-8.8.4.1b7/dcicutils/bundle_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b6/dcicutils/captured_output.py` & `dcicutils-8.8.4.1b7/dcicutils/captured_output.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b6/dcicutils/cloudformation_utils.py` & `dcicutils-8.8.4.1b7/dcicutils/cloudformation_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b6/dcicutils/codebuild_utils.py` & `dcicutils-8.8.4.1b7/dcicutils/codebuild_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b6/dcicutils/command_utils.py` & `dcicutils-8.8.4.1b7/dcicutils/command_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b6/dcicutils/common.py` & `dcicutils-8.8.4.1b7/dcicutils/common.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b6/dcicutils/contribution_scripts.py` & `dcicutils-8.8.4.1b7/dcicutils/contribution_scripts.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b6/dcicutils/contribution_utils.py` & `dcicutils-8.8.4.1b7/dcicutils/contribution_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b6/dcicutils/creds_utils.py` & `dcicutils-8.8.4.1b7/dcicutils/creds_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b6/dcicutils/data_readers.py` & `dcicutils-8.8.4.1b7/dcicutils/data_readers.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b6/dcicutils/data_utils.py` & `dcicutils-8.8.4.1b7/dcicutils/data_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b6/dcicutils/datetime_utils.py` & `dcicutils-8.8.4.1b7/dcicutils/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b6/dcicutils/deployment_utils.py` & `dcicutils-8.8.4.1b7/dcicutils/deployment_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b6/dcicutils/diff_utils.py` & `dcicutils-8.8.4.1b7/dcicutils/diff_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b6/dcicutils/docker_utils.py` & `dcicutils-8.8.4.1b7/dcicutils/docker_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b6/dcicutils/ecr_scripts.py` & `dcicutils-8.8.4.1b7/dcicutils/ecr_scripts.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b6/dcicutils/ecr_utils.py` & `dcicutils-8.8.4.1b7/dcicutils/ecr_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b6/dcicutils/ecs_utils.py` & `dcicutils-8.8.4.1b7/dcicutils/ecs_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b6/dcicutils/env_base.py` & `dcicutils-8.8.4.1b7/dcicutils/env_base.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b6/dcicutils/env_manager.py` & `dcicutils-8.8.4.1b7/dcicutils/env_manager.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b6/dcicutils/env_scripts.py` & `dcicutils-8.8.4.1b7/dcicutils/env_scripts.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b6/dcicutils/env_utils.py` & `dcicutils-8.8.4.1b7/dcicutils/env_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b6/dcicutils/env_utils_legacy.py` & `dcicutils-8.8.4.1b7/dcicutils/env_utils_legacy.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b6/dcicutils/es_utils.py` & `dcicutils-8.8.4.1b7/dcicutils/es_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b6/dcicutils/exceptions.py` & `dcicutils-8.8.4.1b7/dcicutils/exceptions.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b6/dcicutils/ff_mocks.py` & `dcicutils-8.8.4.1b7/dcicutils/ff_mocks.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b6/dcicutils/ff_utils.py` & `dcicutils-8.8.4.1b7/dcicutils/ff_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b6/dcicutils/file_utils.py` & `dcicutils-8.8.4.1b7/dcicutils/file_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b6/dcicutils/function_cache_decorator.py` & `dcicutils-8.8.4.1b7/dcicutils/function_cache_decorator.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b6/dcicutils/glacier_utils.py` & `dcicutils-8.8.4.1b7/dcicutils/glacier_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b6/dcicutils/http_utils.py` & `dcicutils-8.8.4.1b7/dcicutils/http_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b6/dcicutils/jh_utils.py` & `dcicutils-8.8.4.1b7/dcicutils/jh_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b6/dcicutils/kibana/dashboards.json` & `dcicutils-8.8.4.1b7/dcicutils/kibana/dashboards.json`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b6/dcicutils/kibana/readme.md` & `dcicutils-8.8.4.1b7/dcicutils/kibana/readme.md`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b6/dcicutils/lang_utils.py` & `dcicutils-8.8.4.1b7/dcicutils/lang_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b6/dcicutils/license_policies/park-lab-common-server.jsonc` & `dcicutils-8.8.4.1b7/dcicutils/license_policies/park-lab-common-server.jsonc`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b6/dcicutils/license_policies/park-lab-common.jsonc` & `dcicutils-8.8.4.1b7/dcicutils/license_policies/park-lab-common.jsonc`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b6/dcicutils/license_policies/park-lab-gpl-pipeline.jsonc` & `dcicutils-8.8.4.1b7/dcicutils/license_policies/park-lab-gpl-pipeline.jsonc`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b6/dcicutils/license_utils.py` & `dcicutils-8.8.4.1b7/dcicutils/license_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b6/dcicutils/log_utils.py` & `dcicutils-8.8.4.1b7/dcicutils/log_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b6/dcicutils/misc_utils.py` & `dcicutils-8.8.4.1b7/dcicutils/misc_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b6/dcicutils/obfuscation_utils.py` & `dcicutils-8.8.4.1b7/dcicutils/obfuscation_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b6/dcicutils/opensearch_utils.py` & `dcicutils-8.8.4.1b7/dcicutils/opensearch_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b6/dcicutils/portal_object_utils.py` & `dcicutils-8.8.4.1b7/dcicutils/portal_object_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b6/dcicutils/portal_utils.py` & `dcicutils-8.8.4.1b7/dcicutils/portal_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b6/dcicutils/progress_bar.py` & `dcicutils-8.8.4.1b7/dcicutils/progress_bar.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b6/dcicutils/project_utils.py` & `dcicutils-8.8.4.1b7/dcicutils/project_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b6/dcicutils/qa_checkers.py` & `dcicutils-8.8.4.1b7/dcicutils/qa_checkers.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b6/dcicutils/qa_utils.py` & `dcicutils-8.8.4.1b7/dcicutils/qa_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b6/dcicutils/redis_tools.py` & `dcicutils-8.8.4.1b7/dcicutils/redis_tools.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b6/dcicutils/redis_utils.py` & `dcicutils-8.8.4.1b7/dcicutils/redis_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b6/dcicutils/s3_utils.py` & `dcicutils-8.8.4.1b7/dcicutils/s3_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b6/dcicutils/schema_utils.py` & `dcicutils-8.8.4.1b7/dcicutils/schema_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b6/dcicutils/scripts/publish_to_pypi.py` & `dcicutils-8.8.4.1b7/dcicutils/scripts/publish_to_pypi.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b6/dcicutils/scripts/run_license_checker.py` & `dcicutils-8.8.4.1b7/dcicutils/scripts/run_license_checker.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b6/dcicutils/scripts/view_portal_object.py` & `dcicutils-8.8.4.1b7/dcicutils/scripts/view_portal_object.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b6/dcicutils/secrets_utils.py` & `dcicutils-8.8.4.1b7/dcicutils/secrets_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b6/dcicutils/sheet_utils.py` & `dcicutils-8.8.4.1b7/dcicutils/sheet_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b6/dcicutils/snapshot_utils.py` & `dcicutils-8.8.4.1b7/dcicutils/snapshot_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b6/dcicutils/ssl_certificate_utils.py` & `dcicutils-8.8.4.1b7/dcicutils/ssl_certificate_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b6/dcicutils/structured_data.py` & `dcicutils-8.8.4.1b7/dcicutils/structured_data.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b6/dcicutils/submitr/progress_constants.py` & `dcicutils-8.8.4.1b7/dcicutils/submitr/progress_constants.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b6/dcicutils/submitr/ref_lookup_strategy.py` & `dcicutils-8.8.4.1b7/dcicutils/submitr/ref_lookup_strategy.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b6/dcicutils/task_utils.py` & `dcicutils-8.8.4.1b7/dcicutils/task_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b6/dcicutils/tmpfile_utils.py` & `dcicutils-8.8.4.1b7/dcicutils/tmpfile_utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -35,19 +35,19 @@
             return os.path.commonpath([path, tmpdir]) == tmpdir and os.path.exists(path) and os.path.isdir(path)
         except Exception:
             return False
     if is_temporary_directory(tmp_directory_name):  # Guard against errant deletion.
         shutil.rmtree(tmp_directory_name)
 
 
-def create_temporary_file_name(suffix: Optional[str] = None) -> str:
+def create_temporary_file_name(prefix: Optional[str] = None, suffix: Optional[str] = None) -> str:
     """
     Generates and returns the full path to file within the system temporary directory.
     """
-    with tempfile.NamedTemporaryFile(suffix=suffix, delete=False) as tmp_file:
+    with tempfile.NamedTemporaryFile(prefix=prefix, suffix=suffix, delete=False) as tmp_file:
         tmp_file_name = tmp_file.name
     return tmp_file_name
 
 
 def remove_temporary_file(tmp_file_name: str) -> bool:
     """
     Removes the given file; but ONLY if it is (somewhere) within the system temporary directory.
```

### Comparing `dcicutils-8.8.4.1b6/dcicutils/trace_utils.py` & `dcicutils-8.8.4.1b7/dcicutils/trace_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b6/dcicutils/validation_utils.py` & `dcicutils-8.8.4.1b7/dcicutils/validation_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b6/dcicutils/variant_utils.py` & `dcicutils-8.8.4.1b7/dcicutils/variant_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b6/dcicutils/zip_utils.py` & `dcicutils-8.8.4.1b7/dcicutils/zip_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.4.1b6/pyproject.toml` & `dcicutils-8.8.4.1b7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dcicutils"
-version = "8.8.4.1b6"  # TODO: To become 8.8.5
+version = "8.8.4.1b7"  # TODO: To become 8.8.5
 description = "Utility package for interacting with the 4DN Data Portal and other 4DN resources"
 authors = ["4DN-DCIC Team <support@4dnucleome.org>"]
 license = "MIT"
 readme = "README.rst"
 homepage = "https://github.com/4dn-dcic/utils"
 repository = "https://github.com/4dn-dcic/utils"
 packages = [
```

### Comparing `dcicutils-8.8.4.1b6/PKG-INFO` & `dcicutils-8.8.4.1b7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcicutils
-Version: 8.8.4.1b6
+Version: 8.8.4.1b7
 Summary: Utility package for interacting with the 4DN Data Portal and other 4DN resources
 Home-page: https://github.com/4dn-dcic/utils
 License: MIT
 Author: 4DN-DCIC Team
 Author-email: support@4dnucleome.org
 Requires-Python: >=3.8,<3.13
 Classifier: Development Status :: 4 - Beta
```


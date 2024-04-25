# Comparing `tmp/exasol_transformers_extension-1.0.0.tar.gz` & `tmp/exasol_transformers_extension-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exasol_transformers_extension-1.0.0.tar", max compression
+gzip compressed data, was "exasol_transformers_extension-1.0.1.tar", max compression
```

## Comparing `exasol_transformers_extension-1.0.0.tar` & `exasol_transformers_extension-1.0.1.tar`

### file list

```diff
@@ -1,57 +1,57 @@
--rw-r--r--   0        0        0     1063 2024-04-12 11:14:18.044924 exasol_transformers_extension-1.0.0/LICENSE
--rw-r--r--   0        0        0      653 2024-04-12 11:14:18.044924 exasol_transformers_extension-1.0.0/README.md
--rw-r--r--   0        0        0       22 2024-04-12 11:14:18.048924 exasol_transformers_extension-1.0.0/exasol_transformers_extension/__init__.py
--rw-r--r--   0        0        0     1019 2024-04-12 11:14:18.048924 exasol_transformers_extension-1.0.0/exasol_transformers_extension/deploy.py
--rw-r--r--   0        0        0        0 2024-04-12 11:14:18.048924 exasol_transformers_extension-1.0.0/exasol_transformers_extension/deployment/__init__.py
--rw-r--r--   0        0        0     1078 2024-04-12 11:14:18.048924 exasol_transformers_extension-1.0.0/exasol_transformers_extension/deployment/constants.py
--rw-r--r--   0        0        0     1083 2024-04-12 11:14:18.048924 exasol_transformers_extension-1.0.0/exasol_transformers_extension/deployment/deployment_utils.py
--rw-r--r--   0        0        0     3813 2024-04-12 11:14:18.048924 exasol_transformers_extension-1.0.0/exasol_transformers_extension/deployment/language_container.py
--rw-r--r--   0        0        0    13328 2024-04-12 11:14:18.048924 exasol_transformers_extension-1.0.0/exasol_transformers_extension/deployment/language_container_deployer.py
--rw-r--r--   0        0        0     7899 2024-04-12 11:14:18.048924 exasol_transformers_extension-1.0.0/exasol_transformers_extension/deployment/language_container_deployer_cli.py
--rw-r--r--   0        0        0     2376 2024-04-12 11:14:18.048924 exasol_transformers_extension-1.0.0/exasol_transformers_extension/deployment/scripts_deployer.py
--rw-r--r--   0        0        0     1379 2024-04-12 11:14:18.048924 exasol_transformers_extension-1.0.0/exasol_transformers_extension/deployment/scripts_deployer_cli.py
--rw-r--r--   0        0        0     1155 2024-04-12 11:14:18.048924 exasol_transformers_extension-1.0.0/exasol_transformers_extension/deployment/te_language_container_deployer.py
--rw-r--r--   0        0        0        0 2024-04-12 11:14:18.048924 exasol_transformers_extension-1.0.0/exasol_transformers_extension/resources/__init__.py
--rw-r--r--   0        0        0      593 2024-04-12 11:14:18.048924 exasol_transformers_extension-1.0.0/exasol_transformers_extension/resources/templates/filling_mask_udf.jinja.sql
--rw-r--r--   0        0        0      339 2024-04-12 11:14:18.048924 exasol_transformers_extension-1.0.0/exasol_transformers_extension/resources/templates/model_downloader_udf.jinja.sql
--rw-r--r--   0        0        0      662 2024-04-12 11:14:18.048924 exasol_transformers_extension-1.0.0/exasol_transformers_extension/resources/templates/question_answering_udf.jinja.sql
--rw-r--r--   0        0        0      554 2024-04-12 11:14:18.048924 exasol_transformers_extension-1.0.0/exasol_transformers_extension/resources/templates/sequence_classification_single_text_udf.jinja.sql
--rw-r--r--   0        0        0      622 2024-04-12 11:14:18.048924 exasol_transformers_extension-1.0.0/exasol_transformers_extension/resources/templates/sequence_classification_text_pair_udf.jinja.sql
--rw-r--r--   0        0        0      632 2024-04-12 11:14:18.048924 exasol_transformers_extension-1.0.0/exasol_transformers_extension/resources/templates/text_generation_udf.jinja.sql
--rw-r--r--   0        0        0      697 2024-04-12 11:14:18.048924 exasol_transformers_extension-1.0.0/exasol_transformers_extension/resources/templates/token_classification_udf.jinja.sql
--rw-r--r--   0        0        0      722 2024-04-12 11:14:18.048924 exasol_transformers_extension-1.0.0/exasol_transformers_extension/resources/templates/translation_udf.jinja.sql
--rw-r--r--   0        0        0      644 2024-04-12 11:14:18.048924 exasol_transformers_extension-1.0.0/exasol_transformers_extension/resources/templates/zero_shot_text_classification_udf.jinja.sql
--rw-r--r--   0        0        0        0 2024-04-12 11:14:18.048924 exasol_transformers_extension-1.0.0/exasol_transformers_extension/udfs/__init__.py
--rw-r--r--   0        0        0        0 2024-04-12 11:14:18.048924 exasol_transformers_extension-1.0.0/exasol_transformers_extension/udfs/callers/__init__.py
--rw-r--r--   0        0        0      154 2024-04-12 11:14:18.048924 exasol_transformers_extension-1.0.0/exasol_transformers_extension/udfs/callers/filling_mask_udf_call.py
--rw-r--r--   0        0        0      170 2024-04-12 11:14:18.048924 exasol_transformers_extension-1.0.0/exasol_transformers_extension/udfs/callers/model_downloader_udf_call.py
--rw-r--r--   0        0        0      177 2024-04-12 11:14:18.048924 exasol_transformers_extension-1.0.0/exasol_transformers_extension/udfs/callers/question_answering_udf_call.py
--rw-r--r--   0        0        0      224 2024-04-12 11:14:18.048924 exasol_transformers_extension-1.0.0/exasol_transformers_extension/udfs/callers/sequence_classification_single_text_udf_call.py
--rw-r--r--   0        0        0      218 2024-04-12 11:14:18.048924 exasol_transformers_extension-1.0.0/exasol_transformers_extension/udfs/callers/sequence_classification_text_pair_udf_call.py
--rw-r--r--   0        0        0      168 2024-04-12 11:14:18.048924 exasol_transformers_extension-1.0.0/exasol_transformers_extension/udfs/callers/text_generation_udf_call.py
--rw-r--r--   0        0        0      183 2024-04-12 11:14:18.048924 exasol_transformers_extension-1.0.0/exasol_transformers_extension/udfs/callers/token_classification_udf_call.py
--rw-r--r--   0        0        0      158 2024-04-12 11:14:18.048924 exasol_transformers_extension-1.0.0/exasol_transformers_extension/udfs/callers/translation_udf_call.py
--rw-r--r--   0        0        0      206 2024-04-12 11:14:18.048924 exasol_transformers_extension-1.0.0/exasol_transformers_extension/udfs/callers/zero_shot_text_classification_udf.py
--rw-r--r--   0        0        0        0 2024-04-12 11:14:18.048924 exasol_transformers_extension-1.0.0/exasol_transformers_extension/udfs/models/__init__.py
--rw-r--r--   0        0        0    10362 2024-04-12 11:14:18.048924 exasol_transformers_extension-1.0.0/exasol_transformers_extension/udfs/models/base_model_udf.py
--rw-r--r--   0        0        0     4483 2024-04-12 11:14:18.048924 exasol_transformers_extension-1.0.0/exasol_transformers_extension/udfs/models/filling_mask_udf.py
--rw-r--r--   0        0        0     3779 2024-04-12 11:14:18.048924 exasol_transformers_extension-1.0.0/exasol_transformers_extension/udfs/models/model_downloader_udf.py
--rw-r--r--   0        0        0     4258 2024-04-12 11:14:18.048924 exasol_transformers_extension-1.0.0/exasol_transformers_extension/udfs/models/question_answering_udf.py
--rw-r--r--   0        0        0     3251 2024-04-12 11:14:18.048924 exasol_transformers_extension-1.0.0/exasol_transformers_extension/udfs/models/sequence_classification_single_text_udf.py
--rw-r--r--   0        0        0     3509 2024-04-12 11:14:18.048924 exasol_transformers_extension-1.0.0/exasol_transformers_extension/udfs/models/sequence_classification_text_pair_udf.py
--rw-r--r--   0        0        0     3712 2024-04-12 11:14:18.048924 exasol_transformers_extension-1.0.0/exasol_transformers_extension/udfs/models/text_generation_udf.py
--rw-r--r--   0        0        0     4714 2024-04-12 11:14:18.048924 exasol_transformers_extension-1.0.0/exasol_transformers_extension/udfs/models/token_classification_udf.py
--rw-r--r--   0        0        0     3806 2024-04-12 11:14:18.048924 exasol_transformers_extension-1.0.0/exasol_transformers_extension/udfs/models/translation_udf.py
--rw-r--r--   0        0        0     4047 2024-04-12 11:14:18.048924 exasol_transformers_extension-1.0.0/exasol_transformers_extension/udfs/models/zero_shot_text_classification_udf.py
--rw-r--r--   0        0        0     2268 2024-04-12 11:14:18.048924 exasol_transformers_extension-1.0.0/exasol_transformers_extension/upload_model.py
--rw-r--r--   0        0        0        0 2024-04-12 11:14:18.048924 exasol_transformers_extension-1.0.0/exasol_transformers_extension/utils/__init__.py
--rw-r--r--   0        0        0      899 2024-04-12 11:14:18.048924 exasol_transformers_extension-1.0.0/exasol_transformers_extension/utils/bucketfs_model_uploader.py
--rw-r--r--   0        0        0     3246 2024-04-12 11:14:18.048924 exasol_transformers_extension-1.0.0/exasol_transformers_extension/utils/bucketfs_operations.py
--rw-r--r--   0        0        0     1126 2024-04-12 11:14:18.048924 exasol_transformers_extension-1.0.0/exasol_transformers_extension/utils/dataframe_operations.py
--rw-r--r--   0        0        0      383 2024-04-12 11:14:18.048924 exasol_transformers_extension-1.0.0/exasol_transformers_extension/utils/device_management.py
--rw-r--r--   0        0        0     4412 2024-04-12 11:14:18.048924 exasol_transformers_extension-1.0.0/exasol_transformers_extension/utils/huggingface_hub_bucketfs_model_transfer_sp.py
--rw-r--r--   0        0        0     2438 2024-04-12 11:14:18.048924 exasol_transformers_extension-1.0.0/exasol_transformers_extension/utils/load_local_model.py
--rw-r--r--   0        0        0      893 2024-04-12 11:14:18.048924 exasol_transformers_extension-1.0.0/exasol_transformers_extension/utils/model_factory_protocol.py
--rw-r--r--   0        0        0      150 2024-04-12 11:14:18.048924 exasol_transformers_extension-1.0.0/exasol_transformers_extension/utils/temporary_directory_factory.py
--rw-r--r--   0        0        0     1112 2024-04-12 11:14:18.052924 exasol_transformers_extension-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     1824 1970-01-01 00:00:00.000000 exasol_transformers_extension-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-04-25 15:30:01.361847 exasol_transformers_extension-1.0.1/LICENSE
+-rw-r--r--   0        0        0      653 2024-04-25 15:30:01.361847 exasol_transformers_extension-1.0.1/README.md
+-rw-r--r--   0        0        0       22 2024-04-25 15:30:01.365847 exasol_transformers_extension-1.0.1/exasol_transformers_extension/__init__.py
+-rw-r--r--   0        0        0     1019 2024-04-25 15:30:01.365847 exasol_transformers_extension-1.0.1/exasol_transformers_extension/deploy.py
+-rw-r--r--   0        0        0        0 2024-04-25 15:30:01.365847 exasol_transformers_extension-1.0.1/exasol_transformers_extension/deployment/__init__.py
+-rw-r--r--   0        0        0     1078 2024-04-25 15:30:01.365847 exasol_transformers_extension-1.0.1/exasol_transformers_extension/deployment/constants.py
+-rw-r--r--   0        0        0     1083 2024-04-25 15:30:01.365847 exasol_transformers_extension-1.0.1/exasol_transformers_extension/deployment/deployment_utils.py
+-rw-r--r--   0        0        0     3813 2024-04-25 15:30:01.365847 exasol_transformers_extension-1.0.1/exasol_transformers_extension/deployment/language_container.py
+-rw-r--r--   0        0        0    13328 2024-04-25 15:30:01.365847 exasol_transformers_extension-1.0.1/exasol_transformers_extension/deployment/language_container_deployer.py
+-rw-r--r--   0        0        0     7899 2024-04-25 15:30:01.365847 exasol_transformers_extension-1.0.1/exasol_transformers_extension/deployment/language_container_deployer_cli.py
+-rw-r--r--   0        0        0     2376 2024-04-25 15:30:01.365847 exasol_transformers_extension-1.0.1/exasol_transformers_extension/deployment/scripts_deployer.py
+-rw-r--r--   0        0        0     1379 2024-04-25 15:30:01.365847 exasol_transformers_extension-1.0.1/exasol_transformers_extension/deployment/scripts_deployer_cli.py
+-rw-r--r--   0        0        0     1155 2024-04-25 15:30:01.365847 exasol_transformers_extension-1.0.1/exasol_transformers_extension/deployment/te_language_container_deployer.py
+-rw-r--r--   0        0        0        0 2024-04-25 15:30:01.365847 exasol_transformers_extension-1.0.1/exasol_transformers_extension/resources/__init__.py
+-rw-r--r--   0        0        0      593 2024-04-25 15:30:01.365847 exasol_transformers_extension-1.0.1/exasol_transformers_extension/resources/templates/filling_mask_udf.jinja.sql
+-rw-r--r--   0        0        0      339 2024-04-25 15:30:01.365847 exasol_transformers_extension-1.0.1/exasol_transformers_extension/resources/templates/model_downloader_udf.jinja.sql
+-rw-r--r--   0        0        0      662 2024-04-25 15:30:01.365847 exasol_transformers_extension-1.0.1/exasol_transformers_extension/resources/templates/question_answering_udf.jinja.sql
+-rw-r--r--   0        0        0      554 2024-04-25 15:30:01.365847 exasol_transformers_extension-1.0.1/exasol_transformers_extension/resources/templates/sequence_classification_single_text_udf.jinja.sql
+-rw-r--r--   0        0        0      622 2024-04-25 15:30:01.365847 exasol_transformers_extension-1.0.1/exasol_transformers_extension/resources/templates/sequence_classification_text_pair_udf.jinja.sql
+-rw-r--r--   0        0        0      632 2024-04-25 15:30:01.365847 exasol_transformers_extension-1.0.1/exasol_transformers_extension/resources/templates/text_generation_udf.jinja.sql
+-rw-r--r--   0        0        0      697 2024-04-25 15:30:01.365847 exasol_transformers_extension-1.0.1/exasol_transformers_extension/resources/templates/token_classification_udf.jinja.sql
+-rw-r--r--   0        0        0      722 2024-04-25 15:30:01.365847 exasol_transformers_extension-1.0.1/exasol_transformers_extension/resources/templates/translation_udf.jinja.sql
+-rw-r--r--   0        0        0      644 2024-04-25 15:30:01.365847 exasol_transformers_extension-1.0.1/exasol_transformers_extension/resources/templates/zero_shot_text_classification_udf.jinja.sql
+-rw-r--r--   0        0        0        0 2024-04-25 15:30:01.365847 exasol_transformers_extension-1.0.1/exasol_transformers_extension/udfs/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-25 15:30:01.365847 exasol_transformers_extension-1.0.1/exasol_transformers_extension/udfs/callers/__init__.py
+-rw-r--r--   0        0        0      154 2024-04-25 15:30:01.365847 exasol_transformers_extension-1.0.1/exasol_transformers_extension/udfs/callers/filling_mask_udf_call.py
+-rw-r--r--   0        0        0      170 2024-04-25 15:30:01.365847 exasol_transformers_extension-1.0.1/exasol_transformers_extension/udfs/callers/model_downloader_udf_call.py
+-rw-r--r--   0        0        0      177 2024-04-25 15:30:01.365847 exasol_transformers_extension-1.0.1/exasol_transformers_extension/udfs/callers/question_answering_udf_call.py
+-rw-r--r--   0        0        0      224 2024-04-25 15:30:01.365847 exasol_transformers_extension-1.0.1/exasol_transformers_extension/udfs/callers/sequence_classification_single_text_udf_call.py
+-rw-r--r--   0        0        0      218 2024-04-25 15:30:01.365847 exasol_transformers_extension-1.0.1/exasol_transformers_extension/udfs/callers/sequence_classification_text_pair_udf_call.py
+-rw-r--r--   0        0        0      168 2024-04-25 15:30:01.365847 exasol_transformers_extension-1.0.1/exasol_transformers_extension/udfs/callers/text_generation_udf_call.py
+-rw-r--r--   0        0        0      183 2024-04-25 15:30:01.365847 exasol_transformers_extension-1.0.1/exasol_transformers_extension/udfs/callers/token_classification_udf_call.py
+-rw-r--r--   0        0        0      158 2024-04-25 15:30:01.365847 exasol_transformers_extension-1.0.1/exasol_transformers_extension/udfs/callers/translation_udf_call.py
+-rw-r--r--   0        0        0      206 2024-04-25 15:30:01.365847 exasol_transformers_extension-1.0.1/exasol_transformers_extension/udfs/callers/zero_shot_text_classification_udf.py
+-rw-r--r--   0        0        0        0 2024-04-25 15:30:01.365847 exasol_transformers_extension-1.0.1/exasol_transformers_extension/udfs/models/__init__.py
+-rw-r--r--   0        0        0    10362 2024-04-25 15:30:01.365847 exasol_transformers_extension-1.0.1/exasol_transformers_extension/udfs/models/base_model_udf.py
+-rw-r--r--   0        0        0     4483 2024-04-25 15:30:01.365847 exasol_transformers_extension-1.0.1/exasol_transformers_extension/udfs/models/filling_mask_udf.py
+-rw-r--r--   0        0        0     3795 2024-04-25 15:30:01.365847 exasol_transformers_extension-1.0.1/exasol_transformers_extension/udfs/models/model_downloader_udf.py
+-rw-r--r--   0        0        0     4258 2024-04-25 15:30:01.365847 exasol_transformers_extension-1.0.1/exasol_transformers_extension/udfs/models/question_answering_udf.py
+-rw-r--r--   0        0        0     3251 2024-04-25 15:30:01.365847 exasol_transformers_extension-1.0.1/exasol_transformers_extension/udfs/models/sequence_classification_single_text_udf.py
+-rw-r--r--   0        0        0     3509 2024-04-25 15:30:01.365847 exasol_transformers_extension-1.0.1/exasol_transformers_extension/udfs/models/sequence_classification_text_pair_udf.py
+-rw-r--r--   0        0        0     3712 2024-04-25 15:30:01.365847 exasol_transformers_extension-1.0.1/exasol_transformers_extension/udfs/models/text_generation_udf.py
+-rw-r--r--   0        0        0     4714 2024-04-25 15:30:01.365847 exasol_transformers_extension-1.0.1/exasol_transformers_extension/udfs/models/token_classification_udf.py
+-rw-r--r--   0        0        0     3806 2024-04-25 15:30:01.365847 exasol_transformers_extension-1.0.1/exasol_transformers_extension/udfs/models/translation_udf.py
+-rw-r--r--   0        0        0     4047 2024-04-25 15:30:01.365847 exasol_transformers_extension-1.0.1/exasol_transformers_extension/udfs/models/zero_shot_text_classification_udf.py
+-rw-r--r--   0        0        0     2268 2024-04-25 15:30:01.365847 exasol_transformers_extension-1.0.1/exasol_transformers_extension/upload_model.py
+-rw-r--r--   0        0        0        0 2024-04-25 15:30:01.365847 exasol_transformers_extension-1.0.1/exasol_transformers_extension/utils/__init__.py
+-rw-r--r--   0        0        0      899 2024-04-25 15:30:01.365847 exasol_transformers_extension-1.0.1/exasol_transformers_extension/utils/bucketfs_model_uploader.py
+-rw-r--r--   0        0        0     3246 2024-04-25 15:30:01.365847 exasol_transformers_extension-1.0.1/exasol_transformers_extension/utils/bucketfs_operations.py
+-rw-r--r--   0        0        0     1126 2024-04-25 15:30:01.365847 exasol_transformers_extension-1.0.1/exasol_transformers_extension/utils/dataframe_operations.py
+-rw-r--r--   0        0        0      383 2024-04-25 15:30:01.365847 exasol_transformers_extension-1.0.1/exasol_transformers_extension/utils/device_management.py
+-rw-r--r--   0        0        0     4412 2024-04-25 15:30:01.365847 exasol_transformers_extension-1.0.1/exasol_transformers_extension/utils/huggingface_hub_bucketfs_model_transfer_sp.py
+-rw-r--r--   0        0        0     2438 2024-04-25 15:30:01.365847 exasol_transformers_extension-1.0.1/exasol_transformers_extension/utils/load_local_model.py
+-rw-r--r--   0        0        0      893 2024-04-25 15:30:01.365847 exasol_transformers_extension-1.0.1/exasol_transformers_extension/utils/model_factory_protocol.py
+-rw-r--r--   0        0        0      150 2024-04-25 15:30:01.365847 exasol_transformers_extension-1.0.1/exasol_transformers_extension/utils/temporary_directory_factory.py
+-rw-r--r--   0        0        0     1112 2024-04-25 15:30:01.369847 exasol_transformers_extension-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     1824 1970-01-01 00:00:00.000000 exasol_transformers_extension-1.0.1/PKG-INFO
```

### Comparing `exasol_transformers_extension-1.0.0/LICENSE` & `exasol_transformers_extension-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `exasol_transformers_extension-1.0.0/README.md` & `exasol_transformers_extension-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `exasol_transformers_extension-1.0.0/exasol_transformers_extension/deploy.py` & `exasol_transformers_extension-1.0.1/exasol_transformers_extension/deploy.py`

 * *Files identical despite different names*

### Comparing `exasol_transformers_extension-1.0.0/exasol_transformers_extension/deployment/constants.py` & `exasol_transformers_extension-1.0.1/exasol_transformers_extension/deployment/constants.py`

 * *Files identical despite different names*

### Comparing `exasol_transformers_extension-1.0.0/exasol_transformers_extension/deployment/deployment_utils.py` & `exasol_transformers_extension-1.0.1/exasol_transformers_extension/deployment/deployment_utils.py`

 * *Files identical despite different names*

### Comparing `exasol_transformers_extension-1.0.0/exasol_transformers_extension/deployment/language_container.py` & `exasol_transformers_extension-1.0.1/exasol_transformers_extension/deployment/language_container.py`

 * *Files identical despite different names*

### Comparing `exasol_transformers_extension-1.0.0/exasol_transformers_extension/deployment/language_container_deployer.py` & `exasol_transformers_extension-1.0.1/exasol_transformers_extension/deployment/language_container_deployer.py`

 * *Files identical despite different names*

### Comparing `exasol_transformers_extension-1.0.0/exasol_transformers_extension/deployment/language_container_deployer_cli.py` & `exasol_transformers_extension-1.0.1/exasol_transformers_extension/deployment/language_container_deployer_cli.py`

 * *Files identical despite different names*

### Comparing `exasol_transformers_extension-1.0.0/exasol_transformers_extension/deployment/scripts_deployer.py` & `exasol_transformers_extension-1.0.1/exasol_transformers_extension/deployment/scripts_deployer.py`

 * *Files identical despite different names*

### Comparing `exasol_transformers_extension-1.0.0/exasol_transformers_extension/deployment/scripts_deployer_cli.py` & `exasol_transformers_extension-1.0.1/exasol_transformers_extension/deployment/scripts_deployer_cli.py`

 * *Files identical despite different names*

### Comparing `exasol_transformers_extension-1.0.0/exasol_transformers_extension/deployment/te_language_container_deployer.py` & `exasol_transformers_extension-1.0.1/exasol_transformers_extension/deployment/te_language_container_deployer.py`

 * *Files identical despite different names*

### Comparing `exasol_transformers_extension-1.0.0/exasol_transformers_extension/resources/templates/filling_mask_udf.jinja.sql` & `exasol_transformers_extension-1.0.1/exasol_transformers_extension/resources/templates/filling_mask_udf.jinja.sql`

 * *Files identical despite different names*

### Comparing `exasol_transformers_extension-1.0.0/exasol_transformers_extension/resources/templates/question_answering_udf.jinja.sql` & `exasol_transformers_extension-1.0.1/exasol_transformers_extension/resources/templates/question_answering_udf.jinja.sql`

 * *Files identical despite different names*

### Comparing `exasol_transformers_extension-1.0.0/exasol_transformers_extension/resources/templates/sequence_classification_single_text_udf.jinja.sql` & `exasol_transformers_extension-1.0.1/exasol_transformers_extension/resources/templates/sequence_classification_single_text_udf.jinja.sql`

 * *Files identical despite different names*

### Comparing `exasol_transformers_extension-1.0.0/exasol_transformers_extension/resources/templates/sequence_classification_text_pair_udf.jinja.sql` & `exasol_transformers_extension-1.0.1/exasol_transformers_extension/resources/templates/sequence_classification_text_pair_udf.jinja.sql`

 * *Files identical despite different names*

### Comparing `exasol_transformers_extension-1.0.0/exasol_transformers_extension/resources/templates/text_generation_udf.jinja.sql` & `exasol_transformers_extension-1.0.1/exasol_transformers_extension/resources/templates/text_generation_udf.jinja.sql`

 * *Files identical despite different names*

### Comparing `exasol_transformers_extension-1.0.0/exasol_transformers_extension/resources/templates/token_classification_udf.jinja.sql` & `exasol_transformers_extension-1.0.1/exasol_transformers_extension/resources/templates/token_classification_udf.jinja.sql`

 * *Files identical despite different names*

### Comparing `exasol_transformers_extension-1.0.0/exasol_transformers_extension/resources/templates/translation_udf.jinja.sql` & `exasol_transformers_extension-1.0.1/exasol_transformers_extension/resources/templates/translation_udf.jinja.sql`

 * *Files identical despite different names*

### Comparing `exasol_transformers_extension-1.0.0/exasol_transformers_extension/resources/templates/zero_shot_text_classification_udf.jinja.sql` & `exasol_transformers_extension-1.0.1/exasol_transformers_extension/resources/templates/zero_shot_text_classification_udf.jinja.sql`

 * *Files identical despite different names*

### Comparing `exasol_transformers_extension-1.0.0/exasol_transformers_extension/udfs/models/base_model_udf.py` & `exasol_transformers_extension-1.0.1/exasol_transformers_extension/udfs/models/base_model_udf.py`

 * *Files identical despite different names*

### Comparing `exasol_transformers_extension-1.0.0/exasol_transformers_extension/udfs/models/filling_mask_udf.py` & `exasol_transformers_extension-1.0.1/exasol_transformers_extension/udfs/models/filling_mask_udf.py`

 * *Files identical despite different names*

### Comparing `exasol_transformers_extension-1.0.0/exasol_transformers_extension/udfs/models/model_downloader_udf.py` & `exasol_transformers_extension-1.0.1/exasol_transformers_extension/udfs/models/model_downloader_udf.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,15 @@
         # whether there is a token for public model or even what the token is.
         token = False
         if token_conn:
             token_conn_obj = self._exa.get_connection(token_conn)
             token = token_conn_obj.password
 
         # set model path in buckets
-        model_path = bucketfs_operations.get_model_path(sub_dir, model_name)
+        model_path = bucketfs_operations.get_model_path_with_pretrained(sub_dir, model_name)
 
         # create bucketfs location
         bfs_conn_obj = self._exa.get_connection(bfs_conn)
         bucketfs_location = self._bucketfs_factory.create_bucketfs_location(
             url=bfs_conn_obj.address,
             user=bfs_conn_obj.user,
             pwd=bfs_conn_obj.password
```

### Comparing `exasol_transformers_extension-1.0.0/exasol_transformers_extension/udfs/models/question_answering_udf.py` & `exasol_transformers_extension-1.0.1/exasol_transformers_extension/udfs/models/question_answering_udf.py`

 * *Files identical despite different names*

### Comparing `exasol_transformers_extension-1.0.0/exasol_transformers_extension/udfs/models/sequence_classification_single_text_udf.py` & `exasol_transformers_extension-1.0.1/exasol_transformers_extension/udfs/models/sequence_classification_single_text_udf.py`

 * *Files identical despite different names*

### Comparing `exasol_transformers_extension-1.0.0/exasol_transformers_extension/udfs/models/sequence_classification_text_pair_udf.py` & `exasol_transformers_extension-1.0.1/exasol_transformers_extension/udfs/models/sequence_classification_text_pair_udf.py`

 * *Files identical despite different names*

### Comparing `exasol_transformers_extension-1.0.0/exasol_transformers_extension/udfs/models/text_generation_udf.py` & `exasol_transformers_extension-1.0.1/exasol_transformers_extension/udfs/models/text_generation_udf.py`

 * *Files identical despite different names*

### Comparing `exasol_transformers_extension-1.0.0/exasol_transformers_extension/udfs/models/token_classification_udf.py` & `exasol_transformers_extension-1.0.1/exasol_transformers_extension/udfs/models/token_classification_udf.py`

 * *Files identical despite different names*

### Comparing `exasol_transformers_extension-1.0.0/exasol_transformers_extension/udfs/models/translation_udf.py` & `exasol_transformers_extension-1.0.1/exasol_transformers_extension/udfs/models/translation_udf.py`

 * *Files identical despite different names*

### Comparing `exasol_transformers_extension-1.0.0/exasol_transformers_extension/udfs/models/zero_shot_text_classification_udf.py` & `exasol_transformers_extension-1.0.1/exasol_transformers_extension/udfs/models/zero_shot_text_classification_udf.py`

 * *Files identical despite different names*

### Comparing `exasol_transformers_extension-1.0.0/exasol_transformers_extension/upload_model.py` & `exasol_transformers_extension-1.0.1/exasol_transformers_extension/upload_model.py`

 * *Files identical despite different names*

### Comparing `exasol_transformers_extension-1.0.0/exasol_transformers_extension/utils/bucketfs_model_uploader.py` & `exasol_transformers_extension-1.0.1/exasol_transformers_extension/utils/bucketfs_model_uploader.py`

 * *Files identical despite different names*

### Comparing `exasol_transformers_extension-1.0.0/exasol_transformers_extension/utils/bucketfs_operations.py` & `exasol_transformers_extension-1.0.1/exasol_transformers_extension/utils/bucketfs_operations.py`

 * *Files identical despite different names*

### Comparing `exasol_transformers_extension-1.0.0/exasol_transformers_extension/utils/dataframe_operations.py` & `exasol_transformers_extension-1.0.1/exasol_transformers_extension/utils/dataframe_operations.py`

 * *Files identical despite different names*

### Comparing `exasol_transformers_extension-1.0.0/exasol_transformers_extension/utils/huggingface_hub_bucketfs_model_transfer_sp.py` & `exasol_transformers_extension-1.0.1/exasol_transformers_extension/utils/huggingface_hub_bucketfs_model_transfer_sp.py`

 * *Files identical despite different names*

### Comparing `exasol_transformers_extension-1.0.0/exasol_transformers_extension/utils/load_local_model.py` & `exasol_transformers_extension-1.0.1/exasol_transformers_extension/utils/load_local_model.py`

 * *Files identical despite different names*

### Comparing `exasol_transformers_extension-1.0.0/exasol_transformers_extension/utils/model_factory_protocol.py` & `exasol_transformers_extension-1.0.1/exasol_transformers_extension/utils/model_factory_protocol.py`

 * *Files identical despite different names*

### Comparing `exasol_transformers_extension-1.0.0/pyproject.toml` & `exasol_transformers_extension-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "exasol-transformers-extension"
-version = "1.0.0"
+version = "1.0.1"
 description = "An Exasol extension for using state-of-the-art pretrained machine learning models via the Hugging Face Transformers API."
 
 authors = [
     	"Umit Buyuksahin <umit.buyuksahin@exasol.com>",
     	"Torsten Kilias <torsten.kilias@exasol.com>"
 ]
```

### Comparing `exasol_transformers_extension-1.0.0/PKG-INFO` & `exasol_transformers_extension-1.0.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exasol-transformers-extension
-Version: 1.0.0
+Version: 1.0.1
 Summary: An Exasol extension for using state-of-the-art pretrained machine learning models via the Hugging Face Transformers API.
 Home-page: https://github.com/exasol/transformers-extension
 Keywords: exasol
 Author: Umit Buyuksahin
 Author-email: umit.buyuksahin@exasol.com
 Requires-Python: >=3.8.0,<4.0.0
 Classifier: Programming Language :: Python :: 3
```


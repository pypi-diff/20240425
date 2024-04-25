# Comparing `tmp/dominodatalab_data-5.9.0.tar.gz` & `tmp/dominodatalab_data-5.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dominodatalab_data-5.9.0.tar", max compression
+gzip compressed data, was "dominodatalab_data-5.9.1.tar", max compression
```

## Comparing `dominodatalab_data-5.9.0.tar` & `dominodatalab_data-5.9.1.tar`

### file list

```diff
@@ -1,116 +1,116 @@
--rw-r--r--   0        0        0    10891 2022-06-29 07:20:17.949426 dominodatalab_data-5.9.0/LICENSE
--rw-r--r--   0        0        0     5982 2022-06-29 07:20:17.949625 dominodatalab_data-5.9.0/README.md
--rw-r--r--   0        0        0      102 2023-06-29 21:29:35.211838 dominodatalab_data-5.9.0/datasource_api_client/__init__.py
--rw-r--r--   0        0        0       47 2023-06-29 21:29:35.266432 dominodatalab_data-5.9.0/datasource_api_client/api/__init__.py
--rw-r--r--   0        0        0        0 2023-06-29 21:29:35.296851 dominodatalab_data-5.9.0/datasource_api_client/api/datasource/__init__.py
--rw-r--r--   0        0        0     4162 2023-08-30 22:57:34.791278 dominodatalab_data-5.9.0/datasource_api_client/api/datasource/get_datasource_by_name.py
--rw-r--r--   0        0        0        0 2023-06-29 21:29:35.276733 dominodatalab_data-5.9.0/datasource_api_client/api/proxy/__init__.py
--rw-r--r--   0        0        0     3389 2023-08-30 22:57:34.791524 dominodatalab_data-5.9.0/datasource_api_client/api/proxy/get_key_url.py
--rw-r--r--   0        0        0     3442 2023-08-30 22:57:34.791754 dominodatalab_data-5.9.0/datasource_api_client/api/proxy/list_keys.py
--rw-r--r--   0        0        0     2212 2023-08-30 22:57:34.791976 dominodatalab_data-5.9.0/datasource_api_client/api/proxy/log_metric.py
--rw-r--r--   0        0        0     1822 2023-08-30 22:57:34.792298 dominodatalab_data-5.9.0/datasource_api_client/client.py
--rw-r--r--   0        0        0      695 2023-06-29 21:29:35.264784 dominodatalab_data-5.9.0/datasource_api_client/models/__init__.py
--rw-r--r--   0        0        0     1173 2023-06-29 21:29:37.289259 dominodatalab_data-5.9.0/datasource_api_client/models/datasource_config.py
--rw-r--r--   0        0        0     4708 2023-06-29 21:29:37.367598 dominodatalab_data-5.9.0/datasource_api_client/models/datasource_dto.py
--rw-r--r--   0        0        0     1199 2023-06-29 21:29:37.297293 dominodatalab_data-5.9.0/datasource_api_client/models/datasource_dto_added_by.py
--rw-r--r--   0        0        0      464 2023-11-08 22:50:25.371900 dominodatalab_data-5.9.0/datasource_api_client/models/datasource_dto_auth_type.py
--rw-r--r--   0        0        0     1252 2023-11-08 22:50:25.372406 dominodatalab_data-5.9.0/datasource_api_client/models/datasource_dto_data_source_type.py
--rw-r--r--   0        0        0      170 2023-06-29 21:29:36.323525 dominodatalab_data-5.9.0/datasource_api_client/models/datasource_dto_status.py
--rw-r--r--   0        0        0     1905 2023-06-29 21:29:37.336622 dominodatalab_data-5.9.0/datasource_api_client/models/datasource_owner_info.py
--rw-r--r--   0        0        0     1498 2023-06-29 21:29:37.329624 dominodatalab_data-5.9.0/datasource_api_client/models/error_response.py
--rw-r--r--   0        0        0     3569 2023-06-29 21:29:37.365222 dominodatalab_data-5.9.0/datasource_api_client/models/key_request.py
--rw-r--r--   0        0        0     3583 2023-08-30 22:57:34.793769 dominodatalab_data-5.9.0/datasource_api_client/models/list_request.py
--rw-r--r--   0        0        0      153 2023-06-29 21:29:36.330521 dominodatalab_data-5.9.0/datasource_api_client/models/log_metric_m.py
--rw-r--r--   0        0        0      293 2023-08-30 22:57:34.794546 dominodatalab_data-5.9.0/datasource_api_client/models/log_metric_t.py
--rw-r--r--   0        0        0     2084 2023-06-29 21:29:37.359491 dominodatalab_data-5.9.0/datasource_api_client/models/proxy_error_response.py
--rw-r--r--   0        0        0      939 2023-06-29 21:29:37.325116 dominodatalab_data-5.9.0/datasource_api_client/types.py
--rw-r--r--   0        0        0      369 2022-06-29 07:20:17.954805 dominodatalab_data-5.9.0/domino_data/__init__.py
--rw-r--r--   0        0        0        0 2023-01-23 19:50:12.481547 dominodatalab_data-5.9.0/domino_data/_feature_store/__init__.py
--rw-r--r--   0        0        0     3801 2023-06-27 20:05:53.688547 dominodatalab_data-5.9.0/domino_data/_feature_store/client.py
--rw-r--r--   0        0        0      684 2023-01-23 19:50:12.481937 dominodatalab_data-5.9.0/domino_data/_feature_store/exceptions.py
--rw-r--r--   0        0        0     2966 2023-01-23 19:50:12.482093 dominodatalab_data-5.9.0/domino_data/_feature_store/git.py
--rw-r--r--   0        0        0      683 2023-01-23 19:50:12.482249 dominodatalab_data-5.9.0/domino_data/_feature_store/logging.py
--rw-r--r--   0        0        0     1223 2023-01-23 19:50:12.482394 dominodatalab_data-5.9.0/domino_data/_feature_store/run.py
--rw-r--r--   0        0        0     8180 2023-06-27 20:05:53.688988 dominodatalab_data-5.9.0/domino_data/_feature_store/sync.py
--rw-r--r--   0        0        0     4796 2023-11-08 22:50:25.372817 dominodatalab_data-5.9.0/domino_data/auth.py
--rw-r--r--   0        0        0    15311 2023-11-08 22:52:59.983400 dominodatalab_data-5.9.0/domino_data/configuration_gen.py
--rw-r--r--   0        0        0    28192 2023-11-08 22:50:25.373666 dominodatalab_data-5.9.0/domino_data/data_sources.py
--rw-r--r--   0        0        0      894 2022-06-29 07:20:17.955520 dominodatalab_data-5.9.0/domino_data/logging.py
--rw-r--r--   0        0        0     1185 2023-11-08 22:50:25.374058 dominodatalab_data-5.9.0/domino_data/meta.py
--rw-r--r--   0        0        0        0 2022-06-29 07:20:17.955572 dominodatalab_data-5.9.0/domino_data/py.typed
--rw-r--r--   0        0        0        0 2022-06-29 07:20:17.955731 dominodatalab_data-5.9.0/domino_data/training_sets/__init__.py
--rw-r--r--   0        0        0    13955 2023-01-23 19:50:12.484004 dominodatalab_data-5.9.0/domino_data/training_sets/client.py
--rw-r--r--   0        0        0     3588 2022-06-29 07:20:17.956087 dominodatalab_data-5.9.0/domino_data/training_sets/model.py
--rw-r--r--   0        0        0     2566 2023-08-25 17:37:29.336888 dominodatalab_data-5.9.0/domino_data/transfer.py
--rw-r--r--   0        0        0      104 2023-06-29 21:29:27.864249 dominodatalab_data-5.9.0/feature_store_api_client/__init__.py
--rw-r--r--   0        0        0       47 2023-06-29 21:29:27.944538 dominodatalab_data-5.9.0/feature_store_api_client/api/__init__.py
--rw-r--r--   0        0        0        0 2023-06-29 21:29:27.956539 dominodatalab_data-5.9.0/feature_store_api_client/api/default/__init__.py
--rw-r--r--   0        0        0     2657 2023-06-29 21:29:30.863669 dominodatalab_data-5.9.0/feature_store_api_client/api/default/get.py
--rw-r--r--   0        0        0     2861 2023-06-29 21:29:30.917481 dominodatalab_data-5.9.0/feature_store_api_client/api/default/get_feature_view_name_store.py
--rw-r--r--   0        0        0     3383 2023-06-29 21:29:30.928335 dominodatalab_data-5.9.0/feature_store_api_client/api/default/post.py
--rw-r--r--   0        0        0     1870 2023-06-29 21:29:30.884599 dominodatalab_data-5.9.0/feature_store_api_client/api/default/post_featureview.py
--rw-r--r--   0        0        0     3215 2023-06-29 21:29:30.938416 dominodatalab_data-5.9.0/feature_store_api_client/api/default/post_lock.py
--rw-r--r--   0        0        0     3144 2023-06-29 21:29:30.978383 dominodatalab_data-5.9.0/feature_store_api_client/api/default/post_unlock.py
--rw-r--r--   0        0        0     1822 2023-06-29 21:29:30.938423 dominodatalab_data-5.9.0/feature_store_api_client/client.py
--rw-r--r--   0        0        0     1443 2023-06-29 21:29:29.913179 dominodatalab_data-5.9.0/feature_store_api_client/models/__init__.py
--rw-r--r--   0        0        0     2002 2023-06-29 21:29:30.964169 dominodatalab_data-5.9.0/feature_store_api_client/models/auth_config.py
--rw-r--r--   0        0        0     1513 2023-06-29 21:29:30.935820 dominodatalab_data-5.9.0/feature_store_api_client/models/auth_config_fields.py
--rw-r--r--   0        0        0     1166 2023-06-29 21:29:30.938314 dominodatalab_data-5.9.0/feature_store_api_client/models/auth_config_meta.py
--rw-r--r--   0        0        0      170 2023-06-29 21:29:29.908881 dominodatalab_data-5.9.0/feature_store_api_client/models/auth_field_name.py
--rw-r--r--   0        0        0      197 2023-06-29 21:29:29.880517 dominodatalab_data-5.9.0/feature_store_api_client/models/auth_type.py
--rw-r--r--   0        0        0      668 2023-06-29 21:29:29.925664 dominodatalab_data-5.9.0/feature_store_api_client/models/config_field_name.py
--rw-r--r--   0        0        0     2987 2023-06-29 21:29:30.991475 dominodatalab_data-5.9.0/feature_store_api_client/models/create_feature_store_request.py
--rw-r--r--   0        0        0     1323 2023-06-29 21:29:30.950462 dominodatalab_data-5.9.0/feature_store_api_client/models/create_feature_store_request_offline_store_config.py
--rw-r--r--   0        0        0     1832 2023-06-29 21:29:30.987879 dominodatalab_data-5.9.0/feature_store_api_client/models/entity.py
--rw-r--r--   0        0        0     1721 2023-06-29 21:29:31.003904 dominodatalab_data-5.9.0/feature_store_api_client/models/feature.py
--rw-r--r--   0        0        0     3878 2023-06-29 21:29:31.032784 dominodatalab_data-5.9.0/feature_store_api_client/models/feature_store.py
--rw-r--r--   0        0        0     1252 2023-06-29 21:29:30.976834 dominodatalab_data-5.9.0/feature_store_api_client/models/feature_store_offline_store_config.py
--rw-r--r--   0        0        0      175 2023-06-29 21:29:29.946823 dominodatalab_data-5.9.0/feature_store_api_client/models/feature_store_sync_result.py
--rw-r--r--   0        0        0     1148 2023-06-29 21:29:30.983530 dominodatalab_data-5.9.0/feature_store_api_client/models/feature_tags.py
--rw-r--r--   0        0        0     3863 2023-06-29 21:29:31.073823 dominodatalab_data-5.9.0/feature_store_api_client/models/feature_view.py
--rw-r--r--   0        0        0     3261 2023-06-29 21:29:31.061282 dominodatalab_data-5.9.0/feature_store_api_client/models/feature_view_request.py
--rw-r--r--   0        0        0     1209 2023-06-29 21:29:31.015022 dominodatalab_data-5.9.0/feature_store_api_client/models/feature_view_request_tags.py
--rw-r--r--   0        0        0     1171 2023-06-29 21:29:31.032784 dominodatalab_data-5.9.0/feature_store_api_client/models/feature_view_tags.py
--rw-r--r--   0        0        0     2968 2023-06-29 21:29:31.071711 dominodatalab_data-5.9.0/feature_store_api_client/models/field.py
--rw-r--r--   0        0        0      340 2023-06-29 21:29:29.927746 dominodatalab_data-5.9.0/feature_store_api_client/models/git_provider_name.py
--rw-r--r--   0        0        0     2405 2023-06-29 21:29:31.081083 dominodatalab_data-5.9.0/feature_store_api_client/models/lock_feature_store_request.py
--rw-r--r--   0        0        0     1750 2023-06-29 21:29:31.052942 dominodatalab_data-5.9.0/feature_store_api_client/models/metadata.py
--rw-r--r--   0        0        0     2552 2023-06-29 21:29:31.075733 dominodatalab_data-5.9.0/feature_store_api_client/models/offline_store_config.py
--rw-r--r--   0        0        0     1556 2023-06-29 21:29:31.051179 dominodatalab_data-5.9.0/feature_store_api_client/models/offline_store_config_fields.py
--rw-r--r--   0        0        0      219 2023-06-29 21:29:29.941249 dominodatalab_data-5.9.0/feature_store_api_client/models/offline_store_type.py
--rw-r--r--   0        0        0     1895 2023-06-29 21:29:31.074544 dominodatalab_data-5.9.0/feature_store_api_client/models/unlock_feature_store_request.py
--rw-r--r--   0        0        0     2459 2023-06-29 21:29:31.096355 dominodatalab_data-5.9.0/feature_store_api_client/models/upsert_feature_views_request.py
--rw-r--r--   0        0        0      939 2023-06-29 21:29:31.073820 dominodatalab_data-5.9.0/feature_store_api_client/types.py
--rw-r--r--   0        0        0     3858 2023-11-08 23:22:30.245056 dominodatalab_data-5.9.0/pyproject.toml
--rw-r--r--   0        0        0      103 2022-06-29 07:20:17.966039 dominodatalab_data-5.9.0/training_set_api_client/__init__.py
--rw-r--r--   0        0        0       47 2022-06-29 07:20:17.966225 dominodatalab_data-5.9.0/training_set_api_client/api/__init__.py
--rw-r--r--   0        0        0        0 2022-06-29 07:20:17.966370 dominodatalab_data-5.9.0/training_set_api_client/api/default/__init__.py
--rw-r--r--   0        0        0     1441 2022-06-29 07:20:17.966572 dominodatalab_data-5.9.0/training_set_api_client/api/default/delete_training_set_name.py
--rw-r--r--   0        0        0     1576 2022-06-29 07:20:17.966725 dominodatalab_data-5.9.0/training_set_api_client/api/default/delete_training_set_name_number.py
--rw-r--r--   0        0        0     2242 2022-06-29 07:20:17.966887 dominodatalab_data-5.9.0/training_set_api_client/api/default/get_training_set_name.py
--rw-r--r--   0        0        0     2525 2022-06-29 07:20:17.967034 dominodatalab_data-5.9.0/training_set_api_client/api/default/get_training_set_name_number.py
--rw-r--r--   0        0        0     3679 2022-06-29 07:20:17.967232 dominodatalab_data-5.9.0/training_set_api_client/api/default/post_find.py
--rw-r--r--   0        0        0     2832 2022-06-29 07:20:17.967539 dominodatalab_data-5.9.0/training_set_api_client/api/default/post_training_set_name.py
--rw-r--r--   0        0        0     3801 2022-06-29 07:20:17.967802 dominodatalab_data-5.9.0/training_set_api_client/api/default/post_version_find.py
--rw-r--r--   0        0        0     2716 2022-06-29 07:20:17.967984 dominodatalab_data-5.9.0/training_set_api_client/api/default/put_training_set_name.py
--rw-r--r--   0        0        0     3049 2022-06-29 07:20:17.968160 dominodatalab_data-5.9.0/training_set_api_client/api/default/put_training_set_name_number.py
--rw-r--r--   0        0        0     1661 2022-06-29 07:20:17.968332 dominodatalab_data-5.9.0/training_set_api_client/client.py
--rw-r--r--   0        0        0     1139 2022-06-29 07:20:17.968552 dominodatalab_data-5.9.0/training_set_api_client/models/__init__.py
--rw-r--r--   0        0        0     3301 2022-06-29 07:20:17.968737 dominodatalab_data-5.9.0/training_set_api_client/models/create_training_set_version_request.py
--rw-r--r--   0        0        0     1280 2022-06-29 07:20:17.968910 dominodatalab_data-5.9.0/training_set_api_client/models/create_training_set_version_request_meta.py
--rw-r--r--   0        0        0     1995 2022-06-29 07:20:17.969076 dominodatalab_data-5.9.0/training_set_api_client/models/monitoring_meta.py
--rw-r--r--   0        0        0     2411 2022-06-29 07:20:17.969227 dominodatalab_data-5.9.0/training_set_api_client/models/training_set.py
--rw-r--r--   0        0        0     2010 2022-06-29 07:20:17.969360 dominodatalab_data-5.9.0/training_set_api_client/models/training_set_filter.py
--rw-r--r--   0        0        0     1204 2022-06-29 07:20:17.969488 dominodatalab_data-5.9.0/training_set_api_client/models/training_set_filter_meta.py
--rw-r--r--   0        0        0     1171 2022-06-29 07:20:17.969618 dominodatalab_data-5.9.0/training_set_api_client/models/training_set_meta.py
--rw-r--r--   0        0        0     4472 2022-06-29 07:20:17.969755 dominodatalab_data-5.9.0/training_set_api_client/models/training_set_version.py
--rw-r--r--   0        0        0     2545 2022-06-29 07:20:17.969887 dominodatalab_data-5.9.0/training_set_api_client/models/training_set_version_filter.py
--rw-r--r--   0        0        0     1242 2022-06-29 07:20:17.970000 dominodatalab_data-5.9.0/training_set_api_client/models/training_set_version_filter_meta.py
--rw-r--r--   0        0        0     1303 2022-06-29 07:20:17.970108 dominodatalab_data-5.9.0/training_set_api_client/models/training_set_version_filter_training_set_meta.py
--rw-r--r--   0        0        0     1209 2022-06-29 07:20:17.970228 dominodatalab_data-5.9.0/training_set_api_client/models/training_set_version_meta.py
--rw-r--r--   0        0        0     1844 2022-06-29 07:20:17.970347 dominodatalab_data-5.9.0/training_set_api_client/models/update_training_set_request.py
--rw-r--r--   0        0        0     1242 2022-06-29 07:20:17.970465 dominodatalab_data-5.9.0/training_set_api_client/models/update_training_set_request_meta.py
--rw-r--r--   0        0        0     3070 2022-06-29 07:20:17.970588 dominodatalab_data-5.9.0/training_set_api_client/models/update_training_set_version_request.py
--rw-r--r--   0        0        0     1280 2022-06-29 07:20:17.970719 dominodatalab_data-5.9.0/training_set_api_client/models/update_training_set_version_request_meta.py
--rw-r--r--   0        0        0      984 2022-06-29 07:20:17.970827 dominodatalab_data-5.9.0/training_set_api_client/types.py
--rw-r--r--   0        0        0     7361 1970-01-01 00:00:00.000000 dominodatalab_data-5.9.0/PKG-INFO
+-rw-r--r--   0        0        0    10891 2022-12-13 21:08:46.883572 dominodatalab_data-5.9.1/LICENSE
+-rw-r--r--   0        0        0     5982 2023-07-20 22:48:08.992771 dominodatalab_data-5.9.1/README.md
+-rw-r--r--   0        0        0      102 2024-01-10 20:22:26.275374 dominodatalab_data-5.9.1/datasource_api_client/__init__.py
+-rw-r--r--   0        0        0       47 2024-01-10 20:22:26.321294 dominodatalab_data-5.9.1/datasource_api_client/api/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-10 20:22:26.347420 dominodatalab_data-5.9.1/datasource_api_client/api/datasource/__init__.py
+-rw-r--r--   0        0        0     4162 2024-01-10 20:22:27.566352 dominodatalab_data-5.9.1/datasource_api_client/api/datasource/get_datasource_by_name.py
+-rw-r--r--   0        0        0        0 2024-01-10 20:22:26.330129 dominodatalab_data-5.9.1/datasource_api_client/api/proxy/__init__.py
+-rw-r--r--   0        0        0     3389 2024-01-10 20:22:27.556065 dominodatalab_data-5.9.1/datasource_api_client/api/proxy/get_key_url.py
+-rw-r--r--   0        0        0     3442 2024-01-10 20:22:27.562780 dominodatalab_data-5.9.1/datasource_api_client/api/proxy/list_keys.py
+-rw-r--r--   0        0        0     2212 2024-01-10 20:22:27.549204 dominodatalab_data-5.9.1/datasource_api_client/api/proxy/log_metric.py
+-rw-r--r--   0        0        0     1822 2024-01-10 20:22:27.549071 dominodatalab_data-5.9.1/datasource_api_client/client.py
+-rw-r--r--   0        0        0      695 2024-01-10 20:22:26.319612 dominodatalab_data-5.9.1/datasource_api_client/models/__init__.py
+-rw-r--r--   0        0        0     1173 2024-01-10 20:22:27.536289 dominodatalab_data-5.9.1/datasource_api_client/models/datasource_config.py
+-rw-r--r--   0        0        0     4708 2024-01-10 20:22:27.585533 dominodatalab_data-5.9.1/datasource_api_client/models/datasource_dto.py
+-rw-r--r--   0        0        0     1199 2024-01-10 20:22:27.538738 dominodatalab_data-5.9.1/datasource_api_client/models/datasource_dto_added_by.py
+-rw-r--r--   0        0        0      464 2024-01-19 21:58:13.037953 dominodatalab_data-5.9.1/datasource_api_client/models/datasource_dto_auth_type.py
+-rw-r--r--   0        0        0     1252 2024-01-10 20:22:26.969344 dominodatalab_data-5.9.1/datasource_api_client/models/datasource_dto_data_source_type.py
+-rw-r--r--   0        0        0      170 2024-01-10 20:22:26.970640 dominodatalab_data-5.9.1/datasource_api_client/models/datasource_dto_status.py
+-rw-r--r--   0        0        0     1905 2024-01-10 20:22:27.562455 dominodatalab_data-5.9.1/datasource_api_client/models/datasource_owner_info.py
+-rw-r--r--   0        0        0     1498 2024-01-10 20:22:27.563675 dominodatalab_data-5.9.1/datasource_api_client/models/error_response.py
+-rw-r--r--   0        0        0     3569 2024-01-10 20:22:27.597375 dominodatalab_data-5.9.1/datasource_api_client/models/key_request.py
+-rw-r--r--   0        0        0     3585 2024-01-19 23:06:39.461163 dominodatalab_data-5.9.1/datasource_api_client/models/list_request.py
+-rw-r--r--   0        0        0      153 2024-01-10 20:22:26.975120 dominodatalab_data-5.9.1/datasource_api_client/models/log_metric_m.py
+-rw-r--r--   0        0        0      293 2024-01-10 20:22:26.976793 dominodatalab_data-5.9.1/datasource_api_client/models/log_metric_t.py
+-rw-r--r--   0        0        0     2084 2024-01-10 20:22:27.596514 dominodatalab_data-5.9.1/datasource_api_client/models/proxy_error_response.py
+-rw-r--r--   0        0        0      939 2024-01-10 20:22:27.572579 dominodatalab_data-5.9.1/datasource_api_client/types.py
+-rw-r--r--   0        0        0      369 2022-12-13 21:08:46.893659 dominodatalab_data-5.9.1/domino_data/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-20 22:48:08.998268 dominodatalab_data-5.9.1/domino_data/_feature_store/__init__.py
+-rw-r--r--   0        0        0     3801 2024-01-10 19:23:35.110928 dominodatalab_data-5.9.1/domino_data/_feature_store/client.py
+-rw-r--r--   0        0        0      684 2023-07-20 22:48:08.999044 dominodatalab_data-5.9.1/domino_data/_feature_store/exceptions.py
+-rw-r--r--   0        0        0     2966 2023-07-20 22:48:08.999763 dominodatalab_data-5.9.1/domino_data/_feature_store/git.py
+-rw-r--r--   0        0        0      683 2023-07-20 22:48:09.000218 dominodatalab_data-5.9.1/domino_data/_feature_store/logging.py
+-rw-r--r--   0        0        0     1223 2023-07-20 22:48:09.000513 dominodatalab_data-5.9.1/domino_data/_feature_store/run.py
+-rw-r--r--   0        0        0     8180 2024-01-19 21:58:13.041549 dominodatalab_data-5.9.1/domino_data/_feature_store/sync.py
+-rw-r--r--   0        0        0     4796 2024-01-10 19:23:35.113110 dominodatalab_data-5.9.1/domino_data/auth.py
+-rw-r--r--   0        0        0    15311 2024-01-19 23:05:12.680196 dominodatalab_data-5.9.1/domino_data/configuration_gen.py
+-rw-r--r--   0        0        0    28192 2024-01-10 19:23:35.114850 dominodatalab_data-5.9.1/domino_data/data_sources.py
+-rw-r--r--   0        0        0      894 2023-01-04 19:29:57.409242 dominodatalab_data-5.9.1/domino_data/logging.py
+-rw-r--r--   0        0        0     1185 2024-01-10 19:23:35.115990 dominodatalab_data-5.9.1/domino_data/meta.py
+-rw-r--r--   0        0        0        0 2022-12-13 21:08:46.895616 dominodatalab_data-5.9.1/domino_data/py.typed
+-rw-r--r--   0        0        0        0 2022-12-13 21:08:46.895810 dominodatalab_data-5.9.1/domino_data/training_sets/__init__.py
+-rw-r--r--   0        0        0    13955 2023-07-20 22:48:09.003049 dominodatalab_data-5.9.1/domino_data/training_sets/client.py
+-rw-r--r--   0        0        0     3588 2022-12-13 21:08:46.896143 dominodatalab_data-5.9.1/domino_data/training_sets/model.py
+-rw-r--r--   0        0        0     2566 2024-01-10 19:23:35.116762 dominodatalab_data-5.9.1/domino_data/transfer.py
+-rw-r--r--   0        0        0      104 2023-07-20 22:48:09.003666 dominodatalab_data-5.9.1/feature_store_api_client/__init__.py
+-rw-r--r--   0        0        0       47 2023-07-20 22:48:09.003784 dominodatalab_data-5.9.1/feature_store_api_client/api/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-20 22:48:09.003861 dominodatalab_data-5.9.1/feature_store_api_client/api/default/__init__.py
+-rw-r--r--   0        0        0     2657 2023-07-20 22:48:09.003992 dominodatalab_data-5.9.1/feature_store_api_client/api/default/get.py
+-rw-r--r--   0        0        0     2861 2023-07-20 22:48:09.004103 dominodatalab_data-5.9.1/feature_store_api_client/api/default/get_feature_view_name_store.py
+-rw-r--r--   0        0        0     3383 2023-07-20 22:48:09.004198 dominodatalab_data-5.9.1/feature_store_api_client/api/default/post.py
+-rw-r--r--   0        0        0     1870 2023-07-20 22:48:09.004458 dominodatalab_data-5.9.1/feature_store_api_client/api/default/post_featureview.py
+-rw-r--r--   0        0        0     3215 2023-07-20 22:48:09.004596 dominodatalab_data-5.9.1/feature_store_api_client/api/default/post_lock.py
+-rw-r--r--   0        0        0     3144 2023-07-20 22:48:09.004720 dominodatalab_data-5.9.1/feature_store_api_client/api/default/post_unlock.py
+-rw-r--r--   0        0        0     1822 2023-07-20 22:48:09.004825 dominodatalab_data-5.9.1/feature_store_api_client/client.py
+-rw-r--r--   0        0        0     1443 2024-01-10 19:23:35.117989 dominodatalab_data-5.9.1/feature_store_api_client/models/__init__.py
+-rw-r--r--   0        0        0     2002 2023-07-20 22:48:09.005624 dominodatalab_data-5.9.1/feature_store_api_client/models/auth_config.py
+-rw-r--r--   0        0        0     1513 2023-07-20 22:48:09.005775 dominodatalab_data-5.9.1/feature_store_api_client/models/auth_config_fields.py
+-rw-r--r--   0        0        0     1166 2023-07-20 22:48:09.005907 dominodatalab_data-5.9.1/feature_store_api_client/models/auth_config_meta.py
+-rw-r--r--   0        0        0      170 2023-07-20 22:48:09.006010 dominodatalab_data-5.9.1/feature_store_api_client/models/auth_field_name.py
+-rw-r--r--   0        0        0      197 2023-07-20 22:48:09.006118 dominodatalab_data-5.9.1/feature_store_api_client/models/auth_type.py
+-rw-r--r--   0        0        0      668 2023-07-20 22:48:09.006253 dominodatalab_data-5.9.1/feature_store_api_client/models/config_field_name.py
+-rw-r--r--   0        0        0     2987 2023-07-20 22:48:09.006367 dominodatalab_data-5.9.1/feature_store_api_client/models/create_feature_store_request.py
+-rw-r--r--   0        0        0     1323 2023-07-20 22:48:09.006521 dominodatalab_data-5.9.1/feature_store_api_client/models/create_feature_store_request_offline_store_config.py
+-rw-r--r--   0        0        0     1832 2023-07-20 22:48:09.006662 dominodatalab_data-5.9.1/feature_store_api_client/models/entity.py
+-rw-r--r--   0        0        0     1721 2024-01-10 19:23:35.118739 dominodatalab_data-5.9.1/feature_store_api_client/models/feature.py
+-rw-r--r--   0        0        0     3878 2023-07-20 22:48:09.007262 dominodatalab_data-5.9.1/feature_store_api_client/models/feature_store.py
+-rw-r--r--   0        0        0     1252 2023-07-20 22:48:09.007374 dominodatalab_data-5.9.1/feature_store_api_client/models/feature_store_offline_store_config.py
+-rw-r--r--   0        0        0      175 2023-07-20 22:48:09.007477 dominodatalab_data-5.9.1/feature_store_api_client/models/feature_store_sync_result.py
+-rw-r--r--   0        0        0     1148 2024-01-10 19:23:35.119204 dominodatalab_data-5.9.1/feature_store_api_client/models/feature_tags.py
+-rw-r--r--   0        0        0     3863 2023-07-20 22:48:09.007951 dominodatalab_data-5.9.1/feature_store_api_client/models/feature_view.py
+-rw-r--r--   0        0        0     3261 2024-01-10 19:23:35.120678 dominodatalab_data-5.9.1/feature_store_api_client/models/feature_view_request.py
+-rw-r--r--   0        0        0     1209 2023-07-20 22:48:09.008486 dominodatalab_data-5.9.1/feature_store_api_client/models/feature_view_request_tags.py
+-rw-r--r--   0        0        0     1171 2023-07-20 22:48:09.008653 dominodatalab_data-5.9.1/feature_store_api_client/models/feature_view_tags.py
+-rw-r--r--   0        0        0     2968 2023-07-20 22:48:09.008787 dominodatalab_data-5.9.1/feature_store_api_client/models/field.py
+-rw-r--r--   0        0        0      340 2023-07-20 22:48:09.008914 dominodatalab_data-5.9.1/feature_store_api_client/models/git_provider_name.py
+-rw-r--r--   0        0        0     2405 2023-07-20 22:48:09.009041 dominodatalab_data-5.9.1/feature_store_api_client/models/lock_feature_store_request.py
+-rw-r--r--   0        0        0     1750 2023-07-20 22:48:09.009149 dominodatalab_data-5.9.1/feature_store_api_client/models/metadata.py
+-rw-r--r--   0        0        0     2552 2023-07-20 22:48:09.009252 dominodatalab_data-5.9.1/feature_store_api_client/models/offline_store_config.py
+-rw-r--r--   0        0        0     1556 2023-07-20 22:48:09.009349 dominodatalab_data-5.9.1/feature_store_api_client/models/offline_store_config_fields.py
+-rw-r--r--   0        0        0      219 2023-07-20 22:48:09.009470 dominodatalab_data-5.9.1/feature_store_api_client/models/offline_store_type.py
+-rw-r--r--   0        0        0     1895 2023-07-20 22:48:09.009577 dominodatalab_data-5.9.1/feature_store_api_client/models/unlock_feature_store_request.py
+-rw-r--r--   0        0        0     2459 2024-01-10 19:23:35.121243 dominodatalab_data-5.9.1/feature_store_api_client/models/upsert_feature_views_request.py
+-rw-r--r--   0        0        0      939 2023-07-20 22:48:09.009999 dominodatalab_data-5.9.1/feature_store_api_client/types.py
+-rw-r--r--   0        0        0     3858 2024-01-19 23:06:39.461769 dominodatalab_data-5.9.1/pyproject.toml
+-rw-r--r--   0        0        0      103 2022-12-13 21:08:46.910476 dominodatalab_data-5.9.1/training_set_api_client/__init__.py
+-rw-r--r--   0        0        0       47 2022-12-13 21:08:46.910619 dominodatalab_data-5.9.1/training_set_api_client/api/__init__.py
+-rw-r--r--   0        0        0        0 2022-12-13 21:08:46.910785 dominodatalab_data-5.9.1/training_set_api_client/api/default/__init__.py
+-rw-r--r--   0        0        0     1441 2022-12-13 21:08:46.910908 dominodatalab_data-5.9.1/training_set_api_client/api/default/delete_training_set_name.py
+-rw-r--r--   0        0        0     1576 2022-12-13 21:08:46.911013 dominodatalab_data-5.9.1/training_set_api_client/api/default/delete_training_set_name_number.py
+-rw-r--r--   0        0        0     2242 2022-12-13 21:08:46.911099 dominodatalab_data-5.9.1/training_set_api_client/api/default/get_training_set_name.py
+-rw-r--r--   0        0        0     2525 2022-12-13 21:08:46.911182 dominodatalab_data-5.9.1/training_set_api_client/api/default/get_training_set_name_number.py
+-rw-r--r--   0        0        0     3679 2022-12-13 21:08:46.911276 dominodatalab_data-5.9.1/training_set_api_client/api/default/post_find.py
+-rw-r--r--   0        0        0     2832 2022-12-13 21:08:46.911364 dominodatalab_data-5.9.1/training_set_api_client/api/default/post_training_set_name.py
+-rw-r--r--   0        0        0     3801 2022-12-13 21:08:46.911452 dominodatalab_data-5.9.1/training_set_api_client/api/default/post_version_find.py
+-rw-r--r--   0        0        0     2716 2022-12-13 21:08:46.911584 dominodatalab_data-5.9.1/training_set_api_client/api/default/put_training_set_name.py
+-rw-r--r--   0        0        0     3049 2022-12-13 21:08:46.911684 dominodatalab_data-5.9.1/training_set_api_client/api/default/put_training_set_name_number.py
+-rw-r--r--   0        0        0     1661 2022-12-13 21:08:46.911774 dominodatalab_data-5.9.1/training_set_api_client/client.py
+-rw-r--r--   0        0        0     1139 2022-12-13 21:08:46.911917 dominodatalab_data-5.9.1/training_set_api_client/models/__init__.py
+-rw-r--r--   0        0        0     3301 2022-12-13 21:08:46.912007 dominodatalab_data-5.9.1/training_set_api_client/models/create_training_set_version_request.py
+-rw-r--r--   0        0        0     1280 2022-12-13 21:08:46.912105 dominodatalab_data-5.9.1/training_set_api_client/models/create_training_set_version_request_meta.py
+-rw-r--r--   0        0        0     1995 2022-12-13 21:08:46.912303 dominodatalab_data-5.9.1/training_set_api_client/models/monitoring_meta.py
+-rw-r--r--   0        0        0     2411 2022-12-13 21:08:46.912407 dominodatalab_data-5.9.1/training_set_api_client/models/training_set.py
+-rw-r--r--   0        0        0     2010 2022-12-13 21:08:46.912513 dominodatalab_data-5.9.1/training_set_api_client/models/training_set_filter.py
+-rw-r--r--   0        0        0     1204 2022-12-13 21:08:46.912628 dominodatalab_data-5.9.1/training_set_api_client/models/training_set_filter_meta.py
+-rw-r--r--   0        0        0     1171 2022-12-13 21:08:46.912764 dominodatalab_data-5.9.1/training_set_api_client/models/training_set_meta.py
+-rw-r--r--   0        0        0     4472 2022-12-13 21:08:46.912863 dominodatalab_data-5.9.1/training_set_api_client/models/training_set_version.py
+-rw-r--r--   0        0        0     2545 2022-12-13 21:08:46.912963 dominodatalab_data-5.9.1/training_set_api_client/models/training_set_version_filter.py
+-rw-r--r--   0        0        0     1242 2022-12-13 21:08:46.913081 dominodatalab_data-5.9.1/training_set_api_client/models/training_set_version_filter_meta.py
+-rw-r--r--   0        0        0     1303 2022-12-13 21:08:46.913192 dominodatalab_data-5.9.1/training_set_api_client/models/training_set_version_filter_training_set_meta.py
+-rw-r--r--   0        0        0     1209 2022-12-13 21:08:46.913297 dominodatalab_data-5.9.1/training_set_api_client/models/training_set_version_meta.py
+-rw-r--r--   0        0        0     1844 2022-12-13 21:08:46.913396 dominodatalab_data-5.9.1/training_set_api_client/models/update_training_set_request.py
+-rw-r--r--   0        0        0     1242 2022-12-13 21:08:46.913504 dominodatalab_data-5.9.1/training_set_api_client/models/update_training_set_request_meta.py
+-rw-r--r--   0        0        0     3070 2022-12-13 21:08:46.913600 dominodatalab_data-5.9.1/training_set_api_client/models/update_training_set_version_request.py
+-rw-r--r--   0        0        0     1280 2022-12-13 21:08:46.913689 dominodatalab_data-5.9.1/training_set_api_client/models/update_training_set_version_request_meta.py
+-rw-r--r--   0        0        0      984 2022-12-13 21:08:46.913773 dominodatalab_data-5.9.1/training_set_api_client/types.py
+-rw-r--r--   0        0        0     7412 1970-01-01 00:00:00.000000 dominodatalab_data-5.9.1/PKG-INFO
```

### Comparing `dominodatalab_data-5.9.0/LICENSE` & `dominodatalab_data-5.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.9.0/README.md` & `dominodatalab_data-5.9.1/README.md`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.9.0/datasource_api_client/api/datasource/get_datasource_by_name.py` & `dominodatalab_data-5.9.1/datasource_api_client/api/datasource/get_datasource_by_name.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.9.0/datasource_api_client/api/proxy/get_key_url.py` & `dominodatalab_data-5.9.1/datasource_api_client/api/proxy/get_key_url.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.9.0/datasource_api_client/api/proxy/list_keys.py` & `dominodatalab_data-5.9.1/datasource_api_client/api/proxy/list_keys.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.9.0/datasource_api_client/api/proxy/log_metric.py` & `dominodatalab_data-5.9.1/datasource_api_client/api/proxy/log_metric.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.9.0/datasource_api_client/client.py` & `dominodatalab_data-5.9.1/datasource_api_client/client.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.9.0/datasource_api_client/models/__init__.py` & `dominodatalab_data-5.9.1/datasource_api_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.9.0/datasource_api_client/models/datasource_config.py` & `dominodatalab_data-5.9.1/datasource_api_client/models/datasource_config.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.9.0/datasource_api_client/models/datasource_dto.py` & `dominodatalab_data-5.9.1/datasource_api_client/models/datasource_dto.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.9.0/datasource_api_client/models/datasource_dto_added_by.py` & `dominodatalab_data-5.9.1/datasource_api_client/models/datasource_dto_added_by.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.9.0/datasource_api_client/models/datasource_dto_data_source_type.py` & `dominodatalab_data-5.9.1/datasource_api_client/models/datasource_dto_data_source_type.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.9.0/datasource_api_client/models/datasource_owner_info.py` & `dominodatalab_data-5.9.1/datasource_api_client/models/datasource_owner_info.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.9.0/datasource_api_client/models/error_response.py` & `dominodatalab_data-5.9.1/datasource_api_client/models/error_response.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.9.0/datasource_api_client/models/key_request.py` & `dominodatalab_data-5.9.1/datasource_api_client/models/key_request.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.9.0/datasource_api_client/models/list_request.py` & `dominodatalab_data-5.9.1/datasource_api_client/models/list_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
             }
         )
         if config_overwrites is not UNSET:
             field_dict["configOverwrites"] = config_overwrites
         if credential_overwrites is not UNSET:
             field_dict["credentialOverwrites"] = credential_overwrites
         if page_size is not UNSET:
-            field_dict["pageSize"] = page_size
+            field_dict["page_size"] = page_size
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         datasource_id = d.pop("datasourceId")
@@ -73,15 +73,15 @@
         _credential_overwrites = d.pop("credentialOverwrites", UNSET)
         credential_overwrites: Union[Unset, DatasourceConfig]
         if isinstance(_credential_overwrites, Unset):
             credential_overwrites = UNSET
         else:
             credential_overwrites = DatasourceConfig.from_dict(_credential_overwrites)
 
-        page_size = d.pop("pageSize", UNSET)
+        page_size = d.pop("page_size", UNSET)
 
         list_request = cls(
             datasource_id=datasource_id,
             prefix=prefix,
             config_overwrites=config_overwrites,
             credential_overwrites=credential_overwrites,
             page_size=page_size,
```

### Comparing `dominodatalab_data-5.9.0/datasource_api_client/models/proxy_error_response.py` & `dominodatalab_data-5.9.1/datasource_api_client/models/proxy_error_response.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.9.0/datasource_api_client/types.py` & `dominodatalab_data-5.9.1/datasource_api_client/types.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.9.0/domino_data/_feature_store/client.py` & `dominodatalab_data-5.9.1/domino_data/_feature_store/client.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.9.0/domino_data/_feature_store/exceptions.py` & `dominodatalab_data-5.9.1/domino_data/_feature_store/exceptions.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.9.0/domino_data/_feature_store/git.py` & `dominodatalab_data-5.9.1/domino_data/_feature_store/git.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.9.0/domino_data/_feature_store/logging.py` & `dominodatalab_data-5.9.1/domino_data/_feature_store/logging.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.9.0/domino_data/_feature_store/run.py` & `dominodatalab_data-5.9.1/domino_data/_feature_store/run.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.9.0/domino_data/_feature_store/sync.py` & `dominodatalab_data-5.9.1/domino_data/_feature_store/sync.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.9.0/domino_data/auth.py` & `dominodatalab_data-5.9.1/domino_data/auth.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.9.0/domino_data/configuration_gen.py` & `dominodatalab_data-5.9.1/domino_data/configuration_gen.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.9.0/domino_data/data_sources.py` & `dominodatalab_data-5.9.1/domino_data/data_sources.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.9.0/domino_data/logging.py` & `dominodatalab_data-5.9.1/domino_data/logging.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.9.0/domino_data/meta.py` & `dominodatalab_data-5.9.1/domino_data/meta.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.9.0/domino_data/training_sets/client.py` & `dominodatalab_data-5.9.1/domino_data/training_sets/client.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.9.0/domino_data/training_sets/model.py` & `dominodatalab_data-5.9.1/domino_data/training_sets/model.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.9.0/domino_data/transfer.py` & `dominodatalab_data-5.9.1/domino_data/transfer.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.9.0/feature_store_api_client/api/default/get.py` & `dominodatalab_data-5.9.1/feature_store_api_client/api/default/get.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.9.0/feature_store_api_client/api/default/get_feature_view_name_store.py` & `dominodatalab_data-5.9.1/feature_store_api_client/api/default/get_feature_view_name_store.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.9.0/feature_store_api_client/api/default/post.py` & `dominodatalab_data-5.9.1/feature_store_api_client/api/default/post.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.9.0/feature_store_api_client/api/default/post_featureview.py` & `dominodatalab_data-5.9.1/feature_store_api_client/api/default/post_featureview.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.9.0/feature_store_api_client/api/default/post_lock.py` & `dominodatalab_data-5.9.1/feature_store_api_client/api/default/post_lock.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.9.0/feature_store_api_client/api/default/post_unlock.py` & `dominodatalab_data-5.9.1/feature_store_api_client/api/default/post_unlock.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.9.0/feature_store_api_client/client.py` & `dominodatalab_data-5.9.1/feature_store_api_client/client.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.9.0/feature_store_api_client/models/__init__.py` & `dominodatalab_data-5.9.1/feature_store_api_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.9.0/feature_store_api_client/models/auth_config.py` & `dominodatalab_data-5.9.1/feature_store_api_client/models/auth_config.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.9.0/feature_store_api_client/models/auth_config_fields.py` & `dominodatalab_data-5.9.1/feature_store_api_client/models/auth_config_fields.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.9.0/feature_store_api_client/models/auth_config_meta.py` & `dominodatalab_data-5.9.1/feature_store_api_client/models/auth_config_meta.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.9.0/feature_store_api_client/models/config_field_name.py` & `dominodatalab_data-5.9.1/feature_store_api_client/models/config_field_name.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.9.0/feature_store_api_client/models/create_feature_store_request.py` & `dominodatalab_data-5.9.1/feature_store_api_client/models/create_feature_store_request.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.9.0/feature_store_api_client/models/create_feature_store_request_offline_store_config.py` & `dominodatalab_data-5.9.1/feature_store_api_client/models/create_feature_store_request_offline_store_config.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.9.0/feature_store_api_client/models/entity.py` & `dominodatalab_data-5.9.1/feature_store_api_client/models/entity.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.9.0/feature_store_api_client/models/feature.py` & `dominodatalab_data-5.9.1/feature_store_api_client/models/feature.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.9.0/feature_store_api_client/models/feature_store.py` & `dominodatalab_data-5.9.1/feature_store_api_client/models/feature_store.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.9.0/feature_store_api_client/models/feature_store_offline_store_config.py` & `dominodatalab_data-5.9.1/feature_store_api_client/models/feature_store_offline_store_config.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.9.0/feature_store_api_client/models/feature_tags.py` & `dominodatalab_data-5.9.1/feature_store_api_client/models/feature_tags.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.9.0/feature_store_api_client/models/feature_view.py` & `dominodatalab_data-5.9.1/feature_store_api_client/models/feature_view.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.9.0/feature_store_api_client/models/feature_view_request.py` & `dominodatalab_data-5.9.1/feature_store_api_client/models/feature_view_request.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.9.0/feature_store_api_client/models/feature_view_request_tags.py` & `dominodatalab_data-5.9.1/feature_store_api_client/models/feature_view_request_tags.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.9.0/feature_store_api_client/models/feature_view_tags.py` & `dominodatalab_data-5.9.1/feature_store_api_client/models/feature_view_tags.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.9.0/feature_store_api_client/models/field.py` & `dominodatalab_data-5.9.1/feature_store_api_client/models/field.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.9.0/feature_store_api_client/models/lock_feature_store_request.py` & `dominodatalab_data-5.9.1/feature_store_api_client/models/lock_feature_store_request.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.9.0/feature_store_api_client/models/metadata.py` & `dominodatalab_data-5.9.1/feature_store_api_client/models/metadata.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.9.0/feature_store_api_client/models/offline_store_config.py` & `dominodatalab_data-5.9.1/feature_store_api_client/models/offline_store_config.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.9.0/feature_store_api_client/models/offline_store_config_fields.py` & `dominodatalab_data-5.9.1/feature_store_api_client/models/offline_store_config_fields.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.9.0/feature_store_api_client/models/unlock_feature_store_request.py` & `dominodatalab_data-5.9.1/feature_store_api_client/models/unlock_feature_store_request.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.9.0/feature_store_api_client/models/upsert_feature_views_request.py` & `dominodatalab_data-5.9.1/feature_store_api_client/models/upsert_feature_views_request.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.9.0/feature_store_api_client/types.py` & `dominodatalab_data-5.9.1/feature_store_api_client/types.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.9.0/pyproject.toml` & `dominodatalab_data-5.9.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Poetry pyproject.toml: https://python-poetry.org/docs/pyproject/
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "dominodatalab-data"
-version = "5.9.0"
+version = "5.9.1"
 description = "Domino Data API for interacting with Domino Data features"
 readme = "README.md"
 authors = [
     "Gabriel Haim <gabriel.haim@dominodatalab.com>",
     "Aaron Read <aaron.read@dominodatalab.com>",
 ]
 license = "Apache Software License 2.0"
```

### Comparing `dominodatalab_data-5.9.0/training_set_api_client/api/default/delete_training_set_name.py` & `dominodatalab_data-5.9.1/training_set_api_client/api/default/delete_training_set_name.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.9.0/training_set_api_client/api/default/delete_training_set_name_number.py` & `dominodatalab_data-5.9.1/training_set_api_client/api/default/delete_training_set_name_number.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.9.0/training_set_api_client/api/default/get_training_set_name.py` & `dominodatalab_data-5.9.1/training_set_api_client/api/default/get_training_set_name.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.9.0/training_set_api_client/api/default/get_training_set_name_number.py` & `dominodatalab_data-5.9.1/training_set_api_client/api/default/get_training_set_name_number.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.9.0/training_set_api_client/api/default/post_find.py` & `dominodatalab_data-5.9.1/training_set_api_client/api/default/post_find.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.9.0/training_set_api_client/api/default/post_training_set_name.py` & `dominodatalab_data-5.9.1/training_set_api_client/api/default/post_training_set_name.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.9.0/training_set_api_client/api/default/post_version_find.py` & `dominodatalab_data-5.9.1/training_set_api_client/api/default/post_version_find.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.9.0/training_set_api_client/api/default/put_training_set_name.py` & `dominodatalab_data-5.9.1/training_set_api_client/api/default/put_training_set_name.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.9.0/training_set_api_client/api/default/put_training_set_name_number.py` & `dominodatalab_data-5.9.1/training_set_api_client/api/default/put_training_set_name_number.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.9.0/training_set_api_client/client.py` & `dominodatalab_data-5.9.1/training_set_api_client/client.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.9.0/training_set_api_client/models/__init__.py` & `dominodatalab_data-5.9.1/training_set_api_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.9.0/training_set_api_client/models/create_training_set_version_request.py` & `dominodatalab_data-5.9.1/training_set_api_client/models/create_training_set_version_request.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.9.0/training_set_api_client/models/create_training_set_version_request_meta.py` & `dominodatalab_data-5.9.1/training_set_api_client/models/create_training_set_version_request_meta.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.9.0/training_set_api_client/models/monitoring_meta.py` & `dominodatalab_data-5.9.1/training_set_api_client/models/monitoring_meta.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.9.0/training_set_api_client/models/training_set.py` & `dominodatalab_data-5.9.1/training_set_api_client/models/training_set.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.9.0/training_set_api_client/models/training_set_filter.py` & `dominodatalab_data-5.9.1/training_set_api_client/models/training_set_filter.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.9.0/training_set_api_client/models/training_set_filter_meta.py` & `dominodatalab_data-5.9.1/training_set_api_client/models/training_set_filter_meta.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.9.0/training_set_api_client/models/training_set_meta.py` & `dominodatalab_data-5.9.1/training_set_api_client/models/training_set_meta.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.9.0/training_set_api_client/models/training_set_version.py` & `dominodatalab_data-5.9.1/training_set_api_client/models/training_set_version.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.9.0/training_set_api_client/models/training_set_version_filter.py` & `dominodatalab_data-5.9.1/training_set_api_client/models/training_set_version_filter.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.9.0/training_set_api_client/models/training_set_version_filter_meta.py` & `dominodatalab_data-5.9.1/training_set_api_client/models/training_set_version_filter_meta.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.9.0/training_set_api_client/models/training_set_version_filter_training_set_meta.py` & `dominodatalab_data-5.9.1/training_set_api_client/models/training_set_version_filter_training_set_meta.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.9.0/training_set_api_client/models/training_set_version_meta.py` & `dominodatalab_data-5.9.1/training_set_api_client/models/training_set_version_meta.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.9.0/training_set_api_client/models/update_training_set_request.py` & `dominodatalab_data-5.9.1/training_set_api_client/models/update_training_set_request.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.9.0/training_set_api_client/models/update_training_set_request_meta.py` & `dominodatalab_data-5.9.1/training_set_api_client/models/update_training_set_request_meta.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.9.0/training_set_api_client/models/update_training_set_version_request.py` & `dominodatalab_data-5.9.1/training_set_api_client/models/update_training_set_version_request.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.9.0/training_set_api_client/models/update_training_set_version_request_meta.py` & `dominodatalab_data-5.9.1/training_set_api_client/models/update_training_set_version_request_meta.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.9.0/training_set_api_client/types.py` & `dominodatalab_data-5.9.1/training_set_api_client/types.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.9.0/PKG-INFO` & `dominodatalab_data-5.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dominodatalab-data
-Version: 5.9.0
+Version: 5.9.1
 Summary: Domino Data API for interacting with Domino Data features
 Home-page: https://github.com/dominodatalab/domino-data
 License: Apache Software License 2.0
 Author: Gabriel Haim
 Author-email: gabriel.haim@dominodatalab.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -13,14 +13,15 @@
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: attrs (>=20.1.0,<22.0.0)
 Requires-Dist: backoff (>=1.11.1,<2.0.0)
 Requires-Dist: bson (>=0.5.10,<0.6.0)
 Requires-Dist: httpx (>=0.23.0,<0.24.0)
 Requires-Dist: loguru (>=0.5.3,<0.6.0)
 Requires-Dist: pandas (>=1.3.0,<2.0.0)
```


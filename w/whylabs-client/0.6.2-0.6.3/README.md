# Comparing `tmp/whylabs-client-0.6.2.tar.gz` & `tmp/whylabs-client-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whylabs-client-0.6.2.tar", last modified: Fri Apr  5 00:52:39 2024, max compression
+gzip compressed data, was "whylabs-client-0.6.3.tar", last modified: Thu Apr 25 11:53:36 2024, max compression
```

## Comparing `whylabs-client-0.6.2.tar` & `whylabs-client-0.6.3.tar`

### file list

```diff
@@ -1,189 +1,203 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 00:52:39.709554 whylabs-client-0.6.2/
--rw-r--r--   0 root         (0) root         (0)     3400 2024-04-05 00:52:39.709554 whylabs-client-0.6.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    30686 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/README.md
--rw-rw-rw-   0 root         (0) root         (0)       69 2024-04-05 00:52:39.711387 whylabs-client-0.6.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1269 2024-04-05 00:52:39.000000 whylabs-client-0.6.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 00:52:39.678388 whylabs-client-0.6.2/whylabs_client/
--rw-rw-rw-   0 root         (0) root         (0)      753 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 00:52:39.682971 whylabs-client-0.6.2/whylabs_client/api/
--rw-rw-rw-   0 root         (0) root         (0)      217 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/api/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11548 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/api/api_key_api.py
--rw-rw-rw-   0 root         (0) root         (0)    10305 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/api/assets_api.py
--rw-rw-rw-   0 root         (0) root         (0)    12003 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/api/data_api.py
--rw-rw-rw-   0 root         (0) root         (0)    15394 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/api/dataset_metadata_api.py
--rw-rw-rw-   0 root         (0) root         (0)    61561 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/api/dataset_profile_api.py
--rw-rw-rw-   0 root         (0) root         (0)     5992 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/api/debug_events_api.py
--rw-rw-rw-   0 root         (0) root         (0)    10632 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/api/feature_weights_api.py
--rw-rw-rw-   0 root         (0) root         (0)    17246 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/api/log_api.py
--rw-rw-rw-   0 root         (0) root         (0)    20538 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/api/membership_api.py
--rw-rw-rw-   0 root         (0) root         (0)    67193 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/api/models_api.py
--rw-rw-rw-   0 root         (0) root         (0)    56977 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/api/monitor_api.py
--rw-rw-rw-   0 root         (0) root         (0)    22628 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/api/monitor_diagnostics_api.py
--rw-rw-rw-   0 root         (0) root         (0)    56449 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/api/notification_settings_api.py
--rw-rw-rw-   0 root         (0) root         (0)     5648 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/api/policy_api.py
--rw-rw-rw-   0 root         (0) root         (0)     5237 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/api/schema_api.py
--rw-rw-rw-   0 root         (0) root         (0)    10030 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/api/security_api.py
--rw-rw-rw-   0 root         (0) root         (0)    35246 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/api/sessions_api.py
--rw-rw-rw-   0 root         (0) root         (0)     5676 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/api/traces_api.py
--rw-rw-rw-   0 root         (0) root         (0)    24390 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/api/transactions_api.py
--rw-rw-rw-   0 root         (0) root         (0)    37531 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/api_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 00:52:39.682971 whylabs-client-0.6.2/whylabs_client/apis/
--rw-rw-rw-   0 root         (0) root         (0)     1539 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/apis/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    17094 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/configuration.py
--rw-rw-rw-   0 root         (0) root         (0)     5075 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 00:52:39.709554 whylabs-client-0.6.2/whylabs_client/model/
--rw-rw-rw-   0 root         (0) root         (0)      348 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11362 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/account_organization.py
--rw-rw-rw-   0 root         (0) root         (0)    12505 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/account_user.py
--rw-rw-rw-   0 root         (0) root         (0)    11664 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/action_type.py
--rw-rw-rw-   0 root         (0) root         (0)    12221 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/activate_azure_subscription_request.py
--rw-rw-rw-   0 root         (0) root         (0)    11368 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/activate_azure_subscription_response.py
--rw-rw-rw-   0 root         (0) root         (0)    12110 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/add_membership_request.py
--rw-rw-rw-   0 root         (0) root         (0)    11326 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/add_policy_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11353 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/admin_report_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11315 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/admin_report_type.py
--rw-rw-rw-   0 root         (0) root         (0)    16926 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/analysis_results_record.py
--rw-rw-rw-   0 root         (0) root         (0)    14457 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/analysis_results_request.py
--rw-rw-rw-   0 root         (0) root         (0)    11398 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/analysis_results_response.py
--rw-rw-rw-   0 root         (0) root         (0)    13394 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/analyzer_diagnostic_record.py
--rw-rw-rw-   0 root         (0) root         (0)    13341 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/analyzer_failure_record.py
--rw-rw-rw-   0 root         (0) root         (0)    11735 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/analyzer_segment_column_diagnostic_record.py
--rw-rw-rw-   0 root         (0) root         (0)    12179 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/analyzer_segment_columns_diagnostic_request.py
--rw-rw-rw-   0 root         (0) root         (0)    11628 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/analyzer_segment_columns_diagnostic_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11892 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/analyzer_segment_diagnostic_record.py
--rw-rw-rw-   0 root         (0) root         (0)    11584 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/analyzer_segment_failure_record.py
--rw-rw-rw-   0 root         (0) root         (0)    11774 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/analyzer_segments_diagnostic_request.py
--rw-rw-rw-   0 root         (0) root         (0)    12144 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/analyzer_segments_diagnostic_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11487 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/analyzers_diagnostic_request.py
--rw-rw-rw-   0 root         (0) root         (0)    12045 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/analyzers_diagnostic_response.py
--rw-rw-rw-   0 root         (0) root         (0)    12419 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/async_log_response.py
--rw-rw-rw-   0 root         (0) root         (0)    13478 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/aws_marketplace_metadata.py
--rw-rw-rw-   0 root         (0) root         (0)    11837 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/azure_marketplace_contact_payload.py
--rw-rw-rw-   0 root         (0) root         (0)    13360 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/azure_marketplace_subscription_details.py
--rw-rw-rw-   0 root         (0) root         (0)    11420 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/batch_log_reference_request.py
--rw-rw-rw-   0 root         (0) root         (0)    11811 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/batch_log_session_reference_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11784 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/cache_key_type.py
--rw-rw-rw-   0 root         (0) root         (0)    12758 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/column_schema.py
--rw-rw-rw-   0 root         (0) root         (0)    11987 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/create_account_user_request.py
--rw-rw-rw-   0 root         (0) root         (0)    12589 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/create_dataset_profile_upload_response.py
--rw-rw-rw-   0 root         (0) root         (0)    12449 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/create_reference_profile_request.py
--rw-rw-rw-   0 root         (0) root         (0)    12773 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/create_reference_profile_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11118 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/create_session_request.py
--rw-rw-rw-   0 root         (0) root         (0)    11205 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/create_session_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11136 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/create_user_request.py
--rw-rw-rw-   0 root         (0) root         (0)    12492 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/debug_event.py
--rw-rw-rw-   0 root         (0) root         (0)    13384 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/delete_analyzer_result.py
--rw-rw-rw-   0 root         (0) root         (0)    11091 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/delete_analyzer_results_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11091 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/delete_dataset_profiles_response.py
--rw-rw-rw-   0 root         (0) root         (0)    13387 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/delete_profile.py
--rw-rw-rw-   0 root         (0) root         (0)    11748 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/deletion_status.py
--rw-rw-rw-   0 root         (0) root         (0)    11392 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/diagnostic_interval_request.py
--rw-rw-rw-   0 root         (0) root         (0)    12300 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/diagnostic_interval_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11106 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/email_notification_action.py
--rw-rw-rw-   0 root         (0) root         (0)    12349 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/entity_schema.py
--rw-rw-rw-   0 root         (0) root         (0)    12718 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/entity_search_result.py
--rw-rw-rw-   0 root         (0) root         (0)    12004 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/entity_weight_record.py
--rw-rw-rw-   0 root         (0) root         (0)    11561 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/entity_weight_record_metadata.py
--rw-rw-rw-   0 root         (0) root         (0)    11595 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/error_status.py
--rw-rw-rw-   0 root         (0) root         (0)    11465 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/export_trace_partial_success.py
--rw-rw-rw-   0 root         (0) root         (0)    11409 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/export_trace_service_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11225 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/feature_flags.py
--rw-rw-rw-   0 root         (0) root         (0)    11587 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/get_account_memberships_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11593 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/get_asset_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11222 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/get_dataset_metadata_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11283 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/get_default_membership_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11365 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/get_marketplace_metadata_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11446 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/get_memberships_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11417 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/get_notification_settings_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11727 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/get_profile_observatory_link_request.py
--rw-rw-rw-   0 root         (0) root         (0)    12038 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/get_profile_observatory_link_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11334 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/get_session_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11733 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/granularity.py
--rw-rw-rw-   0 root         (0) root         (0)    11496 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/list_models_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11530 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/list_organization_memberships_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11382 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/list_user_api_keys.py
--rw-rw-rw-   0 root         (0) root         (0)    11903 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/log_async_request.py
--rw-rw-rw-   0 root         (0) root         (0)    11575 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/log_reference_request.py
--rw-rw-rw-   0 root         (0) root         (0)    12344 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/log_reference_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11807 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/log_response.py
--rw-rw-rw-   0 root         (0) root         (0)    12791 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/log_session_reference_response.py
--rw-rw-rw-   0 root         (0) root         (0)    12176 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/log_transaction_metadata.py
--rw-rw-rw-   0 root         (0) root         (0)    12015 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/marketplace_dimensions.py
--rw-rw-rw-   0 root         (0) root         (0)    11277 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/member.py
--rw-rw-rw-   0 root         (0) root         (0)    12029 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/membership.py
--rw-rw-rw-   0 root         (0) root         (0)    11852 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/membership_metadata.py
--rw-rw-rw-   0 root         (0) root         (0)    12260 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/metric_schema.py
--rw-rw-rw-   0 root         (0) root         (0)    11624 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/metric_timeseries_record.py
--rw-rw-rw-   0 root         (0) root         (0)    12398 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/metric_timeseries_request.py
--rw-rw-rw-   0 root         (0) root         (0)    11375 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/metric_timeseries_response.py
--rw-rw-rw-   0 root         (0) root         (0)    12785 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/model_metadata_response.py
--rw-rw-rw-   0 root         (0) root         (0)    12539 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/model_type.py
--rw-rw-rw-   0 root         (0) root         (0)    11629 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/monitor_config_version.py
--rw-rw-rw-   0 root         (0) root         (0)    13161 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/notification_action.py
--rw-rw-rw-   0 root         (0) root         (0)    14137 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/notification_action_payload.py
--rw-rw-rw-   0 root         (0) root         (0)    12120 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/notification_relationship_item.py
--rw-rw-rw-   0 root         (0) root         (0)    11242 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/notification_relationship_type.py
--rw-rw-rw-   0 root         (0) root         (0)    12258 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/notification_settings.py
--rw-rw-rw-   0 root         (0) root         (0)    11979 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/notification_settings_day.py
--rw-rw-rw-   0 root         (0) root         (0)    11751 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/notification_sqs_message_cadence.py
--rw-rw-rw-   0 root         (0) root         (0)    14677 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/organization_metadata.py
--rw-rw-rw-   0 root         (0) root         (0)    11771 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/organization_role_members.py
--rw-rw-rw-   0 root         (0) root         (0)    13324 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/organization_summary.py
--rw-rw-rw-   0 root         (0) root         (0)    11215 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/pager_duty_notification_action.py
--rw-rw-rw-   0 root         (0) root         (0)    11759 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/patch_account_memberships_request.py
--rw-rw-rw-   0 root         (0) root         (0)    11512 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/post_asset_request.py
--rw-rw-rw-   0 root         (0) root         (0)    11484 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/post_asset_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11630 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/profile_trace.py
--rw-rw-rw-   0 root         (0) root         (0)    11815 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/profile_traces_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11882 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/provision_new_aws_marketplace_user_response.py
--rw-rw-rw-   0 root         (0) root         (0)    12226 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/provision_new_marketplace_user_request.py
--rw-rw-rw-   0 root         (0) root         (0)    12422 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/provision_new_user_request.py
--rw-rw-rw-   0 root         (0) root         (0)    11574 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/provision_new_user_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11241 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/put_account_memberships_request.py
--rw-rw-rw-   0 root         (0) root         (0)    13077 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/reference_profile_item_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11317 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/remove_membership_request.py
--rw-rw-rw-   0 root         (0) root         (0)    11070 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/response.py
--rw-rw-rw-   0 root         (0) root         (0)    11163 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/revoke_user_session_request.py
--rw-rw-rw-   0 root         (0) root         (0)    11580 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/role.py
--rw-rw-rw-   0 root         (0) root         (0)    11725 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/schema_metadata.py
--rw-rw-rw-   0 root         (0) root         (0)    11513 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/search_index_request.py
--rw-rw-rw-   0 root         (0) root         (0)    11787 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/search_index_type.py
--rw-rw-rw-   0 root         (0) root         (0)    11590 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/search_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11239 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/segment.py
--rw-rw-rw-   0 root         (0) root         (0)    11741 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/segment_list_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11368 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/segment_tag.py
--rw-rw-rw-   0 root         (0) root         (0)    11563 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/segment_weight.py
--rw-rw-rw-   0 root         (0) root         (0)    11133 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/segments_list_request.py
--rw-rw-rw-   0 root         (0) root         (0)    12108 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/session_metadata.py
--rw-rw-rw-   0 root         (0) root         (0)    11350 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/set_default_membership_request.py
--rw-rw-rw-   0 root         (0) root         (0)    11193 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/slack_notification_action.py
--rw-rw-rw-   0 root         (0) root         (0)    11499 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/sort_order.py
--rw-rw-rw-   0 root         (0) root         (0)    11529 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/status_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11104 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/subscription_product_feature.py
--rw-rw-rw-   0 root         (0) root         (0)    11907 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/subscription_product_summary.py
--rw-rw-rw-   0 root         (0) root         (0)    13683 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/subscription_summary.py
--rw-rw-rw-   0 root         (0) root         (0)    11760 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/subscription_tier.py
--rw-rw-rw-   0 root         (0) root         (0)    11886 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/time_period.py
--rw-rw-rw-   0 root         (0) root         (0)    11107 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/transaction_commit_request.py
--rw-rw-rw-   0 root         (0) root         (0)    11921 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/transaction_log_request.py
--rw-rw-rw-   0 root         (0) root         (0)    11160 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/transaction_start_request.py
--rw-rw-rw-   0 root         (0) root         (0)    11118 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/transaction_status_response.py
--rw-rw-rw-   0 root         (0) root         (0)    12934 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/uber_notification_schedule.py
--rw-rw-rw-   0 root         (0) root         (0)    11706 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/update_account_user_request.py
--rw-rw-rw-   0 root         (0) root         (0)    11650 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/update_membership_request.py
--rw-rw-rw-   0 root         (0) root         (0)    11340 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/upload_asset_request.py
--rw-rw-rw-   0 root         (0) root         (0)    11580 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/upload_asset_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11747 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/user.py
--rw-rw-rw-   0 root         (0) root         (0)    14008 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/user_api_key.py
--rw-rw-rw-   0 root         (0) root         (0)    11220 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/user_api_key_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11153 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model/validate_user_session_response.py
--rw-rw-rw-   0 root         (0) root         (0)    81897 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/model_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 00:52:39.709554 whylabs-client-0.6.2/whylabs_client/models/
--rw-rw-rw-   0 root         (0) root         (0)    11886 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    14199 2024-04-05 00:52:30.000000 whylabs-client-0.6.2/whylabs_client/rest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 00:52:39.679304 whylabs-client-0.6.2/whylabs_client.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3400 2024-04-05 00:52:39.000000 whylabs-client-0.6.2/whylabs_client.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8202 2024-04-05 00:52:39.000000 whylabs-client-0.6.2/whylabs_client.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-05 00:52:39.000000 whylabs-client-0.6.2/whylabs_client.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       32 2024-04-05 00:52:39.000000 whylabs-client-0.6.2/whylabs_client.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2024-04-05 00:52:39.000000 whylabs-client-0.6.2/whylabs_client.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 11:53:36.850322 whylabs-client-0.6.3/
+-rw-r--r--   0 root         (0) root         (0)     3400 2024-04-25 11:53:36.850322 whylabs-client-0.6.3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    32711 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/README.md
+-rw-rw-rw-   0 root         (0) root         (0)       69 2024-04-25 11:53:36.850322 whylabs-client-0.6.3/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1269 2024-04-25 11:53:36.000000 whylabs-client-0.6.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 11:53:36.815488 whylabs-client-0.6.3/whylabs_client/
+-rw-rw-rw-   0 root         (0) root         (0)      753 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 11:53:36.820989 whylabs-client-0.6.3/whylabs_client/api/
+-rw-rw-rw-   0 root         (0) root         (0)      217 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/api/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11548 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/api/api_key_api.py
+-rw-rw-rw-   0 root         (0) root         (0)    10305 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/api/assets_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     5193 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/api/container_diagnostics_api.py
+-rw-rw-rw-   0 root         (0) root         (0)    12003 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/api/data_api.py
+-rw-rw-rw-   0 root         (0) root         (0)    15394 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/api/dataset_metadata_api.py
+-rw-rw-rw-   0 root         (0) root         (0)    61856 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/api/dataset_profile_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     5992 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/api/debug_events_api.py
+-rw-rw-rw-   0 root         (0) root         (0)    10632 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/api/feature_weights_api.py
+-rw-rw-rw-   0 root         (0) root         (0)    17246 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/api/log_api.py
+-rw-rw-rw-   0 root         (0) root         (0)    20538 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/api/membership_api.py
+-rw-rw-rw-   0 root         (0) root         (0)    77716 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/api/models_api.py
+-rw-rw-rw-   0 root         (0) root         (0)    56977 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/api/monitor_api.py
+-rw-rw-rw-   0 root         (0) root         (0)    37966 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/api/monitor_diagnostics_api.py
+-rw-rw-rw-   0 root         (0) root         (0)    56449 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/api/notification_settings_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     5648 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/api/policy_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     5237 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/api/schema_api.py
+-rw-rw-rw-   0 root         (0) root         (0)    10030 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/api/security_api.py
+-rw-rw-rw-   0 root         (0) root         (0)    35246 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/api/sessions_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     5676 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/api/traces_api.py
+-rw-rw-rw-   0 root         (0) root         (0)    24390 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/api/transactions_api.py
+-rw-rw-rw-   0 root         (0) root         (0)    37531 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/api_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 11:53:36.820989 whylabs-client-0.6.3/whylabs_client/apis/
+-rw-rw-rw-   0 root         (0) root         (0)     1620 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/apis/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    17094 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/configuration.py
+-rw-rw-rw-   0 root         (0) root         (0)     5075 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 11:53:36.849405 whylabs-client-0.6.3/whylabs_client/model/
+-rw-rw-rw-   0 root         (0) root         (0)      348 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11362 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/account_organization.py
+-rw-rw-rw-   0 root         (0) root         (0)    12505 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/account_user.py
+-rw-rw-rw-   0 root         (0) root         (0)    11664 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/action_type.py
+-rw-rw-rw-   0 root         (0) root         (0)    12221 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/activate_azure_subscription_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    11368 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/activate_azure_subscription_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    12110 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/add_membership_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    11326 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/add_policy_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11353 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/admin_report_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11315 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/admin_report_type.py
+-rw-rw-rw-   0 root         (0) root         (0)    16926 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/analysis_results_record.py
+-rw-rw-rw-   0 root         (0) root         (0)    14457 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/analysis_results_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    11398 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/analysis_results_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    12090 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/analysis_results_summary.py
+-rw-rw-rw-   0 root         (0) root         (0)    13394 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/analyzer_diagnostic_record.py
+-rw-rw-rw-   0 root         (0) root         (0)    13341 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/analyzer_failure_record.py
+-rw-rw-rw-   0 root         (0) root         (0)    11735 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/analyzer_segment_column_diagnostic_record.py
+-rw-rw-rw-   0 root         (0) root         (0)    12179 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/analyzer_segment_columns_diagnostic_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    11628 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/analyzer_segment_columns_diagnostic_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11892 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/analyzer_segment_diagnostic_record.py
+-rw-rw-rw-   0 root         (0) root         (0)    11584 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/analyzer_segment_failure_record.py
+-rw-rw-rw-   0 root         (0) root         (0)    11774 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/analyzer_segments_diagnostic_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    12144 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/analyzer_segments_diagnostic_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11487 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/analyzers_diagnostic_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    12045 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/analyzers_diagnostic_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    13069 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/anomaly_record.py
+-rw-rw-rw-   0 root         (0) root         (0)    11179 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/async_diagnosis_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    12003 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/async_diagnosis_result_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    12419 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/async_log_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    13478 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/aws_marketplace_metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)    11837 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/azure_marketplace_contact_payload.py
+-rw-rw-rw-   0 root         (0) root         (0)    13360 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/azure_marketplace_subscription_details.py
+-rw-rw-rw-   0 root         (0) root         (0)    11420 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/batch_log_reference_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    11811 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/batch_log_session_reference_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    12092 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/batches_summary.py
+-rw-rw-rw-   0 root         (0) root         (0)    11784 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/cache_key_type.py
+-rw-rw-rw-   0 root         (0) root         (0)    12758 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/column_schema.py
+-rw-rw-rw-   0 root         (0) root         (0)    11935 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/condition_record.py
+-rw-rw-rw-   0 root         (0) root         (0)    11987 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/create_account_user_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    12589 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/create_dataset_profile_upload_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    12449 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/create_reference_profile_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    12773 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/create_reference_profile_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11118 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/create_session_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    11205 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/create_session_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11136 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/create_user_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    12492 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/debug_event.py
+-rw-rw-rw-   0 root         (0) root         (0)    13384 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/delete_analyzer_result.py
+-rw-rw-rw-   0 root         (0) root         (0)    11091 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/delete_analyzer_results_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11091 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/delete_dataset_profiles_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    13632 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/delete_profile.py
+-rw-rw-rw-   0 root         (0) root         (0)    11748 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/deletion_status.py
+-rw-rw-rw-   0 root         (0) root         (0)    13688 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/diagnosis_report.py
+-rw-rw-rw-   0 root         (0) root         (0)    12255 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/diagnosis_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    11658 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/diagnosis_request_status.py
+-rw-rw-rw-   0 root         (0) root         (0)    13019 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/diagnostic_data_summary.py
+-rw-rw-rw-   0 root         (0) root         (0)    11392 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/diagnostic_interval_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    12300 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/diagnostic_interval_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11106 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/email_notification_action.py
+-rw-rw-rw-   0 root         (0) root         (0)    12349 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/entity_schema.py
+-rw-rw-rw-   0 root         (0) root         (0)    12004 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/entity_weight_record.py
+-rw-rw-rw-   0 root         (0) root         (0)    11561 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/entity_weight_record_metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)    11595 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/error_status.py
+-rw-rw-rw-   0 root         (0) root         (0)    11465 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/export_trace_partial_success.py
+-rw-rw-rw-   0 root         (0) root         (0)    11409 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/export_trace_service_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    12749 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/failure_record.py
+-rw-rw-rw-   0 root         (0) root         (0)    11225 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/feature_flags.py
+-rw-rw-rw-   0 root         (0) root         (0)    11587 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/get_account_memberships_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11593 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/get_asset_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11222 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/get_dataset_metadata_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11283 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/get_default_membership_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11365 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/get_marketplace_metadata_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11446 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/get_memberships_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11417 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/get_notification_settings_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11727 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/get_profile_observatory_link_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    12038 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/get_profile_observatory_link_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11334 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/get_session_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11733 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/granularity.py
+-rw-rw-rw-   0 root         (0) root         (0)    11496 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/list_models_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11530 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/list_organization_memberships_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11382 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/list_user_api_keys.py
+-rw-rw-rw-   0 root         (0) root         (0)    11903 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/log_async_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    11575 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/log_reference_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    12344 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/log_reference_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11807 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/log_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    12791 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/log_session_reference_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    12176 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/log_transaction_metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)    12015 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/marketplace_dimensions.py
+-rw-rw-rw-   0 root         (0) root         (0)    11277 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/member.py
+-rw-rw-rw-   0 root         (0) root         (0)    12029 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/membership.py
+-rw-rw-rw-   0 root         (0) root         (0)    11852 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/membership_metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)    12026 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/metric_schema.py
+-rw-rw-rw-   0 root         (0) root         (0)    12274 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/metric_schema_fields.py
+-rw-rw-rw-   0 root         (0) root         (0)    11624 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/metric_timeseries_record.py
+-rw-rw-rw-   0 root         (0) root         (0)    12398 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/metric_timeseries_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    11375 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/metric_timeseries_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    12785 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/model_metadata_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    12539 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/model_type.py
+-rw-rw-rw-   0 root         (0) root         (0)    11629 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/monitor_config_version.py
+-rw-rw-rw-   0 root         (0) root         (0)    11257 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/named_count.py
+-rw-rw-rw-   0 root         (0) root         (0)    12731 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/named_metric_schema.py
+-rw-rw-rw-   0 root         (0) root         (0)    13161 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/notification_action.py
+-rw-rw-rw-   0 root         (0) root         (0)    14137 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/notification_action_payload.py
+-rw-rw-rw-   0 root         (0) root         (0)    12120 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/notification_relationship_item.py
+-rw-rw-rw-   0 root         (0) root         (0)    11242 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/notification_relationship_type.py
+-rw-rw-rw-   0 root         (0) root         (0)    12258 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/notification_settings.py
+-rw-rw-rw-   0 root         (0) root         (0)    11979 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/notification_settings_day.py
+-rw-rw-rw-   0 root         (0) root         (0)    11751 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/notification_sqs_message_cadence.py
+-rw-rw-rw-   0 root         (0) root         (0)    14677 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/organization_metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)    11771 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/organization_role_members.py
+-rw-rw-rw-   0 root         (0) root         (0)    13324 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/organization_summary.py
+-rw-rw-rw-   0 root         (0) root         (0)    11215 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/pager_duty_notification_action.py
+-rw-rw-rw-   0 root         (0) root         (0)    11759 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/patch_account_memberships_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    11512 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/post_asset_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    11484 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/post_asset_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    12004 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/profile_summary.py
+-rw-rw-rw-   0 root         (0) root         (0)    11630 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/profile_trace.py
+-rw-rw-rw-   0 root         (0) root         (0)    11815 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/profile_traces_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11882 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/provision_new_aws_marketplace_user_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    12226 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/provision_new_marketplace_user_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    12422 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/provision_new_user_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    11574 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/provision_new_user_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11241 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/put_account_memberships_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    11598 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/quality_issue_record.py
+-rw-rw-rw-   0 root         (0) root         (0)    13077 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/reference_profile_item_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11317 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/remove_membership_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    11070 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11524 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/result_record.py
+-rw-rw-rw-   0 root         (0) root         (0)    11163 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/revoke_user_session_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    11580 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/role.py
+-rw-rw-rw-   0 root         (0) root         (0)    11725 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/schema_metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)    11239 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/segment.py
+-rw-rw-rw-   0 root         (0) root         (0)    11741 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/segment_list_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11368 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/segment_tag.py
+-rw-rw-rw-   0 root         (0) root         (0)    11563 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/segment_weight.py
+-rw-rw-rw-   0 root         (0) root         (0)    11133 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/segments_list_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    12108 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/session_metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)    11350 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/set_default_membership_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    11193 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/slack_notification_action.py
+-rw-rw-rw-   0 root         (0) root         (0)    11499 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/sort_order.py
+-rw-rw-rw-   0 root         (0) root         (0)    11529 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/status_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11104 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/subscription_product_feature.py
+-rw-rw-rw-   0 root         (0) root         (0)    11907 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/subscription_product_summary.py
+-rw-rw-rw-   0 root         (0) root         (0)    13683 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/subscription_summary.py
+-rw-rw-rw-   0 root         (0) root         (0)    11760 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/subscription_tier.py
+-rw-rw-rw-   0 root         (0) root         (0)    11886 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/time_period.py
+-rw-rw-rw-   0 root         (0) root         (0)    11107 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/transaction_commit_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    11921 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/transaction_log_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    11160 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/transaction_start_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    11118 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/transaction_status_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    12934 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/uber_notification_schedule.py
+-rw-rw-rw-   0 root         (0) root         (0)    11706 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/update_account_user_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    11650 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/update_membership_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    11340 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/upload_asset_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    11580 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/upload_asset_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11747 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/user.py
+-rw-rw-rw-   0 root         (0) root         (0)    14008 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/user_api_key.py
+-rw-rw-rw-   0 root         (0) root         (0)    11220 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/user_api_key_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11153 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model/validate_user_session_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    81897 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/model_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 11:53:36.849405 whylabs-client-0.6.3/whylabs_client/models/
+-rw-rw-rw-   0 root         (0) root         (0)    12810 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    14199 2024-04-25 11:53:29.000000 whylabs-client-0.6.3/whylabs_client/rest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 11:53:36.816405 whylabs-client-0.6.3/whylabs_client.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3400 2024-04-25 11:53:36.000000 whylabs-client-0.6.3/whylabs_client.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8819 2024-04-25 11:53:36.000000 whylabs-client-0.6.3/whylabs_client.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-25 11:53:36.000000 whylabs-client-0.6.3/whylabs_client.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       32 2024-04-25 11:53:36.000000 whylabs-client-0.6.3/whylabs_client.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2024-04-25 11:53:36.000000 whylabs-client-0.6.3/whylabs_client.egg-info/top_level.txt
```

### Comparing `whylabs-client-0.6.2/PKG-INFO` & `whylabs-client-0.6.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whylabs-client
-Version: 0.6.2
+Version: 0.6.3
 Summary: WhyLabs API client
 Home-page: UNKNOWN
 Author: WhyLabs
 Author-email: support@whylabs.ai
 License: Apache License 2.0
 Keywords: OpenAPI,OpenAPI-Generator,WhyLabs API client
 Platform: UNKNOWN
```

### Comparing `whylabs-client-0.6.2/README.md` & `whylabs-client-0.6.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # whylabs-client
 WhyLabs API that enables end-to-end AI observability
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 - API version: 0.1
-- Package version: 0.6.2
+- Package version: 0.6.3
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 For more information, please visit [https://whylabs.ai](https://whylabs.ai)
 
 ## Requirements.
 
 Python >= 3.6
 
@@ -96,14 +96,15 @@
 
 Class | Method | HTTP request | Description
 ------------ | ------------- | ------------- | -------------
 *ApiKeyApi* | [**create_api_key**](docs/ApiKeyApi.md#create_api_key) | **POST** /v0/organizations/{org_id}/api-key | Generate an API key for a user.
 *ApiKeyApi* | [**revoke_api_key**](docs/ApiKeyApi.md#revoke_api_key) | **DELETE** /v0/organizations/{org_id}/api-key | Revoke the given API Key, removing its ability to access WhyLabs systems
 *AssetsApi* | [**get_asset**](docs/AssetsApi.md#get_asset) | **GET** /v1/assets/{asset_id} | Endpoint to retrieve assets
 *AssetsApi* | [**upload_asset**](docs/AssetsApi.md#upload_asset) | **POST** /v1/assets/{asset_id}/upload | Endpoint to upload an asset
+*ContainerDiagnosticsApi* | [**send_diagnostics**](docs/ContainerDiagnosticsApi.md#send_diagnostics) | **POST** /v1/container-diagnostics | Send container diagnostics
 *DataApi* | [**analysis_results_data**](docs/DataApi.md#analysis_results_data) | **POST** /v0/organizations/{org_id}/dataset/{dataset_id}/data/analysis-results | Endpoint to query analysis results for a dataset
 *DataApi* | [**metric_timeseries_data**](docs/DataApi.md#metric_timeseries_data) | **POST** /v0/organizations/{org_id}/dataset/{dataset_id}/data/metric-timeseries | Endpoint to query a single metric timeseries for a dataset
 *DatasetProfileApi* | [**create_reference_profile**](docs/DatasetProfileApi.md#create_reference_profile) | **POST** /v0/organizations/{org_id}/dataset-profiles/models/{dataset_id}/reference-profile | Returns data needed to uploading the reference profile
 *DatasetProfileApi* | [**delete_analyzer_results**](docs/DatasetProfileApi.md#delete_analyzer_results) | **DELETE** /v0/organizations/{org_id}/dataset-profiles/models/{dataset_id}/analyzer-results | Deletes a set of analyzer results
 *DatasetProfileApi* | [**delete_dataset_profiles**](docs/DatasetProfileApi.md#delete_dataset_profiles) | **DELETE** /v0/organizations/{org_id}/dataset-profiles/models/{dataset_id} | Deletes a set of dataset profiles
 *DatasetProfileApi* | [**delete_reference_profile**](docs/DatasetProfileApi.md#delete_reference_profile) | **DELETE** /v0/organizations/{org_id}/dataset-profiles/models/{model_id}/reference-profiles/{reference_id} | Delete a single reference profile
 *DatasetProfileApi* | [**get_profile_traces**](docs/DatasetProfileApi.md#get_profile_traces) | **GET** /v0/organizations/{org_id}/dataset-profiles/models/{dataset_id}/trace/{trace_id} | Returns a list for profile traces matching a trace id
@@ -126,22 +127,24 @@
 *MembershipApi* | [**list_organization_memberships**](docs/MembershipApi.md#list_organization_memberships) | **GET** /v0/organizations/{org_id}/membership | List organization memberships
 *MembershipApi* | [**remove_organization_membership**](docs/MembershipApi.md#remove_organization_membership) | **DELETE** /v0/organizations/{org_id}/membership | Removes membership in a given org from a user, using the user&#39;s email address.
 *MembershipApi* | [**update_organization_membership**](docs/MembershipApi.md#update_organization_membership) | **PUT** /v0/organizations/{org_id}/membership | Updates the role in an membership
 *ModelsApi* | [**create_model**](docs/ModelsApi.md#create_model) | **POST** /v0/organizations/{org_id}/models | Create a model with a given name and a time period
 *ModelsApi* | [**deactivate_model**](docs/ModelsApi.md#deactivate_model) | **DELETE** /v0/organizations/{org_id}/models/{model_id} | Mark a model as inactive
 *ModelsApi* | [**delete_entity_schema**](docs/ModelsApi.md#delete_entity_schema) | **DELETE** /v0/organizations/{org_id}/models/{dataset_id}/schema | Delete the entity schema config for a given dataset.
 *ModelsApi* | [**delete_entity_schema_column**](docs/ModelsApi.md#delete_entity_schema_column) | **DELETE** /v0/organizations/{org_id}/models/{dataset_id}/schema/column/{column_id} | Delete the entity schema of a single column for a given dataset.
-*ModelsApi* | [**delete_entity_schema_metric**](docs/ModelsApi.md#delete_entity_schema_metric) | **DELETE** /v0/organizations/{org_id}/models/{dataset_id}/schema/metric/{metric_label} | Delete the schema of a single metric for a given dataset.
+*ModelsApi* | [**delete_entity_schema_metric**](docs/ModelsApi.md#delete_entity_schema_metric) | **DELETE** /v0/organizations/{org_id}/models/{dataset_id}/schema/metric/{metric_name} | Delete the schema of a single metric for a given dataset.
 *ModelsApi* | [**get_entity_schema**](docs/ModelsApi.md#get_entity_schema) | **GET** /v0/organizations/{org_id}/models/{dataset_id}/schema | Get the entity schema config for a given dataset.
 *ModelsApi* | [**get_entity_schema_column**](docs/ModelsApi.md#get_entity_schema_column) | **GET** /v0/organizations/{org_id}/models/{dataset_id}/schema/column/{column_id} | Get the entity schema of a single column for a given dataset.
 *ModelsApi* | [**get_model**](docs/ModelsApi.md#get_model) | **GET** /v0/organizations/{org_id}/models/{model_id} | Get a model metadata
+*ModelsApi* | [**get_named_metric_schemas**](docs/ModelsApi.md#get_named_metric_schemas) | **GET** /v0/organizations/{org_id}/models/{dataset_id}/schema/metrics | Get all of the named metrics for a given dataset.
 *ModelsApi* | [**list_models**](docs/ModelsApi.md#list_models) | **GET** /v0/organizations/{org_id}/models | Get a list of all of the model ids for an organization.
 *ModelsApi* | [**put_entity_schema**](docs/ModelsApi.md#put_entity_schema) | **PUT** /v0/organizations/{org_id}/models/{dataset_id}/schema | Save the entity schema config for a given dataset.
 *ModelsApi* | [**put_entity_schema_column**](docs/ModelsApi.md#put_entity_schema_column) | **PUT** /v0/organizations/{org_id}/models/{dataset_id}/schema/column/{column_id} | Save the entity schema of a single column for a given dataset.
 *ModelsApi* | [**put_entity_schema_metric**](docs/ModelsApi.md#put_entity_schema_metric) | **PUT** /v0/organizations/{org_id}/models/{dataset_id}/schema/metric | Save the schema of a single metric for a given dataset.
+*ModelsApi* | [**put_named_metric_schema**](docs/ModelsApi.md#put_named_metric_schema) | **PUT** /v0/organizations/{org_id}/models/{dataset_id}/schema/metric/{metric_name} | Save the schema of a single named metric for a given dataset.
 *ModelsApi* | [**update_model**](docs/ModelsApi.md#update_model) | **PUT** /v0/organizations/{org_id}/models/{model_id} | Update a model&#39;s metadata
 *MonitorApi* | [**delete_analyzer**](docs/MonitorApi.md#delete_analyzer) | **DELETE** /v0/organizations/{org_id}/models/{dataset_id}/monitor-config/analyzer/{analyzer_id} | Delete the analyzer config for a given dataset.
 *MonitorApi* | [**delete_monitor**](docs/MonitorApi.md#delete_monitor) | **DELETE** /v0/organizations/{org_id}/models/{dataset_id}/monitor-config/monitor/{monitor_id} | Delete the monitor for a given dataset.
 *MonitorApi* | [**get_analyzer**](docs/MonitorApi.md#get_analyzer) | **GET** /v0/organizations/{org_id}/models/{dataset_id}/monitor-config/analyzer/{analyzer_id} | Get the analyzer config for a given dataset.
 *MonitorApi* | [**get_monitor**](docs/MonitorApi.md#get_monitor) | **GET** /v0/organizations/{org_id}/models/{dataset_id}/monitor-config/monitor/{monitor_id} | Get the monitor config for a given dataset.
 *MonitorApi* | [**get_monitor_config_v3**](docs/MonitorApi.md#get_monitor_config_v3) | **GET** /v0/organizations/{org_id}/models/{dataset_id}/monitor-config/v3 | Get the monitor config document for a given dataset.
 *MonitorApi* | [**list_constraints**](docs/MonitorApi.md#list_constraints) | **GET** /v0/organizations/{org_id}/models/{dataset_id}/constraints | List the constraints for a given dataset.
@@ -149,14 +152,17 @@
 *MonitorApi* | [**put_analyzer**](docs/MonitorApi.md#put_analyzer) | **PUT** /v0/organizations/{org_id}/models/{dataset_id}/monitor-config/analyzer/{analyzer_id} | Save the analyzer config for a given dataset.
 *MonitorApi* | [**put_monitor**](docs/MonitorApi.md#put_monitor) | **PUT** /v0/organizations/{org_id}/models/{dataset_id}/monitor-config/monitor/{monitor_id} | Save the monitor for a given dataset.
 *MonitorApi* | [**put_monitor_config_v3**](docs/MonitorApi.md#put_monitor_config_v3) | **PUT** /v0/organizations/{org_id}/models/{dataset_id}/monitor-config/v3 | Save the monitor config document for a given dataset.
 *MonitorApi* | [**validate_monitor_config_v3**](docs/MonitorApi.md#validate_monitor_config_v3) | **PUT** /v0/organizations/{org_id}/models/{dataset_id}/monitor-config/v3/validate | Validate the monitor config document for a given dataset.
 *MonitorDiagnosticsApi* | [**detect_noisy_analyzers**](docs/MonitorDiagnosticsApi.md#detect_noisy_analyzers) | **POST** /v0/organizations/{org_id}/diagnostics/monitor/analyzers | Endpoint to detect noisy or failing analyzers
 *MonitorDiagnosticsApi* | [**detect_noisy_columns**](docs/MonitorDiagnosticsApi.md#detect_noisy_columns) | **POST** /v0/organizations/{org_id}/diagnostics/monitor/analyzer/segment/columns | Endpoint to detect the noisiest columns for a specific analyzer and segment
 *MonitorDiagnosticsApi* | [**detect_noisy_segments**](docs/MonitorDiagnosticsApi.md#detect_noisy_segments) | **POST** /v0/organizations/{org_id}/diagnostics/monitor/analyzer/segments | Endpoint to detect the noisiest segments for a specific analyzer
+*MonitorDiagnosticsApi* | [**diagnose_analyzer_async**](docs/MonitorDiagnosticsApi.md#diagnose_analyzer_async) | **POST** /v0/organizations/{org_id}/diagnostics/monitor/diagnose/analyzer/async | Endpoint to request a diagnosis for a specific analyzer
+*MonitorDiagnosticsApi* | [**diagnose_analyzer_async_result**](docs/MonitorDiagnosticsApi.md#diagnose_analyzer_async_result) | **GET** /v0/organizations/{org_id}/diagnostics/monitor/diagnose/analyzer/async/result | Endpoint to request the result of an async diagnosis
+*MonitorDiagnosticsApi* | [**diagnose_analyzer_sync**](docs/MonitorDiagnosticsApi.md#diagnose_analyzer_sync) | **POST** /v0/organizations/{org_id}/diagnostics/monitor/diagnose/analyzer/sync | Endpoint to diagnose a specific analyzer
 *MonitorDiagnosticsApi* | [**recommend_diagnostic_interval**](docs/MonitorDiagnosticsApi.md#recommend_diagnostic_interval) | **POST** /v0/organizations/{org_id}/diagnostics/monitor/interval | Endpoint to recommend a diagnostic interval
 *NotificationSettingsApi* | [**add_notification_action**](docs/NotificationSettingsApi.md#add_notification_action) | **POST** /v0/notification-settings/{org_id}/actions/{type}/{action_id} | Add new notification action
 *NotificationSettingsApi* | [**delete_notification_action**](docs/NotificationSettingsApi.md#delete_notification_action) | **DELETE** /v0/notification-settings/{org_id}/actions/{action_id} | Delete notification action
 *NotificationSettingsApi* | [**disable_notification_action**](docs/NotificationSettingsApi.md#disable_notification_action) | **PUT** /v0/notification-settings/{org_id}/actions/{action_id}/disable | Disable notification action
 *NotificationSettingsApi* | [**enable_notification_action**](docs/NotificationSettingsApi.md#enable_notification_action) | **PUT** /v0/notification-settings/{org_id}/actions/{action_id}/enable | Enable notification action
 *NotificationSettingsApi* | [**get_email_notification_action_payload**](docs/NotificationSettingsApi.md#get_email_notification_action_payload) | **GET** /v0/notification-settings/actions/email/payload | Get dummy notification action payload
 *NotificationSettingsApi* | [**get_notification_action**](docs/NotificationSettingsApi.md#get_notification_action) | **GET** /v0/notification-settings/{org_id}/actions/{action_id} | Get notification action for id
@@ -196,55 +202,65 @@
  - [AddMembershipRequest](docs/AddMembershipRequest.md)
  - [AddPolicyResponse](docs/AddPolicyResponse.md)
  - [AdminReportResponse](docs/AdminReportResponse.md)
  - [AdminReportType](docs/AdminReportType.md)
  - [AnalysisResultsRecord](docs/AnalysisResultsRecord.md)
  - [AnalysisResultsRequest](docs/AnalysisResultsRequest.md)
  - [AnalysisResultsResponse](docs/AnalysisResultsResponse.md)
+ - [AnalysisResultsSummary](docs/AnalysisResultsSummary.md)
  - [AnalyzerDiagnosticRecord](docs/AnalyzerDiagnosticRecord.md)
  - [AnalyzerFailureRecord](docs/AnalyzerFailureRecord.md)
  - [AnalyzerSegmentColumnDiagnosticRecord](docs/AnalyzerSegmentColumnDiagnosticRecord.md)
  - [AnalyzerSegmentColumnsDiagnosticRequest](docs/AnalyzerSegmentColumnsDiagnosticRequest.md)
  - [AnalyzerSegmentColumnsDiagnosticResponse](docs/AnalyzerSegmentColumnsDiagnosticResponse.md)
  - [AnalyzerSegmentDiagnosticRecord](docs/AnalyzerSegmentDiagnosticRecord.md)
  - [AnalyzerSegmentFailureRecord](docs/AnalyzerSegmentFailureRecord.md)
  - [AnalyzerSegmentsDiagnosticRequest](docs/AnalyzerSegmentsDiagnosticRequest.md)
  - [AnalyzerSegmentsDiagnosticResponse](docs/AnalyzerSegmentsDiagnosticResponse.md)
  - [AnalyzersDiagnosticRequest](docs/AnalyzersDiagnosticRequest.md)
  - [AnalyzersDiagnosticResponse](docs/AnalyzersDiagnosticResponse.md)
+ - [AnomalyRecord](docs/AnomalyRecord.md)
+ - [AsyncDiagnosisResponse](docs/AsyncDiagnosisResponse.md)
+ - [AsyncDiagnosisResultResponse](docs/AsyncDiagnosisResultResponse.md)
  - [AsyncLogResponse](docs/AsyncLogResponse.md)
  - [AzureMarketplaceContactPayload](docs/AzureMarketplaceContactPayload.md)
  - [AzureMarketplaceSubscriptionDetails](docs/AzureMarketplaceSubscriptionDetails.md)
  - [BatchLogReferenceRequest](docs/BatchLogReferenceRequest.md)
  - [BatchLogSessionReferenceResponse](docs/BatchLogSessionReferenceResponse.md)
+ - [BatchesSummary](docs/BatchesSummary.md)
  - [CacheKeyType](docs/CacheKeyType.md)
  - [ColumnSchema](docs/ColumnSchema.md)
+ - [ConditionRecord](docs/ConditionRecord.md)
  - [CreateAccountUserRequest](docs/CreateAccountUserRequest.md)
  - [CreateDatasetProfileUploadResponse](docs/CreateDatasetProfileUploadResponse.md)
  - [CreateReferenceProfileRequest](docs/CreateReferenceProfileRequest.md)
  - [CreateReferenceProfileResponse](docs/CreateReferenceProfileResponse.md)
  - [CreateSessionRequest](docs/CreateSessionRequest.md)
  - [CreateSessionResponse](docs/CreateSessionResponse.md)
  - [CreateUserRequest](docs/CreateUserRequest.md)
  - [DebugEvent](docs/DebugEvent.md)
  - [DeleteAnalyzerResult](docs/DeleteAnalyzerResult.md)
  - [DeleteAnalyzerResultsResponse](docs/DeleteAnalyzerResultsResponse.md)
  - [DeleteDatasetProfilesResponse](docs/DeleteDatasetProfilesResponse.md)
  - [DeleteProfile](docs/DeleteProfile.md)
  - [DeletionStatus](docs/DeletionStatus.md)
+ - [DiagnosisReport](docs/DiagnosisReport.md)
+ - [DiagnosisRequest](docs/DiagnosisRequest.md)
+ - [DiagnosisRequestStatus](docs/DiagnosisRequestStatus.md)
+ - [DiagnosticDataSummary](docs/DiagnosticDataSummary.md)
  - [DiagnosticIntervalRequest](docs/DiagnosticIntervalRequest.md)
  - [DiagnosticIntervalResponse](docs/DiagnosticIntervalResponse.md)
  - [EmailNotificationAction](docs/EmailNotificationAction.md)
  - [EntitySchema](docs/EntitySchema.md)
- - [EntitySearchResult](docs/EntitySearchResult.md)
  - [EntityWeightRecord](docs/EntityWeightRecord.md)
  - [EntityWeightRecordMetadata](docs/EntityWeightRecordMetadata.md)
  - [ErrorStatus](docs/ErrorStatus.md)
  - [ExportTracePartialSuccess](docs/ExportTracePartialSuccess.md)
  - [ExportTraceServiceResponse](docs/ExportTraceServiceResponse.md)
+ - [FailureRecord](docs/FailureRecord.md)
  - [FeatureFlags](docs/FeatureFlags.md)
  - [GetAccountMembershipsResponse](docs/GetAccountMembershipsResponse.md)
  - [GetAssetResponse](docs/GetAssetResponse.md)
  - [GetDatasetMetadataResponse](docs/GetDatasetMetadataResponse.md)
  - [GetDefaultMembershipResponse](docs/GetDefaultMembershipResponse.md)
  - [GetMarketplaceMetadataResponse](docs/GetMarketplaceMetadataResponse.md)
  - [GetMembershipsResponse](docs/GetMembershipsResponse.md)
@@ -263,50 +279,53 @@
  - [LogSessionReferenceResponse](docs/LogSessionReferenceResponse.md)
  - [LogTransactionMetadata](docs/LogTransactionMetadata.md)
  - [MarketplaceDimensions](docs/MarketplaceDimensions.md)
  - [Member](docs/Member.md)
  - [Membership](docs/Membership.md)
  - [MembershipMetadata](docs/MembershipMetadata.md)
  - [MetricSchema](docs/MetricSchema.md)
+ - [MetricSchemaFields](docs/MetricSchemaFields.md)
  - [MetricTimeseriesRecord](docs/MetricTimeseriesRecord.md)
  - [MetricTimeseriesRequest](docs/MetricTimeseriesRequest.md)
  - [MetricTimeseriesResponse](docs/MetricTimeseriesResponse.md)
  - [ModelMetadataResponse](docs/ModelMetadataResponse.md)
  - [ModelType](docs/ModelType.md)
  - [MonitorConfigVersion](docs/MonitorConfigVersion.md)
+ - [NamedCount](docs/NamedCount.md)
+ - [NamedMetricSchema](docs/NamedMetricSchema.md)
  - [NotificationAction](docs/NotificationAction.md)
  - [NotificationActionPayload](docs/NotificationActionPayload.md)
  - [NotificationRelationshipItem](docs/NotificationRelationshipItem.md)
  - [NotificationRelationshipType](docs/NotificationRelationshipType.md)
  - [NotificationSettings](docs/NotificationSettings.md)
  - [NotificationSettingsDay](docs/NotificationSettingsDay.md)
  - [NotificationSqsMessageCadence](docs/NotificationSqsMessageCadence.md)
  - [OrganizationMetadata](docs/OrganizationMetadata.md)
  - [OrganizationRoleMembers](docs/OrganizationRoleMembers.md)
  - [OrganizationSummary](docs/OrganizationSummary.md)
  - [PagerDutyNotificationAction](docs/PagerDutyNotificationAction.md)
  - [PatchAccountMembershipsRequest](docs/PatchAccountMembershipsRequest.md)
  - [PostAssetRequest](docs/PostAssetRequest.md)
  - [PostAssetResponse](docs/PostAssetResponse.md)
+ - [ProfileSummary](docs/ProfileSummary.md)
  - [ProfileTrace](docs/ProfileTrace.md)
  - [ProfileTracesResponse](docs/ProfileTracesResponse.md)
  - [ProvisionNewAWSMarketplaceUserResponse](docs/ProvisionNewAWSMarketplaceUserResponse.md)
  - [ProvisionNewMarketplaceUserRequest](docs/ProvisionNewMarketplaceUserRequest.md)
  - [ProvisionNewUserRequest](docs/ProvisionNewUserRequest.md)
  - [ProvisionNewUserResponse](docs/ProvisionNewUserResponse.md)
  - [PutAccountMembershipsRequest](docs/PutAccountMembershipsRequest.md)
+ - [QualityIssueRecord](docs/QualityIssueRecord.md)
  - [ReferenceProfileItemResponse](docs/ReferenceProfileItemResponse.md)
  - [RemoveMembershipRequest](docs/RemoveMembershipRequest.md)
  - [Response](docs/Response.md)
+ - [ResultRecord](docs/ResultRecord.md)
  - [RevokeUserSessionRequest](docs/RevokeUserSessionRequest.md)
  - [Role](docs/Role.md)
  - [SchemaMetadata](docs/SchemaMetadata.md)
- - [SearchIndexRequest](docs/SearchIndexRequest.md)
- - [SearchIndexType](docs/SearchIndexType.md)
- - [SearchResponse](docs/SearchResponse.md)
  - [Segment](docs/Segment.md)
  - [SegmentListResponse](docs/SegmentListResponse.md)
  - [SegmentTag](docs/SegmentTag.md)
  - [SegmentWeight](docs/SegmentWeight.md)
  - [SegmentsListRequest](docs/SegmentsListRequest.md)
  - [SessionMetadata](docs/SessionMetadata.md)
  - [SetDefaultMembershipRequest](docs/SetDefaultMembershipRequest.md)
```

### Comparing `whylabs-client-0.6.2/setup.py` & `whylabs-client-0.6.3/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from setuptools import setup, find_packages  # noqa: H301
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "RELEASE.md").read_text()
 
 NAME = "whylabs-client"
-VERSION = "0.6.2"
+VERSION = "0.6.3"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `whylabs-client-0.6.2/whylabs_client/__init__.py` & `whylabs-client-0.6.3/whylabs_client/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
     The version of the OpenAPI document: 0.1
     Contact: support@whylabs.ai
     Generated by: https://openapi-generator.tech
 """
 
 
-__version__ = "0.6.2"
+__version__ = "0.6.3"
 
 # import ApiClient
 from whylabs_client.api_client import ApiClient
 
 # import Configuration
 from whylabs_client.configuration import Configuration
```

### Comparing `whylabs-client-0.6.2/whylabs_client/api/api_key_api.py` & `whylabs-client-0.6.3/whylabs_client/api/api_key_api.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.2/whylabs_client/api/assets_api.py` & `whylabs-client-0.6.3/whylabs_client/api/assets_api.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.2/whylabs_client/api/data_api.py` & `whylabs-client-0.6.3/whylabs_client/api/data_api.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.2/whylabs_client/api/dataset_metadata_api.py` & `whylabs-client-0.6.3/whylabs_client/api/dataset_metadata_api.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.2/whylabs_client/api/dataset_profile_api.py` & `whylabs-client-0.6.3/whylabs_client/api/dataset_profile_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -199,24 +199,26 @@
                 'all': [
                     'org_id',
                     'dataset_id',
                     'profile_start_timestamp',
                     'profile_end_timestamp',
                     'before_upload_timestamp',
                     'delete_analyzer_results',
+                    'column_name',
                 ],
                 'required': [
                     'org_id',
                     'dataset_id',
                 ],
                 'nullable': [
                     'profile_start_timestamp',
                     'profile_end_timestamp',
                     'before_upload_timestamp',
                     'delete_analyzer_results',
+                    'column_name',
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
             root_map={
@@ -233,30 +235,34 @@
                         (int, none_type,),
                     'profile_end_timestamp':
                         (int, none_type,),
                     'before_upload_timestamp':
                         (int, none_type,),
                     'delete_analyzer_results':
                         (bool, none_type,),
+                    'column_name':
+                        (str, none_type,),
                 },
                 'attribute_map': {
                     'org_id': 'org_id',
                     'dataset_id': 'dataset_id',
                     'profile_start_timestamp': 'profile_start_timestamp',
                     'profile_end_timestamp': 'profile_end_timestamp',
                     'before_upload_timestamp': 'before_upload_timestamp',
                     'delete_analyzer_results': 'delete_analyzer_results',
+                    'column_name': 'column_name',
                 },
                 'location_map': {
                     'org_id': 'path',
                     'dataset_id': 'path',
                     'profile_start_timestamp': 'query',
                     'profile_end_timestamp': 'query',
                     'before_upload_timestamp': 'query',
                     'delete_analyzer_results': 'query',
+                    'column_name': 'query',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/json'
@@ -960,14 +966,15 @@
             dataset_id (str): The unique dataset ID in your company.
 
         Keyword Args:
             profile_start_timestamp (int, none_type): Optional, scope deleting profiles from and more recent than the timestamp. [optional]
             profile_end_timestamp (int, none_type): Optional, scope deleting profiles older than the timestamp. [optional]
             before_upload_timestamp (int, none_type): Optional, scope deleting profiles uploaded prior to the timestamp. [optional]
             delete_analyzer_results (bool, none_type): [optional]
+            column_name (str, none_type): [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
```

### Comparing `whylabs-client-0.6.2/whylabs_client/api/debug_events_api.py` & `whylabs-client-0.6.3/whylabs_client/api/debug_events_api.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.2/whylabs_client/api/feature_weights_api.py` & `whylabs-client-0.6.3/whylabs_client/api/feature_weights_api.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.2/whylabs_client/api/log_api.py` & `whylabs-client-0.6.3/whylabs_client/api/log_api.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.2/whylabs_client/api/membership_api.py` & `whylabs-client-0.6.3/whylabs_client/api/membership_api.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.2/whylabs_client/api/models_api.py` & `whylabs-client-0.6.3/whylabs_client/api/models_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,16 +22,18 @@
     none_type,
     validate_and_convert_types
 )
 from whylabs_client.model.column_schema import ColumnSchema
 from whylabs_client.model.entity_schema import EntitySchema
 from whylabs_client.model.list_models_response import ListModelsResponse
 from whylabs_client.model.metric_schema import MetricSchema
+from whylabs_client.model.metric_schema_fields import MetricSchemaFields
 from whylabs_client.model.model_metadata_response import ModelMetadataResponse
 from whylabs_client.model.model_type import ModelType
+from whylabs_client.model.named_metric_schema import NamedMetricSchema
 from whylabs_client.model.response import Response
 from whylabs_client.model.time_period import TimePeriod
 
 
 class ModelsApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
@@ -313,29 +315,29 @@
         )
         self.delete_entity_schema_metric_endpoint = _Endpoint(
             settings={
                 'response_type': (Response,),
                 'auth': [
                     'ApiKeyAuth'
                 ],
-                'endpoint_path': '/v0/organizations/{org_id}/models/{dataset_id}/schema/metric/{metric_label}',
+                'endpoint_path': '/v0/organizations/{org_id}/models/{dataset_id}/schema/metric/{metric_name}',
                 'operation_id': 'delete_entity_schema_metric',
                 'http_method': 'DELETE',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'org_id',
                     'dataset_id',
-                    'metric_label',
+                    'metric_name',
                 ],
                 'required': [
                     'org_id',
                     'dataset_id',
-                    'metric_label',
+                    'metric_name',
                 ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
@@ -346,26 +348,26 @@
                 'allowed_values': {
                 },
                 'openapi_types': {
                     'org_id':
                         (str,),
                     'dataset_id':
                         (str,),
-                    'metric_label':
+                    'metric_name':
                         (str,),
                 },
                 'attribute_map': {
                     'org_id': 'org_id',
                     'dataset_id': 'dataset_id',
-                    'metric_label': 'metric_label',
+                    'metric_name': 'metric_name',
                 },
                 'location_map': {
                     'org_id': 'path',
                     'dataset_id': 'path',
-                    'metric_label': 'path',
+                    'metric_name': 'path',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/json'
@@ -547,14 +549,71 @@
                 'accept': [
                     'application/json'
                 ],
                 'content_type': [],
             },
             api_client=api_client
         )
+        self.get_named_metric_schemas_endpoint = _Endpoint(
+            settings={
+                'response_type': ([NamedMetricSchema],),
+                'auth': [
+                    'ApiKeyAuth'
+                ],
+                'endpoint_path': '/v0/organizations/{org_id}/models/{dataset_id}/schema/metrics',
+                'operation_id': 'get_named_metric_schemas',
+                'http_method': 'GET',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'org_id',
+                    'dataset_id',
+                ],
+                'required': [
+                    'org_id',
+                    'dataset_id',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'org_id':
+                        (str,),
+                    'dataset_id':
+                        (str,),
+                },
+                'attribute_map': {
+                    'org_id': 'org_id',
+                    'dataset_id': 'dataset_id',
+                },
+                'location_map': {
+                    'org_id': 'path',
+                    'dataset_id': 'path',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [],
+            },
+            api_client=api_client
+        )
         self.list_models_endpoint = _Endpoint(
             settings={
                 'response_type': (ListModelsResponse,),
                 'auth': [
                     'ApiKeyAuth'
                 ],
                 'endpoint_path': '/v0/organizations/{org_id}/models',
@@ -796,14 +855,84 @@
                 ],
                 'content_type': [
                     'application/json'
                 ]
             },
             api_client=api_client
         )
+        self.put_named_metric_schema_endpoint = _Endpoint(
+            settings={
+                'response_type': (Response,),
+                'auth': [
+                    'ApiKeyAuth'
+                ],
+                'endpoint_path': '/v0/organizations/{org_id}/models/{dataset_id}/schema/metric/{metric_name}',
+                'operation_id': 'put_named_metric_schema',
+                'http_method': 'PUT',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'org_id',
+                    'dataset_id',
+                    'metric_name',
+                    'metric_schema_fields',
+                ],
+                'required': [
+                    'org_id',
+                    'dataset_id',
+                    'metric_name',
+                    'metric_schema_fields',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'org_id':
+                        (str,),
+                    'dataset_id':
+                        (str,),
+                    'metric_name':
+                        (str,),
+                    'metric_schema_fields':
+                        (MetricSchemaFields,),
+                },
+                'attribute_map': {
+                    'org_id': 'org_id',
+                    'dataset_id': 'dataset_id',
+                    'metric_name': 'metric_name',
+                },
+                'location_map': {
+                    'org_id': 'path',
+                    'dataset_id': 'path',
+                    'metric_name': 'path',
+                    'metric_schema_fields': 'body',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [
+                    'application/json'
+                ]
+            },
+            api_client=api_client
+        )
         self.update_model_endpoint = _Endpoint(
             settings={
                 'response_type': (ModelMetadataResponse,),
                 'auth': [
                     'ApiKeyAuth'
                 ],
                 'endpoint_path': '/v0/organizations/{org_id}/models/{model_id}',
@@ -1185,30 +1314,30 @@
             column_id
         return self.delete_entity_schema_column_endpoint.call_with_http_info(**kwargs)
 
     def delete_entity_schema_metric(
         self,
         org_id,
         dataset_id,
-        metric_label,
+        metric_name,
         **kwargs
     ):
         """Delete the schema of a single metric for a given dataset.  # noqa: E501
 
         Delete the schema of a single metric for a given dataset.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.delete_entity_schema_metric(org_id, dataset_id, metric_label, async_req=True)
+        >>> thread = api.delete_entity_schema_metric(org_id, dataset_id, metric_name, async_req=True)
         >>> result = thread.get()
 
         Args:
             org_id (str):
             dataset_id (str):
-            metric_label (str):
+            metric_name (str):
 
         Keyword Args:
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
@@ -1256,16 +1385,16 @@
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['org_id'] = \
             org_id
         kwargs['dataset_id'] = \
             dataset_id
-        kwargs['metric_label'] = \
-            metric_label
+        kwargs['metric_name'] = \
+            metric_name
         return self.delete_entity_schema_metric_endpoint.call_with_http_info(**kwargs)
 
     def get_entity_schema(
         self,
         org_id,
         dataset_id,
         **kwargs
@@ -1489,14 +1618,89 @@
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['org_id'] = \
             org_id
         kwargs['model_id'] = \
             model_id
         return self.get_model_endpoint.call_with_http_info(**kwargs)
 
+    def get_named_metric_schemas(
+        self,
+        org_id,
+        dataset_id,
+        **kwargs
+    ):
+        """Get all of the named metrics for a given dataset.  # noqa: E501
+
+        Get all of the named metrics for a given dataset.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.get_named_metric_schemas(org_id, dataset_id, async_req=True)
+        >>> result = thread.get()
+
+        Args:
+            org_id (str):
+            dataset_id (str):
+
+        Keyword Args:
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            [NamedMetricSchema]
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_content_type'] = kwargs.get(
+            '_content_type')
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['org_id'] = \
+            org_id
+        kwargs['dataset_id'] = \
+            dataset_id
+        return self.get_named_metric_schemas_endpoint.call_with_http_info(**kwargs)
+
     def list_models(
         self,
         org_id,
         **kwargs
     ):
         """Get a list of all of the model ids for an organization.  # noqa: E501
 
@@ -1731,15 +1935,15 @@
         org_id,
         dataset_id,
         metric_schema,
         **kwargs
     ):
         """Save the schema of a single metric for a given dataset.  # noqa: E501
 
-        Save the schema of a single metric for a given dataset.  # noqa: E501
+        Save the schema of a single metric for a given dataset. The metric will be given a name based on the label in the schema, replacing any non-alphanumeric with _.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.put_entity_schema_metric(org_id, dataset_id, metric_schema, async_req=True)
         >>> result = thread.get()
 
         Args:
@@ -1801,14 +2005,97 @@
             org_id
         kwargs['dataset_id'] = \
             dataset_id
         kwargs['metric_schema'] = \
             metric_schema
         return self.put_entity_schema_metric_endpoint.call_with_http_info(**kwargs)
 
+    def put_named_metric_schema(
+        self,
+        org_id,
+        dataset_id,
+        metric_name,
+        metric_schema_fields,
+        **kwargs
+    ):
+        """Save the schema of a single named metric for a given dataset.  # noqa: E501
+
+        Save the schema of a single named metric for a given dataset.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.put_named_metric_schema(org_id, dataset_id, metric_name, metric_schema_fields, async_req=True)
+        >>> result = thread.get()
+
+        Args:
+            org_id (str):
+            dataset_id (str):
+            metric_name (str):
+            metric_schema_fields (MetricSchemaFields):
+
+        Keyword Args:
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            Response
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_content_type'] = kwargs.get(
+            '_content_type')
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['org_id'] = \
+            org_id
+        kwargs['dataset_id'] = \
+            dataset_id
+        kwargs['metric_name'] = \
+            metric_name
+        kwargs['metric_schema_fields'] = \
+            metric_schema_fields
+        return self.put_named_metric_schema_endpoint.call_with_http_info(**kwargs)
+
     def update_model(
         self,
         org_id,
         model_id,
         model_name,
         time_period,
         **kwargs
```

### Comparing `whylabs-client-0.6.2/whylabs_client/api/monitor_api.py` & `whylabs-client-0.6.3/whylabs_client/api/monitor_api.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.2/whylabs_client/api/monitor_diagnostics_api.py` & `whylabs-client-0.6.3/whylabs_client/api/monitor_diagnostics_api.py`

 * *Files 22% similar despite different names*

```diff
@@ -24,14 +24,18 @@
 )
 from whylabs_client.model.analyzer_segment_columns_diagnostic_request import AnalyzerSegmentColumnsDiagnosticRequest
 from whylabs_client.model.analyzer_segment_columns_diagnostic_response import AnalyzerSegmentColumnsDiagnosticResponse
 from whylabs_client.model.analyzer_segments_diagnostic_request import AnalyzerSegmentsDiagnosticRequest
 from whylabs_client.model.analyzer_segments_diagnostic_response import AnalyzerSegmentsDiagnosticResponse
 from whylabs_client.model.analyzers_diagnostic_request import AnalyzersDiagnosticRequest
 from whylabs_client.model.analyzers_diagnostic_response import AnalyzersDiagnosticResponse
+from whylabs_client.model.async_diagnosis_response import AsyncDiagnosisResponse
+from whylabs_client.model.async_diagnosis_result_response import AsyncDiagnosisResultResponse
+from whylabs_client.model.diagnosis_report import DiagnosisReport
+from whylabs_client.model.diagnosis_request import DiagnosisRequest
 from whylabs_client.model.diagnostic_interval_request import DiagnosticIntervalRequest
 from whylabs_client.model.diagnostic_interval_response import DiagnosticIntervalResponse
 
 
 class MonitorDiagnosticsApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
@@ -225,14 +229,199 @@
                 ],
                 'content_type': [
                     'application/json'
                 ]
             },
             api_client=api_client
         )
+        self.diagnose_analyzer_async_endpoint = _Endpoint(
+            settings={
+                'response_type': (AsyncDiagnosisResponse,),
+                'auth': [
+                    'ApiKeyAuth'
+                ],
+                'endpoint_path': '/v0/organizations/{org_id}/diagnostics/monitor/diagnose/analyzer/async',
+                'operation_id': 'diagnose_analyzer_async',
+                'http_method': 'POST',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'org_id',
+                    'diagnosis_request',
+                ],
+                'required': [
+                    'org_id',
+                    'diagnosis_request',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                    'org_id',
+                ]
+            },
+            root_map={
+                'validations': {
+                    ('org_id',): {
+                        'max_length': 128,
+                    },
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'org_id':
+                        (str,),
+                    'diagnosis_request':
+                        (DiagnosisRequest,),
+                },
+                'attribute_map': {
+                    'org_id': 'org_id',
+                },
+                'location_map': {
+                    'org_id': 'path',
+                    'diagnosis_request': 'body',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [
+                    'application/json'
+                ]
+            },
+            api_client=api_client
+        )
+        self.diagnose_analyzer_async_result_endpoint = _Endpoint(
+            settings={
+                'response_type': (AsyncDiagnosisResultResponse,),
+                'auth': [
+                    'ApiKeyAuth'
+                ],
+                'endpoint_path': '/v0/organizations/{org_id}/diagnostics/monitor/diagnose/analyzer/async/result',
+                'operation_id': 'diagnose_analyzer_async_result',
+                'http_method': 'GET',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'org_id',
+                    'diagnosis_id',
+                ],
+                'required': [
+                    'org_id',
+                    'diagnosis_id',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                    'org_id',
+                ]
+            },
+            root_map={
+                'validations': {
+                    ('org_id',): {
+                        'max_length': 128,
+                    },
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'org_id':
+                        (str,),
+                    'diagnosis_id':
+                        (str,),
+                },
+                'attribute_map': {
+                    'org_id': 'org_id',
+                    'diagnosis_id': 'diagnosis_id',
+                },
+                'location_map': {
+                    'org_id': 'path',
+                    'diagnosis_id': 'query',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [],
+            },
+            api_client=api_client
+        )
+        self.diagnose_analyzer_sync_endpoint = _Endpoint(
+            settings={
+                'response_type': (DiagnosisReport,),
+                'auth': [
+                    'ApiKeyAuth'
+                ],
+                'endpoint_path': '/v0/organizations/{org_id}/diagnostics/monitor/diagnose/analyzer/sync',
+                'operation_id': 'diagnose_analyzer_sync',
+                'http_method': 'POST',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'org_id',
+                    'diagnosis_request',
+                ],
+                'required': [
+                    'org_id',
+                    'diagnosis_request',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                    'org_id',
+                ]
+            },
+            root_map={
+                'validations': {
+                    ('org_id',): {
+                        'max_length': 128,
+                    },
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'org_id':
+                        (str,),
+                    'diagnosis_request':
+                        (DiagnosisRequest,),
+                },
+                'attribute_map': {
+                    'org_id': 'org_id',
+                },
+                'location_map': {
+                    'org_id': 'path',
+                    'diagnosis_request': 'body',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [
+                    'application/json'
+                ]
+            },
+            api_client=api_client
+        )
         self.recommend_diagnostic_interval_endpoint = _Endpoint(
             settings={
                 'response_type': (DiagnosticIntervalResponse,),
                 'auth': [
                     'ApiKeyAuth'
                 ],
                 'endpoint_path': '/v0/organizations/{org_id}/diagnostics/monitor/interval',
@@ -513,14 +702,239 @@
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['org_id'] = \
             org_id
         kwargs['analyzer_segments_diagnostic_request'] = \
             analyzer_segments_diagnostic_request
         return self.detect_noisy_segments_endpoint.call_with_http_info(**kwargs)
 
+    def diagnose_analyzer_async(
+        self,
+        org_id,
+        diagnosis_request,
+        **kwargs
+    ):
+        """Endpoint to request a diagnosis for a specific analyzer  # noqa: E501
+
+        Returns a unique request ID for the diagnosis request. Use the DiagnoseAnalyzerAsyncResult endpoint to get the result.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.diagnose_analyzer_async(org_id, diagnosis_request, async_req=True)
+        >>> result = thread.get()
+
+        Args:
+            org_id (str):
+            diagnosis_request (DiagnosisRequest):
+
+        Keyword Args:
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            AsyncDiagnosisResponse
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_content_type'] = kwargs.get(
+            '_content_type')
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['org_id'] = \
+            org_id
+        kwargs['diagnosis_request'] = \
+            diagnosis_request
+        return self.diagnose_analyzer_async_endpoint.call_with_http_info(**kwargs)
+
+    def diagnose_analyzer_async_result(
+        self,
+        org_id,
+        diagnosis_id,
+        **kwargs
+    ):
+        """Endpoint to request the result of an async diagnosis  # noqa: E501
+
+        Returns a response with the request status and the diagnosis report if the request is complete.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.diagnose_analyzer_async_result(org_id, diagnosis_id, async_req=True)
+        >>> result = thread.get()
+
+        Args:
+            org_id (str):
+            diagnosis_id (str):
+
+        Keyword Args:
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            AsyncDiagnosisResultResponse
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_content_type'] = kwargs.get(
+            '_content_type')
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['org_id'] = \
+            org_id
+        kwargs['diagnosis_id'] = \
+            diagnosis_id
+        return self.diagnose_analyzer_async_result_endpoint.call_with_http_info(**kwargs)
+
+    def diagnose_analyzer_sync(
+        self,
+        org_id,
+        diagnosis_request,
+        **kwargs
+    ):
+        """Endpoint to diagnose a specific analyzer  # noqa: E501
+
+        Returns a diagnosis report for a specific analyzer, segment, and interval. Only suitable for small datasets.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.diagnose_analyzer_sync(org_id, diagnosis_request, async_req=True)
+        >>> result = thread.get()
+
+        Args:
+            org_id (str):
+            diagnosis_request (DiagnosisRequest):
+
+        Keyword Args:
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            DiagnosisReport
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_content_type'] = kwargs.get(
+            '_content_type')
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['org_id'] = \
+            org_id
+        kwargs['diagnosis_request'] = \
+            diagnosis_request
+        return self.diagnose_analyzer_sync_endpoint.call_with_http_info(**kwargs)
+
     def recommend_diagnostic_interval(
         self,
         org_id,
         diagnostic_interval_request,
         **kwargs
     ):
         """Endpoint to recommend a diagnostic interval  # noqa: E501
```

### Comparing `whylabs-client-0.6.2/whylabs_client/api/notification_settings_api.py` & `whylabs-client-0.6.3/whylabs_client/api/notification_settings_api.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.2/whylabs_client/api/policy_api.py` & `whylabs-client-0.6.3/whylabs_client/api/policy_api.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.2/whylabs_client/api/schema_api.py` & `whylabs-client-0.6.3/whylabs_client/api/schema_api.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.2/whylabs_client/api/security_api.py` & `whylabs-client-0.6.3/whylabs_client/api/security_api.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.2/whylabs_client/api/sessions_api.py` & `whylabs-client-0.6.3/whylabs_client/api/sessions_api.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.2/whylabs_client/api/traces_api.py` & `whylabs-client-0.6.3/whylabs_client/api/traces_api.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.2/whylabs_client/api/transactions_api.py` & `whylabs-client-0.6.3/whylabs_client/api/transactions_api.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.2/whylabs_client/api_client.py` & `whylabs-client-0.6.3/whylabs_client/api_client.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.2/whylabs_client/apis/__init__.py` & `whylabs-client-0.6.3/whylabs_client/apis/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 #
 #   import sys
 #   sys.setrecursionlimit(n)
 
 # Import APIs into API package:
 from whylabs_client.api.api_key_api import ApiKeyApi
 from whylabs_client.api.assets_api import AssetsApi
+from whylabs_client.api.container_diagnostics_api import ContainerDiagnosticsApi
 from whylabs_client.api.data_api import DataApi
 from whylabs_client.api.dataset_profile_api import DatasetProfileApi
 from whylabs_client.api.dataset_metadata_api import DatasetMetadataApi
 from whylabs_client.api.debug_events_api import DebugEventsApi
 from whylabs_client.api.feature_weights_api import FeatureWeightsApi
 from whylabs_client.api.log_api import LogApi
 from whylabs_client.api.membership_api import MembershipApi
```

### Comparing `whylabs-client-0.6.2/whylabs_client/configuration.py` & `whylabs-client-0.6.3/whylabs_client/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -406,15 +406,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: 0.1\n"\
-               "SDK Package Version: 0.6.2".\
+               "SDK Package Version: 0.6.3".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `whylabs-client-0.6.2/whylabs_client/exceptions.py` & `whylabs-client-0.6.3/whylabs_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.2/whylabs_client/model/account_organization.py` & `whylabs-client-0.6.3/whylabs_client/model/account_organization.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.2/whylabs_client/model/account_user.py` & `whylabs-client-0.6.3/whylabs_client/model/account_user.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.2/whylabs_client/model/action_type.py` & `whylabs-client-0.6.3/whylabs_client/model/action_type.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.2/whylabs_client/model/activate_azure_subscription_request.py` & `whylabs-client-0.6.3/whylabs_client/model/activate_azure_subscription_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.2/whylabs_client/model/activate_azure_subscription_response.py` & `whylabs-client-0.6.3/whylabs_client/model/activate_azure_subscription_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.2/whylabs_client/model/add_membership_request.py` & `whylabs-client-0.6.3/whylabs_client/model/add_membership_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.2/whylabs_client/model/add_policy_response.py` & `whylabs-client-0.6.3/whylabs_client/model/add_policy_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.2/whylabs_client/model/admin_report_response.py` & `whylabs-client-0.6.3/whylabs_client/model/admin_report_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.2/whylabs_client/model/admin_report_type.py` & `whylabs-client-0.6.3/whylabs_client/model/admin_report_type.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.2/whylabs_client/model/analysis_results_record.py` & `whylabs-client-0.6.3/whylabs_client/model/analysis_results_record.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.2/whylabs_client/model/analysis_results_request.py` & `whylabs-client-0.6.3/whylabs_client/model/analysis_results_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.2/whylabs_client/model/analysis_results_response.py` & `whylabs-client-0.6.3/whylabs_client/model/analysis_results_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.2/whylabs_client/model/analyzer_diagnostic_record.py` & `whylabs-client-0.6.3/whylabs_client/model/analyzer_diagnostic_record.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.2/whylabs_client/model/analyzer_failure_record.py` & `whylabs-client-0.6.3/whylabs_client/model/analyzer_failure_record.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.2/whylabs_client/model/analyzer_segment_column_diagnostic_record.py` & `whylabs-client-0.6.3/whylabs_client/model/analyzer_segment_column_diagnostic_record.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.2/whylabs_client/model/analyzer_segment_columns_diagnostic_request.py` & `whylabs-client-0.6.3/whylabs_client/model/analyzer_segment_columns_diagnostic_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.2/whylabs_client/model/analyzer_segment_columns_diagnostic_response.py` & `whylabs-client-0.6.3/whylabs_client/model/analyzer_segment_columns_diagnostic_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.2/whylabs_client/model/analyzer_segment_diagnostic_record.py` & `whylabs-client-0.6.3/whylabs_client/model/analyzer_segment_diagnostic_record.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.2/whylabs_client/model/analyzer_segment_failure_record.py` & `whylabs-client-0.6.3/whylabs_client/model/analyzer_segment_failure_record.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.2/whylabs_client/model/analyzer_segments_diagnostic_request.py` & `whylabs-client-0.6.3/whylabs_client/model/analyzer_segments_diagnostic_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.2/whylabs_client/model/analyzer_segments_diagnostic_response.py` & `whylabs-client-0.6.3/whylabs_client/model/analyzer_segments_diagnostic_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.2/whylabs_client/model/analyzers_diagnostic_request.py` & `whylabs-client-0.6.3/whylabs_client/model/analyzers_diagnostic_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.2/whylabs_client/model/analyzers_diagnostic_response.py` & `whylabs-client-0.6.3/whylabs_client/model/analyzers_diagnostic_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.2/whylabs_client/model/async_log_response.py` & `whylabs-client-0.6.3/whylabs_client/model/async_log_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.2/whylabs_client/model/aws_marketplace_metadata.py` & `whylabs-client-0.6.3/whylabs_client/model/aws_marketplace_metadata.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.2/whylabs_client/model/azure_marketplace_contact_payload.py` & `whylabs-client-0.6.3/whylabs_client/model/azure_marketplace_contact_payload.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.2/whylabs_client/model/azure_marketplace_subscription_details.py` & `whylabs-client-0.6.3/whylabs_client/model/azure_marketplace_subscription_details.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.2/whylabs_client/model/batch_log_reference_request.py` & `whylabs-client-0.6.3/whylabs_client/model/batch_log_reference_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.2/whylabs_client/model/batch_log_session_reference_response.py` & `whylabs-client-0.6.3/whylabs_client/model/batch_log_session_reference_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.2/whylabs_client/model/cache_key_type.py` & `whylabs-client-0.6.3/whylabs_client/model/cache_key_type.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.2/whylabs_client/model/column_schema.py` & `whylabs-client-0.6.3/whylabs_client/model/column_schema.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.2/whylabs_client/model/create_account_user_request.py` & `whylabs-client-0.6.3/whylabs_client/model/create_account_user_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.2/whylabs_client/model/create_dataset_profile_upload_response.py` & `whylabs-client-0.6.3/whylabs_client/model/create_dataset_profile_upload_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.2/whylabs_client/model/create_reference_profile_request.py` & `whylabs-client-0.6.3/whylabs_client/model/create_reference_profile_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.2/whylabs_client/model/create_reference_profile_response.py` & `whylabs-client-0.6.3/whylabs_client/model/create_reference_profile_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.2/whylabs_client/model/create_session_request.py` & `whylabs-client-0.6.3/whylabs_client/model/create_session_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.2/whylabs_client/model/create_session_response.py` & `whylabs-client-0.6.3/whylabs_client/model/create_session_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.2/whylabs_client/model/create_user_request.py` & `whylabs-client-0.6.3/whylabs_client/model/create_user_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.2/whylabs_client/model/debug_event.py` & `whylabs-client-0.6.3/whylabs_client/model/debug_event.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.2/whylabs_client/model/delete_analyzer_result.py` & `whylabs-client-0.6.3/whylabs_client/model/delete_analyzer_result.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.2/whylabs_client/model/delete_analyzer_results_response.py` & `whylabs-client-0.6.3/whylabs_client/model/delete_analyzer_results_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.2/whylabs_client/model/delete_dataset_profiles_response.py` & `whylabs-client-0.6.3/whylabs_client/model/delete_dataset_profiles_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.2/whylabs_client/model/delete_profile.py` & `whylabs-client-0.6.3/whylabs_client/model/delete_profile.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,14 +93,15 @@
             'updated_timestamp': (int,),  # noqa: E501
             'org_id': (str,),  # noqa: E501
             'dataset_id': (str,),  # noqa: E501
             'id': (int, none_type,),  # noqa: E501
             'delete_gte': (int, none_type,),  # noqa: E501
             'delete_lt': (int, none_type,),  # noqa: E501
             'before_upload_ts': (int, none_type,),  # noqa: E501
+            'column_name': (str, none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
@@ -110,14 +111,15 @@
         'updated_timestamp': 'updatedTimestamp',  # noqa: E501
         'org_id': 'orgId',  # noqa: E501
         'dataset_id': 'datasetId',  # noqa: E501
         'id': 'id',  # noqa: E501
         'delete_gte': 'deleteGte',  # noqa: E501
         'delete_lt': 'deleteLt',  # noqa: E501
         'before_upload_ts': 'beforeUploadTs',  # noqa: E501
+        'column_name': 'columnName',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
@@ -164,14 +166,15 @@
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             id (int, none_type): [optional]  # noqa: E501
             delete_gte (int, none_type): [optional]  # noqa: E501
             delete_lt (int, none_type): [optional]  # noqa: E501
             before_upload_ts (int, none_type): [optional]  # noqa: E501
+            column_name (str, none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -261,14 +264,15 @@
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             id (int, none_type): [optional]  # noqa: E501
             delete_gte (int, none_type): [optional]  # noqa: E501
             delete_lt (int, none_type): [optional]  # noqa: E501
             before_upload_ts (int, none_type): [optional]  # noqa: E501
+            column_name (str, none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `whylabs-client-0.6.2/whylabs_client/model/deletion_status.py` & `whylabs-client-0.6.3/whylabs_client/model/deletion_status.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.2/whylabs_client/model/diagnostic_interval_request.py` & `whylabs-client-0.6.3/whylabs_client/model/diagnostic_interval_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.2/whylabs_client/model/diagnostic_interval_response.py` & `whylabs-client-0.6.3/whylabs_client/model/diagnostic_interval_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.2/whylabs_client/model/email_notification_action.py` & `whylabs-client-0.6.3/whylabs_client/model/email_notification_action.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.2/whylabs_client/model/entity_schema.py` & `whylabs-client-0.6.3/whylabs_client/model/entity_schema.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.2/whylabs_client/model/entity_search_result.py` & `whylabs-client-0.6.3/whylabs_client/model/log_reference_request.py`

 * *Files 10% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from whylabs_client.exceptions import ApiAttributeError
 
 
 
-class EntitySearchResult(ModelNormal):
+class LogReferenceRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -78,49 +78,39 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'keywords': (str, none_type,),  # noqa: E501
-            'type': (str, none_type,),  # noqa: E501
-            'org_id': (str, none_type,),  # noqa: E501
-            'dataset_id': (str, none_type,),  # noqa: E501
-            'monitor_id': (str, none_type,),  # noqa: E501
-            'action_id': (str, none_type,),  # noqa: E501
-            'feature_name': (str, none_type,),  # noqa: E501
-            'metadata': (str, none_type,),  # noqa: E501
+            'alias': (str, none_type,),  # noqa: E501
+            'dataset_timestamp': (int, none_type,),  # noqa: E501
+            'region': (str, none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'keywords': 'keywords',  # noqa: E501
-        'type': 'type',  # noqa: E501
-        'org_id': 'orgId',  # noqa: E501
-        'dataset_id': 'datasetId',  # noqa: E501
-        'monitor_id': 'monitorId',  # noqa: E501
-        'action_id': 'actionId',  # noqa: E501
-        'feature_name': 'featureName',  # noqa: E501
-        'metadata': 'metadata',  # noqa: E501
+        'alias': 'alias',  # noqa: E501
+        'dataset_timestamp': 'datasetTimestamp',  # noqa: E501
+        'region': 'region',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """EntitySearchResult - a model defined in OpenAPI
+        """LogReferenceRequest - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -145,22 +135,17 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            keywords (str, none_type): [optional]  # noqa: E501
-            type (str, none_type): [optional]  # noqa: E501
-            org_id (str, none_type): [optional]  # noqa: E501
-            dataset_id (str, none_type): [optional]  # noqa: E501
-            monitor_id (str, none_type): [optional]  # noqa: E501
-            action_id (str, none_type): [optional]  # noqa: E501
-            feature_name (str, none_type): [optional]  # noqa: E501
-            metadata (str, none_type): [optional]  # noqa: E501
+            alias (str, none_type): [optional]  # noqa: E501
+            dataset_timestamp (int, none_type): [optional]  # noqa: E501
+            region (str, none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -201,15 +186,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """EntitySearchResult - a model defined in OpenAPI
+        """LogReferenceRequest - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -234,22 +219,17 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            keywords (str, none_type): [optional]  # noqa: E501
-            type (str, none_type): [optional]  # noqa: E501
-            org_id (str, none_type): [optional]  # noqa: E501
-            dataset_id (str, none_type): [optional]  # noqa: E501
-            monitor_id (str, none_type): [optional]  # noqa: E501
-            action_id (str, none_type): [optional]  # noqa: E501
-            feature_name (str, none_type): [optional]  # noqa: E501
-            metadata (str, none_type): [optional]  # noqa: E501
+            alias (str, none_type): [optional]  # noqa: E501
+            dataset_timestamp (int, none_type): [optional]  # noqa: E501
+            region (str, none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `whylabs-client-0.6.2/whylabs_client/model/entity_weight_record.py` & `whylabs-client-0.6.3/whylabs_client/model/entity_weight_record.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.2/whylabs_client/model/entity_weight_record_metadata.py` & `whylabs-client-0.6.3/whylabs_client/model/entity_weight_record_metadata.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.2/whylabs_client/model/error_status.py` & `whylabs-client-0.6.3/whylabs_client/model/error_status.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.2/whylabs_client/model/export_trace_partial_success.py` & `whylabs-client-0.6.3/whylabs_client/model/export_trace_partial_success.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.2/whylabs_client/model/export_trace_service_response.py` & `whylabs-client-0.6.3/whylabs_client/model/export_trace_service_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.2/whylabs_client/model/feature_flags.py` & `whylabs-client-0.6.3/whylabs_client/model/feature_flags.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.2/whylabs_client/model/get_account_memberships_response.py` & `whylabs-client-0.6.3/whylabs_client/model/get_account_memberships_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.2/whylabs_client/model/get_asset_response.py` & `whylabs-client-0.6.3/whylabs_client/model/get_asset_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.2/whylabs_client/model/get_dataset_metadata_response.py` & `whylabs-client-0.6.3/whylabs_client/model/get_dataset_metadata_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.2/whylabs_client/model/get_default_membership_response.py` & `whylabs-client-0.6.3/whylabs_client/model/get_default_membership_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.2/whylabs_client/model/get_marketplace_metadata_response.py` & `whylabs-client-0.6.3/whylabs_client/model/get_marketplace_metadata_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.2/whylabs_client/model/get_memberships_response.py` & `whylabs-client-0.6.3/whylabs_client/model/get_memberships_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.2/whylabs_client/model/get_notification_settings_response.py` & `whylabs-client-0.6.3/whylabs_client/model/get_notification_settings_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.2/whylabs_client/model/get_profile_observatory_link_request.py` & `whylabs-client-0.6.3/whylabs_client/model/get_profile_observatory_link_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.2/whylabs_client/model/get_profile_observatory_link_response.py` & `whylabs-client-0.6.3/whylabs_client/model/get_profile_observatory_link_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.2/whylabs_client/model/get_session_response.py` & `whylabs-client-0.6.3/whylabs_client/model/get_session_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.2/whylabs_client/model/granularity.py` & `whylabs-client-0.6.3/whylabs_client/model/granularity.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.2/whylabs_client/model/list_models_response.py` & `whylabs-client-0.6.3/whylabs_client/model/list_models_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.2/whylabs_client/model/list_organization_memberships_response.py` & `whylabs-client-0.6.3/whylabs_client/model/list_organization_memberships_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.2/whylabs_client/model/list_user_api_keys.py` & `whylabs-client-0.6.3/whylabs_client/model/list_user_api_keys.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.2/whylabs_client/model/log_async_request.py` & `whylabs-client-0.6.3/whylabs_client/model/log_async_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.2/whylabs_client/model/log_reference_request.py` & `whylabs-client-0.6.3/whylabs_client/model/post_asset_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from whylabs_client.exceptions import ApiAttributeError
 
 
 
-class LogReferenceRequest(ModelNormal):
+class PostAssetRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -78,39 +78,43 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'alias': (str, none_type,),  # noqa: E501
-            'dataset_timestamp': (int, none_type,),  # noqa: E501
-            'region': (str, none_type,),  # noqa: E501
+            'org_id': (str,),  # noqa: E501
+            's3_uri': (str,),  # noqa: E501
+            'tag': (str, none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'alias': 'alias',  # noqa: E501
-        'dataset_timestamp': 'datasetTimestamp',  # noqa: E501
-        'region': 'region',  # noqa: E501
+        'org_id': 'orgId',  # noqa: E501
+        's3_uri': 's3Uri',  # noqa: E501
+        'tag': 'tag',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """LogReferenceRequest - a model defined in OpenAPI
+    def _from_openapi_data(cls, org_id, s3_uri, *args, **kwargs):  # noqa: E501
+        """PostAssetRequest - a model defined in OpenAPI
+
+        Args:
+            org_id (str):
+            s3_uri (str):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -135,17 +139,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            alias (str, none_type): [optional]  # noqa: E501
-            dataset_timestamp (int, none_type): [optional]  # noqa: E501
-            region (str, none_type): [optional]  # noqa: E501
+            tag (str, none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -165,14 +167,16 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.org_id = org_id
+        self.s3_uri = s3_uri
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -185,16 +189,20 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, *args, **kwargs):  # noqa: E501
-        """LogReferenceRequest - a model defined in OpenAPI
+    def __init__(self, org_id, s3_uri, *args, **kwargs):  # noqa: E501
+        """PostAssetRequest - a model defined in OpenAPI
+
+        Args:
+            org_id (str):
+            s3_uri (str):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -219,17 +227,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            alias (str, none_type): [optional]  # noqa: E501
-            dataset_timestamp (int, none_type): [optional]  # noqa: E501
-            region (str, none_type): [optional]  # noqa: E501
+            tag (str, none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -247,14 +253,16 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.org_id = org_id
+        self.s3_uri = s3_uri
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `whylabs-client-0.6.2/whylabs_client/model/log_reference_response.py` & `whylabs-client-0.6.3/whylabs_client/model/log_reference_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.2/whylabs_client/model/log_response.py` & `whylabs-client-0.6.3/whylabs_client/model/log_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.2/whylabs_client/model/log_session_reference_response.py` & `whylabs-client-0.6.3/whylabs_client/model/log_session_reference_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.2/whylabs_client/model/log_transaction_metadata.py` & `whylabs-client-0.6.3/whylabs_client/model/log_transaction_metadata.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.2/whylabs_client/model/marketplace_dimensions.py` & `whylabs-client-0.6.3/whylabs_client/model/marketplace_dimensions.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.2/whylabs_client/model/member.py` & `whylabs-client-0.6.3/whylabs_client/model/member.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.2/whylabs_client/model/membership.py` & `whylabs-client-0.6.3/whylabs_client/model/membership.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.2/whylabs_client/model/membership_metadata.py` & `whylabs-client-0.6.3/whylabs_client/model/membership_metadata.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.2/whylabs_client/model/metric_schema.py` & `whylabs-client-0.6.3/whylabs_client/model/metric_schema.py`

 * *Files 4% similar despite different names*

```diff
@@ -105,17 +105,17 @@
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, label, column, default_metric, *args, **kwargs):  # noqa: E501
         """MetricSchema - a model defined in OpenAPI
 
         Args:
-            label (str): User-friendly label for the metric. This should be a unique for the entity.
+            label (str): User-friendly label for the metric.
             column (str): Entity column to extract the metric from
-            default_metric (str): whylogs metric to extract. Note that other metrics may be available for this column as well, this is the one to be used by default. Should match the values of the SimpleColumnMetric enum within the monitor config schema.
+            default_metric (str): whylogs metric to extract when this schema is applied. Should match the values of the SimpleColumnMetric enum within the monitor config schema.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -194,17 +194,17 @@
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, label, column, default_metric, *args, **kwargs):  # noqa: E501
         """MetricSchema - a model defined in OpenAPI
 
         Args:
-            label (str): User-friendly label for the metric. This should be a unique for the entity.
+            label (str): User-friendly label for the metric.
             column (str): Entity column to extract the metric from
-            default_metric (str): whylogs metric to extract. Note that other metrics may be available for this column as well, this is the one to be used by default. Should match the values of the SimpleColumnMetric enum within the monitor config schema.
+            default_metric (str): whylogs metric to extract when this schema is applied. Should match the values of the SimpleColumnMetric enum within the monitor config schema.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
```

### Comparing `whylabs-client-0.6.2/whylabs_client/model/metric_timeseries_record.py` & `whylabs-client-0.6.3/whylabs_client/model/metric_timeseries_record.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.2/whylabs_client/model/metric_timeseries_request.py` & `whylabs-client-0.6.3/whylabs_client/model/metric_timeseries_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.2/whylabs_client/model/metric_timeseries_response.py` & `whylabs-client-0.6.3/whylabs_client/model/metric_timeseries_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.2/whylabs_client/model/model_metadata_response.py` & `whylabs-client-0.6.3/whylabs_client/model/model_metadata_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.2/whylabs_client/model/model_type.py` & `whylabs-client-0.6.3/whylabs_client/model/model_type.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.2/whylabs_client/model/monitor_config_version.py` & `whylabs-client-0.6.3/whylabs_client/model/monitor_config_version.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.2/whylabs_client/model/notification_action.py` & `whylabs-client-0.6.3/whylabs_client/model/notification_action.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.2/whylabs_client/model/notification_action_payload.py` & `whylabs-client-0.6.3/whylabs_client/model/notification_action_payload.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.2/whylabs_client/model/notification_relationship_item.py` & `whylabs-client-0.6.3/whylabs_client/model/notification_relationship_item.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.2/whylabs_client/model/notification_relationship_type.py` & `whylabs-client-0.6.3/whylabs_client/model/notification_relationship_type.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.2/whylabs_client/model/notification_settings.py` & `whylabs-client-0.6.3/whylabs_client/model/notification_settings.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.2/whylabs_client/model/notification_settings_day.py` & `whylabs-client-0.6.3/whylabs_client/model/notification_settings_day.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.2/whylabs_client/model/notification_sqs_message_cadence.py` & `whylabs-client-0.6.3/whylabs_client/model/notification_sqs_message_cadence.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.2/whylabs_client/model/organization_metadata.py` & `whylabs-client-0.6.3/whylabs_client/model/organization_metadata.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.2/whylabs_client/model/organization_role_members.py` & `whylabs-client-0.6.3/whylabs_client/model/organization_role_members.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.2/whylabs_client/model/organization_summary.py` & `whylabs-client-0.6.3/whylabs_client/model/organization_summary.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.2/whylabs_client/model/pager_duty_notification_action.py` & `whylabs-client-0.6.3/whylabs_client/model/pager_duty_notification_action.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.2/whylabs_client/model/patch_account_memberships_request.py` & `whylabs-client-0.6.3/whylabs_client/model/patch_account_memberships_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.2/whylabs_client/model/post_asset_request.py` & `whylabs-client-0.6.3/whylabs_client/model/transaction_commit_request.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from whylabs_client.exceptions import ApiAttributeError
 
 
 
-class PostAssetRequest(ModelNormal):
+class TransactionCommitRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -78,43 +78,35 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'org_id': (str,),  # noqa: E501
-            's3_uri': (str,),  # noqa: E501
-            'tag': (str, none_type,),  # noqa: E501
+            'verbose': (bool, none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'org_id': 'orgId',  # noqa: E501
-        's3_uri': 's3Uri',  # noqa: E501
-        'tag': 'tag',  # noqa: E501
+        'verbose': 'verbose',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, org_id, s3_uri, *args, **kwargs):  # noqa: E501
-        """PostAssetRequest - a model defined in OpenAPI
-
-        Args:
-            org_id (str):
-            s3_uri (str):
+    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
+        """TransactionCommitRequest - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -139,15 +131,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            tag (str, none_type): [optional]  # noqa: E501
+            verbose (bool, none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -167,16 +159,14 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.org_id = org_id
-        self.s3_uri = s3_uri
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -189,20 +179,16 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, org_id, s3_uri, *args, **kwargs):  # noqa: E501
-        """PostAssetRequest - a model defined in OpenAPI
-
-        Args:
-            org_id (str):
-            s3_uri (str):
+    def __init__(self, *args, **kwargs):  # noqa: E501
+        """TransactionCommitRequest - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -227,15 +213,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            tag (str, none_type): [optional]  # noqa: E501
+            verbose (bool, none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -253,16 +239,14 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.org_id = org_id
-        self.s3_uri = s3_uri
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `whylabs-client-0.6.2/whylabs_client/model/post_asset_response.py` & `whylabs-client-0.6.3/whylabs_client/model/post_asset_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.2/whylabs_client/model/profile_trace.py` & `whylabs-client-0.6.3/whylabs_client/model/profile_trace.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.2/whylabs_client/model/profile_traces_response.py` & `whylabs-client-0.6.3/whylabs_client/model/profile_traces_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.2/whylabs_client/model/provision_new_aws_marketplace_user_response.py` & `whylabs-client-0.6.3/whylabs_client/model/provision_new_aws_marketplace_user_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.2/whylabs_client/model/provision_new_marketplace_user_request.py` & `whylabs-client-0.6.3/whylabs_client/model/provision_new_marketplace_user_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.2/whylabs_client/model/provision_new_user_request.py` & `whylabs-client-0.6.3/whylabs_client/model/provision_new_user_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.2/whylabs_client/model/provision_new_user_response.py` & `whylabs-client-0.6.3/whylabs_client/model/provision_new_user_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.2/whylabs_client/model/put_account_memberships_request.py` & `whylabs-client-0.6.3/whylabs_client/model/put_account_memberships_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.2/whylabs_client/model/reference_profile_item_response.py` & `whylabs-client-0.6.3/whylabs_client/model/reference_profile_item_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.2/whylabs_client/model/remove_membership_request.py` & `whylabs-client-0.6.3/whylabs_client/model/remove_membership_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.2/whylabs_client/model/response.py` & `whylabs-client-0.6.3/whylabs_client/model/response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.2/whylabs_client/model/revoke_user_session_request.py` & `whylabs-client-0.6.3/whylabs_client/model/revoke_user_session_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.2/whylabs_client/model/role.py` & `whylabs-client-0.6.3/whylabs_client/model/role.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.2/whylabs_client/model/schema_metadata.py` & `whylabs-client-0.6.3/whylabs_client/model/schema_metadata.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.2/whylabs_client/model/search_index_request.py` & `whylabs-client-0.6.3/whylabs_client/model/set_default_membership_request.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,20 +26,16 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from whylabs_client.exceptions import ApiAttributeError
 
 
-def lazy_import():
-    from whylabs_client.model.search_index_type import SearchIndexType
-    globals()['SearchIndexType'] = SearchIndexType
 
-
-class SearchIndexRequest(ModelNormal):
+class SetDefaultMembershipRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -67,58 +63,56 @@
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
-        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
-        lazy_import()
         return {
             'org_id': (str,),  # noqa: E501
-            'type': (SearchIndexType,),  # noqa: E501
+            'user_id': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'org_id': 'orgId',  # noqa: E501
-        'type': 'type',  # noqa: E501
+        'user_id': 'userId',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, org_id, type, *args, **kwargs):  # noqa: E501
-        """SearchIndexRequest - a model defined in OpenAPI
+    def _from_openapi_data(cls, org_id, user_id, *args, **kwargs):  # noqa: E501
+        """SetDefaultMembershipRequest - a model defined in OpenAPI
 
         Args:
             org_id (str):
-            type (SearchIndexType):
+            user_id (str):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -171,15 +165,15 @@
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
         self.org_id = org_id
-        self.type = type
+        self.user_id = user_id
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -192,20 +186,20 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, org_id, type, *args, **kwargs):  # noqa: E501
-        """SearchIndexRequest - a model defined in OpenAPI
+    def __init__(self, org_id, user_id, *args, **kwargs):  # noqa: E501
+        """SetDefaultMembershipRequest - a model defined in OpenAPI
 
         Args:
             org_id (str):
-            type (SearchIndexType):
+            user_id (str):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -256,15 +250,15 @@
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
         self.org_id = org_id
-        self.type = type
+        self.user_id = user_id
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `whylabs-client-0.6.2/whylabs_client/model/search_index_type.py` & `whylabs-client-0.6.3/whylabs_client/model/subscription_tier.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from whylabs_client.exceptions import ApiAttributeError
 
 
 
-class SearchIndexType(ModelSimple):
+class SubscriptionTier(ModelSimple):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -49,18 +49,18 @@
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
     allowed_values = {
         ('value',): {
-            'MODELS': "MODELS",
-            'ACTIONS': "ACTIONS",
-            'ENTITY_SCHEMA': "ENTITY_SCHEMA",
-            'MONITOR_CONFIG': "MONITOR_CONFIG",
+            'FREE': "FREE",
+            'PAID': "PAID",
+            'AWS_MARKETPLACE': "AWS_MARKETPLACE",
+            'SUBSCRIPTION': "SUBSCRIPTION",
         },
     }
 
     validations = {
     }
 
     additional_properties_type = None
@@ -99,23 +99,23 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):
-        """SearchIndexType - a model defined in OpenAPI
+        """SubscriptionTier - a model defined in OpenAPI
 
         Note that value can be passed either in args or in kwargs, but not in both.
 
         Args:
-            args[0] (str):, must be one of ["MODELS", "ACTIONS", "ENTITY_SCHEMA", "MONITOR_CONFIG", ]  # noqa: E501
+            args[0] (str):, must be one of ["FREE", "PAID", "AWS_MARKETPLACE", "SUBSCRIPTION", ]  # noqa: E501
 
         Keyword Args:
-            value (str):, must be one of ["MODELS", "ACTIONS", "ENTITY_SCHEMA", "MONITOR_CONFIG", ]  # noqa: E501
+            value (str):, must be one of ["FREE", "PAID", "AWS_MARKETPLACE", "SUBSCRIPTION", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -189,23 +189,23 @@
                 path_to_item=_path_to_item,
                 valid_classes=(self.__class__,),
             )
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):
-        """SearchIndexType - a model defined in OpenAPI
+        """SubscriptionTier - a model defined in OpenAPI
 
         Note that value can be passed either in args or in kwargs, but not in both.
 
         Args:
-            args[0] (str):, must be one of ["MODELS", "ACTIONS", "ENTITY_SCHEMA", "MONITOR_CONFIG", ]  # noqa: E501
+            args[0] (str):, must be one of ["FREE", "PAID", "AWS_MARKETPLACE", "SUBSCRIPTION", ]  # noqa: E501
 
         Keyword Args:
-            value (str):, must be one of ["MODELS", "ACTIONS", "ENTITY_SCHEMA", "MONITOR_CONFIG", ]  # noqa: E501
+            value (str):, must be one of ["FREE", "PAID", "AWS_MARKETPLACE", "SUBSCRIPTION", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
```

### Comparing `whylabs-client-0.6.2/whylabs_client/model/search_response.py` & `whylabs-client-0.6.3/whylabs_client/model/user.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,20 +26,16 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from whylabs_client.exceptions import ApiAttributeError
 
 
-def lazy_import():
-    from whylabs_client.model.entity_search_result import EntitySearchResult
-    globals()['EntitySearchResult'] = EntitySearchResult
 
-
-class SearchResponse(ModelNormal):
+class User(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -67,57 +63,58 @@
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
-        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
-        lazy_import()
         return {
-            'results': ([EntitySearchResult],),  # noqa: E501
-            'request_id': (str, none_type,),  # noqa: E501
+            'user_id': (str,),  # noqa: E501
+            'email': (str,),  # noqa: E501
+            'preferences': (str, none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'results': 'results',  # noqa: E501
-        'request_id': 'requestId',  # noqa: E501
+        'user_id': 'userId',  # noqa: E501
+        'email': 'email',  # noqa: E501
+        'preferences': 'preferences',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, results, *args, **kwargs):  # noqa: E501
-        """SearchResponse - a model defined in OpenAPI
+    def _from_openapi_data(cls, user_id, email, *args, **kwargs):  # noqa: E501
+        """User - a model defined in OpenAPI
 
         Args:
-            results ([EntitySearchResult]):
+            user_id (str): The id of the user.
+            email (str): The user's email address.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -142,15 +139,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            request_id (str, none_type): [optional]  # noqa: E501
+            preferences (str, none_type): The user's JSON serialized preferences. Schema defined in Dashbird.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -170,15 +167,16 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.results = results
+        self.user_id = user_id
+        self.email = email
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -191,19 +189,20 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, results, *args, **kwargs):  # noqa: E501
-        """SearchResponse - a model defined in OpenAPI
+    def __init__(self, user_id, email, *args, **kwargs):  # noqa: E501
+        """User - a model defined in OpenAPI
 
         Args:
-            results ([EntitySearchResult]):
+            user_id (str): The id of the user.
+            email (str): The user's email address.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -228,15 +227,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            request_id (str, none_type): [optional]  # noqa: E501
+            preferences (str, none_type): The user's JSON serialized preferences. Schema defined in Dashbird.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -254,15 +253,16 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.results = results
+        self.user_id = user_id
+        self.email = email
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `whylabs-client-0.6.2/whylabs_client/model/segment.py` & `whylabs-client-0.6.3/whylabs_client/model/segment.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.2/whylabs_client/model/segment_list_response.py` & `whylabs-client-0.6.3/whylabs_client/model/segment_list_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.2/whylabs_client/model/segment_tag.py` & `whylabs-client-0.6.3/whylabs_client/model/segment_tag.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.2/whylabs_client/model/segment_weight.py` & `whylabs-client-0.6.3/whylabs_client/model/segment_weight.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.2/whylabs_client/model/segments_list_request.py` & `whylabs-client-0.6.3/whylabs_client/model/segments_list_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.2/whylabs_client/model/session_metadata.py` & `whylabs-client-0.6.3/whylabs_client/model/session_metadata.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.2/whylabs_client/model/set_default_membership_request.py` & `whylabs-client-0.6.3/whylabs_client/model/update_membership_request.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,16 +26,20 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from whylabs_client.exceptions import ApiAttributeError
 
 
+def lazy_import():
+    from whylabs_client.model.role import Role
+    globals()['Role'] = Role
 
-class SetDefaultMembershipRequest(ModelNormal):
+
+class UpdateMembershipRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -63,56 +67,61 @@
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
+        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
+        lazy_import()
         return {
             'org_id': (str,),  # noqa: E501
-            'user_id': (str,),  # noqa: E501
+            'email': (str,),  # noqa: E501
+            'role': (Role,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'org_id': 'orgId',  # noqa: E501
-        'user_id': 'userId',  # noqa: E501
+        'email': 'email',  # noqa: E501
+        'role': 'role',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, org_id, user_id, *args, **kwargs):  # noqa: E501
-        """SetDefaultMembershipRequest - a model defined in OpenAPI
+    def _from_openapi_data(cls, org_id, email, role, *args, **kwargs):  # noqa: E501
+        """UpdateMembershipRequest - a model defined in OpenAPI
 
         Args:
             org_id (str):
-            user_id (str):
+            email (str):
+            role (Role):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -165,15 +174,16 @@
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
         self.org_id = org_id
-        self.user_id = user_id
+        self.email = email
+        self.role = role
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -186,20 +196,21 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, org_id, user_id, *args, **kwargs):  # noqa: E501
-        """SetDefaultMembershipRequest - a model defined in OpenAPI
+    def __init__(self, org_id, email, role, *args, **kwargs):  # noqa: E501
+        """UpdateMembershipRequest - a model defined in OpenAPI
 
         Args:
             org_id (str):
-            user_id (str):
+            email (str):
+            role (Role):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -250,15 +261,16 @@
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
         self.org_id = org_id
-        self.user_id = user_id
+        self.email = email
+        self.role = role
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `whylabs-client-0.6.2/whylabs_client/model/slack_notification_action.py` & `whylabs-client-0.6.3/whylabs_client/model/slack_notification_action.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.2/whylabs_client/model/sort_order.py` & `whylabs-client-0.6.3/whylabs_client/model/sort_order.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.2/whylabs_client/model/status_response.py` & `whylabs-client-0.6.3/whylabs_client/model/status_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.2/whylabs_client/model/subscription_product_feature.py` & `whylabs-client-0.6.3/whylabs_client/model/subscription_product_feature.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.2/whylabs_client/model/subscription_product_summary.py` & `whylabs-client-0.6.3/whylabs_client/model/subscription_product_summary.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.2/whylabs_client/model/subscription_summary.py` & `whylabs-client-0.6.3/whylabs_client/model/subscription_summary.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.2/whylabs_client/model/subscription_tier.py` & `whylabs-client-0.6.3/whylabs_client/model/diagnosis_request_status.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from whylabs_client.exceptions import ApiAttributeError
 
 
 
-class SubscriptionTier(ModelSimple):
+class DiagnosisRequestStatus(ModelSimple):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -49,18 +49,17 @@
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
     allowed_values = {
         ('value',): {
-            'FREE': "FREE",
-            'PAID': "PAID",
-            'AWS_MARKETPLACE': "AWS_MARKETPLACE",
-            'SUBSCRIPTION': "SUBSCRIPTION",
+            'PENDING': "PENDING",
+            'COMPLETE': "COMPLETE",
+            'FAILED': "FAILED",
         },
     }
 
     validations = {
     }
 
     additional_properties_type = None
@@ -99,23 +98,23 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):
-        """SubscriptionTier - a model defined in OpenAPI
+        """DiagnosisRequestStatus - a model defined in OpenAPI
 
         Note that value can be passed either in args or in kwargs, but not in both.
 
         Args:
-            args[0] (str):, must be one of ["FREE", "PAID", "AWS_MARKETPLACE", "SUBSCRIPTION", ]  # noqa: E501
+            args[0] (str):, must be one of ["PENDING", "COMPLETE", "FAILED", ]  # noqa: E501
 
         Keyword Args:
-            value (str):, must be one of ["FREE", "PAID", "AWS_MARKETPLACE", "SUBSCRIPTION", ]  # noqa: E501
+            value (str):, must be one of ["PENDING", "COMPLETE", "FAILED", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -189,23 +188,23 @@
                 path_to_item=_path_to_item,
                 valid_classes=(self.__class__,),
             )
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):
-        """SubscriptionTier - a model defined in OpenAPI
+        """DiagnosisRequestStatus - a model defined in OpenAPI
 
         Note that value can be passed either in args or in kwargs, but not in both.
 
         Args:
-            args[0] (str):, must be one of ["FREE", "PAID", "AWS_MARKETPLACE", "SUBSCRIPTION", ]  # noqa: E501
+            args[0] (str):, must be one of ["PENDING", "COMPLETE", "FAILED", ]  # noqa: E501
 
         Keyword Args:
-            value (str):, must be one of ["FREE", "PAID", "AWS_MARKETPLACE", "SUBSCRIPTION", ]  # noqa: E501
+            value (str):, must be one of ["PENDING", "COMPLETE", "FAILED", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
```

### Comparing `whylabs-client-0.6.2/whylabs_client/model/time_period.py` & `whylabs-client-0.6.3/whylabs_client/model/time_period.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.2/whylabs_client/model/transaction_commit_request.py` & `whylabs-client-0.6.3/whylabs_client/model/transaction_start_request.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from whylabs_client.exceptions import ApiAttributeError
 
 
 
-class TransactionCommitRequest(ModelNormal):
+class TransactionStartRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -78,35 +78,38 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'verbose': (bool, none_type,),  # noqa: E501
+            'dataset_id': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'verbose': 'verbose',  # noqa: E501
+        'dataset_id': 'datasetId',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """TransactionCommitRequest - a model defined in OpenAPI
+    def _from_openapi_data(cls, dataset_id, *args, **kwargs):  # noqa: E501
+        """TransactionStartRequest - a model defined in OpenAPI
+
+        Args:
+            dataset_id (str):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -131,15 +134,14 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            verbose (bool, none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -159,14 +161,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.dataset_id = dataset_id
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -179,16 +182,19 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, *args, **kwargs):  # noqa: E501
-        """TransactionCommitRequest - a model defined in OpenAPI
+    def __init__(self, dataset_id, *args, **kwargs):  # noqa: E501
+        """TransactionStartRequest - a model defined in OpenAPI
+
+        Args:
+            dataset_id (str):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -213,15 +219,14 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            verbose (bool, none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -239,14 +244,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.dataset_id = dataset_id
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `whylabs-client-0.6.2/whylabs_client/model/transaction_log_request.py` & `whylabs-client-0.6.3/whylabs_client/model/transaction_log_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.2/whylabs_client/model/transaction_start_request.py` & `whylabs-client-0.6.3/whylabs_client/model/async_diagnosis_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from whylabs_client.exceptions import ApiAttributeError
 
 
 
-class TransactionStartRequest(ModelNormal):
+class AsyncDiagnosisResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -78,38 +78,38 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'dataset_id': (str,),  # noqa: E501
+            'diagnosis_id': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'dataset_id': 'datasetId',  # noqa: E501
+        'diagnosis_id': 'diagnosisId',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, dataset_id, *args, **kwargs):  # noqa: E501
-        """TransactionStartRequest - a model defined in OpenAPI
+    def _from_openapi_data(cls, diagnosis_id, *args, **kwargs):  # noqa: E501
+        """AsyncDiagnosisResponse - a model defined in OpenAPI
 
         Args:
-            dataset_id (str):
+            diagnosis_id (str):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -161,15 +161,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.dataset_id = dataset_id
+        self.diagnosis_id = diagnosis_id
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -182,19 +182,19 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, dataset_id, *args, **kwargs):  # noqa: E501
-        """TransactionStartRequest - a model defined in OpenAPI
+    def __init__(self, diagnosis_id, *args, **kwargs):  # noqa: E501
+        """AsyncDiagnosisResponse - a model defined in OpenAPI
 
         Args:
-            dataset_id (str):
+            diagnosis_id (str):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -244,15 +244,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.dataset_id = dataset_id
+        self.diagnosis_id = diagnosis_id
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `whylabs-client-0.6.2/whylabs_client/model/transaction_status_response.py` & `whylabs-client-0.6.3/whylabs_client/model/transaction_status_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.2/whylabs_client/model/uber_notification_schedule.py` & `whylabs-client-0.6.3/whylabs_client/model/uber_notification_schedule.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.2/whylabs_client/model/update_account_user_request.py` & `whylabs-client-0.6.3/whylabs_client/model/update_account_user_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.2/whylabs_client/model/update_membership_request.py` & `whylabs-client-0.6.3/whylabs_client/model/named_count.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,20 +26,16 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from whylabs_client.exceptions import ApiAttributeError
 
 
-def lazy_import():
-    from whylabs_client.model.role import Role
-    globals()['Role'] = Role
 
-
-class UpdateMembershipRequest(ModelNormal):
+class NamedCount(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -67,61 +63,56 @@
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
-        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
-        lazy_import()
         return {
-            'org_id': (str,),  # noqa: E501
-            'email': (str,),  # noqa: E501
-            'role': (Role,),  # noqa: E501
+            'name': (str,),  # noqa: E501
+            'count': (int,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'org_id': 'orgId',  # noqa: E501
-        'email': 'email',  # noqa: E501
-        'role': 'role',  # noqa: E501
+        'name': 'name',  # noqa: E501
+        'count': 'count',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, org_id, email, role, *args, **kwargs):  # noqa: E501
-        """UpdateMembershipRequest - a model defined in OpenAPI
+    def _from_openapi_data(cls, name, count, *args, **kwargs):  # noqa: E501
+        """NamedCount - a model defined in OpenAPI
 
         Args:
-            org_id (str):
-            email (str):
-            role (Role):
+            name (str):
+            count (int):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -173,17 +164,16 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.org_id = org_id
-        self.email = email
-        self.role = role
+        self.name = name
+        self.count = count
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -196,21 +186,20 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, org_id, email, role, *args, **kwargs):  # noqa: E501
-        """UpdateMembershipRequest - a model defined in OpenAPI
+    def __init__(self, name, count, *args, **kwargs):  # noqa: E501
+        """NamedCount - a model defined in OpenAPI
 
         Args:
-            org_id (str):
-            email (str):
-            role (Role):
+            name (str):
+            count (int):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -260,17 +249,16 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.org_id = org_id
-        self.email = email
-        self.role = role
+        self.name = name
+        self.count = count
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `whylabs-client-0.6.2/whylabs_client/model/upload_asset_request.py` & `whylabs-client-0.6.3/whylabs_client/model/upload_asset_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.2/whylabs_client/model/upload_asset_response.py` & `whylabs-client-0.6.3/whylabs_client/model/upload_asset_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.2/whylabs_client/model/user.py` & `whylabs-client-0.6.3/whylabs_client/model/diagnosis_request.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,16 +26,20 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from whylabs_client.exceptions import ApiAttributeError
 
 
+def lazy_import():
+    from whylabs_client.model.segment import Segment
+    globals()['Segment'] = Segment
 
-class User(ModelNormal):
+
+class DiagnosisRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -63,58 +67,67 @@
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
+        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
+        lazy_import()
         return {
-            'user_id': (str,),  # noqa: E501
-            'email': (str,),  # noqa: E501
-            'preferences': (str, none_type,),  # noqa: E501
+            'dataset_id': (str,),  # noqa: E501
+            'analyzer_id': (str,),  # noqa: E501
+            'segment': (Segment,),  # noqa: E501
+            'interval': (str,),  # noqa: E501
+            'columns': ([str],),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'user_id': 'userId',  # noqa: E501
-        'email': 'email',  # noqa: E501
-        'preferences': 'preferences',  # noqa: E501
+        'dataset_id': 'datasetId',  # noqa: E501
+        'analyzer_id': 'analyzerId',  # noqa: E501
+        'segment': 'segment',  # noqa: E501
+        'interval': 'interval',  # noqa: E501
+        'columns': 'columns',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, user_id, email, *args, **kwargs):  # noqa: E501
-        """User - a model defined in OpenAPI
+    def _from_openapi_data(cls, dataset_id, analyzer_id, segment, interval, columns, *args, **kwargs):  # noqa: E501
+        """DiagnosisRequest - a model defined in OpenAPI
 
         Args:
-            user_id (str): The id of the user.
-            email (str): The user's email address.
+            dataset_id (str):
+            analyzer_id (str):
+            segment (Segment):
+            interval (str):
+            columns ([str]):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -139,15 +152,14 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            preferences (str, none_type): The user's JSON serialized preferences. Schema defined in Dashbird.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -167,16 +179,19 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.user_id = user_id
-        self.email = email
+        self.dataset_id = dataset_id
+        self.analyzer_id = analyzer_id
+        self.segment = segment
+        self.interval = interval
+        self.columns = columns
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -189,20 +204,23 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, user_id, email, *args, **kwargs):  # noqa: E501
-        """User - a model defined in OpenAPI
+    def __init__(self, dataset_id, analyzer_id, segment, interval, columns, *args, **kwargs):  # noqa: E501
+        """DiagnosisRequest - a model defined in OpenAPI
 
         Args:
-            user_id (str): The id of the user.
-            email (str): The user's email address.
+            dataset_id (str):
+            analyzer_id (str):
+            segment (Segment):
+            interval (str):
+            columns ([str]):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -227,15 +245,14 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            preferences (str, none_type): The user's JSON serialized preferences. Schema defined in Dashbird.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -253,16 +270,19 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.user_id = user_id
-        self.email = email
+        self.dataset_id = dataset_id
+        self.analyzer_id = analyzer_id
+        self.segment = segment
+        self.interval = interval
+        self.columns = columns
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `whylabs-client-0.6.2/whylabs_client/model/user_api_key.py` & `whylabs-client-0.6.3/whylabs_client/model/user_api_key.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.2/whylabs_client/model/user_api_key_response.py` & `whylabs-client-0.6.3/whylabs_client/model/user_api_key_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.2/whylabs_client/model/validate_user_session_response.py` & `whylabs-client-0.6.3/whylabs_client/model/validate_user_session_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.2/whylabs_client/model_utils.py` & `whylabs-client-0.6.3/whylabs_client/model_utils.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.2/whylabs_client/models/__init__.py` & `whylabs-client-0.6.3/whylabs_client/models/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,55 +18,65 @@
 from whylabs_client.model.add_membership_request import AddMembershipRequest
 from whylabs_client.model.add_policy_response import AddPolicyResponse
 from whylabs_client.model.admin_report_response import AdminReportResponse
 from whylabs_client.model.admin_report_type import AdminReportType
 from whylabs_client.model.analysis_results_record import AnalysisResultsRecord
 from whylabs_client.model.analysis_results_request import AnalysisResultsRequest
 from whylabs_client.model.analysis_results_response import AnalysisResultsResponse
+from whylabs_client.model.analysis_results_summary import AnalysisResultsSummary
 from whylabs_client.model.analyzer_diagnostic_record import AnalyzerDiagnosticRecord
 from whylabs_client.model.analyzer_failure_record import AnalyzerFailureRecord
 from whylabs_client.model.analyzer_segment_column_diagnostic_record import AnalyzerSegmentColumnDiagnosticRecord
 from whylabs_client.model.analyzer_segment_columns_diagnostic_request import AnalyzerSegmentColumnsDiagnosticRequest
 from whylabs_client.model.analyzer_segment_columns_diagnostic_response import AnalyzerSegmentColumnsDiagnosticResponse
 from whylabs_client.model.analyzer_segment_diagnostic_record import AnalyzerSegmentDiagnosticRecord
 from whylabs_client.model.analyzer_segment_failure_record import AnalyzerSegmentFailureRecord
 from whylabs_client.model.analyzer_segments_diagnostic_request import AnalyzerSegmentsDiagnosticRequest
 from whylabs_client.model.analyzer_segments_diagnostic_response import AnalyzerSegmentsDiagnosticResponse
 from whylabs_client.model.analyzers_diagnostic_request import AnalyzersDiagnosticRequest
 from whylabs_client.model.analyzers_diagnostic_response import AnalyzersDiagnosticResponse
+from whylabs_client.model.anomaly_record import AnomalyRecord
+from whylabs_client.model.async_diagnosis_response import AsyncDiagnosisResponse
+from whylabs_client.model.async_diagnosis_result_response import AsyncDiagnosisResultResponse
 from whylabs_client.model.async_log_response import AsyncLogResponse
 from whylabs_client.model.azure_marketplace_contact_payload import AzureMarketplaceContactPayload
 from whylabs_client.model.azure_marketplace_subscription_details import AzureMarketplaceSubscriptionDetails
 from whylabs_client.model.batch_log_reference_request import BatchLogReferenceRequest
 from whylabs_client.model.batch_log_session_reference_response import BatchLogSessionReferenceResponse
+from whylabs_client.model.batches_summary import BatchesSummary
 from whylabs_client.model.cache_key_type import CacheKeyType
 from whylabs_client.model.column_schema import ColumnSchema
+from whylabs_client.model.condition_record import ConditionRecord
 from whylabs_client.model.create_account_user_request import CreateAccountUserRequest
 from whylabs_client.model.create_dataset_profile_upload_response import CreateDatasetProfileUploadResponse
 from whylabs_client.model.create_reference_profile_request import CreateReferenceProfileRequest
 from whylabs_client.model.create_reference_profile_response import CreateReferenceProfileResponse
 from whylabs_client.model.create_session_request import CreateSessionRequest
 from whylabs_client.model.create_session_response import CreateSessionResponse
 from whylabs_client.model.create_user_request import CreateUserRequest
 from whylabs_client.model.debug_event import DebugEvent
 from whylabs_client.model.delete_analyzer_result import DeleteAnalyzerResult
 from whylabs_client.model.delete_analyzer_results_response import DeleteAnalyzerResultsResponse
 from whylabs_client.model.delete_dataset_profiles_response import DeleteDatasetProfilesResponse
 from whylabs_client.model.delete_profile import DeleteProfile
 from whylabs_client.model.deletion_status import DeletionStatus
+from whylabs_client.model.diagnosis_report import DiagnosisReport
+from whylabs_client.model.diagnosis_request import DiagnosisRequest
+from whylabs_client.model.diagnosis_request_status import DiagnosisRequestStatus
+from whylabs_client.model.diagnostic_data_summary import DiagnosticDataSummary
 from whylabs_client.model.diagnostic_interval_request import DiagnosticIntervalRequest
 from whylabs_client.model.diagnostic_interval_response import DiagnosticIntervalResponse
 from whylabs_client.model.email_notification_action import EmailNotificationAction
 from whylabs_client.model.entity_schema import EntitySchema
-from whylabs_client.model.entity_search_result import EntitySearchResult
 from whylabs_client.model.entity_weight_record import EntityWeightRecord
 from whylabs_client.model.entity_weight_record_metadata import EntityWeightRecordMetadata
 from whylabs_client.model.error_status import ErrorStatus
 from whylabs_client.model.export_trace_partial_success import ExportTracePartialSuccess
 from whylabs_client.model.export_trace_service_response import ExportTraceServiceResponse
+from whylabs_client.model.failure_record import FailureRecord
 from whylabs_client.model.feature_flags import FeatureFlags
 from whylabs_client.model.get_account_memberships_response import GetAccountMembershipsResponse
 from whylabs_client.model.get_asset_response import GetAssetResponse
 from whylabs_client.model.get_dataset_metadata_response import GetDatasetMetadataResponse
 from whylabs_client.model.get_default_membership_response import GetDefaultMembershipResponse
 from whylabs_client.model.get_marketplace_metadata_response import GetMarketplaceMetadataResponse
 from whylabs_client.model.get_memberships_response import GetMembershipsResponse
@@ -85,50 +95,53 @@
 from whylabs_client.model.log_session_reference_response import LogSessionReferenceResponse
 from whylabs_client.model.log_transaction_metadata import LogTransactionMetadata
 from whylabs_client.model.marketplace_dimensions import MarketplaceDimensions
 from whylabs_client.model.member import Member
 from whylabs_client.model.membership import Membership
 from whylabs_client.model.membership_metadata import MembershipMetadata
 from whylabs_client.model.metric_schema import MetricSchema
+from whylabs_client.model.metric_schema_fields import MetricSchemaFields
 from whylabs_client.model.metric_timeseries_record import MetricTimeseriesRecord
 from whylabs_client.model.metric_timeseries_request import MetricTimeseriesRequest
 from whylabs_client.model.metric_timeseries_response import MetricTimeseriesResponse
 from whylabs_client.model.model_metadata_response import ModelMetadataResponse
 from whylabs_client.model.model_type import ModelType
 from whylabs_client.model.monitor_config_version import MonitorConfigVersion
+from whylabs_client.model.named_count import NamedCount
+from whylabs_client.model.named_metric_schema import NamedMetricSchema
 from whylabs_client.model.notification_action import NotificationAction
 from whylabs_client.model.notification_action_payload import NotificationActionPayload
 from whylabs_client.model.notification_relationship_item import NotificationRelationshipItem
 from whylabs_client.model.notification_relationship_type import NotificationRelationshipType
 from whylabs_client.model.notification_settings import NotificationSettings
 from whylabs_client.model.notification_settings_day import NotificationSettingsDay
 from whylabs_client.model.notification_sqs_message_cadence import NotificationSqsMessageCadence
 from whylabs_client.model.organization_metadata import OrganizationMetadata
 from whylabs_client.model.organization_role_members import OrganizationRoleMembers
 from whylabs_client.model.organization_summary import OrganizationSummary
 from whylabs_client.model.pager_duty_notification_action import PagerDutyNotificationAction
 from whylabs_client.model.patch_account_memberships_request import PatchAccountMembershipsRequest
 from whylabs_client.model.post_asset_request import PostAssetRequest
 from whylabs_client.model.post_asset_response import PostAssetResponse
+from whylabs_client.model.profile_summary import ProfileSummary
 from whylabs_client.model.profile_trace import ProfileTrace
 from whylabs_client.model.profile_traces_response import ProfileTracesResponse
 from whylabs_client.model.provision_new_aws_marketplace_user_response import ProvisionNewAWSMarketplaceUserResponse
 from whylabs_client.model.provision_new_marketplace_user_request import ProvisionNewMarketplaceUserRequest
 from whylabs_client.model.provision_new_user_request import ProvisionNewUserRequest
 from whylabs_client.model.provision_new_user_response import ProvisionNewUserResponse
 from whylabs_client.model.put_account_memberships_request import PutAccountMembershipsRequest
+from whylabs_client.model.quality_issue_record import QualityIssueRecord
 from whylabs_client.model.reference_profile_item_response import ReferenceProfileItemResponse
 from whylabs_client.model.remove_membership_request import RemoveMembershipRequest
 from whylabs_client.model.response import Response
+from whylabs_client.model.result_record import ResultRecord
 from whylabs_client.model.revoke_user_session_request import RevokeUserSessionRequest
 from whylabs_client.model.role import Role
 from whylabs_client.model.schema_metadata import SchemaMetadata
-from whylabs_client.model.search_index_request import SearchIndexRequest
-from whylabs_client.model.search_index_type import SearchIndexType
-from whylabs_client.model.search_response import SearchResponse
 from whylabs_client.model.segment import Segment
 from whylabs_client.model.segment_list_response import SegmentListResponse
 from whylabs_client.model.segment_tag import SegmentTag
 from whylabs_client.model.segment_weight import SegmentWeight
 from whylabs_client.model.segments_list_request import SegmentsListRequest
 from whylabs_client.model.session_metadata import SessionMetadata
 from whylabs_client.model.set_default_membership_request import SetDefaultMembershipRequest
```

### Comparing `whylabs-client-0.6.2/whylabs_client/rest.py` & `whylabs-client-0.6.3/whylabs_client/rest.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.6.2/whylabs_client.egg-info/PKG-INFO` & `whylabs-client-0.6.3/whylabs_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whylabs-client
-Version: 0.6.2
+Version: 0.6.3
 Summary: WhyLabs API client
 Home-page: UNKNOWN
 Author: WhyLabs
 Author-email: support@whylabs.ai
 License: Apache License 2.0
 Keywords: OpenAPI,OpenAPI-Generator,WhyLabs API client
 Platform: UNKNOWN
```

### Comparing `whylabs-client-0.6.2/whylabs_client.egg-info/SOURCES.txt` & `whylabs-client-0.6.3/whylabs_client.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 whylabs_client.egg-info/SOURCES.txt
 whylabs_client.egg-info/dependency_links.txt
 whylabs_client.egg-info/requires.txt
 whylabs_client.egg-info/top_level.txt
 whylabs_client/api/__init__.py
 whylabs_client/api/api_key_api.py
 whylabs_client/api/assets_api.py
+whylabs_client/api/container_diagnostics_api.py
 whylabs_client/api/data_api.py
 whylabs_client/api/dataset_metadata_api.py
 whylabs_client/api/dataset_profile_api.py
 whylabs_client/api/debug_events_api.py
 whylabs_client/api/feature_weights_api.py
 whylabs_client/api/log_api.py
 whylabs_client/api/membership_api.py
@@ -42,56 +43,66 @@
 whylabs_client/model/add_membership_request.py
 whylabs_client/model/add_policy_response.py
 whylabs_client/model/admin_report_response.py
 whylabs_client/model/admin_report_type.py
 whylabs_client/model/analysis_results_record.py
 whylabs_client/model/analysis_results_request.py
 whylabs_client/model/analysis_results_response.py
+whylabs_client/model/analysis_results_summary.py
 whylabs_client/model/analyzer_diagnostic_record.py
 whylabs_client/model/analyzer_failure_record.py
 whylabs_client/model/analyzer_segment_column_diagnostic_record.py
 whylabs_client/model/analyzer_segment_columns_diagnostic_request.py
 whylabs_client/model/analyzer_segment_columns_diagnostic_response.py
 whylabs_client/model/analyzer_segment_diagnostic_record.py
 whylabs_client/model/analyzer_segment_failure_record.py
 whylabs_client/model/analyzer_segments_diagnostic_request.py
 whylabs_client/model/analyzer_segments_diagnostic_response.py
 whylabs_client/model/analyzers_diagnostic_request.py
 whylabs_client/model/analyzers_diagnostic_response.py
+whylabs_client/model/anomaly_record.py
+whylabs_client/model/async_diagnosis_response.py
+whylabs_client/model/async_diagnosis_result_response.py
 whylabs_client/model/async_log_response.py
 whylabs_client/model/aws_marketplace_metadata.py
 whylabs_client/model/azure_marketplace_contact_payload.py
 whylabs_client/model/azure_marketplace_subscription_details.py
 whylabs_client/model/batch_log_reference_request.py
 whylabs_client/model/batch_log_session_reference_response.py
+whylabs_client/model/batches_summary.py
 whylabs_client/model/cache_key_type.py
 whylabs_client/model/column_schema.py
+whylabs_client/model/condition_record.py
 whylabs_client/model/create_account_user_request.py
 whylabs_client/model/create_dataset_profile_upload_response.py
 whylabs_client/model/create_reference_profile_request.py
 whylabs_client/model/create_reference_profile_response.py
 whylabs_client/model/create_session_request.py
 whylabs_client/model/create_session_response.py
 whylabs_client/model/create_user_request.py
 whylabs_client/model/debug_event.py
 whylabs_client/model/delete_analyzer_result.py
 whylabs_client/model/delete_analyzer_results_response.py
 whylabs_client/model/delete_dataset_profiles_response.py
 whylabs_client/model/delete_profile.py
 whylabs_client/model/deletion_status.py
+whylabs_client/model/diagnosis_report.py
+whylabs_client/model/diagnosis_request.py
+whylabs_client/model/diagnosis_request_status.py
+whylabs_client/model/diagnostic_data_summary.py
 whylabs_client/model/diagnostic_interval_request.py
 whylabs_client/model/diagnostic_interval_response.py
 whylabs_client/model/email_notification_action.py
 whylabs_client/model/entity_schema.py
-whylabs_client/model/entity_search_result.py
 whylabs_client/model/entity_weight_record.py
 whylabs_client/model/entity_weight_record_metadata.py
 whylabs_client/model/error_status.py
 whylabs_client/model/export_trace_partial_success.py
 whylabs_client/model/export_trace_service_response.py
+whylabs_client/model/failure_record.py
 whylabs_client/model/feature_flags.py
 whylabs_client/model/get_account_memberships_response.py
 whylabs_client/model/get_asset_response.py
 whylabs_client/model/get_dataset_metadata_response.py
 whylabs_client/model/get_default_membership_response.py
 whylabs_client/model/get_marketplace_metadata_response.py
 whylabs_client/model/get_memberships_response.py
@@ -110,50 +121,53 @@
 whylabs_client/model/log_session_reference_response.py
 whylabs_client/model/log_transaction_metadata.py
 whylabs_client/model/marketplace_dimensions.py
 whylabs_client/model/member.py
 whylabs_client/model/membership.py
 whylabs_client/model/membership_metadata.py
 whylabs_client/model/metric_schema.py
+whylabs_client/model/metric_schema_fields.py
 whylabs_client/model/metric_timeseries_record.py
 whylabs_client/model/metric_timeseries_request.py
 whylabs_client/model/metric_timeseries_response.py
 whylabs_client/model/model_metadata_response.py
 whylabs_client/model/model_type.py
 whylabs_client/model/monitor_config_version.py
+whylabs_client/model/named_count.py
+whylabs_client/model/named_metric_schema.py
 whylabs_client/model/notification_action.py
 whylabs_client/model/notification_action_payload.py
 whylabs_client/model/notification_relationship_item.py
 whylabs_client/model/notification_relationship_type.py
 whylabs_client/model/notification_settings.py
 whylabs_client/model/notification_settings_day.py
 whylabs_client/model/notification_sqs_message_cadence.py
 whylabs_client/model/organization_metadata.py
 whylabs_client/model/organization_role_members.py
 whylabs_client/model/organization_summary.py
 whylabs_client/model/pager_duty_notification_action.py
 whylabs_client/model/patch_account_memberships_request.py
 whylabs_client/model/post_asset_request.py
 whylabs_client/model/post_asset_response.py
+whylabs_client/model/profile_summary.py
 whylabs_client/model/profile_trace.py
 whylabs_client/model/profile_traces_response.py
 whylabs_client/model/provision_new_aws_marketplace_user_response.py
 whylabs_client/model/provision_new_marketplace_user_request.py
 whylabs_client/model/provision_new_user_request.py
 whylabs_client/model/provision_new_user_response.py
 whylabs_client/model/put_account_memberships_request.py
+whylabs_client/model/quality_issue_record.py
 whylabs_client/model/reference_profile_item_response.py
 whylabs_client/model/remove_membership_request.py
 whylabs_client/model/response.py
+whylabs_client/model/result_record.py
 whylabs_client/model/revoke_user_session_request.py
 whylabs_client/model/role.py
 whylabs_client/model/schema_metadata.py
-whylabs_client/model/search_index_request.py
-whylabs_client/model/search_index_type.py
-whylabs_client/model/search_response.py
 whylabs_client/model/segment.py
 whylabs_client/model/segment_list_response.py
 whylabs_client/model/segment_tag.py
 whylabs_client/model/segment_weight.py
 whylabs_client/model/segments_list_request.py
 whylabs_client/model/session_metadata.py
 whylabs_client/model/set_default_membership_request.py
```


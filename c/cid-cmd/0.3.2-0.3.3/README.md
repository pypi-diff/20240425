# Comparing `tmp/cid_cmd-0.3.2.tar.gz` & `tmp/cid_cmd-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cid_cmd-0.3.2.tar", last modified: Tue Apr 23 12:14:57 2024, max compression
+gzip compressed data, was "cid_cmd-0.3.3.tar", last modified: Thu Apr 25 09:08:11 2024, max compression
```

## Comparing `cid_cmd-0.3.2.tar` & `cid_cmd-0.3.3.tar`

### file list

```diff
@@ -1,156 +1,156 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:14:57.397546 cid_cmd-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-23 12:14:53.000000 cid_cmd-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-23 12:14:53.000000 cid_cmd-0.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     9475 2024-04-23 12:14:57.397546 cid_cmd-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8560 2024-04-23 12:14:53.000000 cid_cmd-0.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:14:57.377546 cid_cmd-0.3.2/cid/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-23 12:14:53.000000 cid_cmd-0.3.2/cid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-23 12:14:53.000000 cid_cmd-0.3.2/cid/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     1872 2024-04-23 12:14:53.000000 cid_cmd-0.3.2/cid/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:14:57.377546 cid_cmd-0.3.2/cid/builtin/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-23 12:14:53.000000 cid_cmd-0.3.2/cid/builtin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:14:57.377546 cid_cmd-0.3.2/cid/builtin/core/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-23 12:14:53.000000 cid_cmd-0.3.2/cid/builtin/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:14:57.377546 cid_cmd-0.3.2/cid/builtin/core/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:14:57.369547 cid_cmd-0.3.2/cid/builtin/core/data/datasets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:14:57.377546 cid_cmd-0.3.2/cid/builtin/core/data/datasets/cid/
--rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-04-23 12:14:53.000000 cid_cmd-0.3.2/cid/builtin/core/data/datasets/cid/compute.json
--rw-r--r--   0 runner    (1001) docker     (127)     2893 2024-04-23 12:14:53.000000 cid_cmd-0.3.2/cid/builtin/core/data/datasets/cid/ec2_running_cost.json
--rw-r--r--   0 runner    (1001) docker     (127)     3777 2024-04-23 12:14:53.000000 cid_cmd-0.3.2/cid/builtin/core/data/datasets/cid/s3_view.json
--rw-r--r--   0 runner    (1001) docker     (127)     8825 2024-04-23 12:14:53.000000 cid_cmd-0.3.2/cid/builtin/core/data/datasets/cid/summary_view.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:14:57.377546 cid_cmd-0.3.2/cid/builtin/core/data/datasets/co/
--rw-r--r--   0 runner    (1001) docker     (127)     9276 2024-04-23 12:14:53.000000 cid_cmd-0.3.2/cid/builtin/core/data/datasets/co/dataset.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:14:57.377546 cid_cmd-0.3.2/cid/builtin/core/data/datasets/cudos/
--rw-r--r--   0 runner    (1001) docker     (127)     6223 2024-04-23 12:14:53.000000 cid_cmd-0.3.2/cid/builtin/core/data/datasets/cudos/hourly_view.json
--rw-r--r--   0 runner    (1001) docker     (127)     8610 2024-04-23 12:14:53.000000 cid_cmd-0.3.2/cid/builtin/core/data/datasets/cudos/resource_view.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:14:57.377546 cid_cmd-0.3.2/cid/builtin/core/data/datasets/kpi/
--rw-r--r--   0 runner    (1001) docker     (127)     3353 2024-04-23 12:14:53.000000 cid_cmd-0.3.2/cid/builtin/core/data/datasets/kpi/kpi_ebs_snap.json
--rw-r--r--   0 runner    (1001) docker     (127)     5069 2024-04-23 12:14:53.000000 cid_cmd-0.3.2/cid/builtin/core/data/datasets/kpi/kpi_ebs_storage_all.json
--rw-r--r--   0 runner    (1001) docker     (127)    20695 2024-04-23 12:14:53.000000 cid_cmd-0.3.2/cid/builtin/core/data/datasets/kpi/kpi_instance_all.json
--rw-r--r--   0 runner    (1001) docker     (127)    11136 2024-04-23 12:14:53.000000 cid_cmd-0.3.2/cid/builtin/core/data/datasets/kpi/kpi_s3_storage_all.json
--rw-r--r--   0 runner    (1001) docker     (127)    15746 2024-04-23 12:14:53.000000 cid_cmd-0.3.2/cid/builtin/core/data/datasets/kpi/kpi_tracker.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:14:57.377546 cid_cmd-0.3.2/cid/builtin/core/data/datasets/shared/
--rw-r--r--   0 runner    (1001) docker     (127)    30612 2024-04-23 12:14:53.000000 cid_cmd-0.3.2/cid/builtin/core/data/datasets/shared/customer_all.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:14:57.377546 cid_cmd-0.3.2/cid/builtin/core/data/datasets/tao/
--rw-r--r--   0 runner    (1001) docker     (127)    69315 2024-04-23 12:14:53.000000 cid_cmd-0.3.2/cid/builtin/core/data/datasets/tao/dataset.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:14:57.381546 cid_cmd-0.3.2/cid/builtin/core/data/datasets/trends/
--rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-04-23 12:14:53.000000 cid_cmd-0.3.2/cid/builtin/core/data/datasets/trends/daily_anomaly_detection.json
--rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-04-23 12:14:53.000000 cid_cmd-0.3.2/cid/builtin/core/data/datasets/trends/monthly_anomaly_detection.json
--rw-r--r--   0 runner    (1001) docker     (127)     4681 2024-04-23 12:14:53.000000 cid_cmd-0.3.2/cid/builtin/core/data/datasets/trends/monthly_bill_by_account.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:14:57.381546 cid_cmd-0.3.2/cid/builtin/core/data/permissions/
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-23 12:14:53.000000 cid_cmd-0.3.2/cid/builtin/core/data/permissions/dashboard_permissions.json
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-23 12:14:53.000000 cid_cmd-0.3.2/cid/builtin/core/data/permissions/dashboard_permissions_namespace.json
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-23 12:14:53.000000 cid_cmd-0.3.2/cid/builtin/core/data/permissions/data_set_permissions.json
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-23 12:14:53.000000 cid_cmd-0.3.2/cid/builtin/core/data/permissions/data_source_permissions.json
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-04-23 12:14:53.000000 cid_cmd-0.3.2/cid/builtin/core/data/permissions/folder_permissions.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:14:57.373546 cid_cmd-0.3.2/cid/builtin/core/data/queries/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:14:57.381546 cid_cmd-0.3.2/cid/builtin/core/data/queries/cid/
--rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-04-23 12:14:53.000000 cid_cmd-0.3.2/cid/builtin/core/data/queries/cid/compute_savings_plan_eligible_spend.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-04-23 12:14:53.000000 cid_cmd-0.3.2/cid/builtin/core/data/queries/cid/ec2_running_cost.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-04-23 12:14:53.000000 cid_cmd-0.3.2/cid/builtin/core/data/queries/cid/ec2_running_cost_ri.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-04-23 12:14:53.000000 cid_cmd-0.3.2/cid/builtin/core/data/queries/cid/ec2_running_cost_sp.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-04-23 12:14:53.000000 cid_cmd-0.3.2/cid/builtin/core/data/queries/cid/ec2_running_cost_sp_ri.sql
--rw-r--r--   0 runner    (1001) docker     (127)     2942 2024-04-23 12:14:53.000000 cid_cmd-0.3.2/cid/builtin/core/data/queries/cid/ri_sp_mapping.sql
--rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-04-23 12:14:53.000000 cid_cmd-0.3.2/cid/builtin/core/data/queries/cid/ri_sp_mapping_ri.sql
--rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-04-23 12:14:53.000000 cid_cmd-0.3.2/cid/builtin/core/data/queries/cid/ri_sp_mapping_sp.sql
--rw-r--r--   0 runner    (1001) docker     (127)     3134 2024-04-23 12:14:53.000000 cid_cmd-0.3.2/cid/builtin/core/data/queries/cid/ri_sp_mapping_sp_ri.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-04-23 12:14:53.000000 cid_cmd-0.3.2/cid/builtin/core/data/queries/cid/s3.sql
--rw-r--r--   0 runner    (1001) docker     (127)     5808 2024-04-23 12:14:53.000000 cid_cmd-0.3.2/cid/builtin/core/data/queries/cid/summary_view.sql
--rw-r--r--   0 runner    (1001) docker     (127)     5533 2024-04-23 12:14:53.000000 cid_cmd-0.3.2/cid/builtin/core/data/queries/cid/summary_view_ri.sql
--rw-r--r--   0 runner    (1001) docker     (127)     5589 2024-04-23 12:14:53.000000 cid_cmd-0.3.2/cid/builtin/core/data/queries/cid/summary_view_sp.sql
--rw-r--r--   0 runner    (1001) docker     (127)     5599 2024-04-23 12:14:53.000000 cid_cmd-0.3.2/cid/builtin/core/data/queries/cid/summary_view_sp_ri.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:14:57.385546 cid_cmd-0.3.2/cid/builtin/core/data/queries/co/
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-23 12:14:53.000000 cid_cmd-0.3.2/cid/builtin/core/data/queries/co/all_options.sql
--rw-r--r--   0 runner    (1001) docker     (127)    14711 2024-04-23 12:14:53.000000 cid_cmd-0.3.2/cid/builtin/core/data/queries/co/auto_scale.json
--rw-r--r--   0 runner    (1001) docker     (127)    27919 2024-04-23 12:14:53.000000 cid_cmd-0.3.2/cid/builtin/core/data/queries/co/auto_scale_options.sql
--rw-r--r--   0 runner    (1001) docker     (127)     9097 2024-04-23 12:14:53.000000 cid_cmd-0.3.2/cid/builtin/core/data/queries/co/ebs_volume.json
--rw-r--r--   0 runner    (1001) docker     (127)    22473 2024-04-23 12:14:53.000000 cid_cmd-0.3.2/cid/builtin/core/data/queries/co/ebs_volume_options.sql
--rw-r--r--   0 runner    (1001) docker     (127)    19144 2024-04-23 12:14:53.000000 cid_cmd-0.3.2/cid/builtin/core/data/queries/co/ec2_instance.json
--rw-r--r--   0 runner    (1001) docker     (127)    28308 2024-04-23 12:14:53.000000 cid_cmd-0.3.2/cid/builtin/core/data/queries/co/ec2_instance_options.sql
--rw-r--r--   0 runner    (1001) docker     (127)     8029 2024-04-23 12:14:53.000000 cid_cmd-0.3.2/cid/builtin/core/data/queries/co/lambda.json
--rw-r--r--   0 runner    (1001) docker     (127)    15340 2024-04-23 12:14:53.000000 cid_cmd-0.3.2/cid/builtin/core/data/queries/co/lambda_options.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:14:57.385546 cid_cmd-0.3.2/cid/builtin/core/data/queries/cudos/
--rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-04-23 12:14:53.000000 cid_cmd-0.3.2/cid/builtin/core/data/queries/cudos/hourly_view.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-23 12:14:53.000000 cid_cmd-0.3.2/cid/builtin/core/data/queries/cudos/hourly_view_ri.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-04-23 12:14:53.000000 cid_cmd-0.3.2/cid/builtin/core/data/queries/cudos/hourly_view_sp.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-04-23 12:14:53.000000 cid_cmd-0.3.2/cid/builtin/core/data/queries/cudos/hourly_view_sp_ri.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1989 2024-04-23 12:14:53.000000 cid_cmd-0.3.2/cid/builtin/core/data/queries/cudos/resource_view.sql
--rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-04-23 12:14:53.000000 cid_cmd-0.3.2/cid/builtin/core/data/queries/cudos/resource_view_ri.sql
--rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-04-23 12:14:53.000000 cid_cmd-0.3.2/cid/builtin/core/data/queries/cudos/resource_view_sp.sql
--rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-04-23 12:14:53.000000 cid_cmd-0.3.2/cid/builtin/core/data/queries/cudos/resource_view_sp_ri.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:14:57.389546 cid_cmd-0.3.2/cid/builtin/core/data/queries/kpi/
--rw-r--r--   0 runner    (1001) docker     (127)    11145 2024-04-23 12:14:53.000000 cid_cmd-0.3.2/cid/builtin/core/data/queries/kpi/first_kpi_instance_mapping_view.sql
--rw-r--r--   0 runner    (1001) docker     (127)     3187 2024-04-23 12:14:53.000000 cid_cmd-0.3.2/cid/builtin/core/data/queries/kpi/kpi_ebs_snap_view.sql
--rw-r--r--   0 runner    (1001) docker     (127)     6192 2024-04-23 12:14:53.000000 cid_cmd-0.3.2/cid/builtin/core/data/queries/kpi/kpi_ebs_storage_view.sql
--rw-r--r--   0 runner    (1001) docker     (127)    24337 2024-04-23 12:14:53.000000 cid_cmd-0.3.2/cid/builtin/core/data/queries/kpi/kpi_instance_all_view.sql
--rw-r--r--   0 runner    (1001) docker     (127)    23573 2024-04-23 12:14:53.000000 cid_cmd-0.3.2/cid/builtin/core/data/queries/kpi/kpi_instance_all_view_noRI.sql
--rw-r--r--   0 runner    (1001) docker     (127)    22559 2024-04-23 12:14:53.000000 cid_cmd-0.3.2/cid/builtin/core/data/queries/kpi/kpi_instance_all_view_noRISP.sql
--rw-r--r--   0 runner    (1001) docker     (127)    23434 2024-04-23 12:14:53.000000 cid_cmd-0.3.2/cid/builtin/core/data/queries/kpi/kpi_instance_all_view_noSP.sql
--rw-r--r--   0 runner    (1001) docker     (127)    11256 2024-04-23 12:14:53.000000 cid_cmd-0.3.2/cid/builtin/core/data/queries/kpi/kpi_s3_storage_view.sql
--rw-r--r--   0 runner    (1001) docker     (127)     9226 2024-04-23 12:14:53.000000 cid_cmd-0.3.2/cid/builtin/core/data/queries/kpi/last_kpi_tracker_view.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:14:57.389546 cid_cmd-0.3.2/cid/builtin/core/data/queries/shared/
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-23 12:14:53.000000 cid_cmd-0.3.2/cid/builtin/core/data/queries/shared/account_map.sql
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-23 12:14:53.000000 cid_cmd-0.3.2/cid/builtin/core/data/queries/shared/account_map_dummy.sql
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-23 12:14:53.000000 cid_cmd-0.3.2/cid/builtin/core/data/queries/shared/aws_accounts.sql
--rw-r--r--   0 runner    (1001) docker     (127)     2731 2024-04-23 12:14:53.000000 cid_cmd-0.3.2/cid/builtin/core/data/queries/shared/aws_regions.sql
--rw-r--r--   0 runner    (1001) docker     (127)     7282 2024-04-23 12:14:53.000000 cid_cmd-0.3.2/cid/builtin/core/data/queries/shared/aws_service_category_map.sql
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-23 12:14:53.000000 cid_cmd-0.3.2/cid/builtin/core/data/queries/shared/business_units_map.sql
--rw-r--r--   0 runner    (1001) docker     (127)     5043 2024-04-23 12:14:53.000000 cid_cmd-0.3.2/cid/builtin/core/data/queries/shared/cur.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-23 12:14:53.000000 cid_cmd-0.3.2/cid/builtin/core/data/queries/shared/payer_account_name_map.sql
--rw-r--r--   0 runner    (1001) docker     (127)   163373 2024-04-23 12:14:53.000000 cid_cmd-0.3.2/cid/builtin/core/data/queries/shared/ta_descriptions.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:14:57.389546 cid_cmd-0.3.2/cid/builtin/core/data/queries/tao/
--rw-r--r--   0 runner    (1001) docker     (127)    35595 2024-04-23 12:14:53.000000 cid_cmd-0.3.2/cid/builtin/core/data/queries/tao/glue_table.json
--rw-r--r--   0 runner    (1001) docker     (127)     5935 2024-04-23 12:14:53.000000 cid_cmd-0.3.2/cid/builtin/core/data/queries/tao/ta_org_view.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:14:57.393546 cid_cmd-0.3.2/cid/builtin/core/data/queries/trends/
--rw-r--r--   0 runner    (1001) docker     (127)      680 2024-04-23 12:14:53.000000 cid_cmd-0.3.2/cid/builtin/core/data/queries/trends/daily_anomaly_detection.sql
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-23 12:14:53.000000 cid_cmd-0.3.2/cid/builtin/core/data/queries/trends/monthly_anomaly_detection.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-04-23 12:14:53.000000 cid_cmd-0.3.2/cid/builtin/core/data/queries/trends/monthly_bill_by_account.sql
--rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-04-23 12:14:53.000000 cid_cmd-0.3.2/cid/builtin/core/data/queries/trends/monthly_bill_by_account_ri.sql
--rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-04-23 12:14:53.000000 cid_cmd-0.3.2/cid/builtin/core/data/queries/trends/monthly_bill_by_account_sp.sql
--rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-04-23 12:14:53.000000 cid_cmd-0.3.2/cid/builtin/core/data/queries/trends/monthly_bill_by_account_sp_ri.sql
--rw-r--r--   0 runner    (1001) docker     (127)    18712 2024-04-23 12:14:53.000000 cid_cmd-0.3.2/cid/builtin/core/data/resources.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    12523 2024-04-23 12:14:53.000000 cid_cmd-0.3.2/cid/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:14:57.393546 cid_cmd-0.3.2/cid/commands/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-23 12:14:53.000000 cid_cmd-0.3.2/cid/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-23 12:14:53.000000 cid_cmd-0.3.2/cid/commands/command_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5353 2024-04-23 12:14:53.000000 cid_cmd-0.3.2/cid/commands/init_qs.py
--rw-r--r--   0 runner    (1001) docker     (127)    92373 2024-04-23 12:14:53.000000 cid_cmd-0.3.2/cid/common.py
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-23 12:14:53.000000 cid_cmd-0.3.2/cid/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    19919 2024-04-23 12:14:53.000000 cid_cmd-0.3.2/cid/export.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:14:57.393546 cid_cmd-0.3.2/cid/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-23 12:14:53.000000 cid_cmd-0.3.2/cid/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12580 2024-04-23 12:14:53.000000 cid_cmd-0.3.2/cid/helpers/account_map.py
--rw-r--r--   0 runner    (1001) docker     (127)    22951 2024-04-23 12:14:53.000000 cid_cmd-0.3.2/cid/helpers/athena.py
--rw-r--r--   0 runner    (1001) docker     (127)     2711 2024-04-23 12:14:53.000000 cid_cmd-0.3.2/cid/helpers/csv2view.py
--rw-r--r--   0 runner    (1001) docker     (127)    10132 2024-04-23 12:14:53.000000 cid_cmd-0.3.2/cid/helpers/cur.py
--rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-04-23 12:14:53.000000 cid_cmd-0.3.2/cid/helpers/diff.py
--rw-r--r--   0 runner    (1001) docker     (127)     3377 2024-04-23 12:14:53.000000 cid_cmd-0.3.2/cid/helpers/glue.py
--rw-r--r--   0 runner    (1001) docker     (127)    21978 2024-04-23 12:14:53.000000 cid_cmd-0.3.2/cid/helpers/iam.py
--rw-r--r--   0 runner    (1001) docker     (127)      938 2024-04-23 12:14:53.000000 cid_cmd-0.3.2/cid/helpers/organizations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:14:57.397546 cid_cmd-0.3.2/cid/helpers/quicksight/
--rw-r--r--   0 runner    (1001) docker     (127)    68635 2024-04-23 12:14:53.000000 cid_cmd-0.3.2/cid/helpers/quicksight/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6731 2024-04-23 12:14:53.000000 cid_cmd-0.3.2/cid/helpers/quicksight/dashboard.py
--rw-r--r--   0 runner    (1001) docker     (127)     3173 2024-04-23 12:14:53.000000 cid_cmd-0.3.2/cid/helpers/quicksight/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)      938 2024-04-23 12:14:53.000000 cid_cmd-0.3.2/cid/helpers/quicksight/datasource.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-23 12:14:53.000000 cid_cmd-0.3.2/cid/helpers/quicksight/resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     3156 2024-04-23 12:14:53.000000 cid_cmd-0.3.2/cid/helpers/quicksight/template.py
--rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-04-23 12:14:53.000000 cid_cmd-0.3.2/cid/helpers/randtime.py
--rw-r--r--   0 runner    (1001) docker     (127)     3302 2024-04-23 12:14:53.000000 cid_cmd-0.3.2/cid/helpers/s3.py
--rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-04-23 12:14:53.000000 cid_cmd-0.3.2/cid/helpers/timezone.py
--rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-04-23 12:14:53.000000 cid_cmd-0.3.2/cid/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     2932 2024-04-23 12:14:53.000000 cid_cmd-0.3.2/cid/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:14:57.373546 cid_cmd-0.3.2/cid/test/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:14:57.397546 cid_cmd-0.3.2/cid/test/python/
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-23 12:14:53.000000 cid_cmd-0.3.2/cid/test/python/test_csv2view.py
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-23 12:14:53.000000 cid_cmd-0.3.2/cid/test/python/test_isolated_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-23 12:14:53.000000 cid_cmd-0.3.2/cid/test/python/test_merge.py
--rw-r--r--   0 runner    (1001) docker     (127)    10836 2024-04-23 12:14:53.000000 cid_cmd-0.3.2/cid/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:14:57.397546 cid_cmd-0.3.2/cid_cmd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9475 2024-04-23 12:14:57.000000 cid_cmd-0.3.2/cid_cmd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5677 2024-04-23 12:14:57.000000 cid_cmd-0.3.2/cid_cmd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 12:14:57.000000 cid_cmd-0.3.2/cid_cmd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-23 12:14:57.000000 cid_cmd-0.3.2/cid_cmd.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-23 12:14:57.000000 cid_cmd-0.3.2/cid_cmd.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-23 12:14:57.000000 cid_cmd-0.3.2/cid_cmd.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-23 12:14:53.000000 cid_cmd-0.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-23 12:14:57.397546 cid_cmd-0.3.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:08:11.275941 cid_cmd-0.3.3/
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     9475 2024-04-25 09:08:11.275941 cid_cmd-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8560 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:08:11.255941 cid_cmd-0.3.3/cid/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1872 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:08:11.259940 cid_cmd-0.3.3/cid/builtin/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:08:11.259940 cid_cmd-0.3.3/cid/builtin/core/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:08:11.259940 cid_cmd-0.3.3/cid/builtin/core/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:08:11.251940 cid_cmd-0.3.3/cid/builtin/core/data/datasets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:08:11.259940 cid_cmd-0.3.3/cid/builtin/core/data/datasets/cid/
+-rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/datasets/cid/compute.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2893 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/datasets/cid/ec2_running_cost.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3777 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/datasets/cid/s3_view.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8825 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/datasets/cid/summary_view.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:08:11.259940 cid_cmd-0.3.3/cid/builtin/core/data/datasets/co/
+-rw-r--r--   0 runner    (1001) docker     (127)     9276 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/datasets/co/dataset.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:08:11.259940 cid_cmd-0.3.3/cid/builtin/core/data/datasets/cudos/
+-rw-r--r--   0 runner    (1001) docker     (127)     6223 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/datasets/cudos/hourly_view.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8610 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/datasets/cudos/resource_view.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:08:11.259940 cid_cmd-0.3.3/cid/builtin/core/data/datasets/kpi/
+-rw-r--r--   0 runner    (1001) docker     (127)     3353 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/datasets/kpi/kpi_ebs_snap.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5069 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/datasets/kpi/kpi_ebs_storage_all.json
+-rw-r--r--   0 runner    (1001) docker     (127)    20695 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/datasets/kpi/kpi_instance_all.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11136 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/datasets/kpi/kpi_s3_storage_all.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15746 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/datasets/kpi/kpi_tracker.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:08:11.259940 cid_cmd-0.3.3/cid/builtin/core/data/datasets/shared/
+-rw-r--r--   0 runner    (1001) docker     (127)    30612 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/datasets/shared/customer_all.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:08:11.259940 cid_cmd-0.3.3/cid/builtin/core/data/datasets/tao/
+-rw-r--r--   0 runner    (1001) docker     (127)    69315 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/datasets/tao/dataset.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:08:11.259940 cid_cmd-0.3.3/cid/builtin/core/data/datasets/trends/
+-rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/datasets/trends/daily_anomaly_detection.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/datasets/trends/monthly_anomaly_detection.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4681 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/datasets/trends/monthly_bill_by_account.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:08:11.263941 cid_cmd-0.3.3/cid/builtin/core/data/permissions/
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/permissions/dashboard_permissions.json
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/permissions/dashboard_permissions_namespace.json
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/permissions/data_set_permissions.json
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/permissions/data_source_permissions.json
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/permissions/folder_permissions.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:08:11.255941 cid_cmd-0.3.3/cid/builtin/core/data/queries/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:08:11.263941 cid_cmd-0.3.3/cid/builtin/core/data/queries/cid/
+-rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/queries/cid/compute_savings_plan_eligible_spend.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/queries/cid/ec2_running_cost.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/queries/cid/ec2_running_cost_ri.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/queries/cid/ec2_running_cost_sp.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/queries/cid/ec2_running_cost_sp_ri.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     2942 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/queries/cid/ri_sp_mapping.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/queries/cid/ri_sp_mapping_ri.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/queries/cid/ri_sp_mapping_sp.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     3134 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/queries/cid/ri_sp_mapping_sp_ri.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/queries/cid/s3.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     5808 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/queries/cid/summary_view.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     5533 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/queries/cid/summary_view_ri.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     5589 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/queries/cid/summary_view_sp.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     5599 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/queries/cid/summary_view_sp_ri.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:08:11.267941 cid_cmd-0.3.3/cid/builtin/core/data/queries/co/
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/queries/co/all_options.sql
+-rw-r--r--   0 runner    (1001) docker     (127)    14711 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/queries/co/auto_scale.json
+-rw-r--r--   0 runner    (1001) docker     (127)    27919 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/queries/co/auto_scale_options.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     9097 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/queries/co/ebs_volume.json
+-rw-r--r--   0 runner    (1001) docker     (127)    22473 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/queries/co/ebs_volume_options.sql
+-rw-r--r--   0 runner    (1001) docker     (127)    19144 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/queries/co/ec2_instance.json
+-rw-r--r--   0 runner    (1001) docker     (127)    28308 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/queries/co/ec2_instance_options.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     8029 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/queries/co/lambda.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15340 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/queries/co/lambda_options.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:08:11.267941 cid_cmd-0.3.3/cid/builtin/core/data/queries/cudos/
+-rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/queries/cudos/hourly_view.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/queries/cudos/hourly_view_ri.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/queries/cudos/hourly_view_sp.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/queries/cudos/hourly_view_sp_ri.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1989 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/queries/cudos/resource_view.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/queries/cudos/resource_view_ri.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/queries/cudos/resource_view_sp.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/queries/cudos/resource_view_sp_ri.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:08:11.267941 cid_cmd-0.3.3/cid/builtin/core/data/queries/kpi/
+-rw-r--r--   0 runner    (1001) docker     (127)    11145 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/queries/kpi/first_kpi_instance_mapping_view.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     3187 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/queries/kpi/kpi_ebs_snap_view.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     6192 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/queries/kpi/kpi_ebs_storage_view.sql
+-rw-r--r--   0 runner    (1001) docker     (127)    24337 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/queries/kpi/kpi_instance_all_view.sql
+-rw-r--r--   0 runner    (1001) docker     (127)    23573 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/queries/kpi/kpi_instance_all_view_noRI.sql
+-rw-r--r--   0 runner    (1001) docker     (127)    22559 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/queries/kpi/kpi_instance_all_view_noRISP.sql
+-rw-r--r--   0 runner    (1001) docker     (127)    23434 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/queries/kpi/kpi_instance_all_view_noSP.sql
+-rw-r--r--   0 runner    (1001) docker     (127)    11256 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/queries/kpi/kpi_s3_storage_view.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     9226 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/queries/kpi/last_kpi_tracker_view.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:08:11.271941 cid_cmd-0.3.3/cid/builtin/core/data/queries/shared/
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/queries/shared/account_map.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/queries/shared/account_map_dummy.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/queries/shared/aws_accounts.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     2731 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/queries/shared/aws_regions.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     7282 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/queries/shared/aws_service_category_map.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/queries/shared/business_units_map.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     5043 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/queries/shared/cur.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/queries/shared/payer_account_name_map.sql
+-rw-r--r--   0 runner    (1001) docker     (127)   163373 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/queries/shared/ta_descriptions.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:08:11.271941 cid_cmd-0.3.3/cid/builtin/core/data/queries/tao/
+-rw-r--r--   0 runner    (1001) docker     (127)    35595 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/queries/tao/glue_table.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5935 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/queries/tao/ta_org_view.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:08:11.271941 cid_cmd-0.3.3/cid/builtin/core/data/queries/trends/
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/queries/trends/daily_anomaly_detection.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/queries/trends/monthly_anomaly_detection.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/queries/trends/monthly_bill_by_account.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/queries/trends/monthly_bill_by_account_ri.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/queries/trends/monthly_bill_by_account_sp.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/queries/trends/monthly_bill_by_account_sp_ri.sql
+-rw-r--r--   0 runner    (1001) docker     (127)    18712 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/builtin/core/data/resources.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    12523 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:08:11.271941 cid_cmd-0.3.3/cid/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/commands/command_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5353 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/commands/init_qs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    92373 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19919 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/export.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:08:11.275941 cid_cmd-0.3.3/cid/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12580 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/helpers/account_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22951 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/helpers/athena.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2711 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/helpers/csv2view.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10126 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/helpers/cur.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/helpers/diff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3377 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/helpers/glue.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21978 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/helpers/iam.py
+-rw-r--r--   0 runner    (1001) docker     (127)      938 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/helpers/organizations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:08:11.275941 cid_cmd-0.3.3/cid/helpers/quicksight/
+-rw-r--r--   0 runner    (1001) docker     (127)    68635 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/helpers/quicksight/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6731 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/helpers/quicksight/dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3173 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/helpers/quicksight/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      938 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/helpers/quicksight/datasource.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/helpers/quicksight/resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3156 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/helpers/quicksight/template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/helpers/randtime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3302 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/helpers/s3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/helpers/timezone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2932 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:08:11.255941 cid_cmd-0.3.3/cid/test/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:08:11.275941 cid_cmd-0.3.3/cid/test/python/
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/test/python/test_csv2view.py
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/test/python/test_isolated_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/test/python/test_merge.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10836 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/cid/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:08:11.275941 cid_cmd-0.3.3/cid_cmd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9475 2024-04-25 09:08:11.000000 cid_cmd-0.3.3/cid_cmd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5677 2024-04-25 09:08:11.000000 cid_cmd-0.3.3/cid_cmd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 09:08:11.000000 cid_cmd-0.3.3/cid_cmd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-25 09:08:11.000000 cid_cmd-0.3.3/cid_cmd.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-25 09:08:11.000000 cid_cmd-0.3.3/cid_cmd.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-25 09:08:11.000000 cid_cmd-0.3.3/cid_cmd.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-25 09:08:07.000000 cid_cmd-0.3.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-25 09:08:11.275941 cid_cmd-0.3.3/setup.cfg
```

### Comparing `cid_cmd-0.3.2/LICENSE` & `cid_cmd-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.2/PKG-INFO` & `cid_cmd-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cid-cmd
-Version: 0.3.2
+Version: 0.3.3
 Summary: Cloud Intelligence Dashboards deployment helper tool
 Home-page: https://github.com/aws-samples/aws-cudos-framework-deployment
 Author: AWS CUDOS Team
 License: MIT
 Keywords: aws,cmd,cli,cost intelligence dashboards
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cid_cmd-0.3.2/README.md` & `cid_cmd-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.2/cid/base.py` & `cid_cmd-0.3.3/cid/base.py`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.2/cid/builtin/core/data/datasets/cid/compute.json` & `cid_cmd-0.3.3/cid/builtin/core/data/datasets/cid/compute.json`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.2/cid/builtin/core/data/datasets/cid/ec2_running_cost.json` & `cid_cmd-0.3.3/cid/builtin/core/data/datasets/cid/ec2_running_cost.json`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.2/cid/builtin/core/data/datasets/cid/s3_view.json` & `cid_cmd-0.3.3/cid/builtin/core/data/datasets/cid/s3_view.json`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.2/cid/builtin/core/data/datasets/cid/summary_view.json` & `cid_cmd-0.3.3/cid/builtin/core/data/datasets/cid/summary_view.json`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.2/cid/builtin/core/data/datasets/co/dataset.json` & `cid_cmd-0.3.3/cid/builtin/core/data/datasets/co/dataset.json`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.2/cid/builtin/core/data/datasets/cudos/hourly_view.json` & `cid_cmd-0.3.3/cid/builtin/core/data/datasets/cudos/hourly_view.json`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.2/cid/builtin/core/data/datasets/cudos/resource_view.json` & `cid_cmd-0.3.3/cid/builtin/core/data/datasets/cudos/resource_view.json`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.2/cid/builtin/core/data/datasets/kpi/kpi_ebs_snap.json` & `cid_cmd-0.3.3/cid/builtin/core/data/datasets/kpi/kpi_ebs_snap.json`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.2/cid/builtin/core/data/datasets/kpi/kpi_ebs_storage_all.json` & `cid_cmd-0.3.3/cid/builtin/core/data/datasets/kpi/kpi_ebs_storage_all.json`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.2/cid/builtin/core/data/datasets/kpi/kpi_instance_all.json` & `cid_cmd-0.3.3/cid/builtin/core/data/datasets/kpi/kpi_instance_all.json`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.2/cid/builtin/core/data/datasets/kpi/kpi_s3_storage_all.json` & `cid_cmd-0.3.3/cid/builtin/core/data/datasets/kpi/kpi_s3_storage_all.json`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.2/cid/builtin/core/data/datasets/kpi/kpi_tracker.json` & `cid_cmd-0.3.3/cid/builtin/core/data/datasets/kpi/kpi_tracker.json`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.2/cid/builtin/core/data/datasets/shared/customer_all.json` & `cid_cmd-0.3.3/cid/builtin/core/data/datasets/shared/customer_all.json`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.2/cid/builtin/core/data/datasets/tao/dataset.json` & `cid_cmd-0.3.3/cid/builtin/core/data/datasets/tao/dataset.json`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.2/cid/builtin/core/data/datasets/trends/daily_anomaly_detection.json` & `cid_cmd-0.3.3/cid/builtin/core/data/datasets/trends/daily_anomaly_detection.json`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.2/cid/builtin/core/data/datasets/trends/monthly_anomaly_detection.json` & `cid_cmd-0.3.3/cid/builtin/core/data/datasets/trends/monthly_anomaly_detection.json`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.2/cid/builtin/core/data/datasets/trends/monthly_bill_by_account.json` & `cid_cmd-0.3.3/cid/builtin/core/data/datasets/trends/monthly_bill_by_account.json`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.2/cid/builtin/core/data/queries/cid/compute_savings_plan_eligible_spend.sql` & `cid_cmd-0.3.3/cid/builtin/core/data/queries/cid/compute_savings_plan_eligible_spend.sql`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.2/cid/builtin/core/data/queries/cid/ec2_running_cost.sql` & `cid_cmd-0.3.3/cid/builtin/core/data/queries/cid/ec2_running_cost.sql`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.2/cid/builtin/core/data/queries/cid/ec2_running_cost_ri.sql` & `cid_cmd-0.3.3/cid/builtin/core/data/queries/cid/ec2_running_cost_ri.sql`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.2/cid/builtin/core/data/queries/cid/ec2_running_cost_sp.sql` & `cid_cmd-0.3.3/cid/builtin/core/data/queries/cid/ec2_running_cost_sp.sql`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.2/cid/builtin/core/data/queries/cid/ec2_running_cost_sp_ri.sql` & `cid_cmd-0.3.3/cid/builtin/core/data/queries/cid/ec2_running_cost_sp_ri.sql`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.2/cid/builtin/core/data/queries/cid/ri_sp_mapping.sql` & `cid_cmd-0.3.3/cid/builtin/core/data/queries/cid/ri_sp_mapping.sql`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.2/cid/builtin/core/data/queries/cid/ri_sp_mapping_ri.sql` & `cid_cmd-0.3.3/cid/builtin/core/data/queries/cid/ri_sp_mapping_ri.sql`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.2/cid/builtin/core/data/queries/cid/ri_sp_mapping_sp.sql` & `cid_cmd-0.3.3/cid/builtin/core/data/queries/cid/ri_sp_mapping_sp.sql`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.2/cid/builtin/core/data/queries/cid/ri_sp_mapping_sp_ri.sql` & `cid_cmd-0.3.3/cid/builtin/core/data/queries/cid/ri_sp_mapping_sp_ri.sql`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.2/cid/builtin/core/data/queries/cid/s3.sql` & `cid_cmd-0.3.3/cid/builtin/core/data/queries/cid/s3.sql`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.2/cid/builtin/core/data/queries/cid/summary_view.sql` & `cid_cmd-0.3.3/cid/builtin/core/data/queries/cid/summary_view.sql`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.2/cid/builtin/core/data/queries/cid/summary_view_ri.sql` & `cid_cmd-0.3.3/cid/builtin/core/data/queries/cid/summary_view_ri.sql`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.2/cid/builtin/core/data/queries/cid/summary_view_sp.sql` & `cid_cmd-0.3.3/cid/builtin/core/data/queries/cid/summary_view_sp.sql`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.2/cid/builtin/core/data/queries/cid/summary_view_sp_ri.sql` & `cid_cmd-0.3.3/cid/builtin/core/data/queries/cid/summary_view_sp_ri.sql`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.2/cid/builtin/core/data/queries/co/auto_scale.json` & `cid_cmd-0.3.3/cid/builtin/core/data/queries/co/auto_scale.json`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.2/cid/builtin/core/data/queries/co/auto_scale_options.sql` & `cid_cmd-0.3.3/cid/builtin/core/data/queries/co/auto_scale_options.sql`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.2/cid/builtin/core/data/queries/co/ebs_volume.json` & `cid_cmd-0.3.3/cid/builtin/core/data/queries/co/ebs_volume.json`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.2/cid/builtin/core/data/queries/co/ebs_volume_options.sql` & `cid_cmd-0.3.3/cid/builtin/core/data/queries/co/ebs_volume_options.sql`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.2/cid/builtin/core/data/queries/co/ec2_instance.json` & `cid_cmd-0.3.3/cid/builtin/core/data/queries/co/ec2_instance.json`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.2/cid/builtin/core/data/queries/co/ec2_instance_options.sql` & `cid_cmd-0.3.3/cid/builtin/core/data/queries/co/ec2_instance_options.sql`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.2/cid/builtin/core/data/queries/co/lambda.json` & `cid_cmd-0.3.3/cid/builtin/core/data/queries/co/lambda.json`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.2/cid/builtin/core/data/queries/co/lambda_options.sql` & `cid_cmd-0.3.3/cid/builtin/core/data/queries/co/lambda_options.sql`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.2/cid/builtin/core/data/queries/cudos/hourly_view.sql` & `cid_cmd-0.3.3/cid/builtin/core/data/queries/cudos/hourly_view.sql`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.2/cid/builtin/core/data/queries/cudos/hourly_view_ri.sql` & `cid_cmd-0.3.3/cid/builtin/core/data/queries/cudos/hourly_view_ri.sql`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.2/cid/builtin/core/data/queries/cudos/hourly_view_sp.sql` & `cid_cmd-0.3.3/cid/builtin/core/data/queries/cudos/hourly_view_sp.sql`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.2/cid/builtin/core/data/queries/cudos/hourly_view_sp_ri.sql` & `cid_cmd-0.3.3/cid/builtin/core/data/queries/cudos/hourly_view_sp_ri.sql`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.2/cid/builtin/core/data/queries/cudos/resource_view.sql` & `cid_cmd-0.3.3/cid/builtin/core/data/queries/cudos/resource_view.sql`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.2/cid/builtin/core/data/queries/cudos/resource_view_ri.sql` & `cid_cmd-0.3.3/cid/builtin/core/data/queries/cudos/resource_view_ri.sql`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.2/cid/builtin/core/data/queries/cudos/resource_view_sp.sql` & `cid_cmd-0.3.3/cid/builtin/core/data/queries/cudos/resource_view_sp.sql`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.2/cid/builtin/core/data/queries/cudos/resource_view_sp_ri.sql` & `cid_cmd-0.3.3/cid/builtin/core/data/queries/cudos/resource_view_sp_ri.sql`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.2/cid/builtin/core/data/queries/kpi/first_kpi_instance_mapping_view.sql` & `cid_cmd-0.3.3/cid/builtin/core/data/queries/kpi/first_kpi_instance_mapping_view.sql`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.2/cid/builtin/core/data/queries/kpi/kpi_ebs_snap_view.sql` & `cid_cmd-0.3.3/cid/builtin/core/data/queries/kpi/kpi_ebs_snap_view.sql`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.2/cid/builtin/core/data/queries/kpi/kpi_ebs_storage_view.sql` & `cid_cmd-0.3.3/cid/builtin/core/data/queries/kpi/kpi_ebs_storage_view.sql`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.2/cid/builtin/core/data/queries/kpi/kpi_instance_all_view.sql` & `cid_cmd-0.3.3/cid/builtin/core/data/queries/kpi/kpi_instance_all_view.sql`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.2/cid/builtin/core/data/queries/kpi/kpi_instance_all_view_noRI.sql` & `cid_cmd-0.3.3/cid/builtin/core/data/queries/kpi/kpi_instance_all_view_noRI.sql`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.2/cid/builtin/core/data/queries/kpi/kpi_instance_all_view_noRISP.sql` & `cid_cmd-0.3.3/cid/builtin/core/data/queries/kpi/kpi_instance_all_view_noRISP.sql`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.2/cid/builtin/core/data/queries/kpi/kpi_instance_all_view_noSP.sql` & `cid_cmd-0.3.3/cid/builtin/core/data/queries/kpi/kpi_instance_all_view_noSP.sql`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.2/cid/builtin/core/data/queries/kpi/kpi_s3_storage_view.sql` & `cid_cmd-0.3.3/cid/builtin/core/data/queries/kpi/kpi_s3_storage_view.sql`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.2/cid/builtin/core/data/queries/kpi/last_kpi_tracker_view.sql` & `cid_cmd-0.3.3/cid/builtin/core/data/queries/kpi/last_kpi_tracker_view.sql`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.2/cid/builtin/core/data/queries/shared/aws_accounts.sql` & `cid_cmd-0.3.3/cid/builtin/core/data/queries/shared/aws_accounts.sql`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.2/cid/builtin/core/data/queries/shared/aws_regions.sql` & `cid_cmd-0.3.3/cid/builtin/core/data/queries/shared/aws_regions.sql`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.2/cid/builtin/core/data/queries/shared/aws_service_category_map.sql` & `cid_cmd-0.3.3/cid/builtin/core/data/queries/shared/aws_service_category_map.sql`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.2/cid/builtin/core/data/queries/shared/cur.yaml` & `cid_cmd-0.3.3/cid/builtin/core/data/queries/shared/cur.yaml`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.2/cid/builtin/core/data/queries/shared/ta_descriptions.sql` & `cid_cmd-0.3.3/cid/builtin/core/data/queries/shared/ta_descriptions.sql`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.2/cid/builtin/core/data/queries/tao/glue_table.json` & `cid_cmd-0.3.3/cid/builtin/core/data/queries/tao/glue_table.json`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.2/cid/builtin/core/data/queries/tao/ta_org_view.sql` & `cid_cmd-0.3.3/cid/builtin/core/data/queries/tao/ta_org_view.sql`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.2/cid/builtin/core/data/queries/trends/daily_anomaly_detection.sql` & `cid_cmd-0.3.3/cid/builtin/core/data/queries/trends/daily_anomaly_detection.sql`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.2/cid/builtin/core/data/queries/trends/monthly_anomaly_detection.sql` & `cid_cmd-0.3.3/cid/builtin/core/data/queries/trends/monthly_anomaly_detection.sql`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.2/cid/builtin/core/data/queries/trends/monthly_bill_by_account.sql` & `cid_cmd-0.3.3/cid/builtin/core/data/queries/trends/monthly_bill_by_account.sql`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.2/cid/builtin/core/data/queries/trends/monthly_bill_by_account_ri.sql` & `cid_cmd-0.3.3/cid/builtin/core/data/queries/trends/monthly_bill_by_account_ri.sql`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.2/cid/builtin/core/data/queries/trends/monthly_bill_by_account_sp.sql` & `cid_cmd-0.3.3/cid/builtin/core/data/queries/trends/monthly_bill_by_account_sp.sql`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.2/cid/builtin/core/data/queries/trends/monthly_bill_by_account_sp_ri.sql` & `cid_cmd-0.3.3/cid/builtin/core/data/queries/trends/monthly_bill_by_account_sp_ri.sql`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.2/cid/builtin/core/data/resources.yaml` & `cid_cmd-0.3.3/cid/builtin/core/data/resources.yaml`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.2/cid/cli.py` & `cid_cmd-0.3.3/cid/cli.py`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.2/cid/commands/init_qs.py` & `cid_cmd-0.3.3/cid/commands/init_qs.py`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.2/cid/common.py` & `cid_cmd-0.3.3/cid/common.py`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.2/cid/export.py` & `cid_cmd-0.3.3/cid/export.py`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.2/cid/helpers/__init__.py` & `cid_cmd-0.3.3/cid/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.2/cid/helpers/account_map.py` & `cid_cmd-0.3.3/cid/helpers/account_map.py`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.2/cid/helpers/athena.py` & `cid_cmd-0.3.3/cid/helpers/athena.py`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.2/cid/helpers/csv2view.py` & `cid_cmd-0.3.3/cid/helpers/csv2view.py`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.2/cid/helpers/cur.py` & `cid_cmd-0.3.3/cid/helpers/cur.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """ Manage AWS CUR
 """
 import json
 import logging
 
 from cid.base import CidBase
-from cid.utils import get_parameter, get_parameters
+from cid.utils import get_parameter, get_parameters, cid_print
 from cid.exceptions import CidCritical
 
 logger = logging.getLogger(__name__)
 
 
 class CUR(CidBase):
     """ Manage AWS CUR
@@ -131,25 +131,26 @@
                 logger.debug('Failed to get crawler info')
         if table_can_be_updated:
             column_type = column_type or self.get_type_of_column(column)
             try:
                 self.athena.query(f'ALTER TABLE {self.table_name} ADD COLUMNS ({column} {column_type})')
             except (self.athena.client.exceptions.ClientError, CidCritical) as exc:
                 raise CidCritical(f'Column {column} is not found in CUR and we were unable to add it. Please check FAQ.') from exc
-            self._metadata = self.athena.get_table_metadata(self.table_name) # refresh table metadata
-            logger.critical(f"Column '{column}' was added to CUR ({self.table_name}). Please make sure crawler do not override that columns. Crawler='{crawler_name}'")
+            # table takes time to update so just adding column to cached data
+            self._metadata.get('Columns', []).append({'Name': column, 'Type': column_type})
+            cid_print(f"Column '{column}' was added to CUR ({self.table_name}).")
             return
 
         # if table cannot be updated, check if it is ri/sp case - let's hope dashboard views can handle it:
         if column in self.sp_required_columns + self.ri_required_columns:
             logger.warn(f"Column '{column}' is not present in ({self.table_name}). Will try to continue without.")
             return
 
         # if a required column is not there and not ri/sp -> stop
-        logger.critical(f"Column '{column}' is not in ({self.table_name}). Cannot continue")
+        logger.critical(f"Column '{column}' is not in ({self.table_name}). Cannot continue.")
 
 
     def table_is_cur(self, table: dict=None, name: str=None, return_reason: bool=False) -> bool:
         """ return True if table metadata fits CUR definition. """
         try:
             table = table or self.athena.get_table_metadata(name)
         except Exception as exc: #pylint: disable=broad-exception-caught
```

### Comparing `cid_cmd-0.3.2/cid/helpers/diff.py` & `cid_cmd-0.3.3/cid/helpers/diff.py`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.2/cid/helpers/glue.py` & `cid_cmd-0.3.3/cid/helpers/glue.py`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.2/cid/helpers/iam.py` & `cid_cmd-0.3.3/cid/helpers/iam.py`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.2/cid/helpers/organizations.py` & `cid_cmd-0.3.3/cid/helpers/organizations.py`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.2/cid/helpers/quicksight/__init__.py` & `cid_cmd-0.3.3/cid/helpers/quicksight/__init__.py`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.2/cid/helpers/quicksight/dashboard.py` & `cid_cmd-0.3.3/cid/helpers/quicksight/dashboard.py`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.2/cid/helpers/quicksight/dataset.py` & `cid_cmd-0.3.3/cid/helpers/quicksight/dataset.py`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.2/cid/helpers/quicksight/datasource.py` & `cid_cmd-0.3.3/cid/helpers/quicksight/datasource.py`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.2/cid/helpers/quicksight/template.py` & `cid_cmd-0.3.3/cid/helpers/quicksight/template.py`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.2/cid/helpers/randtime.py` & `cid_cmd-0.3.3/cid/helpers/randtime.py`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.2/cid/helpers/s3.py` & `cid_cmd-0.3.3/cid/helpers/s3.py`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.2/cid/helpers/timezone.py` & `cid_cmd-0.3.3/cid/helpers/timezone.py`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.2/cid/logger.py` & `cid_cmd-0.3.3/cid/logger.py`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.2/cid/plugin.py` & `cid_cmd-0.3.3/cid/plugin.py`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.2/cid/test/python/test_merge.py` & `cid_cmd-0.3.3/cid/test/python/test_merge.py`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.2/cid/utils.py` & `cid_cmd-0.3.3/cid/utils.py`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.2/cid_cmd.egg-info/PKG-INFO` & `cid_cmd-0.3.3/cid_cmd.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cid-cmd
-Version: 0.3.2
+Version: 0.3.3
 Summary: Cloud Intelligence Dashboards deployment helper tool
 Home-page: https://github.com/aws-samples/aws-cudos-framework-deployment
 Author: AWS CUDOS Team
 License: MIT
 Keywords: aws,cmd,cli,cost intelligence dashboards
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cid_cmd-0.3.2/cid_cmd.egg-info/SOURCES.txt` & `cid_cmd-0.3.3/cid_cmd.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cid_cmd-0.3.2/setup.cfg` & `cid_cmd-0.3.3/setup.cfg`

 * *Files identical despite different names*


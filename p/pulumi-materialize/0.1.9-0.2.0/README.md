# Comparing `tmp/pulumi_materialize-0.1.9.tar.gz` & `tmp/pulumi_materialize-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_materialize-0.1.9.tar", last modified: Fri Mar 29 16:44:52 2024, max compression
+gzip compressed data, was "pulumi_materialize-0.2.0.tar", last modified: Thu Apr 25 15:05:38 2024, max compression
```

## Comparing `pulumi_materialize-0.1.9.tar` & `pulumi_materialize-0.2.0.tar`

### file list

```diff
@@ -1,97 +1,101 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 16:44:52.431204 pulumi_materialize-0.1.9/
--rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-03-29 16:44:52.431204 pulumi_materialize-0.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 16:44:52.431204 pulumi_materialize-0.1.9/pulumi_materialize/
--rw-r--r--   0 runner    (1001) docker     (127)    12726 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   208675 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     8136 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     8502 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/app_password.py
--rw-r--r--   0 runner    (1001) docker     (127)    32086 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)    30123 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/cluster_replica.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 16:44:52.431204 pulumi_materialize-0.1.9/pulumi_materialize/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)    38924 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/connection_aws.py
--rw-r--r--   0 runner    (1001) docker     (127)    25847 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/connection_aws_privatelink.py
--rw-r--r--   0 runner    (1001) docker     (127)    46174 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/connection_confluent_schema_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)    54306 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/connection_kafka.py
--rw-r--r--   0 runner    (1001) docker     (127)    47019 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/connection_mysql.py
--rw-r--r--   0 runner    (1001) docker     (127)    49006 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/connection_postgres.py
--rw-r--r--   0 runner    (1001) docker     (127)    28437 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/connection_ssh_tunnel.py
--rw-r--r--   0 runner    (1001) docker     (127)    12337 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/database.py
--rw-r--r--   0 runner    (1001) docker     (127)     3618 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/get_cluster_replicas.py
--rw-r--r--   0 runner    (1001) docker     (127)     3313 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/get_clusters.py
--rw-r--r--   0 runner    (1001) docker     (127)     5603 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/get_connections.py
--rw-r--r--   0 runner    (1001) docker     (127)     3383 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/get_current_cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     3407 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/get_current_database.py
--rw-r--r--   0 runner    (1001) docker     (127)     3350 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/get_databases.py
--rw-r--r--   0 runner    (1001) docker     (127)     3417 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/get_egress_ips.py
--rw-r--r--   0 runner    (1001) docker     (127)     5398 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/get_indexes.py
--rw-r--r--   0 runner    (1001) docker     (127)     5971 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/get_materialized_views.py
--rw-r--r--   0 runner    (1001) docker     (127)     3202 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/get_roles.py
--rw-r--r--   0 runner    (1001) docker     (127)     4282 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/get_schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/get_scim_configs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/get_scim_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     5399 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/get_secrets.py
--rw-r--r--   0 runner    (1001) docker     (127)     5297 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/get_sinks.py
--rw-r--r--   0 runner    (1001) docker     (127)     5399 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/get_sources.py
--rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/get_sso_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4219 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/get_system_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     4856 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/get_tables.py
--rw-r--r--   0 runner    (1001) docker     (127)     4811 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/get_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     5297 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/get_views.py
--rw-r--r--   0 runner    (1001) docker     (127)    13194 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/grant_cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)    15563 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/grant_cluster_default_privilege.py
--rw-r--r--   0 runner    (1001) docker     (127)    17766 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/grant_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)    20573 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/grant_connection_default_privilege.py
--rw-r--r--   0 runner    (1001) docker     (127)    13280 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/grant_database.py
--rw-r--r--   0 runner    (1001) docker     (127)    15697 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/grant_database_default_privilege.py
--rw-r--r--   0 runner    (1001) docker     (127)    18429 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/grant_materialized_view.py
--rw-r--r--   0 runner    (1001) docker     (127)    10986 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/grant_role.py
--rw-r--r--   0 runner    (1001) docker     (127)    15292 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/grant_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)    18124 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/grant_schema_default_privilege.py
--rw-r--r--   0 runner    (1001) docker     (127)    17366 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/grant_secret.py
--rw-r--r--   0 runner    (1001) docker     (127)    20461 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/grant_secret_default_privilege.py
--rw-r--r--   0 runner    (1001) docker     (127)    17346 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/grant_source.py
--rw-r--r--   0 runner    (1001) docker     (127)    11051 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/grant_system_privilege.py
--rw-r--r--   0 runner    (1001) docker     (127)    17558 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/grant_table.py
--rw-r--r--   0 runner    (1001) docker     (127)    20743 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/grant_table_default_privilege.py
--rw-r--r--   0 runner    (1001) docker     (127)    17166 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/grant_type.py
--rw-r--r--   0 runner    (1001) docker     (127)    20405 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/grant_type_default_privilege.py
--rw-r--r--   0 runner    (1001) docker     (127)    16984 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/grant_view.py
--rw-r--r--   0 runner    (1001) docker     (127)    24878 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/index.py
--rw-r--r--   0 runner    (1001) docker     (127)    28616 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/materialized_view.py
--rw-r--r--   0 runner    (1001) docker     (127)   239623 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    13105 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     2105 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/region.py
--rw-r--r--   0 runner    (1001) docker     (127)    12783 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/role.py
--rw-r--r--   0 runner    (1001) docker     (127)    12920 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/role_parameter.py
--rw-r--r--   0 runner    (1001) docker     (127)    16381 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)    15515 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/scim2_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)    21139 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/secret.py
--rw-r--r--   0 runner    (1001) docker     (127)    44082 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/sink_kafka.py
--rw-r--r--   0 runner    (1001) docker     (127)    68779 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/source_kafka.py
--rw-r--r--   0 runner    (1001) docker     (127)    38877 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/source_loadgen.py
--rw-r--r--   0 runner    (1001) docker     (127)    36122 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/source_mysql.py
--rw-r--r--   0 runner    (1001) docker     (127)    41674 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/source_postgres.py
--rw-r--r--   0 runner    (1001) docker     (127)    37565 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/source_webhook.py
--rw-r--r--   0 runner    (1001) docker     (127)    24196 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/sso_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    10431 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/sso_default_roles.py
--rw-r--r--   0 runner    (1001) docker     (127)    10721 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/sso_domain.py
--rw-r--r--   0 runner    (1001) docker     (127)    12243 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/sso_role_group_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     9794 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/system_parameter.py
--rw-r--r--   0 runner    (1001) docker     (127)    22084 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/table.py
--rw-r--r--   0 runner    (1001) docker     (127)    27574 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/type.py
--rw-r--r--   0 runner    (1001) docker     (127)    11325 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/user.py
--rw-r--r--   0 runner    (1001) docker     (127)    22629 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/view.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 16:44:52.431204 pulumi_materialize-0.1.9/pulumi_materialize.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3369 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-29 16:44:52.431204 pulumi_materialize-0.1.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:05:38.318382 pulumi_materialize-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-04-25 15:05:38.318382 pulumi_materialize-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:05:38.314382 pulumi_materialize-0.2.0/pulumi_materialize/
+-rw-r--r--   0 runner    (1001) docker     (127)    13567 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   215981 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8136 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8502 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/app_password.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13393 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/cloud_region.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31153 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26842 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/cluster_replica.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:05:38.314382 pulumi_materialize-0.2.0/pulumi_materialize/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38924 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/connection_aws.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27833 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/connection_aws_privatelink.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46174 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/connection_confluent_schema_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54306 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/connection_kafka.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47019 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/connection_mysql.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49006 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/connection_postgres.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28437 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/connection_ssh_tunnel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14185 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3618 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/get_cluster_replicas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3313 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/get_clusters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5603 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/get_connections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3383 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/get_current_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3407 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/get_current_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3350 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/get_databases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3417 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/get_egress_ips.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5398 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/get_indexes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5971 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/get_materialized_views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3202 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/get_roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4282 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/get_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/get_scim_configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/get_scim_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5399 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/get_secrets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5297 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/get_sinks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5399 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/get_sources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/get_sso_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4219 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/get_system_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4856 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/get_tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4811 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/get_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5297 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/get_views.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13194 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/grant_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15563 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/grant_cluster_default_privilege.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17766 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/grant_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20573 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/grant_connection_default_privilege.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13280 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/grant_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15697 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/grant_database_default_privilege.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18429 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/grant_materialized_view.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10986 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/grant_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15292 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/grant_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18124 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/grant_schema_default_privilege.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17366 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/grant_secret.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20461 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/grant_secret_default_privilege.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17346 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/grant_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11051 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/grant_system_privilege.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17558 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/grant_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20743 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/grant_table_default_privilege.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17166 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/grant_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20405 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/grant_type_default_privilege.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16984 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/grant_view.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24878 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/index.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28616 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/materialized_view.py
+-rw-r--r--   0 runner    (1001) docker     (127)   247075 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13105 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     2105 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/region.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12783 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12920 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/role_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16381 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15515 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/scim2_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8149 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/scim2_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9230 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/scim2_group_roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9640 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/scim2_group_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21139 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/secret.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44082 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/sink_kafka.py
+-rw-r--r--   0 runner    (1001) docker     (127)    68779 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/source_kafka.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41574 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/source_loadgen.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36122 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/source_mysql.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41674 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/source_postgres.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37565 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/source_webhook.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24196 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/sso_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10431 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/sso_default_roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10721 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/sso_domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12243 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/sso_role_group_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9794 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/system_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22084 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/table.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27574 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11325 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22629 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/view.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:05:38.314382 pulumi_materialize-0.2.0/pulumi_materialize.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3518 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 15:05:38.318382 pulumi_materialize-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/setup.py
```

### Comparing `pulumi_materialize-0.1.9/PKG-INFO` & `pulumi_materialize-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_materialize
-Version: 0.1.9
+Version: 0.2.0
 Summary: A Pulumi package for creating and managing materialize cloud resources.
 Home-page: https://github.com/MaterializeInc/terraform-provider-materialize
 License: Apache-2.0
 Project-URL: Repository, https://github.com/MaterializeInc/terraform-provider-materialize
 Keywords: pulumi materialize category/cloud
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_materialize-0.1.9/README.md` & `pulumi_materialize-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.1.9/pulumi_materialize/__init__.py` & `pulumi_materialize-0.2.0/pulumi_materialize/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
 from . import _utilities
 import typing
 # Export this package's modules as members:
 from .app_password import *
+from .cloud_region import *
 from .cluster import *
 from .cluster_replica import *
 from .connection_aws import *
 from .connection_aws_privatelink import *
 from .connection_confluent_schema_registry import *
 from .connection_kafka import *
 from .connection_mysql import *
@@ -60,14 +61,17 @@
 from .materialized_view import *
 from .provider import *
 from .region import *
 from .role import *
 from .role_parameter import *
 from .schema import *
 from .scim2_configuration import *
+from .scim2_group import *
+from .scim2_group_roles import *
+from .scim2_group_users import *
 from .secret import *
 from .sink_kafka import *
 from .source_kafka import *
 from .source_loadgen import *
 from .source_mysql import *
 from .source_postgres import *
 from .source_webhook import *
@@ -99,14 +103,22 @@
   "fqn": "pulumi_materialize",
   "classes": {
    "materialize:index/appPassword:AppPassword": "AppPassword"
   }
  },
  {
   "pkg": "materialize",
+  "mod": "index/cloudRegion",
+  "fqn": "pulumi_materialize",
+  "classes": {
+   "materialize:index/cloudRegion:CloudRegion": "CloudRegion"
+  }
+ },
+ {
+  "pkg": "materialize",
   "mod": "index/cluster",
   "fqn": "pulumi_materialize",
   "classes": {
    "materialize:index/cluster:Cluster": "Cluster"
   }
  },
  {
@@ -371,14 +383,38 @@
   "fqn": "pulumi_materialize",
   "classes": {
    "materialize:index/sCIM2Configuration:SCIM2Configuration": "SCIM2Configuration"
   }
  },
  {
   "pkg": "materialize",
+  "mod": "index/sCIM2Group",
+  "fqn": "pulumi_materialize",
+  "classes": {
+   "materialize:index/sCIM2Group:SCIM2Group": "SCIM2Group"
+  }
+ },
+ {
+  "pkg": "materialize",
+  "mod": "index/sCIM2GroupRoles",
+  "fqn": "pulumi_materialize",
+  "classes": {
+   "materialize:index/sCIM2GroupRoles:SCIM2GroupRoles": "SCIM2GroupRoles"
+  }
+ },
+ {
+  "pkg": "materialize",
+  "mod": "index/sCIM2GroupUsers",
+  "fqn": "pulumi_materialize",
+  "classes": {
+   "materialize:index/sCIM2GroupUsers:SCIM2GroupUsers": "SCIM2GroupUsers"
+  }
+ },
+ {
+  "pkg": "materialize",
   "mod": "index/sSOConfig",
   "fqn": "pulumi_materialize",
   "classes": {
    "materialize:index/sSOConfig:SSOConfig": "SSOConfig"
   }
  },
  {
```

### Comparing `pulumi_materialize-0.1.9/pulumi_materialize/_inputs.py` & `pulumi_materialize-0.2.0/pulumi_materialize/_inputs.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
 __all__ = [
+    'ClusterSchedulingArgs',
+    'ClusterSchedulingOnRefreshArgs',
     'ConnectionAwsAccessKeyIdArgs',
     'ConnectionAwsAccessKeyIdSecretArgs',
     'ConnectionAwsSecretAccessKeyArgs',
     'ConnectionAwsSessionTokenArgs',
     'ConnectionAwsSessionTokenSecretArgs',
     'ConnectionConfluentSchemaRegistryAwsPrivatelinkArgs',
     'ConnectionConfluentSchemaRegistryPasswordArgs',
@@ -92,14 +94,15 @@
     'SourceKafkaValueFormatAvroSchemaRegistryConnectionArgs',
     'SourceKafkaValueFormatCsvArgs',
     'SourceKafkaValueFormatProtobufArgs',
     'SourceKafkaValueFormatProtobufSchemaRegistryConnectionArgs',
     'SourceLoadgenAuctionOptionsArgs',
     'SourceLoadgenCounterOptionsArgs',
     'SourceLoadgenExposeProgressArgs',
+    'SourceLoadgenKeyValueOptionsArgs',
     'SourceLoadgenMarketingOptionsArgs',
     'SourceLoadgenSubsourceArgs',
     'SourceLoadgenTpchOptionsArgs',
     'SourceMysqlMysqlConnectionArgs',
     'SourceMysqlSubsourceArgs',
     'SourceMysqlTableArgs',
     'SourcePostgresExposeProgressArgs',
@@ -115,14 +118,66 @@
     'TableColumnArgs',
     'TypeListPropertiesArgs',
     'TypeMapPropertiesArgs',
     'TypeRowPropertyArgs',
 ]
 
 @pulumi.input_type
+class ClusterSchedulingArgs:
+    def __init__(__self__, *,
+                 on_refresh: Optional[pulumi.Input['ClusterSchedulingOnRefreshArgs']] = None):
+        """
+        :param pulumi.Input['ClusterSchedulingOnRefreshArgs'] on_refresh: Configuration for refreshing the cluster.
+        """
+        if on_refresh is not None:
+            pulumi.set(__self__, "on_refresh", on_refresh)
+
+    @property
+    @pulumi.getter(name="onRefresh")
+    def on_refresh(self) -> Optional[pulumi.Input['ClusterSchedulingOnRefreshArgs']]:
+        """
+        Configuration for refreshing the cluster.
+        """
+        return pulumi.get(self, "on_refresh")
+
+    @on_refresh.setter
+    def on_refresh(self, value: Optional[pulumi.Input['ClusterSchedulingOnRefreshArgs']]):
+        pulumi.set(self, "on_refresh", value)
+
+
+@pulumi.input_type
+class ClusterSchedulingOnRefreshArgs:
+    def __init__(__self__, *,
+                 enabled: Optional[pulumi.Input[bool]] = None,
+                 rehydration_time_estimate: Optional[pulumi.Input[str]] = None):
+        if enabled is not None:
+            pulumi.set(__self__, "enabled", enabled)
+        if rehydration_time_estimate is not None:
+            pulumi.set(__self__, "rehydration_time_estimate", rehydration_time_estimate)
+
+    @property
+    @pulumi.getter
+    def enabled(self) -> Optional[pulumi.Input[bool]]:
+        return pulumi.get(self, "enabled")
+
+    @enabled.setter
+    def enabled(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "enabled", value)
+
+    @property
+    @pulumi.getter(name="rehydrationTimeEstimate")
+    def rehydration_time_estimate(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "rehydration_time_estimate")
+
+    @rehydration_time_estimate.setter
+    def rehydration_time_estimate(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "rehydration_time_estimate", value)
+
+
+@pulumi.input_type
 class ConnectionAwsAccessKeyIdArgs:
     def __init__(__self__, *,
                  secret: Optional[pulumi.Input['ConnectionAwsAccessKeyIdSecretArgs']] = None,
                  text: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input['ConnectionAwsAccessKeyIdSecretArgs'] secret: The `access_key_id` secret value. Conflicts with `text` within this block.
         :param pulumi.Input[str] text: The `access_key_id` text value. Conflicts with `secret` within this block
@@ -4513,14 +4568,148 @@
 
     @schema_name.setter
     def schema_name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "schema_name", value)
 
 
 @pulumi.input_type
+class SourceLoadgenKeyValueOptionsArgs:
+    def __init__(__self__, *,
+                 keys: pulumi.Input[int],
+                 batch_size: Optional[pulumi.Input[int]] = None,
+                 partitions: Optional[pulumi.Input[int]] = None,
+                 seed: Optional[pulumi.Input[int]] = None,
+                 snapshot_rounds: Optional[pulumi.Input[int]] = None,
+                 tick_interval: Optional[pulumi.Input[str]] = None,
+                 transactional_snapshot: Optional[pulumi.Input[bool]] = None,
+                 value_size: Optional[pulumi.Input[int]] = None):
+        """
+        :param pulumi.Input[int] keys: The number of keys in the source. This must be divisible by the product of 'partitions' and 'batch_size'.
+        :param pulumi.Input[int] batch_size: The number of keys per partition to produce in each update.
+        :param pulumi.Input[int] partitions: The number of partitions to spread the keys across.
+        :param pulumi.Input[int] seed: A per-source seed for seeding the random data.
+        :param pulumi.Input[int] snapshot_rounds: The number of rounds of data to produce as the source starts up.
+        :param pulumi.Input[str] tick_interval: The interval at which the next datum should be emitted. Defaults to one second.
+        :param pulumi.Input[bool] transactional_snapshot: Whether to emit the snapshot as a singular transaction.
+        :param pulumi.Input[int] value_size: The number of bytes in each value.
+        """
+        pulumi.set(__self__, "keys", keys)
+        if batch_size is not None:
+            pulumi.set(__self__, "batch_size", batch_size)
+        if partitions is not None:
+            pulumi.set(__self__, "partitions", partitions)
+        if seed is not None:
+            pulumi.set(__self__, "seed", seed)
+        if snapshot_rounds is not None:
+            pulumi.set(__self__, "snapshot_rounds", snapshot_rounds)
+        if tick_interval is not None:
+            pulumi.set(__self__, "tick_interval", tick_interval)
+        if transactional_snapshot is not None:
+            pulumi.set(__self__, "transactional_snapshot", transactional_snapshot)
+        if value_size is not None:
+            pulumi.set(__self__, "value_size", value_size)
+
+    @property
+    @pulumi.getter
+    def keys(self) -> pulumi.Input[int]:
+        """
+        The number of keys in the source. This must be divisible by the product of 'partitions' and 'batch_size'.
+        """
+        return pulumi.get(self, "keys")
+
+    @keys.setter
+    def keys(self, value: pulumi.Input[int]):
+        pulumi.set(self, "keys", value)
+
+    @property
+    @pulumi.getter(name="batchSize")
+    def batch_size(self) -> Optional[pulumi.Input[int]]:
+        """
+        The number of keys per partition to produce in each update.
+        """
+        return pulumi.get(self, "batch_size")
+
+    @batch_size.setter
+    def batch_size(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "batch_size", value)
+
+    @property
+    @pulumi.getter
+    def partitions(self) -> Optional[pulumi.Input[int]]:
+        """
+        The number of partitions to spread the keys across.
+        """
+        return pulumi.get(self, "partitions")
+
+    @partitions.setter
+    def partitions(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "partitions", value)
+
+    @property
+    @pulumi.getter
+    def seed(self) -> Optional[pulumi.Input[int]]:
+        """
+        A per-source seed for seeding the random data.
+        """
+        return pulumi.get(self, "seed")
+
+    @seed.setter
+    def seed(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "seed", value)
+
+    @property
+    @pulumi.getter(name="snapshotRounds")
+    def snapshot_rounds(self) -> Optional[pulumi.Input[int]]:
+        """
+        The number of rounds of data to produce as the source starts up.
+        """
+        return pulumi.get(self, "snapshot_rounds")
+
+    @snapshot_rounds.setter
+    def snapshot_rounds(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "snapshot_rounds", value)
+
+    @property
+    @pulumi.getter(name="tickInterval")
+    def tick_interval(self) -> Optional[pulumi.Input[str]]:
+        """
+        The interval at which the next datum should be emitted. Defaults to one second.
+        """
+        return pulumi.get(self, "tick_interval")
+
+    @tick_interval.setter
+    def tick_interval(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "tick_interval", value)
+
+    @property
+    @pulumi.getter(name="transactionalSnapshot")
+    def transactional_snapshot(self) -> Optional[pulumi.Input[bool]]:
+        """
+        Whether to emit the snapshot as a singular transaction.
+        """
+        return pulumi.get(self, "transactional_snapshot")
+
+    @transactional_snapshot.setter
+    def transactional_snapshot(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "transactional_snapshot", value)
+
+    @property
+    @pulumi.getter(name="valueSize")
+    def value_size(self) -> Optional[pulumi.Input[int]]:
+        """
+        The number of bytes in each value.
+        """
+        return pulumi.get(self, "value_size")
+
+    @value_size.setter
+    def value_size(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "value_size", value)
+
+
+@pulumi.input_type
 class SourceLoadgenMarketingOptionsArgs:
     def __init__(__self__, *,
                  scale_factor: Optional[pulumi.Input[float]] = None,
                  tick_interval: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[float] scale_factor: (Deprecated) The scale factor for the generator. Defaults to 0.01 (~ 10MB).
         :param pulumi.Input[str] tick_interval: The interval at which the next datum should be emitted. Defaults to one second.
```

### Comparing `pulumi_materialize-0.1.9/pulumi_materialize/_utilities.py` & `pulumi_materialize-0.2.0/pulumi_materialize/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.1.9/pulumi_materialize/app_password.py` & `pulumi_materialize-0.2.0/pulumi_materialize/app_password.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.1.9/pulumi_materialize/cluster.py` & `pulumi_materialize-0.2.0/pulumi_materialize/cluster.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,68 +4,70 @@
 
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
+from . import outputs
+from ._inputs import *
 
 __all__ = ['ClusterArgs', 'Cluster']
 
 @pulumi.input_type
 class ClusterArgs:
     def __init__(__self__, *,
                  availability_zones: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  comment: Optional[pulumi.Input[str]] = None,
                  disk: Optional[pulumi.Input[bool]] = None,
-                 idle_arrangement_merge_effort: Optional[pulumi.Input[int]] = None,
                  introspection_debugging: Optional[pulumi.Input[bool]] = None,
                  introspection_interval: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  ownership_role: Optional[pulumi.Input[str]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  replication_factor: Optional[pulumi.Input[int]] = None,
+                 scheduling: Optional[pulumi.Input['ClusterSchedulingArgs']] = None,
                  size: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a Cluster resource.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] availability_zones: The specific availability zones of the cluster.
         :param pulumi.Input[str] comment: **Public Preview** Comment on an object in the database.
         :param pulumi.Input[bool] disk: **Deprecated**. This attribute is maintained for backward compatibility with existing configurations. New users should use 'cc' sizes for disk access.
-        :param pulumi.Input[int] idle_arrangement_merge_effort: The amount of effort to exert compacting arrangements during idle periods. This is an unstable option! It may be changed or removed at any time.
         :param pulumi.Input[bool] introspection_debugging: Whether to introspect the gathering of the introspection data.
         :param pulumi.Input[str] introspection_interval: The interval at which to collect introspection data.
         :param pulumi.Input[str] name: The identifier for the cluster.
         :param pulumi.Input[str] ownership_role: The owernship role of the object.
         :param pulumi.Input[str] region: The region to use for the resource connection. If not set, the default region is used.
         :param pulumi.Input[int] replication_factor: The number of replicas of each dataflow-powered object to maintain.
+        :param pulumi.Input['ClusterSchedulingArgs'] scheduling: Defines the scheduling parameters for the cluster.
         :param pulumi.Input[str] size: The size of the managed cluster.
         """
         if availability_zones is not None:
             pulumi.set(__self__, "availability_zones", availability_zones)
         if comment is not None:
             pulumi.set(__self__, "comment", comment)
         if disk is not None:
             warnings.warn("""Disk replicas are deprecated and will be removed in a future release. The `disk` attribute will be enabled by default for 'cc' clusters""", DeprecationWarning)
             pulumi.log.warn("""disk is deprecated: Disk replicas are deprecated and will be removed in a future release. The `disk` attribute will be enabled by default for 'cc' clusters""")
         if disk is not None:
             pulumi.set(__self__, "disk", disk)
-        if idle_arrangement_merge_effort is not None:
-            pulumi.set(__self__, "idle_arrangement_merge_effort", idle_arrangement_merge_effort)
         if introspection_debugging is not None:
             pulumi.set(__self__, "introspection_debugging", introspection_debugging)
         if introspection_interval is not None:
             pulumi.set(__self__, "introspection_interval", introspection_interval)
         if name is not None:
             pulumi.set(__self__, "name", name)
         if ownership_role is not None:
             pulumi.set(__self__, "ownership_role", ownership_role)
         if region is not None:
             pulumi.set(__self__, "region", region)
         if replication_factor is not None:
             pulumi.set(__self__, "replication_factor", replication_factor)
+        if scheduling is not None:
+            pulumi.set(__self__, "scheduling", scheduling)
         if size is not None:
             pulumi.set(__self__, "size", size)
 
     @property
     @pulumi.getter(name="availabilityZones")
     def availability_zones(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
@@ -101,26 +103,14 @@
         return pulumi.get(self, "disk")
 
     @disk.setter
     def disk(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "disk", value)
 
     @property
-    @pulumi.getter(name="idleArrangementMergeEffort")
-    def idle_arrangement_merge_effort(self) -> Optional[pulumi.Input[int]]:
-        """
-        The amount of effort to exert compacting arrangements during idle periods. This is an unstable option! It may be changed or removed at any time.
-        """
-        return pulumi.get(self, "idle_arrangement_merge_effort")
-
-    @idle_arrangement_merge_effort.setter
-    def idle_arrangement_merge_effort(self, value: Optional[pulumi.Input[int]]):
-        pulumi.set(self, "idle_arrangement_merge_effort", value)
-
-    @property
     @pulumi.getter(name="introspectionDebugging")
     def introspection_debugging(self) -> Optional[pulumi.Input[bool]]:
         """
         Whether to introspect the gathering of the introspection data.
         """
         return pulumi.get(self, "introspection_debugging")
 
@@ -186,14 +176,26 @@
 
     @replication_factor.setter
     def replication_factor(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "replication_factor", value)
 
     @property
     @pulumi.getter
+    def scheduling(self) -> Optional[pulumi.Input['ClusterSchedulingArgs']]:
+        """
+        Defines the scheduling parameters for the cluster.
+        """
+        return pulumi.get(self, "scheduling")
+
+    @scheduling.setter
+    def scheduling(self, value: Optional[pulumi.Input['ClusterSchedulingArgs']]):
+        pulumi.set(self, "scheduling", value)
+
+    @property
+    @pulumi.getter
     def size(self) -> Optional[pulumi.Input[str]]:
         """
         The size of the managed cluster.
         """
         return pulumi.get(self, "size")
 
     @size.setter
@@ -203,59 +205,59 @@
 
 @pulumi.input_type
 class _ClusterState:
     def __init__(__self__, *,
                  availability_zones: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  comment: Optional[pulumi.Input[str]] = None,
                  disk: Optional[pulumi.Input[bool]] = None,
-                 idle_arrangement_merge_effort: Optional[pulumi.Input[int]] = None,
                  introspection_debugging: Optional[pulumi.Input[bool]] = None,
                  introspection_interval: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  ownership_role: Optional[pulumi.Input[str]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  replication_factor: Optional[pulumi.Input[int]] = None,
+                 scheduling: Optional[pulumi.Input['ClusterSchedulingArgs']] = None,
                  size: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering Cluster resources.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] availability_zones: The specific availability zones of the cluster.
         :param pulumi.Input[str] comment: **Public Preview** Comment on an object in the database.
         :param pulumi.Input[bool] disk: **Deprecated**. This attribute is maintained for backward compatibility with existing configurations. New users should use 'cc' sizes for disk access.
-        :param pulumi.Input[int] idle_arrangement_merge_effort: The amount of effort to exert compacting arrangements during idle periods. This is an unstable option! It may be changed or removed at any time.
         :param pulumi.Input[bool] introspection_debugging: Whether to introspect the gathering of the introspection data.
         :param pulumi.Input[str] introspection_interval: The interval at which to collect introspection data.
         :param pulumi.Input[str] name: The identifier for the cluster.
         :param pulumi.Input[str] ownership_role: The owernship role of the object.
         :param pulumi.Input[str] region: The region to use for the resource connection. If not set, the default region is used.
         :param pulumi.Input[int] replication_factor: The number of replicas of each dataflow-powered object to maintain.
+        :param pulumi.Input['ClusterSchedulingArgs'] scheduling: Defines the scheduling parameters for the cluster.
         :param pulumi.Input[str] size: The size of the managed cluster.
         """
         if availability_zones is not None:
             pulumi.set(__self__, "availability_zones", availability_zones)
         if comment is not None:
             pulumi.set(__self__, "comment", comment)
         if disk is not None:
             warnings.warn("""Disk replicas are deprecated and will be removed in a future release. The `disk` attribute will be enabled by default for 'cc' clusters""", DeprecationWarning)
             pulumi.log.warn("""disk is deprecated: Disk replicas are deprecated and will be removed in a future release. The `disk` attribute will be enabled by default for 'cc' clusters""")
         if disk is not None:
             pulumi.set(__self__, "disk", disk)
-        if idle_arrangement_merge_effort is not None:
-            pulumi.set(__self__, "idle_arrangement_merge_effort", idle_arrangement_merge_effort)
         if introspection_debugging is not None:
             pulumi.set(__self__, "introspection_debugging", introspection_debugging)
         if introspection_interval is not None:
             pulumi.set(__self__, "introspection_interval", introspection_interval)
         if name is not None:
             pulumi.set(__self__, "name", name)
         if ownership_role is not None:
             pulumi.set(__self__, "ownership_role", ownership_role)
         if region is not None:
             pulumi.set(__self__, "region", region)
         if replication_factor is not None:
             pulumi.set(__self__, "replication_factor", replication_factor)
+        if scheduling is not None:
+            pulumi.set(__self__, "scheduling", scheduling)
         if size is not None:
             pulumi.set(__self__, "size", size)
 
     @property
     @pulumi.getter(name="availabilityZones")
     def availability_zones(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
@@ -291,26 +293,14 @@
         return pulumi.get(self, "disk")
 
     @disk.setter
     def disk(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "disk", value)
 
     @property
-    @pulumi.getter(name="idleArrangementMergeEffort")
-    def idle_arrangement_merge_effort(self) -> Optional[pulumi.Input[int]]:
-        """
-        The amount of effort to exert compacting arrangements during idle periods. This is an unstable option! It may be changed or removed at any time.
-        """
-        return pulumi.get(self, "idle_arrangement_merge_effort")
-
-    @idle_arrangement_merge_effort.setter
-    def idle_arrangement_merge_effort(self, value: Optional[pulumi.Input[int]]):
-        pulumi.set(self, "idle_arrangement_merge_effort", value)
-
-    @property
     @pulumi.getter(name="introspectionDebugging")
     def introspection_debugging(self) -> Optional[pulumi.Input[bool]]:
         """
         Whether to introspect the gathering of the introspection data.
         """
         return pulumi.get(self, "introspection_debugging")
 
@@ -376,14 +366,26 @@
 
     @replication_factor.setter
     def replication_factor(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "replication_factor", value)
 
     @property
     @pulumi.getter
+    def scheduling(self) -> Optional[pulumi.Input['ClusterSchedulingArgs']]:
+        """
+        Defines the scheduling parameters for the cluster.
+        """
+        return pulumi.get(self, "scheduling")
+
+    @scheduling.setter
+    def scheduling(self, value: Optional[pulumi.Input['ClusterSchedulingArgs']]):
+        pulumi.set(self, "scheduling", value)
+
+    @property
+    @pulumi.getter
     def size(self) -> Optional[pulumi.Input[str]]:
         """
         The size of the managed cluster.
         """
         return pulumi.get(self, "size")
 
     @size.setter
@@ -395,21 +397,21 @@
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  availability_zones: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  comment: Optional[pulumi.Input[str]] = None,
                  disk: Optional[pulumi.Input[bool]] = None,
-                 idle_arrangement_merge_effort: Optional[pulumi.Input[int]] = None,
                  introspection_debugging: Optional[pulumi.Input[bool]] = None,
                  introspection_interval: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  ownership_role: Optional[pulumi.Input[str]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  replication_factor: Optional[pulumi.Input[int]] = None,
+                 scheduling: Optional[pulumi.Input[pulumi.InputType['ClusterSchedulingArgs']]] = None,
                  size: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Clusters describe logical compute resources that can be used by sources, sinks, indexes, and materialized views. Managed clusters are created by setting the `size` attribute
 
         ## Example Usage
 
@@ -431,21 +433,21 @@
          Cluster id and information be found in the `mz_catalog.mz_clusters` table The region is the region where the database is located (e.g. aws/us-east-1)
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] availability_zones: The specific availability zones of the cluster.
         :param pulumi.Input[str] comment: **Public Preview** Comment on an object in the database.
         :param pulumi.Input[bool] disk: **Deprecated**. This attribute is maintained for backward compatibility with existing configurations. New users should use 'cc' sizes for disk access.
-        :param pulumi.Input[int] idle_arrangement_merge_effort: The amount of effort to exert compacting arrangements during idle periods. This is an unstable option! It may be changed or removed at any time.
         :param pulumi.Input[bool] introspection_debugging: Whether to introspect the gathering of the introspection data.
         :param pulumi.Input[str] introspection_interval: The interval at which to collect introspection data.
         :param pulumi.Input[str] name: The identifier for the cluster.
         :param pulumi.Input[str] ownership_role: The owernship role of the object.
         :param pulumi.Input[str] region: The region to use for the resource connection. If not set, the default region is used.
         :param pulumi.Input[int] replication_factor: The number of replicas of each dataflow-powered object to maintain.
+        :param pulumi.Input[pulumi.InputType['ClusterSchedulingArgs']] scheduling: Defines the scheduling parameters for the cluster.
         :param pulumi.Input[str] size: The size of the managed cluster.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: Optional[ClusterArgs] = None,
@@ -486,21 +488,21 @@
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  availability_zones: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  comment: Optional[pulumi.Input[str]] = None,
                  disk: Optional[pulumi.Input[bool]] = None,
-                 idle_arrangement_merge_effort: Optional[pulumi.Input[int]] = None,
                  introspection_debugging: Optional[pulumi.Input[bool]] = None,
                  introspection_interval: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  ownership_role: Optional[pulumi.Input[str]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  replication_factor: Optional[pulumi.Input[int]] = None,
+                 scheduling: Optional[pulumi.Input[pulumi.InputType['ClusterSchedulingArgs']]] = None,
                  size: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
@@ -509,76 +511,76 @@
 
             __props__.__dict__["availability_zones"] = availability_zones
             __props__.__dict__["comment"] = comment
             if disk is not None and not opts.urn:
                 warnings.warn("""Disk replicas are deprecated and will be removed in a future release. The `disk` attribute will be enabled by default for 'cc' clusters""", DeprecationWarning)
                 pulumi.log.warn("""disk is deprecated: Disk replicas are deprecated and will be removed in a future release. The `disk` attribute will be enabled by default for 'cc' clusters""")
             __props__.__dict__["disk"] = disk
-            __props__.__dict__["idle_arrangement_merge_effort"] = idle_arrangement_merge_effort
             __props__.__dict__["introspection_debugging"] = introspection_debugging
             __props__.__dict__["introspection_interval"] = introspection_interval
             __props__.__dict__["name"] = name
             __props__.__dict__["ownership_role"] = ownership_role
             __props__.__dict__["region"] = region
             __props__.__dict__["replication_factor"] = replication_factor
+            __props__.__dict__["scheduling"] = scheduling
             __props__.__dict__["size"] = size
         super(Cluster, __self__).__init__(
             'materialize:index/cluster:Cluster',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
             availability_zones: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
             comment: Optional[pulumi.Input[str]] = None,
             disk: Optional[pulumi.Input[bool]] = None,
-            idle_arrangement_merge_effort: Optional[pulumi.Input[int]] = None,
             introspection_debugging: Optional[pulumi.Input[bool]] = None,
             introspection_interval: Optional[pulumi.Input[str]] = None,
             name: Optional[pulumi.Input[str]] = None,
             ownership_role: Optional[pulumi.Input[str]] = None,
             region: Optional[pulumi.Input[str]] = None,
             replication_factor: Optional[pulumi.Input[int]] = None,
+            scheduling: Optional[pulumi.Input[pulumi.InputType['ClusterSchedulingArgs']]] = None,
             size: Optional[pulumi.Input[str]] = None) -> 'Cluster':
         """
         Get an existing Cluster resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] availability_zones: The specific availability zones of the cluster.
         :param pulumi.Input[str] comment: **Public Preview** Comment on an object in the database.
         :param pulumi.Input[bool] disk: **Deprecated**. This attribute is maintained for backward compatibility with existing configurations. New users should use 'cc' sizes for disk access.
-        :param pulumi.Input[int] idle_arrangement_merge_effort: The amount of effort to exert compacting arrangements during idle periods. This is an unstable option! It may be changed or removed at any time.
         :param pulumi.Input[bool] introspection_debugging: Whether to introspect the gathering of the introspection data.
         :param pulumi.Input[str] introspection_interval: The interval at which to collect introspection data.
         :param pulumi.Input[str] name: The identifier for the cluster.
         :param pulumi.Input[str] ownership_role: The owernship role of the object.
         :param pulumi.Input[str] region: The region to use for the resource connection. If not set, the default region is used.
         :param pulumi.Input[int] replication_factor: The number of replicas of each dataflow-powered object to maintain.
+        :param pulumi.Input[pulumi.InputType['ClusterSchedulingArgs']] scheduling: Defines the scheduling parameters for the cluster.
         :param pulumi.Input[str] size: The size of the managed cluster.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _ClusterState.__new__(_ClusterState)
 
         __props__.__dict__["availability_zones"] = availability_zones
         __props__.__dict__["comment"] = comment
         __props__.__dict__["disk"] = disk
-        __props__.__dict__["idle_arrangement_merge_effort"] = idle_arrangement_merge_effort
         __props__.__dict__["introspection_debugging"] = introspection_debugging
         __props__.__dict__["introspection_interval"] = introspection_interval
         __props__.__dict__["name"] = name
         __props__.__dict__["ownership_role"] = ownership_role
         __props__.__dict__["region"] = region
         __props__.__dict__["replication_factor"] = replication_factor
+        __props__.__dict__["scheduling"] = scheduling
         __props__.__dict__["size"] = size
         return Cluster(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter(name="availabilityZones")
     def availability_zones(self) -> pulumi.Output[Sequence[str]]:
         """
@@ -602,22 +604,14 @@
         """
         warnings.warn("""Disk replicas are deprecated and will be removed in a future release. The `disk` attribute will be enabled by default for 'cc' clusters""", DeprecationWarning)
         pulumi.log.warn("""disk is deprecated: Disk replicas are deprecated and will be removed in a future release. The `disk` attribute will be enabled by default for 'cc' clusters""")
 
         return pulumi.get(self, "disk")
 
     @property
-    @pulumi.getter(name="idleArrangementMergeEffort")
-    def idle_arrangement_merge_effort(self) -> pulumi.Output[Optional[int]]:
-        """
-        The amount of effort to exert compacting arrangements during idle periods. This is an unstable option! It may be changed or removed at any time.
-        """
-        return pulumi.get(self, "idle_arrangement_merge_effort")
-
-    @property
     @pulumi.getter(name="introspectionDebugging")
     def introspection_debugging(self) -> pulumi.Output[Optional[bool]]:
         """
         Whether to introspect the gathering of the introspection data.
         """
         return pulumi.get(self, "introspection_debugging")
 
@@ -659,13 +653,21 @@
         """
         The number of replicas of each dataflow-powered object to maintain.
         """
         return pulumi.get(self, "replication_factor")
 
     @property
     @pulumi.getter
+    def scheduling(self) -> pulumi.Output[Optional['outputs.ClusterScheduling']]:
+        """
+        Defines the scheduling parameters for the cluster.
+        """
+        return pulumi.get(self, "scheduling")
+
+    @property
+    @pulumi.getter
     def size(self) -> pulumi.Output[Optional[str]]:
         """
         The size of the managed cluster.
         """
         return pulumi.get(self, "size")
```

### Comparing `pulumi_materialize-0.1.9/pulumi_materialize/cluster_replica.py` & `pulumi_materialize-0.2.0/pulumi_materialize/cluster_replica.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,27 +15,25 @@
 class ClusterReplicaArgs:
     def __init__(__self__, *,
                  cluster_name: pulumi.Input[str],
                  size: pulumi.Input[str],
                  availability_zone: Optional[pulumi.Input[str]] = None,
                  comment: Optional[pulumi.Input[str]] = None,
                  disk: Optional[pulumi.Input[bool]] = None,
-                 idle_arrangement_merge_effort: Optional[pulumi.Input[int]] = None,
                  introspection_debugging: Optional[pulumi.Input[bool]] = None,
                  introspection_interval: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  region: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a ClusterReplica resource.
         :param pulumi.Input[str] cluster_name: The cluster whose resources you want to create an additional computation of.
         :param pulumi.Input[str] size: The size of the replica.
         :param pulumi.Input[str] availability_zone: The specific availability zone of the replica.
         :param pulumi.Input[str] comment: **Public Preview** Comment on an object in the database.
         :param pulumi.Input[bool] disk: **Deprecated**. This attribute is maintained for backward compatibility with existing configurations. New users should use 'cc' sizes for disk access.
-        :param pulumi.Input[int] idle_arrangement_merge_effort: The amount of effort to exert compacting arrangements during idle periods. This is an unstable option! It may be changed or removed at any time.
         :param pulumi.Input[bool] introspection_debugging: Whether to introspect the gathering of the introspection data.
         :param pulumi.Input[str] introspection_interval: The interval at which to collect introspection data.
         :param pulumi.Input[str] name: The identifier for the replica.
         :param pulumi.Input[str] region: The region to use for the resource connection. If not set, the default region is used.
         """
         pulumi.set(__self__, "cluster_name", cluster_name)
         pulumi.set(__self__, "size", size)
@@ -44,16 +42,14 @@
         if comment is not None:
             pulumi.set(__self__, "comment", comment)
         if disk is not None:
             warnings.warn("""Disk replicas are deprecated and will be removed in a future release. The `disk` attribute will be enabled by default for 'cc' clusters""", DeprecationWarning)
             pulumi.log.warn("""disk is deprecated: Disk replicas are deprecated and will be removed in a future release. The `disk` attribute will be enabled by default for 'cc' clusters""")
         if disk is not None:
             pulumi.set(__self__, "disk", disk)
-        if idle_arrangement_merge_effort is not None:
-            pulumi.set(__self__, "idle_arrangement_merge_effort", idle_arrangement_merge_effort)
         if introspection_debugging is not None:
             pulumi.set(__self__, "introspection_debugging", introspection_debugging)
         if introspection_interval is not None:
             pulumi.set(__self__, "introspection_interval", introspection_interval)
         if name is not None:
             pulumi.set(__self__, "name", name)
         if region is not None:
@@ -119,26 +115,14 @@
         return pulumi.get(self, "disk")
 
     @disk.setter
     def disk(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "disk", value)
 
     @property
-    @pulumi.getter(name="idleArrangementMergeEffort")
-    def idle_arrangement_merge_effort(self) -> Optional[pulumi.Input[int]]:
-        """
-        The amount of effort to exert compacting arrangements during idle periods. This is an unstable option! It may be changed or removed at any time.
-        """
-        return pulumi.get(self, "idle_arrangement_merge_effort")
-
-    @idle_arrangement_merge_effort.setter
-    def idle_arrangement_merge_effort(self, value: Optional[pulumi.Input[int]]):
-        pulumi.set(self, "idle_arrangement_merge_effort", value)
-
-    @property
     @pulumi.getter(name="introspectionDebugging")
     def introspection_debugging(self) -> Optional[pulumi.Input[bool]]:
         """
         Whether to introspect the gathering of the introspection data.
         """
         return pulumi.get(self, "introspection_debugging")
 
@@ -186,27 +170,25 @@
 @pulumi.input_type
 class _ClusterReplicaState:
     def __init__(__self__, *,
                  availability_zone: Optional[pulumi.Input[str]] = None,
                  cluster_name: Optional[pulumi.Input[str]] = None,
                  comment: Optional[pulumi.Input[str]] = None,
                  disk: Optional[pulumi.Input[bool]] = None,
-                 idle_arrangement_merge_effort: Optional[pulumi.Input[int]] = None,
                  introspection_debugging: Optional[pulumi.Input[bool]] = None,
                  introspection_interval: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  size: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering ClusterReplica resources.
         :param pulumi.Input[str] availability_zone: The specific availability zone of the replica.
         :param pulumi.Input[str] cluster_name: The cluster whose resources you want to create an additional computation of.
         :param pulumi.Input[str] comment: **Public Preview** Comment on an object in the database.
         :param pulumi.Input[bool] disk: **Deprecated**. This attribute is maintained for backward compatibility with existing configurations. New users should use 'cc' sizes for disk access.
-        :param pulumi.Input[int] idle_arrangement_merge_effort: The amount of effort to exert compacting arrangements during idle periods. This is an unstable option! It may be changed or removed at any time.
         :param pulumi.Input[bool] introspection_debugging: Whether to introspect the gathering of the introspection data.
         :param pulumi.Input[str] introspection_interval: The interval at which to collect introspection data.
         :param pulumi.Input[str] name: The identifier for the replica.
         :param pulumi.Input[str] region: The region to use for the resource connection. If not set, the default region is used.
         :param pulumi.Input[str] size: The size of the replica.
         """
         if availability_zone is not None:
@@ -216,16 +198,14 @@
         if comment is not None:
             pulumi.set(__self__, "comment", comment)
         if disk is not None:
             warnings.warn("""Disk replicas are deprecated and will be removed in a future release. The `disk` attribute will be enabled by default for 'cc' clusters""", DeprecationWarning)
             pulumi.log.warn("""disk is deprecated: Disk replicas are deprecated and will be removed in a future release. The `disk` attribute will be enabled by default for 'cc' clusters""")
         if disk is not None:
             pulumi.set(__self__, "disk", disk)
-        if idle_arrangement_merge_effort is not None:
-            pulumi.set(__self__, "idle_arrangement_merge_effort", idle_arrangement_merge_effort)
         if introspection_debugging is not None:
             pulumi.set(__self__, "introspection_debugging", introspection_debugging)
         if introspection_interval is not None:
             pulumi.set(__self__, "introspection_interval", introspection_interval)
         if name is not None:
             pulumi.set(__self__, "name", name)
         if region is not None:
@@ -281,26 +261,14 @@
         return pulumi.get(self, "disk")
 
     @disk.setter
     def disk(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "disk", value)
 
     @property
-    @pulumi.getter(name="idleArrangementMergeEffort")
-    def idle_arrangement_merge_effort(self) -> Optional[pulumi.Input[int]]:
-        """
-        The amount of effort to exert compacting arrangements during idle periods. This is an unstable option! It may be changed or removed at any time.
-        """
-        return pulumi.get(self, "idle_arrangement_merge_effort")
-
-    @idle_arrangement_merge_effort.setter
-    def idle_arrangement_merge_effort(self, value: Optional[pulumi.Input[int]]):
-        pulumi.set(self, "idle_arrangement_merge_effort", value)
-
-    @property
     @pulumi.getter(name="introspectionDebugging")
     def introspection_debugging(self) -> Optional[pulumi.Input[bool]]:
         """
         Whether to introspect the gathering of the introspection data.
         """
         return pulumi.get(self, "introspection_debugging")
 
@@ -362,15 +330,14 @@
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  availability_zone: Optional[pulumi.Input[str]] = None,
                  cluster_name: Optional[pulumi.Input[str]] = None,
                  comment: Optional[pulumi.Input[str]] = None,
                  disk: Optional[pulumi.Input[bool]] = None,
-                 idle_arrangement_merge_effort: Optional[pulumi.Input[int]] = None,
                  introspection_debugging: Optional[pulumi.Input[bool]] = None,
                  introspection_interval: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  size: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
@@ -401,15 +368,14 @@
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] availability_zone: The specific availability zone of the replica.
         :param pulumi.Input[str] cluster_name: The cluster whose resources you want to create an additional computation of.
         :param pulumi.Input[str] comment: **Public Preview** Comment on an object in the database.
         :param pulumi.Input[bool] disk: **Deprecated**. This attribute is maintained for backward compatibility with existing configurations. New users should use 'cc' sizes for disk access.
-        :param pulumi.Input[int] idle_arrangement_merge_effort: The amount of effort to exert compacting arrangements during idle periods. This is an unstable option! It may be changed or removed at any time.
         :param pulumi.Input[bool] introspection_debugging: Whether to introspect the gathering of the introspection data.
         :param pulumi.Input[str] introspection_interval: The interval at which to collect introspection data.
         :param pulumi.Input[str] name: The identifier for the replica.
         :param pulumi.Input[str] region: The region to use for the resource connection. If not set, the default region is used.
         :param pulumi.Input[str] size: The size of the replica.
         """
         ...
@@ -459,15 +425,14 @@
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  availability_zone: Optional[pulumi.Input[str]] = None,
                  cluster_name: Optional[pulumi.Input[str]] = None,
                  comment: Optional[pulumi.Input[str]] = None,
                  disk: Optional[pulumi.Input[bool]] = None,
-                 idle_arrangement_merge_effort: Optional[pulumi.Input[int]] = None,
                  introspection_debugging: Optional[pulumi.Input[bool]] = None,
                  introspection_interval: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  size: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
@@ -483,15 +448,14 @@
                 raise TypeError("Missing required property 'cluster_name'")
             __props__.__dict__["cluster_name"] = cluster_name
             __props__.__dict__["comment"] = comment
             if disk is not None and not opts.urn:
                 warnings.warn("""Disk replicas are deprecated and will be removed in a future release. The `disk` attribute will be enabled by default for 'cc' clusters""", DeprecationWarning)
                 pulumi.log.warn("""disk is deprecated: Disk replicas are deprecated and will be removed in a future release. The `disk` attribute will be enabled by default for 'cc' clusters""")
             __props__.__dict__["disk"] = disk
-            __props__.__dict__["idle_arrangement_merge_effort"] = idle_arrangement_merge_effort
             __props__.__dict__["introspection_debugging"] = introspection_debugging
             __props__.__dict__["introspection_interval"] = introspection_interval
             __props__.__dict__["name"] = name
             __props__.__dict__["region"] = region
             if size is None and not opts.urn:
                 raise TypeError("Missing required property 'size'")
             __props__.__dict__["size"] = size
@@ -505,15 +469,14 @@
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
             availability_zone: Optional[pulumi.Input[str]] = None,
             cluster_name: Optional[pulumi.Input[str]] = None,
             comment: Optional[pulumi.Input[str]] = None,
             disk: Optional[pulumi.Input[bool]] = None,
-            idle_arrangement_merge_effort: Optional[pulumi.Input[int]] = None,
             introspection_debugging: Optional[pulumi.Input[bool]] = None,
             introspection_interval: Optional[pulumi.Input[str]] = None,
             name: Optional[pulumi.Input[str]] = None,
             region: Optional[pulumi.Input[str]] = None,
             size: Optional[pulumi.Input[str]] = None) -> 'ClusterReplica':
         """
         Get an existing ClusterReplica resource's state with the given name, id, and optional extra
@@ -522,30 +485,28 @@
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] availability_zone: The specific availability zone of the replica.
         :param pulumi.Input[str] cluster_name: The cluster whose resources you want to create an additional computation of.
         :param pulumi.Input[str] comment: **Public Preview** Comment on an object in the database.
         :param pulumi.Input[bool] disk: **Deprecated**. This attribute is maintained for backward compatibility with existing configurations. New users should use 'cc' sizes for disk access.
-        :param pulumi.Input[int] idle_arrangement_merge_effort: The amount of effort to exert compacting arrangements during idle periods. This is an unstable option! It may be changed or removed at any time.
         :param pulumi.Input[bool] introspection_debugging: Whether to introspect the gathering of the introspection data.
         :param pulumi.Input[str] introspection_interval: The interval at which to collect introspection data.
         :param pulumi.Input[str] name: The identifier for the replica.
         :param pulumi.Input[str] region: The region to use for the resource connection. If not set, the default region is used.
         :param pulumi.Input[str] size: The size of the replica.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _ClusterReplicaState.__new__(_ClusterReplicaState)
 
         __props__.__dict__["availability_zone"] = availability_zone
         __props__.__dict__["cluster_name"] = cluster_name
         __props__.__dict__["comment"] = comment
         __props__.__dict__["disk"] = disk
-        __props__.__dict__["idle_arrangement_merge_effort"] = idle_arrangement_merge_effort
         __props__.__dict__["introspection_debugging"] = introspection_debugging
         __props__.__dict__["introspection_interval"] = introspection_interval
         __props__.__dict__["name"] = name
         __props__.__dict__["region"] = region
         __props__.__dict__["size"] = size
         return ClusterReplica(resource_name, opts=opts, __props__=__props__)
 
@@ -581,22 +542,14 @@
         """
         warnings.warn("""Disk replicas are deprecated and will be removed in a future release. The `disk` attribute will be enabled by default for 'cc' clusters""", DeprecationWarning)
         pulumi.log.warn("""disk is deprecated: Disk replicas are deprecated and will be removed in a future release. The `disk` attribute will be enabled by default for 'cc' clusters""")
 
         return pulumi.get(self, "disk")
 
     @property
-    @pulumi.getter(name="idleArrangementMergeEffort")
-    def idle_arrangement_merge_effort(self) -> pulumi.Output[Optional[int]]:
-        """
-        The amount of effort to exert compacting arrangements during idle periods. This is an unstable option! It may be changed or removed at any time.
-        """
-        return pulumi.get(self, "idle_arrangement_merge_effort")
-
-    @property
     @pulumi.getter(name="introspectionDebugging")
     def introspection_debugging(self) -> pulumi.Output[Optional[bool]]:
         """
         Whether to introspect the gathering of the introspection data.
         """
         return pulumi.get(self, "introspection_debugging")
```

### Comparing `pulumi_materialize-0.1.9/pulumi_materialize/config/vars.py` & `pulumi_materialize-0.2.0/pulumi_materialize/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.1.9/pulumi_materialize/connection_aws.py` & `pulumi_materialize-0.2.0/pulumi_materialize/connection_aws.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.1.9/pulumi_materialize/connection_aws_privatelink.py` & `pulumi_materialize-0.2.0/pulumi_materialize/connection_aws_privatelink.py`

 * *Files 11% similar despite different names*

```diff
@@ -17,25 +17,27 @@
                  availability_zones: pulumi.Input[Sequence[pulumi.Input[str]]],
                  service_name: pulumi.Input[str],
                  comment: Optional[pulumi.Input[str]] = None,
                  database_name: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  ownership_role: Optional[pulumi.Input[str]] = None,
                  region: Optional[pulumi.Input[str]] = None,
-                 schema_name: Optional[pulumi.Input[str]] = None):
+                 schema_name: Optional[pulumi.Input[str]] = None,
+                 validate: Optional[pulumi.Input[bool]] = None):
         """
         The set of arguments for constructing a ConnectionAwsPrivatelink resource.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] availability_zones: The availability zones of the AWS PrivateLink service.
         :param pulumi.Input[str] service_name: The name of the AWS PrivateLink service.
         :param pulumi.Input[str] comment: **Public Preview** Comment on an object in the database.
         :param pulumi.Input[str] database_name: The identifier for the connection database in Materialize. Defaults to `MZ_DATABASE` environment variable if set or `materialize` if environment variable is not set.
         :param pulumi.Input[str] name: The identifier for the connection.
         :param pulumi.Input[str] ownership_role: The owernship role of the object.
         :param pulumi.Input[str] region: The region to use for the resource connection. If not set, the default region is used.
         :param pulumi.Input[str] schema_name: The identifier for the connection schema in Materialize. Defaults to `public`.
+        :param pulumi.Input[bool] validate: **Private Preview** If the connection should wait for validation.
         """
         pulumi.set(__self__, "availability_zones", availability_zones)
         pulumi.set(__self__, "service_name", service_name)
         if comment is not None:
             pulumi.set(__self__, "comment", comment)
         if database_name is not None:
             pulumi.set(__self__, "database_name", database_name)
@@ -43,14 +45,16 @@
             pulumi.set(__self__, "name", name)
         if ownership_role is not None:
             pulumi.set(__self__, "ownership_role", ownership_role)
         if region is not None:
             pulumi.set(__self__, "region", region)
         if schema_name is not None:
             pulumi.set(__self__, "schema_name", schema_name)
+        if validate is not None:
+            pulumi.set(__self__, "validate", validate)
 
     @property
     @pulumi.getter(name="availabilityZones")
     def availability_zones(self) -> pulumi.Input[Sequence[pulumi.Input[str]]]:
         """
         The availability zones of the AWS PrivateLink service.
         """
@@ -140,40 +144,54 @@
         """
         return pulumi.get(self, "schema_name")
 
     @schema_name.setter
     def schema_name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "schema_name", value)
 
+    @property
+    @pulumi.getter
+    def validate(self) -> Optional[pulumi.Input[bool]]:
+        """
+        **Private Preview** If the connection should wait for validation.
+        """
+        return pulumi.get(self, "validate")
+
+    @validate.setter
+    def validate(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "validate", value)
+
 
 @pulumi.input_type
 class _ConnectionAwsPrivatelinkState:
     def __init__(__self__, *,
                  availability_zones: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  comment: Optional[pulumi.Input[str]] = None,
                  database_name: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  ownership_role: Optional[pulumi.Input[str]] = None,
                  principal: Optional[pulumi.Input[str]] = None,
                  qualified_sql_name: Optional[pulumi.Input[str]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  schema_name: Optional[pulumi.Input[str]] = None,
-                 service_name: Optional[pulumi.Input[str]] = None):
+                 service_name: Optional[pulumi.Input[str]] = None,
+                 validate: Optional[pulumi.Input[bool]] = None):
         """
         Input properties used for looking up and filtering ConnectionAwsPrivatelink resources.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] availability_zones: The availability zones of the AWS PrivateLink service.
         :param pulumi.Input[str] comment: **Public Preview** Comment on an object in the database.
         :param pulumi.Input[str] database_name: The identifier for the connection database in Materialize. Defaults to `MZ_DATABASE` environment variable if set or `materialize` if environment variable is not set.
         :param pulumi.Input[str] name: The identifier for the connection.
         :param pulumi.Input[str] ownership_role: The owernship role of the object.
         :param pulumi.Input[str] principal: The principal of the AWS PrivateLink service.
         :param pulumi.Input[str] qualified_sql_name: The fully qualified name of the connection.
         :param pulumi.Input[str] region: The region to use for the resource connection. If not set, the default region is used.
         :param pulumi.Input[str] schema_name: The identifier for the connection schema in Materialize. Defaults to `public`.
         :param pulumi.Input[str] service_name: The name of the AWS PrivateLink service.
+        :param pulumi.Input[bool] validate: **Private Preview** If the connection should wait for validation.
         """
         if availability_zones is not None:
             pulumi.set(__self__, "availability_zones", availability_zones)
         if comment is not None:
             pulumi.set(__self__, "comment", comment)
         if database_name is not None:
             pulumi.set(__self__, "database_name", database_name)
@@ -187,14 +205,16 @@
             pulumi.set(__self__, "qualified_sql_name", qualified_sql_name)
         if region is not None:
             pulumi.set(__self__, "region", region)
         if schema_name is not None:
             pulumi.set(__self__, "schema_name", schema_name)
         if service_name is not None:
             pulumi.set(__self__, "service_name", service_name)
+        if validate is not None:
+            pulumi.set(__self__, "validate", validate)
 
     @property
     @pulumi.getter(name="availabilityZones")
     def availability_zones(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
         The availability zones of the AWS PrivateLink service.
         """
@@ -308,28 +328,41 @@
         """
         return pulumi.get(self, "service_name")
 
     @service_name.setter
     def service_name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "service_name", value)
 
+    @property
+    @pulumi.getter
+    def validate(self) -> Optional[pulumi.Input[bool]]:
+        """
+        **Private Preview** If the connection should wait for validation.
+        """
+        return pulumi.get(self, "validate")
+
+    @validate.setter
+    def validate(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "validate", value)
+
 
 class ConnectionAwsPrivatelink(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  availability_zones: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  comment: Optional[pulumi.Input[str]] = None,
                  database_name: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  ownership_role: Optional[pulumi.Input[str]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  schema_name: Optional[pulumi.Input[str]] = None,
                  service_name: Optional[pulumi.Input[str]] = None,
+                 validate: Optional[pulumi.Input[bool]] = None,
                  __props__=None):
         """
         An AWS PrivateLink connection establishes a link to an AWS PrivateLink service.
 
         ## Example Usage
 
         ```python
@@ -364,14 +397,15 @@
         :param pulumi.Input[str] comment: **Public Preview** Comment on an object in the database.
         :param pulumi.Input[str] database_name: The identifier for the connection database in Materialize. Defaults to `MZ_DATABASE` environment variable if set or `materialize` if environment variable is not set.
         :param pulumi.Input[str] name: The identifier for the connection.
         :param pulumi.Input[str] ownership_role: The owernship role of the object.
         :param pulumi.Input[str] region: The region to use for the resource connection. If not set, the default region is used.
         :param pulumi.Input[str] schema_name: The identifier for the connection schema in Materialize. Defaults to `public`.
         :param pulumi.Input[str] service_name: The name of the AWS PrivateLink service.
+        :param pulumi.Input[bool] validate: **Private Preview** If the connection should wait for validation.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: ConnectionAwsPrivatelinkArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
@@ -425,14 +459,15 @@
                  comment: Optional[pulumi.Input[str]] = None,
                  database_name: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  ownership_role: Optional[pulumi.Input[str]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  schema_name: Optional[pulumi.Input[str]] = None,
                  service_name: Optional[pulumi.Input[str]] = None,
+                 validate: Optional[pulumi.Input[bool]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
@@ -446,14 +481,15 @@
             __props__.__dict__["name"] = name
             __props__.__dict__["ownership_role"] = ownership_role
             __props__.__dict__["region"] = region
             __props__.__dict__["schema_name"] = schema_name
             if service_name is None and not opts.urn:
                 raise TypeError("Missing required property 'service_name'")
             __props__.__dict__["service_name"] = service_name
+            __props__.__dict__["validate"] = validate
             __props__.__dict__["principal"] = None
             __props__.__dict__["qualified_sql_name"] = None
         secret_opts = pulumi.ResourceOptions(additional_secret_outputs=["principal"])
         opts = pulumi.ResourceOptions.merge(opts, secret_opts)
         super(ConnectionAwsPrivatelink, __self__).__init__(
             'materialize:index/connectionAwsPrivatelink:ConnectionAwsPrivatelink',
             resource_name,
@@ -469,15 +505,16 @@
             database_name: Optional[pulumi.Input[str]] = None,
             name: Optional[pulumi.Input[str]] = None,
             ownership_role: Optional[pulumi.Input[str]] = None,
             principal: Optional[pulumi.Input[str]] = None,
             qualified_sql_name: Optional[pulumi.Input[str]] = None,
             region: Optional[pulumi.Input[str]] = None,
             schema_name: Optional[pulumi.Input[str]] = None,
-            service_name: Optional[pulumi.Input[str]] = None) -> 'ConnectionAwsPrivatelink':
+            service_name: Optional[pulumi.Input[str]] = None,
+            validate: Optional[pulumi.Input[bool]] = None) -> 'ConnectionAwsPrivatelink':
         """
         Get an existing ConnectionAwsPrivatelink resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
@@ -487,14 +524,15 @@
         :param pulumi.Input[str] name: The identifier for the connection.
         :param pulumi.Input[str] ownership_role: The owernship role of the object.
         :param pulumi.Input[str] principal: The principal of the AWS PrivateLink service.
         :param pulumi.Input[str] qualified_sql_name: The fully qualified name of the connection.
         :param pulumi.Input[str] region: The region to use for the resource connection. If not set, the default region is used.
         :param pulumi.Input[str] schema_name: The identifier for the connection schema in Materialize. Defaults to `public`.
         :param pulumi.Input[str] service_name: The name of the AWS PrivateLink service.
+        :param pulumi.Input[bool] validate: **Private Preview** If the connection should wait for validation.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _ConnectionAwsPrivatelinkState.__new__(_ConnectionAwsPrivatelinkState)
 
         __props__.__dict__["availability_zones"] = availability_zones
         __props__.__dict__["comment"] = comment
@@ -502,14 +540,15 @@
         __props__.__dict__["name"] = name
         __props__.__dict__["ownership_role"] = ownership_role
         __props__.__dict__["principal"] = principal
         __props__.__dict__["qualified_sql_name"] = qualified_sql_name
         __props__.__dict__["region"] = region
         __props__.__dict__["schema_name"] = schema_name
         __props__.__dict__["service_name"] = service_name
+        __props__.__dict__["validate"] = validate
         return ConnectionAwsPrivatelink(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter(name="availabilityZones")
     def availability_zones(self) -> pulumi.Output[Sequence[str]]:
         """
         The availability zones of the AWS PrivateLink service.
@@ -584,7 +623,15 @@
     @pulumi.getter(name="serviceName")
     def service_name(self) -> pulumi.Output[str]:
         """
         The name of the AWS PrivateLink service.
         """
         return pulumi.get(self, "service_name")
 
+    @property
+    @pulumi.getter
+    def validate(self) -> pulumi.Output[Optional[bool]]:
+        """
+        **Private Preview** If the connection should wait for validation.
+        """
+        return pulumi.get(self, "validate")
+
```

### Comparing `pulumi_materialize-0.1.9/pulumi_materialize/connection_confluent_schema_registry.py` & `pulumi_materialize-0.2.0/pulumi_materialize/connection_confluent_schema_registry.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.1.9/pulumi_materialize/connection_kafka.py` & `pulumi_materialize-0.2.0/pulumi_materialize/connection_kafka.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.1.9/pulumi_materialize/connection_mysql.py` & `pulumi_materialize-0.2.0/pulumi_materialize/connection_mysql.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.1.9/pulumi_materialize/connection_postgres.py` & `pulumi_materialize-0.2.0/pulumi_materialize/connection_postgres.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.1.9/pulumi_materialize/connection_ssh_tunnel.py` & `pulumi_materialize-0.2.0/pulumi_materialize/connection_ssh_tunnel.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.1.9/pulumi_materialize/database.py` & `pulumi_materialize-0.2.0/pulumi_materialize/database.py`

 * *Files 16% similar despite different names*

```diff
@@ -164,21 +164,35 @@
                  name: Optional[pulumi.Input[str]] = None,
                  ownership_role: Optional[pulumi.Input[str]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         The highest level namespace hierarchy in Materialize.
 
+        **Note**: This resource will not automatically create a public schema.If needed, the public schema must be explicitly defined in your configuration using the `Schema` resource.
+
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_materialize as materialize
 
-        example_database = materialize.Database("exampleDatabase")
+        # Create a Materialize database without a public schema
+        example = materialize.Database("example")
+        # By default, Materialize creates a public schema in each database
+        # The Terraform provider on the other hand does not create a public schema by default
+        # Optionally you can create a public schema in the database using the materialize_schema resource
+        public = materialize.Schema("public", database_name=example.name)
+        # Grant USAGE to the PUBLIC pseudo-role for the public schema
+        # This matches the default behavior of Materialize
+        schema_grant_usage = materialize.GrantSchema("schemaGrantUsage",
+            role_name="PUBLIC",
+            privilege="USAGE",
+            database_name=example.name,
+            schema_name=public.name)
         ```
 
         ## Import
 
         Databases can be imported using the database id
 
         ```sh
@@ -199,21 +213,35 @@
     def __init__(__self__,
                  resource_name: str,
                  args: Optional[DatabaseArgs] = None,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         The highest level namespace hierarchy in Materialize.
 
+        **Note**: This resource will not automatically create a public schema.If needed, the public schema must be explicitly defined in your configuration using the `Schema` resource.
+
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_materialize as materialize
 
-        example_database = materialize.Database("exampleDatabase")
+        # Create a Materialize database without a public schema
+        example = materialize.Database("example")
+        # By default, Materialize creates a public schema in each database
+        # The Terraform provider on the other hand does not create a public schema by default
+        # Optionally you can create a public schema in the database using the materialize_schema resource
+        public = materialize.Schema("public", database_name=example.name)
+        # Grant USAGE to the PUBLIC pseudo-role for the public schema
+        # This matches the default behavior of Materialize
+        schema_grant_usage = materialize.GrantSchema("schemaGrantUsage",
+            role_name="PUBLIC",
+            privilege="USAGE",
+            database_name=example.name,
+            schema_name=public.name)
         ```
 
         ## Import
 
         Databases can be imported using the database id
 
         ```sh
```

### Comparing `pulumi_materialize-0.1.9/pulumi_materialize/get_cluster_replicas.py` & `pulumi_materialize-0.2.0/pulumi_materialize/get_cluster_replicas.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.1.9/pulumi_materialize/get_clusters.py` & `pulumi_materialize-0.2.0/pulumi_materialize/get_clusters.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.1.9/pulumi_materialize/get_connections.py` & `pulumi_materialize-0.2.0/pulumi_materialize/get_connections.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.1.9/pulumi_materialize/get_current_cluster.py` & `pulumi_materialize-0.2.0/pulumi_materialize/get_current_cluster.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.1.9/pulumi_materialize/get_current_database.py` & `pulumi_materialize-0.2.0/pulumi_materialize/get_current_database.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.1.9/pulumi_materialize/get_databases.py` & `pulumi_materialize-0.2.0/pulumi_materialize/get_databases.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.1.9/pulumi_materialize/get_egress_ips.py` & `pulumi_materialize-0.2.0/pulumi_materialize/get_egress_ips.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.1.9/pulumi_materialize/get_indexes.py` & `pulumi_materialize-0.2.0/pulumi_materialize/get_indexes.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.1.9/pulumi_materialize/get_materialized_views.py` & `pulumi_materialize-0.2.0/pulumi_materialize/get_materialized_views.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.1.9/pulumi_materialize/get_roles.py` & `pulumi_materialize-0.2.0/pulumi_materialize/get_roles.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.1.9/pulumi_materialize/get_schemas.py` & `pulumi_materialize-0.2.0/pulumi_materialize/get_schemas.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.1.9/pulumi_materialize/get_scim_configs.py` & `pulumi_materialize-0.2.0/pulumi_materialize/get_scim_configs.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.1.9/pulumi_materialize/get_scim_groups.py` & `pulumi_materialize-0.2.0/pulumi_materialize/get_scim_groups.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.1.9/pulumi_materialize/get_secrets.py` & `pulumi_materialize-0.2.0/pulumi_materialize/get_secrets.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.1.9/pulumi_materialize/get_sinks.py` & `pulumi_materialize-0.2.0/pulumi_materialize/get_sinks.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.1.9/pulumi_materialize/get_sources.py` & `pulumi_materialize-0.2.0/pulumi_materialize/get_sources.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.1.9/pulumi_materialize/get_sso_config.py` & `pulumi_materialize-0.2.0/pulumi_materialize/get_sso_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.1.9/pulumi_materialize/get_system_parameters.py` & `pulumi_materialize-0.2.0/pulumi_materialize/get_system_parameters.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.1.9/pulumi_materialize/get_tables.py` & `pulumi_materialize-0.2.0/pulumi_materialize/get_tables.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.1.9/pulumi_materialize/get_types.py` & `pulumi_materialize-0.2.0/pulumi_materialize/get_types.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.1.9/pulumi_materialize/get_views.py` & `pulumi_materialize-0.2.0/pulumi_materialize/get_views.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.1.9/pulumi_materialize/grant_cluster.py` & `pulumi_materialize-0.2.0/pulumi_materialize/grant_cluster.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.1.9/pulumi_materialize/grant_cluster_default_privilege.py` & `pulumi_materialize-0.2.0/pulumi_materialize/grant_cluster_default_privilege.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.1.9/pulumi_materialize/grant_connection.py` & `pulumi_materialize-0.2.0/pulumi_materialize/grant_connection.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.1.9/pulumi_materialize/grant_connection_default_privilege.py` & `pulumi_materialize-0.2.0/pulumi_materialize/grant_connection_default_privilege.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.1.9/pulumi_materialize/grant_database.py` & `pulumi_materialize-0.2.0/pulumi_materialize/grant_database.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.1.9/pulumi_materialize/grant_database_default_privilege.py` & `pulumi_materialize-0.2.0/pulumi_materialize/grant_database_default_privilege.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.1.9/pulumi_materialize/grant_materialized_view.py` & `pulumi_materialize-0.2.0/pulumi_materialize/grant_materialized_view.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.1.9/pulumi_materialize/grant_role.py` & `pulumi_materialize-0.2.0/pulumi_materialize/grant_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.1.9/pulumi_materialize/grant_schema.py` & `pulumi_materialize-0.2.0/pulumi_materialize/grant_schema.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.1.9/pulumi_materialize/grant_schema_default_privilege.py` & `pulumi_materialize-0.2.0/pulumi_materialize/grant_schema_default_privilege.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.1.9/pulumi_materialize/grant_secret.py` & `pulumi_materialize-0.2.0/pulumi_materialize/grant_secret.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.1.9/pulumi_materialize/grant_secret_default_privilege.py` & `pulumi_materialize-0.2.0/pulumi_materialize/grant_secret_default_privilege.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.1.9/pulumi_materialize/grant_source.py` & `pulumi_materialize-0.2.0/pulumi_materialize/grant_source.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.1.9/pulumi_materialize/grant_system_privilege.py` & `pulumi_materialize-0.2.0/pulumi_materialize/grant_system_privilege.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.1.9/pulumi_materialize/grant_table.py` & `pulumi_materialize-0.2.0/pulumi_materialize/grant_table.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.1.9/pulumi_materialize/grant_table_default_privilege.py` & `pulumi_materialize-0.2.0/pulumi_materialize/grant_table_default_privilege.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.1.9/pulumi_materialize/grant_type.py` & `pulumi_materialize-0.2.0/pulumi_materialize/grant_type.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.1.9/pulumi_materialize/grant_type_default_privilege.py` & `pulumi_materialize-0.2.0/pulumi_materialize/grant_type_default_privilege.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.1.9/pulumi_materialize/grant_view.py` & `pulumi_materialize-0.2.0/pulumi_materialize/grant_view.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.1.9/pulumi_materialize/index.py` & `pulumi_materialize-0.2.0/pulumi_materialize/index.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.1.9/pulumi_materialize/materialized_view.py` & `pulumi_materialize-0.2.0/pulumi_materialize/materialized_view.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.1.9/pulumi_materialize/outputs.py` & `pulumi_materialize-0.2.0/pulumi_materialize/outputs.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 from . import outputs
 
 __all__ = [
+    'ClusterScheduling',
+    'ClusterSchedulingOnRefresh',
     'ConnectionAwsAccessKeyId',
     'ConnectionAwsAccessKeyIdSecret',
     'ConnectionAwsSecretAccessKey',
     'ConnectionAwsSessionToken',
     'ConnectionAwsSessionTokenSecret',
     'ConnectionConfluentSchemaRegistryAwsPrivatelink',
     'ConnectionConfluentSchemaRegistryPassword',
@@ -116,14 +118,15 @@
     'SourceKafkaValueFormatAvroSchemaRegistryConnection',
     'SourceKafkaValueFormatCsv',
     'SourceKafkaValueFormatProtobuf',
     'SourceKafkaValueFormatProtobufSchemaRegistryConnection',
     'SourceLoadgenAuctionOptions',
     'SourceLoadgenCounterOptions',
     'SourceLoadgenExposeProgress',
+    'SourceLoadgenKeyValueOptions',
     'SourceLoadgenMarketingOptions',
     'SourceLoadgenSubsource',
     'SourceLoadgenTpchOptions',
     'SourceMysqlMysqlConnection',
     'SourceMysqlSubsource',
     'SourceMysqlTable',
     'SourcePostgresExposeProgress',
@@ -139,14 +142,88 @@
     'TableColumn',
     'TypeListProperties',
     'TypeMapProperties',
     'TypeRowProperty',
 ]
 
 @pulumi.output_type
+class ClusterScheduling(dict):
+    @staticmethod
+    def __key_warning(key: str):
+        suggest = None
+        if key == "onRefresh":
+            suggest = "on_refresh"
+
+        if suggest:
+            pulumi.log.warn(f"Key '{key}' not found in ClusterScheduling. Access the value via the '{suggest}' property getter instead.")
+
+    def __getitem__(self, key: str) -> Any:
+        ClusterScheduling.__key_warning(key)
+        return super().__getitem__(key)
+
+    def get(self, key: str, default = None) -> Any:
+        ClusterScheduling.__key_warning(key)
+        return super().get(key, default)
+
+    def __init__(__self__, *,
+                 on_refresh: Optional['outputs.ClusterSchedulingOnRefresh'] = None):
+        """
+        :param 'ClusterSchedulingOnRefreshArgs' on_refresh: Configuration for refreshing the cluster.
+        """
+        if on_refresh is not None:
+            pulumi.set(__self__, "on_refresh", on_refresh)
+
+    @property
+    @pulumi.getter(name="onRefresh")
+    def on_refresh(self) -> Optional['outputs.ClusterSchedulingOnRefresh']:
+        """
+        Configuration for refreshing the cluster.
+        """
+        return pulumi.get(self, "on_refresh")
+
+
+@pulumi.output_type
+class ClusterSchedulingOnRefresh(dict):
+    @staticmethod
+    def __key_warning(key: str):
+        suggest = None
+        if key == "rehydrationTimeEstimate":
+            suggest = "rehydration_time_estimate"
+
+        if suggest:
+            pulumi.log.warn(f"Key '{key}' not found in ClusterSchedulingOnRefresh. Access the value via the '{suggest}' property getter instead.")
+
+    def __getitem__(self, key: str) -> Any:
+        ClusterSchedulingOnRefresh.__key_warning(key)
+        return super().__getitem__(key)
+
+    def get(self, key: str, default = None) -> Any:
+        ClusterSchedulingOnRefresh.__key_warning(key)
+        return super().get(key, default)
+
+    def __init__(__self__, *,
+                 enabled: Optional[bool] = None,
+                 rehydration_time_estimate: Optional[str] = None):
+        if enabled is not None:
+            pulumi.set(__self__, "enabled", enabled)
+        if rehydration_time_estimate is not None:
+            pulumi.set(__self__, "rehydration_time_estimate", rehydration_time_estimate)
+
+    @property
+    @pulumi.getter
+    def enabled(self) -> Optional[bool]:
+        return pulumi.get(self, "enabled")
+
+    @property
+    @pulumi.getter(name="rehydrationTimeEstimate")
+    def rehydration_time_estimate(self) -> Optional[str]:
+        return pulumi.get(self, "rehydration_time_estimate")
+
+
+@pulumi.output_type
 class ConnectionAwsAccessKeyId(dict):
     def __init__(__self__, *,
                  secret: Optional['outputs.ConnectionAwsAccessKeyIdSecret'] = None,
                  text: Optional[str] = None):
         """
         :param 'ConnectionAwsAccessKeyIdSecretArgs' secret: The `access_key_id` secret value. Conflicts with `text` within this block.
         :param str text: The `access_key_id` text value. Conflicts with `secret` within this block
@@ -5856,14 +5933,141 @@
         """
         The expose_progress schema name. Defaults to `public`.
         """
         return pulumi.get(self, "schema_name")
 
 
 @pulumi.output_type
+class SourceLoadgenKeyValueOptions(dict):
+    @staticmethod
+    def __key_warning(key: str):
+        suggest = None
+        if key == "batchSize":
+            suggest = "batch_size"
+        elif key == "snapshotRounds":
+            suggest = "snapshot_rounds"
+        elif key == "tickInterval":
+            suggest = "tick_interval"
+        elif key == "transactionalSnapshot":
+            suggest = "transactional_snapshot"
+        elif key == "valueSize":
+            suggest = "value_size"
+
+        if suggest:
+            pulumi.log.warn(f"Key '{key}' not found in SourceLoadgenKeyValueOptions. Access the value via the '{suggest}' property getter instead.")
+
+    def __getitem__(self, key: str) -> Any:
+        SourceLoadgenKeyValueOptions.__key_warning(key)
+        return super().__getitem__(key)
+
+    def get(self, key: str, default = None) -> Any:
+        SourceLoadgenKeyValueOptions.__key_warning(key)
+        return super().get(key, default)
+
+    def __init__(__self__, *,
+                 keys: int,
+                 batch_size: Optional[int] = None,
+                 partitions: Optional[int] = None,
+                 seed: Optional[int] = None,
+                 snapshot_rounds: Optional[int] = None,
+                 tick_interval: Optional[str] = None,
+                 transactional_snapshot: Optional[bool] = None,
+                 value_size: Optional[int] = None):
+        """
+        :param int keys: The number of keys in the source. This must be divisible by the product of 'partitions' and 'batch_size'.
+        :param int batch_size: The number of keys per partition to produce in each update.
+        :param int partitions: The number of partitions to spread the keys across.
+        :param int seed: A per-source seed for seeding the random data.
+        :param int snapshot_rounds: The number of rounds of data to produce as the source starts up.
+        :param str tick_interval: The interval at which the next datum should be emitted. Defaults to one second.
+        :param bool transactional_snapshot: Whether to emit the snapshot as a singular transaction.
+        :param int value_size: The number of bytes in each value.
+        """
+        pulumi.set(__self__, "keys", keys)
+        if batch_size is not None:
+            pulumi.set(__self__, "batch_size", batch_size)
+        if partitions is not None:
+            pulumi.set(__self__, "partitions", partitions)
+        if seed is not None:
+            pulumi.set(__self__, "seed", seed)
+        if snapshot_rounds is not None:
+            pulumi.set(__self__, "snapshot_rounds", snapshot_rounds)
+        if tick_interval is not None:
+            pulumi.set(__self__, "tick_interval", tick_interval)
+        if transactional_snapshot is not None:
+            pulumi.set(__self__, "transactional_snapshot", transactional_snapshot)
+        if value_size is not None:
+            pulumi.set(__self__, "value_size", value_size)
+
+    @property
+    @pulumi.getter
+    def keys(self) -> int:
+        """
+        The number of keys in the source. This must be divisible by the product of 'partitions' and 'batch_size'.
+        """
+        return pulumi.get(self, "keys")
+
+    @property
+    @pulumi.getter(name="batchSize")
+    def batch_size(self) -> Optional[int]:
+        """
+        The number of keys per partition to produce in each update.
+        """
+        return pulumi.get(self, "batch_size")
+
+    @property
+    @pulumi.getter
+    def partitions(self) -> Optional[int]:
+        """
+        The number of partitions to spread the keys across.
+        """
+        return pulumi.get(self, "partitions")
+
+    @property
+    @pulumi.getter
+    def seed(self) -> Optional[int]:
+        """
+        A per-source seed for seeding the random data.
+        """
+        return pulumi.get(self, "seed")
+
+    @property
+    @pulumi.getter(name="snapshotRounds")
+    def snapshot_rounds(self) -> Optional[int]:
+        """
+        The number of rounds of data to produce as the source starts up.
+        """
+        return pulumi.get(self, "snapshot_rounds")
+
+    @property
+    @pulumi.getter(name="tickInterval")
+    def tick_interval(self) -> Optional[str]:
+        """
+        The interval at which the next datum should be emitted. Defaults to one second.
+        """
+        return pulumi.get(self, "tick_interval")
+
+    @property
+    @pulumi.getter(name="transactionalSnapshot")
+    def transactional_snapshot(self) -> Optional[bool]:
+        """
+        Whether to emit the snapshot as a singular transaction.
+        """
+        return pulumi.get(self, "transactional_snapshot")
+
+    @property
+    @pulumi.getter(name="valueSize")
+    def value_size(self) -> Optional[int]:
+        """
+        The number of bytes in each value.
+        """
+        return pulumi.get(self, "value_size")
+
+
+@pulumi.output_type
 class SourceLoadgenMarketingOptions(dict):
     @staticmethod
     def __key_warning(key: str):
         suggest = None
         if key == "scaleFactor":
             suggest = "scale_factor"
         elif key == "tickInterval":
```

### Comparing `pulumi_materialize-0.1.9/pulumi_materialize/provider.py` & `pulumi_materialize-0.2.0/pulumi_materialize/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.1.9/pulumi_materialize/region.py` & `pulumi_materialize-0.2.0/pulumi_materialize/region.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.1.9/pulumi_materialize/role.py` & `pulumi_materialize-0.2.0/pulumi_materialize/role.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.1.9/pulumi_materialize/role_parameter.py` & `pulumi_materialize-0.2.0/pulumi_materialize/role_parameter.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.1.9/pulumi_materialize/schema.py` & `pulumi_materialize-0.2.0/pulumi_materialize/schema.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.1.9/pulumi_materialize/scim2_configuration.py` & `pulumi_materialize-0.2.0/pulumi_materialize/scim2_configuration.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.1.9/pulumi_materialize/secret.py` & `pulumi_materialize-0.2.0/pulumi_materialize/secret.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.1.9/pulumi_materialize/sink_kafka.py` & `pulumi_materialize-0.2.0/pulumi_materialize/sink_kafka.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.1.9/pulumi_materialize/source_kafka.py` & `pulumi_materialize-0.2.0/pulumi_materialize/source_kafka.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.1.9/pulumi_materialize/source_loadgen.py` & `pulumi_materialize-0.2.0/pulumi_materialize/source_loadgen.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,29 +19,31 @@
                  load_generator_type: pulumi.Input[str],
                  auction_options: Optional[pulumi.Input['SourceLoadgenAuctionOptionsArgs']] = None,
                  cluster_name: Optional[pulumi.Input[str]] = None,
                  comment: Optional[pulumi.Input[str]] = None,
                  counter_options: Optional[pulumi.Input['SourceLoadgenCounterOptionsArgs']] = None,
                  database_name: Optional[pulumi.Input[str]] = None,
                  expose_progress: Optional[pulumi.Input['SourceLoadgenExposeProgressArgs']] = None,
+                 key_value_options: Optional[pulumi.Input['SourceLoadgenKeyValueOptionsArgs']] = None,
                  marketing_options: Optional[pulumi.Input['SourceLoadgenMarketingOptionsArgs']] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  ownership_role: Optional[pulumi.Input[str]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  schema_name: Optional[pulumi.Input[str]] = None,
                  tpch_options: Optional[pulumi.Input['SourceLoadgenTpchOptionsArgs']] = None):
         """
         The set of arguments for constructing a SourceLoadgen resource.
-        :param pulumi.Input[str] load_generator_type: The load generator types: [AUCTION MARKETING COUNTER TPCH].
+        :param pulumi.Input[str] load_generator_type: The load generator types: [AUCTION MARKETING COUNTER TPCH KEY VALUE].
         :param pulumi.Input['SourceLoadgenAuctionOptionsArgs'] auction_options: Auction Options.
         :param pulumi.Input[str] cluster_name: The cluster to maintain this source.
         :param pulumi.Input[str] comment: **Public Preview** Comment on an object in the database.
         :param pulumi.Input['SourceLoadgenCounterOptionsArgs'] counter_options: Counter Options.
         :param pulumi.Input[str] database_name: The identifier for the source database in Materialize. Defaults to `MZ_DATABASE` environment variable if set or `materialize` if environment variable is not set.
         :param pulumi.Input['SourceLoadgenExposeProgressArgs'] expose_progress: The name of the progress subsource for the source. If this is not specified, the subsource will be named `<src_name>_progress`.
+        :param pulumi.Input['SourceLoadgenKeyValueOptionsArgs'] key_value_options: KEY VALUE Load Generator Options.
         :param pulumi.Input['SourceLoadgenMarketingOptionsArgs'] marketing_options: Marketing Options.
         :param pulumi.Input[str] name: The identifier for the source.
         :param pulumi.Input[str] ownership_role: The owernship role of the object.
         :param pulumi.Input[str] region: The region to use for the resource connection. If not set, the default region is used.
         :param pulumi.Input[str] schema_name: The identifier for the source schema in Materialize. Defaults to `public`.
         :param pulumi.Input['SourceLoadgenTpchOptionsArgs'] tpch_options: TPCH Options.
         """
@@ -54,14 +56,16 @@
             pulumi.set(__self__, "comment", comment)
         if counter_options is not None:
             pulumi.set(__self__, "counter_options", counter_options)
         if database_name is not None:
             pulumi.set(__self__, "database_name", database_name)
         if expose_progress is not None:
             pulumi.set(__self__, "expose_progress", expose_progress)
+        if key_value_options is not None:
+            pulumi.set(__self__, "key_value_options", key_value_options)
         if marketing_options is not None:
             pulumi.set(__self__, "marketing_options", marketing_options)
         if name is not None:
             pulumi.set(__self__, "name", name)
         if ownership_role is not None:
             pulumi.set(__self__, "ownership_role", ownership_role)
         if region is not None:
@@ -71,15 +75,15 @@
         if tpch_options is not None:
             pulumi.set(__self__, "tpch_options", tpch_options)
 
     @property
     @pulumi.getter(name="loadGeneratorType")
     def load_generator_type(self) -> pulumi.Input[str]:
         """
-        The load generator types: [AUCTION MARKETING COUNTER TPCH].
+        The load generator types: [AUCTION MARKETING COUNTER TPCH KEY VALUE].
         """
         return pulumi.get(self, "load_generator_type")
 
     @load_generator_type.setter
     def load_generator_type(self, value: pulumi.Input[str]):
         pulumi.set(self, "load_generator_type", value)
 
@@ -152,14 +156,26 @@
         return pulumi.get(self, "expose_progress")
 
     @expose_progress.setter
     def expose_progress(self, value: Optional[pulumi.Input['SourceLoadgenExposeProgressArgs']]):
         pulumi.set(self, "expose_progress", value)
 
     @property
+    @pulumi.getter(name="keyValueOptions")
+    def key_value_options(self) -> Optional[pulumi.Input['SourceLoadgenKeyValueOptionsArgs']]:
+        """
+        KEY VALUE Load Generator Options.
+        """
+        return pulumi.get(self, "key_value_options")
+
+    @key_value_options.setter
+    def key_value_options(self, value: Optional[pulumi.Input['SourceLoadgenKeyValueOptionsArgs']]):
+        pulumi.set(self, "key_value_options", value)
+
+    @property
     @pulumi.getter(name="marketingOptions")
     def marketing_options(self) -> Optional[pulumi.Input['SourceLoadgenMarketingOptionsArgs']]:
         """
         Marketing Options.
         """
         return pulumi.get(self, "marketing_options")
 
@@ -233,14 +249,15 @@
     def __init__(__self__, *,
                  auction_options: Optional[pulumi.Input['SourceLoadgenAuctionOptionsArgs']] = None,
                  cluster_name: Optional[pulumi.Input[str]] = None,
                  comment: Optional[pulumi.Input[str]] = None,
                  counter_options: Optional[pulumi.Input['SourceLoadgenCounterOptionsArgs']] = None,
                  database_name: Optional[pulumi.Input[str]] = None,
                  expose_progress: Optional[pulumi.Input['SourceLoadgenExposeProgressArgs']] = None,
+                 key_value_options: Optional[pulumi.Input['SourceLoadgenKeyValueOptionsArgs']] = None,
                  load_generator_type: Optional[pulumi.Input[str]] = None,
                  marketing_options: Optional[pulumi.Input['SourceLoadgenMarketingOptionsArgs']] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  ownership_role: Optional[pulumi.Input[str]] = None,
                  qualified_sql_name: Optional[pulumi.Input[str]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  schema_name: Optional[pulumi.Input[str]] = None,
@@ -251,15 +268,16 @@
         Input properties used for looking up and filtering SourceLoadgen resources.
         :param pulumi.Input['SourceLoadgenAuctionOptionsArgs'] auction_options: Auction Options.
         :param pulumi.Input[str] cluster_name: The cluster to maintain this source.
         :param pulumi.Input[str] comment: **Public Preview** Comment on an object in the database.
         :param pulumi.Input['SourceLoadgenCounterOptionsArgs'] counter_options: Counter Options.
         :param pulumi.Input[str] database_name: The identifier for the source database in Materialize. Defaults to `MZ_DATABASE` environment variable if set or `materialize` if environment variable is not set.
         :param pulumi.Input['SourceLoadgenExposeProgressArgs'] expose_progress: The name of the progress subsource for the source. If this is not specified, the subsource will be named `<src_name>_progress`.
-        :param pulumi.Input[str] load_generator_type: The load generator types: [AUCTION MARKETING COUNTER TPCH].
+        :param pulumi.Input['SourceLoadgenKeyValueOptionsArgs'] key_value_options: KEY VALUE Load Generator Options.
+        :param pulumi.Input[str] load_generator_type: The load generator types: [AUCTION MARKETING COUNTER TPCH KEY VALUE].
         :param pulumi.Input['SourceLoadgenMarketingOptionsArgs'] marketing_options: Marketing Options.
         :param pulumi.Input[str] name: The identifier for the source.
         :param pulumi.Input[str] ownership_role: The owernship role of the object.
         :param pulumi.Input[str] qualified_sql_name: The fully qualified name of the source.
         :param pulumi.Input[str] region: The region to use for the resource connection. If not set, the default region is used.
         :param pulumi.Input[str] schema_name: The identifier for the source schema in Materialize. Defaults to `public`.
         :param pulumi.Input[str] size: The size of the cluster maintaining this source.
@@ -274,14 +292,16 @@
             pulumi.set(__self__, "comment", comment)
         if counter_options is not None:
             pulumi.set(__self__, "counter_options", counter_options)
         if database_name is not None:
             pulumi.set(__self__, "database_name", database_name)
         if expose_progress is not None:
             pulumi.set(__self__, "expose_progress", expose_progress)
+        if key_value_options is not None:
+            pulumi.set(__self__, "key_value_options", key_value_options)
         if load_generator_type is not None:
             pulumi.set(__self__, "load_generator_type", load_generator_type)
         if marketing_options is not None:
             pulumi.set(__self__, "marketing_options", marketing_options)
         if name is not None:
             pulumi.set(__self__, "name", name)
         if ownership_role is not None:
@@ -368,18 +388,30 @@
         return pulumi.get(self, "expose_progress")
 
     @expose_progress.setter
     def expose_progress(self, value: Optional[pulumi.Input['SourceLoadgenExposeProgressArgs']]):
         pulumi.set(self, "expose_progress", value)
 
     @property
+    @pulumi.getter(name="keyValueOptions")
+    def key_value_options(self) -> Optional[pulumi.Input['SourceLoadgenKeyValueOptionsArgs']]:
+        """
+        KEY VALUE Load Generator Options.
+        """
+        return pulumi.get(self, "key_value_options")
+
+    @key_value_options.setter
+    def key_value_options(self, value: Optional[pulumi.Input['SourceLoadgenKeyValueOptionsArgs']]):
+        pulumi.set(self, "key_value_options", value)
+
+    @property
     @pulumi.getter(name="loadGeneratorType")
     def load_generator_type(self) -> Optional[pulumi.Input[str]]:
         """
-        The load generator types: [AUCTION MARKETING COUNTER TPCH].
+        The load generator types: [AUCTION MARKETING COUNTER TPCH KEY VALUE].
         """
         return pulumi.get(self, "load_generator_type")
 
     @load_generator_type.setter
     def load_generator_type(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "load_generator_type", value)
 
@@ -499,14 +531,15 @@
                  opts: Optional[pulumi.ResourceOptions] = None,
                  auction_options: Optional[pulumi.Input[pulumi.InputType['SourceLoadgenAuctionOptionsArgs']]] = None,
                  cluster_name: Optional[pulumi.Input[str]] = None,
                  comment: Optional[pulumi.Input[str]] = None,
                  counter_options: Optional[pulumi.Input[pulumi.InputType['SourceLoadgenCounterOptionsArgs']]] = None,
                  database_name: Optional[pulumi.Input[str]] = None,
                  expose_progress: Optional[pulumi.Input[pulumi.InputType['SourceLoadgenExposeProgressArgs']]] = None,
+                 key_value_options: Optional[pulumi.Input[pulumi.InputType['SourceLoadgenKeyValueOptionsArgs']]] = None,
                  load_generator_type: Optional[pulumi.Input[str]] = None,
                  marketing_options: Optional[pulumi.Input[pulumi.InputType['SourceLoadgenMarketingOptionsArgs']]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  ownership_role: Optional[pulumi.Input[str]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  schema_name: Optional[pulumi.Input[str]] = None,
                  tpch_options: Optional[pulumi.Input[pulumi.InputType['SourceLoadgenTpchOptionsArgs']]] = None,
@@ -543,15 +576,16 @@
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[pulumi.InputType['SourceLoadgenAuctionOptionsArgs']] auction_options: Auction Options.
         :param pulumi.Input[str] cluster_name: The cluster to maintain this source.
         :param pulumi.Input[str] comment: **Public Preview** Comment on an object in the database.
         :param pulumi.Input[pulumi.InputType['SourceLoadgenCounterOptionsArgs']] counter_options: Counter Options.
         :param pulumi.Input[str] database_name: The identifier for the source database in Materialize. Defaults to `MZ_DATABASE` environment variable if set or `materialize` if environment variable is not set.
         :param pulumi.Input[pulumi.InputType['SourceLoadgenExposeProgressArgs']] expose_progress: The name of the progress subsource for the source. If this is not specified, the subsource will be named `<src_name>_progress`.
-        :param pulumi.Input[str] load_generator_type: The load generator types: [AUCTION MARKETING COUNTER TPCH].
+        :param pulumi.Input[pulumi.InputType['SourceLoadgenKeyValueOptionsArgs']] key_value_options: KEY VALUE Load Generator Options.
+        :param pulumi.Input[str] load_generator_type: The load generator types: [AUCTION MARKETING COUNTER TPCH KEY VALUE].
         :param pulumi.Input[pulumi.InputType['SourceLoadgenMarketingOptionsArgs']] marketing_options: Marketing Options.
         :param pulumi.Input[str] name: The identifier for the source.
         :param pulumi.Input[str] ownership_role: The owernship role of the object.
         :param pulumi.Input[str] region: The region to use for the resource connection. If not set, the default region is used.
         :param pulumi.Input[str] schema_name: The identifier for the source schema in Materialize. Defaults to `public`.
         :param pulumi.Input[pulumi.InputType['SourceLoadgenTpchOptionsArgs']] tpch_options: TPCH Options.
         """
@@ -606,14 +640,15 @@
                  opts: Optional[pulumi.ResourceOptions] = None,
                  auction_options: Optional[pulumi.Input[pulumi.InputType['SourceLoadgenAuctionOptionsArgs']]] = None,
                  cluster_name: Optional[pulumi.Input[str]] = None,
                  comment: Optional[pulumi.Input[str]] = None,
                  counter_options: Optional[pulumi.Input[pulumi.InputType['SourceLoadgenCounterOptionsArgs']]] = None,
                  database_name: Optional[pulumi.Input[str]] = None,
                  expose_progress: Optional[pulumi.Input[pulumi.InputType['SourceLoadgenExposeProgressArgs']]] = None,
+                 key_value_options: Optional[pulumi.Input[pulumi.InputType['SourceLoadgenKeyValueOptionsArgs']]] = None,
                  load_generator_type: Optional[pulumi.Input[str]] = None,
                  marketing_options: Optional[pulumi.Input[pulumi.InputType['SourceLoadgenMarketingOptionsArgs']]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  ownership_role: Optional[pulumi.Input[str]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  schema_name: Optional[pulumi.Input[str]] = None,
                  tpch_options: Optional[pulumi.Input[pulumi.InputType['SourceLoadgenTpchOptionsArgs']]] = None,
@@ -628,14 +663,15 @@
 
             __props__.__dict__["auction_options"] = auction_options
             __props__.__dict__["cluster_name"] = cluster_name
             __props__.__dict__["comment"] = comment
             __props__.__dict__["counter_options"] = counter_options
             __props__.__dict__["database_name"] = database_name
             __props__.__dict__["expose_progress"] = expose_progress
+            __props__.__dict__["key_value_options"] = key_value_options
             if load_generator_type is None and not opts.urn:
                 raise TypeError("Missing required property 'load_generator_type'")
             __props__.__dict__["load_generator_type"] = load_generator_type
             __props__.__dict__["marketing_options"] = marketing_options
             __props__.__dict__["name"] = name
             __props__.__dict__["ownership_role"] = ownership_role
             __props__.__dict__["region"] = region
@@ -656,14 +692,15 @@
             opts: Optional[pulumi.ResourceOptions] = None,
             auction_options: Optional[pulumi.Input[pulumi.InputType['SourceLoadgenAuctionOptionsArgs']]] = None,
             cluster_name: Optional[pulumi.Input[str]] = None,
             comment: Optional[pulumi.Input[str]] = None,
             counter_options: Optional[pulumi.Input[pulumi.InputType['SourceLoadgenCounterOptionsArgs']]] = None,
             database_name: Optional[pulumi.Input[str]] = None,
             expose_progress: Optional[pulumi.Input[pulumi.InputType['SourceLoadgenExposeProgressArgs']]] = None,
+            key_value_options: Optional[pulumi.Input[pulumi.InputType['SourceLoadgenKeyValueOptionsArgs']]] = None,
             load_generator_type: Optional[pulumi.Input[str]] = None,
             marketing_options: Optional[pulumi.Input[pulumi.InputType['SourceLoadgenMarketingOptionsArgs']]] = None,
             name: Optional[pulumi.Input[str]] = None,
             ownership_role: Optional[pulumi.Input[str]] = None,
             qualified_sql_name: Optional[pulumi.Input[str]] = None,
             region: Optional[pulumi.Input[str]] = None,
             schema_name: Optional[pulumi.Input[str]] = None,
@@ -679,15 +716,16 @@
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[pulumi.InputType['SourceLoadgenAuctionOptionsArgs']] auction_options: Auction Options.
         :param pulumi.Input[str] cluster_name: The cluster to maintain this source.
         :param pulumi.Input[str] comment: **Public Preview** Comment on an object in the database.
         :param pulumi.Input[pulumi.InputType['SourceLoadgenCounterOptionsArgs']] counter_options: Counter Options.
         :param pulumi.Input[str] database_name: The identifier for the source database in Materialize. Defaults to `MZ_DATABASE` environment variable if set or `materialize` if environment variable is not set.
         :param pulumi.Input[pulumi.InputType['SourceLoadgenExposeProgressArgs']] expose_progress: The name of the progress subsource for the source. If this is not specified, the subsource will be named `<src_name>_progress`.
-        :param pulumi.Input[str] load_generator_type: The load generator types: [AUCTION MARKETING COUNTER TPCH].
+        :param pulumi.Input[pulumi.InputType['SourceLoadgenKeyValueOptionsArgs']] key_value_options: KEY VALUE Load Generator Options.
+        :param pulumi.Input[str] load_generator_type: The load generator types: [AUCTION MARKETING COUNTER TPCH KEY VALUE].
         :param pulumi.Input[pulumi.InputType['SourceLoadgenMarketingOptionsArgs']] marketing_options: Marketing Options.
         :param pulumi.Input[str] name: The identifier for the source.
         :param pulumi.Input[str] ownership_role: The owernship role of the object.
         :param pulumi.Input[str] qualified_sql_name: The fully qualified name of the source.
         :param pulumi.Input[str] region: The region to use for the resource connection. If not set, the default region is used.
         :param pulumi.Input[str] schema_name: The identifier for the source schema in Materialize. Defaults to `public`.
         :param pulumi.Input[str] size: The size of the cluster maintaining this source.
@@ -700,14 +738,15 @@
 
         __props__.__dict__["auction_options"] = auction_options
         __props__.__dict__["cluster_name"] = cluster_name
         __props__.__dict__["comment"] = comment
         __props__.__dict__["counter_options"] = counter_options
         __props__.__dict__["database_name"] = database_name
         __props__.__dict__["expose_progress"] = expose_progress
+        __props__.__dict__["key_value_options"] = key_value_options
         __props__.__dict__["load_generator_type"] = load_generator_type
         __props__.__dict__["marketing_options"] = marketing_options
         __props__.__dict__["name"] = name
         __props__.__dict__["ownership_role"] = ownership_role
         __props__.__dict__["qualified_sql_name"] = qualified_sql_name
         __props__.__dict__["region"] = region
         __props__.__dict__["schema_name"] = schema_name
@@ -761,18 +800,26 @@
     def expose_progress(self) -> pulumi.Output[Optional['outputs.SourceLoadgenExposeProgress']]:
         """
         The name of the progress subsource for the source. If this is not specified, the subsource will be named `<src_name>_progress`.
         """
         return pulumi.get(self, "expose_progress")
 
     @property
+    @pulumi.getter(name="keyValueOptions")
+    def key_value_options(self) -> pulumi.Output[Optional['outputs.SourceLoadgenKeyValueOptions']]:
+        """
+        KEY VALUE Load Generator Options.
+        """
+        return pulumi.get(self, "key_value_options")
+
+    @property
     @pulumi.getter(name="loadGeneratorType")
     def load_generator_type(self) -> pulumi.Output[str]:
         """
-        The load generator types: [AUCTION MARKETING COUNTER TPCH].
+        The load generator types: [AUCTION MARKETING COUNTER TPCH KEY VALUE].
         """
         return pulumi.get(self, "load_generator_type")
 
     @property
     @pulumi.getter(name="marketingOptions")
     def marketing_options(self) -> pulumi.Output[Optional['outputs.SourceLoadgenMarketingOptions']]:
         """
```

### Comparing `pulumi_materialize-0.1.9/pulumi_materialize/source_mysql.py` & `pulumi_materialize-0.2.0/pulumi_materialize/source_mysql.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.1.9/pulumi_materialize/source_postgres.py` & `pulumi_materialize-0.2.0/pulumi_materialize/source_postgres.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.1.9/pulumi_materialize/source_webhook.py` & `pulumi_materialize-0.2.0/pulumi_materialize/source_webhook.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.1.9/pulumi_materialize/sso_config.py` & `pulumi_materialize-0.2.0/pulumi_materialize/sso_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.1.9/pulumi_materialize/sso_default_roles.py` & `pulumi_materialize-0.2.0/pulumi_materialize/sso_default_roles.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.1.9/pulumi_materialize/sso_domain.py` & `pulumi_materialize-0.2.0/pulumi_materialize/sso_domain.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.1.9/pulumi_materialize/sso_role_group_mapping.py` & `pulumi_materialize-0.2.0/pulumi_materialize/sso_role_group_mapping.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.1.9/pulumi_materialize/system_parameter.py` & `pulumi_materialize-0.2.0/pulumi_materialize/system_parameter.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.1.9/pulumi_materialize/table.py` & `pulumi_materialize-0.2.0/pulumi_materialize/table.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.1.9/pulumi_materialize/type.py` & `pulumi_materialize-0.2.0/pulumi_materialize/type.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.1.9/pulumi_materialize/user.py` & `pulumi_materialize-0.2.0/pulumi_materialize/user.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.1.9/pulumi_materialize/view.py` & `pulumi_materialize-0.2.0/pulumi_materialize/view.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.1.9/pulumi_materialize.egg-info/PKG-INFO` & `pulumi_materialize-0.2.0/pulumi_materialize.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-materialize
-Version: 0.1.9
+Version: 0.2.0
 Summary: A Pulumi package for creating and managing materialize cloud resources.
 Home-page: https://github.com/MaterializeInc/terraform-provider-materialize
 License: Apache-2.0
 Project-URL: Repository, https://github.com/MaterializeInc/terraform-provider-materialize
 Keywords: pulumi materialize category/cloud
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_materialize-0.1.9/pulumi_materialize.egg-info/SOURCES.txt` & `pulumi_materialize-0.2.0/pulumi_materialize.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 README.md
 setup.py
 pulumi_materialize/__init__.py
 pulumi_materialize/_inputs.py
 pulumi_materialize/_utilities.py
 pulumi_materialize/app_password.py
+pulumi_materialize/cloud_region.py
 pulumi_materialize/cluster.py
 pulumi_materialize/cluster_replica.py
 pulumi_materialize/connection_aws.py
 pulumi_materialize/connection_aws_privatelink.py
 pulumi_materialize/connection_confluent_schema_registry.py
 pulumi_materialize/connection_kafka.py
 pulumi_materialize/connection_mysql.py
@@ -61,14 +62,17 @@
 pulumi_materialize/pulumi-plugin.json
 pulumi_materialize/py.typed
 pulumi_materialize/region.py
 pulumi_materialize/role.py
 pulumi_materialize/role_parameter.py
 pulumi_materialize/schema.py
 pulumi_materialize/scim2_configuration.py
+pulumi_materialize/scim2_group.py
+pulumi_materialize/scim2_group_roles.py
+pulumi_materialize/scim2_group_users.py
 pulumi_materialize/secret.py
 pulumi_materialize/sink_kafka.py
 pulumi_materialize/source_kafka.py
 pulumi_materialize/source_loadgen.py
 pulumi_materialize/source_mysql.py
 pulumi_materialize/source_postgres.py
 pulumi_materialize/source_webhook.py
```

### Comparing `pulumi_materialize-0.1.9/setup.py` & `pulumi_materialize-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "0.1.9"
+VERSION = "0.2.0"
 def readme():
     try:
         with open('README.md', encoding='utf-8') as f:
             return f.read()
     except FileNotFoundError:
         return "materialize Pulumi Package - Development Version"
```


# Comparing `tmp/dbt-fabric-1.8.2.tar.gz` & `tmp/dbt-fabric-1.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-fabric-1.8.2.tar", last modified: Mon Apr 15 18:44:23 2024, max compression
+gzip compressed data, was "dbt-fabric-1.8.3.tar", last modified: Thu Apr 25 00:47:46 2024, max compression
```

## Comparing `dbt-fabric-1.8.2.tar` & `dbt-fabric-1.8.3.tar`

### file list

```diff
@@ -1,74 +1,81 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 18:44:23.556761 dbt-fabric-1.8.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-15 18:43:43.000000 dbt-fabric-1.8.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-15 18:43:43.000000 dbt-fabric-1.8.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3680 2024-04-15 18:44:23.556761 dbt-fabric-1.8.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2549 2024-04-15 18:43:43.000000 dbt-fabric-1.8.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 18:44:23.544761 dbt-fabric-1.8.2/dbt/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 18:44:23.544761 dbt-fabric-1.8.2/dbt/adapters/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 18:44:23.548761 dbt-fabric-1.8.2/dbt/adapters/fabric/
--rw-r--r--   0 runner    (1001) docker     (127)      682 2024-04-15 18:43:43.000000 dbt-fabric-1.8.2/dbt/adapters/fabric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-15 18:43:43.000000 dbt-fabric-1.8.2/dbt/adapters/fabric/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10093 2024-04-15 18:43:43.000000 dbt-fabric-1.8.2/dbt/adapters/fabric/fabric_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-15 18:43:43.000000 dbt-fabric-1.8.2/dbt/adapters/fabric/fabric_column.py
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-15 18:43:43.000000 dbt-fabric-1.8.2/dbt/adapters/fabric/fabric_configs.py
--rw-r--r--   0 runner    (1001) docker     (127)    16541 2024-04-15 18:43:43.000000 dbt-fabric-1.8.2/dbt/adapters/fabric/fabric_connection_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     2016 2024-04-15 18:43:43.000000 dbt-fabric-1.8.2/dbt/adapters/fabric/fabric_credentials.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 18:44:23.544761 dbt-fabric-1.8.2/dbt/include/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 18:44:23.548761 dbt-fabric-1.8.2/dbt/include/fabric/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-15 18:43:43.000000 dbt-fabric-1.8.2/dbt/include/fabric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-15 18:43:43.000000 dbt-fabric-1.8.2/dbt/include/fabric/dbt_project.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 18:44:23.544761 dbt-fabric-1.8.2/dbt/include/fabric/macros/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 18:44:23.548761 dbt-fabric-1.8.2/dbt/include/fabric/macros/adapters/
--rw-r--r--   0 runner    (1001) docker     (127)     3443 2024-04-15 18:43:43.000000 dbt-fabric-1.8.2/dbt/include/fabric/macros/adapters/apply_grants.sql
--rw-r--r--   0 runner    (1001) docker     (127)     7332 2024-04-15 18:43:43.000000 dbt-fabric-1.8.2/dbt/include/fabric/macros/adapters/catalog.sql
--rw-r--r--   0 runner    (1001) docker     (127)     4775 2024-04-15 18:43:43.000000 dbt-fabric-1.8.2/dbt/include/fabric/macros/adapters/columns.sql
--rw-r--r--   0 runner    (1001) docker     (127)     3763 2024-04-15 18:43:43.000000 dbt-fabric-1.8.2/dbt/include/fabric/macros/adapters/indexes.sql
--rw-r--r--   0 runner    (1001) docker     (127)     3328 2024-04-15 18:43:43.000000 dbt-fabric-1.8.2/dbt/include/fabric/macros/adapters/metadata.sql
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-15 18:43:43.000000 dbt-fabric-1.8.2/dbt/include/fabric/macros/adapters/persist_docs.sql
--rw-r--r--   0 runner    (1001) docker     (127)     4447 2024-04-15 18:43:43.000000 dbt-fabric-1.8.2/dbt/include/fabric/macros/adapters/relation.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-04-15 18:43:43.000000 dbt-fabric-1.8.2/dbt/include/fabric/macros/adapters/schema.sql
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-15 18:43:43.000000 dbt-fabric-1.8.2/dbt/include/fabric/macros/adapters/show.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 18:44:23.544761 dbt-fabric-1.8.2/dbt/include/fabric/macros/materializations/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 18:44:23.544761 dbt-fabric-1.8.2/dbt/include/fabric/macros/materializations/models/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 18:44:23.548761 dbt-fabric-1.8.2/dbt/include/fabric/macros/materializations/models/incremental/
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-15 18:43:43.000000 dbt-fabric-1.8.2/dbt/include/fabric/macros/materializations/models/incremental/incremental_strategies.sql
--rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-04-15 18:43:43.000000 dbt-fabric-1.8.2/dbt/include/fabric/macros/materializations/models/incremental/merge.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 18:44:23.552761 dbt-fabric-1.8.2/dbt/include/fabric/macros/materializations/models/table/
--rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-04-15 18:43:43.000000 dbt-fabric-1.8.2/dbt/include/fabric/macros/materializations/models/table/clone.sql
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-15 18:43:43.000000 dbt-fabric-1.8.2/dbt/include/fabric/macros/materializations/models/table/columns_spec_ddl.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-04-15 18:43:43.000000 dbt-fabric-1.8.2/dbt/include/fabric/macros/materializations/models/table/create_table_as.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-04-15 18:43:43.000000 dbt-fabric-1.8.2/dbt/include/fabric/macros/materializations/models/table/table.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 18:44:23.552761 dbt-fabric-1.8.2/dbt/include/fabric/macros/materializations/models/view/
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-04-15 18:43:43.000000 dbt-fabric-1.8.2/dbt/include/fabric/macros/materializations/models/view/create_view_as.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-04-15 18:43:43.000000 dbt-fabric-1.8.2/dbt/include/fabric/macros/materializations/models/view/view.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 18:44:23.552761 dbt-fabric-1.8.2/dbt/include/fabric/macros/materializations/seeds/
--rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-04-15 18:43:43.000000 dbt-fabric-1.8.2/dbt/include/fabric/macros/materializations/seeds/helpers.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 18:44:23.552761 dbt-fabric-1.8.2/dbt/include/fabric/macros/materializations/snapshots/
--rw-r--r--   0 runner    (1001) docker     (127)     5554 2024-04-15 18:43:43.000000 dbt-fabric-1.8.2/dbt/include/fabric/macros/materializations/snapshots/helpers.sql
--rw-r--r--   0 runner    (1001) docker     (127)     4421 2024-04-15 18:43:43.000000 dbt-fabric-1.8.2/dbt/include/fabric/macros/materializations/snapshots/snapshot.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-15 18:43:43.000000 dbt-fabric-1.8.2/dbt/include/fabric/macros/materializations/snapshots/snapshot_merge.sql
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-15 18:43:43.000000 dbt-fabric-1.8.2/dbt/include/fabric/macros/materializations/snapshots/strategies.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 18:44:23.552761 dbt-fabric-1.8.2/dbt/include/fabric/macros/materializations/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-04-15 18:43:43.000000 dbt-fabric-1.8.2/dbt/include/fabric/macros/materializations/tests/helpers.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 18:44:23.552761 dbt-fabric-1.8.2/dbt/include/fabric/macros/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-15 18:43:43.000000 dbt-fabric-1.8.2/dbt/include/fabric/macros/utils/any_value.sql
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-15 18:43:43.000000 dbt-fabric-1.8.2/dbt/include/fabric/macros/utils/array_construct.sql
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-15 18:43:43.000000 dbt-fabric-1.8.2/dbt/include/fabric/macros/utils/cast_bool_to_text.sql
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-15 18:43:43.000000 dbt-fabric-1.8.2/dbt/include/fabric/macros/utils/concat.sql
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-15 18:43:43.000000 dbt-fabric-1.8.2/dbt/include/fabric/macros/utils/date_trunc.sql
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-15 18:43:43.000000 dbt-fabric-1.8.2/dbt/include/fabric/macros/utils/dateadd.sql
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-15 18:43:43.000000 dbt-fabric-1.8.2/dbt/include/fabric/macros/utils/hash.sql
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-15 18:43:43.000000 dbt-fabric-1.8.2/dbt/include/fabric/macros/utils/last_day.sql
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-15 18:43:43.000000 dbt-fabric-1.8.2/dbt/include/fabric/macros/utils/length.sql
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-15 18:43:43.000000 dbt-fabric-1.8.2/dbt/include/fabric/macros/utils/listagg.sql
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-15 18:43:43.000000 dbt-fabric-1.8.2/dbt/include/fabric/macros/utils/position.sql
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-15 18:43:43.000000 dbt-fabric-1.8.2/dbt/include/fabric/macros/utils/safe_cast.sql
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-15 18:43:43.000000 dbt-fabric-1.8.2/dbt/include/fabric/macros/utils/timestamps.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 18:44:23.556761 dbt-fabric-1.8.2/dbt_fabric.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3680 2024-04-15 18:44:23.000000 dbt-fabric-1.8.2/dbt_fabric.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2549 2024-04-15 18:44:23.000000 dbt-fabric-1.8.2/dbt_fabric.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 18:44:23.000000 dbt-fabric-1.8.2/dbt_fabric.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-15 18:44:23.000000 dbt-fabric-1.8.2/dbt_fabric.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-15 18:44:23.000000 dbt-fabric-1.8.2/dbt_fabric.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 18:44:23.556761 dbt-fabric-1.8.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3368 2024-04-15 18:43:43.000000 dbt-fabric-1.8.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 00:47:46.759906 dbt-fabric-1.8.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-25 00:46:55.000000 dbt-fabric-1.8.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-25 00:46:55.000000 dbt-fabric-1.8.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3680 2024-04-25 00:47:46.759906 dbt-fabric-1.8.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2549 2024-04-25 00:46:55.000000 dbt-fabric-1.8.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 00:47:46.751906 dbt-fabric-1.8.3/dbt/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 00:47:46.751906 dbt-fabric-1.8.3/dbt/adapters/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 00:47:46.751906 dbt-fabric-1.8.3/dbt/adapters/fabric/
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-04-25 00:46:55.000000 dbt-fabric-1.8.3/dbt/adapters/fabric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-25 00:46:55.000000 dbt-fabric-1.8.3/dbt/adapters/fabric/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9641 2024-04-25 00:46:55.000000 dbt-fabric-1.8.3/dbt/adapters/fabric/fabric_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-25 00:46:55.000000 dbt-fabric-1.8.3/dbt/adapters/fabric/fabric_column.py
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-25 00:46:55.000000 dbt-fabric-1.8.3/dbt/adapters/fabric/fabric_configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16541 2024-04-25 00:46:55.000000 dbt-fabric-1.8.3/dbt/adapters/fabric/fabric_connection_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2016 2024-04-25 00:46:55.000000 dbt-fabric-1.8.3/dbt/adapters/fabric/fabric_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)      963 2024-04-25 00:46:55.000000 dbt-fabric-1.8.3/dbt/adapters/fabric/fabric_relation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 00:47:46.755906 dbt-fabric-1.8.3/dbt/adapters/fabric/relation_configs/
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-25 00:46:55.000000 dbt-fabric-1.8.3/dbt/adapters/fabric/relation_configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2290 2024-04-25 00:46:55.000000 dbt-fabric-1.8.3/dbt/adapters/fabric/relation_configs/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-25 00:46:55.000000 dbt-fabric-1.8.3/dbt/adapters/fabric/relation_configs/policies.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 00:47:46.751906 dbt-fabric-1.8.3/dbt/include/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 00:47:46.755906 dbt-fabric-1.8.3/dbt/include/fabric/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-25 00:46:55.000000 dbt-fabric-1.8.3/dbt/include/fabric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-25 00:46:55.000000 dbt-fabric-1.8.3/dbt/include/fabric/dbt_project.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 00:47:46.751906 dbt-fabric-1.8.3/dbt/include/fabric/macros/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 00:47:46.755906 dbt-fabric-1.8.3/dbt/include/fabric/macros/adapters/
+-rw-r--r--   0 runner    (1001) docker     (127)     3443 2024-04-25 00:46:55.000000 dbt-fabric-1.8.3/dbt/include/fabric/macros/adapters/apply_grants.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     7332 2024-04-25 00:46:55.000000 dbt-fabric-1.8.3/dbt/include/fabric/macros/adapters/catalog.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     4775 2024-04-25 00:46:55.000000 dbt-fabric-1.8.3/dbt/include/fabric/macros/adapters/columns.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     3763 2024-04-25 00:46:55.000000 dbt-fabric-1.8.3/dbt/include/fabric/macros/adapters/indexes.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     3411 2024-04-25 00:46:55.000000 dbt-fabric-1.8.3/dbt/include/fabric/macros/adapters/metadata.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-25 00:46:55.000000 dbt-fabric-1.8.3/dbt/include/fabric/macros/adapters/persist_docs.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     3004 2024-04-25 00:46:55.000000 dbt-fabric-1.8.3/dbt/include/fabric/macros/adapters/relation.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-04-25 00:46:55.000000 dbt-fabric-1.8.3/dbt/include/fabric/macros/adapters/schema.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-25 00:46:55.000000 dbt-fabric-1.8.3/dbt/include/fabric/macros/adapters/show.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 00:47:46.751906 dbt-fabric-1.8.3/dbt/include/fabric/macros/materializations/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 00:47:46.751906 dbt-fabric-1.8.3/dbt/include/fabric/macros/materializations/models/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 00:47:46.755906 dbt-fabric-1.8.3/dbt/include/fabric/macros/materializations/models/incremental/
+-rw-r--r--   0 runner    (1001) docker     (127)     4169 2024-04-25 00:46:55.000000 dbt-fabric-1.8.3/dbt/include/fabric/macros/materializations/models/incremental/incremental.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-25 00:46:55.000000 dbt-fabric-1.8.3/dbt/include/fabric/macros/materializations/models/incremental/incremental_strategies.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-04-25 00:46:55.000000 dbt-fabric-1.8.3/dbt/include/fabric/macros/materializations/models/incremental/merge.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 00:47:46.755906 dbt-fabric-1.8.3/dbt/include/fabric/macros/materializations/models/table/
+-rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-04-25 00:46:55.000000 dbt-fabric-1.8.3/dbt/include/fabric/macros/materializations/models/table/clone.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-25 00:46:55.000000 dbt-fabric-1.8.3/dbt/include/fabric/macros/materializations/models/table/columns_spec_ddl.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-04-25 00:46:55.000000 dbt-fabric-1.8.3/dbt/include/fabric/macros/materializations/models/table/create_table_as.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-04-25 00:46:55.000000 dbt-fabric-1.8.3/dbt/include/fabric/macros/materializations/models/table/table.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 00:47:46.755906 dbt-fabric-1.8.3/dbt/include/fabric/macros/materializations/models/view/
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-04-25 00:46:55.000000 dbt-fabric-1.8.3/dbt/include/fabric/macros/materializations/models/view/create_view_as.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-04-25 00:46:55.000000 dbt-fabric-1.8.3/dbt/include/fabric/macros/materializations/models/view/view.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 00:47:46.755906 dbt-fabric-1.8.3/dbt/include/fabric/macros/materializations/seeds/
+-rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-04-25 00:46:55.000000 dbt-fabric-1.8.3/dbt/include/fabric/macros/materializations/seeds/helpers.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 00:47:46.755906 dbt-fabric-1.8.3/dbt/include/fabric/macros/materializations/snapshots/
+-rw-r--r--   0 runner    (1001) docker     (127)     5554 2024-04-25 00:46:55.000000 dbt-fabric-1.8.3/dbt/include/fabric/macros/materializations/snapshots/helpers.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     4421 2024-04-25 00:46:55.000000 dbt-fabric-1.8.3/dbt/include/fabric/macros/materializations/snapshots/snapshot.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-25 00:46:55.000000 dbt-fabric-1.8.3/dbt/include/fabric/macros/materializations/snapshots/snapshot_merge.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-25 00:46:55.000000 dbt-fabric-1.8.3/dbt/include/fabric/macros/materializations/snapshots/strategies.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 00:47:46.759906 dbt-fabric-1.8.3/dbt/include/fabric/macros/materializations/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-04-25 00:46:55.000000 dbt-fabric-1.8.3/dbt/include/fabric/macros/materializations/tests/helpers.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 00:47:46.759906 dbt-fabric-1.8.3/dbt/include/fabric/macros/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-25 00:46:55.000000 dbt-fabric-1.8.3/dbt/include/fabric/macros/utils/any_value.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-25 00:46:55.000000 dbt-fabric-1.8.3/dbt/include/fabric/macros/utils/array_construct.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-25 00:46:55.000000 dbt-fabric-1.8.3/dbt/include/fabric/macros/utils/cast_bool_to_text.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-25 00:46:55.000000 dbt-fabric-1.8.3/dbt/include/fabric/macros/utils/concat.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-25 00:46:55.000000 dbt-fabric-1.8.3/dbt/include/fabric/macros/utils/date_trunc.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-25 00:46:55.000000 dbt-fabric-1.8.3/dbt/include/fabric/macros/utils/dateadd.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-04-25 00:46:55.000000 dbt-fabric-1.8.3/dbt/include/fabric/macros/utils/get_tables_by_pattern.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-25 00:46:55.000000 dbt-fabric-1.8.3/dbt/include/fabric/macros/utils/hash.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-25 00:46:55.000000 dbt-fabric-1.8.3/dbt/include/fabric/macros/utils/last_day.sql
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-25 00:46:55.000000 dbt-fabric-1.8.3/dbt/include/fabric/macros/utils/length.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-25 00:46:55.000000 dbt-fabric-1.8.3/dbt/include/fabric/macros/utils/listagg.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-25 00:46:55.000000 dbt-fabric-1.8.3/dbt/include/fabric/macros/utils/position.sql
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-25 00:46:55.000000 dbt-fabric-1.8.3/dbt/include/fabric/macros/utils/safe_cast.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-25 00:46:55.000000 dbt-fabric-1.8.3/dbt/include/fabric/macros/utils/timestamps.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 00:47:46.759906 dbt-fabric-1.8.3/dbt_fabric.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3680 2024-04-25 00:47:46.000000 dbt-fabric-1.8.3/dbt_fabric.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2867 2024-04-25 00:47:46.000000 dbt-fabric-1.8.3/dbt_fabric.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 00:47:46.000000 dbt-fabric-1.8.3/dbt_fabric.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-25 00:47:46.000000 dbt-fabric-1.8.3/dbt_fabric.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-25 00:47:46.000000 dbt-fabric-1.8.3/dbt_fabric.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 00:47:46.759906 dbt-fabric-1.8.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3368 2024-04-25 00:46:55.000000 dbt-fabric-1.8.3/setup.py
```

### Comparing `dbt-fabric-1.8.2/LICENSE` & `dbt-fabric-1.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt-fabric-1.8.2/PKG-INFO` & `dbt-fabric-1.8.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-fabric
-Version: 1.8.2
+Version: 1.8.3
 Summary: A Microsoft Fabric Synapse Data Warehouse adapter plugin for dbt
 Home-page: https://github.com/microsoft/dbt-fabric
 Author: Pradeep Srikakolapu
 License: MIT
 Project-URL: Setup & configuration, https://docs.getdbt.com/reference/warehouse-profiles/fabric-profile
 Project-URL: Documentation & usage, https://docs.getdbt.com/reference/resource-configs/fabric-configs
 Project-URL: Changelog, https://github.com/microsoft/dbt-fabric/blob/master/CHANGELOG.md
```

### Comparing `dbt-fabric-1.8.2/README.md` & `dbt-fabric-1.8.3/README.md`

 * *Files identical despite different names*

### Comparing `dbt-fabric-1.8.2/dbt/adapters/fabric/__init__.py` & `dbt-fabric-1.8.3/dbt/adapters/fabric/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-fabric-1.8.2/dbt/adapters/fabric/fabric_adapter.py` & `dbt-fabric-1.8.3/dbt/adapters/fabric/fabric_adapter.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,20 +17,22 @@
     ModelLevelConstraint,
 )
 from dbt_common.events.functions import fire_event
 
 from dbt.adapters.fabric.fabric_column import FabricColumn
 from dbt.adapters.fabric.fabric_configs import FabricConfigs
 from dbt.adapters.fabric.fabric_connection_manager import FabricConnectionManager
+from dbt.adapters.fabric.fabric_relation import FabricRelation
 
 
 class FabricAdapter(SQLAdapter):
     ConnectionManager = FabricConnectionManager
     Column = FabricColumn
     AdapterSpecificConfigs = FabricConfigs
+    Relation = FabricRelation
 
     _capabilities: CapabilityDict = CapabilityDict(
         {
             Capability.SchemaMetadataByRelations: CapabilitySupport(support=Support.Full),
             Capability.TableLastModifiedMetadata: CapabilitySupport(support=Support.Full),
         }
     )
@@ -179,30 +181,14 @@
         except BaseException:
             if conn.handle and not getattr(conn.handle, "closed", True):
                 conn.handle.rollback()
             raise
         finally:
             conn.transaction_open = False
 
-    def render_limited(self) -> str:
-        rendered = self.render()
-        if self.limit is None:
-            return rendered
-        elif self.limit == 0:
-            return f"(select * from {rendered} where 1=0) _dbt_top_subq"
-        else:
-            return f"(select TOP {self.limit} * from {rendered}) _dbt_top_subq"
-
-    # TODO: Standardizing quote characters
-    # def quoted(self, identifier):
-    #     return "[{identifier}]".format(
-    #         quote_char=self.quote_character,
-    #         identifier=identifier,
-    #     )
-
     @available
     @classmethod
     def render_column_constraint(cls, constraint: ColumnLevelConstraint) -> Optional[str]:
         rendered_column_constraint = None
         if constraint.type == ConstraintType.not_null:
             rendered_column_constraint = "not null "
         else:
```

### Comparing `dbt-fabric-1.8.2/dbt/adapters/fabric/fabric_column.py` & `dbt-fabric-1.8.3/dbt/adapters/fabric/fabric_column.py`

 * *Files identical despite different names*

### Comparing `dbt-fabric-1.8.2/dbt/adapters/fabric/fabric_connection_manager.py` & `dbt-fabric-1.8.3/dbt/adapters/fabric/fabric_connection_manager.py`

 * *Files identical despite different names*

### Comparing `dbt-fabric-1.8.2/dbt/adapters/fabric/fabric_credentials.py` & `dbt-fabric-1.8.3/dbt/adapters/fabric/fabric_credentials.py`

 * *Files identical despite different names*

### Comparing `dbt-fabric-1.8.2/dbt/include/fabric/macros/adapters/apply_grants.sql` & `dbt-fabric-1.8.3/dbt/include/fabric/macros/adapters/apply_grants.sql`

 * *Files identical despite different names*

### Comparing `dbt-fabric-1.8.2/dbt/include/fabric/macros/adapters/catalog.sql` & `dbt-fabric-1.8.3/dbt/include/fabric/macros/adapters/catalog.sql`

 * *Files identical despite different names*

### Comparing `dbt-fabric-1.8.2/dbt/include/fabric/macros/adapters/columns.sql` & `dbt-fabric-1.8.3/dbt/include/fabric/macros/adapters/columns.sql`

 * *Files identical despite different names*

### Comparing `dbt-fabric-1.8.2/dbt/include/fabric/macros/adapters/indexes.sql` & `dbt-fabric-1.8.3/dbt/include/fabric/macros/adapters/indexes.sql`

 * *Files identical despite different names*

### Comparing `dbt-fabric-1.8.2/dbt/include/fabric/macros/adapters/metadata.sql` & `dbt-fabric-1.8.3/dbt/include/fabric/macros/adapters/metadata.sql`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 
 {% macro fabric__information_schema_name(database) -%}
   information_schema
 {%- endmacro %}
 
 {% macro fabric__list_schemas(database) %}
   {% call statement('list_schemas', fetch_result=True, auto_begin=False) -%}
-
     select  name as [schema]
     from sys.schemas {{ information_schema_hints() }}
   {% endcall %}
   {{ return(load_result('list_schemas').table) }}
 {% endmacro %}
 
 {% macro fabric__check_schema_exists(information_schema, schema) -%}
@@ -24,14 +23,15 @@
     SELECT count(*) as schema_exist FROM sys.schemas WHERE name = '{{ schema }}'
   {%- endcall %}
   {{ return(load_result('check_schema_exists').table) }}
 {% endmacro %}
 
 {% macro fabric__list_relations_without_caching(schema_relation) -%}
   {% call statement('list_relations_without_caching', fetch_result=True) -%}
+    USE [{{ schema_relation.database }}];
     with base as (
       select
         DB_NAME() as [database],
         t.name as [name],
         SCHEMA_NAME(t.schema_id) as [schema],
         'table' as table_type
       from sys.tables as t {{ information_schema_hints() }}
@@ -47,14 +47,15 @@
     where [schema] like '{{ schema_relation.schema }}'
   {% endcall %}
   {{ return(load_result('list_relations_without_caching').table) }}
 {% endmacro %}
 
 {% macro fabric__get_relation_without_caching(schema_relation) -%}
   {% call statement('get_relation_without_caching', fetch_result=True) -%}
+    USE [{{ schema_relation.database }}];
     with base as (
       select
         DB_NAME() as [database],
         t.name as [name],
         SCHEMA_NAME(t.schema_id) as [schema],
         'table' as table_type
       from sys.tables as t {{ information_schema_hints() }}
```

### Comparing `dbt-fabric-1.8.2/dbt/include/fabric/macros/adapters/schema.sql` & `dbt-fabric-1.8.3/dbt/include/fabric/macros/adapters/schema.sql`

 * *Files identical despite different names*

### Comparing `dbt-fabric-1.8.2/dbt/include/fabric/macros/materializations/models/incremental/merge.sql` & `dbt-fabric-1.8.3/dbt/include/fabric/macros/materializations/models/incremental/merge.sql`

 * *Files identical despite different names*

### Comparing `dbt-fabric-1.8.2/dbt/include/fabric/macros/materializations/models/table/clone.sql` & `dbt-fabric-1.8.3/dbt/include/fabric/macros/materializations/models/table/clone.sql`

 * *Files identical despite different names*

### Comparing `dbt-fabric-1.8.2/dbt/include/fabric/macros/materializations/models/table/columns_spec_ddl.sql` & `dbt-fabric-1.8.3/dbt/include/fabric/macros/materializations/models/table/columns_spec_ddl.sql`

 * *Files identical despite different names*

### Comparing `dbt-fabric-1.8.2/dbt/include/fabric/macros/materializations/models/table/create_table_as.sql` & `dbt-fabric-1.8.3/dbt/include/fabric/macros/materializations/models/table/create_table_as.sql`

 * *Files identical despite different names*

### Comparing `dbt-fabric-1.8.2/dbt/include/fabric/macros/materializations/models/table/table.sql` & `dbt-fabric-1.8.3/dbt/include/fabric/macros/materializations/models/table/table.sql`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,36 @@
 {% materialization table, adapter='fabric' %}
 
-  -- Create target relation
+  -- Load target relation
   {%- set target_relation = this.incorporate(type='table') %}
+  -- Load existing relation
+  {%- set relation = fabric__get_relation_without_caching(this) %}
+
+  {% set existing_relation = none %}
+  {% if (relation|length == 1) %}
+    {% set existing_relation = get_or_create_relation(relation[0][0], relation[0][2] , relation[0][1] , relation[0][3])[1] %}
+  {% endif %}
+
+  {%- set backup_relation = none %}
+  {{log("Existing Relation type is "~ existing_relation.type)}}
+  {% if (existing_relation != none and existing_relation.type == "table") %}
+      {%- set backup_relation = make_backup_relation(target_relation, 'table') -%}
+  {% elif (existing_relation != none and existing_relation.type == "view") %}
+      {%- set backup_relation = make_backup_relation(target_relation, 'view') -%}
+  {% endif %}
+
+  {% if (existing_relation != none) %}
+    -- drop the temp relations if they exist already in the database
+    {{ drop_relation_if_exists(backup_relation) }}
+    -- Rename target relation as backup relation
+    {{ adapter.rename_relation(existing_relation, backup_relation) }}
+  {% endif %}
+
   -- grab current tables grants config for comparision later on
   {% set grant_config = config.get('grants') %}
-  {%- set backup_relation = make_backup_relation(target_relation, 'table') -%}
-  -- drop the temp relations if they exist already in the database
-  {{ drop_relation_if_exists(backup_relation) }}
-  -- Rename target relation as backup relation
-  {%- set relation = fabric__get_relation_without_caching(target_relation) %}
-  {% if relation|length > 0 %}
-    {{ adapter.rename_relation(target_relation, backup_relation) }}
-  {% endif %}
 
   {{ run_hooks(pre_hooks, inside_transaction=False) }}
   -- `BEGIN` happens here:
   {{ run_hooks(pre_hooks, inside_transaction=True) }}
 
   -- build model
   {% call statement('main') -%}
@@ -25,17 +40,19 @@
   -- cleanup
   {{ run_hooks(post_hooks, inside_transaction=True) }}
   {% do apply_grants(target_relation, grant_config, should_revoke=should_revoke) %}
   {% do persist_docs(target_relation, model) %}
   -- `COMMIT` happens here
   {{ adapter.commit() }}
 
-  -- finally, drop the foreign key references if exists
-  {{ drop_fk_indexes_on_table(backup_relation) }}
-  -- drop existing/backup relation after the commit
-  {{ drop_relation_if_exists(backup_relation) }}
+  {% if (backup_relation != none) %}
+    -- finally, drop the foreign key references if exists
+    {{ drop_fk_indexes_on_table(backup_relation) }}
+    -- drop existing/backup relation after the commit
+    {{ drop_relation_if_exists(backup_relation) }}
+   {% endif %}
   -- Add constraints including FK relation.
   {{ fabric__build_model_constraints(target_relation) }}
   {{ run_hooks(post_hooks, inside_transaction=False) }}
   {{ return({'relations': [target_relation]}) }}
 
 {% endmaterialization %}
```

### Comparing `dbt-fabric-1.8.2/dbt/include/fabric/macros/materializations/models/view/create_view_as.sql` & `dbt-fabric-1.8.3/dbt/include/fabric/macros/materializations/models/view/create_view_as.sql`

 * *Files identical despite different names*

### Comparing `dbt-fabric-1.8.2/dbt/include/fabric/macros/materializations/models/view/view.sql` & `dbt-fabric-1.8.3/dbt/include/fabric/macros/materializations/models/view/view.sql`

 * *Files 9% similar despite different names*

```diff
@@ -1,40 +1,51 @@
 {% materialization view, adapter='fabric' -%}
 
-  {%- set existing_relation = load_cached_relation(this) -%}
   {%- set target_relation = this.incorporate(type='view') -%}
+  {{log("Target Relation "~target_relation)}}
 
-  -- make back up relation
-  {%- set backup_relation_type = 'view' if existing_relation is none else existing_relation.type -%}
-  {%- set backup_relation = make_backup_relation(target_relation, backup_relation_type) -%}
+  {%- set relation = fabric__get_relation_without_caching(this) %}
+  {% set existing_relation = none %}
+  {% if (relation|length == 1) %}
+    {% set existing_relation = get_or_create_relation(relation[0][0], relation[0][2] , relation[0][1] , relation[0][3])[1] %}
+  {% endif %}
+  {{log("Existing Relation "~existing_relation)}}
+
+  {%- set backup_relation = none %}
+  {{log("Existing Relation type is "~ existing_relation.type)}}
+  {% if (existing_relation != none and existing_relation.type == "table") %}
+      {%- set backup_relation = make_backup_relation(target_relation, 'table') -%}
+  {% elif (existing_relation != none and existing_relation.type == "view") %}
+      {%- set backup_relation = make_backup_relation(target_relation, 'view') -%}
+  {% endif %}
+
+  {% if (existing_relation != none) %}
+    -- drop the temp relations if they exist already in the database
+    {{ drop_relation_if_exists(backup_relation) }}
+    -- Rename target relation as backup relation
+    {{ adapter.rename_relation(existing_relation, backup_relation) }}
+  {% endif %}
 
   {% set grant_config = config.get('grants') %}
   {{ run_hooks(pre_hooks, inside_transaction=False) }}
 
-  -- drop target relation if exists already in the database
-  {{ drop_relation_if_exists(backup_relation) }}
-
-  {%- set relation = fabric__get_relation_without_caching(target_relation) %}
-    {% if relation|length > 0 %}
-        {{ adapter.rename_relation(target_relation, backup_relation) }}
-    {% endif %}
-
   -- `BEGIN` happens here:
   {{ run_hooks(pre_hooks, inside_transaction=True) }}
 
   -- build model
   {% call statement('main') -%}
     {{ get_create_view_as_sql(target_relation, sql) }}
   {%- endcall %}
 
   {% set should_revoke = should_revoke(existing_relation, full_refresh_mode=True) %}
   {% do apply_grants(target_relation, grant_config, should_revoke=should_revoke) %}
 
   {% do persist_docs(target_relation, model) %}
   {{ run_hooks(post_hooks, inside_transaction=True) }}
   {{ adapter.commit() }}
-  {{ drop_relation_if_exists(backup_relation) }}
+  {% if (backup_relation != none) %}
+    {{ drop_relation_if_exists(backup_relation) }}
+  {% endif %}
   {{ run_hooks(post_hooks, inside_transaction=False) }}
-
   {{ return({'relations': [target_relation]}) }}
 
 {%- endmaterialization -%}
```

### Comparing `dbt-fabric-1.8.2/dbt/include/fabric/macros/materializations/seeds/helpers.sql` & `dbt-fabric-1.8.3/dbt/include/fabric/macros/materializations/seeds/helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt-fabric-1.8.2/dbt/include/fabric/macros/materializations/snapshots/helpers.sql` & `dbt-fabric-1.8.3/dbt/include/fabric/macros/materializations/snapshots/helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt-fabric-1.8.2/dbt/include/fabric/macros/materializations/snapshots/snapshot.sql` & `dbt-fabric-1.8.3/dbt/include/fabric/macros/materializations/snapshots/snapshot.sql`

 * *Files identical despite different names*

### Comparing `dbt-fabric-1.8.2/dbt/include/fabric/macros/materializations/snapshots/snapshot_merge.sql` & `dbt-fabric-1.8.3/dbt/include/fabric/macros/materializations/snapshots/snapshot_merge.sql`

 * *Files identical despite different names*

### Comparing `dbt-fabric-1.8.2/dbt/include/fabric/macros/materializations/tests/helpers.sql` & `dbt-fabric-1.8.3/dbt/include/fabric/macros/materializations/tests/helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt-fabric-1.8.2/dbt_fabric.egg-info/PKG-INFO` & `dbt-fabric-1.8.3/dbt_fabric.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-fabric
-Version: 1.8.2
+Version: 1.8.3
 Summary: A Microsoft Fabric Synapse Data Warehouse adapter plugin for dbt
 Home-page: https://github.com/microsoft/dbt-fabric
 Author: Pradeep Srikakolapu
 License: MIT
 Project-URL: Setup & configuration, https://docs.getdbt.com/reference/warehouse-profiles/fabric-profile
 Project-URL: Documentation & usage, https://docs.getdbt.com/reference/resource-configs/fabric-configs
 Project-URL: Changelog, https://github.com/microsoft/dbt-fabric/blob/master/CHANGELOG.md
```

### Comparing `dbt-fabric-1.8.2/dbt_fabric.egg-info/SOURCES.txt` & `dbt-fabric-1.8.3/dbt_fabric.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -5,25 +5,30 @@
 dbt/adapters/fabric/__init__.py
 dbt/adapters/fabric/__version__.py
 dbt/adapters/fabric/fabric_adapter.py
 dbt/adapters/fabric/fabric_column.py
 dbt/adapters/fabric/fabric_configs.py
 dbt/adapters/fabric/fabric_connection_manager.py
 dbt/adapters/fabric/fabric_credentials.py
+dbt/adapters/fabric/fabric_relation.py
+dbt/adapters/fabric/relation_configs/__init__.py
+dbt/adapters/fabric/relation_configs/base.py
+dbt/adapters/fabric/relation_configs/policies.py
 dbt/include/fabric/__init__.py
 dbt/include/fabric/dbt_project.yml
 dbt/include/fabric/macros/adapters/apply_grants.sql
 dbt/include/fabric/macros/adapters/catalog.sql
 dbt/include/fabric/macros/adapters/columns.sql
 dbt/include/fabric/macros/adapters/indexes.sql
 dbt/include/fabric/macros/adapters/metadata.sql
 dbt/include/fabric/macros/adapters/persist_docs.sql
 dbt/include/fabric/macros/adapters/relation.sql
 dbt/include/fabric/macros/adapters/schema.sql
 dbt/include/fabric/macros/adapters/show.sql
+dbt/include/fabric/macros/materializations/models/incremental/incremental.sql
 dbt/include/fabric/macros/materializations/models/incremental/incremental_strategies.sql
 dbt/include/fabric/macros/materializations/models/incremental/merge.sql
 dbt/include/fabric/macros/materializations/models/table/clone.sql
 dbt/include/fabric/macros/materializations/models/table/columns_spec_ddl.sql
 dbt/include/fabric/macros/materializations/models/table/create_table_as.sql
 dbt/include/fabric/macros/materializations/models/table/table.sql
 dbt/include/fabric/macros/materializations/models/view/create_view_as.sql
@@ -36,14 +41,15 @@
 dbt/include/fabric/macros/materializations/tests/helpers.sql
 dbt/include/fabric/macros/utils/any_value.sql
 dbt/include/fabric/macros/utils/array_construct.sql
 dbt/include/fabric/macros/utils/cast_bool_to_text.sql
 dbt/include/fabric/macros/utils/concat.sql
 dbt/include/fabric/macros/utils/date_trunc.sql
 dbt/include/fabric/macros/utils/dateadd.sql
+dbt/include/fabric/macros/utils/get_tables_by_pattern.sql
 dbt/include/fabric/macros/utils/hash.sql
 dbt/include/fabric/macros/utils/last_day.sql
 dbt/include/fabric/macros/utils/length.sql
 dbt/include/fabric/macros/utils/listagg.sql
 dbt/include/fabric/macros/utils/position.sql
 dbt/include/fabric/macros/utils/safe_cast.sql
 dbt/include/fabric/macros/utils/timestamps.sql
```

### Comparing `dbt-fabric-1.8.2/setup.py` & `dbt-fabric-1.8.3/setup.py`

 * *Files identical despite different names*


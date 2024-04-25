# Comparing `tmp/modelbaker-1.7.2.tar.gz` & `tmp/modelbaker-1.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modelbaker-1.7.2.tar", last modified: Mon Mar 11 19:57:19 2024, max compression
+gzip compressed data, was "modelbaker-1.7.3.tar", last modified: Thu Apr 25 15:06:33 2024, max compression
```

## Comparing `modelbaker-1.7.2.tar` & `modelbaker-1.7.3.tar`

### file list

```diff
@@ -1,125 +1,125 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 19:57:19.657474 modelbaker-1.7.2/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-03-11 19:57:09.000000 modelbaker-1.7.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-03-11 19:57:19.653474 modelbaker-1.7.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2956 2024-03-11 19:57:09.000000 modelbaker-1.7.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 19:57:19.637474 modelbaker-1.7.2/modelbaker/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-11 19:57:09.000000 modelbaker-1.7.2/modelbaker/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 19:57:19.637474 modelbaker-1.7.2/modelbaker/dataobjects/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-11 19:57:09.000000 modelbaker-1.7.2/modelbaker/dataobjects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-03-11 19:57:09.000000 modelbaker-1.7.2/modelbaker/dataobjects/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     5050 2024-03-11 19:57:09.000000 modelbaker-1.7.2/modelbaker/dataobjects/form.py
--rw-r--r--   0 runner    (1001) docker     (127)    14353 2024-03-11 19:57:09.000000 modelbaker-1.7.2/modelbaker/dataobjects/layers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4520 2024-03-11 19:57:09.000000 modelbaker-1.7.2/modelbaker/dataobjects/legend.py
--rw-r--r--   0 runner    (1001) docker     (127)    17376 2024-03-11 19:57:09.000000 modelbaker-1.7.2/modelbaker/dataobjects/project.py
--rw-r--r--   0 runner    (1001) docker     (127)     2334 2024-03-11 19:57:09.000000 modelbaker-1.7.2/modelbaker/dataobjects/relations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 19:57:19.641474 modelbaker-1.7.2/modelbaker/db_factory/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-11 19:57:09.000000 modelbaker-1.7.2/modelbaker/db_factory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3705 2024-03-11 19:57:09.000000 modelbaker-1.7.2/modelbaker/db_factory/db_command_config_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     4370 2024-03-11 19:57:09.000000 modelbaker-1.7.2/modelbaker/db_factory/db_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     3433 2024-03-11 19:57:09.000000 modelbaker-1.7.2/modelbaker/db_factory/db_simple_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-03-11 19:57:09.000000 modelbaker-1.7.2/modelbaker/db_factory/gpkg_command_config_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-03-11 19:57:09.000000 modelbaker-1.7.2/modelbaker/db_factory/gpkg_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-03-11 19:57:09.000000 modelbaker-1.7.2/modelbaker/db_factory/gpkg_layer_uri.py
--rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-03-11 19:57:09.000000 modelbaker-1.7.2/modelbaker/db_factory/layer_uri.py
--rw-r--r--   0 runner    (1001) docker     (127)     4603 2024-03-11 19:57:09.000000 modelbaker-1.7.2/modelbaker/db_factory/mssql_command_config_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-03-11 19:57:09.000000 modelbaker-1.7.2/modelbaker/db_factory/mssql_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-03-11 19:57:09.000000 modelbaker-1.7.2/modelbaker/db_factory/mssql_layer_uri.py
--rw-r--r--   0 runner    (1001) docker     (127)     7981 2024-03-11 19:57:09.000000 modelbaker-1.7.2/modelbaker/db_factory/pg_command_config_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     3345 2024-03-11 19:57:09.000000 modelbaker-1.7.2/modelbaker/db_factory/pg_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-03-11 19:57:09.000000 modelbaker-1.7.2/modelbaker/db_factory/pg_layer_uri.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 19:57:19.641474 modelbaker-1.7.2/modelbaker/dbconnector/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-11 19:57:09.000000 modelbaker-1.7.2/modelbaker/dbconnector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-03-11 19:57:09.000000 modelbaker-1.7.2/modelbaker/dbconnector/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    13128 2024-03-11 19:57:09.000000 modelbaker-1.7.2/modelbaker/dbconnector/db_connector.py
--rw-r--r--   0 runner    (1001) docker     (127)    46341 2024-03-11 19:57:09.000000 modelbaker-1.7.2/modelbaker/dbconnector/gpkg_connector.py
--rw-r--r--   0 runner    (1001) docker     (127)    52028 2024-03-11 19:57:09.000000 modelbaker-1.7.2/modelbaker/dbconnector/mssql_connector.py
--rw-r--r--   0 runner    (1001) docker     (127)    54597 2024-03-11 19:57:09.000000 modelbaker-1.7.2/modelbaker/dbconnector/pg_connector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 19:57:19.641474 modelbaker-1.7.2/modelbaker/generator/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-11 19:57:09.000000 modelbaker-1.7.2/modelbaker/generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-03-11 19:57:09.000000 modelbaker-1.7.2/modelbaker/generator/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    50554 2024-03-11 19:57:09.000000 modelbaker-1.7.2/modelbaker/generator/domain_relations_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)    38741 2024-03-11 19:57:09.000000 modelbaker-1.7.2/modelbaker/generator/generator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 19:57:19.645474 modelbaker-1.7.2/modelbaker/ilitoppingmaker/
--rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-03-11 19:57:09.000000 modelbaker-1.7.2/modelbaker/ilitoppingmaker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5494 2024-03-11 19:57:09.000000 modelbaker-1.7.2/modelbaker/ilitoppingmaker/ili2dbsettings.py
--rw-r--r--   0 runner    (1001) docker     (127)     7933 2024-03-11 19:57:09.000000 modelbaker-1.7.2/modelbaker/ilitoppingmaker/ilidata.py
--rw-r--r--   0 runner    (1001) docker     (127)     4743 2024-03-11 19:57:09.000000 modelbaker-1.7.2/modelbaker/ilitoppingmaker/iliprojecttopping.py
--rw-r--r--   0 runner    (1001) docker     (127)     3266 2024-03-11 19:57:09.000000 modelbaker-1.7.2/modelbaker/ilitoppingmaker/ilitarget.py
--rw-r--r--   0 runner    (1001) docker     (127)     6067 2024-03-11 19:57:09.000000 modelbaker-1.7.2/modelbaker/ilitoppingmaker/metaconfig.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 19:57:19.645474 modelbaker-1.7.2/modelbaker/iliwrapper/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-11 19:57:09.000000 modelbaker-1.7.2/modelbaker/iliwrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-03-11 19:57:09.000000 modelbaker-1.7.2/modelbaker/iliwrapper/globals.py
--rw-r--r--   0 runner    (1001) docker     (127)     4537 2024-03-11 19:57:09.000000 modelbaker-1.7.2/modelbaker/iliwrapper/ili2dbargs.py
--rw-r--r--   0 runner    (1001) docker     (127)    16784 2024-03-11 19:57:09.000000 modelbaker-1.7.2/modelbaker/iliwrapper/ili2dbconfig.py
--rw-r--r--   0 runner    (1001) docker     (127)     2179 2024-03-11 19:57:09.000000 modelbaker-1.7.2/modelbaker/iliwrapper/ili2dbtools.py
--rw-r--r--   0 runner    (1001) docker     (127)    13510 2024-03-11 19:57:09.000000 modelbaker-1.7.2/modelbaker/iliwrapper/ili2dbutils.py
--rw-r--r--   0 runner    (1001) docker     (127)    42200 2024-03-11 19:57:09.000000 modelbaker-1.7.2/modelbaker/iliwrapper/ilicache.py
--rw-r--r--   0 runner    (1001) docker     (127)     6182 2024-03-11 19:57:09.000000 modelbaker-1.7.2/modelbaker/iliwrapper/iliexecutable.py
--rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-03-11 19:57:09.000000 modelbaker-1.7.2/modelbaker/iliwrapper/iliexporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-03-11 19:57:09.000000 modelbaker-1.7.2/modelbaker/iliwrapper/iliimporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-03-11 19:57:09.000000 modelbaker-1.7.2/modelbaker/iliwrapper/iliupdater.py
--rw-r--r--   0 runner    (1001) docker     (127)     6192 2024-03-11 19:57:09.000000 modelbaker-1.7.2/modelbaker/iliwrapper/ilivalidator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 19:57:19.645474 modelbaker-1.7.2/modelbaker/libs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-11 19:57:13.000000 modelbaker-1.7.2/modelbaker/libs/__init__.py
--rw-rw-r--   0 runner    (1001) docker     (127)    12895 2020-04-20 14:21:10.000000 modelbaker-1.7.2/modelbaker/libs/deprecation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 19:57:19.649474 modelbaker-1.7.2/modelbaker/libs/packaging/
--rw-rw-r--   0 runner    (1001) docker     (127)      496 2024-03-10 09:38:56.000000 modelbaker-1.7.2/modelbaker/libs/packaging/__init__.py
--rw-rw-r--   0 runner    (1001) docker     (127)     3266 2023-01-30 15:29:48.000000 modelbaker-1.7.2/modelbaker/libs/packaging/_elffile.py
--rw-rw-r--   0 runner    (1001) docker     (127)     9590 2024-03-10 09:34:40.000000 modelbaker-1.7.2/modelbaker/libs/packaging/_manylinux.py
--rw-rw-r--   0 runner    (1001) docker     (127)     2676 2023-10-01 13:58:58.000000 modelbaker-1.7.2/modelbaker/libs/packaging/_musllinux.py
--rw-rw-r--   0 runner    (1001) docker     (127)    10347 2024-03-10 09:34:40.000000 modelbaker-1.7.2/modelbaker/libs/packaging/_parser.py
--rw-rw-r--   0 runner    (1001) docker     (127)     1431 2023-01-30 15:29:48.000000 modelbaker-1.7.2/modelbaker/libs/packaging/_structures.py
--rw-rw-r--   0 runner    (1001) docker     (127)     5292 2023-04-12 17:05:06.000000 modelbaker-1.7.2/modelbaker/libs/packaging/_tokenizer.py
--rw-rw-r--   0 runner    (1001) docker     (127)     8208 2023-04-12 17:05:28.000000 modelbaker-1.7.2/modelbaker/libs/packaging/markers.py
--rw-rw-r--   0 runner    (1001) docker     (127)    33036 2024-01-06 20:39:22.000000 modelbaker-1.7.2/modelbaker/libs/packaging/metadata.py
--rw-rw-r--   0 runner    (1001) docker     (127)        0 2023-01-30 15:29:48.000000 modelbaker-1.7.2/modelbaker/libs/packaging/py.typed
--rw-rw-r--   0 runner    (1001) docker     (127)     2933 2024-03-10 09:34:40.000000 modelbaker-1.7.2/modelbaker/libs/packaging/requirements.py
--rw-rw-r--   0 runner    (1001) docker     (127)    39784 2024-03-10 09:34:40.000000 modelbaker-1.7.2/modelbaker/libs/packaging/specifiers.py
--rw-rw-r--   0 runner    (1001) docker     (127)    18950 2024-01-06 20:39:22.000000 modelbaker-1.7.2/modelbaker/libs/packaging/tags.py
--rw-rw-r--   0 runner    (1001) docker     (127)     5268 2023-10-01 13:58:58.000000 modelbaker-1.7.2/modelbaker/libs/packaging/utils.py
--rw-rw-r--   0 runner    (1001) docker     (127)    16236 2023-10-01 13:58:58.000000 modelbaker-1.7.2/modelbaker/libs/packaging/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 19:57:19.649474 modelbaker-1.7.2/modelbaker/libs/pgserviceparser/
--rw-rw-r--   0 runner    (1001) docker     (127)     1801 2022-06-27 10:25:36.000000 modelbaker-1.7.2/modelbaker/libs/pgserviceparser/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 19:57:19.649474 modelbaker-1.7.2/modelbaker/libs/toppingmaker/
--rw-rw-r--   0 runner    (1001) docker     (127)     1128 2023-12-13 05:24:38.000000 modelbaker-1.7.2/modelbaker/libs/toppingmaker/__init__.py
--rw-rw-r--   0 runner    (1001) docker     (127)     6550 2023-12-13 05:24:38.000000 modelbaker-1.7.2/modelbaker/libs/toppingmaker/exportsettings.py
--rw-rw-r--   0 runner    (1001) docker     (127)    27294 2023-12-13 05:24:38.000000 modelbaker-1.7.2/modelbaker/libs/toppingmaker/projecttopping.py
--rw-rw-r--   0 runner    (1001) docker     (127)     3334 2023-12-13 05:24:38.000000 modelbaker-1.7.2/modelbaker/libs/toppingmaker/target.py
--rw-rw-r--   0 runner    (1001) docker     (127)     1297 2023-12-13 05:24:38.000000 modelbaker-1.7.2/modelbaker/libs/toppingmaker/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 19:57:19.649474 modelbaker-1.7.2/modelbaker/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-11 19:57:09.000000 modelbaker-1.7.2/modelbaker/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6460 2024-03-11 19:57:09.000000 modelbaker-1.7.2/modelbaker/utils/db_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-03-11 19:57:09.000000 modelbaker-1.7.2/modelbaker/utils/globals.py
--rw-r--r--   0 runner    (1001) docker     (127)     9881 2024-03-11 19:57:09.000000 modelbaker-1.7.2/modelbaker/utils/qgis_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10267 2024-03-11 19:57:09.000000 modelbaker-1.7.2/modelbaker/utils/qt_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 19:57:19.653474 modelbaker-1.7.2/modelbaker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-03-11 19:57:19.000000 modelbaker-1.7.2/modelbaker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3725 2024-03-11 19:57:19.000000 modelbaker-1.7.2/modelbaker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-11 19:57:19.000000 modelbaker-1.7.2/modelbaker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-11 19:57:19.000000 modelbaker-1.7.2/modelbaker.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-11 19:57:19.657474 modelbaker-1.7.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      874 2024-03-11 19:57:09.000000 modelbaker-1.7.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 19:57:19.653474 modelbaker-1.7.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    12962 2024-03-11 19:57:09.000000 modelbaker-1.7.2/tests/test_dataset_handling.py
--rw-r--r--   0 runner    (1001) docker     (127)   151890 2024-03-11 19:57:09.000000 modelbaker-1.7.2/tests/test_domain_class_relations.py
--rw-r--r--   0 runner    (1001) docker     (127)     2831 2024-03-11 19:57:09.000000 modelbaker-1.7.2/tests/test_dump.py
--rw-r--r--   0 runner    (1001) docker     (127)    39104 2024-03-11 19:57:09.000000 modelbaker-1.7.2/tests/test_export.py
--rw-r--r--   0 runner    (1001) docker     (127)     3425 2024-03-11 19:57:09.000000 modelbaker-1.7.2/tests/test_get_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     6543 2024-03-11 19:57:09.000000 modelbaker-1.7.2/tests/test_gpkg_pk.py
--rw-r--r--   0 runner    (1001) docker     (127)     2620 2024-03-11 19:57:09.000000 modelbaker-1.7.2/tests/test_ili2dbutils.py
--rw-r--r--   0 runner    (1001) docker     (127)    31704 2024-03-11 19:57:09.000000 modelbaker-1.7.2/tests/test_ilicache.py
--rw-r--r--   0 runner    (1001) docker     (127)    13620 2024-03-11 19:57:09.000000 modelbaker-1.7.2/tests/test_ilitoppingmaker.py
--rw-r--r--   0 runner    (1001) docker     (127)    17928 2024-03-11 19:57:09.000000 modelbaker-1.7.2/tests/test_import.py
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-03-11 19:57:09.000000 modelbaker-1.7.2/tests/test_libili2pg.py
--rw-r--r--   0 runner    (1001) docker     (127)    14531 2024-03-11 19:57:09.000000 modelbaker-1.7.2/tests/test_metaconfig.py
--rw-r--r--   0 runner    (1001) docker     (127)    11343 2024-03-11 19:57:09.000000 modelbaker-1.7.2/tests/test_pgservice.py
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-03-11 19:57:09.000000 modelbaker-1.7.2/tests/test_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)   166557 2024-03-11 19:57:09.000000 modelbaker-1.7.2/tests/test_projectgen.py
--rw-r--r--   0 runner    (1001) docker     (127)   111101 2024-03-11 19:57:09.000000 modelbaker-1.7.2/tests/test_projectgen_extension_optimization.py
--rw-r--r--   0 runner    (1001) docker     (127)    15529 2024-03-11 19:57:09.000000 modelbaker-1.7.2/tests/test_projectgen_generic_databases.py
--rw-r--r--   0 runner    (1001) docker     (127)    40735 2024-03-11 19:57:09.000000 modelbaker-1.7.2/tests/test_projectgen_oids.py
--rw-r--r--   0 runner    (1001) docker     (127)    51641 2024-03-11 19:57:09.000000 modelbaker-1.7.2/tests/test_projecttopping.py
--rw-r--r--   0 runner    (1001) docker     (127)     7594 2024-03-11 19:57:09.000000 modelbaker-1.7.2/tests/test_sequence_reset.py
--rw-r--r--   0 runner    (1001) docker     (127)     5779 2024-03-11 19:57:09.000000 modelbaker-1.7.2/tests/test_update.py
--rw-r--r--   0 runner    (1001) docker     (127)    24379 2024-03-11 19:57:09.000000 modelbaker-1.7.2/tests/test_validate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-03-11 19:57:09.000000 modelbaker-1.7.2/tests/test_z_geom.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:06:33.985567 modelbaker-1.7.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-25 15:06:27.000000 modelbaker-1.7.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-04-25 15:06:33.985567 modelbaker-1.7.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2956 2024-04-25 15:06:27.000000 modelbaker-1.7.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:06:33.965567 modelbaker-1.7.3/modelbaker/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 15:06:27.000000 modelbaker-1.7.3/modelbaker/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:06:33.965567 modelbaker-1.7.3/modelbaker/dataobjects/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 15:06:27.000000 modelbaker-1.7.3/modelbaker/dataobjects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-04-25 15:06:27.000000 modelbaker-1.7.3/modelbaker/dataobjects/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5050 2024-04-25 15:06:27.000000 modelbaker-1.7.3/modelbaker/dataobjects/form.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14353 2024-04-25 15:06:27.000000 modelbaker-1.7.3/modelbaker/dataobjects/layers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4520 2024-04-25 15:06:27.000000 modelbaker-1.7.3/modelbaker/dataobjects/legend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17376 2024-04-25 15:06:27.000000 modelbaker-1.7.3/modelbaker/dataobjects/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2334 2024-04-25 15:06:27.000000 modelbaker-1.7.3/modelbaker/dataobjects/relations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:06:33.969567 modelbaker-1.7.3/modelbaker/db_factory/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 15:06:27.000000 modelbaker-1.7.3/modelbaker/db_factory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3705 2024-04-25 15:06:27.000000 modelbaker-1.7.3/modelbaker/db_factory/db_command_config_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4370 2024-04-25 15:06:27.000000 modelbaker-1.7.3/modelbaker/db_factory/db_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3433 2024-04-25 15:06:27.000000 modelbaker-1.7.3/modelbaker/db_factory/db_simple_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-04-25 15:06:27.000000 modelbaker-1.7.3/modelbaker/db_factory/gpkg_command_config_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-04-25 15:06:27.000000 modelbaker-1.7.3/modelbaker/db_factory/gpkg_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-04-25 15:06:27.000000 modelbaker-1.7.3/modelbaker/db_factory/gpkg_layer_uri.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-04-25 15:06:27.000000 modelbaker-1.7.3/modelbaker/db_factory/layer_uri.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4603 2024-04-25 15:06:27.000000 modelbaker-1.7.3/modelbaker/db_factory/mssql_command_config_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-04-25 15:06:27.000000 modelbaker-1.7.3/modelbaker/db_factory/mssql_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-04-25 15:06:27.000000 modelbaker-1.7.3/modelbaker/db_factory/mssql_layer_uri.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7981 2024-04-25 15:06:27.000000 modelbaker-1.7.3/modelbaker/db_factory/pg_command_config_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3345 2024-04-25 15:06:27.000000 modelbaker-1.7.3/modelbaker/db_factory/pg_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-04-25 15:06:27.000000 modelbaker-1.7.3/modelbaker/db_factory/pg_layer_uri.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:06:33.969567 modelbaker-1.7.3/modelbaker/dbconnector/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 15:06:27.000000 modelbaker-1.7.3/modelbaker/dbconnector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-04-25 15:06:27.000000 modelbaker-1.7.3/modelbaker/dbconnector/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13128 2024-04-25 15:06:27.000000 modelbaker-1.7.3/modelbaker/dbconnector/db_connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46521 2024-04-25 15:06:27.000000 modelbaker-1.7.3/modelbaker/dbconnector/gpkg_connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52246 2024-04-25 15:06:27.000000 modelbaker-1.7.3/modelbaker/dbconnector/mssql_connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54876 2024-04-25 15:06:27.000000 modelbaker-1.7.3/modelbaker/dbconnector/pg_connector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:06:33.969567 modelbaker-1.7.3/modelbaker/generator/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 15:06:27.000000 modelbaker-1.7.3/modelbaker/generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-25 15:06:27.000000 modelbaker-1.7.3/modelbaker/generator/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50554 2024-04-25 15:06:27.000000 modelbaker-1.7.3/modelbaker/generator/domain_relations_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38753 2024-04-25 15:06:27.000000 modelbaker-1.7.3/modelbaker/generator/generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:06:33.973567 modelbaker-1.7.3/modelbaker/ilitoppingmaker/
+-rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-04-25 15:06:27.000000 modelbaker-1.7.3/modelbaker/ilitoppingmaker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5494 2024-04-25 15:06:27.000000 modelbaker-1.7.3/modelbaker/ilitoppingmaker/ili2dbsettings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7933 2024-04-25 15:06:27.000000 modelbaker-1.7.3/modelbaker/ilitoppingmaker/ilidata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4743 2024-04-25 15:06:27.000000 modelbaker-1.7.3/modelbaker/ilitoppingmaker/iliprojecttopping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3266 2024-04-25 15:06:27.000000 modelbaker-1.7.3/modelbaker/ilitoppingmaker/ilitarget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6067 2024-04-25 15:06:27.000000 modelbaker-1.7.3/modelbaker/ilitoppingmaker/metaconfig.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:06:33.973567 modelbaker-1.7.3/modelbaker/iliwrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 15:06:27.000000 modelbaker-1.7.3/modelbaker/iliwrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-04-25 15:06:27.000000 modelbaker-1.7.3/modelbaker/iliwrapper/globals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4537 2024-04-25 15:06:27.000000 modelbaker-1.7.3/modelbaker/iliwrapper/ili2dbargs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16813 2024-04-25 15:06:27.000000 modelbaker-1.7.3/modelbaker/iliwrapper/ili2dbconfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2179 2024-04-25 15:06:27.000000 modelbaker-1.7.3/modelbaker/iliwrapper/ili2dbtools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13510 2024-04-25 15:06:27.000000 modelbaker-1.7.3/modelbaker/iliwrapper/ili2dbutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42200 2024-04-25 15:06:27.000000 modelbaker-1.7.3/modelbaker/iliwrapper/ilicache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6182 2024-04-25 15:06:27.000000 modelbaker-1.7.3/modelbaker/iliwrapper/iliexecutable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-04-25 15:06:27.000000 modelbaker-1.7.3/modelbaker/iliwrapper/iliexporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-04-25 15:06:27.000000 modelbaker-1.7.3/modelbaker/iliwrapper/iliimporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-04-25 15:06:27.000000 modelbaker-1.7.3/modelbaker/iliwrapper/iliupdater.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6192 2024-04-25 15:06:27.000000 modelbaker-1.7.3/modelbaker/iliwrapper/ilivalidator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:06:33.973567 modelbaker-1.7.3/modelbaker/libs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 15:06:30.000000 modelbaker-1.7.3/modelbaker/libs/__init__.py
+-rw-rw-r--   0 runner    (1001) docker     (127)    12895 2020-04-20 14:21:10.000000 modelbaker-1.7.3/modelbaker/libs/deprecation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:06:33.977567 modelbaker-1.7.3/modelbaker/libs/packaging/
+-rw-rw-r--   0 runner    (1001) docker     (127)      496 2024-03-10 09:38:56.000000 modelbaker-1.7.3/modelbaker/libs/packaging/__init__.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     3266 2023-01-30 15:29:48.000000 modelbaker-1.7.3/modelbaker/libs/packaging/_elffile.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     9590 2024-03-10 09:34:40.000000 modelbaker-1.7.3/modelbaker/libs/packaging/_manylinux.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     2676 2023-10-01 13:58:58.000000 modelbaker-1.7.3/modelbaker/libs/packaging/_musllinux.py
+-rw-rw-r--   0 runner    (1001) docker     (127)    10347 2024-03-10 09:34:40.000000 modelbaker-1.7.3/modelbaker/libs/packaging/_parser.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     1431 2023-01-30 15:29:48.000000 modelbaker-1.7.3/modelbaker/libs/packaging/_structures.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     5292 2023-04-12 17:05:06.000000 modelbaker-1.7.3/modelbaker/libs/packaging/_tokenizer.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     8208 2023-04-12 17:05:28.000000 modelbaker-1.7.3/modelbaker/libs/packaging/markers.py
+-rw-rw-r--   0 runner    (1001) docker     (127)    33036 2024-01-06 20:39:22.000000 modelbaker-1.7.3/modelbaker/libs/packaging/metadata.py
+-rw-rw-r--   0 runner    (1001) docker     (127)        0 2023-01-30 15:29:48.000000 modelbaker-1.7.3/modelbaker/libs/packaging/py.typed
+-rw-rw-r--   0 runner    (1001) docker     (127)     2933 2024-03-10 09:34:40.000000 modelbaker-1.7.3/modelbaker/libs/packaging/requirements.py
+-rw-rw-r--   0 runner    (1001) docker     (127)    39784 2024-03-10 09:34:40.000000 modelbaker-1.7.3/modelbaker/libs/packaging/specifiers.py
+-rw-rw-r--   0 runner    (1001) docker     (127)    18950 2024-01-06 20:39:22.000000 modelbaker-1.7.3/modelbaker/libs/packaging/tags.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     5268 2023-10-01 13:58:58.000000 modelbaker-1.7.3/modelbaker/libs/packaging/utils.py
+-rw-rw-r--   0 runner    (1001) docker     (127)    16236 2023-10-01 13:58:58.000000 modelbaker-1.7.3/modelbaker/libs/packaging/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:06:33.977567 modelbaker-1.7.3/modelbaker/libs/pgserviceparser/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1801 2022-06-27 10:25:36.000000 modelbaker-1.7.3/modelbaker/libs/pgserviceparser/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:06:33.977567 modelbaker-1.7.3/modelbaker/libs/toppingmaker/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1128 2023-12-13 05:24:38.000000 modelbaker-1.7.3/modelbaker/libs/toppingmaker/__init__.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     6550 2023-12-13 05:24:38.000000 modelbaker-1.7.3/modelbaker/libs/toppingmaker/exportsettings.py
+-rw-rw-r--   0 runner    (1001) docker     (127)    27294 2023-12-13 05:24:38.000000 modelbaker-1.7.3/modelbaker/libs/toppingmaker/projecttopping.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     3334 2023-12-13 05:24:38.000000 modelbaker-1.7.3/modelbaker/libs/toppingmaker/target.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     1297 2023-12-13 05:24:38.000000 modelbaker-1.7.3/modelbaker/libs/toppingmaker/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:06:33.977567 modelbaker-1.7.3/modelbaker/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 15:06:27.000000 modelbaker-1.7.3/modelbaker/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6460 2024-04-25 15:06:27.000000 modelbaker-1.7.3/modelbaker/utils/db_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-04-25 15:06:27.000000 modelbaker-1.7.3/modelbaker/utils/globals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9881 2024-04-25 15:06:27.000000 modelbaker-1.7.3/modelbaker/utils/qgis_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10267 2024-04-25 15:06:27.000000 modelbaker-1.7.3/modelbaker/utils/qt_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:06:33.985567 modelbaker-1.7.3/modelbaker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-04-25 15:06:33.000000 modelbaker-1.7.3/modelbaker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3725 2024-04-25 15:06:33.000000 modelbaker-1.7.3/modelbaker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 15:06:33.000000 modelbaker-1.7.3/modelbaker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-25 15:06:33.000000 modelbaker-1.7.3/modelbaker.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 15:06:33.985567 modelbaker-1.7.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-04-25 15:06:27.000000 modelbaker-1.7.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:06:33.981567 modelbaker-1.7.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    12962 2024-04-25 15:06:27.000000 modelbaker-1.7.3/tests/test_dataset_handling.py
+-rw-r--r--   0 runner    (1001) docker     (127)   151890 2024-04-25 15:06:27.000000 modelbaker-1.7.3/tests/test_domain_class_relations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2831 2024-04-25 15:06:27.000000 modelbaker-1.7.3/tests/test_dump.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39104 2024-04-25 15:06:27.000000 modelbaker-1.7.3/tests/test_export.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3425 2024-04-25 15:06:27.000000 modelbaker-1.7.3/tests/test_get_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6543 2024-04-25 15:06:27.000000 modelbaker-1.7.3/tests/test_gpkg_pk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2620 2024-04-25 15:06:27.000000 modelbaker-1.7.3/tests/test_ili2dbutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31704 2024-04-25 15:06:27.000000 modelbaker-1.7.3/tests/test_ilicache.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13620 2024-04-25 15:06:27.000000 modelbaker-1.7.3/tests/test_ilitoppingmaker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17928 2024-04-25 15:06:27.000000 modelbaker-1.7.3/tests/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-25 15:06:27.000000 modelbaker-1.7.3/tests/test_libili2pg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14531 2024-04-25 15:06:27.000000 modelbaker-1.7.3/tests/test_metaconfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11343 2024-04-25 15:06:27.000000 modelbaker-1.7.3/tests/test_pgservice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-25 15:06:27.000000 modelbaker-1.7.3/tests/test_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)   166557 2024-04-25 15:06:27.000000 modelbaker-1.7.3/tests/test_projectgen.py
+-rw-r--r--   0 runner    (1001) docker     (127)   111101 2024-04-25 15:06:27.000000 modelbaker-1.7.3/tests/test_projectgen_extension_optimization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15529 2024-04-25 15:06:27.000000 modelbaker-1.7.3/tests/test_projectgen_generic_databases.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40735 2024-04-25 15:06:27.000000 modelbaker-1.7.3/tests/test_projectgen_oids.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51641 2024-04-25 15:06:27.000000 modelbaker-1.7.3/tests/test_projecttopping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7594 2024-04-25 15:06:27.000000 modelbaker-1.7.3/tests/test_sequence_reset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5779 2024-04-25 15:06:27.000000 modelbaker-1.7.3/tests/test_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24379 2024-04-25 15:06:27.000000 modelbaker-1.7.3/tests/test_validate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-04-25 15:06:27.000000 modelbaker-1.7.3/tests/test_z_geom.py
```

### Comparing `modelbaker-1.7.2/LICENSE` & `modelbaker-1.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `modelbaker-1.7.2/PKG-INFO` & `modelbaker-1.7.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modelbaker
-Version: 1.7.2
+Version: 1.7.3
 Summary: The full model baker core
 Home-page: https://github.com/opengisch/QgisModelBakerLibrary
 Author: Dave Signer
 Author-email: david@opengis.ch
 Classifier: Topic :: Database
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Programming Language :: Python :: 3
```

### Comparing `modelbaker-1.7.2/README.md` & `modelbaker-1.7.3/README.md`

 * *Files identical despite different names*

### Comparing `modelbaker-1.7.2/modelbaker/dataobjects/fields.py` & `modelbaker-1.7.3/modelbaker/dataobjects/fields.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.7.2/modelbaker/dataobjects/form.py` & `modelbaker-1.7.3/modelbaker/dataobjects/form.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.7.2/modelbaker/dataobjects/layers.py` & `modelbaker-1.7.3/modelbaker/dataobjects/layers.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.7.2/modelbaker/dataobjects/legend.py` & `modelbaker-1.7.3/modelbaker/dataobjects/legend.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.7.2/modelbaker/dataobjects/project.py` & `modelbaker-1.7.3/modelbaker/dataobjects/project.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.7.2/modelbaker/dataobjects/relations.py` & `modelbaker-1.7.3/modelbaker/dataobjects/relations.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.7.2/modelbaker/db_factory/db_command_config_manager.py` & `modelbaker-1.7.3/modelbaker/db_factory/db_command_config_manager.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.7.2/modelbaker/db_factory/db_factory.py` & `modelbaker-1.7.3/modelbaker/db_factory/db_factory.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.7.2/modelbaker/db_factory/db_simple_factory.py` & `modelbaker-1.7.3/modelbaker/db_factory/db_simple_factory.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.7.2/modelbaker/db_factory/gpkg_command_config_manager.py` & `modelbaker-1.7.3/modelbaker/db_factory/gpkg_command_config_manager.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.7.2/modelbaker/db_factory/gpkg_factory.py` & `modelbaker-1.7.3/modelbaker/db_factory/gpkg_factory.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.7.2/modelbaker/db_factory/gpkg_layer_uri.py` & `modelbaker-1.7.3/modelbaker/db_factory/gpkg_layer_uri.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.7.2/modelbaker/db_factory/layer_uri.py` & `modelbaker-1.7.3/modelbaker/db_factory/layer_uri.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.7.2/modelbaker/db_factory/mssql_command_config_manager.py` & `modelbaker-1.7.3/modelbaker/db_factory/mssql_command_config_manager.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.7.2/modelbaker/db_factory/mssql_factory.py` & `modelbaker-1.7.3/modelbaker/db_factory/mssql_factory.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.7.2/modelbaker/db_factory/mssql_layer_uri.py` & `modelbaker-1.7.3/modelbaker/db_factory/mssql_layer_uri.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.7.2/modelbaker/db_factory/pg_command_config_manager.py` & `modelbaker-1.7.3/modelbaker/db_factory/pg_command_config_manager.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.7.2/modelbaker/db_factory/pg_factory.py` & `modelbaker-1.7.3/modelbaker/db_factory/pg_factory.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.7.2/modelbaker/db_factory/pg_layer_uri.py` & `modelbaker-1.7.3/modelbaker/db_factory/pg_layer_uri.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.7.2/modelbaker/dbconnector/config.py` & `modelbaker-1.7.3/modelbaker/dbconnector/config.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.7.2/modelbaker/dbconnector/db_connector.py` & `modelbaker-1.7.3/modelbaker/dbconnector/db_connector.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.7.2/modelbaker/dbconnector/gpkg_connector.py` & `modelbaker-1.7.3/modelbaker/dbconnector/gpkg_connector.py`

 * *Files 0% similar despite different names*

```diff
@@ -417,15 +417,19 @@
             ):  # e.g., t_id's don't have a fully qualified name
                 attr_order_found = False
                 attr_mapping_found = False
                 for meta_attr in meta_attrs:
                     if record["fully_qualified_name"] != meta_attr["ilielement"]:
                         continue
 
-                    if meta_attr["attr_name"] == "form_order":
+                    if meta_attr["attr_name"] in [
+                        "form_order",  # obsolete
+                        "qgis.modelbaker.form_order",  # obsolete
+                        "qgis.modelbaker.formOrder",
+                    ]:
                         record["attr_order"] = meta_attr["attr_value"]
                         attr_order_found = True
 
                     if meta_attr["attr_name"] == "ili2db.mapping":
                         record["attr_mapping"] = meta_attr["attr_value"]
                         attr_mapping_found = True
```

### Comparing `modelbaker-1.7.2/modelbaker/dbconnector/mssql_connector.py` & `modelbaker-1.7.3/modelbaker/dbconnector/mssql_connector.py`

 * *Files 0% similar despite different names*

```diff
@@ -533,15 +533,18 @@
                 stmt += (
                     ln + "    AND LOWER(c.column_name) = LOWER(oid_domain.columnname)"
                 )
                 stmt += ln + "    AND oid_domain.tag = 'ch.ehi.ili2db.oidDomain'"
                 if metaattrs_exists:
                     stmt += ln + "LEFT JOIN {schema}.t_ili2db_meta_attrs form_order"
                     stmt += ln + "    ON full_name.iliname=form_order.ilielement AND"
-                    stmt += ln + "    form_order.attr_name='form_order'"
+                    stmt += ln + "    form_order.attr_name IN ("
+                    stmt += ln + "        'form_order',"  # obsolete
+                    stmt += ln + "        'qgis.modelbaker.form_order',"  # obsolete
+                    stmt += ln + "        'qgis.modelbaker.formOrder')"
                     stmt += ln + "LEFT JOIN {schema}.t_ili2db_meta_attrs attr_mapping"
                     stmt += ln + "    ON full_name.iliname=attr_mapping.ilielement AND"
                     stmt += ln + "    attr_mapping.attr_name='ili2db.mapping'"
             stmt += ln + "WHERE TABLE_NAME = '{table}' AND TABLE_SCHEMA = '{schema}'"
             if metadata_exists and metaattrs_exists:
                 stmt += ln + "ORDER BY attr_order;"
             stmt = stmt.format(schema=self.schema, table=table_name)
```

### Comparing `modelbaker-1.7.2/modelbaker/dbconnector/pg_connector.py` & `modelbaker-1.7.3/modelbaker/dbconnector/pg_connector.py`

 * *Files 0% similar despite different names*

```diff
@@ -486,15 +486,18 @@
                                                     oid_domain.tag = 'ch.ehi.ili2db.oidDomain'""".format(
                     self.schema
                 )
                 if self._table_exists(PG_METAATTRS_TABLE):
                     attr_order_field = "COALESCE(to_number(form_order.attr_value, '999'), 999) as attr_order,"
                     attr_order_join = """LEFT JOIN {schema}.{t_ili2db_meta_attrs} form_order
                                                             ON full_name.iliname=form_order.ilielement AND
-                                                            form_order.attr_name='form_order'
+                                                            form_order.attr_name IN (
+                                                                'form_order', --obsolete
+                                                                'qgis.modelbaker.form_order', --obsolete
+                                                                'qgis.modelbaker.formOrder')
                                                             """.format(
                         schema=self.schema, t_ili2db_meta_attrs=PG_METAATTRS_TABLE
                     )
                     order_by_attr_order = """ORDER BY attr_order"""
 
                     attr_mapping_field = (
                         "meta_attr_mapping_value.attr_value as attr_mapping,"
```

### Comparing `modelbaker-1.7.2/modelbaker/generator/config.py` & `modelbaker-1.7.3/modelbaker/generator/config.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.7.2/modelbaker/generator/domain_relations_generator.py` & `modelbaker-1.7.3/modelbaker/generator/domain_relations_generator.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.7.2/modelbaker/generator/generator.py` & `modelbaker-1.7.3/modelbaker/generator/generator.py`

 * *Files 0% similar despite different names*

```diff
@@ -230,15 +230,15 @@
                     tilitid=self._db_connector.tilitid,
                     dataset_layer_name=self._db_connector.dataset_table_name,
                 )
             elif "ili_name" in record and record["ili_name"]:
                 meta_attrs = self.get_meta_attrs(record["ili_name"])
                 for attr_record in meta_attrs:
                     if attr_record["attr_name"] in [
-                        "dispExpression",
+                        "dispExpression",  # obsolete
                         "qgis.modelbaker.dispExpression",
                     ]:
                         display_expression = attr_record["attr_value"]
 
             coord_decimals = (
                 record["coord_decimals"] if "coord_decimals" in record else None
             )
```

### Comparing `modelbaker-1.7.2/modelbaker/ilitoppingmaker/__init__.py` & `modelbaker-1.7.3/modelbaker/ilitoppingmaker/__init__.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.7.2/modelbaker/ilitoppingmaker/ili2dbsettings.py` & `modelbaker-1.7.3/modelbaker/ilitoppingmaker/ili2dbsettings.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.7.2/modelbaker/ilitoppingmaker/ilidata.py` & `modelbaker-1.7.3/modelbaker/ilitoppingmaker/ilidata.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.7.2/modelbaker/ilitoppingmaker/iliprojecttopping.py` & `modelbaker-1.7.3/modelbaker/ilitoppingmaker/iliprojecttopping.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.7.2/modelbaker/ilitoppingmaker/ilitarget.py` & `modelbaker-1.7.3/modelbaker/ilitoppingmaker/ilitarget.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.7.2/modelbaker/ilitoppingmaker/metaconfig.py` & `modelbaker-1.7.3/modelbaker/ilitoppingmaker/metaconfig.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.7.2/modelbaker/iliwrapper/globals.py` & `modelbaker-1.7.3/modelbaker/iliwrapper/globals.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.7.2/modelbaker/iliwrapper/ili2dbargs.py` & `modelbaker-1.7.3/modelbaker/iliwrapper/ili2dbargs.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.7.2/modelbaker/iliwrapper/ili2dbconfig.py` & `modelbaker-1.7.3/modelbaker/iliwrapper/ili2dbconfig.py`

 * *Files 0% similar despite different names*

```diff
@@ -248,15 +248,14 @@
 
         if with_action:
             self.append_args(args, ["--schemaimport"], force_append=True)
 
         self.append_args(args, extra_args, force_append=True)
 
         self.append_args(args, ["--coalesceCatalogueRef"], True)
-        self.append_args(args, ["--createEnumTabs"], True)
 
         if self.disable_validation:
             self.append_args(args, ["--sqlEnableNull"], force_append=True)
             self.append_args(args, ["--sqlColsAsText"], force_append=True)
         else:
             self.append_args(args, ["--createNumChecks"], True)
             self.append_args(args, ["--createUnique"], True)
@@ -272,18 +271,19 @@
         self.append_args(args, ["--createMetaInfo"], True)
         self.append_args(args, ["--expandMultilingual"], True)
 
         if self.db_ili_version is None or self.db_ili_version > 3:
             self.append_args(args, ["--createTypeConstraint"], True)
             self.append_args(args, ["--createEnumTabsWithId"], True)
             self.append_args(args, ["--createTidCol"], True)
-
-        # version 3 backwards compatibility (not needed in newer versions)
-        if self.create_import_tid:
-            self.append_args(args, ["--importTid"])
+        else:
+            # version 3 backwards compatibility (not needed in newer versions)
+            self.append_args(args, ["--createEnumTabs"], True)
+            if self.create_import_tid:
+                self.append_args(args, ["--importTid"])
 
         if self.inheritance == "smart1":
             self.append_args(args, ["--smart1Inheritance"])
         elif self.inheritance == "smart2":
             self.append_args(args, ["--smart2Inheritance"])
         else:
             self.append_args(args, ["--noSmartMapping"])
```

### Comparing `modelbaker-1.7.2/modelbaker/iliwrapper/ili2dbtools.py` & `modelbaker-1.7.3/modelbaker/iliwrapper/ili2dbtools.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.7.2/modelbaker/iliwrapper/ili2dbutils.py` & `modelbaker-1.7.3/modelbaker/iliwrapper/ili2dbutils.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.7.2/modelbaker/iliwrapper/ilicache.py` & `modelbaker-1.7.3/modelbaker/iliwrapper/ilicache.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.7.2/modelbaker/iliwrapper/iliexecutable.py` & `modelbaker-1.7.3/modelbaker/iliwrapper/iliexecutable.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.7.2/modelbaker/iliwrapper/iliexporter.py` & `modelbaker-1.7.3/modelbaker/iliwrapper/iliexporter.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.7.2/modelbaker/iliwrapper/iliimporter.py` & `modelbaker-1.7.3/modelbaker/iliwrapper/iliimporter.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.7.2/modelbaker/iliwrapper/iliupdater.py` & `modelbaker-1.7.3/modelbaker/iliwrapper/iliupdater.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.7.2/modelbaker/iliwrapper/ilivalidator.py` & `modelbaker-1.7.3/modelbaker/iliwrapper/ilivalidator.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.7.2/modelbaker/libs/deprecation.py` & `modelbaker-1.7.3/modelbaker/libs/deprecation.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.7.2/modelbaker/libs/packaging/_elffile.py` & `modelbaker-1.7.3/modelbaker/libs/packaging/_elffile.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.7.2/modelbaker/libs/packaging/_manylinux.py` & `modelbaker-1.7.3/modelbaker/libs/packaging/_manylinux.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.7.2/modelbaker/libs/packaging/_musllinux.py` & `modelbaker-1.7.3/modelbaker/libs/packaging/_musllinux.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.7.2/modelbaker/libs/packaging/_parser.py` & `modelbaker-1.7.3/modelbaker/libs/packaging/_parser.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.7.2/modelbaker/libs/packaging/_structures.py` & `modelbaker-1.7.3/modelbaker/libs/packaging/_structures.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.7.2/modelbaker/libs/packaging/_tokenizer.py` & `modelbaker-1.7.3/modelbaker/libs/packaging/_tokenizer.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.7.2/modelbaker/libs/packaging/markers.py` & `modelbaker-1.7.3/modelbaker/libs/packaging/markers.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.7.2/modelbaker/libs/packaging/metadata.py` & `modelbaker-1.7.3/modelbaker/libs/packaging/metadata.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.7.2/modelbaker/libs/packaging/requirements.py` & `modelbaker-1.7.3/modelbaker/libs/packaging/requirements.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.7.2/modelbaker/libs/packaging/specifiers.py` & `modelbaker-1.7.3/modelbaker/libs/packaging/specifiers.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.7.2/modelbaker/libs/packaging/tags.py` & `modelbaker-1.7.3/modelbaker/libs/packaging/tags.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.7.2/modelbaker/libs/packaging/utils.py` & `modelbaker-1.7.3/modelbaker/libs/packaging/utils.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.7.2/modelbaker/libs/packaging/version.py` & `modelbaker-1.7.3/modelbaker/libs/packaging/version.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.7.2/modelbaker/libs/pgserviceparser/__init__.py` & `modelbaker-1.7.3/modelbaker/libs/pgserviceparser/__init__.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.7.2/modelbaker/libs/toppingmaker/__init__.py` & `modelbaker-1.7.3/modelbaker/libs/toppingmaker/__init__.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.7.2/modelbaker/libs/toppingmaker/exportsettings.py` & `modelbaker-1.7.3/modelbaker/libs/toppingmaker/exportsettings.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.7.2/modelbaker/libs/toppingmaker/projecttopping.py` & `modelbaker-1.7.3/modelbaker/libs/toppingmaker/projecttopping.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.7.2/modelbaker/libs/toppingmaker/target.py` & `modelbaker-1.7.3/modelbaker/libs/toppingmaker/target.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.7.2/modelbaker/libs/toppingmaker/utils.py` & `modelbaker-1.7.3/modelbaker/libs/toppingmaker/utils.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.7.2/modelbaker/utils/db_utils.py` & `modelbaker-1.7.3/modelbaker/utils/db_utils.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.7.2/modelbaker/utils/globals.py` & `modelbaker-1.7.3/modelbaker/utils/globals.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.7.2/modelbaker/utils/qgis_utils.py` & `modelbaker-1.7.3/modelbaker/utils/qgis_utils.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.7.2/modelbaker/utils/qt_utils.py` & `modelbaker-1.7.3/modelbaker/utils/qt_utils.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.7.2/modelbaker.egg-info/PKG-INFO` & `modelbaker-1.7.3/modelbaker.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modelbaker
-Version: 1.7.2
+Version: 1.7.3
 Summary: The full model baker core
 Home-page: https://github.com/opengisch/QgisModelBakerLibrary
 Author: Dave Signer
 Author-email: david@opengis.ch
 Classifier: Topic :: Database
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Programming Language :: Python :: 3
```

### Comparing `modelbaker-1.7.2/modelbaker.egg-info/SOURCES.txt` & `modelbaker-1.7.3/modelbaker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `modelbaker-1.7.2/setup.py` & `modelbaker-1.7.3/setup.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.7.2/tests/test_dataset_handling.py` & `modelbaker-1.7.3/tests/test_dataset_handling.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.7.2/tests/test_domain_class_relations.py` & `modelbaker-1.7.3/tests/test_domain_class_relations.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.7.2/tests/test_dump.py` & `modelbaker-1.7.3/tests/test_dump.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.7.2/tests/test_export.py` & `modelbaker-1.7.3/tests/test_export.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.7.2/tests/test_get_models.py` & `modelbaker-1.7.3/tests/test_get_models.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.7.2/tests/test_gpkg_pk.py` & `modelbaker-1.7.3/tests/test_gpkg_pk.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.7.2/tests/test_ili2dbutils.py` & `modelbaker-1.7.3/tests/test_ili2dbutils.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.7.2/tests/test_ilicache.py` & `modelbaker-1.7.3/tests/test_ilicache.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.7.2/tests/test_ilitoppingmaker.py` & `modelbaker-1.7.3/tests/test_ilitoppingmaker.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.7.2/tests/test_import.py` & `modelbaker-1.7.3/tests/test_import.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.7.2/tests/test_libili2pg.py` & `modelbaker-1.7.3/tests/test_libili2pg.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.7.2/tests/test_metaconfig.py` & `modelbaker-1.7.3/tests/test_metaconfig.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.7.2/tests/test_pgservice.py` & `modelbaker-1.7.3/tests/test_pgservice.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.7.2/tests/test_plugin.py` & `modelbaker-1.7.3/tests/test_plugin.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.7.2/tests/test_projectgen.py` & `modelbaker-1.7.3/tests/test_projectgen.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.7.2/tests/test_projectgen_extension_optimization.py` & `modelbaker-1.7.3/tests/test_projectgen_extension_optimization.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.7.2/tests/test_projectgen_generic_databases.py` & `modelbaker-1.7.3/tests/test_projectgen_generic_databases.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.7.2/tests/test_projectgen_oids.py` & `modelbaker-1.7.3/tests/test_projectgen_oids.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.7.2/tests/test_projecttopping.py` & `modelbaker-1.7.3/tests/test_projecttopping.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.7.2/tests/test_sequence_reset.py` & `modelbaker-1.7.3/tests/test_sequence_reset.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.7.2/tests/test_update.py` & `modelbaker-1.7.3/tests/test_update.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.7.2/tests/test_validate.py` & `modelbaker-1.7.3/tests/test_validate.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.7.2/tests/test_z_geom.py` & `modelbaker-1.7.3/tests/test_z_geom.py`

 * *Files identical despite different names*


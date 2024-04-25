# Comparing `tmp/threedigrid-2.2.7.tar.gz` & `tmp/threedigrid-2.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "threedigrid-2.2.7.tar", last modified: Mon Apr 22 11:45:49 2024, max compression
+gzip compressed data, was "threedigrid-2.2.8.tar", last modified: Thu Apr 25 12:14:17 2024, max compression
```

## Comparing `threedigrid-2.2.7.tar` & `threedigrid-2.2.8.tar`

### file list

```diff
@@ -1,131 +1,131 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 11:45:49.710623 threedigrid-2.2.7/
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-22 11:45:45.000000 threedigrid-2.2.7/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3527 2024-04-22 11:45:45.000000 threedigrid-2.2.7/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)    18568 2024-04-22 11:45:45.000000 threedigrid-2.2.7/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-04-22 11:45:45.000000 threedigrid-2.2.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-22 11:45:45.000000 threedigrid-2.2.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    24439 2024-04-22 11:45:49.710623 threedigrid-2.2.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4682 2024-04-22 11:45:45.000000 threedigrid-2.2.7/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 11:45:49.690623 threedigrid-2.2.7/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-22 11:45:45.000000 threedigrid-2.2.7/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     7522 2024-04-22 11:45:45.000000 threedigrid-2.2.7/docs/aggregate_results.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-22 11:45:45.000000 threedigrid-2.2.7/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-22 11:45:45.000000 threedigrid-2.2.7/docs/files.rst
--rw-r--r--   0 runner    (1001) docker     (127)     8338 2024-04-22 11:45:45.000000 threedigrid-2.2.7/docs/functionalities.rst
--rw-r--r--   0 runner    (1001) docker     (127)    37537 2024-04-22 11:45:45.000000 threedigrid-2.2.7/docs/gridadmin.rst
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-22 11:45:45.000000 threedigrid-2.2.7/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-22 11:45:45.000000 threedigrid-2.2.7/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2400 2024-04-22 11:45:45.000000 threedigrid-2.2.7/docs/introduction.rst
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-22 11:45:45.000000 threedigrid-2.2.7/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)     4691 2024-04-22 11:45:45.000000 threedigrid-2.2.7/docs/results.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3432 2024-04-22 11:45:45.000000 threedigrid-2.2.7/docs/structure_control.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-04-22 11:45:45.000000 threedigrid-2.2.7/docs/water_quality_results.rst
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-22 11:45:49.710623 threedigrid-2.2.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-04-22 11:45:45.000000 threedigrid-2.2.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 11:45:49.694623 threedigrid-2.2.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     6510 2024-04-22 11:45:45.000000 threedigrid-2.2.7/tests/test_aggregateresultadmin.py
--rw-r--r--   0 runner    (1001) docker     (127)     5987 2024-04-22 11:45:45.000000 threedigrid-2.2.7/tests/test_exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     7345 2024-04-22 11:45:46.000000 threedigrid-2.2.7/tests/test_filters.py
--rw-r--r--   0 runner    (1001) docker     (127)    21148 2024-04-22 11:45:46.000000 threedigrid-2.2.7/tests/test_gridadmin.py
--rw-r--r--   0 runner    (1001) docker     (127)     7139 2024-04-22 11:45:46.000000 threedigrid-2.2.7/tests/test_gridresultadmin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-04-22 11:45:46.000000 threedigrid-2.2.7/tests/test_id_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-04-22 11:45:46.000000 threedigrid-2.2.7/tests/test_management.py
--rw-r--r--   0 runner    (1001) docker     (127)     2596 2024-04-22 11:45:46.000000 threedigrid-2.2.7/tests/test_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)     2473 2024-04-22 11:45:46.000000 threedigrid-2.2.7/tests/test_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     3990 2024-04-22 11:45:46.000000 threedigrid-2.2.7/tests/test_prepare.py
--rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-04-22 11:45:46.000000 threedigrid-2.2.7/tests/test_prepare_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4005 2024-04-22 11:45:46.000000 threedigrid-2.2.7/tests/test_structure_controls.py
--rw-r--r--   0 runner    (1001) docker     (127)     3665 2024-04-22 11:45:46.000000 threedigrid-2.2.7/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 11:45:49.694623 threedigrid-2.2.7/threedigrid/
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-22 11:45:46.000000 threedigrid-2.2.7/threedigrid/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 11:45:49.698623 threedigrid-2.2.7/threedigrid/admin/
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-22 11:45:46.000000 threedigrid-2.2.7/threedigrid/admin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 11:45:49.698623 threedigrid-2.2.7/threedigrid/admin/breaches/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 11:45:46.000000 threedigrid-2.2.7/threedigrid/admin/breaches/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3617 2024-04-22 11:45:46.000000 threedigrid-2.2.7/threedigrid/admin/breaches/exporters.py
--rw-r--r--   0 runner    (1001) docker     (127)     2881 2024-04-22 11:45:46.000000 threedigrid-2.2.7/threedigrid/admin/breaches/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     3118 2024-04-22 11:45:46.000000 threedigrid-2.2.7/threedigrid/admin/breaches/prepare.py
--rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-04-22 11:45:46.000000 threedigrid-2.2.7/threedigrid/admin/breaches/timeseries_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     6762 2024-04-22 11:45:46.000000 threedigrid-2.2.7/threedigrid/admin/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 11:45:49.698623 threedigrid-2.2.7/threedigrid/admin/crosssections/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 11:45:46.000000 threedigrid-2.2.7/threedigrid/admin/crosssections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1710 2024-04-22 11:45:46.000000 threedigrid-2.2.7/threedigrid/admin/crosssections/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     4039 2024-04-22 11:45:46.000000 threedigrid-2.2.7/threedigrid/admin/exporter_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 11:45:49.698623 threedigrid-2.2.7/threedigrid/admin/exporters/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 11:45:46.000000 threedigrid-2.2.7/threedigrid/admin/exporters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 11:45:49.698623 threedigrid-2.2.7/threedigrid/admin/exporters/geopackage/
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-22 11:45:46.000000 threedigrid-2.2.7/threedigrid/admin/exporters/geopackage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4553 2024-04-22 11:45:46.000000 threedigrid-2.2.7/threedigrid/admin/exporters/geopackage/default.py
--rw-r--r--   0 runner    (1001) docker     (127)     7484 2024-04-22 11:45:46.000000 threedigrid-2.2.7/threedigrid/admin/exporters/geopackage/exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     9428 2024-04-22 11:45:46.000000 threedigrid-2.2.7/threedigrid/admin/gridadmin.py
--rw-r--r--   0 runner    (1001) docker     (127)    21782 2024-04-22 11:45:46.000000 threedigrid-2.2.7/threedigrid/admin/gridresultadmin.py
--rw-r--r--   0 runner    (1001) docker     (127)     8063 2024-04-22 11:45:46.000000 threedigrid-2.2.7/threedigrid/admin/h5py_datasource.py
--rw-r--r--   0 runner    (1001) docker     (127)      958 2024-04-22 11:45:46.000000 threedigrid-2.2.7/threedigrid/admin/h5py_swmr.py
--rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-04-22 11:45:46.000000 threedigrid-2.2.7/threedigrid/admin/idmapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 11:45:49.698623 threedigrid-2.2.7/threedigrid/admin/levees/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 11:45:46.000000 threedigrid-2.2.7/threedigrid/admin/levees/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-04-22 11:45:46.000000 threedigrid-2.2.7/threedigrid/admin/levees/exporters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-04-22 11:45:46.000000 threedigrid-2.2.7/threedigrid/admin/levees/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-04-22 11:45:46.000000 threedigrid-2.2.7/threedigrid/admin/levees/prepare.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 11:45:49.702623 threedigrid-2.2.7/threedigrid/admin/lines/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 11:45:46.000000 threedigrid-2.2.7/threedigrid/admin/lines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4270 2024-04-22 11:45:46.000000 threedigrid-2.2.7/threedigrid/admin/lines/exporters.py
--rw-r--r--   0 runner    (1001) docker     (127)     7215 2024-04-22 11:45:46.000000 threedigrid-2.2.7/threedigrid/admin/lines/models.py
--rw-r--r--   0 runner    (1001) docker     (127)    16777 2024-04-22 11:45:46.000000 threedigrid-2.2.7/threedigrid/admin/lines/prepare.py
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-22 11:45:46.000000 threedigrid-2.2.7/threedigrid/admin/lines/subsets.py
--rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-04-22 11:45:46.000000 threedigrid-2.2.7/threedigrid/admin/lines/timeseries_mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 11:45:49.702623 threedigrid-2.2.7/threedigrid/admin/nodes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 11:45:46.000000 threedigrid-2.2.7/threedigrid/admin/nodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5261 2024-04-22 11:45:46.000000 threedigrid-2.2.7/threedigrid/admin/nodes/exporters.py
--rw-r--r--   0 runner    (1001) docker     (127)    12288 2024-04-22 11:45:46.000000 threedigrid-2.2.7/threedigrid/admin/nodes/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     5316 2024-04-22 11:45:46.000000 threedigrid-2.2.7/threedigrid/admin/nodes/prepare.py
--rw-r--r--   0 runner    (1001) docker     (127)      961 2024-04-22 11:45:46.000000 threedigrid-2.2.7/threedigrid/admin/nodes/subsets.py
--rw-r--r--   0 runner    (1001) docker     (127)     4955 2024-04-22 11:45:46.000000 threedigrid-2.2.7/threedigrid/admin/nodes/timeseries_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)    20857 2024-04-22 11:45:46.000000 threedigrid-2.2.7/threedigrid/admin/prepare.py
--rw-r--r--   0 runner    (1001) docker     (127)     2731 2024-04-22 11:45:46.000000 threedigrid-2.2.7/threedigrid/admin/prepare_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 11:45:49.702623 threedigrid-2.2.7/threedigrid/admin/pumps/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 11:45:46.000000 threedigrid-2.2.7/threedigrid/admin/pumps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-04-22 11:45:46.000000 threedigrid-2.2.7/threedigrid/admin/pumps/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     4304 2024-04-22 11:45:46.000000 threedigrid-2.2.7/threedigrid/admin/pumps/prepare.py
--rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-04-22 11:45:46.000000 threedigrid-2.2.7/threedigrid/admin/pumps/timeseries_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     8926 2024-04-22 11:45:46.000000 threedigrid-2.2.7/threedigrid/admin/rpc_datasource.py
--rw-r--r--   0 runner    (1001) docker     (127)    10057 2024-04-22 11:45:46.000000 threedigrid-2.2.7/threedigrid/admin/serializers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 11:45:49.702623 threedigrid-2.2.7/threedigrid/admin/structure_controls/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 11:45:46.000000 threedigrid-2.2.7/threedigrid/admin/structure_controls/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-04-22 11:45:46.000000 threedigrid-2.2.7/threedigrid/admin/structure_controls/exporters.py
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-22 11:45:46.000000 threedigrid-2.2.7/threedigrid/admin/structure_controls/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     7474 2024-04-22 11:45:46.000000 threedigrid-2.2.7/threedigrid/admin/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10204 2024-04-22 11:45:46.000000 threedigrid-2.2.7/threedigrid/geo_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 11:45:49.702623 threedigrid-2.2.7/threedigrid/management/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 11:45:46.000000 threedigrid-2.2.7/threedigrid/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 11:45:49.702623 threedigrid-2.2.7/threedigrid/management/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 11:45:46.000000 threedigrid-2.2.7/threedigrid/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-04-22 11:45:46.000000 threedigrid-2.2.7/threedigrid/management/commands/kick.py
--rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-04-22 11:45:46.000000 threedigrid-2.2.7/threedigrid/management/help_texts.py
--rw-r--r--   0 runner    (1001) docker     (127)     9564 2024-04-22 11:45:46.000000 threedigrid-2.2.7/threedigrid/numpy_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 11:45:49.706623 threedigrid-2.2.7/threedigrid/orm/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 11:45:46.000000 threedigrid-2.2.7/threedigrid/orm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 11:45:49.706623 threedigrid-2.2.7/threedigrid/orm/base/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 11:45:46.000000 threedigrid-2.2.7/threedigrid/orm/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      947 2024-04-22 11:45:46.000000 threedigrid-2.2.7/threedigrid/orm/base/datasource.py
--rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-22 11:45:46.000000 threedigrid-2.2.7/threedigrid/orm/base/encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-22 11:45:46.000000 threedigrid-2.2.7/threedigrid/orm/base/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2396 2024-04-22 11:45:46.000000 threedigrid-2.2.7/threedigrid/orm/base/exporters.py
--rw-r--r--   0 runner    (1001) docker     (127)     8744 2024-04-22 11:45:46.000000 threedigrid-2.2.7/threedigrid/orm/base/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     6511 2024-04-22 11:45:46.000000 threedigrid-2.2.7/threedigrid/orm/base/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)    17964 2024-04-22 11:45:46.000000 threedigrid-2.2.7/threedigrid/orm/base/models.py
--rw-r--r--   0 runner    (1001) docker     (127)    11698 2024-04-22 11:45:46.000000 threedigrid-2.2.7/threedigrid/orm/base/options.py
--rw-r--r--   0 runner    (1001) docker     (127)    16216 2024-04-22 11:45:46.000000 threedigrid-2.2.7/threedigrid/orm/base/timeseries_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-22 11:45:46.000000 threedigrid-2.2.7/threedigrid/orm/base/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-04-22 11:45:46.000000 threedigrid-2.2.7/threedigrid/orm/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     8933 2024-04-22 11:45:46.000000 threedigrid-2.2.7/threedigrid/orm/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     5047 2024-04-22 11:45:46.000000 threedigrid-2.2.7/threedigrid/orm/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     5530 2024-04-22 11:45:46.000000 threedigrid-2.2.7/threedigrid/orm/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 11:45:49.706623 threedigrid-2.2.7/threedigrid.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    24439 2024-04-22 11:45:49.000000 threedigrid-2.2.7/threedigrid.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3442 2024-04-22 11:45:49.000000 threedigrid-2.2.7/threedigrid.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 11:45:49.000000 threedigrid-2.2.7/threedigrid.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-22 11:45:49.000000 threedigrid-2.2.7/threedigrid.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 11:45:49.000000 threedigrid-2.2.7/threedigrid.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-22 11:45:49.000000 threedigrid-2.2.7/threedigrid.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-22 11:45:49.000000 threedigrid-2.2.7/threedigrid.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:14:17.452208 threedigrid-2.2.8/
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-25 12:14:13.000000 threedigrid-2.2.8/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3527 2024-04-25 12:14:13.000000 threedigrid-2.2.8/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    18666 2024-04-25 12:14:13.000000 threedigrid-2.2.8/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-04-25 12:14:13.000000 threedigrid-2.2.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-25 12:14:13.000000 threedigrid-2.2.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    24537 2024-04-25 12:14:17.452208 threedigrid-2.2.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4682 2024-04-25 12:14:13.000000 threedigrid-2.2.8/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:14:17.436207 threedigrid-2.2.8/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-25 12:14:13.000000 threedigrid-2.2.8/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     7522 2024-04-25 12:14:13.000000 threedigrid-2.2.8/docs/aggregate_results.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-25 12:14:13.000000 threedigrid-2.2.8/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-25 12:14:13.000000 threedigrid-2.2.8/docs/files.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8338 2024-04-25 12:14:13.000000 threedigrid-2.2.8/docs/functionalities.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    37537 2024-04-25 12:14:13.000000 threedigrid-2.2.8/docs/gridadmin.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-25 12:14:13.000000 threedigrid-2.2.8/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-25 12:14:13.000000 threedigrid-2.2.8/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2400 2024-04-25 12:14:13.000000 threedigrid-2.2.8/docs/introduction.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-25 12:14:13.000000 threedigrid-2.2.8/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)     4691 2024-04-25 12:14:13.000000 threedigrid-2.2.8/docs/results.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3432 2024-04-25 12:14:13.000000 threedigrid-2.2.8/docs/structure_control.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-04-25 12:14:13.000000 threedigrid-2.2.8/docs/water_quality_results.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-25 12:14:17.456208 threedigrid-2.2.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-04-25 12:14:13.000000 threedigrid-2.2.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:14:17.440208 threedigrid-2.2.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     6510 2024-04-25 12:14:13.000000 threedigrid-2.2.8/tests/test_aggregateresultadmin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5987 2024-04-25 12:14:13.000000 threedigrid-2.2.8/tests/test_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7345 2024-04-25 12:14:14.000000 threedigrid-2.2.8/tests/test_filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21148 2024-04-25 12:14:14.000000 threedigrid-2.2.8/tests/test_gridadmin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7139 2024-04-25 12:14:14.000000 threedigrid-2.2.8/tests/test_gridresultadmin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-04-25 12:14:14.000000 threedigrid-2.2.8/tests/test_id_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-04-25 12:14:14.000000 threedigrid-2.2.8/tests/test_management.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2596 2024-04-25 12:14:14.000000 threedigrid-2.2.8/tests/test_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2473 2024-04-25 12:14:14.000000 threedigrid-2.2.8/tests/test_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3990 2024-04-25 12:14:14.000000 threedigrid-2.2.8/tests/test_prepare.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-04-25 12:14:14.000000 threedigrid-2.2.8/tests/test_prepare_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4005 2024-04-25 12:14:14.000000 threedigrid-2.2.8/tests/test_structure_controls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3665 2024-04-25 12:14:14.000000 threedigrid-2.2.8/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:14:17.440208 threedigrid-2.2.8/threedigrid/
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-25 12:14:14.000000 threedigrid-2.2.8/threedigrid/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:14:17.444208 threedigrid-2.2.8/threedigrid/admin/
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-25 12:14:14.000000 threedigrid-2.2.8/threedigrid/admin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:14:17.444208 threedigrid-2.2.8/threedigrid/admin/breaches/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 12:14:14.000000 threedigrid-2.2.8/threedigrid/admin/breaches/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3617 2024-04-25 12:14:14.000000 threedigrid-2.2.8/threedigrid/admin/breaches/exporters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2881 2024-04-25 12:14:14.000000 threedigrid-2.2.8/threedigrid/admin/breaches/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3118 2024-04-25 12:14:14.000000 threedigrid-2.2.8/threedigrid/admin/breaches/prepare.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-04-25 12:14:14.000000 threedigrid-2.2.8/threedigrid/admin/breaches/timeseries_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6762 2024-04-25 12:14:14.000000 threedigrid-2.2.8/threedigrid/admin/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:14:17.444208 threedigrid-2.2.8/threedigrid/admin/crosssections/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 12:14:14.000000 threedigrid-2.2.8/threedigrid/admin/crosssections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1710 2024-04-25 12:14:14.000000 threedigrid-2.2.8/threedigrid/admin/crosssections/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4039 2024-04-25 12:14:14.000000 threedigrid-2.2.8/threedigrid/admin/exporter_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:14:17.444208 threedigrid-2.2.8/threedigrid/admin/exporters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 12:14:14.000000 threedigrid-2.2.8/threedigrid/admin/exporters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:14:17.444208 threedigrid-2.2.8/threedigrid/admin/exporters/geopackage/
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-25 12:14:14.000000 threedigrid-2.2.8/threedigrid/admin/exporters/geopackage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4553 2024-04-25 12:14:14.000000 threedigrid-2.2.8/threedigrid/admin/exporters/geopackage/default.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7484 2024-04-25 12:14:14.000000 threedigrid-2.2.8/threedigrid/admin/exporters/geopackage/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9428 2024-04-25 12:14:14.000000 threedigrid-2.2.8/threedigrid/admin/gridadmin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22034 2024-04-25 12:14:14.000000 threedigrid-2.2.8/threedigrid/admin/gridresultadmin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8063 2024-04-25 12:14:14.000000 threedigrid-2.2.8/threedigrid/admin/h5py_datasource.py
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-04-25 12:14:14.000000 threedigrid-2.2.8/threedigrid/admin/h5py_swmr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-04-25 12:14:14.000000 threedigrid-2.2.8/threedigrid/admin/idmapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:14:17.444208 threedigrid-2.2.8/threedigrid/admin/levees/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 12:14:14.000000 threedigrid-2.2.8/threedigrid/admin/levees/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-04-25 12:14:14.000000 threedigrid-2.2.8/threedigrid/admin/levees/exporters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-04-25 12:14:14.000000 threedigrid-2.2.8/threedigrid/admin/levees/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-04-25 12:14:14.000000 threedigrid-2.2.8/threedigrid/admin/levees/prepare.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:14:17.448208 threedigrid-2.2.8/threedigrid/admin/lines/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 12:14:14.000000 threedigrid-2.2.8/threedigrid/admin/lines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4270 2024-04-25 12:14:14.000000 threedigrid-2.2.8/threedigrid/admin/lines/exporters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7215 2024-04-25 12:14:14.000000 threedigrid-2.2.8/threedigrid/admin/lines/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16777 2024-04-25 12:14:14.000000 threedigrid-2.2.8/threedigrid/admin/lines/prepare.py
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-25 12:14:14.000000 threedigrid-2.2.8/threedigrid/admin/lines/subsets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-04-25 12:14:14.000000 threedigrid-2.2.8/threedigrid/admin/lines/timeseries_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:14:17.448208 threedigrid-2.2.8/threedigrid/admin/nodes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 12:14:14.000000 threedigrid-2.2.8/threedigrid/admin/nodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5261 2024-04-25 12:14:14.000000 threedigrid-2.2.8/threedigrid/admin/nodes/exporters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12288 2024-04-25 12:14:14.000000 threedigrid-2.2.8/threedigrid/admin/nodes/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5316 2024-04-25 12:14:14.000000 threedigrid-2.2.8/threedigrid/admin/nodes/prepare.py
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-04-25 12:14:14.000000 threedigrid-2.2.8/threedigrid/admin/nodes/subsets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4955 2024-04-25 12:14:14.000000 threedigrid-2.2.8/threedigrid/admin/nodes/timeseries_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20857 2024-04-25 12:14:14.000000 threedigrid-2.2.8/threedigrid/admin/prepare.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2731 2024-04-25 12:14:14.000000 threedigrid-2.2.8/threedigrid/admin/prepare_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:14:17.448208 threedigrid-2.2.8/threedigrid/admin/pumps/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 12:14:14.000000 threedigrid-2.2.8/threedigrid/admin/pumps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-04-25 12:14:14.000000 threedigrid-2.2.8/threedigrid/admin/pumps/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4304 2024-04-25 12:14:14.000000 threedigrid-2.2.8/threedigrid/admin/pumps/prepare.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-04-25 12:14:14.000000 threedigrid-2.2.8/threedigrid/admin/pumps/timeseries_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8926 2024-04-25 12:14:14.000000 threedigrid-2.2.8/threedigrid/admin/rpc_datasource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10057 2024-04-25 12:14:14.000000 threedigrid-2.2.8/threedigrid/admin/serializers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:14:17.448208 threedigrid-2.2.8/threedigrid/admin/structure_controls/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 12:14:14.000000 threedigrid-2.2.8/threedigrid/admin/structure_controls/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-04-25 12:14:14.000000 threedigrid-2.2.8/threedigrid/admin/structure_controls/exporters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-04-25 12:14:14.000000 threedigrid-2.2.8/threedigrid/admin/structure_controls/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7474 2024-04-25 12:14:14.000000 threedigrid-2.2.8/threedigrid/admin/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10204 2024-04-25 12:14:14.000000 threedigrid-2.2.8/threedigrid/geo_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:14:17.448208 threedigrid-2.2.8/threedigrid/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 12:14:14.000000 threedigrid-2.2.8/threedigrid/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:14:17.448208 threedigrid-2.2.8/threedigrid/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 12:14:14.000000 threedigrid-2.2.8/threedigrid/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-04-25 12:14:14.000000 threedigrid-2.2.8/threedigrid/management/commands/kick.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-04-25 12:14:14.000000 threedigrid-2.2.8/threedigrid/management/help_texts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9564 2024-04-25 12:14:14.000000 threedigrid-2.2.8/threedigrid/numpy_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:14:17.452208 threedigrid-2.2.8/threedigrid/orm/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 12:14:14.000000 threedigrid-2.2.8/threedigrid/orm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:14:17.452208 threedigrid-2.2.8/threedigrid/orm/base/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 12:14:14.000000 threedigrid-2.2.8/threedigrid/orm/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      947 2024-04-25 12:14:14.000000 threedigrid-2.2.8/threedigrid/orm/base/datasource.py
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-25 12:14:14.000000 threedigrid-2.2.8/threedigrid/orm/base/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-25 12:14:14.000000 threedigrid-2.2.8/threedigrid/orm/base/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2396 2024-04-25 12:14:14.000000 threedigrid-2.2.8/threedigrid/orm/base/exporters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8744 2024-04-25 12:14:14.000000 threedigrid-2.2.8/threedigrid/orm/base/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6511 2024-04-25 12:14:14.000000 threedigrid-2.2.8/threedigrid/orm/base/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17964 2024-04-25 12:14:14.000000 threedigrid-2.2.8/threedigrid/orm/base/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11698 2024-04-25 12:14:14.000000 threedigrid-2.2.8/threedigrid/orm/base/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16216 2024-04-25 12:14:14.000000 threedigrid-2.2.8/threedigrid/orm/base/timeseries_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-25 12:14:14.000000 threedigrid-2.2.8/threedigrid/orm/base/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-04-25 12:14:14.000000 threedigrid-2.2.8/threedigrid/orm/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8933 2024-04-25 12:14:14.000000 threedigrid-2.2.8/threedigrid/orm/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5047 2024-04-25 12:14:14.000000 threedigrid-2.2.8/threedigrid/orm/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5530 2024-04-25 12:14:14.000000 threedigrid-2.2.8/threedigrid/orm/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:14:17.452208 threedigrid-2.2.8/threedigrid.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    24537 2024-04-25 12:14:17.000000 threedigrid-2.2.8/threedigrid.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3442 2024-04-25 12:14:17.000000 threedigrid-2.2.8/threedigrid.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 12:14:17.000000 threedigrid-2.2.8/threedigrid.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-25 12:14:17.000000 threedigrid-2.2.8/threedigrid.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 12:14:17.000000 threedigrid-2.2.8/threedigrid.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-25 12:14:17.000000 threedigrid-2.2.8/threedigrid.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-25 12:14:17.000000 threedigrid-2.2.8/threedigrid.egg-info/top_level.txt
```

### Comparing `threedigrid-2.2.7/CONTRIBUTING.rst` & `threedigrid-2.2.8/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.7/HISTORY.rst` & `threedigrid-2.2.8/HISTORY.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 History
 =======
 
+2.2.8 (2024-04-25)
+------------------
+
+- Add `group_by_grid_id` to structure control interface.
+
+
 2.2.7 (2024-04-22)
 ------------------
 
 - Set substance units on Nodes.
 
 - Set exchange level on levl attribute on breach geojson export.
```

### Comparing `threedigrid-2.2.7/LICENSE` & `threedigrid-2.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.7/PKG-INFO` & `threedigrid-2.2.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: threedigrid
-Version: 2.2.7
+Version: 2.2.8
 Summary: Python package for the threedigrid administration
 Home-page: https://github.com/nens/threedigrid
 Author: Lars Claussen
 Author-email: info@nelen-schuurmans.nl
 License: BSD license
 Keywords: threedigrid
 Classifier: Development Status :: 4 - Beta
@@ -194,14 +194,20 @@
 .. _Cookiecutter: https://github.com/audreyr/cookiecutter
 .. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
 
 
 History
 =======
 
+2.2.8 (2024-04-25)
+------------------
+
+- Add `group_by_grid_id` to structure control interface.
+
+
 2.2.7 (2024-04-22)
 ------------------
 
 - Set substance units on Nodes.
 
 - Set exchange level on levl attribute on breach geojson export.
```

### Comparing `threedigrid-2.2.7/README.rst` & `threedigrid-2.2.8/README.rst`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.7/docs/Makefile` & `threedigrid-2.2.8/docs/Makefile`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.7/docs/aggregate_results.rst` & `threedigrid-2.2.8/docs/aggregate_results.rst`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.7/docs/conf.py` & `threedigrid-2.2.8/docs/conf.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.7/docs/functionalities.rst` & `threedigrid-2.2.8/docs/functionalities.rst`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.7/docs/gridadmin.rst` & `threedigrid-2.2.8/docs/gridadmin.rst`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.7/docs/introduction.rst` & `threedigrid-2.2.8/docs/introduction.rst`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.7/docs/make.bat` & `threedigrid-2.2.8/docs/make.bat`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.7/docs/results.rst` & `threedigrid-2.2.8/docs/results.rst`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.7/docs/structure_control.rst` & `threedigrid-2.2.8/docs/structure_control.rst`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.7/docs/water_quality_results.rst` & `threedigrid-2.2.8/docs/water_quality_results.rst`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.7/setup.cfg` & `threedigrid-2.2.8/setup.cfg`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.7/setup.py` & `threedigrid-2.2.8/setup.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.7/tests/test_aggregateresultadmin.py` & `threedigrid-2.2.8/tests/test_aggregateresultadmin.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.7/tests/test_exporter.py` & `threedigrid-2.2.8/tests/test_exporter.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.7/tests/test_filters.py` & `threedigrid-2.2.8/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.7/tests/test_gridadmin.py` & `threedigrid-2.2.8/tests/test_gridadmin.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.7/tests/test_gridresultadmin.py` & `threedigrid-2.2.8/tests/test_gridresultadmin.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.7/tests/test_id_mapper.py` & `threedigrid-2.2.8/tests/test_id_mapper.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.7/tests/test_management.py` & `threedigrid-2.2.8/tests/test_management.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.7/tests/test_meta.py` & `threedigrid-2.2.8/tests/test_meta.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.7/tests/test_options.py` & `threedigrid-2.2.8/tests/test_options.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.7/tests/test_prepare.py` & `threedigrid-2.2.8/tests/test_prepare.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.7/tests/test_prepare_utils.py` & `threedigrid-2.2.8/tests/test_prepare_utils.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.7/tests/test_structure_controls.py` & `threedigrid-2.2.8/tests/test_structure_controls.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.7/tests/test_utils.py` & `threedigrid-2.2.8/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.7/threedigrid/admin/breaches/exporters.py` & `threedigrid-2.2.8/threedigrid/admin/breaches/exporters.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.7/threedigrid/admin/breaches/models.py` & `threedigrid-2.2.8/threedigrid/admin/breaches/models.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.7/threedigrid/admin/breaches/prepare.py` & `threedigrid-2.2.8/threedigrid/admin/breaches/prepare.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.7/threedigrid/admin/breaches/timeseries_mixin.py` & `threedigrid-2.2.8/threedigrid/admin/breaches/timeseries_mixin.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.7/threedigrid/admin/constants.py` & `threedigrid-2.2.8/threedigrid/admin/constants.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.7/threedigrid/admin/crosssections/models.py` & `threedigrid-2.2.8/threedigrid/admin/crosssections/models.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.7/threedigrid/admin/exporter_constants.py` & `threedigrid-2.2.8/threedigrid/admin/exporter_constants.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.7/threedigrid/admin/exporters/geopackage/default.py` & `threedigrid-2.2.8/threedigrid/admin/exporters/geopackage/default.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.7/threedigrid/admin/exporters/geopackage/exporter.py` & `threedigrid-2.2.8/threedigrid/admin/exporters/geopackage/exporter.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.7/threedigrid/admin/gridadmin.py` & `threedigrid-2.2.8/threedigrid/admin/gridadmin.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.7/threedigrid/admin/gridresultadmin.py` & `threedigrid-2.2.8/threedigrid/admin/gridresultadmin.py`

 * *Files 1% similar despite different names*

```diff
@@ -441,23 +441,30 @@
         action_type = self.action_type[mask][0]
         source_table, source_table_id = self.struct_control.get_source_table(
             action_type, grid_id
         )
 
         return StructureControl(
             id=id,
+            grid_id=grid_id,
             source_table=source_table,
             source_table_id=source_table_id,
             time=self.time[mask],
             action_type=action_type,
             action_value_1=self.action_value_1[mask],
             action_value_2=self.action_value_2[mask],
             is_active=self.is_active[mask],
         )
 
+    def group_by_grid_id(self, value: int) -> List[StructureControl]:
+        """
+        Get all structure control actions with ``grid_id == value``
+        """
+        return self._group_by("grid_id", value)
+
     def group_by_action_type(self, value: str) -> List[StructureControl]:
         """
         Get all structure control actions with ``action_type == value``
         """
         return self._group_by("action_type", value)
 
     def group_by_is_active(self, value: int) -> List[StructureControl]:
@@ -467,19 +474,19 @@
         return self._group_by("is_active", value)
 
     def group_by_time(self, min: float, max: float) -> List[StructureControl]:
         """Get all structure control actions where ``min <= time <= max``"""
         return self._group_by_in_between("time", min, max)
 
     def group_by_action_value_1(self, min: float, max: float) -> List[StructureControl]:
-        """Get all structure control actions with ``action_value_1 == value``"""
+        """Get all structure control actions where ``min <= action_value_1 <= max``"""
         return self._group_by_in_between("action_value_1", min, max)
 
     def group_by_action_value_2(self, min: float, max: float) -> List[StructureControl]:
-        """Get all structure control actions with ``action_value_2 == value``"""
+        """Get all structure control actions where ``min <= action_value_2 <= max``"""
         return self._group_by_in_between("action_value_2", min, max)
 
     def _group_by(
         self, type: str, value: Union[int, float, str]
     ) -> List[StructureControl]:
         """Group control action by a type, and sort them by unique id
```

### Comparing `threedigrid-2.2.7/threedigrid/admin/h5py_datasource.py` & `threedigrid-2.2.8/threedigrid/admin/h5py_datasource.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.7/threedigrid/admin/h5py_swmr.py` & `threedigrid-2.2.8/threedigrid/admin/h5py_swmr.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.7/threedigrid/admin/idmapper.py` & `threedigrid-2.2.8/threedigrid/admin/idmapper.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.7/threedigrid/admin/levees/exporters.py` & `threedigrid-2.2.8/threedigrid/admin/levees/exporters.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.7/threedigrid/admin/levees/models.py` & `threedigrid-2.2.8/threedigrid/admin/levees/models.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.7/threedigrid/admin/levees/prepare.py` & `threedigrid-2.2.8/threedigrid/admin/levees/prepare.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.7/threedigrid/admin/lines/exporters.py` & `threedigrid-2.2.8/threedigrid/admin/lines/exporters.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.7/threedigrid/admin/lines/models.py` & `threedigrid-2.2.8/threedigrid/admin/lines/models.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.7/threedigrid/admin/lines/prepare.py` & `threedigrid-2.2.8/threedigrid/admin/lines/prepare.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.7/threedigrid/admin/lines/subsets.py` & `threedigrid-2.2.8/threedigrid/admin/lines/subsets.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.7/threedigrid/admin/lines/timeseries_mixin.py` & `threedigrid-2.2.8/threedigrid/admin/lines/timeseries_mixin.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.7/threedigrid/admin/nodes/exporters.py` & `threedigrid-2.2.8/threedigrid/admin/nodes/exporters.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.7/threedigrid/admin/nodes/models.py` & `threedigrid-2.2.8/threedigrid/admin/nodes/models.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.7/threedigrid/admin/nodes/prepare.py` & `threedigrid-2.2.8/threedigrid/admin/nodes/prepare.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.7/threedigrid/admin/nodes/subsets.py` & `threedigrid-2.2.8/threedigrid/admin/nodes/subsets.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.7/threedigrid/admin/nodes/timeseries_mixin.py` & `threedigrid-2.2.8/threedigrid/admin/nodes/timeseries_mixin.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.7/threedigrid/admin/prepare.py` & `threedigrid-2.2.8/threedigrid/admin/prepare.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.7/threedigrid/admin/prepare_utils.py` & `threedigrid-2.2.8/threedigrid/admin/prepare_utils.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.7/threedigrid/admin/pumps/models.py` & `threedigrid-2.2.8/threedigrid/admin/pumps/models.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.7/threedigrid/admin/pumps/prepare.py` & `threedigrid-2.2.8/threedigrid/admin/pumps/prepare.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.7/threedigrid/admin/pumps/timeseries_mixin.py` & `threedigrid-2.2.8/threedigrid/admin/pumps/timeseries_mixin.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.7/threedigrid/admin/rpc_datasource.py` & `threedigrid-2.2.8/threedigrid/admin/rpc_datasource.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.7/threedigrid/admin/serializers.py` & `threedigrid-2.2.8/threedigrid/admin/serializers.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.7/threedigrid/admin/structure_controls/exporters.py` & `threedigrid-2.2.8/threedigrid/admin/structure_controls/exporters.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.7/threedigrid/admin/structure_controls/models.py` & `threedigrid-2.2.8/threedigrid/admin/structure_controls/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,23 +8,25 @@
     timed_control = "timed_control"
 
 
 class StructureControl:
     def __init__(
         self,
         id: str,
+        grid_id: int,
         source_table: str,
         source_table_id: int,
         time: List[float],
         action_type: str,
         action_value_1: List[float],
         action_value_2: List[float],
         is_active: List[int],
     ) -> None:
         self.id = id
+        self.grid_id = grid_id
         self.source_table = source_table
         self.source_table_id = source_table_id
         self.time = time
         self.action_type = action_type
         self.action_value_1 = action_value_1
         self.action_value_2 = action_value_2
         self.is_active = is_active
```

### Comparing `threedigrid-2.2.7/threedigrid/admin/utils.py` & `threedigrid-2.2.8/threedigrid/admin/utils.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.7/threedigrid/geo_utils.py` & `threedigrid-2.2.8/threedigrid/geo_utils.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.7/threedigrid/management/commands/kick.py` & `threedigrid-2.2.8/threedigrid/management/commands/kick.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.7/threedigrid/management/help_texts.py` & `threedigrid-2.2.8/threedigrid/management/help_texts.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.7/threedigrid/numpy_utils.py` & `threedigrid-2.2.8/threedigrid/numpy_utils.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.7/threedigrid/orm/base/datasource.py` & `threedigrid-2.2.8/threedigrid/orm/base/datasource.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.7/threedigrid/orm/base/encoder.py` & `threedigrid-2.2.8/threedigrid/orm/base/encoder.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.7/threedigrid/orm/base/exporters.py` & `threedigrid-2.2.8/threedigrid/orm/base/exporters.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.7/threedigrid/orm/base/fields.py` & `threedigrid-2.2.8/threedigrid/orm/base/fields.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.7/threedigrid/orm/base/filters.py` & `threedigrid-2.2.8/threedigrid/orm/base/filters.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.7/threedigrid/orm/base/models.py` & `threedigrid-2.2.8/threedigrid/orm/base/models.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.7/threedigrid/orm/base/options.py` & `threedigrid-2.2.8/threedigrid/orm/base/options.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.7/threedigrid/orm/base/timeseries_mixin.py` & `threedigrid-2.2.8/threedigrid/orm/base/timeseries_mixin.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.7/threedigrid/orm/base/utils.py` & `threedigrid-2.2.8/threedigrid/orm/base/utils.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.7/threedigrid/orm/constants.py` & `threedigrid-2.2.8/threedigrid/orm/constants.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.7/threedigrid/orm/fields.py` & `threedigrid-2.2.8/threedigrid/orm/fields.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.7/threedigrid/orm/filters.py` & `threedigrid-2.2.8/threedigrid/orm/filters.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.7/threedigrid/orm/models.py` & `threedigrid-2.2.8/threedigrid/orm/models.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.7/threedigrid.egg-info/PKG-INFO` & `threedigrid-2.2.8/threedigrid.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: threedigrid
-Version: 2.2.7
+Version: 2.2.8
 Summary: Python package for the threedigrid administration
 Home-page: https://github.com/nens/threedigrid
 Author: Lars Claussen
 Author-email: info@nelen-schuurmans.nl
 License: BSD license
 Keywords: threedigrid
 Classifier: Development Status :: 4 - Beta
@@ -194,14 +194,20 @@
 .. _Cookiecutter: https://github.com/audreyr/cookiecutter
 .. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
 
 
 History
 =======
 
+2.2.8 (2024-04-25)
+------------------
+
+- Add `group_by_grid_id` to structure control interface.
+
+
 2.2.7 (2024-04-22)
 ------------------
 
 - Set substance units on Nodes.
 
 - Set exchange level on levl attribute on breach geojson export.
```

### Comparing `threedigrid-2.2.7/threedigrid.egg-info/SOURCES.txt` & `threedigrid-2.2.8/threedigrid.egg-info/SOURCES.txt`

 * *Files identical despite different names*


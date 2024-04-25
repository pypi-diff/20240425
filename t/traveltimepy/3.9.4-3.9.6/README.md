# Comparing `tmp/traveltimepy-3.9.4.tar.gz` & `tmp/traveltimepy-3.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "traveltimepy-3.9.4.tar", last modified: Thu Apr 11 15:45:25 2024, max compression
+gzip compressed data, was "traveltimepy-3.9.6.tar", last modified: Thu Apr 25 08:18:59 2024, max compression
```

## Comparing `traveltimepy-3.9.4.tar` & `traveltimepy-3.9.6.tar`

### file list

```diff
@@ -1,84 +1,86 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:45:25.021324 traveltimepy-3.9.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-11 15:45:12.000000 traveltimepy-3.9.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-11 15:45:12.000000 traveltimepy-3.9.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    29487 2024-04-11 15:45:25.021324 traveltimepy-3.9.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    29216 2024-04-11 15:45:12.000000 traveltimepy-3.9.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:45:25.013324 traveltimepy-3.9.4/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-11 15:45:12.000000 traveltimepy-3.9.4/benchmarks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-04-11 15:45:12.000000 traveltimepy-3.9.4/benchmarks/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-04-11 15:45:12.000000 traveltimepy-3.9.4/benchmarks/time_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-04-11 15:45:12.000000 traveltimepy-3.9.4/benchmarks/time_filter_fast.py
--rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-04-11 15:45:12.000000 traveltimepy-3.9.4/benchmarks/time_map.py
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-04-11 15:45:25.021324 traveltimepy-3.9.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-11 15:45:12.000000 traveltimepy-3.9.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:45:25.013324 traveltimepy-3.9.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-11 15:45:12.000000 traveltimepy-3.9.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-04-11 15:45:12.000000 traveltimepy-3.9.4/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-11 15:45:12.000000 traveltimepy-3.9.4/tests/geocoding_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-11 15:45:12.000000 traveltimepy-3.9.4/tests/map_info_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1811 2024-04-11 15:45:12.000000 traveltimepy-3.9.4/tests/postcodes_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-04-11 15:45:12.000000 traveltimepy-3.9.4/tests/routes_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      715 2024-04-11 15:45:12.000000 traveltimepy-3.9.4/tests/supported_locations.py
--rw-r--r--   0 runner    (1001) docker     (127)      910 2024-04-11 15:45:12.000000 traveltimepy-3.9.4/tests/time_filter_fast_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-04-11 15:45:12.000000 traveltimepy-3.9.4/tests/time_filter_proto_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      904 2024-04-11 15:45:12.000000 traveltimepy-3.9.4/tests/time_filter_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5271 2024-04-11 15:45:12.000000 traveltimepy-3.9.4/tests/time_map_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4173 2024-04-11 15:45:12.000000 traveltimepy-3.9.4/tests/wkt_parsing_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-04-11 15:45:12.000000 traveltimepy-3.9.4/tests/wkt_pretty_print_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      763 2024-04-11 15:45:12.000000 traveltimepy-3.9.4/tests/wkt_validate_objects_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:45:25.017324 traveltimepy-3.9.4/traveltimepy/
--rw-r--r--   0 runner    (1001) docker     (127)     3700 2024-04-11 15:45:16.000000 traveltimepy-3.9.4/traveltimepy/TimeFilterFastRequest_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2650 2024-04-11 15:45:16.000000 traveltimepy-3.9.4/traveltimepy/TimeFilterFastResponse_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-04-11 15:45:12.000000 traveltimepy-3.9.4/traveltimepy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-11 15:45:12.000000 traveltimepy-3.9.4/traveltimepy/accept_type.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:45:25.017324 traveltimepy-3.9.4/traveltimepy/dto/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-11 15:45:12.000000 traveltimepy-3.9.4/traveltimepy/dto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3057 2024-04-11 15:45:12.000000 traveltimepy-3.9.4/traveltimepy/dto/common.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:45:25.017324 traveltimepy-3.9.4/traveltimepy/dto/requests/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-11 15:45:12.000000 traveltimepy-3.9.4/traveltimepy/dto/requests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-04-11 15:45:12.000000 traveltimepy-3.9.4/traveltimepy/dto/requests/postcodes.py
--rw-r--r--   0 runner    (1001) docker     (127)     3261 2024-04-11 15:45:12.000000 traveltimepy-3.9.4/traveltimepy/dto/requests/postcodes_zones.py
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-11 15:45:12.000000 traveltimepy-3.9.4/traveltimepy/dto/requests/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-04-11 15:45:12.000000 traveltimepy-3.9.4/traveltimepy/dto/requests/routes.py
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-04-11 15:45:12.000000 traveltimepy-3.9.4/traveltimepy/dto/requests/supported_locations.py
--rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-04-11 15:45:12.000000 traveltimepy-3.9.4/traveltimepy/dto/requests/time_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2033 2024-04-11 15:45:12.000000 traveltimepy-3.9.4/traveltimepy/dto/requests/time_filter_fast.py
--rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-04-11 15:45:12.000000 traveltimepy-3.9.4/traveltimepy/dto/requests/time_filter_proto.py
--rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-04-11 15:45:12.000000 traveltimepy-3.9.4/traveltimepy/dto/requests/time_map.py
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-11 15:45:12.000000 traveltimepy-3.9.4/traveltimepy/dto/requests/time_map_geojson.py
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-04-11 15:45:12.000000 traveltimepy-3.9.4/traveltimepy/dto/requests/time_map_wkt.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:45:25.021324 traveltimepy-3.9.4/traveltimepy/dto/responses/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-11 15:45:12.000000 traveltimepy-3.9.4/traveltimepy/dto/responses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-11 15:45:12.000000 traveltimepy-3.9.4/traveltimepy/dto/responses/error.py
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-11 15:45:12.000000 traveltimepy-3.9.4/traveltimepy/dto/responses/map_info.py
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-11 15:45:12.000000 traveltimepy-3.9.4/traveltimepy/dto/responses/postcodes.py
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-11 15:45:12.000000 traveltimepy-3.9.4/traveltimepy/dto/responses/routes.py
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-11 15:45:12.000000 traveltimepy-3.9.4/traveltimepy/dto/responses/supported_locations.py
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-11 15:45:12.000000 traveltimepy-3.9.4/traveltimepy/dto/responses/time_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-11 15:45:12.000000 traveltimepy-3.9.4/traveltimepy/dto/responses/time_filter_fast.py
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-11 15:45:12.000000 traveltimepy-3.9.4/traveltimepy/dto/responses/time_filter_proto.py
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-11 15:45:12.000000 traveltimepy-3.9.4/traveltimepy/dto/responses/time_map.py
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-11 15:45:12.000000 traveltimepy-3.9.4/traveltimepy/dto/responses/time_map_wkt.py
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-04-11 15:45:12.000000 traveltimepy-3.9.4/traveltimepy/dto/responses/zones.py
--rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-04-11 15:45:12.000000 traveltimepy-3.9.4/traveltimepy/dto/transportation.py
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-11 15:45:12.000000 traveltimepy-3.9.4/traveltimepy/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     3746 2024-04-11 15:45:12.000000 traveltimepy-3.9.4/traveltimepy/http.py
--rw-r--r--   0 runner    (1001) docker     (127)      760 2024-04-11 15:45:12.000000 traveltimepy-3.9.4/traveltimepy/itertools.py
--rw-r--r--   0 runner    (1001) docker     (127)    24873 2024-04-11 15:45:12.000000 traveltimepy-3.9.4/traveltimepy/mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-04-11 15:45:12.000000 traveltimepy-3.9.4/traveltimepy/proto_http.py
--rw-r--r--   0 runner    (1001) docker     (127)    20368 2024-04-11 15:45:12.000000 traveltimepy-3.9.4/traveltimepy/sdk.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-11 15:45:12.000000 traveltimepy-3.9.4/traveltimepy/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:45:25.021324 traveltimepy-3.9.4/traveltimepy/wkt/
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-04-11 15:45:12.000000 traveltimepy-3.9.4/traveltimepy/wkt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-11 15:45:12.000000 traveltimepy-3.9.4/traveltimepy/wkt/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-11 15:45:12.000000 traveltimepy-3.9.4/traveltimepy/wkt/error.py
--rw-r--r--   0 runner    (1001) docker     (127)     3194 2024-04-11 15:45:12.000000 traveltimepy-3.9.4/traveltimepy/wkt/geometries.py
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-11 15:45:12.000000 traveltimepy-3.9.4/traveltimepy/wkt/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     4165 2024-04-11 15:45:12.000000 traveltimepy-3.9.4/traveltimepy/wkt/parsing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:45:25.017324 traveltimepy-3.9.4/traveltimepy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    29487 2024-04-11 15:45:24.000000 traveltimepy-3.9.4/traveltimepy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-04-11 15:45:24.000000 traveltimepy-3.9.4/traveltimepy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 15:45:24.000000 traveltimepy-3.9.4/traveltimepy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 15:45:24.000000 traveltimepy-3.9.4/traveltimepy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-11 15:45:24.000000 traveltimepy-3.9.4/traveltimepy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-11 15:45:24.000000 traveltimepy-3.9.4/traveltimepy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:18:59.268463 traveltimepy-3.9.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-25 08:18:44.000000 traveltimepy-3.9.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-25 08:18:44.000000 traveltimepy-3.9.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    32697 2024-04-25 08:18:59.268463 traveltimepy-3.9.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    32426 2024-04-25 08:18:44.000000 traveltimepy-3.9.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:18:59.256463 traveltimepy-3.9.6/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-25 08:18:44.000000 traveltimepy-3.9.6/benchmarks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-04-25 08:18:44.000000 traveltimepy-3.9.6/benchmarks/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-04-25 08:18:44.000000 traveltimepy-3.9.6/benchmarks/time_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-04-25 08:18:44.000000 traveltimepy-3.9.6/benchmarks/time_filter_fast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-04-25 08:18:44.000000 traveltimepy-3.9.6/benchmarks/time_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-04-25 08:18:59.268463 traveltimepy-3.9.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-25 08:18:44.000000 traveltimepy-3.9.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:18:59.260463 traveltimepy-3.9.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-25 08:18:44.000000 traveltimepy-3.9.6/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-04-25 08:18:44.000000 traveltimepy-3.9.6/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-04-25 08:18:44.000000 traveltimepy-3.9.6/tests/distance_map_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-25 08:18:44.000000 traveltimepy-3.9.6/tests/geocoding_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-25 08:18:44.000000 traveltimepy-3.9.6/tests/map_info_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1811 2024-04-25 08:18:44.000000 traveltimepy-3.9.6/tests/postcodes_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-04-25 08:18:44.000000 traveltimepy-3.9.6/tests/routes_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-04-25 08:18:44.000000 traveltimepy-3.9.6/tests/supported_locations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2024-04-25 08:18:44.000000 traveltimepy-3.9.6/tests/time_filter_fast_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-04-25 08:18:44.000000 traveltimepy-3.9.6/tests/time_filter_proto_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-04-25 08:18:44.000000 traveltimepy-3.9.6/tests/time_filter_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5271 2024-04-25 08:18:44.000000 traveltimepy-3.9.6/tests/time_map_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4173 2024-04-25 08:18:44.000000 traveltimepy-3.9.6/tests/wkt_parsing_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-04-25 08:18:44.000000 traveltimepy-3.9.6/tests/wkt_pretty_print_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-04-25 08:18:44.000000 traveltimepy-3.9.6/tests/wkt_validate_objects_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:18:59.260463 traveltimepy-3.9.6/traveltimepy/
+-rw-r--r--   0 runner    (1001) docker     (127)     3700 2024-04-25 08:18:51.000000 traveltimepy-3.9.6/traveltimepy/TimeFilterFastRequest_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2650 2024-04-25 08:18:51.000000 traveltimepy-3.9.6/traveltimepy/TimeFilterFastResponse_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-04-25 08:18:44.000000 traveltimepy-3.9.6/traveltimepy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-25 08:18:44.000000 traveltimepy-3.9.6/traveltimepy/accept_type.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:18:59.264463 traveltimepy-3.9.6/traveltimepy/dto/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-25 08:18:44.000000 traveltimepy-3.9.6/traveltimepy/dto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3139 2024-04-25 08:18:44.000000 traveltimepy-3.9.6/traveltimepy/dto/common.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:18:59.264463 traveltimepy-3.9.6/traveltimepy/dto/requests/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-25 08:18:44.000000 traveltimepy-3.9.6/traveltimepy/dto/requests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3157 2024-04-25 08:18:44.000000 traveltimepy-3.9.6/traveltimepy/dto/requests/distance_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-04-25 08:18:44.000000 traveltimepy-3.9.6/traveltimepy/dto/requests/postcodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3261 2024-04-25 08:18:44.000000 traveltimepy-3.9.6/traveltimepy/dto/requests/postcodes_zones.py
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-25 08:18:44.000000 traveltimepy-3.9.6/traveltimepy/dto/requests/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-04-25 08:18:44.000000 traveltimepy-3.9.6/traveltimepy/dto/requests/routes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-04-25 08:18:44.000000 traveltimepy-3.9.6/traveltimepy/dto/requests/supported_locations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-04-25 08:18:44.000000 traveltimepy-3.9.6/traveltimepy/dto/requests/time_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2151 2024-04-25 08:18:44.000000 traveltimepy-3.9.6/traveltimepy/dto/requests/time_filter_fast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-04-25 08:18:44.000000 traveltimepy-3.9.6/traveltimepy/dto/requests/time_filter_proto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3260 2024-04-25 08:18:44.000000 traveltimepy-3.9.6/traveltimepy/dto/requests/time_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-25 08:18:44.000000 traveltimepy-3.9.6/traveltimepy/dto/requests/time_map_geojson.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-04-25 08:18:44.000000 traveltimepy-3.9.6/traveltimepy/dto/requests/time_map_wkt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:18:59.264463 traveltimepy-3.9.6/traveltimepy/dto/responses/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-25 08:18:44.000000 traveltimepy-3.9.6/traveltimepy/dto/responses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-25 08:18:44.000000 traveltimepy-3.9.6/traveltimepy/dto/responses/error.py
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-25 08:18:44.000000 traveltimepy-3.9.6/traveltimepy/dto/responses/map_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-25 08:18:44.000000 traveltimepy-3.9.6/traveltimepy/dto/responses/postcodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-25 08:18:44.000000 traveltimepy-3.9.6/traveltimepy/dto/responses/routes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-25 08:18:44.000000 traveltimepy-3.9.6/traveltimepy/dto/responses/supported_locations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-25 08:18:44.000000 traveltimepy-3.9.6/traveltimepy/dto/responses/time_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-25 08:18:44.000000 traveltimepy-3.9.6/traveltimepy/dto/responses/time_filter_fast.py
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-25 08:18:44.000000 traveltimepy-3.9.6/traveltimepy/dto/responses/time_filter_proto.py
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-25 08:18:44.000000 traveltimepy-3.9.6/traveltimepy/dto/responses/time_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-25 08:18:44.000000 traveltimepy-3.9.6/traveltimepy/dto/responses/time_map_wkt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-04-25 08:18:44.000000 traveltimepy-3.9.6/traveltimepy/dto/responses/zones.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-04-25 08:18:44.000000 traveltimepy-3.9.6/traveltimepy/dto/transportation.py
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-25 08:18:44.000000 traveltimepy-3.9.6/traveltimepy/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3746 2024-04-25 08:18:44.000000 traveltimepy-3.9.6/traveltimepy/http.py
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-04-25 08:18:44.000000 traveltimepy-3.9.6/traveltimepy/itertools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27981 2024-04-25 08:18:44.000000 traveltimepy-3.9.6/traveltimepy/mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-04-25 08:18:44.000000 traveltimepy-3.9.6/traveltimepy/proto_http.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21930 2024-04-25 08:18:44.000000 traveltimepy-3.9.6/traveltimepy/sdk.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-25 08:18:44.000000 traveltimepy-3.9.6/traveltimepy/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:18:59.268463 traveltimepy-3.9.6/traveltimepy/wkt/
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-04-25 08:18:44.000000 traveltimepy-3.9.6/traveltimepy/wkt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-25 08:18:44.000000 traveltimepy-3.9.6/traveltimepy/wkt/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-25 08:18:44.000000 traveltimepy-3.9.6/traveltimepy/wkt/error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3194 2024-04-25 08:18:44.000000 traveltimepy-3.9.6/traveltimepy/wkt/geometries.py
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-25 08:18:44.000000 traveltimepy-3.9.6/traveltimepy/wkt/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4165 2024-04-25 08:18:44.000000 traveltimepy-3.9.6/traveltimepy/wkt/parsing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:18:59.260463 traveltimepy-3.9.6/traveltimepy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    32697 2024-04-25 08:18:59.000000 traveltimepy-3.9.6/traveltimepy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2380 2024-04-25 08:18:59.000000 traveltimepy-3.9.6/traveltimepy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 08:18:59.000000 traveltimepy-3.9.6/traveltimepy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 08:18:59.000000 traveltimepy-3.9.6/traveltimepy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-25 08:18:59.000000 traveltimepy-3.9.6/traveltimepy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-25 08:18:59.000000 traveltimepy-3.9.6/traveltimepy.egg-info/top_level.txt
```

### Comparing `traveltimepy-3.9.4/LICENSE` & `traveltimepy-3.9.6/LICENSE`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.9.4/PKG-INFO` & `traveltimepy-3.9.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: traveltimepy
-Version: 3.9.4
+Version: 3.9.6
 Summary: "Python Interface to Travel Time."
 Author: TravelTime
 License: MIT
 Keywords: traveltimepy,api,maps
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: test
@@ -78,14 +78,17 @@
 * departure_time: datetime - Leave departure location at no earlier than given time. Cannot be specified with
   arrival_time.
 * travel_time: int - Maximum journey time (in seconds). Maximum value is 14400. Default value is 3600
 * transportation: Union - Transportation mode and related parameters.
 * search_range: Range - When enabled, range adds an arrival window to the arrival time, and results are returned for any
   journeys that arrive during this window.
 * level_of_detail: LevelOfDetail - When enabled, allows the user to specify how detailed the isochrones should be.
+* snap_penalty: SnapPenalty - When enabled, walking time and distance from the departure location to the nearest road, 
+  and from the nearest road to the arrival location, are added to the total travel time and distance of a journey. 
+  Enabled by default.
 
 ### JSON response
 
 #### Returns:
 
 * results: List[TimeMapResult] - The list of isochrone shapes.
 
@@ -213,14 +216,17 @@
 * arrival_time: datetime - Be at arrival location at no later than given time. Cannot be specified with departure_time.
 * departure_time: datetime - Leave departure location at no earlier than given time. Cannot be specified with
   arrival_time.
 * travel_time: int - Maximum journey time (in seconds). Maximum value is 14400. Default value is 3600
 * transportation: Union - Transportation mode and related parameters.
 * search_range: Range - When enabled, range adds an arrival window to the arrival time, and results are returned for any
   journeys that arrive during this window.
+* snap_penalty: SnapPenalty - When enabled, walking time and distance from the departure location to the nearest road, 
+  and from the nearest road to the arrival location, are added to the total travel time and distance of a journey. 
+  Enabled by default.
 
 #### Returns:
 
 * results: List[TimeMapResult] - The list of isochrone shapes.
 
 #### Example:
 
@@ -257,14 +263,17 @@
 * arrival_time: datetime - Be at arrival location at no later than given time. Cannot be specified with departure_time.
 * departure_time: datetime - Leave departure location at no earlier than given time. Cannot be specified with
   arrival_time.
 * travel_time: int - Maximum journey time (in seconds). Maximum value is 14400. Default value is 3600
 * transportation: Union - Transportation mode and related parameters.
 * search_range: Range - When enabled, range adds an arrival window to the arrival time, and results are returned for any
   journeys that arrive during this window.
+* snap_penalty: SnapPenalty - When enabled, walking time and distance from the departure location to the nearest road, 
+  and from the nearest road to the arrival location, are added to the total travel time and distance of a journey. 
+  Enabled by default.
 
 #### Returns:
 
 * results: List[TimeMapResult] - The list of isochrone shapes.
 
 #### Example:
 
@@ -285,14 +294,59 @@
 
     print(results)
 
 
 asyncio.run(main())
 ```
 
+### [Distance Map](https://docs.traveltime.com/api/reference/distance-map)
+
+Given origin coordinates, find shapes of zones reachable within corresponding travel distance.
+
+#### Takes:
+
+* coordinates: List[Coordinates] - Coordinates of the arrival or departure location.
+* arrival_time: datetime - Be at arrival location at no later than given time. Cannot be specified with departure_time.
+* departure_time: datetime - Leave departure location at no earlier than given time. Cannot be specified with
+  arrival_time.
+* travel_distance: int - Maximum journey distance (in meters). Maximum value is 800000 (800km). Minimum value is 75. 
+  Default value is 900.
+* transportation: Union - Transportation mode and related parameters.
+* level_of_detail: LevelOfDetail - When enabled, allows the user to specify how detailed the isochrones should be.
+* snap_penalty: SnapPenalty - When enabled, walking time and distance from the departure location to the nearest road, 
+  and from the nearest road to the arrival location, are added to the total travel time and distance of a journey. 
+  Enabled by default.
+
+#### Returns:
+
+* results: List[TimeMapResult] - The list of isochrone shapes
+
+#### Example:
+
+```python
+import asyncio
+from datetime import datetime
+
+from traveltimepy import Driving, Coordinates, TravelTimeSdk
+
+
+async def main():
+    sdk = TravelTimeSdk("YOUR_APP_ID", "YOUR_APP_KEY")
+
+    results = await sdk.distance_map_async(
+        coordinates=[Coordinates(lat=51.507609, lng=-0.128315), Coordinates(lat=51.517609, lng=-0.138315)],
+        arrival_time=datetime.now(),
+        transportation=Driving()
+    )
+    print(results)
+
+
+asyncio.run(main())
+```
+
 ### [Distance Matrix (Time Filter)](https://docs.traveltime.com/api/reference/travel-time-distance-matrix)
 
 Given origin and destination points filter out points that cannot be reached within specified time limit. Find out
 travel times, distances and costs between an origin and up to 2,000 destination points.
 
 #### Takes:
 
@@ -303,14 +357,17 @@
 * departure_time: datetime - Leave departure location at no earlier than given time. Cannot be specified with
   arrival_time.
 * transportation: Union - Transportation mode and related parameters.
 * travel_time: int - Maximum journey time (in seconds). Maximum value is 14400. Default value is 3600.
 * properties: List[Property] - Properties to be returned about the points. Default value is travel_time.
 * range: FullRange - When enabled, range adds an arrival window to the arrival time, and results are returned for any
   journeys that arrive during this window.
+* snap_penalty: SnapPenalty - When enabled, walking time and distance from the departure location to the nearest road, 
+  and from the nearest road to the arrival location, are added to the total travel time and distance of a journey. 
+  Enabled by default.
 
 #### Returns:
 
 * results: List[TimeFilterResult] - The results list of reachable and unreachable locations.
 
 #### Example:
 
@@ -359,14 +416,17 @@
 * search_ids: Dict[str, List[str]] - Searches from a target location to destinations. You can define up to 100,000
   destinations
 * transportation: Union - Transportation mode and related parameters.
 * travel_time: int - Maximum journey time (in seconds). Maximum value is 10800. Default value is 3600.
 * properties: List[Property] - Properties to be returned about the points. Default value is travel_time.
 * one_to_many: boolean - if one_to_many is equal to true, then it'll be a forward search (one to many matrix), false -
   backward search (many to one matrix). Default value is True.
+* snap_penalty: SnapPenalty - When enabled, walking time and distance from the departure location to the nearest road, 
+  and from the nearest road to the arrival location, are added to the total travel time and distance of a journey. 
+  Enabled by default.
 
 #### Returns:
 
 * results: List[TimeFilterFastResult] - The results list of reachable and unreachable locations.
 
 #### Example:
 
@@ -461,14 +521,17 @@
 * arrival_time: datetime - Be at arrival location at no later than given time. Cannot be specified with departure_time.
 * departure_time: datetime - Leave departure location at no earlier than given time. Cannot be specified with
   arrival_time.
 * transportation: Union - Transportation mode and related parameters.
 * properties: List[Property] - Properties to be returned about the locations. Default value is travel_time.
 * range: FullRange - When enabled, range adds an arrival window to the arrival time, and results are returned for any
   journeys that arrive during this window.
+* snap_penalty: SnapPenalty - When enabled, walking time and distance from the departure location to the nearest road, 
+  and from the nearest road to the arrival location, are added to the total travel time and distance of a journey. 
+  Enabled by default.
 
 #### Returns:
 
 * results: List[RoutesResult] - The results list of routes.
 
 #### Example:
```

### Comparing `traveltimepy-3.9.4/README.md` & `traveltimepy-3.9.6/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -66,14 +66,17 @@
 * departure_time: datetime - Leave departure location at no earlier than given time. Cannot be specified with
   arrival_time.
 * travel_time: int - Maximum journey time (in seconds). Maximum value is 14400. Default value is 3600
 * transportation: Union - Transportation mode and related parameters.
 * search_range: Range - When enabled, range adds an arrival window to the arrival time, and results are returned for any
   journeys that arrive during this window.
 * level_of_detail: LevelOfDetail - When enabled, allows the user to specify how detailed the isochrones should be.
+* snap_penalty: SnapPenalty - When enabled, walking time and distance from the departure location to the nearest road, 
+  and from the nearest road to the arrival location, are added to the total travel time and distance of a journey. 
+  Enabled by default.
 
 ### JSON response
 
 #### Returns:
 
 * results: List[TimeMapResult] - The list of isochrone shapes.
 
@@ -201,14 +204,17 @@
 * arrival_time: datetime - Be at arrival location at no later than given time. Cannot be specified with departure_time.
 * departure_time: datetime - Leave departure location at no earlier than given time. Cannot be specified with
   arrival_time.
 * travel_time: int - Maximum journey time (in seconds). Maximum value is 14400. Default value is 3600
 * transportation: Union - Transportation mode and related parameters.
 * search_range: Range - When enabled, range adds an arrival window to the arrival time, and results are returned for any
   journeys that arrive during this window.
+* snap_penalty: SnapPenalty - When enabled, walking time and distance from the departure location to the nearest road, 
+  and from the nearest road to the arrival location, are added to the total travel time and distance of a journey. 
+  Enabled by default.
 
 #### Returns:
 
 * results: List[TimeMapResult] - The list of isochrone shapes.
 
 #### Example:
 
@@ -245,14 +251,17 @@
 * arrival_time: datetime - Be at arrival location at no later than given time. Cannot be specified with departure_time.
 * departure_time: datetime - Leave departure location at no earlier than given time. Cannot be specified with
   arrival_time.
 * travel_time: int - Maximum journey time (in seconds). Maximum value is 14400. Default value is 3600
 * transportation: Union - Transportation mode and related parameters.
 * search_range: Range - When enabled, range adds an arrival window to the arrival time, and results are returned for any
   journeys that arrive during this window.
+* snap_penalty: SnapPenalty - When enabled, walking time and distance from the departure location to the nearest road, 
+  and from the nearest road to the arrival location, are added to the total travel time and distance of a journey. 
+  Enabled by default.
 
 #### Returns:
 
 * results: List[TimeMapResult] - The list of isochrone shapes.
 
 #### Example:
 
@@ -273,14 +282,59 @@
 
     print(results)
 
 
 asyncio.run(main())
 ```
 
+### [Distance Map](https://docs.traveltime.com/api/reference/distance-map)
+
+Given origin coordinates, find shapes of zones reachable within corresponding travel distance.
+
+#### Takes:
+
+* coordinates: List[Coordinates] - Coordinates of the arrival or departure location.
+* arrival_time: datetime - Be at arrival location at no later than given time. Cannot be specified with departure_time.
+* departure_time: datetime - Leave departure location at no earlier than given time. Cannot be specified with
+  arrival_time.
+* travel_distance: int - Maximum journey distance (in meters). Maximum value is 800000 (800km). Minimum value is 75. 
+  Default value is 900.
+* transportation: Union - Transportation mode and related parameters.
+* level_of_detail: LevelOfDetail - When enabled, allows the user to specify how detailed the isochrones should be.
+* snap_penalty: SnapPenalty - When enabled, walking time and distance from the departure location to the nearest road, 
+  and from the nearest road to the arrival location, are added to the total travel time and distance of a journey. 
+  Enabled by default.
+
+#### Returns:
+
+* results: List[TimeMapResult] - The list of isochrone shapes
+
+#### Example:
+
+```python
+import asyncio
+from datetime import datetime
+
+from traveltimepy import Driving, Coordinates, TravelTimeSdk
+
+
+async def main():
+    sdk = TravelTimeSdk("YOUR_APP_ID", "YOUR_APP_KEY")
+
+    results = await sdk.distance_map_async(
+        coordinates=[Coordinates(lat=51.507609, lng=-0.128315), Coordinates(lat=51.517609, lng=-0.138315)],
+        arrival_time=datetime.now(),
+        transportation=Driving()
+    )
+    print(results)
+
+
+asyncio.run(main())
+```
+
 ### [Distance Matrix (Time Filter)](https://docs.traveltime.com/api/reference/travel-time-distance-matrix)
 
 Given origin and destination points filter out points that cannot be reached within specified time limit. Find out
 travel times, distances and costs between an origin and up to 2,000 destination points.
 
 #### Takes:
 
@@ -291,14 +345,17 @@
 * departure_time: datetime - Leave departure location at no earlier than given time. Cannot be specified with
   arrival_time.
 * transportation: Union - Transportation mode and related parameters.
 * travel_time: int - Maximum journey time (in seconds). Maximum value is 14400. Default value is 3600.
 * properties: List[Property] - Properties to be returned about the points. Default value is travel_time.
 * range: FullRange - When enabled, range adds an arrival window to the arrival time, and results are returned for any
   journeys that arrive during this window.
+* snap_penalty: SnapPenalty - When enabled, walking time and distance from the departure location to the nearest road, 
+  and from the nearest road to the arrival location, are added to the total travel time and distance of a journey. 
+  Enabled by default.
 
 #### Returns:
 
 * results: List[TimeFilterResult] - The results list of reachable and unreachable locations.
 
 #### Example:
 
@@ -347,14 +404,17 @@
 * search_ids: Dict[str, List[str]] - Searches from a target location to destinations. You can define up to 100,000
   destinations
 * transportation: Union - Transportation mode and related parameters.
 * travel_time: int - Maximum journey time (in seconds). Maximum value is 10800. Default value is 3600.
 * properties: List[Property] - Properties to be returned about the points. Default value is travel_time.
 * one_to_many: boolean - if one_to_many is equal to true, then it'll be a forward search (one to many matrix), false -
   backward search (many to one matrix). Default value is True.
+* snap_penalty: SnapPenalty - When enabled, walking time and distance from the departure location to the nearest road, 
+  and from the nearest road to the arrival location, are added to the total travel time and distance of a journey. 
+  Enabled by default.
 
 #### Returns:
 
 * results: List[TimeFilterFastResult] - The results list of reachable and unreachable locations.
 
 #### Example:
 
@@ -449,14 +509,17 @@
 * arrival_time: datetime - Be at arrival location at no later than given time. Cannot be specified with departure_time.
 * departure_time: datetime - Leave departure location at no earlier than given time. Cannot be specified with
   arrival_time.
 * transportation: Union - Transportation mode and related parameters.
 * properties: List[Property] - Properties to be returned about the locations. Default value is travel_time.
 * range: FullRange - When enabled, range adds an arrival window to the arrival time, and results are returned for any
   journeys that arrive during this window.
+* snap_penalty: SnapPenalty - When enabled, walking time and distance from the departure location to the nearest road, 
+  and from the nearest road to the arrival location, are added to the total travel time and distance of a journey. 
+  Enabled by default.
 
 #### Returns:
 
 * results: List[RoutesResult] - The results list of routes.
 
 #### Example:
```

### Comparing `traveltimepy-3.9.4/benchmarks/common.py` & `traveltimepy-3.9.6/benchmarks/common.py`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.9.4/benchmarks/time_filter.py` & `traveltimepy-3.9.6/benchmarks/time_filter.py`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.9.4/benchmarks/time_filter_fast.py` & `traveltimepy-3.9.6/benchmarks/time_filter_fast.py`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.9.4/benchmarks/time_map.py` & `traveltimepy-3.9.6/benchmarks/time_map.py`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.9.4/setup.cfg` & `traveltimepy-3.9.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.9.4/tests/conftest.py` & `traveltimepy-3.9.6/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.9.4/tests/postcodes_test.py` & `traveltimepy-3.9.6/tests/postcodes_test.py`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.9.4/tests/routes_test.py` & `traveltimepy-3.9.6/tests/time_filter_test.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,29 +2,29 @@
 from datetime import datetime
 
 from traveltimepy import PublicTransport
 
 
 @pytest.mark.asyncio
 async def test_departures(sdk, locations):
-    results = await sdk.routes_async(
+    results = await sdk.time_filter_async(
         locations=locations,
         search_ids={
             "London center": ["Hyde Park", "ZSL London Zoo"],
             "ZSL London Zoo": ["Hyde Park", "London center"],
         },
         transportation=PublicTransport(),
         departure_time=datetime.now(),
     )
     assert len(results) == 2
 
 
 @pytest.mark.asyncio
 async def test_arrivals(sdk, locations):
-    results = await sdk.routes_async(
+    results = await sdk.time_filter_async(
         locations=locations,
         search_ids={
             "London center": ["Hyde Park", "ZSL London Zoo"],
             "ZSL London Zoo": ["Hyde Park", "London center"],
         },
         transportation=PublicTransport(),
         departure_time=datetime.now(),
```

### Comparing `traveltimepy-3.9.4/tests/supported_locations.py` & `traveltimepy-3.9.6/tests/supported_locations.py`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.9.4/tests/time_filter_fast_test.py` & `traveltimepy-3.9.6/tests/time_filter_fast_test.py`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.9.4/tests/time_filter_proto_test.py` & `traveltimepy-3.9.6/tests/time_filter_proto_test.py`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.9.4/tests/time_map_test.py` & `traveltimepy-3.9.6/tests/time_map_test.py`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.9.4/tests/wkt_parsing_test.py` & `traveltimepy-3.9.6/tests/wkt_parsing_test.py`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.9.4/tests/wkt_pretty_print_test.py` & `traveltimepy-3.9.6/tests/wkt_pretty_print_test.py`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.9.4/tests/wkt_validate_objects_test.py` & `traveltimepy-3.9.6/tests/wkt_validate_objects_test.py`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.9.4/traveltimepy/TimeFilterFastRequest_pb2.py` & `traveltimepy-3.9.6/traveltimepy/TimeFilterFastRequest_pb2.py`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.9.4/traveltimepy/TimeFilterFastResponse_pb2.py` & `traveltimepy-3.9.6/traveltimepy/TimeFilterFastResponse_pb2.py`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.9.4/traveltimepy/__init__.py` & `traveltimepy-3.9.6/traveltimepy/__init__.py`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.9.4/traveltimepy/dto/common.py` & `traveltimepy-3.9.6/traveltimepy/dto/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,14 +119,19 @@
 class Property(str, Enum):
     TRAVEL_TIME = "travel_time"
     DISTANCE = "distance"
     ROUTE = "route"
     FARES = "fares"
 
 
+class SnapPenalty(str, Enum):
+    ENABLED = "enabled"
+    DISABLED = "disabled"
+
+
 class PropertyProto(int, Enum):
     DISTANCE = 1
 
 
 class FullRange(BaseModel):
     enabled: bool
     max_results: int
```

### Comparing `traveltimepy-3.9.4/traveltimepy/dto/requests/postcodes.py` & `traveltimepy-3.9.6/traveltimepy/dto/requests/postcodes.py`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.9.4/traveltimepy/dto/requests/postcodes_zones.py` & `traveltimepy-3.9.6/traveltimepy/dto/requests/postcodes_zones.py`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.9.4/traveltimepy/dto/requests/routes.py` & `traveltimepy-3.9.6/traveltimepy/dto/requests/routes.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from datetime import datetime
 from typing import List, Optional, Union
 
 from pydantic.main import BaseModel
 
-from traveltimepy.dto.common import Location, Property, FullRange
+from traveltimepy.dto.common import Location, Property, FullRange, SnapPenalty
 from traveltimepy.dto.transportation import (
     PublicTransport,
     Driving,
     Ferry,
     Walking,
     Cycling,
     DrivingTrain,
@@ -30,14 +30,15 @@
         Walking,
         Cycling,
         DrivingTrain,
         CyclingPublicTransport,
     ]
     properties: List[Property]
     range: Optional[FullRange] = None
+    snap_penalty: Optional[SnapPenalty] = None
 
 
 class DepartureSearch(BaseModel):
     id: str
     arrival_location_ids: List[str]
     departure_location_id: str
     departure_time: datetime
@@ -48,14 +49,15 @@
         Walking,
         Cycling,
         DrivingTrain,
         CyclingPublicTransport,
     ]
     properties: List[Property]
     range: Optional[FullRange] = None
+    snap_penalty: Optional[SnapPenalty] = None
 
 
 class RoutesRequest(TravelTimeRequest[RoutesResponse]):
     locations: List[Location]
     departure_searches: List[DepartureSearch]
     arrival_searches: List[ArrivalSearch]
```

### Comparing `traveltimepy-3.9.4/traveltimepy/dto/requests/supported_locations.py` & `traveltimepy-3.9.6/traveltimepy/dto/requests/supported_locations.py`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.9.4/traveltimepy/dto/requests/time_filter.py` & `traveltimepy-3.9.6/traveltimepy/dto/requests/time_filter.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from datetime import datetime
 from typing import List, Optional, Union
 
 from pydantic.main import BaseModel
 
-from traveltimepy.dto.common import Location, FullRange, Property
+from traveltimepy.dto.common import Location, FullRange, Property, SnapPenalty
 from traveltimepy.dto.requests.request import TravelTimeRequest
 from traveltimepy.dto.responses.time_filter import TimeFilterResponse
 from traveltimepy.itertools import split, flatten
 from traveltimepy.dto.transportation import (
     PublicTransport,
     Driving,
     Ferry,
@@ -31,14 +31,15 @@
         Walking,
         Cycling,
         DrivingTrain,
         CyclingPublicTransport,
     ]
     properties: List[Property]
     range: Optional[FullRange] = None
+    snap_penalty: Optional[SnapPenalty] = None
 
 
 class DepartureSearch(BaseModel):
     id: str
     arrival_location_ids: List[str]
     departure_location_id: str
     departure_time: datetime
@@ -50,14 +51,15 @@
         Walking,
         Cycling,
         DrivingTrain,
         CyclingPublicTransport,
     ]
     properties: List[Property]
     range: Optional[FullRange] = None
+    snap_penalty: Optional[SnapPenalty] = None
 
 
 class TimeFilterRequest(TravelTimeRequest[TimeFilterResponse]):
     locations: List[Location]
     departure_searches: List[DepartureSearch]
     arrival_searches: List[ArrivalSearch]
```

### Comparing `traveltimepy-3.9.4/traveltimepy/dto/requests/time_filter_fast.py` & `traveltimepy-3.9.6/traveltimepy/proto_http.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,72 +1,50 @@
-from typing import List
-from typing_extensions import Literal
+from typing import Dict
 
-from pydantic import BaseModel
-
-from traveltimepy.dto.common import Location, Property
-from traveltimepy.dto.requests.request import TravelTimeRequest
-from traveltimepy.dto.responses.time_filter_fast import TimeFilterFastResponse
-from traveltimepy.itertools import split, flatten
-
-
-class Transportation(BaseModel):
-    type: Literal[
-        "public_transport",
-        "driving",
-        "cycling",
-        "walking",
-        "walking+ferry",
-        "cycling+ferry",
-        "driving+ferry",
-        "driving+public_transport",
-    ]
-
-
-class OneToMany(BaseModel):
-    id: str
-    departure_location_id: str
-    arrival_location_ids: List[str]
-    transportation: Transportation
-    travel_time: int
-    arrival_time_period: str
-    properties: List[Property]
-
-
-class ManyToOne(BaseModel):
-    id: str
-    arrival_location_id: str
-    departure_location_ids: List[str]
-    transportation: Transportation
-    travel_time: int
-    arrival_time_period: str
-    properties: List[Property]
-
-
-class ArrivalSearches(BaseModel):
-    many_to_one: List[ManyToOne]
-    one_to_many: List[OneToMany]
-
-
-class TimeFilterFastRequest(TravelTimeRequest[TimeFilterFastResponse]):
-    locations: List[Location]
-    arrival_searches: ArrivalSearches
-
-    def split_searches(self, window_size: int) -> List[TravelTimeRequest]:
-        return [
-            TimeFilterFastRequest(
-                locations=self.locations,
-                arrival_searches=ArrivalSearches(
-                    one_to_many=one_to_many, many_to_one=many_to_one
-                ),
-            )
-            for one_to_many, many_to_one in split(
-                self.arrival_searches.one_to_many,
-                self.arrival_searches.many_to_one,
-                window_size,
-            )
-        ]
-
-    def merge(self, responses: List[TimeFilterFastResponse]) -> TimeFilterFastResponse:
-        return TimeFilterFastResponse(
-            results=flatten([response.results for response in responses])
+from aiohttp import (
+    ClientSession,
+    ClientResponse,
+    BasicAuth,
+    TCPConnector,
+    ClientTimeout,
+)
+
+from traveltimepy.TimeFilterFastResponse_pb2 import TimeFilterFastResponse
+from traveltimepy.TimeFilterFastRequest_pb2 import TimeFilterFastRequest
+from traveltimepy.dto.responses.time_filter_proto import TimeFilterProtoResponse
+from traveltimepy.errors import ApiError
+
+
+async def send_proto_async(
+    url: str,
+    headers: Dict[str, str],
+    data: TimeFilterFastRequest,
+    app_id: str,
+    api_key: str,
+    timeout: int,
+) -> TimeFilterProtoResponse:
+    async with ClientSession(
+        timeout=ClientTimeout(total=timeout), connector=TCPConnector(ssl=False)
+    ) as session:
+        async with session.post(
+            url=url,
+            headers=headers,
+            data=data.SerializeToString(),
+            auth=BasicAuth(app_id, api_key),
+        ) as resp:
+            return await _process_response(resp)
+
+
+async def _process_response(response: ClientResponse) -> TimeFilterProtoResponse:
+    content = await response.read()
+    if response.status != 200:
+        msg = (
+            f"Travel Time API proto request failed with error code: {response.status}\n"
+        )
+        raise ApiError(msg)
+    else:
+        response_body = TimeFilterFastResponse()
+        response_body.ParseFromString(content)
+        return TimeFilterProtoResponse(
+            travel_times=response_body.properties.travelTimes[:],
+            distances=response_body.properties.distances[:],
         )
```

### Comparing `traveltimepy-3.9.4/traveltimepy/dto/requests/time_filter_proto.py` & `traveltimepy-3.9.6/traveltimepy/dto/requests/time_filter_proto.py`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.9.4/traveltimepy/dto/requests/time_map.py` & `traveltimepy-3.9.6/traveltimepy/dto/requests/distance_map.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,84 +3,84 @@
 
 from typing import List, Optional
 
 from pydantic.main import BaseModel
 
 from traveltimepy import (
     Coordinates,
-    Range,
     PublicTransport,
     Driving,
     Ferry,
     Walking,
     Cycling,
     DrivingTrain,
     CyclingPublicTransport,
     LevelOfDetail,
 )
+from traveltimepy.dto.common import SnapPenalty
 from traveltimepy.dto.requests.request import TravelTimeRequest
 from traveltimepy.dto.responses.time_map import TimeMapResponse
 from traveltimepy.itertools import split, flatten
 
 
 class DepartureSearch(BaseModel):
     id: str
     coords: Coordinates
     departure_time: datetime
-    travel_time: int
+    travel_distance: int
     transportation: typing.Union[
         PublicTransport,
         Driving,
         Ferry,
         Walking,
         Cycling,
         DrivingTrain,
         CyclingPublicTransport,
     ]
-    range: Optional[Range] = None
     level_of_detail: Optional[LevelOfDetail] = None
+    snap_penalty: Optional[SnapPenalty] = None
 
 
 class ArrivalSearch(BaseModel):
     id: str
     coords: Coordinates
     arrival_time: datetime
-    travel_time: int
+    travel_distance: int
     transportation: typing.Union[
         PublicTransport,
         Driving,
         Ferry,
         Walking,
         Cycling,
         DrivingTrain,
         CyclingPublicTransport,
     ]
-    range: Optional[Range] = None
     level_of_detail: Optional[LevelOfDetail] = None
+    snap_penalty: Optional[SnapPenalty] = None
 
 
 class Intersection(BaseModel):
     id: str
     search_ids: List[str]
 
 
 class Union(BaseModel):
     id: str
     search_ids: List[str]
 
 
-class TimeMapRequest(TravelTimeRequest[TimeMapResponse]):
+class DistanceMapRequest(TravelTimeRequest[TimeMapResponse]):
     departure_searches: List[DepartureSearch]
     arrival_searches: List[ArrivalSearch]
     unions: List[Union] = None
     intersections: List[Intersection] = None
 
     def split_searches(self, window_size: int) -> List[TravelTimeRequest]:
         return [
-            TimeMapRequest(
+            DistanceMapRequest(
                 departure_searches=departures,
                 arrival_searches=arrivals,
                 unions=self.unions,
                 intersections=self.intersections,
             )
             for departures, arrivals in split(
                 self.departure_searches, self.arrival_searches, window_size
```

### Comparing `traveltimepy-3.9.4/traveltimepy/dto/requests/time_map_geojson.py` & `traveltimepy-3.9.6/traveltimepy/dto/requests/time_map_geojson.py`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.9.4/traveltimepy/dto/requests/time_map_wkt.py` & `traveltimepy-3.9.6/traveltimepy/dto/requests/time_map_wkt.py`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.9.4/traveltimepy/dto/responses/routes.py` & `traveltimepy-3.9.6/traveltimepy/dto/responses/routes.py`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.9.4/traveltimepy/dto/responses/time_filter.py` & `traveltimepy-3.9.6/traveltimepy/dto/responses/time_filter.py`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.9.4/traveltimepy/dto/responses/time_filter_fast.py` & `traveltimepy-3.9.6/traveltimepy/dto/responses/time_filter_fast.py`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.9.4/traveltimepy/dto/responses/time_map_wkt.py` & `traveltimepy-3.9.6/traveltimepy/dto/responses/time_map_wkt.py`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.9.4/traveltimepy/dto/responses/zones.py` & `traveltimepy-3.9.6/traveltimepy/dto/responses/zones.py`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.9.4/traveltimepy/dto/transportation.py` & `traveltimepy-3.9.6/traveltimepy/dto/transportation.py`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.9.4/traveltimepy/http.py` & `traveltimepy-3.9.6/traveltimepy/http.py`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.9.4/traveltimepy/itertools.py` & `traveltimepy-3.9.6/traveltimepy/itertools.py`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.9.4/traveltimepy/mapper.py` & `traveltimepy-3.9.6/traveltimepy/mapper.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import math
 from typing import Dict, Union, List, Optional
 
+from traveltimepy.dto.requests.distance_map import DistanceMapRequest
 from traveltimepy.dto.requests.time_map_geojson import TimeMapRequestGeojson
 from traveltimepy.dto.requests.time_map_wkt import TimeMapWKTRequest
 from traveltimepy.errors import ApiError
 from traveltimepy import TimeFilterFastRequest_pb2
 
 from traveltimepy.dto.common import (
     Location,
@@ -13,14 +14,15 @@
     Property,
     Range,
     LevelOfDetail,
     PropertyProto,
     TimeInfo,
     ArrivalTime,
     DepartureTime,
+    SnapPenalty,
 )
 from traveltimepy.dto.transportation import (
     PublicTransport,
     Driving,
     Ferry,
     Walking,
     Cycling,
@@ -38,14 +40,15 @@
 from traveltimepy.dto.requests.postcodes_zones import (
     PostcodesDistrictsRequest,
     PostcodesSectorsRequest,
 )
 from traveltimepy.dto.requests.time_map import TimeMapRequest
 
 from traveltimepy.dto.requests import (
+    distance_map,
     time_filter,
     time_filter_fast,
     postcodes,
     postcodes_zones,
     routes,
     time_map,
 )
@@ -63,14 +66,15 @@
         DrivingTrain,
         CyclingPublicTransport,
     ],
     properties: Optional[List[Property]],
     time_info: TimeInfo,
     travel_time: int,
     range: Optional[FullRange],
+    snap_penalty: Optional[SnapPenalty] = None,
 ) -> TimeFilterRequest:
     if properties is None:
         properties = [Property.TRAVEL_TIME]
     if isinstance(time_info, ArrivalTime):
         return TimeFilterRequest(
             locations=locations,
             arrival_searches=[
@@ -81,14 +85,15 @@
                         departure_id for departure_id in departure_ids
                     ],
                     arrival_time=time_info.value,
                     travel_time=travel_time,
                     transportation=transportation,
                     properties=properties,
                     range=range,
+                    snap_penalty=snap_penalty,
                 )
                 for arrival_id, departure_ids in search_ids.items()
             ],
             departure_searches=[],
         )
     elif isinstance(time_info, DepartureTime):
         return TimeFilterRequest(
@@ -99,14 +104,15 @@
                     departure_location_id=departure_id,
                     arrival_location_ids=[arrival_id for arrival_id in arrival_ids],
                     departure_time=time_info.value,
                     travel_time=travel_time,
                     transportation=transportation,
                     properties=properties,
                     range=range,
+                    snap_penalty=snap_penalty,
                 )
                 for departure_id, arrival_ids in search_ids.items()
             ],
             arrival_searches=[],
         )
     else:
         raise ApiError("arrival_time or departure_time should be specified")
@@ -115,14 +121,15 @@
 def create_time_filter_fast(
     locations: List[Location],
     search_ids: Dict[str, List[str]],
     transportation: Transportation,
     travel_time: int = 3600,
     properties: Optional[List[Property]] = None,
     one_to_many: bool = False,
+    snap_penalty: Optional[SnapPenalty] = None,
 ) -> TimeFilterFastRequest:
     if properties is None:
         properties = [Property.TRAVEL_TIME]
     if one_to_many:
         return TimeFilterFastRequest(
             locations=locations,
             arrival_searches=time_filter_fast.ArrivalSearches(
@@ -131,14 +138,15 @@
                         id=departure_id,
                         departure_location_id=departure_id,
                         arrival_location_ids=arrival_ids,
                         transportation=transportation,
                         travel_time=travel_time,
                         arrival_time_period="weekday_morning",
                         properties=properties,
+                        snap_penalty=snap_penalty,
                     )
                     for departure_id, arrival_ids in search_ids.items()
                 ],
                 many_to_one=[],
             ),
         )
     else:
@@ -150,14 +158,15 @@
                         id=arrival_id,
                         arrival_location_id=arrival_id,
                         departure_location_ids=departure_ids,
                         transportation=transportation,
                         travel_time=travel_time,
                         arrival_time_period="weekday_morning",
                         properties=properties,
+                        snap_penalty=snap_penalty,
                     )
                     for arrival_id, departure_ids in search_ids.items()
                 ],
                 one_to_many=[],
             ),
         )
 
@@ -344,26 +353,28 @@
         DrivingTrain,
         CyclingPublicTransport,
     ],
     travel_time: int,
     time_info: TimeInfo,
     search_range: Optional[Range],
     level_of_detail: Optional[LevelOfDetail],
+    snap_penalty: Optional[SnapPenalty],
 ) -> TimeMapRequest:
     if isinstance(time_info, ArrivalTime):
         return TimeMapRequest(
             arrival_searches=[
                 time_map.ArrivalSearch(
                     id=f"Search {ind}",
                     coords=cur_coordinates,
                     travel_time=travel_time,
                     arrival_time=time_info.value,
                     transportation=transportation,
                     range=search_range,
                     level_of_detail=level_of_detail,
+                    snap_penalty=snap_penalty,
                 )
                 for ind, cur_coordinates in enumerate(coordinates)
             ],
             departure_searches=[],
             unions=[],
             intersections=[],
         )
@@ -374,14 +385,15 @@
                     id=f"Search {ind}",
                     coords=cur_coordinates,
                     travel_time=travel_time,
                     departure_time=time_info.value,
                     transportation=transportation,
                     range=search_range,
                     level_of_detail=level_of_detail,
+                    snap_penalty=snap_penalty,
                 )
                 for ind, cur_coordinates in enumerate(coordinates)
             ],
             arrival_searches=[],
             unions=[],
             intersections=[],
         )
@@ -400,26 +412,28 @@
         DrivingTrain,
         CyclingPublicTransport,
     ],
     travel_time: int,
     time_info: TimeInfo,
     search_range: Optional[Range],
     level_of_detail: Optional[LevelOfDetail],
+    snap_penalty: Optional[SnapPenalty] = None,
 ) -> TimeMapRequestGeojson:
     if isinstance(time_info, ArrivalTime):
         return TimeMapRequestGeojson(
             arrival_searches=[
                 time_map.ArrivalSearch(
                     id=f"Search {ind}",
                     coords=cur_coordinates,
                     travel_time=travel_time,
                     arrival_time=time_info.value,
                     transportation=transportation,
                     range=search_range,
                     level_of_detail=level_of_detail,
+                    snap_penalty=snap_penalty,
                 )
                 for ind, cur_coordinates in enumerate(coordinates)
             ],
             departure_searches=[],
         )
     elif isinstance(time_info, DepartureTime):
         return TimeMapRequestGeojson(
@@ -428,14 +442,15 @@
                     id=f"Search {ind}",
                     coords=cur_coordinates,
                     travel_time=travel_time,
                     departure_time=time_info.value,
                     transportation=transportation,
                     range=search_range,
                     level_of_detail=level_of_detail,
+                    snap_penalty=snap_penalty,
                 )
                 for ind, cur_coordinates in enumerate(coordinates)
             ],
             arrival_searches=[],
         )
     else:
         raise ApiError("arrival_time or departure_time should be specified")
@@ -452,26 +467,28 @@
         DrivingTrain,
         CyclingPublicTransport,
     ],
     travel_time: int,
     time_info: TimeInfo,
     search_range: Optional[Range],
     level_of_detail: Optional[LevelOfDetail],
+    snap_penalty: Optional[SnapPenalty] = None,
 ) -> TimeMapWKTRequest:
     if isinstance(time_info, ArrivalTime):
         return TimeMapWKTRequest(
             arrival_searches=[
                 time_map.ArrivalSearch(
                     id=f"Search {ind}",
                     coords=cur_coordinates,
                     travel_time=travel_time,
                     arrival_time=time_info.value,
                     transportation=transportation,
                     range=search_range,
                     level_of_detail=level_of_detail,
+                    snap_penalty=snap_penalty
                 )
                 for ind, cur_coordinates in enumerate(coordinates)
             ],
             departure_searches=[],
             unions=[],
             intersections=[],
         )
@@ -481,14 +498,71 @@
                 time_map.DepartureSearch(
                     id=f"Search {ind}",
                     coords=cur_coordinates,
                     travel_time=travel_time,
                     departure_time=time_info.value,
                     transportation=transportation,
                     range=search_range,
+                    snap_penalty=snap_penalty
+                )
+                for ind, cur_coordinates in enumerate(coordinates)
+            ],
+            arrival_searches=[],
+            unions=[],
+            intersections=[],
+        )
+    else:
+        raise ApiError("arrival_time or departure_time should be specified")
+
+
+def create_distance_map(
+    coordinates: List[Coordinates],
+    transportation: Union[
+        PublicTransport,
+        Driving,
+        Ferry,
+        Walking,
+        Cycling,
+        DrivingTrain,
+        CyclingPublicTransport,
+    ],
+    travel_distance: int,
+    time_info: TimeInfo,
+    level_of_detail: Optional[LevelOfDetail],
+    snap_penalty: Optional[SnapPenalty],
+) -> DistanceMapRequest:
+    if isinstance(time_info, ArrivalTime):
+        return DistanceMapRequest(
+            arrival_searches=[
+                distance_map.ArrivalSearch(
+                    id=f"Search {ind}",
+                    coords=cur_coordinates,
+                    travel_distance=travel_distance,
+                    arrival_time=time_info.value,
+                    transportation=transportation,
+                    level_of_detail=level_of_detail,
+                    snap_penalty=snap_penalty,
+                )
+                for ind, cur_coordinates in enumerate(coordinates)
+            ],
+            departure_searches=[],
+            unions=[],
+            intersections=[],
+        )
+    elif isinstance(time_info, DepartureTime):
+        return DistanceMapRequest(
+            departure_searches=[
+                distance_map.DepartureSearch(
+                    id=f"Search {ind}",
+                    coords=cur_coordinates,
+                    travel_distance=travel_distance,
+                    departure_time=time_info.value,
+                    transportation=transportation,
+                    level_of_detail=level_of_detail,
+                    snap_penalty=snap_penalty,
                 )
                 for ind, cur_coordinates in enumerate(coordinates)
             ],
             arrival_searches=[],
             unions=[],
             intersections=[],
         )
@@ -507,26 +581,28 @@
         DrivingTrain,
         CyclingPublicTransport,
     ],
     travel_time: int,
     time_info: TimeInfo,
     search_range: Optional[Range],
     level_of_detail: Optional[LevelOfDetail],
+    snap_penalty: Optional[SnapPenalty] = None,
 ) -> TimeMapRequest:
     if isinstance(time_info, ArrivalTime):
         return TimeMapRequest(
             arrival_searches=[
                 time_map.ArrivalSearch(
                     id=f"Search {ind}",
                     coords=cur_coordinates,
                     travel_time=travel_time,
                     arrival_time=time_info.value,
                     transportation=transportation,
                     range=search_range,
                     level_of_detail=level_of_detail,
+                    snap_penalty=snap_penalty
                 )
                 for ind, cur_coordinates in enumerate(coordinates)
             ],
             departure_searches=[],
             unions=[],
             intersections=[
                 time_map.Intersection(
@@ -542,14 +618,15 @@
                     id=f"Search {ind}",
                     coords=cur_coordinates,
                     travel_time=travel_time,
                     departure_time=time_info.value,
                     transportation=transportation,
                     range=search_range,
                     level_of_detail=level_of_detail,
+                    snap_penalty=snap_penalty
                 )
                 for ind, cur_coordinates in enumerate(coordinates)
             ],
             arrival_searches=[],
             unions=[],
             intersections=[
                 time_map.Intersection(
@@ -573,26 +650,28 @@
         DrivingTrain,
         CyclingPublicTransport,
     ],
     travel_time: int,
     time_info: TimeInfo,
     search_range: Optional[Range],
     level_of_detail: Optional[LevelOfDetail],
+    snap_penalty: Optional[SnapPenalty] = None,
 ) -> TimeMapRequest:
     if isinstance(time_info, ArrivalTime):
         return TimeMapRequest(
             arrival_searches=[
                 time_map.ArrivalSearch(
                     id=f"Search {ind}",
                     coords=cur_coordinates,
                     travel_time=travel_time,
                     arrival_time=time_info.value,
                     transportation=transportation,
                     range=search_range,
                     level_of_detail=level_of_detail,
+                    snap_penalty=snap_penalty,
                 )
                 for ind, cur_coordinates in enumerate(coordinates)
             ],
             departure_searches=[],
             unions=[
                 time_map.Union(
                     id="Union search",
@@ -608,14 +687,15 @@
                     id=f"Search {ind}",
                     coords=cur_coordinates,
                     travel_time=travel_time,
                     departure_time=time_info.value,
                     transportation=transportation,
                     range=search_range,
                     level_of_detail=level_of_detail,
+                    snap_penalty=snap_penalty
                 )
                 for ind, cur_coordinates in enumerate(coordinates)
             ],
             arrival_searches=[],
             unions=[
                 time_map.Union(
                     id="Union search",
@@ -639,14 +719,15 @@
         Cycling,
         DrivingTrain,
         CyclingPublicTransport,
     ],
     time_info: TimeInfo,
     properties: Optional[List[Property]],
     range: Optional[FullRange],
+    snap_penalty: Optional[SnapPenalty],
 ) -> RoutesRequest:
     if properties is None:
         properties = [Property.TRAVEL_TIME]
     if isinstance(time_info, ArrivalTime):
         return RoutesRequest(
             locations=locations,
             arrival_searches=[
@@ -656,14 +737,15 @@
                     departure_location_ids=[
                         departure_id for departure_id in departure_ids
                     ],
                     arrival_time=time_info.value,
                     transportation=transportation,
                     properties=properties,
                     range=range,
+                    snap_penalty=snap_penalty,
                 )
                 for arrival_id, departure_ids in search_ids.items()
             ],
             departure_searches=[],
         )
     elif isinstance(time_info, DepartureTime):
         return RoutesRequest(
@@ -673,14 +755,15 @@
                     id=departure_id,
                     departure_location_id=departure_id,
                     arrival_location_ids=[arrival_id for arrival_id in arrival_ids],
                     departure_time=time_info.value,
                     transportation=transportation,
                     properties=properties,
                     range=range,
+                    snap_penalty=snap_penalty,
                 )
                 for departure_id, arrival_ids in search_ids.items()
             ],
             arrival_searches=[],
         )
     else:
         raise ApiError("arrival_time or departure_time should be specified")
```

### Comparing `traveltimepy-3.9.4/traveltimepy/sdk.py` & `traveltimepy-3.9.6/traveltimepy/sdk.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,14 +8,15 @@
     Property,
     FullRange,
     Range,
     LevelOfDetail,
     PropertyProto,
     DepartureTime,
     ArrivalTime,
+    SnapPenalty,
 )
 from traveltimepy.dto.responses.time_map_wkt import (
     TimeMapWKTResponse,
 )
 from traveltimepy.dto.responses.time_filter_proto import TimeFilterProtoResponse
 from traveltimepy.dto.transportation import (
     PublicTransport,
@@ -53,14 +54,15 @@
     PostcodesDistrictsResponse,
     PostcodesSectorsResponse,
     PostcodesDistrictsResult,
     PostcodesSectorsResult,
 )
 
 from traveltimepy.mapper import (
+    create_distance_map,
     create_time_filter,
     create_time_filter_fast,
     create_postcodes,
     create_districts,
     create_sectors,
     create_routes,
     create_proto_request,
@@ -120,14 +122,15 @@
             CyclingPublicTransport,
         ],
         properties: Optional[List[Property]] = None,
         departure_time: Optional[datetime] = None,
         arrival_time: Optional[datetime] = None,
         travel_time: int = 3600,
         range: Optional[FullRange] = None,
+        snap_penalty: Optional[SnapPenalty] = None,
     ) -> List[TimeFilterResult]:
         time_info = get_time_info(departure_time, arrival_time)
 
         resp = await send_post_async(
             TimeFilterResponse,
             "time-filter",
             self._headers(AcceptType.JSON),
@@ -135,14 +138,15 @@
                 locations,
                 search_ids,
                 transportation,
                 properties,
                 time_info,
                 travel_time,
                 range,
+                snap_penalty,
             ),
             self._sdk_params,
         )
 
         return resp.results
 
     async def map_info_async(self) -> List[Map]:
@@ -207,26 +211,28 @@
         self,
         locations: List[Location],
         search_ids: Dict[str, List[str]],
         transportation: Transportation,
         travel_time: int = 3600,
         properties: Optional[List[Property]] = None,
         one_to_many: bool = True,
+        snap_penalty: Optional[SnapPenalty] = None,
     ) -> List[TimeFilterFastResult]:
         resp = await send_post_async(
             TimeFilterFastResponse,
             "time-filter/fast",
             self._headers(AcceptType.JSON),
             create_time_filter_fast(
                 locations,
                 search_ids,
                 transportation,
                 travel_time,
                 properties,
                 one_to_many,
+                snap_penalty
             ),
             self._sdk_params,
         )
         return resp.results
 
     async def postcodes_async(
         self,
@@ -353,28 +359,30 @@
             DrivingTrain,
             CyclingPublicTransport,
         ],
         departure_time: Optional[datetime] = None,
         arrival_time: Optional[datetime] = None,
         properties: Optional[List[Property]] = None,
         range: Optional[FullRange] = None,
+        snap_penalty: Optional[SnapPenalty] = None,
     ) -> List[RoutesResult]:
         time_info = get_time_info(departure_time, arrival_time)
 
         resp = await send_post_async(
             RoutesResponse,
             "routes",
             self._headers(AcceptType.JSON),
             create_routes(
                 locations,
                 search_ids,
                 transportation,
                 time_info,
                 properties,
                 range,
+                snap_penalty
             ),
             self._sdk_params,
         )
         return resp.results
 
     async def time_filter_proto_async(
         self,
@@ -490,28 +498,30 @@
             CyclingPublicTransport,
         ],
         departure_time: Optional[datetime] = None,
         arrival_time: Optional[datetime] = None,
         travel_time: int = 3600,
         search_range: Optional[Range] = None,
         level_of_detail: Optional[LevelOfDetail] = None,
+        snap_penalty: Optional[SnapPenalty] = None,
     ) -> List[TimeMapResult]:
         time_info = get_time_info(departure_time, arrival_time)
 
         resp = await send_post_async(
             TimeMapResponse,
             "time-map",
             self._headers(AcceptType.JSON),
             create_time_map(
                 coordinates,
                 transportation,
                 travel_time,
                 time_info,
                 search_range,
                 level_of_detail,
+                snap_penalty,
             ),
             self._sdk_params,
         )
         return resp.results
 
     async def time_map_geojson_async(
         self,
@@ -526,28 +536,30 @@
             CyclingPublicTransport,
         ],
         departure_time: Optional[datetime] = None,
         arrival_time: Optional[datetime] = None,
         travel_time: int = 3600,
         search_range: Optional[Range] = None,
         level_of_detail: Optional[LevelOfDetail] = None,
+        snap_penalty: Optional[SnapPenalty] = None,
     ) -> FeatureCollection:
         time_info = get_time_info(departure_time, arrival_time)
 
         resp = await send_post_async(
             FeatureCollection,
             "time-map",
             self._headers(AcceptType.GEO_JSON),
             create_time_map_geojson(
                 coordinates,
                 transportation,
                 travel_time,
                 time_info,
                 search_range,
                 level_of_detail,
+                snap_penalty,
             ),
             self._sdk_params,
         )
         return resp
 
     async def time_map_wkt_async(
         self,
@@ -562,28 +574,30 @@
             CyclingPublicTransport,
         ],
         departure_time: Optional[datetime] = None,
         arrival_time: Optional[datetime] = None,
         travel_time: int = 3600,
         search_range: Optional[Range] = None,
         level_of_detail: Optional[LevelOfDetail] = None,
+        snap_penalty: Optional[SnapPenalty] = None,
     ) -> TimeMapWKTResponse:
         time_info = get_time_info(departure_time, arrival_time)
 
         resp = await send_post_async(
             TimeMapWKTResponse,
             "time-map",
             self._headers(AcceptType.WKT),
             create_time_map_wkt(
                 coordinates,
                 transportation,
                 travel_time,
                 time_info,
                 search_range,
                 level_of_detail,
+                snap_penalty,
             ),
             self._sdk_params,
         )
         return resp
 
     async def time_map_wkt_no_holes_async(
         self,
@@ -598,33 +612,65 @@
             CyclingPublicTransport,
         ],
         departure_time: Optional[datetime] = None,
         arrival_time: Optional[datetime] = None,
         travel_time: int = 3600,
         search_range: Optional[Range] = None,
         level_of_detail: Optional[LevelOfDetail] = None,
+        snap_penalty: Optional[SnapPenalty] = None,
     ) -> TimeMapWKTResponse:
         time_info = get_time_info(departure_time, arrival_time)
 
         resp = await send_post_async(
             TimeMapWKTResponse,
             "time-map",
             self._headers(AcceptType.WKT_NO_HOLES),
             create_time_map_wkt(
                 coordinates,
                 transportation,
                 travel_time,
                 time_info,
                 search_range,
                 level_of_detail,
+                snap_penalty,
             ),
             self._sdk_params,
         )
         return resp
 
+    async def distance_map_async(
+        self,
+        coordinates: List[Coordinates],
+        transportation: Union[
+            PublicTransport,
+            Driving,
+            Ferry,
+            Walking,
+            Cycling,
+            DrivingTrain,
+            CyclingPublicTransport,
+        ],
+        departure_time: Optional[datetime] = None,
+        arrival_time: Optional[datetime] = None,
+        travel_distance: int = 900,
+        level_of_detail: Optional[LevelOfDetail] = None,
+        snap_penalty: Optional[SnapPenalty] = None,
+    ) -> List[TimeMapResult]:
+        time_info = get_time_info(departure_time, arrival_time)
+        resp = await send_post_async(
+            TimeMapResponse,
+            "distance-map",
+            self._headers(AcceptType.JSON),
+            create_distance_map(
+                coordinates, transportation, travel_distance, time_info, level_of_detail, snap_penalty
+            ),
+            self._sdk_params,
+        )
+        return resp.results
+
     @staticmethod
     def _geocoding_reverse_params(lat: float, lng: float) -> Dict[str, str]:
         full_query = {"lat": lat, "lng": lng}
         return {
             key: str(value) for (key, value) in full_query.items() if value is not None
         }
 
@@ -666,14 +712,11 @@
         }
 
 
 def get_time_info(departure_time: Optional[datetime], arrival_time: Optional[datetime]):
     if departure_time and arrival_time:
         raise ApiError("arrival_time and departure_time cannot be both specified")
 
-    time_info = None
     if departure_time:
-        time_info = DepartureTime(departure_time)
+        return DepartureTime(departure_time)
     elif arrival_time:
-        time_info = ArrivalTime(arrival_time)
-
-    return time_info
+        return ArrivalTime(arrival_time)
```

### Comparing `traveltimepy-3.9.4/traveltimepy/wkt/error.py` & `traveltimepy-3.9.6/traveltimepy/wkt/error.py`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.9.4/traveltimepy/wkt/geometries.py` & `traveltimepy-3.9.6/traveltimepy/wkt/geometries.py`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.9.4/traveltimepy/wkt/parsing.py` & `traveltimepy-3.9.6/traveltimepy/wkt/parsing.py`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.9.4/traveltimepy.egg-info/PKG-INFO` & `traveltimepy-3.9.6/traveltimepy.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: traveltimepy
-Version: 3.9.4
+Version: 3.9.6
 Summary: "Python Interface to Travel Time."
 Author: TravelTime
 License: MIT
 Keywords: traveltimepy,api,maps
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: test
@@ -78,14 +78,17 @@
 * departure_time: datetime - Leave departure location at no earlier than given time. Cannot be specified with
   arrival_time.
 * travel_time: int - Maximum journey time (in seconds). Maximum value is 14400. Default value is 3600
 * transportation: Union - Transportation mode and related parameters.
 * search_range: Range - When enabled, range adds an arrival window to the arrival time, and results are returned for any
   journeys that arrive during this window.
 * level_of_detail: LevelOfDetail - When enabled, allows the user to specify how detailed the isochrones should be.
+* snap_penalty: SnapPenalty - When enabled, walking time and distance from the departure location to the nearest road, 
+  and from the nearest road to the arrival location, are added to the total travel time and distance of a journey. 
+  Enabled by default.
 
 ### JSON response
 
 #### Returns:
 
 * results: List[TimeMapResult] - The list of isochrone shapes.
 
@@ -213,14 +216,17 @@
 * arrival_time: datetime - Be at arrival location at no later than given time. Cannot be specified with departure_time.
 * departure_time: datetime - Leave departure location at no earlier than given time. Cannot be specified with
   arrival_time.
 * travel_time: int - Maximum journey time (in seconds). Maximum value is 14400. Default value is 3600
 * transportation: Union - Transportation mode and related parameters.
 * search_range: Range - When enabled, range adds an arrival window to the arrival time, and results are returned for any
   journeys that arrive during this window.
+* snap_penalty: SnapPenalty - When enabled, walking time and distance from the departure location to the nearest road, 
+  and from the nearest road to the arrival location, are added to the total travel time and distance of a journey. 
+  Enabled by default.
 
 #### Returns:
 
 * results: List[TimeMapResult] - The list of isochrone shapes.
 
 #### Example:
 
@@ -257,14 +263,17 @@
 * arrival_time: datetime - Be at arrival location at no later than given time. Cannot be specified with departure_time.
 * departure_time: datetime - Leave departure location at no earlier than given time. Cannot be specified with
   arrival_time.
 * travel_time: int - Maximum journey time (in seconds). Maximum value is 14400. Default value is 3600
 * transportation: Union - Transportation mode and related parameters.
 * search_range: Range - When enabled, range adds an arrival window to the arrival time, and results are returned for any
   journeys that arrive during this window.
+* snap_penalty: SnapPenalty - When enabled, walking time and distance from the departure location to the nearest road, 
+  and from the nearest road to the arrival location, are added to the total travel time and distance of a journey. 
+  Enabled by default.
 
 #### Returns:
 
 * results: List[TimeMapResult] - The list of isochrone shapes.
 
 #### Example:
 
@@ -285,14 +294,59 @@
 
     print(results)
 
 
 asyncio.run(main())
 ```
 
+### [Distance Map](https://docs.traveltime.com/api/reference/distance-map)
+
+Given origin coordinates, find shapes of zones reachable within corresponding travel distance.
+
+#### Takes:
+
+* coordinates: List[Coordinates] - Coordinates of the arrival or departure location.
+* arrival_time: datetime - Be at arrival location at no later than given time. Cannot be specified with departure_time.
+* departure_time: datetime - Leave departure location at no earlier than given time. Cannot be specified with
+  arrival_time.
+* travel_distance: int - Maximum journey distance (in meters). Maximum value is 800000 (800km). Minimum value is 75. 
+  Default value is 900.
+* transportation: Union - Transportation mode and related parameters.
+* level_of_detail: LevelOfDetail - When enabled, allows the user to specify how detailed the isochrones should be.
+* snap_penalty: SnapPenalty - When enabled, walking time and distance from the departure location to the nearest road, 
+  and from the nearest road to the arrival location, are added to the total travel time and distance of a journey. 
+  Enabled by default.
+
+#### Returns:
+
+* results: List[TimeMapResult] - The list of isochrone shapes
+
+#### Example:
+
+```python
+import asyncio
+from datetime import datetime
+
+from traveltimepy import Driving, Coordinates, TravelTimeSdk
+
+
+async def main():
+    sdk = TravelTimeSdk("YOUR_APP_ID", "YOUR_APP_KEY")
+
+    results = await sdk.distance_map_async(
+        coordinates=[Coordinates(lat=51.507609, lng=-0.128315), Coordinates(lat=51.517609, lng=-0.138315)],
+        arrival_time=datetime.now(),
+        transportation=Driving()
+    )
+    print(results)
+
+
+asyncio.run(main())
+```
+
 ### [Distance Matrix (Time Filter)](https://docs.traveltime.com/api/reference/travel-time-distance-matrix)
 
 Given origin and destination points filter out points that cannot be reached within specified time limit. Find out
 travel times, distances and costs between an origin and up to 2,000 destination points.
 
 #### Takes:
 
@@ -303,14 +357,17 @@
 * departure_time: datetime - Leave departure location at no earlier than given time. Cannot be specified with
   arrival_time.
 * transportation: Union - Transportation mode and related parameters.
 * travel_time: int - Maximum journey time (in seconds). Maximum value is 14400. Default value is 3600.
 * properties: List[Property] - Properties to be returned about the points. Default value is travel_time.
 * range: FullRange - When enabled, range adds an arrival window to the arrival time, and results are returned for any
   journeys that arrive during this window.
+* snap_penalty: SnapPenalty - When enabled, walking time and distance from the departure location to the nearest road, 
+  and from the nearest road to the arrival location, are added to the total travel time and distance of a journey. 
+  Enabled by default.
 
 #### Returns:
 
 * results: List[TimeFilterResult] - The results list of reachable and unreachable locations.
 
 #### Example:
 
@@ -359,14 +416,17 @@
 * search_ids: Dict[str, List[str]] - Searches from a target location to destinations. You can define up to 100,000
   destinations
 * transportation: Union - Transportation mode and related parameters.
 * travel_time: int - Maximum journey time (in seconds). Maximum value is 10800. Default value is 3600.
 * properties: List[Property] - Properties to be returned about the points. Default value is travel_time.
 * one_to_many: boolean - if one_to_many is equal to true, then it'll be a forward search (one to many matrix), false -
   backward search (many to one matrix). Default value is True.
+* snap_penalty: SnapPenalty - When enabled, walking time and distance from the departure location to the nearest road, 
+  and from the nearest road to the arrival location, are added to the total travel time and distance of a journey. 
+  Enabled by default.
 
 #### Returns:
 
 * results: List[TimeFilterFastResult] - The results list of reachable and unreachable locations.
 
 #### Example:
 
@@ -461,14 +521,17 @@
 * arrival_time: datetime - Be at arrival location at no later than given time. Cannot be specified with departure_time.
 * departure_time: datetime - Leave departure location at no earlier than given time. Cannot be specified with
   arrival_time.
 * transportation: Union - Transportation mode and related parameters.
 * properties: List[Property] - Properties to be returned about the locations. Default value is travel_time.
 * range: FullRange - When enabled, range adds an arrival window to the arrival time, and results are returned for any
   journeys that arrive during this window.
+* snap_penalty: SnapPenalty - When enabled, walking time and distance from the departure location to the nearest road, 
+  and from the nearest road to the arrival location, are added to the total travel time and distance of a journey. 
+  Enabled by default.
 
 #### Returns:
 
 * results: List[RoutesResult] - The results list of routes.
 
 #### Example:
```

### Comparing `traveltimepy-3.9.4/traveltimepy.egg-info/SOURCES.txt` & `traveltimepy-3.9.6/traveltimepy.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 benchmarks/__init__.py
 benchmarks/common.py
 benchmarks/time_filter.py
 benchmarks/time_filter_fast.py
 benchmarks/time_map.py
 tests/__init__.py
 tests/conftest.py
+tests/distance_map_test.py
 tests/geocoding_test.py
 tests/map_info_test.py
 tests/postcodes_test.py
 tests/routes_test.py
 tests/supported_locations.py
 tests/time_filter_fast_test.py
 tests/time_filter_proto_test.py
@@ -39,14 +40,15 @@
 traveltimepy.egg-info/not-zip-safe
 traveltimepy.egg-info/requires.txt
 traveltimepy.egg-info/top_level.txt
 traveltimepy/dto/__init__.py
 traveltimepy/dto/common.py
 traveltimepy/dto/transportation.py
 traveltimepy/dto/requests/__init__.py
+traveltimepy/dto/requests/distance_map.py
 traveltimepy/dto/requests/postcodes.py
 traveltimepy/dto/requests/postcodes_zones.py
 traveltimepy/dto/requests/request.py
 traveltimepy/dto/requests/routes.py
 traveltimepy/dto/requests/supported_locations.py
 traveltimepy/dto/requests/time_filter.py
 traveltimepy/dto/requests/time_filter_fast.py
```


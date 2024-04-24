# Comparing `tmp/hydroserver-sensorthings-0.2.8.tar.gz` & `tmp/hydroserver-sensorthings-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hydroserver-sensorthings-0.2.8.tar", last modified: Tue Jan 16 20:27:03 2024, max compression
+gzip compressed data, was "hydroserver-sensorthings-0.2.9.tar", last modified: Wed Jan 24 21:32:52 2024, max compression
```

## Comparing `hydroserver-sensorthings-0.2.8.tar` & `hydroserver-sensorthings-0.2.9.tar`

### file list

```diff
@@ -1,106 +1,106 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 20:27:03.592709 hydroserver-sensorthings-0.2.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-01-16 20:26:48.000000 hydroserver-sensorthings-0.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-01-16 20:27:03.592709 hydroserver-sensorthings-0.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-01-16 20:26:48.000000 hydroserver-sensorthings-0.2.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-01-16 20:26:49.000000 hydroserver-sensorthings-0.2.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-01-16 20:27:03.592709 hydroserver-sensorthings-0.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-01-16 20:26:49.000000 hydroserver-sensorthings-0.2.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 20:27:03.572708 hydroserver-sensorthings-0.2.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 20:27:03.592709 hydroserver-sensorthings-0.2.8/src/hydroserver_sensorthings.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-01-16 20:27:03.000000 hydroserver-sensorthings-0.2.8/src/hydroserver_sensorthings.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3690 2024-01-16 20:27:03.000000 hydroserver-sensorthings-0.2.8/src/hydroserver_sensorthings.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-16 20:27:03.000000 hydroserver-sensorthings-0.2.8/src/hydroserver_sensorthings.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-01-16 20:27:03.000000 hydroserver-sensorthings-0.2.8/src/hydroserver_sensorthings.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-01-16 20:27:03.000000 hydroserver-sensorthings-0.2.8/src/hydroserver_sensorthings.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-16 20:27:03.000000 hydroserver-sensorthings-0.2.8/src/hydroserver_sensorthings.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 20:27:03.580709 hydroserver-sensorthings-0.2.8/src/sensorthings/
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-01-16 20:26:49.000000 hydroserver-sensorthings-0.2.8/src/sensorthings/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 20:27:03.580709 hydroserver-sensorthings-0.2.8/src/sensorthings/backends/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-16 20:26:49.000000 hydroserver-sensorthings-0.2.8/src/sensorthings/backends/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 20:27:03.580709 hydroserver-sensorthings-0.2.8/src/sensorthings/backends/frostserver/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-16 20:26:49.000000 hydroserver-sensorthings-0.2.8/src/sensorthings/backends/frostserver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-01-16 20:26:49.000000 hydroserver-sensorthings-0.2.8/src/sensorthings/backends/frostserver/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-01-16 20:26:49.000000 hydroserver-sensorthings-0.2.8/src/sensorthings/backends/frostserver/engine.py
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-01-16 20:26:49.000000 hydroserver-sensorthings-0.2.8/src/sensorthings/backends/frostserver/renderers.py
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-01-16 20:26:49.000000 hydroserver-sensorthings-0.2.8/src/sensorthings/backends/frostserver/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 20:27:03.580709 hydroserver-sensorthings-0.2.8/src/sensorthings/backends/odm2/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-16 20:26:49.000000 hydroserver-sensorthings-0.2.8/src/sensorthings/backends/odm2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-01-16 20:26:49.000000 hydroserver-sensorthings-0.2.8/src/sensorthings/backends/odm2/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)      972 2024-01-16 20:26:49.000000 hydroserver-sensorthings-0.2.8/src/sensorthings/backends/odm2/engine.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-16 20:26:49.000000 hydroserver-sensorthings-0.2.8/src/sensorthings/backends/odm2/models.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-16 20:26:49.000000 hydroserver-sensorthings-0.2.8/src/sensorthings/backends/odm2/schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-01-16 20:26:49.000000 hydroserver-sensorthings-0.2.8/src/sensorthings/backends/odm2/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 20:27:03.584709 hydroserver-sensorthings-0.2.8/src/sensorthings/backends/sensorthings_v1_1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-16 20:26:49.000000 hydroserver-sensorthings-0.2.8/src/sensorthings/backends/sensorthings_v1_1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-01-16 20:26:49.000000 hydroserver-sensorthings-0.2.8/src/sensorthings/backends/sensorthings_v1_1/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)     8180 2024-01-16 20:26:49.000000 hydroserver-sensorthings-0.2.8/src/sensorthings/backends/sensorthings_v1_1/engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     2969 2024-01-16 20:26:49.000000 hydroserver-sensorthings-0.2.8/src/sensorthings/backends/sensorthings_v1_1/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-01-16 20:26:49.000000 hydroserver-sensorthings-0.2.8/src/sensorthings/backends/sensorthings_v1_1/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 20:27:03.584709 hydroserver-sensorthings-0.2.8/src/sensorthings/components/
--rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-01-16 20:26:49.000000 hydroserver-sensorthings-0.2.8/src/sensorthings/components/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 20:27:03.584709 hydroserver-sensorthings-0.2.8/src/sensorthings/components/datastreams/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-16 20:26:49.000000 hydroserver-sensorthings-0.2.8/src/sensorthings/components/datastreams/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-01-16 20:26:49.000000 hydroserver-sensorthings-0.2.8/src/sensorthings/components/datastreams/engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     3616 2024-01-16 20:26:49.000000 hydroserver-sensorthings-0.2.8/src/sensorthings/components/datastreams/schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)     4040 2024-01-16 20:26:49.000000 hydroserver-sensorthings-0.2.8/src/sensorthings/components/datastreams/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 20:27:03.584709 hydroserver-sensorthings-0.2.8/src/sensorthings/components/featuresofinterest/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-16 20:26:49.000000 hydroserver-sensorthings-0.2.8/src/sensorthings/components/featuresofinterest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      930 2024-01-16 20:26:49.000000 hydroserver-sensorthings-0.2.8/src/sensorthings/components/featuresofinterest/engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-01-16 20:26:49.000000 hydroserver-sensorthings-0.2.8/src/sensorthings/components/featuresofinterest/schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)     4379 2024-01-16 20:26:49.000000 hydroserver-sensorthings-0.2.8/src/sensorthings/components/featuresofinterest/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 20:27:03.584709 hydroserver-sensorthings-0.2.8/src/sensorthings/components/historicallocations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-16 20:26:49.000000 hydroserver-sensorthings-0.2.8/src/sensorthings/components/historicallocations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      969 2024-01-16 20:26:49.000000 hydroserver-sensorthings-0.2.8/src/sensorthings/components/historicallocations/engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     1868 2024-01-16 20:26:49.000000 hydroserver-sensorthings-0.2.8/src/sensorthings/components/historicallocations/schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)     4426 2024-01-16 20:26:49.000000 hydroserver-sensorthings-0.2.8/src/sensorthings/components/historicallocations/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 20:27:03.584709 hydroserver-sensorthings-0.2.8/src/sensorthings/components/locations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-16 20:26:49.000000 hydroserver-sensorthings-0.2.8/src/sensorthings/components/locations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-01-16 20:26:49.000000 hydroserver-sensorthings-0.2.8/src/sensorthings/components/locations/engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-01-16 20:26:49.000000 hydroserver-sensorthings-0.2.8/src/sensorthings/components/locations/schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)     3809 2024-01-16 20:26:49.000000 hydroserver-sensorthings-0.2.8/src/sensorthings/components/locations/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 20:27:03.588709 hydroserver-sensorthings-0.2.8/src/sensorthings/components/observations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-16 20:26:49.000000 hydroserver-sensorthings-0.2.8/src/sensorthings/components/observations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-01-16 20:26:49.000000 hydroserver-sensorthings-0.2.8/src/sensorthings/components/observations/engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     4093 2024-01-16 20:26:49.000000 hydroserver-sensorthings-0.2.8/src/sensorthings/components/observations/schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)     7875 2024-01-16 20:26:49.000000 hydroserver-sensorthings-0.2.8/src/sensorthings/components/observations/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5315 2024-01-16 20:26:49.000000 hydroserver-sensorthings-0.2.8/src/sensorthings/components/observations/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 20:27:03.588709 hydroserver-sensorthings-0.2.8/src/sensorthings/components/observedproperties/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-16 20:26:49.000000 hydroserver-sensorthings-0.2.8/src/sensorthings/components/observedproperties/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-01-16 20:26:49.000000 hydroserver-sensorthings-0.2.8/src/sensorthings/components/observedproperties/engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-01-16 20:26:49.000000 hydroserver-sensorthings-0.2.8/src/sensorthings/components/observedproperties/schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)     4300 2024-01-16 20:26:49.000000 hydroserver-sensorthings-0.2.8/src/sensorthings/components/observedproperties/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 20:27:03.588709 hydroserver-sensorthings-0.2.8/src/sensorthings/components/root/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-16 20:26:49.000000 hydroserver-sensorthings-0.2.8/src/sensorthings/components/root/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-01-16 20:26:49.000000 hydroserver-sensorthings-0.2.8/src/sensorthings/components/root/schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-01-16 20:26:49.000000 hydroserver-sensorthings-0.2.8/src/sensorthings/components/root/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 20:27:03.588709 hydroserver-sensorthings-0.2.8/src/sensorthings/components/sensors/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-16 20:26:49.000000 hydroserver-sensorthings-0.2.8/src/sensorthings/components/sensors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-01-16 20:26:49.000000 hydroserver-sensorthings-0.2.8/src/sensorthings/components/sensors/engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-01-16 20:26:49.000000 hydroserver-sensorthings-0.2.8/src/sensorthings/components/sensors/schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-01-16 20:26:49.000000 hydroserver-sensorthings-0.2.8/src/sensorthings/components/sensors/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3698 2024-01-16 20:26:49.000000 hydroserver-sensorthings-0.2.8/src/sensorthings/components/sensors/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 20:27:03.588709 hydroserver-sensorthings-0.2.8/src/sensorthings/components/things/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-16 20:26:49.000000 hydroserver-sensorthings-0.2.8/src/sensorthings/components/things/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-01-16 20:26:49.000000 hydroserver-sensorthings-0.2.8/src/sensorthings/components/things/engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-01-16 20:26:49.000000 hydroserver-sensorthings-0.2.8/src/sensorthings/components/things/schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)     3668 2024-01-16 20:26:49.000000 hydroserver-sensorthings-0.2.8/src/sensorthings/components/things/views.py
--rw-r--r--   0 runner    (1001) docker     (127)    27967 2024-01-16 20:26:49.000000 hydroserver-sensorthings-0.2.8/src/sensorthings/engine.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 20:27:03.588709 hydroserver-sensorthings-0.2.8/src/sensorthings/extras/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-16 20:26:49.000000 hydroserver-sensorthings-0.2.8/src/sensorthings/extras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-01-16 20:26:49.000000 hydroserver-sensorthings-0.2.8/src/sensorthings/extras/iso_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     9683 2024-01-16 20:26:49.000000 hydroserver-sensorthings-0.2.8/src/sensorthings/main.py
--rw-r--r--   0 runner    (1001) docker     (127)    10683 2024-01-16 20:26:49.000000 hydroserver-sensorthings-0.2.8/src/sensorthings/middleware.py
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-01-16 20:26:49.000000 hydroserver-sensorthings-0.2.8/src/sensorthings/renderer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-01-16 20:26:49.000000 hydroserver-sensorthings-0.2.8/src/sensorthings/router.py
--rw-r--r--   0 runner    (1001) docker     (127)     2569 2024-01-16 20:26:49.000000 hydroserver-sensorthings-0.2.8/src/sensorthings/schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)     2365 2024-01-16 20:26:49.000000 hydroserver-sensorthings-0.2.8/src/sensorthings/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     8500 2024-01-16 20:26:49.000000 hydroserver-sensorthings-0.2.8/src/sensorthings/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-01-16 20:26:49.000000 hydroserver-sensorthings-0.2.8/src/sensorthings/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 20:27:03.592709 hydroserver-sensorthings-0.2.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      850 2024-01-16 20:26:49.000000 hydroserver-sensorthings-0.2.8/tests/test_allow_partial_decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-01-16 20:26:49.000000 hydroserver-sensorthings-0.2.8/tests/test_iso_interval_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-01-16 20:26:49.000000 hydroserver-sensorthings-0.2.8/tests/test_iso_time_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-01-16 20:26:49.000000 hydroserver-sensorthings-0.2.8/tests/test_metadata_field_validator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3521 2024-01-16 20:26:49.000000 hydroserver-sensorthings-0.2.8/tests/test_resolve_chained_entity_url.py
--rw-r--r--   0 runner    (1001) docker     (127)     4972 2024-01-16 20:26:49.000000 hydroserver-sensorthings-0.2.8/tests/test_sensorthings_abstract_engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-01-16 20:26:49.000000 hydroserver-sensorthings-0.2.8/tests/test_whitespace_validator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 21:32:52.326970 hydroserver-sensorthings-0.2.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-01-24 21:32:39.000000 hydroserver-sensorthings-0.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-01-24 21:32:52.326970 hydroserver-sensorthings-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-01-24 21:32:39.000000 hydroserver-sensorthings-0.2.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-01-24 21:32:39.000000 hydroserver-sensorthings-0.2.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-01-24 21:32:52.326970 hydroserver-sensorthings-0.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-01-24 21:32:39.000000 hydroserver-sensorthings-0.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 21:32:52.310970 hydroserver-sensorthings-0.2.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 21:32:52.326970 hydroserver-sensorthings-0.2.9/src/hydroserver_sensorthings.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-01-24 21:32:52.000000 hydroserver-sensorthings-0.2.9/src/hydroserver_sensorthings.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3690 2024-01-24 21:32:52.000000 hydroserver-sensorthings-0.2.9/src/hydroserver_sensorthings.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-24 21:32:52.000000 hydroserver-sensorthings-0.2.9/src/hydroserver_sensorthings.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-01-24 21:32:52.000000 hydroserver-sensorthings-0.2.9/src/hydroserver_sensorthings.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-01-24 21:32:52.000000 hydroserver-sensorthings-0.2.9/src/hydroserver_sensorthings.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-24 21:32:52.000000 hydroserver-sensorthings-0.2.9/src/hydroserver_sensorthings.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 21:32:52.318970 hydroserver-sensorthings-0.2.9/src/sensorthings/
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-01-24 21:32:39.000000 hydroserver-sensorthings-0.2.9/src/sensorthings/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 21:32:52.318970 hydroserver-sensorthings-0.2.9/src/sensorthings/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-24 21:32:39.000000 hydroserver-sensorthings-0.2.9/src/sensorthings/backends/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 21:32:52.318970 hydroserver-sensorthings-0.2.9/src/sensorthings/backends/frostserver/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-24 21:32:39.000000 hydroserver-sensorthings-0.2.9/src/sensorthings/backends/frostserver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-01-24 21:32:39.000000 hydroserver-sensorthings-0.2.9/src/sensorthings/backends/frostserver/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-01-24 21:32:39.000000 hydroserver-sensorthings-0.2.9/src/sensorthings/backends/frostserver/engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-01-24 21:32:39.000000 hydroserver-sensorthings-0.2.9/src/sensorthings/backends/frostserver/renderers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-01-24 21:32:39.000000 hydroserver-sensorthings-0.2.9/src/sensorthings/backends/frostserver/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 21:32:52.318970 hydroserver-sensorthings-0.2.9/src/sensorthings/backends/odm2/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-24 21:32:39.000000 hydroserver-sensorthings-0.2.9/src/sensorthings/backends/odm2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-01-24 21:32:39.000000 hydroserver-sensorthings-0.2.9/src/sensorthings/backends/odm2/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-01-24 21:32:39.000000 hydroserver-sensorthings-0.2.9/src/sensorthings/backends/odm2/engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-24 21:32:39.000000 hydroserver-sensorthings-0.2.9/src/sensorthings/backends/odm2/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-24 21:32:39.000000 hydroserver-sensorthings-0.2.9/src/sensorthings/backends/odm2/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-01-24 21:32:39.000000 hydroserver-sensorthings-0.2.9/src/sensorthings/backends/odm2/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 21:32:52.318970 hydroserver-sensorthings-0.2.9/src/sensorthings/backends/sensorthings_v1_1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-24 21:32:39.000000 hydroserver-sensorthings-0.2.9/src/sensorthings/backends/sensorthings_v1_1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-01-24 21:32:39.000000 hydroserver-sensorthings-0.2.9/src/sensorthings/backends/sensorthings_v1_1/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8180 2024-01-24 21:32:39.000000 hydroserver-sensorthings-0.2.9/src/sensorthings/backends/sensorthings_v1_1/engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2969 2024-01-24 21:32:39.000000 hydroserver-sensorthings-0.2.9/src/sensorthings/backends/sensorthings_v1_1/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-01-24 21:32:39.000000 hydroserver-sensorthings-0.2.9/src/sensorthings/backends/sensorthings_v1_1/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 21:32:52.318970 hydroserver-sensorthings-0.2.9/src/sensorthings/components/
+-rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-01-24 21:32:39.000000 hydroserver-sensorthings-0.2.9/src/sensorthings/components/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 21:32:52.318970 hydroserver-sensorthings-0.2.9/src/sensorthings/components/datastreams/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-24 21:32:39.000000 hydroserver-sensorthings-0.2.9/src/sensorthings/components/datastreams/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-01-24 21:32:39.000000 hydroserver-sensorthings-0.2.9/src/sensorthings/components/datastreams/engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3616 2024-01-24 21:32:39.000000 hydroserver-sensorthings-0.2.9/src/sensorthings/components/datastreams/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4040 2024-01-24 21:32:39.000000 hydroserver-sensorthings-0.2.9/src/sensorthings/components/datastreams/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 21:32:52.322970 hydroserver-sensorthings-0.2.9/src/sensorthings/components/featuresofinterest/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-24 21:32:39.000000 hydroserver-sensorthings-0.2.9/src/sensorthings/components/featuresofinterest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-01-24 21:32:39.000000 hydroserver-sensorthings-0.2.9/src/sensorthings/components/featuresofinterest/engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-01-24 21:32:39.000000 hydroserver-sensorthings-0.2.9/src/sensorthings/components/featuresofinterest/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4379 2024-01-24 21:32:39.000000 hydroserver-sensorthings-0.2.9/src/sensorthings/components/featuresofinterest/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 21:32:52.322970 hydroserver-sensorthings-0.2.9/src/sensorthings/components/historicallocations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-24 21:32:39.000000 hydroserver-sensorthings-0.2.9/src/sensorthings/components/historicallocations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      969 2024-01-24 21:32:39.000000 hydroserver-sensorthings-0.2.9/src/sensorthings/components/historicallocations/engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1868 2024-01-24 21:32:39.000000 hydroserver-sensorthings-0.2.9/src/sensorthings/components/historicallocations/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4426 2024-01-24 21:32:39.000000 hydroserver-sensorthings-0.2.9/src/sensorthings/components/historicallocations/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 21:32:52.322970 hydroserver-sensorthings-0.2.9/src/sensorthings/components/locations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-24 21:32:39.000000 hydroserver-sensorthings-0.2.9/src/sensorthings/components/locations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-01-24 21:32:39.000000 hydroserver-sensorthings-0.2.9/src/sensorthings/components/locations/engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-01-24 21:32:39.000000 hydroserver-sensorthings-0.2.9/src/sensorthings/components/locations/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3809 2024-01-24 21:32:39.000000 hydroserver-sensorthings-0.2.9/src/sensorthings/components/locations/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 21:32:52.322970 hydroserver-sensorthings-0.2.9/src/sensorthings/components/observations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-24 21:32:39.000000 hydroserver-sensorthings-0.2.9/src/sensorthings/components/observations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-01-24 21:32:39.000000 hydroserver-sensorthings-0.2.9/src/sensorthings/components/observations/engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4093 2024-01-24 21:32:39.000000 hydroserver-sensorthings-0.2.9/src/sensorthings/components/observations/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7875 2024-01-24 21:32:39.000000 hydroserver-sensorthings-0.2.9/src/sensorthings/components/observations/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5315 2024-01-24 21:32:39.000000 hydroserver-sensorthings-0.2.9/src/sensorthings/components/observations/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 21:32:52.322970 hydroserver-sensorthings-0.2.9/src/sensorthings/components/observedproperties/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-24 21:32:39.000000 hydroserver-sensorthings-0.2.9/src/sensorthings/components/observedproperties/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-01-24 21:32:39.000000 hydroserver-sensorthings-0.2.9/src/sensorthings/components/observedproperties/engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-01-24 21:32:39.000000 hydroserver-sensorthings-0.2.9/src/sensorthings/components/observedproperties/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4300 2024-01-24 21:32:39.000000 hydroserver-sensorthings-0.2.9/src/sensorthings/components/observedproperties/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 21:32:52.322970 hydroserver-sensorthings-0.2.9/src/sensorthings/components/root/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-24 21:32:39.000000 hydroserver-sensorthings-0.2.9/src/sensorthings/components/root/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-01-24 21:32:39.000000 hydroserver-sensorthings-0.2.9/src/sensorthings/components/root/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-01-24 21:32:39.000000 hydroserver-sensorthings-0.2.9/src/sensorthings/components/root/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 21:32:52.326970 hydroserver-sensorthings-0.2.9/src/sensorthings/components/sensors/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-24 21:32:39.000000 hydroserver-sensorthings-0.2.9/src/sensorthings/components/sensors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-01-24 21:32:39.000000 hydroserver-sensorthings-0.2.9/src/sensorthings/components/sensors/engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-01-24 21:32:39.000000 hydroserver-sensorthings-0.2.9/src/sensorthings/components/sensors/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-01-24 21:32:39.000000 hydroserver-sensorthings-0.2.9/src/sensorthings/components/sensors/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3698 2024-01-24 21:32:39.000000 hydroserver-sensorthings-0.2.9/src/sensorthings/components/sensors/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 21:32:52.326970 hydroserver-sensorthings-0.2.9/src/sensorthings/components/things/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-24 21:32:39.000000 hydroserver-sensorthings-0.2.9/src/sensorthings/components/things/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-01-24 21:32:39.000000 hydroserver-sensorthings-0.2.9/src/sensorthings/components/things/engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-01-24 21:32:39.000000 hydroserver-sensorthings-0.2.9/src/sensorthings/components/things/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3668 2024-01-24 21:32:39.000000 hydroserver-sensorthings-0.2.9/src/sensorthings/components/things/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27967 2024-01-24 21:32:39.000000 hydroserver-sensorthings-0.2.9/src/sensorthings/engine.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 21:32:52.326970 hydroserver-sensorthings-0.2.9/src/sensorthings/extras/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-24 21:32:39.000000 hydroserver-sensorthings-0.2.9/src/sensorthings/extras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-01-24 21:32:39.000000 hydroserver-sensorthings-0.2.9/src/sensorthings/extras/iso_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9683 2024-01-24 21:32:39.000000 hydroserver-sensorthings-0.2.9/src/sensorthings/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10683 2024-01-24 21:32:39.000000 hydroserver-sensorthings-0.2.9/src/sensorthings/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-01-24 21:32:39.000000 hydroserver-sensorthings-0.2.9/src/sensorthings/renderer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-01-24 21:32:39.000000 hydroserver-sensorthings-0.2.9/src/sensorthings/router.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2569 2024-01-24 21:32:39.000000 hydroserver-sensorthings-0.2.9/src/sensorthings/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2365 2024-01-24 21:32:39.000000 hydroserver-sensorthings-0.2.9/src/sensorthings/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8500 2024-01-24 21:32:39.000000 hydroserver-sensorthings-0.2.9/src/sensorthings/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-01-24 21:32:39.000000 hydroserver-sensorthings-0.2.9/src/sensorthings/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 21:32:52.326970 hydroserver-sensorthings-0.2.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-01-24 21:32:39.000000 hydroserver-sensorthings-0.2.9/tests/test_allow_partial_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-01-24 21:32:39.000000 hydroserver-sensorthings-0.2.9/tests/test_iso_interval_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-01-24 21:32:39.000000 hydroserver-sensorthings-0.2.9/tests/test_iso_time_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-01-24 21:32:39.000000 hydroserver-sensorthings-0.2.9/tests/test_metadata_field_validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3521 2024-01-24 21:32:39.000000 hydroserver-sensorthings-0.2.9/tests/test_resolve_chained_entity_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4972 2024-01-24 21:32:39.000000 hydroserver-sensorthings-0.2.9/tests/test_sensorthings_abstract_engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-01-24 21:32:39.000000 hydroserver-sensorthings-0.2.9/tests/test_whitespace_validator.py
```

### Comparing `hydroserver-sensorthings-0.2.8/LICENSE` & `hydroserver-sensorthings-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `hydroserver-sensorthings-0.2.8/README.md` & `hydroserver-sensorthings-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `hydroserver-sensorthings-0.2.8/src/hydroserver_sensorthings.egg-info/SOURCES.txt` & `hydroserver-sensorthings-0.2.9/src/hydroserver_sensorthings.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hydroserver-sensorthings-0.2.8/src/sensorthings/backends/frostserver/engine.py` & `hydroserver-sensorthings-0.2.9/src/sensorthings/backends/frostserver/engine.py`

 * *Files identical despite different names*

### Comparing `hydroserver-sensorthings-0.2.8/src/sensorthings/backends/odm2/engine.py` & `hydroserver-sensorthings-0.2.9/src/sensorthings/backends/odm2/engine.py`

 * *Files identical despite different names*

### Comparing `hydroserver-sensorthings-0.2.8/src/sensorthings/backends/sensorthings_v1_1/engine.py` & `hydroserver-sensorthings-0.2.9/src/sensorthings/backends/sensorthings_v1_1/engine.py`

 * *Files identical despite different names*

### Comparing `hydroserver-sensorthings-0.2.8/src/sensorthings/backends/sensorthings_v1_1/models.py` & `hydroserver-sensorthings-0.2.9/src/sensorthings/backends/sensorthings_v1_1/models.py`

 * *Files identical despite different names*

### Comparing `hydroserver-sensorthings-0.2.8/src/sensorthings/components/__init__.py` & `hydroserver-sensorthings-0.2.9/src/sensorthings/components/__init__.py`

 * *Files identical despite different names*

### Comparing `hydroserver-sensorthings-0.2.8/src/sensorthings/components/datastreams/engine.py` & `hydroserver-sensorthings-0.2.9/src/sensorthings/components/datastreams/engine.py`

 * *Files identical despite different names*

### Comparing `hydroserver-sensorthings-0.2.8/src/sensorthings/components/datastreams/schemas.py` & `hydroserver-sensorthings-0.2.9/src/sensorthings/components/datastreams/schemas.py`

 * *Files identical despite different names*

### Comparing `hydroserver-sensorthings-0.2.8/src/sensorthings/components/datastreams/views.py` & `hydroserver-sensorthings-0.2.9/src/sensorthings/components/datastreams/views.py`

 * *Files identical despite different names*

### Comparing `hydroserver-sensorthings-0.2.8/src/sensorthings/components/featuresofinterest/engine.py` & `hydroserver-sensorthings-0.2.9/src/sensorthings/components/featuresofinterest/engine.py`

 * *Files identical despite different names*

### Comparing `hydroserver-sensorthings-0.2.8/src/sensorthings/components/featuresofinterest/schemas.py` & `hydroserver-sensorthings-0.2.9/src/sensorthings/components/featuresofinterest/schemas.py`

 * *Files identical despite different names*

### Comparing `hydroserver-sensorthings-0.2.8/src/sensorthings/components/featuresofinterest/views.py` & `hydroserver-sensorthings-0.2.9/src/sensorthings/components/featuresofinterest/views.py`

 * *Files identical despite different names*

### Comparing `hydroserver-sensorthings-0.2.8/src/sensorthings/components/historicallocations/engine.py` & `hydroserver-sensorthings-0.2.9/src/sensorthings/components/historicallocations/engine.py`

 * *Files identical despite different names*

### Comparing `hydroserver-sensorthings-0.2.8/src/sensorthings/components/historicallocations/schemas.py` & `hydroserver-sensorthings-0.2.9/src/sensorthings/components/historicallocations/schemas.py`

 * *Files identical despite different names*

### Comparing `hydroserver-sensorthings-0.2.8/src/sensorthings/components/historicallocations/views.py` & `hydroserver-sensorthings-0.2.9/src/sensorthings/components/historicallocations/views.py`

 * *Files identical despite different names*

### Comparing `hydroserver-sensorthings-0.2.8/src/sensorthings/components/locations/engine.py` & `hydroserver-sensorthings-0.2.9/src/sensorthings/components/locations/engine.py`

 * *Files identical despite different names*

### Comparing `hydroserver-sensorthings-0.2.8/src/sensorthings/components/locations/schemas.py` & `hydroserver-sensorthings-0.2.9/src/sensorthings/components/locations/schemas.py`

 * *Files identical despite different names*

### Comparing `hydroserver-sensorthings-0.2.8/src/sensorthings/components/locations/views.py` & `hydroserver-sensorthings-0.2.9/src/sensorthings/components/locations/views.py`

 * *Files identical despite different names*

### Comparing `hydroserver-sensorthings-0.2.8/src/sensorthings/components/observations/engine.py` & `hydroserver-sensorthings-0.2.9/src/sensorthings/components/observations/engine.py`

 * *Files identical despite different names*

### Comparing `hydroserver-sensorthings-0.2.8/src/sensorthings/components/observations/schemas.py` & `hydroserver-sensorthings-0.2.9/src/sensorthings/components/observations/schemas.py`

 * *Files identical despite different names*

### Comparing `hydroserver-sensorthings-0.2.8/src/sensorthings/components/observations/utils.py` & `hydroserver-sensorthings-0.2.9/src/sensorthings/components/observations/utils.py`

 * *Files identical despite different names*

### Comparing `hydroserver-sensorthings-0.2.8/src/sensorthings/components/observations/views.py` & `hydroserver-sensorthings-0.2.9/src/sensorthings/components/observations/views.py`

 * *Files identical despite different names*

### Comparing `hydroserver-sensorthings-0.2.8/src/sensorthings/components/observedproperties/engine.py` & `hydroserver-sensorthings-0.2.9/src/sensorthings/components/observedproperties/engine.py`

 * *Files identical despite different names*

### Comparing `hydroserver-sensorthings-0.2.8/src/sensorthings/components/observedproperties/schemas.py` & `hydroserver-sensorthings-0.2.9/src/sensorthings/components/observedproperties/schemas.py`

 * *Files identical despite different names*

### Comparing `hydroserver-sensorthings-0.2.8/src/sensorthings/components/observedproperties/views.py` & `hydroserver-sensorthings-0.2.9/src/sensorthings/components/observedproperties/views.py`

 * *Files identical despite different names*

### Comparing `hydroserver-sensorthings-0.2.8/src/sensorthings/components/root/views.py` & `hydroserver-sensorthings-0.2.9/src/sensorthings/components/root/views.py`

 * *Files identical despite different names*

### Comparing `hydroserver-sensorthings-0.2.8/src/sensorthings/components/sensors/engine.py` & `hydroserver-sensorthings-0.2.9/src/sensorthings/components/sensors/engine.py`

 * *Files identical despite different names*

### Comparing `hydroserver-sensorthings-0.2.8/src/sensorthings/components/sensors/schemas.py` & `hydroserver-sensorthings-0.2.9/src/sensorthings/components/sensors/schemas.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import TYPE_CHECKING, Literal, List
+from typing import TYPE_CHECKING, Literal, List, Optional
 from pydantic import Field, AnyHttpUrl, validator
 from ninja import Schema
 from sensorthings.schemas import BaseListResponse, BaseGetResponse, BasePostBody, BasePatchBody, NestedEntity
 from sensorthings.validators import allow_partial
 from sensorthings.components.sensors.utils import metadata_validator
 
 if TYPE_CHECKING:
@@ -17,15 +17,15 @@
 
 
 class SensorFields(Schema):
     name: str
     description: str
     encoding_type: sensorEncodingTypes = Field(..., alias='encodingType')
     sensor_metadata: str = Field(..., alias='metadata')
-    properties: dict = {}
+    properties: Optional[dict] = None
 
     _metadata_validator = validator('sensor_metadata', allow_reuse=True, check_fields=False)(metadata_validator)
 
 
 class SensorRelations(Schema):
     datastreams: List['Datastream'] = []
```

### Comparing `hydroserver-sensorthings-0.2.8/src/sensorthings/components/sensors/utils.py` & `hydroserver-sensorthings-0.2.9/src/sensorthings/components/sensors/utils.py`

 * *Files identical despite different names*

### Comparing `hydroserver-sensorthings-0.2.8/src/sensorthings/components/sensors/views.py` & `hydroserver-sensorthings-0.2.9/src/sensorthings/components/sensors/views.py`

 * *Files identical despite different names*

### Comparing `hydroserver-sensorthings-0.2.8/src/sensorthings/components/things/engine.py` & `hydroserver-sensorthings-0.2.9/src/sensorthings/components/things/engine.py`

 * *Files identical despite different names*

### Comparing `hydroserver-sensorthings-0.2.8/src/sensorthings/components/things/schemas.py` & `hydroserver-sensorthings-0.2.9/src/sensorthings/components/things/schemas.py`

 * *Files identical despite different names*

### Comparing `hydroserver-sensorthings-0.2.8/src/sensorthings/components/things/views.py` & `hydroserver-sensorthings-0.2.9/src/sensorthings/components/things/views.py`

 * *Files identical despite different names*

### Comparing `hydroserver-sensorthings-0.2.8/src/sensorthings/engine.py` & `hydroserver-sensorthings-0.2.9/src/sensorthings/engine.py`

 * *Files identical despite different names*

### Comparing `hydroserver-sensorthings-0.2.8/src/sensorthings/extras/iso_types.py` & `hydroserver-sensorthings-0.2.9/src/sensorthings/extras/iso_types.py`

 * *Files identical despite different names*

### Comparing `hydroserver-sensorthings-0.2.8/src/sensorthings/main.py` & `hydroserver-sensorthings-0.2.9/src/sensorthings/main.py`

 * *Files identical despite different names*

### Comparing `hydroserver-sensorthings-0.2.8/src/sensorthings/middleware.py` & `hydroserver-sensorthings-0.2.9/src/sensorthings/middleware.py`

 * *Files identical despite different names*

### Comparing `hydroserver-sensorthings-0.2.8/src/sensorthings/router.py` & `hydroserver-sensorthings-0.2.9/src/sensorthings/router.py`

 * *Files identical despite different names*

### Comparing `hydroserver-sensorthings-0.2.8/src/sensorthings/schemas.py` & `hydroserver-sensorthings-0.2.9/src/sensorthings/schemas.py`

 * *Files identical despite different names*

### Comparing `hydroserver-sensorthings-0.2.8/src/sensorthings/settings.py` & `hydroserver-sensorthings-0.2.9/src/sensorthings/settings.py`

 * *Files identical despite different names*

### Comparing `hydroserver-sensorthings-0.2.8/src/sensorthings/utils.py` & `hydroserver-sensorthings-0.2.9/src/sensorthings/utils.py`

 * *Files identical despite different names*

### Comparing `hydroserver-sensorthings-0.2.8/src/sensorthings/validators.py` & `hydroserver-sensorthings-0.2.9/src/sensorthings/validators.py`

 * *Files identical despite different names*

### Comparing `hydroserver-sensorthings-0.2.8/tests/test_allow_partial_decorator.py` & `hydroserver-sensorthings-0.2.9/tests/test_allow_partial_decorator.py`

 * *Files identical despite different names*

### Comparing `hydroserver-sensorthings-0.2.8/tests/test_iso_interval_type.py` & `hydroserver-sensorthings-0.2.9/tests/test_iso_interval_type.py`

 * *Files identical despite different names*

### Comparing `hydroserver-sensorthings-0.2.8/tests/test_iso_time_type.py` & `hydroserver-sensorthings-0.2.9/tests/test_iso_time_type.py`

 * *Files identical despite different names*

### Comparing `hydroserver-sensorthings-0.2.8/tests/test_metadata_field_validator.py` & `hydroserver-sensorthings-0.2.9/tests/test_metadata_field_validator.py`

 * *Files identical despite different names*

### Comparing `hydroserver-sensorthings-0.2.8/tests/test_resolve_chained_entity_url.py` & `hydroserver-sensorthings-0.2.9/tests/test_resolve_chained_entity_url.py`

 * *Files identical despite different names*

### Comparing `hydroserver-sensorthings-0.2.8/tests/test_sensorthings_abstract_engine.py` & `hydroserver-sensorthings-0.2.9/tests/test_sensorthings_abstract_engine.py`

 * *Files identical despite different names*

### Comparing `hydroserver-sensorthings-0.2.8/tests/test_whitespace_validator.py` & `hydroserver-sensorthings-0.2.9/tests/test_whitespace_validator.py`

 * *Files identical despite different names*

